## NDVI Assessment & Market Analysis

---

## 📌 Project Overview
This project supports the sale of a residential property by combining **remote sensing analysis** with **local market research**. The objective is to provide a data-driven perspective on both the **environmental quality of the property** and its **position within the housing market**.

---

## 🌿 NDVI (Normalized Difference Vegetation Index) Analysis

### Objective
Evaluate vegetation health and landscape quality surrounding the property to enhance marketing appeal and environmental insight.

---

### Data Source
- High-resolution satellite imagery (WorldView multispectral)
- 4-band imagery:
  - Band 1: N/A  
  - Band 2: Blue  
  - Band 3: Green  
  - Band 4: Near Infrared (NIR)
 
  <img width="1000" alt="image" src="https://github.com/user-attachments/assets/cfc5dbcf-3fcb-4a71-9c13-2a49f8bab3e6">

---

### Methodology

#### 1. Data Preparation
- Imported multispectral raster into QGIS
- Verified band configuration:
  - Red = Band 3  
  - NIR = Band 4  

#### 2. NDVI Calculation
Used Raster Calculator with the formula:

```text
NDVI = (Band 4 - Band 3) / (Band 4 + Band 3)
