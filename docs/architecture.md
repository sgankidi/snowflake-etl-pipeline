# Architecture

**Pattern:** RAW → STAGING → DW (DIM/FACT)

1. **RAW**: Landing tables (no/low transformation)
2. **STAGING**: Cleaned tables, incremental `MERGE`
3. **DW**: Dimensional model (DIM + FACT), incremental `MERGE`

This repo focuses on showing practical SQL patterns used in Snowflake ELT.
