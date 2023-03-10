---
layout: container
name:  "quay.io/biocontainers/bioconductor-ahwikipathwaysdbs"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-ahwikipathwaysdbs/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-ahwikipathwaysdbs/container.yaml"
updated_at: "2023-01-13 03:30:20.161547"
latest: "0.99.4--r42hdfd78af_3"
container_url: "https://biocontainers.pro/tools/bioconductor-ahwikipathwaysdbs"

versions:
 - "0.99.4--r41hdfd78af_2"
 - "0.99.4--r42hdfd78af_3"
description: "shpc-registry automated BioContainers addition for bioconductor-ahwikipathwaysdbs"
config: {"url": "https://biocontainers.pro/tools/bioconductor-ahwikipathwaysdbs", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-ahwikipathwaysdbs", "latest": {"0.99.4--r42hdfd78af_3": "sha256:1f99ca21af10355578eac462270502a186b65b307b57004ee0e4e113bebf4750"}, "tags": {"0.99.4--r41hdfd78af_2": "sha256:d535a63c9095e254d266bff511d96806d6d861e075bf7ffcae96e11f9a2c9c21", "0.99.4--r42hdfd78af_3": "sha256:1f99ca21af10355578eac462270502a186b65b307b57004ee0e4e113bebf4750"}, "docker": "quay.io/biocontainers/bioconductor-ahwikipathwaysdbs"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-ahwikipathwaysdbs.
shpc-registry automated BioContainers addition for bioconductor-ahwikipathwaysdbs
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-ahwikipathwaysdbs
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-ahwikipathwaysdbs:0.99.4--r42hdfd78af_3
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-ahwikipathwaysdbs/0.99.4--r42hdfd78af_3
$ module help quay.io/biocontainers/bioconductor-ahwikipathwaysdbs/0.99.4--r42hdfd78af_3
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-ahwikipathwaysdbs-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ahwikipathwaysdbs-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ahwikipathwaysdbs-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-ahwikipathwaysdbs-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-ahwikipathwaysdbs-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-ahwikipathwaysdbs-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-ahwikipathwaysdbs

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