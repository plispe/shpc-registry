---
layout: container
name:  "quay.io/biocontainers/bioconductor-jaspar2014"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-jaspar2014/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-jaspar2014/container.yaml"
updated_at: "2023-01-13 03:25:18.097384"
latest: "1.34.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-jaspar2014"

versions:
 - "1.30.0--r41hdfd78af_1"
 - "1.34.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-jaspar2014"
config: {"url": "https://biocontainers.pro/tools/bioconductor-jaspar2014", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-jaspar2014", "latest": {"1.34.0--r42hdfd78af_0": "sha256:b75a6093e10f072e01b35ee0a331a83669b5475c5297a695fe0605f7215173b4"}, "tags": {"1.30.0--r41hdfd78af_1": "sha256:a5e209270387a937cd3aa2c9334264607d912f140768604b1fd69a5dbf2aed64", "1.34.0--r42hdfd78af_0": "sha256:b75a6093e10f072e01b35ee0a331a83669b5475c5297a695fe0605f7215173b4"}, "docker": "quay.io/biocontainers/bioconductor-jaspar2014"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-jaspar2014.
shpc-registry automated BioContainers addition for bioconductor-jaspar2014
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-jaspar2014
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-jaspar2014:1.34.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-jaspar2014/1.34.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-jaspar2014/1.34.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-jaspar2014-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-jaspar2014-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-jaspar2014-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-jaspar2014-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-jaspar2014-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-jaspar2014-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-jaspar2014

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