---
layout: container
name:  "quay.io/biocontainers/bioconductor-epistack"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-epistack/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-epistack/container.yaml"
updated_at: "2023-01-13 03:08:26.841578"
latest: "1.4.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-epistack"

versions:
 - "1.0.0--r41hdfd78af_0"
 - "1.4.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-epistack"
config: {"url": "https://biocontainers.pro/tools/bioconductor-epistack", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-epistack", "latest": {"1.4.0--r42hdfd78af_0": "sha256:e40241854112b6238f66d7c99386f27660922057f10b101503ff050407193023"}, "tags": {"1.0.0--r41hdfd78af_0": "sha256:b64a53fd2a85db0d6077e27c716921c5728ea473b13b2d3f0761db49a26ae2db", "1.4.0--r42hdfd78af_0": "sha256:e40241854112b6238f66d7c99386f27660922057f10b101503ff050407193023"}, "docker": "quay.io/biocontainers/bioconductor-epistack"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-epistack.
shpc-registry automated BioContainers addition for bioconductor-epistack
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-epistack
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-epistack:1.4.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-epistack/1.4.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-epistack/1.4.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-epistack-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-epistack-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-epistack-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-epistack-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-epistack-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-epistack-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-epistack

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