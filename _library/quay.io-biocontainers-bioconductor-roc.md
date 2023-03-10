---
layout: container
name:  "quay.io/biocontainers/bioconductor-roc"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-roc/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-roc/container.yaml"
updated_at: "2023-01-13 03:01:10.311355"
latest: "1.74.0--r42hc247a5b_0"
container_url: "https://biocontainers.pro/tools/bioconductor-roc"

versions:
 - "1.70.0--r41hc247a5b_2"
 - "1.74.0--r42hc247a5b_0"
description: "shpc-registry automated BioContainers addition for bioconductor-roc"
config: {"url": "https://biocontainers.pro/tools/bioconductor-roc", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-roc", "latest": {"1.74.0--r42hc247a5b_0": "sha256:2e23b080bbca6cc4cc00c6bafafc7459f3ac002363552b0d3c049356081fe067"}, "tags": {"1.70.0--r41hc247a5b_2": "sha256:8c0f071fb9135c2db7b5f626b18e8df17ab2c5de7c26ba9f5de9a6bd24abe850", "1.74.0--r42hc247a5b_0": "sha256:2e23b080bbca6cc4cc00c6bafafc7459f3ac002363552b0d3c049356081fe067"}, "docker": "quay.io/biocontainers/bioconductor-roc"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-roc.
shpc-registry automated BioContainers addition for bioconductor-roc
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-roc
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-roc:1.74.0--r42hc247a5b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-roc/1.74.0--r42hc247a5b_0
$ module help quay.io/biocontainers/bioconductor-roc/1.74.0--r42hc247a5b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-roc-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-roc-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-roc-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-roc-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-roc-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-roc-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-roc

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