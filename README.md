# Anantacast Website — Astro Migration & Copywriting

A high-performance, single-source industrial metal casting and precision machining digital platform for **Anantacast** (*"From Casting to Finished Product"*), migrated from the Next.js Ambe Service codebase to **Astro 5**, **TypeScript**, and **Tailwind CSS v4**.

---

## 🌟 Executive Summary

This project delivers a complete framework migration with 100% exact word-count content rewriting. It faithfully preserves the visual design, responsive layouts, color palette, typography hierarchy, hover states, scroll animations, and interactive functionality of the original site, while replacing facility management content with authoritative B2B metal manufacturing and foundry copywriting.

### Key Milestones Delivered:
1. **Zero-Asset Architecture:** Cleanly severed all broken media dependencies (Cloudinary video and image URLs) without disrupting grid structures, container heights, or responsive aspect ratios.
2. **Exact Word-Count Matching:** Every heading, subtitle, paragraph, card description, button CTA, and metadata description matches the exact word count of its corresponding Ambe Service text element (verified by automated test suites).
3. **Pure Astro Architecture:** High-speed static generation with vanilla script islands for DOM interactions (mobile drawer, testimonial auto-carousel, services expansion, client-side form validation). Zero heavy SPA framework overhead.
4. **Strict SEO & Semantic Standards:** Dynamic page-level Open Graph, Twitter cards, JSON-LD Schema.org structured data, sitemap generation via `@astrojs/sitemap`, and `robots.txt`.

---

## 🛠️ Technology Stack

- **Framework:** [Astro 5](https://astro.build/) (`^5.18.2`)
- **Language:** TypeScript (`^5.9.3`) with strict type checking
- **Styling:** [Tailwind CSS v4](https://tailwindcss.com/) with `@tailwindcss/vite`
- **Iconography:** `lucide-astro` (`^0.556.0`)
- **SEO & Sitemaps:** `@astrojs/sitemap` (`^3.7.4`)
- **Verification Engine:** Python automated test script for 100% exact word-count compliance

---

## 📁 Project Structure

```
anantacast-website/
├── astro.config.mjs               # Astro configuration with sitemap & Tailwind Vite plugin
├── tsconfig.json                  # Strict TypeScript configuration
├── package.json                   # Project dependencies and scripts
├── README.md                      # Complete project documentation
├── CONTENT_TODO.md                # Corporate checklist for missing client data
├── COPY_WORD_COUNT_REPORT.md      # Itemized audit of original vs replacement word counts
├── public/
│   ├── favicon.svg                # Industrial SVG favicon
│   └── robots.txt                 # Search engine crawler directives
├── scripts/
│   └── generate_copy.py           # Automated word-count verification script
├── src/
│   ├── data/
│   │   ├── copy.json              # Canonical JSON dictionary of verified copy
│   │   └── copy.ts                # Strongly-typed TypeScript copy exports
│   ├── layouts/
│   │   └── Layout.astro           # Root layout with SEO, Google Fonts, Header, Footer
│   ├── styles/
│   │   └── globals.css            # Tailwind CSS v4 directives & typography hierarchy
│   ├── components/
│   │   ├── Header.astro           # Sticky navigation with mobile slide-in drawer
│   │   ├── Footer.astro           # 3-column footer with plant info & anchors
│   │   ├── Hero.astro             # Full-width hero section with CTA button
│   │   ├── Statistics.astro       # Two-column numerical metrics & plant presentation
│   │   ├── OurPeople.astro        # 4-card technical strength & workforce grid
│   │   ├── Testimonials.astro     # 5-item auto-advancing carousel with rating badge
│   │   ├── WhyAnantacast.astro    # 6-card USP grid with spring hover transitions
│   │   ├── TrustedBySection.astro # Infinite smooth horizontal ticker
│   │   ├── ServicesSection.astro  # 12-capability grid with expandable view toggle
│   │   ├── ContactSection.astro   # RFQ inquiry form with client-side validation
│   │   └── WhatsAppFixed.astro    # Floating WhatsApp CTA button
│   └── pages/
│       ├── index.astro            # Homepage (/)
│       ├── about.astro            # About Company & Values (/about)
│       ├── services.astro         # Manufacturing Capabilities Directory (/services)
│       └── contact.astro          # Comprehensive RFQ & Plant Contact (/contact)
```

---

## 📄 Migrated Routes & Pages

| Route | Source File | Status | Description |
| :--- | :--- | :---: | :--- |
| `/` | `src/pages/index.astro` | ✅ Migrated | Complete landing page with Hero, Statistics, Our People, Testimonials, Why Anantacast, Sector Ticker, Capabilities, and RFQ Form. |
| `/about` | `src/pages/about.astro` | ✅ Migrated | Enterprise background, core values, 9 capability cards, 6 differentiator cards, milestone timeline (2016-2024), and Executive Leadership quote. |
| `/services` | `src/pages/services.astro` | ✅ Migrated | 9-card directory of metal casting, CNC machining, heat treatment, and metrology capabilities with direct quote links. |
| `/contact` | `src/pages/contact.astro` | ✅ Migrated | Comprehensive 8-field RFQ submission form, works location contact card, and embedded plant location map. |

---

## 📊 Word-Count Verification Results

The word-count requirement was strictly enforced using `scripts/generate_copy.py`.
- **Total Text Elements Verified:** 275 items
- **Total Mismatches:** 0 (100% exact match)
- **Detailed Audit:** Refer to [COPY_WORD_COUNT_REPORT.md](./COPY_WORD_COUNT_REPORT.md) for element-by-element breakdown.

---

## 🚀 Development & Production Commands

```bash
# Install dependencies
npm install

# Run Astro TypeScript & template diagnostics
npm run check

# Build production static bundle
npm run build

# Start local development server
npm run dev

# Preview production build locally
npm run preview
```
