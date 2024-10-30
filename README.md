#  <p align="center">**Linear and Logistic Regression Analysis**</p>

# I. Introduction

## <p align="center">Linear Regression: *World Happiness Report*</p>

*<div align="justify">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Linear Regression* is a statistical analysis that is in common use in estimating the relationship between a one-dimensional dependent variable and the one or more independent variables. In the case of *World Happiness Report*, linear regression analysis can be of particular use to determine how socio-economic production measured through (GDP per capita), social support, health (life expectancy), freedom to make life choices, trust in government (perceived corruption), and generosity influence the overall happiness of a country. Through the examination of these relations, it is possible to determine how much each factor adds to the level of happiness of subjects of this analysis and how much level of happiness is likely to be estimated at different future points in time on the basis of these factors.</div>

## <p align="center">Logistic Regression: *Credit Card Fraud Detection*</p>

*<div align="justify">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Logistic Regression* is a statistical method used for binary classification problems. In the context of *Credit Card Fraud Detection*, the goal is to classify transactions as either "fraudulent" or "non-fraudulent." This technique works by modeling the probability that a given transaction belongs to a particular class based on various input features, such as time of transaction, some confidential features, and Transaction Amount.

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

<div align="justify">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The datasets used for this analysis are from the Credit Card Fraud Detection that contains transactions made by credit cards in September 2013 by European cardholders. The dataset includes several key variables that influence the class weather a transaction is "fraudulent" or "non-fraudulent", including:

  - **Time:** The time of transaction.

  - **V1-V28:** The confidential feature that are the principal components obtained with PCA.

  -  **Amount:** The transaction amount.

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

