#  Use Case 2 - Prediciton of Material Environmental Indicator

### Use Case Specification
This use case specifies on the semantic definition, modelling, and prediction of materials environmental performance indicators.

### Data Source
The SLiCE data model provides information to material’s and building element’s environmental impacts. SLiCE (Röck et al., 2023) is developed as a tool for systematic analysis of environmental hotspot across the life cycle of buildings and construction elements using data compliant with the SLiCE building data model.

### Conceptual Model
<img src="https://github.com/user-attachments/assets/ecdc23a9-21be-4fb6-8b10-6abbbfbd6f87" alt="Concept Model" width="50%" />


### ANN integration pipeline
ANN is choose due to handling more complex, non-linear relationship and bigger among of data. The missing values are dismissed and feature engineering is applied to analyse the significancy of the features relationships using the data variance, the level of relevant information contained within a variable in relation to the others. It reduced the number of features (the impact category) from 27 to 8.Furhtermore, the string values, such as material names are encoded to an multi-dimensional array to include the full information per material property record.

Two prediction models are selected that include the training and the evaluation of the model.
**Multilayer perceptron (MLP) neural network**
This use case studies the neural network feedforward architecture, using the library Keras and Tenser flow.

**Support Vector Machine (SVM)**

![Integration Pipeline](https://github.com/user-attachments/assets/727e3884-3cf8-48b3-a528-9cfd4b479646)



### Data quality
##### Data source
Data definitions and calculations follow EN 15978 
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

## FAIR Analysis
### Findable
URI: https://github.com/mroeck/slice_hotspots/tree/develop
### Accessible:
### Interoperable:
### Reusable:
