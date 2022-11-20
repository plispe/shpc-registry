---
layout: container
name:  "quay.io/biocontainers/bioconductor-cardinal"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-cardinal/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-cardinal/container.yaml"
updated_at: "2022-11-19 23:54:42.885397"
latest: "2.12.0--r41hc247a5b_2"
container_url: "https://biocontainers.pro/tools/bioconductor-cardinal"
aliases:
 - "fftw-wisdom"
 - "fftw-wisdom-to-conf"
 - "fftwf-wisdom"
 - "fftwl-wisdom"
 - "x86_64-conda-linux-gnu-gfortran.bin"
versions:
 - "2.8.0--r40h399db7b_2"
 - "2.12.0--r41hc247a5b_2"
 - "2.10.0--r41h399db7b_0"
description: "shpc-registry automated BioContainers addition for bioconductor-cardinal"
config: {"url": "https://biocontainers.pro/tools/bioconductor-cardinal", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-cardinal", "latest": {"2.12.0--r41hc247a5b_2": "sha256:bc355cf3d07962ccd4246ce8be97374089fc740d498487c4ff635c2db9fc6441"}, "tags": {"2.8.0--r40h399db7b_2": "sha256:49af076e3f9f5c67f9482c909e947758ea730cbcabc6a25ea3054b284f60b396", "2.12.0--r41hc247a5b_2": "sha256:bc355cf3d07962ccd4246ce8be97374089fc740d498487c4ff635c2db9fc6441", "2.10.0--r41h399db7b_0": "sha256:83536b553aba4f728628d62a59f8eaf8b9a5468f21675dcf0c0e05333ab96804"}, "docker": "quay.io/biocontainers/bioconductor-cardinal", "aliases": {"fftw-wisdom": "/usr/local/bin/fftw-wisdom", "fftw-wisdom-to-conf": "/usr/local/bin/fftw-wisdom-to-conf", "fftwf-wisdom": "/usr/local/bin/fftwf-wisdom", "fftwl-wisdom": "/usr/local/bin/fftwl-wisdom", "x86_64-conda-linux-gnu-gfortran.bin": "/usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-cardinal.
shpc-registry automated BioContainers addition for bioconductor-cardinal
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-cardinal
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-cardinal:2.12.0--r41hc247a5b_2
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-cardinal/2.12.0--r41hc247a5b_2
$ module help quay.io/biocontainers/bioconductor-cardinal/2.12.0--r41hc247a5b_2
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-cardinal-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-cardinal-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-cardinal-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-cardinal-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-cardinal-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-cardinal-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### fftw-wisdom

```bash
$ singularity exec <container> /usr/local/bin/fftw-wisdom
$ podman run --it --rm --entrypoint /usr/local/bin/fftw-wisdom   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/fftw-wisdom   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### fftw-wisdom-to-conf

```bash
$ singularity exec <container> /usr/local/bin/fftw-wisdom-to-conf
$ podman run --it --rm --entrypoint /usr/local/bin/fftw-wisdom-to-conf   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/fftw-wisdom-to-conf   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### fftwf-wisdom

```bash
$ singularity exec <container> /usr/local/bin/fftwf-wisdom
$ podman run --it --rm --entrypoint /usr/local/bin/fftwf-wisdom   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/fftwf-wisdom   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### fftwl-wisdom

```bash
$ singularity exec <container> /usr/local/bin/fftwl-wisdom
$ podman run --it --rm --entrypoint /usr/local/bin/fftwl-wisdom   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/fftwl-wisdom   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### x86_64-conda-linux-gnu-gfortran.bin

```bash
$ singularity exec <container> /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin
$ podman run --it --rm --entrypoint /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/x86_64-conda-linux-gnu-gfortran.bin   -v ${PWD} -w ${PWD} <container> -c " $@"
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