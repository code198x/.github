# Code198x — org container

> Read [`PRINCIPLES.md`](.github/PRINCIPLES.md) first. [`MANIFESTO.md`](.github/MANIFESTO.md) is why the project exists.

Code198x develops the games development and programming curriculum, website, Pattern Library, Vault and code samples. Read [the project charter](https://github.com/code198x/docs/blob/main/PROJECT.md) for current goals and [the documentation index](https://github.com/code198x/docs/blob/main/README.md) for authoring guidance.

## Umbrella context

This folder is the org container for the `code198x` GitHub organisation. It is not a Git repo; each child folder is an independent repo with its own remote. Commit inside the repo that owns the file.

Family principles govern cross-project work. Code198x specifications apply the current charter; previous reasoning remains in Git history. Cite original hardware sources precisely rather than treating curriculum prose as hardware authority.

## Current launch context

October 2026 is the public launch target. The launch surface is the four core platforms, each with a complete on-ramp at the current Definition of Done bar:

- ZX Spectrum
- Commodore 64
- Commodore Amiga
- Nintendo Entertainment System

Current shipped/planned state lives in the website catalogues, authored lessons, samples and Git. October is planning context, not a claim of completion. The immediate curriculum focus is re-specifying Spectrum BASIC and assembly as independent entry points; new game sequences remain proposals until agreed. BASIC games need not meet commercial standards: quality is relative to the agreed scope.

## Working rules

- Work inside the child repo that owns the change.
- Check the relevant child repo status before committing.
- Keep code samples in `code-samples/`; curriculum pages include them through `CodeFromFile`.
- Use British English, except use “program” for computer programs.
- Verify screenshots and captures before using them in public-facing content.
- Distinguish proposals, source-checked claims, builds and configuration-specific execution evidence.
- Public content and repositories must not mention private collections or local library paths; cite original sources or public pages directly.

## Repos in this org

| Repo | Purpose |
|---|---|
| `website/` | Astro site serving the curriculum, Pattern Library, Vault, and project pages. |
| `docs/` | Current project goals, curriculum specifications, system design material and workflow guidance. |
| `code-samples/` | Working code used by curriculum units. |
| `scripts/` | Shared Code198x helper scripts. |
| `.github/` | Org profile, health files, and this org-container context. |
| `substack-drafts/` | Code198x Substack/article drafts. |

## Active tooling paths

| Platform | Build path | Output |
|---|---|---|
| ZX Spectrum | Asm198x native assembler | `.sna` and related Spectrum outputs |
| C64 | Asm198x native assembler | `.prg` |
| Amiga | Asm198x native assembler, mastered by Build198x | bootable `.adf` |
| NES | Asm198x native assembler | `.nes` |

Capture work should use the current documented capture path for the target repo/platform. Cross-project migration rationale lives in [`../decisions/code198x-dev-tooling-migration.md`](../decisions/code198x-dev-tooling-migration.md).

## Key docs

- `docs/README.md` — Code198x docs navigation.
- `docs/PROJECT.md` — current Code198x goals and direction; update this and the relevant specification when intent changes.
- `docs/specifications/` — curriculum, unit, brief, Vault, Pattern Library, assets, pseudocode and voice specs.
- `docs/platforms/` — retained game designs and prototype investigations for review.
- `docs/website.md` — website, sources, capture, validation and publishing workflow.
- `docs/work.md` — current bounded tasks and component proposals.

For cross-project work, start from the umbrella [`../README.md`](../README.md) and [`../docs/start-here.md`](../docs/start-here.md).
