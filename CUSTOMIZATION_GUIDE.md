# Reem Jawad Horizon Theme Customization Guide

## GitHub Repository
**URL**: https://github.com/HIS-AliKarasneh/reem-jawad-horizon-theme

## How to Connect to Shopify
1. Go to **Shopify Admin > Online Store > Themes**
2. Click **Add theme > Connect from GitHub**
3. Select `HIS-AliKarasneh/reem-jawad-horizon-theme` repository
4. Choose `main` branch
5. Click **Connect**

---

## Design Analysis - What Needs to Change

### Brand Colors (Theme Editor Settings)
| Element | Current (Horizon Default) | Target (Reem Jawad) |
|---------|---------------------------|---------------------|
| Background | `#FFFFFF` | `#FAFAFA` (off-white) |
| Primary Accent | `#000F9F` (blue) | `#C9A962` (gold) |
| Text/Headings | `#000000` | `#1A1A1A` (soft black) |
| Buttons | Blue | Gold `#C9A962` with black text |
| Borders | `#E6E6E6` | `#E5E5E5` |

### Typography (Theme Editor Settings)
| Element | Target Font |
|---------|-------------|
| Headings | Playfair Display or similar serif |
| Body | Work Sans (Horizon default is fine) |
| Accent | Italic serif for "Grace", "Stitch" style text |

---

## Page-by-Page Customizations

### Homepage
- Hero section with beach/elegant image
- "COLLECTIONS" grid (3 cards)
- "ITEMS ON SALE" product row
- Second Collections section
- Instagram Feed section

### Store/Collection Page
- Banner with "The Summer Collection"
- Category tabs
- Color swatch filters
- Product grid 4-column
- "Load More Products" button

### Product Page
- Thumbnail gallery + main image
- Title, price, color swatches, size selector
- Quantity selector + Add to Cart
- Wishlist heart icon
- Accordion: Product Features, Shipping, Care
- "Complete the Look" recommendations

### About Page (Custom Template Needed)
- Hero banner "Our Story of Grace"
- Alternating image/text sections
- Core Values 3-column grid
- Testimonial section
- Instagram Feed

### Contact Page
- Header banner "Get in Touch"
- 2-column: Form left, Contact Info right
- Instagram Feed footer

### Cart Page
- "Your Shopping Bag" layout
- Order Summary sidebar
- "Complete the Look" recommendations

---

## Required Custom Work

1. **Arabic Locale (RTL Support)** - Create `locales/ar.json`
2. **Custom About Page Template** - Create `templates/page.about.json`
3. **Instagram Feed Section** - Use app or create custom section
4. **Color Scheme Updates** - Update settings with gold/black palette

---

## Quick Start

```bash
# Install Shopify CLI
npm install -g @shopify/cli

# Preview theme
shopify theme dev --store your-store.myshopify.com
```