# 📦 What Makes NYC Hotter

This data visualization project focuses on the urban heat island effect in NYC. By introducing the urban heat island (UHI) phenomenon in New York City and exploring the potential factors that contribute to it, this project aims to provide viewers with a comprehensive understanding of UHI and offer insights for future urban planning and mitigation strategies.

**Project Link: https://kharlewu.net/uhi_nyc/**

## 🌟 Features

- Line charts of the temperature difference between Central Park and White Plains
- Map of the UHI Index in NYC
- Raster Data Analysis
- Principal Component Analysis and Geographic Weighted Regression on Temperature

## 🚀 Getting Started

### Prerequisites

```bash
pip install -r requirements.txt
```

### Installation

Clone the repository:

```bash
git clone https://github.com/KharleWu/UHI_NYC.git
```

## 🧱 Project Structure

```bash
UHI_NYC/
│
├── Code/                           # Code file
│   │
│   ├── Data_Processing.ipynb       # Including all the data processing and preliminary analysis
│   ├── Raster_Processing.ipynb     # Including all the raster data processing using ** GDAL, Rasterio, and Zonal_Stat **
│   ├── GWR_Analysis.ipynb          # Including all the PCA and GWR Analysis Process
│   ├── Temperature_Line.html       # The HTML file for the temperature line chart (Data Source is in NWS_Temperature file)
│   ├── UHI_Index.html              # The HTML file for the the UHI_Index map (Data Source is in UHI_Index file)
│   ├── Pearson_Corr.html           # The HTML file for the Pearson Correlation chart between Temperature and other independent variables 
│   ├── PCA_Screenplot.html         # The HTML file for the PCA's results
│
├── NWS_Temperature/                # Data file for the temperature line chart
│   │
│   ├── Avg_Temperature_Final.csv   # The final data file used in the Temperature_Line.html
│   ├── Data/                       # The raw data file, sourced from the National Weather Service (NWS)                
│
├── UHI_Index/                      # Data file for the UHI_Index map
│   │
│   ├── UHI_Index.geojson           # The final data file used in the UHI_Index.html
│   ├── Classification.png          # A data distribution histogram showing the data analysis of the UHI_Index data
│   ├── Data/                       # The raw data file, sourced from the NYC Open Data and Climate Central
│
├── USGS_Raster/                    # Data file for the Raster Data Analysis
│   │
│   ├── Block.geojson               # The NYC census block geodata
│   ├── Borough.geojson             # The NYC borough geodata
│   ├── BlockGroup_shp/             # The NYC census block group geodata
│   ├── Example_Pic/                # The Example pics file with all the raster data analysis results
│
├── UHI_PCA/                        # Data file for the UHI's PCA and GWR Analysis
│   │
│   ├── BlockGroup_Final.geojson    # The final data file used in the PCA and GWR Analysis with all the dependent and independent data
│   ├── corr_pic.png                # The Pearson Correlation Matrix pic
│   ├── Final Temperature/          # The Final Temperature Raster Data
│
├── UHI_NYC.jpg                     # The JPG Version of the poster
├── UHI_NYC.pdf                     # The PDF Version of the poster
├── README.md
└── requirements.txt
```

## 🤝 Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## 🩷 The End
Thank you for clicking on this repository, hope you find the project helpful.

## Poster
![UHI_NYC](UHI_NYC.jpg)
