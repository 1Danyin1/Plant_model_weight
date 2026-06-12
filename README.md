# Plant_model_weight
## Trained Machine Learning and Deep Learning Models for Crop Agronomic Trait Prediction
## 1. Project Overview
This repository contains the **trained model weights, supplementary results, and usage instructions** for the study:
> *Predicting Crop Agronomic Traits Using Multitemporal Vegetation Indices and Chlorophyll Fluorescence Parameters via Machine Learning*
High-throughput phenotyping (HTP) based on spectral and fluorescence sensing provides an efficient way to estimate crop growth and yield traits non-destructively. This project develops a comprehensive modeling pipeline that integrates multi-temporal vegetation indices and chlorophyll fluorescence parameters to predict five key agronomic traits, including tiller number, plant height, root length, root dry weight, and shoot dry weight.
This repository hosts the final optimized models from the study, which can be reused, validated, or extended in future research.
## 2. Repository Structure
Plant_model_weight
├── README.md 
└── Trained_Models.zip 
### 2.1 `Trained_Models.zip` Contents
The archive contains:
- **Traditional machine learning models** (`.pkl` format, saved via `joblib`):
## 3. Experimental Background
### 3.1 Study Design
The dataset was collected from a greenhouse experiment with repeated measurements across multiple growth stages. Sampling time points include both days after treatment (`DAT`) and days after reoxygenation (`DAO`).
### 3.2 Input Features
The feature set combines two categories of HTP-derived parameters:
1. **Vegetation indices (22)**
   NDVI, PRI, SIPI, SR, NDRE, GNDVI, CI, MCARI, TVI, OSAVI, PSRI, CRI, NPCI, REP, WBI, PRI570, EVI, MTCI, VARI, CRI700, NDVI705, SR750_700
2. **Chlorophyll fluorescence parameters (16)**
   NPQ_Lss, avg_QY_L4, avg_qN_Lss6, avg_qP_Lss6, avg_qL_Lss6, Fp, avg_NPQ_L4, Ft_L4, avg_Fq_D3, Rfd_Lss, qL_L4, avg_NPQ_Lss, Fm, avg_Rfd_L4, avg_qP_D3
### 3.3 Target Agronomic Traits
Five traits were selected based on their agronomic relevance and heritability:
- `Tiller_number`: Effective tiller count per plant
- `Height`: Plant height (cm)
- `Root_length`: Maximum root length (cm)
- `Root_dry_weight`: Root biomass (g)
- `Shoot_dry_weight`: Above-ground biomass (g)

## 4. Usage Instructions
### 4.1 Environment Requirements
The models were trained with the following key dependencies (Python ≥ 3.8).

   
