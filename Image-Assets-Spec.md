# Image Asset Specification
**STAR Health Website — Site-wide Image Dimensions & Direction**
**Prepared by:** Byte Development
**Date:** May 2026
**Status:** Active — referenced by all wireframes

---

## Purpose

This document is the single source of truth for image dimensions, aspect ratios, and creative direction across the STAR Health website. It exists so that:

- **Enrique** can shoot, crop, and export photography to the correct specifications before handing over.
- **Samuel (Byte Dev)** has a reference to validate delivered assets against before placing them in the build.
- **Thomas** has a clear view of what is being requested and why.

If any wireframe or page is updated to require a new image size, this document must be updated to match.

---

## Dimension Specifications

All dimensions are in pixels (width × height), assumed to be the final delivered crop. Where possible, originals should be supplied at 2× the listed dimension to allow for high-DPI/retina rendering — but the final crop should match the aspect ratio listed exactly.

### Homepage

| Asset | Dimensions | Aspect Ratio | Notes |
|---|---|---|---|
| Hero background | 1920 × 1080 | 16:9 | Full-bleed at top of homepage. Subject must be safe around centre (text overlays). |
| About / Audience photo | 1200 × 900 | 4:3 | Sits within the About SHM section. People-led, environmental. |
| Course card thumbnails | 800 × 450 | 16:9 | One per featured course card. Consistent style and lighting across all cards is critical. |
| Homepage shop banner products | 400 × 400 | 1:1 | Square product cutouts for the shop promo strip on the homepage. White or transparent background preferred. |

### RTT Landing Page

| Asset | Dimensions | Aspect Ratio | Notes |
|---|---|---|---|
| Hero background | 1920 × 1080 | 16:9 | Reuses the homepage spec. Subject: team-based training scenario. No visible weapons or blood. |
| RTT audience photo | 800 × 1000 | 4:5 | Portrait orientation. Instructor demonstrating to a small group. Used in the "Who This Is For" section. |

### Shop Page

| Asset | Dimensions | Aspect Ratio | Notes |
|---|---|---|---|
| Shop hero featured product | 900 × 675 | 4:3 | Hero product spotlight at the top of the shop. Clean background, high resolution. |
| Product grid cards | 600 × 600 | 1:1 | Square product cutouts for every item in the product grid. Consistency across the grid is more important than artistic variation per shot. |
| Featured kit spotlight | 900 × 900 | 1:1 | Square hero treatment for the featured kit section further down the shop. |

---

## Creative Direction Summary

Detailed page-specific direction lives in `RTT-Page-Design-Directions.md`. The site-wide principles below apply to all photography regardless of which page it appears on:

| Principle | Do | Don't |
|---|---|---|
| Lighting | Natural or soft studio lighting; clean shadows | Harsh flash, high-contrast action-cam look |
| Subjects | Real participants and instructors in real scenarios | Posed stock-photo-style shots |
| Environment | Controlled, professional, neutral backgrounds | Cluttered, distracting, or unbranded environments |
| Tone (RTT) | Authoritative, controlled, capable | Aggressive, military surplus, gore |
| Tone (Homepage / Fire Safety) | Approachable, professional, credible | Sterile, overly corporate, generic |
| Resolution | 2× the final crop size where possible, exported as JPEG (85% quality) or PNG for transparency | Phone-screenshot quality, low-DPI exports |

---

## Delivery Format

- **File format:** JPEG for photography, PNG only where transparency is required (product cutouts).
- **Colour profile:** sRGB.
- **Compression:** JPEG quality 85% is the target — visually indistinguishable from original at typical screen sizes without inflating page weight.
- **Naming convention:** `[page]_[asset-name]_[dimensions].jpg` — e.g., `homepage_hero_1920x1080.jpg`, `shop_grid_kit01_600x600.jpg`. Lowercase, hyphenated, no spaces.
- **Delivery channel:** Canva links or shared cloud folder, per current workflow with Enrique.

---

## Provenance

These dimensions were specified by Samuel to Enrique via the SHM social media group on **2026-03-31** and confirmed in use across the three delivered wireframes. This document formalises that conversation.

---

## Outstanding Image Requirements

These are the specific shots still needed at the time of writing (2026-05-12). Update as each is delivered.

- [ ] Homepage hero background (1920 × 1080) — pending from Enrique's next course shoot.
- [ ] Homepage About / Audience photo (1200 × 900) — pending.
- [ ] Homepage course card thumbnails (800 × 450) — pending, one per featured course.
- [ ] Homepage shop banner products (400 × 400) — pending; coordinate with Dom on which products to feature.
- [ ] RTT hero background (1920 × 1080) — pending from Enrique's next course shoot.
- [ ] RTT audience photo (800 × 1000) — pending.
- [x] Initial batch of approved imagery delivered via Canva (2026-05-07, 4 images).
- [ ] Shop hero featured product (900 × 675) — pending; product photography is Dom's responsibility per Enrique.
- [ ] Shop product grid cards (600 × 600) — pending from Dom; one per product in the catalogue (43 products).
- [ ] Shop featured kit spotlight (900 × 900) — pending from Dom.
- [ ] Fire Safety page imagery (dimensions TBC once wireframe is produced) — pending course scope from Dom and on-site / mobile delivery photography from Enrique.

---

*This document is updated whenever a new image requirement is introduced or an existing one is fulfilled. Treat it as living.*
