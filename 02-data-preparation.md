# Data Preparation

**Week 3 Deliverable — GeoDev Lab Africa, Cohort One**

---

> **Author:** *Adeniran Adeniyi Damilola*

> This document explains how I prepared the spatial datasets for my Emergency Service Accessibility Analysis in Abeokuta North and Abeokuta South, Ogun State, Nigeria. It covers coordinate reference systems, extracting the study area, data preparation, quality checks, and the final outputs for network analysis.

---

## 1. Coordinate System Decisions

**Working CRS:** EPSG:32631 — WGS 84 / UTM zone 31N

> I used EPSG:32631 as the working coordinate reference system because the project involves measuring road-network distances and examining access to emergency facilities. This projected coordinate system uses metres, making it suitable for local distance analysis in the study area.

---

| Dataset                             | CRS as downloaded            | CRS after preparation | Operation                |
| ----------------------------------- | ---------------------------- | --------------------- | ------------------------ |
| Ward boundaries                     | EPSG:4326             | EPSG:32631            | Reprojected  |
| Road network                        | EPSG:4326             | EPSG:32631            | Reprojected  |
| Fire stations                       | EPSG:4326              | EPSG:32631            | Reprojected  |
| Police stations                     | EPSG:4326             | EPSG:32631            | Reprojected   |
| Ward centroids                      | Derived from ward boundaries | EPSG:32631            | Generated  |
| Population                       | EPSG:4326 | EPSG:32631            | Reprojected  |

---

> Reprojecting transforms coordinates from one coordinate reference system to another. Assigning a CRS only defines how existing coordinates should be interpreted; it does not transform them.
The datasets were prepared in a common CRS to support spatial overlay and network analysis.

---

## 2. Extracting the Study Area

The study area covers two local government areas in Ogun State, Nigeria:

* *Abeokuta North*
* *Abeokuta South*

---

> I used the administrative boundary data to identify and extract the two local government areas required for the project.
This reduced the geographical coverage to the study area and provided the boundary for preparing the remaining datasets.
The ward boundaries were also prepared to support accessibility analysis at ward level.

---


## 3. Clipping Datasets to the Study Area


| Dataset                   | Features before clipping | Features after clipping |
| ------------------------- | -----------------------: | ----------------------: |
| Ward boundaries           |       4044   |   42 |
| Road network              |     6461  |  6461 |
| Fire stations             |  44   |   11    |
| Police stations           |    802    |   1  |
| Population            |    raster        |     columns and row 502, 496    |

*Note: The feature counts should be updated using the actual results from the GIS processing.*

---

## 4. Preparing the Road Network and Emergency Facilities

### Road Network

> The road network was prepared for network analysis. I checked the spatial coverage and suitability of the road data for modelling routes between ward centroids and emergency facilities.

Road connectivity is important because the analysis estimates travel distance along the road network rather than straight-line distance.

---

### Emergency Facilities

> Fire and police station locations were prepared as destination points for the accessibility analysis.
Their locations were reviewed in relation to the study area to support the investigation of access from different wards.

---

### Ward Centroids

> Ward centroids were used to represent the wards as starting points for the Closest Facility analysis.
These points provide a consistent way to compare network distances between wards and emergency stations. However, a centroid does not represent the exact location of every resident within a ward.

---

## 5. The Five Quality Checks

I used five checks to review the prepared datasets before analysis.

| Quality check                                | Result          | Action taken                                 |
| -------------------------------------------- | --------------- | -------------------------------------------- |
| Is the CRS correct and consistent?           | yes | Reprojected datasets where required          |
| Are there missing values in required fields? | yes | Reviewed and corrected available information |
| Are there duplicate features?                | no | no action                      |
| Is the geometry valid?                       | yes | no action        |
| Does the data cover the entire study area?   | yes | no action                     |

---


## 6. Problems Found and Actions Taken

### Problem 1: Incomplete Spatial Data

*Some datasets are not contain in emergency facility within the study area.*

**Action:** The available datasets were reviewed and prepared for the analysis. 

---

### Problem 2: Road Network Connectivity

*A road network may contain disconnected segments or intersections that are not properly connected. These issues can affect route calculations.*

**Action:** The road network was prepared for network analysis, with connectivity requiring verification before the results are interpreted as realistic travel distances.

---

### Problem 3: Missing Attribute Information

*Some attributes required for analysis or interpretation may be incomplete.*

> **Action:** The available attribute information was reviewed. Missing values should only be filled when reliable information is available; otherwise, they should remain unknown.

---

## 7. Analysis-Ready Output

> The prepared datasets were organised for use in the emergency service accessibility analysis.

* **Output directory:** `data/processed/`
* **Format:** GeoPackage (`.gpkg`), 
* **Working CRS:** EPSG:32631
* **Software:** QGIS 
* **Preparation method:** GIS-based data preparation and quality checks

---

> The intended outputs include the study area boundary, ward boundaries, road network, fire station locations, police station locations, population and ward centroids.

---

## 8. What I Learned

This stage reinforced three important lessons:

 *Consistent coordinate systems matter.* Spatial datasets need compatible coordinate systems for accurate distance analysis.
*Data quality affects accessibility results.* Missing facilities, incomplete roads, and disconnected network segments can influence the results.
*Preparation comes before analysis.* Reliable network analysis depends on correctly prepared boundaries, roads, and emergency facility locations.

---
Preparing these datasets established the foundation for investigating how easily emergency services can reach different parts of Abeokuta North and Abeokuta South.

---

**Status:** Week 3 — Data preparation.

**Next:** Network analysis to investigate road-based accessibility to emergency facilities and identify wards with longer travel distances.

---

> Adeniran Adeniyi Damilola · GeoDev Lab Africa
> *Learn. Build. Collaborate. Transform.*
