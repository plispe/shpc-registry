---
layout: container
name:  "quay.io/biocontainers/opentargets"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/opentargets/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/opentargets/container.yaml"
updated_at: "2023-01-13 03:27:16.849200"
latest: "3.1.16--pyh864c0ab_1"
container_url: "https://biocontainers.pro/tools/opentargets"

versions:
 - "3.1.16--pyh864c0ab_1"
description: "shpc-registry automated BioContainers addition for opentargets"
config: {"url": "https://biocontainers.pro/tools/opentargets", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for opentargets", "latest": {"3.1.16--pyh864c0ab_1": "sha256:6fcc27a9c5c1996bc6bcf7054ad7946201fc9b4ff41c629b8a7b35c8d702183d"}, "tags": {"3.1.16--pyh864c0ab_1": "sha256:6fcc27a9c5c1996bc6bcf7054ad7946201fc9b4ff41c629b8a7b35c8d702183d"}, "docker": "quay.io/biocontainers/opentargets"}
---

This module is a singularity container wrapper for quay.io/biocontainers/opentargets.
shpc-registry automated BioContainers addition for opentargets
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/opentargets
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/opentargets:3.1.16--pyh864c0ab_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/opentargets/3.1.16--pyh864c0ab_1
$ module help quay.io/biocontainers/opentargets/3.1.16--pyh864c0ab_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### opentargets-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### opentargets-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### opentargets-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### opentargets-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### opentargets-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### opentargets-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### opentargets

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