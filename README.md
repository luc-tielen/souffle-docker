# souffle-docker

A docker image for running Souffle.

Usage:

```bash
# Building the image
$ docker build -f Dockerfile . -t souffle
# Launching a shell inside the container
$ docker run --rm -it souffle bash
# Building Datalog code (assuming there is a program.dl in $PWD
$ docker run -v $PWD:/code --rm -it souffle souffle -g /code/program.cpp /code/program.dl
```
