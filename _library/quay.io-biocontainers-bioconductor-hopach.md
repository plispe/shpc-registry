---
layout: container
name:  "quay.io/biocontainers/bioconductor-hopach"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-hopach/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-hopach/container.yaml"
updated_at: "2023-01-13 03:08:28.508597"
latest: "2.58.0--r42hc0cfd56_0"
container_url: "https://biocontainers.pro/tools/bioconductor-hopach"

versions:
 - "2.54.0--r41hc0cfd56_2"
 - "2.58.0--r42hc0cfd56_0"
description: "shpc-registry automated BioContainers addition for bioconductor-hopach"
config: {"url": "https://biocontainers.pro/tools/bioconductor-hopach", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-hopach", "latest": {"2.58.0--r42hc0cfd56_0": "sha256:2927cdcb00fb64ab8434f33f3437e26e58fa9679af9bcd2e7cf68ac92d140bef"}, "tags": {"2.54.0--r41hc0cfd56_2": "sha256:a9ada561104f5a197859106c33e5f516830d3e3a3b5611382cc851179ef083c1", "2.58.0--r42hc0cfd56_0": "sha256:2927cdcb00fb64ab8434f33f3437e26e58fa9679af9bcd2e7cf68ac92d140bef"}, "docker": "quay.io/biocontainers/bioconductor-hopach"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-hopach.
shpc-registry automated BioContainers addition for bioconductor-hopach
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-hopach
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-hopach:2.58.0--r42hc0cfd56_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-hopach/2.58.0--r42hc0cfd56_0
$ module help quay.io/biocontainers/bioconductor-hopach/2.58.0--r42hc0cfd56_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-hopach-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-hopach-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-hopach-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-hopach-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-hopach-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-hopach-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-hopach

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