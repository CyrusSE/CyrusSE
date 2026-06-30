# CyrusSE — GitHub Profile README

This repository powers the GitHub profile page for [@CyrusSE](https://github.com/CyrusSE).

GitHub displays `README.md` from a **public** repository with the **same name as your username**.

## Files

| Path | Purpose |
|------|---------|
| `README.md` | Profile content shown on github.com/CyrusSE |
| `assets/header.svg` | Terminal-style banner (portfolio palette) |
| `assets/badge-linkedin.svg` | LinkedIn badge (shields.io dropped linkedin icon) |
| `assets/badge-linkedin-flat.svg` | Flat LinkedIn badge for connect row |

## Design system

Matched to the [Portofolio](https://github.com/CyrusSE/Portofolio) site:

| Token | Value | Usage |
|-------|-------|--------|
| void | `#0a0c10` | Background |
| text | `#e8eaed` | Primary copy |
| muted | `#8b93a7` | Secondary copy |
| flag | `#c4f042` | Accent / highlights |
| grid | `#2a3140` | Borders |

## Updating content

1. Edit `README.md` for copy, stats, projects, and badges.
2. Keep counts in sync with `Portofolio/src/data/profile.ts` when portfolio data changes.
3. Commit to `main` — profile updates within a few minutes.

### Useful snippets

**Portfolio badge**

```markdown
[![Portfolio](https://img.shields.io/badge/portfolio-Portofolio-c4f042?style=for-the-badge&labelColor=0a0c10&logo=github&logoColor=c4f042)](https://github.com/CyrusSE/Portofolio)
```

**LinkedIn badge** (local — shields.io no longer embeds `logo=linkedin`)

```markdown
[![LinkedIn](./assets/badge-linkedin.svg)](https://linkedin.com/in/faisalsan)
```

**GitHub stats** (`github-readme-stats.vercel.app` often 503 — use summary cards)

```markdown
<img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=CyrusSE&theme=github_dark" alt="GitHub stats" />
<img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=CyrusSE&theme=github_dark" alt="Top languages" />
<img src="https://streak-stats.demolab.com/?user=CyrusSE&theme=dark&background=0a0c10&border=2a3140&ring=c4f042&fire=c4f042&currStreakLabel=c4f042" alt="GitHub streak" />
```

## Local preview

GitHub renders Markdown + HTML + SVG. Quick check:

```bash
# optional — any Markdown previewer works for structure; stats images need network
open README.md
```

For pixel-perfect review, push to a branch and view on GitHub.

## Notes

- Stats use `github-profile-summary-cards` + `streak-stats.demolab.com` (rickstaa/vercel stats often down).
- LinkedIn shields use repo SVGs; `logo=linkedin` no longer renders on img.shields.io.
- Profile README does **not** support custom CSS — use shields, HTML tables, `<details>`, and images.
