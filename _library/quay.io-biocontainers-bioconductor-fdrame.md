---
layout: container
name:  "quay.io/biocontainers/bioconductor-fdrame"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-fdrame/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-fdrame/container.yaml"
updated_at: "2023-01-13 03:07:09.431419"
latest: "1.70.0--r42hc0cfd56_0"
container_url: "https://biocontainers.pro/tools/bioconductor-fdrame"

versions:
 - "1.66.0--r41hc0cfd56_2"
 - "1.70.0--r42hc0cfd56_0"
description: "shpc-registry automated BioContainers addition for bioconductor-fdrame"
config: {"url": "https://biocontainers.pro/tools/bioconductor-fdrame", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-fdrame", "latest": {"1.70.0--r42hc0cfd56_0": "sha256:605530d62f299f7038896709cf76176daf031cb31348264c76455bd4b5796f07"}, "tags": {"1.66.0--r41hc0cfd56_2": "sha256:d794d14fe3eb4ffb17e694ce1c96f9758a4fe0628a2b4afb37b31e9347a75a80", "1.70.0--r42hc0cfd56_0": "sha256:605530d62f299f7038896709cf76176daf031cb31348264c76455bd4b5796f07"}, "docker": "quay.io/biocontainers/bioconductor-fdrame"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-fdrame.
shpc-registry automated BioContainers addition for bioconductor-fdrame
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-fdrame
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-fdrame:1.70.0--r42hc0cfd56_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-fdrame/1.70.0--r42hc0cfd56_0
$ module help quay.io/biocontainers/bioconductor-fdrame/1.70.0--r42hc0cfd56_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-fdrame-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-fdrame-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-fdrame-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-fdrame-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-fdrame-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-fdrame-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-fdrame

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