# Colab Boilerplate

There's a video showing this process at https://docs.google.com/presentation/d/1jekywpnM3BDC0XIp0BzGl03ttxOUWIKmfEZoCzcQYHw/edit#slide=id.g1fa9bc073a0_0_23

A new feature of BigQuery is automatic creation of a boilerplate Colab Python notebook that sets data analysts up for integration with BigQuery datasts.

1. Create a data results set (for example, do a SQL query on your data to get a set of results).
2. In the part of the BigQuery screen where your results are shown, find the button marked "EXPLORE DATA", and click it.  Choose "Explore with Colab Notebook"
3. A Python kernel Colab Notebook will be created for you with all the cells in place that allow you to connect to your dataset programatically. 
4. Run the cells in order and pay close attention to when you're required to authenticate, and follow the instructions and grant the appropriate permissions as needed.
5. Use the notebook to analyze data, and save and share it as desired.