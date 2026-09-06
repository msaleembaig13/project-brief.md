# My Geodev - lab project

Which settlements in Dera Ghazi Khan District are more than 7 km by road from the nearest health facility, and where are the potential healthcare accessibility gaps?

### Why it matters.

Dera Ghazi Khan District contains a large number of rural and remote settlements, where access to healthcare can be affected by distance and road connectivity. Although health facilities exist across the district, the presence of a facility does not necessarily mean that surrounding communities can reach it easily.

Measuring straight-line distance can also give a misleading picture of accessibility because people travel along roads. Identifying settlements that are more than 7 km by road from their nearest health facility can help highlight potentially underserved communities, support healthcare infrastructure planning, and identify priority areas for improving access to essential health services.

### The data I need.

Dera Ghazi Khan District boundary: Polygon boundary defining the study area.

Tehsil boundaries: Administrative boundaries for analyzing healthcare accessibility across different tehsils.

Settlement locations: Point locations of villages, towns, and other settlements within Dera Ghazi Khan District.

Health facilities: Locations and types of hospitals, Basic Health Units (BHUs), Rural Health Centres (RHCs), dispensaries, and other healthcare facilities.

Road network: Connected road network covering the study area, required to calculate realistic road distance between settlements and health facilities.

Population data: Population distribution or settlement-level population estimates to understand the number of people potentially affected by poor healthcare accessibility.

### The data Source

Administrative boundaries – Humanitarian Data Exchange (HDX) / OCHA – https://data.humdata.org

Settlement locations – OpenStreetMap – https://www.openstreetmap.org

Health facilities – Open Data Pakistan, Pakistan Health Sites – https://opendata.com.pk/dataset/pakistan-health-sites

Road network – OpenStreetMap / Geofabrik – https://download.geofabrik.de

Population data – WorldPop – https://www.worldpop.org

### Methodology

I will map settlements and health facilities across Dera Ghazi Khan District and prepare the available road network for network analysis. Instead of using straight-line buffers, I will calculate the shortest road-network distance from each settlement to its nearest health facility.

The results will then be classified using the 7 km threshold:

0–7 km: Within the project accessibility threshold
More than 7 km: Potentially underserved

I will overlay the results with tehsil boundaries and population data to identify where healthcare accessibility gaps are concentrated and which areas may have the greatest potential impact.

### Tools I would use

QGIS / ArcGIS Pro – for spatial data preparation, network analysis, proximity analysis, mapping, and visualization.

Python / ArcPy – for automating data processing and analysis where appropriate.

OpenStreetMap / Geofabrik – for settlement and road-network data.

GitHub – for version control, project documentation, and sharing the project workflow.

### What I would build.

I would build an interactive Healthcare Accessibility Map and Dashboard for Dera Ghazi Khan District showing settlements, health facilities, road networks, and accessibility zones.

The dashboard would allow users to explore a settlement and identify its nearest health facility, the shortest road distance to that facility, and whether the settlement falls beyond the 7 km accessibility threshold.

The final product would provide a simple spatial decision-support tool for identifying potential healthcare gap areas and prioritizing locations for further investigation or infrastructure planning.

### Limitations

OpenStreetMap road and settlement data may be incomplete, particularly in remote or rural areas, and some health facilities may be missing or have outdated coordinates. Road-network distance also does not account for traffic, road conditions, seasonal accessibility, travel speed, or health-facility capacity.

The 7 km threshold is an analytical criterion for this project and should not be interpreted as an official healthcare accessibility standard without validation from relevant health authorities.

Field verification and more detailed population, road-condition, travel-time, and health-facility capacity data would strengthen the analysis.

### Project Status

Currently in the planning and data collection stage.
