---
layout: container
name:  "quay.io/biocontainers/real"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/real/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/real/container.yaml"
updated_at: "2023-01-13 03:24:08.019973"
latest: "1.0--he941832_1"
container_url: "https://biocontainers.pro/tools/real"
aliases:
 - "real"
versions:
 - "1.0--he941832_1"
description: "shpc-registry automated BioContainers addition for real"
config: {"url": "https://biocontainers.pro/tools/real", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for real", "latest": {"1.0--he941832_1": "sha256:c920674b2d4585707b038124415b46b0c535eedbc5fe75b23df3693ad7bf5e1f"}, "tags": {"1.0--he941832_1": "sha256:c920674b2d4585707b038124415b46b0c535eedbc5fe75b23df3693ad7bf5e1f"}, "docker": "quay.io/biocontainers/real", "aliases": {"real": "/usr/local/bin/real"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/real.
shpc-registry automated BioContainers addition for real
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/real
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/real:1.0--he941832_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/real/1.0--he941832_1
$ module help quay.io/biocontainers/real/1.0--he941832_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### real-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### real-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### real-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### real-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### real-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### real-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### real

```bash
$ singularity exec <container> /usr/local/bin/real
$ podman run --it --rm --entrypoint /usr/local/bin/real   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/real   -v ${PWD} -w ${PWD} <container> -c " $@"
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