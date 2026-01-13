# Snowflake ETL / ELT Pipeline (Raw → Staging → Dim/Fact)

This project demonstrates a simple, interview-ready **Snowflake ELT** pattern:
- Load raw data to **RAW**
- Transform into **STAGING**
- Build **DIM** and **FACT** tables
- Use **incremental loads** with `MERGE`

## Tech
- Snowflake SQL
- (Optional) Python loader stub

## Folder Structure
- `sql/` – Snowflake SQL scripts
- `python/` – optional loading helpers
- `docs/` – architecture notes

## How to Run (high level)
1. Create schemas/tables in Snowflake (`sql/01_raw_to_staging.sql`)
2. Build dimensions (`sql/02_dims.sql`)
3. Build facts (`sql/03_facts.sql`)
4. Re-run `MERGE` statements to simulate incremental loads

## Data Model (Example)
- `DIM_CUSTOMER`
- `DIM_PRODUCT`
- `FACT_ORDERS`

## Notes
This repo uses sample tables and patterns meant for portfolio/demo purposes.

