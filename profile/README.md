# Code Like It's 198x

**Learn assembly by building complete games for classic computers.**

> *"Still teaching the world to code, 40 years later."*

---

## What is Code198x?

Code198x teaches game development through complete projects. No isolated exercises — you build real, playable games from start to finish, learning assembly along the way.

Each game is broken into units. Each unit introduces one concept, adds one feature, and ends with working code you can run. By the final unit, you have a complete game and understand every line.

**Website:** [code198x.stevehill.xyz](https://code198x.stevehill.xyz)

---

## Games

### Commodore 64

| Game | Units | What You Learn |
|------|-------|----------------|
| **SID Symphony** | 16 | 6510 assembly, SID audio, state machines, input handling, visual effects |

A rhythm game. Build from an empty screen to a full game with three-track gameplay, timing grades, combo multipliers, high scores, and pause functionality.

### ZX Spectrum

| Game | Units | What You Learn |
|------|-------|----------------|
| **Ink War** | 16 | Z80 assembly, ULA graphics, keyboard input, game state, territory mechanics |

A territory control strategy game. Two players compete to claim cells on a grid, with expanding territories and strategic blocking.

### Commodore Amiga

| Game | Units | What You Learn |
|------|-------|----------------|
| **Hop** | 16 | 68000 assembly, Copper, Blitter, Paula audio, bitplane graphics |

A Frogger-style arcade game. Guide your frog across traffic and rivers, avoiding hazards and riding logs to reach safety.

### Nintendo Entertainment System

| Game | Units | What You Learn |
|------|-------|----------------|
| **Neon Nexus** | 16 | 6502 assembly, PPU graphics, APU audio, NMI handling, sprite management |

A fixed-screen action game. Navigate an arena with multiple enemy types, collect items, and survive with progressive difficulty.

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
| Commodore 64 | [SID Symphony Unit 1](https://code198x.stevehill.xyz/commodore-64/game-01-sid-symphony/unit-01) |
| ZX Spectrum | [Ink War Unit 1](https://code198x.stevehill.xyz/sinclair-zx-spectrum/game-01-ink-war/unit-01) |
| Amiga | [Hop Unit 1](https://code198x.stevehill.xyz/commodore-amiga/game-01-hop/unit-01) |
| NES | [Neon Nexus Unit 1](https://code198x.stevehill.xyz/nintendo-entertainment-system/game-01-neon-nexus/unit-01) |

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

**Start building:** [code198x.stevehill.xyz](https://code198x.stevehill.xyz)
