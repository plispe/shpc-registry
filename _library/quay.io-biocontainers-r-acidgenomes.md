---
layout: container
name:  "quay.io/biocontainers/r-acidgenomes"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/r-acidgenomes/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/r-acidgenomes/container.yaml"
updated_at: "2023-01-13 02:50:24.133164"
latest: "0.4.4--r42hdfd78af_1"
container_url: "https://biocontainers.pro/tools/r-acidgenomes"

versions:
 - "0.3.0--r41hdfd78af_0"
 - "0.4.4--r42hdfd78af_1"
description: "shpc-registry automated BioContainers addition for r-acidgenomes"
config: {"url": "https://biocontainers.pro/tools/r-acidgenomes", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for r-acidgenomes", "latest": {"0.4.4--r42hdfd78af_1": "sha256:e84f7017a7be9372600a058cb8b85b3ac4817b104b962827aff805ecf0a50012"}, "tags": {"0.3.0--r41hdfd78af_0": "sha256:44d5d46dc2e579e3443a74aacca29eb700f3168cb05513863d84f7307eaea512", "0.4.4--r42hdfd78af_1": "sha256:e84f7017a7be9372600a058cb8b85b3ac4817b104b962827aff805ecf0a50012"}, "docker": "quay.io/biocontainers/r-acidgenomes"}
---

This module is a singularity container wrapper for quay.io/biocontainers/r-acidgenomes.
shpc-registry automated BioContainers addition for r-acidgenomes
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/r-acidgenomes
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/r-acidgenomes:0.4.4--r42hdfd78af_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/r-acidgenomes/0.4.4--r42hdfd78af_1
$ module help quay.io/biocontainers/r-acidgenomes/0.4.4--r42hdfd78af_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### r-acidgenomes-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### r-acidgenomes-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### r-acidgenomes-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### r-acidgenomes-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### r-acidgenomes-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### r-acidgenomes-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### r-acidgenomes

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