---
layout: container
name:  "quay.io/biocontainers/bioconductor-breastcancerunt"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-breastcancerunt/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-breastcancerunt/container.yaml"
updated_at: "2022-11-19 23:51:51.356048"
latest: "1.36.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-breastcancerunt"
aliases:
 - ".bioconductor-breastcancerunt-post-link.sh"
 - ".bioconductor-breastcancerunt-pre-unlink.sh"
versions:
 - "1.32.0--r41hdfd78af_1"
 - "1.36.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-breastcancerunt"
config: {"url": "https://biocontainers.pro/tools/bioconductor-breastcancerunt", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-breastcancerunt", "latest": {"1.36.0--r42hdfd78af_0": "sha256:4f2125b7f042834efd42e5fc3d69ec564f83ab66862fd54f4e71913de140fc77"}, "tags": {"1.32.0--r41hdfd78af_1": "sha256:5b24e1d47cb32ec8f64308ae53a97253c3cec150286f601b18983d182bf0233a", "1.36.0--r42hdfd78af_0": "sha256:4f2125b7f042834efd42e5fc3d69ec564f83ab66862fd54f4e71913de140fc77"}, "docker": "quay.io/biocontainers/bioconductor-breastcancerunt", "aliases": {".bioconductor-breastcancerunt-post-link.sh": "/usr/local/bin/.bioconductor-breastcancerunt-post-link.sh", ".bioconductor-breastcancerunt-pre-unlink.sh": "/usr/local/bin/.bioconductor-breastcancerunt-pre-unlink.sh"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-breastcancerunt.
shpc-registry automated BioContainers addition for bioconductor-breastcancerunt
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-breastcancerunt
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-breastcancerunt:1.36.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-breastcancerunt/1.36.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-breastcancerunt/1.36.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-breastcancerunt-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-breastcancerunt-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-breastcancerunt-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-breastcancerunt-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-breastcancerunt-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-breastcancerunt-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .bioconductor-breastcancerunt-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-breastcancerunt-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-breastcancerunt-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-breastcancerunt-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### .bioconductor-breastcancerunt-pre-unlink.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-breastcancerunt-pre-unlink.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-breastcancerunt-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-breastcancerunt-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
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