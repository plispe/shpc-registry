---
layout: container
name:  "quay.io/biocontainers/extract_fullseq"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/extract_fullseq/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/extract_fullseq/container.yaml"
updated_at: "2023-01-13 03:27:23.081049"
latest: "3.101--3"
container_url: "https://biocontainers.pro/tools/extract_fullseq"
aliases:
 - "extract_fullseq"
versions:
 - "3.101--3"
description: "shpc-registry automated BioContainers addition for extract_fullseq"
config: {"url": "https://biocontainers.pro/tools/extract_fullseq", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for extract_fullseq", "latest": {"3.101--3": "sha256:9c4fb0f1c50aaf454e68b619cfea21b5fae8afca0e38d2e64c77380f5af8221c"}, "tags": {"3.101--3": "sha256:9c4fb0f1c50aaf454e68b619cfea21b5fae8afca0e38d2e64c77380f5af8221c"}, "docker": "quay.io/biocontainers/extract_fullseq", "aliases": {"extract_fullseq": "/usr/local/bin/extract_fullseq"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/extract_fullseq.
shpc-registry automated BioContainers addition for extract_fullseq
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/extract_fullseq
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/extract_fullseq:3.101--3
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/extract_fullseq/3.101--3
$ module help quay.io/biocontainers/extract_fullseq/3.101--3
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### extract_fullseq-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### extract_fullseq-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### extract_fullseq-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### extract_fullseq-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### extract_fullseq-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### extract_fullseq-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### extract_fullseq

```bash
$ singularity exec <container> /usr/local/bin/extract_fullseq
$ podman run --it --rm --entrypoint /usr/local/bin/extract_fullseq   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/extract_fullseq   -v ${PWD} -w ${PWD} <container> -c " $@"
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