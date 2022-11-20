---
layout: container
name:  "quay.io/biocontainers/bioconductor-clariomshumantranscriptcluster.db"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-clariomshumantranscriptcluster.db/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-clariomshumantranscriptcluster.db/container.yaml"
updated_at: "2022-11-20 00:42:12.168113"
latest: "8.8.0--r42hdfd78af_2"
container_url: "https://biocontainers.pro/tools/bioconductor-clariomshumantranscriptcluster.db"
aliases:
 - ".bioconductor-clariomshumantranscriptcluster.db-post-link.sh"
 - ".bioconductor-clariomshumantranscriptcluster.db-pre-unlink.sh"
versions:
 - "8.8.0--r41hdfd78af_1"
 - "8.8.0--r42hdfd78af_2"
description: "shpc-registry automated BioContainers addition for bioconductor-clariomshumantranscriptcluster.db"
config: {"url": "https://biocontainers.pro/tools/bioconductor-clariomshumantranscriptcluster.db", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-clariomshumantranscriptcluster.db", "latest": {"8.8.0--r42hdfd78af_2": "sha256:771ac0ce465b70070d4e8db5f8cf498338e81b713a4f1885cdbe5c9a660a8277"}, "tags": {"8.8.0--r41hdfd78af_1": "sha256:3b5ca01f3b0b9bf2878ed4388248e375d321b06d6a09245556bcd010b48d86d8", "8.8.0--r42hdfd78af_2": "sha256:771ac0ce465b70070d4e8db5f8cf498338e81b713a4f1885cdbe5c9a660a8277"}, "docker": "quay.io/biocontainers/bioconductor-clariomshumantranscriptcluster.db", "aliases": {".bioconductor-clariomshumantranscriptcluster.db-post-link.sh": "/usr/local/bin/.bioconductor-clariomshumantranscriptcluster.db-post-link.sh", ".bioconductor-clariomshumantranscriptcluster.db-pre-unlink.sh": "/usr/local/bin/.bioconductor-clariomshumantranscriptcluster.db-pre-unlink.sh"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-clariomshumantranscriptcluster.db.
shpc-registry automated BioContainers addition for bioconductor-clariomshumantranscriptcluster.db
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-clariomshumantranscriptcluster.db
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-clariomshumantranscriptcluster.db:8.8.0--r42hdfd78af_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-clariomshumantranscriptcluster.db/8.8.0--r42hdfd78af_2
$ module help quay.io/biocontainers/bioconductor-clariomshumantranscriptcluster.db/8.8.0--r42hdfd78af_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-clariomshumantranscriptcluster.db-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-clariomshumantranscriptcluster.db-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-clariomshumantranscriptcluster.db-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-clariomshumantranscriptcluster.db-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-clariomshumantranscriptcluster.db-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-clariomshumantranscriptcluster.db-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .bioconductor-clariomshumantranscriptcluster.db-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-clariomshumantranscriptcluster.db-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-clariomshumantranscriptcluster.db-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-clariomshumantranscriptcluster.db-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### .bioconductor-clariomshumantranscriptcluster.db-pre-unlink.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-clariomshumantranscriptcluster.db-pre-unlink.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-clariomshumantranscriptcluster.db-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-clariomshumantranscriptcluster.db-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
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