# Plan: Nieuwe Website SVzoto.nl

## Over SVzoto

SVzoto is een bedrijf opgericht door **Zoef Arends** en **Tony Drijver**, gevestigd in Assen.
Ze leveren gecertificeerde verkeersregelaars en evenementpersoneel voor festivals, conferenties, sportevenementen en infrastructuurprojecten.

**Huidige website:** https://svzoto.nl/ — gebouwd met WordPress + Kubio (gratis tier).

---

## Doel van het project

Een volledig nieuwe, moderne website bouwen die:
- Professioneler overkomt dan de huidige WordPress/Kubio-site
- Sneller laadt en beter scoort op SEO
- Een contactformulier bevat (ontbreekt nu)
- Een offerte-aanvraagformulier bevat (ontbreekt nu)
- Mobielvriendelijk en responsive is
- Eenvoudig te onderhouden is zonder WordPress

---

## Technische stack

| Onderdeel       | Keuze                              | Reden                                          |
|-----------------|------------------------------------|-------------------------------------------------|
| Basis           | **Plain HTML**                     | Simpel, geen build tools nodig, overal te hosten|
| Styling         | **Tailwind CSS** (via CDN)         | Snel te stylen, geen build stap nodig            |
| Formulieren     | **Formspree** of **Netlify Forms** | Geen backend nodig, makkelijk in te richten      |
| Hosting         | **Netlify**, **Vercel** of eigen   | Statische bestanden, werkt overal                |
| Animaties       | **CSS transitions** + lichte JS    | Subtiel en professioneel, geen zware libraries   |

> **Voordeel:** Puur statische HTML-bestanden — kan gehost worden op elke webserver,
> inclusief hun huidige hosting. Geen PHP, geen database, geen build proces nodig.

---

## Paginastructuur

### 1. Homepage (`/`)
- Hero-sectie met headline, korte intro en CTA-knop ("Vraag een offerte aan")
- Diensten-overzicht (cards met iconen)
- "Waarom SVzoto?" — USP's (gecertificeerd, flexibel, scherpe tarieven, 24/7)
- Referenties / portfolio-preview (recente evenementen)
- CTA-balk met contactknop

### 2. Over ons (`/over-ons`)
- Verhaal van Zoef en Tony
- Foto's van het team
- Missie en visie
- Certificeringen en kwalificaties

### 3. Diensten (`/diensten`)
- Overzichtspagina met alle diensten als cards
- Per dienst een subpagina:
  - `/diensten/verkeersregelaars` — hoofddienst, uitgebreid beschreven
  - `/diensten/ehbo-medewerkers`
  - `/diensten/kassa-medewerkers`
  - `/diensten/toilet-medewerkers`
  - `/diensten/parkeerbeheer`
  - `/diensten/overig`

### 4. Infra werk (`/infra-werk`)
- Beschrijving van infrastructuurwerk
- Certificeringen (VCA, BRL9101TVM)
- Contactgegevens voor inhuur

### 5. Portfolio (`/portfolio`)
- Galerij met uitgevoerde evenementen
- Per evenement: foto's, korte beschrijving, datum
- Eventueel filteren op type dienst

### 6. Contact (`/contact`)
- Contactgegevens (telefoon, e-mail, adres)
- **Contactformulier** (nieuw!)
- Google Maps embed met locatie
- Social media links (Facebook, LinkedIn, Instagram)

### 7. Offerte aanvragen (`/offerte`)
- **Offerte-aanvraagformulier** (nieuw!)
- Velden: naam, bedrijf, e-mail, telefoon, type dienst, datum evenement, locatie, omschrijving
- Bevestigingsmail na verzending

### 8. Algemene voorwaarden (`/algemene-voorwaarden`)
- Volledige tekst van de voorwaarden (nu alleen "mail ons")

---

## Design richting

### Kleuren
Gebaseerd op het huidige merk, maar verfijnd:

