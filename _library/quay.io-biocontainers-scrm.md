---
layout: container
name:  "quay.io/biocontainers/scrm"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/scrm/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/scrm/container.yaml"
updated_at: "2023-01-13 03:12:07.497696"
latest: "1.7.4--h9f5acd7_2"
container_url: "https://biocontainers.pro/tools/scrm"
aliases:
 - "scrm"
versions:
 - "1.7.4--h9f5acd7_2"
description: "shpc-registry automated BioContainers addition for scrm"
config: {"url": "https://biocontainers.pro/tools/scrm", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for scrm", "latest": {"1.7.4--h9f5acd7_2": "sha256:efea949a39e5b1fdbdccc5e871995dedf0e7327fa0a7791e42ea04fdf7b2477c"}, "tags": {"1.7.4--h9f5acd7_2": "sha256:efea949a39e5b1fdbdccc5e871995dedf0e7327fa0a7791e42ea04fdf7b2477c"}, "docker": "quay.io/biocontainers/scrm", "aliases": {"scrm": "/usr/local/bin/scrm"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/scrm.
shpc-registry automated BioContainers addition for scrm
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/scrm
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/scrm:1.7.4--h9f5acd7_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/scrm/1.7.4--h9f5acd7_2
$ module help quay.io/biocontainers/scrm/1.7.4--h9f5acd7_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### scrm-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### scrm-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### scrm-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### scrm-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### scrm-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### scrm-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### scrm

```bash
$ singularity exec <container> /usr/local/bin/scrm
$ podman run --it --rm --entrypoint /usr/local/bin/scrm   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/scrm   -v ${PWD} -w ${PWD} <container> -c " $@"
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