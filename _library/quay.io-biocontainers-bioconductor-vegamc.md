---
layout: container
name:  "quay.io/biocontainers/bioconductor-vegamc"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-vegamc/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-vegamc/container.yaml"
updated_at: "2023-01-13 03:29:35.817230"
latest: "3.36.0--r42hc0cfd56_0"
container_url: "https://biocontainers.pro/tools/bioconductor-vegamc"

versions:
 - "3.32.0--r41hc0cfd56_2"
 - "3.36.0--r42hc0cfd56_0"
description: "shpc-registry automated BioContainers addition for bioconductor-vegamc"
config: {"url": "https://biocontainers.pro/tools/bioconductor-vegamc", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-vegamc", "latest": {"3.36.0--r42hc0cfd56_0": "sha256:8d9df5a17ab3d60b59ce00bb91baf0bc24e8232c6c678773c3e838a715fff28a"}, "tags": {"3.32.0--r41hc0cfd56_2": "sha256:1b40ecae1fd4f39679f129563b7287b702f0200ff80d1e94fd4738f6df5e2a31", "3.36.0--r42hc0cfd56_0": "sha256:8d9df5a17ab3d60b59ce00bb91baf0bc24e8232c6c678773c3e838a715fff28a"}, "docker": "quay.io/biocontainers/bioconductor-vegamc"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-vegamc.
shpc-registry automated BioContainers addition for bioconductor-vegamc
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-vegamc
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-vegamc:3.36.0--r42hc0cfd56_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-vegamc/3.36.0--r42hc0cfd56_0
$ module help quay.io/biocontainers/bioconductor-vegamc/3.36.0--r42hc0cfd56_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-vegamc-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-vegamc-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-vegamc-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-vegamc-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-vegamc-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-vegamc-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-vegamc

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