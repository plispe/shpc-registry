---
layout: container
name:  "quay.io/biocontainers/bcalm"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bcalm/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bcalm/container.yaml"
updated_at: "2023-01-13 03:14:26.425265"
latest: "2.2.3--h5b5514e_3"
container_url: "https://biocontainers.pro/tools/bcalm"
aliases:
 - "bcalm"
 - "h5cc"
versions:
 - "2.2.3--h5b5514e_3"
description: "shpc-registry automated BioContainers addition for bcalm"
config: {"url": "https://biocontainers.pro/tools/bcalm", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bcalm", "latest": {"2.2.3--h5b5514e_3": "sha256:4259eb31aeb9f935607e54fe490f53e864810dea412b11c6369b18f132e4c87b"}, "tags": {"2.2.3--h5b5514e_3": "sha256:4259eb31aeb9f935607e54fe490f53e864810dea412b11c6369b18f132e4c87b"}, "docker": "quay.io/biocontainers/bcalm", "aliases": {"bcalm": "/usr/local/bin/bcalm", "h5cc": "/usr/local/bin/h5cc"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bcalm.
shpc-registry automated BioContainers addition for bcalm
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bcalm
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bcalm:2.2.3--h5b5514e_3
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bcalm/2.2.3--h5b5514e_3
$ module help quay.io/biocontainers/bcalm/2.2.3--h5b5514e_3
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bcalm-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bcalm-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bcalm-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bcalm-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bcalm-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bcalm-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### bcalm

```bash
$ singularity exec <container> /usr/local/bin/bcalm
$ podman run --it --rm --entrypoint /usr/local/bin/bcalm   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/bcalm   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### h5cc

```bash
$ singularity exec <container> /usr/local/bin/h5cc
$ podman run --it --rm --entrypoint /usr/local/bin/h5cc   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/h5cc   -v ${PWD} -w ${PWD} <container> -c " $@"
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