---
layout: container
name:  "quay.io/biocontainers/bioconductor-ga4ghshiny"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-ga4ghshiny/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-ga4ghshiny/container.yaml"
updated_at: "2023-01-13 03:24:03.481324"
latest: "1.20.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-ga4ghshiny"
aliases:
 - "gio-launch-desktop"
 - "c89"
 - "c99"
versions:
 - "1.8.0--r36_0"
 - "1.20.0--r42hdfd78af_0"
 - "1.16.0--r41hdfd78af_0"
 - "1.14.0--r41hdfd78af_0"
 - "1.12.0--r40hdfd78af_1"
 - "1.10.0--r40_0"
description: "shpc-registry automated BioContainers addition for bioconductor-ga4ghshiny"
config: {"url": "https://biocontainers.pro/tools/bioconductor-ga4ghshiny", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-ga4ghshiny", "latest": {"1.20.0--r42hdfd78af_0": "sha256:e28692b47a5f65e1f02e333faee8f753482c2ddcb8c1b68e942786434f141bb5"}, "tags": {"1.8.0--r36_0": "sha256:a19bc8b63a4a7faf4ad57319e9714fa5f6cf791941f00e555c1fbf6c633c4664", "1.20.0--r42hdfd78af_0": "sha256:e28692b47a5f65e1f02e333faee8f753482c2ddcb8c1b68e942786434f141bb5", "1.16.0--r41hdfd78af_0": "sha256:2d27178ec9a8de0e12fee44c398ce3e90c4badd1c937add1fd2d93a53ca7d863", "1.14.0--r41hdfd78af_0": "sha256:5eb4eec4308c9910f3959e39bd4f8a69bb685358e23d4392bfb0073e3ca6da88", "1.12.0--r40hdfd78af_1": "sha256:695cb48c3f86a6102ed1f3b20d539a0e4cf2983ec5e6aa2fe3c3b3ce0707f02b", "1.10.0--r40_0": "sha256:3284f1e69a2804a19c192185ac6267938797ed1583a974eed34384354c23c86f"}, "docker": "quay.io/biocontainers/bioconductor-ga4ghshiny", "aliases": {"gio-launch-desktop": "/usr/local/bin/gio-launch-desktop", "c89": "/usr/local/bin/c89", "c99": "/usr/local/bin/c99"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-ga4ghshiny.
shpc-registry automated BioContainers addition for bioconductor-ga4ghshiny
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-ga4ghshiny
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-ga4ghshiny:1.20.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-ga4ghshiny/1.20.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-ga4ghshiny/1.20.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-ga4ghshiny-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ga4ghshiny-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ga4ghshiny-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-ga4ghshiny-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-ga4ghshiny-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-ga4ghshiny-inspect-deffile:

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