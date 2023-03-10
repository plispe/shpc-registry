---
layout: container
name:  "quay.io/biocontainers/r-wgcna"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/r-wgcna/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/r-wgcna/container.yaml"
updated_at: "2023-01-13 02:54:41.782502"
latest: "1.71--r42hecf12ef_2"
container_url: "https://biocontainers.pro/tools/r-wgcna"

versions:
 - "1.71--r41hecf12ef_0"
 - "1.71--r42hecf12ef_2"
description: "shpc-registry automated BioContainers addition for r-wgcna"
config: {"url": "https://biocontainers.pro/tools/r-wgcna", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for r-wgcna", "latest": {"1.71--r42hecf12ef_2": "sha256:1ed10b40e891b9aeadfb004b4b2f5445117f7cd4bf45e54fef6131d20ea79361"}, "tags": {"1.71--r41hecf12ef_0": "sha256:cf8283be7ca15cb9cd473d76baebdc0ba3d0b46b14a89ec1334095c36d3f2f7e", "1.71--r42hecf12ef_2": "sha256:1ed10b40e891b9aeadfb004b4b2f5445117f7cd4bf45e54fef6131d20ea79361"}, "docker": "quay.io/biocontainers/r-wgcna"}
---

This module is a singularity container wrapper for quay.io/biocontainers/r-wgcna.
shpc-registry automated BioContainers addition for r-wgcna
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/r-wgcna
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/r-wgcna:1.71--r42hecf12ef_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/r-wgcna/1.71--r42hecf12ef_2
$ module help quay.io/biocontainers/r-wgcna/1.71--r42hecf12ef_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### r-wgcna-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### r-wgcna-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### r-wgcna-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### r-wgcna-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### r-wgcna-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### r-wgcna-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### r-wgcna

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
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