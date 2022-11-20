---
layout: container
name:  "quay.io/biocontainers/bioconductor-prebsdata"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-prebsdata/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-prebsdata/container.yaml"
updated_at: "2022-11-20 00:15:13.568364"
latest: "1.30.0--r41hdfd78af_1"
container_url: "https://biocontainers.pro/tools/bioconductor-prebsdata"
aliases:
 - ".bioconductor-prebsdata-post-link.sh"
 - ".bioconductor-prebsdata-pre-unlink.sh"
versions:
 - "1.30.0--r41hdfd78af_1"
description: "shpc-registry automated BioContainers addition for bioconductor-prebsdata"
config: {"url": "https://biocontainers.pro/tools/bioconductor-prebsdata", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-prebsdata", "latest": {"1.30.0--r41hdfd78af_1": "sha256:eaf27840a3437a21bf506db0ef089b7f493a2f01dfde8ff5a4ad04edc3c26e17"}, "tags": {"1.30.0--r41hdfd78af_1": "sha256:eaf27840a3437a21bf506db0ef089b7f493a2f01dfde8ff5a4ad04edc3c26e17"}, "docker": "quay.io/biocontainers/bioconductor-prebsdata", "aliases": {".bioconductor-prebsdata-post-link.sh": "/usr/local/bin/.bioconductor-prebsdata-post-link.sh", ".bioconductor-prebsdata-pre-unlink.sh": "/usr/local/bin/.bioconductor-prebsdata-pre-unlink.sh"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-prebsdata.
shpc-registry automated BioContainers addition for bioconductor-prebsdata
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-prebsdata
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-prebsdata:1.30.0--r41hdfd78af_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-prebsdata/1.30.0--r41hdfd78af_1
$ module help quay.io/biocontainers/bioconductor-prebsdata/1.30.0--r41hdfd78af_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-prebsdata-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-prebsdata-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-prebsdata-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-prebsdata-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-prebsdata-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-prebsdata-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .bioconductor-prebsdata-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-prebsdata-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-prebsdata-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-prebsdata-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### .bioconductor-prebsdata-pre-unlink.sh

```bash
$ singularity exec <container> /usr/local/bin/.bioconductor-prebsdata-pre-unlink.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.bioconductor-prebsdata-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.bioconductor-prebsdata-pre-unlink.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
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