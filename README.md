# OECD Economic Analysis - Microsoft Fabric Portfolio

## Overview
Analysis of the correlation between unemployment rate and GDP growth rate 
across 11 countries using Microsoft Fabric.

## Countries
G7 (Japan, USA, Canada, UK, Germany, France, Italy) + Netherlands, Sweden, Denmark, Croatia

## Data Source
- OECD Data Explorer: Annual Labour Force Survey (Unemployment Rate)
- OECD Data Explorer: NAAG Chapter 1 GDP (GDP Growth Rate)
- Period: 2000-2024

## Architecture
Medallion Architecture (Bronze / Silver / Gold)

### Bronze
- Raw CSV files from OECD

### Silver
- Cleaned and selected columns
- Renamed to business-friendly names

### Gold
- dimCountry
- dimYear
- factEconomic (Unemployment Rate × GDP Growth Rate)

## Tools & Technologies
- Microsoft Fabric Lakehouse
- PySpark / Spark SQL
- Delta Lake
- Power BI

## Key Finding
No strong overall correlation was found between unemployment rate and GDP growth rate. 
However, Canada showed the strongest negative correlation among all countries.

## Visualization
OECD_Report.png
