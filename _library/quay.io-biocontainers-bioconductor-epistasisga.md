---
layout: container
name:  "quay.io/biocontainers/bioconductor-epistasisga"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-epistasisga/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-epistasisga/container.yaml"
updated_at: "2023-01-13 02:52:08.391785"
latest: "1.0.0--r42hc247a5b_0"
container_url: "https://biocontainers.pro/tools/bioconductor-epistasisga"
aliases:
 - "glpsol"
versions:
 - "1.0.0--r42hc247a5b_0"
description: "singularity registry hpc automated addition for bioconductor-epistasisga"
config: {"url": "https://biocontainers.pro/tools/bioconductor-epistasisga", "maintainer": "@vsoch", "description": "singularity registry hpc automated addition for bioconductor-epistasisga", "latest": {"1.0.0--r42hc247a5b_0": "sha256:504a3d6c60343c7e17ea0d8851e46764c70c5b9a3839be9f62f195defc9cf10f"}, "tags": {"1.0.0--r42hc247a5b_0": "sha256:504a3d6c60343c7e17ea0d8851e46764c70c5b9a3839be9f62f195defc9cf10f"}, "docker": "quay.io/biocontainers/bioconductor-epistasisga", "aliases": {"glpsol": "/usr/local/bin/glpsol"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-epistasisga.
singularity registry hpc automated addition for bioconductor-epistasisga
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-epistasisga
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-epistasisga:1.0.0--r42hc247a5b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-epistasisga/1.0.0--r42hc247a5b_0
$ module help quay.io/biocontainers/bioconductor-epistasisga/1.0.0--r42hc247a5b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-epistasisga-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-epistasisga-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-epistasisga-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-epistasisga-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-epistasisga-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-epistasisga-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### glpsol

```bash
$ singularity exec <container> /usr/local/bin/glpsol
$ podman run --it --rm --entrypoint /usr/local/bin/glpsol   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/glpsol   -v ${PWD} -w ${PWD} <container> -c " $@"
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