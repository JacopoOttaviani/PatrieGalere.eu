# PatrieGalere.eu

**Interactive map of deaths in Italian prisons — 2002 to 2026.**

---

## About

PatrieGalere is an open-source civic technology project that maps every recorded death inside Italian penitentiaries from 2002 to the present. Each prison facility is represented as a proportionally-sized marker on an interactive map of Italy, broken down by cause of death.

The project was first hand-coded in 2011 by [Jacopo Ottaviani](https://www.linkedin.com/in/jacopo-ottaviani/) and published in Italy's *Il Fatto Quotidiano* and in the UK by [*The Guardian*](https://www.theguardian.com/news/datablog/2012/may/23/italian-prisoners-deaths). It was identified at the time as Italy's first data journalism project. This is a complete rebuild with modern technologies, a revised design, and bilingual (Italian / English) support.

---

## Features

- **Interactive map** — one marker per prison facility, sized proportionally to total deaths
- **Cause of death filters** — suicide, illness, overdose, unknown, and more
- **Statistics panel** — donut chart by cause, bar chart of top 10 facilities, year-by-year trend line
- **Bilingual** — full Italian and English interface
- **Mobile-friendly** — responsive layout for all screen sizes

---

## Data

| Field | Detail |
|---|---|
| **Source** | [Ristretti Orizzonti](https://www.ristretti.org) |
| **Coverage** | 2002 – 2026 |
| **Last updated** | 2026-05-20 |
| **Format** | XLS (`morti.carcere.xls`) |
| **Granularity** | Individual death records per facility, per year, per cause |

[Ristretti Orizzonti](https://www.ristretti.org) is a magazine and documentation centre on prisons, active since 1999 inside Padua's penitentiary. It collects and publishes systematic records on deaths in Italian penitentiaries and is one of Italy's main independent observers of the prison system.

---

## Tech stack

| Library | Purpose |
|---|---|
| [Leaflet 1.9.4](https://leafletjs.com) | Interactive map |
| [Leaflet.markercluster 1.5.3](https://github.com/Leaflet/Leaflet.markercluster) | Marker clustering |
| [Chart.js](https://www.chartjs.org) | Donut, bar, and line charts |

No build step, no framework, no bundler. A single `index.html` file with inline CSS and JavaScript.

---

## Files

```
index.html          — the entire application (map, charts, UI, i18n)
italy.geojson       — Italian regional geodata for the base layer
morti.carcere.xls   — prison deaths dataset (source: Ristretti Orizzonti)
favicon.svg / .png  — site icons
CHANGELOG.md        — version history
```

---

## Related resources

- [DAP — Statistical Office](https://www.giustizia.it/giustizia/it/mg_1_14.page) — official Italian prison population data (Department of Penitentiary Administration)
- [Associazione Antigone](https://www.antigone.it/) — Italian association for rights in the penal system; annual inspection reports
- [Ristretti Orizzonti](https://www.ristretti.org/) — primary data source; independent prison observatory since 1999
- [Made in Jail](https://www.madeinjail.org/) — vocational training in screen printing for incarcerated people, Rebibbia prison, Rome (est. 1983)
- [Made in Carcere](https://www.madeincarcere.it/) — social brand producing ethical goods from Lecce women's prison (est. 2007)
- [Pastificio Futuro](https://www.giustizia.it/giustizia/it/mg_1_21_1.page?contentId=PRD1435487) — pasta workshop inside Casal del Marmo juvenile prison, Rome

---

## License

Data © [Ristretti Orizzonti](https://www.ristretti.org). Code by [Jacopo Ottaviani](https://www.linkedin.com/in/jacopo-ottaviani/).
