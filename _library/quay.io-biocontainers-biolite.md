---
layout: container
name:  "quay.io/biocontainers/biolite"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/biolite/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/biolite/container.yaml"
updated_at: "2023-01-13 03:24:27.070672"
latest: "1.2.0--py27_0"
container_url: "https://biocontainers.pro/tools/biolite"

versions:
 - "1.2.0--py27_0"
description: "shpc-registry automated BioContainers addition for biolite"
config: {"url": "https://biocontainers.pro/tools/biolite", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for biolite", "latest": {"1.2.0--py27_0": "sha256:17c0d9b5f4490122f7a910290af275f3ad87050ca5b2077b6a9933e410e706e0"}, "tags": {"1.2.0--py27_0": "sha256:17c0d9b5f4490122f7a910290af275f3ad87050ca5b2077b6a9933e410e706e0"}, "docker": "quay.io/biocontainers/biolite"}
---

This module is a singularity container wrapper for quay.io/biocontainers/biolite.
shpc-registry automated BioContainers addition for biolite
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/biolite
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/biolite:1.2.0--py27_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/biolite/1.2.0--py27_0
$ module help quay.io/biocontainers/biolite/1.2.0--py27_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### biolite-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### biolite-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### biolite-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### biolite-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### biolite-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### biolite-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### biolite

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