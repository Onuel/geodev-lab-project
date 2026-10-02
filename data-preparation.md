# Data preparation

**Week 3 deliverable.** GeoDev Lab Africa, Cohort One.
Author: <your name> Emmanuel

What I reprojected, what I clipped, what I checked, and what I fixed.

---

## 1. Coordinate system decisions

**Working CRS:** <EPSG:32631>

**Why this one:** EPSG:4326 uses degrees, but area and distance and length calculations need meters so why i projected to CRS to get accurate measurement.

| Dataset | CRS as downloaded | CRS after | Operation |
|---|---|---|---|
| <name> | EPSG:4326 | EPSG:32631 | Reprojected |


## 2. Clipping to the study area

- **Boundary used:** Nigerian Boundary
- **Link** https://data.grid3.org/datasets/GRID3::grid3-nga-operational-lga-boundaries/about
- **Features before clipping:** 36
- **Features after clipping:** 1



## 3. Preparing the Copernicus DEM

The Copernicus DEM (GLO-30)

- **Source:** https://portal.opentopography.org/datasets

The Dem provides elevation information

- Reprojected to EPSG:32631 meters is needed for accurate elevation bassed analysis in Eti-Osa

## 4. Settlement Extent
Settlements extents provides the extent to the study area boundaries

- **Source:** https://data.grid3.org/datasets/GRID3::grid3-nga-settlement-extents-v4-1/about



## 5. The analysis-ready output

- **File:** `data/processed/<filename>.gpkg`
- **Format:** GeoPackage
- **CRS:** <EPSG:XXXX> 32631


**Status:** Week 3 complete. First spatial analysis in Week 4.
