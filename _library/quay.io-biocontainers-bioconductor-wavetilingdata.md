---
layout: container
name:  "quay.io/biocontainers/bioconductor-wavetilingdata"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-wavetilingdata/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-wavetilingdata/container.yaml"
updated_at: "2023-01-13 03:33:35.623392"
latest: "1.26.0--r40hdfd78af_1"
container_url: "https://biocontainers.pro/tools/bioconductor-wavetilingdata"
aliases:
 - "x86_64-conda-linux-gnu-gfortran.bin"
versions:
 - "1.26.0--r40hdfd78af_1"
description: "shpc-registry automated BioContainers addition for bioconductor-wavetilingdata"
config: {"url": "https://biocontainers.pro/tools/bioconductor-wavetilingdata", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-wavetilingdata", "latest": {"1.26.0--r40hdfd78af_1": "sha256:e110afe33bece848bd7ab064a8089434211e495c853f9e54ffc6e5a121dca7a7"}, "tags": {"1.26.0--r40hdfd78af_1": "sha256:e110afe33bece848bd7ab064a8089434211e495c853f9e54ffc6e5a121dca7a7"}, "docker": "quay.io/biocontainers/bioconductor-wavetilingdata", "aliases": {"x86_64-conda-linux-gnu-gfortran.bin": "/usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-wavetilingdata.
shpc-registry automated BioContainers addition for bioconductor-wavetilingdata
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-wavetilingdata
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-wavetilingdata:1.26.0--r40hdfd78af_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-wavetilingdata/1.26.0--r40hdfd78af_1
$ module help quay.io/biocontainers/bioconductor-wavetilingdata/1.26.0--r40hdfd78af_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-wavetilingdata-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-wavetilingdata-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-wavetilingdata-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-wavetilingdata-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-wavetilingdata-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-wavetilingdata-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### x86_64-conda-linux-gnu-gfortran.bin

```bash
$ singularity exec <container> /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin
$ podman run --it --rm --entrypoint /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin   -v ${PWD} -w ${PWD} <container> -c " $@"
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