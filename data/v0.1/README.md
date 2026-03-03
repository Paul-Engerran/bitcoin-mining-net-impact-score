# Dataset v0.1 (draft) — Site×Grid baseline (2024)

![Status](https://img.shields.io/badge/status-early%20draft-yellow)
![Snapshot](https://img.shields.io/badge/snapshot-2026--03--03-informational)

# Dataset v0.1 (draft) — Site×Grid baseline (2024)

**Status:** very early draft / work in progress (not peer-reviewed)  
**Generated on:** 2026-03-03  
**Purpose:** portfolio + transparent research log (documenting early steps)

## Attention / early-stage notice (please read)
This v0.1 snapshot reflects an **early, exploratory stage** of the project. Some fields are intentionally incomplete because the underlying public sources are heterogeneous, and part of the work is precisely to **document what is observable vs. what is not**.

In particular:
- Some rows may have missing `Zone`, `Grid_CO2_g_per_kWh`, or `Est_CO2_t`. When `Zone` or grid-intensity inputs are missing or not reliably attributable, **no Scope 2 estimate should be inferred** from that row.
- `Intensity_Source_URL` can be missing when the intensity factor is derived from an intermediate compilation step or when the primary reference still needs verification. These gaps are tracked and will be closed iteratively.
- `LoadFactor_assumed_percent` is an explicit modeling assumption used for initial normalization; it is subject to revision and sensitivity checks in later versions.

The project’s stance is: **document everything from the earliest steps**, even when imperfect, rather than publish a polished result without traceability. This repository is maintained alongside academic work and personal projects; the goal is to converge toward a publication-grade framework over time, not to claim peer-reviewed certainty at v0.1.

## Files
- `ESG_CBECI_data_dictionary.csv` — field definitions and units
- `NIS_ingest_sites_2024.csv` — site-level table (ingest-ready), incl. zone mapping and `Source_URL` where available
- `ESG_operators_2024_summary.csv` — operator-level aggregation (from the site table)
- `ESG_zones_2024_summary.csv` — zone-level aggregation (from the site table)

## Scope & boundary (baseline)
- Unit of analysis: **mining site paired with its electricity accounting zone** (“site×grid”)
- Emissions boundary: **Scope 2, location-based** (annual average grid intensity by zone, when attributable)
- Outputs: annual MWh and estimated tCO₂ (when attributable)

## Notes / limitations
- Values and mappings may change as sources are updated or corrected.
- This snapshot is **baseline-only**; Net Impact Score (NIS) credits are handled separately and require auditable, time-stamped evidence.
- For reproducibility, cite **commit hash + access date** when using this dataset.
