---
layout: container
name:  "quay.io/biocontainers/bioconductor-metaseq"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-metaseq/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-metaseq/container.yaml"
updated_at: "2023-01-13 02:55:57.431457"
latest: "1.38.0--r42hc247a5b_0"
container_url: "https://biocontainers.pro/tools/bioconductor-metaseq"

versions:
 - "1.34.0--r41hc247a5b_2"
 - "1.38.0--r42hc247a5b_0"
description: "shpc-registry automated BioContainers addition for bioconductor-metaseq"
config: {"url": "https://biocontainers.pro/tools/bioconductor-metaseq", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-metaseq", "latest": {"1.38.0--r42hc247a5b_0": "sha256:b98d8b751d98885fee17468dc843ce0f201775ff20ec02242c008c74d040fe63"}, "tags": {"1.34.0--r41hc247a5b_2": "sha256:0d2003b258093e7989c6c350a28a1b500c3129ac1e94d27b1dae5e97f8807af0", "1.38.0--r42hc247a5b_0": "sha256:b98d8b751d98885fee17468dc843ce0f201775ff20ec02242c008c74d040fe63"}, "docker": "quay.io/biocontainers/bioconductor-metaseq"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-metaseq.
shpc-registry automated BioContainers addition for bioconductor-metaseq
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-metaseq
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-metaseq:1.38.0--r42hc247a5b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-metaseq/1.38.0--r42hc247a5b_0
$ module help quay.io/biocontainers/bioconductor-metaseq/1.38.0--r42hc247a5b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-metaseq-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-metaseq-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-metaseq-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-metaseq-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-metaseq-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-metaseq-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-metaseq

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