# Havenfall — Mobile GDD (Strategy + Survival + City Builder + Story)

Version: 0.1 (Draft)
Owner: Design Team
Last Updated: 2025-08-16

## High Concept
- Elevator pitch: Build and defend a living survivor settlement in a collapsing world. Lead squads on risky expeditions, rescue and develop unique survivors, and push the story forward through hard choices as evolving zombie swarms and hostile factions threaten your city.
- Genre blend: Strategy + Survival + City Builder + Narrative (mobile-first)
- Pillars:
  - Living survivors with traits, relationships, and mental states
  - Evolving threats: horde AI that responds to your noise, growth, and time of day
  - Tactical expeditions with base stakes and story consequences
  - Fair F2P: cosmetics and QoL, not power

## Target & Positioning
- Audience: Midcore builders/strategy players; fans of State of Survival, Fallout Shelter, XCOM-like tactics; narrative-driven gamers.
- Platform: iOS and Android.
- Session model: 3–7 short sessions/day (3–10 min) + 1 longer (15–25 min) for story/raids.
- Camera & art style: Isometric stylized-realistic; readable silhouettes; strong day/night contrast and weather.

## Core Loops
- Moment-to-moment (2–5 min): Collect outputs → assign survivors to jobs → craft/repair → send squad on a mission → pick a narrative choice → reinforce defenses.
- Mid-term (daily/weekly): Upgrade HQ and production → unlock tech → defend horde nights → manage survivor morale/relationships → faction diplomacy.
- Long-term (seasonal): Expand territory → unlock new biomes and special infected → seasonal story arcs and alliance ops → base prestige resets with meta rewards.

## World & Narrative
- Theme: Post-apocalyptic, zombie outbreak with special infected and mutated biomes.
- Tone: Hope through hardship; ethical dilemmas and scarcity; community-building.
- Season 1 overview (8–10 chapters): Escape quarantine → establish base → meet Traders → first moral choice (save a trapped family vs. secure generator) → Screamer reveal → first horde night → faction entanglements → Chapter guardian showdown.
- Player identity: Settlement leader finding a balance between survival efficiency and human values.

## Systems Overview

### Base Building
- Grid placement: 1x1–4x4 footprints; roads optional; adjacency bonuses (e.g., Farm next to Water Tower +10% output).
- Construction: Build time + resources; builder queue; survivor labor speeds construction.
- Upgrades: Multi-step upgrades add new sockets/modules, not just % boosts.
- Defenses: Walls, gates, turrets, traps; pathing, choke points, ammo/power upkeep.
- Key buildings (see `/docs/tables/buildings.csv` for details): HQ, Housing, Farm, Water Still/Purifier, Workshop, Armory, Med Bay, Generator/Solar/Battery, Storage, Walls/Gates/Turrets/Traps, Detector/Watchtowers, Radio Tower, Greenhouse, Water Tower.

### Survivors
- Acquisition: Rescue missions, radio calls, trade, story recruits.
- Archetypes: Scavenger, Medic, Engineer, Defender, Leader, Scout, Cook, Farmer (multi-class via training).
- Attributes: Strength, Agility, Intellect, Resolve; Level 1–30 with perk picks at milestone levels.
- Traits: 2–4 persistent quirks (e.g., Night Owl, Hemophobic) that affect jobs and combat.
- States: Morale, Fatigue, Injury (light/moderate/critical), Infection (progression clock), Relationships (rival/bond).
- Roles & schedules: Job assignment affects output and growth; day/night shifts manage fatigue and night debuffs.
- Risk: Default no permadeath; Iron mode optional. Injuries persist and require Med Bay time.

### Resources & Economy
- Primary: Food, Water, Wood, Metal, Electronics, Meds, Ammo, Fuel, Power (virtual), Population, Morale.
- Secondary: Parts, Chemicals, Fabric, Rare Components.
- Flows: Survivors consume food/water daily; power produced/consumed per tick; upkeep for defenses (ammo/fuel/meds); storage caps and overflow decay.
- Noise: Generators, turrets, and loud missions generate noise → increases Horde Interest → spawns sieges; management via silencers, weather, batteries, scheduling.

### Research & Crafting
- Tech branches: Survival, Engineering, Defense, Society. Research requires resources + time; scientists accelerate.
- Crafting: Weapons, armor, tools, traps, consumables; blueprints drop from bosses/POIs.
- Augments: Sockets on buildings or gear; augment families align with tech branches.

### World & Exploration
- Overworld: Fog-of-war hex map; POIs tagged (Store, Clinic, Police Station, Factory, Quarantine Zone).
- Risk bands: Green/Yellow/Red/Black zones with escalating threats and loot.
- Mission types: Scavenge, Rescue, Recon, Clear, Escort, Trade, Story; timers, stealth options, noise risk.
- Travel: Squad speed; vehicles (van/truck) with fuel costs; ambush chance modified by Scout skill.
- Weather & time: Night increases zombie aggression but improves stealth; rain reduces noise radius but hits solar output.

### Combat
- Primary mode: Real-time-with-pause (RTwP) squad tactics (4–6 units), cover, cone of fire; radial commands and ability buttons on mobile. Auto-resolve for low-risk.
- Accessibility: Optional turn-based toggle.
- Systems: Noise spawns waves; elevation/choke points; limited ammo/stamina; abilities (taunt, suppress, grenade, stim).
- Siege mode: Base defense events with trap pre-placement; multi-lane with elite specials.

