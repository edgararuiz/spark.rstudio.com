# `spark_save_table`: Saves a Spark DataFrame as a Spark table

## Description


 Saves a Spark DataFrame and as a Spark table.


## Usage

```r
spark_save_table(x, path, mode = NULL, options = list())
```


## Arguments

Argument      |Description
------------- |----------------
```x```     |     A Spark DataFrame or dplyr operation
```path```     |     The path to the file. Needs to be accessible from the cluster. Supports the "hdfs://" , "s3n://" and "file://" protocols.
```mode```     |     Specifies the behavior when data or table already exists.
```options```     |     A list of strings with additional options.

## Seealso


 Other Spark serialization routines: [`spark_load_table`](spark_load_table.html) ,
  [`spark_read_csv`](spark_read_csv.html) ,
  [`spark_read_jdbc`](spark_read_jdbc.html) ,
  [`spark_read_json`](spark_read_json.html) ,
  [`spark_read_parquet`](spark_read_parquet.html) ,
  [`spark_read_source`](spark_read_source.html) ,
  [`spark_read_table`](spark_read_table.html) ,
  [`spark_write_csv`](spark_write_csv.html) ,
  [`spark_write_json`](spark_write_json.html) ,
  [`spark_write_parquet`](spark_write_parquet.html) ,
  [`spark_write_table`](spark_write_table.html) 


