---
layout: container
name:  "quay.io/biocontainers/archer"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/archer/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/archer/container.yaml"
updated_at: "2023-01-13 03:44:54.196678"
latest: "0.1.1--he881be0_0"
container_url: "https://biocontainers.pro/tools/archer"
aliases:
 - "archer"
versions:
 - "0.1.1--he881be0_0"
description: "shpc-registry automated BioContainers addition for archer"
config: {"url": "https://biocontainers.pro/tools/archer", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for archer", "latest": {"0.1.1--he881be0_0": "sha256:c0492839a938f5581c79409cf339c781dfb112f32b438eb89b17a5860d0c810a"}, "tags": {"0.1.1--he881be0_0": "sha256:c0492839a938f5581c79409cf339c781dfb112f32b438eb89b17a5860d0c810a"}, "docker": "quay.io/biocontainers/archer", "aliases": {"archer": "/usr/local/bin/archer"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/archer.
shpc-registry automated BioContainers addition for archer
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/archer
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/archer:0.1.1--he881be0_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/archer/0.1.1--he881be0_0
$ module help quay.io/biocontainers/archer/0.1.1--he881be0_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### archer-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### archer-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### archer-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### archer-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### archer-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### archer-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### archer

```bash
$ singularity exec <container> /usr/local/bin/archer
$ podman run --it --rm --entrypoint /usr/local/bin/archer   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/archer   -v ${PWD} -w ${PWD} <container> -c " $@"
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