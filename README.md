### 🌌 **Analysis of Cellular Network Coverage in Diverse Terrains of Sri Lanka**  

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1T-t7ZqpDwy6RX0L300ZD953qPVIcy4hY?usp=sharing)  
 

#### 📍 **Project Overview**
This project leverages **Geographic Information Systems (GIS)** to analyze cellular network coverage in **Sri Lanka**. By integrating **cellular tower data, population density information, and terrain elevation data**, we aim to:
- **Assess** signal propagation and distribution across diverse terrains.
- **Identify** coverage gaps based on real-world data.
- **Optimize** potential locations for new cellular towers.
- **Visualize** network coverage for different technologies (LTE, GSM, UMTS).

**Note:** Cellular data differs somewhat from actual data because publicly available data was limited. Some random data points were populated to fill gaps.



## 📊 **Data Sources**
- **Cellular Tower Data:**  
  - [OpenCelliD](https://opencellid.org/) – Open database of cell towers  
  - [CellMapper](https://www.cellmapper.net/) – Crowd-sourced network coverage  
  - [OpenStreetMap](https://wiki.openstreetmap.org/wiki/OpenStreetMap) – Map data integration  
- **Terrain Data:**  
  - [NASA SRTM Digital Elevation Model](https://developers.google.com/earth-engine/datasets/catalog/USGS_SRTMGL1_003)  
  - Google Terrain Hybrid  
- **Population Data:**  
  - [WorldPop](https://www.worldpop.org/) – High-resolution population maps  
- **Administrative Areas:**  
  - [GADM](https://gadm.org/data.html) – Spatial data for administrative boundaries  



## 🌍 **GIS & QGIS Analysis**
✅ **Cell Tower Mapping**  
✅ **Viewshed Analysis** (Simulating signal propagation using terrain elevation)  
✅ **Population Density Mapping**  
✅ **PostGIS Integration** (Efficient spatial data management)  

**Assumptions:**  
📱 **Tower height:** 70m (approximate)  
📶 **Signal radius:** 5km per tower  



## 🤖 **Colab-Based Analysis**
🔹 **Tower Analysis:**  
- **Visualizing tower locations** and carrier distribution  
- **Classification by operator:** Mobitel, Dialog, Airtel, Hutch  
- **Classification by technology:** 2G, 3G, 4G, LTE  

🔹 **Population Analysis:**  
- **District-level aggregation** of population  
- **Heat maps** for density visualization  

🔹 **Signal Propagation Analysis:**  
- **Coverage visualization** based on terrain impact  
- **Identification of weak coverage areas**  

🔹 **Time-Lapse Analysis:**  
- **Animated visualization of tower deployment over time**  



## 🚀 **Getting Started**
### 🛠️ **Requirements**
To replicate the analysis, you need:
- **Python 3.8+**
- **Google Colab**
- **QGIS** for GIS-based mapping
- **PostgreSQL with PostGIS** (optional for advanced analysis)

### 🏗 **Installation**
```bash
pip install ipywidgets rasterio geopandas numpy pandas matplotlib
```

### 🛠 **Run the Notebook**
1. Open [Google Colab](https://colab.research.google.com/)
2. Upload the `.ipynb` file or run it from GitHub:
   ```python
   !git clone https://github.com/YOUR_USERNAME/gis-project
   ```
3. Run the cells sequentially.

