---
layout: container
name:  "quay.io/biocontainers/bioconductor-gopro"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-gopro/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-gopro/container.yaml"
updated_at: "2023-01-13 03:10:53.876836"
latest: "1.24.0--r42hc247a5b_0"
container_url: "https://biocontainers.pro/tools/bioconductor-gopro"
aliases:
 - "wget"
 - "c89"
 - "c99"
versions:
 - "1.8.0--r351hf484d3e_0"
 - "1.20.0--r41hc247a5b_2"
 - "1.18.0--r41h399db7b_0"
 - "1.16.0--r40h399db7b_1"
 - "1.14.0--r40h5f743cb_0"
 - "1.12.0--r36he1b5a44_0"
 - "1.24.0--r42hc247a5b_0"
description: "shpc-registry automated BioContainers addition for bioconductor-gopro"
config: {"url": "https://biocontainers.pro/tools/bioconductor-gopro", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-gopro", "latest": {"1.24.0--r42hc247a5b_0": "sha256:41b6685132f3d59b721520116f5d156d4066d66f50fc0408b9fac98ecde87c11"}, "tags": {"1.8.0--r351hf484d3e_0": "sha256:1da51e006a66eaee5ba08a555ca3940c96c8b93536eb01150a1a35380557ffb5", "1.20.0--r41hc247a5b_2": "sha256:75efc16c002161a49d7f4ac31d4e4c35ab38a892b11ee02237f140a40f443915", "1.18.0--r41h399db7b_0": "sha256:af0cdfea9a20c1b68fc2b3e9d2c503969fa7257fb3055ecb464e56edd5e6d402", "1.16.0--r40h399db7b_1": "sha256:6ed7b1bcc262ea9c15baed5f781fd4244ab7a4583a7f96d391baae3385da97b0", "1.14.0--r40h5f743cb_0": "sha256:e7af4f6b62426060ea1ccfbc37a75376eadec861b8381a459dd5e25519639103", "1.12.0--r36he1b5a44_0": "sha256:68dc4aad8082686def07736191e79b69c6adc47b5d4b7ca1b312bc6ec5de0f5c", "1.24.0--r42hc247a5b_0": "sha256:41b6685132f3d59b721520116f5d156d4066d66f50fc0408b9fac98ecde87c11"}, "docker": "quay.io/biocontainers/bioconductor-gopro", "aliases": {"wget": "/usr/local/bin/wget", "c89": "/usr/local/bin/c89", "c99": "/usr/local/bin/c99"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-gopro.
shpc-registry automated BioContainers addition for bioconductor-gopro
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-gopro
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-gopro:1.24.0--r42hc247a5b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-gopro/1.24.0--r42hc247a5b_0
$ module help quay.io/biocontainers/bioconductor-gopro/1.24.0--r42hc247a5b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-gopro-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-gopro-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-gopro-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-gopro-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-gopro-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-gopro-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### wget

```bash
$ singularity exec <container> /usr/local/bin/wget
$ podman run --it --rm --entrypoint /usr/local/bin/wget   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/wget   -v ${PWD} -w ${PWD} <container> -c " $@"
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