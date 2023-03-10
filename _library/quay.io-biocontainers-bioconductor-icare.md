---
layout: container
name:  "quay.io/biocontainers/bioconductor-icare"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-icare/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-icare/container.yaml"
updated_at: "2023-01-13 03:22:58.896809"
latest: "1.26.0--r42hc0cfd56_0"
container_url: "https://biocontainers.pro/tools/bioconductor-icare"

versions:
 - "1.22.0--r41hc0cfd56_2"
 - "1.26.0--r42hc0cfd56_0"
description: "shpc-registry automated BioContainers addition for bioconductor-icare"
config: {"url": "https://biocontainers.pro/tools/bioconductor-icare", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-icare", "latest": {"1.26.0--r42hc0cfd56_0": "sha256:bb5667c3e2a30891dfb825d7b9473df888f3cea16d75391a1e73913c54c67e00"}, "tags": {"1.22.0--r41hc0cfd56_2": "sha256:d96ca382cd12cae3d1da3fbd175563650e5da2715a8cdb0bc760ec2b2df65813", "1.26.0--r42hc0cfd56_0": "sha256:bb5667c3e2a30891dfb825d7b9473df888f3cea16d75391a1e73913c54c67e00"}, "docker": "quay.io/biocontainers/bioconductor-icare"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-icare.
shpc-registry automated BioContainers addition for bioconductor-icare
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-icare
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-icare:1.26.0--r42hc0cfd56_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-icare/1.26.0--r42hc0cfd56_0
$ module help quay.io/biocontainers/bioconductor-icare/1.26.0--r42hc0cfd56_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-icare-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-icare-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-icare-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-icare-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-icare-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-icare-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-icare

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