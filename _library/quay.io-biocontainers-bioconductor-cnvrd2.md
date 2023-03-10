---
layout: container
name:  "quay.io/biocontainers/bioconductor-cnvrd2"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-cnvrd2/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-cnvrd2/container.yaml"
updated_at: "2023-01-13 02:57:07.610757"
latest: "1.36.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-cnvrd2"
aliases:
 - "jags"
versions:
 - "1.32.0--r41hdfd78af_0"
 - "1.36.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-cnvrd2"
config: {"url": "https://biocontainers.pro/tools/bioconductor-cnvrd2", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-cnvrd2", "latest": {"1.36.0--r42hdfd78af_0": "sha256:d9f4956ebdfbbdd841de35f193bf828324493e5003970031f474041181e4a189"}, "tags": {"1.32.0--r41hdfd78af_0": "sha256:3d938bcc74b3631f4cb53021f5a12fefaa0470d4cbd162e49c76da5e888e63b5", "1.36.0--r42hdfd78af_0": "sha256:d9f4956ebdfbbdd841de35f193bf828324493e5003970031f474041181e4a189"}, "docker": "quay.io/biocontainers/bioconductor-cnvrd2", "aliases": {"jags": "/usr/local/bin/jags"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-cnvrd2.
shpc-registry automated BioContainers addition for bioconductor-cnvrd2
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-cnvrd2
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-cnvrd2:1.36.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-cnvrd2/1.36.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-cnvrd2/1.36.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-cnvrd2-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-cnvrd2-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-cnvrd2-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-cnvrd2-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-cnvrd2-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-cnvrd2-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### jags

```bash
$ singularity exec <container> /usr/local/bin/jags
$ podman run --it --rm --entrypoint /usr/local/bin/jags   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/jags   -v ${PWD} -w ${PWD} <container> -c " $@"
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