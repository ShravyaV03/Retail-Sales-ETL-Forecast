
# Azure Data Factory Pipeline Structure

## Pipeline: RetailSales_ETL

### Activities:
1. **Get Metadata** – Inspect source file in Blob Storage
2. **Copy Data** – Load raw CSV into staging area
3. **Data Flow Activity** – Perform transformations:
   - Parse date
   - Filter nulls
   - Compute Total_Sales
   - Normalize column names
4. **Sink** – Load to Azure Synapse Analytics

### Triggers:
- Scheduled Daily
