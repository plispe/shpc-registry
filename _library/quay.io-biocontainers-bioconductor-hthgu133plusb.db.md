---
layout: container
name:  "quay.io/biocontainers/bioconductor-hthgu133plusb.db"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-hthgu133plusb.db/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-hthgu133plusb.db/container.yaml"
updated_at: "2022-11-20 00:01:24.642908"
latest: "3.13.0--r42hdfd78af_2"
container_url: "https://biocontainers.pro/tools/bioconductor-hthgu133plusb.db"
aliases:
 - ".bioconductor-hthgu133plusb.db-post-link.sh"
 - ".bioconductor-hthgu133plusb.db-pre-unlink.sh"
versions:
 - "3.13.0--r41hdfd78af_1"
 - "3.13.0--r42hdfd78af_2"
description: "shpc-registry automated BioContainers addition for bioconductor-hthgu133plusb.db"
config: {"url": "https://biocontainers.pro/tools/bioconductor-hthgu133plusb.db", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-hthgu133plusb.db", "latest": {"3.13.0--r42hdfd78af_2": "sha256:608496b6d97f89c029f9b6ace6e79821189da6b3bfbf4e50deff6e69339b4519"}, "tags": {"3.13.0--r41hdfd78af_1": "sha256:56e3f6264bb1b4458d6d2730d31d26d427ff208737da44fc48b2202e72a868a5", "3.13.0--r42hdfd78af_2": "sha256:608496b6d97f89c029f9b6ace6e79821189da6b3bfbf4e50deff6e69339b4519"}, "docker": "quay.io/biocontainers/bioconductor-hthgu133plusb.db", "aliases": {".bioconductor-hthgu133plusb.db-post-link.sh": "/usr/local/bin/.bioconductor-hthgu133plusb.db-post-link.sh", ".bioconductor-hthgu133plusb.db-pre-unlink.sh": "/usr/local/bin/.bioconductor-hthgu133plusb.db-pre-unlink.sh"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-hthgu133plusb.db.
shpc-registry automated BioContainers addition for bioconductor-hthgu133plusb.db
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-hthgu133plusb.db
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-hthgu133plusb.db:3.13.0--r42hdfd78af_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-hthgu133plusb.db/3.13.0--r42hdfd78af_2
$ module help quay.io/biocontainers/bioconductor-hthgu133plusb.db/3.13.0--r42hdfd78af_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-hthgu133plusb.db-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-hthgu133plusb.db-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-hthgu133plusb.db-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-hthgu133plusb.db-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-hthgu133plusb.db-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-hthgu133plusb.db-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .bioconductor-hthgu133plusb.db-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-hthgu133plusb.db-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-hthgu133plusb.db-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-hthgu133plusb.db-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### .bioconductor-hthgu133plusb.db-pre-unlink.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-hthgu133plusb.db-pre-unlink.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-hthgu133plusb.db-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-hthgu133plusb.db-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
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