---
layout: container
name:  "quay.io/biocontainers/bioconductor-rnbeads.mm9"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-rnbeads.mm9/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-rnbeads.mm9/container.yaml"
updated_at: "2023-01-13 03:39:37.278027"
latest: "1.30.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-rnbeads.mm9"

versions:
 - "1.26.0--r41hdfd78af_1"
 - "1.30.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-rnbeads.mm9"
config: {"url": "https://biocontainers.pro/tools/bioconductor-rnbeads.mm9", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-rnbeads.mm9", "latest": {"1.30.0--r42hdfd78af_0": "sha256:d68729d958ff5f34dc78fe6c996bd659877d1ddd6a07541e89e7843e32148803"}, "tags": {"1.26.0--r41hdfd78af_1": "sha256:632a7104529b462dbabce50d1ff43a01fc9b6ff9f3383f49e1bdde747db47fd6", "1.30.0--r42hdfd78af_0": "sha256:d68729d958ff5f34dc78fe6c996bd659877d1ddd6a07541e89e7843e32148803"}, "docker": "quay.io/biocontainers/bioconductor-rnbeads.mm9"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-rnbeads.mm9.
shpc-registry automated BioContainers addition for bioconductor-rnbeads.mm9
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-rnbeads.mm9
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-rnbeads.mm9:1.30.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-rnbeads.mm9/1.30.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-rnbeads.mm9/1.30.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-rnbeads.mm9-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-rnbeads.mm9-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-rnbeads.mm9-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-rnbeads.mm9-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-rnbeads.mm9-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-rnbeads.mm9-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-rnbeads.mm9

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