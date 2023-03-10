---
layout: container
name:  "quay.io/biocontainers/bioconductor-htrat230pmcdf"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-htrat230pmcdf/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-htrat230pmcdf/container.yaml"
updated_at: "2023-01-13 03:23:11.419108"
latest: "2.18.0--r42hdfd78af_11"
container_url: "https://biocontainers.pro/tools/bioconductor-htrat230pmcdf"

versions:
 - "2.18.0--r41hdfd78af_9"
 - "2.18.0--r41hdfd78af_10"
 - "2.18.0--r42hdfd78af_11"
description: "shpc-registry automated BioContainers addition for bioconductor-htrat230pmcdf"
config: {"url": "https://biocontainers.pro/tools/bioconductor-htrat230pmcdf", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-htrat230pmcdf", "latest": {"2.18.0--r42hdfd78af_11": "sha256:caccb449017bc41d755c5308862e6cf4791298804b7f55138967499643a7a3e0"}, "tags": {"2.18.0--r41hdfd78af_9": "sha256:7ca8ad6f73d6a454b00caaa1484a37809b680d0e7d69172e133b642aaec9bc35", "2.18.0--r41hdfd78af_10": "sha256:f4f16707caa86cb9c8eee838f8024f9686842827c5798096c45a99e6fb6eb4b9", "2.18.0--r42hdfd78af_11": "sha256:caccb449017bc41d755c5308862e6cf4791298804b7f55138967499643a7a3e0"}, "docker": "quay.io/biocontainers/bioconductor-htrat230pmcdf"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-htrat230pmcdf.
shpc-registry automated BioContainers addition for bioconductor-htrat230pmcdf
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-htrat230pmcdf
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-htrat230pmcdf:2.18.0--r42hdfd78af_11
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-htrat230pmcdf/2.18.0--r42hdfd78af_11
$ module help quay.io/biocontainers/bioconductor-htrat230pmcdf/2.18.0--r42hdfd78af_11
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-htrat230pmcdf-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-htrat230pmcdf-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-htrat230pmcdf-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-htrat230pmcdf-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-htrat230pmcdf-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-htrat230pmcdf-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-htrat230pmcdf

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