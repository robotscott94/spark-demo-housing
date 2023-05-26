# spark-demo-housing

## Purpose
Housing data is loaded into a spark session and analyzed by running various queries. This notebook shows how to interact with distributed data sets as well as testing the speed of queries under different conditions.

## Tools
PySpark is the primary tool used to interact with the housing data set. PySpar is the Python API used to interact with Apache Spark which is a distributed computing framework for large-scale data analysis. PySpark lets users upload, manipulate, query and store data in a scalable way. 

## Results
Various queries are shown that break down average home prices by year for a variety of features. Then, the same query is run three times under different conditions: with an uncached table (stored in disk), a cached table (stored in memory) and on a table partitioned as a parquet table. The cached table had the shortest run time, while the uncached and parquet data were a close second and third, respectively. Given the small data set, the time differences are negligible.

