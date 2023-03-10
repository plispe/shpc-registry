---
layout: container
name:  "quay.io/biocontainers/bioconductor-gwas.bayes"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-gwas.bayes/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-gwas.bayes/container.yaml"
updated_at: "2023-01-13 02:47:59.861486"
latest: "1.8.0--r42hc247a5b_0"
container_url: "https://biocontainers.pro/tools/bioconductor-gwas.bayes"

versions:
 - "1.4.0--r41hc247a5b_2"
 - "1.8.0--r42hc247a5b_0"
description: "shpc-registry automated BioContainers addition for bioconductor-gwas.bayes"
config: {"url": "https://biocontainers.pro/tools/bioconductor-gwas.bayes", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-gwas.bayes", "latest": {"1.8.0--r42hc247a5b_0": "sha256:20c2f590f2d5d7713f393c5795cb14425b35892bb28ef37ee8f806c56f1cb9db"}, "tags": {"1.4.0--r41hc247a5b_2": "sha256:1035dbb14b6a300bf5e99cba295f63bdffb60d34c28ef9949abda4eaac5d9618", "1.8.0--r42hc247a5b_0": "sha256:20c2f590f2d5d7713f393c5795cb14425b35892bb28ef37ee8f806c56f1cb9db"}, "docker": "quay.io/biocontainers/bioconductor-gwas.bayes"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-gwas.bayes.
shpc-registry automated BioContainers addition for bioconductor-gwas.bayes
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-gwas.bayes
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-gwas.bayes:1.8.0--r42hc247a5b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-gwas.bayes/1.8.0--r42hc247a5b_0
$ module help quay.io/biocontainers/bioconductor-gwas.bayes/1.8.0--r42hc247a5b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-gwas.bayes-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-gwas.bayes-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-gwas.bayes-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-gwas.bayes-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-gwas.bayes-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-gwas.bayes-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-gwas.bayes

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