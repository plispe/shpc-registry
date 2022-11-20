---
layout: container
name:  "quay.io/biocontainers/bioconductor-drivernet"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-drivernet/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-drivernet/container.yaml"
updated_at: "2022-11-20 00:58:05.132593"
latest: "1.34.0--r41hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-drivernet"

versions:
 - "1.34.0--r41hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-drivernet"
config: {"url": "https://biocontainers.pro/tools/bioconductor-drivernet", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-drivernet", "latest": {"1.34.0--r41hdfd78af_0": "sha256:1c37126ab6b558d916024e333c5e3152ea8449121a8fca192f2577f7a0b7cc6d"}, "tags": {"1.34.0--r41hdfd78af_0": "sha256:1c37126ab6b558d916024e333c5e3152ea8449121a8fca192f2577f7a0b7cc6d"}, "docker": "quay.io/biocontainers/bioconductor-drivernet"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-drivernet.
shpc-registry automated BioContainers addition for bioconductor-drivernet
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-drivernet
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-drivernet:1.34.0--r41hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-drivernet/1.34.0--r41hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-drivernet/1.34.0--r41hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-drivernet-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-drivernet-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-drivernet-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-drivernet-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-drivernet-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-drivernet-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-drivernet

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