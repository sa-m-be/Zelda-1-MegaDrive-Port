# Help and troubleshooting

## Before testing

Use a build from a distribution you are authorized to access. Keep your original ROM and save files backed up. Check the release notes for the exact supported revision.

## The game does not start

Check the ROM checksum, emulator or flash cartridge compatibility and the console region. I use the Japanese Mega Drive Model 1 with EverDrive V3 Pro as my reference hardware setup, and BlastEm for development tests.

## Video, sound or pause issues

Please identify the scene, dungeon or menu where the issue occurs. Include whether it is reproducible after a reset and whether you are using an emulator or original hardware.

## Converter issues

The web converter is still a prototype. It can validate a supported NES ROM and update an existing MD13 build to MD35, but cannot yet compile the game directly from the NES ROM. The local build frontend is also experimental. See [BUILD.md](BUILD.md).

## Reporting a problem

Open an Issue and include the ROM revision or SHA-256, console region, hardware or emulator version, flash cartridge and firmware if applicable, and exact steps to reproduce. Please do not attach ROMs or extracted copyrighted assets.
