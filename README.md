# mongodbfs

## Installation (Linux)

1) Install PyMongo

```
pip install pymongo
```

2) Add these lines to `/etc/mc/mc.ext`

```
# mongodb
regex/i/\.mongodb$
        Open=%cd %p/mongodbfs://
```

3) Place the `mongodbfs` script under `/usr/lib/mc/extfs.d/`

## Usage

Create a `*.mongodb` file containing a MongoDB URI as a single string. For example

```
$ cat mubuntu.mongodb 
mongodb://mubuntu:9088
```

You can then highlight the file by the cursor in `mc` and hit `Enter` - that should open the VFS.
