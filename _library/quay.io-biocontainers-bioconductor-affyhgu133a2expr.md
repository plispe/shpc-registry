---
layout: container
name:  "quay.io/biocontainers/bioconductor-affyhgu133a2expr"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-affyhgu133a2expr/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-affyhgu133a2expr/container.yaml"
updated_at: "2023-01-13 03:14:57.332950"
latest: "1.33.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-affyhgu133a2expr"

versions:
 - "1.30.0--r41hdfd78af_1"
 - "1.33.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-affyhgu133a2expr"
config: {"url": "https://biocontainers.pro/tools/bioconductor-affyhgu133a2expr", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-affyhgu133a2expr", "latest": {"1.33.0--r42hdfd78af_0": "sha256:8a3f16dd05dcb5acd0071252ca257d355d10ec79fae15caec8ce0a390dfdef51"}, "tags": {"1.30.0--r41hdfd78af_1": "sha256:c3e4de96cd9ae1717b9d0ccfced2e752d372bb1f5f85d0a70c7e76af4b9a3102", "1.33.0--r42hdfd78af_0": "sha256:8a3f16dd05dcb5acd0071252ca257d355d10ec79fae15caec8ce0a390dfdef51"}, "docker": "quay.io/biocontainers/bioconductor-affyhgu133a2expr"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-affyhgu133a2expr.
shpc-registry automated BioContainers addition for bioconductor-affyhgu133a2expr
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-affyhgu133a2expr
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-affyhgu133a2expr:1.33.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-affyhgu133a2expr/1.33.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-affyhgu133a2expr/1.33.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-affyhgu133a2expr-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-affyhgu133a2expr-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-affyhgu133a2expr-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-affyhgu133a2expr-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-affyhgu133a2expr-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-affyhgu133a2expr-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-affyhgu133a2expr

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