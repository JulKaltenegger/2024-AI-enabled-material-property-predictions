#  Use Case 1 - Prediction of Material Physical Property 
### Use Case Specification
This use case specifies on the semantic definition, modelling, and prediction of materials physical properties. Physical material properties are fundamental cornerstone to detect thermal resistance, structural integrity and in further perspective the life cycle inventories for environmental impact assessments. 

### Data source
The 2021 ASHRAE Handbook—Fundamentals is chosen as it covers basic set of building materials and property data used in the HVAC&R industry. It covers thermodynamics, psychrometrics, and heat transfer, and provide practical guidance on building envelope, indoor environmental quality, load calculations, duct and piping system design, refrigerants, energy resources, sustainability, a new chapter on climate change, and more. In particular it contains material physical properties, including material density (ρ) (kg/m3), conductivity (λ) (W/m⋅K), and specific heat capacity (⁠J/kg⋅K).

### Conceptual Model
The following conceptual model is designed:
(a) inputs (Xn) are the independent variables (material name, material conductivity, material specific heat capacity)
(b) outputs (Yn) is the dependent variables (material density)

<img src="https://github.com/user-attachments/assets/3f027f15-99f7-4fa7-8c2f-ac93fb0fbf1c" alt="Concept Model" width="50%" />

### Regression ML model
Further, regression is chosen because of a forecast task using continues data. The task is composed of two steps: the data source processing, during which the relationship between data points and known labels is understood as well as the missing values are treated. The second step, the prediction step, a probabilistic process that uses the above mentioned dataset to train a linear regression model.

![Integration Pipeline](https://github.com/user-attachments/assets/9baf1bae-05b6-47be-8eed-8f87c2dbcda6)

The goal of this ML method is to fit a linear model with the feature’s coefficients β1..βn to minimize the residual sum of square between the observed and the predicted linear approximation of the dependent variable ŷ. The following assumptions yield.

**Linear regression:** Null Hypothesis H_0: we assume linearity. Loss Function (L_0) Mean Square error (MSE) is the sum of the squared vertical distances between the predicted and the true values. 
**Regularized Linear Regression:** Uses the same hypothesis and loss functions but uses a regularization term in the loss function to prevent overfitting. A penalty term, that shrinks the value of feature weights, thus preventing values to be too closely fitted to the training data. Three regulasiation terms are: **Lasso**, **Ridge**, and **Elasticnet**.
**Kernel Ridge Regression (KRR):** The same ridge loss is used, but the hypothesis function consists in a Kernel function which allows to capture non-linearities. When relations between data are non- linear, Kernel functions allow to remap features to a high-dimensional space, where their behavior becomes linear. Three Kernel functions are compared: **Linear (LIN)**, **Polynomial (POL)** and **Radial Basis Function (RBF)**.


## FAIR Analysis
### Data quality
### Findable
URI: https://app.knovel.com/kn/resources/kpCK08G9X5/toc?filter=table
### Accessible:
Via University library
### Interoperable:
CSV file forma, can be read locally only
### Reusable:
CSV file to be downloaded and reused. The data file format need to be changed for metrics.
