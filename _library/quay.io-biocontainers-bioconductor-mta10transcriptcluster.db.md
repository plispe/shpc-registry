---
layout: container
name:  "quay.io/biocontainers/bioconductor-mta10transcriptcluster.db"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-mta10transcriptcluster.db/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-mta10transcriptcluster.db/container.yaml"
updated_at: "2023-01-13 03:37:32.838710"
latest: "8.8.0--r42hdfd78af_2"
container_url: "https://biocontainers.pro/tools/bioconductor-mta10transcriptcluster.db"

versions:
 - "8.8.0--r41hdfd78af_1"
 - "8.8.0--r42hdfd78af_2"
description: "shpc-registry automated BioContainers addition for bioconductor-mta10transcriptcluster.db"
config: {"url": "https://biocontainers.pro/tools/bioconductor-mta10transcriptcluster.db", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-mta10transcriptcluster.db", "latest": {"8.8.0--r42hdfd78af_2": "sha256:47014240479733821ab4b86aaf1da68348b8d60c9dd3213bf2d32a435965dd0b"}, "tags": {"8.8.0--r41hdfd78af_1": "sha256:15a68da7557976b5025c4b6b4ccc206362b7e1d91651755dbff547be8d8abbc4", "8.8.0--r42hdfd78af_2": "sha256:47014240479733821ab4b86aaf1da68348b8d60c9dd3213bf2d32a435965dd0b"}, "docker": "quay.io/biocontainers/bioconductor-mta10transcriptcluster.db"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-mta10transcriptcluster.db.
shpc-registry automated BioContainers addition for bioconductor-mta10transcriptcluster.db
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-mta10transcriptcluster.db
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-mta10transcriptcluster.db:8.8.0--r42hdfd78af_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-mta10transcriptcluster.db/8.8.0--r42hdfd78af_2
$ module help quay.io/biocontainers/bioconductor-mta10transcriptcluster.db/8.8.0--r42hdfd78af_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-mta10transcriptcluster.db-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-mta10transcriptcluster.db-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-mta10transcriptcluster.db-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-mta10transcriptcluster.db-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-mta10transcriptcluster.db-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-mta10transcriptcluster.db-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-mta10transcriptcluster.db

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