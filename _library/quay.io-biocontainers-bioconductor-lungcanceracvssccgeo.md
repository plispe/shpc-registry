---
layout: container
name:  "quay.io/biocontainers/bioconductor-lungcanceracvssccgeo"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-lungcanceracvssccgeo/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-lungcanceracvssccgeo/container.yaml"
updated_at: "2023-01-13 03:29:50.980981"
latest: "1.34.0--r42hdfd78af_1"
container_url: "https://biocontainers.pro/tools/bioconductor-lungcanceracvssccgeo"

versions:
 - "1.30.0--r41hdfd78af_1"
 - "1.34.0--r42hdfd78af_1"
 - "1.33.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-lungcanceracvssccgeo"
config: {"url": "https://biocontainers.pro/tools/bioconductor-lungcanceracvssccgeo", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-lungcanceracvssccgeo", "latest": {"1.34.0--r42hdfd78af_1": "sha256:bcb752a41e6f3539d6ddfb87dd96f72b55391d74ca595c00a614c6a0524e27b6"}, "tags": {"1.30.0--r41hdfd78af_1": "sha256:a85961ba83366da8f9889e4b3817fa615b556d7b8dd4b1fdf9888594c00d2d2c", "1.34.0--r42hdfd78af_1": "sha256:bcb752a41e6f3539d6ddfb87dd96f72b55391d74ca595c00a614c6a0524e27b6", "1.33.0--r42hdfd78af_0": "sha256:454c20900dc158b8d96ed1bd07575df0bbccff6d76c4adf41a69eb425988a825"}, "docker": "quay.io/biocontainers/bioconductor-lungcanceracvssccgeo"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-lungcanceracvssccgeo.
shpc-registry automated BioContainers addition for bioconductor-lungcanceracvssccgeo
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-lungcanceracvssccgeo
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-lungcanceracvssccgeo:1.34.0--r42hdfd78af_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-lungcanceracvssccgeo/1.34.0--r42hdfd78af_1
$ module help quay.io/biocontainers/bioconductor-lungcanceracvssccgeo/1.34.0--r42hdfd78af_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-lungcanceracvssccgeo-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-lungcanceracvssccgeo-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-lungcanceracvssccgeo-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-lungcanceracvssccgeo-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-lungcanceracvssccgeo-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-lungcanceracvssccgeo-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-lungcanceracvssccgeo

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