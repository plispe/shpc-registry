---
layout: container
name:  "quay.io/biocontainers/bayestyper"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bayestyper/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bayestyper/container.yaml"
updated_at: "2023-01-13 03:01:06.645606"
latest: "1.5--h176a8bc_0"
container_url: "https://biocontainers.pro/tools/bayestyper"
aliases:
 - "bayesTyper"
 - "bayesTyperTools"
versions:
 - "1.5--h176a8bc_0"
description: "shpc-registry automated BioContainers addition for bayestyper"
config: {"url": "https://biocontainers.pro/tools/bayestyper", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bayestyper", "latest": {"1.5--h176a8bc_0": "sha256:370d1f8a36cbc9ec5114852d834dd60037b74f3b3ab09c58ccecea0197cfd4f0"}, "tags": {"1.5--h176a8bc_0": "sha256:370d1f8a36cbc9ec5114852d834dd60037b74f3b3ab09c58ccecea0197cfd4f0"}, "docker": "quay.io/biocontainers/bayestyper", "aliases": {"bayesTyper": "/usr/local/bin/bayesTyper", "bayesTyperTools": "/usr/local/bin/bayesTyperTools"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bayestyper.
shpc-registry automated BioContainers addition for bayestyper
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bayestyper
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bayestyper:1.5--h176a8bc_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bayestyper/1.5--h176a8bc_0
$ module help quay.io/biocontainers/bayestyper/1.5--h176a8bc_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bayestyper-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bayestyper-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bayestyper-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bayestyper-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bayestyper-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bayestyper-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### bayesTyper

```bash
$ singularity exec <container> /usr/local/bin/bayesTyper
$ podman run --it --rm --entrypoint /usr/local/bin/bayesTyper   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/bayesTyper   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### bayesTyperTools

```bash
$ singularity exec <container> /usr/local/bin/bayesTyperTools
$ podman run --it --rm --entrypoint /usr/local/bin/bayesTyperTools   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/bayesTyperTools   -v ${PWD} -w ${PWD} <container> -c " $@"
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