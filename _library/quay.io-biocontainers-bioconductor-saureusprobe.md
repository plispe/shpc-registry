---
layout: container
name:  "quay.io/biocontainers/bioconductor-saureusprobe"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-saureusprobe/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-saureusprobe/container.yaml"
updated_at: "2022-11-20 00:04:48.038651"
latest: "2.18.0--r42hdfd78af_10"
container_url: "https://biocontainers.pro/tools/bioconductor-saureusprobe"
aliases:
 - ".bioconductor-saureusprobe-post-link.sh"
 - ".bioconductor-saureusprobe-pre-unlink.sh"
versions:
 - "2.18.0--r41hdfd78af_9"
 - "2.18.0--r42hdfd78af_10"
description: "shpc-registry automated BioContainers addition for bioconductor-saureusprobe"
config: {"url": "https://biocontainers.pro/tools/bioconductor-saureusprobe", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-saureusprobe", "latest": {"2.18.0--r42hdfd78af_10": "sha256:930e0e103cf4eeec8c74bc935daad60f9ed1e90450a1a0ba7a2cb25f51f54ebb"}, "tags": {"2.18.0--r41hdfd78af_9": "sha256:0117d5953709d8bb9b4dddc33d13223cf71a8d19c6983e3747bfafcac72fdb12", "2.18.0--r42hdfd78af_10": "sha256:930e0e103cf4eeec8c74bc935daad60f9ed1e90450a1a0ba7a2cb25f51f54ebb"}, "docker": "quay.io/biocontainers/bioconductor-saureusprobe", "aliases": {".bioconductor-saureusprobe-post-link.sh": "/usr/local/bin/.bioconductor-saureusprobe-post-link.sh", ".bioconductor-saureusprobe-pre-unlink.sh": "/usr/local/bin/.bioconductor-saureusprobe-pre-unlink.sh"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-saureusprobe.
shpc-registry automated BioContainers addition for bioconductor-saureusprobe
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-saureusprobe
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-saureusprobe:2.18.0--r42hdfd78af_10
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-saureusprobe/2.18.0--r42hdfd78af_10
$ module help quay.io/biocontainers/bioconductor-saureusprobe/2.18.0--r42hdfd78af_10
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-saureusprobe-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-saureusprobe-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-saureusprobe-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-saureusprobe-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-saureusprobe-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-saureusprobe-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .bioconductor-saureusprobe-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-saureusprobe-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-saureusprobe-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-saureusprobe-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### .bioconductor-saureusprobe-pre-unlink.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-saureusprobe-pre-unlink.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-saureusprobe-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-saureusprobe-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
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