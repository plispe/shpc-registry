---
layout: container
name:  "quay.io/biocontainers/bioconductor-made4"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-made4/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-made4/container.yaml"
updated_at: "2023-01-13 03:20:06.119103"
latest: "1.72.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-made4"

versions:
 - "1.68.0--r41hdfd78af_0"
 - "1.72.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-made4"
config: {"url": "https://biocontainers.pro/tools/bioconductor-made4", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-made4", "latest": {"1.72.0--r42hdfd78af_0": "sha256:c1e505659c7f1d8546bc01339243ef81e4a6af2bdb0a27b5af5018b079cbc79a"}, "tags": {"1.68.0--r41hdfd78af_0": "sha256:25211e7238c48cb27d01bb748bf94fb5c9e888d29df183d376acbe7c6271961d", "1.72.0--r42hdfd78af_0": "sha256:c1e505659c7f1d8546bc01339243ef81e4a6af2bdb0a27b5af5018b079cbc79a"}, "docker": "quay.io/biocontainers/bioconductor-made4"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-made4.
shpc-registry automated BioContainers addition for bioconductor-made4
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-made4
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-made4:1.72.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-made4/1.72.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-made4/1.72.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-made4-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-made4-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-made4-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-made4-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-made4-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-made4-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-made4

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