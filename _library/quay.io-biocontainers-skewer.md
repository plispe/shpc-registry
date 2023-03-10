---
layout: container
name:  "quay.io/biocontainers/skewer"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/skewer/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/skewer/container.yaml"
updated_at: "2023-01-13 02:56:12.916739"
latest: "0.2.2--hc9558a2_3"
container_url: "https://biocontainers.pro/tools/skewer"
aliases:
 - "skewer"
versions:
 - "0.2.2--hc9558a2_3"
description: "shpc-registry automated BioContainers addition for skewer"
config: {"url": "https://biocontainers.pro/tools/skewer", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for skewer", "latest": {"0.2.2--hc9558a2_3": "sha256:7aa88909b49729c20a3711c59751cc119582d35d67c9b0efde3f727e98d85cc6"}, "tags": {"0.2.2--hc9558a2_3": "sha256:7aa88909b49729c20a3711c59751cc119582d35d67c9b0efde3f727e98d85cc6"}, "docker": "quay.io/biocontainers/skewer", "aliases": {"skewer": "/usr/local/bin/skewer"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/skewer.
shpc-registry automated BioContainers addition for skewer
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/skewer
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/skewer:0.2.2--hc9558a2_3
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/skewer/0.2.2--hc9558a2_3
$ module help quay.io/biocontainers/skewer/0.2.2--hc9558a2_3
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### skewer-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### skewer-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### skewer-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### skewer-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### skewer-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### skewer-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### skewer

```bash
$ singularity exec <container> /usr/local/bin/skewer
$ podman run --it --rm --entrypoint /usr/local/bin/skewer   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/skewer   -v ${PWD} -w ${PWD} <container> -c " $@"
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