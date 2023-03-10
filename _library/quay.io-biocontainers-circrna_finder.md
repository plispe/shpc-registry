---
layout: container
name:  "quay.io/biocontainers/circrna_finder"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/circrna_finder/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/circrna_finder/container.yaml"
updated_at: "2023-01-13 03:45:45.781699"
latest: "1.2--pl5321hdfd78af_1"
container_url: "https://biocontainers.pro/tools/circrna_finder"
aliases:
 - "filterCirc.awk"
 - "filterSpliceSiteCircles.pl"
 - "nrForwardSplicedReads.pl"
 - "postProcessStarAlignment.pl"
 - "runStar.pl"
 - "starCirclesToBed.pl"
 - "basenc"
 - "b2sum"
 - "base32"
 - "base64"
 - "basename"
 - "cat"
 - "chcon"
 - "chgrp"
 - "chmod"
 - "chown"
 - "chroot"
 - "cksum"
 - "comm"
 - "cp"
 - "csplit"
 - "cut"
 - "date"
 - "dd"
 - "df"
 - "dir"
 - "dircolors"
 - "dirname"
 - "du"
 - "echo"
 - "env"
versions:
 - "1.2--pl5321hdfd78af_0"
 - "1.2--pl5321hdfd78af_1"
description: "singularity registry hpc automated addition for circrna_finder"
config: {"url": "https://biocontainers.pro/tools/circrna_finder", "maintainer": "@vsoch", "description": "singularity registry hpc automated addition for circrna_finder", "latest": {"1.2--pl5321hdfd78af_1": "sha256:1697e581c8005132377fbd9f16cbbe43df7bbb950b01a0ad9ce27699b62b5b4c"}, "tags": {"1.2--pl5321hdfd78af_0": "sha256:caee621721cd157a319d54fa2af54a878f3cab9dc43eed69603cd2b0fb8f44ae", "1.2--pl5321hdfd78af_1": "sha256:1697e581c8005132377fbd9f16cbbe43df7bbb950b01a0ad9ce27699b62b5b4c"}, "docker": "quay.io/biocontainers/circrna_finder", "aliases": {"filterCirc.awk": "/usr/local/bin/filterCirc.awk", "filterSpliceSiteCircles.pl": "/usr/local/bin/filterSpliceSiteCircles.pl", "nrForwardSplicedReads.pl": "/usr/local/bin/nrForwardSplicedReads.pl", "postProcessStarAlignment.pl": "/usr/local/bin/postProcessStarAlignment.pl", "runStar.pl": "/usr/local/bin/runStar.pl", "starCirclesToBed.pl": "/usr/local/bin/starCirclesToBed.pl", "basenc": "/usr/local/bin/basenc", "b2sum": "/usr/local/bin/b2sum", "base32": "/usr/local/bin/base32", "base64": "/usr/local/bin/base64", "basename": "/usr/local/bin/basename", "cat": "/usr/local/bin/cat", "chcon": "/usr/local/bin/chcon", "chgrp": "/usr/local/bin/chgrp", "chmod": "/usr/local/bin/chmod", "chown": "/usr/local/bin/chown", "chroot": "/usr/local/bin/chroot", "cksum": "/usr/local/bin/cksum", "comm": "/usr/local/bin/comm", "cp": "/usr/local/bin/cp", "csplit": "/usr/local/bin/csplit", "cut": "/usr/local/bin/cut", "date": "/usr/local/bin/date", "dd": "/usr/local/bin/dd", "df": "/usr/local/bin/df", "dir": "/usr/local/bin/dir", "dircolors": "/usr/local/bin/dircolors", "dirname": "/usr/local/bin/dirname", "du": "/usr/local/bin/du", "echo": "/usr/local/bin/echo", "env": "/usr/local/bin/env"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/circrna_finder.
singularity registry hpc automated addition for circrna_finder
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/circrna_finder
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/circrna_finder:1.2--pl5321hdfd78af_1
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/circrna_finder/1.2--pl5321hdfd78af_1
$ module help quay.io/biocontainers/circrna_finder/1.2--pl5321hdfd78af_1
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### circrna_finder-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### circrna_finder-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### circrna_finder-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### circrna_finder-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### circrna_finder-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### circrna_finder-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### filterCirc.awk

```bash
$ singularity exec <container> /usr/local/bin/filterCirc.awk
$ podman run --it --rm --entrypoint /usr/local/bin/filterCirc.awk   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/filterCirc.awk   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### filterSpliceSiteCircles.pl

```bash
$ singularity exec <container> /usr/local/bin/filterSpliceSiteCircles.pl
$ podman run --it --rm --entrypoint /usr/local/bin/filterSpliceSiteCircles.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/filterSpliceSiteCircles.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### nrForwardSplicedReads.pl

```bash
$ singularity exec <container> /usr/local/bin/nrForwardSplicedReads.pl
$ podman run --it --rm --entrypoint /usr/local/bin/nrForwardSplicedReads.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/nrForwardSplicedReads.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### postProcessStarAlignment.pl

```bash
$ singularity exec <container> /usr/local/bin/postProcessStarAlignment.pl
$ podman run --it --rm --entrypoint /usr/local/bin/postProcessStarAlignment.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/postProcessStarAlignment.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### runStar.pl

```bash
$ singularity exec <container> /usr/local/bin/runStar.pl
$ podman run --it --rm --entrypoint /usr/local/bin/runStar.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/runStar.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### starCirclesToBed.pl

```bash
$ singularity exec <container> /usr/local/bin/starCirclesToBed.pl
$ podman run --it --rm --entrypoint /usr/local/bin/starCirclesToBed.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/starCirclesToBed.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### basenc

```bash
$ singularity exec <container> /usr/local/bin/basenc
$ podman run --it --rm --entrypoint /usr/local/bin/basenc   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/basenc   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### b2sum

```bash
$ singularity exec <container> /usr/local/bin/b2sum
$ podman run --it --rm --entrypoint /usr/local/bin/b2sum   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/b2sum   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### base32

```bash
$ singularity exec <container> /usr/local/bin/base32
$ podman run --it --rm --entrypoint /usr/local/bin/base32   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/base32   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### base64

```bash
$ singularity exec <container> /usr/local/bin/base64
$ podman run --it --rm --entrypoint /usr/local/bin/base64   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/base64   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### basename

```bash
$ singularity exec <container> /usr/local/bin/basename
$ podman run --it --rm --entrypoint /usr/local/bin/basename   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/basename   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### cat

```bash
$ singularity exec <container> /usr/local/bin/cat
$ podman run --it --rm --entrypoint /usr/local/bin/cat   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/cat   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### chcon

```bash
$ singularity exec <container> /usr/local/bin/chcon
$ podman run --it --rm --entrypoint /usr/local/bin/chcon   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/chcon   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### chgrp

```bash
$ singularity exec <container> /usr/local/bin/chgrp
$ podman run --it --rm --entrypoint /usr/local/bin/chgrp   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/chgrp   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### chmod

```bash
$ singularity exec <container> /usr/local/bin/chmod
$ podman run --it --rm --entrypoint /usr/local/bin/chmod   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/chmod   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### chown

```bash
$ singularity exec <container> /usr/local/bin/chown
$ podman run --it --rm --entrypoint /usr/local/bin/chown   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/chown   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### chroot

```bash
$ singularity exec <container> /usr/local/bin/chroot
$ podman run --it --rm --entrypoint /usr/local/bin/chroot   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/chroot   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### cksum

```bash
$ singularity exec <container> /usr/local/bin/cksum
$ podman run --it --rm --entrypoint /usr/local/bin/cksum   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/cksum   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### comm

```bash
$ singularity exec <container> /usr/local/bin/comm
$ podman run --it --rm --entrypoint /usr/local/bin/comm   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/comm   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### cp

```bash
$ singularity exec <container> /usr/local/bin/cp
$ podman run --it --rm --entrypoint /usr/local/bin/cp   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/cp   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### csplit

```bash
$ singularity exec <container> /usr/local/bin/csplit
$ podman run --it --rm --entrypoint /usr/local/bin/csplit   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/csplit   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### cut

```bash
$ singularity exec <container> /usr/local/bin/cut
$ podman run --it --rm --entrypoint /usr/local/bin/cut   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/cut   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### date

```bash
$ singularity exec <container> /usr/local/bin/date
$ podman run --it --rm --entrypoint /usr/local/bin/date   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/date   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### dd

```bash
$ singularity exec <container> /usr/local/bin/dd
$ podman run --it --rm --entrypoint /usr/local/bin/dd   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/dd   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### df

```bash
$ singularity exec <container> /usr/local/bin/df
$ podman run --it --rm --entrypoint /usr/local/bin/df   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/df   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### dir

```bash
$ singularity exec <container> /usr/local/bin/dir
$ podman run --it --rm --entrypoint /usr/local/bin/dir   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/dir   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### dircolors

```bash
$ singularity exec <container> /usr/local/bin/dircolors
$ podman run --it --rm --entrypoint /usr/local/bin/dircolors   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/dircolors   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### dirname

```bash
$ singularity exec <container> /usr/local/bin/dirname
$ podman run --it --rm --entrypoint /usr/local/bin/dirname   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/dirname   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### du

```bash
$ singularity exec <container> /usr/local/bin/du
$ podman run --it --rm --entrypoint /usr/local/bin/du   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/du   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### echo

```bash
$ singularity exec <container> /usr/local/bin/echo
$ podman run --it --rm --entrypoint /usr/local/bin/echo   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/echo   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### env

```bash
$ singularity exec <container> /usr/local/bin/env
$ podman run --it --rm --entrypoint /usr/local/bin/env   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/env   -v ${PWD} -w ${PWD} <container> -c " $@"
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