---
layout: container
name:  "quay.io/biocontainers/expat"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/expat/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/expat/container.yaml"
updated_at: "2023-01-13 02:58:30.940314"
latest: "2.1.0--0"
container_url: "https://biocontainers.pro/tools/expat"

versions:
 - "2.1.0--0"
description: "shpc-registry automated BioContainers addition for expat"
config: {"url": "https://biocontainers.pro/tools/expat", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for expat", "latest": {"2.1.0--0": "sha256:66b31c6f6e2771418f024b60a5582907dc792971b25cd72ce7718967b568523f"}, "tags": {"2.1.0--0": "sha256:66b31c6f6e2771418f024b60a5582907dc792971b25cd72ce7718967b568523f"}, "docker": "quay.io/biocontainers/expat"}
---

This module is a singularity container wrapper for quay.io/biocontainers/expat.
shpc-registry automated BioContainers addition for expat
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/expat
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/expat:2.1.0--0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/expat/2.1.0--0
$ module help quay.io/biocontainers/expat/2.1.0--0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### expat-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### expat-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### expat-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### expat-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### expat-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### expat-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### expat

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