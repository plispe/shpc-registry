---
layout: container
name:  "quay.io/biocontainers/bioconductor-hthgu133afrmavecs"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-hthgu133afrmavecs/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-hthgu133afrmavecs/container.yaml"
updated_at: "2023-01-13 03:04:27.395040"
latest: "1.3.0--r42hdfd78af_10"
container_url: "https://biocontainers.pro/tools/bioconductor-hthgu133afrmavecs"

versions:
 - "1.3.0--r41hdfd78af_9"
 - "1.3.0--r42hdfd78af_10"
description: "shpc-registry automated BioContainers addition for bioconductor-hthgu133afrmavecs"
config: {"url": "https://biocontainers.pro/tools/bioconductor-hthgu133afrmavecs", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-hthgu133afrmavecs", "latest": {"1.3.0--r42hdfd78af_10": "sha256:69a4a6efdac7001905fb4834e1950fc434a5f1495bfe077344e322b45675d616"}, "tags": {"1.3.0--r41hdfd78af_9": "sha256:7c026d892e494f6422b0330548761e02c15a2c6893fd3e47705c3ac816c7b20f", "1.3.0--r42hdfd78af_10": "sha256:69a4a6efdac7001905fb4834e1950fc434a5f1495bfe077344e322b45675d616"}, "docker": "quay.io/biocontainers/bioconductor-hthgu133afrmavecs"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-hthgu133afrmavecs.
shpc-registry automated BioContainers addition for bioconductor-hthgu133afrmavecs
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-hthgu133afrmavecs
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-hthgu133afrmavecs:1.3.0--r42hdfd78af_10
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-hthgu133afrmavecs/1.3.0--r42hdfd78af_10
$ module help quay.io/biocontainers/bioconductor-hthgu133afrmavecs/1.3.0--r42hdfd78af_10
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-hthgu133afrmavecs-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-hthgu133afrmavecs-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-hthgu133afrmavecs-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-hthgu133afrmavecs-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-hthgu133afrmavecs-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-hthgu133afrmavecs-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-hthgu133afrmavecs

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