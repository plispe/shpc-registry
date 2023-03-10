---
layout: container
name:  "quay.io/biocontainers/bioconductor-fabia"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-fabia/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-fabia/container.yaml"
updated_at: "2023-01-13 03:00:11.742115"
latest: "2.44.0--r42hc0cfd56_0"
container_url: "https://biocontainers.pro/tools/bioconductor-fabia"

versions:
 - "2.40.0--r41hc0cfd56_2"
 - "2.44.0--r42hc0cfd56_0"
description: "shpc-registry automated BioContainers addition for bioconductor-fabia"
config: {"url": "https://biocontainers.pro/tools/bioconductor-fabia", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-fabia", "latest": {"2.44.0--r42hc0cfd56_0": "sha256:e6b763536d2dafabad12d4c848257348a8e92eabd90f8db67aac6a804924e826"}, "tags": {"2.40.0--r41hc0cfd56_2": "sha256:44b7c08f1dedd7567d6353bd0865a882d5470b490a431d0f03db116a9d7c14fa", "2.44.0--r42hc0cfd56_0": "sha256:e6b763536d2dafabad12d4c848257348a8e92eabd90f8db67aac6a804924e826"}, "docker": "quay.io/biocontainers/bioconductor-fabia"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-fabia.
shpc-registry automated BioContainers addition for bioconductor-fabia
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-fabia
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-fabia:2.44.0--r42hc0cfd56_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-fabia/2.44.0--r42hc0cfd56_0
$ module help quay.io/biocontainers/bioconductor-fabia/2.44.0--r42hc0cfd56_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-fabia-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-fabia-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-fabia-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-fabia-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-fabia-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-fabia-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-fabia

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