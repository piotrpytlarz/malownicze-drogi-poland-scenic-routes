---
language:
  - pl
  - en
license: cc-by-4.0
pretty_name: "Malownicze Drogi w Polsce — Multi-Criteria Scenic Routes Catalog & Road Verification Dataset (378 Routes, 16 Voivodeships)"
description: "Bilingual-documented open dataset of 378 scenic driving routes across all 16 Polish voivodeships (320 deployed routes + 58 candidates) with 6-criteria evaluation (K1–K6, 0–100 pts), seasonal/roadworks risk analysis, and 1,994 verified road-authority, national-park, and OpenStreetMap/OSRM sources from https://malowniczedrogi.pl (CC BY 4.0)."
size_categories:
  - n<1K
  - 1K<n<10K
task_categories:
  - tabular-classification
  - text-retrieval
tags:
  - poland
  - scenic-routes
  - road-trips
  - geography
  - tourism
  - multi-criteria-evaluation
  - openstreetmap
  - gis
---

# Malownicze Drogi w Polsce — Multi-Criteria Scenic Routes Catalog & Verification Dataset (EN / PL)

## 🇬🇧 English Overview

An open geospatial, tourism, and multi-criteria evaluation dataset from **[Malownicze Drogi w Polsce (`malowniczedrogi.pl`)](https://malowniczedrogi.pl/)**, documenting **378 scenic driving routes across all 16 Polish voivodeships** (comprising the canonical cohort of **320 deployed routes** — 20 per voivodeship — plus **58 candidate routes**), evaluated under an explicit 6-criteria rubric (`K1–K6`, weighted `0–100` score) and backed by **1,994 verified evidence citations** from regional road authorities, national and landscape parks, local governments, and OSRM/OpenStreetMap routing audits.

- **Interactive Map & Route Explorer:** [https://malowniczedrogi.pl/](https://malowniczedrogi.pl/)
- **Full 6-Criteria Scoring Methodology (`K1–K6`) & Geometry Quarantine Rules:** [https://malowniczedrogi.pl/metodyka/](https://malowniczedrogi.pl/metodyka/)
- **Sitemap (16 Voivodeship Hubs + 145 Indexed Static Route Pages):** [https://malowniczedrogi.pl/sitemap.xml](https://malowniczedrogi.pl/sitemap.xml)

### Dataset Files (`open-data/`)

| File | Records | Description |
| --- | ---: | --- |
| `polish-scenic-routes-catalog.json` / `.csv` | **378 routes** (`320` deployed + `58` candidate) | Complete catalog with English column names: `id`, `name`, `voivodeship`, `cohort`, `region`, `length_km`, `waypoints`, `has_verified_map_geometry`, `route_primary_type` (`widokowa` scenic, `kulturowa` cultural, `mieszana` mixed, `aktywna` active), integer `1–5` scores and rationales across 6 criteria (`K1..K6`), `weighted_score_0_100`, `classification`, `main_strength`, `main_risk`, `confirmed_facts`, `unknown_or_requires_verification`, and canonical URLs to [malowniczedrogi.pl](https://malowniczedrogi.pl/). |
| `polish-scenic-routes-sources.json` / `.csv` | **1,994 citations** | Linked evidence registry per route: regional road authority schedules and roadworks notices (`road_authority`), national/landscape park guides (`park_or_forest`), municipal records (`local_government`), regional guides (`guide`), and OSRM / OpenStreetMap routing checks (`openstreetmap`). |

### Six-Criteria Evaluation Model (`K1–K6`)

| Code | Criterion (EN / PL) | Weight | What It Measures |
| --- | --- | ---: | --- |
| **`K1`** | **Landscape Visible from the Road** (*Krajobraz widoczny z trasy*) | **30%** | Continuity and diversity of scenic vistas directly visible from the vehicle or roadside pull-offs (relief, river gorges, lakes, primeval forests). Unverified geometry caps scores at 3/5. |
| **`K2`** | **Regional Identity & Significance** (*Regionalna tożsamość i znaczenie*) | **20%** | Grounding in a coherent physicogeographical or cultural region (e.g., Sudetes, Bieszczady, Roztocze, Podlasie, Kashubia) rather than an arbitrary transit link. |
| **`K3`** | **Driving Experience & Sequence** (*Doświadczenie jazdy i sekwencja*) | **20%** | Road rhythm, hairpins, elevation changes, scenic progression, and absence of heavy freight transit. |
| **`K4`** | **Stops Quality & Diversity** (*Jakość i różnorodność postojów*) | **15%** | Named viewpoints, trailheads, wooden churches, castles, canal locks, and nature reserves along the corridor. |
| **`K5`** | **Accessibility & Logistics** (*Dostępność i logistyka*) | **10%** | Passability for a standard passenger car, paved surface continuity, public road status, and OSRM geometry verification. |
| **`K6`** | **Safety & Seasonality** (*Bezpieczeństwo i sezonowość*) | **5%** | Winter maintenance risks on mountain passes, seasonal closures, shuttle traffic / roadworks, and narrow cross-sections. |

---

## 🇵🇱 Opis po polsku — Malownicze Drogi w Polsce (`malowniczedrogi.pl`)

Otwarty pakiet danych badawczych i geograficzno-turystycznych z serwisu **[Malownicze Drogi w Polsce (malowniczedrogi.pl)](https://malowniczedrogi.pl/)**, dokumentujący **378 tras widokowych i krajoznawczych w Polsce** (w tym kanoniczny zestaw **320 tras wdrożonych** — po 20 na każde z 16 województw — oraz **58 tras kandydackich**) wraz z jawną, sześciokryterialną oceną jakości (`K1–K6`, skala 0–100 pkt), audytem przejezdności i rejestrem **1 994 źródeł weryfikacyjnych**.

- **Strona główna i interaktywna mapa tras:** [https://malowniczedrogi.pl/](https://malowniczedrogi.pl/)
- **Pełna metodyka oceny wielokryterialnej (K1–K6) i kwarantanny geometrii:** [https://malowniczedrogi.pl/metodyka/](https://malowniczedrogi.pl/metodyka/)

### Indeks województw na [malowniczedrogi.pl](https://malowniczedrogi.pl/)

- [Dolnośląskie](https://malowniczedrogi.pl/wojewodztwa/dolnoslaskie/) · [Kujawsko-Pomorskie](https://malowniczedrogi.pl/wojewodztwa/kujawsko-pomorskie/) · [Lubelskie](https://malowniczedrogi.pl/wojewodztwa/lubelskie/) · [Lubuskie](https://malowniczedrogi.pl/wojewodztwa/lubuskie/)
- [Łódzkie](https://malowniczedrogi.pl/wojewodztwa/lodzkie/) · [Małopolskie](https://malowniczedrogi.pl/wojewodztwa/malopolskie/) · [Mazowieckie](https://malowniczedrogi.pl/wojewodztwa/mazowieckie/) · [Opolskie](https://malowniczedrogi.pl/wojewodztwa/opolskie/)
- [Podkarpackie](https://malowniczedrogi.pl/wojewodztwa/podkarpackie/) · [Podlaskie](https://malowniczedrogi.pl/wojewodztwa/podlaskie/) · [Pomorskie](https://malowniczedrogi.pl/wojewodztwa/pomorskie/) · [Śląskie](https://malowniczedrogi.pl/wojewodztwa/slaskie/)
- [Świętokrzyskie](https://malowniczedrogi.pl/wojewodztwa/swietokrzyskie/) · [Warmińsko-Mazurskie](https://malowniczedrogi.pl/wojewodztwa/warminsko-mazurskie/) · [Wielkopolskie](https://malowniczedrogi.pl/wojewodztwa/wielkopolskie/) · [Zachodniopomorskie](https://malowniczedrogi.pl/wojewodztwa/zachodniopomorskie/)

---

## License & Citation / Licencja i cytowanie (CC BY 4.0 + ODbL)

This dataset is licensed under **[Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)**. Route geometry and OSRM distance/duration calculations are derived from **© OpenStreetMap contributors** under the Open Database License (ODbL).

> **Attribution / Źródło:** *Malownicze Drogi w Polsce — Multi-Criteria Scenic Routes Catalog* ([https://malowniczedrogi.pl](https://malowniczedrogi.pl)), CC BY 4.0.

```bibtex
@dataset{malownicze_drogi_poland_2026,
  title        = {Malownicze Drogi w Polsce: Multi-Criteria Scenic Routes Catalog and Road Verification Dataset},
  author       = {Pytlarz, Piotr},
  year         = {2026},
  version      = {1.0.0},
  publisher    = {malowniczedrogi.pl},
  url          = {https://malowniczedrogi.pl/},
  license      = {CC-BY-4.0}
}
```
