---
layout: container
name:  "quay.io/biocontainers/bioconductor-grndata"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-grndata/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-grndata/container.yaml"
updated_at: "2023-01-13 03:01:08.685265"
latest: "1.29.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-grndata"

versions:
 - "1.26.0--r41hdfd78af_1"
 - "1.29.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-grndata"
config: {"url": "https://biocontainers.pro/tools/bioconductor-grndata", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-grndata", "latest": {"1.29.0--r42hdfd78af_0": "sha256:c7074fa46e4e6176ef739b1ddf3a7bef52b91d060fe3313136964dd254c93bb0"}, "tags": {"1.26.0--r41hdfd78af_1": "sha256:1a0c8ad51000e9e40a154f706b2f1e8dbea1150a168361af08bce45c73886759", "1.29.0--r42hdfd78af_0": "sha256:c7074fa46e4e6176ef739b1ddf3a7bef52b91d060fe3313136964dd254c93bb0"}, "docker": "quay.io/biocontainers/bioconductor-grndata"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-grndata.
shpc-registry automated BioContainers addition for bioconductor-grndata
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-grndata
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-grndata:1.29.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-grndata/1.29.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-grndata/1.29.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-grndata-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-grndata-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-grndata-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-grndata-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-grndata-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-grndata-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-grndata

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