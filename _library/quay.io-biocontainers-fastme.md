---
layout: container
name:  "quay.io/biocontainers/fastme"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/fastme/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/fastme/container.yaml"
updated_at: "2023-01-13 02:59:35.522967"
latest: "2.1.6.1--hec16e2b_1"
container_url: "https://biocontainers.pro/tools/fastme"
aliases:
 - "fastme"
versions:
 - "2.1.6.1--hec16e2b_1"
description: "shpc-registry automated BioContainers addition for fastme"
config: {"url": "https://biocontainers.pro/tools/fastme", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for fastme", "latest": {"2.1.6.1--hec16e2b_1": "sha256:c8d8a3ec03c7fb87f9dc0bd79bbca11dc409588d9f9e32d5fb9c9bad38e9df39"}, "tags": {"2.1.6.1--hec16e2b_1": "sha256:c8d8a3ec03c7fb87f9dc0bd79bbca11dc409588d9f9e32d5fb9c9bad38e9df39"}, "docker": "quay.io/biocontainers/fastme", "aliases": {"fastme": "/usr/local/bin/fastme"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/fastme.
shpc-registry automated BioContainers addition for fastme
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/fastme
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/fastme:2.1.6.1--hec16e2b_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/fastme/2.1.6.1--hec16e2b_1
$ module help quay.io/biocontainers/fastme/2.1.6.1--hec16e2b_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### fastme-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### fastme-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### fastme-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### fastme-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### fastme-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### fastme-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### fastme

```bash
$ singularity exec <container> /usr/local/bin/fastme
$ podman run --it --rm --entrypoint /usr/local/bin/fastme   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/fastme   -v ${PWD} -w ${PWD} <container> -c " $@"
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