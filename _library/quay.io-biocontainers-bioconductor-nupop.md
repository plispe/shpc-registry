---
layout: container
name:  "quay.io/biocontainers/bioconductor-nupop"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-nupop/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-nupop/container.yaml"
updated_at: "2023-01-13 03:45:10.568051"
latest: "2.6.0--r42hefde4a7_0"
container_url: "https://biocontainers.pro/tools/bioconductor-nupop"

versions:
 - "2.2.0--r41hefde4a7_2"
 - "2.6.0--r42hefde4a7_0"
description: "shpc-registry automated BioContainers addition for bioconductor-nupop"
config: {"url": "https://biocontainers.pro/tools/bioconductor-nupop", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-nupop", "latest": {"2.6.0--r42hefde4a7_0": "sha256:b56c214c8285b07f716059a3005475ff33c05de044b123e571991a33064bf2e5"}, "tags": {"2.2.0--r41hefde4a7_2": "sha256:570f4d0cb7bb3299f4ba501423a3958c3b46bb50e96da4a4032319d029f54223", "2.6.0--r42hefde4a7_0": "sha256:b56c214c8285b07f716059a3005475ff33c05de044b123e571991a33064bf2e5"}, "docker": "quay.io/biocontainers/bioconductor-nupop"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-nupop.
shpc-registry automated BioContainers addition for bioconductor-nupop
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-nupop
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-nupop:2.6.0--r42hefde4a7_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-nupop/2.6.0--r42hefde4a7_0
$ module help quay.io/biocontainers/bioconductor-nupop/2.6.0--r42hefde4a7_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-nupop-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-nupop-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-nupop-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-nupop-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-nupop-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-nupop-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-nupop

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