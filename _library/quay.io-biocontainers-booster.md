---
layout: container
name:  "quay.io/biocontainers/booster"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/booster/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/booster/container.yaml"
updated_at: "2023-01-13 02:52:26.807101"
latest: "0.1.2--hec16e2b_4"
container_url: "https://biocontainers.pro/tools/booster"
aliases:
 - "booster"
versions:
 - "0.1.2--hec16e2b_4"
description: "shpc-registry automated BioContainers addition for booster"
config: {"url": "https://biocontainers.pro/tools/booster", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for booster", "latest": {"0.1.2--hec16e2b_4": "sha256:548ea4089fd808f6a5f9a62754914f03fcce65305195aa79dda765f64c48c6eb"}, "tags": {"0.1.2--hec16e2b_4": "sha256:548ea4089fd808f6a5f9a62754914f03fcce65305195aa79dda765f64c48c6eb"}, "docker": "quay.io/biocontainers/booster", "aliases": {"booster": "/usr/local/bin/booster"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/booster.
shpc-registry automated BioContainers addition for booster
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/booster
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/booster:0.1.2--hec16e2b_4
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/booster/0.1.2--hec16e2b_4
$ module help quay.io/biocontainers/booster/0.1.2--hec16e2b_4
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### booster-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### booster-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### booster-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### booster-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### booster-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### booster-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### booster

```bash
$ singularity exec <container> /usr/local/bin/booster
$ podman run --it --rm --entrypoint /usr/local/bin/booster   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/booster   -v ${PWD} -w ${PWD} <container> -c " $@"
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