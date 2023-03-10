---
layout: container
name:  "quay.io/biocontainers/verkko"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/verkko/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/verkko/container.yaml"
updated_at: "2023-01-13 02:55:39.954309"
latest: "1.2--h64afbab_0"
container_url: "https://biocontainers.pro/tools/verkko"

versions:
 - "1.1--h64afbab_0"
 - "1.2--h64afbab_0"
 - "1.1--h64afbab_1"
description: "shpc-registry automated BioContainers addition for verkko"
config: {"url": "https://biocontainers.pro/tools/verkko", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for verkko", "latest": {"1.2--h64afbab_0": "sha256:d4f8db736d1df768b5afc2b5d8e4f29634356f6f51f0a6eb8c411a4835fbfb4f"}, "tags": {"1.1--h64afbab_0": "sha256:7f5e46ea6b03f3d1873c4a06b681f24a9db1bda10a03d4b0e59f0a4d881d6d4a", "1.2--h64afbab_0": "sha256:d4f8db736d1df768b5afc2b5d8e4f29634356f6f51f0a6eb8c411a4835fbfb4f", "1.1--h64afbab_1": "sha256:d88c307bac8a0dfed25ec704fe2a48ccb9fd306ff7f82e35797d9411765eada4"}, "docker": "quay.io/biocontainers/verkko"}
---

This module is a singularity container wrapper for quay.io/biocontainers/verkko.
shpc-registry automated BioContainers addition for verkko
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/verkko
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/verkko:1.2--h64afbab_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/verkko/1.2--h64afbab_0
$ module help quay.io/biocontainers/verkko/1.2--h64afbab_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### verkko-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### verkko-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### verkko-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### verkko-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### verkko-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### verkko-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### verkko

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