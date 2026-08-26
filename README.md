# Lev Family Health — Design System

A design-system bundle for **claude.ai/design**, and the versioned source of truth for Lev's
visual identity.

Open `reference/index.html` in a browser for the whole system on one page.

Colour and logo values are read from the master vector file (`Lev logos.ai`, 1 Jul 2026) — that
file is the authority. Type, scale, spacing and component patterns are measured off the
Ready Ads library. Fonts are licensed to JAM.

Compiled August 2026 · JAM Strategic Communications.

---

## What's in here

```
tokens.css                        canonical token source — colour, type, spacing, radii, layout
foundations/color.html            palette, sub-brand grounds, pairing rules
foundations/typography.html       Martina Plantijn + Graphik, full scale
foundations/logo.html             nine lockups, four marks, clear space, naming rules
foundations/shapes.html           quarter arc, square, chevron
foundations/layout-spacing.html   page architecture, 8pt scale, the closing band
components/service-chips.html     four services, four grounds, three states
components/headline-block.html    eyebrow → display headline → standfirst
components/action-cards.html      stacked instruction blocks
components/location-block.html    Pomona and Monsey
components/hours-table.html       divided columns, community calendar
components/photo-frame.html       image plus opposing shape accents
components/testimonial-card.html  Lev Listens
components/footer-band.html       the navy band that ends every piece
subbrands/womens-health.html      blush ground, magenta accent, pill service list
assets/                           13 vector lockups and marks, SVG
assets/source/                    the master Lev logos.ai — authority for colour and logo
reference/index.html              the whole system as one self-contained page
docs/                             the Brand Guidelines deck
```

Every preview file is standalone HTML with its tokens inlined, and carries a first-line
`<!-- @dsCard group="…" name="…" subtitle="…" -->` marker so the Design System pane builds its
card index automatically.

---

## Loading it into Claude Design

This bundle was built outside an authorised Claude Design session, so it has not been pushed
yet. Two ways in:

**A. From a Claude Design session.** Open the Lev design-system project at claude.ai/design and
use *Send to Claude Code Web*. That seeds the project into the workspace with design-system
authorisation, and the bundle can be pushed straight in.

**B. From a terminal Claude Code session.** Run `/design-login`, then `/design-sync` pointed at
this folder. Files are pushed incrementally, one component at a time — never as a wholesale
replace.

Either way the target project must be created as a **design-system** project. That type is
fixed at creation; pushing into a regular project will not convert it.

---

## One open item

**A "Lev Health" descender is running in produced work and is not in the master file.** The
logo suite carries two descenders — *Family Health* and *Women's Health*. Several ads in the
Ready Ads folder close with a shortened *Lev Health* lockup, and at least one closes with the
wordmark alone. Either the short lockup is added to the master file as a sanctioned tenth, or
the ads are corrected to *Lev Family Health*. It should not stay in both states.

## Fonts

Graphik (Commercial Type) and Martina Plantijn (Klim) are licensed to JAM. The previews in this
bundle fall back to Figtree and Spectral so they render anywhere — install the licensed files
for anything that ships.
