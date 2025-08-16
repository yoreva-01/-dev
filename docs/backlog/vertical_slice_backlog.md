# Vertical Slice Backlog (12 Weeks)

Goal: Playable core loop with 1 biome, 4–6 missions, 6 survivors, 4 enemy types, small siege, basic story, ethical F2P.
Team assumption: ~10–14 people cross-discipline.

## Week 1 — Foundations
- Design: GDD v0.1; balance KPIs + economy stub; mission templates v0
- Engineering: Unity project setup (URP, Addressables, DOTS sample), repo, CI build
- Art: Style guide, proxy kitbash for buildings/units, lighting pass v0
- Data: ScriptableObject + JSON mirror pipeline; remote config stub
- Acceptance: Android/iOS dev build; empty map loads at 60 FPS on target device

## Week 2 — Base Loop v0
- Build placement grid, collision, rotation, refunds
- Buildings: `Housing L1`, `Farm L1`, `Water Still L1`, `Storage L1`
- Collection interaction and timers; storage caps
- Survivors panel list; assign to jobs; basic output modifiers
- Acceptance: Produce/collect food/water; survivors affect outputs

## Week 3 — Missions v0
- Overworld hex map with fog; POI markers; travel timer
- Squad assembly (4 units), auto-fill, gear check
- RTwP prototype: move, attack, ability slot; basic enemy AI (Walker, Runner)
- Mission outcome → rewards and injuries
- Acceptance: Complete a scavenge mission and return loot

## Week 4 — Tech & Craft v0
- Tech tree UI; Survival/Engineering tier 1
- Workshop craft: basic weapons and medkits; equip gear
- Med Bay: treat injuries; recovery timers
- Acceptance: Research a node; craft and equip an item; heal an injury

## Week 5 — Defenses v0
- Walls, Gate, Spike Trap, Ballistic Turret; ammo/power hooks
- Pathing lanes and choke points; safe-build preview
- Acceptance: Place defenses that alter pathing; turret consumes ammo

## Week 6 — Horde Night v0
- Horde director v0 (noise → interest → trigger)
- Siege event: 3 short waves; Screamer special infected
- Damage report and morale impacts
- Acceptance: Trigger and survive a mini-siege

## Week 7 — Story & FTUE v0
- FTUE guided flow; minimal narrative beats and choices
- Journal screen with chapter progress
- Acceptance: New account completes FTUE in <12 minutes; D0 retention test-ready

## Week 8 — Factions & Trade v0
- Trader faction intro; basic reputation; dynamic prices
- Trade mission and convoy escort template
- Acceptance: Complete one trade and see price shift with rep

## Week 9 — Survivors Depth v1
- Traits, morale, fatigue; day/night schedules
- Relationships (rival/bond) hooks into checks
- Acceptance: Traits visibly affect jobs/combat; morale impacts output

## Week 10 — Performance & Polish
- Pooling, LODs, horde budget tiers; device matrix tests
- Art polish pass on 6 buildings, 2 turrets, 4 zombies, 6 survivors
- Acceptance: 60 FPS target on mid devices during small siege

## Week 11 — Monetization & Live Ops v0
- Cosmetic inventory; store (cosmetics/QoL only); reward ads (capped)
- Battle pass scaffolding (cosmetic track); live config hooks
- Acceptance: Purchase cosmetic, equip on survivor/base; ads capped per day

## Week 12 — Stabilization & Playtest
- Balance pass; analytics events; bug crush
- External playtest (N=50–100); survey and telemetry review
- Go/No-go for Alpha scope
- Acceptance: 95% crash-free sessions; FTUE completion >70%

Risks tracked: pathing exploits, device perf, economy stalls; weekly reviews and mitigations.