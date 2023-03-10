---
layout: container
name:  "quay.io/biocontainers/bioconductor-mnem"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-mnem/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-mnem/container.yaml"
updated_at: "2023-01-13 02:48:03.169545"
latest: "1.14.0--r42hc247a5b_0"
container_url: "https://biocontainers.pro/tools/bioconductor-mnem"
aliases:
 - "x86_64-conda-linux-gnu-gfortran.bin"
versions:
 - "1.8.0--r41h399db7b_0"
 - "1.14.0--r42hc247a5b_0"
 - "1.10.0--r41hc247a5b_2"
description: "shpc-registry automated BioContainers addition for bioconductor-mnem"
config: {"url": "https://biocontainers.pro/tools/bioconductor-mnem", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-mnem", "latest": {"1.14.0--r42hc247a5b_0": "sha256:40cc0a551191bed4f940aeb8474747f9c099a740a5aec7ca7209f5c69dfb04e4"}, "tags": {"1.8.0--r41h399db7b_0": "sha256:bda62cdfda52acaebac431bb93799c17bbe102d1310e6f5669b2f7e0745f7cb0", "1.14.0--r42hc247a5b_0": "sha256:40cc0a551191bed4f940aeb8474747f9c099a740a5aec7ca7209f5c69dfb04e4", "1.10.0--r41hc247a5b_2": "sha256:747565ff4ab5f596c71d4aede333a117652a67f6822bec9ace4ce6aa87d24365"}, "docker": "quay.io/biocontainers/bioconductor-mnem", "aliases": {"x86_64-conda-linux-gnu-gfortran.bin": "/usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-mnem.
shpc-registry automated BioContainers addition for bioconductor-mnem
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-mnem
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-mnem:1.14.0--r42hc247a5b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-mnem/1.14.0--r42hc247a5b_0
$ module help quay.io/biocontainers/bioconductor-mnem/1.14.0--r42hc247a5b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-mnem-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-mnem-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-mnem-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-mnem-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-mnem-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-mnem-inspect-deffile:

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