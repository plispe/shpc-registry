---
layout: container
name:  "quay.io/biocontainers/dig2"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/dig2/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/dig2/container.yaml"
updated_at: "2023-01-13 03:36:50.348820"
latest: "1.0--hec16e2b_4"
container_url: "https://biocontainers.pro/tools/dig2"
aliases:
 - "dig2"
versions:
 - "1.0--hec16e2b_4"
description: "shpc-registry automated BioContainers addition for dig2"
config: {"url": "https://biocontainers.pro/tools/dig2", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for dig2", "latest": {"1.0--hec16e2b_4": "sha256:40f977a1846ea2fe50b3c42ee11323b6f0bb86af1d75e6ec149552eed22cb86e"}, "tags": {"1.0--hec16e2b_4": "sha256:40f977a1846ea2fe50b3c42ee11323b6f0bb86af1d75e6ec149552eed22cb86e"}, "docker": "quay.io/biocontainers/dig2", "aliases": {"dig2": "/usr/local/bin/dig2"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/dig2.
shpc-registry automated BioContainers addition for dig2
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/dig2
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/dig2:1.0--hec16e2b_4
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/dig2/1.0--hec16e2b_4
$ module help quay.io/biocontainers/dig2/1.0--hec16e2b_4
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### dig2-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### dig2-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### dig2-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### dig2-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### dig2-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### dig2-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### dig2

```bash
$ singularity exec <container> /usr/local/bin/dig2
$ podman run --it --rm --entrypoint /usr/local/bin/dig2   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/dig2   -v ${PWD} -w ${PWD} <container> -c " $@"
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