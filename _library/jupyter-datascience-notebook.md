---
layout: container
name:  "jupyter/datascience-notebook"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/jupyter/datascience-notebook/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/jupyter/datascience-notebook/container.yaml"
updated_at: "2023-01-13 02:47:15.024297"
latest: "2022-12-15"
container_url: "https://hub.docker.com/r/jupyter/datascience-notebook"
aliases:
 - "run-notebook"
versions:
 - "4.0"
 - "latest"
 - "2022-04-05"
 - "2022-03-28"
 - "2022-02-28"
 - "2022-01-31"
 - "2021-12-27"
 - "2022-04-25"
 - "2022-05-31"
 - "2022-06-27"
 - "2022-08-23"
 - "2022-07-27"
 - "2022-08-29"
 - "2022-09-30"
 - "2022-11-15"
 - "2022-10-31"
 - "2022-12-15"
 - "2022-11-28"
description: "Jupyter Datascience Notebook from https://github.com/jupyter/docker-stacks"
config: {"docker": "jupyter/datascience-notebook", "url": "https://hub.docker.com/r/jupyter/datascience-notebook", "maintainer": "@vsoch", "description": "Jupyter Datascience Notebook from https://github.com/jupyter/docker-stacks", "latest": {"2022-12-15": "sha256:09516082adc8c9be07c7fca05bbec39e3895aeb4fb027ef2160a835d5ac398f6"}, "tags": {"4.0": "sha256:5e5bf78bfa351c0255cea5269a0461afbf6b50b51e923a7436229208ea8487f9", "latest": "sha256:09516082adc8c9be07c7fca05bbec39e3895aeb4fb027ef2160a835d5ac398f6", "2022-04-05": "sha256:f7a82d58c25e0b578ba47e696123be2aa590987a3c2bb1df979b3bfdc728b783", "2022-03-28": "sha256:955a943ea994def00f31bf7e07a44ab966c66b0795c3036e65d550e8e9082413", "2022-02-28": "sha256:e6b6f2a13249c9b571b2bb385b9af2f674977d7247e6f8519c1a012dd98b4813", "2022-01-31": "sha256:23deac05d7cae99e61a46ddc176a8eae4d7a4ff774f8b556fe155bba85660014", "2021-12-27": "sha256:676f4ecbd9f9ff21c774ec44dbac480021e195d73aeb6eb03fa572288f50f5d1", "2022-04-25": "sha256:466e41c228ca890d37d46c590c0641f55b516fe3f5b8dd7c9b36aac0ffa9d514", "2022-05-31": "sha256:227d569a52d91cacea8f10c858f14b1099475b0435b1edba7372cbf898a8b6fb", "2022-06-27": "sha256:2d9e15b4a796c08ecff5c8a80e707790369c20f8caf20d7ce8683f7d07bf078d", "2022-08-23": "sha256:08677b8b71501eceb37cbd12f1fe0d5a80b3fe3e1b8caa2cbdd8bcd37429caaa", "2022-07-27": "sha256:3301e740348a4c26c60e96bb13437d4d1217136d7c68c1758bab2e718b8b7050", "2022-08-29": "sha256:90ffc2819aaf86e5a2c2c6a581c925690abbcfa40c581d8f1045ddb83c7f8130", "2022-09-30": "sha256:e0e94c7fcbc7ba3ad8d6260f82bd7f7a6715a0db050fcf8d49cd97b198186703", "2022-11-15": "sha256:3bfa9baf32a022061341ec779fde58c44a3939481a964acf2b408528aa5ad686", "2022-10-31": "sha256:23584d1939486b01ccf1f6dc70ad3db798a466d187d50322c12b86656a6571fb", "2022-12-15": "sha256:09516082adc8c9be07c7fca05bbec39e3895aeb4fb027ef2160a835d5ac398f6", "2022-11-28": "sha256:d0532c681d48039a45622dce9c4637ae90d5303e7e1ca319c611b096881e87cf"}, "aliases": [{"name": "run-notebook", "command": "jupyter notebook --no-browser --port=$(shuf -i 2000-65000 -n 1) --ip 0.0.0.0"}]}
---

This module is a singularity container wrapper for jupyter/datascience-notebook.
Jupyter Datascience Notebook from https://github.com/jupyter/docker-stacks
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install jupyter/datascience-notebook
```

Or a specific version:

```bash
$ shpc install jupyter/datascience-notebook:2022-12-15
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load jupyter/datascience-notebook/2022-12-15
$ module help jupyter/datascience-notebook/2022-12-15
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### datascience-notebook-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### datascience-notebook-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### datascience-notebook-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### datascience-notebook-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### datascience-notebook-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### datascience-notebook-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### run-notebook

```bash
$ singularity exec <container> jupyter notebook --no-browser --port=$(shuf -i 2000-65000 -n 1) --ip 0.0.0.0
$ podman run --it --rm --entrypoint    -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint    -v ${PWD} -w ${PWD} <container> -c " $@"
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