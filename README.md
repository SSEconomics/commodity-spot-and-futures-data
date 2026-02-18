
# Monthly Commodity Spot and Futures Data (17 Primary Commodities)

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

## Overview
This repository provides end-of-month spot prices, mixed-frequency data, and futures forecasts for 17 primary commodities across the energy, metals, and agricultural sectors. It includes standard monthly averages alongside end-of-month high-frequency observations to facilitate testing against the random walk hypothesis.

**Current Status (Preprint Archive):** This repository serves as a static data archive (data through Dec 2022) accompanying the LCERPA Working Paper 2024-3: *Can Futures Prices Predict the Real Price of Primary Commodities?*

---

## Data Access & Setup

### 1. Spot Prices (`spot_data.zip`)
Provides monthly time series for nominal spot prices in U.S. dollars (USD) for 17 commodities. 
* **`All` Tab:** Contains the end-of-month (`x_eom`) and monthly average (`x_ave`) spot prices.
* **Commodity-Specific Tabs:** Includes standard monthly data plus mixed-frequency "k-days-from-EOM" series (`x_eom1` through `x_eom20`), representing the spot price observed *k* trading days before month-end.

### 2. Futures Data & Forecasts (`futures_data.zip`)
Contains 17 Excel workbooks (one per commodity) divided into two folders:
* **`Futures Forecasts/`**: Futures-based forecasts constructed under five different curve-construction assumptions (e.g., End-of-Month adjustment, 5-day average, Monthly average). Columns (e.g., `f_fut#_m_yyyy`) provide the entire sequence of forecasts for horizons t+1 to T from a specific information set.
* **`Futures Data/`**: The contract-level futures prices aligned by delivery horizon (e.g., `CL1`...`CL130` for WTI) before interpolation. Useful for researchers building custom curve constructions.

---

## Commodities Covered
* **Energy:** WTI crude oil, Henry Hub natural gas, Heating oil, Gasoline, Ethanol
* **Metals:** Copper, Aluminum, Nickel, Zinc, Tin, Lead, Gold, Silver, Platinum
* **Agriculture:** Wheat, Corn, Soybeans

*(Note: Authoritative mapping of each commodity to its Bloomberg ticker, market, and source is available in the paper's Appendix A Data Appendix Table A.1).*

---

## Replication Materials
This repository is intended for general research use. A separate replication package will be provided shortly.

---

## How to Cite
When using this dataset, please cite the accompanying working paper and the original data sources listed in the paper:

> Farag, M., S. Snudden, and G. Upton (2024). *Can Futures Prices Predict the Real Price of Primary Commodities?* LCERPA Working Paper 2024-3.

<details>
<summary><b>Click to copy BibTeX entry</b></summary>

```bibtex
@techreport{farag2024futures,
  title={Can Futures Prices Predict the Real Price of Primary Commodities?},
  author={Farag, M. and Snudden, S. and Upton, G.},
  year={2024},
  institution={Laurier Centre for Economic Research and Policy Analysis},
  type={LCERPA Working Paper},
  number={2024-3}
}

```

</details>

---

## Quick Start: Code & Examples *(Coming Soon!)*

Starter code will be provided in both **R** and **Stata** to demonstrate how to easily load the spot prices and align the raw futures panels.

### [R Users]

See `scripts/analysis_r.R` *(Coming Soon)*.

### [Stata Users]

See `scripts/analysis_stata.do` *(Coming Soon)*.


