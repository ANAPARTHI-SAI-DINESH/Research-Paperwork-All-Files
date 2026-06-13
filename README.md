# Enhanced Wearable Health Sensor Data Analysis — Multi-Athlete System

A thesis research project analyzing physiological and biomechanical data from wearable
sensors across multiple athletes. The work processes raw multi-sensor recordings to derive
clinical-grade health metrics and assess risk indicators (arrhythmia, stroke, and heat-stroke).

## Overview

The analysis covers all athletes in the dataset and computes, per subject:

- 🫀 **Heart Rate (HR)** — raw HR, processed BPM
- 💓 **Heart Rate Variability (HRV)** — RMSSD, pNN50, SDNN, Triangular Index
- 🩸 **Blood Pressure (BP)** — systolic / diastolic, pulse pressure, MAP
- 🫁 **Respiration Rate** — raw and processed respiration rate
- 🩸 **Oxygen Saturation (SpO₂)** — raw SpO₂ and deviation tracking
- 🌡️ **Thermal & activity** — body temperature, heat index, steps, activity level
- 🏃 **Motion** — accelerometer and gyroscope (x/y/z)
- ⚠️ **Risk categories** — health risk, arrhythmia, heat-stroke, and stroke risk

## Repository Contents

| File | Description |
|------|-------------|
| `enhanced_wearable_sensor_data.csv` | The wearable sensor dataset used in the analysis. |
| `Thesis defense.pdf` | Thesis defense presentation slides. |

> 📓 **Analysis code:** The Jupyter notebooks (`.ipynb`) live in a separate **private**
> repository (`Research-Paperwork-Code`) and are not included here. Access available on request.

## Dataset

`enhanced_wearable_sensor_data.csv` contains time-stamped, per-athlete sensor readings.
Key columns include:

- **Identity / context:** `timestamp`, `subject_id`, `age`, `gender`
- **Cardiovascular:** `heart_rate_bpm`, `systolic_bp_mmhg`, `diastolic_bp_mmhg`,
  `hrv_rmssd_ms`, `hrv_pnn50_percent`, `hrv_sdnn_ms`, `hrv_triangular_index`
- **Respiratory / oxygen:** `respiration_rate_bpm`, `spo2_percent`
- **Thermal / environment:** `body_temperature_celsius`, `ambient_temperature_celsius`,
  `humidity_percent`, `heat_index`
- **Activity / motion:** `activity_level`, `steps_count`, `emg_signal_strength`,
  `accel_x_g`, `accel_y_g`, `accel_z_g`, `gyro_x_dps`, `gyro_y_dps`, `gyro_z_dps`
- **Wellbeing / risk:** `stress_level`, `sleep_quality_score`, `health_risk_category`,
  `arrhythmia_detected`, `heat_stroke_risk`, `stroke_risk_category`

## Getting Started

```bash
# Clone the repository
git clone https://github.com/ANAPARTHI-SAI-DINESH/Research-Paperwork-All-Files.git
cd Research-Paperwork-All-Files

# (Recommended) create a virtual environment, then install common dependencies
pip install pandas numpy matplotlib seaborn scipy scikit-learn jupyter
```

The analysis notebooks are maintained in the private `Research-Paperwork-Code` repository.
With access to that repo, place its `.ipynb` files alongside `enhanced_wearable_sensor_data.csv`
and run the cells in order — the notebooks expect the dataset in the same folder.

## Author

**Sai Dinesh Anaparthi** ([@ANAPARTHI-SAI-DINESH](https://github.com/ANAPARTHI-SAI-DINESH))
