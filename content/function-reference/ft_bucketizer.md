# `ft_bucketizer`: Feature Transformation -- Bucketizer

## Description


 Similar to list() 's [`cut`](cut.html) function, this transforms a numeric column
 into a discretized column, with breaks specified through the `splits` 
 parameter.


## Usage

```r
ft_bucketizer(x, input.col = NULL, output.col = NULL, splits, ...)
```


## Arguments

Argument      |Description
------------- |----------------
```x```     |     An object (usually a `spark_tbl` ) coercable to a Spark DataFrame.
```input.col```     |     The name of the input column(s).
```output.col```     |     The name of the output column.
```splits```     |     A numeric vector of cutpoints, indicating the bucket boundaries.
```...```     |     Optional arguments; currently unused.

## Seealso


 See [http://spark.apache.org/docs/latest/ml-features.html](http://spark.apache.org/docs/latest/ml-features.html) for
 more information on the set of transformations available for DataFrame
 columns in Spark.
 
 Other feature transformation routines: [`ft_binarizer`](ft_binarizer.html) ,
  [`ft_count_vectorizer`](ft_count_vectorizer.html) ,
  [`ft_discrete_cosine_transform`](ft_discrete_cosine_transform.html) ,
  [`ft_elementwise_product`](ft_elementwise_product.html) ,
  [`ft_index_to_string`](ft_index_to_string.html) ,
  [`ft_one_hot_encoder`](ft_one_hot_encoder.html) ,
  [`ft_quantile_discretizer`](ft_quantile_discretizer.html) ,
  [`ft_regex_tokenizer`](ft_regex_tokenizer.html) ,
  [`ft_sql_transformer`](ft_sql_transformer.html) ,
  [`ft_string_indexer`](ft_string_indexer.html) ,
  [`ft_tokenizer`](ft_tokenizer.html) ,
  [`ft_vector_assembler`](ft_vector_assembler.html) ,
  [`sdf_mutate`](sdf_mutate.html) 


