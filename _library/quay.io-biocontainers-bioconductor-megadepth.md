---
layout: container
name:  "quay.io/biocontainers/bioconductor-megadepth"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-megadepth/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-megadepth/container.yaml"
updated_at: "2023-01-13 03:27:09.030219"
latest: "1.8.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-megadepth"

versions:
 - "1.4.0--r41hdfd78af_0"
 - "1.8.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-megadepth"
config: {"url": "https://biocontainers.pro/tools/bioconductor-megadepth", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-megadepth", "latest": {"1.8.0--r42hdfd78af_0": "sha256:8c7cef912305ebaa2e69c419f4d1664f5e307a052f45245dff75bebf343e421d"}, "tags": {"1.4.0--r41hdfd78af_0": "sha256:41b0c42750ccdbd3359d17ab7a3c5d98b145223cead3596102bf58645591c893", "1.8.0--r42hdfd78af_0": "sha256:8c7cef912305ebaa2e69c419f4d1664f5e307a052f45245dff75bebf343e421d"}, "docker": "quay.io/biocontainers/bioconductor-megadepth"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-megadepth.
shpc-registry automated BioContainers addition for bioconductor-megadepth
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-megadepth
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-megadepth:1.8.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-megadepth/1.8.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-megadepth/1.8.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-megadepth-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-megadepth-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-megadepth-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-megadepth-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-megadepth-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-megadepth-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-megadepth

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