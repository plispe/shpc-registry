---
layout: container
name:  "quay.io/biocontainers/bioconductor-derfinderdata"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-derfinderdata/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-derfinderdata/container.yaml"
updated_at: "2023-01-13 03:30:53.397069"
latest: "2.15.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-derfinderdata"
aliases:
 - "x86_64-conda-linux-gnu-gfortran.bin"
versions:
 - "2.8.1--r40hdfd78af_0"
 - "2.15.0--r42hdfd78af_0"
 - "2.12.0--r41hdfd78af_1"
 - "2.10.0--r41hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-derfinderdata"
config: {"url": "https://biocontainers.pro/tools/bioconductor-derfinderdata", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-derfinderdata", "latest": {"2.15.0--r42hdfd78af_0": "sha256:961ab413e27ebd7cf6325dbc9f87f4ee5ec894f93dfccb107b456afa60db8808"}, "tags": {"2.8.1--r40hdfd78af_0": "sha256:73228542504179377e475b57bce07216699f9fc4580b0294b3c89d7814562178", "2.15.0--r42hdfd78af_0": "sha256:961ab413e27ebd7cf6325dbc9f87f4ee5ec894f93dfccb107b456afa60db8808", "2.12.0--r41hdfd78af_1": "sha256:4fe2fa647acf3cf33046ccd9023f649c6f675eba5ed39a1cf468111d4c1e714b", "2.10.0--r41hdfd78af_0": "sha256:9e8514ecd08eadeda1639557beb1f67ee6c75a573bc34e788033d5f2f2af7d63"}, "docker": "quay.io/biocontainers/bioconductor-derfinderdata", "aliases": {"x86_64-conda-linux-gnu-gfortran.bin": "/usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-derfinderdata.
shpc-registry automated BioContainers addition for bioconductor-derfinderdata
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-derfinderdata
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-derfinderdata:2.15.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-derfinderdata/2.15.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-derfinderdata/2.15.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-derfinderdata-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-derfinderdata-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-derfinderdata-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-derfinderdata-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-derfinderdata-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-derfinderdata-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### x86_64-conda-linux-gnu-gfortran.bin

```bash
$ singularity exec <container> /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin
$ podman run --it --rm --entrypoint /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin   -v ${PWD} -w ${PWD} <container> -c " $@"
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