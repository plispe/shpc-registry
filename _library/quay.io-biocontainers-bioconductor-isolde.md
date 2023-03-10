---
layout: container
name:  "quay.io/biocontainers/bioconductor-isolde"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-isolde/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-isolde/container.yaml"
updated_at: "2023-01-13 02:57:27.298711"
latest: "1.26.0--r42hc0cfd56_0"
container_url: "https://biocontainers.pro/tools/bioconductor-isolde"
aliases:
 - "ncurses5-config"
 - "ncursesw5-config"
versions:
 - "1.8.0--r341h470a237_0"
 - "1.22.0--r41hc0cfd56_2"
 - "1.20.0--r41hd029910_0"
 - "1.15.0--r40h037d062_0"
 - "1.14.0--r36h516909a_0"
 - "1.12.0--r36h516909a_1"
 - "1.26.0--r42hc0cfd56_0"
description: "shpc-registry automated BioContainers addition for bioconductor-isolde"
config: {"url": "https://biocontainers.pro/tools/bioconductor-isolde", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-isolde", "latest": {"1.26.0--r42hc0cfd56_0": "sha256:721615e2c9331428d8367a54444f65ec6380b496b73c6bb3535feb1055acad3e"}, "tags": {"1.8.0--r341h470a237_0": "sha256:a634508bc0cbe032f34949ba7cb760a30c2fe2b258a42355d32268ebd14b6ae2", "1.22.0--r41hc0cfd56_2": "sha256:81e54aa4e9574e717bee99c8ced337e413d49573191d1b51c567d8040c6e442d", "1.20.0--r41hd029910_0": "sha256:8ee4c94ffb826fe79afa62cd69ea0eb0f781f1027391b76003c63d8d0acfadcb", "1.15.0--r40h037d062_0": "sha256:fb00f09d922d42f0bdcdf88708ef0f87515c95eee72bc476bf13d268c332874f", "1.14.0--r36h516909a_0": "sha256:914fda989831e8d16a9798dcc8f5a0af2f874229f310177ee6ac1caccdc35acf", "1.12.0--r36h516909a_1": "sha256:e93d5be5d01dbf27249da95acd583b7b1cabb36a9de401efc4511d24970a2069", "1.26.0--r42hc0cfd56_0": "sha256:721615e2c9331428d8367a54444f65ec6380b496b73c6bb3535feb1055acad3e"}, "docker": "quay.io/biocontainers/bioconductor-isolde", "aliases": {"ncurses5-config": "/usr/local/bin/ncurses5-config", "ncursesw5-config": "/usr/local/bin/ncursesw5-config"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-isolde.
shpc-registry automated BioContainers addition for bioconductor-isolde
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-isolde
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-isolde:1.26.0--r42hc0cfd56_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-isolde/1.26.0--r42hc0cfd56_0
$ module help quay.io/biocontainers/bioconductor-isolde/1.26.0--r42hc0cfd56_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-isolde-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-isolde-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-isolde-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-isolde-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-isolde-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-isolde-inspect-deffile:

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