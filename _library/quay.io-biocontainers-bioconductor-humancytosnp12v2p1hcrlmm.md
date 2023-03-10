---
layout: container
name:  "quay.io/biocontainers/bioconductor-humancytosnp12v2p1hcrlmm"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-humancytosnp12v2p1hcrlmm/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-humancytosnp12v2p1hcrlmm/container.yaml"
updated_at: "2023-01-13 03:26:18.130444"
latest: "1.0.1--r42hdfd78af_10"
container_url: "https://biocontainers.pro/tools/bioconductor-humancytosnp12v2p1hcrlmm"

versions:
 - "1.0.1--r41hdfd78af_9"
 - "1.0.1--r42hdfd78af_10"
description: "shpc-registry automated BioContainers addition for bioconductor-humancytosnp12v2p1hcrlmm"
config: {"url": "https://biocontainers.pro/tools/bioconductor-humancytosnp12v2p1hcrlmm", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-humancytosnp12v2p1hcrlmm", "latest": {"1.0.1--r42hdfd78af_10": "sha256:847fe483d3d7acc2e3656035df572daf0c72328286011a458f79ff8df36006c2"}, "tags": {"1.0.1--r41hdfd78af_9": "sha256:d4263a908c63775addab11b179c4e9fae1b2021cc3d774a02c5270b3841e8e48", "1.0.1--r42hdfd78af_10": "sha256:847fe483d3d7acc2e3656035df572daf0c72328286011a458f79ff8df36006c2"}, "docker": "quay.io/biocontainers/bioconductor-humancytosnp12v2p1hcrlmm"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-humancytosnp12v2p1hcrlmm.
shpc-registry automated BioContainers addition for bioconductor-humancytosnp12v2p1hcrlmm
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-humancytosnp12v2p1hcrlmm
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-humancytosnp12v2p1hcrlmm:1.0.1--r42hdfd78af_10
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-humancytosnp12v2p1hcrlmm/1.0.1--r42hdfd78af_10
$ module help quay.io/biocontainers/bioconductor-humancytosnp12v2p1hcrlmm/1.0.1--r42hdfd78af_10
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-humancytosnp12v2p1hcrlmm-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-humancytosnp12v2p1hcrlmm-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-humancytosnp12v2p1hcrlmm-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-humancytosnp12v2p1hcrlmm-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-humancytosnp12v2p1hcrlmm-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-humancytosnp12v2p1hcrlmm-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-humancytosnp12v2p1hcrlmm

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