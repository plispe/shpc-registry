---
layout: container
name:  "quay.io/biocontainers/bioconductor-dirichletmultinomial"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-dirichletmultinomial/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-dirichletmultinomial/container.yaml"
updated_at: "2023-01-13 02:57:02.677240"
latest: "1.40.0--r42hda872b5_0"
container_url: "https://biocontainers.pro/tools/bioconductor-dirichletmultinomial"

versions:
 - "1.36.0--r41hda872b5_3"
 - "1.40.0--r42hda872b5_0"
description: "shpc-registry automated BioContainers addition for bioconductor-dirichletmultinomial"
config: {"url": "https://biocontainers.pro/tools/bioconductor-dirichletmultinomial", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-dirichletmultinomial", "latest": {"1.40.0--r42hda872b5_0": "sha256:ce47eed3da7e84a71fffc84426124bddf80f1534ba840a9796fee754909b00df"}, "tags": {"1.36.0--r41hda872b5_3": "sha256:255216cfe4681869fe889960d05b957dfe3ac2cecc8f37babb15e02cf3725c32", "1.40.0--r42hda872b5_0": "sha256:ce47eed3da7e84a71fffc84426124bddf80f1534ba840a9796fee754909b00df"}, "docker": "quay.io/biocontainers/bioconductor-dirichletmultinomial"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-dirichletmultinomial.
shpc-registry automated BioContainers addition for bioconductor-dirichletmultinomial
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-dirichletmultinomial
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-dirichletmultinomial:1.40.0--r42hda872b5_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-dirichletmultinomial/1.40.0--r42hda872b5_0
$ module help quay.io/biocontainers/bioconductor-dirichletmultinomial/1.40.0--r42hda872b5_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-dirichletmultinomial-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-dirichletmultinomial-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-dirichletmultinomial-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-dirichletmultinomial-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-dirichletmultinomial-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-dirichletmultinomial-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-dirichletmultinomial

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