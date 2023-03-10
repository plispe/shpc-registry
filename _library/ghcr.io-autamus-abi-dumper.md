---
layout: container
name:  "ghcr.io/autamus/abi-dumper"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/ghcr.io/autamus/abi-dumper/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/ghcr.io/autamus/abi-dumper/container.yaml"
updated_at: "2023-01-13 03:47:11.894168"
latest: "1.2"
container_url: "https://github.com/orgs/autamus/packages/container/package/abi-dumper"
aliases:
 - "abi-dumper"
versions:
 - "1.2"
 - "latest"
description: "ABI Dumper is a tool for dumping ABI information of an ELF object containing DWARF debug info."
config: {"docker": "ghcr.io/autamus/abi-dumper", "url": "https://github.com/orgs/autamus/packages/container/package/abi-dumper", "maintainer": "@vsoch", "description": "ABI Dumper is a tool for dumping ABI information of an ELF object containing DWARF debug info.", "latest": {"1.2": "sha256:53c6bb9fa5bf0f0029580dff7f48bb5f410657f8acb497b5a80504355407da9f"}, "tags": {"1.2": "sha256:53c6bb9fa5bf0f0029580dff7f48bb5f410657f8acb497b5a80504355407da9f", "latest": "sha256:53c6bb9fa5bf0f0029580dff7f48bb5f410657f8acb497b5a80504355407da9f"}, "aliases": {"abi-dumper": "/opt/view/bin/abi-dumper"}}
---

This module is a singularity container wrapper for ghcr.io/autamus/abi-dumper.
ABI Dumper is a tool for dumping ABI information of an ELF object containing DWARF debug info.
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install ghcr.io/autamus/abi-dumper
```

Or a specific version:

```bash
$ shpc install ghcr.io/autamus/abi-dumper:1.2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load ghcr.io/autamus/abi-dumper/1.2
$ module help ghcr.io/autamus/abi-dumper/1.2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### abi-dumper-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### abi-dumper-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### abi-dumper-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### abi-dumper-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### abi-dumper-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### abi-dumper-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### abi-dumper

```bash
$ singularity exec <container> /opt/view/bin/abi-dumper
$ podman run --it --rm --entrypoint /opt/view/bin/abi-dumper   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /opt/view/bin/abi-dumper   -v ${PWD} -w ${PWD} <container> -c " $@"
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