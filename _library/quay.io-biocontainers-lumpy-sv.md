---
layout: container
name:  "quay.io/biocontainers/lumpy-sv"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/lumpy-sv/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/lumpy-sv/container.yaml"
updated_at: "2023-01-13 03:33:22.070480"
latest: "0.3.1--hdfd78af_3"
container_url: "https://biocontainers.pro/tools/lumpy-sv"

versions:
 - "0.3.1--hdfd78af_3"
description: "shpc-registry automated BioContainers addition for lumpy-sv"
config: {"url": "https://biocontainers.pro/tools/lumpy-sv", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for lumpy-sv", "latest": {"0.3.1--hdfd78af_3": "sha256:9f39cc174d539e86dfe51fdc6b9d7c555908a934805c057525cf383729afc3c3"}, "tags": {"0.3.1--hdfd78af_3": "sha256:9f39cc174d539e86dfe51fdc6b9d7c555908a934805c057525cf383729afc3c3"}, "docker": "quay.io/biocontainers/lumpy-sv"}
---

This module is a singularity container wrapper for quay.io/biocontainers/lumpy-sv.
shpc-registry automated BioContainers addition for lumpy-sv
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/lumpy-sv
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/lumpy-sv:0.3.1--hdfd78af_3
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/lumpy-sv/0.3.1--hdfd78af_3
$ module help quay.io/biocontainers/lumpy-sv/0.3.1--hdfd78af_3
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### lumpy-sv-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### lumpy-sv-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### lumpy-sv-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### lumpy-sv-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### lumpy-sv-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### lumpy-sv-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### lumpy-sv

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