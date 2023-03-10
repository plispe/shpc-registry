---
layout: container
name:  "quay.io/biocontainers/ncbi-ngs-sdk"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/ncbi-ngs-sdk/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/ncbi-ngs-sdk/container.yaml"
updated_at: "2023-01-13 02:49:01.154436"
latest: "3.0.1--pl5321h629fbf0_0"
container_url: "https://biocontainers.pro/tools/ncbi-ngs-sdk"

versions:
 - "2.9.3--h550f44e_0"
 - "2.11.2--pl5321h629fbf0_1"
 - "2.10.9--hff44eed_1"
 - "3.0.1--pl5321h629fbf0_0"
description: "shpc-registry automated BioContainers addition for ncbi-ngs-sdk"
config: {"url": "https://biocontainers.pro/tools/ncbi-ngs-sdk", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for ncbi-ngs-sdk", "latest": {"3.0.1--pl5321h629fbf0_0": "sha256:e2cf83b838413148c86b635931ad4188efc27886ef716e814aa42195b237e95e"}, "tags": {"2.9.3--h550f44e_0": "sha256:1c812d0ca140f83a5d6ffe5ddcae56ba22b0ce1319c874e3e686eee3f3da4b4b", "2.11.2--pl5321h629fbf0_1": "sha256:9327c997f364619cdf6aa5b3d0f160aab253cebe73e9260e52056c21434a293a", "2.10.9--hff44eed_1": "sha256:b547e797dbd2b7554f1aa423e6ab41a282613e8606a64c70c164920cedc36e37", "3.0.1--pl5321h629fbf0_0": "sha256:e2cf83b838413148c86b635931ad4188efc27886ef716e814aa42195b237e95e"}, "docker": "quay.io/biocontainers/ncbi-ngs-sdk"}
---

This module is a singularity container wrapper for quay.io/biocontainers/ncbi-ngs-sdk.
shpc-registry automated BioContainers addition for ncbi-ngs-sdk
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/ncbi-ngs-sdk
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/ncbi-ngs-sdk:3.0.1--pl5321h629fbf0_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/ncbi-ngs-sdk/3.0.1--pl5321h629fbf0_0
$ module help quay.io/biocontainers/ncbi-ngs-sdk/3.0.1--pl5321h629fbf0_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### ncbi-ngs-sdk-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### ncbi-ngs-sdk-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### ncbi-ngs-sdk-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### ncbi-ngs-sdk-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### ncbi-ngs-sdk-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### ncbi-ngs-sdk-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### ncbi-ngs-sdk

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