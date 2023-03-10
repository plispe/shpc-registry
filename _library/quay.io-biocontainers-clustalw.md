---
layout: container
name:  "quay.io/biocontainers/clustalw"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/clustalw/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/clustalw/container.yaml"
updated_at: "2023-01-13 02:55:05.554086"
latest: "2.1--h9f5acd7_7"
container_url: "https://biocontainers.pro/tools/clustalw"
aliases:
 - "clustalw"
 - "clustalw2"
versions:
 - "2.1--h9f5acd7_7"
description: "shpc-registry automated BioContainers addition for clustalw"
config: {"url": "https://biocontainers.pro/tools/clustalw", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for clustalw", "latest": {"2.1--h9f5acd7_7": "sha256:b6a0bd2d397078fa1a35d7f4cef68a75ea953dbaa101781c48cdebc3994c4972"}, "tags": {"2.1--h9f5acd7_7": "sha256:b6a0bd2d397078fa1a35d7f4cef68a75ea953dbaa101781c48cdebc3994c4972"}, "docker": "quay.io/biocontainers/clustalw", "aliases": {"clustalw": "/usr/local/bin/clustalw", "clustalw2": "/usr/local/bin/clustalw2"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/clustalw.
shpc-registry automated BioContainers addition for clustalw
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/clustalw
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/clustalw:2.1--h9f5acd7_7
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/clustalw/2.1--h9f5acd7_7
$ module help quay.io/biocontainers/clustalw/2.1--h9f5acd7_7
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### clustalw-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### clustalw-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### clustalw-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### clustalw-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### clustalw-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### clustalw-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### clustalw

```bash
$ singularity exec <container> /usr/local/bin/clustalw
$ podman run --it --rm --entrypoint /usr/local/bin/clustalw   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/clustalw   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### clustalw2

```bash
$ singularity exec <container> /usr/local/bin/clustalw2
$ podman run --it --rm --entrypoint /usr/local/bin/clustalw2   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/clustalw2   -v ${PWD} -w ${PWD} <container> -c " $@"
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