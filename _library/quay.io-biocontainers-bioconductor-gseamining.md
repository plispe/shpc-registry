---
layout: container
name:  "quay.io/biocontainers/bioconductor-gseamining"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-gseamining/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-gseamining/container.yaml"
updated_at: "2023-01-13 02:52:35.330154"
latest: "1.8.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-gseamining"

versions:
 - "1.4.0--r41hdfd78af_0"
 - "1.8.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-gseamining"
config: {"url": "https://biocontainers.pro/tools/bioconductor-gseamining", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-gseamining", "latest": {"1.8.0--r42hdfd78af_0": "sha256:89b012a3d0060ff64e6e5e5a546f2ce8feeac1681c7f6dcf33ab7a137c604d80"}, "tags": {"1.4.0--r41hdfd78af_0": "sha256:4a92e666d700d905e7fc93e31835df5c8b3b5fb6fdc6a7455f6d75c676e3a96c", "1.8.0--r42hdfd78af_0": "sha256:89b012a3d0060ff64e6e5e5a546f2ce8feeac1681c7f6dcf33ab7a137c604d80"}, "docker": "quay.io/biocontainers/bioconductor-gseamining"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-gseamining.
shpc-registry automated BioContainers addition for bioconductor-gseamining
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-gseamining
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-gseamining:1.8.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-gseamining/1.8.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-gseamining/1.8.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-gseamining-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-gseamining-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-gseamining-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-gseamining-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-gseamining-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-gseamining-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-gseamining

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