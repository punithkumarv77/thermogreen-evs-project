# ThermoGreen — Urban Heat Island Analytics & Cooling Planner

**Subject:** Environmental Studies and E-Waste Management (BCS508)  
**Selected Topic:** Urban Heat Islands  

## Overview
ThermoGreen is an interactive web prototype designed to map neighborhood-level Urban Heat Island (UHI) hotspots, analyze green canopy deficits, provide targeted heat-risk advisories, and simulate how green infrastructure (urban trees, cool roofs, permeable pavements, and water bodies) lowers urban temperatures, AC electricity consumption, and CO₂ emissions.

## System Architecture (Input → Processing → Output)
- **Input:** Landsat-8/9 TIRS & MODIS Land Surface Temperature (LST), Sentinel-2 NDVI vegetation cover, GIS impervious surface data, IMD rural baseline weather, and ESP32/BME280 IoT micro-climate sensors.
- **Processing:** Spatial normalization, UHI intensity calculation (ΔT = T_urban − T_rural), DBSCAN hotspot clustering, and empirical cooling regression modeling for temperature drop, AC energy saved (MWh), and CO₂ avoided (tonnes).
- **Output:** Interactive color-coded thermal map, urban cooling intervention simulator, filterable neighborhood dataset, and profile-specific heat advisories.

## How to Run / Deploy
1. **Run Locally:** Double-click `index.html` to open it in any web browser (no server or internet required).
2. **Deploy on Netlify Drop:** Go to https://app.netlify.com/drop and drag-and-drop this folder to get a live `.netlify.app` link.
3. **Deploy on Tiiny.site:** Go to https://tiiny.site and upload this zip file or `index.html`.
4. **Deploy on GitHub Pages:** Push `index.html` to a public GitHub repository and enable **Settings → Pages → Deploy from main branch**.
