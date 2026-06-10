# AGENTS.md — Lucy's AI Image Vault (Public Release Repo)

## What this repo is

This is the **public GitHub release repository** for Lucy's AI Image Vault — a cross-platform desktop app that helps Artistly.ai users archive, organize, and sync their AI-generated images locally before Artistly's 1-year auto-deletion removes them.

**Audience:** End users downloading the app. There is one active developer (Ed). External open-source contributors are possible in the future.

This is **not** the private dev repo. There are no internal planning docs, session notes, or in-progress experiments here.

---

## What Codex should help with

- **User-facing documentation** — writing and editing README.md, Lucys_AI_Image_Vault_Quick_Start_Guide, and any future feature docs
- **GitHub release notes and changelogs** — drafting release descriptions, version history entries
- **GitHub issues** — triaging bug reports and feature requests, drafting responses to users
- **External contributor PRs** — reviewing contributions for accuracy and consistency with the existing docs and project tone
- **Keeping docs in sync** — updating documentation when app behavior changes

---

## What Codex should avoid

- Referencing the private dev repo or any internal session notes, planning docs, or experiments
- Adding developer-facing architecture detail beyond what is already in the public docs
- Assuming the user wants debug or dev-workflow help — for those tasks, Ed uses a separate private dev repo
- Inventing internal implementation details that aren't documented here

---

## Repository contents

| File / Folder | Purpose |
|---|---|
| `README.md` | Main landing page |
| `VaultIcon.png` | App icon used in README.md header |
| `docs/Lucys_AI_Image_Vault_Quick_Start_Guide.md` | User-facing setup and first-run guide |
| `docs/` | PDF and plain-text versions of user docs + Feature Documentation draft |
| `docs/README_FIRST.txt` | Plain-text setup guide bundled with downloads |
| `docs/Lucys_AI_Image_Vault_Quick_Start_Guide.pdf` | PDF version of the setup guide |
| `docs/Lucys AI Image Vault - Feature Documentation.md` | Detailed feature reference (draft, work in progress) |
| `docs/Lucys AI Image Vault - Feature Documentation.pdf` | PDF version of the feature docs |
| `docs/Playwright_Explainer.pdf` | Plain-language explanation of how cloud sync works |
| `docs/Tech_Stack_Explainer.pdf` | Overview of the app's technology for curious users |
| `screenshots/` | Screenshots and GIFs used in docs (populated before each release) |
| Release binaries | Distributed via GitHub Releases — not committed to the repo |

## Release bundle contents (Windows ZIP / macOS DMG)

Each release package should include only:

- App binary (`LucysVault.exe` or `LucysVault.app`)
- `README_FIRST.txt`
- `Lucys_AI_Image_Vault_Quick_Start_Guide.pdf`
- `LICENSE`

Keep bundles lean. The Feature Documentation PDF, Playwright Explainer, and Tech Stack Explainer live on GitHub — do not bundle them. The Quick Start Guide PDF covers everything a user needs to get started offline.

---

## Tech stack (for accurate documentation assistance)

- **Desktop shell:** FastAPI backend + pywebview window
- **Frontend:** React 18 SPA compiled into a single `index.html` (no build step)
- **Database:** SQLite
- **Cloud sync automation:** Playwright (controls a bundled browser to log into Artistly)
- **Packaging:** PyInstaller, targeting Windows `.exe` and macOS `.app`
- **Utility scripts:** Python scripts for cloud sync, bulk operations, and DB maintenance

Keep documentation descriptions at the user level — "the app opens a browser window and connects to your Artistly account" is more appropriate than "Playwright drives a Chromium instance."

---

## Writing style for docs

- Warm, plain-language tone — users are creative people, not necessarily technical
- Use emoji sparingly and only where they already appear in existing docs (step headers, warnings)
- Warnings about data safety (cloud sync trap, vault location choice) should stay prominent — users have lost data from ignoring them
- Platform-specific callouts (Windows vs. Mac, macOS Gatekeeper) are important and should be preserved
