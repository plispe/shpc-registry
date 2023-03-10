---
layout: container
name:  "quay.io/biocontainers/dextractor"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/dextractor/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/dextractor/container.yaml"
updated_at: "2023-01-13 03:12:55.196017"
latest: "1.0p2--h7a6849f_5"
container_url: "https://biocontainers.pro/tools/dextractor"
aliases:
 - "dex2DB"
 - "dexar"
 - "dexqv"
 - "dexta"
 - "dextract"
 - "undexar"
 - "undexqv"
 - "undexta"
 - "mirror_server"
 - "mirror_server_stop"
 - "h5clear"
 - "h5format_convert"
 - "h5watch"
 - "h5fc"
 - "gif2h5"
 - "h52gif"
 - "h5c++"
 - "h5copy"
versions:
 - "1.0p2--h7a6849f_5"
description: "shpc-registry automated BioContainers addition for dextractor"
config: {"url": "https://biocontainers.pro/tools/dextractor", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for dextractor", "latest": {"1.0p2--h7a6849f_5": "sha256:6ce12cec2c4d2e2ff88acb7d37b7566e33200f6ad4ad846209555826e754ec96"}, "tags": {"1.0p2--h7a6849f_5": "sha256:6ce12cec2c4d2e2ff88acb7d37b7566e33200f6ad4ad846209555826e754ec96"}, "docker": "quay.io/biocontainers/dextractor", "aliases": {"dex2DB": "/usr/local/bin/dex2DB", "dexar": "/usr/local/bin/dexar", "dexqv": "/usr/local/bin/dexqv", "dexta": "/usr/local/bin/dexta", "dextract": "/usr/local/bin/dextract", "undexar": "/usr/local/bin/undexar", "undexqv": "/usr/local/bin/undexqv", "undexta": "/usr/local/bin/undexta", "mirror_server": "/usr/local/bin/mirror_server", "mirror_server_stop": "/usr/local/bin/mirror_server_stop", "h5clear": "/usr/local/bin/h5clear", "h5format_convert": "/usr/local/bin/h5format_convert", "h5watch": "/usr/local/bin/h5watch", "h5fc": "/usr/local/bin/h5fc", "gif2h5": "/usr/local/bin/gif2h5", "h52gif": "/usr/local/bin/h52gif", "h5c++": "/usr/local/bin/h5c++", "h5copy": "/usr/local/bin/h5copy"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/dextractor.
shpc-registry automated BioContainers addition for dextractor
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/dextractor
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/dextractor:1.0p2--h7a6849f_5
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/dextractor/1.0p2--h7a6849f_5
$ module help quay.io/biocontainers/dextractor/1.0p2--h7a6849f_5
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### dextractor-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### dextractor-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### dextractor-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### dextractor-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### dextractor-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### dextractor-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### dex2DB

```bash
$ singularity exec <container> /usr/local/bin/dex2DB
$ podman run --it --rm --entrypoint /usr/local/bin/dex2DB   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/dex2DB   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### dexar

```bash
$ singularity exec <container> /usr/local/bin/dexar
$ podman run --it --rm --entrypoint /usr/local/bin/dexar   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/dexar   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### dexqv

```bash
$ singularity exec <container> /usr/local/bin/dexqv
$ podman run --it --rm --entrypoint /usr/local/bin/dexqv   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/dexqv   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### dexta

```bash
$ singularity exec <container> /usr/local/bin/dexta
$ podman run --it --rm --entrypoint /usr/local/bin/dexta   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/dexta   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### dextract

```bash
$ singularity exec <container> /usr/local/bin/dextract
$ podman run --it --rm --entrypoint /usr/local/bin/dextract   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/dextract   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### undexar

```bash
$ singularity exec <container> /usr/local/bin/undexar
$ podman run --it --rm --entrypoint /usr/local/bin/undexar   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/undexar   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### undexqv

```bash
$ singularity exec <container> /usr/local/bin/undexqv
$ podman run --it --rm --entrypoint /usr/local/bin/undexqv   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/undexqv   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### undexta

```bash
$ singularity exec <container> /usr/local/bin/undexta
$ podman run --it --rm --entrypoint /usr/local/bin/undexta   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/undexta   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### mirror_server

```bash
$ singularity exec <container> /usr/local/bin/mirror_server
$ podman run --it --rm --entrypoint /usr/local/bin/mirror_server   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/mirror_server   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### mirror_server_stop

```bash
$ singularity exec <container> /usr/local/bin/mirror_server_stop
$ podman run --it --rm --entrypoint /usr/local/bin/mirror_server_stop   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/mirror_server_stop   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### h5clear

```bash
$ singularity exec <container> /usr/local/bin/h5clear
$ podman run --it --rm --entrypoint /usr/local/bin/h5clear   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/h5clear   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### h5format_convert

```bash
$ singularity exec <container> /usr/local/bin/h5format_convert
$ podman run --it --rm --entrypoint /usr/local/bin/h5format_convert   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/h5format_convert   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### h5watch

```bash
$ singularity exec <container> /usr/local/bin/h5watch
$ podman run --it --rm --entrypoint /usr/local/bin/h5watch   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/h5watch   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### h5fc

```bash
$ singularity exec <container> /usr/local/bin/h5fc
$ podman run --it --rm --entrypoint /usr/local/bin/h5fc   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/h5fc   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### gif2h5

```bash
$ singularity exec <container> /usr/local/bin/gif2h5
$ podman run --it --rm --entrypoint /usr/local/bin/gif2h5   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/gif2h5   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### h52gif

```bash
$ singularity exec <container> /usr/local/bin/h52gif
$ podman run --it --rm --entrypoint /usr/local/bin/h52gif   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/h52gif   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### h5c++

```bash
$ singularity exec <container> /usr/local/bin/h5c++
$ podman run --it --rm --entrypoint /usr/local/bin/h5c++   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/h5c++   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### h5copy

```bash
$ singularity exec <container> /usr/local/bin/h5copy
$ podman run --it --rm --entrypoint /usr/local/bin/h5copy   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/h5copy   -v ${PWD} -w ${PWD} <container> -c " $@"
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