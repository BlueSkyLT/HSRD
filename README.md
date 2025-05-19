# HSRD
the HybridSAR Road Dataset (HSRD) released with the paper [Leveraging Mixed Data Sources for Enhanced Road Segmentation in Synthetic Aperture Radar Images](https://doi.org/10.3390/rs16163024).

## Dataset Overview
The HybridSAR Road Dataset (HSRD) is a comprehensive dataset designed to facilitate road segmentation tasks using Synthetic Aperture Radar (SAR) imagery. This dataset addresses the scarcity of high-resolution annotated SAR data by integrating real and synthesized SAR datasets. HSRD includes sub-meter resolution SAR images and corresponding road labels, making it an invaluable resource for researchers and practitioners in remote sensing, urban planning, and disaster management.

## Dataset Composition
The HSRD dataset comprises three main components:

**SpaceNet 6 Road (SN6R) Dataset**: This dataset includes high-resolution SAR images and road labels sourced from OpenStreetMap (OSM). The SAR images are derived from the SpaceNet 6 Challenge, covering the city of Rotterdam.

**DG-SAR Dataset**: Synthesized from the DeepGlobe (DG) optical dataset using an EO2SAR image translation model. This dataset provides SAR-like images generated from high-resolution electro-optical (EO) images.

**SN3-SAR Dataset**: Synthesized from the SpaceNet 3 (SN3) optical dataset using an EO2SAR image translation model. Similar to DG-SAR, this dataset offers SAR-like images generated from high-resolution EO images.


| Dataset Group | Subset            | Total Number of Images | Image Size (px) | Spatial Resolution (m) | Region(s) of Interest |
|---------------|-------------------|------------------------|-----------------|------------------------|-----------------------|
| SN6R          | -                 | 3401                   | 900             | 0.5                    | Rotterdam             |
| DG-SAR        | -                 | 6226                   | 512             | 0.3                    | Thailand              |
| SN3-SAR       | (Total)           | 2780                   | 1300            | 0.5                    |                       |
|               | SN3-Paris         | 310                    |                 |                        | Paris                 |
|               | SN3-Vegas         | 989                    |                 |                        | Vegas                 |
|               | SN3-Shanghai      | 1198                   |                 |                        | Shanghai              |
|               | SN3-Khartoum      | 283                    |                 |                        | Khartoum              |
  

The data source, data collection and preprocessing methodology are documented in detail in the paper.

## Dataset Structure
```
The HybridSAR Road Dataset (HSRD) (17.33 GB)
├── DG-SAR/
│   ├── SAR/
│   └── mask/
├── SN3-SAR/
│   ├── SN3-Kartoum/
│   │   ├── SAR/
│   │   └── mask/
│   ├── SN3-Paris/
│   ├── SN3-Shanghai/
│   └── SN3-Vegas/
└── SN6R/
    ├── SAR/
    └── mask/
```

## Download the Dataset
~~Download the dataset [here](https://drive.google.com/drive/folders/1NcoTCeylKDd3Oz97cmmiT4zMPBniilTr?usp=sharing).~~
The full dataset is host on Kaggle [The HybridSAR Road Dataset (HSRD)](https://www.kaggle.com/datasets/irislan/hybridsar-hsrd).

## Acknowledgements
We would like to thank the SpaceNet team, DeepGlobe Challenge organizers, and OpenStreetMap contributors for providing the foundational data used to create this dataset and [DDAGAN](https://doi.org/10.3390/rs15071878) for the EO2SAR translation model.

## Citation
```
@Article{lan2024hsrd,
AUTHOR = {Lan, Tian and He, Shuting and Qing, Yuanyuan and Wen, Bihan},
TITLE = {Leveraging Mixed Data Sources for Enhanced Road Segmentation in Synthetic Aperture Radar Images},
JOURNAL = {Remote Sensing},
VOLUME = {16},
YEAR = {2024},
NUMBER = {16},
ARTICLE-NUMBER = {3024},
URL = {https://www.mdpi.com/2072-4292/16/16/3024},
ISSN = {2072-4292},
DOI = {10.3390/rs16163024}
}
```

## License
This dataset is released under the MIT License.

## Contact
For any questions or issues, please contact lant0003 at ntu.edu.sg.
