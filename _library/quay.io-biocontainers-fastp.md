---
layout: container
name:  "quay.io/biocontainers/fastp"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/fastp/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/fastp/container.yaml"
updated_at: "2023-01-13 03:09:29.644464"
latest: "0.23.2--h5f740d0_3"
container_url: "https://biocontainers.pro/tools/fastp"

versions:
 - "0.22.0--h2e03b76_0"
 - "0.23.2--h5f740d0_3"
description: "shpc-registry automated BioContainers addition for fastp"
config: {"url": "https://biocontainers.pro/tools/fastp", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for fastp", "latest": {"0.23.2--h5f740d0_3": "sha256:2489fe56260bde05bdf72a8ead4892033b9a05dc4525affb909405bea7839d1b"}, "tags": {"0.22.0--h2e03b76_0": "sha256:e94097ae4ca17394b35d59a20d9a9f6d8972992bd47d1783f00c26e86ca82c2b", "0.23.2--h5f740d0_3": "sha256:2489fe56260bde05bdf72a8ead4892033b9a05dc4525affb909405bea7839d1b"}, "docker": "quay.io/biocontainers/fastp"}
---

This module is a singularity container wrapper for quay.io/biocontainers/fastp.
shpc-registry automated BioContainers addition for fastp
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/fastp
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/fastp:0.23.2--h5f740d0_3
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/fastp/0.23.2--h5f740d0_3
$ module help quay.io/biocontainers/fastp/0.23.2--h5f740d0_3
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### fastp-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### fastp-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### fastp-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### fastp-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### fastp-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### fastp-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### fastp

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