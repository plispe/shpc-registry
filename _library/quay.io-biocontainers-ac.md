---
layout: container
name:  "quay.io/biocontainers/ac"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/ac/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/ac/container.yaml"
updated_at: "2023-01-13 03:42:57.836039"
latest: "1.1--h87f3376_2"
container_url: "https://biocontainers.pro/tools/ac"
aliases:
 - "AC"
versions:
 - "1.1--h87f3376_2"
description: "shpc-registry automated BioContainers addition for ac"
config: {"url": "https://biocontainers.pro/tools/ac", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for ac", "latest": {"1.1--h87f3376_2": "sha256:c38f2916e02283c67ad86f8a0083d77da97447272877191f09dced17f5159bc9"}, "tags": {"1.1--h87f3376_2": "sha256:c38f2916e02283c67ad86f8a0083d77da97447272877191f09dced17f5159bc9"}, "docker": "quay.io/biocontainers/ac", "aliases": {"AC": "/usr/local/bin/AC"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/ac.
shpc-registry automated BioContainers addition for ac
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/ac
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/ac:1.1--h87f3376_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/ac/1.1--h87f3376_2
$ module help quay.io/biocontainers/ac/1.1--h87f3376_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### ac-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### ac-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### ac-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### ac-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### ac-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### ac-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### AC

```bash
$ singularity exec <container> /usr/local/bin/AC
$ podman run --it --rm --entrypoint /usr/local/bin/AC   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/AC   -v ${PWD} -w ${PWD} <container> -c " $@"
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