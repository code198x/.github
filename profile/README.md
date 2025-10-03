# Code Like It's 198x

**Learn retro game development on classic 8-bit and 16-bit systems.**

> *"WOW, look what I can make this thing do!"*

---

## What is Code198x?

Code198x is a structured educational platform teaching game development for classic computers and consoles. Our philosophy: **every lesson ends with a wonder moment** — a working program you can see, play with, and understand in 15-20 minutes.

We're not building encyclopaedias. We're recreating the magic of typing in programs from 1980s magazines and seeing pixels come alive.

### Learning Philosophy

- **One concept, one program, one WOW moment** — no textbooks, just working code
- **15-20 minutes per lesson** — immediate gratification, not multi-hour marathons
- **No "mastery" claims** — this is an introductory journey (lessons 1-4096 of a complete education)
- **Structured progression** — every phase has concrete lessons, not vague "create your own projects"

---

## Supported Systems

### Currently Available

| System | Status | Lessons |
|--------|--------|---------|
| **Commodore 64** | 🟢 Active Development | BASIC: 64 lessons (8 weeks) <br> Assembly: In progress |
| **ZX Spectrum** | 🟡 Planned | — |
| **NES** | 🟡 Planned | — |
| **Amiga** | 🟡 Planned | — |

### Commodore 64 Learning Path

1. **BASIC (8 weeks, 64 lessons)** — Start here if you've never programmed
   - Week 1-2: Foundations & Core Programming
   - Week 3-4: Graphics, Sound & Game Elements
   - Week 5: Complete Mini-Games (8 playable games)
   - Week 6: Advanced Techniques (hardware tricks)
   - Week 7: Polish & Features (professional touches)
   - Week 8: Complete Projects (full games)

2. **Transition Course (8 lessons)** — Bridge from BASIC to Assembly
   - Why BASIC hits limits
   - First taste of 6502 Assembly
   - Hybrid BASIC+Assembly programs

3. **Assembly (ongoing)** — Deep dive into 6502 machine code
   - Direct hardware control
   - Professional game dev techniques
   - Performance optimization

---

## Repository Guide

### 📚 Core Repositories

#### [website](https://github.com/code198x/website)
The main educational platform built with Astro 5.14.1. All lesson content, interactive components, and documentation.

- **Tech**: Astro, MDX, TypeScript
- **URL**: https://code198x.stevehill.xyz
- **Content**: Lesson pages, tutorials, reference materials

#### [code-samples](https://github.com/code198x/code-samples)
All working code examples from every lesson. Organised by system and week.

- **Structure**: `/{system}/basic/week-{N}/lesson-{NN}/`
- **Format**: Ready-to-run programs (`.bas`, `.asm`, `.prg`)
- **Purpose**: Copy/paste code directly into emulators

#### [commodore-64-dev](https://github.com/code198x/commodore-64-dev)
Docker-based C64 development environment with ACME assembler, VICE emulator, and build tools.

- **Tech**: Docker, ACME, VICE
- **Usage**: Cross-platform C64 development setup
- **Purpose**: Write and test C64 code on modern systems

---

## Getting Started

### For Learners

**Complete beginners start here:**

