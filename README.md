# Iron Steel

**Iron Order 1919–inspired fan strategy game**

Single-player province strategy inspired by *Iron Order 1919*, *Call of War*, and the Supremacy engine (*Conflict of Nations*, *Supremacy 1914*).

Fan project — not affiliated with Bytro Labs, Dorado Games, Twin Harbour Interactive, or Stillfront Group.

---

## Official public release: v0.19

**v0.19 is the first official public playable release.**

Earlier tags (v0.1–v0.18) were **prereleases** used while the prototype was iterated. v0.19 is the milestone build intended for public playtesting.

[Download iron-steel-v0.19.html](https://github.com/AmazighOasisAzul/iron-steel/releases) from the [releases page](https://github.com/AmazighOasisAzul/iron-steel/releases) (attach the v0.19 asset to a `v0.19` release if it is not listed yet).

Open the HTML file in a modern desktop browser. It runs offline, needs no install, and does not contact a game server.

### What is new in v0.19

- **Main menu** — game does not start until **Start Match**
- **Play Offline** setup: map, difficulty, faction (Crimson / Cobalt / Random), optional match seed
- **Difficulty locked** for the match once it begins
- **Pause menu**: Resume, Restart Match, Return to Main Menu
- **Play Online** lobby shell (UI only — service not connected)
- **Gold Shop** — account-level premium Gold wallet, data-driven packages, checkout placeholder (no real payments)
- **How to Play** and **Credits / Version** screens
- **Event Log** window with filters and unread badge
- **Production requirements** (Barracks, Heavy factory, Ordnance foundry, Airbase, Port)
- **Queue limits** (max 3 build / 3 train per city)
- **Combat** continues each tick until one side is destroyed; paths cancel when battle starts
- **Speed** 1× / 2× / 4× applied once via tick rate
- **Seeded RNG** for reproducible matches
- **Clear feedback** on invalid or unreachable moves

### Core gameplay (carried forward)

- **1v1 single-player** on the Frontier map (22 × 14 provinces, 200px tiles)
- **12-unit roster** including militia, infantry lines, scout cars, mechs, AA, artillery, fighters, bombers, destroyers
- **Match resources:** Food, Metal, Oil, Manpower, Cash, Research Points
- **Gold** is a separate **account/premium** currency — not produced in matches and not used for combat balance
- **Capital system**, upkeep, research trees, market trades, terrain modifiers
- **Ground-only** tile and city capture; air and navy fight but do not claim land
- **Bot campaign phases** with Easy / Normal / Hard behavior

## How to play

1. Download the **v0.19** HTML from [Releases](https://github.com/AmazighOasisAzul/iron-steel/releases).
2. Open it in a modern browser.
3. From the main menu choose **Play Offline**, set difficulty and faction, then **Start Match**.
4. Click units, then a province, to move. Click an owned city to queue units or buildings.
5. Use Research, Market, Diplomacy, the Events button, and the pause menu (☰).

## Implementation status

v0.19 is a single self-contained HTML file (inline CSS and JavaScript, canvas map). No build step, backend, multiplayer service, real payments, or account server. Preferences can be stored in the browser; the demo Gold wallet is local/demo only and is not a permanent store of truth for purchases.

## Release history

| Version | Status | Notes |
|---------|--------|-------|
| v0.1–v0.16 | Prerelease | Map, economy, bot, research, capital iterations |
| v0.17 | Prerelease | Difficulty, air fuel/shadow, diplomacy replies |
| v0.18 | Prerelease | Facing direction, plane faction color fix |
| **v0.19** | **Official public playable** | Menus, Gold Shop shell, Event Log, production gates, combat/speed fixes, multiplayer-ready UI foundations |

## Roadmap

- Playtest balance (costs, phases, difficulty pacing)
- Polish first map (rivers, ports, claims)
- Facing/orientation polish where still imperfect
- Fog of war / intel
- Real audio when assets exist
- Second map only after the first map and bot feel solid
- Multiplayer, real checkout, and accounts when infrastructure exists

## Disclaimer

Independent fan project for learning and fun. All rights to the original titles belong to their respective owners.
