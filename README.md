# WSCROLLER

A precalculated sine scroller proof-of-concept for the Wonderswan, built from the Japanese WonderWitch manual and compiled with the LCC86 C compiler. It runs on a real Wonderswan but not in emulators. There were some issues with version control, so if it doesn't run on your Wonderswan, please let me know.

## Description

This is a minimalist Wonderswan game/demo that showcases a sine wave-based scrolling effect. The program displays text and creates an animated sine wave scroll on the Wonderswan's display.

## Features

- **Sine Wave Scroller**: Uses a precalculated 256-entry sine table for smooth wave animation
- **Real Hardware Support**: Confirmed to work on actual Wonderswan devices
- **Simple Controls**:
  - UP button: Slow down animation
  - DOWN button: Speed up animation
  - START button: Exit program
- **Minimal Resource Usage**: Designed for the Wonderswan's limited capabilities
- **Historical Artifact**: Built from Japanese WonderWitch development materials

## Technical Details

### Hardware
- **Platform**: Wonderswan handheld console
- **Compiler**: LCC86 C compiler
- **Source Material**: Japanese WonderWitch development manual

### Code Structure

**scroll6.c**: Main program file
- Precalculated sine table (256 values) for efficient wave generation
- Real-time scroll position calculation using modulo arithmetic
- Game loop with user input handling
- Text display functionality

**scroll.cf**: Compilation configuration file
- WonderWitch project file format
- Specifies program name, output format, and build parameters

**BOOT_H.FX**: Compiled binary
- Executable Wonderswan game file (.FX format)
- Ready to run on real hardware

## How to Use

### On Real Hardware
1. Transfer the `BOOT_H.FX` file to your Wonderswan using WonderWitch tools
2. Run the program on your device
3. Use the controls to adjust animation speed
4. Press START to exit

### Building from Source (if you have WonderWitch)
1. Install LCC86 compiler and WonderWitch SDK
2. Compile with the provided configuration: `scroll.cf`
3. This will generate the `.FX` executable file

## Known Issues

- **Emulator Compatibility**: The program does not run correctly in Wonderswan emulators due to differences in hardware emulation or timing
- **Version Control**: There were some issues with the original version control history of this project
- **Kanji Display**: Depends on your Wonderswan's language settings

## Wonderswan Platform

The Wonderswan is a monochrome handheld console released by Bandai in 1999. It features:
- 224×144 pixel display
- 16-bit CPU (x86-based)
- Limited RAM (64KB)
- Cartridge-based games

## Historical Context

The WonderWitch was a development kit released by Bandai that allowed hobbyists to create games for the Wonderswan. This project represents early amateur game development for the platform, showcasing creative solutions for animation on extremely resource-constrained hardware.

## License

This project is a historical preservation of WonderWitch sample code. Check the original WonderWitch SDK documentation for licensing information.

## Notes

- This is a proof-of-concept demonstrating sine wave animation techniques
- The precalculated sine table approach was a common optimization technique on retro hardware
- If you have a real Wonderswan and this doesn't run, please open an issue with details about your device

---

*A historical artifact from the WonderWitch era of handheld game development.*
