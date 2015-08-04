---
layout: news_item
title: HAMM/Mortar, about 5 billions unknowns on 40K cores using Feel++
date: 2014-09-01
author: prudhomm
fullname: Christophe Prud'homme
categories: [project]
project: [HAMM/Mortar]
tags: feelpp
---

We are developing a substructuring preconditioner for the
\\(h\\)-\\(p\\) mortar method. In order to corroborate the
mathematical properties of this preconditioner we ran various test to
check the dependency with respect to \\(H\\) (the number of
subdomaines), \\(h\\) the grid size within the subdomains and \\(p\\)
the polynomial degree used by the finite element approximation.

We have the following result

<center>\\(\mathrm{cond}(P^{-1} A) \leq p^{3/2} (1+\mathrm{log}(\frac{H p^2}{h}))^2\\\)</center>

where \\(P\\) is our preconditioner and \\(A\\) is the Schur
complement associated to the \\(h-p\\) mortar discretisation of an
elliptic problem.

We plot below the ratio for  \\(p=1,...,5\\) and \\(H/h = 80\\)

<center>\\(\lambda^p = \dfrac{\mathrm{cond}(P^{-1} A)}{(1+\mathrm{log}(\frac{H p^2}{h}))^2} \\)</center>

as well as the number of iterations needed to decrease the relative residual by 1e-6


 Cores          |\\(\lambda^1\\)(iterations) |\\(\lambda^2\\)(iterations)    |\\(\lambda^3\\)(iterations)  |\\(\lambda^4\\)(iterations)   |\\(\lambda^5\\)(iterations)
----------------|----------------------------|-------------------------------|-----------------------------|------------------------------|----------------------------------
 16             |1.65(31)                    |1.14(32)                       |1.06(33)                     |1.03(38)                      |1.02(39)
 64             |1.74(31)                    |1.21(33)                       |1.11(35)                     |1.07(40)                      |1.07(42)
 256            |1.76(28)                    |1.23(32)                       |1.12(34)                     |1.08(36)                      |1.06(40)
 1024           |1.78(27)                    |1.23(29)                       |1.12(31)                     |1.08(32)                      |1.06(34)
 4096           |1.79(25)                    |1.23(28)                       |1.12(29)                     |1.08(31)                      |1.06(31)
 16384          |1.52(20)                    |0.88(22)                       |0.91(26)                     |0.94(27)                      |0.96(28)
 22500          |1.52(19)                    |0.88(20)                       |0.69(22)                     |0.95(26)                      |0.99(27)
 40000          |1.52(17)                    |0.88(20)                       |0.69(22)                     |0.68(23)                      |(N/A)(N/A)

As you can see the number of iterations increase very little as
\\(p\\) increases and stays constant or decreases as the number of
subdomains increases which is of course a very nice feature.

Here is the table with the number of degrees of freedom corresponding
to these calculations at 40000 cores, we reach about 5 billions of
unknowns.

Order | Unknowns
:----:|:--------:
1 | 295'725'687
2 | 1'182'838'857
3 | 2'661'337'501
4 | 4'731'229'377

The last computation at \\(p=4\\) takes about **150s**.

These computations have been done at the mesocentre of Strasbourg from 16 to 256 cores then on Curie at the TGCC in France up to 40000 cores !

This work is the result of the collaboration between Abdoulaye Samake and Christophe Prud'homme from [Cemosis](http://www.cemosis.fr) and Silvia Bertoluzza and Micol Pennacchio from [IMATI](http://www.imati.cnr.it).

The submitted paper is available on [HAL](https://hal.archives-ouvertes.fr/hal-01066606v1).
