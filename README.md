DSE6311_Capstone_Project
Merrimack Data Science Capstone Project

Members: Daniel Jackson, Nischal Panta, Nelson Tran

Project Title: COVID-19’s Effect on US College Students 


Research Question
Does COVID-19 have an impact on college students in the US? And if so, is there a way to determine which groups are affected the most? 


Hypothesis
COVID-19 had a significant impact on the anxiety levels of college students because of the unique stressors associated with the pandemic.


Prediction
College students were more likely to have higher anxiety due to the effects that COVID-19 had on factors such as outdoor activity, screen time, and exercise


Introduction
We are interested in understanding the impact that COVID-19 had on college students during the global pandemic. It was an unforeseen event that negatively impacted so many around the world. We wanted to focus on college students specifically. These institutions were not prepared to handle the magnitude of the pandemic. Obtaining a college degree is stressful within itself. When combined with a pandemic, college students then had to deal with something out of their control. This was the catalyst for a new form of anxiety that students have never experienced before. This research paper is meant to analyze the effects that COVID-19 had on those college students. We want to use the information and data provided by students themselves to be able to predict which students will suffer from anxiety in the future when faced with similar circumstances. To ensure that funds, attention, and services are properly provided to those in need. We will be focusing on US college students specifically, but we feel that our findings can be implemented in other fields and institutions.
	
	For our research proposal, we are going to be creating a quantitative regression model to predict the effects that COVID-19 had on college students’ anxiety levels. We are assuming that there are similar studies out there on the general population. However, we want to focus on college students as they were a vulnerable subgroup during the pandemic. The goal of this research project is to help education institutions provide support services and create new policies that will help students who experienced a change in their anxiety levels. Although the question is not unique in itself, some studies have addressed COVID-19 effects on the general public. The novelty of our project lies in the fact that it is solely analyzing and studying the effects of COVID-19 on college students. It is worth our time to explore this question, as we want to provide insights into how COVID-19 affected students during the pandemic. This will be very valuable in aiding/informing educational institutions and policymakers of the psychological effects of the pandemic on students. This information can be used in designing better support systems and policies to help cope with those with increased anxiety levels. This will also be useful for building the base for other areas of mental health and public health research. 
	
	As mentioned our research proposal is not an original one. We are taking the improvement approach. We are looking to combine multiple feelings from students into one standalone feeling, which will be our response variable. Our response variable will be called “total anxiety level”. We will dive deeper into this a little later in our proposal. We will be coding in R for our project. 
	
	We found a dataset from seven universities in the US: Arizona State University, Clemson University, North Carolina State, Oregon State University, Pennsylvania State University, and the University of Montana. There are 2,534 observations (students) from 14,174 total surveys sent out across all seven colleges. The survey was targeted at students’ feelings and lifestyles during Covid-19. The data that we will be using can be found in the links below: 
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7790395/#sec021 pone.0245327.s010.csv  
 	
	Our response variable will be a quantitative variable. We will call our response variable “avg_anxiety_level”. It will be a quantitative variable of the total anxiety level experienced by a US college student. We will be combining the scores of multiple feelings regarding COVID-19 into one response variable and then take the average. The scores of feelings that will be combined: Afraid, Irritable, Guilty, Sad, Preoccupied, and Stressed. We will take the value of each variable, add them, average them, and then assign that to a new variable in our data set. We will then create a quantitative regression model to predict the response variable. We will use numerous predictor variables from the survey. Most of the predictors in the dataset are qualitative, but there are also some quantitative variables. Using the mean squared errors of our predictions, we will test the performance of our models and choose a final one which we will use for our final submission. Our data dictionary will have a better summary of each variable used. We will be removing and merging some features before and during our exploratory data analysis. The structure of our analysis plan will be as follows:


Analysis Plan
Data Cleaning and Preparation:
Remove and merge features as necessary.
Create a data dictionary to summarize each variable used in the analysis.

Exploratory Data Analysis:
Clean and prepare the data for modeling.
Create histograms to visualize our variables and their spread and decide whether outlines need to be removed.
Round-up imputed values from previous machine-learning models for certain variables
Combine scores of multiple feelings into a new variable "total_anxiety_level."

Model Fitting:
Split the data into training (80 percent) and test (20 percent) sets.
Use a KNN model to predict many missing values
Perform Principal Component Analysis to help reduce dimensionality and prevent overfitting
Create models to predict our response variable

Model Evaluation:
Use mean squared error (MSE) to measure the accuracy of training and test predictions of all our models.
Select the model that performs best on the test data using the MSE.

Policy Development:
Identify the demographics of students most affected by Covid-19.
Develop targeted support systems (creation of an extra variable for those who are over the threshold) and policies for these students to reduce anxiety.
