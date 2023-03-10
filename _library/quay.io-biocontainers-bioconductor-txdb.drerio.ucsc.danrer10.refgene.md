---
layout: container
name:  "quay.io/biocontainers/bioconductor-txdb.drerio.ucsc.danrer10.refgene"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-txdb.drerio.ucsc.danrer10.refgene/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-txdb.drerio.ucsc.danrer10.refgene/container.yaml"
updated_at: "2023-01-13 03:34:47.264424"
latest: "3.4.6--r42hdfd78af_9"
container_url: "https://biocontainers.pro/tools/bioconductor-txdb.drerio.ucsc.danrer10.refgene"

versions:
 - "3.4.6--r41hdfd78af_8"
 - "3.4.6--r42hdfd78af_9"
description: "shpc-registry automated BioContainers addition for bioconductor-txdb.drerio.ucsc.danrer10.refgene"
config: {"url": "https://biocontainers.pro/tools/bioconductor-txdb.drerio.ucsc.danrer10.refgene", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-txdb.drerio.ucsc.danrer10.refgene", "latest": {"3.4.6--r42hdfd78af_9": "sha256:1e7fbc1a5363defa46c224714ea9c81b87a9e17cc736c0f3f9be21c1e72d2ed1"}, "tags": {"3.4.6--r41hdfd78af_8": "sha256:d7e6136c54c794171f29e91b9c22e8800ffd898e5644b0d64bde57e5186eee20", "3.4.6--r42hdfd78af_9": "sha256:1e7fbc1a5363defa46c224714ea9c81b87a9e17cc736c0f3f9be21c1e72d2ed1"}, "docker": "quay.io/biocontainers/bioconductor-txdb.drerio.ucsc.danrer10.refgene"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-txdb.drerio.ucsc.danrer10.refgene.
shpc-registry automated BioContainers addition for bioconductor-txdb.drerio.ucsc.danrer10.refgene
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-txdb.drerio.ucsc.danrer10.refgene
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-txdb.drerio.ucsc.danrer10.refgene:3.4.6--r42hdfd78af_9
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-txdb.drerio.ucsc.danrer10.refgene/3.4.6--r42hdfd78af_9
$ module help quay.io/biocontainers/bioconductor-txdb.drerio.ucsc.danrer10.refgene/3.4.6--r42hdfd78af_9
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-txdb.drerio.ucsc.danrer10.refgene-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-txdb.drerio.ucsc.danrer10.refgene-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-txdb.drerio.ucsc.danrer10.refgene-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-txdb.drerio.ucsc.danrer10.refgene-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-txdb.drerio.ucsc.danrer10.refgene-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-txdb.drerio.ucsc.danrer10.refgene-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-txdb.drerio.ucsc.danrer10.refgene

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