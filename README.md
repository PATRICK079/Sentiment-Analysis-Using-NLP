# Sentiment-Analysis-Using-NLP

<img width="800" alt="Screen Shot 2024-10-12 at 02 32 28" src="https://github.com/user-attachments/assets/1432790c-e24c-4cf2-bcd5-758f7dbafee9">
# Introduction

This repository contains a comprehensive implementation of sentiment analysis, including data preprocessing, feature extraction, model training, and evaluation. The goal is to explore various methods for sentiment classification using traditional machine learning algorithms, providing a thorough understanding of how to build sentiment analysis models effectively.

# Business Problem
 A Ccompany  struggled with processing and analyzing customer feedback. The manual review of emails and social media comments was time-consuming and inconsistent. Customer service teams were overwhelmed, resulting in missed opportunities to address critical issues that were affecting customer satisfaction and leading to customer loss. Now, they have employed me to help with creating a robust algorithm that can generize so well to solve thier business problem

 # Problem Encountered/ Solution

 During my project, I encountered the following  issues 
 
●  when using GaussianNB, which requires dense input, and  the vectorization process i.e CountVectorizer produced a sparse matrix and i kept getting errors.

  To resolve this, I needed to create a custom transformer that converts the sparse matrix into a dense numpy array and ensures the data is of type float.

● I also encountered an issue where the data needed to be explicitly converted to float for compatibility with the machine learning model

   i resolved this by creating a custom transformer to ensure that all input data is properly converted to float format before being passed to the model.

# Key Learnings from the Project

● I learned how to convert sparse matrices to dense arrays using a custom transformer, ensuring compatibility with models that don’t accept sparse input.
 
● I gained experience in creating custom transformers using sklearn.base.TransformerMixin to adapt data for model input, ensuring data type consistency (such as converting to float64).

● learned how to leverage scikit-learn’s Pipeline, I was able to chain together preprocessing (vectorization, custom transformers) and modeling (classification 

with GaussianNB) seamlessly, improving maintainability and modularity of the code.

● I improved my skills in debugging and troubleshooting issues related to input format, allowing me to create efficient solutions using custom transformers.


● The use of scikit-learn pipelines taught me how to organize code in a more modular way.


# Model Implentation

  I built 4 machine learning models; logistic regression, voting classifier, random forest classifer and  GaussianNB. They all performed 
  
  so well except  GaussianNB that got accuracy of 28%.  Voting classifier and logistic regression is my best model based on generalization. 

# KINDLY HAVE A LOOK AT MY DETAILED NOTEBOOK FOR MY STEP BY STEP SOLUTION AND  INSIGHTS . THANK YOU

# Dataset Citation

source: KAGGLE

URL: https://www.kaggle.com/datasets/praveengovi/emotions-dataset-for-nlp
   
   
