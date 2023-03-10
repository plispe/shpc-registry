---
layout: container
name:  "quay.io/biocontainers/knot"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/knot/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/knot/container.yaml"
updated_at: "2023-01-13 03:11:24.551639"
latest: "1.0.0--1"
container_url: "https://biocontainers.pro/tools/knot"

versions:
 - "1.0.0--1"
description: "shpc-registry automated BioContainers addition for knot"
config: {"url": "https://biocontainers.pro/tools/knot", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for knot", "latest": {"1.0.0--1": "sha256:f680b35239cd806eb9c387ed6644088c5f4664a959b7c0fc4a2784822291fb19"}, "tags": {"1.0.0--1": "sha256:f680b35239cd806eb9c387ed6644088c5f4664a959b7c0fc4a2784822291fb19"}, "docker": "quay.io/biocontainers/knot"}
---

This module is a singularity container wrapper for quay.io/biocontainers/knot.
shpc-registry automated BioContainers addition for knot
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/knot
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/knot:1.0.0--1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/knot/1.0.0--1
$ module help quay.io/biocontainers/knot/1.0.0--1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### knot-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### knot-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### knot-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### knot-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### knot-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### knot-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### knot

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