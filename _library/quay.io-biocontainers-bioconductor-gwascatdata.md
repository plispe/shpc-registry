---
layout: container
name:  "quay.io/biocontainers/bioconductor-gwascatdata"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-gwascatdata/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-gwascatdata/container.yaml"
updated_at: "2023-01-13 03:07:36.480471"
latest: "0.99.6--r42hdfd78af_3"
container_url: "https://biocontainers.pro/tools/bioconductor-gwascatdata"

versions:
 - "0.99.6--r41hdfd78af_2"
 - "0.99.6--r42hdfd78af_3"
description: "shpc-registry automated BioContainers addition for bioconductor-gwascatdata"
config: {"url": "https://biocontainers.pro/tools/bioconductor-gwascatdata", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-gwascatdata", "latest": {"0.99.6--r42hdfd78af_3": "sha256:8d0bd3e668f4faf771aa5bc33f59baa05f1735864b487f082b97dbe7eb81e498"}, "tags": {"0.99.6--r41hdfd78af_2": "sha256:5fb3abad91828c71290b8a0be52464bba439f1988fe573f5acb443210167cb09", "0.99.6--r42hdfd78af_3": "sha256:8d0bd3e668f4faf771aa5bc33f59baa05f1735864b487f082b97dbe7eb81e498"}, "docker": "quay.io/biocontainers/bioconductor-gwascatdata"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-gwascatdata.
shpc-registry automated BioContainers addition for bioconductor-gwascatdata
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-gwascatdata
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-gwascatdata:0.99.6--r42hdfd78af_3
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-gwascatdata/0.99.6--r42hdfd78af_3
$ module help quay.io/biocontainers/bioconductor-gwascatdata/0.99.6--r42hdfd78af_3
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-gwascatdata-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-gwascatdata-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-gwascatdata-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-gwascatdata-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-gwascatdata-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-gwascatdata-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-gwascatdata

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