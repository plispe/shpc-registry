---
layout: container
name:  "quay.io/biocontainers/bioconductor-affyplm"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-affyplm/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-affyplm/container.yaml"
updated_at: "2023-01-13 03:09:20.669890"
latest: "1.74.0--r42hc0cfd56_0"
container_url: "https://biocontainers.pro/tools/bioconductor-affyplm"

versions:
 - "1.70.0--r41hc0cfd56_2"
 - "1.74.0--r42hc0cfd56_0"
description: "shpc-registry automated BioContainers addition for bioconductor-affyplm"
config: {"url": "https://biocontainers.pro/tools/bioconductor-affyplm", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-affyplm", "latest": {"1.74.0--r42hc0cfd56_0": "sha256:91e22a83bbff3832ecc6935197beaaf6aeb9fee549e2cd4952fb705ac17b9143"}, "tags": {"1.70.0--r41hc0cfd56_2": "sha256:eda663877f2478247ccac4287c240dea3688a64e17b829eddab73758add10279", "1.74.0--r42hc0cfd56_0": "sha256:91e22a83bbff3832ecc6935197beaaf6aeb9fee549e2cd4952fb705ac17b9143"}, "docker": "quay.io/biocontainers/bioconductor-affyplm"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-affyplm.
shpc-registry automated BioContainers addition for bioconductor-affyplm
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-affyplm
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-affyplm:1.74.0--r42hc0cfd56_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-affyplm/1.74.0--r42hc0cfd56_0
$ module help quay.io/biocontainers/bioconductor-affyplm/1.74.0--r42hc0cfd56_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-affyplm-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-affyplm-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-affyplm-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-affyplm-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-affyplm-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-affyplm-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-affyplm

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