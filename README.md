# Project Zomboid Reference

Static, self-contained reference tables for Project Zomboid (Build 42), parsed
directly from the game files. The exact game build each page was generated from
is shown in every page header.

## Pages

- **`index.html`** — landing page: a short description and links into each
  section.
- **`seeds.html`** — Seed & crop reference: growth time, water needs,
  sow/best/risk months, and yields. Filter by name, type, sow month, or
  cold-hardiness.
- **`cars.html`** — Vehicle stats (max speed, engine force/quality/loudness,
  mass, seats, trunk capacity, roof racks, repair level, crash protection) for
  the base game plus Workshop mods, with thumbnails and a full-size hover
  preview. Filter by type/source.
- **`livestock.html`** — Farm animals: products, maturation, gestation, trailer
  size, temperament, and breed gene tendencies.
- **`guns.html`** — Firearms, with per-gun attachment/upgrade lists (scopes,
  red dots, lasers, choke tubes, recoil pads, slings) and durability.
- **`melee.html`** — Melee weapons: damage, DPS, reach, swing speed, max hits
  per swing, crit, knockdown, durability, door/tree damage, and skill type.
- **`tools.html`** — Tools: what each does, durability (≈ uses before breaking),
  and weight. Includes weapons that double as tools (axes, hammers, saws — ⚔,
  also on the Melee tab).
- **`crafting.html`** — Crafting/building recipes for all 14 craftable skills.
  Set your level for each skill (saved in your browser) and it surfaces the
  no-waste **crafting cycles** you can run right now, plus the most XP-efficient
  recipes per skill. Each skill has its own sortable sub-page
  (`craft_<Skill>.html`) with full XP / materials / tools / time.
- **`food.html`** — Food & nutrition: hunger/thirst restored, calories, carbs,
  fat, protein, mood effect, and spoilage for every food item. Pick an evolved
  recipe (stew, soup, pizza…) to see what **one** of each ingredient adds.
- **`foraging.html`** — Natural forageables (berries, mushrooms, herbs, fruit,
  veg, medicinal plants…) with the area they're found in, season, peak months,
  Foraging level needed, amount, XP, and a poison flag.
- **`actions.html`** — Action XP: how much XP in-world actions grant and which
  skill they train (butchering, milking, fishing, foraging, vehicle work, first
  aid, trapping…). Filterable by skill and area. Literal amounts where the game
  files give a constant; "varies"/ranges/"engine-granted" where it's computed at
  runtime. (Crafting-recipe XP lives on the Crafting page; combat XP scales per
  hit.)

Every item links to its [PZ Wiki](https://pzwiki.net) page; modded vehicles link
to their Steam Workshop page instead.

Each page is a single HTML file with all data and styling embedded — no build
step, no external dependencies, works offline by opening the file directly.
Vehicle table images are small thumbnails (full render on hover) and a service
worker caches them so they download at most once.

## Image credits

Vehicle images are used here for non-commercial fan reference and remain the
property of their owners:

- **Vanilla vehicle renders** — © The Indie Stone; obtained from
  [PZwiki](https://pzwiki.net) (per-variant `<Script>_Model.png` renders,
  CC BY-SA per PZwiki's licensing).
- **Modded vehicle previews** — © their respective mod authors; obtained from
  each mod's Steam Workshop page (variants within a mod share that mod's
  preview).

## Notes

Vehicle trunk capacities are full-condition values; in-game capacity scales down
with trunk part condition. Values shown in grey / marked as interior slots are
best-estimate (item-tier dependent) rather than fixed.
