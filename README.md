#  <p align="center">**Linear and Logistic Regression**</p>

# I. Introduction

## <p align="center">Linear Regression: *World Happiness Report*</p>

*<div align="justify">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Linear Regression* is a statistical analysis that is in common use in estimating the relationship between a one-dimensional dependent variable and the one or more independent variables. In the case of *World Happiness Report*, linear regression analysis can be of particular use to determine how economic production measured through Gross Domestic Product per Person – GDPPP, social support, health of a nation measured by life expectancy, freedom of an individual to make choices regarding his life, government credibility gauged by perceived corruption and citizens’ generosity are interrelated and affect the overall happiness of a certain country. Through the examination of these relations, it is possible to determine how much each factor adds to the level of happiness of subjects of this analysis and how much level of happiness is likely to be estimated at different future points in time on the basis of these factors.</div>

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

# IV. Documentation

## 1. Methodology

## <p align="center">Linear Regression: *World Happiness Report*</p>

The following steps outline the methodology used for this analysis:

## Part 1: Data Preprocessing: Handle missing values, outliers, and normalize data if necessary.

### **1. Importing Datasets** 

<p align="center">
  <img src="https://github.com/user-attachments/assets/90cfe5d6-af20-4af5-b23e-d1f25ad6c30d"/>
</p>

**Data_2015**

