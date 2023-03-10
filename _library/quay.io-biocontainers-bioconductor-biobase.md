---
layout: container
name:  "quay.io/biocontainers/bioconductor-biobase"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-biobase/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-biobase/container.yaml"
updated_at: "2023-01-13 02:52:25.591132"
latest: "2.58.0--r42hc0cfd56_0"
container_url: "https://biocontainers.pro/tools/bioconductor-biobase"

versions:
 - "2.54.0--r41hc0cfd56_2"
 - "2.58.0--r42hc0cfd56_0"
description: "shpc-registry automated BioContainers addition for bioconductor-biobase"
config: {"url": "https://biocontainers.pro/tools/bioconductor-biobase", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-biobase", "latest": {"2.58.0--r42hc0cfd56_0": "sha256:6c6dae68c9df7132515793e2212a6080075a5421440e4410ab079cae751addfa"}, "tags": {"2.54.0--r41hc0cfd56_2": "sha256:09d23e89a31b22e5a06172b65fe1561670501c066b1c28981aa7f139efb5d94e", "2.58.0--r42hc0cfd56_0": "sha256:6c6dae68c9df7132515793e2212a6080075a5421440e4410ab079cae751addfa"}, "docker": "quay.io/biocontainers/bioconductor-biobase"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-biobase.
shpc-registry automated BioContainers addition for bioconductor-biobase
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-biobase
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-biobase:2.58.0--r42hc0cfd56_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-biobase/2.58.0--r42hc0cfd56_0
$ module help quay.io/biocontainers/bioconductor-biobase/2.58.0--r42hc0cfd56_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-biobase-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-biobase-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-biobase-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-biobase-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-biobase-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-biobase-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-biobase

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