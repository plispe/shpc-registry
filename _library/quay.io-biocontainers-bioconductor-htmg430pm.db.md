---
layout: container
name:  "quay.io/biocontainers/bioconductor-htmg430pm.db"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-htmg430pm.db/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-htmg430pm.db/container.yaml"
updated_at: "2023-01-13 02:55:49.742900"
latest: "3.13.0--r42hdfd78af_2"
container_url: "https://biocontainers.pro/tools/bioconductor-htmg430pm.db"

versions:
 - "3.13.0--r41hdfd78af_1"
 - "3.13.0--r42hdfd78af_2"
description: "shpc-registry automated BioContainers addition for bioconductor-htmg430pm.db"
config: {"url": "https://biocontainers.pro/tools/bioconductor-htmg430pm.db", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-htmg430pm.db", "latest": {"3.13.0--r42hdfd78af_2": "sha256:807ffcda05d83e907e62cbd4c5b92a16668d977e9e04f763f81d18b1aa97d4ac"}, "tags": {"3.13.0--r41hdfd78af_1": "sha256:e318f561361d117b0e0c6723c33bae4e53567034a53de4277e6d66a4e3f59013", "3.13.0--r42hdfd78af_2": "sha256:807ffcda05d83e907e62cbd4c5b92a16668d977e9e04f763f81d18b1aa97d4ac"}, "docker": "quay.io/biocontainers/bioconductor-htmg430pm.db"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-htmg430pm.db.
shpc-registry automated BioContainers addition for bioconductor-htmg430pm.db
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-htmg430pm.db
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-htmg430pm.db:3.13.0--r42hdfd78af_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-htmg430pm.db/3.13.0--r42hdfd78af_2
$ module help quay.io/biocontainers/bioconductor-htmg430pm.db/3.13.0--r42hdfd78af_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-htmg430pm.db-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-htmg430pm.db-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-htmg430pm.db-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-htmg430pm.db-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-htmg430pm.db-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-htmg430pm.db-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-htmg430pm.db

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