---
layout: container
name:  "quay.io/biocontainers/simwalk2"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/simwalk2/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/simwalk2/container.yaml"
updated_at: "2023-01-13 03:20:47.721513"
latest: "2.91--hb2e0dee_4"
container_url: "https://biocontainers.pro/tools/simwalk2"
aliases:
 - "simwalk2"
versions:
 - "2.91--hb2e0dee_4"
description: "shpc-registry automated BioContainers addition for simwalk2"
config: {"url": "https://biocontainers.pro/tools/simwalk2", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for simwalk2", "latest": {"2.91--hb2e0dee_4": "sha256:ebf2afe6ca3fca8d4827a9542d6711ab1b748fb90958c7b11f7531f0a295571b"}, "tags": {"2.91--hb2e0dee_4": "sha256:ebf2afe6ca3fca8d4827a9542d6711ab1b748fb90958c7b11f7531f0a295571b"}, "docker": "quay.io/biocontainers/simwalk2", "aliases": {"simwalk2": "/usr/local/bin/simwalk2"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/simwalk2.
shpc-registry automated BioContainers addition for simwalk2
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/simwalk2
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/simwalk2:2.91--hb2e0dee_4
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/simwalk2/2.91--hb2e0dee_4
$ module help quay.io/biocontainers/simwalk2/2.91--hb2e0dee_4
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### simwalk2-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### simwalk2-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### simwalk2-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### simwalk2-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### simwalk2-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### simwalk2-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### simwalk2

```bash
$ singularity exec <container> /usr/local/bin/simwalk2
$ podman run --it --rm --entrypoint /usr/local/bin/simwalk2   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/simwalk2   -v ${PWD} -w ${PWD} <container> -c " $@"
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