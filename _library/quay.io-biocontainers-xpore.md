---
layout: container
name:  "quay.io/biocontainers/xpore"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/xpore/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/xpore/container.yaml"
updated_at: "2023-01-13 03:12:36.102961"
latest: "2.1--pyh5e36f6f_0"
container_url: "https://biocontainers.pro/tools/xpore"
aliases:
 - "epylint"
 - "isort"
 - "isort-identify-imports"
 - "pyensembl"
 - "pylint"
 - "pyreverse"
 - "symilar"
 - "xpore"
 - "xpore-dataprep"
 - "xpore-diffmod"
 - "mirror_server"
 - "mirror_server_stop"
 - "chardetect"
 - "f2py3.9"
 - "h5clear"
 - "h5format_convert"
 - "h5watch"
 - "h5fc"
 - "gif2h5"
 - "h52gif"
versions:
 - "2.1--pyh5e36f6f_0"
description: "shpc-registry automated BioContainers addition for xpore"
config: {"url": "https://biocontainers.pro/tools/xpore", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for xpore", "latest": {"2.1--pyh5e36f6f_0": "sha256:5424b9d305ba65acb392496a740c731807a51de10689d117ad0c85b3991668f4"}, "tags": {"2.1--pyh5e36f6f_0": "sha256:5424b9d305ba65acb392496a740c731807a51de10689d117ad0c85b3991668f4"}, "docker": "quay.io/biocontainers/xpore", "aliases": {"epylint": "/usr/local/bin/epylint", "isort": "/usr/local/bin/isort", "isort-identify-imports": "/usr/local/bin/isort-identify-imports", "pyensembl": "/usr/local/bin/pyensembl", "pylint": "/usr/local/bin/pylint", "pyreverse": "/usr/local/bin/pyreverse", "symilar": "/usr/local/bin/symilar", "xpore": "/usr/local/bin/xpore", "xpore-dataprep": "/usr/local/bin/xpore-dataprep", "xpore-diffmod": "/usr/local/bin/xpore-diffmod", "mirror_server": "/usr/local/bin/mirror_server", "mirror_server_stop": "/usr/local/bin/mirror_server_stop", "chardetect": "/usr/local/bin/chardetect", "f2py3.9": "/usr/local/bin/f2py3.9", "h5clear": "/usr/local/bin/h5clear", "h5format_convert": "/usr/local/bin/h5format_convert", "h5watch": "/usr/local/bin/h5watch", "h5fc": "/usr/local/bin/h5fc", "gif2h5": "/usr/local/bin/gif2h5", "h52gif": "/usr/local/bin/h52gif"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/xpore.
shpc-registry automated BioContainers addition for xpore
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/xpore
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/xpore:2.1--pyh5e36f6f_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/xpore/2.1--pyh5e36f6f_0
$ module help quay.io/biocontainers/xpore/2.1--pyh5e36f6f_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### xpore-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### xpore-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### xpore-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### xpore-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### xpore-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### xpore-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### epylint

```bash
$ singularity exec <container> /usr/local/bin/epylint
$ podman run --it --rm --entrypoint /usr/local/bin/epylint   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/epylint   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### isort

```bash
$ singularity exec <container> /usr/local/bin/isort
$ podman run --it --rm --entrypoint /usr/local/bin/isort   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/isort   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### isort-identify-imports

```bash
$ singularity exec <container> /usr/local/bin/isort-identify-imports
$ podman run --it --rm --entrypoint /usr/local/bin/isort-identify-imports   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/isort-identify-imports   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pyensembl

```bash
$ singularity exec <container> /usr/local/bin/pyensembl
$ podman run --it --rm --entrypoint /usr/local/bin/pyensembl   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pyensembl   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pylint

```bash
$ singularity exec <container> /usr/local/bin/pylint
$ podman run --it --rm --entrypoint /usr/local/bin/pylint   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pylint   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pyreverse

```bash
$ singularity exec <container> /usr/local/bin/pyreverse
$ podman run --it --rm --entrypoint /usr/local/bin/pyreverse   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pyreverse   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### symilar

```bash
$ singularity exec <container> /usr/local/bin/symilar
$ podman run --it --rm --entrypoint /usr/local/bin/symilar   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/symilar   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### xpore

```bash
$ singularity exec <container> /usr/local/bin/xpore
$ podman run --it --rm --entrypoint /usr/local/bin/xpore   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/xpore   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### xpore-dataprep

```bash
$ singularity exec <container> /usr/local/bin/xpore-dataprep
$ podman run --it --rm --entrypoint /usr/local/bin/xpore-dataprep   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/xpore-dataprep   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### xpore-diffmod

```bash
$ singularity exec <container> /usr/local/bin/xpore-diffmod
$ podman run --it --rm --entrypoint /usr/local/bin/xpore-diffmod   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/xpore-diffmod   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### mirror_server

```bash
$ singularity exec <container> /usr/local/bin/mirror_server
$ podman run --it --rm --entrypoint /usr/local/bin/mirror_server   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/mirror_server   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### mirror_server_stop

```bash
$ singularity exec <container> /usr/local/bin/mirror_server_stop
$ podman run --it --rm --entrypoint /usr/local/bin/mirror_server_stop   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/mirror_server_stop   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### chardetect

```bash
$ singularity exec <container> /usr/local/bin/chardetect
$ podman run --it --rm --entrypoint /usr/local/bin/chardetect   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/chardetect   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### f2py3.9

```bash
$ singularity exec <container> /usr/local/bin/f2py3.9
$ podman run --it --rm --entrypoint /usr/local/bin/f2py3.9   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/f2py3.9   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### h5clear

```bash
$ singularity exec <container> /usr/local/bin/h5clear
$ podman run --it --rm --entrypoint /usr/local/bin/h5clear   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/h5clear   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### h5format_convert

```bash
$ singularity exec <container> /usr/local/bin/h5format_convert
$ podman run --it --rm --entrypoint /usr/local/bin/h5format_convert   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/h5format_convert   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### h5watch

```bash
$ singularity exec <container> /usr/local/bin/h5watch
$ podman run --it --rm --entrypoint /usr/local/bin/h5watch   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/h5watch   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### h5fc

```bash
$ singularity exec <container> /usr/local/bin/h5fc
$ podman run --it --rm --entrypoint /usr/local/bin/h5fc   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/h5fc   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### gif2h5

```bash
$ singularity exec <container> /usr/local/bin/gif2h5
$ podman run --it --rm --entrypoint /usr/local/bin/gif2h5   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/gif2h5   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### h52gif

```bash
$ singularity exec <container> /usr/local/bin/h52gif
$ podman run --it --rm --entrypoint /usr/local/bin/h52gif   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/h52gif   -v ${PWD} -w ${PWD} <container> -c " $@"
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