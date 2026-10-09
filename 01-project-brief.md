# Data Notes

**week 2 deliverable.** GeoDev Lab Africa, Cohort One. 

>  Author: Adeniyi Damilola Adeniran 

## Summary

| SN | Dataset | Type | Retriveed | Status|
|---|---|---|---|---|
| 1 | Administrative boundary level 3 | vector | August 20 | OK |
| 2 | Fire station | Vector | August 20 | OK |
| 3 | Police Station | vector | August 20 | ok |
| 4 | Road | vector | August 20 | Ok |



### GRID3 Nigeria Operational Local Government Area (LGA) Boundaries (administrative level 2)

* source: [GRID3]()
* Downloaded:Friday, September 4, 2026 5:30:38 PM
* Total size: 19 KB,
* CRS: EPSG:4326 - WGS 84
* 6 features, polygons
* columns:ID_0, ISO, NAME_0, ID_1, NAME_1, ID_2, NAME_2, TYPE_2, ENGTYPE_2, NL_NAME_2, VARNAME_2
* No null in ward name
* cover my study area fully
  


### OSM roads, Extracted via Quick OSM

* Source: [openstreetmap]()
* Quary: highway=* within Abeokuta zone
* Extracted: Extracted date: Friday, September 4, 2026 8:31:38 PM
* Total size: (1.2 MB),
* CRS: EPSG:4326 - WGS 84
* 5,551 features, lines
* many have no surface tag, so paved and unpaved can not be separeted everywhere
* Coverage looks good in the built-up area, sparse at the edge

  

### Police station 

* source: [GRID3]()
* Downloaded:Friday, September 4, 2026 5:30:38 PM
* Total size: 19 KB,
* CRS: EPSG:4326 - WGS 84
* 6 features, point
* columns:ID_0, ISO, NAME_0, ID_1, NAME_1, ID_2, NAME_2, TYPE_2, ENGTYPE_2, NL_NAME_2, VARNAME_2
* No null in ward name
* cover my study area fully
  

  ###  Fire station
  
* source: [GRID3]()
* Downloaded:Friday, September 4, 2026 5:30:38 PM
* Total size: 19 KB,
* CRS: EPSG:4326 - WGS 84
* 6 features, point
* columns:ID_0, ISO, NAME_0, ID_1, NAME_1, ID_2, NAME_2, TYPE_2, ENGTYPE_2, NL_NAME_2, VARNAME_2
* No null in ward name
* cover my study area fully


  **Status:** week 2 complete. Reprojection and quality check in Week 3, see [Data preparation](03-data-preparation.md)
  
