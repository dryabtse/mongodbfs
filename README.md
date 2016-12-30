# mongodbfs

## Installation

1) Add these lines to `/etc/mc/mc.ext`

```
# mongodb
regex/i/\.mongodb$
        Open=%cd %p/mongodbfs://
```

2) Place the `mongodbfs` script under `/usr/lib/mc/extfs.d/`

## Usage

Create a `*.mongodb` file containing a MongoDB URI as a single string
