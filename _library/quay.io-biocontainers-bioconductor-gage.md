---
layout: container
name:  "quay.io/biocontainers/bioconductor-gage"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-gage/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-gage/container.yaml"
updated_at: "2023-01-13 02:58:01.828545"
latest: "2.48.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-gage"

versions:
 - "2.44.0--r41hdfd78af_0"
 - "2.48.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-gage"
config: {"url": "https://biocontainers.pro/tools/bioconductor-gage", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-gage", "latest": {"2.48.0--r42hdfd78af_0": "sha256:bd2e963c1b5fe48ee04991fddd191fcb7d78ea82c0e3ade9cab14441e222c1e1"}, "tags": {"2.44.0--r41hdfd78af_0": "sha256:0a2558bb748ae2e2de215ba08672c195cbf7879339c884440b191b74823d2e46", "2.48.0--r42hdfd78af_0": "sha256:bd2e963c1b5fe48ee04991fddd191fcb7d78ea82c0e3ade9cab14441e222c1e1"}, "docker": "quay.io/biocontainers/bioconductor-gage"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-gage.
shpc-registry automated BioContainers addition for bioconductor-gage
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-gage
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-gage:2.48.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-gage/2.48.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-gage/2.48.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-gage-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-gage-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-gage-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-gage-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-gage-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-gage-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-gage

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