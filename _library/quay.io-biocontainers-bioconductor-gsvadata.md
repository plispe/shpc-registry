---
layout: container
name:  "quay.io/biocontainers/bioconductor-gsvadata"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-gsvadata/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-gsvadata/container.yaml"
updated_at: "2023-01-13 03:10:27.398858"
latest: "1.34.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-gsvadata"

versions:
 - "1.30.0--r41hdfd78af_1"
 - "1.34.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-gsvadata"
config: {"url": "https://biocontainers.pro/tools/bioconductor-gsvadata", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-gsvadata", "latest": {"1.34.0--r42hdfd78af_0": "sha256:6b884bae8568e50aad08cb0101ff964e99f7019a10052b29a7b7585a54891ffc"}, "tags": {"1.30.0--r41hdfd78af_1": "sha256:f639b52895e384cf2759943bee6ed76fb1f857fe23bc8990c4182658039f5082", "1.34.0--r42hdfd78af_0": "sha256:6b884bae8568e50aad08cb0101ff964e99f7019a10052b29a7b7585a54891ffc"}, "docker": "quay.io/biocontainers/bioconductor-gsvadata"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-gsvadata.
shpc-registry automated BioContainers addition for bioconductor-gsvadata
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-gsvadata
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-gsvadata:1.34.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-gsvadata/1.34.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-gsvadata/1.34.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-gsvadata-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-gsvadata-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-gsvadata-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-gsvadata-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-gsvadata-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-gsvadata-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-gsvadata

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