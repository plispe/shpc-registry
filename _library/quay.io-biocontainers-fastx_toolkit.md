---
layout: container
name:  "quay.io/biocontainers/fastx_toolkit"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/fastx_toolkit/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/fastx_toolkit/container.yaml"
updated_at: "2023-01-13 02:48:48.846015"
latest: "0.0.14--h87f3376_10"
container_url: "https://biocontainers.pro/tools/fastx_toolkit"

versions:
 - "0.0.14--he1b5a44_8"
 - "0.0.14--h87f3376_10"
description: "shpc-registry automated BioContainers addition for fastx_toolkit"
config: {"url": "https://biocontainers.pro/tools/fastx_toolkit", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for fastx_toolkit", "latest": {"0.0.14--h87f3376_10": "sha256:ce4316e55413966f2dd1993936b86dbd488ba6f17c9044eefd2fa2e41f220a70"}, "tags": {"0.0.14--he1b5a44_8": "sha256:8ac88163b78821a449c1fec672e9b9cf9c4993c18d067a9afa0a8769a5e3f607", "0.0.14--h87f3376_10": "sha256:ce4316e55413966f2dd1993936b86dbd488ba6f17c9044eefd2fa2e41f220a70"}, "docker": "quay.io/biocontainers/fastx_toolkit"}
---

This module is a singularity container wrapper for quay.io/biocontainers/fastx_toolkit.
shpc-registry automated BioContainers addition for fastx_toolkit
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/fastx_toolkit
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/fastx_toolkit:0.0.14--h87f3376_10
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/fastx_toolkit/0.0.14--h87f3376_10
$ module help quay.io/biocontainers/fastx_toolkit/0.0.14--h87f3376_10
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### fastx_toolkit-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### fastx_toolkit-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### fastx_toolkit-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### fastx_toolkit-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### fastx_toolkit-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### fastx_toolkit-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### fastx_toolkit

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