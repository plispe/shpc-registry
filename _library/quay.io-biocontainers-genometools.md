---
layout: container
name:  "quay.io/biocontainers/genometools"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/genometools/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/genometools/container.yaml"
updated_at: "2023-01-13 03:01:41.774733"
latest: "1.2.1--py27_0"
container_url: "https://biocontainers.pro/tools/genometools"

versions:
 - "1.2.1--py27_0"
description: "shpc-registry automated BioContainers addition for genometools"
config: {"url": "https://biocontainers.pro/tools/genometools", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for genometools", "latest": {"1.2.1--py27_0": "sha256:59a28d8a230f7a503ad13680b118da06ce7d9d6425723af3a9a4ce45ab80ea75"}, "tags": {"1.2.1--py27_0": "sha256:59a28d8a230f7a503ad13680b118da06ce7d9d6425723af3a9a4ce45ab80ea75"}, "docker": "quay.io/biocontainers/genometools"}
---

This module is a singularity container wrapper for quay.io/biocontainers/genometools.
shpc-registry automated BioContainers addition for genometools
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/genometools
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/genometools:1.2.1--py27_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/genometools/1.2.1--py27_0
$ module help quay.io/biocontainers/genometools/1.2.1--py27_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### genometools-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### genometools-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### genometools-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### genometools-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### genometools-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### genometools-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### genometools

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