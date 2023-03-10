---
layout: container
name:  "quay.io/biocontainers/r-acidsinglecell"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/r-acidsinglecell/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/r-acidsinglecell/container.yaml"
updated_at: "2023-01-13 03:39:54.523274"
latest: "0.3.3--r42hdfd78af_1"
container_url: "https://biocontainers.pro/tools/r-acidsinglecell"

versions:
 - "0.2.0--r41hdfd78af_0"
 - "0.3.3--r42hdfd78af_1"
description: "shpc-registry automated BioContainers addition for r-acidsinglecell"
config: {"url": "https://biocontainers.pro/tools/r-acidsinglecell", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for r-acidsinglecell", "latest": {"0.3.3--r42hdfd78af_1": "sha256:2b15a88cf883b0e6df6f347feaf770c7ccab55af410e3d0144dbbd7d53c297ac"}, "tags": {"0.2.0--r41hdfd78af_0": "sha256:28547717f9ab2bbce71036b8347db6a2b766d568fd75f4cc4b865cdfa5f3b1f9", "0.3.3--r42hdfd78af_1": "sha256:2b15a88cf883b0e6df6f347feaf770c7ccab55af410e3d0144dbbd7d53c297ac"}, "docker": "quay.io/biocontainers/r-acidsinglecell"}
---

This module is a singularity container wrapper for quay.io/biocontainers/r-acidsinglecell.
shpc-registry automated BioContainers addition for r-acidsinglecell
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/r-acidsinglecell
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/r-acidsinglecell:0.3.3--r42hdfd78af_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/r-acidsinglecell/0.3.3--r42hdfd78af_1
$ module help quay.io/biocontainers/r-acidsinglecell/0.3.3--r42hdfd78af_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### r-acidsinglecell-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### r-acidsinglecell-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### r-acidsinglecell-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### r-acidsinglecell-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### r-acidsinglecell-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### r-acidsinglecell-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### r-acidsinglecell

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