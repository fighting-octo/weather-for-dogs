# 🐾 Weather for Dogs

A local weather portal with a smart **dog‑walking safety index**. Enter your location and it tells you the current weather, an hour‑by‑hour forecast, a 5‑day outlook, and — most importantly — **when the best time is to walk your dog today and for how long**, tuned to your dog's breed.

**Live site:** _(GitHub Pages URL appears here once published)_

## Features

- **📍 Location search** with a disambiguation menu when multiple places match (defaults to Palo Alto, California). °F / °C toggle.
- **🕐 Hourly forecast** (trailing 12 hours) with temperature, rain chance, and wind direction.
- **🐾 Doggie Walk & Play Index** — the centerpiece:
  - A **"best time to walk"** headline with a recommended duration.
  - A **rest‑of‑day walkability timeline** (now → end of day), color‑coded per hour, with the best window highlighted.
  - A breed‑aware safety engine weighing **heat, cold, wind, air quality, fatigue and rain** across 33 breeds.
  - Clear 5‑stage rating (Safe → Danger), warnings, and breed‑specific gear recommendations (sweater, booties, water, shade…).
- **📅 5‑day forecast** with high/low, conditions, rain chance and wind.
- **🌾 Pollen & allergy index** (live where available, seasonal estimate otherwise).

## Tech

A single self‑contained `index.html` — no build step, no dependencies, no API keys. Weather, air‑quality and pollen data come from the free [Open‑Meteo](https://open-meteo.com) API. Weather icons are inline SVG so they render identically everywhere.

## Running locally

Just open `index.html` in any modern browser (needs an internet connection for weather data and the mascot's web font).

---

_Guidance only — not veterinary or medical advice._
