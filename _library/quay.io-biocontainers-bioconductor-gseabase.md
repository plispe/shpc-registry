---
layout: container
name:  "quay.io/biocontainers/bioconductor-gseabase"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-gseabase/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-gseabase/container.yaml"
updated_at: "2023-01-13 02:53:45.727978"
latest: "1.60.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-gseabase"

versions:
 - "1.56.0--r41hdfd78af_0"
 - "1.60.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-gseabase"
config: {"url": "https://biocontainers.pro/tools/bioconductor-gseabase", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-gseabase", "latest": {"1.60.0--r42hdfd78af_0": "sha256:f60024cc99a506b35159fc3eed41ad2a19889a7da2f2e032e946b04457f07e59"}, "tags": {"1.56.0--r41hdfd78af_0": "sha256:7c6f35899aaf29007ab48d1318fc520cb962b318087b28ffcf47334307044802", "1.60.0--r42hdfd78af_0": "sha256:f60024cc99a506b35159fc3eed41ad2a19889a7da2f2e032e946b04457f07e59"}, "docker": "quay.io/biocontainers/bioconductor-gseabase"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-gseabase.
shpc-registry automated BioContainers addition for bioconductor-gseabase
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-gseabase
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-gseabase:1.60.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-gseabase/1.60.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-gseabase/1.60.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-gseabase-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-gseabase-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-gseabase-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-gseabase-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-gseabase-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-gseabase-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-gseabase

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