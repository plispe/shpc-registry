---
layout: container
name:  "quay.io/biocontainers/bioconductor-medipsdata"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-medipsdata/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-medipsdata/container.yaml"
updated_at: "2023-01-13 03:37:54.191937"
latest: "1.33.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-medipsdata"

versions:
 - "1.30.0--r41hdfd78af_1"
 - "1.33.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-medipsdata"
config: {"url": "https://biocontainers.pro/tools/bioconductor-medipsdata", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-medipsdata", "latest": {"1.33.0--r42hdfd78af_0": "sha256:9c0d69cdc21ba467851c6b1a1455d77125790772814206a479dc9712f8d15e9a"}, "tags": {"1.30.0--r41hdfd78af_1": "sha256:8676a95e25196bf38951bcf8a0378d2204a0251d1fd40620e0324d654cf9ab49", "1.33.0--r42hdfd78af_0": "sha256:9c0d69cdc21ba467851c6b1a1455d77125790772814206a479dc9712f8d15e9a"}, "docker": "quay.io/biocontainers/bioconductor-medipsdata"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-medipsdata.
shpc-registry automated BioContainers addition for bioconductor-medipsdata
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-medipsdata
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-medipsdata:1.33.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-medipsdata/1.33.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-medipsdata/1.33.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-medipsdata-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-medipsdata-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-medipsdata-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-medipsdata-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-medipsdata-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-medipsdata-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-medipsdata

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