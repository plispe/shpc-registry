---
layout: container
name:  "quay.io/biocontainers/glimpse-bio"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/glimpse-bio/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/glimpse-bio/container.yaml"
updated_at: "2023-01-13 02:58:42.847927"
latest: "1.1.1--h0303221_3"
container_url: "https://biocontainers.pro/tools/glimpse-bio"
aliases:
 - "GLIMPSE_chunk"
 - "GLIMPSE_concordance"
 - "GLIMPSE_ligate"
 - "GLIMPSE_phase"
 - "GLIMPSE_sample"
 - "GLIMPSE_snparray"
 - "htsfile"
 - "bgzip"
 - "tabix"
versions:
 - "v1.1.1--hd3cd7f2_0"
 - "1.1.1--h0303221_3"
description: "shpc-registry automated BioContainers addition for glimpse-bio"
config: {"url": "https://biocontainers.pro/tools/glimpse-bio", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for glimpse-bio", "latest": {"1.1.1--h0303221_3": "sha256:bd344086b0116b07dfe588efa3fc9bb112ab5cd942409c9d18b1c733178f9bc5"}, "tags": {"v1.1.1--hd3cd7f2_0": "sha256:31ea0d60db8f22d95c3d6cc8c4ca3899e7c4ee659169a00b93ba7c0e0fd1a207", "1.1.1--h0303221_3": "sha256:bd344086b0116b07dfe588efa3fc9bb112ab5cd942409c9d18b1c733178f9bc5"}, "docker": "quay.io/biocontainers/glimpse-bio", "aliases": {"GLIMPSE_chunk": "/usr/local/bin/GLIMPSE_chunk", "GLIMPSE_concordance": "/usr/local/bin/GLIMPSE_concordance", "GLIMPSE_ligate": "/usr/local/bin/GLIMPSE_ligate", "GLIMPSE_phase": "/usr/local/bin/GLIMPSE_phase", "GLIMPSE_sample": "/usr/local/bin/GLIMPSE_sample", "GLIMPSE_snparray": "/usr/local/bin/GLIMPSE_snparray", "htsfile": "/usr/local/bin/htsfile", "bgzip": "/usr/local/bin/bgzip", "tabix": "/usr/local/bin/tabix"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/glimpse-bio.
shpc-registry automated BioContainers addition for glimpse-bio
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/glimpse-bio
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/glimpse-bio:1.1.1--h0303221_3
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/glimpse-bio/1.1.1--h0303221_3
$ module help quay.io/biocontainers/glimpse-bio/1.1.1--h0303221_3
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### glimpse-bio-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### glimpse-bio-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### glimpse-bio-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### glimpse-bio-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### glimpse-bio-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### glimpse-bio-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### GLIMPSE_chunk

```bash
$ singularity exec <container> /usr/local/bin/GLIMPSE_chunk
$ podman run --it --rm --entrypoint /usr/local/bin/GLIMPSE_chunk   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/GLIMPSE_chunk   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### GLIMPSE_concordance

```bash
$ singularity exec <container> /usr/local/bin/GLIMPSE_concordance
$ podman run --it --rm --entrypoint /usr/local/bin/GLIMPSE_concordance   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/GLIMPSE_concordance   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### GLIMPSE_ligate

```bash
$ singularity exec <container> /usr/local/bin/GLIMPSE_ligate
$ podman run --it --rm --entrypoint /usr/local/bin/GLIMPSE_ligate   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/GLIMPSE_ligate   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### GLIMPSE_phase

```bash
$ singularity exec <container> /usr/local/bin/GLIMPSE_phase
$ podman run --it --rm --entrypoint /usr/local/bin/GLIMPSE_phase   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/GLIMPSE_phase   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### GLIMPSE_sample

```bash
$ singularity exec <container> /usr/local/bin/GLIMPSE_sample
$ podman run --it --rm --entrypoint /usr/local/bin/GLIMPSE_sample   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/GLIMPSE_sample   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### GLIMPSE_snparray

```bash
$ singularity exec <container> /usr/local/bin/GLIMPSE_snparray
$ podman run --it --rm --entrypoint /usr/local/bin/GLIMPSE_snparray   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/GLIMPSE_snparray   -v ${PWD} -w ${PWD} <container> -c " $@"
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