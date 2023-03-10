---
layout: container
name:  "ghcr.io/autamus/bwa"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/ghcr.io/autamus/bwa/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/ghcr.io/autamus/bwa/container.yaml"
updated_at: "2023-01-13 03:46:22.431333"
latest: "0.7.17"
container_url: "https://github.com/orgs/autamus/packages/container/package/bwa"
aliases:
 - "bwa"
versions:
 - "0.7.17"
 - "latest"
description: "BWA is a software package for mapping low-divergent sequences against a large reference genome, such as the human genome."
config: {"docker": "ghcr.io/autamus/bwa", "url": "https://github.com/orgs/autamus/packages/container/package/bwa", "maintainer": "@vsoch", "description": "BWA is a software package for mapping low-divergent sequences against a large reference genome, such as the human genome.", "latest": {"0.7.17": "sha256:cec40797bbe92df24dc4ddf9e9c9cce44fe068bfbf27b0e3bc0b3b6be65b6e3a"}, "tags": {"0.7.17": "sha256:cec40797bbe92df24dc4ddf9e9c9cce44fe068bfbf27b0e3bc0b3b6be65b6e3a", "latest": "sha256:cec40797bbe92df24dc4ddf9e9c9cce44fe068bfbf27b0e3bc0b3b6be65b6e3a"}, "aliases": {"bwa": "/opt/view/bin/bwa"}}
---

This module is a singularity container wrapper for ghcr.io/autamus/bwa.
BWA is a software package for mapping low-divergent sequences against a large reference genome, such as the human genome.
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install ghcr.io/autamus/bwa
```

Or a specific version:

```bash
$ shpc install ghcr.io/autamus/bwa:0.7.17
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load ghcr.io/autamus/bwa/0.7.17
$ module help ghcr.io/autamus/bwa/0.7.17
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bwa-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bwa-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bwa-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bwa-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bwa-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bwa-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### bwa

```bash
$ singularity exec <container> /opt/view/bin/bwa
$ podman run --it --rm --entrypoint /opt/view/bin/bwa   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /opt/view/bin/bwa   -v ${PWD} -w ${PWD} <container> -c " $@"
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