---
layout: container
name:  "quay.io/biocontainers/variantbam"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/variantbam/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/variantbam/container.yaml"
updated_at: "2023-01-13 02:50:34.400278"
latest: "1.4.4a--h468198e_6"
container_url: "https://biocontainers.pro/tools/variantbam"
aliases:
 - "variant"
versions:
 - "1.4.4a--h468198e_6"
description: "shpc-registry automated BioContainers addition for variantbam"
config: {"url": "https://biocontainers.pro/tools/variantbam", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for variantbam", "latest": {"1.4.4a--h468198e_6": "sha256:9df194aa4587d56ce8ece6926ade793be0095947f7a7c3e791b1969a295422cd"}, "tags": {"1.4.4a--h468198e_6": "sha256:9df194aa4587d56ce8ece6926ade793be0095947f7a7c3e791b1969a295422cd"}, "docker": "quay.io/biocontainers/variantbam", "aliases": {"variant": "/usr/local/bin/variant"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/variantbam.
shpc-registry automated BioContainers addition for variantbam
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/variantbam
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/variantbam:1.4.4a--h468198e_6
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/variantbam/1.4.4a--h468198e_6
$ module help quay.io/biocontainers/variantbam/1.4.4a--h468198e_6
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### variantbam-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### variantbam-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### variantbam-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### variantbam-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### variantbam-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### variantbam-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### variant

```bash
$ singularity exec <container> /usr/local/bin/variant
$ podman run --it --rm --entrypoint /usr/local/bin/variant   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/variant   -v ${PWD} -w ${PWD} <container> -c " $@"
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