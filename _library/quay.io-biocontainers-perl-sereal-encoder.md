---
layout: container
name:  "quay.io/biocontainers/perl-sereal-encoder"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/perl-sereal-encoder/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/perl-sereal-encoder/container.yaml"
updated_at: "2023-01-13 03:29:43.593178"
latest: "4.025--pl5321hec16e2b_1"
container_url: "https://biocontainers.pro/tools/perl-sereal-encoder"
aliases:
 - "perl5.32.1"
 - "streamzip"
versions:
 - "4.025--pl5321hec16e2b_1"
description: "shpc-registry automated BioContainers addition for perl-sereal-encoder"
config: {"url": "https://biocontainers.pro/tools/perl-sereal-encoder", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for perl-sereal-encoder", "latest": {"4.025--pl5321hec16e2b_1": "sha256:93c3c37178e783b2dc5cb1609aa8898e95499bb657088bd9acbaa6dfdd3e1808"}, "tags": {"4.025--pl5321hec16e2b_1": "sha256:93c3c37178e783b2dc5cb1609aa8898e95499bb657088bd9acbaa6dfdd3e1808"}, "docker": "quay.io/biocontainers/perl-sereal-encoder", "aliases": {"perl5.32.1": "/usr/local/bin/perl5.32.1", "streamzip": "/usr/local/bin/streamzip"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/perl-sereal-encoder.
shpc-registry automated BioContainers addition for perl-sereal-encoder
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/perl-sereal-encoder
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/perl-sereal-encoder:4.025--pl5321hec16e2b_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/perl-sereal-encoder/4.025--pl5321hec16e2b_1
$ module help quay.io/biocontainers/perl-sereal-encoder/4.025--pl5321hec16e2b_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### perl-sereal-encoder-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### perl-sereal-encoder-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### perl-sereal-encoder-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### perl-sereal-encoder-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### perl-sereal-encoder-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### perl-sereal-encoder-inspect-deffile:

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