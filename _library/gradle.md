---
layout: container
name:  "gradle"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/gradle/container.yaml"
config_url: "https://raw.githubusercontent.com/singularityhub/shpc-registry/main/gradle/container.yaml"
updated_at: "2023-01-13 03:47:34.248574"
latest: "7-jdk19"
container_url: "https://hub.docker.com/_/gradle"
aliases:
 - "gradle"
versions:
 - "7.0.0-hotspot"
 - "7.0.1-hotspot"
 - "7.0.2-hotspot"
 - "7.1.0-hotspot"
 - "7.1.1-hotspot"
 - "7.2.0"
 - "7.3.0"
 - "7.3.3"
 - "7.4.0"
 - "latest"
 - "7"
 - "7-jdk17"
 - "7-jdk16"
 - "7-jdk11"
 - "7-jdk-openj9"
 - "7-jdk18"
 - "7-jdk19"
description: "Gradle is a build tool with a focus on build automation and support for multi-language development."
config: {"docker": "gradle", "url": "https://hub.docker.com/_/gradle", "maintainer": "@vsoch", "description": "Gradle is a build tool with a focus on build automation and support for multi-language development.", "latest": {"7-jdk19": "sha256:7b0d5ddb28458a90fe235884f89f89f216dac9604ae2d2e8504462af3f75ad61"}, "tags": {"7.0.0-hotspot": "sha256:cef49a7bdb0c53dc0d64ed24f375fb0fdd6e3489d0b4fcd393f0c8c09be11320", "7.0.1-hotspot": "sha256:f3207f774a8ceb3286e0b65ca1864cfab639797a307c3d505bc6775adfb28d66", "7.0.2-hotspot": "sha256:b36aabaa3f4b333aae071be8658ad2fa558bcaea9e31b3e8dc42f6e7846cbd01", "7.1.0-hotspot": "sha256:92c0f3381fd8db612dac10b5b584d68376c192bae6b1a11b2190780a60411fe4", "7.1.1-hotspot": "sha256:19d9bdf24a291e5d7ac758c8d0c7d8f2f5d641b130d17b556dbab2c49701bf3e", "7.2.0": "sha256:67de4380b26d2b5406077cf5439b3488d139f7fedd9bdb8ddfadbe277750ede8", "7.3.0": "sha256:1f65f4991aa496cf835cbce10290bdc71c1cb526b4df807d97c4f51b863f2399", "7.3.3": "sha256:8d037a3bd86fc48b591ad778d6eb6130e641bad1be546923e6d097a7ad7708eb", "7.4.0": "sha256:5248d0e8f7f6ad2095c3a053d5461daa17b02097410f0e9f6397f8f4dedc34bf", "latest": "sha256:9073fad2045e28b86d2d1669bc219739a84771635f033aed0fa293835dd5fad0", "7": "sha256:9073fad2045e28b86d2d1669bc219739a84771635f033aed0fa293835dd5fad0", "7-jdk17": "sha256:9073fad2045e28b86d2d1669bc219739a84771635f033aed0fa293835dd5fad0", "7-jdk16": "sha256:f174c0dcf9a84b4035f1fcb62f0340ddc69c0b93320e0d35f097d20ce2ca89d5", "7-jdk11": "sha256:e33f31f2e48f955f12464db35c041438a7b1ffc7fc7e1f069bbabca3254dd81a", "7-jdk-openj9": "sha256:acd908af42e1bee2f841eeac031d41317ab3fddcc3ec9d0d4e1cb4b28be24f5f", "7-jdk18": "sha256:f3c6308a57fa86af3c05ed1746cd041035074ed932cb9fecc0a0efedad35955e", "7-jdk19": "sha256:7b0d5ddb28458a90fe235884f89f89f216dac9604ae2d2e8504462af3f75ad61"}, "aliases": {"gradle": "/usr/bin/gradle"}}
---

This module is a singularity container wrapper for gradle.
Gradle is a build tool with a focus on build automation and support for multi-language development.
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install gradle
```

Or a specific version:

```bash
$ shpc install gradle:7-jdk19
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load gradle/7-jdk19
$ module help gradle/7-jdk19
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### gradle-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### gradle-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### gradle-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### gradle-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### gradle-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### gradle-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### gradle

```bash
$ singularity exec <container> /usr/bin/gradle
$ podman run --it --rm --entrypoint /usr/bin/gradle   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/bin/gradle   -v ${PWD} -w ${PWD} <container> -c " $@"
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