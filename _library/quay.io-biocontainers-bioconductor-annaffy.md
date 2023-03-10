---
layout: container
name:  "quay.io/biocontainers/bioconductor-annaffy"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-annaffy/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-annaffy/container.yaml"
updated_at: "2023-01-13 03:31:41.960394"
latest: "1.70.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-annaffy"

versions:
 - "1.66.0--r41hdfd78af_0"
 - "1.70.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-annaffy"
config: {"url": "https://biocontainers.pro/tools/bioconductor-annaffy", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-annaffy", "latest": {"1.70.0--r42hdfd78af_0": "sha256:3f614fe39298f3a873ce71f23806b2bcc57b3560d8f958ac011808ecd9716d74"}, "tags": {"1.66.0--r41hdfd78af_0": "sha256:51e06e818cb194e9d049f0165266217da7e2f0ec9e8cd2ea97c430b282708eb6", "1.70.0--r42hdfd78af_0": "sha256:3f614fe39298f3a873ce71f23806b2bcc57b3560d8f958ac011808ecd9716d74"}, "docker": "quay.io/biocontainers/bioconductor-annaffy"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-annaffy.
shpc-registry automated BioContainers addition for bioconductor-annaffy
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-annaffy
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-annaffy:1.70.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-annaffy/1.70.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-annaffy/1.70.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-annaffy-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-annaffy-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-annaffy-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-annaffy-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-annaffy-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-annaffy-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-annaffy

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