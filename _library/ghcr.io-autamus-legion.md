---
layout: container
name:  "ghcr.io/autamus/legion"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/ghcr.io/autamus/legion/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/ghcr.io/autamus/legion/container.yaml"
updated_at: "2023-01-13 03:47:12.306476"
latest: "21.03.0"
container_url: "https://github.com/orgs/autamus/packages/container/package/legion"
aliases:
 - "legion_prof.py"
 - "legion_serializer.py"
 - "legion_spy.py"
versions:
 - "21.03.0"
 - "latest"
description: "Legion is a data-centric parallel programming system for writing portable high performance programs targeted at distributed heterogeneous architectures."
config: {"docker": "ghcr.io/autamus/legion", "url": "https://github.com/orgs/autamus/packages/container/package/legion", "maintainer": "@vsoch", "description": "Legion is a data-centric parallel programming system for writing portable high performance programs targeted at distributed heterogeneous architectures.", "latest": {"21.03.0": "sha256:86251e961b1c9a01954bbfd123c7e69a4cf8a70014f586beac9365ca9e4a3e1c"}, "tags": {"21.03.0": "sha256:86251e961b1c9a01954bbfd123c7e69a4cf8a70014f586beac9365ca9e4a3e1c", "latest": "sha256:86251e961b1c9a01954bbfd123c7e69a4cf8a70014f586beac9365ca9e4a3e1c"}, "aliases": {"legion_prof.py": "/opt/view/bin/legion_prof.py", "legion_serializer.py": "/opt/view/bin/legion_serializer.py", "legion_spy.py": "/opt/view/bin/legion_spy.py"}}
---

This module is a singularity container wrapper for ghcr.io/autamus/legion.
Legion is a data-centric parallel programming system for writing portable high performance programs targeted at distributed heterogeneous architectures.
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install ghcr.io/autamus/legion
```

Or a specific version:

```bash
$ shpc install ghcr.io/autamus/legion:21.03.0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load ghcr.io/autamus/legion/21.03.0
$ module help ghcr.io/autamus/legion/21.03.0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### legion-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### legion-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### legion-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### legion-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### legion-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### legion-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### legion_prof.py

```bash
$ singularity exec <container> /opt/view/bin/legion_prof.py
$ podman run --it --rm --entrypoint /opt/view/bin/legion_prof.py   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /opt/view/bin/legion_prof.py   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### legion_serializer.py

```bash
$ singularity exec <container> /opt/view/bin/legion_serializer.py
$ podman run --it --rm --entrypoint /opt/view/bin/legion_serializer.py   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /opt/view/bin/legion_serializer.py   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### legion_spy.py

```bash
$ singularity exec <container> /opt/view/bin/legion_spy.py
$ podman run --it --rm --entrypoint /opt/view/bin/legion_spy.py   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /opt/view/bin/legion_spy.py   -v ${PWD} -w ${PWD} <container> -c " $@"
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