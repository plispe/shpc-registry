---
layout: container
name:  "quay.io/biocontainers/tbb"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/tbb/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/tbb/container.yaml"
updated_at: "2023-01-13 03:09:18.588025"
latest: "4.4_20150728--0"
container_url: "https://biocontainers.pro/tools/tbb"

versions:
 - "4.4_20150728--0"
description: "shpc-registry automated BioContainers addition for tbb"
config: {"url": "https://biocontainers.pro/tools/tbb", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for tbb", "latest": {"4.4_20150728--0": "sha256:ddf897ca939f561a5a0565cc1ad9b6540d6791486e2cec51900d4f259b57fe01"}, "tags": {"4.4_20150728--0": "sha256:ddf897ca939f561a5a0565cc1ad9b6540d6791486e2cec51900d4f259b57fe01"}, "docker": "quay.io/biocontainers/tbb"}
---

This module is a singularity container wrapper for quay.io/biocontainers/tbb.
shpc-registry automated BioContainers addition for tbb
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/tbb
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/tbb:4.4_20150728--0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/tbb/4.4_20150728--0
$ module help quay.io/biocontainers/tbb/4.4_20150728--0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### tbb-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### tbb-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### tbb-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### tbb-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### tbb-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### tbb-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### tbb

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