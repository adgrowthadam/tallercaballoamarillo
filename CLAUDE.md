# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Landing page for **Taller Caballo Amarillo** — a music and art academy in Veracruz, México. Built by AdGrowth Agency. Goal: lead generation via a free first session offer.

Always read `copy.txt` before writing any code — all Spanish-language copy for every section lives there.

## Output

- **Single file**: `index.html` with all CSS and JS embedded (no separate files)
- **No external frameworks or libraries** — Google Fonts is the only allowed external resource

## Images

- All images go in `/images/` folder (not available yet — use solid color placeholders)
- Above each image tag, leave a comment describing what it will be and any effect, e.g.:
  ```html
  <!-- IMAGE: images/hero.jpg | Effect: B&W + dark fade overlay -->
  ```
- Never use picsum, unsplash, or any external image service

## Page Structure (sections in order)

1. **Hero** — headline, subheadline, CTA button (scrolls to form)
2. **About** — short paragraph about the academy
3. **What we offer** — 3 or 4 cards
4. **Benefits** — icons + short text
5. **Form** — empty `<div id="ghl-form">` with comment `<!-- GHL embed goes here -->`
6. **Footer** — name, location, social placeholders

> The full copywriting (including FAQ, disciplines, teachers, and CTA sections) is in `copy.txt`. Map that content into the sections above.

## Design System

**Colors** (use CSS variables for all):
- `--primary: #F2B705`
- `--orange-mid: #F29F05`
- `--orange-deep: #F28705`
- `--red-orange: #F24405`
- `--text: #FFFFFF` (all text in white)

**Typography**: Google Fonts — **Montserrat** for all text (headings, body, buttons, everything)

**Style**: warm, creative, artistic but professional. Language: Spanish.

## Technical Requirements

- Mobile-first, fully responsive
- Smooth scroll behavior
- Scroll animations via Intersection Observer (no libraries)
- CSS variables for all colors and fonts
- Clean, well-commented code
- **Form**: `<div id="ghl-form">` — GHL embed placeholder (no native form submission)
- **Meta Pixel**: fire `Lead` event when the form area is interacted with
- CTA button repeated in Hero, after disciplines/offers section, and in final CTA

## Pending Client Content

Before going live:
- Teacher names, photos, and bios (violin + painting)
- Official WhatsApp number
- Available schedules by discipline
- Real class photos
- Exact address within Colonia Florista, Veracruz
