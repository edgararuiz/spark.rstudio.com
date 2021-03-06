# `sdf-saveload`: Save / Load a Spark DataFrame

## Description


 Routines for saving and loading Spark DataFrames.


## Usage

```r
sdf_save_table(x, name, overwrite = FALSE, append = FALSE)
sdf_load_table(sc, name)
sdf_save_parquet(x, path, overwrite = FALSE, append = FALSE)
sdf_load_parquet(sc, path)
```


## Arguments

Argument      |Description
------------- |----------------
```x```     |     An object coercable to a Spark DataFrame (typically, a `tbl_spark` ).
```name```     |     The table name to assign to the saved Spark DataFrame.
```overwrite```     |     Boolean; overwrite a pre-existing table of the same name?
```append```     |     Boolean; append to a pre-existing table of the same name?
```sc```     |     A `spark_connection` object.
```path```     |     The path where the Spark DataFrame should be saved.

