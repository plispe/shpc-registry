---
layout: container
name:  "quay.io/biocontainers/bioconductor-hicdatalymphoblast"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-hicdatalymphoblast/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-hicdatalymphoblast/container.yaml"
updated_at: "2022-11-20 01:03:51.298756"
latest: "1.33.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-hicdatalymphoblast"
aliases:
 - ".bioconductor-hicdatalymphoblast-post-link.sh"
 - ".bioconductor-hicdatalymphoblast-pre-unlink.sh"
versions:
 - "1.30.0--r41hdfd78af_1"
 - "1.33.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-hicdatalymphoblast"
config: {"url": "https://biocontainers.pro/tools/bioconductor-hicdatalymphoblast", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-hicdatalymphoblast", "latest": {"1.33.0--r42hdfd78af_0": "sha256:64db90d26c20c8a9e68296c37f9f1793be4fde0b8b9ed7503a06e88580f76e22"}, "tags": {"1.30.0--r41hdfd78af_1": "sha256:45129e6c3847707dae936594ccaa2cf3fa4df57aa3586ab7efc07ef063e14df2", "1.33.0--r42hdfd78af_0": "sha256:64db90d26c20c8a9e68296c37f9f1793be4fde0b8b9ed7503a06e88580f76e22"}, "docker": "quay.io/biocontainers/bioconductor-hicdatalymphoblast", "aliases": {".bioconductor-hicdatalymphoblast-post-link.sh": "/usr/local/bin/.bioconductor-hicdatalymphoblast-post-link.sh", ".bioconductor-hicdatalymphoblast-pre-unlink.sh": "/usr/local/bin/.bioconductor-hicdatalymphoblast-pre-unlink.sh"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-hicdatalymphoblast.
shpc-registry automated BioContainers addition for bioconductor-hicdatalymphoblast
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-hicdatalymphoblast
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-hicdatalymphoblast:1.33.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-hicdatalymphoblast/1.33.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-hicdatalymphoblast/1.33.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-hicdatalymphoblast-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-hicdatalymphoblast-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-hicdatalymphoblast-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-hicdatalymphoblast-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-hicdatalymphoblast-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-hicdatalymphoblast-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .bioconductor-hicdatalymphoblast-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-hicdatalymphoblast-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-hicdatalymphoblast-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-hicdatalymphoblast-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### .bioconductor-hicdatalymphoblast-pre-unlink.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-hicdatalymphoblast-pre-unlink.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-hicdatalymphoblast-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-hicdatalymphoblast-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
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