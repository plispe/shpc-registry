---
layout: container
name:  "quay.io/biocontainers/perl-mime-types"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/perl-mime-types/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/perl-mime-types/container.yaml"
updated_at: "2023-01-13 03:30:06.966971"
latest: "2.24--pl5321hdfd78af_0"
container_url: "https://biocontainers.pro/tools/perl-mime-types"
aliases:
 - "perl5.32.1"
 - "streamzip"
versions:
 - "2.22--pl5321hdfd78af_0"
 - "2.24--pl5321hdfd78af_0"
 - "2.23--pl5321hdfd78af_0"
description: "shpc-registry automated BioContainers addition for perl-mime-types"
config: {"url": "https://biocontainers.pro/tools/perl-mime-types", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for perl-mime-types", "latest": {"2.24--pl5321hdfd78af_0": "sha256:3000a691e1d7c8bcd8eee5e5731355492e93a2d8dc4afb285cbcfe7e09002cfc"}, "tags": {"2.22--pl5321hdfd78af_0": "sha256:c1c581fcd8170a21a5bb34a4f16957ea71e7df9379b40ffafc66ddb5e08e714f", "2.24--pl5321hdfd78af_0": "sha256:3000a691e1d7c8bcd8eee5e5731355492e93a2d8dc4afb285cbcfe7e09002cfc", "2.23--pl5321hdfd78af_0": "sha256:56ac065356f7bd38c16b7c93a7238c6d04c4ea1420808234e6d17386dab37ee2"}, "docker": "quay.io/biocontainers/perl-mime-types", "aliases": {"perl5.32.1": "/usr/local/bin/perl5.32.1", "streamzip": "/usr/local/bin/streamzip"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/perl-mime-types.
shpc-registry automated BioContainers addition for perl-mime-types
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/perl-mime-types
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/perl-mime-types:2.24--pl5321hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/perl-mime-types/2.24--pl5321hdfd78af_0
$ module help quay.io/biocontainers/perl-mime-types/2.24--pl5321hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### perl-mime-types-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### perl-mime-types-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### perl-mime-types-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### perl-mime-types-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### perl-mime-types-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### perl-mime-types-inspect-deffile:

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