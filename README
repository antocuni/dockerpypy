Docker images to build pypy; only the 32bit version so far.

At the moment is just a quick hack which works on my machine: in particular,
it mounts the directory /home/antocuni/pypy as a volume.

To use:

```
$ cd 32bit
$ make build
$ make run

$ # now we are inside the docker image
$ cd pypy/default/pypy/goal
$ ../../rpython/bin/rpython -Ojit targetpypystandalone.py
```
