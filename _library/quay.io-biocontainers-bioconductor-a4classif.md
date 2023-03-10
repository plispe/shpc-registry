---
layout: container
name:  "quay.io/biocontainers/bioconductor-a4classif"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-a4classif/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-a4classif/container.yaml"
updated_at: "2023-01-13 03:26:53.829952"
latest: "1.46.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-a4classif"

versions:
 - "1.42.0--r41hdfd78af_0"
 - "1.46.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-a4classif"
config: {"url": "https://biocontainers.pro/tools/bioconductor-a4classif", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-a4classif", "latest": {"1.46.0--r42hdfd78af_0": "sha256:f8a860c6326be72087987f6b2aa6d571ee23a052e338816b29cb2677db202c12"}, "tags": {"1.42.0--r41hdfd78af_0": "sha256:5d1bfc36c3c9c89a3b32d603fb16d44d7e273d05be0e1d8b21090af67a7d0c21", "1.46.0--r42hdfd78af_0": "sha256:f8a860c6326be72087987f6b2aa6d571ee23a052e338816b29cb2677db202c12"}, "docker": "quay.io/biocontainers/bioconductor-a4classif"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-a4classif.
shpc-registry automated BioContainers addition for bioconductor-a4classif
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-a4classif
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-a4classif:1.46.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-a4classif/1.46.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-a4classif/1.46.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-a4classif-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-a4classif-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-a4classif-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-a4classif-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-a4classif-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-a4classif-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-a4classif

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