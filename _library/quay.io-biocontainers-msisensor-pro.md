---
layout: container
name:  "quay.io/biocontainers/msisensor-pro"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/msisensor-pro/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/msisensor-pro/container.yaml"
updated_at: "2023-01-13 03:44:26.791913"
latest: "1.2.0--ha04fe3b_4"
container_url: "https://biocontainers.pro/tools/msisensor-pro"
aliases:
 - "msisensor-pro"
 - "htsfile"
 - "bgzip"
 - "tabix"
versions:
 - "v1.2.0--hfc31af2_0"
 - "1.2.0--ha04fe3b_4"
description: "shpc-registry automated BioContainers addition for msisensor-pro"
config: {"url": "https://biocontainers.pro/tools/msisensor-pro", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for msisensor-pro", "latest": {"1.2.0--ha04fe3b_4": "sha256:9499c1a8c58ae0ab30c37a51d36a4d795a2093425e1ad671d0ce0d33723940b7"}, "tags": {"v1.2.0--hfc31af2_0": "sha256:7a73de995ab598c1819d5476f7450ad0c311d5235651a6466c445d74338d230e", "1.2.0--ha04fe3b_4": "sha256:9499c1a8c58ae0ab30c37a51d36a4d795a2093425e1ad671d0ce0d33723940b7"}, "docker": "quay.io/biocontainers/msisensor-pro", "aliases": {"msisensor-pro": "/usr/local/bin/msisensor-pro", "htsfile": "/usr/local/bin/htsfile", "bgzip": "/usr/local/bin/bgzip", "tabix": "/usr/local/bin/tabix"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/msisensor-pro.
shpc-registry automated BioContainers addition for msisensor-pro
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/msisensor-pro
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/msisensor-pro:1.2.0--ha04fe3b_4
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/msisensor-pro/1.2.0--ha04fe3b_4
$ module help quay.io/biocontainers/msisensor-pro/1.2.0--ha04fe3b_4
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### msisensor-pro-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### msisensor-pro-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### msisensor-pro-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### msisensor-pro-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### msisensor-pro-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### msisensor-pro-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### msisensor-pro

```bash
$ singularity exec <container> /usr/local/bin/msisensor-pro
$ podman run --it --rm --entrypoint /usr/local/bin/msisensor-pro   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/msisensor-pro   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### htsfile

```bash
$ singularity exec <container> /usr/local/bin/htsfile
$ podman run --it --rm --entrypoint /usr/local/bin/htsfile   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/htsfile   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### bgzip

```bash
$ singularity exec <container> /usr/local/bin/bgzip
$ podman run --it --rm --entrypoint /usr/local/bin/bgzip   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/bgzip   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### tabix

```bash
$ singularity exec <container> /usr/local/bin/tabix
$ podman run --it --rm --entrypoint /usr/local/bin/tabix   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/tabix   -v ${PWD} -w ${PWD} <container> -c " $@"
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