---
layout: news_item
title: 'Feel++ 0.98.0 Released'
date: 2014-05-22
author: prudhomm
fullname: Christophe Prud'homme
version: v0.98.0-final
categories: [release]
tags: [feelpp]
---

Feel++ 0.98.0 has been released. The tarball is [here](https://github.com/feelpp/feelpp/releases) and it is available on
[Feel++ Homebrew-Science](https://github.com/feelpp/homebrew-science) for
MacOSX and [Ubuntu Feel++ PPA](https://launchpad.net/~feelpp/+archive/ppa),
Debian packages should be available really soon now.

Feel++ 0.98.0 brings various new features such that

 - Mortar approximation in 2D tested up to order 5 on both hypercube and
   simplex

 - Initialization of elements of functions at construction with an expression

{% highlight c++ %}
  auto Xh = Pch<2>(mesh);
  // u is a scalar field initialized to x*y
  auto u = Xh->element(expr("x*y:x:y"));
  auto Vh = Pchv<2>(mesh);
  // v is a vector field initialized to (sin(pi*x),sin(pi*y))
  auto v = Xh->element(expr<2,1>("{sin(pi*x),sin(pi*y)}:x:y"));
{% endhighlight %}

 Also element of function spaces have now a `on` member functions that allows
 in the case of nodal basis functions to set the function to the interpolant
 with respect to the associated finite element over a range of elements

 {% highlight c++ %}
  u.on( range=markedelements(mesh,"material 1"),
       _expr=expr("x+y:x:y") );
 {% endhighlight %}

 - Lambda expression up to three arguments

 {% highlight c++ %}
  auto I = integrate(_range=elements(mesh), _e1*_e2);
  auto Xh = Pch<2>(mesh);
  auto u = Xh->element(expr("x*y:x:y"));
  auto v = Xh->element(expr<2,1>("{sin(pi*x),sin(pi*y)}:x:y"));
  std::cout << "I(u,v) = I(gradv(u), idv(v)).evaluate();
  {% endhighlight %}

  This example does not however really illustrate the usefulness of this
  feature, this feature is used now to switch between approximations types
  such as finite element and reduced basis approximations in the empirical
  interpolation method.

 - Refactoring of the solver/preconditioner framework, the changes are
   essentially internal. However it does bring some new options in the command
   line of cfg files.


Finally check out the [changelog][] for a more
exhaustive list of changes. Happy Feeling!

[changelog]: /docs/develop/ChangeLog.html
