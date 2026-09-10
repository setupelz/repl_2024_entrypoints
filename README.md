# Entry points for assessing 'fair shares' in national mitigation contributions

[![paper](https://img.shields.io/badge/paper-10.1088%2F1748--9326%2Fada45f-1f6feb)](https://doi.org/10.1088/1748-9326/ada45f) [![Zenodo](https://zenodo.org/badge/862120956.svg)](https://zenodo.org/badge/latestdoi/862120956) [![licence](https://img.shields.io/badge/licence-MIT-8a8f98)](LICENSE)

- Paper: https://doi.org/10.1088/1748-9326/ada45f
- Archive of record: https://zenodo.org/badge/latestdoi/862120956 (every release is archived on Zenodo)
- Summary page: https://setupelz.com/work/fair-shares-entry-points.html

Replication archive for:

> Pelz, S., Ganti, G., Pachauri, S., Rogelj, J. and Riahi, K. (2025). Entry
> points for assessing 'fair shares' in national mitigation contributions.
> *Environmental Research Letters* 20(2), 024012.
> https://doi.org/10.1088/1748-9326/ada45f

The paper proposes entry points for fair-share assessment of nationally
determined contributions and illustrates them with a European Union case
study. This archive holds the case-study figure code and its inputs.

## What is here

| Path | Content |
| --- | --- |
| `Code/visualisation.R` | Builds the EU case-study figure (`fig1.png`) from the two input tables; loads packages with `pacman`. |
| `Data/rcb_Lamboll_1.5p50_ALLCOUNTRY_gt_co2ffi_terr_yearend.csv` | Country-level fair-share allocations of the 1.5 °C (50%) remaining carbon budget (Lamboll et al. 2023) under the allocation approaches of the paper, fossil and industrial CO2, territorial, year-end accounting. |
| `Data/region_rcb_EU27_1.5p50_Lamboll_ffi.csv` | The same allocations aggregated to the EU27, by year, with cumulative emissions from 1990, 2015 and 2016. |
| `Data/countrygroups/R11.yaml`, `iso3c.csv` | Region to ISO3 mappings used for the aggregation. |
| `fig1.png` | The published case-study figure. |

The allocations were computed with the `fair-shares` library
(https://github.com/setupelz/fair-shares); this archive keeps the resulting
tables so the figure reproduces without it.

## Running

Open `2024_entrypointscasestudy.Rproj` and source `Code/visualisation.R`.

## Licence

MIT (`LICENSE`).
