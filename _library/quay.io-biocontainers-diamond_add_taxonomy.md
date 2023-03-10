---
layout: container
name:  "quay.io/biocontainers/diamond_add_taxonomy"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/diamond_add_taxonomy/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/diamond_add_taxonomy/container.yaml"
updated_at: "2023-01-13 03:39:29.028466"
latest: "0.1.2--py36_0"
container_url: "https://biocontainers.pro/tools/diamond_add_taxonomy"

versions:
 - "0.1.2--py36_0"
description: "shpc-registry automated BioContainers addition for diamond_add_taxonomy"
config: {"url": "https://biocontainers.pro/tools/diamond_add_taxonomy", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for diamond_add_taxonomy", "latest": {"0.1.2--py36_0": "sha256:d9c9ab826eb2fd7cae507212f2540821b8ef88f5a12571d4cd2ecddae36c7b38"}, "tags": {"0.1.2--py36_0": "sha256:d9c9ab826eb2fd7cae507212f2540821b8ef88f5a12571d4cd2ecddae36c7b38"}, "docker": "quay.io/biocontainers/diamond_add_taxonomy"}
---

This module is a singularity container wrapper for quay.io/biocontainers/diamond_add_taxonomy.
shpc-registry automated BioContainers addition for diamond_add_taxonomy
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/diamond_add_taxonomy
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/diamond_add_taxonomy:0.1.2--py36_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/diamond_add_taxonomy/0.1.2--py36_0
$ module help quay.io/biocontainers/diamond_add_taxonomy/0.1.2--py36_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### diamond_add_taxonomy-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### diamond_add_taxonomy-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### diamond_add_taxonomy-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### diamond_add_taxonomy-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### diamond_add_taxonomy-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### diamond_add_taxonomy-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### diamond_add_taxonomy

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