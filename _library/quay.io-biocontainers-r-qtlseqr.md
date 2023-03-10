---
layout: container
name:  "quay.io/biocontainers/r-qtlseqr"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/r-qtlseqr/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/r-qtlseqr/container.yaml"
updated_at: "2023-01-13 03:35:37.206902"
latest: "0.7.5.2--r42h9f5acd7_4"
container_url: "https://biocontainers.pro/tools/r-qtlseqr"

versions:
 - "0.7.5.2--r41h9f5acd7_3"
 - "0.7.5.2--r42h9f5acd7_4"
description: "shpc-registry automated BioContainers addition for r-qtlseqr"
config: {"url": "https://biocontainers.pro/tools/r-qtlseqr", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for r-qtlseqr", "latest": {"0.7.5.2--r42h9f5acd7_4": "sha256:1c2274ca910e9363c66343dda8406fa559bb493f06910fd502544b06b1b3e153"}, "tags": {"0.7.5.2--r41h9f5acd7_3": "sha256:bee93102d5df32746c52d318ff5123f28603e4a97adcb2104c0eb260d2ea2304", "0.7.5.2--r42h9f5acd7_4": "sha256:1c2274ca910e9363c66343dda8406fa559bb493f06910fd502544b06b1b3e153"}, "docker": "quay.io/biocontainers/r-qtlseqr"}
---

This module is a singularity container wrapper for quay.io/biocontainers/r-qtlseqr.
shpc-registry automated BioContainers addition for r-qtlseqr
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/r-qtlseqr
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/r-qtlseqr:0.7.5.2--r42h9f5acd7_4
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/r-qtlseqr/0.7.5.2--r42h9f5acd7_4
$ module help quay.io/biocontainers/r-qtlseqr/0.7.5.2--r42h9f5acd7_4
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### r-qtlseqr-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### r-qtlseqr-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### r-qtlseqr-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### r-qtlseqr-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### r-qtlseqr-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### r-qtlseqr-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### r-qtlseqr

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