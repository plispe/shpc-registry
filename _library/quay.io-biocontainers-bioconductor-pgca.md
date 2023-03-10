---
layout: container
name:  "quay.io/biocontainers/bioconductor-pgca"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-pgca/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-pgca/container.yaml"
updated_at: "2023-01-13 02:55:25.302699"
latest: "1.22.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-pgca"
aliases:
 - "gio-launch-desktop"
 - "c89"
 - "c99"
versions:
 - "1.8.0--r36_1"
 - "1.18.0--r41hdfd78af_0"
 - "1.16.0--r41hdfd78af_0"
 - "1.14.0--r40hdfd78af_1"
 - "1.12.0--r40_0"
 - "1.10.0--r36_0"
 - "1.22.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-pgca"
config: {"url": "https://biocontainers.pro/tools/bioconductor-pgca", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-pgca", "latest": {"1.22.0--r42hdfd78af_0": "sha256:d71de2e90139ecf3f963e866c504eaa4b3ccf1b501f2e07dc910928d65cf0119"}, "tags": {"1.8.0--r36_1": "sha256:ec781610e8d3943311435926a4931099947c6b5ef9dfdba976e0b52040e136bd", "1.18.0--r41hdfd78af_0": "sha256:e0f652fbb7ca2d802d0803f7e9bc1af90bf826eb488f7b326cb4cfd7ebe10213", "1.16.0--r41hdfd78af_0": "sha256:6f75a576f4877cdfa263976b7f198600663e03631ee025ad85b9decef0da9087", "1.14.0--r40hdfd78af_1": "sha256:5c6ed77f782f7329bac2da0f694a7b6877eee851a86a05058ffb7a6e99383dda", "1.12.0--r40_0": "sha256:095474f8929cdc151515326976c8ef414ac341c286487fae24750ecc443c5a6f", "1.10.0--r36_0": "sha256:33e7bd98fbdde9ff45dabcd6f7bbe7b0e6dc21b86e76701e01c52ad553f557c3", "1.22.0--r42hdfd78af_0": "sha256:d71de2e90139ecf3f963e866c504eaa4b3ccf1b501f2e07dc910928d65cf0119"}, "docker": "quay.io/biocontainers/bioconductor-pgca", "aliases": {"gio-launch-desktop": "/usr/local/bin/gio-launch-desktop", "c89": "/usr/local/bin/c89", "c99": "/usr/local/bin/c99"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-pgca.
shpc-registry automated BioContainers addition for bioconductor-pgca
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-pgca
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-pgca:1.22.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-pgca/1.22.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-pgca/1.22.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-pgca-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-pgca-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-pgca-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-pgca-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-pgca-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-pgca-inspect-deffile:

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