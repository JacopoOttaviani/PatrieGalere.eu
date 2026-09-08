# Changelog

All notable changes to this project are documented here, in reverse chronological order.

---

## 2026-09-08

### Fixed
- **Basemap** — CARTO stopped serving its Positron basemap anonymously and now stamps every tile with an "API KEY REQUIRED" watermark. Replaced with [OpenFreeMap](https://openfreemap.org/) Positron vector tiles (MapLibre GL via `maplibre-gl-leaflet`), which keep the same light-grey cartography with no API key, no account and no usage cap. Falls back to OpenStreetMap raster tiles where WebGL is unavailable.

---

## 2026-05-21

### Added
- **"Altre iniziative" panel** — new sidebar with links to related organisations and civic projects, bilingual (IT/EN), accessible via dedicated button in the bottom bar
- **"Buy me a coffee" button** — Ko-fi link in the bottom bar, bilingual (IT/EN), with tooltip on hover

---

## 2026-05-20

### Added
- **Favicon (SVG + PNG)** — site icon added in both vector and raster formats; linked in `index.html` ([`1af4c35`](../../commit/1af4c35), [`70be27b`](../../commit/70be27b))
- **English version** — full bilingual support added alongside the Italian interface ([`fc97a8b`](../../commit/fc97a8b))

### Fixed
- **Sidebar layout** — sidebars corrected and expanded with additional project information ([`4edccc8`](../../commit/4edccc8))
- **Filter spacing** — spacing inconsistencies between filter elements resolved ([`fc97a8b`](../../commit/fc97a8b))

### Initial release
- **First commit** — core application launched: interactive map (`index.html`), Italian regional geodata (`italy.geojson`), and prison deaths dataset (`morti.carcere.xls`) ([`8819137`](../../commit/8819137))
