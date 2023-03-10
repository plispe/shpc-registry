---
layout: container
name:  "quay.io/biocontainers/bioconductor-smad"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-smad/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-smad/container.yaml"
updated_at: "2023-01-13 02:49:52.681860"
latest: "1.14.0--r42hc247a5b_0"
container_url: "https://biocontainers.pro/tools/bioconductor-smad"
aliases:
 - "x86_64-conda-linux-gnu-gfortran.bin"
versions:
 - "1.8.0--r41h399db7b_0"
 - "1.14.0--r42hc247a5b_0"
 - "1.10.0--r41hc247a5b_2"
description: "shpc-registry automated BioContainers addition for bioconductor-smad"
config: {"url": "https://biocontainers.pro/tools/bioconductor-smad", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-smad", "latest": {"1.14.0--r42hc247a5b_0": "sha256:6c37cc5e8f6922a04dcaf41c6de8499471643f3191477847bdb186fea9c657f0"}, "tags": {"1.8.0--r41h399db7b_0": "sha256:a2b707a2eda3cb2c1e7763d528aaae9c7b7ce23a11e21b34909c80ca43d5b0a0", "1.14.0--r42hc247a5b_0": "sha256:6c37cc5e8f6922a04dcaf41c6de8499471643f3191477847bdb186fea9c657f0", "1.10.0--r41hc247a5b_2": "sha256:fb3c59477ffe879840cd9de51f40edbd258ea7adf854dc19f129b244c2ecdefe"}, "docker": "quay.io/biocontainers/bioconductor-smad", "aliases": {"x86_64-conda-linux-gnu-gfortran.bin": "/usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-smad.
shpc-registry automated BioContainers addition for bioconductor-smad
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-smad
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-smad:1.14.0--r42hc247a5b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-smad/1.14.0--r42hc247a5b_0
$ module help quay.io/biocontainers/bioconductor-smad/1.14.0--r42hc247a5b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-smad-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-smad-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-smad-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-smad-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-smad-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-smad-inspect-deffile:

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