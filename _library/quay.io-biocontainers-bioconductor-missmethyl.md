---
layout: container
name:  "quay.io/biocontainers/bioconductor-missmethyl"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-missmethyl/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-missmethyl/container.yaml"
updated_at: "2023-01-13 03:45:06.428338"
latest: "1.32.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-missmethyl"
aliases:
 - "x86_64-conda-linux-gnu-gfortran.bin"
versions:
 - "1.26.0--r41hdfd78af_0"
 - "1.32.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-missmethyl"
config: {"url": "https://biocontainers.pro/tools/bioconductor-missmethyl", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-missmethyl", "latest": {"1.32.0--r42hdfd78af_0": "sha256:820a426a01944f1883331d4b314537f1ded09f532f3b4555a5f2b168e0d49fe1"}, "tags": {"1.26.0--r41hdfd78af_0": "sha256:232a00f7a738d72a7bec65af2ec860614d64d310a82fdcc5baab6c69c86839a9", "1.32.0--r42hdfd78af_0": "sha256:820a426a01944f1883331d4b314537f1ded09f532f3b4555a5f2b168e0d49fe1"}, "docker": "quay.io/biocontainers/bioconductor-missmethyl", "aliases": {"x86_64-conda-linux-gnu-gfortran.bin": "/usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-missmethyl.
shpc-registry automated BioContainers addition for bioconductor-missmethyl
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-missmethyl
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-missmethyl:1.32.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-missmethyl/1.32.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-missmethyl/1.32.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-missmethyl-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-missmethyl-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-missmethyl-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-missmethyl-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-missmethyl-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-missmethyl-inspect-deffile:

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