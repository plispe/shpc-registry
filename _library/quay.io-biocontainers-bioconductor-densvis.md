---
layout: container
name:  "quay.io/biocontainers/bioconductor-densvis"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-densvis/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-densvis/container.yaml"
updated_at: "2023-01-13 03:09:08.939238"
latest: "1.8.0--r42hc247a5b_0"
container_url: "https://biocontainers.pro/tools/bioconductor-densvis"

versions:
 - "1.4.0--r41hc247a5b_2"
 - "1.8.0--r42hc247a5b_0"
description: "shpc-registry automated BioContainers addition for bioconductor-densvis"
config: {"url": "https://biocontainers.pro/tools/bioconductor-densvis", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-densvis", "latest": {"1.8.0--r42hc247a5b_0": "sha256:ab9ef67509ad1c79e50c0db6eb69509eb01504304a3f52799de86cb51e790476"}, "tags": {"1.4.0--r41hc247a5b_2": "sha256:594159b6af145a90070412d0f1ebb3044f7ab1efdb982430ecdbb0f829764088", "1.8.0--r42hc247a5b_0": "sha256:ab9ef67509ad1c79e50c0db6eb69509eb01504304a3f52799de86cb51e790476"}, "docker": "quay.io/biocontainers/bioconductor-densvis"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-densvis.
shpc-registry automated BioContainers addition for bioconductor-densvis
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-densvis
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-densvis:1.8.0--r42hc247a5b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-densvis/1.8.0--r42hc247a5b_0
$ module help quay.io/biocontainers/bioconductor-densvis/1.8.0--r42hc247a5b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-densvis-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-densvis-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-densvis-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-densvis-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-densvis-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-densvis-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-densvis

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