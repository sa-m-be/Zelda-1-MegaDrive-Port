# Frequently asked questions

## Is this a NES emulator?
No. My goal is to run the game natively on Mega Drive hardware. The port uses translated 68000 code and target-specific routines rather than a NES CPU interpreter.

## What version am I working on?
MD35 is my current reference build for this repository. Earlier development filenames may not reflect the actual internal revision; I use SHA-256 to identify the build.

## Is the port finished?
It is still in development. I have tested movement, scrolling, dungeon rendering and audio, but complete playthroughs of both quests and save/load validation are still on my roadmap.

## Have you tested it on original hardware?
Yes. I tested it on my original Japanese Mega Drive Model 1 (NTSC-J) with an EverDrive V3 Pro. I have not certified compatibility with every other console and cartridge combination.

## Does it run at 60 fps?
That is my performance target. I have not verified a sustained 60 fps in every gameplay scenario.

## Where can I download the port?
Check Releases for any available distribution. I am developing a local web converter and reviewing distribution rights. I do not include a complete original or converted ROM in this documentation repository.

## Will I need to install Python?
My aim is to eliminate that requirement for end users. The browser prototype is not yet capable of compiling directly from a NES ROM. The experimental local build frontend still requires Python and the matching toolchain.

## Why does the sound differ from the NES version?
The two consoles use different sound hardware. I am adapting the original behavior to PSG, YM2612 and Z80 and continuing to refine audio balance and timing.

## How can I help?
Open an Issue with reproducible steps, or see [CONTRIBUTING.md](CONTRIBUTING.md). For troubleshooting, see [HELP.md](HELP.md).
