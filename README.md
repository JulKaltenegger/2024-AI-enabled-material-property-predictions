# Evaluation of methods for AI-enabled material property predictions
This work evaluates modelling and predicting building material information methods, including accounting for incomplete data. A conceptual process framework outlines a possible symbiosis between sub-symbolic and symbolic methods, addressing material properties and indicators. Finally, two use cases are introduced and (partially) implemented that predict material information (physical properties and environmental indicators).  

* Evaluation of Neuro-Symbolic AI in material property prediction
*	Conceptual Process Framework 
*	Early-stage implementation of studied methods [Use Case 1 and 2]


## Evaluation of Neuro-symbolic AI methods
Neuro-symbolic AI methods are investigated that deal with working with different data sources, modelling, predicting material property data, and validating the results. The aim is to find a symbiosis of data-driven (sub-symbolic) and knowledge-driven (symbolic) approaches in both modelling and predicting building material information.

Four research fields are chosen to review the state of the art in material property data modelling and prediction. The data modelling, addressing semantic analysis and concept definitions, discuss Natural language processing (NLP) and semantic knowledge graphs. The property prediction discusses Machine Learning (ML) tasks and Artificial Neural Networks (ANN) tasks. Besides the sub-symbolics, also symbolic inference on knowledge graph is studied. 
Further references cam be found in the 'LiteratureList.xlsx'.


| Method | Data Source | Data modelling | Data prediction and population | Data validation and storage |
| :-----------------: | :----------: | :----------: | :--------: | :--------: |
| | Extract Transform Load | Semantic analysis and concept definition | Data-driven and logic approach | Exploration |
| Sub-Symbolic AI | Feature engineering, Imputation and Missing Values | Natural Language Processing (NLP) | Machine Learning (ML) and Artificial Neural Networks (ANN) | Model Evaluation |
| Symbolic AI | Knowledge Engineering and Ontology | Semantic Knowledge Graph | Knowlegde Graph inference, Link prediction, Description Logic | Resolution-based reasoning |

## Conceptual Process Framework
The process framework takes up the previous divisions and puts them in relation and order to each other. In this way, both subdomains can be designed to interact with each other throughout the data modelling and prediction steps.

- (I)	The data processing handles data sources in various file formats and applies knowledge engineering and feature engineering in parallel. Statistically significant features are acknowledged as part of domain knowledge engineering and can be integrated as concept within a domain-specific knowlegde graph. NLP is utilised to detect semantic similarities between various concept that are defined throughout various (open) data models. As such, a multi dimensional property enrichment for material types in a specific building context is enabled.
- (II) The data prediction addresses missing information as part of individual data sources as well as missing links between information models for materials and buildings. ML and ANN (sub-symbolic) are used to predict missing material properties, and knowledge graphs and logic (symbolic) are used to shape rules that enable the linking of multi-scalar material information.

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






