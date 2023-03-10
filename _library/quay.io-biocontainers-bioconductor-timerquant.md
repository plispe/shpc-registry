---
layout: container
name:  "quay.io/biocontainers/bioconductor-timerquant"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-timerquant/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-timerquant/container.yaml"
updated_at: "2023-01-13 03:44:49.715309"
latest: "1.27.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-timerquant"

versions:
 - "1.24.0--r41hdfd78af_1"
 - "1.27.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-timerquant"
config: {"url": "https://biocontainers.pro/tools/bioconductor-timerquant", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-timerquant", "latest": {"1.27.0--r42hdfd78af_0": "sha256:247bf7fc845c7fff3f826c6a6ac5af3473d12cc709680e077e83638ef1a41c94"}, "tags": {"1.24.0--r41hdfd78af_1": "sha256:e48b927fe50ee8c5d92a043adb506e340888e520766cc2bf7456445e025a8520", "1.27.0--r42hdfd78af_0": "sha256:247bf7fc845c7fff3f826c6a6ac5af3473d12cc709680e077e83638ef1a41c94"}, "docker": "quay.io/biocontainers/bioconductor-timerquant"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-timerquant.
shpc-registry automated BioContainers addition for bioconductor-timerquant
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-timerquant
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-timerquant:1.27.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-timerquant/1.27.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-timerquant/1.27.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-timerquant-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-timerquant-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-timerquant-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-timerquant-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-timerquant-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-timerquant-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-timerquant

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