---
layout: container
name:  "quay.io/biocontainers/bioconductor-acme"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-acme/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-acme/container.yaml"
updated_at: "2023-01-13 02:51:43.682974"
latest: "2.54.0--r42hc0cfd56_0"
container_url: "https://biocontainers.pro/tools/bioconductor-acme"

versions:
 - "2.50.0--r41hc0cfd56_2"
 - "2.54.0--r42hc0cfd56_0"
description: "shpc-registry automated BioContainers addition for bioconductor-acme"
config: {"url": "https://biocontainers.pro/tools/bioconductor-acme", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-acme", "latest": {"2.54.0--r42hc0cfd56_0": "sha256:add961f4d145fa3a0f21f368c686c5c4b775cb4fed16a549a83d78fb6424fb7b"}, "tags": {"2.50.0--r41hc0cfd56_2": "sha256:4fd50d3647cc843691a64ea2b22d9f2436907dc3bf5473fad2be8664cd8df3b1", "2.54.0--r42hc0cfd56_0": "sha256:add961f4d145fa3a0f21f368c686c5c4b775cb4fed16a549a83d78fb6424fb7b"}, "docker": "quay.io/biocontainers/bioconductor-acme"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-acme.
shpc-registry automated BioContainers addition for bioconductor-acme
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-acme
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-acme:2.54.0--r42hc0cfd56_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-acme/2.54.0--r42hc0cfd56_0
$ module help quay.io/biocontainers/bioconductor-acme/2.54.0--r42hc0cfd56_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-acme-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-acme-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-acme-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-acme-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-acme-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-acme-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-acme

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