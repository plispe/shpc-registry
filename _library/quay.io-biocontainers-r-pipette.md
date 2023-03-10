---
layout: container
name:  "quay.io/biocontainers/r-pipette"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/r-pipette/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/r-pipette/container.yaml"
updated_at: "2023-01-13 02:51:11.757259"
latest: "0.10.1--r42hdfd78af_1"
container_url: "https://biocontainers.pro/tools/r-pipette"

versions:
 - "0.8.0--r41hdfd78af_0"
 - "0.10.1--r42hdfd78af_1"
 - "0.8.0--r41hdfd78af_1"
description: "shpc-registry automated BioContainers addition for r-pipette"
config: {"url": "https://biocontainers.pro/tools/r-pipette", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for r-pipette", "latest": {"0.10.1--r42hdfd78af_1": "sha256:6a9cf12053e3e28412e519dfee8562db04ea2fadf522354a4332b10a2c6ce596"}, "tags": {"0.8.0--r41hdfd78af_0": "sha256:5ac1750a3fdd6f03d7b8b54ab314e91e1c5b5a9c5324a21cecc549e83969f0f2", "0.10.1--r42hdfd78af_1": "sha256:6a9cf12053e3e28412e519dfee8562db04ea2fadf522354a4332b10a2c6ce596", "0.8.0--r41hdfd78af_1": "sha256:92ce019b66d0b33c0732e6aba0718709e208e8d61557d08a80a8df66477b44ea"}, "docker": "quay.io/biocontainers/r-pipette"}
---

This module is a singularity container wrapper for quay.io/biocontainers/r-pipette.
shpc-registry automated BioContainers addition for r-pipette
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/r-pipette
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/r-pipette:0.10.1--r42hdfd78af_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/r-pipette/0.10.1--r42hdfd78af_1
$ module help quay.io/biocontainers/r-pipette/0.10.1--r42hdfd78af_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### r-pipette-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### r-pipette-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### r-pipette-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### r-pipette-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### r-pipette-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### r-pipette-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### r-pipette

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