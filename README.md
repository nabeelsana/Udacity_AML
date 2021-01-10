# Optimizing an ML Pipeline in Azure

## Overview
This project is part of the Udacity Azure ML Nanodegree.
In this project, we build and optimize an Azure ML pipeline using the Python SDK and a provided Scikit-learn model.
This model is then compared to an Azure AutoML run.

## Summary
The dataset represents direct markting campaign of a bank. Each record represnts a potential target for deposit placement with the bank and recorded results whether effort led to placement of deposit or not (target column "y"). 
Task of machine learning was to train a binary classification model so as to predict whether a potential target of marketing campaign will place deposit or not. 

We used two machine learning pipelines, with primary metric as "Accuracy", as follws: 
i) Scikit-learn piple line with Logistic Regrsssion Classifier and hyperdrive for hyperparameter tuning.
ii) Microsoft Azure proprietary AutoML pipeline for automated machine learing including selection of classifiers and their hyperparameters.

Best models selected under each of the pipelines are as follows: 
i) Scikit-learn : Logistic Regression model with 91.138% Accuracy parameter values: C1: 0.48392209 , max_iter: 200.
ii) Azure AutoML:   model with % Accuracy parameter values:                    

Therefore best pipeline was \\ and best model was \\ with % Accuracy
## Scikit-learn Pipeline
**Explain the pipeline architecture, including data, hyperparameter tuning, and classification algorithm.**

**What are the benefits of the parameter sampler you chose?**

**What are the benefits of the early stopping policy you chose?**

## AutoML
**In 1-2 sentences, describe the model and hyperparameters generated by AutoML.**

## Pipeline comparison
**Compare the two models and their performance. What are the differences in accuracy? In architecture? If there was a difference, why do you think there was one?**

## Future work
**What are some areas of improvement for future experiments? Why might these improvements help the model?**

## Proof of cluster clean up
We used AmlCompute command delete() (documented in our python notebook) to clean up cluster as both pipeline runs has finished.
