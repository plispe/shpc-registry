---
layout: container
name:  "quay.io/biocontainers/peakranger"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/peakranger/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/peakranger/container.yaml"
updated_at: "2023-01-13 03:12:08.327781"
latest: "1.18--h7ff8a90_6"
container_url: "https://biocontainers.pro/tools/peakranger"
aliases:
 - "peakranger"
versions:
 - "1.18--h7ff8a90_6"
description: "shpc-registry automated BioContainers addition for peakranger"
config: {"url": "https://biocontainers.pro/tools/peakranger", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for peakranger", "latest": {"1.18--h7ff8a90_6": "sha256:8b5362df08ee2ab33efb3e1bada5178a18cb30960c3f598994969bc00fd6a0b4"}, "tags": {"1.18--h7ff8a90_6": "sha256:8b5362df08ee2ab33efb3e1bada5178a18cb30960c3f598994969bc00fd6a0b4"}, "docker": "quay.io/biocontainers/peakranger", "aliases": {"peakranger": "/usr/local/bin/peakranger"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/peakranger.
shpc-registry automated BioContainers addition for peakranger
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/peakranger
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/peakranger:1.18--h7ff8a90_6
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/peakranger/1.18--h7ff8a90_6
$ module help quay.io/biocontainers/peakranger/1.18--h7ff8a90_6
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### peakranger-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### peakranger-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### peakranger-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### peakranger-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### peakranger-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### peakranger-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### peakranger

```bash
$ singularity exec <container> /usr/local/bin/peakranger
$ podman run --it --rm --entrypoint /usr/local/bin/peakranger   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/peakranger   -v ${PWD} -w ${PWD} <container> -c " $@"
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