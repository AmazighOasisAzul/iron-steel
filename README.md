# Iron Steel

**Iron Order 1919–inspired fan prototype**

Single-player province strategy inspired by *Iron Order 1919*, *Call of War*, and the Supremacy engine (*Conflict of Nations*, *Supremacy 1914*).

Fan project — not affiliated with Bytro Labs, Dorado Games, Twin Harbour Interactive, or Stillfront Group.

## Current playable release: v0.17

[Download the v0.17 HTML build](https://github.com/AmazighOasisAzul/iron-steel/releases/download/v0.17/iron-steel-v0.17.html) or browse the [releases page](https://github.com/AmazighOasisAzul/iron-steel/releases).

v0.17 is a self-contained browser game: download the HTML file and open it in a modern desktop browser. It runs offline, needs no installation, and does not contact a game server.

### v0.17 highlights

- **1v1 single-player:** a 22 × 14 province map (200 px logical tiles), with three cities per side and six neutral cities.
- **12-unit roster:** militia, light infantry, infantry, assault infantry, scout cars, light/heavy mech, AA, artillery, fighters, bombers, and destroyers.
- **Resources:** Food, Metal, Oil, Manpower, Cash, and Research Points. Gold is deliberately locked; Goods and Rare Materials are not used.
- **Economy:** city/building income, timed construction and training queues, fixed resource trades, upkeep, and negative stockpiles (except Research Points).
- **Capital system:** capitals give strong local defence. Losing one reduces resource production and combat by 20% and raises upkeep by 75% until a new capital is completed.
- **15 buildings:** Capital, Barracks, Heavy Factory, Ordnance Foundry, Airbase, Power Plant, Industry, Farm, Bank, Recruiting Office, Rail Line, Fortress, Port, Secret Lab, and Supply Hub.
- **Building effects:** Supply Hubs halve local unit upkeep; Rail Lines increase movement; Power Plants speed training; Secret Labs generate Research Points; Fortresses reduce incoming combat damage.
- **Research:** infantry, armour, artillery, air, naval, economy, and doctrine trees with real combat, upkeep, cost, train-time, and income effects.
- **Territory/capture:** only ground units claim open land and capture cities. Air and naval units fight but never claim territory.
- **Map terrain:** plains, forests, hills, mountains, passable rivers, lakes, shallow/deep water, and impassable tiles.
- **Settings:** Easy/Normal/Hard difficulty, enemy political-territory view, plus sound/music/graphics preference stubs stored locally in the browser.
- **Diplomacy UI:** Greeting, Trade, Truce, and War messages receive a simple default bot reply.

## Bot campaign and difficulty

The bot plans movement every few ticks, expands across neutral land/cities, develops its cities, researches, trades for shortages, and uses anti-stacking destination reservations.

- Bot ground stacks are capped at **8 units per tile**; player stacks are unrestricted.
- Normal campaign phases: **Early Scout** (to tick 70) → **Air / Navy** (110) → **Mid Invasion** (160) → **Defend** (200) → **Re-scout** (230) → **Final Offensive**.
- On Normal, bot ground forces may assault player cities from tick 150; Hard opens this at tick 120 and skips the defensive phase.
- Easy keeps the bot in expansion/defence behavior and never allows it to assault player cities.
- All difficulties increase late-game bot pressure after tick 250.

## How to play

1. Download [iron-steel-v0.17.html](https://github.com/AmazighOasisAzul/iron-steel/releases/download/v0.17/iron-steel-v0.17.html).
2. Open it in a modern browser.
3. Click one or more friendly units, then click a destination province to issue movement orders.
4. Click an owned province to queue units or buildings.
5. Use the **Research**, **Market**, and **Diplomacy** tabs. Open **Settings** from the ⚙ button; scroll the map to zoom.

## Implementation status

The current v0.17 game is a single HTML file with inline CSS and JavaScript, rendered through an HTML canvas. It has no build step, external runtime dependency, backend, multiplayer service, account system, or save/load game system. Only the settings choices are stored locally in the browser.

The repository's `prototypes/` files are historical placeholders. The current playable v0.17 source is published as the release HTML asset, rather than as a maintained source file on `main`.

## Release history

| Version | Notes |
|---------|-------|
| v0.1–v0.8 | Early prototypes, map and tile work |
| v0.9 | Full roster, Secret Lab, 200 px tiles, log toggle |
| v0.10 | Market trades, timed unit production, Gold locked, bot expansion |
| v0.11 | Food/Cash, research trees, no Rare Materials |
| v0.12 | Goods removed; unit upkeep; economy research effects; no disband |
| v0.13 | Capital system; Supply Hub, Power Plant, Recruiting Office, Rail Line; settings; own-territory tint |
| v0.14 | Light infantry; bot postures; ground-only capture; bot ground-stack cap |
| v0.15 | Player cities as bot objective; expansion cover; destination reservations |
| v0.16 | Phased bot campaign, city-assault gates, phase-based production |
| **v0.17** | **Current playable release** — difficulty settings, aircraft movement oil cost/shadows, and refined diplomacy/UI |

## Future direction

- Keep the current playable source in the repository before the next feature build.
- Balance and playtest campaign pacing, unit costs, terrain, and difficulty.
- Polish the first map, including clear river/port/claim rules.
- Add fog of war and intel.
- Add real audio when assets exist.
- Consider a second map only after the first map is solid.
- Explore multiplayer lobbies/host rules, coalitions, custom maps, and gamemodes as later-stage work.

## Disclaimer

Independent fan prototype for learning and fun. All rights to the original titles belong to their respective owners.
