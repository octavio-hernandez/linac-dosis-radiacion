# 🏥 LINAC Radiation Dose Quality Control

Analysis of daily radiation dose measurements from a medical linear accelerator (LINAC), evaluating deviations against clinical thresholds and applying environmental corrections.

## 📋 Dataset
- **Records:** 500 simulated daily measurements (2025–2026)
- **Variables:** Measured dose, target dose, temperature, atmospheric pressure
- **Target:** Percentage deviation from the 2.0 Gy reference dose

## 🔍 Analysis
- Calculation of percentage deviation from the target dose
- Detection of clinical alerts when deviation exceeds ±3%
- Histogram of error distribution with warning (±2%) and stop (±3%) thresholds
- Application of the **KTP correction factor** (temperature and pressure) to adjust measurements
- Comparison of precision: original vs. corrected deviation using boxplots

## 📊 Key Findings
- 63 out of 500 days exceeded the ±3% clinical stop threshold
- The KTP correction factor modifies the dispersion of measurements, reflecting real environmental effects
- Visual separation between corrected and uncorrected deviations confirms the importance of environmental calibration

## 🛠️ Technologies
![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Pandas-green)
![NumPy](https://img.shields.io/badge/NumPy-orange)
![Matplotlib](https://img.shields.io/badge/Matplotlib-red)
![Seaborn](https://img.shields.io/badge/Seaborn-purple)

## 📁 File
| File | Description |
|------|-------------|
| `Dosis_rad_LINAC.ipynb` | Full analysis notebook with markdown documentation |