![image](https://github.com/user-attachments/assets/87b71d46-98ba-48f8-b4f8-21e89827bed1)

**Data_2016**

![image](https://github.com/user-attachments/assets/b767386a-21ec-40c8-a883-235013f5c437)

**Data_2017**

![image](https://github.com/user-attachments/assets/69f8faa0-497a-4157-98d8-3ffdc66fc9e2)

**Data_2018**

![image](https://github.com/user-attachments/assets/c9fbc323-c877-44cb-9d37-6efe9f924e81)

**Data_2019**

![image](https://github.com/user-attachments/assets/e8dafab5-b8f4-46bc-9331-f74758bc219d)

### **2. Checking for missing values in the datasets**

<p align="center">
  <img src="https://github.com/user-attachments/assets/d826cae1-1287-4fc3-ae77-4d7a79cc3330"/>
</p>

**Data_2015**

![image](https://github.com/user-attachments/assets/21dd090c-f013-4c46-ada3-74ed50e42fd1)

**Data_2016**

![image](https://github.com/user-attachments/assets/b923507b-5372-4f90-8af0-9726fa0ef07f)

**Data_2017**

![image](https://github.com/user-attachments/assets/f3005fbf-fa19-48bd-a378-bb8d17068494)

**Data_2018**

![image](https://github.com/user-attachments/assets/1449a3f2-ed8d-4ccf-ac38-46ec2cf8d824)
      
### Since there is one null in the Perception of corruption in the Data_2018, we need to fix it.

### 2.1 Impute the missing value with the mean of the column

![image](https://github.com/user-attachments/assets/bc86b603-597b-45a4-9ab9-b54adc3cf68d)

### 2.2 Verify that there are no more missing values

![image](https://github.com/user-attachments/assets/e0fc4123-d013-4bcd-b58b-fe6a08a3897c)

**Data_2019**

![image](https://github.com/user-attachments/assets/98567014-7e50-44a9-87e4-89bd5e3ad7d5)

### **3. Standardizing features**

![image](https://github.com/user-attachments/assets/3ff3789c-5838-4350-a374-27b8a3e22592)

![image](https://github.com/user-attachments/assets/d9329ca5-524d-498d-a6a8-f93927ee9923)

### **3.1 Extracting the dependent variable (Happiness Score)**

![image](https://github.com/user-attachments/assets/ddf11495-d4ab-4013-a8b5-b7335137375d)

### **3.2 Displaying the standardized data**

![image](https://github.com/user-attachments/assets/089a7674-a134-494b-986b-926c558ad3d9)

### **4. Getting the Inputs and Outputs

**Data_2015_Inputs**

![image](https://github.com/user-attachments/assets/44afec4a-a659-4130-816f-0684214fdb54)

**Data_2015_Outputs**

![image](https://github.com/user-attachments/assets/915eb236-c32d-4574-827a-c9fa57e139cc)

**Data_2016_Inputs**

![image](https://github.com/user-attachments/assets/3e4cd442-3a65-45c4-8e06-5bed90ddaf66)

**Data_2016_Outputs**

![image](https://github.com/user-attachments/assets/c37acee9-d13b-4aac-939e-f1a39e8c9a77)

**Data_2017_Inputs**

![image](https://github.com/user-attachments/assets/c238f3a2-021b-422c-996a-c7d5b450906c)

**Data_2017_Outputs**

![image](https://github.com/user-attachments/assets/21058594-f89d-4abf-9b5b-7cdcc2da08d5)

**Data_2018_Inputs**

![image](https://github.com/user-attachments/assets/008de900-5b89-41d4-9eb7-5b79c1449770)

**Data_2018_Outputs**

![image](https://github.com/user-attachments/assets/8c723a06-38b1-418e-af47-39125f0617da)

**Data_2019_Inputs**

![image](https://github.com/user-attachments/assets/637d7a75-a557-4d51-a6a5-7188aa093eac)

**Data_2019_Outputs**

![image](https://github.com/user-attachments/assets/3079c5a7-0b9d-44e3-b6ba-5a38878330ad)


### **5. Creating the Training Set and the Test Set**

![image](https://github.com/user-attachments/assets/79eb750f-d077-4ccf-9836-84ffb42d1f2c)


## Part 2: Model Implementation: Use appropriate libraries (e.g., Scikit-learn in Python).

### **2.1. Building the model**

![image](https://github.com/user-attachments/assets/94a3bd79-62e8-4b70-bf84-ff7b3ea84795)

### **2.2 Training the Model**

![image](https://github.com/user-attachments/assets/0853c046-8693-4144-8750-1c7f65218fe9)

### **2.3 Training the Model**

![image](https://github.com/user-attachments/assets/b3ae2221-9749-4f3f-9cad-5dde2d630978)

### **2.4 Inference**

**Data_2015**

![image](https://github.com/user-attachments/assets/348285f1-60f9-4ff5-8987-072b8b71310d)

**Data_2016**

![image](https://github.com/user-attachments/assets/68098ee1-972c-4f2c-b5c2-418d6c85ac7f)

**Data_2017**

![image](https://github.com/user-attachments/assets/aa2ab30f-5c2b-4b50-930e-be7299123de4)

**Data_2018**

![image](https://github.com/user-attachments/assets/2fa043b9-91f9-452b-a71a-21f91a2f9a9d)

**Data_2019**

![image](https://github.com/user-attachments/assets/8ea619b8-3e14-4af9-ac17-aad0e385fd47)

## Part 3: Evaluation Metrics: Calculate R-squared, Mean Squared Error, etc.

### **3.1 Calculate R-squared and MSE for the models**

![image](https://github.com/user-attachments/assets/5d0ddf0f-3adc-46a6-8829-a0f0c462eb62)

### **3.2 R-Squared**

![image](https://github.com/user-attachments/assets/672b2425-3319-4d16-8cb7-692198748814)

### **3.3 Mean Squared Error**

![image](https://github.com/user-attachments/assets/43fea5c2-4cd2-44d4-ac69-3c3fa529d36d)

## Part 4: Interpretation: Explain the significance of coefficients and the model's predictive power.

**Data_2015**

![image](https://github.com/user-attachments/assets/b2ce9391-7cf5-4e50-bd3a-c74e2fd71799)

**Data_2016**

![image](https://github.com/user-attachments/assets/531f2bfa-ffe7-4719-827e-579076c5a5f3)

**Data_2017**

![image](https://github.com/user-attachments/assets/f8623141-b865-422c-9aab-be17243b63ff)

**Data_2018**

![image](https://github.com/user-attachments/assets/313b20d8-1e91-4b33-9cad-1f7a0a0a8028)

**Data_2019**

![image](https://github.com/user-attachments/assets/d6d4a675-0d36-45f5-9e85-f0488285d4e8)

## <p align="center">Logistic Regression: *Credit Card Fraud Detection*</p>

## 2. Results

## Visualization
## <p align="center">Linear Regression: *World Happiness Report*</p>
## <p align="center">Logistic Regression: *Credit Card Fraud Detection*</p>


## 3. Discussion

# V. Reference

 - Wikipedia contributors. (2024b, October 15). Linear regression. Wikipedia. https://en.wikipedia.org/wiki/Linear_regression
 - World Happiness Report Link: https://www.kaggle.com/datasets/unsdsn/world-happiness 
 - Credit Card Fraud Detection Dataset Link: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud


Code Comments: Ensure all code is well-commented and readable.

Methodology: Document each step taken during analysis.

Results: Summarize findings and include tables or charts where appropriate.

Discussion: Reflect on the results, compare the two regression methods, and mention any limitations.
