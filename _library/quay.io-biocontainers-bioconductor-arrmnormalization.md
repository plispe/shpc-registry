---
layout: container
name:  "quay.io/biocontainers/bioconductor-arrmnormalization"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-arrmnormalization/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-arrmnormalization/container.yaml"
updated_at: "2023-01-13 03:24:54.779369"
latest: "1.38.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-arrmnormalization"

versions:
 - "1.34.0--r41hdfd78af_0"
 - "1.38.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-arrmnormalization"
config: {"url": "https://biocontainers.pro/tools/bioconductor-arrmnormalization", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-arrmnormalization", "latest": {"1.38.0--r42hdfd78af_0": "sha256:edb5ea52ece9ed192fdadedc98777d60e6e67e3195dafc052f759fc32fc64be5"}, "tags": {"1.34.0--r41hdfd78af_0": "sha256:04890f26fe6ba479d4490a8a0807d8e210fb3fce56d49088db830b0714825f8e", "1.38.0--r42hdfd78af_0": "sha256:edb5ea52ece9ed192fdadedc98777d60e6e67e3195dafc052f759fc32fc64be5"}, "docker": "quay.io/biocontainers/bioconductor-arrmnormalization"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-arrmnormalization.
shpc-registry automated BioContainers addition for bioconductor-arrmnormalization
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-arrmnormalization
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-arrmnormalization:1.38.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-arrmnormalization/1.38.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-arrmnormalization/1.38.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-arrmnormalization-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-arrmnormalization-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-arrmnormalization-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-arrmnormalization-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-arrmnormalization-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-arrmnormalization-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-arrmnormalization

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