# Iron Steel

**Iron Order 1919–inspired fan strategy game**

Single-player province strategy inspired by *Iron Order 1919*, *Call of War*, and the Supremacy engine (*Conflict of Nations*, *Supremacy 1914*).

Fan project — not affiliated with Bytro Labs, Dorado Games, Twin Harbour Interactive, or Stillfront Group.

---

## Latest release: v0.23

Download **iron-steel-v0.23.html** from the [releases page](https://github.com/AmazighOasisAzul/iron-steel/releases).

Open the HTML file in a modern desktop browser. It runs offline, needs no install, and does not contact a game server.

**v0.19** was the first official public playable milestone. **v0.20–v0.22** were prereleases. **v0.23** is the current published build.

### What is new in v0.23

- **Official favicon** — IRON / STEEL mark
- **Gold Shop**
  - Tabs: Buy premium currency | Buy a premium account | Cosmetics
  - Original packs (Scout, Officer, General, Marshal) **plus** Supremacy-style scale packs (1,500–250,000 Gold)
  - EUR prices; Popular tag on War Chest
  - Premium account demo offer (checkout not connected)
- **Global Commodity Exchange**
  - Full trade-route table (expanded offers for food, metal, oil, cash)
  - Stockpile bar and Market Reform efficiency
  - Open by clicking **Food / Metal / Oil / Cash** on the top bar
  - Market tab removed from the command sidebar
- **Win-mode setup** — extra fields only appear for the selected win mode

### From v0.20–v0.22 (included)

- Longer base tick pace; 1× / 2× / 3× / 4× speed
- Negative-balance confirmation modal (Spend anyway / Spend Gold / Cancel)
- Desert terrain; deep-water isolation; destination-based move costs
- Victory points (city 5, land 1, water/river 0) and multiple win modes
- Combat roles by tile owner; full stack combat; capture after combat
- Live **combat panel** (terrain, fort/capital, damage, losses)
- Easy difficulty: bot never attacks or captures the player
- Settings enforcement: gold ban, ground stack cap, air/navy off
- Building limits, diminishing returns, bot income/production by difficulty
- AI focus rotation (expand / defend / pressure)
- Research panel shows RP and Secret Lab status

### Core gameplay

- **1v1 single-player** on the Frontier map (22 × 14 provinces, 200px tiles)
- Unit roster: militia, light/infantry lines, scout cars, mechs, AA, artillery, fighters, bombers, destroyers
- **Match resources:** Food, Metal, Oil, Manpower, Cash, Research Points
- **Gold** is account/premium currency — not produced in matches
- Capital system, upkeep, research trees, terrain modifiers
- Ground-only tile and city capture
- Bot campaign phases with Easy / Normal / Hard

## How to play

1. Download the latest HTML from [Releases](https://github.com/AmazighOasisAzul/iron-steel/releases).
2. Open it in a modern browser.
3. **Play Offline** → set difficulty, faction, optional win mode → **Start Match**.
4. Click units, then a province, to move. Click an owned city to queue units or buildings.
5. Click **Food / Metal / Oil / Cash** on the top bar for the commodity exchange.
6. Use Research, Diplomacy, Events, and the pause menu (☰).

## Implementation status

Single self-contained HTML file (inline CSS and JavaScript, canvas map). No build step, backend, multiplayer service, real payments, or account server. Preferences and demo Gold wallet use local browser storage only.

## Release history

| Version | Status | Notes |
|---------|--------|-------|
| v0.1–v0.18 | Prerelease | Map, economy, bot, research, capital iterations |
| **v0.19** | First official public playable | Menus, Gold Shop shell, Event Log, production gates |
| v0.20–v0.22 | Prerelease | Pace, combat fixes, AI, market/terrain polish |
| **v0.23** | **Current release** | Favicon, full Gold Shop packs, commodity exchange, win-mode UI |

## Roadmap

### Near term

- Playtest balance (costs, phases, difficulty pacing)
- Fixed default 1v1 map layout as the stable baseline
- Facing / unit orientation polish
- Bot refinements (frontlines, scouting, less stacking)

### Map terrain rules (design law)

- **Deep water never touches land** — shallow water between deep and land
- **Shallow water** forms coastal rings and lake shores
- **Rivers** from mountain tiles; passable for ground, not claimable, 0 VP, not navigable for navy
- **Impassable** only when fully surrounded by mountains
- City placement may vary; bulk terrain stays coherent

### Intel and fog of war

- Fog of war / unexplored provinces
- Scout and air intel ranges
- Espionage-style information
- Shared vision for future coalitions

### UI expansion

- Province inspector / floating city card
- Better unit selection, stack list, path preview
- Combat panel as map-anchored or collapsible drawer
- Research tree layout improvements
- Minimap / strategic overview
- Accessibility: contrast, scale, keyboard basics

### Audio

- Sound effects and music when assets exist (currently Coming Soon)

### Maps, map creation, and modes

- Second official map after the first map and bot feel solid
- **Map creation** — terrain, cities, spawns, water rules, win setup
- Custom maps and gamemodes (host rules: gold, win conditions, toggles)
- Larger tiles under consideration (e.g. 400px / 600px)

### Multiplayer and social

- Multiplayer lobbies and host rules
- Real accounts, match history, server-backed Gold wallet / checkout
- **Coalitions / clans**
- Spectator and replay foundations

### Later-stage systems

- Cosmetics fully wired to Gold Shop
- Cross-match progression that does not break match balance
- Mobile / touch layout if demand exists

## Disclaimer

Independent fan project for learning and fun. All rights to the original titles belong to their respective owners.
