---
layout: container
name:  "quay.io/biocontainers/libidn"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/libidn/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/libidn/container.yaml"
updated_at: "2023-01-13 02:58:24.393633"
latest: "7.45.0--h87f3376_6"
container_url: "https://biocontainers.pro/tools/libidn"
aliases:
 - "idn"
versions:
 - "7.45.0--h87f3376_6"
description: "shpc-registry automated BioContainers addition for libidn"
config: {"url": "https://biocontainers.pro/tools/libidn", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for libidn", "latest": {"7.45.0--h87f3376_6": "sha256:04c8fc17e0ef3e5aae46f5b16a28639e3529238c0ecc944e0fb82bf0ed511d42"}, "tags": {"7.45.0--h87f3376_6": "sha256:04c8fc17e0ef3e5aae46f5b16a28639e3529238c0ecc944e0fb82bf0ed511d42"}, "docker": "quay.io/biocontainers/libidn", "aliases": {"idn": "/usr/local/bin/idn"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/libidn.
shpc-registry automated BioContainers addition for libidn
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/libidn
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/libidn:7.45.0--h87f3376_6
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/libidn/7.45.0--h87f3376_6
$ module help quay.io/biocontainers/libidn/7.45.0--h87f3376_6
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### libidn-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### libidn-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### libidn-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### libidn-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### libidn-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### libidn-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### idn

```bash
$ singularity exec <container> /usr/local/bin/idn
$ podman run --it --rm --entrypoint /usr/local/bin/idn   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/idn   -v ${PWD} -w ${PWD} <container> -c " $@"
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