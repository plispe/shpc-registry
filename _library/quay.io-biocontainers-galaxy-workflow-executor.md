---
layout: container
name:  "quay.io/biocontainers/galaxy-workflow-executor"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/galaxy-workflow-executor/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/galaxy-workflow-executor/container.yaml"
updated_at: "2023-01-13 02:59:12.250268"
latest: "0.2.6--pyh5e36f6f_0"
container_url: "https://biocontainers.pro/tools/galaxy-workflow-executor"
aliases:
 - "bioblend-galaxy-tests"
 - "generate_params_from_workflow.py"
 - "run_galaxy_workflow.py"
 - "asadmin"
 - "bundle_image"
 - "cfadmin"
 - "cq"
 - "cwutil"
 - "dynamodb_dump"
 - "dynamodb_load"
 - "elbadmin"
 - "fetch_file"
 - "glacier"
versions:
 - "0.2.6--pyh5e36f6f_0"
description: "shpc-registry automated BioContainers addition for galaxy-workflow-executor"
config: {"url": "https://biocontainers.pro/tools/galaxy-workflow-executor", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for galaxy-workflow-executor", "latest": {"0.2.6--pyh5e36f6f_0": "sha256:0337c95e597e44e0a4a516d264b271e4ded01f63ba9091815994ec8b7292d744"}, "tags": {"0.2.6--pyh5e36f6f_0": "sha256:0337c95e597e44e0a4a516d264b271e4ded01f63ba9091815994ec8b7292d744"}, "docker": "quay.io/biocontainers/galaxy-workflow-executor", "aliases": {"bioblend-galaxy-tests": "/usr/local/bin/bioblend-galaxy-tests", "generate_params_from_workflow.py": "/usr/local/bin/generate_params_from_workflow.py", "run_galaxy_workflow.py": "/usr/local/bin/run_galaxy_workflow.py", "asadmin": "/usr/local/bin/asadmin", "bundle_image": "/usr/local/bin/bundle_image", "cfadmin": "/usr/local/bin/cfadmin", "cq": "/usr/local/bin/cq", "cwutil": "/usr/local/bin/cwutil", "dynamodb_dump": "/usr/local/bin/dynamodb_dump", "dynamodb_load": "/usr/local/bin/dynamodb_load", "elbadmin": "/usr/local/bin/elbadmin", "fetch_file": "/usr/local/bin/fetch_file", "glacier": "/usr/local/bin/glacier"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/galaxy-workflow-executor.
shpc-registry automated BioContainers addition for galaxy-workflow-executor
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/galaxy-workflow-executor
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/galaxy-workflow-executor:0.2.6--pyh5e36f6f_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/galaxy-workflow-executor/0.2.6--pyh5e36f6f_0
$ module help quay.io/biocontainers/galaxy-workflow-executor/0.2.6--pyh5e36f6f_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### galaxy-workflow-executor-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### galaxy-workflow-executor-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### galaxy-workflow-executor-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### galaxy-workflow-executor-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### galaxy-workflow-executor-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### galaxy-workflow-executor-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### bioblend-galaxy-tests

```bash
$ singularity exec <container> /usr/local/bin/bioblend-galaxy-tests
$ podman run --it --rm --entrypoint /usr/local/bin/bioblend-galaxy-tests   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/bioblend-galaxy-tests   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### generate_params_from_workflow.py

```bash
$ singularity exec <container> /usr/local/bin/generate_params_from_workflow.py
$ podman run --it --rm --entrypoint /usr/local/bin/generate_params_from_workflow.py   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/generate_params_from_workflow.py   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### run_galaxy_workflow.py

```bash
$ singularity exec <container> /usr/local/bin/run_galaxy_workflow.py
$ podman run --it --rm --entrypoint /usr/local/bin/run_galaxy_workflow.py   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/run_galaxy_workflow.py   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### asadmin

```bash
$ singularity exec <container> /usr/local/bin/asadmin
$ podman run --it --rm --entrypoint /usr/local/bin/asadmin   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/asadmin   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### bundle_image

```bash
$ singularity exec <container> /usr/local/bin/bundle_image
$ podman run --it --rm --entrypoint /usr/local/bin/bundle_image   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/bundle_image   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### cfadmin

```bash
$ singularity exec <container> /usr/local/bin/cfadmin
$ podman run --it --rm --entrypoint /usr/local/bin/cfadmin   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/cfadmin   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### cq

```bash
$ singularity exec <container> /usr/local/bin/cq
$ podman run --it --rm --entrypoint /usr/local/bin/cq   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/cq   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### cwutil

```bash
$ singularity exec <container> /usr/local/bin/cwutil
$ podman run --it --rm --entrypoint /usr/local/bin/cwutil   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/cwutil   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### dynamodb_dump

```bash
$ singularity exec <container> /usr/local/bin/dynamodb_dump
$ podman run --it --rm --entrypoint /usr/local/bin/dynamodb_dump   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/dynamodb_dump   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### dynamodb_load

```bash
$ singularity exec <container> /usr/local/bin/dynamodb_load
$ podman run --it --rm --entrypoint /usr/local/bin/dynamodb_load   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/dynamodb_load   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### elbadmin

```bash
$ singularity exec <container> /usr/local/bin/elbadmin
$ podman run --it --rm --entrypoint /usr/local/bin/elbadmin   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/elbadmin   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### fetch_file

```bash
$ singularity exec <container> /usr/local/bin/fetch_file
$ podman run --it --rm --entrypoint /usr/local/bin/fetch_file   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/fetch_file   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### glacier

```bash
$ singularity exec <container> /usr/local/bin/glacier
$ podman run --it --rm --entrypoint /usr/local/bin/glacier   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/glacier   -v ${PWD} -w ${PWD} <container> -c " $@"
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