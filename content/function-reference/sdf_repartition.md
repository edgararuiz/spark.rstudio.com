# `sdf_repartition`: Repartition a Spark DataFrame

## Description


 Repartition a Spark DataFrame


## Usage

```r
sdf_repartition(x, partitions = NULL, partition_by = NULL)
```


## Arguments

Argument      |Description
------------- |----------------
```x```     |     An object coercable to a Spark DataFrame (typically, a `tbl_spark` ).
```partitions```     |     number of partitions
```partition_by```     |     vector of column names used for partitioning, only supported for Spark 2.0+

