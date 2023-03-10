---
layout: container
name:  "quay.io/biocontainers/bioconductor-monocle"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-monocle/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-monocle/container.yaml"
updated_at: "2023-01-13 02:49:45.611054"
latest: "2.26.0--r42hc247a5b_0"
container_url: "https://biocontainers.pro/tools/bioconductor-monocle"
aliases:
 - "wget"
 - "ncurses5-config"
 - "ncursesw5-config"
versions:
 - "2.8.0--r341hfc679d8_0"
 - "2.26.0--r42hc247a5b_0"
 - "2.22.0--r41hc247a5b_2"
 - "2.20.0--r41h399db7b_0"
 - "2.18.0--r40h399db7b_2"
 - "2.16.0--r40h5f743cb_0"
description: "shpc-registry automated BioContainers addition for bioconductor-monocle"
config: {"url": "https://biocontainers.pro/tools/bioconductor-monocle", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-monocle", "latest": {"2.26.0--r42hc247a5b_0": "sha256:e9a8139512f2bd14a5ea1cfd28d2d295d23a58e7f89d0fdc5878f0ab15775fe7"}, "tags": {"2.8.0--r341hfc679d8_0": "sha256:a351da663530d44884ecb005cf40003b01a99da5b431fae7388753a04698e31b", "2.26.0--r42hc247a5b_0": "sha256:e9a8139512f2bd14a5ea1cfd28d2d295d23a58e7f89d0fdc5878f0ab15775fe7", "2.22.0--r41hc247a5b_2": "sha256:712af7b0a485ed214d67f103523379f7e7b0f13b52c236b383095b5933ba5295", "2.20.0--r41h399db7b_0": "sha256:51411ba7c19918c72e0fa85407c2ef666abf6057e54c5e4cdd00170def05eaf7", "2.18.0--r40h399db7b_2": "sha256:282c1b4d9064c8a08274ec13138ac15938ec5b6e52328f66c3b018843ba5896f", "2.16.0--r40h5f743cb_0": "sha256:2fae4aeec7b50901dc616a19e8637cc5ba3791c438bc90a1eb58d9500a7c1fc2"}, "docker": "quay.io/biocontainers/bioconductor-monocle", "aliases": {"wget": "/usr/local/bin/wget", "ncurses5-config": "/usr/local/bin/ncurses5-config", "ncursesw5-config": "/usr/local/bin/ncursesw5-config"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-monocle.
shpc-registry automated BioContainers addition for bioconductor-monocle
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-monocle
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-monocle:2.26.0--r42hc247a5b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-monocle/2.26.0--r42hc247a5b_0
$ module help quay.io/biocontainers/bioconductor-monocle/2.26.0--r42hc247a5b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-monocle-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-monocle-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-monocle-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-monocle-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-monocle-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-monocle-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### wget

```bash
$ singularity exec <container> /usr/local/bin/wget
$ podman run --it --rm --entrypoint /usr/local/bin/wget   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/wget   -v ${PWD} -w ${PWD} <container> -c " $@"
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