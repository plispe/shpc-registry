---
layout: container
name:  "quay.io/biocontainers/sctools"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/sctools/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/sctools/container.yaml"
updated_at: "2023-01-13 03:01:53.703285"
latest: "1.0.0--hd03093a_2"
container_url: "https://biocontainers.pro/tools/sctools"
aliases:
 - "sctools_demultiplex"
versions:
 - "1.0.0--hd03093a_2"
description: "shpc-registry automated BioContainers addition for sctools"
config: {"url": "https://biocontainers.pro/tools/sctools", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for sctools", "latest": {"1.0.0--hd03093a_2": "sha256:6b8a23ce4487ab761d8489d782bacd89b2aa04d3dd8f3ec88e093afcd79010fb"}, "tags": {"1.0.0--hd03093a_2": "sha256:6b8a23ce4487ab761d8489d782bacd89b2aa04d3dd8f3ec88e093afcd79010fb"}, "docker": "quay.io/biocontainers/sctools", "aliases": {"sctools_demultiplex": "/usr/local/bin/sctools_demultiplex"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/sctools.
shpc-registry automated BioContainers addition for sctools
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/sctools
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/sctools:1.0.0--hd03093a_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/sctools/1.0.0--hd03093a_2
$ module help quay.io/biocontainers/sctools/1.0.0--hd03093a_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### sctools-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### sctools-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### sctools-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### sctools-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### sctools-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### sctools-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### sctools_demultiplex

```bash
$ singularity exec <container> /usr/local/bin/sctools_demultiplex
$ podman run --it --rm --entrypoint /usr/local/bin/sctools_demultiplex   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/sctools_demultiplex   -v ${PWD} -w ${PWD} <container> -c " $@"
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