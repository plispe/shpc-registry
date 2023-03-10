---
layout: container
name:  "quay.io/biocontainers/chromap"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/chromap/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/chromap/container.yaml"
updated_at: "2023-01-13 03:15:34.220960"
latest: "0.2.3--hd03093a_1"
container_url: "https://biocontainers.pro/tools/chromap"
aliases:
 - "chromap"
versions:
 - "0.2.3--hd03093a_1"
description: "shpc-registry automated BioContainers addition for chromap"
config: {"url": "https://biocontainers.pro/tools/chromap", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for chromap", "latest": {"0.2.3--hd03093a_1": "sha256:9a8e62c7881cb59f42978d78eb55934ea11fd4fbfc01d0964b92dbf08e43e22c"}, "tags": {"0.2.3--hd03093a_1": "sha256:9a8e62c7881cb59f42978d78eb55934ea11fd4fbfc01d0964b92dbf08e43e22c"}, "docker": "quay.io/biocontainers/chromap", "aliases": {"chromap": "/usr/local/bin/chromap"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/chromap.
shpc-registry automated BioContainers addition for chromap
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/chromap
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/chromap:0.2.3--hd03093a_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/chromap/0.2.3--hd03093a_1
$ module help quay.io/biocontainers/chromap/0.2.3--hd03093a_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### chromap-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### chromap-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### chromap-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### chromap-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### chromap-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### chromap-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### chromap

```bash
$ singularity exec <container> /usr/local/bin/chromap
$ podman run --it --rm --entrypoint /usr/local/bin/chromap   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/chromap   -v ${PWD} -w ${PWD} <container> -c " $@"
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