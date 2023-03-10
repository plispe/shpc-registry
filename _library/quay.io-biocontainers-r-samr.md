---
layout: container
name:  "quay.io/biocontainers/r-samr"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/r-samr/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/r-samr/container.yaml"
updated_at: "2023-01-13 03:31:54.215110"
latest: "3.0--r42hec16e2b_6"
container_url: "https://biocontainers.pro/tools/r-samr"

versions:
 - "3.0--r41hec16e2b_5"
 - "3.0--r42hec16e2b_6"
description: "shpc-registry automated BioContainers addition for r-samr"
config: {"url": "https://biocontainers.pro/tools/r-samr", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for r-samr", "latest": {"3.0--r42hec16e2b_6": "sha256:598dcdf87e158d871857594b289b8a378758bc4cd0f1024efb2eba6a9ea08e95"}, "tags": {"3.0--r41hec16e2b_5": "sha256:a239cf260718c3285f25d9a3954d246dfd2bc6ed44826843720a0dbb45d95f68", "3.0--r42hec16e2b_6": "sha256:598dcdf87e158d871857594b289b8a378758bc4cd0f1024efb2eba6a9ea08e95"}, "docker": "quay.io/biocontainers/r-samr"}
---

This module is a singularity container wrapper for quay.io/biocontainers/r-samr.
shpc-registry automated BioContainers addition for r-samr
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/r-samr
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/r-samr:3.0--r42hec16e2b_6
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/r-samr/3.0--r42hec16e2b_6
$ module help quay.io/biocontainers/r-samr/3.0--r42hec16e2b_6
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### r-samr-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### r-samr-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### r-samr-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### r-samr-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### r-samr-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### r-samr-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### r-samr

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