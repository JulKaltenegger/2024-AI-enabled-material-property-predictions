# Evaluation of methods for AI-enabled material property predictions
This work evaluates methods for modelling and predicting building material information, including accounting for incomplete data. A conceptual process framework outlines a possible symbiosis between sub-symbolic and symbolic methods, addressing material properties and indicators. Finally, two use cases are introduced and (partially) implemented that predict material information (physical properties and environmental indicators).  

* Evaluation of Neuro-Symbolic AI in material property prediction
*	Conceptual Process Framework 
*	Early-stage implementation of studied methods [Use Case 1 and 2]


## Evaluation of Neuro-symbolic AI methods
Neuro-symbolic AI methods are investigated to work with different data sources, modelling, predicting material property data, and validating the results. The aim is to find a symbiosis of data-driven (sub-symbolic) and knowledge-driven (symbolic) approaches in both modelling and predicting building material information.

The research fields indicated in the table below are selected to review the state of the art in material property data modelling and prediction. The data modelling, studying semantic analysis and concept definitions, address Natural language processing (NLP) and semantic knowledge graphs. The property prediction discusses Machine Learning (ML) and Artificial Neural Networks (ANN) tasks. Knowledge graph inference and link prediction are also studied. Further references can be found in the 'LiteratureList.xlsx'.


|  | Data source processing | Data modelling | Data prediction and population | Data validation and storage |
| :-----------------: | :----------: | :----------: | :--------: | :--------: |
| | Extract Transform Load | Semantic analysis and concept definition | Data-driven and logic approach | Exploration |
| Sub-Symbolic AI | Feature engineering, Imputation and Missing Values | Natural Language Processing (NLP) | Machine Learning (ML) and Artificial Neural Networks (ANN) | Model Evaluation |
| Symbolic AI | Knowledge Engineering and Ontology | Semantic Knowledge Graph | Knowlegde Graph inference, Link prediction, Description Logic | Resolution-based reasoning |

## Conceptual Process Framework
The process framework takes up the previous research fields and relates them to each other. This way, methods of both AI subdomains (sub-symbolic and symbolic) can be designed to interact with each other throughout the data modelling and prediction steps.

- (I)	 Data processing handles data sources in various file formats and applies knowledge engineering and feature engineering simultaneously. Statistically significant features are acknowledged as part of domain knowledge engineering and can be integrated as a concept within a domain-specific knowledge graph. NLP is utilised to detect semantic similarities between various concepts that are defined throughout multiple (open) data models. As such, domain-specific knowledge graphs can be interlinked in a flexible contextual model and thus can respond to specific use cases.
- (II) Data prediction addresses missing information in individual data sources and missing links between concepts that describe materials and buildings in various aggregations and scales. ML and ANN (sub-symbolic) train prediction models and eventually forecast material property data per material type in a building use-specific context. Knowledge graphs and logic (symbolic) are used to shape rules and conditions. Missing data and links can be predicted, and by that, complex reasoning challenges can be overcome. For instance, material performances for a specific type of building in a specific climate region can be predicted under certain probabilities following conditional rules and data-driven forecasts. As such, quantitative property predictions enrich a qualitative multi-scalar material information knowledge graph.

<div align="center">
<img src="https://github.com/user-attachments/assets/477e815b-7ffb-49a6-9ddf-d4358aa40d42" alt="Concept Diagram" />
</div>

## Early-stage implementation of studied methods

An early-stage experiments is tested against two uses cases addressing symbolic methods to analyse semantics and capture domain knowledge and sub-symbolic methods, to predict material properties, see figure below.The aim is to enrich material type definitions for a building model with material physical properties and predict the life cycle indicators to compute environmental performance assessments on a building element level.

The first use case studies material physical property prediction (data source: ASHRAE), and the second use case studies environmental impact predictions (data source: SLiCE). The suggested implementation framework addresses knowledge engineering to detect domain-specific concepts that are used as input for the ML models. The accuracy of data-driven ML results strongly depends on the quality and quantity of available data. Therefore, feature engineering methods and imputing missing data, using simple and iterative imputations are studied. Prediction models are studied utilising supervised multiple regression and a multilayer feed-forward network as modelling tasks. Model evaluation criteria are utilized to assess the predictive capacity of the proposed learning algorithms. 

Both data sets show multi scalar information structure, as SLICE and ASHREA represent different scale. SLiCE is based on a building element level, while ASHRAE is based on material level.

<div align="center">
<img src="https://github.com/user-attachments/assets/9fa062de-9113-4130-93fb-fce8b3d6634c" alt="image2" width="75%"  />
</div>