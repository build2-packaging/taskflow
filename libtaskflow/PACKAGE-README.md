# libtaskflow - Img align="right" width="10%" src="image/taskflow_logo

This is a `build2` package for the [`<UPSTREAM-NAME>`](https://<UPSTREAM-URL>)
C++ library. It provides <SUMMARY-OF-FUNCTIONALITY>.


## Usage

To start using `libtaskflow` in your project, add the following `depends`
value to your `manifest`, adjusting the version constraint as appropriate:

```
depends: libtaskflow ^<VERSION>
```

Then import the library in your `buildfile`:

```
import libs = libtaskflow%lib{<TARGET>}
```


## Importable targets

This package provides the following importable targets:

```
lib{<TARGET>}
```

<DESCRIPTION-OF-IMPORTABLE-TARGETS>


## Configuration variables

This package provides the following configuration variables:

```
[bool] config.libtaskflow.<VARIABLE> ?= false
```

<DESCRIPTION-OF-CONFIG-VARIABLES>
