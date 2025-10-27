# libtaskflow - General-purpose Task-parallel Programming System

This is a `build2` package for the [`taskflow`](https://github.com/taskflow/taskflow)
C++ library. It provides task decomposition strategies that incorporate
both regular and irregular compute patterns, together with a work-stealing
scheduler to optimize your multithreaded performance.


## Usage

To start using `libtaskflow` in your project, add the following `depends`
value to your `manifest`, adjusting the version constraint as appropriate:

```
depends: libtaskflow ^3.10.0
```

Then import the library in your `buildfile`:

```
import libs = libtaskflow%lib{taskflow}
```


## Importable targets

This package provides the following importable targets:

```
lib{taskflow}
```

Taskflow lets you quickly implement task decomposition strategies
that incorporate both regular and irregular compute patterns,
together with an efficient *work-stealing* scheduler to optimize your
multithreaded performance.


## Configuration variables

This package provides the following configuration variables:

```
[bool] config.libtaskflow.task_pool ?= true
[bool] config.libtaskflow.atomic_notifier ?= ($cxx.std >= 20)

[bool] config.libtaskflow.cuda ?= false
```

- `task_pool`       : Enable/Disable task pool optimization.
- `atomic_notifier` : Enable/Disable atomic notifier (requires C++20).
- `cuda`            : Enable/Disable the `<taskflow/cuda/...>` headers.
