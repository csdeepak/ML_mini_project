#  Sediment Particle Size Distribution Prediction

This repository contains the **Machine Learning Mini Project** for predicting sediment particle size distributions (PSD) — specifically the **median particle diameter (d50)** and **variance (σ²)** — from co-located hydrodynamic and water-quality measurements.

The project is based on the dataset and approach described in a Stanford study and follows the course mini-project guidelines.

---

## 📌 Project Overview
- **Objective**: Develop machine learning models to predict sediment particle size characteristics from environmental measurements.  
- **Inputs (features)**: salinity, wave-orbital velocity, refractive index, temperature, chlorophyll-a, absorption ratios, tidal velocity, etc.  
- **Outputs (targets)**:  
  - Median grain size (**d50**)  
  - PSD variance (**σ²**)  
- **Evaluation Metrics**:  
  - Coefficient of determination (**R²**)  
  - Root Mean Square Error (**RMSE**)  
  - Mean Absolute Error (**MAE**)  

---

## 📂 Repository Structure
```bash
sedpred-project/
├─ data/                 # raw and processed datasets (not pushed to repo if large)
│   └─ README.md         # notes on dataset sources
├─ notebooks/
│   ├─ 01_EDA.ipynb      # exploratory data analysis
│   ├─ 02_models.ipynb   # baseline models (RF, SVR)
│   └─ 03_final_results.ipynb # final evaluation & plots
├─ src/
│   ├─ preprocess.py     # data cleaning and preprocessing functions
│   ├─ train.py          # model training pipeline
│   └─ evaluate.py       # evaluation and visualization scripts
├─ figures/              # generated plots & figures
├─ requirements.txt      # dependencies
├─ .gitignore
├─ README.md             # project documentation
└─ one_page_writeup.pdf  # final report (to be added)
