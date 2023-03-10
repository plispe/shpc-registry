---
layout: container
name:  "quay.io/biocontainers/vgan"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/vgan/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/vgan/container.yaml"
updated_at: "2023-01-13 03:08:01.341923"
latest: "1.0.1--h9ee0642_0"
container_url: "https://biocontainers.pro/tools/vgan"
aliases:
 - "vgan"
versions:
 - "1.0.0--h9ee0642_0"
 - "1.0.1--h9ee0642_0"
description: "shpc-registry automated BioContainers addition for vgan"
config: {"url": "https://biocontainers.pro/tools/vgan", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for vgan", "latest": {"1.0.1--h9ee0642_0": "sha256:4e2802be45a59eaf31150ba13684d4b22ff5b3bbd1e7dbe5a9d64a69a2a8cd6d"}, "tags": {"1.0.0--h9ee0642_0": "sha256:f9dc8985ea433743023ff9499cd6c23e6cffdb1335b024d315bc47469f08926c", "1.0.1--h9ee0642_0": "sha256:4e2802be45a59eaf31150ba13684d4b22ff5b3bbd1e7dbe5a9d64a69a2a8cd6d"}, "docker": "quay.io/biocontainers/vgan", "aliases": {"vgan": "/usr/local/bin/vgan"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/vgan.
shpc-registry automated BioContainers addition for vgan
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/vgan
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/vgan:1.0.1--h9ee0642_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/vgan/1.0.1--h9ee0642_0
$ module help quay.io/biocontainers/vgan/1.0.1--h9ee0642_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### vgan-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### vgan-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### vgan-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### vgan-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### vgan-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### vgan-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### vgan

```bash
$ singularity exec <container> /usr/local/bin/vgan
$ podman run --it --rm --entrypoint /usr/local/bin/vgan   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/vgan   -v ${PWD} -w ${PWD} <container> -c " $@"
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