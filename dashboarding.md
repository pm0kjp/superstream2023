# Dashboarding

There's a video showing this process at https://docs.google.com/presentation/d/1jekywpnM3BDC0XIp0BzGl03ttxOUWIKmfEZoCzcQYHw/edit#slide=id.g1fa9bc073a0_0_5.

Dashboarding in BigQuery is possible thanks to a well-integrated third party tool, Looker Studio.  To create a dashboard:

1. Create a data results set (for example, do a SQL query on your data to get a set of results).
2. In the part of the BigQuery screen where your results are shown, find the button marked "EXPLORE DATA", and click it.  Choose "Explore with Looker Studio."
3. You probably already have a sample table displayed, which is Looker Studio's guess at what might be useful.  Take a look around at:
    * The types of tables and graphs that are available to you
    * The "tab" structure at the bottom of the document
    * The "data" and "style" options for the currently selected chart
4. Use "Add a Chart" and select the chart style and the dimensions you wish to use from your data.
5. Design the layout of your dashboard, add text as needed, delete any default elements you don't need, and save your dashboard. (to save, you'll have to sign up to use Data Studio).
6. If desired, save and share your dashboard (this requires you to give some permissions and affirm that you know what data you're sharing).