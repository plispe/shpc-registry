---
layout: container
name:  "quay.io/biocontainers/bioconductor-hthgu133aprobe"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-hthgu133aprobe/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-hthgu133aprobe/container.yaml"
updated_at: "2023-01-13 03:23:31.483459"
latest: "2.18.0--r42hdfd78af_10"
container_url: "https://biocontainers.pro/tools/bioconductor-hthgu133aprobe"

versions:
 - "2.18.0--r41hdfd78af_9"
 - "2.18.0--r42hdfd78af_10"
description: "shpc-registry automated BioContainers addition for bioconductor-hthgu133aprobe"
config: {"url": "https://biocontainers.pro/tools/bioconductor-hthgu133aprobe", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-hthgu133aprobe", "latest": {"2.18.0--r42hdfd78af_10": "sha256:c6ab89d6ad612ebd75787425b2272f55dc4f4e55c2e5f7804812578cb63120ee"}, "tags": {"2.18.0--r41hdfd78af_9": "sha256:05df9afc6c5bf9dbf5a3499a9e8db523a2cb693f18b70a07dc8788098893fe69", "2.18.0--r42hdfd78af_10": "sha256:c6ab89d6ad612ebd75787425b2272f55dc4f4e55c2e5f7804812578cb63120ee"}, "docker": "quay.io/biocontainers/bioconductor-hthgu133aprobe"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-hthgu133aprobe.
shpc-registry automated BioContainers addition for bioconductor-hthgu133aprobe
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-hthgu133aprobe
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-hthgu133aprobe:2.18.0--r42hdfd78af_10
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-hthgu133aprobe/2.18.0--r42hdfd78af_10
$ module help quay.io/biocontainers/bioconductor-hthgu133aprobe/2.18.0--r42hdfd78af_10
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-hthgu133aprobe-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-hthgu133aprobe-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-hthgu133aprobe-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-hthgu133aprobe-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-hthgu133aprobe-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-hthgu133aprobe-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-hthgu133aprobe

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