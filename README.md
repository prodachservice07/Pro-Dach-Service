# Pro Dach Service — Website

Official website for **Pro Dach Service**, an Austrian roofing company based in Vienna. Built as a static single-page application in HTML/CSS/JS, deployed via Vercel.

---

## Live Site

> Deployed at: `https://pro-dach-service.vercel.app` (add custom domain: `profidachservice.at`)

---

## Project Structure

```
/
├── index.html          # Full site — all pages, styles, and logic in one file
├── image-slot.js       # Image slot/placeholder helper (design tool utility)
├── vercel.json         # Vercel routing config (SPA fallback to index.html)
├── assets/
│   ├── hero-roof2.jpg          # Home hero background photo
│   ├── ueberdachung-hero.png   # Überdachung page hero
│   ├── dachsanierung-hero.png  # Dachsanierung page hero
│   ├── verzinnung-hero.png     # Verzinnung page hero
│   ├── zimmermann-hero.png     # Zimmererarbeiten page hero
│   ├── kontakt-hero.png        # Kontakt page hero
│   ├── prodach-logo.png        # Logo variant
│   ├── profi-dach-logo.png     # Logo variant
│   ├── projects/               # 35 project photos (p01–p35, ern-a, ern-b)
│   ├── services/               # Service illustration icons (s1–s6, zaune)
│   ├── dachform/               # Roof type images (ziegel, trapez, stehende, fliesen)
│   ├── sanierung/              # Sanierung material images
│   └── spenglerei/             # Spenglerei service images
```

---

## Pages

| Page | Section ID | Description |
|---|---|---|
| Startseite | `#home` | Hero, trust badges, services overview, project gallery, testimonials |
| Überdachung & Neueindeckung | `#ueberdachung` | Service detail, roof types, material options |
| Dachsanierung | `#dachsanierung` | Sanierung services, process steps |
| Spenglerei & Verzinnung | `#verzinnung` | Sheet metal, gutters, materials |
| Zimmererarbeiten | `#zimmermann` | Timber framing, roof structures |
| Kontakt | `#kontakt` | Contact form, Google Maps, opening hours |

---

## Tech Stack

- **Pure HTML/CSS/JS** — no framework, no build step
- **Font:** Inter (Google Fonts — 400, 500, 700, 900)
- **Forms:** FormSubmit.co → `contact@prodachservice.at`
- **Maps:** Google Maps embed (Quellenstraße 157, 1100 Wien)
- **Deployment:** Vercel (static)

---

## Key Features

- Sticky navbar with scroll-progress bar and mobile drawer
- Animated hero sections with photo backgrounds (Ken Burns effect on Überdachung)
- Project photo gallery with lightbox — 35 photos in 3 auto-scrolling marquee rows
- Floating WhatsApp button (`wa.me/+4368181411903`) and back-to-top button
- Contact form with FormSubmit (no backend needed)
- Full SEO: `<meta>` tags, Open Graph, Twitter Card, JSON-LD `RoofingContractor` schema
- `sitemap.xml` and `robots.txt` included
- Language: German (Austrian) — `lang="de-AT"`

---

## Business Info

| Field | Value |
|---|---|
| Company | Pro Dach Service |
| Phone | +43 681 8141 1903 |
| Email | contact@prodachservice.at |
| Address | Quellenstraße 157, 1100 Wien |
| Hours | Mon–Fri 08:00–18:30, Sat–Sun 08:00–15:00 |
| Website | https://www.profidachservice.at |

---

## Future Changes / Roadmap

### Content
- [ ] Replace placeholder project photos with new job site photos
- [ ] Add more customer testimonials / reviews
- [ ] Add a blog or news section for SEO (seasonal roofing tips, project spotlights)
- [ ] Add before/after sliders for renovation projects

### Features
- [ ] Multi-language support (EN for international clients)
- [ ] Online quote request form with file upload (roof photos)
- [ ] WhatsApp chat widget with pre-filled message templates
- [ ] Cookie consent banner (DSGVO/GDPR compliance for AT)
- [ ] Google Analytics or Plausible integration

### Technical
- [ ] Split into separate HTML pages or migrate to a framework (Astro recommended for SEO)
- [ ] Add image lazy-loading and WebP conversion for faster load times
- [ ] Set up a custom domain on Vercel (`profidachservice.at`)
- [ ] Add Vercel Analytics for traffic monitoring
- [ ] CI: auto-deploy on push to `main`

---

## Deployment

This site deploys automatically on Vercel from the `main` branch. No build step required.

To deploy manually:
```bash
# Just push to main — Vercel handles the rest
git push origin main
```

To run locally:
```bash
python -m http.server 8080
# then open http://localhost:8080
```

---

## Contributing

1. Branch off `main`
2. Make changes to `index.html` or assets
3. Open a pull request with a short description of what changed and why
4. Merge to `main` — Vercel deploys automatically
