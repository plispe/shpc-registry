---
layout: container
name:  "quay.io/biocontainers/fgwas"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/fgwas/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/fgwas/container.yaml"
updated_at: "2023-01-13 03:28:09.309824"
latest: "0.3.6--heafd8fd_5"
container_url: "https://biocontainers.pro/tools/fgwas"
aliases:
 - "fgwas"
 - "test"
versions:
 - "0.3.6--heafd8fd_5"
description: "shpc-registry automated BioContainers addition for fgwas"
config: {"url": "https://biocontainers.pro/tools/fgwas", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for fgwas", "latest": {"0.3.6--heafd8fd_5": "sha256:912312c92a31d147493dc1977ccd48d229a9acc493b347a5029d1fa7a41c28cb"}, "tags": {"0.3.6--heafd8fd_5": "sha256:912312c92a31d147493dc1977ccd48d229a9acc493b347a5029d1fa7a41c28cb"}, "docker": "quay.io/biocontainers/fgwas", "aliases": {"fgwas": "/usr/local/bin/fgwas", "test": "/usr/local/bin/test"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/fgwas.
shpc-registry automated BioContainers addition for fgwas
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/fgwas
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/fgwas:0.3.6--heafd8fd_5
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/fgwas/0.3.6--heafd8fd_5
$ module help quay.io/biocontainers/fgwas/0.3.6--heafd8fd_5
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### fgwas-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### fgwas-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### fgwas-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### fgwas-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### fgwas-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### fgwas-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### fgwas

```bash
$ singularity exec <container> /usr/local/bin/fgwas
$ podman run --it --rm --entrypoint /usr/local/bin/fgwas   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/fgwas   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### test

```bash
$ singularity exec <container> /usr/local/bin/test
$ podman run --it --rm --entrypoint /usr/local/bin/test   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/test   -v ${PWD} -w ${PWD} <container> -c " $@"
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