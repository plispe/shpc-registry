---
layout: container
name:  "quay.io/biocontainers/bioconductor-rtu34cdf"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-rtu34cdf/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-rtu34cdf/container.yaml"
updated_at: "2023-01-13 03:21:13.906365"
latest: "2.18.0--r42hdfd78af_10"
container_url: "https://biocontainers.pro/tools/bioconductor-rtu34cdf"

versions:
 - "2.18.0--r41hdfd78af_9"
 - "2.18.0--r42hdfd78af_10"
description: "shpc-registry automated BioContainers addition for bioconductor-rtu34cdf"
config: {"url": "https://biocontainers.pro/tools/bioconductor-rtu34cdf", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-rtu34cdf", "latest": {"2.18.0--r42hdfd78af_10": "sha256:4ee6656a7419978e1f28f12e97909830c861acb88203e1cfbed978ec39341f6b"}, "tags": {"2.18.0--r41hdfd78af_9": "sha256:aa8524a5d81b84f9e609cd329e6cfc0b22cd5958f1612bea4cd973f7d351e0be", "2.18.0--r42hdfd78af_10": "sha256:4ee6656a7419978e1f28f12e97909830c861acb88203e1cfbed978ec39341f6b"}, "docker": "quay.io/biocontainers/bioconductor-rtu34cdf"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-rtu34cdf.
shpc-registry automated BioContainers addition for bioconductor-rtu34cdf
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-rtu34cdf
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-rtu34cdf:2.18.0--r42hdfd78af_10
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-rtu34cdf/2.18.0--r42hdfd78af_10
$ module help quay.io/biocontainers/bioconductor-rtu34cdf/2.18.0--r42hdfd78af_10
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-rtu34cdf-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-rtu34cdf-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-rtu34cdf-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-rtu34cdf-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-rtu34cdf-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-rtu34cdf-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-rtu34cdf

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