---
layout: container
name:  "quay.io/biocontainers/sga"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/sga/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/sga/container.yaml"
updated_at: "2023-01-13 03:30:39.064258"
latest: "0.10.15--h4dc6686_7"
container_url: "https://biocontainers.pro/tools/sga"
aliases:
 - "sga"
 - "sga-astat.py"
 - "sga-bam2de.pl"
 - "sga-mergeDriver.pl"
 - "bamtools"
versions:
 - "0.10.15--h4dc6686_7"
description: "shpc-registry automated BioContainers addition for sga"
config: {"url": "https://biocontainers.pro/tools/sga", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for sga", "latest": {"0.10.15--h4dc6686_7": "sha256:f490091d6ff477a3e47caa623526f3877a9e9ccf23a062e642ffaf9c2d502b35"}, "tags": {"0.10.15--h4dc6686_7": "sha256:f490091d6ff477a3e47caa623526f3877a9e9ccf23a062e642ffaf9c2d502b35"}, "docker": "quay.io/biocontainers/sga", "aliases": {"sga": "/usr/local/bin/sga", "sga-astat.py": "/usr/local/bin/sga-astat.py", "sga-bam2de.pl": "/usr/local/bin/sga-bam2de.pl", "sga-mergeDriver.pl": "/usr/local/bin/sga-mergeDriver.pl", "bamtools": "/usr/local/bin/bamtools"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/sga.
shpc-registry automated BioContainers addition for sga
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/sga
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/sga:0.10.15--h4dc6686_7
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/sga/0.10.15--h4dc6686_7
$ module help quay.io/biocontainers/sga/0.10.15--h4dc6686_7
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### sga-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### sga-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### sga-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### sga-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### sga-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### sga-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### sga

```bash
$ singularity exec <container> /usr/local/bin/sga
$ podman run --it --rm --entrypoint /usr/local/bin/sga   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/sga   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### sga-astat.py

```bash
$ singularity exec <container> /usr/local/bin/sga-astat.py
$ podman run --it --rm --entrypoint /usr/local/bin/sga-astat.py   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/sga-astat.py   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### sga-bam2de.pl

```bash
$ singularity exec <container> /usr/local/bin/sga-bam2de.pl
$ podman run --it --rm --entrypoint /usr/local/bin/sga-bam2de.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/sga-bam2de.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### sga-mergeDriver.pl

```bash
$ singularity exec <container> /usr/local/bin/sga-mergeDriver.pl
$ podman run --it --rm --entrypoint /usr/local/bin/sga-mergeDriver.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/sga-mergeDriver.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### bamtools

```bash
$ singularity exec <container> /usr/local/bin/bamtools
$ podman run --it --rm --entrypoint /usr/local/bin/bamtools   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/bamtools   -v ${PWD} -w ${PWD} <container> -c " $@"
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