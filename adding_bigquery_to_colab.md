# Adding BigQuery Functionality to a Colab notebook

Aside: Not sure what a Colab notebook is?  If you've ever used a Jupyter (formerly iPython) notebook, then Google's Colaboratory (Colab) will be a fairly easy leap.

Regardless, you'll certainly benefit from the fact that Colaboratory communicates very easily with BigQuery!

1. Click on this link to a Colaboratory (Colab) notebook, and if prompted to log in or select your account, **choose the same one** you're using for your work in BigQuery:

https://colab.research.google.com/notebooks/bigquery.ipynb

This is Google's own intro to the integration between Colab and BigQuery.  

2.  Notice that there are three listed ways to integrate BigQuery with Colab.  I prefer to use the second listed method, "Use BigQuery through google-cloud-bigquery".

3.  Save a copy of this notebook by clicking on "Copy to Drive" or File > Save a copy in Drive.

4.  Use the method you prefer in a new notebook (File > New notebook) by using copy / paste.  

5.  Add your project id (read on below if you're not sure how to find this) in the appropriate place:

  * If you use "BigQuery via magics", find where "yourprojectid" is mentioned and replace it with the quoted string of your project ID.
  * If you use "BigQuery through google-cloud-bigquery", find where [your project ID] is mentioned and replace that with your project ID.
  * If you use "BigQuery through pandas-gbq", find the text "project_id=project_id" and replace the second "project_id" with your quoted project ID string.

6. To actually use BigQuery, you'll need to use SQL queries to obtain data.  Learning SQL is beyond the scope of this repository, but there are some good examples to get you started in Google's sample notebook.

7. Don't forget [authentication](authenticating_in_colab.md)!