![image](https://github.com/user-attachments/assets/95df0593-5a86-4051-b75f-a195b09e821f)

X_train

![image](https://github.com/user-attachments/assets/58493d99-fe08-4033-9a92-cc8902eefac7)

X_test

![image](https://github.com/user-attachments/assets/25e2aae7-a21e-4ff8-9535-c3cb14fb542d)

y_train

![image](https://github.com/user-attachments/assets/732928af-bada-4ec4-af8a-628ef1b9c603)

y_test

![image](https://github.com/user-attachments/assets/4ec43156-0454-4b5c-a012-1386ce063b48)


## Part 2: Model Implementation: Use appropriate libraries (e.g., Scikit-learn in Python).

### **2.1. Building the model**

![image](https://github.com/user-attachments/assets/4151fe1a-b6dd-478d-b5fe-c2970b7c842c)

### **2.2 Training the Model**

![image](https://github.com/user-attachments/assets/1afb8315-e66f-4bf3-9c6d-0c57df2cb2b4)

### **2.3 Inference**

y_pred

![image](https://github.com/user-attachments/assets/16dda3f0-0732-4a6d-b6f5-0d0dbc987cf3)

y_test

![image](https://github.com/user-attachments/assets/50dc187b-cd0a-4ac6-a0e3-a95a34d8ba21)

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

The following steps outline the methodology used for this analysis:

## Part 1: Data Preprocessing: Encode categorical variables, balance classes if needed.

### **1.1 Importing Datasets** 

![image](https://github.com/user-attachments/assets/9a3374f2-bfca-4714-8d0a-c0e9a29137be)

![image](https://github.com/user-attachments/assets/4142ad78-b239-46bb-8874-e2ff3da765a6)

![image](https://github.com/user-attachments/assets/c377c948-dc9b-4111-95ab-323889467e1b)

### **1.2 Getting the Inputs and Outputs**

![image](https://github.com/user-attachments/assets/0e3304ae-fc69-45af-8482-935635aa39fa)

X

![image](https://github.com/user-attachments/assets/13fe3347-b2a3-4786-b439-79d3226a4dd9)

y

![image](https://github.com/user-attachments/assets/8bcd694b-f508-45b6-a41f-b57f9708d8f5)

### **1.3 Creating the Training Set and the Test Set**

![image](https://github.com/user-attachments/assets/aa9ca2e4-cffa-499f-98af-a2d3d7bbd20c)

X_train

![image](https://github.com/user-attachments/assets/bdaf326d-29a5-4fc2-b707-108ed0ff3c4a)

X_test

![image](https://github.com/user-attachments/assets/a63895dc-ac52-4c66-a45f-374ca87afb05)

y_train

![image](https://github.com/user-attachments/assets/61f64660-6f89-43fa-b7fb-96b1b0f3db1a)

y_test

![image](https://github.com/user-attachments/assets/c6c69f9c-7357-4cc9-ac40-502f2ccd9711)


### **1.4 Feature Scaling**

![image](https://github.com/user-attachments/assets/af34c60a-8fe3-41fa-96cf-24cbc7bb5418)

X_train

![image](https://github.com/user-attachments/assets/faa864fa-b971-4a20-b3f5-d246e5ff7e95)

## Part 2: Model Implementation: Use appropriate libraries.

### **2.1. Building the model**

![image](https://github.com/user-attachments/assets/be40c465-7541-47d7-8a66-ded140388f4f)

### **2.2. Training the Model**

![image](https://github.com/user-attachments/assets/efa7b273-65c7-4bf7-9695-a6461b85dd9c)

### **2.3. Inference**

![image](https://github.com/user-attachments/assets/a5b65d99-e0e1-46c4-9690-4bf5c3ae9dea)

y_pred

![image](https://github.com/user-attachments/assets/488951e9-69a8-45be-af3e-71f6a8612752)

y_test

![image](https://github.com/user-attachments/assets/a127a7fa-e21f-4dd0-ae98-18944dc4a286)

![image](https://github.com/user-attachments/assets/eb706f0c-e72d-43b0-a17d-485fb5b59bcd)
![image](https://github.com/user-attachments/assets/3b80e44f-f3e2-4887-8fa3-031a704bf0f5)

![image](https://github.com/user-attachments/assets/11c1d4b5-685b-4683-b9c1-e7940e71e5ce)
![image](https://github.com/user-attachments/assets/018bcfac-4498-4d39-9d7f-121b5d5fada9)

## Part 3: Evaluation Metrics: Calculate Accuracy.

### **3.1. Confusion Matrix**

![image](https://github.com/user-attachments/assets/1d7a9c25-0e33-44fb-813a-c67c64373d71)

### **3.2. Accuracy**

![image](https://github.com/user-attachments/assets/2288c8cd-2f6e-4652-803e-b4757600c963)

## 2. Results

## <p align="center">Linear Regression: *World Happiness Report*</p>

### Summary & Findings 
Inference 

y_pred
- These are the predicted happiness scores produced by the trained linear regression model for the same countries in the test set.

![image](https://github.com/user-attachments/assets/16dda3f0-0732-4a6d-b6f5-0d0dbc987cf3)

y_test
- This is the actual data from the test set.
  
![image](https://github.com/user-attachments/assets/8cc6a9c0-280f-44d8-8249-a5dd15e4fac8)

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

Inference 

y_pred
- These are the predicted class produced by the trained logistic regression model from the test set.

![image](https://github.com/user-attachments/assets/5632e852-8c3f-4169-a7fb-6d851805d27d)

y_test
- These are the actual data from the test set.

![image](https://github.com/user-attachments/assets/ad361706-482d-48cf-8549-90f1b5f1edab)

- In summary the y_pred values and y_test values are close to each other, it means that the model's prediction is accurate.

Interpretation
  
### Visualization

### Confussion Matrix Display

![image](https://github.com/user-attachments/assets/3fd837ff-f73c-4bd3-a155-3b9b2a3dfbc7)

<p align="center">
  <img src= "https://github.com/user-attachments/assets/d46c3b67-03e4-45ca-a83d-d39f37ba4da7"/>
</p>


- The model accurately identified 56,489 legitimate transactions. 
- The model wrongly identified 12 legitimate transactions as fraud, which can lead to customer inconvenience.
- The model failed to detect 20 fraudulent transactions, which is critical because these represent potential losses.
- The model successfully flagged 81 actual frauds. 

## 3. Discussion

# V. Reference

 - Wikipedia contributors. (2024b, October 15). Linear regression. Wikipedia. https://en.wikipedia.org/wiki/Linear_regression
 - World Happiness Report Link: https://www.kaggle.com/datasets/unsdsn/world-happiness 
 - Credit Card Fraud Detection Dataset Link: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud


Code Comments: Ensure all code is well-commented and readable.

Methodology: Document each step taken during analysis.

Results: Summarize findings and include tables or charts where appropriate.

Discussion: Reflect on the results, compare the two regression methods, and mention any limitations.
