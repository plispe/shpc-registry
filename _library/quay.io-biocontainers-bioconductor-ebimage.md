---
layout: container
name:  "quay.io/biocontainers/bioconductor-ebimage"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-ebimage/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-ebimage/container.yaml"
updated_at: "2023-01-13 03:30:57.887763"
latest: "4.40.0--r42hc247a5b_0"
container_url: "https://biocontainers.pro/tools/bioconductor-ebimage"
aliases:
 - "fftw-wisdom"
 - "fftw-wisdom-to-conf"
 - "fftwf-wisdom"
 - "fftwl-wisdom"
versions:
 - "4.36.0--r41hc247a5b_2"
 - "4.40.0--r42hc247a5b_0"
description: "shpc-registry automated BioContainers addition for bioconductor-ebimage"
config: {"url": "https://biocontainers.pro/tools/bioconductor-ebimage", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-ebimage", "latest": {"4.40.0--r42hc247a5b_0": "sha256:b5a367203f4b38f1cef542a631af34afd6014cce6628cacbb7de8a6c8fb97188"}, "tags": {"4.36.0--r41hc247a5b_2": "sha256:3a4318c3c88f06c470f967aae5473b2524d9067cba30077d65ee81a9eddac5cc", "4.40.0--r42hc247a5b_0": "sha256:b5a367203f4b38f1cef542a631af34afd6014cce6628cacbb7de8a6c8fb97188"}, "docker": "quay.io/biocontainers/bioconductor-ebimage", "aliases": {"fftw-wisdom": "/usr/local/bin/fftw-wisdom", "fftw-wisdom-to-conf": "/usr/local/bin/fftw-wisdom-to-conf", "fftwf-wisdom": "/usr/local/bin/fftwf-wisdom", "fftwl-wisdom": "/usr/local/bin/fftwl-wisdom"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-ebimage.
shpc-registry automated BioContainers addition for bioconductor-ebimage
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-ebimage
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-ebimage:4.40.0--r42hc247a5b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-ebimage/4.40.0--r42hc247a5b_0
$ module help quay.io/biocontainers/bioconductor-ebimage/4.40.0--r42hc247a5b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-ebimage-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ebimage-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ebimage-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-ebimage-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-ebimage-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-ebimage-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### fftw-wisdom

```bash
$ singularity exec <container> /usr/local/bin/fftw-wisdom
$ podman run --it --rm --entrypoint /usr/local/bin/fftw-wisdom   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/fftw-wisdom   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### fftw-wisdom-to-conf

```bash
$ singularity exec <container> /usr/local/bin/fftw-wisdom-to-conf
$ podman run --it --rm --entrypoint /usr/local/bin/fftw-wisdom-to-conf   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/fftw-wisdom-to-conf   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### fftwf-wisdom

```bash
$ singularity exec <container> /usr/local/bin/fftwf-wisdom
$ podman run --it --rm --entrypoint /usr/local/bin/fftwf-wisdom   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/fftwf-wisdom   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### fftwl-wisdom

```bash
$ singularity exec <container> /usr/local/bin/fftwl-wisdom
$ podman run --it --rm --entrypoint /usr/local/bin/fftwl-wisdom   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/fftwl-wisdom   -v ${PWD} -w ${PWD} <container> -c " $@"
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