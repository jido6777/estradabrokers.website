# EstradaBrokers — Real Estate Website

> // Freelance project developed for EstradaBrokers, a real estate agency based in Colombia.

**Live site → [estradabrokerssas.com](https://estradabrokerssas.com)**

---

## About

Landing page built for **EstradaBrokers**, a Colombian real estate agency. The site allows visitors to browse available properties, filter by type and price, contact the agency directly via WhatsApp, and view each property's location on Google Maps — all from a single clean page.

---

## Features

- **Dynamic property listing** — properties loaded from a JSON file, no backend required
- **Filters** — browse by category: rent, buy or lot; with price range slider
- **Image slider** — per-property media carousel with dot navigation and full-size view
- **WhatsApp integration** — direct contact button pre-filled with the property name and price
- **Google Maps** — location link for each property
- **Rich property details** — rooms, bathrooms, area (m²), parking, stratum, floor and neighborhood
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
            ├── favicon.svg
            └── [property-folder]/
                ├── thumbs/         ← compressed images for the card slider
                └── [full images]   ← full-res images for lightbox/zoom
```

---

## Adding Properties

Properties are managed through `assets/data/properties.json`. Each entry follows this structure:

```json
{
  "type": "arriendo",
  "price": 2100000,
  "title": "Property name",
  "location": "Full address, City, Colombia",
  "neighborhood": "Neighborhood or building name",
  "city": "City",
  "rooms": 1,
  "baths": 1,
  "area": 30,
  "parking": null,
  "stratum": 4,
  "floor": 4,
  "description": "Brief description of the property.",
  "whatsapp": "573042465513",
  "media": [
    "assets/media/images/[folder]/thumbs/image_01.webp"
  ],
  "mediaFull": [
    "assets/media/images/[folder]/image_01.webp"
  ]
}
```

### Field reference

| Field | Type | Values / Notes |
|---|---|---|
| `type` | string | `"arriendo"`, `"venta"`, `"lote"` |
| `price` | number | Amount in COP (no dots or commas) |
| `title` | string | Display name of the property |
| `location` | string | Full address shown on Maps link |
| `neighborhood` | string | Neighborhood or building name |
| `city` | string | City name |
| `rooms` | number | Number of bedrooms |
| `baths` | number | Number of bathrooms |
| `area` | number | Area in m² |
| `parking` | number \| null | Parking spots, or `null` if none |
| `stratum` | number | Colombian socioeconomic stratum (1–6) |
| `floor` | number \| null | Floor number, or `null` if N/A |
| `description` | string | Short description shown on the card |
| `whatsapp` | string | Phone number with country code, no `+` |
| `media` | array | Thumbnail images for the card slider (`.webp` recommended) |
| `mediaFull` | array | Full-resolution images for lightbox view |

> **Image tip:** Place thumbnails in a `thumbs/` subfolder inside each property's image folder. Use `.webp` format for best performance.

---

## Credits

Developed by **[Jido](https://jido6777.github.io/website/)** — Web Developer.  
All property content and branding belong to EstradaBrokers.

---

<p align="center">
  jido6777 · 2026
</p>
