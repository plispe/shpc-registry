---
layout: container
name:  "quay.io/biocontainers/bioconductor-ihw"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-ihw/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-ihw/container.yaml"
updated_at: "2023-01-13 03:27:59.763962"
latest: "1.26.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-ihw"
aliases:
 - "ncurses5-config"
 - "ncursesw5-config"
versions:
 - "1.8.0--r341_0"
 - "1.26.0--r42hdfd78af_0"
 - "1.22.0--r41hdfd78af_0"
 - "1.20.0--r41hdfd78af_0"
 - "1.18.0--r40hdfd78af_1"
 - "1.14.0--r36_0"
description: "shpc-registry automated BioContainers addition for bioconductor-ihw"
config: {"url": "https://biocontainers.pro/tools/bioconductor-ihw", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-ihw", "latest": {"1.26.0--r42hdfd78af_0": "sha256:08997fa2c35a36d4b81b41123d75fbe72585ad8037ccf37f1dadd9a0cea11c2f"}, "tags": {"1.8.0--r341_0": "sha256:572c9e44dcb91d13b59d4026d31378feb57b08431b3ac78b1c7cc96512dfccff", "1.26.0--r42hdfd78af_0": "sha256:08997fa2c35a36d4b81b41123d75fbe72585ad8037ccf37f1dadd9a0cea11c2f", "1.22.0--r41hdfd78af_0": "sha256:35e1fbb263c08a6af2d14fa45e467f2b794ce6e16808ecc7f85ad1ed76adc91a", "1.20.0--r41hdfd78af_0": "sha256:fae28ecff768cb9983b904d937155d735632b208736426ca0a2a8cef42f72833", "1.18.0--r40hdfd78af_1": "sha256:b8b125deaa9b59e99286473678292083c5b01c527e709c57677fbca834f28484", "1.14.0--r36_0": "sha256:8658e3521e42aff15b80221317e2405ad337e012b33d7bae557760092bd11aca"}, "docker": "quay.io/biocontainers/bioconductor-ihw", "aliases": {"ncurses5-config": "/usr/local/bin/ncurses5-config", "ncursesw5-config": "/usr/local/bin/ncursesw5-config"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-ihw.
shpc-registry automated BioContainers addition for bioconductor-ihw
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-ihw
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-ihw:1.26.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-ihw/1.26.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-ihw/1.26.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-ihw-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ihw-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ihw-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-ihw-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-ihw-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-ihw-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### ncurses5-config

```bash
$ singularity exec <container> /usr/local/bin/ncurses5-config
$ podman run --it --rm --entrypoint /usr/local/bin/ncurses5-config   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/ncurses5-config   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### ncursesw5-config

```bash
$ singularity exec <container> /usr/local/bin/ncursesw5-config
$ podman run --it --rm --entrypoint /usr/local/bin/ncursesw5-config   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/ncursesw5-config   -v ${PWD} -w ${PWD} <container> -c " $@"
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