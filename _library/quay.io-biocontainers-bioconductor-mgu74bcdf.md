---
layout: container
name:  "quay.io/biocontainers/bioconductor-mgu74bcdf"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-mgu74bcdf/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-mgu74bcdf/container.yaml"
updated_at: "2023-01-13 03:15:10.850309"
latest: "2.18.0--r42hdfd78af_10"
container_url: "https://biocontainers.pro/tools/bioconductor-mgu74bcdf"

versions:
 - "2.18.0--r41hdfd78af_9"
 - "2.18.0--r42hdfd78af_10"
description: "shpc-registry automated BioContainers addition for bioconductor-mgu74bcdf"
config: {"url": "https://biocontainers.pro/tools/bioconductor-mgu74bcdf", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-mgu74bcdf", "latest": {"2.18.0--r42hdfd78af_10": "sha256:05dc2f4c03c355d9f635450d0cbb922a0eb8f62281b491595f0fe07b7c747f44"}, "tags": {"2.18.0--r41hdfd78af_9": "sha256:15ba9a4f4c29f0e406f14a5f8c716ab8d4f1f9c7553a46893e0ef058ad1e843d", "2.18.0--r42hdfd78af_10": "sha256:05dc2f4c03c355d9f635450d0cbb922a0eb8f62281b491595f0fe07b7c747f44"}, "docker": "quay.io/biocontainers/bioconductor-mgu74bcdf"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-mgu74bcdf.
shpc-registry automated BioContainers addition for bioconductor-mgu74bcdf
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-mgu74bcdf
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-mgu74bcdf:2.18.0--r42hdfd78af_10
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-mgu74bcdf/2.18.0--r42hdfd78af_10
$ module help quay.io/biocontainers/bioconductor-mgu74bcdf/2.18.0--r42hdfd78af_10
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-mgu74bcdf-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-mgu74bcdf-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-mgu74bcdf-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-mgu74bcdf-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-mgu74bcdf-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-mgu74bcdf-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-mgu74bcdf

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