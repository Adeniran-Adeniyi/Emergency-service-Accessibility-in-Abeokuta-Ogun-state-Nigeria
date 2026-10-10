# Data Notes

**week 2 deliverable.** GeoDev Lab Africa, Cohort One. 

>  Author: Adeniyi Damilola Adeniran 
---

## Summary

| SN | Dataset | Type | Retriveed | Status|
|---|---|---|---|---|
| 1 | Administrative boundary level 3 | vector | August 20 | OK |
| 2 | Fire station | Vector | August 20 | OK |
| 3 | Police Station | vector | August 20 | ok |
| 4 | Road | vector | August 20 | Ok |

---

### GRID3 Nigeria Operational Local Government Area (LGA) Boundaries (administrative level 2)

* source: [GRID3](https://data.grid3.org/datasets/GRID3::grid3-nga-operational-wards-v3-0/about)
* Downloaded:Friday, September 4, 2026 5:30:38 PM
* Total size: 19 KB,
* CRS: EPSG:4326 - WGS 84
* 34 features, polygons
* columns:FID, Shape *, globalid, uniq_id, timestamp, editor, lganame, lgacode, statename, statecode, source, amapcode, Shape_Leng, Shape_Area
* No null in ward name
* cover my study area fully
  
``` 
QUARY : SELECT* FROM NGA_Ward WHERE "lganame" = 'Abeokuta South' OR "lganame" = 'Abeokuta North'
```
 
---


### OSM roads, Extracted via Quick OSM

* Source: [openstreetmap](https://www.openstreetmap.org/#map=9/7.278/3.441)
```
Quary: highway=* within Abk_north_south
```
* Extracted: Extracted date: Friday, September 4, 2026 8:31:38 PM
* Total size: (1.2 MB),
* CRS: EPSG:4326 - WGS 84
* 6461 features, lines
* many have no surface tag, so paved and unpaved can not be separeted everywhere
* Coverage looks good in the built-up area, sparse at the edge
---
  

### Police station 

* source: [GRID3](https://grid3.org/geospatial-data-nigeria)
* Downloaded:Friday, September 4, 2026 5:30:38 PM
* Total size: 19 KB,
* CRS: EPSG:4326 - WGS 84
* 802 features, point
* columns:globalid, uniq_id, timestamp, editor, scdy_edtor, wardname, wardcode, lganame, lgacode, statename, statecode, source, plc_st_nam
* No null in ward name
* cover my study area fully
--- 

  ###  Fire station
 
* source: [GRID3](https://grid3.org/geospatial-data-nigeria)
* Downloaded:Friday, September 4, 2026 5:30:38 PM
* Total size: 19 KB,
* CRS: EPSG:4326 - WGS 84
* 44 features, point
* columns: OBJECTID_1, latitude, longitude, global_id, ward_code, ward_name, lga_code, lga_name, state_code, state_name, poi_file_n, uniqueID
* No null in ward name
* cover my study area fully

--- 

 ### population 
 * source: [GRID3](https://grid3.org/geospatial-data-nigeria)
* Downloaded:Friday, September 4, 2026 5:30:38 PM
* Total size: 59.43 MB,
* CRS: EPSG:4326 - WGS 84
* raster, GeoTiff
* cover my study area fully

---

  **Status:** week 2 complete. Reprojection and quality check in Week 3, see [Data preparation](03-data-preparation.md)
  
