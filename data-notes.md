# Data notes

## GRID3 Nigeria Operational LGA Boundaries
-Source: https://data.grid3.org
-Downloaded: 12th September 2026
- features 774 with 10 Columns 
Covers my LGA fully
658KB
The operational wards is not available for Lagos even with the recent update of 3.0 on the grid3 website.

## Elevation SRTM data
-Portal.opentopography.org
-Downloaded: 12th September 2026
1.22MB


## GRID3 Nigeria Settlements Extent v4.1
-Source: https://data.grid3.org
-Downloaded: 12th September 2026
651mb


## OSM  with QuickOSM
-Downloaded : Waterways 
            : Coastline
	    : Lagoons
- many columns have NULL
Exported and Saved as Geopackage in the Raw Folder.

## CRS and Preparation
-Source vector layers arrived in **EPSG:4326 (WGS 84)**.
-Study area: **Eti-Osa LGA**, extracted from **GRID3 LGA boundaries**.
-Settlements, waterways/watercourses, wards and study boundary** were prepared for analysis and reprojected to **EPSG:32631 (WGS 84 / UTM Zone 31N)** for accurate distance and area measurements.
* Waterways were obtained from **OpenStreetMap (QuickOSM)** and prepared for the **200 m watercourse buffer** analysis.
* Area check: **177.932 km²**. This differs from published figures of **174.90 km², 174.067 km², and approximately 192–193 km²**; the GIS-derived value was retained and flagged.
-CRS check:** analysis layers verified as EPSG:32631.
-Coordinate check:** settlement latitude/longitude values checked for missing or invalid records.
-Spatial extent check:** settlements and waterways checked against the Eti-Osa boundary.
-Geometry check:** layers checked for invalid/problematic geometries before analysis.
-Clipping/reprojection check:** outputs visually checked for correct alignment with the study boundary.
-Working/analysis-ready files are stored in **`data/processed/`**; raw source files remain untouched.
