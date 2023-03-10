---
layout: container
name:  "quay.io/biocontainers/bioconductor-guitar"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-guitar/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-guitar/container.yaml"
updated_at: "2023-01-13 03:00:32.255312"
latest: "2.14.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-guitar"
aliases:
 - "x86_64-conda-linux-gnu-gfortran.bin"
versions:
 - "2.8.0--r41hdfd78af_0"
 - "2.14.0--r42hdfd78af_0"
 - "2.10.0--r41hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-guitar"
config: {"url": "https://biocontainers.pro/tools/bioconductor-guitar", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-guitar", "latest": {"2.14.0--r42hdfd78af_0": "sha256:6b7a70274ae67005a211ce5ea18b826de2c2063e13e0fe899b3b689582dbbde6"}, "tags": {"2.8.0--r41hdfd78af_0": "sha256:981df27e5f77e1ad25f7595f116aaff11ee15851295a004b3d5c3e2a5919a75b", "2.14.0--r42hdfd78af_0": "sha256:6b7a70274ae67005a211ce5ea18b826de2c2063e13e0fe899b3b689582dbbde6", "2.10.0--r41hdfd78af_0": "sha256:ae0a9c96a7df734dd67820350ebffd4b7659d6395fba0d4528012c4298bc88d8"}, "docker": "quay.io/biocontainers/bioconductor-guitar", "aliases": {"x86_64-conda-linux-gnu-gfortran.bin": "/usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-guitar.
shpc-registry automated BioContainers addition for bioconductor-guitar
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-guitar
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-guitar:2.14.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-guitar/2.14.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-guitar/2.14.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-guitar-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-guitar-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-guitar-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-guitar-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-guitar-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-guitar-inspect-deffile:

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