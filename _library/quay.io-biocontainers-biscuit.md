---
layout: container
name:  "quay.io/biocontainers/biscuit"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/biscuit/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/biscuit/container.yaml"
updated_at: "2023-01-13 03:34:28.442193"
latest: "1.1.0.20220707--he272189_1"
container_url: "https://biocontainers.pro/tools/biscuit"
aliases:
 - "QC.sh"
 - "biscuit"
 - "build_biscuit_QC_assets.pl"
 - "build_biscuit_QC_assets.pl.bak"
 - "perl5.32.1"
 - "streamzip"
versions:
 - "1.1.0.20220707--he272189_1"
description: "shpc-registry automated BioContainers addition for biscuit"
config: {"url": "https://biocontainers.pro/tools/biscuit", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for biscuit", "latest": {"1.1.0.20220707--he272189_1": "sha256:ca540d2b392d0e2ea6525b0b4e88e99eed713deff2bd6cec942e01b14333e270"}, "tags": {"1.1.0.20220707--he272189_1": "sha256:ca540d2b392d0e2ea6525b0b4e88e99eed713deff2bd6cec942e01b14333e270"}, "docker": "quay.io/biocontainers/biscuit", "aliases": {"QC.sh": "/usr/local/bin/QC.sh", "biscuit": "/usr/local/bin/biscuit", "build_biscuit_QC_assets.pl": "/usr/local/bin/build_biscuit_QC_assets.pl", "build_biscuit_QC_assets.pl.bak": "/usr/local/bin/build_biscuit_QC_assets.pl.bak", "perl5.32.1": "/usr/local/bin/perl5.32.1", "streamzip": "/usr/local/bin/streamzip"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/biscuit.
shpc-registry automated BioContainers addition for biscuit
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/biscuit
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/biscuit:1.1.0.20220707--he272189_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/biscuit/1.1.0.20220707--he272189_1
$ module help quay.io/biocontainers/biscuit/1.1.0.20220707--he272189_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### biscuit-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### biscuit-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### biscuit-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### biscuit-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### biscuit-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### biscuit-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### QC.sh

```bash
$ singularity exec <container> /usr/local/bin/QC.sh
$ podman run --it --rm --entrypoint /usr/local/bin/QC.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/QC.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### biscuit

```bash
$ singularity exec <container> /usr/local/bin/biscuit
$ podman run --it --rm --entrypoint /usr/local/bin/biscuit   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/biscuit   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### build_biscuit_QC_assets.pl

```bash
$ singularity exec <container> /usr/local/bin/build_biscuit_QC_assets.pl
$ podman run --it --rm --entrypoint /usr/local/bin/build_biscuit_QC_assets.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/build_biscuit_QC_assets.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### build_biscuit_QC_assets.pl.bak

```bash
$ singularity exec <container> /usr/local/bin/build_biscuit_QC_assets.pl.bak
$ podman run --it --rm --entrypoint /usr/local/bin/build_biscuit_QC_assets.pl.bak   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/build_biscuit_QC_assets.pl.bak   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### perl5.32.1

```bash
$ singularity exec <container> /usr/local/bin/perl5.32.1
$ podman run --it --rm --entrypoint /usr/local/bin/perl5.32.1   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/perl5.32.1   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### streamzip

```bash
$ singularity exec <container> /usr/local/bin/streamzip
$ podman run --it --rm --entrypoint /usr/local/bin/streamzip   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/streamzip   -v ${PWD} -w ${PWD} <container> -c " $@"
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