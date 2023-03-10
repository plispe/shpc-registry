---
layout: container
name:  "quay.io/biocontainers/bioconductor-cydar"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-cydar/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-cydar/container.yaml"
updated_at: "2023-01-13 03:22:36.185805"
latest: "1.22.0--r42hc247a5b_0"
container_url: "https://biocontainers.pro/tools/bioconductor-cydar"
aliases:
 - "gio-launch-desktop"
 - "c89"
 - "c99"
versions:
 - "1.8.0--r36he1b5a44_1"
 - "1.18.0--r41hc247a5b_2"
 - "1.16.0--r41h399db7b_0"
 - "1.14.0--r40h399db7b_2"
 - "1.12.0--r40h5f743cb_0"
 - "1.10.0--r36he1b5a44_0"
 - "1.22.0--r42hc247a5b_0"
description: "shpc-registry automated BioContainers addition for bioconductor-cydar"
config: {"url": "https://biocontainers.pro/tools/bioconductor-cydar", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-cydar", "latest": {"1.22.0--r42hc247a5b_0": "sha256:d34e26f17eb250583982c0712a872f5ac9c56b9ce1f0e990e91001853871a28e"}, "tags": {"1.8.0--r36he1b5a44_1": "sha256:3c34bf8a1b42ec91799fbee12380b7047eeb0e2bf5f3a51b3ca7b786f03e6090", "1.18.0--r41hc247a5b_2": "sha256:45d364aac7eecde5d9008481a32f8e6704635be5a9ca7cfc50a9da2f075b7f23", "1.16.0--r41h399db7b_0": "sha256:93713c17a9004f6b6f2a94a3490092b4a0ae8e9fd5cc6307f228b1c513bbb7cb", "1.14.0--r40h399db7b_2": "sha256:0293febf97ecab22d63f3936624c3230a8c2e8e5e842282fa0a4d3cfe4250932", "1.12.0--r40h5f743cb_0": "sha256:0729f2cdbb795d2f26a15a2a48a6fa80692aeeb1823eeac2c37479016ffa0718", "1.10.0--r36he1b5a44_0": "sha256:380352fb6779dd7fbba6e6d2389f44e976a967bafecc2ae4a0ce52cab0896ff5", "1.22.0--r42hc247a5b_0": "sha256:d34e26f17eb250583982c0712a872f5ac9c56b9ce1f0e990e91001853871a28e"}, "docker": "quay.io/biocontainers/bioconductor-cydar", "aliases": {"gio-launch-desktop": "/usr/local/bin/gio-launch-desktop", "c89": "/usr/local/bin/c89", "c99": "/usr/local/bin/c99"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-cydar.
shpc-registry automated BioContainers addition for bioconductor-cydar
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-cydar
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-cydar:1.22.0--r42hc247a5b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-cydar/1.22.0--r42hc247a5b_0
$ module help quay.io/biocontainers/bioconductor-cydar/1.22.0--r42hc247a5b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-cydar-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-cydar-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-cydar-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-cydar-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-cydar-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-cydar-inspect-deffile:

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