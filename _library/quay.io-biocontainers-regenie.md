---
layout: container
name:  "quay.io/biocontainers/regenie"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/regenie/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/regenie/container.yaml"
updated_at: "2023-01-13 03:16:57.312753"
latest: "3.2.3--h2b233e7_0"
container_url: "https://biocontainers.pro/tools/regenie"
aliases:
 - "regenie"
versions:
 - "3.2.1--h2b233e7_0"
 - "3.2.2.1--h2b233e7_0"
 - "3.2.3--h2b233e7_0"
description: "shpc-registry automated BioContainers addition for regenie"
config: {"url": "https://biocontainers.pro/tools/regenie", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for regenie", "latest": {"3.2.3--h2b233e7_0": "sha256:e27627a48b73f8b9445925680fd1ca3e0842481523af310f288ef9179b6313b0"}, "tags": {"3.2.1--h2b233e7_0": "sha256:fcba678511c3aa20834806a63412cdbb01efdd0936e13867e371c82e530e92f4", "3.2.2.1--h2b233e7_0": "sha256:80b207405ae5421d0eae3e005a6b47243a22828125df5b97631198d234231aff", "3.2.3--h2b233e7_0": "sha256:e27627a48b73f8b9445925680fd1ca3e0842481523af310f288ef9179b6313b0"}, "docker": "quay.io/biocontainers/regenie", "aliases": {"regenie": "/usr/local/bin/regenie"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/regenie.
shpc-registry automated BioContainers addition for regenie
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/regenie
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/regenie:3.2.3--h2b233e7_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/regenie/3.2.3--h2b233e7_0
$ module help quay.io/biocontainers/regenie/3.2.3--h2b233e7_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### regenie-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### regenie-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### regenie-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### regenie-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### regenie-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### regenie-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### regenie

```bash
$ singularity exec <container> /usr/local/bin/regenie
$ podman run --it --rm --entrypoint /usr/local/bin/regenie   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/regenie   -v ${PWD} -w ${PWD} <container> -c " $@"
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