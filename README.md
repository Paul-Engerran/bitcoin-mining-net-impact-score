# Bitcoin Energy Accountability — Site×Grid Baseline & Net Impact Scoring (NIS)

![Status](https://img.shields.io/badge/status-working%20draft-yellow)
![Last update](https://img.shields.io/badge/last%20update-2026--03--03-informational)

This repository contains data and code for a site-level ("site×grid") baseline assessment of Bitcoin mining electricity use and location-based Scope 2 emissions, plus an auditable extension: a conservative **Net Impact Score (NIS)** framework.

## What this is (and what it is not)
### Baseline (auditable)
- Unit of analysis: **mining site paired with its electricity accounting zone**
- Emissions boundary: **location-based Scope 2** (annual average intensity by official zone)
- Outputs: site-level and operator-level annual MWh and tCO₂ (plus zone summaries)

### NIS (conservative extension)
NIS assigns credits **only** when backed by publicly auditable evidence (e.g., time-stamped curtailed MWh tied to program settlements; hourly time-matched clean procurement in the same zone).  
If evidence is missing, **credits default to zero**.

> NIS does not replace the baseline. It is a layered framework designed to evolve with disclosures.

## Repository structure
- `data/`
  - `CBECI_ingest_sites_2024.csv` — cleaned ingest-ready site table
  - `ESG_sites_2024_master_*.csv` — master / working tables (may include WIP columns)
  - `ESG_operators_2024_summary*.csv` — operator rollups
  - `ESG_zones_2024_summary.csv` — zone rollups
  - `ESG_CBECI_data_dictionary.csv` — field definitions
- `docs/` — methodology notes, assumptions, changelog (recommended)
- `paper/` — draft manuscript PDF (optional)
- `notebooks/` — exploratory notebooks (clearly labeled if WIP)

## Reproduce
1. Install dependencies (Python ≥3.10): `pandas`, `numpy`, `matplotlib`
2. Run: `python scripts/build_operator_tables.py` (or open the replication notebook if provided)
3. Outputs are regenerated from the site-level CSV.

## How to cite
If you use this repository, please cite:
- the dataset release (when available), or
- this GitHub repository (commit hash + access date).

A `CITATION.cff` will be added once the first stable release is tagged.

## Contact
- Author: Paul Engerran
- Issues & suggestions: please open a GitHub issue with sources/links.
