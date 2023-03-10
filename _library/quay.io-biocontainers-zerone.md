---
layout: container
name:  "quay.io/biocontainers/zerone"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/zerone/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/zerone/container.yaml"
updated_at: "2023-01-13 03:30:28.744329"
latest: "1.0--h7132678_4"
container_url: "https://biocontainers.pro/tools/zerone"
aliases:
 - "zerone"
versions:
 - "1.0--h7132678_4"
description: "shpc-registry automated BioContainers addition for zerone"
config: {"url": "https://biocontainers.pro/tools/zerone", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for zerone", "latest": {"1.0--h7132678_4": "sha256:bf6485873c9659356c16f57d9c641534e6916e77b3d7a58089346a747f3fd72a"}, "tags": {"1.0--h7132678_4": "sha256:bf6485873c9659356c16f57d9c641534e6916e77b3d7a58089346a747f3fd72a"}, "docker": "quay.io/biocontainers/zerone", "aliases": {"zerone": "/usr/local/bin/zerone"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/zerone.
shpc-registry automated BioContainers addition for zerone
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/zerone
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/zerone:1.0--h7132678_4
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/zerone/1.0--h7132678_4
$ module help quay.io/biocontainers/zerone/1.0--h7132678_4
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### zerone-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### zerone-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### zerone-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### zerone-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### zerone-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### zerone-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### zerone

```bash
$ singularity exec <container> /usr/local/bin/zerone
$ podman run --it --rm --entrypoint /usr/local/bin/zerone   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/zerone   -v ${PWD} -w ${PWD} <container> -c " $@"
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