# Code Like It's 198x

**Learn assembly by building complete games for classic computers.**

> *"Still teaching the world to code, 40 years later."*

---

## What is Code198x?

Code198x teaches game development through complete projects. No isolated exercises — you build real, playable games from start to finish, learning assembly along the way.

Each game is broken into units. Each unit introduces one concept, adds one feature, and ends with working code you can run. By the final unit, you have a complete game and understand every line.

**Website:** [code198x.stevehill.xyz](https://code198x.stevehill.xyz)

---

## Current Games

### Commodore 64

| Game | Status | Units | What You Learn |
|------|--------|-------|----------------|
| **SID Symphony** | ✅ Complete | 16 | 6510 assembly, SID audio, state machines, input handling, visual effects |

**SID Symphony** is a rhythm game. You build it from an empty screen to a full game with three-track gameplay, timing grades, combo multipliers, high scores, and pause functionality — all in 6510 assembly.

### Coming Soon

| System | Game | Status |
|--------|------|--------|
| **ZX Spectrum** | TBD | Z80 assembly — next in development |
| **NES** | TBD | 6502 assembly — planned |
| **Amiga** | TBD | 68000 assembly — planned |

---

## Repositories

| Repository | Purpose |
|------------|---------|
| [**website**](https://github.com/code198x/website) | All lesson content (Astro + MDX) |
| [**code-samples**](https://github.com/code198x/code-samples) | Working source code for every unit |
| [**commodore-64-dev**](https://github.com/code198x/commodore-64-dev) | Docker-based C64 development environment |

---

## Getting Started

**Start SID Symphony:**

1. Visit [code198x.stevehill.xyz/commodore-64/game-01-sid-symphony](https://code198x.stevehill.xyz/commodore-64/game-01-sid-symphony)
2. Follow Unit 1
3. Type the code into VICE (or use the Docker environment)
4. Build from there — each unit adds one feature

**Set up the development environment:**

```bash
git clone https://github.com/code198x/commodore-64-dev.git
cd commodore-64-dev
docker-compose up -d
docker-compose exec workspace bash
```

You now have ACME assembler and VICE emulator ready to go.

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
- **ACME** — reliable cross-assembly
- **The retro community** — keeping these machines alive
- **Original 8-bit developers** — proving what's possible with limited hardware

---

**Start building:** [code198x.stevehill.xyz](https://code198x.stevehill.xyz)
