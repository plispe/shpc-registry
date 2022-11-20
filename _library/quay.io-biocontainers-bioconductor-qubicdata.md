---
layout: container
name:  "quay.io/biocontainers/bioconductor-qubicdata"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-qubicdata/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-qubicdata/container.yaml"
updated_at: "2022-11-20 00:33:53.721490"
latest: "1.22.0--r41hdfd78af_1"
container_url: "https://biocontainers.pro/tools/bioconductor-qubicdata"
aliases:
 - ".bioconductor-qubicdata-post-link.sh"
 - ".bioconductor-qubicdata-pre-unlink.sh"
versions:
 - "1.22.0--r41hdfd78af_1"
description: "shpc-registry automated BioContainers addition for bioconductor-qubicdata"
config: {"url": "https://biocontainers.pro/tools/bioconductor-qubicdata", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-qubicdata", "latest": {"1.22.0--r41hdfd78af_1": "sha256:473d6dbb59f23c36cf4d61758d1b6609d2760640df916af9801c22109d07c7aa"}, "tags": {"1.22.0--r41hdfd78af_1": "sha256:473d6dbb59f23c36cf4d61758d1b6609d2760640df916af9801c22109d07c7aa"}, "docker": "quay.io/biocontainers/bioconductor-qubicdata", "aliases": {".bioconductor-qubicdata-post-link.sh": "/usr/local/bin/.bioconductor-qubicdata-post-link.sh", ".bioconductor-qubicdata-pre-unlink.sh": "/usr/local/bin/.bioconductor-qubicdata-pre-unlink.sh"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-qubicdata.
shpc-registry automated BioContainers addition for bioconductor-qubicdata
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-qubicdata
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-qubicdata:1.22.0--r41hdfd78af_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-qubicdata/1.22.0--r41hdfd78af_1
$ module help quay.io/biocontainers/bioconductor-qubicdata/1.22.0--r41hdfd78af_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-qubicdata-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-qubicdata-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-qubicdata-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-qubicdata-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-qubicdata-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-qubicdata-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .bioconductor-qubicdata-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-qubicdata-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-qubicdata-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-qubicdata-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### .bioconductor-qubicdata-pre-unlink.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-qubicdata-pre-unlink.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-qubicdata-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-qubicdata-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
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