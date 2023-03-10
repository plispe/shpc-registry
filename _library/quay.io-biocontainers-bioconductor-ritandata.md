---
layout: container
name:  "quay.io/biocontainers/bioconductor-ritandata"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-ritandata/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-ritandata/container.yaml"
updated_at: "2023-01-13 03:15:22.888576"
latest: "1.22.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-ritandata"
aliases:
 - "gio-launch-desktop"
 - "c89"
 - "c99"
versions:
 - "1.8.0--r36_1"
 - "1.22.0--r42hdfd78af_0"
 - "1.21.0--r42hdfd78af_0"
 - "1.20.0--r41hdfd78af_0"
 - "1.18.1--r41hdfd78af_0"
 - "1.16.0--r41hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-ritandata"
config: {"url": "https://biocontainers.pro/tools/bioconductor-ritandata", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-ritandata", "latest": {"1.22.0--r42hdfd78af_0": "sha256:13c22f4f6991fd29f9d44022d07c8551775f56c0022d710a6e19890bd4b87fd5"}, "tags": {"1.8.0--r36_1": "sha256:82032f69af8b0579fc56e423cacc258671746d2c9a8e2104866e2238b7e58ebd", "1.22.0--r42hdfd78af_0": "sha256:13c22f4f6991fd29f9d44022d07c8551775f56c0022d710a6e19890bd4b87fd5", "1.21.0--r42hdfd78af_0": "sha256:c29774bec46febeecfc94b30577dfe68c2c97c942bafd8bbb723963b82940493", "1.20.0--r41hdfd78af_0": "sha256:ae2fd9e77f44edbe7bf18f5a4d28a3f326028b33a0c6e3420096b2ac62533c72", "1.18.1--r41hdfd78af_0": "sha256:35ea5392d63ea26400bfd5c7f99fa474d07e25284c2a0e24558a4f85c33fddae", "1.16.0--r41hdfd78af_0": "sha256:0e9c7acffa03e04a2394eb5b20c07ab0175a3dd5a39a874b2d5fbd04f1309fa5"}, "docker": "quay.io/biocontainers/bioconductor-ritandata", "aliases": {"gio-launch-desktop": "/usr/local/bin/gio-launch-desktop", "c89": "/usr/local/bin/c89", "c99": "/usr/local/bin/c99"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-ritandata.
shpc-registry automated BioContainers addition for bioconductor-ritandata
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-ritandata
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-ritandata:1.22.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-ritandata/1.22.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-ritandata/1.22.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-ritandata-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ritandata-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ritandata-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-ritandata-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-ritandata-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-ritandata-inspect-deffile:

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