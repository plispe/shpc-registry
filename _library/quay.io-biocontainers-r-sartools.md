---
layout: container
name:  "quay.io/biocontainers/r-sartools"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/r-sartools/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/r-sartools/container.yaml"
updated_at: "2022-11-20 01:02:48.288167"
latest: "1.8.1--r41hdfd78af_0"
container_url: "https://biocontainers.pro/tools/r-sartools"
aliases:
 - "pandoc"
versions:
 - "1.8.1--r41hdfd78af_0"
description: "shpc-registry automated BioContainers addition for r-sartools"
config: {"url": "https://biocontainers.pro/tools/r-sartools", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for r-sartools", "latest": {"1.8.1--r41hdfd78af_0": "sha256:4ba629e9bc716be475498dec39aa0eff4482bc28029cb3bbeeebffc3a7b55e57"}, "tags": {"1.8.1--r41hdfd78af_0": "sha256:4ba629e9bc716be475498dec39aa0eff4482bc28029cb3bbeeebffc3a7b55e57"}, "docker": "quay.io/biocontainers/r-sartools", "aliases": {"pandoc": "/usr/local/bin/pandoc"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/r-sartools.
shpc-registry automated BioContainers addition for r-sartools
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/r-sartools
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/r-sartools:1.8.1--r41hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/r-sartools/1.8.1--r41hdfd78af_0
$ module help quay.io/biocontainers/r-sartools/1.8.1--r41hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### r-sartools-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### r-sartools-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### r-sartools-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### r-sartools-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### r-sartools-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### r-sartools-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### pandoc

```bash
$ singularity exec <container> /usr/local/bin/pandoc
$ podman run --it --rm --entrypoint /usr/local/bin/pandoc   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pandoc   -v ${PWD} -w ${PWD} <container> -c " $@"
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