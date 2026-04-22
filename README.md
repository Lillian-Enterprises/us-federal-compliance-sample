# Lillian Enterprises — U.S. Federal Compliance Dataset (Sample Release)

**Publisher:** Lillian Enterprises LLC · Knoxville, Tennessee · Est. 2026
**Contact:** msa@lillianenterprises.com · https://lillianenterprises.com
**License:** Creative Commons Attribution-NonCommercial 4.0 (CC BY-NC 4.0)
**Release:** April 2026 (Sample / Public Surface)

---

## What this is

A cross-program U.S. federal compliance dataset reconciled at the facility level via EPA's FRS `REGISTRY_ID`. The full dataset consolidates records from:

- **SDWA** — Safe Drinking Water Act violations, Lead Service Line inventories, UCMR5 PFAS detections
- **NPDES** — National Pollutant Discharge Elimination System permits and enforcement
- **RCRA** — Resource Conservation and Recovery Act hazardous-waste generation and handling
- **ICIS-AIR** — Integrated Compliance Information System air-program violations
- **TRI** — Toxics Release Inventory 5-year trend
- **NRC** — National Response Center incident reports (water contamination, material-reached-water events)

Each figure in the full product is footnoted to the originating federal-database row. All source material is public. The value of the format is the cross-program consolidation, not any single program's data.

## What's in this sample

Three representative tables plus the methodology overview:

| File | Rows | Description |
|---|---|---|
| `sample_top100_community_water_systems.csv` | 100 | Top 100 community water systems by SDWA Lead Service Line Inventory missed milestones. Columns: Rank, PWSID, System Name, State, City, Population Served, Service Connections, Missed Milestones. |
| `sample_state_summary.csv` | 61 | State-level rollup: Total CWS count, aggregate population served, cumulative missed LSL milestones. |
| `sample_nrc_repeat_offenders.csv` | 130 | Top NRC incident-report repeat offenders by `RESPONSIBLE_COMPANY`, with water-contamination event counts and material-reached-water counts. |
| `methodology.pdf` | 4 pp | Overview of the reconciliation pipeline, data sources, source-citation convention, and refresh cadence. |

The full April 2026 release covers 695+ facilities with the complete cross-program matrix (single-facility, multi-program, state-rollup, and sector-rollup views).

## Intended audiences

- **Public-finance credit desks** — screening municipal water issuers for infrastructure-compliance exposure
- **Municipal-bond research** — pre-issuance due diligence on water-utility obligors
- **Environmental-insurance underwriters** — portfolio-exposure reconciliation for environmental liability lines
- **Environmental due-diligence consultancies** — single-facility briefs for M&A and procurement intake
- **Institutional ESG/shareholder research** — cross-program federal-record reconciliation for AGM-season engagement
- **Journalists & public-interest researchers** — fact-checkable source-cited baseline for investigative work

## How to obtain the full product

Three delivery tiers:

### 1. Single-facility compliance dossier — $2,500 (one-time, retail)

Pre-built 14-page PDF for a specific facility covering SDWA, NPDES, RCRA, ICIS-AIR cross-program records with per-row source citation. Immediate delivery via signed URL (valid 72 hours). Current catalog includes 11 flagship facilities:

- Chemours Washington Works WV · Alcoa Warrick IN · LSB El Dorado AR · Westlake Proctor WV · LyondellBasell La Porte TX · Phillips 66 Sweeny TX · Teck Red Dog AK · Clean Harbors Kimball NE · PPG Circleville OH · Dow Sabine TX · Duke Energy Belews Creek NC

→ **[Purchase a single-facility dossier](https://buy.stripe.com/14A6oH9FfdKx6LCaZq3F601)**

Or select a specific facility from the catalog: https://lillianenterprises.com (Request an Engagement Letter link).

### 2. Practice-group data access — subscription (contact for pricing)

A curated subset of the full dataset sized to a specific practice, sector, or state. Quarterly refresh; source citations preserved at the row level.

### 3. Enterprise / firm-wide access — subscription (contact for pricing)

Full national cross-program dataset with quarterly refresh, API access, and custom coverage scoping. Intended for institutional credit, insurance underwriting, and ESG research workflows.

**Inquire:** msa@lillianenterprises.com — write "Engagement Letter Request" in the subject. Scope letter returned within two business days. No calls required.

## Technical notes

- All CSVs are UTF-8, comma-delimited, with a single header row.
- `PWSID` follows EPA's standard 9-character format (state prefix + numeric ID).
- `REGISTRY_ID` (full dataset only) is EPA Facility Registry Service identifier, canonical cross-program join key.
- Date fields are ISO-8601 where present.
- Missing values are empty cells (not `NULL` / `NaN` / `-1`).

## Compliance & posture

Lillian Enterprises LLC is a data analysis and research firm. **We are not a law firm.** Nothing in this dataset or its accompanying materials constitutes legal, regulatory, financial, or investment advice. All analysis derives from publicly available federal records. Buyers and downstream users make their own interpretations; we provide the consolidated record, not the conclusion.

This sample is released under **CC BY-NC 4.0** — you may share and adapt for non-commercial purposes with attribution. Commercial use (including internal-business redistribution) requires a paid subscription per the tiers above.

## Changelog

- **2026-04-22** — Initial sample release across Kaggle / HuggingFace / GitHub. Three CSVs + methodology PDF. Full April 2026 dataset covers 695+ facilities.

## Citation

If you use this sample in academic or journalistic work, please cite:

> Lillian Enterprises LLC (2026). *U.S. Federal Compliance Dataset — Sample Release.* Knoxville, TN. https://lillianenterprises.com

---

© 2026 Lillian Enterprises LLC. Sample data released under CC BY-NC 4.0. Full dataset licensed commercially.
