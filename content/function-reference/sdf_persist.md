# `sdf_persist`: Persist a Spark DataFrame

## Description


 Persist a Spark DataFrame, forcing any pending computations and (optionally)
 serializing the results to disk.


## Usage

```r
sdf_persist(x, storage.level = "MEMORY_AND_DISK")
```


## Arguments

Argument      |Description
------------- |----------------
```x```     |     An object coercable to a Spark DataFrame (typically, a `tbl_spark` ).
```storage.level```     |     The storage level to be used. Please view the [Spark Documentation](http://spark.apache.org/docs/latest/programming-guide.html#rdd-persistence)  for information on what storage levels are accepted.

## Details


 Spark DataFrames invoke their operations lazily -- pending operations are
 deferred until their results are actually needed. Persisting a Spark
 DataFrame effectively 'forces' any pending computations, and then persists
 the generated Spark DataFrame as requested (to memory, to disk, or
 otherwise).
 
 Users of Spark should be careful to persist the results of any computations
 which are non-deterministic -- otherwise, one might see that the values
 within a column seem to 'change' as new operations are performed on that
 data set.


