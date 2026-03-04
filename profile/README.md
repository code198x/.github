# Code Like It's 198x

**Learn assembly by building complete games for classic computers.**

> *"Still teaching the world to code, 40 years later."*

---

## What is Code198x?

Code198x teaches game development through complete projects. No isolated exercises — you build real, playable games from start to finish, learning assembly along the way.

Each game is broken into units. Each unit introduces one concept, adds one feature, and ends with working code you can run. By the final unit, you have a complete game and understand every line.

**Website:** [code198x.com](https://code198x.com)

---

## Games

### Commodore 64

| Game | Units | What You Learn |
|------|-------|----------------|
| **Starfield** | 128 | VIC-II sprites, joystick input, SID sound, raster interrupts |

A single-screen space shooter with hardware sprites. Build from an empty screen to a complete game with player controls, enemies, scoring, and sound effects.

### ZX Spectrum

| Game | Units | What You Learn |
|------|-------|----------------|
| **Shadowkeep** | 128 | Z80 assembly, attribute system, screen memory, room data, keyboard input |

A top-down maze explorer where attributes are the game. Navigate rooms, uncover the map, and survive what lurks in the keep.

### Commodore Amiga

| Game | Units | What You Learn |
|------|-------|----------------|
| **Exodus** | 128 | 68000 assembly, Copper lists, Blitter operations, Paula audio, bitplane graphics |

A terrain puzzle where the Blitter IS the gameplay. Guide creatures across hazardous landscapes using the Amiga's custom chips.

### Nintendo Entertainment System

| Game | Units | What You Learn |
|------|-------|----------------|
| **Dash** | 128 | 6502 assembly, PPU graphics, sprite management, NMI handling, controller input |

A fast-paced side-scrolling runner with obstacle avoidance. Build from a static screen to a complete game with scrolling, hazards, and scoring.

---

## Repositories

| Repository | Purpose |
|------------|---------|
| [**website**](https://github.com/code198x/website) | All lesson content (Astro + MDX) |
| [**code-samples**](https://github.com/code198x/code-samples) | Working source code for every unit |
| [**commodore-64-dev**](https://github.com/code198x/commodore-64-dev) | Docker C64 development environment |
| [**sinclair-zx-spectrum-dev**](https://github.com/code198x/sinclair-zx-spectrum-dev) | Docker ZX Spectrum development environment |
| [**commodore-amiga-dev**](https://github.com/code198x/commodore-amiga-dev) | Docker Amiga development environment |
| [**nintendo-entertainment-system-dev**](https://github.com/code198x/nintendo-entertainment-system-dev) | Docker NES development environment |

---

## Getting Started

**Pick a platform and start Unit 1:**

| Platform | Start Here |
|----------|------------|
| Commodore 64 | [Starfield Unit 1](https://code198x.com/commodore-64/assembly/game-01-starfield/unit-01) |
| ZX Spectrum | [Shadowkeep Unit 1](https://code198x.com/sinclair-zx-spectrum/assembly/game-01-shadowkeep/unit-01) |
| Amiga | [Exodus Unit 1](https://code198x.com/commodore-amiga/assembly/game-01-exodus/unit-01) |
| NES | [Dash Unit 1](https://code198x.com/nintendo-entertainment-system/assembly/game-01-dash/unit-01) |

**Set up a development environment:**

```bash
# Example: Commodore 64
git clone https://github.com/code198x/commodore-64-dev.git
cd commodore-64-dev
docker-compose up -d
docker-compose exec workspace bash
```

Each platform has its own Docker container with assembler and emulator ready to go.

---

## Philosophy

- **Complete games, not exercises** — every project results in something playable
- **One concept per unit** — focused learning without overwhelm
- **Working code first** — understand by doing, not by reading theory
- **Assembly from day one** — no BASIC preamble, straight to the metal
- **British English throughout** — colour, not color

---

## Contributing

- **Issues**: Report problems or suggest improvements
- **Discussions**: Questions and ideas welcome
- **Code**: See CONTRIBUTING.md in individual repositories

---

## Recognition

This project exists because of:

- **VICE Team** — cycle-accurate C64 emulation
- **ACME** — reliable cross-assembly for C64
- **Fuse** — ZX Spectrum emulation
- **pasmonext** — Z80 cross-assembly
- **FS-UAE** — Amiga emulation
- **vasm** — 68000 cross-assembly
- **Mesen** — NES emulation
- **cc65** — 6502 cross-assembly
- **The retro community** — keeping these machines alive
- **Original 8-bit developers** — proving what's possible with limited hardware

---

**Start building:** [code198x.com](https://code198x.com)
