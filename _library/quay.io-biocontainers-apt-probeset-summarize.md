---
layout: container
name:  "quay.io/biocontainers/apt-probeset-summarize"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/apt-probeset-summarize/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/apt-probeset-summarize/container.yaml"
updated_at: "2023-01-13 03:33:55.247768"
latest: "2.10.0--h9f5acd7_3"
container_url: "https://biocontainers.pro/tools/apt-probeset-summarize"
aliases:
 - "apt-probeset-summarize"
versions:
 - "2.10.0--h9f5acd7_3"
description: "shpc-registry automated BioContainers addition for apt-probeset-summarize"
config: {"url": "https://biocontainers.pro/tools/apt-probeset-summarize", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for apt-probeset-summarize", "latest": {"2.10.0--h9f5acd7_3": "sha256:9b0d8782daca43d81dd1e18752c012e435d24d45efe5fb0a17ef243ddefcd390"}, "tags": {"2.10.0--h9f5acd7_3": "sha256:9b0d8782daca43d81dd1e18752c012e435d24d45efe5fb0a17ef243ddefcd390"}, "docker": "quay.io/biocontainers/apt-probeset-summarize", "aliases": {"apt-probeset-summarize": "/usr/local/bin/apt-probeset-summarize"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/apt-probeset-summarize.
shpc-registry automated BioContainers addition for apt-probeset-summarize
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/apt-probeset-summarize
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/apt-probeset-summarize:2.10.0--h9f5acd7_3
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/apt-probeset-summarize/2.10.0--h9f5acd7_3
$ module help quay.io/biocontainers/apt-probeset-summarize/2.10.0--h9f5acd7_3
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### apt-probeset-summarize-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### apt-probeset-summarize-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### apt-probeset-summarize-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### apt-probeset-summarize-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### apt-probeset-summarize-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### apt-probeset-summarize-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### apt-probeset-summarize

```bash
$ singularity exec <container> /usr/local/bin/apt-probeset-summarize
$ podman run --it --rm --entrypoint /usr/local/bin/apt-probeset-summarize   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/apt-probeset-summarize   -v ${PWD} -w ${PWD} <container> -c " $@"
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