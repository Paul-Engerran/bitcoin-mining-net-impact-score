# Bitcoin Energy Accountability — Site×Grid Baseline & Net Impact Scoring (NIS)

![Status](https://img.shields.io/badge/status-working%20draft-yellow)
![Last update](https://img.shields.io/badge/last%20update-2026--03--03-informational)

**Note:** This is an early-stage research project maintained alongside academic work and side projects; the goal is transparent documentation and reproducibility, not a peer-reviewed claim at this stage.

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
- `data/processed/`
  - `v0.1/` — baseline snapshot (site table + operator/zone rollups + data dictionary)
- `data/wip/`
  - intermediate tables (may contain temporary columns / fixes)
- `docs/` — methodology notes, assumptions, changelog (recommended)
- `paper/` — draft manuscript (optional; clearly labeled not peer-reviewed)
- `notebooks/` — exploratory notebooks (clearly labeled if WIP)

## Reproduce
1. Install dependencies (Python ≥3.10): `pandas`, `numpy`, `matplotlib`
2. Run: `python scripts/build_operator_tables.py` (or open the replication notebook if provided)
3. Outputs are regenerated from the site-level CSV.

## How to cite
Please cite this repository using the **commit hash** and **access date**.
A `CITATION.cff` will be provided when the first snapshot release is tagged.

## Contact
- Author: Paul Engerran
- Issues & suggestions: please open a GitHub issue with sources/links.
