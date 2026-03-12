# bilinear-interpolation
# Spatial Regridding of Climate Forecast Data using Bilinear Interpolation

Reprojects and regrids climate forecast NetCDF data onto a common observation grid in **EPSG:3034** using bilinear interpolation.

## Workflow

1. Load observation grid from tab-separated `.txt` file (EPSG:3034)
2. Visualize observation grid on a basemap
3. Build target `xarray` dataset from unique x/y coordinates
4. Load model NetCDF and assign CRS
5. Reproject model data to EPSG:3034
6. Regrid to target grid using bilinear interpolation
7. Save regridded output as NetCDF
