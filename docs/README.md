# Havenfall Documentation Index

This folder contains the Game Design Document (GDD), balance tables, data schemas, UX flows, and planning backlog for the vertical slice.

## Reading order
1. `GDD.md` — High-level design, systems overview, production plan.
2. `ux/flows.md` — UX flows for FTUE, base loop, missions, sieges.
3. `tables/` — Concrete balance data in CSVs (buildings, levels, enemies, survivors, tech, items, missions, factions, events).
4. `schemas/` — JSON schemas and sample params for integration.
5. `backlog/vertical_slice_backlog.md` — 12-week delivery plan.

## Tables
- `tables/buildings.csv` — Building catalog and adjacency.
- `tables/building_levels.csv` — Level-by-level costs and outputs.
- `tables/enemies.csv` — Enemy stats, classes, and notes.
- `tables/survivors.csv` — Survivor roster with attributes and traits.
- `tables/tech.csv` — Tech tree, prerequisites, costs, and unlocks.
- `tables/items.csv` — Weapons/armor/tools/consumables and craft costs.
- `tables/missions.csv` — Mission templates by POI and risk.
- `tables/factions.csv` — Faction reputations and behaviors.
- `tables/events.csv` — Incidents, triggers, effects.

## Schemas
- `schemas/params.schema.json` — Balance/data contract for runtime.
- `schemas/params.sample.json` — Example values matching the schema.

## Notes
- All numbers are placeholder and ready for tuning via remote config.
- CSVs are structured for import into Google Sheets or Unity Addressables-driven data pipeline.
- Submit changes via PR with a short change-log in commit message.