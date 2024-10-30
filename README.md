#  <p align="center">**Linear and Logistic Regression Analysis**</p>

# I. Introduction

## <p align="center">Linear Regression: *World Happiness Report*</p>

*<div align="justify">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Linear Regression* is a statistical analysis that is in common use in estimating the relationship between a one-dimensional dependent variable and the one or more independent variables. In the case of *World Happiness Report*, linear regression analysis can be of particular use to determine how socio-economic production measured through (GDP per capita), social support, health (life expectancy), freedom to make life choices, trust in government (perceived corruption), and generosity influence the overall happiness of a country. Through the examination of these relations, it is possible to determine how much each factor adds to the level of happiness of subjects of this analysis and how much level of happiness is likely to be estimated at different future points in time on the basis of these factors.</div>

## <p align="center">Logistic Regression: *Credit Card Fraud Detection*</p>

# II. Dataset Description

## <p align="center">Linear Regression: *World Happiness Report*</p>

<div align="justify">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The datasets used for this analysis are from the World Happiness Reports spanning from 2015 to 2019. Each dataset includes several key variables that influence a country’s happiness score, including:</div>

- **Happiness Score:** The overall score that ranks the happiness level of each country based on survey data.

- **Economy (GDP per Capita):** A measure of the economic output per person in a country, used to assess the material well-being of citizens.

- **Family (Social Support):** The level of support available to individuals from family, friends, or social networks.

- **Health (Life Expectancy):** The expected lifespan of individuals in each country.

- **Freedom to Make Life Choices:** The degree of personal freedom individuals have in making life decisions.

- **Trust (Government Corruption):** The perceived level of corruption in a country’s government and institutions.

- **Generosity:** The amount of charitable donations and overall generosity within the population.

- **Dystopia Residual:** A hypothetical measure representing the worst possible scenario of a country in terms of these factors, used as a baseline for comparison.

## <p align="center">Logistic Regression: *Credit Card Fraud Detection*</p>

# III. Project Objectives

1. To apply Linear Regression analysis in predicting outcomes based on a continuous dependent variable by performing data preprocessing, model implementation, and evaluating the model's predictive performance using metrics such as R-squared and Mean Squared Error.

2. To interpret the coefficients and predictive power of the Linear Regression model, explaining the relationship between the independent and dependent variables.

3. To execute Logistic Regression analysis for classifying outcomes of a categorical dependent variable through data preprocessing, model implementation, and evaluation using accuracy and confusion matrices.

4. To assess the classification performance of the Logistic Regression model and discuss the importance of features in influencing the predicted outcomes.

# IV. Documentation

## 1. Methodology

## <p align="center">Linear Regression: *World Happiness Report*</p>

The following steps outline the methodology used for this analysis:

## Part 1: Data Preprocessing: Handle missing values, outliers, and normalize data if necessary.

### **1.1 Importing Datasets** 