### Enemies
- Baselines: Walker (baseline, swarmable), Runner (fast, low HP), Brute (armored, gate breaker), Spitter (acid pools), Screamer (calls reinforcements), Burrower (bypass walls), Bosses (chapter guardians with mechanics).
- See `/docs/tables/enemies.csv` for parameters.

### Factions & Diplomacy
- AI factions: Traders, Raiders, Militias, Cultists. Reputation impacts prices, aid, or raids.
- Systems: Contracts, non-aggression, joint expeditions, betrayal events.
- Dynamic economy: Prices shift by scarcity and reputation; convoy escort missions.

### Events & Story
- Chapter structure: 8–10 chapters in Season 1; each ~2–3 hours.
- Dilemmas: 2–3 narrative choices/week with visible stat checks and hidden relationship checks.
- Random incidents: Disease outbreak, theft, power failure, night terror, trait conflicts.

## Progression
- HQ levels: 1–10; gates building caps and unlocks biomes at L4/7/10.
- Threat tiers: Global multipliers increase spawn rarity and boss mechanics.
- Survivor growth: XP from jobs and missions; cross-training unlocks hybrid perks.
- Onboarding (first 24h):
  - Day 0: Build shelter, farm, water; first rescue; scripted night mini-siege.
  - Day 1: Craft basic weapons; world recon; meet Traders; first faction choice.
  - Day 3: First horde night; tutorial on traps and choke points.

## Social & Live Ops
- Alliances: 30–50 players; donate resources, help speed-ups, shared tech node buffs.
- Alliance Ops: Map bosses, convoy escorts, horde fortifications (temporary community structures).
- Events: Weekend Horde Rush, Story reruns, Resource surges, Boss time trials.
- Seasons: 6–10 weeks with new biome, specials, cosmetics, story arc; soft reset with persistent meta unlocks.

## Monetization (Fair F2P)
- Cosmetics: Survivor outfits, weapon skins, base themes, emotes, banners.
- Convenience: Extra builder slot, queue slots, cosmetic drones; time accelerators via soft currency/ad rewards.
- Battle pass: Cosmetic track + QoL vouchers; no exclusive power.
- Offers: Resource bundles capped per day; pity-timers for rare blueprints.
- Ads: Optional reward ads (finishers, daily cache, revive token); frequency caps.

## UX & Accessibility
- Controls: Tap-to-move, drag-select, radial command wheel, long-press inspect; left-hand mode.
- Clarity: Color-blind palette, scalable fonts, outline modes at night.
- Assist: Auto-resolve, aim assist, “safe build” preview for pathing; condensed “what changed?” logs.
- See `/docs/ux/flows.md` for detailed flows and wireflows.

## Technical & Tools
- Engine: Unity 2022+ URP; DOTS for hordes; Addressables for streaming.
- Client: 60 FPS target on mid devices; adaptive horde budgets.
- Server: Authoritative economy; identity/inventory/cloud save/matchmaking; deterministic combat seeds for replays.
- Data: ScriptableObjects mirrored to JSON; remote config for balance and events.
- Anti-cheat: Server-verified timers/resources; checksums on mission outcomes.

## Analytics & Soft Launch
- KPIs: D1 40–50%, D7 10–15%, ARPDAU $0.08–$0.15, FTUE completion >70%.
- Instrumentation: Mission outcomes, survivor states, horde intensity, choke-point kills, churn predictors (injury/queue blocks).
- A/B tests: Auto-resolve availability, horde cadence, early economy generosity.
- Soft launch plan: 2–3 geos, 8–12 weeks; 3 content updates; prioritize stability and D7.

## Content Pipeline
- Editors: Node-based story tool, mission generator (POI templates, enemy packs), loot table editor, building config sheets.
- Localization: Key-based, RTL support, 12+ languages; VO stubs.
- Build & CI: Per-commit build, smoke tests, automated balance sanity checks.

## Production Plan
- Vertical slice (10–12 weeks): Base loop, small siege, 1 biome, 4–6 missions, 6 survivors, 4 enemy types, basic story.
- Alpha (12–16 weeks): Tech tree L1–5, faction intro, horde director v1, crafting, onboarding Day 3 complete.
- Beta/Soft launch (12 weeks): Season 1 Chapter 1–6, alliances v1, live-ops pipeline, monetization light.
- Global: Season 1 complete, new biome, alliance ops v2, content cadence.

## Risks & Mitigations
- Pathing/defense exploits: Precompute valid lanes; anti-cheese heuristics; event-driven path reroute.
- Overcomplex survivor management: Recommended assignments; role UI; auto-rotation schedules.
- Device performance: Adaptive spawn scaling; proxy crowds; pooling; LODs.
- Balance fatigue: Remote config live tuning; challenge bands; opt-in Iron mode.

## References
- Tables: See `/docs/tables/*.csv` for buildings, techs, items, enemies, survivors.
- Schemas: See `/docs/schemas/*.json` for data contracts.
- UX: See `/docs/ux/flows.md` for flows; `/docs/backlog/vertical_slice_backlog.md` for 12-week plan.

---

Appendix A: Sample Balance Params (see `/docs/schemas/params.sample.json`)
Appendix B: Example Mission Template (see `/docs/tables`)