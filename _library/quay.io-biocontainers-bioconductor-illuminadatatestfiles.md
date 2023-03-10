---
layout: container
name:  "quay.io/biocontainers/bioconductor-illuminadatatestfiles"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-illuminadatatestfiles/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-illuminadatatestfiles/container.yaml"
updated_at: "2023-01-13 03:20:24.458389"
latest: "1.35.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-illuminadatatestfiles"

versions:
 - "1.32.0--r41hdfd78af_1"
 - "1.35.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-illuminadatatestfiles"
config: {"url": "https://biocontainers.pro/tools/bioconductor-illuminadatatestfiles", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-illuminadatatestfiles", "latest": {"1.35.0--r42hdfd78af_0": "sha256:c64283244d033e866257bdcb54a9b382a7b16767710d403e856438adbd6941d0"}, "tags": {"1.32.0--r41hdfd78af_1": "sha256:5c1057145f4010b558883a2e4d010093aa223ab5196600e46b9592011be423e6", "1.35.0--r42hdfd78af_0": "sha256:c64283244d033e866257bdcb54a9b382a7b16767710d403e856438adbd6941d0"}, "docker": "quay.io/biocontainers/bioconductor-illuminadatatestfiles"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-illuminadatatestfiles.
shpc-registry automated BioContainers addition for bioconductor-illuminadatatestfiles
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-illuminadatatestfiles
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-illuminadatatestfiles:1.35.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-illuminadatatestfiles/1.35.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-illuminadatatestfiles/1.35.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-illuminadatatestfiles-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-illuminadatatestfiles-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-illuminadatatestfiles-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-illuminadatatestfiles-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-illuminadatatestfiles-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-illuminadatatestfiles-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-illuminadatatestfiles

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