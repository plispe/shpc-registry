---
layout: container
name:  "quay.io/biocontainers/pandaseq"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/pandaseq/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/pandaseq/container.yaml"
updated_at: "2023-01-13 03:06:41.236617"
latest: "2.11--h67092d7_6"
container_url: "https://biocontainers.pro/tools/pandaseq"
aliases:
 - "pandaseq"
 - "pandaseq-checkid"
 - "pandaseq-diff"
 - "pandaseq-hang"
 - "pandaxs"
versions:
 - "2.8.1--h67092d7_5"
 - "2.11--h67092d7_6"
description: "shpc-registry automated BioContainers addition for pandaseq"
config: {"url": "https://biocontainers.pro/tools/pandaseq", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for pandaseq", "latest": {"2.11--h67092d7_6": "sha256:9073ca60900d33d015cee556698c66e1eea806e9ef461ef723eea5643107a096"}, "tags": {"2.8.1--h67092d7_5": "sha256:1be33559ab6f1f426f99c2e0d8230f52643df009756da4a6e6ece0dbf04e5f18", "2.11--h67092d7_6": "sha256:9073ca60900d33d015cee556698c66e1eea806e9ef461ef723eea5643107a096"}, "docker": "quay.io/biocontainers/pandaseq", "aliases": {"pandaseq": "/usr/local/bin/pandaseq", "pandaseq-checkid": "/usr/local/bin/pandaseq-checkid", "pandaseq-diff": "/usr/local/bin/pandaseq-diff", "pandaseq-hang": "/usr/local/bin/pandaseq-hang", "pandaxs": "/usr/local/bin/pandaxs"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/pandaseq.
shpc-registry automated BioContainers addition for pandaseq
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/pandaseq
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/pandaseq:2.11--h67092d7_6
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/pandaseq/2.11--h67092d7_6
$ module help quay.io/biocontainers/pandaseq/2.11--h67092d7_6
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### pandaseq-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### pandaseq-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### pandaseq-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### pandaseq-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### pandaseq-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### pandaseq-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### pandaseq

```bash
$ singularity exec <container> /usr/local/bin/pandaseq
$ podman run --it --rm --entrypoint /usr/local/bin/pandaseq   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pandaseq   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pandaseq-checkid

```bash
$ singularity exec <container> /usr/local/bin/pandaseq-checkid
$ podman run --it --rm --entrypoint /usr/local/bin/pandaseq-checkid   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pandaseq-checkid   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pandaseq-diff

```bash
$ singularity exec <container> /usr/local/bin/pandaseq-diff
$ podman run --it --rm --entrypoint /usr/local/bin/pandaseq-diff   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pandaseq-diff   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pandaseq-hang

```bash
$ singularity exec <container> /usr/local/bin/pandaseq-hang
$ podman run --it --rm --entrypoint /usr/local/bin/pandaseq-hang   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pandaseq-hang   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pandaxs

```bash
$ singularity exec <container> /usr/local/bin/pandaxs
$ podman run --it --rm --entrypoint /usr/local/bin/pandaxs   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pandaxs   -v ${PWD} -w ${PWD} <container> -c " $@"
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