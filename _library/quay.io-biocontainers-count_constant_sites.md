---
layout: container
name:  "quay.io/biocontainers/count_constant_sites"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/count_constant_sites/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/count_constant_sites/container.yaml"
updated_at: "2023-01-13 03:38:17.112717"
latest: "0.1.1--h9ee0642_1"
container_url: "https://biocontainers.pro/tools/count_constant_sites"
aliases:
 - "count_constant_sites"
versions:
 - "0.1.1--h9ee0642_1"
description: "shpc-registry automated BioContainers addition for count_constant_sites"
config: {"url": "https://biocontainers.pro/tools/count_constant_sites", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for count_constant_sites", "latest": {"0.1.1--h9ee0642_1": "sha256:45f1c5a082d8877ebbb3e3cb5f1792d78341692826437d2d7bcc3131e3eb9dce"}, "tags": {"0.1.1--h9ee0642_1": "sha256:45f1c5a082d8877ebbb3e3cb5f1792d78341692826437d2d7bcc3131e3eb9dce"}, "docker": "quay.io/biocontainers/count_constant_sites", "aliases": {"count_constant_sites": "/usr/local/bin/count_constant_sites"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/count_constant_sites.
shpc-registry automated BioContainers addition for count_constant_sites
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/count_constant_sites
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/count_constant_sites:0.1.1--h9ee0642_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/count_constant_sites/0.1.1--h9ee0642_1
$ module help quay.io/biocontainers/count_constant_sites/0.1.1--h9ee0642_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### count_constant_sites-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### count_constant_sites-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### count_constant_sites-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### count_constant_sites-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### count_constant_sites-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### count_constant_sites-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### count_constant_sites

```bash
$ singularity exec <container> /usr/local/bin/count_constant_sites
$ podman run --it --rm --entrypoint /usr/local/bin/count_constant_sites   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/count_constant_sites   -v ${PWD} -w ${PWD} <container> -c " $@"
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