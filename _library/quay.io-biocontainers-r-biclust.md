---
layout: container
name:  "quay.io/biocontainers/r-biclust"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/r-biclust/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/r-biclust/container.yaml"
updated_at: "2023-01-13 03:26:55.494901"
latest: "1.2.0--r3.4.1_0"
container_url: "https://biocontainers.pro/tools/r-biclust"
aliases:
 - "ncurses5-config"
 - "ncursesw5-config"
versions:
 - "1.2.0--r3.4.1_0"
description: "shpc-registry automated BioContainers addition for r-biclust"
config: {"url": "https://biocontainers.pro/tools/r-biclust", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for r-biclust", "latest": {"1.2.0--r3.4.1_0": "sha256:d42998c72201856cdaf937dcde82abb50b83035e59e160721f4aaf2f618a4b8d"}, "tags": {"1.2.0--r3.4.1_0": "sha256:d42998c72201856cdaf937dcde82abb50b83035e59e160721f4aaf2f618a4b8d"}, "docker": "quay.io/biocontainers/r-biclust", "aliases": {"ncurses5-config": "/usr/local/bin/ncurses5-config", "ncursesw5-config": "/usr/local/bin/ncursesw5-config"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/r-biclust.
shpc-registry automated BioContainers addition for r-biclust
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/r-biclust
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/r-biclust:1.2.0--r3.4.1_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/r-biclust/1.2.0--r3.4.1_0
$ module help quay.io/biocontainers/r-biclust/1.2.0--r3.4.1_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### r-biclust-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### r-biclust-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### r-biclust-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### r-biclust-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### r-biclust-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### r-biclust-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### ncurses5-config

```bash
$ singularity exec <container> /usr/local/bin/ncurses5-config
$ podman run --it --rm --entrypoint /usr/local/bin/ncurses5-config   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/ncurses5-config   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### ncursesw5-config

```bash
$ singularity exec <container> /usr/local/bin/ncursesw5-config
$ podman run --it --rm --entrypoint /usr/local/bin/ncursesw5-config   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/ncursesw5-config   -v ${PWD} -w ${PWD} <container> -c " $@"
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