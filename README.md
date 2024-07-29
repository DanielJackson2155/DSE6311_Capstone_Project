# DSE6311_Capstone_Project
 Merrimack Data Science Capstone Project

Members: Daniel Jackson, Nischal Panta, Nelson Tran

Project Title: COVID-19’s Effect on US College Students 
 
 For our research proposal, we are going to be creating 9 quantitative regression models to predict the effects that COVID-19 had on college students’ anxiety levels. We are assuming that there are similar studies out there on the general population. However, we want to focus on college students as they were a vulnerable subgroup during the pandemic. The goal of this research project is to help education institutions provide support services and create new policies that will help students who experienced a change in their anxiety levels. Although the question is not unique in itself, some studies have addressed COVID effects on the general public. The novelty of our project lies in the fact that it is solely analyzing and studying the effects of COVID-19 on college students. It is worth our time to explore this question, as we want to provide insights into how COVID-19 affected students during the pandemic. This will be very valuable in aiding/informing educational institutions and policymakers of the psychological effects of the pandemic on students. This information can be used in designing better support systems and policies to help cope with those with increased anxiety levels. This will also be useful for building the base for other areas of mental health and public health research. 

As mentioned our research proposal is not an original one. We are taking the improvement approach. We are looking to combine multiple feelings from students into one standalone feeling, which will be our response variable. Our response variable will be called “total anxiety level” (total_anxiety_level). We will dive deeper into this a little later in our proposal. We will be coding in R for our project. 

Here is our hypothesis: COVID-19 had a significant impact on the anxiety levels of college students because of the unique stressors associated with the pandemic. 
Here is our prediction: College students were more likely to have higher anxiety due to the effects that COVID-19 had on factors such as outdoor activity, screen time, and exercise. 

We found a dataset from seven universities in the US: Arizona State University, Clemson University, North Carolina State, Oregon State University, Pennsylvania State University, and the University of Montana. There are 2,534 observations (students) from 14,174 total surveys sent out across all seven colleges. The survey was targeted at students’ feelings and lifestyles during Covid-19. The data that we will be using can be found in the links below: 
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7790395/#sec021 pone.0245327.s010.csv  
 
 Our response variable will be a quantitative variable. We will call our response variable “anxiety_level”. It will be a quantitative variable of the total anxiety level experienced by a US college student. We will be combining the scores of multiple feelings regarding COVID-19 into one response variable. The scores of feelings that will be combined: Afraid, Irritable, Guilty, Sad, Preoccupied, and Stressed. We will take the value of each variable, add them, and then assign that to a new variable in our data set. We will then create 9 different quantitative regression models to predict the response variable. The 9 models that we will fit are as follows: multiple linear regression, ridge regression, lasso regression, PCA, PLS, regression trees, bagging, random forest, and boosted. We will use numerous predictor variables from the survey. Most of the predictors in the dataset are qualitative, but there are also some quantitative variables. Using the mean squared errors for each test we will test the performance of our models and choose a final one which we will use for our final submission. Our data dictionary will have a better summary of each variable used. We will be removing and merging some features before and during our exploratory data analysis. The structured processes are as follows:

Analysis Plan:
Data Cleaning and Preparation:
Remove and merge features as necessary.
Create a data dictionary to summarize each variable used in the analysis.

Exploratory Data Analysis:
Clean and prepare the data for modeling.
Create histograms to visualize our variables and their spread and decide whether outlines need to be removed.
Round-up imputed values from previous machine-learning models for certain variables.
Use a KNN model to predict many missing values
Combine scores of multiple feelings into a new variable "total_anxiety_level."
Perform unsupervised machine learning: which we can use to help reduce dimensionality and prevent overfitting

Model Fitting:
Split the data into training (70 percent) and test (30 percent) sets.
Create 9 different machine learning models to predict our response variable and in the test data compare them

Model Evaluation:
Use mean squared error (MSE) to measure the accuracy of test predictions of all our models.
Select the model that performs best on the test data using the MSE.
Policy Development:
Identify the demographics of students most affected by Covid-19.
Develop targeted support systems (creation of an extra variable for those who are over the threshold) and policies for these students to reduce anxiety.
