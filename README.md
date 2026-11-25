# The Legend of Zelda — Mega Drive / Genesis Port

![Platform](https://img.shields.io/badge/platform-Mega%20Drive%20%2F%20Genesis-blue) ![Status](https://img.shields.io/badge/status-experimental-orange) ![Hardware tested](https://img.shields.io/badge/hardware-tested-brightgreen) ![Architecture](https://img.shields.io/badge/architecture-68000%20%2F%20Z80-lightgrey)

An unofficial fan-led technical project exploring a native adaptation of the original 1986 NES game for the Sega Mega Drive / Genesis. The goal is to reproduce the original gameplay on Sega hardware without embedding a NES emulator.

[Português (Brasil)](README.pt-BR.md) · [FAQ](FAQ.md) · [Build](BUILD.md) · [Changelog](CHANGELOG.md) · [Roadmap](ROADMAP.md) · [Contributing](CONTRIBUTING.md) · [Credits](CREDITS.md)

## Development status

The most recent development milestone recorded in this documentation is MD22. The project remains experimental; this is not a claim of full game completion or hardware compatibility.

| Subsystem | Reported status |
| --- | --- |
| Native execution | Implemented; further verification needed |
| Player movement and controls | Working in development tests |
| Overworld and dungeon scrolling | Working in development tests |
| Dungeon borders | Corrected in recent revisions |
| Music | Working in development tests |
| Sword and damage sound effects | Present; volume balance needs tuning |
| Original hardware | Tested on Japanese Mega Drive Model 1 with EverDrive V3 Pro (developer report) |
| Full game, both quests and save behavior | Not yet certified |

## Hardware compatibility

The port has been tested on an original Japanese Sega Mega Drive Model 1 (NTSC-J) using an EverDrive V3 Pro flash cartridge, as reported by the project developer. Exact tested build, cartridge firmware, test duration and scope were not specified. This is not a full compatibility certification.

| Configuration | Status |
| --- | --- |
| Mega Drive Model 1 (Japan) + EverDrive V3 Pro | Tested |
| Mega Drive Model 2 | Not yet verified |
| Genesis (North America) | Not yet verified |
| Mega Drive (PAL) | Not yet verified |
| FPGA / MiSTer | Not yet verified |

## Getting started

See [BUILD.md](BUILD.md) for the intended build and testing workflow. No downloadable build is included in this documentation package. When an authorized release is available, follow its version-specific instructions.

## Project goals

- Native operation on Mega Drive / Genesis hardware.
- Faithful gameplay, graphics timing, controls and sound behavior.
- A 60 fps performance target where practical; not a measured guarantee.
- Reproducible builds, documented changes and community testing.

## Feedback

Use GitHub Issues to report a reproducible bug. Include the build identifier, emulator or console, region and steps to reproduce. See [CONTRIBUTING.md](CONTRIBUTING.md).

## Rights and distribution

This is an unofficial project, not affiliated with, endorsed by or sponsored by Nintendo or Sega. The original game and its protected content remain the property of their respective rights holders. This repository must not include unauthorized ROMs, extracted assets, or other material that the uploader has no right to distribute. Any patch or translated code must also be reviewed for redistribution rights. No license to third-party intellectual property is granted by this notice.
