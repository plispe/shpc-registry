---
layout: container
name:  "quay.io/biocontainers/r-metap"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/r-metap/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/r-metap/container.yaml"
updated_at: "2023-01-13 03:44:32.969868"
latest: "1.4--r42h3121a25_2"
container_url: "https://biocontainers.pro/tools/r-metap"
aliases:
 - "x86_64-conda-linux-gnu-gfortran.bin"
versions:
 - "1.4--r41h3121a25_1"
 - "1.4--r42h3121a25_2"
description: "shpc-registry automated BioContainers addition for r-metap"
config: {"url": "https://biocontainers.pro/tools/r-metap", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for r-metap", "latest": {"1.4--r42h3121a25_2": "sha256:c49f87abf837f3a7c3bb4a37043c438888e3e1d89eecb6a1f427bcd0cb9325a1"}, "tags": {"1.4--r41h3121a25_1": "sha256:00a941d0f27796d7324acce24ff54ee9626b23e5c3db7b0c060a81e32c831def", "1.4--r42h3121a25_2": "sha256:c49f87abf837f3a7c3bb4a37043c438888e3e1d89eecb6a1f427bcd0cb9325a1"}, "docker": "quay.io/biocontainers/r-metap", "aliases": {"x86_64-conda-linux-gnu-gfortran.bin": "/usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/r-metap.
shpc-registry automated BioContainers addition for r-metap
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/r-metap
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/r-metap:1.4--r42h3121a25_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/r-metap/1.4--r42h3121a25_2
$ module help quay.io/biocontainers/r-metap/1.4--r42h3121a25_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### r-metap-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### r-metap-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### r-metap-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### r-metap-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### r-metap-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### r-metap-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### x86_64-conda-linux-gnu-gfortran.bin

```bash
$ singularity exec <container> /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin
$ podman run --it --rm --entrypoint /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin   -v ${PWD} -w ${PWD} <container> -c " $@"
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