---
layout: container
name:  "quay.io/biocontainers/bioconductor-txdb.ggallus.ucsc.galgal4.refgene"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-txdb.ggallus.ucsc.galgal4.refgene/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-txdb.ggallus.ucsc.galgal4.refgene/container.yaml"
updated_at: "2023-01-13 02:49:39.367027"
latest: "3.12.0--r42hdfd78af_5"
container_url: "https://biocontainers.pro/tools/bioconductor-txdb.ggallus.ucsc.galgal4.refgene"
aliases:
 - "gio-launch-desktop"
 - "c89"
 - "c99"
versions:
 - "3.4.6--r36_1"
 - "3.12.0--r42hdfd78af_5"
 - "3.11.0--r40_0"
 - "3.10.0--r36_0"
description: "shpc-registry automated BioContainers addition for bioconductor-txdb.ggallus.ucsc.galgal4.refgene"
config: {"url": "https://biocontainers.pro/tools/bioconductor-txdb.ggallus.ucsc.galgal4.refgene", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-txdb.ggallus.ucsc.galgal4.refgene", "latest": {"3.12.0--r42hdfd78af_5": "sha256:74cf7c3032007d4b7d1eb38285aec6439863b795f594bee3ec57d323eaaf37d2"}, "tags": {"3.4.6--r36_1": "sha256:b1f1065325b8609c1112ff514d0c5a20f0b323a5ff364ae344f6626eaa05e973", "3.12.0--r42hdfd78af_5": "sha256:74cf7c3032007d4b7d1eb38285aec6439863b795f594bee3ec57d323eaaf37d2", "3.11.0--r40_0": "sha256:06543ad6b9bcead2dd1a1d68897caccd213de764abc975e0914ea38077417518", "3.10.0--r36_0": "sha256:0a848111f2ab9f644e8fa96af2c00f42aff2f7ca48fe8a48da383e4d5d90cc64"}, "docker": "quay.io/biocontainers/bioconductor-txdb.ggallus.ucsc.galgal4.refgene", "aliases": {"gio-launch-desktop": "/usr/local/bin/gio-launch-desktop", "c89": "/usr/local/bin/c89", "c99": "/usr/local/bin/c99"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-txdb.ggallus.ucsc.galgal4.refgene.
shpc-registry automated BioContainers addition for bioconductor-txdb.ggallus.ucsc.galgal4.refgene
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-txdb.ggallus.ucsc.galgal4.refgene
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-txdb.ggallus.ucsc.galgal4.refgene:3.12.0--r42hdfd78af_5
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-txdb.ggallus.ucsc.galgal4.refgene/3.12.0--r42hdfd78af_5
$ module help quay.io/biocontainers/bioconductor-txdb.ggallus.ucsc.galgal4.refgene/3.12.0--r42hdfd78af_5
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-txdb.ggallus.ucsc.galgal4.refgene-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-txdb.ggallus.ucsc.galgal4.refgene-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-txdb.ggallus.ucsc.galgal4.refgene-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-txdb.ggallus.ucsc.galgal4.refgene-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-txdb.ggallus.ucsc.galgal4.refgene-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-txdb.ggallus.ucsc.galgal4.refgene-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### gio-launch-desktop

```bash
$ singularity exec <container> /usr/local/bin/gio-launch-desktop
$ podman run --it --rm --entrypoint /usr/local/bin/gio-launch-desktop   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/gio-launch-desktop   -v ${PWD} -w ${PWD} <container> -c " $@"
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