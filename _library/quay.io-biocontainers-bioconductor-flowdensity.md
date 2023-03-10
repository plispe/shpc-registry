---
layout: container
name:  "quay.io/biocontainers/bioconductor-flowdensity"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-flowdensity/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-flowdensity/container.yaml"
updated_at: "2023-01-13 02:58:53.869137"
latest: "1.32.0--r42hd91ffd7_0"
container_url: "https://biocontainers.pro/tools/bioconductor-flowdensity"
aliases:
 - "uconv"
 - "tclsh8.5"
 - "wish8.5"
 - "ncursesw5-config"
versions:
 - "1.6.0--r3.3.2_0"
 - "1.32.0--r42hd91ffd7_0"
 - "1.28.0--r41hd91ffd7_0"
 - "1.26.0--r41hd91ffd7_0"
 - "1.24.0--r40hd91ffd7_1"
 - "1.22.0--r40hbc14f71_0"
description: "shpc-registry automated BioContainers addition for bioconductor-flowdensity"
config: {"url": "https://biocontainers.pro/tools/bioconductor-flowdensity", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-flowdensity", "latest": {"1.32.0--r42hd91ffd7_0": "sha256:a44885f49467dbeec0d9e89efcf80343789376a4681c48a6df7a9f3fd1f41378"}, "tags": {"1.6.0--r3.3.2_0": "sha256:c768a35bc18cd010a55d28284153632eeaed324512d81a5032020a6eccfc6986", "1.32.0--r42hd91ffd7_0": "sha256:a44885f49467dbeec0d9e89efcf80343789376a4681c48a6df7a9f3fd1f41378", "1.28.0--r41hd91ffd7_0": "sha256:e64f16896d03c5acb65f2166fe8144490fb9cfb256d4afa2e2b3f92936a4a94e", "1.26.0--r41hd91ffd7_0": "sha256:fecd302e36feb7756cc24889823fcd3cdc9c428a9126d670d49776e1d97f69ed", "1.24.0--r40hd91ffd7_1": "sha256:1d0af0318cecd6db568a6ac6167588670c1d79c1c09237445eeb4669833ac380", "1.22.0--r40hbc14f71_0": "sha256:9c92d8703e269526f098bcb7183c9136ada67aca3d0a3864ce65e2810c942520"}, "docker": "quay.io/biocontainers/bioconductor-flowdensity", "aliases": {"uconv": "/usr/local/bin/uconv", "tclsh8.5": "/usr/local/bin/tclsh8.5", "wish8.5": "/usr/local/bin/wish8.5", "ncursesw5-config": "/usr/local/bin/ncursesw5-config"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-flowdensity.
shpc-registry automated BioContainers addition for bioconductor-flowdensity
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-flowdensity
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-flowdensity:1.32.0--r42hd91ffd7_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-flowdensity/1.32.0--r42hd91ffd7_0
$ module help quay.io/biocontainers/bioconductor-flowdensity/1.32.0--r42hd91ffd7_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-flowdensity-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-flowdensity-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-flowdensity-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-flowdensity-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-flowdensity-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-flowdensity-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### uconv

```bash
$ singularity exec <container> /usr/local/bin/uconv
$ podman run --it --rm --entrypoint /usr/local/bin/uconv   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/uconv   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### tclsh8.5

```bash
$ singularity exec <container> /usr/local/bin/tclsh8.5
$ podman run --it --rm --entrypoint /usr/local/bin/tclsh8.5   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/tclsh8.5   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### wish8.5

```bash
$ singularity exec <container> /usr/local/bin/wish8.5
$ podman run --it --rm --entrypoint /usr/local/bin/wish8.5   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/wish8.5   -v ${PWD} -w ${PWD} <container> -c " $@"
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