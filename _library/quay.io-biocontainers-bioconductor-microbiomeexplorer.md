---
layout: container
name:  "quay.io/biocontainers/bioconductor-microbiomeexplorer"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-microbiomeexplorer/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-microbiomeexplorer/container.yaml"
updated_at: "2023-01-13 03:36:54.400379"
latest: "1.8.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-microbiomeexplorer"
aliases:
 - "pandoc"
versions:
 - "1.4.0--r41hdfd78af_0"
 - "1.8.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-microbiomeexplorer"
config: {"url": "https://biocontainers.pro/tools/bioconductor-microbiomeexplorer", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-microbiomeexplorer", "latest": {"1.8.0--r42hdfd78af_0": "sha256:d1a920e59a435108b8ae5ecd13a6dcfe4805eb8e3730610bffa4476a6dc96f40"}, "tags": {"1.4.0--r41hdfd78af_0": "sha256:5363ab9da69d8734647a0010ddb325d19a2265482eceda0e364c94ba01909701", "1.8.0--r42hdfd78af_0": "sha256:d1a920e59a435108b8ae5ecd13a6dcfe4805eb8e3730610bffa4476a6dc96f40"}, "docker": "quay.io/biocontainers/bioconductor-microbiomeexplorer", "aliases": {"pandoc": "/usr/local/bin/pandoc"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-microbiomeexplorer.
shpc-registry automated BioContainers addition for bioconductor-microbiomeexplorer
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-microbiomeexplorer
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-microbiomeexplorer:1.8.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-microbiomeexplorer/1.8.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-microbiomeexplorer/1.8.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-microbiomeexplorer-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-microbiomeexplorer-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-microbiomeexplorer-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-microbiomeexplorer-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-microbiomeexplorer-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-microbiomeexplorer-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### pandoc

```bash
$ singularity exec <container> /usr/local/bin/pandoc
$ podman run --it --rm --entrypoint /usr/local/bin/pandoc   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pandoc   -v ${PWD} -w ${PWD} <container> -c " $@"
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