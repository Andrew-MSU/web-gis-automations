# Automated GIS Layer Styling

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.14640807.svg)](https://doi.org/10.5281/zenodo.14640807)

This repository contains an IPython notebook designed for automating the styling of GIS layers using ArcGIS Online. It demonstrates how to replicate styling from one layer in a web map to another feature layer.

## Notebook Contents
- **ArcGIS Connection**: How to connect to ArcGIS Online using Python.
- **Layer Identification**: Techniques to search for and identify specific layers within a web map.
- **Styling Extraction**: Extracting style information from an existing layer.
- **Layer Update**: Applying extracted styles to a different layer.

## Prerequisites
- **ArcGIS API for Python** installed in your Python environment.
- **ArcGIS Online Account** with appropriate permissions to edit feature layers.
- **Basic Python and GIS Knowledge**

## How to Use

### In Jupyter Notebook
1. Clone the repository to your local machine or environment.
2. Navigate to the directory containing the notebook:
   ```bash
   cd path/to/your/repository
   ```
3. Launch Jupyter Notebook
   ```bash
   jupyter notebook
   ```
4. Open the notebook and run each cell sequentially. Replace placeholder information (like URLs, user credentials, and item IDs) with your actual data.

### In ArcGIS Online Notebooks
1. Log in to your ArcGIS Online account.
2. Navigate to the **Notebooks** section.
3. Click **New Notebook** and select the appropriate runtime (e.g., Python Standard).
4. Upload the `data-types-in-gis.ipynb` file to your notebook environment:
   - Use the **Upload Files** option in the **Files** section.
5. Run the notebook cells sequentially to complete the exercises and mapping example.

## License
This notebook and its associated files are licensed under the MIT License. See the `LICENSE` file for more details.

## Acknowledgments
Thanks to the GIS community and students who contributed feedback on this notebook.
