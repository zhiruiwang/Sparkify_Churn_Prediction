# Sparkify_Churn_Prediction

### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [Files Description](#files)
4. [Result](#Result)


## Installation <a name="installation"></a>

This project uses the following Python libraries:

Pyspark

itertools

re

h2o

Matplotlib

You will also need to have software installed to run and execute a Jupyter Notebook.

If you do not have Python installed yet, it is highly recommended that you install the Anaconda distribution of Python, which already has the above packages and more included. And for Spark, I am using Databricks, but you can also do this using AWS or IBM Cloud.

## Project Motivation<a name="motivation"></a>

This is udacity's capstone project, using spark to analyze user behavior data from music app Sparkify.

Sparkify is a music app, this dataset contains two months of sparkify user behavior log. The log contains some basic information about the user as well as information about a single action. A user can contain many entries. In the data, a part of the user is churned, through the cancellation of the account behavior can be distinguished.

## Files Description<a name="files"></a>

**Sprakify .html** Databricks notebook, main file of the project, it demonstrates the process of using pyspark to explore the data and build the model.

**Sprakify .ipynb** Jupyter notebook output from Databricks, if you want to use local, AWS or IBM cloud to run, this file would be better to start. But since the notebook is designed for Databricks, **viewing it in GitHub will be very messy!**

**medium-sparkify-event-data.json** Input data of the workflow, can be found in following [link](https://s3.amazonaws.com/video.udacity-data.com/topher/2018/December/5c1d6681_medium-sparkify-event-data/medium-sparkify-event-data.json)

## Result

This project defined customer churn as to whether a user visited the Cancellation Confirmation page. We used a sample dataset in a Databricks pyspark cluster that can be easily scaled to much larger datasets (big data). We trained a XGBoost model on the engineered features, which give us AUC of 0.84 in the testing data. The variable importance plot is inline with the exploratory analysis we did before implementing the model.

I post a blog about the detail, you can find it [here](https://zhiruiwang.github.io/Sparkify_Churn_Prediction/).
