---
layout: container
name:  "quay.io/biocontainers/fastq-multx"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/fastq-multx/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/fastq-multx/container.yaml"
updated_at: "2022-11-20 00:45:48.932249"
latest: "1.4.2--h9f5acd7_2"
container_url: "https://biocontainers.pro/tools/fastq-multx"
aliases:
 - "fastq-multx"
versions:
 - "1.4.2--h9f5acd7_2"
description: "shpc-registry automated BioContainers addition for fastq-multx"
config: {"url": "https://biocontainers.pro/tools/fastq-multx", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for fastq-multx", "latest": {"1.4.2--h9f5acd7_2": "sha256:cdc4a85646a0a79053076460657ca015c047a49c6c74752080c603699cc4f266"}, "tags": {"1.4.2--h9f5acd7_2": "sha256:cdc4a85646a0a79053076460657ca015c047a49c6c74752080c603699cc4f266"}, "docker": "quay.io/biocontainers/fastq-multx", "aliases": {"fastq-multx": "/usr/local/bin/fastq-multx"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/fastq-multx.
shpc-registry automated BioContainers addition for fastq-multx
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/fastq-multx
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/fastq-multx:1.4.2--h9f5acd7_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/fastq-multx/1.4.2--h9f5acd7_2
$ module help quay.io/biocontainers/fastq-multx/1.4.2--h9f5acd7_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### fastq-multx-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### fastq-multx-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### fastq-multx-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### fastq-multx-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### fastq-multx-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### fastq-multx-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### fastq-multx

```bash
$ singularity exec <container> /usr/local/bin/fastq-multx
$ podman run --it --rm --entrypoint /usr/local/bin/fastq-multx   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/fastq-multx   -v ${PWD} -w ${PWD} <container> -c " $@"
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