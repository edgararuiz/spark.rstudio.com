# `spark_compile`: Compile Scala sources into a Java Archive

## Description


 Given a set of `scala` source files, compile them
 into a Java Archive ( `jar` ).


## Usage

```r
spark_compile(jar_name, spark_home = NULL, filter = NULL, scalac = NULL,
  jar = NULL, jar_dep = NULL)
```


## Arguments

Argument      |Description
------------- |----------------
```spark_home```     |     The path to the Spark sources to be used alongside compilation.
```filter```     |     An optional function, used to filter out discovered `scala`  files during compilation. This can be used to ensure that e.g. certain files are only compiled with certain versions of Spark, and so on.
```scalac```     |     The path to the `scalac` program to be used, for compilation of `scala` files.
```jar```     |     The path to the `jar` program to be used, for generating of the resulting `jar` .
```jar_dep```     |     An optional list of additional `jar` dependencies.
```name```     |     The name to assign to the target `jar` .

