---
layout: container
name:  "quay.io/biocontainers/bioconductor-gmrp"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-gmrp/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-gmrp/container.yaml"
updated_at: "2023-01-13 03:37:49.269411"
latest: "1.26.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-gmrp"
aliases:
 - "wget"
 - "ncurses5-config"
 - "ncursesw5-config"
versions:
 - "1.8.1--r341_0"
 - "1.22.0--r41hdfd78af_0"
 - "1.20.0--r41hdfd78af_0"
 - "1.18.0--r40hdfd78af_1"
 - "1.16.0--r40_0"
 - "1.14.0--r36_0"
 - "1.26.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-gmrp"
config: {"url": "https://biocontainers.pro/tools/bioconductor-gmrp", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-gmrp", "latest": {"1.26.0--r42hdfd78af_0": "sha256:6d8c59ff7b1a53037e2de0c607f06d2b03d71ba6e8fcc61ee19a309181a4b36c"}, "tags": {"1.8.1--r341_0": "sha256:e328c43b5f84272283a433fcac7f14908ba65f988e08570bfa86cbc68b7360f1", "1.22.0--r41hdfd78af_0": "sha256:7977b55bedef437d64289324ce54e8dc94adf1e90a8c4304a431ffb21e844de5", "1.20.0--r41hdfd78af_0": "sha256:0c519a7bc8f1615fc25a95866be2154d51c858846b16ce1e3aec1e856a78954b", "1.18.0--r40hdfd78af_1": "sha256:05babf8faee7fa73cad7448b6da4b7423cf5253fa6553ae66e9bc848a7f34fbb", "1.16.0--r40_0": "sha256:fd0481fc152397a45d959fd3a7540cf8f809e9e1e93cd7108d87c65a10baaf6c", "1.14.0--r36_0": "sha256:acdd2af87e83535995ecfbce731247a8bd28c9f4de1492eecf0afd08385c7c87", "1.26.0--r42hdfd78af_0": "sha256:6d8c59ff7b1a53037e2de0c607f06d2b03d71ba6e8fcc61ee19a309181a4b36c"}, "docker": "quay.io/biocontainers/bioconductor-gmrp", "aliases": {"wget": "/usr/local/bin/wget", "ncurses5-config": "/usr/local/bin/ncurses5-config", "ncursesw5-config": "/usr/local/bin/ncursesw5-config"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-gmrp.
shpc-registry automated BioContainers addition for bioconductor-gmrp
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-gmrp
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-gmrp:1.26.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-gmrp/1.26.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-gmrp/1.26.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-gmrp-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-gmrp-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-gmrp-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-gmrp-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-gmrp-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-gmrp-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### wget

```bash
$ singularity exec <container> /usr/local/bin/wget
$ podman run --it --rm --entrypoint /usr/local/bin/wget   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/wget   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### ncurses5-config

```bash
$ singularity exec <container> /usr/local/bin/ncurses5-config
$ podman run --it --rm --entrypoint /usr/local/bin/ncurses5-config   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/ncurses5-config   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### ncursesw5-config

```bash
$ singularity exec <container> /usr/local/bin/ncursesw5-config
$ podman run --it --rm --entrypoint /usr/local/bin/ncursesw5-config   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/ncursesw5-config   -v ${PWD} -w ${PWD} <container> -c " $@"
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