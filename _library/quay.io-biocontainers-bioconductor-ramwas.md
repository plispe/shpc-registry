---
layout: container
name:  "quay.io/biocontainers/bioconductor-ramwas"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-ramwas/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-ramwas/container.yaml"
updated_at: "2023-01-13 03:44:48.897944"
latest: "1.22.0--r42hc0cfd56_0"
container_url: "https://biocontainers.pro/tools/bioconductor-ramwas"
aliases:
 - "gio-launch-desktop"
 - "c89"
 - "c99"
versions:
 - "1.8.0--r36h516909a_1"
 - "1.22.0--r42hc0cfd56_0"
 - "1.18.0--r41hc0cfd56_2"
 - "1.16.0--r41hd029910_0"
 - "1.14.0--r40hd029910_1"
 - "1.12.0--r40h037d062_0"
description: "shpc-registry automated BioContainers addition for bioconductor-ramwas"
config: {"url": "https://biocontainers.pro/tools/bioconductor-ramwas", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-ramwas", "latest": {"1.22.0--r42hc0cfd56_0": "sha256:54b9d5995b5375eb47b43044a6306bd74616b76c0eee56dacdfbcb0aaa7bdec0"}, "tags": {"1.8.0--r36h516909a_1": "sha256:812e544f776fbc4af27dd1ad862ea6c74a4a9849b2403cc452dcf792a4d4cf9a", "1.22.0--r42hc0cfd56_0": "sha256:54b9d5995b5375eb47b43044a6306bd74616b76c0eee56dacdfbcb0aaa7bdec0", "1.18.0--r41hc0cfd56_2": "sha256:3658661b929abe6ddef6ab30dcfc83640ca590db52a7986f2f8313d6bc7e0dd6", "1.16.0--r41hd029910_0": "sha256:e9d62be7b8323519e8dab0b9354dc0b5491d91b56f96c384668e360016b9922e", "1.14.0--r40hd029910_1": "sha256:dcc7233f17f99af6d7b9f25781162bff974046a0ebe82c6e6a315e862c3706d5", "1.12.0--r40h037d062_0": "sha256:136de63820e263b5d8bbfe14aae04ee4dda3e11c1b06cc2ac2336fffc3570274"}, "docker": "quay.io/biocontainers/bioconductor-ramwas", "aliases": {"gio-launch-desktop": "/usr/local/bin/gio-launch-desktop", "c89": "/usr/local/bin/c89", "c99": "/usr/local/bin/c99"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-ramwas.
shpc-registry automated BioContainers addition for bioconductor-ramwas
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-ramwas
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-ramwas:1.22.0--r42hc0cfd56_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-ramwas/1.22.0--r42hc0cfd56_0
$ module help quay.io/biocontainers/bioconductor-ramwas/1.22.0--r42hc0cfd56_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-ramwas-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ramwas-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ramwas-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-ramwas-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-ramwas-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-ramwas-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### gio-launch-desktop

```bash
$ singularity exec <container> /usr/local/bin/gio-launch-desktop
$ podman run --it --rm --entrypoint /usr/local/bin/gio-launch-desktop   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/gio-launch-desktop   -v ${PWD} -w ${PWD} <container> -c " $@"
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