---
layout: container
name:  "quay.io/biocontainers/r-lme4qtl"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/r-lme4qtl/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/r-lme4qtl/container.yaml"
updated_at: "2023-01-13 03:12:14.583222"
latest: "0.1.10--r42h9ee0642_5"
container_url: "https://biocontainers.pro/tools/r-lme4qtl"
aliases:
 - "x86_64-conda-linux-gnu-gfortran.bin"
versions:
 - "0.1.10--r41h9ee0642_4"
 - "0.1.10--r42h9ee0642_5"
description: "shpc-registry automated BioContainers addition for r-lme4qtl"
config: {"url": "https://biocontainers.pro/tools/r-lme4qtl", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for r-lme4qtl", "latest": {"0.1.10--r42h9ee0642_5": "sha256:3bef009e642ba4e7a46a0bfadee29b089d5593ef4897242b55582b8ca52651f2"}, "tags": {"0.1.10--r41h9ee0642_4": "sha256:0044f60b307f24dcff532a867d9f8e3123829bec6b50068e11c9335d1bab97ba", "0.1.10--r42h9ee0642_5": "sha256:3bef009e642ba4e7a46a0bfadee29b089d5593ef4897242b55582b8ca52651f2"}, "docker": "quay.io/biocontainers/r-lme4qtl", "aliases": {"x86_64-conda-linux-gnu-gfortran.bin": "/usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/r-lme4qtl.
shpc-registry automated BioContainers addition for r-lme4qtl
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/r-lme4qtl
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/r-lme4qtl:0.1.10--r42h9ee0642_5
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/r-lme4qtl/0.1.10--r42h9ee0642_5
$ module help quay.io/biocontainers/r-lme4qtl/0.1.10--r42h9ee0642_5
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### r-lme4qtl-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### r-lme4qtl-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### r-lme4qtl-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### r-lme4qtl-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### r-lme4qtl-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### r-lme4qtl-inspect-deffile:

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