# Build and test guide

## Current build pipeline

I am consolidating the development revisions into a reproducible build. The experimental local converter uses the original USA PRG0 iNES ROM, generates the translated code and graphics, builds MD13 with the matching toolchain and applies nine incremental overlays to reconstruct MD35.

The original toolchain is MarsDev v1.0.0-rc1 with SGDK 1.81. The local frontend requires Python 3.10+, GNU Make and a compatible build environment. Full clean compilation from NES input and native desktop compatibility are not yet validated.

| Reference | SHA-256 |
| --- | --- |
| NES USA PRG0, 131088 bytes | `8f72dc2e98572eb4ba7c3a902bca5f69c448fc4391837e5f8f0d4556280440ac` |
| MD13 | `900f98c16f930b8d1c77e725497169022ea4e102b62b65139e3e7707070f4699` |
| MD35, 2097152 bytes | `dc4d6ffdcbca7156333c0b07cdd00a98977e733913a1174e9a636c205bf24a09` |

I have verified the generated MD13 source files against the archived outputs and the overlay chain against the MD35 reference binary. This does not yet establish a successful clean build from the original NES ROM.

## Browser converter

My browser prototype validates the NES input, has an experimental source-generation mode and supports the MD13-to-MD35 updater. The updater has been verified with the reference hashes. Direct browser compilation to a playable ROM and full browser UI testing are still pending. The source-generation mode uses a Pyodide runtime fetched from a CDN; it is not a standalone offline build.

## Testing

My real-hardware setup is an original Japanese Mega Drive Model 1 with EverDrive V3 Pro. I also test with BlastEm. Planned regression coverage includes boot, title, controls, both quests, dungeon transitions, pause menu, saves, audio and complex combat scenes.

I will publish specific build instructions and approved files once the pipeline and distribution review are complete.
