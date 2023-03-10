---
layout: container
name:  "quay.io/biocontainers/pbsim2"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/pbsim2/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/pbsim2/container.yaml"
updated_at: "2023-01-13 03:43:14.740069"
latest: "2.0.1--h9f5acd7_1"
container_url: "https://biocontainers.pro/tools/pbsim2"
aliases:
 - "pbsim"
versions:
 - "2.0.1--h9f5acd7_1"
description: "shpc-registry automated BioContainers addition for pbsim2"
config: {"url": "https://biocontainers.pro/tools/pbsim2", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for pbsim2", "latest": {"2.0.1--h9f5acd7_1": "sha256:49018554d0a1bd2a553a9aac5d543fdf6f066264ba291e4b7d3251a01fcdd458"}, "tags": {"2.0.1--h9f5acd7_1": "sha256:49018554d0a1bd2a553a9aac5d543fdf6f066264ba291e4b7d3251a01fcdd458"}, "docker": "quay.io/biocontainers/pbsim2", "aliases": {"pbsim": "/usr/local/bin/pbsim"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/pbsim2.
shpc-registry automated BioContainers addition for pbsim2
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/pbsim2
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/pbsim2:2.0.1--h9f5acd7_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/pbsim2/2.0.1--h9f5acd7_1
$ module help quay.io/biocontainers/pbsim2/2.0.1--h9f5acd7_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### pbsim2-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### pbsim2-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### pbsim2-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### pbsim2-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### pbsim2-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### pbsim2-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### pbsim

```bash
$ singularity exec <container> /usr/local/bin/pbsim
$ podman run --it --rm --entrypoint /usr/local/bin/pbsim   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pbsim   -v ${PWD} -w ${PWD} <container> -c " $@"
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