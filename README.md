# Iron Steel

**Iron Order 1919–inspired fan prototype**

Single-player province strategy inspired by *Iron Order 1919*, *Call of War*, and the Supremacy engine (*Conflict of Nations*, *Supremacy 1914*).

Fan project — not affiliated with Bytro Labs, Dorado Games, Twin Harbour Interactive, or Stillfront Group.

## Latest release: v0.15

Playable builds are on the [releases page](https://github.com/AmazighOasisAzul/iron-steel/releases).

Download the HTML for a release and open it in any modern browser.

### Features (through v0.15)

- **1v1 single-player** vs rule-based bot (square grid, 200px tiles, mouse-wheel zoom)
- **Resources:** Food, Metal, Oil, Manpower, Cash, RP — Gold locked. No Goods. No Rare materials.
- **Capital:** One per side; destroyed on city capture; −20% output and high upkeep until rebuilt
- **Buildings:** Capital, Barracks, Heavy factory, Ordnance foundry, Airbase, Power plant, Industry, Farm, Bank, Recruiting office, Rail line, Fortress, Port, Secret lab, Supply hub
- **Upkeep:** Units drain Food, Metal, Oil, Cash, Manpower; can go negative; no disband
- **Capture:** Ground units only; air and navy do not claim tiles or cities
- **Bot (v0.14–v0.15):** Postures (secure / scout / defend / attack); scout types (militia, light infantry, scout car, plane); max 8 bot ground units per tile; anti-stack reservations; player cities as final objective with expansion as cover
- **Settings:** Sound, music, graphics stubs; show enemy political territory
- **Research / market / timed production** as in earlier versions

### Known bot gaps (next work — not shipped yet)

- Still rushes player cities too early; needs a **phased campaign** with long tick delays before ground city assaults
- Planned phases: early scout → air/navy harassment → mid-game ground invasion → defend → scout → final offensive, while expanding and taking neutral cities

## How to play

1. Download the HTML from the [releases page](https://github.com/AmazighOasisAzul/iron-steel/releases) and open it in a browser.
2. Click a unit (or stack) → click a province to move.
3. Click a province you own to queue units or buildings.
4. Mouse wheel to zoom.
5. Use Research, Market, and Diplomacy tabs; open Settings from the top bar.

## Versions

| Version | Notes |
|---------|-------|
| v0.1–v0.8 | Early prototypes, map and tile work |
| v0.9 | Full roster, Secret lab, 200px tiles, log toggle |
| v0.10 | Market trades, timed unit production, gold locked, bot expansion |
| v0.11 | Food / Cash, research trees (no rare) |
| v0.12 | Goods removed; unit upkeep; Logistics / War economy / Industrial push; no disband |
| v0.13 | Capital system; supply hub / power / recruit / rail; settings popup; own-only territory tint |
| v0.14 | Light infantry; bot postures; ground-only capture; bot ground stack max 8; fewer messages |
| **v0.15** | **Current release** — player cities as final objective; expansion as secondary cover; anti-stack destination reserves |

## Roadmap

- **Bot campaign phases** (scout → air/navy → mid invasion → defend → final push) with tick gates before city assaults
- 1v1 map polish (rivers not claimable; layout fixes) — after bot feels right
- Second map — only after first map and bot are solid
- Fog of war / intel
- Real audio when assets exist
- Multiplayer lobbies and host rules (including gold toggle)
- Coalitions / clans
- Custom maps and gamemodes

## Disclaimer

Independent fan prototype for learning and fun. All rights to the original titles belong to their respective owners.
