---
layout: container
name:  "quay.io/biocontainers/bioconductor-greengenes13.5mgdb"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-greengenes13.5mgdb/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-greengenes13.5mgdb/container.yaml"
updated_at: "2023-01-13 02:54:32.433896"
latest: "2.0.0--r40hdfd78af_6"
container_url: "https://biocontainers.pro/tools/bioconductor-greengenes13.5mgdb"
aliases:
 - "x86_64-conda-linux-gnu-gfortran.bin"
versions:
 - "2.0.0--r40hdfd78af_6"
description: "shpc-registry automated BioContainers addition for bioconductor-greengenes13.5mgdb"
config: {"url": "https://biocontainers.pro/tools/bioconductor-greengenes13.5mgdb", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-greengenes13.5mgdb", "latest": {"2.0.0--r40hdfd78af_6": "sha256:8bcd9b39f01e46ea77e46de9d7586be44dac8157fc78994e84515b73209f41a8"}, "tags": {"2.0.0--r40hdfd78af_6": "sha256:8bcd9b39f01e46ea77e46de9d7586be44dac8157fc78994e84515b73209f41a8"}, "docker": "quay.io/biocontainers/bioconductor-greengenes13.5mgdb", "aliases": {"x86_64-conda-linux-gnu-gfortran.bin": "/usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-greengenes13.5mgdb.
shpc-registry automated BioContainers addition for bioconductor-greengenes13.5mgdb
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-greengenes13.5mgdb
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-greengenes13.5mgdb:2.0.0--r40hdfd78af_6
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-greengenes13.5mgdb/2.0.0--r40hdfd78af_6
$ module help quay.io/biocontainers/bioconductor-greengenes13.5mgdb/2.0.0--r40hdfd78af_6
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-greengenes13.5mgdb-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-greengenes13.5mgdb-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-greengenes13.5mgdb-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-greengenes13.5mgdb-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-greengenes13.5mgdb-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-greengenes13.5mgdb-inspect-deffile:

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