---
layout: container
name:  "quay.io/biocontainers/mustang"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/mustang/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/mustang/container.yaml"
updated_at: "2023-01-13 03:10:52.948731"
latest: "3.2.3--h2d50403_1"
container_url: "https://biocontainers.pro/tools/mustang"
aliases:
 - "mustang"
versions:
 - "3.2.3--h2d50403_1"
description: "shpc-registry automated BioContainers addition for mustang"
config: {"url": "https://biocontainers.pro/tools/mustang", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for mustang", "latest": {"3.2.3--h2d50403_1": "sha256:3af4616105496cfb71fb8bc740914f2e73ccd937180c6a8946d9d906f63f587d"}, "tags": {"3.2.3--h2d50403_1": "sha256:3af4616105496cfb71fb8bc740914f2e73ccd937180c6a8946d9d906f63f587d"}, "docker": "quay.io/biocontainers/mustang", "aliases": {"mustang": "/usr/local/bin/mustang"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/mustang.
shpc-registry automated BioContainers addition for mustang
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/mustang
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/mustang:3.2.3--h2d50403_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/mustang/3.2.3--h2d50403_1
$ module help quay.io/biocontainers/mustang/3.2.3--h2d50403_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### mustang-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### mustang-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### mustang-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### mustang-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### mustang-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### mustang-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### mustang

```bash
$ singularity exec <container> /usr/local/bin/mustang
$ podman run --it --rm --entrypoint /usr/local/bin/mustang   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/mustang   -v ${PWD} -w ${PWD} <container> -c " $@"
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