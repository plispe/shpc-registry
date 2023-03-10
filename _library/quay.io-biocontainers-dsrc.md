---
layout: container
name:  "quay.io/biocontainers/dsrc"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/dsrc/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/dsrc/container.yaml"
updated_at: "2023-01-13 03:03:29.147174"
latest: "2015.06.04--h7ff8a90_4"
container_url: "https://biocontainers.pro/tools/dsrc"
aliases:
 - "dsrc"
versions:
 - "2015.06.04--h7ff8a90_4"
description: "shpc-registry automated BioContainers addition for dsrc"
config: {"url": "https://biocontainers.pro/tools/dsrc", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for dsrc", "latest": {"2015.06.04--h7ff8a90_4": "sha256:c09ee47a183d8abed7ca2de63e23f2e1e02e185328a5096e786ddd75109964ef"}, "tags": {"2015.06.04--h7ff8a90_4": "sha256:c09ee47a183d8abed7ca2de63e23f2e1e02e185328a5096e786ddd75109964ef"}, "docker": "quay.io/biocontainers/dsrc", "aliases": {"dsrc": "/usr/local/bin/dsrc"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/dsrc.
shpc-registry automated BioContainers addition for dsrc
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/dsrc
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/dsrc:2015.06.04--h7ff8a90_4
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/dsrc/2015.06.04--h7ff8a90_4
$ module help quay.io/biocontainers/dsrc/2015.06.04--h7ff8a90_4
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### dsrc-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### dsrc-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### dsrc-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### dsrc-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### dsrc-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### dsrc-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### dsrc

```bash
$ singularity exec <container> /usr/local/bin/dsrc
$ podman run --it --rm --entrypoint /usr/local/bin/dsrc   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/dsrc   -v ${PWD} -w ${PWD} <container> -c " $@"
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