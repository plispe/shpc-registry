---
layout: container
name:  "quay.io/biocontainers/bioconductor-microbiomemarker"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-microbiomemarker/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-microbiomemarker/container.yaml"
updated_at: "2023-01-13 03:24:17.536326"
latest: "1.4.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-microbiomemarker"

versions:
 - "1.0.0--r41hdfd78af_0"
 - "1.4.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-microbiomemarker"
config: {"url": "https://biocontainers.pro/tools/bioconductor-microbiomemarker", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-microbiomemarker", "latest": {"1.4.0--r42hdfd78af_0": "sha256:5037955f5c9332544d3cf7faa7a38988b545ce5739fab764b9499f37bf9b793e"}, "tags": {"1.0.0--r41hdfd78af_0": "sha256:3a9837f375c2fe4093c4c33208c969bcbd38daed0716b6c7b0ae7d002a67114d", "1.4.0--r42hdfd78af_0": "sha256:5037955f5c9332544d3cf7faa7a38988b545ce5739fab764b9499f37bf9b793e"}, "docker": "quay.io/biocontainers/bioconductor-microbiomemarker"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-microbiomemarker.
shpc-registry automated BioContainers addition for bioconductor-microbiomemarker
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-microbiomemarker
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-microbiomemarker:1.4.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-microbiomemarker/1.4.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-microbiomemarker/1.4.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-microbiomemarker-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-microbiomemarker-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-microbiomemarker-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-microbiomemarker-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-microbiomemarker-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-microbiomemarker-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-microbiomemarker

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