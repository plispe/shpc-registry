---
layout: container
name:  "quay.io/biocontainers/bioconductor-muscle"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-muscle/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-muscle/container.yaml"
updated_at: "2023-01-13 03:39:24.130141"
latest: "3.40.0--r42hc247a5b_0"
container_url: "https://biocontainers.pro/tools/bioconductor-muscle"

versions:
 - "3.36.0--r41hc247a5b_2"
 - "3.40.0--r42hc247a5b_0"
description: "shpc-registry automated BioContainers addition for bioconductor-muscle"
config: {"url": "https://biocontainers.pro/tools/bioconductor-muscle", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-muscle", "latest": {"3.40.0--r42hc247a5b_0": "sha256:1e65564055c026d4dceec663ac41c92b82d99aa7c767a4cdbe98186fce247746"}, "tags": {"3.36.0--r41hc247a5b_2": "sha256:1904411d39d7c00dbf18cef33c82180ce03eec476ea7b87e2e34c220e81bdf57", "3.40.0--r42hc247a5b_0": "sha256:1e65564055c026d4dceec663ac41c92b82d99aa7c767a4cdbe98186fce247746"}, "docker": "quay.io/biocontainers/bioconductor-muscle"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-muscle.
shpc-registry automated BioContainers addition for bioconductor-muscle
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-muscle
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-muscle:3.40.0--r42hc247a5b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-muscle/3.40.0--r42hc247a5b_0
$ module help quay.io/biocontainers/bioconductor-muscle/3.40.0--r42hc247a5b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-muscle-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-muscle-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-muscle-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-muscle-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-muscle-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-muscle-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-muscle

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