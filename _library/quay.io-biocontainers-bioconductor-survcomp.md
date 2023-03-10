---
layout: container
name:  "quay.io/biocontainers/bioconductor-survcomp"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-survcomp/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-survcomp/container.yaml"
updated_at: "2023-01-13 03:22:10.814646"
latest: "1.48.0--r42hc247a5b_0"
container_url: "https://biocontainers.pro/tools/bioconductor-survcomp"

versions:
 - "1.44.1--r41hc247a5b_1"
 - "1.48.0--r42hc247a5b_0"
description: "shpc-registry automated BioContainers addition for bioconductor-survcomp"
config: {"url": "https://biocontainers.pro/tools/bioconductor-survcomp", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-survcomp", "latest": {"1.48.0--r42hc247a5b_0": "sha256:1ffde0b01b75af513d8b94738832570fc8253f53b5a22afe9540fb16bbc5c66d"}, "tags": {"1.44.1--r41hc247a5b_1": "sha256:7e9b331f948570c8fe5498279f2f2456342c2a8e7b55aa7d4707e52516497017", "1.48.0--r42hc247a5b_0": "sha256:1ffde0b01b75af513d8b94738832570fc8253f53b5a22afe9540fb16bbc5c66d"}, "docker": "quay.io/biocontainers/bioconductor-survcomp"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-survcomp.
shpc-registry automated BioContainers addition for bioconductor-survcomp
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-survcomp
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-survcomp:1.48.0--r42hc247a5b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-survcomp/1.48.0--r42hc247a5b_0
$ module help quay.io/biocontainers/bioconductor-survcomp/1.48.0--r42hc247a5b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-survcomp-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-survcomp-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-survcomp-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-survcomp-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-survcomp-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-survcomp-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-survcomp

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