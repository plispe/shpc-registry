---
layout: container
name:  "quay.io/biocontainers/bioconductor-hiergwas"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-hiergwas/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-hiergwas/container.yaml"
updated_at: "2023-01-13 02:57:49.074533"
latest: "1.28.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-hiergwas"

versions:
 - "1.24.0--r41hdfd78af_0"
 - "1.28.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-hiergwas"
config: {"url": "https://biocontainers.pro/tools/bioconductor-hiergwas", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-hiergwas", "latest": {"1.28.0--r42hdfd78af_0": "sha256:caa10be6053a89cc11eed6dffecde474b5049e910e88ca60f4cab613377f1686"}, "tags": {"1.24.0--r41hdfd78af_0": "sha256:3cfde919da0148507c6ade5febdf0ca0cd23a18952a65f870bbc2d3035c5d7ef", "1.28.0--r42hdfd78af_0": "sha256:caa10be6053a89cc11eed6dffecde474b5049e910e88ca60f4cab613377f1686"}, "docker": "quay.io/biocontainers/bioconductor-hiergwas"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-hiergwas.
shpc-registry automated BioContainers addition for bioconductor-hiergwas
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-hiergwas
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-hiergwas:1.28.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-hiergwas/1.28.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-hiergwas/1.28.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-hiergwas-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-hiergwas-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-hiergwas-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-hiergwas-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-hiergwas-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-hiergwas-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-hiergwas

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