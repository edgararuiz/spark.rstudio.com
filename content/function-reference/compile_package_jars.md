# `compile_package_jars`: Compile Scala sources into a Java Archive (jar)

## Description


 Compile the `scala` source files contained within an list() package
 into a Java Archive ( `jar` ) file that can be loaded and used within
 a Spark environment.


## Usage

```r
compile_package_jars(..., spec = NULL)
```


## Arguments

Argument      |Description
------------- |----------------
```...```     |     Optional compilation specifications, as generated by `spark_compilation_spec` . When no arguments are passed, `spark_default_compilation_spec` is used instead.
```spec```     |     An optional list of compilation specifications. When set, this option takes precedence over arguments passed to `...` .

