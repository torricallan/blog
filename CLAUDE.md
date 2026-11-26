# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Personal website for Torri Callan, a Senior Data Scientist focused on sports performance analytics. The site is a lean professional landing page (Home, Generative Periodisation, Research, Contact). Long-form writing lives on Substack (Generative Periodisation, https://generativeperiodisation.substack.com); the homepage's main call to action links there, and the Generative Periodisation tab (`writing.qmd`) uses copy from the Substack About page plus a short hand-picked list of Substack posts (edited directly in `writing.qmd`). Keep the homepage clean: no post lists there.

**Primary goal**: Establish credibility through thoughtful writing, not flashy design.

## Build Commands

```bash
# Preview with live reload
quarto preview

# Render the site
quarto render

# Render a single page
quarto render contact.qmd
```

## Site Structure

```
./
├── _quarto.yml          # Site configuration
├── custom.scss          # Theme (colors, typography)
├── styles.css           # Layout rules
├── index.qmd            # Landing page
├── writing.qmd          # Hand-picked links to Substack posts
├── research.qmd         # PhD thesis, publications, Google Scholar link
├── contact.qmd          # Contact page
└── posts/               # Archive of old posts (NOT rendered)
```

Only the pages listed under `project.render` in `_quarto.yml` are built. `posts/` is kept as an archive and is deliberately excluded; posts are not hosted on this site.

## Design Specifications

### Colour Palette

- **Background**: warm-white `#fffbeb`
- **Body text**: charcoal `#292524`
- **Links**: terracotta `#c2410c`
- **Accents**: muted-gold `#a16207`, muted-green `#059669`
- **Neutrals**: stone-grey `#78716c`, stone-light `#d6d3d1`

### Typography

- **Headings**: Inter (sans-serif)
- **Body**: Source Serif 4 (serif)
- **Code**: JetBrains Mono (monospace)
- **Body size**: 18px, line-height 1.65

### Layout

- **Article width**: 700px max (set via `format.html.grid.body-width` in `_quarto.yml`)
- **Navigation**: Minimal horizontal (Home | Generative Periodisation | Research | Contact), with the name as the navbar brand
- **Links**: terracotta with a faint stone-light underline that darkens on hover
- **Palette variables**: defined at the top of `custom.scss`; use them rather than raw hex values

### Design Principles

- Prioritise simplicity; when in doubt, leave it out
- Generous whitespace
- No gradients, drop shadows, stock photography, or clever animations
- No sidebar clutter, category clouds, or prominent social icons

## Notes for Claude Code

- Test locally with `quarto preview` before committing
- Commit frequently with clear messages
- Ask before adding dependencies or complexity
- Reference this file when making design decisions
