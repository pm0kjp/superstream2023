
# BigQuery ML

While there are multiple ways to perform machine learning on data stored in BigQuery, let's consider just one: BigQuery ML.

To use BigQuery ML, you first create a model using the Standard SQL query language.  For example, the query below adds a new model called `nyc_311_arima` to a dataset I previously created (`my_models`).  

```
CREATE OR REPLACE MODEL my_models.nyc_311_arima
-- options will vary based on model type
-- but in this case, we select a model type
-- and add some specific parameters for that model
-- type (e.g. accounting for US holidays)
OPTIONS
  (model_type = 'ARIMA_PLUS',
   time_series_timestamp_col = 'created_on',
   time_series_data_col = 'num_service_requests',
   auto_arima = TRUE,
   holiday_region='US',
   data_frequency = 'AUTO_FREQUENCY',
   decompose_time_series = TRUE
  ) AS
-- a query below that returns a timeseries dataset
-- (date and number of 311 requests for each date)
SELECT 
 EXTRACT(DATE from created_date) as created_on,
 COUNT(unique_key) AS num_service_requests
FROM `bigquery-public-data.new_york_311.311_service_requests` 
GROUP BY created_on
```

Once that model is created, you can use that model for prediction.  For example, the query below takes the model I just created and uses it to create 365 predictions of daily 311 report volume.

```
SELECT * FROM ML.FORECAST(MODEL `superstream2023.my_models.nyc_311_arima`, STRUCT(365 AS horizon, 0.8 AS confidence_level))
```
