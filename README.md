# The Legend of Zelda — Mega Drive / Genesis Native Port

![Platform](https://img.shields.io/badge/platform-Mega%20Drive%20%2F%20Genesis-blue) ![Hardware](https://img.shields.io/badge/hardware-tested-brightgreen) ![Status](https://img.shields.io/badge/status-in%20development-orange)

[Português (Brasil)](README.pt-BR.md) · [FAQ](FAQ.md) · [Help](HELP.md) · [Build](BUILD.md) · [Changelog](CHANGELOG.md) · [Roadmap](ROADMAP.md) · [Contributing](CONTRIBUTING.md)

## About my project

I started this project to bring the original 1986 NES game, The Legend of Zelda, to the Sega Mega Drive / Genesis as a native port, not as an emulator. My goal is to preserve the original gameplay and experience while adapting the game to the architecture of Sega's 16-bit console.

The game logic runs on the Motorola 68000. I use static translation of the original PRG0 code alongside native routines for video, controls and other platform-specific behavior. Audio uses the Mega Drive's PSG, YM2612 and Z80 for the reserved DMC effects. The sound implementation remains an approximation of the original NES APU.

## Current development status

My current reference build includes the work on movement, scrolling, dungeon rendering, sound and pause-screen corrections. I am continuing to validate the game and refine compatibility.

| Feature | Status |
| --- | --- |
| Native 68000 execution | Implemented |
| Player movement and controls | Working in development tests |
| Overworld and dungeon scrolling | Working in development tests |
| Dungeon rendering | Corrected in development tests |
| Music and sound effects | Implemented; further audio validation planned |
| Title and pause menu | Updated |
| Original hardware | Tested on the setup below |
| Full playthroughs of both quests and save/load | Full validation pending |
| Sustained 60 fps in all scenes | Not yet verified |

## Real hardware testing

I have tested the port on my original Japanese Sega Mega Drive Model 1 (NTSC-J) using an EverDrive V3 Pro flash cartridge. This is my real-hardware test setup; I am not claiming complete compatibility across all console revisions or regions.

| Configuration | Status |
| --- | --- |
| Mega Drive Model 1 (Japan) + EverDrive V3 Pro | Tested |
| Mega Drive Model 2 | Not yet verified |
| Genesis (North America) | Not yet verified |
| Mega Drive (PAL) | Not yet verified |
| MiSTer / FPGA | Not yet verified |

I also use BlastEm during development. I plan to expand testing and welcome reproducible reports from other setups.

## Web converter

My [web converter](https://sa-m-be.github.io/Zelda-1-MegaDrive-Converter/) is designed to generate the port locally from a compatible original NES ROM, without desktop installations or an external SDK. The direct conversion engine has been verified against my reference ROM outside the browser; full browser integration testing and distribution review are still pending. When the converter is ready for use, select the NES ROM, choose **Generate Mega Drive ROM**, then **Download PORT**. See [BUILD.md](BUILD.md) for technical details.

## Getting started and feedback

Check [Help](HELP.md) and [FAQ](FAQ.md) for instructions and current limitations. I will document available releases and their requirements in GitHub Releases. If you find a bug, please open an Issue with the revision, your setup and the steps to reproduce it.

## Credits and rights

I maintain this independent fan project under the GitHub account [sa-m-be](https://github.com/sa-m-be). See [CREDITS.md](CREDITS.md) for acknowledgments.

The Legend of Zelda and its original content belong to their respective rights holders. This project is not affiliated with or endorsed by Nintendo or Sega. I do not provide an original NES ROM or a complete converted ROM in this documentation repository. I am reviewing the redistribution rights of code and patches before making them publicly available.
