---
layout: container
name:  "quay.io/biocontainers/bioconductor-beachmat"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-beachmat/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-beachmat/container.yaml"
updated_at: "2023-01-13 03:35:10.197019"
latest: "2.14.0--r42hc247a5b_0"
container_url: "https://biocontainers.pro/tools/bioconductor-beachmat"
aliases:
 - "x86_64-conda-linux-gnu-gfortran.bin"
versions:
 - "2.8.0--r41h399db7b_0"
 - "2.14.0--r42hc247a5b_0"
 - "2.10.0--r41hc247a5b_2"
description: "shpc-registry automated BioContainers addition for bioconductor-beachmat"
config: {"url": "https://biocontainers.pro/tools/bioconductor-beachmat", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-beachmat", "latest": {"2.14.0--r42hc247a5b_0": "sha256:f24cbf0d202ad3a5091f8c0cb35440f57c83880ff5757d01ac52c9acf0bd75db"}, "tags": {"2.8.0--r41h399db7b_0": "sha256:59f89eeaa0653e777d623574f908dd365141b2f4ca040d2df35f90fff9676927", "2.14.0--r42hc247a5b_0": "sha256:f24cbf0d202ad3a5091f8c0cb35440f57c83880ff5757d01ac52c9acf0bd75db", "2.10.0--r41hc247a5b_2": "sha256:e69c1cce07f67cb7248da843f945e32332b94d91bc72e27dd2c36ae70a200a2d"}, "docker": "quay.io/biocontainers/bioconductor-beachmat", "aliases": {"x86_64-conda-linux-gnu-gfortran.bin": "/usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-beachmat.
shpc-registry automated BioContainers addition for bioconductor-beachmat
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-beachmat
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-beachmat:2.14.0--r42hc247a5b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-beachmat/2.14.0--r42hc247a5b_0
$ module help quay.io/biocontainers/bioconductor-beachmat/2.14.0--r42hc247a5b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-beachmat-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-beachmat-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-beachmat-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-beachmat-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-beachmat-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-beachmat-inspect-deffile:

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