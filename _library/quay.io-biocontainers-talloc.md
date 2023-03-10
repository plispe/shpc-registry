---
layout: container
name:  "quay.io/biocontainers/talloc"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/talloc/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/talloc/container.yaml"
updated_at: "2023-01-13 03:06:16.984045"
latest: "2.1.9--0"
container_url: "https://biocontainers.pro/tools/talloc"

versions:
 - "2.1.9--0"
description: "shpc-registry automated BioContainers addition for talloc"
config: {"url": "https://biocontainers.pro/tools/talloc", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for talloc", "latest": {"2.1.9--0": "sha256:55187548fd8f8a225bef01b8352871a2af2159409e2ed0f4051a53a9cdba4fcf"}, "tags": {"2.1.9--0": "sha256:55187548fd8f8a225bef01b8352871a2af2159409e2ed0f4051a53a9cdba4fcf"}, "docker": "quay.io/biocontainers/talloc"}
---

This module is a singularity container wrapper for quay.io/biocontainers/talloc.
shpc-registry automated BioContainers addition for talloc
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/talloc
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/talloc:2.1.9--0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/talloc/2.1.9--0
$ module help quay.io/biocontainers/talloc/2.1.9--0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### talloc-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### talloc-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### talloc-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### talloc-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### talloc-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### talloc-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### talloc

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