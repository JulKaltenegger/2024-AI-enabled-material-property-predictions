#  Use Case 2 - Prediciton of Material Environmental Indicator
Data Source: SLiCE Hotspot analysis 



## FAIR Analysis

### Data quality

##### Data source
Data definitions and calculations follow EN 15978 (Röck et al., 2023)
##### Terminology 

| Terminology | Class |  Instance | 
| :-----------------:   | :----------: | :----------: |
|Spatial attribute (keys)|  |"EW05 CLT + str blown" 
| Element   | ElementName |  "21"
| Element | ElementClassification |"Wall - external finish, Cladding, Panel, Cork (32-80 mm)" 
| Worksection | WorksectionName |  "Cork (32-80mm)"
| Product/Propcess | ActivityName |  "Cork slab {RER}| production | Alloc Rec, U"
| TechflowName | TechflowName |
|Temporal attribute (keys)| |
| LifeCycleStage | LCSName |  "A1-3: Product stage"
| LifeCycleModule | LCMCode |  "A1-3"
| PointInTime | ActivityYear | "0"
| ActivityType | ActivityType | "Material in"
| Indicator Attributes (values) |      |
| LCIamounts | techflowAmount | "11.2"
| LCIamounts | TechflowUnit | "tkm"
| LCIA results | indicatorGWP | "15.7813488"
| LCIA results | indicator_PM | "0.0143808"
| LCIA results | indicator_EP | "0.0098672"

##### Completeness 
(Number of empty value)
fully open to public, missing value for all indicators: 2014/6195

#####  Relevance 
(What is the purpose of the data, how can we use it)
A tool for systematic analysis of environmental hotspot across the life cycle of buildings and construction elements using data compliant with the SLiCE building data model.

##### Reliability 
(Are the indicator definition and data collection and analysis processes clear and are these consistently applied over time)
Indicators used are in line with LCA standardisations, follow EN 15978.

### Findable

URI: https://github.com/mroeck/slice_hotspots/tree/develop

### Accessible:

### Interoperable:

### Reusable:
