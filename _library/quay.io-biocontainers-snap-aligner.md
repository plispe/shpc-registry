---
layout: container
name:  "quay.io/biocontainers/snap-aligner"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/snap-aligner/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/snap-aligner/container.yaml"
updated_at: "2023-01-13 03:33:13.041580"
latest: "2.0.1--hd03093a_1"
container_url: "https://biocontainers.pro/tools/snap-aligner"
aliases:
 - "snap-aligner"
versions:
 - "2.0.1--hd03093a_1"
description: "shpc-registry automated BioContainers addition for snap-aligner"
config: {"url": "https://biocontainers.pro/tools/snap-aligner", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for snap-aligner", "latest": {"2.0.1--hd03093a_1": "sha256:47899129f7830517f018b20096f047e8940b828b38e3323d5890a3721ab4e8da"}, "tags": {"2.0.1--hd03093a_1": "sha256:47899129f7830517f018b20096f047e8940b828b38e3323d5890a3721ab4e8da"}, "docker": "quay.io/biocontainers/snap-aligner", "aliases": {"snap-aligner": "/usr/local/bin/snap-aligner"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/snap-aligner.
shpc-registry automated BioContainers addition for snap-aligner
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/snap-aligner
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/snap-aligner:2.0.1--hd03093a_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/snap-aligner/2.0.1--hd03093a_1
$ module help quay.io/biocontainers/snap-aligner/2.0.1--hd03093a_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### snap-aligner-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### snap-aligner-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### snap-aligner-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### snap-aligner-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### snap-aligner-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### snap-aligner-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### snap-aligner

```bash
$ singularity exec <container> /usr/local/bin/snap-aligner
$ podman run --it --rm --entrypoint /usr/local/bin/snap-aligner   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/snap-aligner   -v ${PWD} -w ${PWD} <container> -c " $@"
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