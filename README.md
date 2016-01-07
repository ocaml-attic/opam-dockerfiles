This repository contains a set of [Docker](http://docker.com) container definitions for various combination of [OCaml](https://ocaml.org) and the [OPAM](https://opam.ocaml.org) package manager.  The containers all come preinstalled with a working compiler and an OPAM environment.  Using it as simple as:

```
docker pull ocaml/opam
docker run -ti ocaml/opam bash
```

...to get a working development environment.  You can grab a specific distribution and test out external dependencies as well:
```
docker run ocaml/opam:ubuntu-14.04_ocaml-4.02.3 opam depext -i cohttp lwt ssl
```

The latest stable distributions are summarised below.  The default OCaml version available in the container is marked with a &#127347; symbol, and a system installation of OCaml (as opposed to a locally compiled switch) is marked with a &#127362; symbol.

Distribution | Available Switches | Command
------------ | ------------------ | -------
Alpine | 4.02.3 &#127362;&#127347; | `docker pull ocaml/opam:alpine`
CentOS | 4.02.3 &#127347; | `docker pull ocaml/opam:centos`
Debian | 4.01.0 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:debian`
Fedora | 4.02.2 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:fedora`
OracleLinux | 4.02.3 &#127347; | `docker pull ocaml/opam:oraclelinux`
Ubuntu | 4.01.0 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:ubuntu`

There are also individual containers available for each combination
   of an OS distribution and an OCaml revision. These should be useful for
   testing and continuous integration, since they will remain pinned to these
   versions for as long as the upstream distribution is supported.  Note that
   older releases may have security issues if upstream stops maintaining them.

Distro | Compiler | Command
------ | -------- | -------
Alpine 3.3 | 4.00.1 &#127347; | `docker pull ocaml/opam:alpine-3.3_ocaml-4.00.1`
CentOS 6 | 4.00.1 &#127347; | `docker pull ocaml/opam:centos-6_ocaml-4.00.1`
CentOS 7 | 4.00.1 &#127347; | `docker pull ocaml/opam:centos-7_ocaml-4.00.1`
Debian Stable | 4.00.1 &#127347; | `docker pull ocaml/opam:debian-stable_ocaml-4.00.1`
Debian Testing | 4.00.1 &#127347; | `docker pull ocaml/opam:debian-testing_ocaml-4.00.1`
Debian Unstable | 4.00.1 &#127347; | `docker pull ocaml/opam:debian-unstable_ocaml-4.00.1`
Fedora 22 | 4.00.1 &#127347; | `docker pull ocaml/opam:fedora-22_ocaml-4.00.1`
Fedora 23 | 4.00.1 &#127347; | `docker pull ocaml/opam:fedora-23_ocaml-4.00.1`
OracleLinux 7 | 4.00.1 &#127347; | `docker pull ocaml/opam:oraclelinux-7_ocaml-4.00.1`
Ubuntu 12.04 | 4.00.1 &#127347; | `docker pull ocaml/opam:ubuntu-12.04_ocaml-4.00.1`
Ubuntu 14.04 | 4.00.1 &#127347; | `docker pull ocaml/opam:ubuntu-14.04_ocaml-4.00.1`
Ubuntu 15.10 | 4.00.1 &#127347; | `docker pull ocaml/opam:ubuntu-15.10_ocaml-4.00.1`
Ubuntu 16.04 | 4.00.1 &#127347; | `docker pull ocaml/opam:ubuntu-16.04_ocaml-4.00.1`
Alpine 3.3 | 4.01.0 &#127347; | `docker pull ocaml/opam:alpine-3.3_ocaml-4.01.0`
CentOS 6 | 4.01.0 &#127347; | `docker pull ocaml/opam:centos-6_ocaml-4.01.0`
CentOS 7 | 4.01.0 &#127347; | `docker pull ocaml/opam:centos-7_ocaml-4.01.0`
Debian Stable | 4.01.0 &#127362;&#127347; | `docker pull ocaml/opam:debian-stable_ocaml-4.01.0`
Debian Testing | 4.01.0 &#127347; | `docker pull ocaml/opam:debian-testing_ocaml-4.01.0`
Debian Unstable | 4.01.0 &#127347; | `docker pull ocaml/opam:debian-unstable_ocaml-4.01.0`
Fedora 22 | 4.01.0 &#127347; | `docker pull ocaml/opam:fedora-22_ocaml-4.01.0`
Fedora 23 | 4.01.0 &#127347; | `docker pull ocaml/opam:fedora-23_ocaml-4.01.0`
OracleLinux 7 | 4.01.0 &#127347; | `docker pull ocaml/opam:oraclelinux-7_ocaml-4.01.0`
Ubuntu 12.04 | 4.01.0 &#127347; | `docker pull ocaml/opam:ubuntu-12.04_ocaml-4.01.0`
Ubuntu 14.04 | 4.01.0 &#127362;&#127347; | `docker pull ocaml/opam:ubuntu-14.04_ocaml-4.01.0`
Ubuntu 15.10 | 4.01.0 &#127362;&#127347; | `docker pull ocaml/opam:ubuntu-15.10_ocaml-4.01.0`
Ubuntu 16.04 | 4.01.0 &#127347; | `docker pull ocaml/opam:ubuntu-16.04_ocaml-4.01.0`
Alpine 3.3 | 4.02.3 &#127362;&#127347; | `docker pull ocaml/opam:alpine-3.3_ocaml-4.02.3`
CentOS 6 | 4.02.3 &#127347; | `docker pull ocaml/opam:centos-6_ocaml-4.02.3`
CentOS 7 | 4.02.3 &#127347; | `docker pull ocaml/opam:centos-7_ocaml-4.02.3`
Debian Stable | 4.02.3 &#127347; | `docker pull ocaml/opam:debian-stable_ocaml-4.02.3`
Debian Testing | 4.02.3 &#127362;&#127347; | `docker pull ocaml/opam:debian-testing_ocaml-4.02.3`
Debian Unstable | 4.02.3 &#127362;&#127347; | `docker pull ocaml/opam:debian-unstable_ocaml-4.02.3`
Fedora 22 | 4.02.3 &#127347; | `docker pull ocaml/opam:fedora-22_ocaml-4.02.3`
Fedora 23 | 4.02.3 &#127347; | `docker pull ocaml/opam:fedora-23_ocaml-4.02.3`
OracleLinux 7 | 4.02.3 &#127347; | `docker pull ocaml/opam:oraclelinux-7_ocaml-4.02.3`
Ubuntu 12.04 | 4.02.3 &#127347; | `docker pull ocaml/opam:ubuntu-12.04_ocaml-4.02.3`
Ubuntu 14.04 | 4.02.3 &#127347; | `docker pull ocaml/opam:ubuntu-14.04_ocaml-4.02.3`
Ubuntu 15.10 | 4.02.3 &#127347; | `docker pull ocaml/opam:ubuntu-15.10_ocaml-4.02.3`
Ubuntu 16.04 | 4.02.3 &#127362;&#127347; | `docker pull ocaml/opam:ubuntu-16.04_ocaml-4.02.3`
Alpine 3.3 | 4.03.0+trunk &#127347; | `docker pull ocaml/opam:alpine-3.3_ocaml-4.03.0_trunk`
CentOS 6 | 4.03.0+trunk &#127347; | `docker pull ocaml/opam:centos-6_ocaml-4.03.0_trunk`
CentOS 7 | 4.03.0+trunk &#127347; | `docker pull ocaml/opam:centos-7_ocaml-4.03.0_trunk`
Debian Stable | 4.03.0+trunk &#127347; | `docker pull ocaml/opam:debian-stable_ocaml-4.03.0_trunk`
Debian Testing | 4.03.0+trunk &#127347; | `docker pull ocaml/opam:debian-testing_ocaml-4.03.0_trunk`
Debian Unstable | 4.03.0+trunk &#127347; | `docker pull ocaml/opam:debian-unstable_ocaml-4.03.0_trunk`
Fedora 22 | 4.03.0+trunk &#127347; | `docker pull ocaml/opam:fedora-22_ocaml-4.03.0_trunk`
Fedora 23 | 4.03.0+trunk &#127347; | `docker pull ocaml/opam:fedora-23_ocaml-4.03.0_trunk`
OracleLinux 7 | 4.03.0+trunk &#127347; | `docker pull ocaml/opam:oraclelinux-7_ocaml-4.03.0_trunk`
Ubuntu 12.04 | 4.03.0+trunk &#127347; | `docker pull ocaml/opam:ubuntu-12.04_ocaml-4.03.0_trunk`
Ubuntu 14.04 | 4.03.0+trunk &#127347; | `docker pull ocaml/opam:ubuntu-14.04_ocaml-4.03.0_trunk`
Ubuntu 15.10 | 4.03.0+trunk &#127347; | `docker pull ocaml/opam:ubuntu-15.10_ocaml-4.03.0_trunk`
Ubuntu 16.04 | 4.03.0+trunk &#127347; | `docker pull ocaml/opam:ubuntu-16.04_ocaml-4.03.0_trunk`


## Contributing

To discuss these containers, please e-mail Anil Madhavapeddy <anil@recoil.org> or the OPAM development list at <opam-devel@lists.ocaml.org>. Contributions of Dockerfiles for additional OS distributions are most welcome! The files here are all autogenerated from the [ocaml-docker-scripts](https://github.com/avsm/ocaml-docker-scripts) repository, so please do not submit any PRs directly to this location. The containers are built and hosted on the Docker Hub [ocaml organisation](https://hub.docker.com/u/ocaml).