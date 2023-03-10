---
layout: container
name:  "quay.io/biocontainers/bioconductor-methylinheritance"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-methylinheritance/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-methylinheritance/container.yaml"
updated_at: "2023-01-13 03:34:37.048374"
latest: "1.22.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-methylinheritance"
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
description: "shpc-registry automated BioContainers addition for bioconductor-methylinheritance"
config: {"url": "https://biocontainers.pro/tools/bioconductor-methylinheritance", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-methylinheritance", "latest": {"1.22.0--r42hdfd78af_0": "sha256:e4ca008514480d910c2ccf2dd21be4e1a261d8f77453d6aaa3dffb89db439e67"}, "tags": {"1.8.0--r36_1": "sha256:a83baa8fc04389bfa90ea8220a3c2de0b8c8e4a474e495da0bd86bda0e54b86e", "1.18.0--r41hdfd78af_0": "sha256:4179ec2835184ee657d7ba21c43a0037f7fcd629801cc946c11c7061c468d901", "1.16.0--r41hdfd78af_0": "sha256:f159c326269e0ddf758b53347d34e50f5bd1e3068d62411839771c9e91c85ce8", "1.14.0--r40hdfd78af_1": "sha256:bad14b3ba6dc7500a0824e0c1710d29f33c2eb5acd9273fcfc39298829218a1c", "1.12.0--r40_0": "sha256:8b6dbc2a7451526f41371e4bd0a4d0f15afc4f110f31daa096b5c20addfe5b1e", "1.10.0--r36_0": "sha256:5f44f8c19aa0ad68ea327eeb165155a1b4abd4a03af20cddcca883c00601f134", "1.22.0--r42hdfd78af_0": "sha256:e4ca008514480d910c2ccf2dd21be4e1a261d8f77453d6aaa3dffb89db439e67"}, "docker": "quay.io/biocontainers/bioconductor-methylinheritance", "aliases": {"gio-launch-desktop": "/usr/local/bin/gio-launch-desktop", "c89": "/usr/local/bin/c89", "c99": "/usr/local/bin/c99"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-methylinheritance.
shpc-registry automated BioContainers addition for bioconductor-methylinheritance
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-methylinheritance
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-methylinheritance:1.22.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-methylinheritance/1.22.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-methylinheritance/1.22.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-methylinheritance-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-methylinheritance-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-methylinheritance-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-methylinheritance-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-methylinheritance-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-methylinheritance-inspect-deffile:

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