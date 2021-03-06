# `livy_install`: Install Livy

## Description


 Automatically download and install [list("livy")](http://livy.io/) .
 livy provides a REST API to Spark.
 
 Find the LIVY_HOME directory for a given version of Livy that
 was previously installed using [`livy_install`](livy_install.html) .


## Usage

```r
livy_install(version = "0.3.0", spark_home = NULL, spark_version = NULL)
livy_available_versions()
livy_install_dir()
livy_installed_versions()
livy_home_dir(version = NULL)
```


## Arguments

Argument      |Description
------------- |----------------
```version```     |     The version of livy to be installed.
```spark_home```     |     The path to a Spark installation. The downloaded and installed version of livy will then be associated with this Spark installation. When unset ( NULL ), the value is inferred based on the value of spark_version supplied.
```spark_version```     |     The version of Spark to use. When unset ( NULL ), the value is inferred based on the value of livy_version supplied. A version of Spark known to be compatible with the requested version of livy is chosen when possible.
```version```     |     Version of Livy

## Value


 Path to LIVY_HOME (or `NULL` if the specified version
 was not found).


