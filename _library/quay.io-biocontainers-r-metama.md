---
layout: container
name:  "quay.io/biocontainers/r-metama"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/r-metama/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/r-metama/container.yaml"
updated_at: "2023-01-13 03:26:48.906860"
latest: "3.1.3--r42h3121a25_1"
container_url: "https://biocontainers.pro/tools/r-metama"

versions:
 - "3.1.3--r41h3121a25_0"
 - "3.1.3--r42h3121a25_1"
description: "shpc-registry automated BioContainers addition for r-metama"
config: {"url": "https://biocontainers.pro/tools/r-metama", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for r-metama", "latest": {"3.1.3--r42h3121a25_1": "sha256:575e5f635b599712be9dd8f3951ee6afd13bf709578b0b17ac622f7053d11040"}, "tags": {"3.1.3--r41h3121a25_0": "sha256:a29a5c52a5256267dd8cbd52754cca5e9d501065e9d5fa129812ae7c1f46d004", "3.1.3--r42h3121a25_1": "sha256:575e5f635b599712be9dd8f3951ee6afd13bf709578b0b17ac622f7053d11040"}, "docker": "quay.io/biocontainers/r-metama"}
---

This module is a singularity container wrapper for quay.io/biocontainers/r-metama.
shpc-registry automated BioContainers addition for r-metama
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/r-metama
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/r-metama:3.1.3--r42h3121a25_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/r-metama/3.1.3--r42h3121a25_1
$ module help quay.io/biocontainers/r-metama/3.1.3--r42h3121a25_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### r-metama-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### r-metama-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### r-metama-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### r-metama-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### r-metama-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### r-metama-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### r-metama

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
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