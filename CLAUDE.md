# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Personal website for Torri Callan, a Senior Data Scientist focused on sports performance analytics. The site serves as a professional presence and hosts long-form writing on data science and sports periodisation.

**Primary goal**: Establish credibility through thoughtful writing, not flashy design.

## Build Commands

```bash
# Preview with live reload
quarto preview

# Render the site
quarto render

# Render a single post
quarto render posts/periodisation-statistical-modelling.qmd
```

## Site Structure

```
./
├── _quarto.yml          # Site configuration
├── custom.scss          # Theme (colors, typography)
├── styles.css           # Layout rules
├── index.qmd            # Landing page
├── writing.qmd          # Blog listing
├── about.qmd            # About page
├── contact.qmd          # Contact page
└── posts/               # Blog posts
```

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

- **Article width**: 700px max
- **Wide figures**: 950px max (for visualisations)
- **Navigation**: Minimal horizontal (Home | Writing | About | Contact)

### Design Principles

- Prioritise simplicity; when in doubt, leave it out
- Generous whitespace
- No gradients, drop shadows, stock photography, or clever animations
- No sidebar clutter, category clouds, or prominent social icons

## Blog Post Template

```markdown
---
title: "Post Title"
author: "Torri Callan"
date: YYYY-MM-DD
categories: [category1, category2]
description: "One or two sentence description for the listing page."
draft: false
---

Content here...
```

## Notes for Claude Code

- Test locally with `quarto preview` before committing
- Commit frequently with clear messages
- Ask before adding dependencies or complexity
- Reference this file when making design decisions
