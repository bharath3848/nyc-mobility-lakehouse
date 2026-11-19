# NYC Mobility Lakehouse

## Project Overview

End-to-end Data Engineering project using Databricks Lakehouse architecture.

## Technologies

- Databricks
- PySpark
- Delta Lake
- SQL
- Unity Catalog
- Lakeflow Pipelines
- Databricks Asset Bundles (DABs)
- GitHub Actions

---

## Phase 1 - Environment Setup ✅

- Created Databricks Free Edition workspace
- Verified Spark environment
- Created raw_data volume

---

## Data Sources

### NYC Yellow Taxi Trip Data
- File: yellow_tripdata_2024-01.parquet
- Rows: 2,964,624
- Columns: 19

### NYC Taxi Zone Lookup
- File: taxi_zone_lookup.csv
- Rows: 265

---

## Bronze Layer ✅

### bronze_trips

Added ingestion metadata:

- source_file
- ingestion_timestamp

### bronze_zones

Added ingestion metadata:

- source_file
- ingestion_timestamp

---

## Data Profiling Findings

- Total Trips: 2,964,624
- Average Fare: 18.18
- Highest Fare: 5000
- Lowest Fare: -899
- Negative Fare Records: 37,448

---

## Next Steps

- Create Silver layer
- Join trip and zone data
- Build business-friendly location dimensions
- Implement data quality checks
- Create Gold layer KPIs
- Implement Lakeflow pipelines
- Add DABs and CI/CD