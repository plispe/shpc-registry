---
layout: container
name:  "quay.io/biocontainers/nucamino"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/nucamino/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/nucamino/container.yaml"
updated_at: "2023-01-13 03:40:29.817197"
latest: "0.1.3--h9ee0642_2"
container_url: "https://biocontainers.pro/tools/nucamino"
aliases:
 - "nucamino"
versions:
 - "0.1.3--h9ee0642_2"
description: "shpc-registry automated BioContainers addition for nucamino"
config: {"url": "https://biocontainers.pro/tools/nucamino", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for nucamino", "latest": {"0.1.3--h9ee0642_2": "sha256:daa0f35e8474307c5353cbd4b4c976b075150f0c1c0a5d8cf9544d8c3f3ce246"}, "tags": {"0.1.3--h9ee0642_2": "sha256:daa0f35e8474307c5353cbd4b4c976b075150f0c1c0a5d8cf9544d8c3f3ce246"}, "docker": "quay.io/biocontainers/nucamino", "aliases": {"nucamino": "/usr/local/bin/nucamino"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/nucamino.
shpc-registry automated BioContainers addition for nucamino
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/nucamino
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/nucamino:0.1.3--h9ee0642_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/nucamino/0.1.3--h9ee0642_2
$ module help quay.io/biocontainers/nucamino/0.1.3--h9ee0642_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### nucamino-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### nucamino-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### nucamino-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### nucamino-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### nucamino-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### nucamino-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### nucamino

```bash
$ singularity exec <container> /usr/local/bin/nucamino
$ podman run --it --rm --entrypoint /usr/local/bin/nucamino   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/nucamino   -v ${PWD} -w ${PWD} <container> -c " $@"
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