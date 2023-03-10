---
layout: container
name:  "quay.io/biocontainers/cafe"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/cafe/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/cafe/container.yaml"
updated_at: "2023-01-13 02:53:19.150442"
latest: "5.0.0--h5b5514e_1"
container_url: "https://biocontainers.pro/tools/cafe"
aliases:
 - "cafe5"
versions:
 - "5.0.0--h5b5514e_1"
description: "shpc-registry automated BioContainers addition for cafe"
config: {"url": "https://biocontainers.pro/tools/cafe", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for cafe", "latest": {"5.0.0--h5b5514e_1": "sha256:53927ab415c8c09c6e1070c5caa3d7f043b260becf9f3ced1bb62400b2a08bf2"}, "tags": {"5.0.0--h5b5514e_1": "sha256:53927ab415c8c09c6e1070c5caa3d7f043b260becf9f3ced1bb62400b2a08bf2"}, "docker": "quay.io/biocontainers/cafe", "aliases": {"cafe5": "/usr/local/bin/cafe5"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/cafe.
shpc-registry automated BioContainers addition for cafe
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/cafe
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/cafe:5.0.0--h5b5514e_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/cafe/5.0.0--h5b5514e_1
$ module help quay.io/biocontainers/cafe/5.0.0--h5b5514e_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### cafe-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### cafe-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### cafe-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### cafe-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### cafe-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### cafe-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### cafe5

```bash
$ singularity exec <container> /usr/local/bin/cafe5
$ podman run --it --rm --entrypoint /usr/local/bin/cafe5   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/cafe5   -v ${PWD} -w ${PWD} <container> -c " $@"
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