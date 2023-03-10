---
layout: container
name:  "quay.io/biocontainers/bioconductor-micrornaome"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-micrornaome/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-micrornaome/container.yaml"
updated_at: "2023-01-13 03:07:06.580391"
latest: "1.20.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-micrornaome"
aliases:
 - "gio-launch-desktop"
 - "c89"
 - "c99"
versions:
 - "1.8.0--r36_0"
 - "1.20.0--r42hdfd78af_0"
 - "1.16.0--r41hdfd78af_1"
 - "1.14.0--r41hdfd78af_0"
 - "1.12.0--r40hdfd78af_1"
 - "1.10.0--r40_0"
description: "shpc-registry automated BioContainers addition for bioconductor-micrornaome"
config: {"url": "https://biocontainers.pro/tools/bioconductor-micrornaome", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-micrornaome", "latest": {"1.20.0--r42hdfd78af_0": "sha256:d5331bf6b00707c9e53502ea104fca2493591d000c72db3492aab1745f046469"}, "tags": {"1.8.0--r36_0": "sha256:a557144d03190db977828dede7136307c87ca377b19e5fe4cf90eb0eb0f3a763", "1.20.0--r42hdfd78af_0": "sha256:d5331bf6b00707c9e53502ea104fca2493591d000c72db3492aab1745f046469", "1.16.0--r41hdfd78af_1": "sha256:e1b95d6620bf038339acae2e82b4eafdd28205a40ed6b7414abebbcaceb032f9", "1.14.0--r41hdfd78af_0": "sha256:7d904bbb610401b2aa03ef8cbc3e99f331fbc327dd9dc4d6a57623ee2e7cdd1b", "1.12.0--r40hdfd78af_1": "sha256:b1b4332dafe20b0720ce2c52dcbd5f186a422629f3cf90454c3760b4bfa702a7", "1.10.0--r40_0": "sha256:15d3f600292d6a68bbb4b83d4046f22de3a03c2526910543213ff80dd5e45c9b"}, "docker": "quay.io/biocontainers/bioconductor-micrornaome", "aliases": {"gio-launch-desktop": "/usr/local/bin/gio-launch-desktop", "c89": "/usr/local/bin/c89", "c99": "/usr/local/bin/c99"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-micrornaome.
shpc-registry automated BioContainers addition for bioconductor-micrornaome
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-micrornaome
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-micrornaome:1.20.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-micrornaome/1.20.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-micrornaome/1.20.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-micrornaome-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-micrornaome-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-micrornaome-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-micrornaome-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-micrornaome-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-micrornaome-inspect-deffile:

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