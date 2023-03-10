---
layout: container
name:  "quay.io/biocontainers/prot-scriber"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/prot-scriber/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/prot-scriber/container.yaml"
updated_at: "2023-01-13 03:06:32.527217"
latest: "0.1.4--hec16e2b_0"
container_url: "https://biocontainers.pro/tools/prot-scriber"
aliases:
 - "prot-scriber"
versions:
 - "0.1.4--hec16e2b_0"
description: "singularity registry hpc automated addition for prot-scriber"
config: {"url": "https://biocontainers.pro/tools/prot-scriber", "maintainer": "@vsoch", "description": "singularity registry hpc automated addition for prot-scriber", "latest": {"0.1.4--hec16e2b_0": "sha256:8c825e56691649ace668e3019ce802672dc32ee8208bc7d0edfe55174b15c49b"}, "tags": {"0.1.4--hec16e2b_0": "sha256:8c825e56691649ace668e3019ce802672dc32ee8208bc7d0edfe55174b15c49b"}, "docker": "quay.io/biocontainers/prot-scriber", "aliases": {"prot-scriber": "/usr/local/bin/prot-scriber"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/prot-scriber.
singularity registry hpc automated addition for prot-scriber
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/prot-scriber
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/prot-scriber:0.1.4--hec16e2b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/prot-scriber/0.1.4--hec16e2b_0
$ module help quay.io/biocontainers/prot-scriber/0.1.4--hec16e2b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### prot-scriber-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### prot-scriber-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### prot-scriber-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### prot-scriber-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### prot-scriber-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### prot-scriber-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### prot-scriber

```bash
$ singularity exec <container> /usr/local/bin/prot-scriber
$ podman run --it --rm --entrypoint /usr/local/bin/prot-scriber   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/prot-scriber   -v ${PWD} -w ${PWD} <container> -c " $@"
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