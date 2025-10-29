# E-GCS-Dataset: Enhanced Generic Color Steel Dataset for Remote Sensing  

The **E-GCS Dataset** (Enhanced Generic Color Steel Dataset) is a large-scale, multi-scenario remote sensing dataset designed specifically for the identification and analysis of color steel buildings. It provides labeled samples to support research in fields such as remote sensing image processing, semantic segmentation, and urban spatial analysis.  


## 1. Dataset Overview  

- **Purpose**: Address the scarcity of specialized datasets for color steel building extraction in remote sensing, and improve the robustness of models under complex scenarios (e.g., lighting variations, roof slopes, background interference).  
- **Coverage**:  
  - **Spatial Scope**: Covers all provinces in China (excluding Hong Kong, Macao, and Taiwan), organized by provincial administrative divisions.  
  - **Scene Types**: Includes typical scenarios with color steel structures, such as industrial parks, commercial buildings, and residential areas.  
  - **Color Categories**: Focuses on three main types of color steel: blue, red, and white.  
- **Data Format**: High-resolution remote sensing images (in `.tif` format) and pixel-level semantic label masks (in `.png` format).  


## 2. Dataset Structure  

The dataset follows this structure:  
```
E-GCS-Dataset/
├── [Province Name]/  # e.g., jiangsu (Jiangsu Province), guangdong (Guangdong Province)
│   ├── JPEGImages/   # High-resolution remote sensing images
│   │   ├── 1.tif
│   │   ├── 2.tif
│   │   └── ...
│   └── SegmentationClass/  # Pixel-level semantic label masks
│       ├── 1.png
│       ├── 2.png
│       └── ...
└── README.md        # This file
```  


## 3. Key Features & Technical Innovations  

- **Color Space Optimization**:  
  - Generates differentiated adaptive masks for blue, red, and white color steel buildings to eliminate background interference.  
  - Applies regional feature enhancement and multi-scale guided filtering to restore color consistency under complex lighting conditions and roof slopes.  
- **Multi-Scenario Coverage**: Diverse scenes (industrial, commercial, residential) and geographic distributions ensure the generalization ability of models.  
- **Refined Labeling**: Pixel-level annotations for color steel regions, enabling high-precision semantic segmentation tasks.  


## 4. License  

This dataset is released under the [MIT License](https://opensource.org/licenses/MIT) for academic and research purposes only. Commercial use is prohibited without explicit permission.  


## 5. Contact  

For questions or suggestions, please contact:  
- Email: sunminjie01@163.com
