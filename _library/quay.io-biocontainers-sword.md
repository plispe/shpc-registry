---
layout: container
name:  "quay.io/biocontainers/sword"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/sword/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/sword/container.yaml"
updated_at: "2023-01-13 03:38:06.200478"
latest: "1.0.4--h9f5acd7_2"
container_url: "https://biocontainers.pro/tools/sword"
aliases:
 - "sword"
versions:
 - "1.0.4--h9f5acd7_2"
description: "shpc-registry automated BioContainers addition for sword"
config: {"url": "https://biocontainers.pro/tools/sword", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for sword", "latest": {"1.0.4--h9f5acd7_2": "sha256:61184b79d6d96c10de6e9479f9fc6420474edd67a5392b5e3c677194f8d1363d"}, "tags": {"1.0.4--h9f5acd7_2": "sha256:61184b79d6d96c10de6e9479f9fc6420474edd67a5392b5e3c677194f8d1363d"}, "docker": "quay.io/biocontainers/sword", "aliases": {"sword": "/usr/local/bin/sword"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/sword.
shpc-registry automated BioContainers addition for sword
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/sword
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/sword:1.0.4--h9f5acd7_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/sword/1.0.4--h9f5acd7_2
$ module help quay.io/biocontainers/sword/1.0.4--h9f5acd7_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### sword-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### sword-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### sword-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### sword-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### sword-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### sword-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### sword

```bash
$ singularity exec <container> /usr/local/bin/sword
$ podman run --it --rm --entrypoint /usr/local/bin/sword   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/sword   -v ${PWD} -w ${PWD} <container> -c " $@"
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