---
layout: container
name:  "quay.io/biocontainers/bioconductor-rsamtools"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-rsamtools/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-rsamtools/container.yaml"
updated_at: "2023-01-13 02:59:55.617387"
latest: "2.14.0--r42hc247a5b_0"
container_url: "https://biocontainers.pro/tools/bioconductor-rsamtools"
aliases:
 - "x86_64-conda-linux-gnu-gfortran.bin"
versions:
 - "2.8.0--r41h399db7b_0"
 - "2.14.0--r42hc247a5b_0"
 - "2.10.0--r41hc247a5b_2"
description: "shpc-registry automated BioContainers addition for bioconductor-rsamtools"
config: {"url": "https://biocontainers.pro/tools/bioconductor-rsamtools", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-rsamtools", "latest": {"2.14.0--r42hc247a5b_0": "sha256:3304ee07aaf448e94400a20b54205480511334ca36cfbd4b7b28b4ee3fcd0b6d"}, "tags": {"2.8.0--r41h399db7b_0": "sha256:f1a30562969e0e5c44438411b893f1dd2d55896f54429dd38e6ba5d48542d486", "2.14.0--r42hc247a5b_0": "sha256:3304ee07aaf448e94400a20b54205480511334ca36cfbd4b7b28b4ee3fcd0b6d", "2.10.0--r41hc247a5b_2": "sha256:5019fffc2c980107a193227ab25c907ec1453c608817cd7be190ec106f3e15e9"}, "docker": "quay.io/biocontainers/bioconductor-rsamtools", "aliases": {"x86_64-conda-linux-gnu-gfortran.bin": "/usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-rsamtools.
shpc-registry automated BioContainers addition for bioconductor-rsamtools
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-rsamtools
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-rsamtools:2.14.0--r42hc247a5b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-rsamtools/2.14.0--r42hc247a5b_0
$ module help quay.io/biocontainers/bioconductor-rsamtools/2.14.0--r42hc247a5b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-rsamtools-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-rsamtools-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-rsamtools-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-rsamtools-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-rsamtools-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-rsamtools-inspect-deffile:

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