---
layout: container
name:  "quay.io/biocontainers/bioconductor-gosemsim"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-gosemsim/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-gosemsim/container.yaml"
updated_at: "2023-01-13 02:49:53.094950"
latest: "2.24.0--r42hc247a5b_0"
container_url: "https://biocontainers.pro/tools/bioconductor-gosemsim"
aliases:
 - "wget"
 - "c89"
 - "c99"
versions:
 - "2.8.0--r351hf484d3e_0"
 - "2.24.0--r42hc247a5b_0"
 - "2.20.0--r41hc247a5b_2"
 - "2.18.0--r41h399db7b_0"
 - "2.16.1--r40h399db7b_0"
 - "2.14.0--r40h5f743cb_0"
description: "shpc-registry automated BioContainers addition for bioconductor-gosemsim"
config: {"url": "https://biocontainers.pro/tools/bioconductor-gosemsim", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-gosemsim", "latest": {"2.24.0--r42hc247a5b_0": "sha256:de5615604cf1674e57c0f950af96bbc3d16092027cefe08139e985642f93c3f7"}, "tags": {"2.8.0--r351hf484d3e_0": "sha256:d190962b3f941f9b7f8928843b07367e8e2b77362fe7f9ed4edc6de4a826093d", "2.24.0--r42hc247a5b_0": "sha256:de5615604cf1674e57c0f950af96bbc3d16092027cefe08139e985642f93c3f7", "2.20.0--r41hc247a5b_2": "sha256:65eb0b680d4409d310c45d72507179e16db075cef56b22ea929fb70fd122fc91", "2.18.0--r41h399db7b_0": "sha256:6801a93f8dbb1200126d397a3e94a01901c9ab5a19fbc90fc9f9127c9d58e21b", "2.16.1--r40h399db7b_0": "sha256:ee802746877546f631da4d8ea61deda86f65ab66c74d7b09a2b82d6312d9b93f", "2.14.0--r40h5f743cb_0": "sha256:7acd3d6d488ff434f3706210dc9616bb8c7cd092b195d79e95d8b8e6b6740b51"}, "docker": "quay.io/biocontainers/bioconductor-gosemsim", "aliases": {"wget": "/usr/local/bin/wget", "c89": "/usr/local/bin/c89", "c99": "/usr/local/bin/c99"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-gosemsim.
shpc-registry automated BioContainers addition for bioconductor-gosemsim
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-gosemsim
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-gosemsim:2.24.0--r42hc247a5b_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-gosemsim/2.24.0--r42hc247a5b_0
$ module help quay.io/biocontainers/bioconductor-gosemsim/2.24.0--r42hc247a5b_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-gosemsim-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-gosemsim-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-gosemsim-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-gosemsim-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-gosemsim-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-gosemsim-inspect-deffile:

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