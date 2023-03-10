---
layout: container
name:  "quay.io/biocontainers/bioconductor-kegglincs"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-kegglincs/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-kegglincs/container.yaml"
updated_at: "2023-01-13 02:49:43.111218"
latest: "1.24.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-kegglincs"
aliases:
 - "wget"
 - "c89"
 - "c99"
versions:
 - "1.8.0--r351_0"
 - "1.20.0--r41hdfd78af_0"
 - "1.18.0--r41hdfd78af_0"
 - "1.16.0--r40hdfd78af_1"
 - "1.14.0--r40_0"
 - "1.12.0--r36_1"
 - "1.24.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-kegglincs"
config: {"url": "https://biocontainers.pro/tools/bioconductor-kegglincs", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-kegglincs", "latest": {"1.24.0--r42hdfd78af_0": "sha256:253b7a6a0897141f69a63d5e89a2031911530ed666f132107b29895b7ce9d621"}, "tags": {"1.8.0--r351_0": "sha256:aea1d34e36c09c106278f183a1e9bf3d6d92997dcd64671db6346a2318aaee1b", "1.20.0--r41hdfd78af_0": "sha256:66667297a3e6e5cf6266ed0af0df087f327f5a5149a3f9370e0a621a3dadcbeb", "1.18.0--r41hdfd78af_0": "sha256:77ca0af5c3642854a47e19c5de6d3e1601dc56d0f66fb93ce02850739002788d", "1.16.0--r40hdfd78af_1": "sha256:1368cac851ea6b9a7df3a84004c6837590aa3bee4f8608f5d7b43453c6b8e197", "1.14.0--r40_0": "sha256:6172aa87494c69937e0d65697b78205adf975d742ed0bc14f79a05ba62c3b193", "1.12.0--r36_1": "sha256:a011fac147e612ac239dd4f4200107af31034d53031c6ce62feb719f8577f6e3", "1.24.0--r42hdfd78af_0": "sha256:253b7a6a0897141f69a63d5e89a2031911530ed666f132107b29895b7ce9d621"}, "docker": "quay.io/biocontainers/bioconductor-kegglincs", "aliases": {"wget": "/usr/local/bin/wget", "c89": "/usr/local/bin/c89", "c99": "/usr/local/bin/c99"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-kegglincs.
shpc-registry automated BioContainers addition for bioconductor-kegglincs
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-kegglincs
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-kegglincs:1.24.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-kegglincs/1.24.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-kegglincs/1.24.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-kegglincs-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-kegglincs-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-kegglincs-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-kegglincs-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-kegglincs-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-kegglincs-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### wget

```bash
$ singularity exec <container> /usr/local/bin/wget
$ podman run --it --rm --entrypoint /usr/local/bin/wget   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/wget   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### c89

```bash
$ singularity exec <container> /usr/local/bin/c89
$ podman run --it --rm --entrypoint /usr/local/bin/c89   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/c89   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### c99

```bash
$ singularity exec <container> /usr/local/bin/c99
$ podman run --it --rm --entrypoint /usr/local/bin/c99   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/c99   -v ${PWD} -w ${PWD} <container> -c " $@"
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