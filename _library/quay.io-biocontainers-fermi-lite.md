---
layout: container
name:  "quay.io/biocontainers/fermi-lite"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/fermi-lite/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/fermi-lite/container.yaml"
updated_at: "2023-01-13 02:52:45.967789"
latest: "0.1--h7132678_5"
container_url: "https://biocontainers.pro/tools/fermi-lite"
aliases:
 - "fml-asm"
versions:
 - "0.1--h7132678_5"
description: "shpc-registry automated BioContainers addition for fermi-lite"
config: {"url": "https://biocontainers.pro/tools/fermi-lite", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for fermi-lite", "latest": {"0.1--h7132678_5": "sha256:cd0193712125eac5ddf1632862f4882efde3a116788c9a3a317a847f6d6cb518"}, "tags": {"0.1--h7132678_5": "sha256:cd0193712125eac5ddf1632862f4882efde3a116788c9a3a317a847f6d6cb518"}, "docker": "quay.io/biocontainers/fermi-lite", "aliases": {"fml-asm": "/usr/local/bin/fml-asm"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/fermi-lite.
shpc-registry automated BioContainers addition for fermi-lite
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/fermi-lite
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/fermi-lite:0.1--h7132678_5
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/fermi-lite/0.1--h7132678_5
$ module help quay.io/biocontainers/fermi-lite/0.1--h7132678_5
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### fermi-lite-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### fermi-lite-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### fermi-lite-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### fermi-lite-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### fermi-lite-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### fermi-lite-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### fml-asm

```bash
$ singularity exec <container> /usr/local/bin/fml-asm
$ podman run --it --rm --entrypoint /usr/local/bin/fml-asm   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/fml-asm   -v ${PWD} -w ${PWD} <container> -c " $@"
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