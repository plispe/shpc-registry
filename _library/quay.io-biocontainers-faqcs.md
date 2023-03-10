---
layout: container
name:  "quay.io/biocontainers/faqcs"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/faqcs/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/faqcs/container.yaml"
updated_at: "2023-01-13 02:50:33.991348"
latest: "2.10--r41hd03093a_3"
container_url: "https://biocontainers.pro/tools/faqcs"
aliases:
 - "FaQCs"
versions:
 - "2.10--r41hd03093a_3"
description: "shpc-registry automated BioContainers addition for faqcs"
config: {"url": "https://biocontainers.pro/tools/faqcs", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for faqcs", "latest": {"2.10--r41hd03093a_3": "sha256:41f3f43b38fa6d32523380fe05ce5ce9a78ab669bdecf9bd56fe42e9444dff56"}, "tags": {"2.10--r41hd03093a_3": "sha256:41f3f43b38fa6d32523380fe05ce5ce9a78ab669bdecf9bd56fe42e9444dff56"}, "docker": "quay.io/biocontainers/faqcs", "aliases": {"FaQCs": "/usr/local/bin/FaQCs"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/faqcs.
shpc-registry automated BioContainers addition for faqcs
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/faqcs
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/faqcs:2.10--r41hd03093a_3
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/faqcs/2.10--r41hd03093a_3
$ module help quay.io/biocontainers/faqcs/2.10--r41hd03093a_3
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### faqcs-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### faqcs-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### faqcs-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### faqcs-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### faqcs-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### faqcs-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### FaQCs

```bash
$ singularity exec <container> /usr/local/bin/FaQCs
$ podman run --it --rm --entrypoint /usr/local/bin/FaQCs   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/FaQCs   -v ${PWD} -w ${PWD} <container> -c " $@"
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