---
layout: container
name:  "quay.io/biocontainers/bioconductor-rmagpie"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-rmagpie/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-rmagpie/container.yaml"
updated_at: "2023-01-13 03:02:47.097432"
latest: "1.54.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-rmagpie"

versions:
 - "1.50.0--r41hdfd78af_0"
 - "1.54.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-rmagpie"
config: {"url": "https://biocontainers.pro/tools/bioconductor-rmagpie", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-rmagpie", "latest": {"1.54.0--r42hdfd78af_0": "sha256:c028acc5bfd72a65477a6ff269c21fabb3ae3b52ea9ff9fdd1b93569174efb3e"}, "tags": {"1.50.0--r41hdfd78af_0": "sha256:f86e8e25483f89ba04854c1b9983ebcaf7c4d9f986d34e1357ea80fc2de84f98", "1.54.0--r42hdfd78af_0": "sha256:c028acc5bfd72a65477a6ff269c21fabb3ae3b52ea9ff9fdd1b93569174efb3e"}, "docker": "quay.io/biocontainers/bioconductor-rmagpie"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-rmagpie.
shpc-registry automated BioContainers addition for bioconductor-rmagpie
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-rmagpie
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-rmagpie:1.54.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-rmagpie/1.54.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-rmagpie/1.54.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-rmagpie-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-rmagpie-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-rmagpie-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-rmagpie-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-rmagpie-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-rmagpie-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-rmagpie

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
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