# Email Campaign Effectiveness Prediction
![GitHib Logo](https://github.com/Bhushan0097/03.CAPSTONE.ML.Classification--Email-Campaign-Effectiveness-Prediction/blob/main/Header.jpg)

## Overview
This repository contains the code and resources for a supervised machine learning project aimed at predicting whether a deliverd email will be read , acknowledged or ignored. The dataset used is `data_email_campaign.csv`.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Dependencies](#dependencies)
- [ML Model Training and Evaluation](#mL-Model-training-and-evaluation)



## Introduction

Bike share demand prediction is a critical aspect of urban transportation planning. This project focuses on using machine learning techniques to predict bike rental demand in Seoul, aiding in efficient resource allocation and city planning.

## Dataset

The dataset `data_email_campaign.csv` is included in the  📁 `data` directory. It contains information about bike rentals, including weather conditions, temperature, humidity, and other relevant features.

The `data_email_campaign.csv` file contains the following columns:

- **Email_Id**    Email id of customer
- **Email_Type** Email type contains 2 categories :  1 and 2. We can assume that the types are like promotional email or sales email
- **Subject_Hotness_Score**   It is the email’s subject’s score on the basis of how good and effective the content is
- **Email_Source_Type**    It represents the source of the email like sales, marketing or product type email
- **Email_Campaign_Type**   The campaign type of the email   
- **Customer_Location**    Categorical data which explains the different demographic location of the customers   
- **Total_Past_Communications**    This columns contains the total previous mails from the same source   
- **Time_Email_sent_Category**    The time of the day when the email was sent   
- **Word_Count**    Total count of word in each email   
- **Total_links**    Total number of links in the email   
- **Total_Images**    Total Number of images in the email   
- **Email_Status**    Our target variable which contains whether the mail 

## Dependencies

The project is developed using Python and relies on the following libraries:

- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Documentation

The project involves the following steps: <br>
<ol>
  <li>  Data Cleaning and Preparation </li>
  <li>  Exploratory Data Analysis </li>
  <li>  Visualization and Insights </li>
  <li>  Hypothesis Testing </li>
  <li>  Feature Enginerring & Data Pre-processing </li>
  <li>  ML Model Training , Implementation and Evaluation </li>
</ol>

### Data Cleaning and Preparation
The first step in this project involves cleaning and preparing the data. This includes checking for missing data, removing duplicates, and converting data types. Some of the specific tasks involved in this step include:

- Handling missing data
- Removing duplicates
- Converting data types
- TimeSeries Analysis

### Exploratory Data Analysis
The next step in the project is to conduct exploratory data analysis.
This involves examining the data to understand its distribution, central tendencies, and correlations between variables.

### Hypothesis Testing

Hypothesis testing , a statistical method used to make inferences about a population based on a sample of data. To perform hypothesis testing on the 'data_email_campaign.csv' dataset, we first  start with a null hypothesis (H0) and an alternative hypothesis (H1), then use statistical tests to determine if there is enough evidence to reject the null hypothesis in favor of the alternative hypothesis.

Below is  general step-by-step guide on to perform hypothesis testing on a dataset like SeoulBikeData.csv:<br>
   <ol>
    <li>  Define the Hypotheses </li>
    <li>  Choose a Significance Level (α)</li>
    <li>  Select the Test </li>
    <li>  Perform the Test</li>
    <li>  Analyze the Results </li>
    <li>  Draw Conclusions </li> 
   </ol>


### Feature Enginerring & Data Pre-processing
<ol>
  <li>Handling Missing Values </li>
<li> Handling Outliers </li>
<li> Label Encoding </li>
<li> Textual Data Preprocessing </li>
<li> Feature Manipulation & Selection </li>
  <li> Data Transformation </li>
<li> Data Scaling </li>
<li> Dimesionality Reduction </li>
<li> Data Splitting </li>
</ol>

### ML Model Training and Evaluation
The dependent variable  is **Rented Bike Count** is a contionus variable. Hence to Regression ML algorithms are used to train the model to predict the depedent variable. <br>
Following are the ML algorithms on which the model is trained
<ol> 
<li> Logistic Regression </li>
<li> Random Forest Classification </li>
  <li> XGBoost Classification </li>
</ol>



<table>
        <thead>
            <tr style="background-color:#f2f2f2;">
                <th colspan="1" ></th>
                <th colspan="5" >Test</th>
		<th colspan="5" >Train</th>
            </tr>
            <tr>
		<th > Sr No.</th>
                <th > Model Name</th>
                <th >Accuracy</th>
				<th >Recall</th>
				<th >Precision</th>
				<th >F1score</th>
				<th >AUC</th>
				<th >Accuracy</th>
				<th >Recall</th>
				<th >Precision</th>
				<th >F1score</th>
    			<th >AUC</th>
       </tr>
        </thead>
        <tbody>
<tr>
      <th >0</th>
      <td  >Logistic Regression</td>
      <td >0.542400</td>
      <td   >0.542400</td>
      <td  >0.527200</td>
      <td  >0.517300</td>
      <td  >0.729900</td>
      <td  >0.583100</td>
      <td  >0.583100</td>
      <td  >0.608800</td>
      <td  >0.583700</td>
      <td >0.766600</td>
    </tr>
    <tr>
      <th>1</th>
      <td  >Logistic Regression + GridSearchCV</td>
      <td  >0.542000</td>
      <td  >0.542000</td>
      <td  >0.526900</td>
      <td  >0.516300</td>
      <td  >0.729700</td>
      <td  >0.582800</td>
      <td  >0.582800</td>
      <td  >0.608600</td>
      <td  >0.583100</td>
      <td >0.766500</td>
    </tr>
    <tr>
      <th>2</th>
      <td >Random Forest</td>
      <td >0.999700</td>
      <td >0.999700</td>
      <td >0.999700</td>
      <td >0.999700</td>
      <td >1.000000</td>
      <td >0.808700</td>
      <td >0.808700</td>
      <td >0.808400</td>
      <td >0.808300</td>
      <td >0.911100</td>
    </tr>
    <tr>
      <th>3</th>
      <td >Random Forest + GridSearchCV</td>
      <td >0.999700</td>
      <td >0.999700</td>
      <td >0.999700</td>
      <td >0.999700</td>
      <td >1.000000</td>
      <td >0.809200</td>
      <td >0.809200</td>
      <td >0.808700</td>
      <td >0.808700</td>
      <td >0.911900</td>
    </tr>
    <tr>
      <th>4</th>
      <td >XGboost</td>
      <td >0.808700</td>
      <td >0.808700</td>
      <td >0.809500</td>
      <td >0.802600</td>
      <td >0.935500</td>
      <td >0.776600</td>
      <td >0.776600</td>
      <td >0.765500</td>
      <td >0.765800</td>
      <td >0.895100</td>
    </tr>
    <tr>
      <th>5</th>
      <td >XGboost + GridSearchCV</td>
      <td >0.999300</td>
      <td >0.999300</td>
      <td >0.999300</td>
      <td >0.999300</td>
      <td >1.000000</td>
      <td >0.824700</td>
      <td >0.824700</td>
      <td >0.821200</td>
      <td >0.822300</td>
      <td >0.914100</td>
    </tr>
        </tbody>
    </table>

