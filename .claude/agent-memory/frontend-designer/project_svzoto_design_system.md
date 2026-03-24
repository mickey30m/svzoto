---
name: SVzoto Design System
description: Brand colors, fonts, Tailwind config, and component patterns for the SVzoto website (verkeersregelaars & evenementondersteuning)
type: project
---

SVzoto is a static HTML website for a traffic control and event support company based in Assen, Netherlands.

**Colors (Tailwind custom):** primary=#2f7cff, accent=#f97c20, navy=#1a1d2e, light=#f5f7fa
**Fonts:** Plus Jakarta Sans (headings, font-heading), Inter (body, font-body) via Google Fonts
**CSS:** Tailwind CDN + custom.css (scroll animations: fade-in, slide-left, slide-right; hero-gradient; service-card hover; cta-pulse; form focus styles)
**JS:** js/main.js handles mobile menu, header scroll shadow, IntersectionObserver for scroll animations, counter animation

**Header pattern:** Fixed, bg-navy/95 backdrop-blur, h-20. Logo is orange rounded-lg box with "SV" + "SVzoto" text. Desktop nav with dropdown for "Diensten". Mobile hamburger menu. Active nav link uses text-white (inactive uses text-gray-300). "Offerte aanvragen" button is always bg-accent.

**Footer pattern:** bg-navy, 4-column grid (brand+socials, diensten links, contact info, navigation). Bottom bar with copyright and link to algemene-voorwaarden.

**Sub-page hero pattern:** bg-navy pt-32 pb-16 with decorative blurred circles, breadcrumb nav, h1 font-heading font-extrabold text-white.

**Address:** Zonnedauwstraat 12, 9404 JR Assen
**Founders:** Zoef Arends (06-40828502, zoefarends@gmail.com), Tony Drijver (06-51232934, tonystechnischedienstverlening@gmail.com)

**Why:** Maintaining consistency across all pages is critical since this is a multi-page static site with no templating engine.
**How to apply:** Always copy exact header/footer HTML from index.html, only changing active nav state. Use same Tailwind config block, Google Fonts links, custom.css reference, and js/main.js script tag.
