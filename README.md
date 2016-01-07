The latest stable distributions are summarised below.  The default OCaml version available in the container is marked with a &#127347; symbol, and a system installation of OCaml (as opposed to a locally compiled switch) is marked with a &#127362; symbol.

Distribution | Available Switches | Command
------------ | ------------------ | -------
ubuntu | `4.01.0` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:ubuntu`
debian | `4.01.0` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:debian`
fedora | `4.02.2` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:fedora`
centos | `4.02.3` &#127347; | `docker pull ocaml/opam:centos`
oraclelinux | `4.02.3` &#127347; | `docker pull ocaml/opam:oraclelinux`
alpine | `4.02.3` &#127362;&#127347; | `docker pull ocaml/opam:alpine`

There are also individual containers available for each combination
   of an OS distribution and an OCaml revision. These should be useful for
   testing and continuous integration, since they will remain pinned to these
   versions for as long as the upstream distribution is supported.  Note that
   older releases may have security issues if upstream stops maintaining them.

Distribution and Compiler | Command
------------------------- | -------
ubuntu-12.04 with OCaml `3.12.1` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:ubuntu-12.04`
ubuntu-14.04 with OCaml `4.01.0` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:ubuntu-14.04`
ubuntu-15.10 with OCaml `4.01.0` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:ubuntu-15.10`
ubuntu-16.04 with OCaml `4.02.3` &#127362;&#127347; | `docker pull ocaml/opam:ubuntu-16.04`
debian-stable with OCaml `4.01.0` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:debian-stable`
debian-testing with OCaml `4.02.3` &#127362;&#127347; | `docker pull ocaml/opam:debian-testing`
debian-unstable with OCaml `4.02.3` &#127362;&#127347; | `docker pull ocaml/opam:debian-unstable`
fedora-22 with OCaml `4.02.0` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:fedora-22`
fedora-23 with OCaml `4.02.2` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:fedora-23`
centos-6 with OCaml `4.02.3` &#127347; | `docker pull ocaml/opam:centos-6`
centos-7 with OCaml `4.02.3` &#127347; | `docker pull ocaml/opam:centos-7`
oraclelinux-7 with OCaml `4.02.3` &#127347; | `docker pull ocaml/opam:oraclelinux-7`
alpine-3.3 with OCaml `4.02.3` &#127362;&#127347; | `docker pull ocaml/opam:alpine-3.3`
ubuntu-12.04 with OCaml `3.12.1` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:ubuntu-12.04`
ubuntu-14.04 with OCaml `4.01.0` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:ubuntu-14.04`
ubuntu-15.10 with OCaml `4.01.0` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:ubuntu-15.10`
ubuntu-16.04 with OCaml `4.02.3` &#127362;&#127347; | `docker pull ocaml/opam:ubuntu-16.04`
debian-stable with OCaml `4.01.0` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:debian-stable`
debian-testing with OCaml `4.02.3` &#127362;&#127347; | `docker pull ocaml/opam:debian-testing`
debian-unstable with OCaml `4.02.3` &#127362;&#127347; | `docker pull ocaml/opam:debian-unstable`
fedora-22 with OCaml `4.02.0` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:fedora-22`
fedora-23 with OCaml `4.02.2` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:fedora-23`
centos-6 with OCaml `4.02.3` &#127347; | `docker pull ocaml/opam:centos-6`
centos-7 with OCaml `4.02.3` &#127347; | `docker pull ocaml/opam:centos-7`
oraclelinux-7 with OCaml `4.02.3` &#127347; | `docker pull ocaml/opam:oraclelinux-7`
alpine-3.3 with OCaml `4.02.3` &#127362;&#127347; | `docker pull ocaml/opam:alpine-3.3`
ubuntu-12.04 with OCaml `3.12.1` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:ubuntu-12.04`
ubuntu-14.04 with OCaml `4.01.0` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:ubuntu-14.04`
ubuntu-15.10 with OCaml `4.01.0` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:ubuntu-15.10`
ubuntu-16.04 with OCaml `4.02.3` &#127362;&#127347; | `docker pull ocaml/opam:ubuntu-16.04`
debian-stable with OCaml `4.01.0` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:debian-stable`
debian-testing with OCaml `4.02.3` &#127362;&#127347; | `docker pull ocaml/opam:debian-testing`
debian-unstable with OCaml `4.02.3` &#127362;&#127347; | `docker pull ocaml/opam:debian-unstable`
fedora-22 with OCaml `4.02.0` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:fedora-22`
fedora-23 with OCaml `4.02.2` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:fedora-23`
centos-6 with OCaml `4.02.3` &#127347; | `docker pull ocaml/opam:centos-6`
centos-7 with OCaml `4.02.3` &#127347; | `docker pull ocaml/opam:centos-7`
oraclelinux-7 with OCaml `4.02.3` &#127347; | `docker pull ocaml/opam:oraclelinux-7`
alpine-3.3 with OCaml `4.02.3` &#127362;&#127347; | `docker pull ocaml/opam:alpine-3.3`
ubuntu-12.04 with OCaml `3.12.1` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:ubuntu-12.04`
ubuntu-14.04 with OCaml `4.01.0` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:ubuntu-14.04`
ubuntu-15.10 with OCaml `4.01.0` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:ubuntu-15.10`
ubuntu-16.04 with OCaml `4.02.3` &#127362;&#127347; | `docker pull ocaml/opam:ubuntu-16.04`
debian-stable with OCaml `4.01.0` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:debian-stable`
debian-testing with OCaml `4.02.3` &#127362;&#127347; | `docker pull ocaml/opam:debian-testing`
debian-unstable with OCaml `4.02.3` &#127362;&#127347; | `docker pull ocaml/opam:debian-unstable`
fedora-22 with OCaml `4.02.0` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:fedora-22`
fedora-23 with OCaml `4.02.2` &#127362;, `4.02.3` &#127347; | `docker pull ocaml/opam:fedora-23`
centos-6 with OCaml `4.02.3` &#127347; | `docker pull ocaml/opam:centos-6`
centos-7 with OCaml `4.02.3` &#127347; | `docker pull ocaml/opam:centos-7`
oraclelinux-7 with OCaml `4.02.3` &#127347; | `docker pull ocaml/opam:oraclelinux-7`
alpine-3.3 with OCaml `4.02.3` &#127362;&#127347; | `docker pull ocaml/opam:alpine-3.3`