1. Visit [code198x.stevehill.xyz](https://code198x.stevehill.xyz)
2. Choose **Commodore 64 → BASIC Course → Week 1**
3. Follow **Lesson 1: First Program**
4. Type code into an emulator (we recommend VICE)
5. See your first program run!

**Have programming experience?**

- Jump to Week 3 (Graphics & Sound) or Week 5 (Complete Mini-Games)
- Browse [code-samples](https://github.com/code198x/code-samples) to see what you'll build

### For Contributors

**Want to help improve lessons or add systems?**

1. Clone the [website](https://github.com/code198x/website) repository
2. Read `CLAUDE.md` for project structure
3. Check existing issues or propose new content
4. Follow the lesson template pattern from existing content

---

## Development Environment

### Quick Start (Docker)

```bash
# Clone the C64 dev environment
git clone https://github.com/code198x/commodore-64-dev.git
cd commodore-64-dev

# Start the environment
docker-compose up -d
docker-compose exec workspace bash

# You now have: ACME assembler, VICE emulator, build tools
```

### Local Website Development

```bash
# Clone and run the website
git clone https://github.com/code198x/website.git
cd website
npm install
npm run dev  # Starts dev server on localhost:4321
```

---

## Project Structure

### Content Organisation

**No phases, no tiers** — we dropped that complexity. Current structure:

```
Commodore 64
├── BASIC Course (8 weeks × 8 lessons = 64 lessons)
├── Transition Course (8 lessons)
└── Assembly Course (ongoing development)
```

Each lesson is self-contained:
- **Why** this concept matters
- **Basic Example** (5-10 lines)
- **Practical Example** (10-15 lines)
- **WOW Moment** (20-40 lines of impressive code)
- **Quick Reference** (syntax essentials)

### Code Sample Convention

```
code-samples/
└── commodore-64/
    └── basic/
        └── week-1/
            └── lesson-01/
                ├── basic.bas       # Simple demo
                ├── practical.bas   # Practical example
                └── main.bas        # The WOW moment
```

---

## Philosophy & Standards

### Language Guidelines

- **British English throughout** — all content written from UK perspective
- **Never use "mastery" terminology** — we're teaching, not claiming expertise
- **Beginner-friendly explanations** — assume zero prior knowledge
- **Show, don't tell** — working code beats paragraphs of theory

### Quality Standards

- ONE concept per lesson
- 15-20 minute completion time
- Immediately visible results
- Working code that runs first time
- No dependencies on previous lessons (except foundational Week 1)

### What We Avoid

- ❌ Academic jargon without context
- ❌ "Now try making your own..." without guidance
- ❌ Multi-hour tutorial marathons
- ❌ Textbook reference dumps
- ❌ Assuming prior programming knowledge

---

## Community & Support

- **Issues**: Report problems or suggest improvements in respective repositories
- **Discussions**: Use GitHub Discussions for questions and ideas
- **Contributing**: See individual repo CONTRIBUTING.md files
- **Website**: https://code198x.stevehill.xyz

---

## Technical Stack

### Website
- **Framework**: Astro 5.14.1 (static site generation)
- **Content**: MDX with frontmatter
- **Syntax Highlighting**: Prism.js with custom C64/Assembly support
- **Hosting**: Static deployment

### Development Tools
- **C64 Assembler**: ACME (cross-assembler)
- **Emulators**: VICE (C64), Fuse (ZX Spectrum)
- **Build System**: Docker containers with complete toolchains
- **CI/CD**: GitHub Actions

### Code Samples
- **C64 BASIC**: `.bas` files (BASIC V2 format)
- **C64 Assembly**: `.asm` source → `.prg` binaries
- **All platforms**: Ready-to-run programs included

---

## Project Status

### Active Development

- ✅ **C64 BASIC Course**: All 64 lessons complete
- 🚧 **C64 Assembly Course**: Week 1-2 in progress
- 🚧 **C64 Transition Course**: Planned
- 📋 **ZX Spectrum**: Planning phase
- 📋 **NES**: Planning phase
- 📋 **Amiga**: Planning phase

### Recent Milestones

- **January 2025**: Completed all 64 C64 BASIC lessons (weeks 1-8)
- **January 2025**: Established simplified course structure (dropped phases/tiers)
- **January 2025**: Extracted 192 working code samples

---

## Recognition

This project stands on the shoulders of:

- **Compute! Magazine** — inspiration for the "type-in program" format
- **VICE Team** — incredible C64 emulation
- **Retro gaming community** — keeping these systems alive
- **Original 8-bit developers** — showing us what's possible with limited hardware

---

**Start your retro game dev journey today:** [code198x.stevehill.xyz](https://code198x.stevehill.xyz)

*Because the best way to understand modern game development is to see how it was done when every byte mattered.*
