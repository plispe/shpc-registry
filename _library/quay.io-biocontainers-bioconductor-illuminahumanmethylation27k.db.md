---
layout: container
name:  "quay.io/biocontainers/bioconductor-illuminahumanmethylation27k.db"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-illuminahumanmethylation27k.db/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-illuminahumanmethylation27k.db/container.yaml"
updated_at: "2023-01-13 03:34:41.529556"
latest: "1.4.8--r42hdfd78af_10"
container_url: "https://biocontainers.pro/tools/bioconductor-illuminahumanmethylation27k.db"

versions:
 - "1.4.8--r41hdfd78af_9"
 - "1.4.8--r42hdfd78af_10"
description: "shpc-registry automated BioContainers addition for bioconductor-illuminahumanmethylation27k.db"
config: {"url": "https://biocontainers.pro/tools/bioconductor-illuminahumanmethylation27k.db", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-illuminahumanmethylation27k.db", "latest": {"1.4.8--r42hdfd78af_10": "sha256:2327f37e985579ebbc3422adf4b9d950fa6730095c98cca6be66a1e4c1f702c1"}, "tags": {"1.4.8--r41hdfd78af_9": "sha256:271f5dcbadfd52e95eca68ce076950a4fe458826a0da1896b8b6cfc75db073c4", "1.4.8--r42hdfd78af_10": "sha256:2327f37e985579ebbc3422adf4b9d950fa6730095c98cca6be66a1e4c1f702c1"}, "docker": "quay.io/biocontainers/bioconductor-illuminahumanmethylation27k.db"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-illuminahumanmethylation27k.db.
shpc-registry automated BioContainers addition for bioconductor-illuminahumanmethylation27k.db
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-illuminahumanmethylation27k.db
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-illuminahumanmethylation27k.db:1.4.8--r42hdfd78af_10
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-illuminahumanmethylation27k.db/1.4.8--r42hdfd78af_10
$ module help quay.io/biocontainers/bioconductor-illuminahumanmethylation27k.db/1.4.8--r42hdfd78af_10
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-illuminahumanmethylation27k.db-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-illuminahumanmethylation27k.db-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-illuminahumanmethylation27k.db-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-illuminahumanmethylation27k.db-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-illuminahumanmethylation27k.db-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-illuminahumanmethylation27k.db-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-illuminahumanmethylation27k.db

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