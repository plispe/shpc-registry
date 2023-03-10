---
layout: container
name:  "quay.io/biocontainers/pindel"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/pindel/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/pindel/container.yaml"
updated_at: "2023-01-13 03:09:19.420024"
latest: "0.2.5b9--h28e74a2_8"
container_url: "https://biocontainers.pro/tools/pindel"
aliases:
 - "pindel"
 - "pindel2vcf"
 - "pindel2vcf4tcga"
 - "sam2pindel"
 - "htsfile"
 - "bgzip"
 - "tabix"
versions:
 - "0.2.5b9--h28e74a2_8"
description: "shpc-registry automated BioContainers addition for pindel"
config: {"url": "https://biocontainers.pro/tools/pindel", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for pindel", "latest": {"0.2.5b9--h28e74a2_8": "sha256:ce38f1010f2629154aab0b415d7d4848900290e7907ebfa90e52c932006916ef"}, "tags": {"0.2.5b9--h28e74a2_8": "sha256:ce38f1010f2629154aab0b415d7d4848900290e7907ebfa90e52c932006916ef"}, "docker": "quay.io/biocontainers/pindel", "aliases": {"pindel": "/usr/local/bin/pindel", "pindel2vcf": "/usr/local/bin/pindel2vcf", "pindel2vcf4tcga": "/usr/local/bin/pindel2vcf4tcga", "sam2pindel": "/usr/local/bin/sam2pindel", "htsfile": "/usr/local/bin/htsfile", "bgzip": "/usr/local/bin/bgzip", "tabix": "/usr/local/bin/tabix"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/pindel.
shpc-registry automated BioContainers addition for pindel
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/pindel
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/pindel:0.2.5b9--h28e74a2_8
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/pindel/0.2.5b9--h28e74a2_8
$ module help quay.io/biocontainers/pindel/0.2.5b9--h28e74a2_8
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### pindel-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### pindel-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### pindel-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### pindel-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### pindel-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### pindel-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### pindel

```bash
$ singularity exec <container> /usr/local/bin/pindel
$ podman run --it --rm --entrypoint /usr/local/bin/pindel   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pindel   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pindel2vcf

```bash
$ singularity exec <container> /usr/local/bin/pindel2vcf
$ podman run --it --rm --entrypoint /usr/local/bin/pindel2vcf   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pindel2vcf   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pindel2vcf4tcga

```bash
$ singularity exec <container> /usr/local/bin/pindel2vcf4tcga
$ podman run --it --rm --entrypoint /usr/local/bin/pindel2vcf4tcga   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pindel2vcf4tcga   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### sam2pindel

```bash
$ singularity exec <container> /usr/local/bin/sam2pindel
$ podman run --it --rm --entrypoint /usr/local/bin/sam2pindel   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/sam2pindel   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### htsfile

```bash
$ singularity exec <container> /usr/local/bin/htsfile
$ podman run --it --rm --entrypoint /usr/local/bin/htsfile   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/htsfile   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### bgzip

```bash
$ singularity exec <container> /usr/local/bin/bgzip
$ podman run --it --rm --entrypoint /usr/local/bin/bgzip   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/bgzip   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### tabix

```bash
$ singularity exec <container> /usr/local/bin/tabix
$ podman run --it --rm --entrypoint /usr/local/bin/tabix   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/tabix   -v ${PWD} -w ${PWD} <container> -c " $@"
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