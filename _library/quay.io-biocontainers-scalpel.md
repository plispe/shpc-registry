---
layout: container
name:  "quay.io/biocontainers/scalpel"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/scalpel/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/quay.io/biocontainers/scalpel/container.yaml"
updated_at: "2023-01-13 02:52:26.405464"
latest: "0.5.4--h9a52abd_4"
container_url: "https://biocontainers.pro/tools/scalpel"
aliases:
 - "scalpel-discovery"
 - "scalpel-export"
 - "gff2gff.py"
 - "bamtools"
 - "guess-ploidy.py"
 - "plot-roh.py"
 - "run-roh.pl"
 - "color-chrs.pl"
 - "plot-vcfstats"
 - "bcftools"
 - "vcfutils.pl"
 - "fasta-sanitize.pl"
versions:
 - "0.5.4--h9a52abd_4"
description: "shpc-registry automated BioContainers addition for scalpel"
config: {"url": "https://biocontainers.pro/tools/scalpel", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for scalpel", "latest": {"0.5.4--h9a52abd_4": "sha256:18fc7f5410282728c88da09f23406b5ae0d1e883439b579f55bd0e221e5c6052"}, "tags": {"0.5.4--h9a52abd_4": "sha256:18fc7f5410282728c88da09f23406b5ae0d1e883439b579f55bd0e221e5c6052"}, "docker": "quay.io/biocontainers/scalpel", "aliases": {"scalpel-discovery": "/usr/local/bin/scalpel-discovery", "scalpel-export": "/usr/local/bin/scalpel-export", "gff2gff.py": "/usr/local/bin/gff2gff.py", "bamtools": "/usr/local/bin/bamtools", "guess-ploidy.py": "/usr/local/bin/guess-ploidy.py", "plot-roh.py": "/usr/local/bin/plot-roh.py", "run-roh.pl": "/usr/local/bin/run-roh.pl", "color-chrs.pl": "/usr/local/bin/color-chrs.pl", "plot-vcfstats": "/usr/local/bin/plot-vcfstats", "bcftools": "/usr/local/bin/bcftools", "vcfutils.pl": "/usr/local/bin/vcfutils.pl", "fasta-sanitize.pl": "/usr/local/bin/fasta-sanitize.pl"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/scalpel.
shpc-registry automated BioContainers addition for scalpel
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/scalpel
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/scalpel:0.5.4--h9a52abd_4
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/scalpel/0.5.4--h9a52abd_4
$ module help quay.io/biocontainers/scalpel/0.5.4--h9a52abd_4
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### scalpel-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### scalpel-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### scalpel-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### scalpel-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### scalpel-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### scalpel-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### scalpel-discovery

```bash
$ singularity exec <container> /usr/local/bin/scalpel-discovery
$ podman run --it --rm --entrypoint /usr/local/bin/scalpel-discovery   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/scalpel-discovery   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### scalpel-export

```bash
$ singularity exec <container> /usr/local/bin/scalpel-export
$ podman run --it --rm --entrypoint /usr/local/bin/scalpel-export   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/scalpel-export   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### gff2gff.py

```bash
$ singularity exec <container> /usr/local/bin/gff2gff.py
$ podman run --it --rm --entrypoint /usr/local/bin/gff2gff.py   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/gff2gff.py   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### bamtools

```bash
$ singularity exec <container> /usr/local/bin/bamtools
$ podman run --it --rm --entrypoint /usr/local/bin/bamtools   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/bamtools   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### guess-ploidy.py

```bash
$ singularity exec <container> /usr/local/bin/guess-ploidy.py
$ podman run --it --rm --entrypoint /usr/local/bin/guess-ploidy.py   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/guess-ploidy.py   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### plot-roh.py

```bash
$ singularity exec <container> /usr/local/bin/plot-roh.py
$ podman run --it --rm --entrypoint /usr/local/bin/plot-roh.py   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/plot-roh.py   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### run-roh.pl

```bash
$ singularity exec <container> /usr/local/bin/run-roh.pl
$ podman run --it --rm --entrypoint /usr/local/bin/run-roh.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/run-roh.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### color-chrs.pl

```bash
$ singularity exec <container> /usr/local/bin/color-chrs.pl
$ podman run --it --rm --entrypoint /usr/local/bin/color-chrs.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/color-chrs.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### plot-vcfstats

```bash
$ singularity exec <container> /usr/local/bin/plot-vcfstats
$ podman run --it --rm --entrypoint /usr/local/bin/plot-vcfstats   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/plot-vcfstats   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### bcftools

```bash
$ singularity exec <container> /usr/local/bin/bcftools
$ podman run --it --rm --entrypoint /usr/local/bin/bcftools   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/bcftools   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### vcfutils.pl

```bash
$ singularity exec <container> /usr/local/bin/vcfutils.pl
$ podman run --it --rm --entrypoint /usr/local/bin/vcfutils.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/vcfutils.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### fasta-sanitize.pl

```bash
$ singularity exec <container> /usr/local/bin/fasta-sanitize.pl
$ podman run --it --rm --entrypoint /usr/local/bin/fasta-sanitize.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/fasta-sanitize.pl   -v ${PWD} -w ${PWD} <container> -c " $@"
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