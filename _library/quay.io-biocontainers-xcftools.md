---
layout: container
name:  "quay.io/biocontainers/xcftools"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/xcftools/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/xcftools/container.yaml"
updated_at: "2023-01-13 03:02:25.334324"
latest: "1.0.7--1"
container_url: "https://biocontainers.pro/tools/xcftools"
aliases:
 - "xcf2png"
 - "xcf2pnm"
 - "xcfinfo"
 - "xcfview"
versions:
 - "1.0.7--1"
description: "shpc-registry automated BioContainers addition for xcftools"
config: {"url": "https://biocontainers.pro/tools/xcftools", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for xcftools", "latest": {"1.0.7--1": "sha256:3388ffe4ae48929ef39f97b34c76114c5db6049902c893016a4285a442130577"}, "tags": {"1.0.7--1": "sha256:3388ffe4ae48929ef39f97b34c76114c5db6049902c893016a4285a442130577"}, "docker": "quay.io/biocontainers/xcftools", "aliases": {"xcf2png": "/usr/local/bin/xcf2png", "xcf2pnm": "/usr/local/bin/xcf2pnm", "xcfinfo": "/usr/local/bin/xcfinfo", "xcfview": "/usr/local/bin/xcfview"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/xcftools.
shpc-registry automated BioContainers addition for xcftools
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/xcftools
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/xcftools:1.0.7--1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/xcftools/1.0.7--1
$ module help quay.io/biocontainers/xcftools/1.0.7--1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### xcftools-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### xcftools-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### xcftools-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### xcftools-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### xcftools-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### xcftools-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### xcf2png

```bash
$ singularity exec <container> /usr/local/bin/xcf2png
$ podman run --it --rm --entrypoint /usr/local/bin/xcf2png   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/xcf2png   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### xcf2pnm

```bash
$ singularity exec <container> /usr/local/bin/xcf2pnm
$ podman run --it --rm --entrypoint /usr/local/bin/xcf2pnm   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/xcf2pnm   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### xcfinfo

```bash
$ singularity exec <container> /usr/local/bin/xcfinfo
$ podman run --it --rm --entrypoint /usr/local/bin/xcfinfo   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/xcfinfo   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### xcfview

```bash
$ singularity exec <container> /usr/local/bin/xcfview
$ podman run --it --rm --entrypoint /usr/local/bin/xcfview   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/xcfview   -v ${PWD} -w ${PWD} <container> -c " $@"
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