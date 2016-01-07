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
Ubuntu | 4.01.0 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:ubuntu`
Debian | 4.01.0 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:debian`
Fedora | 4.02.2 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:fedora`
CentOS | 4.02.3 &#127347; | `docker pull ocaml/opam:centos`
OracleLinux | 4.02.3 &#127347; | `docker pull ocaml/opam:oraclelinux`
Alpine | 4.02.3 &#127362;&#127347; | `docker pull ocaml/opam:alpine`

There are also individual containers available for each combination
   of an OS distribution and an OCaml revision. These should be useful for
   testing and continuous integration, since they will remain pinned to these
   versions for as long as the upstream distribution is supported.  Note that
   older releases may have security issues if upstream stops maintaining them.

Distribution and Compiler | Command
------------------------- | -------
Ubuntu 12.04 with OCaml 3.12.1 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:ubuntu-12.04`
Ubuntu 14.04 with OCaml 4.01.0 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:ubuntu-14.04`
Ubuntu 15.10 with OCaml 4.01.0 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:ubuntu-15.10`
Ubuntu 16.04 with OCaml 4.02.3 &#127362;&#127347; | `docker pull ocaml/opam:ubuntu-16.04`
Debian Stable with OCaml 4.01.0 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:debian-stable`
Debian Testing with OCaml 4.02.3 &#127362;&#127347; | `docker pull ocaml/opam:debian-testing`
Debian Unstable with OCaml 4.02.3 &#127362;&#127347; | `docker pull ocaml/opam:debian-unstable`
Fedora 22 with OCaml 4.02.0 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:fedora-22`
Fedora 23 with OCaml 4.02.2 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:fedora-23`
CentOS 6 with OCaml 4.02.3 &#127347; | `docker pull ocaml/opam:centos-6`
CentOS 7 with OCaml 4.02.3 &#127347; | `docker pull ocaml/opam:centos-7`
OracleLinux 7 with OCaml 4.02.3 &#127347; | `docker pull ocaml/opam:oraclelinux-7`
Alpine 3.3 with OCaml 4.02.3 &#127362;&#127347; | `docker pull ocaml/opam:alpine-3.3`
Ubuntu 12.04 with OCaml 3.12.1 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:ubuntu-12.04`
Ubuntu 14.04 with OCaml 4.01.0 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:ubuntu-14.04`
Ubuntu 15.10 with OCaml 4.01.0 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:ubuntu-15.10`
Ubuntu 16.04 with OCaml 4.02.3 &#127362;&#127347; | `docker pull ocaml/opam:ubuntu-16.04`
Debian Stable with OCaml 4.01.0 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:debian-stable`
Debian Testing with OCaml 4.02.3 &#127362;&#127347; | `docker pull ocaml/opam:debian-testing`
Debian Unstable with OCaml 4.02.3 &#127362;&#127347; | `docker pull ocaml/opam:debian-unstable`
Fedora 22 with OCaml 4.02.0 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:fedora-22`
Fedora 23 with OCaml 4.02.2 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:fedora-23`
CentOS 6 with OCaml 4.02.3 &#127347; | `docker pull ocaml/opam:centos-6`
CentOS 7 with OCaml 4.02.3 &#127347; | `docker pull ocaml/opam:centos-7`
OracleLinux 7 with OCaml 4.02.3 &#127347; | `docker pull ocaml/opam:oraclelinux-7`
Alpine 3.3 with OCaml 4.02.3 &#127362;&#127347; | `docker pull ocaml/opam:alpine-3.3`
Ubuntu 12.04 with OCaml 3.12.1 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:ubuntu-12.04`
Ubuntu 14.04 with OCaml 4.01.0 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:ubuntu-14.04`
Ubuntu 15.10 with OCaml 4.01.0 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:ubuntu-15.10`
Ubuntu 16.04 with OCaml 4.02.3 &#127362;&#127347; | `docker pull ocaml/opam:ubuntu-16.04`
Debian Stable with OCaml 4.01.0 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:debian-stable`
Debian Testing with OCaml 4.02.3 &#127362;&#127347; | `docker pull ocaml/opam:debian-testing`
Debian Unstable with OCaml 4.02.3 &#127362;&#127347; | `docker pull ocaml/opam:debian-unstable`
Fedora 22 with OCaml 4.02.0 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:fedora-22`
Fedora 23 with OCaml 4.02.2 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:fedora-23`
CentOS 6 with OCaml 4.02.3 &#127347; | `docker pull ocaml/opam:centos-6`
CentOS 7 with OCaml 4.02.3 &#127347; | `docker pull ocaml/opam:centos-7`
OracleLinux 7 with OCaml 4.02.3 &#127347; | `docker pull ocaml/opam:oraclelinux-7`
Alpine 3.3 with OCaml 4.02.3 &#127362;&#127347; | `docker pull ocaml/opam:alpine-3.3`
Ubuntu 12.04 with OCaml 3.12.1 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:ubuntu-12.04`
Ubuntu 14.04 with OCaml 4.01.0 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:ubuntu-14.04`
Ubuntu 15.10 with OCaml 4.01.0 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:ubuntu-15.10`
Ubuntu 16.04 with OCaml 4.02.3 &#127362;&#127347; | `docker pull ocaml/opam:ubuntu-16.04`
Debian Stable with OCaml 4.01.0 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:debian-stable`
Debian Testing with OCaml 4.02.3 &#127362;&#127347; | `docker pull ocaml/opam:debian-testing`
Debian Unstable with OCaml 4.02.3 &#127362;&#127347; | `docker pull ocaml/opam:debian-unstable`
Fedora 22 with OCaml 4.02.0 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:fedora-22`
Fedora 23 with OCaml 4.02.2 &#127362;, 4.02.3 &#127347; | `docker pull ocaml/opam:fedora-23`
CentOS 6 with OCaml 4.02.3 &#127347; | `docker pull ocaml/opam:centos-6`
CentOS 7 with OCaml 4.02.3 &#127347; | `docker pull ocaml/opam:centos-7`
OracleLinux 7 with OCaml 4.02.3 &#127347; | `docker pull ocaml/opam:oraclelinux-7`
Alpine 3.3 with OCaml 4.02.3 &#127362;&#127347; | `docker pull ocaml/opam:alpine-3.3`

To discuss these containers, please e-mail Anil Madhavapeddy <anil@recoil.org> or the OPAM development list at <opam-devel@lists.ocaml.org>.