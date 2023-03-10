---
layout: container
name:  "quay.io/biocontainers/bioconductor-dsqtl"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-dsqtl/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-dsqtl/container.yaml"
updated_at: "2023-01-13 02:51:34.630105"
latest: "0.28.0--r40hdfd78af_1"
container_url: "https://biocontainers.pro/tools/bioconductor-dsqtl"
aliases:
 - "x86_64-conda-linux-gnu-gfortran.bin"
versions:
 - "0.28.0--r40hdfd78af_1"
description: "shpc-registry automated BioContainers addition for bioconductor-dsqtl"
config: {"url": "https://biocontainers.pro/tools/bioconductor-dsqtl", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-dsqtl", "latest": {"0.28.0--r40hdfd78af_1": "sha256:9496488702608b2a631e1d33db2d7a989d567a4d85c9b60582df66097177138a"}, "tags": {"0.28.0--r40hdfd78af_1": "sha256:9496488702608b2a631e1d33db2d7a989d567a4d85c9b60582df66097177138a"}, "docker": "quay.io/biocontainers/bioconductor-dsqtl", "aliases": {"x86_64-conda-linux-gnu-gfortran.bin": "/usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-dsqtl.
shpc-registry automated BioContainers addition for bioconductor-dsqtl
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-dsqtl
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-dsqtl:0.28.0--r40hdfd78af_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-dsqtl/0.28.0--r40hdfd78af_1
$ module help quay.io/biocontainers/bioconductor-dsqtl/0.28.0--r40hdfd78af_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-dsqtl-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-dsqtl-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-dsqtl-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-dsqtl-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-dsqtl-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-dsqtl-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### x86_64-conda-linux-gnu-gfortran.bin

```bash
$ singularity exec <container> /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin
$ podman run --it --rm --entrypoint /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin   -v ${PWD} -w ${PWD} <container> -c " $@"
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