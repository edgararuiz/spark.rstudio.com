# `register_extension`: Register a Package that Implements a Spark Extension

## Description


 Registering an extension package will result in the package being
 automatically scanned for spark dependencies when a connection to Spark is
 created.


## Usage

```r
register_extension(package)
registered_extensions()
```


## Arguments

Argument      |Description
------------- |----------------
```package```     |     The package(s) to register.

## Note


 Packages should typically register their extensions in their
  `.onLoad` hook -- this ensures that their extensions are registered
 when their namespaces are loaded.


