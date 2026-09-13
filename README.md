# Financial Instrument Reference Data Pipeline

> JPMorgan Chase & Co | Oct 2016 – Jul 2018

## Overview

Designed and operated a financial instrument reference data pipeline ingesting and
standardising **4M+ instruments** into the JPMorgan Global Instrument Master (GIM)
system — the golden source for all downstream client systems.

## Pipeline Architecture

```
Bloomberg Data License (BDL)
    ↓  Daily file delivery (SFTP)
File Ingestion Layer
    ↓  Validation: completeness · format · referential integrity
Standardisation (Python scripts)
    ↓  Normalise ISIN · LEI · ticker · CUSIP · SEDOL
Global Instrument Master (GIM)
    ↓  Golden source — 4M+ instruments
Downstream Client Systems
    (Middle Office · Trade Support · Settlements)
```

## Data Processed

| Data Type | Source | Volume |
|---|---|---|
| Equity instruments | Bloomberg · Refinitiv | 2M+ |
| Fixed income | Bloomberg | 1M+ |
| Derivatives | Internal · Bloomberg | 500K+ |
| FX instruments | Internal | 200K+ |

## Reference Data Identifiers Managed

- **ISIN** — International Securities Identification Number
- **LEI** — Legal Entity Identifier
- **CUSIP** — Committee on Uniform Securities Identification Procedures
- **SEDOL** — Stock Exchange Daily Official List
- **Bloomberg ticker** — proprietary identifier
- **Exchange codes** — MIC (Market Identifier Code)

## Corporate Actions Processed

Stock splits · Dividends · When Issued · Listings · Delistings
Ticker symbol changes · Reverse splits · ID number changes · Name changes

## Data Quality

- **99% data integrity** achieved for client golden source systems
- Daily Quality Alerts across market sessions
- Cross-validation against internal client-initiated changes
- Reconciliation against Middle Office, Trade Support, Settlements

## Technology Stack

Python · SQL · Bloomberg Data License · SFTP · ISIN · LEI · Reference Data Management
