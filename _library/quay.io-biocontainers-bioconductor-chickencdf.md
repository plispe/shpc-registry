---
layout: container
name:  "quay.io/biocontainers/bioconductor-chickencdf"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-chickencdf/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-chickencdf/container.yaml"
updated_at: "2023-01-13 03:18:46.069434"
latest: "2.18.0--r42hdfd78af_11"
container_url: "https://biocontainers.pro/tools/bioconductor-chickencdf"

versions:
 - "2.18.0--r41hdfd78af_9"
 - "2.18.0--r42hdfd78af_11"
description: "shpc-registry automated BioContainers addition for bioconductor-chickencdf"
config: {"url": "https://biocontainers.pro/tools/bioconductor-chickencdf", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-chickencdf", "latest": {"2.18.0--r42hdfd78af_11": "sha256:ff01694c96286a29ce00ffa7a3575aaac2eaf4d9059603fec7c32d380e8fb5bb"}, "tags": {"2.18.0--r41hdfd78af_9": "sha256:e4d7fedb05377b54e8f607aa6531bfcca03f33f55c02643b227394794564c904", "2.18.0--r42hdfd78af_11": "sha256:ff01694c96286a29ce00ffa7a3575aaac2eaf4d9059603fec7c32d380e8fb5bb"}, "docker": "quay.io/biocontainers/bioconductor-chickencdf"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-chickencdf.
shpc-registry automated BioContainers addition for bioconductor-chickencdf
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-chickencdf
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-chickencdf:2.18.0--r42hdfd78af_11
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-chickencdf/2.18.0--r42hdfd78af_11
$ module help quay.io/biocontainers/bioconductor-chickencdf/2.18.0--r42hdfd78af_11
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-chickencdf-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-chickencdf-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-chickencdf-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-chickencdf-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-chickencdf-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-chickencdf-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-chickencdf

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