---
layout: container
name:  "quay.io/biocontainers/starcode"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/starcode/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/starcode/container.yaml"
updated_at: "2023-01-13 03:21:39.028175"
latest: "1.4--hec16e2b_2"
container_url: "https://biocontainers.pro/tools/starcode"
aliases:
 - "starcode"
versions:
 - "1.4--hec16e2b_2"
description: "shpc-registry automated BioContainers addition for starcode"
config: {"url": "https://biocontainers.pro/tools/starcode", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for starcode", "latest": {"1.4--hec16e2b_2": "sha256:130c9c6d1dd73e5b7e28c79c7ef798ce3beab3603679767c8d31e0eb36825aac"}, "tags": {"1.4--hec16e2b_2": "sha256:130c9c6d1dd73e5b7e28c79c7ef798ce3beab3603679767c8d31e0eb36825aac"}, "docker": "quay.io/biocontainers/starcode", "aliases": {"starcode": "/usr/local/bin/starcode"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/starcode.
shpc-registry automated BioContainers addition for starcode
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/starcode
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/starcode:1.4--hec16e2b_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/starcode/1.4--hec16e2b_2
$ module help quay.io/biocontainers/starcode/1.4--hec16e2b_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### starcode-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### starcode-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### starcode-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### starcode-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### starcode-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### starcode-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### starcode

```bash
$ singularity exec <container> /usr/local/bin/starcode
$ podman run --it --rm --entrypoint /usr/local/bin/starcode   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/starcode   -v ${PWD} -w ${PWD} <container> -c " $@"
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