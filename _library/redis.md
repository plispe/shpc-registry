---
layout: container
name:  "redis"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/redis/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/redis/container.yaml"
updated_at: "2023-01-13 03:46:14.575796"
latest: "7-alpine3.17"
container_url: "https://hub.docker.com/r/_/redis"
aliases:
 - "redis-benchmark"
 - "redis-check-aof"
 - "redis-check-rdb"
 - "redis-cli"
 - "redis-sentinel"
 - "redis-server"
versions:
 - "6.2.3-alpine"
 - "6.2.4-alpine"
 - "6.2.5"
 - "6.2.6"
 - "7.0-rc"
 - "latest"
 - "6"
 - "6-alpine3.15"
 - "6.2"
 - "7"
 - "7-alpine3.15"
 - "7.0"
 - "7-alpine3.16"
 - "6-alpine3.16"
 - "7-alpine3.17"
 - "6-alpine3.17"
description: "Redis is an open-source, networked, in-memory, key-value data store with optional durability."
config: {"docker": "redis", "url": "https://hub.docker.com/r/_/redis", "maintainer": "@vsoch", "description": "Redis is an open-source, networked, in-memory, key-value data store with optional durability.", "filter": ["^(?!.*32bit).*$"], "latest": {"7-alpine3.17": "sha256:9dc2499d6c21f869a6e22b170003483d3fca8c03992f4a11f6493c0b392da40f"}, "tags": {"6.2.3-alpine": "sha256:f8f0e809a4281714c33edf86f6da6cc2d4058c8549e44d8c83303c28b3123072", "6.2.4-alpine": "sha256:0039796b887fd30e460353f14e46ba1004152aa97f5f59094cc21eac445fc89b", "6.2.5": "sha256:c98f0230b5f1831f4f5dd764c4ea8ef11d3e3a1a3593278eb952373d97c82b27", "6.2.6": "sha256:b7fd1a2c89d09a836f659d72c52d27b9f71202c97014a47639f87c992e8c0f1b", "7.0-rc": "sha256:359475c7f0c0a8a28444ca36799b087bb98c8f9db0ee9fa5c13017b4d1693fb5", "latest": "sha256:8184cfe57f205ab34c62bd0e9552dffeb885d2a7f82ce4295c0df344cb6f0007", "6": "sha256:8cf5e722ac88a9fbc03aa9f3e66767d88f809596746a2d35b3e73b7cdfbf0870", "6-alpine3.15": "sha256:4091b9da835824257744fba095932e470078eb2c0025899ac1c6944b2d638c7e", "6.2": "sha256:8cf5e722ac88a9fbc03aa9f3e66767d88f809596746a2d35b3e73b7cdfbf0870", "7": "sha256:8184cfe57f205ab34c62bd0e9552dffeb885d2a7f82ce4295c0df344cb6f0007", "7-alpine3.15": "sha256:541e6d75df5dfb08e8859929bab06da265673808a6f2285abe6b7c76c1c98c6e", "7.0": "sha256:8184cfe57f205ab34c62bd0e9552dffeb885d2a7f82ce4295c0df344cb6f0007", "7-alpine3.16": "sha256:2700d5097763fda285c463f4eefc3d0730a2df2a9d48e66707b19d5a5e5f23d4", "6-alpine3.16": "sha256:aeaf1a7251c9cdaead1bef13d68aac16b0e22326ecfefdb6079008ffab81065d", "7-alpine3.17": "sha256:9dc2499d6c21f869a6e22b170003483d3fca8c03992f4a11f6493c0b392da40f", "6-alpine3.17": "sha256:3f0f123a9204babd071a5f651c28a6ee5c07eb641d7f3e6f869bf5ab3ee9871e"}, "aliases": {"redis-benchmark": "/usr/local/bin/redis-benchmark", "redis-check-aof": "/usr/local/bin/redis-check-aof", "redis-check-rdb": "/usr/local/bin/redis-check-rdb", "redis-cli": "/usr/local/bin/redis-cli", "redis-sentinel": "/usr/local/bin/redis-sentinel", "redis-server": "/usr/local/bin/redis-server"}}
---

This module is a singularity container wrapper for redis.
Redis is an open-source, networked, in-memory, key-value data store with optional durability.
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install redis
```

Or a specific version:

```bash
$ shpc install redis:7-alpine3.17
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load redis/7-alpine3.17
$ module help redis/7-alpine3.17
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### redis-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### redis-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### redis-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### redis-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### redis-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### redis-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### redis-benchmark

```bash
$ singularity exec <container> /usr/local/bin/redis-benchmark
$ podman run --it --rm --entrypoint /usr/local/bin/redis-benchmark   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/redis-benchmark   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### redis-check-aof

```bash
$ singularity exec <container> /usr/local/bin/redis-check-aof
$ podman run --it --rm --entrypoint /usr/local/bin/redis-check-aof   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/redis-check-aof   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### redis-check-rdb

```bash
$ singularity exec <container> /usr/local/bin/redis-check-rdb
$ podman run --it --rm --entrypoint /usr/local/bin/redis-check-rdb   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/redis-check-rdb   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### redis-cli

```bash
$ singularity exec <container> /usr/local/bin/redis-cli
$ podman run --it --rm --entrypoint /usr/local/bin/redis-cli   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/redis-cli   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### redis-sentinel

```bash
$ singularity exec <container> /usr/local/bin/redis-sentinel
$ podman run --it --rm --entrypoint /usr/local/bin/redis-sentinel   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/redis-sentinel   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### redis-server

```bash
$ singularity exec <container> /usr/local/bin/redis-server
$ podman run --it --rm --entrypoint /usr/local/bin/redis-server   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/redis-server   -v ${PWD} -w ${PWD} <container> -c " $@"
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