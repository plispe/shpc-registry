---
layout: container
name:  "quay.io/biocontainers/wtdbg"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/wtdbg/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/wtdbg/container.yaml"
updated_at: "2023-01-13 02:57:20.352604"
latest: "2.5--h5b5514e_2"
container_url: "https://biocontainers.pro/tools/wtdbg"

versions:
 - "2.5--h5b5514e_2"
description: "shpc-registry automated BioContainers addition for wtdbg"
config: {"url": "https://biocontainers.pro/tools/wtdbg", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for wtdbg", "latest": {"2.5--h5b5514e_2": "sha256:463392406f8c4a36e48b2d23b158014778301ceb754ec5c5b6c0ba3fabc67038"}, "tags": {"2.5--h5b5514e_2": "sha256:463392406f8c4a36e48b2d23b158014778301ceb754ec5c5b6c0ba3fabc67038"}, "docker": "quay.io/biocontainers/wtdbg"}
---

This module is a singularity container wrapper for quay.io/biocontainers/wtdbg.
shpc-registry automated BioContainers addition for wtdbg
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/wtdbg
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/wtdbg:2.5--h5b5514e_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/wtdbg/2.5--h5b5514e_2
$ module help quay.io/biocontainers/wtdbg/2.5--h5b5514e_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### wtdbg-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### wtdbg-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### wtdbg-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### wtdbg-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### wtdbg-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### wtdbg-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### wtdbg

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