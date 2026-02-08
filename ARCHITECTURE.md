# Site Architecture & Design Direction
**Project:** PEPTATION - Hair Regrowth E-Commerce Site (WordPress + WooCommerce)  
**Brand:** Peptation  
**Reference:** Fleava.shop  
**Created:** 2026-02-06  
**Status:** 🟡 Awaiting Approval

---

## 🏷️ Brand Identity

**Name:** PEPTATION  
**Logo:** White serif text on black (wide letter-spacing, elegant)  
**Color Direction:** Option C - Minimal Prestige (Black/White/Gold)

---

## 📋 Overview

Building a luxury, high-end hair regrowth product website. Similar product line to Fleava but with elevated design—beautiful, polished, premium feel.

---

## 🏗️ Site Structure

### Core Pages (Custom HTML Templates)

| Page | Purpose | Priority |
|------|---------|----------|
| **Homepage** | Hero, value props, testimonials, science, products, FAQ | 🔴 High |
| **Shop/Collection** | Product grid with filters | 🔴 High |
| **Product Page** | Single product detail, gallery, tabs, reviews | 🔴 High |
| **How It Works** | Science/ingredients deep-dive | 🟡 Medium |
| **About Us** | Brand story, mission | 🟡 Medium |
| **Contact** | Form, support info | 🟡 Medium |
| **FAQ** | Standalone FAQ page | 🟢 Low |

### WooCommerce Template Overrides

| Template | Description |
|----------|-------------|
| `cart.php` | Shopping cart page |
| `checkout.php` | Checkout flow |
| `my-account.php` | Customer dashboard |
| `order-confirmation.php` | Thank you / order summary |
| `single-product.php` | Product detail (if not custom) |
| `archive-product.php` | Shop/collection grid |

---

## 🛍️ Product Line (Based on Reference)

| Product | Type | Notes |
|---------|------|-------|
| **Hair Regrowth Serum** | Main product | Copper peptide formula, hero SKU |
| **Shampoo** | Complementary | Mentioned in FAQ |
| **Conditioner** | Complementary | Mentioned in FAQ |
| **Supplements** | Complementary | Oral supplements for hair health |
| **Bundle/Kit** | Upsell | Complete system package |

**Pricing Strategy (Fleava reference):**
- Single: $59 (was $89)
- Buy 2: Better per-unit
- Buy 3: Best value
- Subscription: Monthly delivery option

---

## 🎨 Design Direction

### Vibe
**Luxury. Clinical. Trustworthy. Elevated.**

Think: Aesop meets medical aesthetics. Clean, premium, sophisticated—not cheap DTC vibes.

### Problems with Fleava's Design
- Generic stock imagery
- Inconsistent spacing
- Cluttered sections
- Typical "dropship" aesthetic
- Too many competing CTAs

### Our Approach
- **Generous whitespace** — let elements breathe
- **Refined typography** — elegant serifs for headlines, clean sans for body
- **Subtle animations** — smooth reveals, tasteful micro-interactions
- **Photography-forward** — high-quality product shots, real textures
- **Restrained color** — sophisticated palette, not shouty

---

## 🎨 Color Scheme Options

### Option A: "Clinical Luxury" (Recommended)
```
Primary:      #1A1A2E (Deep Navy/Black)
Secondary:    #C9A959 (Warm Gold)
Accent:       #4A6FA5 (Muted Steel Blue)
Background:   #FAFAFA (Off-White)
Surface:      #FFFFFF (Pure White)
Text:         #1A1A2E (Primary)
Text Muted:   #6B7280 (Gray)
Success:      #2D5A4A (Forest Green)
```
**Vibe:** Sophisticated, gender-neutral, premium skincare feel

### Option B: "Modern Apothecary"
```
Primary:      #2C3E2D (Deep Forest)
Secondary:    #D4AF37 (Classic Gold)
Accent:       #8B7355 (Warm Bronze)
Background:   #F5F3EF (Warm Cream)
Surface:      #FFFFFF
Text:         #1F2421 (Near Black)
Text Muted:   #5C5C5C
Success:      #3D5A3D (Sage)
```
**Vibe:** Natural, botanical, heritage brand feel

### Option C: "Minimal Prestige"
```
Primary:      #000000 (Pure Black)
Secondary:    #B8860B (Dark Gold)
Accent:       #1C1C1C (Soft Black)
Background:   #FFFFFF (Pure White)
Surface:      #F8F8F8 (Light Gray)
Text:         #000000
Text Muted:   #757575
Success:      #006400 (Dark Green)
```
**Vibe:** High contrast, bold, Apple-esque minimalism

---

## 📐 Typography Recommendation

### Headlines
**Playfair Display** or **Cormorant Garamond**
- Elegant serif with personality
- Used sparingly for major headings

### Body / UI
**Inter** or **DM Sans**
- Clean, highly readable
- Modern but not cold

### Example Pairing
```css
--font-display: 'Playfair Display', Georgia, serif;
--font-body: 'Inter', -apple-system, sans-serif;
```

---

## 🧩 Component Library (To Build)

### Global
- [ ] Header/Navigation
- [ ] Footer
- [ ] Button styles (primary, secondary, outline, ghost)
- [ ] Form inputs
- [ ] Cards
- [ ] Modal/Drawer

### Homepage Sections
- [ ] Hero with video/image background
- [ ] Trust badges / social proof bar
- [ ] Benefits grid (icons + text)
- [ ] Testimonial carousel
- [ ] Science/ingredients showcase
- [ ] Product feature cards
- [ ] Comparison table
- [ ] FAQ accordion
- [ ] CTA banner

### Product Page
- [ ] Image gallery with zoom
- [ ] Product info (title, price, variants)
- [ ] Add to cart with quantity
- [ ] Tabs (How to use, Ingredients, Reviews)
- [ ] Related products
- [ ] Reviews section

### WooCommerce
- [ ] Cart summary
- [ ] Checkout form styling
- [ ] Order confirmation
- [ ] Account pages

---

## 📁 File Structure

```
/templates
  /pages
    index.html          # Homepage
    shop.html           # Product collection
    product.html        # Single product
    how-it-works.html   # Science page
    about.html          # About us
    contact.html        # Contact
    faq.html            # FAQ standalone
  /woo-templates
    cart.html           # Cart page
    checkout.html       # Checkout
    my-account.html     # Account dashboard
    order-confirm.html  # Thank you
  /components
    header.html
    footer.html
    hero.html
    testimonials.html
    benefits.html
    faq-accordion.html
    product-card.html
    ...
/assets
  /css
    main.css            # Compiled styles
    variables.css       # Design tokens
  /js
    main.js
  /images
    (placeholder images)
```

---

## ❓ Questions Before Building

1. **Color scheme preference?** (A, B, C, or custom direction?)
2. **Brand name?** (Need for logo placeholder, copy)
3. **Product names?** (Or should I create placeholder names?)
4. **Any specific features** beyond what Fleava has?
5. **Mobile-first or desktop-first?** (I'd recommend mobile-first)
6. **Do you have product images**, or should I use placeholders?

---

## ✅ Next Steps (After Approval)

1. Finalize color scheme and typography
2. Build CSS framework / design tokens
3. Create component library
4. Build homepage first (main template)
5. Product page template
6. Shop/collection template
7. WooCommerce templates
8. Polish and responsive testing

---

*Ready when you are. Hit me with your color preference and any changes to the structure.*
