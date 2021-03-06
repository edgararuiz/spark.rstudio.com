# `sdf_separate_column`: Separate a Vector Column into Scalar Columns

## Description


 Given a vector column in a Spark DataFrame, split that
 into `n` separate columns, each column made up of
 the different elements in the column `column` .


## Usage

```r
sdf_separate_column(x, column, into = NULL)
```


## Arguments

Argument      |Description
------------- |----------------
```x```     |     An object coercable to a Spark DataFrame (typically, a `tbl_spark` ).
```column```     |     The name of a (vector-typed) column.
```into```     |     A specification of the columns that should be generated from `column` . This can either be a vector of column names, or an list() list mapping column names to the (1-based) index at which a particular vector element should be extracted.

