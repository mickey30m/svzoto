---
name: SVzoto design system
description: Design system details for SVzoto website - colors, fonts, Tailwind config, component patterns, page structure
type: project
---

## SVzoto Website Design System

**Stack:** Static HTML, Tailwind CDN, vanilla JS, custom CSS
**Fonts:** Syne (headings, weight 600/700/800), Inter (body, weight 400/500/600/700) via Google Fonts
**Colors:** primary=#2f7cff, accent=#f97c20, navy=#1a1d2e, light=#f5f7fa

**Layout:** max-w-7xl container, px-4 sm:px-6 lg:px-8 padding
**Header:** Fixed, bg-navy/95, backdrop-blur-sm, h-20, desktop nav hidden on lg:, mobile menu toggle
**Footer:** 4-column grid (brand+socials, diensten, contact, navigatie), copyright bar with border-t

**Sub-page heroes:** bg-navy, pt-32 pb-20, hero-gradient overlay, decorative blurred circles, breadcrumb nav, bottom SVG wave

**Animation classes:** .fade-in, .slide-left, .slide-right (IntersectionObserver triggers .visible)
**Card patterns:** rounded-2xl, shadow-lg, border border-gray-100, p-8, hover translateY(-8px)
**CTA sections:** bg-navy, decorative blur circles, cta-pulse animation on primary button

**Active nav:** text-white font-medium (desktop), text-white font-medium (mobile); inactive: text-gray-300 hover:text-white
**Section labels:** text-primary font-semibold text-sm uppercase tracking-widest

**Why:** Documenting these patterns avoids re-reading index.html each time new pages are created.
**How to apply:** Use these exact patterns when building new SVzoto pages to maintain visual consistency.
