# Big World

An [Ignitron](https://codeberg.org/ignitron/ignitron) mod for **Allumeria** (0.16.6+). It makes worlds bigger and stops caves from punching holes through hills.

**[⬇ Download the latest release](../../releases/latest)**

## Features

- **4× the land.** New worlds are **2048×2048** blocks; vanilla is 1024×1024. You can set any size from 512 to 4096.
- **Biomes scale with the world.** Snow and desert get bigger and move further out from spawn, so the extra space isn't just more plain forest.
- **Cleaner hills.** Cave tunnels no longer burst out of hillsides and leave ragged gouges. A cave near a hill face gets one rounded, walk-in **cave mouth** (about 3×3) at the bottom of the hill instead. Flat ground stays sealed.

Everything here only affects **new** worlds. Existing saves load normally and stay as they were.

## Install

1. Install the Ignitron loader (0.8.10 or newer): <https://codeberg.org/ignitron/ignitron>
2. Download `BigWorld-<version>.zip` from [Releases](../../releases/latest).
3. Drop the zip into `Allumeria/mods/` **as is**. Don't unzip it.
4. Start the game and create a new world.

## Config

`mods/BigWorldMap.config.json` is created on first launch. Edit it while the game is closed.

| Setting | Default | What it does |
|---|---|---|
| `world_size_chunks` | `64` | World width in chunks (vanilla 32, range 16–128) |
| `scale_biomes_with_world` | `true` | Spread snow/desert biomes out with the world size |
| `cave_entrances` | `true` | Turn the cave-mouth change on or off |
| `cave_mouth_size` | `1.6` | Tunnel radius (1.6 is about 3×3) |
| `cave_mouth_max_length` | `16` | How far from the cave a hill face can be |
| `cave_entrance_chance` | `1.0` | 0–1, chance that a qualifying cave gets a mouth |
| `cave_entrance_spacing` | `40` | Minimum blocks between two cave mouths |

## License

All rights reserved. You're free to download Big World and use it to play Allumeria. Please don't redistribute, repackage, or modify it without permission. See [LICENSE](LICENSE).
