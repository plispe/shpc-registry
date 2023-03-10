---
layout: container
name:  "quay.io/biocontainers/bioconductor-svaplsseq"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-svaplsseq/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-svaplsseq/container.yaml"
updated_at: "2023-01-13 03:25:32.156350"
latest: "1.13.0--r40_0"
container_url: "https://biocontainers.pro/tools/bioconductor-svaplsseq"
aliases:
 - "idn2"
 - "wget"
 - "c89"
 - "c99"
versions:
 - "1.8.1--r351_0"
 - "1.13.0--r40_0"
 - "1.12.0--r36_0"
 - "1.10.0--r36_1"
description: "shpc-registry automated BioContainers addition for bioconductor-svaplsseq"
config: {"url": "https://biocontainers.pro/tools/bioconductor-svaplsseq", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-svaplsseq", "latest": {"1.13.0--r40_0": "sha256:277ff84918a5b45bc650cec5b77c655e3aab47b8983aca7bab4fad24da0e3fb8"}, "tags": {"1.8.1--r351_0": "sha256:e401f5dcf3927326f5dd2dd336e8ddbdc1f166d76d91906d11e6d07c2374fc3f", "1.13.0--r40_0": "sha256:277ff84918a5b45bc650cec5b77c655e3aab47b8983aca7bab4fad24da0e3fb8", "1.12.0--r36_0": "sha256:77239871ab071d2582e1fbc9d298013e3f0715ffd8320f43c3048f6b5ba9643c", "1.10.0--r36_1": "sha256:16b06b741c4fe7cd2b2da53c3e3a186a01891aecbac1207b87ea7cb56174f0b9"}, "docker": "quay.io/biocontainers/bioconductor-svaplsseq", "aliases": {"idn2": "/usr/local/bin/idn2", "wget": "/usr/local/bin/wget", "c89": "/usr/local/bin/c89", "c99": "/usr/local/bin/c99"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-svaplsseq.
shpc-registry automated BioContainers addition for bioconductor-svaplsseq
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-svaplsseq
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-svaplsseq:1.13.0--r40_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-svaplsseq/1.13.0--r40_0
$ module help quay.io/biocontainers/bioconductor-svaplsseq/1.13.0--r40_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-svaplsseq-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-svaplsseq-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-svaplsseq-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-svaplsseq-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-svaplsseq-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-svaplsseq-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### idn2

```bash
$ singularity exec <container> /usr/local/bin/idn2
$ podman run --it --rm --entrypoint /usr/local/bin/idn2   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/idn2   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### wget

```bash
$ singularity exec <container> /usr/local/bin/wget
$ podman run --it --rm --entrypoint /usr/local/bin/wget   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/wget   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### c89

```bash
$ singularity exec <container> /usr/local/bin/c89
$ podman run --it --rm --entrypoint /usr/local/bin/c89   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/c89   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### c99

```bash
$ singularity exec <container> /usr/local/bin/c99
$ podman run --it --rm --entrypoint /usr/local/bin/c99   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/c99   -v ${PWD} -w ${PWD} <container> -c " $@"
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