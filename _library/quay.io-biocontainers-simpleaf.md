---
layout: container
name:  "quay.io/biocontainers/simpleaf"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/simpleaf/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/simpleaf/container.yaml"
updated_at: "2023-01-13 03:08:28.098565"
latest: "0.8.1--h9f5acd7_0"
container_url: "https://biocontainers.pro/tools/simpleaf"
aliases:
 - "alevin-fry"
 - "pyroe"
 - "simpleaf"
 - "salmon"
 - "scanpy"
 - "docutils"
 - "x86_64-conda_cos7-linux-gnu-ld"
 - "sphinx-apidoc"
 - "sphinx-autogen"
 - "sphinx-build"
 - "sphinx-quickstart"
 - "pybabel"
 - "tabulate"
versions:
 - "0.5.3--h9f5acd7_0"
 - "0.6.0--h9f5acd7_0"
 - "0.7.0--h9f5acd7_0"
 - "0.8.1--h9f5acd7_0"
description: "shpc-registry automated BioContainers addition for simpleaf"
config: {"url": "https://biocontainers.pro/tools/simpleaf", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for simpleaf", "latest": {"0.8.1--h9f5acd7_0": "sha256:874dbd54eab72081541c15ac90e27517fb0e8b92cf1c4b636c38ac3aadb3ffc6"}, "tags": {"0.5.3--h9f5acd7_0": "sha256:e3d091171880db081708f097fab967b6d6bfd517087b8da1ded720727356d032", "0.6.0--h9f5acd7_0": "sha256:fc9f851428207eb47fc4421c8e5c3bc7d3d0cd13a871d563a7342597da178ffe", "0.7.0--h9f5acd7_0": "sha256:262452b892c9255f684ccd13ace6385c31b0ef9e4291b80583eec2bdb4885f6e", "0.8.1--h9f5acd7_0": "sha256:874dbd54eab72081541c15ac90e27517fb0e8b92cf1c4b636c38ac3aadb3ffc6"}, "docker": "quay.io/biocontainers/simpleaf", "aliases": {"alevin-fry": "/usr/local/bin/alevin-fry", "pyroe": "/usr/local/bin/pyroe", "simpleaf": "/usr/local/bin/simpleaf", "salmon": "/usr/local/bin/salmon", "scanpy": "/usr/local/bin/scanpy", "docutils": "/usr/local/bin/docutils", "x86_64-conda_cos7-linux-gnu-ld": "/usr/local/bin/x86_64-conda_cos7-linux-gnu-ld", "sphinx-apidoc": "/usr/local/bin/sphinx-apidoc", "sphinx-autogen": "/usr/local/bin/sphinx-autogen", "sphinx-build": "/usr/local/bin/sphinx-build", "sphinx-quickstart": "/usr/local/bin/sphinx-quickstart", "pybabel": "/usr/local/bin/pybabel", "tabulate": "/usr/local/bin/tabulate"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/simpleaf.
shpc-registry automated BioContainers addition for simpleaf
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/simpleaf
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/simpleaf:0.8.1--h9f5acd7_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/simpleaf/0.8.1--h9f5acd7_0
$ module help quay.io/biocontainers/simpleaf/0.8.1--h9f5acd7_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### simpleaf-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### simpleaf-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### simpleaf-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### simpleaf-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### simpleaf-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### simpleaf-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### alevin-fry

```bash
$ singularity exec <container> /usr/local/bin/alevin-fry
$ podman run --it --rm --entrypoint /usr/local/bin/alevin-fry   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/alevin-fry   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pyroe

```bash
$ singularity exec <container> /usr/local/bin/pyroe
$ podman run --it --rm --entrypoint /usr/local/bin/pyroe   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pyroe   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### simpleaf

```bash
$ singularity exec <container> /usr/local/bin/simpleaf
$ podman run --it --rm --entrypoint /usr/local/bin/simpleaf   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/simpleaf   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### salmon

```bash
$ singularity exec <container> /usr/local/bin/salmon
$ podman run --it --rm --entrypoint /usr/local/bin/salmon   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/salmon   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### scanpy

```bash
$ singularity exec <container> /usr/local/bin/scanpy
$ podman run --it --rm --entrypoint /usr/local/bin/scanpy   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/scanpy   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### docutils

```bash
$ singularity exec <container> /usr/local/bin/docutils
$ podman run --it --rm --entrypoint /usr/local/bin/docutils   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/docutils   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### x86_64-conda_cos7-linux-gnu-ld

```bash
$ singularity exec <container> /usr/local/bin/x86_64-conda_cos7-linux-gnu-ld
$ podman run --it --rm --entrypoint /usr/local/bin/x86_64-conda_cos7-linux-gnu-ld   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/x86_64-conda_cos7-linux-gnu-ld   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### sphinx-apidoc

```bash
$ singularity exec <container> /usr/local/bin/sphinx-apidoc
$ podman run --it --rm --entrypoint /usr/local/bin/sphinx-apidoc   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/sphinx-apidoc   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### sphinx-autogen

```bash
$ singularity exec <container> /usr/local/bin/sphinx-autogen
$ podman run --it --rm --entrypoint /usr/local/bin/sphinx-autogen   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/sphinx-autogen   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### sphinx-build

```bash
$ singularity exec <container> /usr/local/bin/sphinx-build
$ podman run --it --rm --entrypoint /usr/local/bin/sphinx-build   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/sphinx-build   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### sphinx-quickstart

```bash
$ singularity exec <container> /usr/local/bin/sphinx-quickstart
$ podman run --it --rm --entrypoint /usr/local/bin/sphinx-quickstart   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/sphinx-quickstart   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pybabel

```bash
$ singularity exec <container> /usr/local/bin/pybabel
$ podman run --it --rm --entrypoint /usr/local/bin/pybabel   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pybabel   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### tabulate

```bash
$ singularity exec <container> /usr/local/bin/tabulate
$ podman run --it --rm --entrypoint /usr/local/bin/tabulate   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/tabulate   -v ${PWD} -w ${PWD} <container> -c " $@"
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