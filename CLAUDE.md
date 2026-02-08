# CLAUDE.md — peptation-website

## Project

Static HTML/CSS template site for PEPTATION, a luxury GHK-Cu hair growth serum brand. Templates are designed for conversion to WooCommerce theme files.

## Tech Stack

- Pure HTML5 / CSS3 (no framework, no build tools)
- Vanilla JavaScript for interactive components
- CSS custom properties for theming (`assets/css/variables.css`)
- Google Fonts: Playfair Display (headlines) + Inter (body)

## Key Paths

- `templates/pages/` — Core website pages (index, shop, product, how-it-works, contact)
- `templates/woo-templates/` — WooCommerce-ready templates (cart, checkout)
- `assets/css/main.css` — Full stylesheet
- `assets/css/variables.css` — CSS design tokens
- `assets/images/` — Product and brand images

## How to Preview

```bash
cd /root/projects/peptation-website
python3 -m http.server 8000
# Visit: http://localhost:8000/templates/pages/index.html
```

Or open any HTML file directly in a browser.

## Design System

- **Color Scheme:** Minimal Prestige (Black/Gold/White)
- **Primary:** Deep Navy #1A1A2E, Gold #C9A227
- **Typography:** Playfair Display (headings), Inter (body)

## Rules

- No build tools — keep it pure static HTML/CSS
- Use CSS custom properties from `variables.css` for all colors and spacing
- Maintain mobile-responsive design across all templates
- WooCommerce templates in `woo-templates/` should stay conversion-ready
- Reference `ARCHITECTURE.md` for detailed design specs
