# Data notes
**Week 2 deliverable.** GeoDev Lab Africa, Cohort One.

Author: Emmanuel

## GRID3 Nigeria Settlement Extents v4.1 (published August 2026)
- Source: https://data.grid3.org/datasets/GRID3::grid3-nga-settlement-extents-v4-1/about
- Downloaded: 12/09/2026
- Columns: fid (integer), block_id (text), country (text) iso3 (text), block_area_sqm (decimal), block_perimeter (decimal), block_neigbor_count (integer), building_count (integer), building_area_max (decimal), building_area_sum (decimal), building_area_median (decimal), building_area_stdev (decimal), building_area_percentage (decimal), extent_type (text), mgrs_code (text), ndvi_mean (decimal), evi_mean (decimal), building_max_height (decimal), building_mean_height (decimal), blocks_per_settl_extent (integer), building_count_density_quantile_rank (decimal), building_max_area_quantile_rank (decimal), building_count_density (decimal), bd_class (text), ma_class (text), composite_class (text)
- No specific name field
- Covers my LGA fully


## OSM river, extracted via QuickOSM
- Query: waterway=  rivers, streams, drains and canal within Eti-Osa LGA extent
- Extracted: 12/09/2026
- 724 features, lines
- Coverage looks good in both built-up area and edges

## OSM coastline, extracted via QuickOSM
- Query: natural= coastline within Eti-Osa LGA extent
- Extracted: 12/09/2026
- 724 features, lines
- Coverage looks good in both built-up area and edges

## OSM Lagoon, extracted via QuickOSM
- Query: natural= water within Eti-Osa LGA extent
- Extracted: 12/09/2026
- 86 features, lines
- Coverage looks good in both built-up area and edges

## Elevation — Copernicus DEM (30 m) 
Source — https://portal.opentopography.org - Geotiff  
- Downloaded: 13/09/2026

## CRS and preparation
-All source layers arrived in EPSG:4326
-Study area: Eti-Osa L.G.A., Lagos State, Nigeria, extracted from GRID3 Settlements extent 4.1
-All layers reprojected and clipped to study area, EPSG:32632 (WGS84-UTM ZONE 32N)
-Area check: Eti-Osa L.G.A.: 177.932 square kilometers (does not match published figures which states that Eti-Osa has an area of 174.90 or 174.067 square km). so my computed area is about 3 square km larger than the published record
-working files in data/processed/, raw files untouched and not pushed to GitHub due to large file sizes. Only the processed files were pushed because they have manageable file sizes
