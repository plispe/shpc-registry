---
layout: container
name:  "quay.io/biocontainers/bioconductor-outrider"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-outrider/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-outrider/container.yaml"
updated_at: "2023-01-13 03:10:38.538916"
latest: "1.16.0--r42hc247a5b_0"
container_url: "https://biocontainers.pro/tools/bioconductor-outrider"
aliases:
 - "x86_64-conda-linux-gnu-gfortran.bin"
versions:
 - "1.8.0--r40h399db7b_1"
 - "1.16.0--r42hc247a5b_0"
 - "1.12.0--r41hc247a5b_2"
 - "1.10.0--r41h399db7b_0"
description: "shpc-registry automated BioContainers addition for bioconductor-outrider"
config: {"url": "https://biocontainers.pro/tools/bioconductor-outrider", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-outrider", "latest": {"1.16.0--r42hc247a5b_0": "sha256:fe98bcc5033b3c17b9bae8db1d4511302409811c39b199af99033d717ae640f5"}, "tags": {"1.8.0--r40h399db7b_1": "sha256:649ebc8f3b5e92668a5500a95876a5b16e47a9d665f4df7234f79280c98380fc", "1.16.0--r42hc247a5b_0": "sha256:fe98bcc5033b3c17b9bae8db1d4511302409811c39b199af99033d717ae640f5", "1.12.0--r41hc247a5b_2": "sha256:b3d116071a8f3eee8658f00000550d9a5615835413b618ef760919dd1f5da895", "1.10.0--r41h399db7b_0": "sha256:84f9a6960621c0aeaf561013c72b572f761ea1765ed60081728158fae33001ad"}, "docker": "quay.io/biocontainers/bioconductor-outrider", "aliases": {"x86_64-conda-linux-gnu-gfortran.bin": "/usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-outrider.
shpc-registry automated BioContainers addition for bioconductor-outrider
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-outrider
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-outrider:1.16.0--r42hc247a5b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-outrider/1.16.0--r42hc247a5b_0
$ module help quay.io/biocontainers/bioconductor-outrider/1.16.0--r42hc247a5b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-outrider-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-outrider-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-outrider-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-outrider-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-outrider-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-outrider-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### x86_64-conda-linux-gnu-gfortran.bin

```bash
$ singularity exec <container> /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin
$ podman run --it --rm --entrypoint /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin   -v ${PWD} -w ${PWD} <container> -c " $@"
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