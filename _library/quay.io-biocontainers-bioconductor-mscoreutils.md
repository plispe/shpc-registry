---
layout: container
name:  "quay.io/biocontainers/bioconductor-mscoreutils"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-mscoreutils/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-mscoreutils/container.yaml"
updated_at: "2023-01-13 02:54:29.188827"
latest: "1.10.0--r42hc247a5b_0"
container_url: "https://biocontainers.pro/tools/bioconductor-mscoreutils"

versions:
 - "1.6.2--r41hc247a5b_0"
 - "1.10.0--r42hc247a5b_0"
description: "shpc-registry automated BioContainers addition for bioconductor-mscoreutils"
config: {"url": "https://biocontainers.pro/tools/bioconductor-mscoreutils", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-mscoreutils", "latest": {"1.10.0--r42hc247a5b_0": "sha256:b991342ba20d3f7157de11f4f344ae9dea5140e9d2f54b616117ccd055625cc1"}, "tags": {"1.6.2--r41hc247a5b_0": "sha256:27e654ec2ffcf65573f539bbf0d203a93b154bac6a51a4161f24ca5eb7c6f150", "1.10.0--r42hc247a5b_0": "sha256:b991342ba20d3f7157de11f4f344ae9dea5140e9d2f54b616117ccd055625cc1"}, "docker": "quay.io/biocontainers/bioconductor-mscoreutils"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-mscoreutils.
shpc-registry automated BioContainers addition for bioconductor-mscoreutils
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-mscoreutils
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-mscoreutils:1.10.0--r42hc247a5b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-mscoreutils/1.10.0--r42hc247a5b_0
$ module help quay.io/biocontainers/bioconductor-mscoreutils/1.10.0--r42hc247a5b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-mscoreutils-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-mscoreutils-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-mscoreutils-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-mscoreutils-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-mscoreutils-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-mscoreutils-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-mscoreutils

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