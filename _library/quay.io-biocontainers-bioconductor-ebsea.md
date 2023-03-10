---
layout: container
name:  "quay.io/biocontainers/bioconductor-ebsea"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-ebsea/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-ebsea/container.yaml"
updated_at: "2023-01-13 02:55:53.793532"
latest: "1.26.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-ebsea"

versions:
 - "1.8.0--r351_0"
 - "1.26.0--r42hdfd78af_0"
 - "1.22.0--r41hdfd78af_0"
 - "1.20.0--r41hdfd78af_0"
 - "1.18.0--r40hdfd78af_1"
 - "1.16.0--r40_0"
description: "shpc-registry automated BioContainers addition for bioconductor-ebsea"
config: {"url": "https://biocontainers.pro/tools/bioconductor-ebsea", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-ebsea", "latest": {"1.26.0--r42hdfd78af_0": "sha256:ac87c0255520af14875eb968245e0232bc8b291ae501a687f5cfd5d8e7425096"}, "tags": {"1.8.0--r351_0": "sha256:962cdfbe5d182a89b133c1ec45f1cccf62abbcbe077ea3e26aedf28c8266dd40", "1.26.0--r42hdfd78af_0": "sha256:ac87c0255520af14875eb968245e0232bc8b291ae501a687f5cfd5d8e7425096", "1.22.0--r41hdfd78af_0": "sha256:9ca414092e6929812fe605bf3f759dcdfdd7104550a64fa1035d523fb32a781b", "1.20.0--r41hdfd78af_0": "sha256:8d85752c2b4672fcec9be543337f932239573f0cc0ddbee970327f12729fdc3c", "1.18.0--r40hdfd78af_1": "sha256:d81576f4a242b6e9e5870d2b55ed26083659760cabc8d9e9af3f090813cdd55b", "1.16.0--r40_0": "sha256:03a31952031ac44ed3bddae44f047359027f9c704e2a8cf74d94eff60b580b35"}, "docker": "quay.io/biocontainers/bioconductor-ebsea"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-ebsea.
shpc-registry automated BioContainers addition for bioconductor-ebsea
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-ebsea
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-ebsea:1.26.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-ebsea/1.26.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-ebsea/1.26.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-ebsea-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ebsea-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-ebsea-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-ebsea-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-ebsea-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-ebsea-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-ebsea

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