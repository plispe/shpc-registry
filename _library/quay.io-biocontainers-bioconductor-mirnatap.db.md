---
layout: container
name:  "quay.io/biocontainers/bioconductor-mirnatap.db"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-mirnatap.db/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-mirnatap.db/container.yaml"
updated_at: "2023-01-13 03:14:47.849846"
latest: "0.99.10--r42hdfd78af_13"
container_url: "https://biocontainers.pro/tools/bioconductor-mirnatap.db"
aliases:
 - "x86_64-conda-linux-gnu-gfortran.bin"
versions:
 - "0.99.10--r40hdfd78af_9"
 - "0.99.10--r42hdfd78af_13"
description: "shpc-registry automated BioContainers addition for bioconductor-mirnatap.db"
config: {"url": "https://biocontainers.pro/tools/bioconductor-mirnatap.db", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-mirnatap.db", "latest": {"0.99.10--r42hdfd78af_13": "sha256:5be392db3f746ae4f9dde2a8f40235546cfb540f93dc00ea17179937c1cffad9"}, "tags": {"0.99.10--r40hdfd78af_9": "sha256:b3ee070a7fca2719a8184e637f1bc17fed0030f16da827dc381774279061ba1c", "0.99.10--r42hdfd78af_13": "sha256:5be392db3f746ae4f9dde2a8f40235546cfb540f93dc00ea17179937c1cffad9"}, "docker": "quay.io/biocontainers/bioconductor-mirnatap.db", "aliases": {"x86_64-conda-linux-gnu-gfortran.bin": "/usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-mirnatap.db.
shpc-registry automated BioContainers addition for bioconductor-mirnatap.db
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-mirnatap.db
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-mirnatap.db:0.99.10--r42hdfd78af_13
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-mirnatap.db/0.99.10--r42hdfd78af_13
$ module help quay.io/biocontainers/bioconductor-mirnatap.db/0.99.10--r42hdfd78af_13
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-mirnatap.db-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-mirnatap.db-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-mirnatap.db-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-mirnatap.db-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-mirnatap.db-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-mirnatap.db-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### x86_64-conda-linux-gnu-gfortran.bin

```bash
$ singularity exec <container> /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin
$ podman run --it --rm --entrypoint /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin   -v ${PWD} -w ${PWD} <container> -c " $@"
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