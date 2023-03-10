---
layout: container
name:  "quay.io/biocontainers/rustybam"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/rustybam/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/rustybam/container.yaml"
updated_at: "2023-01-13 02:52:54.990273"
latest: "0.1.31--hc52b9a9_0"
container_url: "https://biocontainers.pro/tools/rustybam"
aliases:
 - "rb"
 - "rustybam"
versions:
 - "0.1.30--hc52b9a9_1"
 - "0.1.31--hc52b9a9_0"
description: "shpc-registry automated BioContainers addition for rustybam"
config: {"url": "https://biocontainers.pro/tools/rustybam", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for rustybam", "latest": {"0.1.31--hc52b9a9_0": "sha256:168d060c5f48fba1b0b125a1df02f8f5a4d28e7eab0e0f9f6a32266f65101db5"}, "tags": {"0.1.30--hc52b9a9_1": "sha256:e056aa9311c66cad3c2d34cda1ea4636defe9621040e764a8ebbd18573080771", "0.1.31--hc52b9a9_0": "sha256:168d060c5f48fba1b0b125a1df02f8f5a4d28e7eab0e0f9f6a32266f65101db5"}, "docker": "quay.io/biocontainers/rustybam", "aliases": {"rb": "/usr/local/bin/rb", "rustybam": "/usr/local/bin/rustybam"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/rustybam.
shpc-registry automated BioContainers addition for rustybam
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/rustybam
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/rustybam:0.1.31--hc52b9a9_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/rustybam/0.1.31--hc52b9a9_0
$ module help quay.io/biocontainers/rustybam/0.1.31--hc52b9a9_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### rustybam-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### rustybam-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### rustybam-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### rustybam-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### rustybam-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### rustybam-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### rb

```bash
$ singularity exec <container> /usr/local/bin/rb
$ podman run --it --rm --entrypoint /usr/local/bin/rb   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/rb   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### rustybam

```bash
$ singularity exec <container> /usr/local/bin/rustybam
$ podman run --it --rm --entrypoint /usr/local/bin/rustybam   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/rustybam   -v ${PWD} -w ${PWD} <container> -c " $@"
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