# Import AVISHEKK NAIYA and add category shopping flow

## What the repository contains
- A TanStack Start catalogue page at `/` with the approved AVISHEKK NAIYA header, eight category cards, responsive two/four-column layout, and eight bundled 4:5 images.
- The visual system uses Cormorant Garamond headings, Manrope body text, an ivory background, black header, gold/brown accents, compact borders, and restrained hover motion.
- The current source has no product records, API, database, footer, category routes, or product-detail page. Its category cards are visual only.

## Implementation
1. Import the inspected repository into this project at its current public commit, preserving the existing home page, logo, assets, typography, colors, spacing, animations, and responsive behavior.
2. Extract the existing header into a shared component without changing its appearance, so home, collection, and product pages use the same navigation.
3. Make every existing category card a full-card link to `/collections/$category`, with the exact eight requested category slugs.
4. Add a structured local product catalogue keyed by category because the repository contains no product dataset or API. Include product names, descriptions, prices, discounts, badges, sizes, fabrics, colors, occasions, craft, availability, and reusable category imagery.
5. Build the dynamic collection page with category-aware metadata, breadcrumb, title, description, search, relevant tabs, functional filter groups, clear-all action, dynamic product count, sorting, and grid/list controls.
6. Match the supplied listing reference while staying within the imported design system: tall 4:5 imagery, compact premium cards, four columns on desktop, two to three on tablet, two on mobile, and a mobile filter drawer to avoid horizontal overflow.
7. Add `/products/$productSlug` and reuse the same catalogue records for an exact-product detail view. Product cards and “View Product” actions will use typed navigation to this route.
8. Add unique titles, descriptions, Open Graph metadata, and Twitter metadata for both new content routes.

## Verification
- Check home appearance before and after to ensure only click behavior changed.
- Test all eight category-card links and confirm each page shows only its category products.
- Test search, tabs, every supported filter, clear-all, all sort choices, and grid/list switching.
- Test a product card and button through to the matching detail page, then back to its collection.
- Check desktop, tablet, and mobile layouts for image proportion, visible garments, card readability, and horizontal overflow.

## Technical details
- Keep TanStack file-based routing; no new routing system or backend is needed.
- Use the repository’s existing semantic design tokens and shared button controls.
- Product counts will be dynamic for the included local catalogue rather than falsely displaying 124 when only a smaller supplied dataset exists.
