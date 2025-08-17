# Assignment 1: Part D – Comprehensive Final Report

This repository contains my work for **COMP SCI 7209: Big Data Analysis and Project – Assignment 1 (Part D)** at the University of Adelaide.  
It includes the modelling code, visualisations, and replication package for the **bushfire ignition risk modelling task**.

---

##  Project Overview
The project investigates:
- **Research Question**: Which weather and fuel conditions lead to a spike in the number of new bushfire ignitions (≥10 DEA hotspots) in South Australia the following day?  
- **Approach**:  
  - Built an **NRM × day panel dataset (2014–2024)**  
  - Applied **feature engineering** (VPD, DTR, API, FFDI, NDVI)  
  - Trained multiple classifiers (Logistic Regression, RF, XGBoost, LightGBM, etc.) with imbalance-aware pipelines  
  - Evaluated using **nested TimeSeriesSplit CV**, **threshold calibration**, and **F1/ROC/PR AUC metrics**

The final report summarises the methodology, results, prescriptions, and recommendations.

---

## Repository Structure

-

## Datasets

 **Datasets are NOT included in this repository.**  
Due to licensing and storage constraints, you must **download them yourself** or **contact me to request access**.

Sources used:
- [DEA Sentinel Hotspots (2014–2024)](https://www.ga.gov.au/scientific-topics/dea/dea-data-and-products/dea-hotspots)  
- [SILO Australian Climate Data](https://www.longpaddock.qld.gov.au/silo/)  
- [ERA5-Land Reanalysis Data](https://cds.climate.copernicus.eu/datasets/reanalysis-era5-land-timeseries?tab=download)  
- [SA NRM Boundaries](https://www.waterconnect.sa.gov.au)  
- [Google Earth Engine NDVI](https://developers.google.com/earth-engine/datasets/tags/vegetation-indices)  

 After downloading, place files into `./data/` and update file paths in the notebook (e.g., `sa_daily_panel.parquet`, `MODIS_NDVI_daily_interp.csv`).

---

##  Setup

Clone the repo:
```bash
use your own path in cloab then:
conda create -n python=3.10


For questions or dataset access, please reach out:
Wenze Wang – wenze.wang@student.adelaide.edu.au
