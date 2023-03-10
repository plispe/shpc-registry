---
layout: container
name:  "quay.io/biocontainers/bioconductor-annmap"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-annmap/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-annmap/container.yaml"
updated_at: "2023-01-13 03:07:50.066869"
latest: "1.40.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-annmap"
aliases:
 - "my_print_defaults"
 - "mysql_config"
 - "perror"
versions:
 - "1.36.0--r41hdfd78af_0"
 - "1.40.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-annmap"
config: {"url": "https://biocontainers.pro/tools/bioconductor-annmap", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-annmap", "latest": {"1.40.0--r42hdfd78af_0": "sha256:cfea53eb668f3954134754c0ba74beff5011ed036a7f46010f0c6732ed19ce6a"}, "tags": {"1.36.0--r41hdfd78af_0": "sha256:c7e0332122ab972cb8cba4291bff66d11e60356d8a87410ae6b52e4fe0de09a0", "1.40.0--r42hdfd78af_0": "sha256:cfea53eb668f3954134754c0ba74beff5011ed036a7f46010f0c6732ed19ce6a"}, "docker": "quay.io/biocontainers/bioconductor-annmap", "aliases": {"my_print_defaults": "/usr/local/bin/my_print_defaults", "mysql_config": "/usr/local/bin/mysql_config", "perror": "/usr/local/bin/perror"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-annmap.
shpc-registry automated BioContainers addition for bioconductor-annmap
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-annmap
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-annmap:1.40.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-annmap/1.40.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-annmap/1.40.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-annmap-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-annmap-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-annmap-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-annmap-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-annmap-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-annmap-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### my_print_defaults

```bash
$ singularity exec <container> /usr/local/bin/my_print_defaults
$ podman run --it --rm --entrypoint /usr/local/bin/my_print_defaults   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/my_print_defaults   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### mysql_config

```bash
$ singularity exec <container> /usr/local/bin/mysql_config
$ podman run --it --rm --entrypoint /usr/local/bin/mysql_config   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/mysql_config   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### perror

```bash
$ singularity exec <container> /usr/local/bin/perror
$ podman run --it --rm --entrypoint /usr/local/bin/perror   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/perror   -v ${PWD} -w ${PWD} <container> -c " $@"
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