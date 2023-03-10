---
layout: container
name:  "quay.io/biocontainers/bioconductor-minfidataepic"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-minfidataepic/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-minfidataepic/container.yaml"
updated_at: "2023-01-13 03:09:57.252086"
latest: "1.24.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-minfidataepic"
aliases:
 - "wget"
 - "c89"
 - "c99"
versions:
 - "1.8.0--r351_0"
 - "1.18.0--r41hdfd78af_0"
 - "1.16.0--r40hdfd78af_1"
 - "1.14.0--r40_0"
 - "1.12.0--r36_0"
 - "1.10.0--r36_1"
 - "1.24.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-minfidataepic"
config: {"url": "https://biocontainers.pro/tools/bioconductor-minfidataepic", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-minfidataepic", "latest": {"1.24.0--r42hdfd78af_0": "sha256:e184e585ba72c5ff56989fc0eacfb10cbac20aa3698e33ad82dd4ea460edae33"}, "tags": {"1.8.0--r351_0": "sha256:9a826041673dac9668d52d58dc6f7aa4e1b0c360959c204587b9d9c554e12283", "1.18.0--r41hdfd78af_0": "sha256:851fe3776f9128fcb928f8e3ca4b0d694685a2e11962b27c6f544128fbc6a6fb", "1.16.0--r40hdfd78af_1": "sha256:b4f60934ad5594643405f460759d39b450af3eab0ae695fdde0bb2dd2065f123", "1.14.0--r40_0": "sha256:bf8c9089b2b9724ddec8c538a6d01c52cc3cc09ff60c6ec33b8f0fec68439834", "1.12.0--r36_0": "sha256:15b59cc617d61fd77a457b2ba753524ea6f7485114b3d18a100c2090b0cf2434", "1.10.0--r36_1": "sha256:f660567828938561d4c9cfe498afb6e5eda3fb7abe9e949f95a6a5207c8400be", "1.24.0--r42hdfd78af_0": "sha256:e184e585ba72c5ff56989fc0eacfb10cbac20aa3698e33ad82dd4ea460edae33"}, "docker": "quay.io/biocontainers/bioconductor-minfidataepic", "aliases": {"wget": "/usr/local/bin/wget", "c89": "/usr/local/bin/c89", "c99": "/usr/local/bin/c99"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-minfidataepic.
shpc-registry automated BioContainers addition for bioconductor-minfidataepic
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-minfidataepic
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-minfidataepic:1.24.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-minfidataepic/1.24.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-minfidataepic/1.24.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-minfidataepic-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-minfidataepic-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-minfidataepic-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-minfidataepic-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-minfidataepic-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-minfidataepic-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### wget

```bash
$ singularity exec <container> /usr/local/bin/wget
$ podman run --it --rm --entrypoint /usr/local/bin/wget   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/wget   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### c89

```bash
$ singularity exec <container> /usr/local/bin/c89
$ podman run --it --rm --entrypoint /usr/local/bin/c89   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/c89   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### c99

```bash
$ singularity exec <container> /usr/local/bin/c99
$ podman run --it --rm --entrypoint /usr/local/bin/c99   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/c99   -v ${PWD} -w ${PWD} <container> -c " $@"
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