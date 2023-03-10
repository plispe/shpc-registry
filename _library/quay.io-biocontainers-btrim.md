---
layout: container
name:  "quay.io/biocontainers/btrim"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/btrim/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/btrim/container.yaml"
updated_at: "2023-01-13 03:31:59.946354"
latest: "1.0.1--h9f5acd7_4"
container_url: "https://biocontainers.pro/tools/btrim"
aliases:
 - "btrim"
versions:
 - "1.0.1--h9f5acd7_4"
description: "shpc-registry automated BioContainers addition for btrim"
config: {"url": "https://biocontainers.pro/tools/btrim", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for btrim", "latest": {"1.0.1--h9f5acd7_4": "sha256:97287a335ce891434e0dc38cc940c3f33f6365f1a6a1bc6c909b503a4b58b9fa"}, "tags": {"1.0.1--h9f5acd7_4": "sha256:97287a335ce891434e0dc38cc940c3f33f6365f1a6a1bc6c909b503a4b58b9fa"}, "docker": "quay.io/biocontainers/btrim", "aliases": {"btrim": "/usr/local/bin/btrim"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/btrim.
shpc-registry automated BioContainers addition for btrim
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/btrim
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/btrim:1.0.1--h9f5acd7_4
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/btrim/1.0.1--h9f5acd7_4
$ module help quay.io/biocontainers/btrim/1.0.1--h9f5acd7_4
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### btrim-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### btrim-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### btrim-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### btrim-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### btrim-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### btrim-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### btrim

```bash
$ singularity exec <container> /usr/local/bin/btrim
$ podman run --it --rm --entrypoint /usr/local/bin/btrim   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/btrim   -v ${PWD} -w ${PWD} <container> -c " $@"
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