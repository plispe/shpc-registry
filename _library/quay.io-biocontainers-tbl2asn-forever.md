---
layout: container
name:  "quay.io/biocontainers/tbl2asn-forever"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/tbl2asn-forever/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/tbl2asn-forever/container.yaml"
updated_at: "2023-01-13 02:59:44.974368"
latest: "25.7.2f--hec16e2b_2"
container_url: "https://biocontainers.pro/tools/tbl2asn-forever"
aliases:
 - "faketime"
 - "real-tbl2asn"
 - "tbl2asn"
 - "idn"
versions:
 - "25.7f--0"
 - "25.7.2f--hec16e2b_2"
description: "shpc-registry automated BioContainers addition for tbl2asn-forever"
config: {"url": "https://biocontainers.pro/tools/tbl2asn-forever", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for tbl2asn-forever", "latest": {"25.7.2f--hec16e2b_2": "sha256:642a72422bcc442c22ddf9fb9ca9822eb890809742bd35f1e8a24f1078b0a426"}, "tags": {"25.7f--0": "sha256:e63cde4eb1597dee1a01c414b625d269eb2c5c172cf20102264d1c0e6e057b33", "25.7.2f--hec16e2b_2": "sha256:642a72422bcc442c22ddf9fb9ca9822eb890809742bd35f1e8a24f1078b0a426"}, "docker": "quay.io/biocontainers/tbl2asn-forever", "aliases": {"faketime": "/usr/local/bin/faketime", "real-tbl2asn": "/usr/local/bin/real-tbl2asn", "tbl2asn": "/usr/local/bin/tbl2asn", "idn": "/usr/local/bin/idn"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/tbl2asn-forever.
shpc-registry automated BioContainers addition for tbl2asn-forever
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/tbl2asn-forever
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/tbl2asn-forever:25.7.2f--hec16e2b_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/tbl2asn-forever/25.7.2f--hec16e2b_2
$ module help quay.io/biocontainers/tbl2asn-forever/25.7.2f--hec16e2b_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### tbl2asn-forever-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### tbl2asn-forever-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### tbl2asn-forever-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### tbl2asn-forever-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### tbl2asn-forever-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### tbl2asn-forever-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### faketime

```bash
$ singularity exec <container> /usr/local/bin/faketime
$ podman run --it --rm --entrypoint /usr/local/bin/faketime   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/faketime   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### real-tbl2asn

```bash
$ singularity exec <container> /usr/local/bin/real-tbl2asn
$ podman run --it --rm --entrypoint /usr/local/bin/real-tbl2asn   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/real-tbl2asn   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### tbl2asn

```bash
$ singularity exec <container> /usr/local/bin/tbl2asn
$ podman run --it --rm --entrypoint /usr/local/bin/tbl2asn   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/tbl2asn   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### idn

```bash
$ singularity exec <container> /usr/local/bin/idn
$ podman run --it --rm --entrypoint /usr/local/bin/idn   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/idn   -v ${PWD} -w ${PWD} <container> -c " $@"
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