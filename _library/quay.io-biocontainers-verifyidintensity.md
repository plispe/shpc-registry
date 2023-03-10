---
layout: container
name:  "quay.io/biocontainers/verifyidintensity"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/verifyidintensity/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/verifyidintensity/container.yaml"
updated_at: "2023-01-13 03:18:36.470907"
latest: "0.0.1--h7ff8a90_2"
container_url: "https://biocontainers.pro/tools/verifyidintensity"
aliases:
 - "verifyIDintensity"
versions:
 - "0.0.1--h7ff8a90_2"
description: "shpc-registry automated BioContainers addition for verifyidintensity"
config: {"url": "https://biocontainers.pro/tools/verifyidintensity", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for verifyidintensity", "latest": {"0.0.1--h7ff8a90_2": "sha256:bd0fd29d2513849dc3d258d99ac25235672c7be4fd49f89410cf8441a3833c65"}, "tags": {"0.0.1--h7ff8a90_2": "sha256:bd0fd29d2513849dc3d258d99ac25235672c7be4fd49f89410cf8441a3833c65"}, "docker": "quay.io/biocontainers/verifyidintensity", "aliases": {"verifyIDintensity": "/usr/local/bin/verifyIDintensity"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/verifyidintensity.
shpc-registry automated BioContainers addition for verifyidintensity
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/verifyidintensity
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/verifyidintensity:0.0.1--h7ff8a90_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/verifyidintensity/0.0.1--h7ff8a90_2
$ module help quay.io/biocontainers/verifyidintensity/0.0.1--h7ff8a90_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### verifyidintensity-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### verifyidintensity-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### verifyidintensity-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### verifyidintensity-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### verifyidintensity-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### verifyidintensity-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### verifyIDintensity

```bash
$ singularity exec <container> /usr/local/bin/verifyIDintensity
$ podman run --it --rm --entrypoint /usr/local/bin/verifyIDintensity   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/verifyIDintensity   -v ${PWD} -w ${PWD} <container> -c " $@"
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