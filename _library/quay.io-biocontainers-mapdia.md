---
layout: container
name:  "quay.io/biocontainers/mapdia"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/mapdia/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/mapdia/container.yaml"
updated_at: "2023-01-13 03:21:43.542807"
latest: "3.1.0--h87f3376_3"
container_url: "https://biocontainers.pro/tools/mapdia"
aliases:
 - "mapDIA"
versions:
 - "3.1.0--h87f3376_3"
description: "shpc-registry automated BioContainers addition for mapdia"
config: {"url": "https://biocontainers.pro/tools/mapdia", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for mapdia", "latest": {"3.1.0--h87f3376_3": "sha256:5dd2e76310560a97ac9bffb2d9b9392fd3db34e39a004e87b1639da5d2ed47b7"}, "tags": {"3.1.0--h87f3376_3": "sha256:5dd2e76310560a97ac9bffb2d9b9392fd3db34e39a004e87b1639da5d2ed47b7"}, "docker": "quay.io/biocontainers/mapdia", "aliases": {"mapDIA": "/usr/local/bin/mapDIA"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/mapdia.
shpc-registry automated BioContainers addition for mapdia
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/mapdia
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/mapdia:3.1.0--h87f3376_3
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/mapdia/3.1.0--h87f3376_3
$ module help quay.io/biocontainers/mapdia/3.1.0--h87f3376_3
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### mapdia-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### mapdia-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### mapdia-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### mapdia-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### mapdia-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### mapdia-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### mapDIA

```bash
$ singularity exec <container> /usr/local/bin/mapDIA
$ podman run --it --rm --entrypoint /usr/local/bin/mapDIA   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/mapDIA   -v ${PWD} -w ${PWD} <container> -c " $@"
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