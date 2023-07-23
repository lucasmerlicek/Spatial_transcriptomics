# README for Spacial Transcriptomics analysis

This repository contains two scripts for a project focused on exploring the spatial biology of cancer using Visium data. The scripts perform the following tasks:

1. **Importation of the preprocessed data**
2. **Normalization of the data**
3. **Extraction and subsetting of the data for analysis**
4. **Spatial analysis and characterization of Ductal Carcinoma In Situ (DCIS) cells**
5. **Investigation of cell type co-occurrences**
6. **Interpretation and comparison of the results with a preprint**

These scripts use several R libraries including Seurat, tidyr, ggplot2, patchwork, and ISCHIA.

## Installation and setup

Before running these scripts, ensure you have the following R packages installed: Seurat, SeuratDisk, tidyr, ggplot2, patchwork, and ISCHIA. If not, they can be installed using `install.packages()` in R.

## Running the Scripts

Both scripts can be run independently by sourcing them in R. These scripts load preprocessed data from RData files, perform several data manipulation tasks, and produce visualizations. For the scripts to function properly, ensure that the working directory is set to the location where the scripts and data files are saved.

## Script Details

The scripts perform the following specific tasks:

1. **Importing and Loading Libraries and Preprocessed Data**

    The scripts load required R libraries and preprocessed data files "vis_processed.RData" and "RCTD_full.RData".

2. **Normalization and Data Preparation**

    Weights from the RCTD results are normalized and converted into a data frame. Visium data is subset, and cell type names are modified to comply with certain requirements. Metadata is added to the Visium data, and cell type names are stored in a variable for future use.

3. **DCIS Characterization**

    The scripts characterize and compare two grades of DCIS, DCIS1 and DCIS2. The characterization includes spatial plotting, detection of co-occurrences of various cell types with DCIS1 and DCIS2, and interpretation of the observed results. This task is split into three sub-tasks: Characterization of DCIS2 cells, Characterization of DCIS1 cells, and Comparison between DCIS1 and DCIS2 cells.

4. **Spatial Co-localization**

    The scripts allow the user to choose a cell type or composition cluster to focus on, and then observe how it spatially co-localizes with other cell types.

5. **Whole Slide Investigation**

    The scripts also perform a global-level analysis to visualize co-occurrences and potential interactions between cell types across the whole slide.

6. **Data Comparison**

    The scripts compare the spatial localization of the cell types deconvoluted in Visium with what is reported in a preprint. This comparison is used to identify swapped cell type labels.



## Course and Tutorial Information

These scripts were developed in the context of the "Spatial Biology of Cancer" course at ETH Zürich. The course is part of the master's degree program in Biotechnology at the same university and is led by Prof. Andreas Moor.

This work was inspired by and heavily influenced by the excellent tutorial on spatial transcriptomics analysis written by Simona Baghai. Her tutorial provided valuable insights and guidance that shaped the structure and content of our scripts.

## Data Availability

Please note that the raw data used in this project is not included in this repository due to privacy and ethical considerations. However, the scripts are designed to be general and flexible, and can be used with other similar data sets with minor modifications.

## Acknowledgements

We are grateful to Prof. Andreas Moor for his guidance and support throughout the course and the development of this project. We also want to express our deep gratitude to Simona Baghai for her enlightening tutorial, which served as a significant resource for our understanding and implementation of the spatial transcriptomics analysis in this project. 

## Authors

Arthur Theuer and Lucas Mer. 

## License

This project is licensed under the MIT License. 

## Contact

For any questions or further clarifications, please feel free to contact us. Our contact information can be found in our GitHub profiles.
