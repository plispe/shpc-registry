---
layout: container
name:  "quay.io/biocontainers/smafa"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/smafa/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/smafa/container.yaml"
updated_at: "2023-01-13 03:28:10.970411"
latest: "0.5.0--hec16e2b_2"
container_url: "https://biocontainers.pro/tools/smafa"
aliases:
 - "smafa"
versions:
 - "0.5.0--hec16e2b_2"
description: "shpc-registry automated BioContainers addition for smafa"
config: {"url": "https://biocontainers.pro/tools/smafa", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for smafa", "latest": {"0.5.0--hec16e2b_2": "sha256:bfab3052298105cd88386083a2cca6b77dba01f1f0768276a8ab87f0941b4c12"}, "tags": {"0.5.0--hec16e2b_2": "sha256:bfab3052298105cd88386083a2cca6b77dba01f1f0768276a8ab87f0941b4c12"}, "docker": "quay.io/biocontainers/smafa", "aliases": {"smafa": "/usr/local/bin/smafa"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/smafa.
shpc-registry automated BioContainers addition for smafa
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/smafa
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/smafa:0.5.0--hec16e2b_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/smafa/0.5.0--hec16e2b_2
$ module help quay.io/biocontainers/smafa/0.5.0--hec16e2b_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### smafa-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### smafa-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### smafa-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### smafa-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### smafa-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### smafa-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### smafa

```bash
$ singularity exec <container> /usr/local/bin/smafa
$ podman run --it --rm --entrypoint /usr/local/bin/smafa   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/smafa   -v ${PWD} -w ${PWD} <container> -c " $@"
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