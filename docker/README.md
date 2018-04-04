## Create the Docker Image ##

A quick refresher on docker commands is available at the [docker cheatsheet](https://github.com/wsargent/docker-cheat-sheet).

A docker image with all required prerequisites can be built with the `Makefile` in this directory:

```
make operational_build
```

## Test the Docker Image ##

Having built the docker image we can now test it:

```
docker run -ti monitoring-node-utils geojson-merge --help
usage: geojson-merge [-s] FILE FILE2 FILE3

  --stream (or -s): use streaming mode for large files
```
