---
layout: container
name:  "quay.io/biocontainers/proteowizard"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/proteowizard/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/proteowizard/container.yaml"
updated_at: "2023-01-13 03:00:23.245560"
latest: "3_0_9992--h2d50403_2"
container_url: "https://biocontainers.pro/tools/proteowizard"
aliases:
 - "chainsaw"
 - "idcat"
 - "idconvert"
 - "msaccess"
 - "msbenchmark"
 - "mscat"
 - "msconvert"
 - "msdiff"
 - "msdir"
 - "msistats"
 - "mspicture"
 - "peakaboo"
 - "pepcat"
 - "pepsum"
 - "qtofpeakpicker"
 - "sldout"
 - "txt2mzml"
versions:
 - "3_0_9992--h2d50403_2"
description: "shpc-registry automated BioContainers addition for proteowizard"
config: {"url": "https://biocontainers.pro/tools/proteowizard", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for proteowizard", "latest": {"3_0_9992--h2d50403_2": "sha256:3b1753654e2d825d6ee34192cdf0d08b886565fb7ed1fd01c4f4c713968c304f"}, "tags": {"3_0_9992--h2d50403_2": "sha256:3b1753654e2d825d6ee34192cdf0d08b886565fb7ed1fd01c4f4c713968c304f"}, "docker": "quay.io/biocontainers/proteowizard", "aliases": {"chainsaw": "/usr/local/bin/chainsaw", "idcat": "/usr/local/bin/idcat", "idconvert": "/usr/local/bin/idconvert", "msaccess": "/usr/local/bin/msaccess", "msbenchmark": "/usr/local/bin/msbenchmark", "mscat": "/usr/local/bin/mscat", "msconvert": "/usr/local/bin/msconvert", "msdiff": "/usr/local/bin/msdiff", "msdir": "/usr/local/bin/msdir", "msistats": "/usr/local/bin/msistats", "mspicture": "/usr/local/bin/mspicture", "peakaboo": "/usr/local/bin/peakaboo", "pepcat": "/usr/local/bin/pepcat", "pepsum": "/usr/local/bin/pepsum", "qtofpeakpicker": "/usr/local/bin/qtofpeakpicker", "sldout": "/usr/local/bin/sldout", "txt2mzml": "/usr/local/bin/txt2mzml"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/proteowizard.
shpc-registry automated BioContainers addition for proteowizard
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/proteowizard
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/proteowizard:3_0_9992--h2d50403_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/proteowizard/3_0_9992--h2d50403_2
$ module help quay.io/biocontainers/proteowizard/3_0_9992--h2d50403_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### proteowizard-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### proteowizard-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### proteowizard-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### proteowizard-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### proteowizard-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### proteowizard-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### chainsaw

```bash
$ singularity exec <container> /usr/local/bin/chainsaw
$ podman run --it --rm --entrypoint /usr/local/bin/chainsaw   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/chainsaw   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### idcat

```bash
$ singularity exec <container> /usr/local/bin/idcat
$ podman run --it --rm --entrypoint /usr/local/bin/idcat   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/idcat   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### idconvert

```bash
$ singularity exec <container> /usr/local/bin/idconvert
$ podman run --it --rm --entrypoint /usr/local/bin/idconvert   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/idconvert   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### msaccess

```bash
$ singularity exec <container> /usr/local/bin/msaccess
$ podman run --it --rm --entrypoint /usr/local/bin/msaccess   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/msaccess   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### msbenchmark

```bash
$ singularity exec <container> /usr/local/bin/msbenchmark
$ podman run --it --rm --entrypoint /usr/local/bin/msbenchmark   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/msbenchmark   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### mscat

```bash
$ singularity exec <container> /usr/local/bin/mscat
$ podman run --it --rm --entrypoint /usr/local/bin/mscat   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/mscat   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### msconvert

```bash
$ singularity exec <container> /usr/local/bin/msconvert
$ podman run --it --rm --entrypoint /usr/local/bin/msconvert   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/msconvert   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### msdiff

```bash
$ singularity exec <container> /usr/local/bin/msdiff
$ podman run --it --rm --entrypoint /usr/local/bin/msdiff   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/msdiff   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### msdir

```bash
$ singularity exec <container> /usr/local/bin/msdir
$ podman run --it --rm --entrypoint /usr/local/bin/msdir   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/msdir   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### msistats

```bash
$ singularity exec <container> /usr/local/bin/msistats
$ podman run --it --rm --entrypoint /usr/local/bin/msistats   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/msistats   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### mspicture

```bash
$ singularity exec <container> /usr/local/bin/mspicture
$ podman run --it --rm --entrypoint /usr/local/bin/mspicture   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/mspicture   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### peakaboo

```bash
$ singularity exec <container> /usr/local/bin/peakaboo
$ podman run --it --rm --entrypoint /usr/local/bin/peakaboo   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/peakaboo   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pepcat

```bash
$ singularity exec <container> /usr/local/bin/pepcat
$ podman run --it --rm --entrypoint /usr/local/bin/pepcat   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pepcat   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### pepsum

```bash
$ singularity exec <container> /usr/local/bin/pepsum
$ podman run --it --rm --entrypoint /usr/local/bin/pepsum   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/pepsum   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### qtofpeakpicker

```bash
$ singularity exec <container> /usr/local/bin/qtofpeakpicker
$ podman run --it --rm --entrypoint /usr/local/bin/qtofpeakpicker   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/qtofpeakpicker   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### sldout

```bash
$ singularity exec <container> /usr/local/bin/sldout
$ podman run --it --rm --entrypoint /usr/local/bin/sldout   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/sldout   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### txt2mzml

```bash
$ singularity exec <container> /usr/local/bin/txt2mzml
$ podman run --it --rm --entrypoint /usr/local/bin/txt2mzml   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/txt2mzml   -v ${PWD} -w ${PWD} <container> -c " $@"
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