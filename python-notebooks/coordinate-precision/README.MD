# Coordinate Precision Visualizer

This repository contains a Jupyter notebook that visualizes the impact of decimal precision in latitude and longitude coordinates on a map. It demonstrates how increasing the number of decimal places reduces the uncertainty area (bounding box) around a given point, overlaid on OpenStreetMap tiles.

The notebook is adapted from an Observable post by Volodymyr Agafonkin: [Latitude and Longitude Precision](https://observablehq.com/@mourner/latitude-and-longitude-precision).

## Features

- Converts latitude/longitude to pixel coordinates for map rendering.
- Generates interactive HTML-based maps using OpenStreetMap tiles.
- Highlights the bounding box for a specified precision level (0 to 6 decimal places).
- Automatically adjusts zoom based on precision for better visualization.
- Includes an optional QR code generator for sharing a related ArcGIS notebook URL.

## Example Output

The notebook renders maps like the following (simplified description; run the notebook for interactive views):

- **Precision 0**: Covers a large area (e.g., country-scale).
- **Precision 6**: Covers a very small area (e.g., centimeter-scale).

A red bounding box on each map shows the precision uncertainty.

## Requirements

- Python 3.x
- Jupyter Notebook or JupyterLab
- Core libraries (included in standard Python/Jupyter):
  - `math`
  - `IPython.display` (for HTML rendering)
- Optional (for QR code generation):
  - `qrcode` (install via `pip install qrcode[pil]` for image support)

The notebook was tested in an ArcGIS Notebook environment but should work in any standard Jupyter setup.

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/your-username/coordinate-precision-visualizer.git
   cd coordinate-precision-visualizer
   ```

2. Install dependencies (if using the QR code section):
   ```
   pip install qrcode[pil]
   ```

## Usage

1. Open the notebook in Jupyter:
   ```
   jupyter notebook coordinate_precision.ipynb
   ```

2. Run all cells to see the visualizations for precisions 0 through 6.
   - The maps use example coordinates near London (-0.124572, 51.500743).
   - Customize the `lng` and `lat` variables to test other locations.
   - The notebook includes a comment for Montana State University coordinates (add them if desired).

3. For the QR code:
   - Run the relevant cells to generate and display a QR code linking to an ArcGIS-hosted version of the notebook.

## Customization

- Change the `precision` range in the loop to visualize other levels.
- Adjust map dimensions (`w` and `h`) in the `osm_map` function.
- Set `auto_zoom=False` and provide a manual `zoom` for fixed-scale views.

## Credits

- Original concept and math: Volodymyr Agafonkin (@mourner).
- Adapted for Jupyter with OSM integration.
- OpenStreetMap tiles: © [OpenStreetMap contributors](https://osm.org/copyright).

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details (add one if needed).

Feel free to contribute or report issues!