| Kleur          | Hex       | Gebruik                        |
|----------------|-----------|--------------------------------|
| Primair blauw  | `#2f7cff` | Knoppen, links, accenten       |
| Oranje accent  | `#f97c20` | CTA's, highlights              |
| Donker navy    | `#1a1d2e` | Header, footer, tekst          |
| Lichtgrijs     | `#f5f7fa` | Achtergronden, secties         |
| Wit            | `#ffffff` | Content achtergrond            |

### Typografie
- **Headings:** Syne of Syncopate (herkenbaar uit huidige branding)
- **Body:** Inter of Open Sans (leesbaar, modern)

### Stijlkenmerken
- Strak en professioneel, passend bij de veiligheidssector
- Subtiele animaties bij scrollen (fade-in, slide-up)
- Afgeronde kaarten met schaduw voor diensten
- Grote, heldere foto's van evenementen en verkeersregelaars
- Duidelijke call-to-actions op elke pagina

---

## Fasering

### Fase 1 — Basis opzetten
- [ ] Mapstructuur inrichten (html-bestanden, css/, img/, js/)
- [ ] Tailwind CSS via CDN koppelen
- [ ] Globale styling opzetten (kleuren, typografie, spacing)
- [ ] Header met navigatie (incl. mobiel hamburger menu)
- [ ] Footer met contactinfo en social links
- [ ] Herbruikbare structuur: header/footer als include of copy per pagina

### Fase 2 — Pagina's bouwen
- [ ] Homepage met alle secties
- [ ] Over ons pagina
- [ ] Diensten overzichtspagina
- [ ] Individuele dienstpagina's (6 stuks)
- [ ] Infra werk pagina
- [ ] Contact pagina met formulier
- [ ] Offerte pagina met formulier
- [ ] Algemene voorwaarden pagina

### Fase 3 — Portfolio & Content
- [ ] Portfolio pagina met galerij
- [ ] Afbeeldingen optimaliseren en in `img/` plaatsen
- [ ] Alle teksten finaliseren
- [ ] SEO meta tags en Open Graph data

### Fase 4 — Afwerking & Launch
- [ ] Responsive design testen (mobiel, tablet, desktop)
- [ ] Performance optimalisatie (Lighthouse score 90+)
- [ ] Formulieren koppelen en testen
- [ ] Favicon en branding assets
- [ ] Domein koppelen en live zetten

---

## Contactgegevens (referentie)

- **Zoef Arends:** 06-40828502 / zoefarends@gmail.com
- **Tony Drijver:** 06-51232934 / tonystechnischedienstverlening@gmail.com
- **Algemeen:** info@svzoto.nl
- **Adres:** Zonnedauwstraat 12, 9404 JR, Assen
- **Facebook:** facebook.com/groups/1858778944581169
- **LinkedIn:** linkedin.com/in/sv-zoto-99984230a/
- **Instagram:** instagram.com/svzoto/

---

## Beeldmateriaal

### Beschikbare foto's
- `WhatsApp Image 2026-01-28 at 15.46.56.jpeg` — Teamfoto van 4 verkeersregelaars in uniform (bruikbaar voor Over ons / Hero)
- Er komen nog meer foto's aan — website wordt opgebouwd met echte fotografie

### Richtlijnen beeldmateriaal
- **Echte foto's** gebruiken, geen cartoon/illustratie-stijl
- Foto's van het team, evenementen en werkzaamheden
- Professionele uitstraling, passend bij de veiligheidssector
- Afbeeldingen handmatig geoptimaliseerd (compressie) en met `loading="lazy"` in HTML

---

## Notities

- De huidige site mist een contactformulier en offerteformulier — dit is een prioriteit
- De algemene voorwaarden pagina is nu een placeholder — inhoud moet aangeleverd worden
- Portfolio bevat momenteel 4 evenementen uit 2024 — kan uitgebreid worden
- Tagline: *"Uw veiligheid staat bij ons voorop!"*
- De twee cartoon-afbeeldingen (watermarked) worden **niet** gebruikt voor de website
