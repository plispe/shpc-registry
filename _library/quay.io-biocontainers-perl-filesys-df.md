---
layout: container
name:  "quay.io/biocontainers/perl-filesys-df"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/perl-filesys-df/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/perl-filesys-df/container.yaml"
updated_at: "2023-01-13 03:46:04.669740"
latest: "0.92--pl5321hec16e2b_5"
container_url: "https://biocontainers.pro/tools/perl-filesys-df"
aliases:
 - "perl5.32.1"
 - "streamzip"
versions:
 - "0.92--pl5321hec16e2b_5"
description: "shpc-registry automated BioContainers addition for perl-filesys-df"
config: {"url": "https://biocontainers.pro/tools/perl-filesys-df", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for perl-filesys-df", "latest": {"0.92--pl5321hec16e2b_5": "sha256:507c9f025eef8d2130f4dd4c58e3a07dec0d8a365debcb1bd6b2596e4074de79"}, "tags": {"0.92--pl5321hec16e2b_5": "sha256:507c9f025eef8d2130f4dd4c58e3a07dec0d8a365debcb1bd6b2596e4074de79"}, "docker": "quay.io/biocontainers/perl-filesys-df", "aliases": {"perl5.32.1": "/usr/local/bin/perl5.32.1", "streamzip": "/usr/local/bin/streamzip"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/perl-filesys-df.
shpc-registry automated BioContainers addition for perl-filesys-df
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/perl-filesys-df
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/perl-filesys-df:0.92--pl5321hec16e2b_5
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/perl-filesys-df/0.92--pl5321hec16e2b_5
$ module help quay.io/biocontainers/perl-filesys-df/0.92--pl5321hec16e2b_5
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### perl-filesys-df-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### perl-filesys-df-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### perl-filesys-df-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### perl-filesys-df-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### perl-filesys-df-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### perl-filesys-df-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### perl5.32.1

```bash
$ singularity exec <container> /usr/local/bin/perl5.32.1
$ podman run --it --rm --entrypoint /usr/local/bin/perl5.32.1   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/perl5.32.1   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### streamzip

```bash
$ singularity exec <container> /usr/local/bin/streamzip
$ podman run --it --rm --entrypoint /usr/local/bin/streamzip   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/streamzip   -v ${PWD} -w ${PWD} <container> -c " $@"
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