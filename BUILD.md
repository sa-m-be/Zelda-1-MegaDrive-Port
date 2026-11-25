# Build and test guide

## Current build pipeline

I am consolidating the development revisions into a reproducible build. The experimental local converter uses the original USA PRG0 iNES ROM, generates the translated code and graphics, builds MD13 with the matching toolchain and applies nine incremental overlays to reconstruct MD35.

The original toolchain is MarsDev v1.0.0-rc1 with SGDK 1.81. The local frontend requires Python 3.10+, GNU Make and a compatible build environment. That earlier toolchain-based pipeline is not yet validated as a clean build. The newer direct conversion engine described below has been verified outside the browser.

| Reference | SHA-256 |
| --- | --- |
| NES USA PRG0, 131088 bytes | `8f72dc2e98572eb4ba7c3a902bca5f69c448fc4391837e5f8f0d4556280440ac` |
| MD13 | `900f98c16f930b8d1c77e725497169022ea4e102b62b65139e3e7707070f4699` |
| MD35, 2097152 bytes | `dc4d6ffdcbca7156333c0b07cdd00a98977e733913a1174e9a636c205bf24a09` |

I have verified the generated MD13 source files against the archived outputs and the overlay chain against the MD35 reference binary. This does not yet establish a successful clean build from the original NES ROM.

## Browser converter

My newer direct conversion engine uses a fixed pre-linked runtime, a local 6502-to-68000 translator, a two-pass assembler, graphics reconstruction and revision overlays. I verified the resulting ROM byte for byte against the reference in desktop Python. The web interface loads Pyodide from a CDN, without requiring a desktop SDK or an intermediate ROM. Full browser integration testing and distribution review remain pending. See the [converter repository](https://github.com/sa-m-be/Zelda-1-MegaDrive-Converter).

## Testing

My real-hardware setup is an original Japanese Mega Drive Model 1 with EverDrive V3 Pro. I also test with BlastEm. Planned regression coverage includes boot, title, controls, both quests, dungeon transitions, pause menu, saves, audio and complex combat scenes.

I will publish specific build instructions and approved files once the pipeline and distribution review are complete.
