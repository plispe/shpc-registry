---
layout: container
name:  "quay.io/biocontainers/bioconductor-r3cpet"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-r3cpet/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-r3cpet/container.yaml"
updated_at: "2023-01-13 03:15:25.370977"
latest: "1.30.0--r42hc247a5b_0"
container_url: "https://biocontainers.pro/tools/bioconductor-r3cpet"
aliases:
 - "glpsol"
versions:
 - "1.26.0--r41hc247a5b_3"
 - "1.30.0--r42hc247a5b_0"
description: "shpc-registry automated BioContainers addition for bioconductor-r3cpet"
config: {"url": "https://biocontainers.pro/tools/bioconductor-r3cpet", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-r3cpet", "latest": {"1.30.0--r42hc247a5b_0": "sha256:673eb791a5aeb6a3b2ebec18facb5d1b3236971df5c786eb03347dd48499269b"}, "tags": {"1.26.0--r41hc247a5b_3": "sha256:471eecbf6441e29722e94829a2ee8638150f4b23077d75488823eb16af0a59aa", "1.30.0--r42hc247a5b_0": "sha256:673eb791a5aeb6a3b2ebec18facb5d1b3236971df5c786eb03347dd48499269b"}, "docker": "quay.io/biocontainers/bioconductor-r3cpet", "aliases": {"glpsol": "/usr/local/bin/glpsol"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-r3cpet.
shpc-registry automated BioContainers addition for bioconductor-r3cpet
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-r3cpet
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-r3cpet:1.30.0--r42hc247a5b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-r3cpet/1.30.0--r42hc247a5b_0
$ module help quay.io/biocontainers/bioconductor-r3cpet/1.30.0--r42hc247a5b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-r3cpet-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-r3cpet-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-r3cpet-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-r3cpet-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-r3cpet-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-r3cpet-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### glpsol

```bash
$ singularity exec <container> /usr/local/bin/glpsol
$ podman run --it --rm --entrypoint /usr/local/bin/glpsol   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/glpsol   -v ${PWD} -w ${PWD} <container> -c " $@"
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