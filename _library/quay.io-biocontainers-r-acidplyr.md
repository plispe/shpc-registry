---
layout: container
name:  "quay.io/biocontainers/r-acidplyr"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/r-acidplyr/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/r-acidplyr/container.yaml"
updated_at: "2023-01-13 02:52:56.634855"
latest: "0.3.2--r42hdfd78af_1"
container_url: "https://biocontainers.pro/tools/r-acidplyr"

versions:
 - "0.2.0--r41hdfd78af_0"
 - "0.2.0--r41hdfd78af_1"
 - "0.3.2--r42hdfd78af_1"
description: "shpc-registry automated BioContainers addition for r-acidplyr"
config: {"url": "https://biocontainers.pro/tools/r-acidplyr", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for r-acidplyr", "latest": {"0.3.2--r42hdfd78af_1": "sha256:34643d02cad183deda70e12255bc25b5ae54be1eceb4d2261e43fd9c15a9e8dc"}, "tags": {"0.2.0--r41hdfd78af_0": "sha256:3d3d96c8325669aa2724e505f174ed2e4aa957c6e0ef174d6289b1b7c8b52cd1", "0.2.0--r41hdfd78af_1": "sha256:c9c8ad610a9cc354fa3cfb93b0a46623d6d7431b1113ce6fe5d6507b20b88c50", "0.3.2--r42hdfd78af_1": "sha256:34643d02cad183deda70e12255bc25b5ae54be1eceb4d2261e43fd9c15a9e8dc"}, "docker": "quay.io/biocontainers/r-acidplyr"}
---

This module is a singularity container wrapper for quay.io/biocontainers/r-acidplyr.
shpc-registry automated BioContainers addition for r-acidplyr
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/r-acidplyr
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/r-acidplyr:0.3.2--r42hdfd78af_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/r-acidplyr/0.3.2--r42hdfd78af_1
$ module help quay.io/biocontainers/r-acidplyr/0.3.2--r42hdfd78af_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### r-acidplyr-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### r-acidplyr-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### r-acidplyr-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### r-acidplyr-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### r-acidplyr-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### r-acidplyr-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### r-acidplyr

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