---
layout: container
name:  "quay.io/biocontainers/itsxpress"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/itsxpress/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/itsxpress/container.yaml"
updated_at: "2023-01-13 03:15:48.045424"
latest: "1.8.0--pyhdfd78af_2"
container_url: "https://biocontainers.pro/tools/itsxpress"
aliases:
 - "aclocal.bak"
 - "autoheader.bak"
 - "autom4te.bak"
 - "automake.bak"
 - "autoreconf.bak"
 - "autoscan.bak"
 - "autoupdate.bak"
 - "ifnames.bak"
 - "itsxpress"
 - "kmutate.sh"
 - "runhmm.sh"
 - "kmerposition.sh"
 - "reformatpb.sh"
 - "summarizecoverage.sh"
 - "alltoall.sh"
 - "analyzesketchresults.sh"
 - "comparessu.sh"
 - "filtersilva.sh"
 - "sketchblacklist2.sh"
versions:
 - "1.8.0--pyhdfd78af_2"
description: "shpc-registry automated BioContainers addition for itsxpress"
config: {"url": "https://biocontainers.pro/tools/itsxpress", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for itsxpress", "latest": {"1.8.0--pyhdfd78af_2": "sha256:688a48b2d785bc59556d33d3520450fcd6b206d95a5034c7fb245c37d6f6838c"}, "tags": {"1.8.0--pyhdfd78af_2": "sha256:688a48b2d785bc59556d33d3520450fcd6b206d95a5034c7fb245c37d6f6838c"}, "docker": "quay.io/biocontainers/itsxpress", "aliases": {"aclocal.bak": "/usr/local/bin/aclocal.bak", "autoheader.bak": "/usr/local/bin/autoheader.bak", "autom4te.bak": "/usr/local/bin/autom4te.bak", "automake.bak": "/usr/local/bin/automake.bak", "autoreconf.bak": "/usr/local/bin/autoreconf.bak", "autoscan.bak": "/usr/local/bin/autoscan.bak", "autoupdate.bak": "/usr/local/bin/autoupdate.bak", "ifnames.bak": "/usr/local/bin/ifnames.bak", "itsxpress": "/usr/local/bin/itsxpress", "kmutate.sh": "/usr/local/bin/kmutate.sh", "runhmm.sh": "/usr/local/bin/runhmm.sh", "kmerposition.sh": "/usr/local/bin/kmerposition.sh", "reformatpb.sh": "/usr/local/bin/reformatpb.sh", "summarizecoverage.sh": "/usr/local/bin/summarizecoverage.sh", "alltoall.sh": "/usr/local/bin/alltoall.sh", "analyzesketchresults.sh": "/usr/local/bin/analyzesketchresults.sh", "comparessu.sh": "/usr/local/bin/comparessu.sh", "filtersilva.sh": "/usr/local/bin/filtersilva.sh", "sketchblacklist2.sh": "/usr/local/bin/sketchblacklist2.sh"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/itsxpress.
shpc-registry automated BioContainers addition for itsxpress
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/itsxpress
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/itsxpress:1.8.0--pyhdfd78af_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/itsxpress/1.8.0--pyhdfd78af_2
$ module help quay.io/biocontainers/itsxpress/1.8.0--pyhdfd78af_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### itsxpress-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### itsxpress-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### itsxpress-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### itsxpress-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### itsxpress-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### itsxpress-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### aclocal.bak

```bash
$ singularity exec <container> /usr/local/bin/aclocal.bak
$ podman run --it --rm --entrypoint /usr/local/bin/aclocal.bak   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/aclocal.bak   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### autoheader.bak

```bash
$ singularity exec <container> /usr/local/bin/autoheader.bak
$ podman run --it --rm --entrypoint /usr/local/bin/autoheader.bak   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/autoheader.bak   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### autom4te.bak

```bash
$ singularity exec <container> /usr/local/bin/autom4te.bak
$ podman run --it --rm --entrypoint /usr/local/bin/autom4te.bak   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/autom4te.bak   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### automake.bak

```bash
$ singularity exec <container> /usr/local/bin/automake.bak
$ podman run --it --rm --entrypoint /usr/local/bin/automake.bak   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/automake.bak   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### autoreconf.bak

```bash
$ singularity exec <container> /usr/local/bin/autoreconf.bak
$ podman run --it --rm --entrypoint /usr/local/bin/autoreconf.bak   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/autoreconf.bak   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### autoscan.bak

```bash
$ singularity exec <container> /usr/local/bin/autoscan.bak
$ podman run --it --rm --entrypoint /usr/local/bin/autoscan.bak   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/autoscan.bak   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### autoupdate.bak

```bash
$ singularity exec <container> /usr/local/bin/autoupdate.bak
$ podman run --it --rm --entrypoint /usr/local/bin/autoupdate.bak   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/autoupdate.bak   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### ifnames.bak

```bash
$ singularity exec <container> /usr/local/bin/ifnames.bak
$ podman run --it --rm --entrypoint /usr/local/bin/ifnames.bak   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/ifnames.bak   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### itsxpress

```bash
$ singularity exec <container> /usr/local/bin/itsxpress
$ podman run --it --rm --entrypoint /usr/local/bin/itsxpress   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/itsxpress   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### kmutate.sh

```bash
$ singularity exec <container> /usr/local/bin/kmutate.sh
$ podman run --it --rm --entrypoint /usr/local/bin/kmutate.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/kmutate.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### runhmm.sh

```bash
$ singularity exec <container> /usr/local/bin/runhmm.sh
$ podman run --it --rm --entrypoint /usr/local/bin/runhmm.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/runhmm.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### kmerposition.sh

```bash
$ singularity exec <container> /usr/local/bin/kmerposition.sh
$ podman run --it --rm --entrypoint /usr/local/bin/kmerposition.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/kmerposition.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### reformatpb.sh

```bash
$ singularity exec <container> /usr/local/bin/reformatpb.sh
$ podman run --it --rm --entrypoint /usr/local/bin/reformatpb.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/reformatpb.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### summarizecoverage.sh

```bash
$ singularity exec <container> /usr/local/bin/summarizecoverage.sh
$ podman run --it --rm --entrypoint /usr/local/bin/summarizecoverage.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/summarizecoverage.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### alltoall.sh

```bash
$ singularity exec <container> /usr/local/bin/alltoall.sh
$ podman run --it --rm --entrypoint /usr/local/bin/alltoall.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/alltoall.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### analyzesketchresults.sh

```bash
$ singularity exec <container> /usr/local/bin/analyzesketchresults.sh
$ podman run --it --rm --entrypoint /usr/local/bin/analyzesketchresults.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/analyzesketchresults.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### comparessu.sh

```bash
$ singularity exec <container> /usr/local/bin/comparessu.sh
$ podman run --it --rm --entrypoint /usr/local/bin/comparessu.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/comparessu.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### filtersilva.sh

```bash
$ singularity exec <container> /usr/local/bin/filtersilva.sh
$ podman run --it --rm --entrypoint /usr/local/bin/filtersilva.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/filtersilva.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### sketchblacklist2.sh

```bash
$ singularity exec <container> /usr/local/bin/sketchblacklist2.sh
$ podman run --it --rm --entrypoint /usr/local/bin/sketchblacklist2.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/sketchblacklist2.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```



In the above, the `<container>` directive will reference an actual container provided
by the module, for the version you have chosen to load. An environment file in the
module folder will also be bound. Note that although a container
might provide custom commands, every container exposes unique exec, shell, run, and
inspect aliases. For anycommands above, you can export:

 - SINGULARITY_OPTS: to define custom options for singularity (e.g., --debug)
 - SINGULARITY_COMMAND_OPTS: to define custom options for the command (e.g., -b)
 - PODMAN_OPTS: to define custom options for podman or docker
 - PODMAN_COMMAND_OPTS: to define custom options for the command

<br>

### Install

You can install shpc locally (for yourself or your user base) as follows:

```bash
$ git clone https://github.com/singularityhub/singularity-hpc
$ cd singularity-hpc
$ pip install -e .
```

Have any questions, or want to request a new module or version? [ask for help!](https://github.com/singularityhub/singularity-hpc/issues)