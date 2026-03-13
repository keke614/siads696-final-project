# siads696-final-project
siads696-final-project

# Political Ideology Classification from Congressional Tweets

Author: Wuke Zhang  
Course: SIADS 696 Final Project  
University of Michigan – Master of Applied Data Science

---

## Project Overview

This project studies whether political ideology can be identified from the text content of tweets posted by members of the U.S. Congress.

The main idea is to see if machine learning models can distinguish Democratic tweets and Republican tweets based on language patterns. Political communication on social media is interesting because politicians often express ideological position through short messages.

In this project, both supervised learning and unsupervised learning methods are used.

For supervised learning, several models are compared:

- Logistic Regression  
- Linear SVM  
- Multinomial Naive Bayes  
- Random Forest  

The goal is to evaluate which model performs better for text classification.

For unsupervised learning, clustering is used to explore whether the tweets contain internal thematic structure.

---

## Dataset

The dataset contains tweets from members of the U.S. Congress.

The original dataset is organized into several CSV files according to party and chamber:

- Democrats (both chambers)  
- Democrats (House)  
- Democrats (Senate)  
- Republicans (both chambers)  
- Republicans (House)  
- Republicans (Senate)  

The full datasets are relatively large and cannot be uploaded to GitHub.

To make the project reproducible, sample datasets are included in this repository. Each sample file contains the first 100 rows from the original dataset.

Included sample files:

- sample_Democrats_both_chambers.csv  
- sample_Democrats_house.csv  
- sample_Democrats_senate.csv  
- sample_Republicans_both_chambers.csv  
- sample_Republicans_house.csv  
- sample_Republicans_senate.csv  

These files are sufficient to understand the structure of the data and run the notebook.

---

## Methods

The project uses a typical machine learning pipeline for text classification.

Main steps include:

1. TF-IDF vectorization for text representation  
2. Dimensionality reduction using TruncatedSVD  
3. Training supervised classification models  
4. Cross-validation for model comparison  
5. Failure analysis to understand misclassified examples  

For unsupervised analysis, KMeans clustering is applied to explore potential topic structures in the tweets.

Model performance is evaluated using accuracy and F1 score.

---

## Repository Structure
 ```
analysis.ipynb
Political Ideology Classification from Congress.pdf

sample_Democrats_both_chambers.csv
sample_Democrats_house.csv
sample_Democrats_senate.csv
sample_Republicans_both_chambers.csv
sample_Republicans_house.csv
sample_Republicans_senate.csv
 ```  
Main notebook containing the full analysis workflow.

Political Ideology Classification from Congression.pdf  
Final report describing the project, methods, results, and discussion.

Sample datasets  
Small subset of the data used to illustrate the dataset structure.

---

## Environment

The analysis was implemented in Python.

Main libraries used:

- pandas  
- scikit-learn  
- numpy  
- matplotlib  

The notebook can be run directly in a standard Jupyter environment.

---

## Reproducibility

To reproduce the workflow:

1. Open `analysis.ipynb` in Jupyter Notebook.  
2. Make sure the required Python libraries are installed.  
3. Run the cells sequentially.

Because the full dataset is not included, the sample data mainly serves to illustrate the structure and allow the notebook to execute.
