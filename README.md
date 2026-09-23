# Data notes



### Dera Ghazi Khan District Boundary



Source: Humanitarian Data Exchange (HDX) / OCHA — https://data.humdata.org

Study area: Dera Ghazi Khan District, Punjab, Pakistan

Geometry: Polygon

CRS: EPSG:4326 (WGS 84)

Study area extracted from the Pakistan administrative boundary dataset (pakadm)

The district boundary was used to define the project study area

Completeness: The district boundary provides full coverage of the study area

Positional: The boundary was reviewed in QGIS and aligns with the prepared spatial datasets

Fitness: It is fit for defining the study area and clipping the other project datasets



### Tehsil Boundaries



Source: Humanitarian Data Exchange (HDX) / OCHA — https://data.humdata.org

Study area: Dera Ghazi Khan District

Geometry: Polygons

CRS: EPSG:4326 (WGS 84)

Used to analyze healthcare accessibility patterns across different tehsils

Completeness: The available tehsil boundaries cover the study area

Positional: The boundaries were reviewed against the district study area

Attribute: Contains administrative information required for tehsil-level analysis

Fitness: It is fit for summarizing and comparing healthcare accessibility across tehsils



### Settlement Locations



Source: OpenStreetMap — https://www.openstreetmap.org

Study area: Dera Ghazi Khan District

Geometry: Points

CRS: EPSG:4326 (WGS 84)

Used to represent villages, towns, and other settlements

Completeness: Settlement coverage may be incomplete, particularly in remote and rural areas

Currency: OpenStreetMap data is continuously updated; the download date should be recorded with the final dataset

Positional: Settlement locations should be reviewed against satellite imagery where necessary

Attribute: Settlement names and available settlement information are used to identify individual locations

Fitness: It is fit for the project accessibility analysis, subject to limitations in rural settlement coverage



### Health Facilities



Source: Open Data Pakistan — Pakistan Health Sites — https://opendata.com.pk/dataset/pakistan-health-sites

Study area: Dera Ghazi Khan District

Geometry: Points

CRS: EPSG:4326 (WGS 84)

Used to represent healthcare facilities within the study area

Facility types may include hospitals, Basic Health Units (BHUs), Rural Health Centres (RHCs), dispensaries, and other healthcare facilities

Completeness: The dataset may not contain every health facility currently operating in the study area

Positional: Facility locations should be reviewed against available reference imagery or other authoritative sources

Attribute: Facility names and available facility-type information support the healthcare accessibility analysis

Fitness: It is fit for identifying potential healthcare access points, subject to completeness and positional limitations



### Roads



Source: OpenStreetMap / Geofabrik — https://download.geofabrik.de

Study area: Dera Ghazi Khan District

Geometry: Lines

CRS: EPSG:4326 (WGS 84)

Used to construct the road network for shortest-path accessibility analysis

Completeness: Road coverage may be incomplete in some rural and remote areas

Currency: OpenStreetMap road data is continuously updated; the download date should be recorded with the final dataset

Positional: Road geometries should be reviewed against satellite imagery where necessary

Attribute: Available road classifications and road-network attributes support network preparation

Fitness: It is fit for road-network distance analysis, subject to network completeness and connectivity limitations



### Population Data



Source: WorldPop — https://www.worldpop.org

Study area: Dera Ghazi Khan District

Geometry: Raster

CRS: Dataset-dependent; reprojected to the project working CRS during processing

Used to estimate the population potentially affected by healthcare accessibility gaps

Completeness: Population coverage is available as a spatial population surface

Currency: The selected WorldPop year should be recorded with the final dataset

Positional: Population estimates are represented spatially through the raster grid rather than individual population locations

Attribute: Population values represent estimated population counts/density according to the selected WorldPop product

Fitness: It is fit for estimating the potential population impact of identified accessibility gaps, subject to the limitations of gridded population estimates



### CRS and Preparation



All source vector data arrived in EPSG:4326 (WGS 84)

Study Area: Dera Ghazi Khan District, extracted from the pakadm administrative boundary dataset

All relevant layers were reprojected to EPSG:32643 (WGS 84 / UTM Zone 43N)

Spatial layers were clipped to the Dera Ghazi Khan District study area

Area Check: The Dera Ghazi Khan district boundary was reviewed to confirm that the prepared study area and spatial datasets align correctly

The projected CRS provides a metric coordinate system suitable for subsequent distance and network analysis

Working files are stored in data/processed/


Raw source files remain untouched in data/raw/

Prepared data will be used for the next stage of healthcare accessibility analysis
