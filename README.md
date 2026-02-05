# Air Quality Analysis in Amsterdam (PM10 and PM2.5)

## Project Overview
This repository contains the analysis of air quality in **Amsterdam, The Netherlands**, focusing on Particulate Matter (**PM10 and PM2.5**). The study investigates the impact of traffic peak hours on air quality along bike paths and identifies spatial trends in pollution across various neighborhoods.

The project was developed as part of the "Acquisition & Exploration of Geo Data" course at the **University of Twente (ITC)**.

## Objectives
* **Temporal Analysis**: Compare air quality along bike paths during peak hours (06:00–09:00 and 16:00–18:30) versus off-peak hours.
* **Spatial Analysis**: Identify Amsterdam neighborhoods with the highest and lowest annual air pollution.
* **Reliability Assessment**: Determine areas with the most and least reliable air pollution data based on sensor density and data variance.

## Data Sources
The analysis covers the period from **May 1, 2021, to April 30, 2022**, using:
* **Luchtmeetnet**: Official hourly air quality measurements.
* **Samenmeten (RIVM)**: Community-based low-cost sensor data.
* **PDOK**: Administrative boundaries and neighborhood data for Amsterdam.
* **OpenStreetMap (OSM)**: Spatial data for bike paths and road networks.

## Methodology
1.  **Data Acquisition**: Automated extraction of air quality data using Python scripts to interface with Luchtmeetnet and Samenmeten APIs.
2.  **Preprocessing**: Data cleaning and segregation into peak/off-peak periods and weekday/weekend categories.
3.  **Spatial Interpolation**: Used **Inverse Distance Weighted (IDW)** interpolation in ArcGIS Pro to create continuous pollution surfaces from point sensor data.
4.  **Zonal Statistics**: Aggregated interpolated data to the neighborhood level to compare mean PM concentrations.
5.  **Statistical Validation**: Generated histograms, boxplots, and QQplots in **R** to analyze data distribution, skewness, and the reliability of the measurements.

## Key Findings
* **Traffic Impact**: Significant increases in PM10 were observed during peak hours, often exceeding EU safety thresholds in high-traffic corridors.
* **Neighborhood Trends**: Industrial zones and the city center exhibited the highest pollution levels, while coastal areas and parks (e.g., near the Amstel or Amsterdamse Bos) showed significantly better air quality.
* **Data Reliability**: Reliability is highest in the Western and Central districts due to higher sensor density, while peripheral areas show higher uncertainty.

## Tech Stack
* **Python**: Data extraction and API management.
* **ArcGIS Pro**: Spatial analysis, IDW interpolation, and mapping.
* **R**: Statistical analysis and data visualization.

## Author
**Hamza Nadeem** M.Sc. Geo-Information Science and Earth Observation (GFM)  
University of Twente, ITC Faculty  
January 2024
