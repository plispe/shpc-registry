---
layout: container
name:  "quay.io/biocontainers/bioconductor-hca"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-hca/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-hca/container.yaml"
updated_at: "2023-01-13 03:00:17.907484"
latest: "1.6.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-hca"

versions:
 - "1.2.0--r41hdfd78af_0"
 - "1.6.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-hca"
config: {"url": "https://biocontainers.pro/tools/bioconductor-hca", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-hca", "latest": {"1.6.0--r42hdfd78af_0": "sha256:0db59e82ec782967b47c4da4629d46922aacdffff2ebbd360feeba1230d7b3b5"}, "tags": {"1.2.0--r41hdfd78af_0": "sha256:ab20a261fedc655b8ca2ff9d60e04f40b6b4d200aa8046344f5100c597c67df1", "1.6.0--r42hdfd78af_0": "sha256:0db59e82ec782967b47c4da4629d46922aacdffff2ebbd360feeba1230d7b3b5"}, "docker": "quay.io/biocontainers/bioconductor-hca"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-hca.
shpc-registry automated BioContainers addition for bioconductor-hca
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-hca
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-hca:1.6.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-hca/1.6.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-hca/1.6.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-hca-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-hca-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-hca-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-hca-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-hca-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-hca-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-hca

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