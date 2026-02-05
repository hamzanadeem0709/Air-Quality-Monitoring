# Air Quality Analysis in Amsterdam (PM10 and PM2.5)

## Project Overview
This repository contains the analysis of air quality in **Amsterdam, The Netherlands**, focusing on Particulate Matter (**PM10 and PM2.5**). 

![Air Quality Overview Map](https://github.com/hamzanadeem0709/Air-Quality-Monitoring/blob/main/PM10-Peakhours.jpg)
*Figure 1: Spatial distribution of PM10 across Amsterdam neighborhoods.*

## Objectives
* **Temporal Analysis**: Compare air quality during peak hours versus off-peak hours.
* **Spatial Analysis**: Identify neighborhoods with the highest and lowest annual pollution.
* **Reliability Assessment**: Evaluate sensor data quality.

## Methodology
The workflow involved data extraction via APIs, spatial interpolation using IDW in ArcGIS Pro, and statistical validation in R.

![Workflow Diagram](path/to/your/methodology_flowchart.png)

## Key Results

### 1. Peak vs. Off-Peak Analysis
Analysis shows significant increases in PM10 during peak traffic hours (06:00–09:00).
![Peak Hour Comparison](path/to/your/peak_comparison_chart.png)

### 2. Statistical Distribution
Histograms and QQplots were used to verify the data distribution and identify skewness.
![Statistical Analysis](path/to/your/histograms_plots.png)

## Tech Stack
* **Python**: Data extraction (APIs).
* **ArcGIS Pro**: IDW interpolation & Zonal Statistics.
* **R**: Statistical visualization.

## Author
**Hamza Nadeem** (s3158551)
