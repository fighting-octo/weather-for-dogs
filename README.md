# 🐾 doggyweather

A local weather portal with a smart **dog‑walking safety index**. Enter your location and it tells you the current weather, an hour‑by‑hour forecast, a 5‑day outlook, and — most importantly — **when the best time is to walk your dog today and for how long**, tuned to your dog's breed, age and build.

**Live site:** **[doggyweather.com](https://doggyweather.com)**

## Features

- **📍 Location search** with a disambiguation menu when multiple places match (defaults to Palo Alto, California). °F / °C toggle.
- **🐶 Your dog's profile** — name, breed, age (puppy / adult / senior) and build. The name appears in the headline, and every recommendation is written for that dog.
- **🕐 Hourly forecast** (trailing 12 hours) with temperature, rain chance, and wind direction.
- **🐾 Doggie Walk & Play Index** — the centerpiece:
  - A **"best time to walk"** headline with a recommended duration.
  - A **rest‑of‑day walkability timeline** (now → end of day), color‑coded per hour, with the best window highlighted.
  - A breed‑aware safety engine weighing **heat, cold, wind, air quality, fatigue and rain** across 34 breeds, with a separate, steeper heat curve for flat‑faced (brachycephalic) breeds.
  - Clear 5‑stage rating (Safe → Danger), warnings, and breed‑specific gear recommendations (sweater, booties, water, shade…).
  - **Pavement paw‑safety guide** with temperature bands and the 7‑second back‑of‑hand test.
- **📅 5‑day forecast** with high/low, conditions, rain chance and wind.
- **🌾 Pollen & allergy index** (live where available, seasonal estimate otherwise).
- **🗺️ Neighborhood Walk Guide** (premium, unlocked with a Buy Me a Coffee code) — pick a walk length and get nearby dog parks and green spaces, a walking route, and a reachable‑area ring on an interactive map.

## Tech

A single self‑contained `index.html` — no build step and no API keys. Hosted on GitHub Pages.

Runtime dependencies are loaded from CDNs: [Leaflet](https://leafletjs.com/) 1.9.4 for the map and the Pacifico web font from Google Fonts. Weather icons are inline SVG so they render identically everywhere.

## Running locally

Just open `index.html` in any modern browser. It needs an internet connection for weather data, the map, and the headline's web font.

## Data sources & credits

- Weather, air‑quality and pollen data from [Open‑Meteo](https://open-meteo.com), licensed [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
- Map data, tiles and places © [OpenStreetMap](https://www.openstreetmap.org/copyright) contributors, available under the [Open Database License (ODbL)](https://opendatacommons.org/licenses/odbl/). Places are queried through the [Overpass API](https://overpass-api.de/).
- Walking routes by [OSRM](https://project-osrm.org/) and reachable‑area rings by [Valhalla](https://valhalla.github.io/valhalla/), both on public demo servers operated by [FOSSGIS e.V.](https://www.fossgis.de/) Those are shared community servers, not production infrastructure — self‑host or use a paid provider if traffic grows.
- Map display by [Leaflet](https://leafletjs.com/) (BSD‑2‑Clause).

---

_Guidance only — not veterinary or medical advice._
