---
layout: container
name:  "quay.io/biocontainers/perl-www-mechanize"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/perl-www-mechanize/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/perl-www-mechanize/container.yaml"
updated_at: "2023-01-13 03:34:36.229582"
latest: "1.91--pl526_1"
container_url: "https://biocontainers.pro/tools/perl-www-mechanize"
aliases:
 - "mech-dump"
 - "config_data"
 - "htmltree"
 - "lwp-download"
 - "lwp-dump"
 - "lwp-mirror"
 - "lwp-request"
 - "cpanm"
 - "perl5.26.2"
 - "podselect"
versions:
 - "1.91--pl526_1"
description: "shpc-registry automated BioContainers addition for perl-www-mechanize"
config: {"url": "https://biocontainers.pro/tools/perl-www-mechanize", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for perl-www-mechanize", "latest": {"1.91--pl526_1": "sha256:f5def9e813648e86260f4731c9f7976a0cfa63cb457e189bf9b5bd179bf86b12"}, "tags": {"1.91--pl526_1": "sha256:f5def9e813648e86260f4731c9f7976a0cfa63cb457e189bf9b5bd179bf86b12"}, "docker": "quay.io/biocontainers/perl-www-mechanize", "aliases": {"mech-dump": "/usr/local/bin/mech-dump", "config_data": "/usr/local/bin/config_data", "htmltree": "/usr/local/bin/htmltree", "lwp-download": "/usr/local/bin/lwp-download", "lwp-dump": "/usr/local/bin/lwp-dump", "lwp-mirror": "/usr/local/bin/lwp-mirror", "lwp-request": "/usr/local/bin/lwp-request", "cpanm": "/usr/local/bin/cpanm", "perl5.26.2": "/usr/local/bin/perl5.26.2", "podselect": "/usr/local/bin/podselect"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/perl-www-mechanize.
shpc-registry automated BioContainers addition for perl-www-mechanize
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/perl-www-mechanize
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/perl-www-mechanize:1.91--pl526_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/perl-www-mechanize/1.91--pl526_1
$ module help quay.io/biocontainers/perl-www-mechanize/1.91--pl526_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### perl-www-mechanize-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### perl-www-mechanize-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### perl-www-mechanize-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### perl-www-mechanize-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### perl-www-mechanize-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### perl-www-mechanize-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### mech-dump

```bash
$ singularity exec <container> /usr/local/bin/mech-dump
$ podman run --it --rm --entrypoint /usr/local/bin/mech-dump   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/mech-dump   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### config_data

```bash
$ singularity exec <container> /usr/local/bin/config_data
$ podman run --it --rm --entrypoint /usr/local/bin/config_data   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/config_data   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### htmltree

```bash
$ singularity exec <container> /usr/local/bin/htmltree
$ podman run --it --rm --entrypoint /usr/local/bin/htmltree   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/htmltree   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### lwp-download

```bash
$ singularity exec <container> /usr/local/bin/lwp-download
$ podman run --it --rm --entrypoint /usr/local/bin/lwp-download   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/lwp-download   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### lwp-dump

```bash
$ singularity exec <container> /usr/local/bin/lwp-dump
$ podman run --it --rm --entrypoint /usr/local/bin/lwp-dump   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/lwp-dump   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### lwp-mirror

```bash
$ singularity exec <container> /usr/local/bin/lwp-mirror
$ podman run --it --rm --entrypoint /usr/local/bin/lwp-mirror   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/lwp-mirror   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### lwp-request

```bash
$ singularity exec <container> /usr/local/bin/lwp-request
$ podman run --it --rm --entrypoint /usr/local/bin/lwp-request   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/lwp-request   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### cpanm

```bash
$ singularity exec <container> /usr/local/bin/cpanm
$ podman run --it --rm --entrypoint /usr/local/bin/cpanm   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/cpanm   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### perl5.26.2

```bash
$ singularity exec <container> /usr/local/bin/perl5.26.2
$ podman run --it --rm --entrypoint /usr/local/bin/perl5.26.2   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/perl5.26.2   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### podselect

```bash
$ singularity exec <container> /usr/local/bin/podselect
$ podman run --it --rm --entrypoint /usr/local/bin/podselect   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/podselect   -v ${PWD} -w ${PWD} <container> -c " $@"
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