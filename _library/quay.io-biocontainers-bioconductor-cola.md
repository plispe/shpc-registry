---
layout: container
name:  "quay.io/biocontainers/bioconductor-cola"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-cola/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-cola/container.yaml"
updated_at: "2023-01-13 03:20:39.863478"
latest: "2.4.0--r42hc247a5b_0"
container_url: "https://biocontainers.pro/tools/bioconductor-cola"

versions:
 - "2.0.0--r41hc247a5b_2"
 - "2.4.0--r42hc247a5b_0"
description: "shpc-registry automated BioContainers addition for bioconductor-cola"
config: {"url": "https://biocontainers.pro/tools/bioconductor-cola", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-cola", "latest": {"2.4.0--r42hc247a5b_0": "sha256:c84985241edc3edd31a45312c1334be0781fcb34463b02bd01ef3d8f0802a7fe"}, "tags": {"2.0.0--r41hc247a5b_2": "sha256:830504cb3b77991958e21dce8fa75b9a58f12f9202f6b498410cf0316740d04e", "2.4.0--r42hc247a5b_0": "sha256:c84985241edc3edd31a45312c1334be0781fcb34463b02bd01ef3d8f0802a7fe"}, "docker": "quay.io/biocontainers/bioconductor-cola"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-cola.
shpc-registry automated BioContainers addition for bioconductor-cola
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-cola
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-cola:2.4.0--r42hc247a5b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-cola/2.4.0--r42hc247a5b_0
$ module help quay.io/biocontainers/bioconductor-cola/2.4.0--r42hc247a5b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-cola-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-cola-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-cola-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-cola-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-cola-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-cola-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-cola

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