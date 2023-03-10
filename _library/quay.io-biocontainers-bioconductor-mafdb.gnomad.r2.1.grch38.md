---
layout: container
name:  "quay.io/biocontainers/bioconductor-mafdb.gnomad.r2.1.grch38"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-mafdb.gnomad.r2.1.grch38/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-mafdb.gnomad.r2.1.grch38/container.yaml"
updated_at: "2023-01-13 03:14:14.216152"
latest: "3.10.0--r41hdfd78af_4"
container_url: "https://biocontainers.pro/tools/bioconductor-mafdb.gnomad.r2.1.grch38"

versions:
 - "3.10.0--r41hdfd78af_4"
description: "shpc-registry automated BioContainers addition for bioconductor-mafdb.gnomad.r2.1.grch38"
config: {"url": "https://biocontainers.pro/tools/bioconductor-mafdb.gnomad.r2.1.grch38", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-mafdb.gnomad.r2.1.grch38", "latest": {"3.10.0--r41hdfd78af_4": "sha256:777bd4fc4dd75ea293ce05de3f14c490a85b9bfa7e496f0e2e30017aa8751107"}, "tags": {"3.10.0--r41hdfd78af_4": "sha256:777bd4fc4dd75ea293ce05de3f14c490a85b9bfa7e496f0e2e30017aa8751107"}, "docker": "quay.io/biocontainers/bioconductor-mafdb.gnomad.r2.1.grch38"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-mafdb.gnomad.r2.1.grch38.
shpc-registry automated BioContainers addition for bioconductor-mafdb.gnomad.r2.1.grch38
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-mafdb.gnomad.r2.1.grch38
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-mafdb.gnomad.r2.1.grch38:3.10.0--r41hdfd78af_4
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-mafdb.gnomad.r2.1.grch38/3.10.0--r41hdfd78af_4
$ module help quay.io/biocontainers/bioconductor-mafdb.gnomad.r2.1.grch38/3.10.0--r41hdfd78af_4
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-mafdb.gnomad.r2.1.grch38-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-mafdb.gnomad.r2.1.grch38-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-mafdb.gnomad.r2.1.grch38-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-mafdb.gnomad.r2.1.grch38-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-mafdb.gnomad.r2.1.grch38-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-mafdb.gnomad.r2.1.grch38-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-mafdb.gnomad.r2.1.grch38

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