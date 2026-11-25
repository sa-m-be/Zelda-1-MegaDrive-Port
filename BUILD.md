# Build and test guide (provisional)

The original source archive was not included when preparing these docs. The exact assembler, toolchain, dependencies, entry point, output format and build commands must be verified before publishing a reproducible build guide. Do not treat the following as executable instructions.

## Before publishing a build

1. Identify the precise source revision and build script.
2. Record required tool names, versions and installation instructions.
3. If an input ROM is required, document the exact revision, size and checksum; never include the original ROM without authorization.
4. Review the sources, generated outputs, and any patches for redistribution rights.
5. Record the actual command and output checksum for a successful clean build.

## Known hardware test environment

- Console: original Japanese Sega Mega Drive Model 1 (NTSC-J).
- Flash cartridge: EverDrive V3 Pro (developer-reported name).
- Status: tested, according to the project developer. Exact build, firmware and scope remain to be recorded.

## Testing checklist

- Boot and title screen; start and select; player movement and attack.
- Overworld scrolling in all four directions; dungeon entry and exits.
- Collision, enemies, sword and damage sounds; music transitions.
- Save/load, both quests and long play sessions.
- Emulator name/version and region; separately document hardware and flash cartridge testing.

Do not label untested behavior as supported. Attach logs or legally shareable evidence to bug reports.
