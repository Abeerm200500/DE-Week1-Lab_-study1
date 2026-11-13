# Week 1 Data Engineering Lab

## Scenario
A small online shop sends daily order data as a CSV file. A manager wants a reliable summary of valid orders by city.

## Pipeline plan
- Source: `orders.csv` (daily batch file)
- Raw destination: BigQuery table `de_intro.raw_orders`
- Curated output: query results after checking and filtering the data
- User of the output: shop manager

## Local data check
Before reporting, record at least two issues you found in the CSV and what you recommend doing with each.

1. Issue and recommendation: missing value and dub, no quntuty 
2. Issue and recommendation:and dub
3. Issue and recommendation:, no quntuty

## What the pipeline does
The data pipeline ingests raw customer orders from a CSV file into Google BigQuery, where data quality issues (such as missing cities, non-positive quantities, and duplicates) are identified and filtered out using SQL queries, resulting in a clean, reliable dataset ready for reporting.