---
layout: container
name:  "quay.io/biocontainers/r-cssam"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/r-cssam/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/r-cssam/container.yaml"
updated_at: "2023-01-13 03:12:56.876420"
latest: "1.4--r41h9f5acd7_3"
container_url: "https://biocontainers.pro/tools/r-cssam"

versions:
 - "1.4--r41h9f5acd7_2"
 - "1.4--r41h9f5acd7_3"
description: "shpc-registry automated BioContainers addition for r-cssam"
config: {"url": "https://biocontainers.pro/tools/r-cssam", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for r-cssam", "latest": {"1.4--r41h9f5acd7_3": "sha256:0f03926cc646a9ca355a6f49cd7979340c58f3f65ebad6957a1205eb9d483ed8"}, "tags": {"1.4--r41h9f5acd7_2": "sha256:6ff08b7ca96f736267a5e21b4c459183531bf7a264f593c6719b20f1fff4fcbf", "1.4--r41h9f5acd7_3": "sha256:0f03926cc646a9ca355a6f49cd7979340c58f3f65ebad6957a1205eb9d483ed8"}, "docker": "quay.io/biocontainers/r-cssam"}
---

This module is a singularity container wrapper for quay.io/biocontainers/r-cssam.
shpc-registry automated BioContainers addition for r-cssam
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/r-cssam
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/r-cssam:1.4--r41h9f5acd7_3
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/r-cssam/1.4--r41h9f5acd7_3
$ module help quay.io/biocontainers/r-cssam/1.4--r41h9f5acd7_3
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### r-cssam-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### r-cssam-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### r-cssam-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### r-cssam-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### r-cssam-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### r-cssam-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### r-cssam

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