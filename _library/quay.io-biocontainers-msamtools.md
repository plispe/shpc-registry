---
layout: container
name:  "quay.io/biocontainers/msamtools"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/msamtools/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/msamtools/container.yaml"
updated_at: "2023-01-13 02:58:54.274628"
latest: "1.1.0--h7132678_1"
container_url: "https://biocontainers.pro/tools/msamtools"
aliases:
 - "msamtools"
versions:
 - "1.1.0--h7132678_1"
description: "shpc-registry automated BioContainers addition for msamtools"
config: {"url": "https://biocontainers.pro/tools/msamtools", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for msamtools", "latest": {"1.1.0--h7132678_1": "sha256:8e1d08bc288c309dcc266e7817d4a8342e0f2aa3b551a8c7949ea22c8337b1ea"}, "tags": {"1.1.0--h7132678_1": "sha256:8e1d08bc288c309dcc266e7817d4a8342e0f2aa3b551a8c7949ea22c8337b1ea"}, "docker": "quay.io/biocontainers/msamtools", "aliases": {"msamtools": "/usr/local/bin/msamtools"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/msamtools.
shpc-registry automated BioContainers addition for msamtools
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/msamtools
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/msamtools:1.1.0--h7132678_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/msamtools/1.1.0--h7132678_1
$ module help quay.io/biocontainers/msamtools/1.1.0--h7132678_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### msamtools-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### msamtools-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### msamtools-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### msamtools-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### msamtools-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### msamtools-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### msamtools

```bash
$ singularity exec <container> /usr/local/bin/msamtools
$ podman run --it --rm --entrypoint /usr/local/bin/msamtools   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/msamtools   -v ${PWD} -w ${PWD} <container> -c " $@"
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