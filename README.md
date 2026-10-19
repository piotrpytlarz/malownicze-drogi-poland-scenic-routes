---
language:
  - pl
license: cc-by-4.0
pretty_name: "Malownicze Drogi w Polsce — Multi-Criteria Scenic Routes Catalog & Road Verification Dataset (378 Routes, 16 Voivodeships)"
description: "Otwarty zbiór danych 378 malowniczych tras samochodowych w Polsce (320 tras głównych w 16 województwach oraz 58 tras kandydackich) z 6-kryterialną oceną krajobrazową i logistyczną (K1–K6), wynikami 0–100 pkt, analizą ryzyka sezonowego oraz rejestrem źródeł zarządców dróg i parków narodowych z serwisu https://malowniczedrogi.pl."
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

# Malownicze Drogi w Polsce — Multi-Criteria Scenic Routes Catalog & Verification Dataset

Otwarty pakiet danych badawczych i geograficzno-turystycznych z serwisu **[Malownicze Drogi w Polsce (malowniczedrogi.pl)](https://malowniczedrogi.pl/)**, dokumentujący **378 tras widokowych i krajoznawczych w Polsce** (w tym kanoniczny zestaw **320 tras wdrożonych** — po 20 na każde z 16 województw — oraz **58 tras kandydackich**) wraz z jawną, sześciokryterialną oceną jakości (`K1–K6`, skala 0–100 pkt), audytem przejezdności i rejestrem źródeł weryfikacyjnych.

- **Strona główna i interaktywna mapa tras:** [https://malowniczedrogi.pl/](https://malowniczedrogi.pl/)
- **Pełna metodyka oceny wielokryterialnej (K1–K6) i kwarantanny geometrii:** [https://malowniczedrogi.pl/metodyka/](https://malowniczedrogi.pl/metodyka/)
- **Mapa strony (16 województw + 145 zweryfikowanych kart tras SEO):** [https://malowniczedrogi.pl/sitemap.xml](https://malowniczedrogi.pl/sitemap.xml)

---

## Zawartość pakietu (`open-data/`)

| Plik | Liczba rekordów | Opis zawartości |
| --- | ---: | --- |
| `polish-scenic-routes-catalog.json` / `.csv` | **378 tras** (320 `deployed` + 58 `candidate`) | Pełny katalog tras widokowych w 16 województwach: punkty przelotowe (`waypoints`), długość (`length_km`), region fizycznogeograficzny, typ trasy (`widokowa`, `kulturowa`, `mieszana`, `aktywna`), wyniki i uzasadnienia w 6 kryteriach (`K1..K6`), wynik ważony `0–100`, klasyfikacja, główny atut (`main_strength`), główne ryzyko (`main_risk`), potwierdzone fakty, elementy wymagające weryfikacji przed wyjazdem oraz kanoniczne linki URL do [malowniczedrogi.pl](https://malowniczedrogi.pl/). |
| `polish-scenic-routes-sources.json` / `.csv` | **~1 900 przypisów źródłowych** | Powiązane z trasami źródła dowodowe: wykazy i komunikaty wojewódzkich zarządów dróg (`road_authority`), plany i przewodniki parków narodowych i krajobrazowych (`park_or_forest`), dokumenty samorządowe (`local_government`), przewodniki regionalne (`guide`) oraz obliczenia OSRM / OpenStreetMap (`openstreetmap`). |

---

## Sześciokryterialny model oceny tras (`K1–K6`)

Każda trasa w zbiorze została oceniona na skali całkowitej `1–5` w sześciu wymiarach (szczegółowa dokumentacja kotwic punktowych znajduje się na stronie **[Metodyka oceny tras](https://malowniczedrogi.pl/metodyka/)**):

1. **`K1` — Krajobraz widoczny z trasy (waga 30%):** Ciągłość i różnorodność otwarć widokowych dostępnych bezpośrednio z samochodu lub przydrożnych zatok (rzeźba terenu, doliny rzeczne, jeziora, zwarte kompleksy leśne). Brak potwierdzonej geometrii lub widoczności blokuje oceny `4–5`.
2. **`K2` — Regionalna tożsamość i znaczenie (waga 20%):** Osadzenie szlaku w spójnym regionie fizycznogeograficznym lub kulturowym (np. Sudety, Roztocze, Podlasie, Kaszuby, Żuławy) ponad przypadkowy łącznik tranzytowy.
3. **`K3` — Doświadczenie jazdy i sekwencja (waga 20%):** Rytm drogi, serpentyny, zmiany wysokości, czytelność sekwencji krajobrazowej oraz uciążliwość ruchu ciężarowego.
4. **`K4` — Jakość i różnorodność postojów (waga 15%):** Udokumentowane punkty widokowe, leśne parkingi z nazwą i funkcją, zabytki, śluzy, rezerwaty i krótkie podejścia piesze.
5. **`K5` — Dostępność i logistyka (waga 10%):** Przejezdność dla standardowego samochodu osobowego, ciągłość nawierzchni asfaltowej, status publicznego dostępu i weryfikacja geometrii.
6. **`K6` — Bezpieczeństwo i sezonowość (waga 5%):** Ryzyka zimowego utrzymania na przełęczach górskich, sezonowe zamknięcia, ruch wahadłowy, wąskie przekroje i ruch turystyczny.

---

## Indeks województw na [malowniczedrogi.pl](https://malowniczedrogi.pl/)

- [Dolnośląskie](https://malowniczedrogi.pl/wojewodztwa/dolnoslaskie/) · [Kujawsko-Pomorskie](https://malowniczedrogi.pl/wojewodztwa/kujawsko-pomorskie/) · [Lubelskie](https://malowniczedrogi.pl/wojewodztwa/lubelskie/) · [Lubuskie](https://malowniczedrogi.pl/wojewodztwa/lubuskie/)
- [Łódzkie](https://malowniczedrogi.pl/wojewodztwa/lodzkie/) · [Małopolskie](https://malowniczedrogi.pl/wojewodztwa/malopolskie/) · [Mazowieckie](https://malowniczedrogi.pl/wojewodztwa/mazowieckie/) · [Opolskie](https://malowniczedrogi.pl/wojewodztwa/opolskie/)
- [Podkarpackie](https://malowniczedrogi.pl/wojewodztwa/podkarpackie/) · [Podlaskie](https://malowniczedrogi.pl/wojewodztwa/podlaskie/) · [Pomorskie](https://malowniczedrogi.pl/wojewodztwa/pomorskie/) · [Śląskie](https://malowniczedrogi.pl/wojewodztwa/slaskie/)
- [Świętokrzyskie](https://malowniczedrogi.pl/wojewodztwa/swietokrzyskie/) · [Warmińsko-Mazurskie](https://malowniczedrogi.pl/wojewodztwa/warminsko-mazurskie/) · [Wielkopolskie](https://malowniczedrogi.pl/wojewodztwa/wielkopolskie/) · [Zachodniopomorskie](https://malowniczedrogi.pl/wojewodztwa/zachodniopomorskie/)

---

## Licencja i cytowanie (CC BY 4.0 + ODbL)

Zbiór danych, opisy, oceny `K1–K6` i uzasadnienia są udostępniane na licencji **[Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)**. Dane geometryczne i wyliczenia drogowe OSRM bazują na danych **© OpenStreetMap contributors** (licencja ODbL).

Przy wykorzystaniu zbioru w analizach GIS, modelach rekomendacyjnych, przewodnikach lub badaniach turystycznych prosimy o podanie atrybucji z aktywnym linkiem:

> **Źródło:** *Malownicze Drogi w Polsce — Katalog i wielokryterialna ocena tras widokowych* ([https://malowniczedrogi.pl](https://malowniczedrogi.pl)), licencja CC BY 4.0.

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
