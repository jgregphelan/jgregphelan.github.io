# J. Greg Phelan — Editorial & Development Portfolio Website

## Project Summary

A clean, modern single-page portfolio website for J. Greg Phelan, positioning him for roles in
technical communication, editorial leadership, AI communication, and content strategy. The site
should feel like a blend of a literary portfolio, a thoughtful product/design page, and a
professional project archive. Tone: clear, understated, human, and credible.

## Tech Stack

- Vanilla HTML5, CSS3, JavaScript (no frameworks)
- Single HTML file with embedded or linked CSS
- No build tools or bundlers required
- Live Server (VS Code extension) for local development

## Key Commands

```bash
# Open in browser during development
# Right-click index.html → "Open with Live Server"
# Or: open index.html directly in any browser
```

## File Structure

```
/
├── index.html          # Single-page site — all content lives here
├── css/
│   └── styles.css      # All styles
├── js/
│   └── main.js         # Minimal JS (smooth scroll, sticky nav only)
└── assets/
    └── (images if needed)
```

## Design Specification

### Typography

```css
/* Headings, navigation, buttons, captions, metadata */
font-family: "Inter Tight", "Helvetica Neue", Arial, sans-serif;

/* Body text, essays, summaries, descriptions */
font-family: Charter, Georgia, "Times New Roman", serif;
```

### Color Palette

```css
--color-bg:         #fafaf8;   /* Warm off-white background */
--color-text:       #1a1a1a;   /* Charcoal / soft black */
--color-secondary:  #6b6b6b;   /* Muted gray for metadata/captions */
--color-accent:     #2a5caa;   /* Restrained blue for links, dividers, buttons */
--color-divider:    #e0ddd8;   /* Subtle section dividers */
```

### Layout Principles

- Generous white space and wide margins
- Max content width ~760px, centered
- Restrained, spacious, editorial feel
- No animations unless extremely subtle (e.g., nav transition on scroll)
- Strong contrast for accessibility (WCAG AA minimum)
- Fully mobile-responsive

## Page Structure & Section Order

Single-page with sticky top navigation linking to anchors:

1. `#hero`             — Name, tagline, optional hero summary
2. `#profile`          — Career narrative paragraph
3. `#unusually-suited` — Bulleted credential highlights
4. `#editorial`        — Project Write Now, book inc
5. `#technical`        — NYT articles, tech columnist, other publications
6. `#technology`       — Bell Labs, ePresence, charity: water
7. `#teaching`         — Monmouth University
8. `#ai`               — Current AI interests
9. `#education`        — Columbia, Bennington, U of Delaware
10. `#contact`         — Links / contact placeholder

## Navigation

- Sticky top nav with anchor links to all sections
- Use short nav labels (e.g., "Profile", "Editorial", "Technical", "Technology", "Teaching", "AI", "Education", "Contact")
- Simple, horizontal nav — no dropdowns

## Live Links

All links must be real, clickable hrefs. Use article/org titles as link text — never display raw URLs.

| Link Text | URL |
|---|---|
| Project Write Now | https://www.projectwritenow.org |
| For Student Essayists, An Automated Grader | https://www.nytimes.com/2003/09/04/technology/for-student-essayists-an-automated-grader.html |
| It's Got a Good Beat but Where's the Cover? | https://www.nytimes.com/2003/11/06/technology/it-s-got-a-good-beat-but-where-s-the-cover.html |
| He Helped Put the Blue in Blue Note | https://www.nytimes.com/2005/05/22/nyregion/he-helped-put-the-blue-in-blue-note.html |

All external links should open in a new tab (`target="_blank" rel="noopener"`).

## Coding Standards

- Semantic HTML elements throughout (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`)
- CSS custom properties (variables) for all colors and fonts
- Clean, readable, maintainable CSS — no utility-class frameworks
- Minimal JavaScript — only for sticky nav behavior and smooth scroll
- No animations beyond subtle nav transitions
- Accessible: proper heading hierarchy, alt text, sufficient color contrast
- No external dependencies beyond Google Fonts (Inter Tight)

## What to Avoid

- Corporate jargon or hype in copy
- Dense text blocks — preserve whitespace in layout
- Visual clutter or decorative elements
- Heavy animations or transitions
- Frameworks (React, Vue, Tailwind, Bootstrap)
- Displaying raw URLs as link text

## Footer

Include a simple footer with:
- Site title: "J. Greg Phelan Editorial & Development Portfolio"
- Email: jgregphelan@gmail.com
