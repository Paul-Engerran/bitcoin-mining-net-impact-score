# Bitcoin Energy Accountability — Net Impact Score (NIS)

![Status](https://img.shields.io/badge/status-working%20draft-yellow)
![Last update](https://img.shields.io/badge/last%20update-2026--03--03-informational)

**Working paper (in progress).**  
This repository develops a *baseline* and a **Net Impact Score (NIS)** to compare Bitcoin mining actors beyond gross electricity use (MWh), by incorporating observable grid-facing practices (e.g., demand response, curtailment absorption, ancillary services).

## What this is (and is not)

**Goal.** Provide a *comparable* and *auditable* quantification framework to discuss **net system impact** rather than raw consumption.

**Non-goals.**  
- Not claiming a definitive “true” footprint of the entire Bitcoin network.
- Not assuming perfect observability of energy provenance or marginal emissions.

## Core contribution

- A **baseline**: consistent accounting rules and public-data sourcing strategy (public miners + grid/operator sources when available).
- A **Net Impact Score (NIS)**: adjustments to gross MWh using explicit criteria tied to grid interaction and energy context.
- A transparency stance: document assumptions, uncertainty ranges, and data limitations.

## Repository structure

- `paper/` — manuscript sources (draft)
- `data/` — extracted public data / references to sources
- `method/` — methodology notes and scoring logic
- `BIBLIOGRAPHY.md` — living bibliography (human-readable)
- `references.bib` — BibTeX references (machine-readable)
- `CITATION.cff` — how to cite this repo

## Roadmap (living)

- [ ] v0.1 — Scope definition & system boundaries
- [ ] v0.2 — Baseline rules + data dictionary
- [ ] v0.3 — NIS scoring rubric (criteria + weights) + sensitivity checks
- [ ] v0.4 — Case studies (e.g., ERCOT-style flexible load)
- [ ] v0.5 — Robustness, limitations, and comparability discussion
- [ ] v1.0 — Preprint release (SSRN / HAL / arXiv) + archived dataset

## How to cite

Until a preprint is released, please cite the repository:

See `CITATION.cff`.

## Bibliography

See **BIBLIOGRAPHY.md** (categorized) and `references.bib`.

## License

Code: MIT (or your choice)  
Text/manuscript: CC BY 4.0 (or your choice)
