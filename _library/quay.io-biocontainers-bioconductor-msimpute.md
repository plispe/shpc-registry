---
layout: container
name:  "quay.io/biocontainers/bioconductor-msimpute"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-msimpute/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-msimpute/container.yaml"
updated_at: "2023-01-13 03:04:42.150936"
latest: "1.8.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-msimpute"

versions:
 - "1.4.0--r41hdfd78af_0"
 - "1.8.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-msimpute"
config: {"url": "https://biocontainers.pro/tools/bioconductor-msimpute", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-msimpute", "latest": {"1.8.0--r42hdfd78af_0": "sha256:24e167f5f4a501e2561bac0dc76b65dad41ea35008feaac79952d34a26ab8b2e"}, "tags": {"1.4.0--r41hdfd78af_0": "sha256:4176ec6d112d6b28128199960353ae2b671cf5573d2b8a496e1b5f8f208ac399", "1.8.0--r42hdfd78af_0": "sha256:24e167f5f4a501e2561bac0dc76b65dad41ea35008feaac79952d34a26ab8b2e"}, "docker": "quay.io/biocontainers/bioconductor-msimpute"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-msimpute.
shpc-registry automated BioContainers addition for bioconductor-msimpute
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-msimpute
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-msimpute:1.8.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-msimpute/1.8.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-msimpute/1.8.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-msimpute-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-msimpute-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-msimpute-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-msimpute-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-msimpute-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-msimpute-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-msimpute

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