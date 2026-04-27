# EstradaBrokers — Real Estate Website

> // Freelance project developed for EstradaBrokers, a real estate agency based in Colombia.

**Live site → [jido6777.github.io/estradabrokers.website]([http://estradabrokerssas.com/])**

---

## About

Landing page built for **EstradaBrokers**, a Colombian real estate agency. The site allows visitors to browse available properties, filter by type, contact the agency directly via WhatsApp, and view each property's location on Google Maps — all from a single clean page.

---

## Features

- **Dynamic property listing** — properties loaded from a JSON file, no backend required
- **Filters** — browse by category: rent, buy or lot
- **Image slider** — per-property media carousel with dot navigation
- **WhatsApp integration** — direct contact button pre-filled with the property name and price
- **Google Maps** — location link for each property
- **Contact section** — email, WhatsApp, Instagram, Facebook, TikTok and YouTube
- **Responsive design** — mobile and desktop ready

---

## Stack

```
HTML · CSS · JavaScript
Data served from a local JSON file — no frameworks, no backend.
```

---

## Structure

```
estradabrokers.website/
├── index.html
└── assets/
    ├── data/
    │   └── properties.json
    └── media/
        └── images/
            └── favicon.svg
```

---

## Adding Properties

Properties are managed through `assets/data/properties.json`. Each entry follows this structure:

```json
{
  "title": "Property name",
  "price": 500000000,
  "type": "Comprar",
  "description": "Brief description",
  "location": "https://maps.google.com/...",
  "media": [
    "assets/media/images/property1.jpg"
  ]
}
```

---

## Credits

Developed by **[Jido](https://jido6777.github.io/website/)** — Web Developer.  
All property content and branding belong to EstradaBrokers.

---

<p align="center">
  jido6777 · 2026
</p>
