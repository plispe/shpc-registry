---
layout: container
name:  "quay.io/biocontainers/bioconductor-purecn"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-purecn/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-purecn/container.yaml"
updated_at: "2023-01-13 03:03:50.453691"
latest: "2.4.0--r42hdfd78af_0"
container_url: "https://biocontainers.pro/tools/bioconductor-purecn"

versions:
 - "2.0.2--r41hdfd78af_0"
 - "2.4.0--r42hdfd78af_0"
description: "shpc-registry automated BioContainers addition for bioconductor-purecn"
config: {"url": "https://biocontainers.pro/tools/bioconductor-purecn", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-purecn", "latest": {"2.4.0--r42hdfd78af_0": "sha256:f16a1db142358eb8484173db201478b5409433a536c6a982ddf838859ed5b259"}, "tags": {"2.0.2--r41hdfd78af_0": "sha256:a746e40a7f06b5491361003eaaade6c830e85e2365721461217373772f0a25c0", "2.4.0--r42hdfd78af_0": "sha256:f16a1db142358eb8484173db201478b5409433a536c6a982ddf838859ed5b259"}, "docker": "quay.io/biocontainers/bioconductor-purecn"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-purecn.
shpc-registry automated BioContainers addition for bioconductor-purecn
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-purecn
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-purecn:2.4.0--r42hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-purecn/2.4.0--r42hdfd78af_0
$ module help quay.io/biocontainers/bioconductor-purecn/2.4.0--r42hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-purecn-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-purecn-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-purecn-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-purecn-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-purecn-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-purecn-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-purecn

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