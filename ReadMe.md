## Udacity Data Pipeline Project

In this particular project we are creating an ETL pipeline for a fictional company called Sparkify. Sparkify is a streaming music service. They have decided to incorporate more automation and robustness in their pipelines and infrastructure.

  The management is also concerned with data quality, most likely so that data scientists do not have to perform ETL to gain valuable insight into the data. Also, in traditional business intelligence efforts it is imperative to deliver accurate data as financial and operational decisions are made from the analysis performed on the data.

## Project Steps

The structure of the project is as follows;

    * dags
      ** udac_example.py
      ** dimension_subdag.py

    * plugins
      ** helpers
        *** sql_queries.py

    * operators
      ** __init__.py
      ** create_table.py
      ** data_quality.py
      ** load_dimension.py
      ** load_fact.py
      ** stage_redshift.py


## Dags

  The Dag does a number of things in sequence in order to insert json files from an s3 bucket to a redshift cluster (sql database).
