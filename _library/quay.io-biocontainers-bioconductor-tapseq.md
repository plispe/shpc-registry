---
layout: container
name:  "quay.io/biocontainers/bioconductor-tapseq"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-tapseq/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-tapseq/container.yaml"
updated_at: "2023-01-13 03:39:38.493008"
latest: "1.10.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-tapseq"

versions:
 - "1.6.0--r41hdfd78af_0"
 - "1.10.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-tapseq"
config: {"url": "https://biocontainers.pro/tools/bioconductor-tapseq", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-tapseq", "latest": {"1.10.0--r42hdfd78af_0": "sha256:b5b3fd18d6b8272fdb980f3e69f2ebbf23c855fd22f231b5eb05162b9a6a47f5"}, "tags": {"1.6.0--r41hdfd78af_0": "sha256:5f374ab1b5ac15bd5762d8009f8b728bbeb07c8c9494513110152f722ff2c8c9", "1.10.0--r42hdfd78af_0": "sha256:b5b3fd18d6b8272fdb980f3e69f2ebbf23c855fd22f231b5eb05162b9a6a47f5"}, "docker": "quay.io/biocontainers/bioconductor-tapseq"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-tapseq.
shpc-registry automated BioContainers addition for bioconductor-tapseq
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-tapseq
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-tapseq:1.10.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-tapseq/1.10.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-tapseq/1.10.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-tapseq-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-tapseq-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-tapseq-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-tapseq-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-tapseq-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-tapseq-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-tapseq

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