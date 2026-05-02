# 🌱 NDVI Time Series Analysis using Google Earth Engine

## 📌 Project Overview

This project focuses on analyzing **Normalized Difference Vegetation Index (NDVI)** trends over time using satellite data. The objective is to monitor vegetation health, seasonal variability, and agricultural patterns using remote sensing techniques.

The analysis is performed using **Google Earth Engine (GEE)** and Python-based geospatial tools.

---

## 🎯 Objectives

* To compute NDVI from satellite imagery
* To analyze temporal vegetation dynamics
* To observe seasonal trends (Kharif vs Rabi)
* To generate visual outputs for interpretation

---

## 🛰️ Dataset

* **Source:** Sentinel-2 Satellite Data
* **Platform:** Google Earth Engine
* **Bands Used:**

  * NIR (B8)
  * Red (B4)

---

## ⚙️ Methodology

1. Load Sentinel-2 image collection
2. Filter by region of interest (ROI) and time period
3. Apply cloud masking (if applicable)
4. Compute NDVI using:

[
NDVI = \frac{(NIR - Red)}{(NIR + Red)}
]

5. Generate time-series data
6. Visualize NDVI maps and trends

---

## 🧠 Code

Full implementation available here:
👉 **[Open Notebook](./NDVI_Timeseries.ipynb)**

Key snippet:

```python
ndvi = image.normalizedDifference(['B8', 'B4']).rename('NDVI')
```

---

## 📊 Results

### 🌾 NDVI Spatial Distribution



https://github.com/user-attachments/assets/fea2f8d9-218c-4975-882f-6ec439fcd711





---

### 📈 NDVI Time Series Trend

<img width="1785" height="1181" alt="image" src="https://github.com/user-attachments/assets/9be375fd-360c-4ccd-9343-3b79a70b5a87" />


---

## 🔍 Key Findings

* NDVI values show clear seasonal variation
* Demonstrates effectiveness of satellite-based crop monitoring

---

## 🚀 How to Run

1. Clone this repository
2. Open Google Earth Engine / Jupyter Notebook
3. Run `NDVI_Timeseries.ipynb`
4. Export results (GeoTIFF / PNG)

---

## 📁 Project Structure

```
├── NDVI_Timeseries.ipynb
├── images/
│   ├── ndvi_map.png
│   └── ndvi_timeseries.png
└── README.md
```

---

## 🧑‍🌾 Applications

* Precision Agriculture
* Crop health monitoring
* Drought assessment
* Land use analysis

---

## 📌 Future Scope

* Integration with machine learning models
* Multi-index analysis (EVI, NDWI)
* District-level agricultural monitoring
* Climate change impact assessment

---

## 👨‍🎓 Author

**Akashnil Kaibartta**

---
