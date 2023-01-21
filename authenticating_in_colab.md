# Authenticating 

Aside: Not sure what a Colab notebook is?  If you've ever used a Jupyter (formerly iPython) notebook, then Google's Colaboratory (Colab) will be a fairly easy leap.

Regardless, you'll certainly benefit from the fact that Colaboratory communicates very easily with BigQuery!

1. Click on this link to a Colaboratory (Colab) notebook, and if prompted to log in or select your account, **choose the same one** you're using for your work in BigQuery:

https://colab.research.google.com/notebooks/bigquery.ipynb

This is Google's own intro to the integration between Colab and BigQuery.  

2.  Notice the cell near the top with the text "Provide your credentials to the runtime."  This is the first step, telling Google Colab who you are.

3.  Save a copy of this notebook (if you don't already have a copy) by clicking on "Copy to Drive" or File > Save a copy in Drive.

4.  Copy the authentication cell into a new notebook (File > New notebook) or an existing notebook you're working on by using copy / paste.  

5.  When the authentication cell gets run, instructions will pop up on the screen and the notebook will pause execution until you go through the steps of authenticating via clicking.  If you're logged in to the same account in Colab that you use for accessing BigQuery in GCP, this should be a fairly simple process.  

6. To actually use BigQuery, you'll need to use SQL queries to obtain data.  Learning SQL is beyond the scope of this repository, but there are some good examples to get you started in Google's sample notebook.


