---
layout: container
name:  "quay.io/biocontainers/pblat"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/pblat/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/pblat/container.yaml"
updated_at: "2023-01-13 03:44:41.533364"
latest: "2.5--h0e0aaa8_2"
container_url: "https://biocontainers.pro/tools/pblat"
aliases:
 - "pblat"
versions:
 - "2.5--h0e0aaa8_2"
description: "shpc-registry automated BioContainers addition for pblat"
config: {"url": "https://biocontainers.pro/tools/pblat", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for pblat", "latest": {"2.5--h0e0aaa8_2": "sha256:07898573fc6ed4747ee08443d2268b9f2adc7a38aaf3bf61ac67be64289d5ec5"}, "tags": {"2.5--h0e0aaa8_2": "sha256:07898573fc6ed4747ee08443d2268b9f2adc7a38aaf3bf61ac67be64289d5ec5"}, "docker": "quay.io/biocontainers/pblat", "aliases": {"pblat": "/usr/local/bin/pblat"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/pblat.
shpc-registry automated BioContainers addition for pblat
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/pblat
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/pblat:2.5--h0e0aaa8_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/pblat/2.5--h0e0aaa8_2
$ module help quay.io/biocontainers/pblat/2.5--h0e0aaa8_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### pblat-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### pblat-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### pblat-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### pblat-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### pblat-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### pblat-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### pblat

```bash
$ singularity exec <container> /usr/local/bin/pblat
$ podman run --it --rm --entrypoint /usr/local/bin/pblat   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pblat   -v ${PWD} -w ${PWD} <container> -c " $@"
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