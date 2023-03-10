---
layout: container
name:  "quay.io/biocontainers/seqan3"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/seqan3/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/seqan3/container.yaml"
updated_at: "2023-01-13 03:42:23.834080"
latest: "3.2.0--hdfd78af_0"
container_url: "https://biocontainers.pro/tools/seqan3"

versions:
 - "3.2.0--hdfd78af_0"
description: "shpc-registry automated BioContainers addition for seqan3"
config: {"url": "https://biocontainers.pro/tools/seqan3", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for seqan3", "latest": {"3.2.0--hdfd78af_0": "sha256:8ff1046707a4f70ac1ba002e997cbac80056af4e8bdaa9f857e202ee79264483"}, "tags": {"3.2.0--hdfd78af_0": "sha256:8ff1046707a4f70ac1ba002e997cbac80056af4e8bdaa9f857e202ee79264483"}, "docker": "quay.io/biocontainers/seqan3"}
---

This module is a singularity container wrapper for quay.io/biocontainers/seqan3.
shpc-registry automated BioContainers addition for seqan3
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/seqan3
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/seqan3:3.2.0--hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/seqan3/3.2.0--hdfd78af_0
$ module help quay.io/biocontainers/seqan3/3.2.0--hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### seqan3-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### seqan3-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### seqan3-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### seqan3-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### seqan3-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### seqan3-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### seqan3

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