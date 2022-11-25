# Predicting Click on Ads

## Work Environment

**Tool** : Jupyter Notebook \
**Programming Language** : Python 3 \
**Visualization** : Matplotlib, Seaborn \
**Dataset** : [Click Ads Data]() 

## Project Background
A company wants to know the effectiveness of an advertisement that they display, this is important for the company to be able to find out how much the advertising has been marketed so that it can attract customers to see the advertisement.

This project aims to reduce the cost of advertisement targeting by 50%, and increase gross profit by 5%. By processing historical advertisement data and finding insights and patterns that occur, it can help companies determine marketing targets. The focus of this project is to create a machine learning classification model that functions to determine the right target customers. 

The result of this project is that we managed to decrease advertisement cost by 51%, and increase gross profit by 9%. We also provide actionable recommendations that can be applied by the marketing team can prioritize the specific customer segment so that the gross profit of the company can increase.

## Dataset Overview
The dataset contains 1,000 unique observations with 10 features in various data types. Each row represent customers' demographics, and behaiour records on website and ads in 7 months period. There are missing values in 4 columns (Daily Time Spent on Site, Area Income, Daily Internet Usage, Male), and 1 misdefined data type (Timestamp).

## Preprocessing
  1. Handling Missing Values
  2. Feature Engineering
  3. Drop Unnecessary Features
  4. Feature Encoding
  5. Feature Scaling

## Modeling
We leveraged logistic regression, decision tree, random forest, and KNN algorithms. Among the 4 models, the logistic regression model results the highest AUC, meaning that the model is the best able to distinguish between classes.

With classification threshold 0.5, the model is able to predict up to 97% of the existing potential interested users in the ads, with the risk of targeting disinterested users due to predicting errors of 1%. It means for every 100 users who are predicted to be  interested, there is 1  who is actually not interested in the ads. The **most important features** in prediction are **daily time spent on site, daily internet usage, area income, and age**.

  <p align="center">
  <img width="560" img width="243" alt="summary" src="https://user-images.githubusercontent.com/98371569/204020700-65fa4d11-d15d-4191-8714-9dca3dac8690.png">
    <br </br>
   <img width="560" img width="243" alt="summary" src="https://user-images.githubusercontent.com/98371569/204020967-b6b312f6-7efb-427a-99bb-e7822e53296b.png">
    <br </br>
    <img width="560" img width="243" alt="summary" src="https://user-images.githubusercontent.com/98371569/204021056-f70bc5b8-1081-4cbd-bffc-bf087cec0c33.png">
    <br </br>
  </p>
  
  
## Recommendations
  <p align="center">
  <img width="560" img width="243" alt="summary" src="https://user-images.githubusercontent.com/98371569/204021788-ccff9075-2380-48bb-a073-0fa352cb7762.png">
    <br </br>
  </p>
 
 We should **targeting ads** to the **mature users** (age between 36 - 61) who belong to a **low social class** (earning around 300M/year) with daily time spent on site between 32-68 mins. The ads must advertise products or services whose value isn’t higher than their buying power. There is no particular ad category that they are significantly interested to.
