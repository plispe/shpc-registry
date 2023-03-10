---
layout: container
name:  "quay.io/biocontainers/yass"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/yass/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/yass/container.yaml"
updated_at: "2023-01-13 03:02:16.714708"
latest: "1.14--hec16e2b_4"
container_url: "https://biocontainers.pro/tools/yass"
aliases:
 - "yass"
versions:
 - "1.14--hec16e2b_4"
description: "shpc-registry automated BioContainers addition for yass"
config: {"url": "https://biocontainers.pro/tools/yass", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for yass", "latest": {"1.14--hec16e2b_4": "sha256:113978fad44a05bd09585d62a1fc6df4e33b7c5f3bd01c305039d8641abe1fd4"}, "tags": {"1.14--hec16e2b_4": "sha256:113978fad44a05bd09585d62a1fc6df4e33b7c5f3bd01c305039d8641abe1fd4"}, "docker": "quay.io/biocontainers/yass", "aliases": {"yass": "/usr/local/bin/yass"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/yass.
shpc-registry automated BioContainers addition for yass
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/yass
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/yass:1.14--hec16e2b_4
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/yass/1.14--hec16e2b_4
$ module help quay.io/biocontainers/yass/1.14--hec16e2b_4
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### yass-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### yass-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### yass-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### yass-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### yass-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### yass-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### yass

```bash
$ singularity exec <container> /usr/local/bin/yass
$ podman run --it --rm --entrypoint /usr/local/bin/yass   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/yass   -v ${PWD} -w ${PWD} <container> -c " $@"
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