---
layout: container
name:  "quay.io/biocontainers/bioconductor-rtu34probe"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-rtu34probe/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-rtu34probe/container.yaml"
updated_at: "2023-01-13 03:39:21.267084"
latest: "2.18.0--r42hdfd78af_10"
container_url: "https://biocontainers.pro/tools/bioconductor-rtu34probe"

versions:
 - "2.18.0--r41hdfd78af_9"
 - "2.18.0--r42hdfd78af_10"
description: "shpc-registry automated BioContainers addition for bioconductor-rtu34probe"
config: {"url": "https://biocontainers.pro/tools/bioconductor-rtu34probe", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-rtu34probe", "latest": {"2.18.0--r42hdfd78af_10": "sha256:d02afc0131b477c19f2dab179e1141f7898e5989ebcae05112a3c2f21d15054b"}, "tags": {"2.18.0--r41hdfd78af_9": "sha256:abc93a8bad2adf31acb16bd8be3d8474843b703767c306b450bff88feb52cabe", "2.18.0--r42hdfd78af_10": "sha256:d02afc0131b477c19f2dab179e1141f7898e5989ebcae05112a3c2f21d15054b"}, "docker": "quay.io/biocontainers/bioconductor-rtu34probe"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-rtu34probe.
shpc-registry automated BioContainers addition for bioconductor-rtu34probe
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-rtu34probe
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-rtu34probe:2.18.0--r42hdfd78af_10
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-rtu34probe/2.18.0--r42hdfd78af_10
$ module help quay.io/biocontainers/bioconductor-rtu34probe/2.18.0--r42hdfd78af_10
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-rtu34probe-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-rtu34probe-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-rtu34probe-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-rtu34probe-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-rtu34probe-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-rtu34probe-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-rtu34probe

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