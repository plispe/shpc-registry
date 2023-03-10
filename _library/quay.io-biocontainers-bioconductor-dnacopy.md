---
layout: container
name:  "quay.io/biocontainers/bioconductor-dnacopy"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-dnacopy/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-dnacopy/container.yaml"
updated_at: "2023-01-13 03:01:48.736313"
latest: "1.72.0--r42hefde4a7_0"
container_url: "https://biocontainers.pro/tools/bioconductor-dnacopy"

versions:
 - "1.68.0--r41hefde4a7_2"
 - "1.72.0--r42hefde4a7_0"
description: "shpc-registry automated BioContainers addition for bioconductor-dnacopy"
config: {"url": "https://biocontainers.pro/tools/bioconductor-dnacopy", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-dnacopy", "latest": {"1.72.0--r42hefde4a7_0": "sha256:7eb2309f94e2912458dcf46f67890dccbb16b15e51912de80e72d5e5d7b5d486"}, "tags": {"1.68.0--r41hefde4a7_2": "sha256:47435e845138630fbb7cc910441f609744ac2499c17a950e9202c4bc13a8cda7", "1.72.0--r42hefde4a7_0": "sha256:7eb2309f94e2912458dcf46f67890dccbb16b15e51912de80e72d5e5d7b5d486"}, "docker": "quay.io/biocontainers/bioconductor-dnacopy"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-dnacopy.
shpc-registry automated BioContainers addition for bioconductor-dnacopy
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-dnacopy
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-dnacopy:1.72.0--r42hefde4a7_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-dnacopy/1.72.0--r42hefde4a7_0
$ module help quay.io/biocontainers/bioconductor-dnacopy/1.72.0--r42hefde4a7_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-dnacopy-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-dnacopy-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-dnacopy-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-dnacopy-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-dnacopy-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-dnacopy-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-dnacopy

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