# `spark_install`: Download and install various versions of Spark

## Description


 Install versions of Spark for use with local Spark connections
 (i.e. `spark_connect(master = "local"` )


## Usage

```r
spark_install(version = NULL, hadoop_version = NULL, reset = TRUE,
  logging = "INFO", verbose = interactive())
spark_uninstall(version, hadoop_version)
spark_install_dir()
spark_install_tar(tarfile)
spark_installed_versions()
spark_available_versions()
```


## Arguments

Argument      |Description
------------- |----------------
```version```     |     Version of Spark to install. See `spark_available_versions` for a list of supported versions
```hadoop_version```     |     Version of Hadoop to install. See `spark_available_versions` for a list of supported versions
```reset```     |     Attempts to reset settings to defaults.
```logging```     |     Logging level to configure install. Supported options: "WARN", "INFO"
```verbose```     |     Report information as Spark is downloaded / installed
```tarfile```     |     Path to TAR file conforming to the pattern spark-###-bin-(hadoop)?### where ### reference spark and hadoop versions respectively.

## Value


 List with information about the installed version.


