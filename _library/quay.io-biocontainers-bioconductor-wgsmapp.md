---
layout: container
name:  "quay.io/biocontainers/bioconductor-wgsmapp"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-wgsmapp/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-wgsmapp/container.yaml"
updated_at: "2023-01-13 03:10:05.678034"
latest: "1.10.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-wgsmapp"

versions:
 - "1.6.0--r41hdfd78af_1"
 - "1.10.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-wgsmapp"
config: {"url": "https://biocontainers.pro/tools/bioconductor-wgsmapp", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-wgsmapp", "latest": {"1.10.0--r42hdfd78af_0": "sha256:f4a84e0e6a27b60ed8c20e2c866776203c8a2849dea5004e747bb29241902314"}, "tags": {"1.6.0--r41hdfd78af_1": "sha256:93e8e9b35fcd9fd19002c1bf0f781a9f47d408640bcc4ef3fb0c25538fe71662", "1.10.0--r42hdfd78af_0": "sha256:f4a84e0e6a27b60ed8c20e2c866776203c8a2849dea5004e747bb29241902314"}, "docker": "quay.io/biocontainers/bioconductor-wgsmapp"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-wgsmapp.
shpc-registry automated BioContainers addition for bioconductor-wgsmapp
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-wgsmapp
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-wgsmapp:1.10.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-wgsmapp/1.10.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-wgsmapp/1.10.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-wgsmapp-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-wgsmapp-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-wgsmapp-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-wgsmapp-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-wgsmapp-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-wgsmapp-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-wgsmapp

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