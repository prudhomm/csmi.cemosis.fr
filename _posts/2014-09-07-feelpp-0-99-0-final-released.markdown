---
layout: news_item
title: 'Feel++ 0.99.0 Released'
date: 2014-09-07
author: prudhomm
fullname: Christophe Prud'homme
version: v0.99.0-final
categories: [release]
tags: feelpp
---

Feel++ 0.99.0 has been released. The tarball is [here](https://github.com/feelpp/feelpp/releases) and it is available on
[Feel++ Homebrew-Science](https://github.com/feelpp/homebrew-science) for
MacOSX and [Ubuntu Feel++ PPA](https://launchpad.net/~feelpp/+archive/ppa),
Debian packages should be available really soon now.

Feel++ 0.99.0 brings various new features such that

 - In memory mesh generation without having the go through disk read-write
 - Parallel file export
   - ensightgold format and MPI-IO
   - HDF5 and Xdmf file formats
 - Support Fast Marching for hypercube
 - Support for NLOpt a non-linear optimisation library

Finally check out the [changelog][] for a more
exhaustive list of changes. Happy Feeling!

[changelog]: /docs/develop/ChangeLog.html
