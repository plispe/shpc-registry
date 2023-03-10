---
layout: container
name:  "quay.io/biocontainers/r-dimsum"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/r-dimsum/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/r-dimsum/container.yaml"
updated_at: "2023-01-13 03:35:45.780358"
latest: "1.2.11--r42hdfd78af_1"
container_url: "https://biocontainers.pro/tools/r-dimsum"
aliases:
 - "DiMSum"
 - "DiMSum.R"
 - "starcode"
 - "cutadapt"
 - "vsearch"
 - "fastqc"
 - "igzip"
 - "pbunzip2"
 - "pbzcat"
 - "pbzip2"
 - "pigz"
 - "unpigz"
 - "pandoc"
versions:
 - "1.2.9--r41hdfd78af_0"
 - "1.2.11--r42hdfd78af_1"
description: "shpc-registry automated BioContainers addition for r-dimsum"
config: {"url": "https://biocontainers.pro/tools/r-dimsum", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for r-dimsum", "latest": {"1.2.11--r42hdfd78af_1": "sha256:49dc119451afd6a109d76423a93241ab43ec9f988bcc4182ff8debdede1b790a"}, "tags": {"1.2.9--r41hdfd78af_0": "sha256:93b3f9f4310f3c370e5bfd09963575f6b8728c94342e3d6a4d0e1ea7d2d0f78e", "1.2.11--r42hdfd78af_1": "sha256:49dc119451afd6a109d76423a93241ab43ec9f988bcc4182ff8debdede1b790a"}, "docker": "quay.io/biocontainers/r-dimsum", "aliases": {"DiMSum": "/usr/local/bin/DiMSum", "DiMSum.R": "/usr/local/bin/DiMSum.R", "starcode": "/usr/local/bin/starcode", "cutadapt": "/usr/local/bin/cutadapt", "vsearch": "/usr/local/bin/vsearch", "fastqc": "/usr/local/bin/fastqc", "igzip": "/usr/local/bin/igzip", "pbunzip2": "/usr/local/bin/pbunzip2", "pbzcat": "/usr/local/bin/pbzcat", "pbzip2": "/usr/local/bin/pbzip2", "pigz": "/usr/local/bin/pigz", "unpigz": "/usr/local/bin/unpigz", "pandoc": "/usr/local/bin/pandoc"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/r-dimsum.
shpc-registry automated BioContainers addition for r-dimsum
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/r-dimsum
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/r-dimsum:1.2.11--r42hdfd78af_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/r-dimsum/1.2.11--r42hdfd78af_1
$ module help quay.io/biocontainers/r-dimsum/1.2.11--r42hdfd78af_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### r-dimsum-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### r-dimsum-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### r-dimsum-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### r-dimsum-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### r-dimsum-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### r-dimsum-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### DiMSum

```bash
$ singularity exec <container> /usr/local/bin/DiMSum
$ podman run --it --rm --entrypoint /usr/local/bin/DiMSum   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/DiMSum   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### DiMSum.R

```bash
$ singularity exec <container> /usr/local/bin/DiMSum.R
$ podman run --it --rm --entrypoint /usr/local/bin/DiMSum.R   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/DiMSum.R   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### starcode

```bash
$ singularity exec <container> /usr/local/bin/starcode
$ podman run --it --rm --entrypoint /usr/local/bin/starcode   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/starcode   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### cutadapt

```bash
$ singularity exec <container> /usr/local/bin/cutadapt
$ podman run --it --rm --entrypoint /usr/local/bin/cutadapt   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/cutadapt   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### vsearch

```bash
$ singularity exec <container> /usr/local/bin/vsearch
$ podman run --it --rm --entrypoint /usr/local/bin/vsearch   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/vsearch   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### fastqc

```bash
$ singularity exec <container> /usr/local/bin/fastqc
$ podman run --it --rm --entrypoint /usr/local/bin/fastqc   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/fastqc   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### igzip

```bash
$ singularity exec <container> /usr/local/bin/igzip
$ podman run --it --rm --entrypoint /usr/local/bin/igzip   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/igzip   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pbunzip2

```bash
$ singularity exec <container> /usr/local/bin/pbunzip2
$ podman run --it --rm --entrypoint /usr/local/bin/pbunzip2   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pbunzip2   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pbzcat

```bash
$ singularity exec <container> /usr/local/bin/pbzcat
$ podman run --it --rm --entrypoint /usr/local/bin/pbzcat   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pbzcat   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pbzip2

```bash
$ singularity exec <container> /usr/local/bin/pbzip2
$ podman run --it --rm --entrypoint /usr/local/bin/pbzip2   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pbzip2   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pigz

```bash
$ singularity exec <container> /usr/local/bin/pigz
$ podman run --it --rm --entrypoint /usr/local/bin/pigz   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pigz   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### unpigz

```bash
$ singularity exec <container> /usr/local/bin/unpigz
$ podman run --it --rm --entrypoint /usr/local/bin/unpigz   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/unpigz   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pandoc

```bash
$ singularity exec <container> /usr/local/bin/pandoc
$ podman run --it --rm --entrypoint /usr/local/bin/pandoc   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pandoc   -v ${PWD} -w ${PWD} <container> -c " $@"
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