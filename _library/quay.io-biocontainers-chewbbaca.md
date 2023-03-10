---
layout: container
name:  "quay.io/biocontainers/chewbbaca"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/chewbbaca/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/chewbbaca/container.yaml"
updated_at: "2023-01-13 03:33:34.375345"
latest: "3.0.0--pyhdfd78af_0"
container_url: "https://biocontainers.pro/tools/chewbbaca"
aliases:
 - "chewBBACA.py"
 - "chewie"
 - "clustalw"
 - "CA.pm"
 - "cacert.pem"
 - "clustalw2"
 - "index-themes"
 - "mafft-sparsecore.rb"
 - "einsi"
 - "fftns"
 - "fftnsi"
 - "ginsi"
versions:
 - "2.8.5--pyhdfd78af_0"
 - "3.0.0--pyhdfd78af_0"
 - "2.8.5--pyhdfd78af_1"
description: "shpc-registry automated BioContainers addition for chewbbaca"
config: {"url": "https://biocontainers.pro/tools/chewbbaca", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for chewbbaca", "latest": {"3.0.0--pyhdfd78af_0": "sha256:293aba861b02baa4bfef96577bc3e10a71381acdefc4117d3f6682ef71304aab"}, "tags": {"2.8.5--pyhdfd78af_0": "sha256:3c32318871e17ad1e6b4b0d38085fb6ca25e250ced5721798705944d8fc3c9a0", "3.0.0--pyhdfd78af_0": "sha256:293aba861b02baa4bfef96577bc3e10a71381acdefc4117d3f6682ef71304aab", "2.8.5--pyhdfd78af_1": "sha256:4cd89b7427fcfeb607852783168b8cffbc22578b935dc06dc3e52d0193ecff15"}, "docker": "quay.io/biocontainers/chewbbaca", "aliases": {"chewBBACA.py": "/usr/local/bin/chewBBACA.py", "chewie": "/usr/local/bin/chewie", "clustalw": "/usr/local/bin/clustalw", "CA.pm": "/usr/local/bin/CA.pm", "cacert.pem": "/usr/local/bin/cacert.pem", "clustalw2": "/usr/local/bin/clustalw2", "index-themes": "/usr/local/bin/index-themes", "mafft-sparsecore.rb": "/usr/local/bin/mafft-sparsecore.rb", "einsi": "/usr/local/bin/einsi", "fftns": "/usr/local/bin/fftns", "fftnsi": "/usr/local/bin/fftnsi", "ginsi": "/usr/local/bin/ginsi"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/chewbbaca.
shpc-registry automated BioContainers addition for chewbbaca
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/chewbbaca
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/chewbbaca:3.0.0--pyhdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/chewbbaca/3.0.0--pyhdfd78af_0
$ module help quay.io/biocontainers/chewbbaca/3.0.0--pyhdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### chewbbaca-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### chewbbaca-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### chewbbaca-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### chewbbaca-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### chewbbaca-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### chewbbaca-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### chewBBACA.py

```bash
$ singularity exec <container> /usr/local/bin/chewBBACA.py
$ podman run --it --rm --entrypoint /usr/local/bin/chewBBACA.py   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/chewBBACA.py   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### chewie

```bash
$ singularity exec <container> /usr/local/bin/chewie
$ podman run --it --rm --entrypoint /usr/local/bin/chewie   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/chewie   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### clustalw

```bash
$ singularity exec <container> /usr/local/bin/clustalw
$ podman run --it --rm --entrypoint /usr/local/bin/clustalw   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/clustalw   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### CA.pm

```bash
$ singularity exec <container> /usr/local/bin/CA.pm
$ podman run --it --rm --entrypoint /usr/local/bin/CA.pm   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/CA.pm   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### cacert.pem

```bash
$ singularity exec <container> /usr/local/bin/cacert.pem
$ podman run --it --rm --entrypoint /usr/local/bin/cacert.pem   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/cacert.pem   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### clustalw2

```bash
$ singularity exec <container> /usr/local/bin/clustalw2
$ podman run --it --rm --entrypoint /usr/local/bin/clustalw2   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/clustalw2   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### index-themes

```bash
$ singularity exec <container> /usr/local/bin/index-themes
$ podman run --it --rm --entrypoint /usr/local/bin/index-themes   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/index-themes   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### mafft-sparsecore.rb

```bash
$ singularity exec <container> /usr/local/bin/mafft-sparsecore.rb
$ podman run --it --rm --entrypoint /usr/local/bin/mafft-sparsecore.rb   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/mafft-sparsecore.rb   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### einsi

```bash
$ singularity exec <container> /usr/local/bin/einsi
$ podman run --it --rm --entrypoint /usr/local/bin/einsi   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/einsi   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### fftns

```bash
$ singularity exec <container> /usr/local/bin/fftns
$ podman run --it --rm --entrypoint /usr/local/bin/fftns   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/fftns   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### fftnsi

```bash
$ singularity exec <container> /usr/local/bin/fftnsi
$ podman run --it --rm --entrypoint /usr/local/bin/fftnsi   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/fftnsi   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### ginsi

```bash
$ singularity exec <container> /usr/local/bin/ginsi
$ podman run --it --rm --entrypoint /usr/local/bin/ginsi   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/ginsi   -v ${PWD} -w ${PWD} <container> -c " $@"
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