---
layout: container
name:  "quay.io/biocontainers/ocrad"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/ocrad/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/ocrad/container.yaml"
updated_at: "2023-01-13 02:56:11.282213"
latest: "0.21--h470a237_1"
container_url: "https://biocontainers.pro/tools/ocrad"
aliases:
 - "ocrad"
versions:
 - "0.21--h470a237_1"
description: "shpc-registry automated BioContainers addition for ocrad"
config: {"url": "https://biocontainers.pro/tools/ocrad", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for ocrad", "latest": {"0.21--h470a237_1": "sha256:01f099c2bb4c87d487fcd2d18167d64fe8b55f0939d276933ca5be5be2e68314"}, "tags": {"0.21--h470a237_1": "sha256:01f099c2bb4c87d487fcd2d18167d64fe8b55f0939d276933ca5be5be2e68314"}, "docker": "quay.io/biocontainers/ocrad", "aliases": {"ocrad": "/usr/local/bin/ocrad"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/ocrad.
shpc-registry automated BioContainers addition for ocrad
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/ocrad
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/ocrad:0.21--h470a237_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/ocrad/0.21--h470a237_1
$ module help quay.io/biocontainers/ocrad/0.21--h470a237_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### ocrad-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### ocrad-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### ocrad-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### ocrad-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### ocrad-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### ocrad-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### ocrad

```bash
$ singularity exec <container> /usr/local/bin/ocrad
$ podman run --it --rm --entrypoint /usr/local/bin/ocrad   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/ocrad   -v ${PWD} -w ${PWD} <container> -c " $@"
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