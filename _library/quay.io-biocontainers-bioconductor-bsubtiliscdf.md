---
layout: container
name:  "quay.io/biocontainers/bioconductor-bsubtiliscdf"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-bsubtiliscdf/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-bsubtiliscdf/container.yaml"
updated_at: "2023-01-13 03:34:53.769693"
latest: "2.18.0--r42hdfd78af_10"
container_url: "https://biocontainers.pro/tools/bioconductor-bsubtiliscdf"

versions:
 - "2.18.0--r41hdfd78af_9"
 - "2.18.0--r42hdfd78af_10"
description: "shpc-registry automated BioContainers addition for bioconductor-bsubtiliscdf"
config: {"url": "https://biocontainers.pro/tools/bioconductor-bsubtiliscdf", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-bsubtiliscdf", "latest": {"2.18.0--r42hdfd78af_10": "sha256:9cd7b0d7c0851c01897901d091d8538fbe9eda8aa0c57a19096fe6e648e2642d"}, "tags": {"2.18.0--r41hdfd78af_9": "sha256:1c4accc5ac5087c1506f9e46f4cb904194c704d7d21ea2cedb1ad824c200281f", "2.18.0--r42hdfd78af_10": "sha256:9cd7b0d7c0851c01897901d091d8538fbe9eda8aa0c57a19096fe6e648e2642d"}, "docker": "quay.io/biocontainers/bioconductor-bsubtiliscdf"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-bsubtiliscdf.
shpc-registry automated BioContainers addition for bioconductor-bsubtiliscdf
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-bsubtiliscdf
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-bsubtiliscdf:2.18.0--r42hdfd78af_10
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-bsubtiliscdf/2.18.0--r42hdfd78af_10
$ module help quay.io/biocontainers/bioconductor-bsubtiliscdf/2.18.0--r42hdfd78af_10
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-bsubtiliscdf-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-bsubtiliscdf-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-bsubtiliscdf-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-bsubtiliscdf-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-bsubtiliscdf-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-bsubtiliscdf-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-bsubtiliscdf

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