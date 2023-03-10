---
layout: container
name:  "quay.io/biocontainers/rmblast"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/rmblast/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/rmblast/container.yaml"
updated_at: "2023-01-13 03:27:33.008125"
latest: "2.11.0--h6200dbe_0"
container_url: "https://biocontainers.pro/tools/rmblast"
aliases:
 - "rmblastn"
 - "build.sh"
 - "common.go"
 - "rchive.go"
 - "blast_report"
 - "blastdb_convert"
 - "blastdb_path"
 - "setup-deps.log"
 - "setup.sh"
 - "xtract.go"
 - "certtool"
versions:
 - "2.9.0--h2d02072_0"
 - "2.11.0--h6200dbe_0"
 - "2.10.0--h2d02072_0"
description: "shpc-registry automated BioContainers addition for rmblast"
config: {"url": "https://biocontainers.pro/tools/rmblast", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for rmblast", "latest": {"2.11.0--h6200dbe_0": "sha256:35bfaf4fc9138db97d259e20fd841e11789c2c27e3a21f3ce04f0c9ad6dda69e"}, "tags": {"2.9.0--h2d02072_0": "sha256:851b999b4326e2fdb0e0aa1803c30452d8e04a85ca5242a6d695836623f5d54c", "2.11.0--h6200dbe_0": "sha256:35bfaf4fc9138db97d259e20fd841e11789c2c27e3a21f3ce04f0c9ad6dda69e", "2.10.0--h2d02072_0": "sha256:65dd33a34d3310810b257829b248d53e82b86c74884bf6cbf89a10ee91066f63"}, "docker": "quay.io/biocontainers/rmblast", "aliases": {"rmblastn": "/usr/local/bin/rmblastn", "build.sh": "/usr/local/bin/build.sh", "common.go": "/usr/local/bin/common.go", "rchive.go": "/usr/local/bin/rchive.go", "blast_report": "/usr/local/bin/blast_report", "blastdb_convert": "/usr/local/bin/blastdb_convert", "blastdb_path": "/usr/local/bin/blastdb_path", "setup-deps.log": "/usr/local/bin/setup-deps.log", "setup.sh": "/usr/local/bin/setup.sh", "xtract.go": "/usr/local/bin/xtract.go", "certtool": "/usr/local/bin/certtool"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/rmblast.
shpc-registry automated BioContainers addition for rmblast
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/rmblast
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/rmblast:2.11.0--h6200dbe_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/rmblast/2.11.0--h6200dbe_0
$ module help quay.io/biocontainers/rmblast/2.11.0--h6200dbe_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### rmblast-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### rmblast-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### rmblast-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### rmblast-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### rmblast-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### rmblast-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### rmblastn

```bash
$ singularity exec <container> /usr/local/bin/rmblastn
$ podman run --it --rm --entrypoint /usr/local/bin/rmblastn   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/rmblastn   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### build.sh

```bash
$ singularity exec <container> /usr/local/bin/build.sh
$ podman run --it --rm --entrypoint /usr/local/bin/build.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/build.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### common.go

```bash
$ singularity exec <container> /usr/local/bin/common.go
$ podman run --it --rm --entrypoint /usr/local/bin/common.go   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/common.go   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### rchive.go

```bash
$ singularity exec <container> /usr/local/bin/rchive.go
$ podman run --it --rm --entrypoint /usr/local/bin/rchive.go   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/rchive.go   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### blast_report

```bash
$ singularity exec <container> /usr/local/bin/blast_report
$ podman run --it --rm --entrypoint /usr/local/bin/blast_report   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/blast_report   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### blastdb_convert

```bash
$ singularity exec <container> /usr/local/bin/blastdb_convert
$ podman run --it --rm --entrypoint /usr/local/bin/blastdb_convert   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/blastdb_convert   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### blastdb_path

```bash
$ singularity exec <container> /usr/local/bin/blastdb_path
$ podman run --it --rm --entrypoint /usr/local/bin/blastdb_path   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/blastdb_path   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### setup-deps.log

```bash
$ singularity exec <container> /usr/local/bin/setup-deps.log
$ podman run --it --rm --entrypoint /usr/local/bin/setup-deps.log   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/setup-deps.log   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### setup.sh

```bash
$ singularity exec <container> /usr/local/bin/setup.sh
$ podman run --it --rm --entrypoint /usr/local/bin/setup.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/setup.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### xtract.go

```bash
$ singularity exec <container> /usr/local/bin/xtract.go
$ podman run --it --rm --entrypoint /usr/local/bin/xtract.go   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/xtract.go   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### certtool

```bash
$ singularity exec <container> /usr/local/bin/certtool
$ podman run --it --rm --entrypoint /usr/local/bin/certtool   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/certtool   -v ${PWD} -w ${PWD} <container> -c " $@"
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