---
layout: container
name:  "quay.io/biocontainers/recognizer"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/recognizer/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/recognizer/container.yaml"
updated_at: "2023-01-13 03:21:22.588950"
latest: "1.8.3--hdfd78af_0"
container_url: "https://biocontainers.pro/tools/recognizer"
aliases:
 - "ktClassifyHits"
 - "ktImportHits"
 - "recognizer.py"
 - "ktClassifyBLAST"
 - "ktGetContigMagnitudes"
 - "ktGetLCA"
 - "ktGetLibPath"
 - "ktGetTaxIDFromAcc"
 - "ktGetTaxInfo"
 - "ktImportBLAST"
 - "ktImportDiskUsage"
 - "ktImportEC"
 - "ktImportFCP"
versions:
 - "1.8.3--hdfd78af_0"
description: "shpc-registry automated BioContainers addition for recognizer"
config: {"url": "https://biocontainers.pro/tools/recognizer", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for recognizer", "latest": {"1.8.3--hdfd78af_0": "sha256:60847fe452ed6e4f4c30a677c8ecea0b4f788acbcc8ab44514a6355c0b4e5275"}, "tags": {"1.8.3--hdfd78af_0": "sha256:60847fe452ed6e4f4c30a677c8ecea0b4f788acbcc8ab44514a6355c0b4e5275"}, "docker": "quay.io/biocontainers/recognizer", "aliases": {"ktClassifyHits": "/usr/local/bin/ktClassifyHits", "ktImportHits": "/usr/local/bin/ktImportHits", "recognizer.py": "/usr/local/bin/recognizer.py", "ktClassifyBLAST": "/usr/local/bin/ktClassifyBLAST", "ktGetContigMagnitudes": "/usr/local/bin/ktGetContigMagnitudes", "ktGetLCA": "/usr/local/bin/ktGetLCA", "ktGetLibPath": "/usr/local/bin/ktGetLibPath", "ktGetTaxIDFromAcc": "/usr/local/bin/ktGetTaxIDFromAcc", "ktGetTaxInfo": "/usr/local/bin/ktGetTaxInfo", "ktImportBLAST": "/usr/local/bin/ktImportBLAST", "ktImportDiskUsage": "/usr/local/bin/ktImportDiskUsage", "ktImportEC": "/usr/local/bin/ktImportEC", "ktImportFCP": "/usr/local/bin/ktImportFCP"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/recognizer.
shpc-registry automated BioContainers addition for recognizer
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/recognizer
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/recognizer:1.8.3--hdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/recognizer/1.8.3--hdfd78af_0
$ module help quay.io/biocontainers/recognizer/1.8.3--hdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### recognizer-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### recognizer-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### recognizer-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### recognizer-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### recognizer-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### recognizer-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### ktClassifyHits

```bash
$ singularity exec <container> /usr/local/bin/ktClassifyHits
$ podman run --it --rm --entrypoint /usr/local/bin/ktClassifyHits   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/ktClassifyHits   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### ktImportHits

```bash
$ singularity exec <container> /usr/local/bin/ktImportHits
$ podman run --it --rm --entrypoint /usr/local/bin/ktImportHits   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/ktImportHits   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### recognizer.py

```bash
$ singularity exec <container> /usr/local/bin/recognizer.py
$ podman run --it --rm --entrypoint /usr/local/bin/recognizer.py   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/recognizer.py   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### ktClassifyBLAST

```bash
$ singularity exec <container> /usr/local/bin/ktClassifyBLAST
$ podman run --it --rm --entrypoint /usr/local/bin/ktClassifyBLAST   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/ktClassifyBLAST   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### ktGetContigMagnitudes

```bash
$ singularity exec <container> /usr/local/bin/ktGetContigMagnitudes
$ podman run --it --rm --entrypoint /usr/local/bin/ktGetContigMagnitudes   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/ktGetContigMagnitudes   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### ktGetLCA

```bash
$ singularity exec <container> /usr/local/bin/ktGetLCA
$ podman run --it --rm --entrypoint /usr/local/bin/ktGetLCA   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/ktGetLCA   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### ktGetLibPath

```bash
$ singularity exec <container> /usr/local/bin/ktGetLibPath
$ podman run --it --rm --entrypoint /usr/local/bin/ktGetLibPath   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/ktGetLibPath   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### ktGetTaxIDFromAcc

```bash
$ singularity exec <container> /usr/local/bin/ktGetTaxIDFromAcc
$ podman run --it --rm --entrypoint /usr/local/bin/ktGetTaxIDFromAcc   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/ktGetTaxIDFromAcc   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### ktGetTaxInfo

```bash
$ singularity exec <container> /usr/local/bin/ktGetTaxInfo
$ podman run --it --rm --entrypoint /usr/local/bin/ktGetTaxInfo   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/ktGetTaxInfo   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### ktImportBLAST

```bash
$ singularity exec <container> /usr/local/bin/ktImportBLAST
$ podman run --it --rm --entrypoint /usr/local/bin/ktImportBLAST   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/ktImportBLAST   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### ktImportDiskUsage

```bash
$ singularity exec <container> /usr/local/bin/ktImportDiskUsage
$ podman run --it --rm --entrypoint /usr/local/bin/ktImportDiskUsage   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/ktImportDiskUsage   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### ktImportEC

```bash
$ singularity exec <container> /usr/local/bin/ktImportEC
$ podman run --it --rm --entrypoint /usr/local/bin/ktImportEC   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/ktImportEC   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### ktImportFCP

```bash
$ singularity exec <container> /usr/local/bin/ktImportFCP
$ podman run --it --rm --entrypoint /usr/local/bin/ktImportFCP   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/ktImportFCP   -v ${PWD} -w ${PWD} <container> -c " $@"
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