---
layout: container
name:  "quay.io/biocontainers/micropita"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/micropita/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/micropita/container.yaml"
updated_at: "2023-01-13 02:56:47.179629"
latest: "1.1.0--1"
container_url: "https://biocontainers.pro/tools/micropita"

versions:
 - "1.1.0--1"
description: "shpc-registry automated BioContainers addition for micropita"
config: {"url": "https://biocontainers.pro/tools/micropita", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for micropita", "latest": {"1.1.0--1": "sha256:d77cdd9a2b9967242c4fd1494e9dd1d7b9032622c9dccc26cacbde073b428a9a"}, "tags": {"1.1.0--1": "sha256:d77cdd9a2b9967242c4fd1494e9dd1d7b9032622c9dccc26cacbde073b428a9a"}, "docker": "quay.io/biocontainers/micropita"}
---

This module is a singularity container wrapper for quay.io/biocontainers/micropita.
shpc-registry automated BioContainers addition for micropita
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/micropita
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/micropita:1.1.0--1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/micropita/1.1.0--1
$ module help quay.io/biocontainers/micropita/1.1.0--1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### micropita-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### micropita-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### micropita-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### micropita-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### micropita-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### micropita-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### micropita

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