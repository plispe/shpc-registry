---
layout: container
name:  "quay.io/biocontainers/bioconductor-gpumagic"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-gpumagic/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-gpumagic/container.yaml"
updated_at: "2023-01-13 02:56:34.130734"
latest: "1.14.0--r42hc247a5b_0"
container_url: "https://biocontainers.pro/tools/bioconductor-gpumagic"
aliases:
 - "x86_64-conda-linux-gnu-gfortran.bin"
versions:
 - "1.8.0--r41h399db7b_0"
 - "1.14.0--r42hc247a5b_0"
 - "1.10.0--r41h619a076_1"
description: "shpc-registry automated BioContainers addition for bioconductor-gpumagic"
config: {"url": "https://biocontainers.pro/tools/bioconductor-gpumagic", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-gpumagic", "latest": {"1.14.0--r42hc247a5b_0": "sha256:3c73af63c14dc74c5fde9efa0af35406488eea7db5407eda29eb8dc95bd237a0"}, "tags": {"1.8.0--r41h399db7b_0": "sha256:c3f94f30b30c35d1b78b6dd2d5c548839bd77e3f8b972427a6e833e3dd4f1b9d", "1.14.0--r42hc247a5b_0": "sha256:3c73af63c14dc74c5fde9efa0af35406488eea7db5407eda29eb8dc95bd237a0", "1.10.0--r41h619a076_1": "sha256:fc7f15d78b2abd3a82706c0f00448aa25f3086bd0c9fb69e32eef8cce1a09573"}, "docker": "quay.io/biocontainers/bioconductor-gpumagic", "aliases": {"x86_64-conda-linux-gnu-gfortran.bin": "/usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-gpumagic.
shpc-registry automated BioContainers addition for bioconductor-gpumagic
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-gpumagic
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-gpumagic:1.14.0--r42hc247a5b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-gpumagic/1.14.0--r42hc247a5b_0
$ module help quay.io/biocontainers/bioconductor-gpumagic/1.14.0--r42hc247a5b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-gpumagic-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-gpumagic-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-gpumagic-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-gpumagic-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-gpumagic-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-gpumagic-inspect-deffile:

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