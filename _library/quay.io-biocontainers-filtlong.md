---
layout: container
name:  "quay.io/biocontainers/filtlong"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/filtlong/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/filtlong/container.yaml"
updated_at: "2023-01-13 03:11:32.467799"
latest: "0.2.1--hd03093a_1"
container_url: "https://biocontainers.pro/tools/filtlong"
aliases:
 - "filtlong"
versions:
 - "0.2.1--hd03093a_1"
description: "shpc-registry automated BioContainers addition for filtlong"
config: {"url": "https://biocontainers.pro/tools/filtlong", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for filtlong", "latest": {"0.2.1--hd03093a_1": "sha256:e53a2eb7c9880047f0767fe8315696265d14d2bf575aac973b4e72a2448b494b"}, "tags": {"0.2.1--hd03093a_1": "sha256:e53a2eb7c9880047f0767fe8315696265d14d2bf575aac973b4e72a2448b494b"}, "docker": "quay.io/biocontainers/filtlong", "aliases": {"filtlong": "/usr/local/bin/filtlong"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/filtlong.
shpc-registry automated BioContainers addition for filtlong
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/filtlong
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/filtlong:0.2.1--hd03093a_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/filtlong/0.2.1--hd03093a_1
$ module help quay.io/biocontainers/filtlong/0.2.1--hd03093a_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### filtlong-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### filtlong-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### filtlong-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### filtlong-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### filtlong-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### filtlong-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### filtlong

```bash
$ singularity exec <container> /usr/local/bin/filtlong
$ podman run --it --rm --entrypoint /usr/local/bin/filtlong   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/filtlong   -v ${PWD} -w ${PWD} <container> -c " $@"
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