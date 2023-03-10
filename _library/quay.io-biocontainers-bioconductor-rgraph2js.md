---
layout: container
name:  "quay.io/biocontainers/bioconductor-rgraph2js"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-rgraph2js/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-rgraph2js/container.yaml"
updated_at: "2023-01-13 03:21:45.598219"
latest: "1.26.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-rgraph2js"

versions:
 - "1.8.0--r351_0"
 - "1.26.0--r42hdfd78af_0"
 - "1.22.0--r41hdfd78af_0"
 - "1.20.0--r41hdfd78af_0"
 - "1.18.0--r40hdfd78af_1"
 - "1.16.0--r40_0"
description: "shpc-registry automated BioContainers addition for bioconductor-rgraph2js"
config: {"url": "https://biocontainers.pro/tools/bioconductor-rgraph2js", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-rgraph2js", "latest": {"1.26.0--r42hdfd78af_0": "sha256:c707162d9acee948ee31432cdb4bc89b7e38fa1537584b9d1fbc231fd09beca3"}, "tags": {"1.8.0--r351_0": "sha256:3f91db46e2a9c38090b552a20bad405a2e6fc52790389e5df9fcbb62491f1bb0", "1.26.0--r42hdfd78af_0": "sha256:c707162d9acee948ee31432cdb4bc89b7e38fa1537584b9d1fbc231fd09beca3", "1.22.0--r41hdfd78af_0": "sha256:7a900d08b116d09af0f0b53c1579bd12f364c337484a95505024b162087ed742", "1.20.0--r41hdfd78af_0": "sha256:047f383ddfeaf53dca9304a9aacab38248ee07a8c95a2f195a783d52379844fd", "1.18.0--r40hdfd78af_1": "sha256:06be7a061857d86c05f0aed1d3b3253ae27e56e0500a4c2074bc96d24fd9b10e", "1.16.0--r40_0": "sha256:9ae5c4d62d421da4b4c3d170f8cc3b0b6c2ec71cede5edfd129530af93a2f252"}, "docker": "quay.io/biocontainers/bioconductor-rgraph2js"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-rgraph2js.
shpc-registry automated BioContainers addition for bioconductor-rgraph2js
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-rgraph2js
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-rgraph2js:1.26.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-rgraph2js/1.26.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-rgraph2js/1.26.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-rgraph2js-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-rgraph2js-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-rgraph2js-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-rgraph2js-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-rgraph2js-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-rgraph2js-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-rgraph2js

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