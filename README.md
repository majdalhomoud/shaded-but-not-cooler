# Shaded but Not Cooler – analysis code

Code for: Al-Homoud, M. "Shaded but Not Cooler: A GIS–Microclimate and Heat-Island Assessment of Pedestrian Heat and
Walkability in Riyadh's Historic Core and Al-Waha (King Salman District)". F1000Research.

- **Archived version (version 1.0):** https://doi.org/10.5281/zenodo.24405095
- **Underlying data:** https://doi.org/10.5281/zenodo.24404896
- **Extended data:** https://doi.org/10.5281/zenodo.24405023
- **Licence:** MIT (see `LICENSE`)

## Notebooks (run in this order)

1. **1_Main_model_run.ipynb** – the main run, with its outputs of 4 November 2026: 1 m sun position, building and tree
   shadows, sky view factor and SOLWEIG-type mean radiant temperature; hour-by-hour shade, Tmrt and UTCI on the design
   day; measured street widths and pedestrian realms; scenarios (cool pavement, shade sails); SOLWEIG check; statistics
   and figures.
2. **2_Heat_island_LCZ_hexagons.ipynb** – reads the outputs of Notebook 1: Landsat LST and Getis–Ord Gi* hot spots, MODIS
   day and night surface heat island, Local Climate Zones with ESA WorldCover, link to the old-core walkability hexagons.
3. **3_Main_model_rerun_version.ipynb** – the same workflow as Notebook 1 with longer automatic retries for the online
   data services (no stored outputs); use it to re-run the analysis.

## How to run

Open a notebook in Google Colaboratory (File → Upload notebook) and choose **Runtime → Run all**. Each notebook installs
its Python packages with pip and saves its results to Google Drive (folder `thermal_oldcore_alwaha`). All input data are
open and downloaded automatically; their versions and access dates are listed in Extended data Table S1.

## Citation

Al-Homoud, M. 2026. "Shaded but Not Cooler: Analysis Code." Version 1.0. Zenodo. https://doi.org/10.5281/zenodo.24405095
