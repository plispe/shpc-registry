---
layout: container
name:  "quay.io/biocontainers/bioconductor-epitxdb.sc.saccer3"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-epitxdb.sc.saccer3/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-epitxdb.sc.saccer3/container.yaml"
updated_at: "2023-01-13 03:00:28.978386"
latest: "0.99.5--r42hdfd78af_3"
container_url: "https://biocontainers.pro/tools/bioconductor-epitxdb.sc.saccer3"

versions:
 - "0.99.5--r41hdfd78af_2"
 - "0.99.5--r42hdfd78af_3"
description: "shpc-registry automated BioContainers addition for bioconductor-epitxdb.sc.saccer3"
config: {"url": "https://biocontainers.pro/tools/bioconductor-epitxdb.sc.saccer3", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-epitxdb.sc.saccer3", "latest": {"0.99.5--r42hdfd78af_3": "sha256:869ffff15d91cd6a8312f74edb170a4ccd84e59eb0b57002c18a0ebc88273001"}, "tags": {"0.99.5--r41hdfd78af_2": "sha256:83fbdab38edc36892dd83a3030eef3462b9e33ec28f75e7fc318edd6c18c2b4a", "0.99.5--r42hdfd78af_3": "sha256:869ffff15d91cd6a8312f74edb170a4ccd84e59eb0b57002c18a0ebc88273001"}, "docker": "quay.io/biocontainers/bioconductor-epitxdb.sc.saccer3"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-epitxdb.sc.saccer3.
shpc-registry automated BioContainers addition for bioconductor-epitxdb.sc.saccer3
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-epitxdb.sc.saccer3
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-epitxdb.sc.saccer3:0.99.5--r42hdfd78af_3
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-epitxdb.sc.saccer3/0.99.5--r42hdfd78af_3
$ module help quay.io/biocontainers/bioconductor-epitxdb.sc.saccer3/0.99.5--r42hdfd78af_3
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-epitxdb.sc.saccer3-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-epitxdb.sc.saccer3-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-epitxdb.sc.saccer3-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-epitxdb.sc.saccer3-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-epitxdb.sc.saccer3-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-epitxdb.sc.saccer3-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-epitxdb.sc.saccer3

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