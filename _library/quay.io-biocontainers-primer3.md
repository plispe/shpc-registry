---
layout: container
name:  "quay.io/biocontainers/primer3"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/primer3/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/primer3/container.yaml"
updated_at: "2023-01-13 03:15:45.177585"
latest: "2.6.1--pl5321h87f3376_2"
container_url: "https://biocontainers.pro/tools/primer3"

versions:
 - "v2.5.0--pl526he1b5a44_0"
 - "2.6.1--pl5321h87f3376_2"
 - "2.5.0--pl5262h1b792b2_1"
description: "shpc-registry automated BioContainers addition for primer3"
config: {"url": "https://biocontainers.pro/tools/primer3", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for primer3", "latest": {"2.6.1--pl5321h87f3376_2": "sha256:02b13b3403cab8201b92d0580de6fadca4e19fae6caaedc0d6cb36cb8afb5568"}, "tags": {"v2.5.0--pl526he1b5a44_0": "sha256:860d430a579f69ce45c4a729c7215e5dbabad650a988d7b7bcdef677be278d71", "2.6.1--pl5321h87f3376_2": "sha256:02b13b3403cab8201b92d0580de6fadca4e19fae6caaedc0d6cb36cb8afb5568", "2.5.0--pl5262h1b792b2_1": "sha256:f7913349cc10b498da1058fbcb848539e816bd437f2ab4b211252d636b3e840f"}, "docker": "quay.io/biocontainers/primer3"}
---

This module is a singularity container wrapper for quay.io/biocontainers/primer3.
shpc-registry automated BioContainers addition for primer3
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/primer3
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/primer3:2.6.1--pl5321h87f3376_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/primer3/2.6.1--pl5321h87f3376_2
$ module help quay.io/biocontainers/primer3/2.6.1--pl5321h87f3376_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### primer3-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### primer3-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### primer3-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### primer3-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### primer3-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### primer3-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### primer3

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
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