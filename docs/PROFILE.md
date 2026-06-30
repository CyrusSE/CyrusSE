# CyrusSE — GitHub Profile README

This repository powers the GitHub profile page for [@CyrusSE](https://github.com/CyrusSE).

GitHub displays `README.md` from a **public** repository with the **same name as your username**.

## Files

| Path | Purpose |
|------|---------|
| `README.md` | Profile content shown on github.com/CyrusSE |
| `assets/header.svg` | Terminal-style banner (portfolio palette) |

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

**GitHub stats card (portfolio colors)**

```markdown
<img src="https://github-readme-stats.vercel.app/api?username=CyrusSE&show_icons=true&theme=transparent&bg_color=0a0c10&text_color=e8eaed&icon_color=c4f042&title_color=c4f042&border_color=2a3140" />
```

## Local preview

GitHub renders Markdown + HTML + SVG. Quick check:

```bash
# optional — any Markdown previewer works for structure; stats images need network
open README.md
```

For pixel-perfect review, push to a branch and view on GitHub.

## Notes

- `github-readme-stats` and `github-readme-streak-stats` are third-party services; cards load from external URLs.
- Private repo contributions appear in stats only when `count_private=true` (already set on the stats card).
- Profile README does **not** support custom CSS — use shields, HTML tables, `<details>`, and images.
