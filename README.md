# Soil Mapping & Agricultural Management Zone Delineation  
## Geostatistics + Machine Learning for Precision Agriculture

## Overview
End-to-end geospatial data science project to analyze soil variability and segment agricultural land into optimized **management zones** for precision farming.

The project integrates:
- Geostatistics (Kriging interpolation)
- Multivariate analysis (PCA)
- Machine Learning (Fuzzy clustering)
- Spatial analytics (GIS)

to transform raw soil data into **actionable land segmentation for optimized resource allocation**.

---

## Business Problem

Agricultural land is often managed as if soil conditions were uniform.

In reality:
- Soil properties vary significantly across space  
- Uniform application of inputs (fertilizers, irrigation, etc.) leads to:
  - Overuse → higher costs & environmental damage  
  - Underuse → reduced crop yields  

This creates inefficiencies in both **production and cost management** :contentReference[oaicite:0]{index=0}  

---

## Solution

A data-driven framework was developed to:

- Model spatial variability of soil properties  
- Generate continuous soil maps using geostatistics  
- Reduce dimensionality of complex soil data  
- Segment land into optimized **management zones**  
- Enable **precision agriculture strategies**

---

## Study Area

- Location: Calango, Lima, Peru  
- Two agricultural fields:
  - Field A: 0.84 ha (mandarin crop)  
  - Field B: 6.93 ha (uncultivated land)

Georeferenced soil samples were collected and analyzed in laboratory conditions.

---

## Data & Features

Soil properties analyzed:

- Texture (sand, silt, clay)
- Soil moisture
- Organic matter
- pH
- Electrical conductivity (salinity)
- Terrain slope (DEM)

These variables directly impact crop productivity and input efficiency.

---

## Architecture

### Workflow

Soil Sampling (GPS)  
→ Lab Analysis  
→ Data Cleaning (R)  
→ Spatial Modeling (ArcGIS - Kriging)  
→ Feature Engineering  
→ PCA (Dimensionality Reduction)  
→ Clustering (Fuzzy C-Means)  
→ Management Zones (GIS Maps)

---

## Geostatistics (Spatial Modeling)

- Kriging interpolation used to generate continuous spatial maps  
- Semivariograms fitted to model spatial dependence  
- LOOCV (cross-validation) used to optimize models  

### Model Quality
- Interpolation models achieved acceptable to good accuracy (nRMSE < 30%) :contentReference[oaicite:1]{index=1}  

---

## Dimensionality Reduction (PCA)

- Standardized variables (Z-score normalization)  
- Principal Component Analysis applied  
- Components with eigenvalue > 1 selected  

👉 Result:
- Reduced complexity while preserving key soil variability patterns  

---

## Machine Learning (Clustering)

Fuzzy C-Means clustering used to delineate management zones:

- Allows soft membership (realistic for spatial data)  
- Captures gradual transitions between zones  

### Model Selection

Optimal number of zones determined using:

- Fuzzy Performance Index (FPI)  
- Normalized Classification Entropy (NCE) :contentReference[oaicite:2]{index=2}  

---

## Results

- Optimal segmentation: **2 management zones per field** :contentReference[oaicite:3]{index=3}  
- Statistically significant differences between zones in:
  - Organic matter  
  - Soil texture  
  - Moisture  
  - Slope  

These differences justify **differentiated agricultural management strategies**.

---

## Business Impact

This solution enables:

- Variable-rate application of inputs (fertilizers, irrigation)  
- Reduced operational costs  
- Increased crop yields  
- Sustainable land management  

👉 Direct application in:
- Precision agriculture  
- Agribusiness optimization  
- Land investment analysis  

---

## Tech Stack

- R (data analysis, PCA, clustering)
- ArcGIS (geospatial modeling)
- GIS tools (DEM processing)
- Statistical methods (Kriging, hypothesis testing)

---

## Key Techniques

- Geostatistical interpolation (Kriging)
- Semivariogram modeling
- Cross-validation (LOOCV)
- PCA (dimensionality reduction)
- Fuzzy clustering (unsupervised ML)
- Hypothesis testing (t-test, Mann-Whitney)

---

## Real-World Applications

- Precision agriculture optimization  
- Smart fertilizer and irrigation planning  
- Soil variability analysis  
- Agricultural consulting  
- Environmental impact reduction  

---

## 🔗 Links

- 🌐 Portfolio: https://federicogarland.github.io/FedericoGarlandWebsite/  
- 💼 LinkedIn: https://www.linkedin.com/in/federico-garland/