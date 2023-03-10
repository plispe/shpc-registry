---
layout: container
name:  "quay.io/biocontainers/perl-findbin"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/perl-findbin/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/perl-findbin/container.yaml"
updated_at: "2023-01-13 02:51:09.719257"
latest: "1.51--pl5321hdfd78af_3"
container_url: "https://biocontainers.pro/tools/perl-findbin"

versions:
 - "1.51--pl5321hdfd78af_3"
description: "shpc-registry automated BioContainers addition for perl-findbin"
config: {"url": "https://biocontainers.pro/tools/perl-findbin", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for perl-findbin", "latest": {"1.51--pl5321hdfd78af_3": "sha256:a6994160382956da8a8b33179d683663d5a8f28fd6c3cf303cfbd5480dffb236"}, "tags": {"1.51--pl5321hdfd78af_3": "sha256:a6994160382956da8a8b33179d683663d5a8f28fd6c3cf303cfbd5480dffb236"}, "docker": "quay.io/biocontainers/perl-findbin"}
---

This module is a singularity container wrapper for quay.io/biocontainers/perl-findbin.
shpc-registry automated BioContainers addition for perl-findbin
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/perl-findbin
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/perl-findbin:1.51--pl5321hdfd78af_3
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/perl-findbin/1.51--pl5321hdfd78af_3
$ module help quay.io/biocontainers/perl-findbin/1.51--pl5321hdfd78af_3
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### perl-findbin-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### perl-findbin-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### perl-findbin-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### perl-findbin-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### perl-findbin-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### perl-findbin-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### perl-findbin

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