![image](https://github.com/user-attachments/assets/f906f83a-6599-45b6-a8cd-8e7bb3291a93)

![image](https://github.com/user-attachments/assets/6984e566-da2c-4fbf-9e97-3d6b7f468356)

### **1.2 Checking for missing values in the datasets**

![image](https://github.com/user-attachments/assets/db3ad7fe-8f98-4cca-b429-69dc58e0b12d)

### **1.3 Standardizing features**

![image](https://github.com/user-attachments/assets/b846f332-6c87-4c77-a0cc-f228fe136028)

![image](https://github.com/user-attachments/assets/ce5aa007-ff9c-418c-aa74-df8c67d40518)

### **1.4 Getting the Inputs and Outputs**

Independent Variables

![image](https://github.com/user-attachments/assets/b51d1ea1-d341-418c-93a3-92138a14f4a8)

Dependent Variables

![image](https://github.com/user-attachments/assets/e3f356bf-0043-4632-8106-a2e488982229)

### **1.5 Creating the Training Set and the Test Set**

![image](https://github.com/user-attachments/assets/09e91773-b674-403f-8513-c9c7c85920d4)

X_train

![image](https://github.com/user-attachments/assets/b56fb5e3-6386-4853-a4bd-32fa8160628d)

X_test

![image](https://github.com/user-attachments/assets/c7805bc7-baa5-4eac-8652-86298928bb3e)

y_train

![image](https://github.com/user-attachments/assets/9f5edc9f-7068-455f-b1c7-9262a55d0ce7)

y_test

![image](https://github.com/user-attachments/assets/4d7eab36-180c-4966-866e-830cea996f55)


## Part 2: Model Implementation: Use appropriate libraries (e.g., Scikit-learn in Python).

### **2.1. Building the model**

![image](https://github.com/user-attachments/assets/4151fe1a-b6dd-478d-b5fe-c2970b7c842c)

### **2.2 Training the Model**

![image](https://github.com/user-attachments/assets/1afb8315-e66f-4bf3-9c6d-0c57df2cb2b4)

### **2.3 Inference**

y_pred

![image](https://github.com/user-attachments/assets/e08e3e16-7bbf-429a-b1d6-86947d87894c)

y_test

![image](https://github.com/user-attachments/assets/4e839acf-6de0-4b5e-a8dc-9d1645bde44c)

## Part 3: Evaluation Metrics: Calculate R-squared, Mean Squared Error, etc.

### **3.1 R-Squared**

![image](https://github.com/user-attachments/assets/42bbf008-3aa4-4e1b-bda0-8cda4f2b24f1)

### **3.2 Adjusted R-Squared**

![image](https://github.com/user-attachments/assets/2d0b729b-885d-478a-b602-117286ec9420)

### **3.3 Mean Squared Error**

![image](https://github.com/user-attachments/assets/5365cf57-6beb-4e85-8cf5-7d47ce933b96)

## Part 4: Interpretation: Explain the significance of coefficients and the model's predictive power.

![image](https://github.com/user-attachments/assets/f35e1b0d-687e-4093-ace6-cbc0e592921a)

## <p align="center">Logistic Regression: *Credit Card Fraud Detection*</p>


## 2. Results

## <p align="center">Linear Regression: *World Happiness Report*</p>

### Summary & Findings 
Inference 

y_pred
- These are the predicted happiness scores produced by the trained linear regression model for the same countries in the test set.

![image](https://github.com/user-attachments/assets/5d907c00-3796-43b5-bdea-57f0cf295947)

y_test
- This is the actual data from the test set.
  
![image](https://github.com/user-attachments/assets/f881c2aa-1ee2-483e-8f13-1cf85bd95b96)

- In summary the y_pred values and y_test values are close to each other, it means that the model's prediction is accurate. 

R-Squared

![image](https://github.com/user-attachments/assets/ea030447-62a3-439d-a7cc-3c8b3255ce9f)

- This picture shows that 99.99999035357195 percent, which means that the independent variable is a good fit to explain the variation in the dependent variable.

Mean Squared Error

![image](https://github.com/user-attachments/assets/54ba719b-d256-4c74-a4fe-2b2b219625df)

- This picture shows the difference between actual and predicted values, and the values that we acquired is np.float64(9.863758664533044e-08).

Interpretation

![image](https://github.com/user-attachments/assets/9a510d72-d230-40be-87aa-5131503748e0)

- This picture show how much the dependent variable (Happiness Score) is expected to increase when the corresponding independent variable increases. Positive coefficients indicate a positive impact on happiness and Negative coefficients indicate a negative impact on happiness.
- In this case the results that we obtain in Economy	is 1.000103, means that countries with higher GDPs tend to have higher happiness scores.
- Family	is 0.999954, means that strong family tends to have higher happiness scores.
- Health	is 0.999862, means that having a better health contribute to happiness and it just same in the Freedom, Trust, Generosity, and Dystopia Residual

### Visualization

### Actual vs. Predicted Happiness Score

![image](https://github.com/user-attachments/assets/c7a5e1e7-bf85-4843-a38b-b92428b1cec5)

<p align="center">
  <img src="https://github.com/user-attachments/assets/fb04fc4b-a815-4d5b-bcc5-be7fe53d2490"/>
</p>

- This plot compares the actual happiness scores from the test data with the predicted scores from the model.
- The red line represents the line of perfect prediction (where actual = predicted).
- Since the point is on line, it means that the model's prediction of Happiness Score is somewhat equal to the actual value.

## <p align="center">Logistic Regression: *Credit Card Fraud Detection*</p>

### Summary & Findings 

### Visualization

## 3. Discussion

# V. Reference

 - Wikipedia contributors. (2024b, October 15). Linear regression. Wikipedia. https://en.wikipedia.org/wiki/Linear_regression
 - World Happiness Report Link: https://www.kaggle.com/datasets/unsdsn/world-happiness 
 - Credit Card Fraud Detection Dataset Link: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud


Code Comments: Ensure all code is well-commented and readable.

Methodology: Document each step taken during analysis.

Results: Summarize findings and include tables or charts where appropriate.

Discussion: Reflect on the results, compare the two regression methods, and mention any limitations.
