# PEPTATION Website Templates

Luxury e-commerce website templates for Peptation — a GHK-Cu hair growth serum brand.

## Brand

- **Name:** PEPTATION
- **Product:** GHK-Cu Hair Growth Serum (30ml)
- **Color Scheme:** Deep Navy (#1A1A2E) + Gold (#C9A227) + White
- **Typography:** Playfair Display (display) + Inter (body)

## File Structure

```
peptation-website/
├── ARCHITECTURE.md              # Design specs, color palette, structure
├── README.md                    # This file
├── assets/
│   ├── css/
│   │   ├── main.css             # Full stylesheet (17KB)
│   │   └── variables.css        # CSS custom properties
│   └── images/
│       ├── logo-peptation.png   # Brand logo
│       ├── product-bottle-box.jpg
│       ├── product-box-angle.jpg
│       └── product-box-front.jpg
└── templates/
    ├── pages/
    │   ├── index.html           # Homepage
    │   ├── shop.html            # Product collection
    │   ├── product.html         # Single product page
    │   ├── how-it-works.html    # Science/ingredients deep-dive
    │   └── contact.html         # Contact form + info
    └── woo-templates/
        ├── cart.html            # Shopping cart
        └── checkout.html        # Checkout flow
```

## Pages

| Page | Description | Status |
|------|-------------|--------|
| Homepage | Hero, benefits, products, science, testimonials, FAQ | ✅ Complete |
| Shop | Filterable product grid, single product + placeholders | ✅ Complete |
| Product | Gallery, quantity selector, tabs, reviews | ✅ Complete |
| How It Works | Science explanation, timeline, research, comparison | ✅ Complete |
| Contact | Contact form, support info, FAQ preview | ✅ Complete |
| Cart | Cart items, upsell, promo codes, summary | ✅ Complete |
| Checkout | Multi-step form, payment, order summary | ✅ Complete |

## Key Features

- **Mobile-responsive** — All pages work on mobile
- **CSS Custom Properties** — Easy theme customization via variables.css
- **Interactive elements** — FAQ accordion, gallery, tabs, filters
- **Trust signals** — Guarantee badges, shipping info, security notices
- **Upsell components** — Cart upsells, quantity bundles
- **Placeholder-ready** — Easy to swap images for real product shots

## WordPress/WooCommerce Integration

Templates in `/woo-templates/` are styled mockups ready to be converted to WooCommerce theme templates:

- `cart.html` → `woocommerce/cart/cart.php`
- `checkout.html` → `woocommerce/checkout/form-checkout.php`

The CSS framework (`main.css`) can be enqueued in your theme to maintain consistent styling.

## Preview

Open any HTML file directly in a browser to preview. For best results:

```bash
cd ~/projects/peptation-website
python3 -m http.server 8000
# Then visit http://localhost:8000/templates/pages/index.html
```

## Next Steps

- [ ] Add real product photography (white background, lifestyle shots)
- [ ] Connect to WooCommerce
- [ ] Add email capture / newsletter signup
- [ ] Implement progress tracker feature
- [ ] Add video testimonials section
- [ ] SEO meta tags optimization
- [ ] Add legal pages (Privacy, Terms, Refund Policy)

---

Built by Burek 🥟 | February 2026
