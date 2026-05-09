# Apennines Territory Analysis — Gli Appennini come Palinsesto

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Book](https://img.shields.io/badge/Book-Donzelli_Editore_2025-blue)](https://www.donzelli.it)
[![Python](https://img.shields.io/badge/Python-3.8%2B-green?logo=python)](https://www.python.org/)
[![QGIS](https://img.shields.io/badge/GIS-QGIS_3.x-brightgreen)](https://qgis.org/)
[![GeoPandas](https://img.shields.io/badge/GeoPandas-0.14%2B-blue)](https://geopandas.org/)
[![Folium](https://img.shields.io/badge/Folium-0.14%2B-green)](https://python-visualization.github.io/folium/)

---

## Overview

This repository documents the data analysis and visualisations produced for the chapter:

> **Barbera, F. & Varavallo, G. (2025).** *Gli Appennini come palinsesto. Territorio, demografia, economia.* In F. Di Cosmo (a cura di), *Montagne a bassa definizione. Gli Appennini tra crisi di identità e cambiamento.* Donzelli Editore, Roma. ISBN 978-88-5522-692-9

The chapter develops a quantitative portrait of the Italian Apennine ridge through the metaphor of the **palimpsest** — a dynamic landscape where natural, demographic, and economic layers are continuously stratified and rewritten. The analysis covers **992 Apennine municipalities** (12.55% of all Italian municipalities, representing 4.45% of the national population).

---

## Research Context

The Apennines are Italy's largest orographic chain — larger than Hungary, Portugal, or Austria — yet remain largely invisible in national policy debates, often described as a "low-definition mountain." This work aims to reduce that opacity by building an empirically grounded, multi-dimensional portrait of Apennine territory across three analytical dimensions:

- **Geography & environment** — altimetric distribution and forest cover along the ridge
- **Demography & settlement** — population trends, urbanisation degree, foreign residents (2011–2021)
- **Economy & labour** — local economic units, employees by sector (ATECO), unemployment rates

---
## Maps & Figures

### Altimetric zones and Apennine municipalities

![Municipalities by Altimetric Zone and Apennine Municipalities](apennine_municipalities_map.svg)

*Left: Italian municipalities by altimetric zone. Right: Apennine municipalities identified for the analysis (992 comuni, 12.55% of all Italian municipalities). Source: ISTAT (2022) — elaboration by Barbera & Varavallo (2025).*

Further visualisations will be added progressively and cover:

- Forest cover distribution along the ridge
- Demographic dynamics 2011–2021 (population change and foreign residents)
- Economic activity distribution: services and industry by municipality
- Employees by economic sector across Apennine provinces

---

## Data Sources

| Dimension | Variables | Source | Year |
|---|---|---|---|
| Geography | Altimetric zone, forest cover (%) | ISTAT, MIPAAF | 2020–2022 |
| Demography | Population change, urbanisation, foreign residents | ISTAT, Eurostat | 2011–2021 |
| Economy | Local units, employees by sector, unemployment | ISTAT Asia Register | 2020–2022 |
| Territory | SNAI classification (Polo → Ultraperiferico) | SNAI | 2021–2027 |

---

## Key Findings

**Geography & Environment** — Forest cover varies from below 25% to above 75% along the ridge, concentrated in the central and northern sections. Expanding forests — a result of post-war agricultural abandonment — do not automatically generate ecosystem value without active sustainable management.

**Demography** — 77% of Apennine municipalities are in demographic decline, with an average population loss of ~8% over the past 40 years (vs. +10% nationally). 91.4% of municipalities are classified as rural (Eurostat); 51.7% fall in the peripheral or ultra-peripheral SNAI categories. A counter-trend is emerging in some municipalities where growing foreign resident populations are partially offsetting native emigration.

**Economy & Labour** — Services dominate (>70% of economic activity in most municipalities), with significant concentrations in Emilia-Romagna, Lazio, and Tuscany. Industrial activity is sparse and fragmented. Unemployment rates show a sharp North-South divide, exceeding 20% in parts of Calabria and Sicily.

---

## Methodology

The analysis combines:

- **Python / Jupyter** — data cleaning, merging of ISTAT/Eurostat/SNAI datasets, statistical analysis and chart generation
- **GeoPandas** — geospatial data manipulation, spatial joins between municipal boundaries and thematic datasets, and map-ready dataframe exports
- **Folium** — interactive map rendering for exploratory spatial analysis
- **QGIS** — cartographic processing of altimetric zones, forest cover shapefiles, and demographic variables; final map production and SVG/PNG export
- **Conceptual framework** — the palimpsest metaphor (Corboz, 1998): each analytical layer is treated as a stratum of a living archive continuously rewritten by human and natural agency

---

## Tech Stack

| Tool | Version | Purpose |
|---|---|---|
| Python | 3.8+ | Data analysis and scripting |
| Jupyter Notebook | — | Interactive analysis environment |
| pandas | — | Tabular data processing |
| [GeoPandas](https://geopandas.org/) | 0.14+ | Geospatial data manipulation and spatial joins |
| [Folium](https://python-visualization.github.io/folium/) | 0.14+ | Interactive map rendering |
| matplotlib / seaborn | — | Statistical charts and figures |
| [QGIS](https://qgis.org/) | 3.x | Cartographic processing and map production |

---



## Citation

```bibtex
@incollection{barbera_varavallo_2025,
  author    = {Barbera, Filippo and Varavallo, Giuseppe},
  title     = {Gli {A}ppennini come palinsesto. {T}erritorio, demografia, economia},
  booktitle = {Montagne a bassa definizione. {G}li {A}ppennini tra crisi
               di identit{\`a} e cambiamento},
  editor    = {Di Cosmo, Federico},
  publisher = {Donzelli Editore},
  address   = {Roma},
  year      = {2025},
  pages     = {83--105},
  isbn      = {978-88-5522-692-9}
}
```

---

## Authors

**Filippo Barbera** — Department of Cultures, Politics and Society, University of Turin & Collegio Carlo Alberto
✉ filippo.barbera@unito.it

**Giuseppe Varavallo** — Department of Cultures, Politics and Society & Department of Economics and Statistics "Cognetti de Martiis", University of Turin
✉ giuseppe.varavallo@unito.it

---

## License

Code and data: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). The published chapter text is © 2025 Donzelli Editore.
