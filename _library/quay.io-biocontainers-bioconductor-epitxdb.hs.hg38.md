---
layout: container
name:  "quay.io/biocontainers/bioconductor-epitxdb.hs.hg38"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-epitxdb.hs.hg38/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-epitxdb.hs.hg38/container.yaml"
updated_at: "2023-01-13 03:30:34.974862"
latest: "0.99.7--r42hdfd78af_5"
container_url: "https://biocontainers.pro/tools/bioconductor-epitxdb.hs.hg38"

versions:
 - "0.99.7--r41hdfd78af_4"
 - "0.99.7--r42hdfd78af_5"
description: "shpc-registry automated BioContainers addition for bioconductor-epitxdb.hs.hg38"
config: {"url": "https://biocontainers.pro/tools/bioconductor-epitxdb.hs.hg38", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-epitxdb.hs.hg38", "latest": {"0.99.7--r42hdfd78af_5": "sha256:c4229a70f6496320029cb23654571d022e09cac9f0835ac8c26a340407891385"}, "tags": {"0.99.7--r41hdfd78af_4": "sha256:6850ddf51fab1a808105bd409175d30a03d150f63b549091462a112d3fe9e980", "0.99.7--r42hdfd78af_5": "sha256:c4229a70f6496320029cb23654571d022e09cac9f0835ac8c26a340407891385"}, "docker": "quay.io/biocontainers/bioconductor-epitxdb.hs.hg38"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-epitxdb.hs.hg38.
shpc-registry automated BioContainers addition for bioconductor-epitxdb.hs.hg38
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-epitxdb.hs.hg38
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-epitxdb.hs.hg38:0.99.7--r42hdfd78af_5
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-epitxdb.hs.hg38/0.99.7--r42hdfd78af_5
$ module help quay.io/biocontainers/bioconductor-epitxdb.hs.hg38/0.99.7--r42hdfd78af_5
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-epitxdb.hs.hg38-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-epitxdb.hs.hg38-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-epitxdb.hs.hg38-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-epitxdb.hs.hg38-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-epitxdb.hs.hg38-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-epitxdb.hs.hg38-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-epitxdb.hs.hg38

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