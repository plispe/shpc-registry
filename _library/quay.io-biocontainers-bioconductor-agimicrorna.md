---
layout: container
name:  "quay.io/biocontainers/bioconductor-agimicrorna"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-agimicrorna/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-agimicrorna/container.yaml"
updated_at: "2023-01-13 03:27:16.436677"
latest: "2.48.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-agimicrorna"

versions:
 - "2.44.0--r41hdfd78af_0"
 - "2.48.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-agimicrorna"
config: {"url": "https://biocontainers.pro/tools/bioconductor-agimicrorna", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-agimicrorna", "latest": {"2.48.0--r42hdfd78af_0": "sha256:ce875c2ae3dfcdeda5f4d7c04dfde461288977e22ba270cc6a4807fb643efb41"}, "tags": {"2.44.0--r41hdfd78af_0": "sha256:ebb035fb858af4cd62788acf63ac2c8307f68ca7705ebb52850e8171cf1076ad", "2.48.0--r42hdfd78af_0": "sha256:ce875c2ae3dfcdeda5f4d7c04dfde461288977e22ba270cc6a4807fb643efb41"}, "docker": "quay.io/biocontainers/bioconductor-agimicrorna"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-agimicrorna.
shpc-registry automated BioContainers addition for bioconductor-agimicrorna
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-agimicrorna
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-agimicrorna:2.48.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-agimicrorna/2.48.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-agimicrorna/2.48.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-agimicrorna-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-agimicrorna-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-agimicrorna-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-agimicrorna-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-agimicrorna-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-agimicrorna-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-agimicrorna

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