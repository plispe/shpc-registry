---
layout: container
name:  "quay.io/biocontainers/nanoq"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/nanoq/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/nanoq/container.yaml"
updated_at: "2023-01-13 03:02:46.274997"
latest: "0.9.0--hec16e2b_1"
container_url: "https://biocontainers.pro/tools/nanoq"
aliases:
 - "nanoq"
versions:
 - "0.9.0--hec16e2b_1"
description: "shpc-registry automated BioContainers addition for nanoq"
config: {"url": "https://biocontainers.pro/tools/nanoq", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for nanoq", "latest": {"0.9.0--hec16e2b_1": "sha256:af189ba24d7292e77f3d429517685f4b5e2a711f9213bc1c0dfa29da1af9b5a7"}, "tags": {"0.9.0--hec16e2b_1": "sha256:af189ba24d7292e77f3d429517685f4b5e2a711f9213bc1c0dfa29da1af9b5a7"}, "docker": "quay.io/biocontainers/nanoq", "aliases": {"nanoq": "/usr/local/bin/nanoq"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/nanoq.
shpc-registry automated BioContainers addition for nanoq
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/nanoq
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/nanoq:0.9.0--hec16e2b_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/nanoq/0.9.0--hec16e2b_1
$ module help quay.io/biocontainers/nanoq/0.9.0--hec16e2b_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### nanoq-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### nanoq-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### nanoq-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### nanoq-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### nanoq-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### nanoq-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### nanoq

```bash
$ singularity exec <container> /usr/local/bin/nanoq
$ podman run --it --rm --entrypoint /usr/local/bin/nanoq   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/nanoq   -v ${PWD} -w ${PWD} <container> -c " $@"
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