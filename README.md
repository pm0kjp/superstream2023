# superstream2023

This repository accompanies the presentation by Joy Payton entitled ["Driving Data Insights with Google BigQuery: Trying it on for Size"](https://docs.google.com/presentation/d/1jekywpnM3BDC0XIp0BzGl03ttxOUWIKmfEZoCzcQYHw/edit?usp=sharing), given in February 2023. The goal of that presentation is to help learners understand how BigQuery can drive data insights in different ways for different stakeholders.


## BigQuery Caper Crew

| Caper Role | Data Talent |
| ---------- | ------- |
| [Mastermind](#mastermind) | Your C-Suite / Senior Leader, who needs the big picture in a dashboard |
| [Insider](#insider) | Your data subject matter expert and data provisioner, who wants to understand ETL |
| [Hacker](#hacker) | The data analyst who throws together quick and dirty notebooks for exploratory data analysis |
| [Safecracker](#safecracker) | The data scientist who gets at the deep insights through machine learning |

## Insider

Your **insider** is the data SME, the person who knows the data well.

(Department heads, DBAs, data lake contributors…)

Concern: 

> "How do I get the data into BigQuery?"

**Info for the Insider**

* BigQuery is for tabular data, and you can get data into BigQuery in a number of ways.
    * Object Storage for flat files like .csvs via Google Cloud Storage
    * Ingestion of various types of flat file data directly  into Google BigQuery
    * Integration with other public cloud providers like AWS
    * Streaming data options
* Data organization:
    * Projects hold
        * Datasets which hold
            * Tables    

**Tasks this crew member will be interested in:**

* [Creating a Google Cloud Platform Project](create_new_project.md)
* [Enabling BigQuery within a project](enable_bigquery.md)
* [Enabling Google Cloud Storage within a project](enable_gcs.md)
    * Adding a new bucket
    * Adding files and folders to a bucket
* [Adding a dataset to BigQuery](adding_dataset.md)
* [Adding data to a dataset in BigQuery](adding_data_to
_dataset.md)
    - From files in Google Cloud Storage
    - From local data
    - From third party connections (e.g. AWS, Azure)
    - Other methods (two dozen and counting!)

## Mastermind

Your **mastermind** is a senior decision maker who cares about the big picture.

(VPs, C-Suite…)

Concern: 

"How can I see insights via a dashboard I can understand easily?"

**Info for the Mastermind**

* Dashboards using Looker Studio are easy to create and change, existing staff will pick this up right away
* There's some built in data privacy double-checking
* Sharing is simple and intuitive

Tasks this crew member will be interested in:

* [Dashboarding in Data Studio](dashboarding.md)


## Hacker

Your **hacker** is a data analyst who loves working in a Jupyter notebook for quick exploration.

(Data analysts, developers, data scientists…)

Concern: 

"How can I access BigQuery data from a notebook?"

**Info for the Hacker:**

* Google Colab provides multi-language support for notebooks
* Colab is very well integrated into BigQuery
* A boilerplate Colab notebook is just one click away!

**Tasks this crew member will be interested in:**

* [Automatic creation of Colab boilerplate](colab_boilerplate.md)
* [Manual method: authenticating to GCP in a Colab notebook](authenticating_in_colab.md)
* [Manual method: adding BigQuery data in a Colab notebook](adding_bigquery_to_colab.md)


## Safecracker

Your **safecracker** is a data scientist who wants to get valuable insights that lead to predictive value.

(Data scientists, CDO, data engineers…)

Concern: 

> "How can I do machine learning?"

**Info for the Safecracker:**

* BigQuery ML steps:
    * Create a dataset to hold your model(s)
    * Write a model creation query in SQL
    * Inspect your model 
    * Use your model for prediction

**Tasks this crew member will be interested in:**

* [Use BigQuery ML](bigquery_ml.md)


