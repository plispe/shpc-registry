---
layout: container
name:  "quay.io/biocontainers/r-coenocliner"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/r-coenocliner/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/r-coenocliner/container.yaml"
updated_at: "2023-01-13 03:03:07.370833"
latest: "0.2_2--r351h6115d3f_2"
container_url: "https://biocontainers.pro/tools/r-coenocliner"
aliases:
 - "c89"
 - "c99"
versions:
 - "0.2_2--r351h6115d3f_2"
description: "shpc-registry automated BioContainers addition for r-coenocliner"
config: {"url": "https://biocontainers.pro/tools/r-coenocliner", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for r-coenocliner", "latest": {"0.2_2--r351h6115d3f_2": "sha256:58e0abcc20522c7e070121fd8c433b63914cb55a63123f655b14cc4e85370024"}, "tags": {"0.2_2--r351h6115d3f_2": "sha256:58e0abcc20522c7e070121fd8c433b63914cb55a63123f655b14cc4e85370024"}, "docker": "quay.io/biocontainers/r-coenocliner", "aliases": {"c89": "/usr/local/bin/c89", "c99": "/usr/local/bin/c99"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/r-coenocliner.
shpc-registry automated BioContainers addition for r-coenocliner
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/r-coenocliner
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/r-coenocliner:0.2_2--r351h6115d3f_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/r-coenocliner/0.2_2--r351h6115d3f_2
$ module help quay.io/biocontainers/r-coenocliner/0.2_2--r351h6115d3f_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### r-coenocliner-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### r-coenocliner-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### r-coenocliner-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### r-coenocliner-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### r-coenocliner-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### r-coenocliner-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### c89

```bash
$ singularity exec <container> /usr/local/bin/c89
$ podman run --it --rm --entrypoint /usr/local/bin/c89   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/c89   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### c99

```bash
$ singularity exec <container> /usr/local/bin/c99
$ podman run --it --rm --entrypoint /usr/local/bin/c99   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/c99   -v ${PWD} -w ${PWD} <container> -c " $@"
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