---
layout: container
name:  "quay.io/biocontainers/sam"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/sam/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/sam/container.yaml"
updated_at: "2023-01-13 03:26:38.631294"
latest: "3.5--1"
container_url: "https://biocontainers.pro/tools/sam"

versions:
 - "3.5--1"
description: "shpc-registry automated BioContainers addition for sam"
config: {"url": "https://biocontainers.pro/tools/sam", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for sam", "latest": {"3.5--1": "sha256:a14041ebedab5db21783ac3877f4d192e43ccb3c149c6d1f134ad3c333ca39d5"}, "tags": {"3.5--1": "sha256:a14041ebedab5db21783ac3877f4d192e43ccb3c149c6d1f134ad3c333ca39d5"}, "docker": "quay.io/biocontainers/sam"}
---

This module is a singularity container wrapper for quay.io/biocontainers/sam.
shpc-registry automated BioContainers addition for sam
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/sam
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/sam:3.5--1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/sam/3.5--1
$ module help quay.io/biocontainers/sam/3.5--1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### sam-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### sam-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### sam-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### sam-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### sam-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### sam-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### sam

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