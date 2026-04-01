# Przykłady kart i dashboardu

Gotowy przykładowy dashboard (Lovelace, język interfejsu PL) znajduje się w repozytorium:

- [examples/dashboard-lovelance-PL.yaml](../examples/dashboard-lovelance-PL.yaml)

Zawiera m.in.:

- wykresy cen dzisiaj i jutro (**ApexCharts Card**),
- kafelki i listy encji (ceny, okna PSE, okna konfigurowalne, progi, sensory binarne),
- drugi widok **Kompas Energetyczny** z siatką 24 godzin (kolory jak na stronie PSE) — wymaga **Button Card** z HACS.

## Wymagania (HACS)

| Karta | Repozytorium / nazwa w HACS |
|-------|-----------------------------|
| `custom:apexcharts-card` | ApexCharts Card |
| `custom:button-card` | button-card |

## Entity ID a język Home Assistant

Identyfikatory encji (`sensor.rce_pse_…`, `binary_sensor.rce_pse_…`) są budowane m.in. z nazw tłumaczeń interfejsu. Przy **języku polskim** będą to slugi po polsku (np. `sensor.rce_pse_cena`, `sensor.rce_pse_kompas_energetyczny_dzisiaj`). Przy innym języku — odpowiedniki angielskie. Przed użyciem YAML sprawdź encje w **Narzędzia deweloperskie** i ewentualnie podmień `entity` w pliku.

## Zrzuty ekranu

Poprzednie osobne przykłady kart i grafiki w `examples/images/` zostały zastąpione jednym plikiem dashboardu; możesz dodać własne zrzuty do dokumentacji po dostosowaniu widoku u siebie.
