---
layout: container
name:  "quay.io/biocontainers/rdflib"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/rdflib/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/rdflib/container.yaml"
updated_at: "2023-01-13 03:39:05.319558"
latest: "4.2.2--py36_0"
container_url: "https://biocontainers.pro/tools/rdflib"

versions:
 - "4.2.2--py36_0"
description: "shpc-registry automated BioContainers addition for rdflib"
config: {"url": "https://biocontainers.pro/tools/rdflib", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for rdflib", "latest": {"4.2.2--py36_0": "sha256:81c10a629ea681cd88a3cfa08639f8ad0dc6b8cdbdb5c8705c018ce49be9bf55"}, "tags": {"4.2.2--py36_0": "sha256:81c10a629ea681cd88a3cfa08639f8ad0dc6b8cdbdb5c8705c018ce49be9bf55"}, "docker": "quay.io/biocontainers/rdflib"}
---

This module is a singularity container wrapper for quay.io/biocontainers/rdflib.
shpc-registry automated BioContainers addition for rdflib
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/rdflib
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/rdflib:4.2.2--py36_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/rdflib/4.2.2--py36_0
$ module help quay.io/biocontainers/rdflib/4.2.2--py36_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### rdflib-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### rdflib-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### rdflib-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### rdflib-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### rdflib-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### rdflib-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### rdflib

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