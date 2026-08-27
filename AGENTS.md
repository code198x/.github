# Code198x — org container

> Read [`PRINCIPLES.md`](PRINCIPLES.md) first.

Code198x is the curriculum, website, pattern-library, code-sample, platform-dev, and publishing sibling in the 198x family.

## Umbrella context

This folder is the org container for the `code198x` GitHub organisation. It is not a Git repo; each child folder is an independent repo with its own remote. Commit inside the repo that owns the file.

The umbrella context is [`../CLAUDE.md`](../CLAUDE.md); cross-project decisions live in [`../decisions/`](../decisions/). Hardware facts cite the 198x source-of-truth layers rather than becoming canonical inside curriculum docs.

## Current launch context

October 2026 is the public launch target. The launch surface is the four core platforms, each with a complete on-ramp at the current Definition of Done bar:

- ZX Spectrum
- Commodore 64
- Commodore Amiga
- Nintendo Entertainment System

Current shipped/planned state lives in the website module catalogues and git, not in prose trackers. Code198x decisions explain the rationale.

## Working rules

- Work inside the child repo that owns the change.
- Check the relevant child repo status before committing.
- Keep code samples in `code-samples/`; curriculum pages include them through `CodeFromFile`.
- Use British English, except use “program” for computer programs.
- Verify screenshots and captures before using them in public-facing content.
- Treat hardware facts as derived from `reference/`, `syntheses/`, and Emu198x knowledge; do not make curriculum docs the first canonical home of hardware facts.

## Repos in this org

| Repo | Purpose |
|---|---|
| `website/` | Astro site serving the curriculum, Pattern Library, Vault, and project pages. |
| `docs/` | Curriculum specifications, platform references, decisions, and content workflow docs. |
| `code-samples/` | Working code used by curriculum units. |
| `scripts/` | Shared Code198x helper scripts. |
| `.github/` | Org profile, health files, and this org-container context. |
| `substack-drafts/` | Code198x Substack/article drafts. |
| `commodore-amiga-dev/` | Amiga development container. Still the Amiga build path. |

## Active tooling paths

| Platform | Build path | Output |
|---|---|---|
| ZX Spectrum | Asm198x native assembler | `.sna` and related Spectrum outputs |
| C64 | Asm198x native assembler | `.prg` |
| Amiga | `commodore-amiga-dev/` Docker tooling (vasm) | executable |
| NES | Asm198x native assembler | `.nes` |

Capture work should use the current documented capture path for the target repo/platform. Cross-project migration rationale lives in [`../decisions/code198x-dev-tooling-migration.md`](../decisions/code198x-dev-tooling-migration.md).

## Key docs

- `docs/index.md` — Code198x docs navigation.
- `docs/decisions/` — Code198x binding decisions.
- `docs/specifications/` — curriculum, unit, brief, Vault, Pattern Library, content model, and voice specs.
- `docs/platforms/` — per-platform reference and curriculum framing.
- `docs/infrastructure/` — capture pipeline and Astro site notes.

For cross-project work, start from the umbrella [`../README.md`](../README.md) and [`../docs/start-here.md`](../docs/start-here.md).
