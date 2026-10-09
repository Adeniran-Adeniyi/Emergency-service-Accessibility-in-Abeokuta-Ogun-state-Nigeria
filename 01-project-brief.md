# Project Brief

**Week 1 Deliverable.** GeoDev Lab Africa, Cohort One.

> **Author:** Adeniran Adeniyi Damilola

## 1. The Question

> Which areas in Abeokuta North and Abeokuta South have poorer access to emergency services, and how can GIS help us understand the problem?

## 2. Why This Matters

When an emergency happens, getting help quickly can make a big difference. However, emergency facilities may be far from some communities, and the road network may affect how easily emergency services can reach people.

Abeokuta North and Abeokuta South have different settlements, roads, population distributions, and emergency facility locations. Understanding how these factors relate to one another can help identify areas that may face accessibility challenges.

This project uses GIS and network analysis to examine the locations of fire and police stations, how they connect to communities through the road network, and which wards have longer travel distances to emergency facilities.

The aim is to provide spatial information that can support better emergency service planning.

## 3. Study Area

The study area covers two Local Government Areas in Ogun State, Nigeria:

- Abeokuta North
- Abeokuta South

The analysis focuses on the distribution of emergency facilities, the road network, and accessibility across the wards within these local government areas.

**Study Area Map:** Add a link to your emergency service study area map here.

## 4. What I Mean by the Terms

- **Emergency services:** Services such as fire and police services that respond to emergencies.
- **Emergency facilities:** The mapped locations of fire stations and police stations included in this project.
- **Accessibility:** How easily a location can be reached through the road network.
- **Travel distance:** The distance travelled along the road network between a starting point and an emergency facility.
- **Ward:** An administrative area used to examine differences in accessibility across the study area.
- **Network analysis:** A GIS method used to analyse routes, connectivity, and distances along a road network.

## 5. Where Each Dataset Comes From

| Data item | Source | Purpose |
|---|---|---|
| LGA administrative boundaries | [GRID3](https://data.grid3.org/datasets/2bb616a49ee84f409427cc2143787113_0/explore?location=9.077959%2C8.685290%2C5) | Define the study area |
| Ward boundaries | To be documented | Examine accessibility by ward |
| Road network | [OpenStreetMap](https://www.openstreetmap.org/) | Analyse routes and road-network distances |
| Fire stations | To be documented | Identify fire emergency facilities |
| Police stations | To be documented | Identify police facilities |
| Population data | To be documented | Understand the population potentially affected by accessibility challenges |

*The final data sources and formats will be documented after confirming the datasets used in the analysis.*

## 6. What "Done" Looks Like

The expected outcome is a set of maps and spatial analysis results showing the distribution of emergency facilities and differences in road-network accessibility across Abeokuta North and Abeokuta South.

The project aims to produce:

1. **Emergency Facilities Map** — showing the locations of fire and police stations.
2. **Road Network Map** — showing the road connections within the study area.
3. **Emergency Service Accessibility Map** — showing road-network distances between ward centroids and emergency facilities.
4. **Ward Accessibility Comparison** — identifying wards with longer travel distances.
5. **Population and Accessibility Map** — highlighting wards that may need further attention when population and accessibility are considered together.
6. **Closest Facility Analysis** — showing routes from selected ward centroids to nearby emergency facilities.

## 7. Note on Data Quality

The analysis depends on the quality and completeness of the available datasets.

OpenStreetMap will be used for road network data where appropriate, while administrative boundaries, emergency facility locations, and population data will be obtained from suitable sources.

The completeness of mapped emergency facilities may vary. Some facilities may be missing, and the road network may contain gaps or connectivity errors.

The analysis will also use ward centroids to represent starting locations. These points provide a consistent way to compare wards, but they do not represent the exact location of every resident.

**Important:** Road-network distance is not the same as actual emergency response time. Traffic, road conditions, vehicle availability, staffing, and dispatch procedures may also affect how quickly emergency services arrive.

## 8. Project Goal

The goal is to demonstrate how GIS can help answer an everyday question: **How easily can emergency services reach people who need them?**

By identifying differences in accessibility, the project aims to provide information that can support further investigation and more informed emergency service planning.

---

**Status:** Week 1 — Project brief.

**Next:** Week 2 — Data acquisition and documentation.

> Adeniran Adeniyi Damilola · GeoDev Lab Africa  
> *Learn. Build. Collaborate. Transform.*
