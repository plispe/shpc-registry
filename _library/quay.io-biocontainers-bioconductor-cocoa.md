---
layout: container
name:  "quay.io/biocontainers/bioconductor-cocoa"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-cocoa/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-cocoa/container.yaml"
updated_at: "2023-01-13 02:59:16.337701"
latest: "2.12.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-cocoa"

versions:
 - "2.8.0--r41hdfd78af_0"
 - "2.12.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-cocoa"
config: {"url": "https://biocontainers.pro/tools/bioconductor-cocoa", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-cocoa", "latest": {"2.12.0--r42hdfd78af_0": "sha256:d83d49d9ee2171af75c138bf5d9ac011eb67d39748ef7dafd791439081051204"}, "tags": {"2.8.0--r41hdfd78af_0": "sha256:53a384957f4f6f364a3fd94adf03e44039de5b7b322c1af9773198eca9a11a4a", "2.12.0--r42hdfd78af_0": "sha256:d83d49d9ee2171af75c138bf5d9ac011eb67d39748ef7dafd791439081051204"}, "docker": "quay.io/biocontainers/bioconductor-cocoa"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-cocoa.
shpc-registry automated BioContainers addition for bioconductor-cocoa
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-cocoa
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-cocoa:2.12.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-cocoa/2.12.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-cocoa/2.12.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-cocoa-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-cocoa-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-cocoa-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-cocoa-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-cocoa-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-cocoa-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-cocoa

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