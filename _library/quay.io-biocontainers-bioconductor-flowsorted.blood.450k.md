---
layout: container
name:  "quay.io/biocontainers/bioconductor-flowsorted.blood.450k"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-flowsorted.blood.450k/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-flowsorted.blood.450k/container.yaml"
updated_at: "2023-01-13 03:42:09.827634"
latest: "1.36.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-flowsorted.blood.450k"

versions:
 - "1.32.0--r41hdfd78af_1"
 - "1.36.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-flowsorted.blood.450k"
config: {"url": "https://biocontainers.pro/tools/bioconductor-flowsorted.blood.450k", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-flowsorted.blood.450k", "latest": {"1.36.0--r42hdfd78af_0": "sha256:df93fc9dc24aaa095131f8cbc43eade7deb04d66cb00ba5c9e4d3d816a081c6b"}, "tags": {"1.32.0--r41hdfd78af_1": "sha256:c5d6da9dcd0730f4cf0a7e377bd90d40b627061e5488ed82d5bb35c3954a28de", "1.36.0--r42hdfd78af_0": "sha256:df93fc9dc24aaa095131f8cbc43eade7deb04d66cb00ba5c9e4d3d816a081c6b"}, "docker": "quay.io/biocontainers/bioconductor-flowsorted.blood.450k"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-flowsorted.blood.450k.
shpc-registry automated BioContainers addition for bioconductor-flowsorted.blood.450k
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-flowsorted.blood.450k
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-flowsorted.blood.450k:1.36.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-flowsorted.blood.450k/1.36.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-flowsorted.blood.450k/1.36.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-flowsorted.blood.450k-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-flowsorted.blood.450k-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-flowsorted.blood.450k-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-flowsorted.blood.450k-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-flowsorted.blood.450k-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-flowsorted.blood.450k-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-flowsorted.blood.450k

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