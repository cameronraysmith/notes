+++
title = "maxima"
author = ["Cameron Smith"]
lastmod = 2020-11-30T00:42:39-05:00
slug = "maxima"
draft = false
+++

## references {#references}

-   [Maxima manual](http://maxima.sourceforge.net/docs/manual/maxima.html)
-   [Tensor manipulation in GPL Maxima by Viktor Toth in 2007]({{< relref "Tensor_manipulation_in_GPL_Maxima_by_Viktor_Toth_in_2007" >}})
    -   [Viktor Toth's up-to-date implementations of atensor, ctensor, itensor](https://www.vttoth.com/CMS/projects/61-the-maxima-computer-algebra-system)
-   [Edwin Woollett's Maxima by Example](http://web.csulb.edu/~woollett/)
-   [Catalogue of Spacetimes by Mueller and Grave in 2009]({{< relref "Catalogue_of_Spacetimes_by_Mueller_and_Grave_in_2009" >}})
-   Test conversion of [mathphysics/GR.ipynb at master · ernestyalumni/mathphysics](https://github.com/ernestyalumni/mathphysics/blob/master/playground/GR.ipynb) into [maxima]({{< relref "maxima" >}}) via [Tensor manipulation in GPL Maxima by Viktor Toth in 2007]({{< relref "Tensor_manipulation_in_GPL_Maxima_by_Viktor_Toth_in_2007" >}}).
-   [calyau/maxima-tutorial-notebooks](https://github.com/calyau/maxima-tutorial-notebooks)


## maxima in org-babel {#maxima-in-org-babel}

-   Note maxima does not have sessions


### general usage {#general-usage}

-   If we want to generate tex from maxima in org-mode files we can use [Inline Display of Maxima LaTeX Output](https://orgmode.org/worg/org-contrib/babel/languages/ob-doc-maxima.html#org40fb6cc)

\\[{{e^ {- x }}\over{x}}\\]

-   Example of Taylor series

\\[U\left(a\right)+\left(\left.{{d}\over{d\,x}}\,U\left(x\right)
 \right|\_{x=a}\right)\,\left(x-a\right)+{{\left(\left.{{d^2}\over{d\,
 x^2}}\,U\left(x\right)\right|\_{x=a}\right)\,\left(x-a\right)^2
 }\over{2}}+\cdots \\]


### plotting {#plotting}

<!--list-separator-->

-  Test figure inclusion of arbitrary file

    <a id="orgb127b75"></a>

    </ox-hugo/maxima-3d.pdf>
