---
layout: container
name:  "golang"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/golang/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/golang/container.yaml"
updated_at: "2023-01-13 03:47:34.658458"
latest: "1.20-rc"
container_url: "https://hub.docker.com/r/_/golang"
aliases:
 - "go"
 - "gofmt"
versions:
 - "1.16.4-alpine"
 - "1.16.5-alpine"
 - "1.17-rc-alpine"
 - "1.17.0"
 - "1.17.2"
 - "1.17.3"
 - "1.18-rc"
 - "latest"
 - "1"
 - "1.18"
 - "1.17rc2"
 - "1.17rc2-buster"
 - "1.19-rc"
 - "1.18-rc-buster"
 - "1.19"
 - "1.17"
 - "1.16"
 - "1.20-rc"
description: "Go (a.k.a., Golang) is a programming language first developed at Google."
config: {"docker": "golang", "url": "https://hub.docker.com/r/_/golang", "maintainer": "@vsoch", "description": "Go (a.k.a., Golang) is a programming language first developed at Google.", "latest": {"1.20-rc": "sha256:40fa0b89ee20f82fecc020244f7d005988f6327d527cf5671b4dd93739de9712"}, "filter": ["^(?!nano).*$", "^(?!windows).*$"], "tags": {"1.16.4-alpine": "sha256:0dc62c5cc2d97657c17ff3bc0224214e10226e245c94317e352ee8a2c54368b4", "1.16.5-alpine": "sha256:45f32e963bb3cc408cfcd01a8e76b2872fb238f602ec5481cd75393da29369c0", "1.17-rc-alpine": "sha256:787111a3069abdb2c4d8c0b27dff2a29cef8b147f8e7a431f5a464ea84ebfa41", "1.17.0": "sha256:7dbfeb9d51c049e8bfe36cf1a4217c7b1ba304bf0eb72d57d0c04f405589f122", "1.17.2": "sha256:124966f5d54a41317ee81ccfe5f849d4f0deef4ed3c5c32c20be855c51c15027", "1.17.3": "sha256:199102125d11c943c927a8a33911ef960ca72c4879e307c7c2e40ceaa72201e3", "1.18-rc": "sha256:2da497bcc0c9ff09d4185907068c6f137d14e8848059971072f2e9cc936aae70", "latest": "sha256:660f138b4477001d65324a51fa158c1b868651b44e43f0953bf062e9f38b72f3", "1": "sha256:660f138b4477001d65324a51fa158c1b868651b44e43f0953bf062e9f38b72f3", "1.18": "sha256:00d63686b480f6dc866e93ddc4b29efa2db03274a687e6495c2cfbfe615d638e", "1.17rc2": "sha256:c5b50f8381dcc9223b63dbb3e9f558eea0650310232bbc2dde8c3b861c60d1b2", "1.17rc2-buster": "sha256:824267ad82d38a31225b61038ac8735b791396d7df2a6c58f761756964ab4d2d", "1.19-rc": "sha256:c0feb14adb4e346527d86f09bdbcdbe33d1dac5876fbc12c567cd90808e6af4c", "1.18-rc-buster": "sha256:9acf37d060418071d7dbad182979fedc8289eaff0105806a0de2d1a389716fa6", "1.19": "sha256:660f138b4477001d65324a51fa158c1b868651b44e43f0953bf062e9f38b72f3", "1.17": "sha256:87262e4a4c7db56158a80a18fefdc4fee5accc41b59cde821e691d05541bbb18", "1.16": "sha256:5f6a4662de3efc6d6bb812d02e9de3d8698eea16b8eb7281f03e6f3e8383018e", "1.20-rc": "sha256:40fa0b89ee20f82fecc020244f7d005988f6327d527cf5671b4dd93739de9712"}, "aliases": {"go": "/usr/local/go/bin/go", "gofmt": "/usr/local/go/bin/gofmt"}}
---

This module is a singularity container wrapper for golang.
Go (a.k.a., Golang) is a programming language first developed at Google.
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install golang
```

Or a specific version:

```bash
$ shpc install golang:1.20-rc
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load golang/1.20-rc
$ module help golang/1.20-rc
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### golang-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### golang-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### golang-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### golang-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### golang-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### golang-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### go

```bash
$ singularity exec <container> /usr/local/go/bin/go
$ podman run --it --rm --entrypoint /usr/local/go/bin/go   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/go/bin/go   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### gofmt

```bash
$ singularity exec <container> /usr/local/go/bin/gofmt
$ podman run --it --rm --entrypoint /usr/local/go/bin/gofmt   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/go/bin/gofmt   -v ${PWD} -w ${PWD} <container> -c " $@"
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