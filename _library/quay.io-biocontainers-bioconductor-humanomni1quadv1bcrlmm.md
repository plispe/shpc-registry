---
layout: container
name:  "quay.io/biocontainers/bioconductor-humanomni1quadv1bcrlmm"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-humanomni1quadv1bcrlmm/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-humanomni1quadv1bcrlmm/container.yaml"
updated_at: "2023-01-13 02:50:11.707091"
latest: "1.0.3--r42hdfd78af_10"
container_url: "https://biocontainers.pro/tools/bioconductor-humanomni1quadv1bcrlmm"

versions:
 - "1.0.3--r41hdfd78af_9"
 - "1.0.3--r42hdfd78af_10"
description: "shpc-registry automated BioContainers addition for bioconductor-humanomni1quadv1bcrlmm"
config: {"url": "https://biocontainers.pro/tools/bioconductor-humanomni1quadv1bcrlmm", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-humanomni1quadv1bcrlmm", "latest": {"1.0.3--r42hdfd78af_10": "sha256:21eddd87569efb630626a02e5148dcc327ec0869cedc33a349549e69be4e37d6"}, "tags": {"1.0.3--r41hdfd78af_9": "sha256:15c13c93e95357ceacc2f389bbdaa8bc9aa2413422525b016a9fc62519992b70", "1.0.3--r42hdfd78af_10": "sha256:21eddd87569efb630626a02e5148dcc327ec0869cedc33a349549e69be4e37d6"}, "docker": "quay.io/biocontainers/bioconductor-humanomni1quadv1bcrlmm"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-humanomni1quadv1bcrlmm.
shpc-registry automated BioContainers addition for bioconductor-humanomni1quadv1bcrlmm
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-humanomni1quadv1bcrlmm
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-humanomni1quadv1bcrlmm:1.0.3--r42hdfd78af_10
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-humanomni1quadv1bcrlmm/1.0.3--r42hdfd78af_10
$ module help quay.io/biocontainers/bioconductor-humanomni1quadv1bcrlmm/1.0.3--r42hdfd78af_10
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-humanomni1quadv1bcrlmm-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-humanomni1quadv1bcrlmm-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-humanomni1quadv1bcrlmm-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-humanomni1quadv1bcrlmm-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-humanomni1quadv1bcrlmm-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-humanomni1quadv1bcrlmm-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-humanomni1quadv1bcrlmm

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