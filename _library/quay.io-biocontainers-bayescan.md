---
layout: container
name:  "quay.io/biocontainers/bayescan"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bayescan/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bayescan/container.yaml"
updated_at: "2023-01-13 03:36:40.966351"
latest: "2.0.1--h9f5acd7_4"
container_url: "https://biocontainers.pro/tools/bayescan"
aliases:
 - "bayescan2"
versions:
 - "2.0.1--h9f5acd7_4"
description: "shpc-registry automated BioContainers addition for bayescan"
config: {"url": "https://biocontainers.pro/tools/bayescan", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bayescan", "latest": {"2.0.1--h9f5acd7_4": "sha256:eb0c8ff2758b2cc408436b45b88cdcaed3e6b5a2d070528f5b58af60ed9da0cb"}, "tags": {"2.0.1--h9f5acd7_4": "sha256:eb0c8ff2758b2cc408436b45b88cdcaed3e6b5a2d070528f5b58af60ed9da0cb"}, "docker": "quay.io/biocontainers/bayescan", "aliases": {"bayescan2": "/usr/local/bin/bayescan2"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bayescan.
shpc-registry automated BioContainers addition for bayescan
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bayescan
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bayescan:2.0.1--h9f5acd7_4
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bayescan/2.0.1--h9f5acd7_4
$ module help quay.io/biocontainers/bayescan/2.0.1--h9f5acd7_4
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bayescan-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bayescan-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bayescan-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bayescan-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bayescan-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bayescan-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### bayescan2

```bash
$ singularity exec <container> /usr/local/bin/bayescan2
$ podman run --it --rm --entrypoint /usr/local/bin/bayescan2   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/bayescan2   -v ${PWD} -w ${PWD} <container> -c " $@"
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