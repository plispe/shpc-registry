---
layout: container
name:  "bids/pymvpa"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/bids/pymvpa/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/bids/pymvpa/container.yaml"
updated_at: "2023-01-13 02:47:05.244719"
latest: "v4.0.1"
container_url: "https://hub.docker.com/r/bids/pymvpa"

versions:
 - "latest"
 - "v2.0.2"
 - "v4.0.1"
 - "unstable"
description: "Take fMRI data and generates ROI based MultiVariate Pattern Analysis (MVPA) outputs (https://github.com/BIDS-Apps/PyMVPA)"
config: {"docker": "bids/pymvpa", "url": "https://hub.docker.com/r/bids/pymvpa", "maintainer": "@vsoch", "description": "Take fMRI data and generates ROI based MultiVariate Pattern Analysis (MVPA) outputs (https://github.com/BIDS-Apps/PyMVPA)", "latest": {"v4.0.1": "sha256:e29fbce4e72f4dc53fcada1ddeb2e7bfc8ef7f696b5b6ac8492c9d0689ce8e5d"}, "tags": {"latest": "sha256:6d6487b2c548d336a4758aa371ce2adb630255c46f59aeac550a2fc94dc24e9c", "v2.0.2": "sha256:6d6487b2c548d336a4758aa371ce2adb630255c46f59aeac550a2fc94dc24e9c", "v4.0.1": "sha256:e29fbce4e72f4dc53fcada1ddeb2e7bfc8ef7f696b5b6ac8492c9d0689ce8e5d", "unstable": "sha256:6d6487b2c548d336a4758aa371ce2adb630255c46f59aeac550a2fc94dc24e9c"}, "filter": ["v*"]}
---

This module is a singularity container wrapper for bids/pymvpa.
Take fMRI data and generates ROI based MultiVariate Pattern Analysis (MVPA) outputs (https://github.com/BIDS-Apps/PyMVPA)
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install bids/pymvpa
```

Or a specific version:

```bash
$ shpc install bids/pymvpa:v4.0.1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load bids/pymvpa/v4.0.1
$ module help bids/pymvpa/v4.0.1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### pymvpa-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### pymvpa-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### pymvpa-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### pymvpa-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### pymvpa-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### pymvpa-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### pymvpa

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