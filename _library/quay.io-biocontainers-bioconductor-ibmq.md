---
layout: container
name:  "quay.io/biocontainers/bioconductor-ibmq"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-ibmq/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-ibmq/container.yaml"
updated_at: "2023-01-13 02:48:06.481021"
latest: "1.38.0--r42hda872b5_0"
container_url: "https://biocontainers.pro/tools/bioconductor-ibmq"

versions:
 - "1.34.0--r41hda872b5_3"
 - "1.38.0--r42hda872b5_0"
description: "shpc-registry automated BioContainers addition for bioconductor-ibmq"
config: {"url": "https://biocontainers.pro/tools/bioconductor-ibmq", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-ibmq", "latest": {"1.38.0--r42hda872b5_0": "sha256:2c68c56e235ed92f37131e31992b2f3127dc0763841db6a23a63c927b753458a"}, "tags": {"1.34.0--r41hda872b5_3": "sha256:66ace09fb0072250bb2a949c9a12a16cb9530d7cbb9327a0ff952f42bd626222", "1.38.0--r42hda872b5_0": "sha256:2c68c56e235ed92f37131e31992b2f3127dc0763841db6a23a63c927b753458a"}, "docker": "quay.io/biocontainers/bioconductor-ibmq"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-ibmq.
shpc-registry automated BioContainers addition for bioconductor-ibmq
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-ibmq
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-ibmq:1.38.0--r42hda872b5_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-ibmq/1.38.0--r42hda872b5_0
$ module help quay.io/biocontainers/bioconductor-ibmq/1.38.0--r42hda872b5_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-ibmq-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ibmq-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ibmq-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-ibmq-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-ibmq-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-ibmq-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-ibmq

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