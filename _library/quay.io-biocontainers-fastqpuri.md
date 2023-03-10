---
layout: container
name:  "quay.io/biocontainers/fastqpuri"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/fastqpuri/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/fastqpuri/container.yaml"
updated_at: "2023-01-13 03:39:15.561527"
latest: "1.0.7--r41h67092d7_4"
container_url: "https://biocontainers.pro/tools/fastqpuri"
aliases:
 - "Qreport"
 - "Sreport"
 - "makeBloom"
 - "makeTree"
 - "trimFilter"
 - "trimFilterPE"
 - "pandoc"
versions:
 - "1.0.7--r41h67092d7_4"
description: "shpc-registry automated BioContainers addition for fastqpuri"
config: {"url": "https://biocontainers.pro/tools/fastqpuri", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for fastqpuri", "latest": {"1.0.7--r41h67092d7_4": "sha256:986507af918272086f85cdb538c7d0bb18bd641b045c49d2979ed1d68a64ba73"}, "tags": {"1.0.7--r41h67092d7_4": "sha256:986507af918272086f85cdb538c7d0bb18bd641b045c49d2979ed1d68a64ba73"}, "docker": "quay.io/biocontainers/fastqpuri", "aliases": {"Qreport": "/usr/local/bin/Qreport", "Sreport": "/usr/local/bin/Sreport", "makeBloom": "/usr/local/bin/makeBloom", "makeTree": "/usr/local/bin/makeTree", "trimFilter": "/usr/local/bin/trimFilter", "trimFilterPE": "/usr/local/bin/trimFilterPE", "pandoc": "/usr/local/bin/pandoc"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/fastqpuri.
shpc-registry automated BioContainers addition for fastqpuri
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/fastqpuri
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/fastqpuri:1.0.7--r41h67092d7_4
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/fastqpuri/1.0.7--r41h67092d7_4
$ module help quay.io/biocontainers/fastqpuri/1.0.7--r41h67092d7_4
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### fastqpuri-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### fastqpuri-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### fastqpuri-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### fastqpuri-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### fastqpuri-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### fastqpuri-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### Qreport

```bash
$ singularity exec <container> /usr/local/bin/Qreport
$ podman run --it --rm --entrypoint /usr/local/bin/Qreport   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/Qreport   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### Sreport

```bash
$ singularity exec <container> /usr/local/bin/Sreport
$ podman run --it --rm --entrypoint /usr/local/bin/Sreport   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/Sreport   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### makeBloom

```bash
$ singularity exec <container> /usr/local/bin/makeBloom
$ podman run --it --rm --entrypoint /usr/local/bin/makeBloom   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/makeBloom   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### makeTree

```bash
$ singularity exec <container> /usr/local/bin/makeTree
$ podman run --it --rm --entrypoint /usr/local/bin/makeTree   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/makeTree   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### trimFilter

```bash
$ singularity exec <container> /usr/local/bin/trimFilter
$ podman run --it --rm --entrypoint /usr/local/bin/trimFilter   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/trimFilter   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### trimFilterPE

```bash
$ singularity exec <container> /usr/local/bin/trimFilterPE
$ podman run --it --rm --entrypoint /usr/local/bin/trimFilterPE   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/trimFilterPE   -v ${PWD} -w ${PWD} <container> -c " $@"
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