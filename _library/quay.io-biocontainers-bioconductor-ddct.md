---
layout: container
name:  "quay.io/biocontainers/bioconductor-ddct"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-ddct/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-ddct/container.yaml"
updated_at: "2023-01-13 03:31:38.698169"
latest: "1.54.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-ddct"

versions:
 - "1.50.0--r41hdfd78af_0"
 - "1.54.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-ddct"
config: {"url": "https://biocontainers.pro/tools/bioconductor-ddct", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-ddct", "latest": {"1.54.0--r42hdfd78af_0": "sha256:fe333a1947fad8856ef5bf95c7253452a6b6efb110789cf8417f86020d6cdc6c"}, "tags": {"1.50.0--r41hdfd78af_0": "sha256:783b21596d8be4d1aad55aacda5e7db86188939ca2f859c67c4f37abf02f3837", "1.54.0--r42hdfd78af_0": "sha256:fe333a1947fad8856ef5bf95c7253452a6b6efb110789cf8417f86020d6cdc6c"}, "docker": "quay.io/biocontainers/bioconductor-ddct"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-ddct.
shpc-registry automated BioContainers addition for bioconductor-ddct
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-ddct
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-ddct:1.54.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-ddct/1.54.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-ddct/1.54.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-ddct-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ddct-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ddct-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-ddct-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-ddct-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-ddct-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-ddct

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