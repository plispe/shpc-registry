---
layout: container
name:  "quay.io/biocontainers/bioconductor-diffhic"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-diffhic/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-diffhic/container.yaml"
updated_at: "2023-01-13 03:08:21.356319"
latest: "1.30.0--r42hc247a5b_0"
container_url: "https://biocontainers.pro/tools/bioconductor-diffhic"

versions:
 - "1.26.0--r41hc247a5b_2"
 - "1.30.0--r42hc247a5b_0"
description: "shpc-registry automated BioContainers addition for bioconductor-diffhic"
config: {"url": "https://biocontainers.pro/tools/bioconductor-diffhic", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-diffhic", "latest": {"1.30.0--r42hc247a5b_0": "sha256:c294c1dc37c7cd90aef6f429cac80977d9d11e6dca0044a433dd590c0e141a5a"}, "tags": {"1.26.0--r41hc247a5b_2": "sha256:b4f7d6eae7af3542c5c939afd2e24f5be82aff005679e658b709b5fd3faface6", "1.30.0--r42hc247a5b_0": "sha256:c294c1dc37c7cd90aef6f429cac80977d9d11e6dca0044a433dd590c0e141a5a"}, "docker": "quay.io/biocontainers/bioconductor-diffhic"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-diffhic.
shpc-registry automated BioContainers addition for bioconductor-diffhic
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-diffhic
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-diffhic:1.30.0--r42hc247a5b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-diffhic/1.30.0--r42hc247a5b_0
$ module help quay.io/biocontainers/bioconductor-diffhic/1.30.0--r42hc247a5b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-diffhic-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-diffhic-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-diffhic-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-diffhic-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-diffhic-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-diffhic-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-diffhic

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