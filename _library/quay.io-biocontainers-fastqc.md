---
layout: container
name:  "quay.io/biocontainers/fastqc"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/fastqc/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/fastqc/container.yaml"
updated_at: "2023-01-13 03:15:32.111609"
latest: "0.11.9--hdfd78af_1"
container_url: "https://biocontainers.pro/tools/fastqc"

versions:
 - "0.11.9--hdfd78af_1"
description: "shpc-registry automated BioContainers addition for fastqc"
config: {"url": "https://biocontainers.pro/tools/fastqc", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for fastqc", "latest": {"0.11.9--hdfd78af_1": "sha256:0c60406af11b0723339df05b10a592aa3f8c9a4d2ec8f213cbe11051e7264a25"}, "tags": {"0.11.9--hdfd78af_1": "sha256:0c60406af11b0723339df05b10a592aa3f8c9a4d2ec8f213cbe11051e7264a25"}, "docker": "quay.io/biocontainers/fastqc"}
---

This module is a singularity container wrapper for quay.io/biocontainers/fastqc.
shpc-registry automated BioContainers addition for fastqc
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/fastqc
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/fastqc:0.11.9--hdfd78af_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/fastqc/0.11.9--hdfd78af_1
$ module help quay.io/biocontainers/fastqc/0.11.9--hdfd78af_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### fastqc-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### fastqc-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### fastqc-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### fastqc-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### fastqc-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### fastqc-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### fastqc

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