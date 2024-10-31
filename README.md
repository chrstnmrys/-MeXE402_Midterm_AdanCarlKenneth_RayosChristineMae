# <p align="center">**$$ {\color{red}Linear \space \color{red}and \space \color{red}Logistic \space \color{red}Regression \space \color{red}{Analysis}} $$**</p>


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

![image](https://github.com/user-attachments/assets/20b20c75-0e84-4492-8a2d-c8dd4c7a371e)

![image](https://github.com/user-attachments/assets/3aa0f32d-85e3-40a7-826c-5fcc3e06ef42)

### **1.2 Checking for missing values in the datasets**

![image](https://github.com/user-attachments/assets/64eeac9d-a5ee-4fa3-9cc8-2559c531cc95)

![image](https://github.com/user-attachments/assets/882526e7-71eb-4e05-be93-21584afa9f6b)
 - This picture shows that there is no missing values in the dataset

### **1.3 Standardizing features**

![image](https://github.com/user-attachments/assets/3eb72ced-2590-4853-9cb6-f3e3fbab89b5)

![image](https://github.com/user-attachments/assets/2d9496c9-da2a-4786-9fd6-3f15500623b3)

### **1.4 Extracting the dependent variable (Happiness Score)**

![image](https://github.com/user-attachments/assets/477f5014-990f-4b58-a74d-435f1274b840)

### **1.5 Displaying the standardized data**

![image](https://github.com/user-attachments/assets/db973705-134b-4e03-bbd4-21a28448774e)

### **1.6 Getting the Inputs and Outputs**

Independent Variables

![image](https://github.com/user-attachments/assets/55b9d086-0406-4720-bf47-4dbadfdfe0af)

Dependent Variables

![image](https://github.com/user-attachments/assets/63e7159f-7dff-41c6-9202-4a0f6fd4db07)

### **1.7 Creating the Training Set and the Test Set**

![image](https://github.com/user-attachments/assets/81ebebd8-9703-42d7-9c06-ab947e8f48f8)

X_train

![image](https://github.com/user-attachments/assets/89f41728-703e-43af-bf41-ebbe724a1002)

X_test

![image](https://github.com/user-attachments/assets/de8b723d-5e41-42c1-91f4-42e6a3dfcc41)

y_train

![image](https://github.com/user-attachments/assets/f37b29f1-4654-45b3-b37c-4607a0034a2d)

y_test

![image](https://github.com/user-attachments/assets/024b6670-ce9d-4ce2-9a35-81174ddc4ea4)


## Part 2: Model Implementation: Use appropriate libraries (e.g., Scikit-learn in Python).

### **2.1. Building the model**

![image](https://github.com/user-attachments/assets/71f8fde8-0f23-4269-9379-a82e86162b61)

### **2.2 Training the Model**

![image](https://github.com/user-attachments/assets/903ac8a7-5627-477f-a189-6b68ab97c324)

### **2.3 Inference**

y_pred

![image](https://github.com/user-attachments/assets/2a9b9b35-e903-4faa-8819-2b5862a24873)

y_test

![image](https://github.com/user-attachments/assets/564219f5-e4c0-42d7-9c7d-a7f3431d5b1e)

## Part 3: Evaluation Metrics: Calculate R-squared, Mean Squared Error, etc.

### **3.1 R-Squared**

![image](https://github.com/user-attachments/assets/0b086623-ac56-467b-8592-2c68151885eb)

### **3.2 Adjusted R-Squared**

![image](https://github.com/user-attachments/assets/2ddb0720-d5be-4310-9cb2-beeaa9f25eab)

### **3.3 Mean Squared Error**

![image](https://github.com/user-attachments/assets/daeb8169-bbd5-45c9-bd3e-c9240acdf0a2)

## Part 4: Interpretation: Explain the significance of coefficients and the model's predictive power.

![image](https://github.com/user-attachments/assets/dd4d94f7-d2f4-471a-809b-ced518ab530a)

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
Inference:

y_pred
- These are the predicted happiness scores produced by the trained linear regression model for the same countries in the test set.

![image](https://github.com/user-attachments/assets/2a9b9b35-e903-4faa-8819-2b5862a24873)

y_test
- This is the actual data from the test set.
  
![image](https://github.com/user-attachments/assets/564219f5-e4c0-42d7-9c7d-a7f3431d5b1e)

- In summary the y_pred values and y_test values are close to each other, it means that the model's prediction is accurate. 

R-Squared

![image](https://github.com/user-attachments/assets/0b086623-ac56-467b-8592-2c68151885eb)

- This picture shows that 0.9406654043085512 percent, which means that the independent variable is a good fit to explain the variation in the dependent variable.

Mean Squared Error

![image](https://github.com/user-attachments/assets/daeb8169-bbd5-45c9-bd3e-c9240acdf0a2)

- This picture shows the difference between actual and predicted values, and the values that we acquired is np.float64(0.06067138321461446).
  
Interpretation:

![image](https://github.com/user-attachments/assets/dd4d94f7-d2f4-471a-809b-ced518ab530a)

- This picture show how much the dependent variable (Happiness Score) is expected to increase when the corresponding independent variable increases. Positive coefficients indicate a positive impact on happiness and Negative coefficients indicate a negative impact on happiness.
- In this case the results that we obtain in Happiness Rank	is -0.246276, means that countries with lower rank tends to have a lower happiness score.
- Standard Error is -0.009279, means that having a low standard error, reflects a low happiness score. 
- Economy	is 0.167077, means that countries with higher GDPs tend to have higher happiness scores.
- Family	is 0.176670, means that strong family tends to have higher happiness scores.
- Health	is 0.132987, means that having a better health contribute to happiness.
  
### Visualization

### Actual vs. Predicted Happiness Score

![image](https://github.com/user-attachments/assets/a8b45982-e941-471e-9bd4-6206e6366230)

<p align="center">
  <img src="https://github.com/user-attachments/assets/744d6876-421b-416e-a3b5-d5c3c933815c"/>
</p>

This plot is a scatter plot showing the relationship between actual happiness scores and predicted happiness scores from a regression model. Here’s how to interpret it:

- X-Axis (Actual Happiness Score): Represents the actual values of happiness scores from the data.

- Y-Axis (Predicted Happiness Score): Represents the predicted happiness scores that your model generated based on the input features.

- Blue Dots: Each dot represents a single observation, with its position indicating the actual happiness score (x-axis) and the predicted score (y-axis).

- Red Line: The red line represents the line y=x,  which is the line of perfect predictions. If all points lie exactly on this line, it would indicate that the model predicted each happiness score perfectly

Analysis
- Since most points are close to the red line, it indicates that the model is predicting the happiness scores fairly accurately though some points far from the line, indicating errors in the model’s predictions for those specific observations.


## <p align="center">Logistic Regression: *Credit Card Fraud Detection*</p>


### Summary & Findings 

Inference:

y_pred
- These are the predicted class produced by the trained logistic regression model from the test set.

![image](https://github.com/user-attachments/assets/5632e852-8c3f-4169-a7fb-6d851805d27d)

y_test
- These are the actual data from the test set.

![image](https://github.com/user-attachments/assets/ad361706-482d-48cf-8549-90f1b5f1edab)

- In summary the y_pred values and y_test values are close to each other, it means that the model's prediction is accurate.

Interpretation:

Accuracy
- The model shows high accuracy, but potentially misleading due to imbalnace.

![image](https://github.com/user-attachments/assets/5b71ac43-3ac7-4a80-8ff0-3c36460ad282)

Precision (Positive Predictive Value)
- The model shows good fraud detection accuracy, with 87.1% of projected fraudulent transactions turning out to be fraudulent.

![image](https://github.com/user-attachments/assets/2e2d3396-7d2e-46ff-b483-1481b5e45a05)

Recall (Sensitivity or True Positive Rate)
- About 80.2% of real fraud cases are captured by the model; nonetheless, it would need to be improved to catch additional fraud.

![image](https://github.com/user-attachments/assets/81c1e306-f849-4dd2-8d5f-51047f8a27b0)

F1 Score
- The model balances precision and recall, providing an overall performance score for fraud detection.

![image](https://github.com/user-attachments/assets/68a2efab-58d3-4a54-b11e-7ec44d48b871)

Importance of the features
Transaction Amount
- Strange transaction amounts are frequently associated with fraud because, in order to evade discovery, scammers may try to charge big sums or test the card with little purchases.
- Since notable variations from a user's typical spending pattern can be powerful indicators of fraudulent behavior, models can be impacted as frequently include transaction amount as a key characteristic.

Transaction Time
- Unusual periods, like late at night when the real cardholder might not be active, are more likely to see fraudulent transactions take place.
- It impacted the model as it may detect suspicious activity during off-peak hours by using time-related data (such as the day of the week and the hour).
### Visualization

### Confussion Matrix Display

![image](https://github.com/user-attachments/assets/3fd837ff-f73c-4bd3-a155-3b9b2a3dfbc7)

<p align="center">
  <img src= "https://github.com/user-attachments/assets/d46c3b67-03e4-45ca-a83d-d39f37ba4da7"/>
</p>

- The model accurately identified 56,489 legitimate transactions. (True Negative)
- The model wrongly identified 12 legitimate transactions as fraud, which can lead to customer inconvenience. (False Positive)
- The model failed to detect 20 fraudulent transactions, which is critical because these represent potential losses. (False Negative)
- The model successfully flagged 81 actual frauds. (True Positive)

## 3. Discussion

## <p align="center">Linear Regression: *World Happiness Report*</p>

In this analysis, we examined the World Happiness Report dataset to understand how various socio-economic factors—such as GDP per capita, social support, and health—influence a country’s Happiness Score. We applied Linear Regression to identify the impact of these factors on happiness.

Key Findings:
1. Linear Regression Model results showed that factors like GDP per capita, social support, and health have a positive association with happiness, meaning that higher values in these variables tend to correspond with higher happiness scores.

2. The model’s R-squared value was 0.9406654043085512 percent, indicating that the model's prediction is somehow accurate to the true value. Mean Squared Error (MSE) value was 0.06067138321461446, it means the model's predictive accuracy is a good fit indicating that there is fairly difference between the true value and predicted value.

3. Each coefficient in the model helps explain the effect of a one-unit increase in a socio-economic factor on the happiness score. For instance, a higher coefficient for GDP per capita implies a stronger influence of economic production on happiness score.
   
## <p align="center">Logistic Regression: *Credit Card Fraud Detection*</p>


# V. Reference

 - Wikipedia contributors. (2024b, October 15). Linear regression. Wikipedia. https://en.wikipedia.org/wiki/Linear_regression
 - World Happiness Report Link: https://www.kaggle.com/datasets/unsdsn/world-happiness 
 - Credit Card Fraud Detection Dataset Link: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

