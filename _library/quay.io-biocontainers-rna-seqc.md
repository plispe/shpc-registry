---
layout: container
name:  "quay.io/biocontainers/rna-seqc"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/rna-seqc/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/rna-seqc/container.yaml"
updated_at: "2023-01-13 03:27:24.725418"
latest: "2.3.5--h335d4e2_3"
container_url: "https://biocontainers.pro/tools/rna-seqc"
aliases:
 - "rnaseqc"
versions:
 - "2.3.5--h335d4e2_3"
description: "shpc-registry automated BioContainers addition for rna-seqc"
config: {"url": "https://biocontainers.pro/tools/rna-seqc", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for rna-seqc", "latest": {"2.3.5--h335d4e2_3": "sha256:0b135dad0c88d19a477a85d4f7765bbff19d6aa99eb1b316ab2132debebc68f8"}, "tags": {"2.3.5--h335d4e2_3": "sha256:0b135dad0c88d19a477a85d4f7765bbff19d6aa99eb1b316ab2132debebc68f8"}, "docker": "quay.io/biocontainers/rna-seqc", "aliases": {"rnaseqc": "/usr/local/bin/rnaseqc"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/rna-seqc.
shpc-registry automated BioContainers addition for rna-seqc
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/rna-seqc
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/rna-seqc:2.3.5--h335d4e2_3
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/rna-seqc/2.3.5--h335d4e2_3
$ module help quay.io/biocontainers/rna-seqc/2.3.5--h335d4e2_3
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### rna-seqc-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### rna-seqc-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### rna-seqc-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### rna-seqc-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### rna-seqc-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### rna-seqc-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### rnaseqc

```bash
$ singularity exec <container> /usr/local/bin/rnaseqc
$ podman run --it --rm --entrypoint /usr/local/bin/rnaseqc   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/rnaseqc   -v ${PWD} -w ${PWD} <container> -c " $@"
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