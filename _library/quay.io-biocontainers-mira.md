---
layout: container
name:  "quay.io/biocontainers/mira"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/mira/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/mira/container.yaml"
updated_at: "2023-01-13 03:06:10.045046"
latest: "4.9.6--1"
container_url: "https://biocontainers.pro/tools/mira"
aliases:
 - "mira"
 - "mira-install-sls-rrna.sh"
 - "mirabait"
 - "miraconvert"
 - "miramem"
versions:
 - "4.9.6--1"
description: "shpc-registry automated BioContainers addition for mira"
config: {"url": "https://biocontainers.pro/tools/mira", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for mira", "latest": {"4.9.6--1": "sha256:f4c88e806e307861cf65f5d3bbbf5056007838540dc3647a3850579d95984c18"}, "tags": {"4.9.6--1": "sha256:f4c88e806e307861cf65f5d3bbbf5056007838540dc3647a3850579d95984c18"}, "docker": "quay.io/biocontainers/mira", "aliases": {"mira": "/usr/local/bin/mira", "mira-install-sls-rrna.sh": "/usr/local/bin/mira-install-sls-rrna.sh", "mirabait": "/usr/local/bin/mirabait", "miraconvert": "/usr/local/bin/miraconvert", "miramem": "/usr/local/bin/miramem"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/mira.
shpc-registry automated BioContainers addition for mira
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/mira
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/mira:4.9.6--1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/mira/4.9.6--1
$ module help quay.io/biocontainers/mira/4.9.6--1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### mira-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### mira-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### mira-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### mira-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### mira-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### mira-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### mira

```bash
$ singularity exec <container> /usr/local/bin/mira
$ podman run --it --rm --entrypoint /usr/local/bin/mira   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/mira   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### mira-install-sls-rrna.sh

```bash
$ singularity exec <container> /usr/local/bin/mira-install-sls-rrna.sh
$ podman run --it --rm --entrypoint /usr/local/bin/mira-install-sls-rrna.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/mira-install-sls-rrna.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### mirabait

```bash
$ singularity exec <container> /usr/local/bin/mirabait
$ podman run --it --rm --entrypoint /usr/local/bin/mirabait   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/mirabait   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### miraconvert

```bash
$ singularity exec <container> /usr/local/bin/miraconvert
$ podman run --it --rm --entrypoint /usr/local/bin/miraconvert   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/miraconvert   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### miramem

```bash
$ singularity exec <container> /usr/local/bin/miramem
$ podman run --it --rm --entrypoint /usr/local/bin/miramem   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/miramem   -v ${PWD} -w ${PWD} <container> -c " $@"
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