---
layout: container
name:  "quay.io/biocontainers/bioconductor-affydata"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-affydata/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-affydata/container.yaml"
updated_at: "2022-11-20 00:31:03.695432"
latest: "1.46.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-affydata"
aliases:
 - ".bioconductor-affydata-post-link.sh"
 - ".bioconductor-affydata-pre-unlink.sh"
versions:
 - "1.42.0--r41hdfd78af_1"
 - "1.46.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-affydata"
config: {"url": "https://biocontainers.pro/tools/bioconductor-affydata", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-affydata", "latest": {"1.46.0--r42hdfd78af_0": "sha256:79f1df927469bb141b518735b9ee2fb44fb5dfe16b1ae4a67370b1dc5d2cd7bc"}, "tags": {"1.42.0--r41hdfd78af_1": "sha256:8d220eb8a24a7a943bb27e30c66b18f6c5e566b32cc4b32960272a4c86789b37", "1.46.0--r42hdfd78af_0": "sha256:79f1df927469bb141b518735b9ee2fb44fb5dfe16b1ae4a67370b1dc5d2cd7bc"}, "docker": "quay.io/biocontainers/bioconductor-affydata", "aliases": {".bioconductor-affydata-post-link.sh": "/usr/local/bin/.bioconductor-affydata-post-link.sh", ".bioconductor-affydata-pre-unlink.sh": "/usr/local/bin/.bioconductor-affydata-pre-unlink.sh"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-affydata.
shpc-registry automated BioContainers addition for bioconductor-affydata
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-affydata
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-affydata:1.46.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-affydata/1.46.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-affydata/1.46.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-affydata-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-affydata-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-affydata-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-affydata-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-affydata-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-affydata-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .bioconductor-affydata-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-affydata-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-affydata-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-affydata-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### .bioconductor-affydata-pre-unlink.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-affydata-pre-unlink.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-affydata-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-affydata-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
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