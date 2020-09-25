+++
title = "Physics from Symmetry by Jakob Schwichtenberg in 2015"
author = ["Cameron Smith"]
lastmod = 2020-09-21T11:13:52-04:00
slug = "Physics_from_Symmetry_by_Jakob_Schwichtenberg_in_2015"
draft = false
+++

## \![Physics from Symmetry by Jakob Schwichtenberg in 2015 Cover](<https://lh3.googleusercontent.com/Pv7ch%5FxOw-qgh7yJbWRGmkjAUp0fGyQtJrvG26NK4RW0JdX8ZtnwZqL8KEdCRyd8CMlQHTt9SXhui-iMJy3ynQsn39cKOUwJLT3mCEN%5FCVY0RfCxPwXSIToY4to2uTV5Z3LV8Ibgl7I=w603-h802-no>) {#physics-from-symmetry-by-jakob-schwichtenberg-in-2015-cover--https-lh3-dot-googleusercontent-dot-com-pv7ch-xow-qgh7yjbwrgmkjaup0fgyqtjrvg26nk4rw0jdx8ztnwzql8kedcryd8cmlqhtt9sxhui-imjy3ynqsn39ckouwjlt3mcen-cvy0rfcxpwxsitoy4to2utv5z3lv8ibgl7i-w603-h802-no}


## [books]({{< relref "books" >}}), [physics]({{< relref "physics" >}}), [symmetry]({{< relref "symmetry" >}}) {#books--books-dot-md--physics--physics-dot-md--symmetry--symmetry-dot-md}


## Part I: Foundations {#part-i-foundations}


### 1. Introduction (8) {#1-dot-introduction--8}

<!--list-separator-->

-  1.1 What we cannot derive

<!--list-separator-->

-  1.2 Book overview

<!--list-separator-->

-  1.3 Elementary particles and fundamental forces


### 2. Special relativity (14) {#2-dot-special-relativity--14}

<!--list-separator-->

-  2.1 The invariant of special relativity

<!--list-separator-->

-  2.2 Proper time

<!--list-separator-->

-  2.3 Upper speed limit

<!--list-separator-->

-  2.4 The Minkowski Notation

<!--list-separator-->

-  2.5 Lorentz transformations

<!--list-separator-->

-  2.6 Invariance, symmetry, and covariance


## Part II: Symmetry tools {#part-ii-symmetry-tools}


### 3. Lie Group Theory (66) {#3-dot-lie-group-theory--66}

<!--list-separator-->

-  Overview

    <!--list-separator-->

    -  The goal is to derive the (fundamental representations) of the (double cover) of the (Poincare group)

        <!--list-separator-->

        -  What is the Poincare group?

            <!--list-separator-->

            -  Rotations plus boosts plus translations = Lorentz group plus translations = Poincare group

        <!--list-separator-->

        -  What is a double cover?

        <!--list-separator-->

        -  What are fundamental representations?

    <!--list-separator-->

    -  We will always start with some known transformations, derive the Lie algebra and use this Lie algebra to get different representations of the symmetry transformations.

<!--list-separator-->

-  3.1 Groups

<!--list-separator-->

-  3.2 Rotations in two dimensions

    <!--list-separator-->

    -  \\(U(1)\\) and \\(SO(2)\\) are isomorphic descriptions of 2-dimensional rotations

    <!--list-separator-->

    -  3.2.1 Rotations with unit complex numbers

<!--list-separator-->

-  3.3 Rotations in three dimensions

    <!--list-separator-->

    -  The group \\(SO(3)\\) is described by 3-dimensional rotation matrices analogous to those for 2-dimensions. The corresponding second description requires a generalization of the complex numbers from 2 to higher dimensions. There are no 3-dimensional complex numbers but there are 4-dimensional ones called quaternions.

    <!--list-separator-->

    -  3.3.1 Quaternions

        <!--list-separator-->

        -  Three complex units \\(i,j,k\\) such that \\(i^2 = j^2 = k^2 = -1\\) and \\(ijk=-1\\)

        <!--list-separator-->

        -  Unit quaternions can be written as \\(2 \times 2\\) matrices with complex elements. For \\(q = a\mathbf{1} + b \mathbf{i} + c \mathbf{j} + d \mathbf{k}\\) the corresponding matrix is \\(( (a + d i, -b \* c i), (b \* c i, a -d i))\\) (interpreted as a list of rows)

        <!--list-separator-->

        -  A unit quaternion \\(u\\) does not induce a rotation on \\(v\\) by simple multiplication but rather the transformation \\(v' = q^{-1} v q\\) for a quaternion \\(q\\) is the correct means of encoding 3-dimensional rotations as quaternions.

        <!--list-separator-->

        -  \\(SU(2)\\) is the <span class="underline"><span class="underline">double-cover</span></span> of \\(SO(3)\\) . It is always possible to map elements of \\(SU(2)\\) to a single element of \\(SO(3)\\) unambiguously but the map in the other direction does not produce a unique element of \\(SU(2)\\) from each element of \\(SO(3)\\)

        <!--list-separator-->

        -  There is a means of using two copies of \\(SU(2)\\) to describe rotations in four dimensions

<!--list-separator-->

-  3.4 Lie Algebras

    <!--list-separator-->

    -  Overview

        <!--list-separator-->

        -  In contrast to discrete groups, continuous groups have elements that are arbitrarily close to the identity

            <!--list-separator-->

            -  For group identity \\(I\\), generator \\(X\\), and small parameter \\(\epsilon\\), \\(g(\epsilon) = I + \epsilon X\\) where \\(g(\epsilon)\\) is within \\(\epsilon X\\) of the identity element of the group \\(I\\)

            <!--list-separator-->

            -  \\(h(\theta) = (I+\epsilon X)^k = \lim\_{N \rightarrow \infty} (I+ \frac{\theta}{N} X)^N = e^{\theta X}\\)

            <!--list-separator-->

            -  The form of the generator \\(X\\) is given via a Taylor series expansion about the identity, \\(I\\), of an arbitrary continuously parameterized group element \\(h(\theta)\\)

                <!--list-separator-->

                -  \\(h(\theta) = \sum\_n \frac{d^n h}{d \theta^n} \vert\_{\theta=0} \theta^n = e^{\frac{dh}{d \theta} \vert\_{\theta=0} \theta}\\)

                <!--list-separator-->

                -  \\(X = \frac{dh}{d \theta}\vert\_{\theta=0}\\)

        <!--list-separator-->

        -  For matrix Lie groups, such as \\(G\\), the corresponding Lie algebra, \\(\mathfrak{g}\\), is the collection of objects that give an element of the group when exponentiated

            <!--list-separator-->

            -  \\(X \in \mathfrak{g} \Leftrightarrow e^{tX} \in G\\)

        <!--list-separator-->

        -  The composition rule of the Lie algebra is given by the Baker-Campbell-Hausdorff formula

            <!--list-separator-->

            -  \\(e^X \circ e^Y = e^{X+Y+\frac{1}{2}[X,Y] +\frac{1}{12}[X,[X,Y]]-\frac{1}{12}[Y,[X,Y]]+\cdots}\\)

            <!--list-separator-->

            -  This is where the <span class="underline"><span class="underline">Lie bracket</span></span> enters: the operation defined by \\([ , ]\\) is given, for matrix Lie groups, by \\([X,Y] = XY \* YX\\)

            <!--list-separator-->

            -  Thus the group operation under which the Lie algebra is closed is the Lie bracket \\([ , ]\\) as opposed to matrix multiplication or some other operation

        <!--list-separator-->

        -  The modern definition of a Lie algebra depends upon the behavior of the generators under the Lie bracket. Different groups may have the same Lie algebra. There is, however, exactly one distinguished Lie group for each Lie algebra. This is followed up in section 3.4.2.

    <!--list-separator-->

    -  3.4.1 The generators and Lie algebra of \\(SO(3)\\)

        <!--list-separator-->

        -  Example of how one can derive the Lie algebra of a given group

        <!--list-separator-->

        -  Defining constraints of \\(SO(3)\\) are \\(O^T O = I\\) and \\(\det(O) = 1\\)

        <!--list-separator-->

        -  The group elements, \\(O\\), can be written in terms of a generator \\(J\\) as $ O = e<sup>&Phi; J</sup>$

        <!--list-separator-->

        -  In terms of the constraints this is \\(O^T O = I \Rightarrow J^T + J =0\\) and \\(\det(O) = 1 \Rightarrow \mathrm{tr}(J) = 0\\) (using the fact that \\(\det (e^A) = e^{\mathrm{tr} (A)}\\))

        <!--list-separator-->

        -  This leaves \\((J\_i)\_{jk} = -\epsilon\_{ijk}\\) in terms of the Levi-Civita symbol

        <!--list-separator-->

        -  We can refer to the Lie bracket relation of the basis generators as the Lie algebra

            <!--list-separator-->

            -  \\([J\_i , J\_j] = \epsilon\_{ijk} J\_k\\) (for anti-Hermitian generators with complex eigenvalues)

            <!--list-separator-->

            -  \\([J\_i , J\_j] = i \epsilon\_{ijk} J\_k\\) (for Hermitian generators with real eigenvalues)

    <!--list-separator-->

    -  3.4.2 The abstract definition of a Lie algebra

        <!--list-separator-->

        -  Recall bilinearity, anticommutativity and the Jacobi identity

        <!--list-separator-->

        -  The definition of a Lie algebra requires no reference to any Lie group

    <!--list-separator-->

    -  3.4.3 The generators and Lie Algebra of \\(SU(2)\\)

        <!--list-separator-->

        -  \\(SU(2)\\) is the group of unitary \\(2 \times 2\\) matrices with unit determinant

            <!--list-separator-->

            -  Unitarity: \\(U^{\dagger} U = U U^{\dagger} = 1\\)

            <!--list-separator-->

            -  Unit determinant: \\(\det(U) = 1\\)

        <!--list-separator-->

        -  Imposing the conditions on the generatiors \\(J\_1, J\_2, \ldots\\)

            <!--list-separator-->

            -  Unitarity implies Hermitian: $J\_i<sup>&dagger;</sup> = J\_i $

            <!--list-separator-->

            -  Unit determinant implies tracelss: \\(\mathrm{tr} (J\_i) = 0\\)

            <!--list-separator-->

            -  The generators are thus traceless, Hermitian \\(2 \times 2\\) matrices called the Pauli matrices (usually written as \\(\sigma\_1, \sigma\_2, \sigma\_3\\))

        <!--list-separator-->

        -  For \\(J\_i = \frac{1}{2} \sigma\_i\\) the Lie algebra as given by the Lie bracket relation of the basis generators

            <!--list-separator-->

            -  \\([J\_i, J\_j] = i \epsilon\_{ijk} J\_k\\)

        <!--list-separator-->

        -

    <!--list-separator-->

    -  3.4.4 The abstract definition of a Lie group

        <!--list-separator-->

        -  A Lie group is a group that is also a differentiable manifold and whose group operation induces a differentiable map of the manifold into itself

        <!--list-separator-->

        -  There is precisely one simply-connected Lie group corresponding to each Lie algebra. Furthermore this simply-connected group is distinguished by the fact that there are structure-preserving maps ****to**** all other groups that share its Lie algebra but not in the opposite direction

        <!--list-separator-->

        -  The distinguished simply-connected Lie group for a given Lie algebra is called the ****covering group****

        <!--list-separator-->

        -  Example: There is a two-to-one map from \\(SU(2)\\) to \\(SO(3)\\) that identifies two points of \\(SU(2)\\) which is the 3-sphere with one point of \\(SO(3)\\) which is the hemi-3-sphere

        <!--list-separator-->

        -  To describe elementary particles one uses the representations of the covering group of the Poincare group instead of just the usual representation one uses to transform four-vectors.

        <!--list-separator-->

        -  We are able to derive the representations of the most fundamental group belonging to a given Lie algebra by deriving representations of the Lie algebra and then placing the generators into the exponential function to get matrices representing group elements

<!--list-separator-->

-  3.5 Representation theory

    <!--list-separator-->

    -  A representation is a map between any group element \\(g\\) of a group \\(G\\) and a linear transformation \\(R(g)\\) of some vector-space \\(V\\) in such a way that the group properties are perserved

    <!--list-separator-->

    -  Similarity transformation

        <!--list-separator-->

        -  \\(R \rightarrow R' = S^{-1} R S\\)

    <!--list-separator-->

    -  Invariant subspace

        <!--list-separator-->

        -  \\(V' \subseteq V\\) is an invariant subspace if for \\(v \in V'\\) we have \\(R(g) v \in V'\\) for all \\(g \in G\\)

    <!--list-separator-->

    -  A subrepresentation of \\(R\\), \\(R'\\), of \\(G\\) on \\(V'\\) is given by \\(R'(g) v = R(g) v\\) for all \\(v \in V'\\)

    <!--list-separator-->

    -  An irreducible representation is a representation of a group \\(G\\) on a vector space \\(V\\) that has no invariant subspaces besides \\(0\\) and \\(V\\). These representations are fundamental in the sense that they are not made up of smaller subrepresentations. Moreover all other representations are constructed from irreducible representations.

    <!--list-separator-->

    -  A Casimir element \\(C\\) is built from generators of the Lie algebra such that it commutes with every generator \\(X\\) of the group (i.e. \\([C,X]=0\\))

        <!--list-separator-->

        -  Schur's lemma says that for an irreducible representation \\(R \colon \mathfrak{g} \rightarrow \mathrm{GL}(V)\\) any linear operator \\(T \colon V \rightarrow V\\) that commutes with all operators \\(R(X)\\) must be a scalar multiple of the identity operator.

        <!--list-separator-->

        -  Casimir elements thus give linear operators with constant values for each representation, which provides a natural way of labelling representations.

    <!--list-separator-->

    -  For any Lie group, one or more of the generators can be diagonalized using similarity transformations. These diagonalized generators have eigenvectors that form the basis for the vector space associated to the representation. The set of diagonal generators is called the Cartan subalgebra and the corresponding generators Cartan generators.

        <!--list-separator-->

        -  The eigenvalues of Cartan generators are used to give charge labels to elementary particles

        <!--list-separator-->

        -  For \\(SU(3)\\) there are two Cartan generators associated to the strong interactions

        <!--list-separator-->

        -  For \\(SU(2)\\) there is one Cartan generator associated to weak interactions

<!--list-separator-->

-  3.6 SU(2)

    <!--list-separator-->

    -  3.6.1 The finite-dimensional irreducible representations of SU(2)

        <!--list-separator-->

        -  It is convenient to define ****ladder operators**** as linear combinations of \\(J\_1\\) and \\(J\_2\\)

            <!--list-separator-->

            -  \\(J\_+ = \frac{1}{\sqrt{2}} (J\_1 + i J\_2)\\)

            <!--list-separator-->

            -  \\(J\_\* = \frac{1}{\sqrt{2}} (J\_1 \* i J\_2)\\)

        <!--list-separator-->

        -  The set of generators of \\(SU(2)\\) given by \\(\\{J\_+, J\_-, J\_3 \\}\\) satisfies

            <!--list-separator-->

            -  \\([J\_3, J\_{\pm}] = \pm J\_{\pm}\\)

            <!--list-separator-->

            -  \\([J\_+, J\_-] = J\_3\\)

        <!--list-separator-->

        -  The maximum eigenvalue of \\(J\_3\\) is \\(j := b + N\\)

        <!--list-separator-->

        -  The minimum eigenvalue is \\(j \* M\\)

        <!--list-separator-->

        -  In general there are \\(2j + 1\\) eigenstates with eigenvalues \\(\\{-j, -j+1, \ldots, j-1, j\\}\\) which is only possible if \\(j\\) is an integer or half-integer

        <!--list-separator-->

        -  Representations of \\(SU(2)\\) on a $2 j + 1$-dimensional vector space \\(V\_j\\) with eigenvectors \\(v\_k\\) of \\(J\_3\\) contain all irreducible representations of \\(SU(2)\\)

    <!--list-separator-->

    -  3.6.2 The Casimir operator of SU(2)

        <!--list-separator-->

        -  Recall that a Casimir operator \\(C\\) is a function of the group generators and for all generators \\(X\\), \\([C,X] = 0\\)

        <!--list-separator-->

        -  \\(SU(2)\\) has one Casimir operator \\(J^2 := (J\_1)^2 + (J\_2)^2 + (J\_3)^2\\) which satisfies the condition \\([J^2, J\_i] = 0\\)

        <!--list-separator-->

        -  In terms of the ladder operators \\(J\_{\pm}\\), \\(J^2 = J\_+ J\_\* + J\_\* J\_+ +(J\_3)^2\\)

        <!--list-separator-->

        -  \\(J^2 v\_k = j(j+1)v\_k\\)

    <!--list-separator-->

    -  3.6.3 The representation of SU(2) in one dimension

        <!--list-separator-->

        -  The representation is trivial for the case \\(j=0\\) which corresponds to a 1-dimensional vector space and the \\(1 \times 1\\) matrices satisfying the commutations relations are trivially \\(0\\).

    <!--list-separator-->

    -  3.6.4 The representation of SU(2) in two dimensions

        <!--list-separator-->

        -  For \\(j=\frac{1}{2}\\) the representation is 2-dimensional and the generator \\(J\_3\\) has eigenvalues \\(\frac{1}{2}\\) and \\(-\frac{1}{2}\\)

        <!--list-separator-->

        -  The corresponding eigenvectors are \\(v\_{\frac{1}{2}} = (1 \; 0)^T\\) and \\(v\_{-\frac{1}{2}} = (0 \; 1)^T\\)

        <!--list-separator-->

        -

    <!--list-separator-->

    -  3.6.5 The representation of SU(2) in three dimensions

        <!--list-separator-->

        -  For three dimensions the eigenvalues of \\(J\_3\\) must be \\(\\{1, 0, -1\\}\\)

<!--list-separator-->

-  3.7 The Lorentz Group O(1,3)

    <!--list-separator-->

    -  Overview

        <!--list-separator-->

        -  The well-known vector representation of the Lorentz group by 4x4 matrices acting on four vectors is unable to describe physical systems that nevertheless can be described by alternative representations

        <!--list-separator-->

        -  The previous fact ultimately justifies the introduction and use of Lie theory. Lie theory enables the identification of the hidden abstract structure of a symmetry and using the language revealed there we are able to describe fundamental phenomena that we observe in nature

        <!--list-separator-->

        -  The Lorentz group is the set of all transformations that preserve the inner product of Minkowski space.

            <!--list-separator-->

            -  For example, the group \\(O(4)\\) preserves \\((x^0)^2 + (x^1)^2 + (x^2)^2 + (x^3)^2\\)

            <!--list-separator-->

            -  The inner product of Minkowski space is \\(x^{\mu} x\_{\mu} = x^{\mu} \eta\_{\mu \nu} x^{\nu} = (x^0)^2 \* (x^1)^2 \* (x^2)^2 \* (x^3)^2\\)

                <!--list-separator-->

                -  recall that \\(\eta\_{\mu \nu}\\) is the metric of Minkowski space given by \\(\mathrm{diag} (1, -1, -1 , -1)\\)

            <!--list-separator-->

            -  The Lorentz group is thus referred to as \\(O(1,3)\\) to denote that it provides symmetries for Minkowski space whose metric has 1 positive and 3 negatives along the diagonal

                <!--list-separator-->

                -  Lorentz transformations are conventionally referred to as \\(\Lambda\\)

            <!--list-separator-->

            -  The Lorentz transformations are defined by their preservation of the Minkowski metric

                <!--list-separator-->

                -  \\(\Lambda^{\sigma}\_{\mu} \eta\_{\sigma \rho} \Lambda^{\rho}\_{\nu} = \eta\_{\mu \nu}\\) in index notation

                <!--list-separator-->

                -  \\(\Lambda^T \eta \Lambda = \eta\\) in matrix notation

                <!--list-separator-->

                -  \\(\det(\Lambda)^2 = 1 \Rightarrow \det(\Lambda) = \pm 1\\)

            <!--list-separator-->

            -  The proper orthochronous Lorentz group, $SO(1,3)^&uarr; $ preserves the orientation of the coordinate system and the direction of time

            <!--list-separator-->

            -  The parity operator \\(\Lambda\_P\\) provides reflections and the time-reversal operator \\(\Lambda\_T\\) reverses time

            <!--list-separator-->

            -  The complete Lorentz group \\(O(1,3)\\) is given by

                <!--list-separator-->

                -  $O(1,3) = \\{ SO(1,3)^&uarr;, &Lambda;\_P SO(1,3)^&uarr;, &Lambda;\_T SO(1,3)^&uarr;, &Lambda;\_P &Lambda;\_T SO(1,3)^&uarr; \\} $

                <!--list-separator-->

                -  This is to say that beginning with the proper orthochronous subgroup of the Lorentz group, we can access the other components via reflection, time-reversal, and the combination of reflection with time-reversal respectively comprising the four components

            <!--list-separator-->

            -  Any representation of the Lorentz group can be found via representations of the proper orthochronous Lorentz group, $SO(1,3)^&uarr; $, the parity operator, and the time-reversal operator.

    <!--list-separator-->

    -  3.7.1 One representation of the Lorentz group

        <!--list-separator-->

        -  A 4x4 matrix has 16 parameters

        <!--list-separator-->

        -  The defining condition of the Lorentz group contains 10 constraints restricting the number of free parameters of a 4x4 representation of the Lorentz group to 6

            <!--list-separator-->

            -  Put a generic 4x4 matrix \\(\Lambda\\) into the equations given by \\(\Lambda^T \eta \Lambda = \eta\\)

        <!--list-separator-->

        -  If we find 6 linearly independent generators, that specifically satisfy the conditions then we have a complete Lie algebra for the Lorentz group

        <!--list-separator-->

        -  Example: solve for the generators of boosts along the \\(x, y\\), and \\(z\\) axes and then exponentiate to produce representations of the corresponding Lorentz transformations

        <!--list-separator-->

        -  The \\(J\_i\\) generators of spatial rotations only are equivalent for \\(O(3)\\) and $SO(1,3)^&uarr; $ . The \\(K\_i\\) provide generators for the transformations that simultaneously involve space and time called ****boosts****

    <!--list-separator-->

    -  3.7.2 Generators of the other components of the Lorentz group

        <!--list-separator-->

        -  In the previous section we completed the description of the first component of the set $O(1,3) = \\{ SO(1,3)^&uarr;, &Lambda;\_P SO(1,3)^&uarr;, &Lambda;\_T SO(1,3)^&uarr;, &Lambda;\_P &Lambda;\_T SO(1,3)^&uarr; \\} $ by combining the generators of spatial rotations \\(J\_i\\) with the boosts \\(K\_i\\)

        <!--list-separator-->

        -  The generators of the remaining components of the Lorentz group only require acting on these with the parity operation \\(\Lambda\_P\\) and \\(\Lambda\_T\\) on the matrices \\(J\_i\\) and \\(K\_i\\)

        <!--list-separator-->

        -  Under parity transformation \\(J\_i \rightarrow J\_i\\) and \\(K\_i \rightarrow -K\_i\\)

        <!--list-separator-->

        -  Under time-reversal transformation we arrive at the same result \\(J\_i \rightarrow J\_i\\) and \\(K\_i \rightarrow -K\_i\\)

    <!--list-separator-->

    -  3.7.3 The Lie Algebra of the proper orthochronous Lorentz group

        <!--list-separator-->

        -  The Lie algebra is given by the commutators of the generators derived in the previous sections

            <!--list-separator-->

            -  \\([J\_i, J\_j] = i \epsilon\_{ijk} J\_k\\)

            <!--list-separator-->

            -  \\([J\_i, K\_j] = i \epsilon\_{ijk} K\_k\\)

            <!--list-separator-->

            -  \\([K\_i, K\_j] = -i \epsilon\_{ijk} J\_k\\)

        <!--list-separator-->

        -  A general Lorentz transformation is given by \\(\Lambda = e^{i J \theta + iK \Phi}\\)

        <!--list-separator-->

        -  Note that the two generator types, \\(J\_i\\) and \\(K\_i\\) of rotations and boosts respectively, do not commute with each other. The rotation generators are closed under commutation. The boost generators are not closed under commutation.

        <!--list-separator-->

        -  New operators that are both closed under commutation and commute with each other are

            <!--list-separator-->

            -  \\(N\_i^{\pm} = \frac{1}{2} (J\_i \pm i K\_i)\\)

            <!--list-separator-->

            -  The following are the commutation relations associated with the operators \\(N\_i\\)

                <!--list-separator-->

                -  \\([N\_i^+, N\_j^+] = i \epsilon\_{ijk} N\_k^+\\)

                <!--list-separator-->

                -  \\([N\_i^-, N\_j^-] = i \epsilon\_{ijk} N\_k^-\\)

                <!--list-separator-->

                -  \\([N\_i^+, N\_j^-] = 0\\)

            <!--list-separator-->

            -  These correspond to two copies of the Lie algebra of \\(SU(2)\\): one for each of \\(N\_i^+\\) and \\(N\_i^-\\)

        <!--list-separator-->

        -  The Lie algebra of \\(SO(1,3)\_+^{\uparrow}\\) thus consists of two copies of the Lie algebra of \\(SU(2)\\)

        <!--list-separator-->

        -  Deriving irreducible representations of the Lie algebra of the Lorentz group gives irreducible representations of the covering group of the Lorentz group

        <!--list-separator-->

        -  The covering group of the Lorentz group is \\(SL(2,C)\\) which is the set of 2x2 matrices with unit determinant and complex entries

        <!--list-separator-->

        -  Since each irreducible representation of the Lie algebra of \\(SU(2)\\) can be labelled by the scalar value \\(j\\) of the Casimir operator of \\(SU(2)\\) and since the Lie algebra of the covering group of the Lorentz group consists of two copies of \\(SU(2)\\) then we can label representations of the latter by \\((j\_1, j\_2)\\).

        <!--list-separator-->

        -  The Lorentz algebra can be written compactly in terms of \\(M\_{\mu \nu}\\)

            <!--list-separator-->

            -  \\(J\_i = \frac{1}{2} \epsilon\_{ijk} M\_{jk}\\)

            <!--list-separator-->

            -  \\(K\_i = M\_{0i}\\)

            <!--list-separator-->

            -  \\([M\_{\mu \nu}, M\_{\rho \sigma}] = i(\eta\_{\mu \rho} M\_{\nu \sigma} \* \eta\_{\mu \sigma} M\_{\nu \rho} \* \eta\_{\nu \rho} M\_{\mu \sigma} + \eta\_{\nu \sigma} M\_{\mu \rho})\\)

    <!--list-separator-->

    -  3.7.4 The (0,0) representation

        <!--list-separator-->

        -  \\(N\_i^+ = N\_i^\* =0 \rightarrow e^{N\_i^+} = e^{N\_i^-} = e^0 = 1\\)

        <!--list-separator-->

        -  The \\((0,0)\\) representation of the Lorentz group acts on objects that do not change under Lorentz transformations and this representation is called the ****Lorentz scalar representation****

    <!--list-separator-->

    -  3.7.5 The (1/2, 0) representation

        <!--list-separator-->

        -  Generators

            <!--list-separator-->

            -  \\(N\_i^+ = \frac{\sigma\_i}{2} = iK\_i\\)

            <!--list-separator-->

            -  \\(N\_i^\* = \frac{1}{2}(J\_i-iK\_i) = 0 \Longrightarrow J\_i = iK\_i\\)

            <!--list-separator-->

            -  \\(K\_i = \frac{-i}{2} \sigma\_i\\)

        <!--list-separator-->

        -  Group elements

            <!--list-separator-->

            -  Rotations

                <!--list-separator-->

                -  \\(R\_{\theta} = e^{i \vec{\theta} \vec{J}} = e^{i \vec{\theta} \frac{\vec{\sigma}}{2}}\\)

            <!--list-separator-->

            -  Boosts

                <!--list-separator-->

                -  \\(B\_{\theta} = e^{i \vec{\phi} \vec{K}} = e^{\vec{\phi} \frac{\vec{\sigma}}{2}}\\)

        <!--list-separator-->

        -  Writing the exponential function as a series expansion and substituting the explicit matrix forms of the Pauli matrices gives ****explicit representations of the group elements**** in terms of ****2x2 complex matrices****. Note the fact that the ****2x2 complex**** nature of this representation also implies that it acts on two-component objects called ****left-chiral [spinors]({{< relref "spinors" >}})**** which can be shown to correspond to ****spin-up**** and ****spin-down**** states

        <!--list-separator-->

        -  The fact that they are the objects that transform under the \\((\frac{1}{2}, 0)\\) representation of the Lorentz group can be taken as defining the left-chiral [spinors]({{< relref "spinors" >}})

            <!--list-separator-->

            -  \\(\chi\_L = ( (\chi\_L)\_1 , (\chi\_L)\_2 )^T\\)

            <!--list-separator-->

            -  Note the distinguishing feature that arises from the presence of the \\(\frac{1}{2}\\) factor in the exponent stretches the usual \\(2 \pi\\) rotation into one of angle \\(4 \pi\\) which diverges from the usual period of rotation of a vector returning to its original position after a \\(2 \pi\\) rotation leading to the identification of \\(0\\) and \\(2 \pi\\).

    <!--list-separator-->

    -  3.7.6 The (0, 1/2) representation

        <!--list-separator-->

        -  This is precisely analogous to the previous section

        <!--list-separator-->

        -  Group elements

            <!--list-separator-->

            -  Rotations

                <!--list-separator-->

                -  \\(R\_{\theta} = e^{i \vec{\theta} \vec{J}} = e^{i \vec{\theta} \frac{\vec{\sigma}}{2}}\\)

            <!--list-separator-->

            -  Boosts

                <!--list-separator-->

                -  \\(B\_{\theta} = e^{i \vec{\phi} \vec{K}} = e^{\* \vec{\phi} \frac{\vec{\sigma}}{2}}\\)

        <!--list-separator-->

        -  Note that rotations are equivalent but boosts contain a minus sign in the exponent leading to the definition of the ****right-chiral [spinors]({{< relref "spinors" >}})****

            <!--list-separator-->

            -  \\(\chi\_R = ( (\chi\_R)\_1 , (\chi\_R)\_2 )^T\\)

        <!--list-separator-->

        -  Together the objects that transform under the \\((0, \frac{1}{2})\\) and \\((\frac{1}{2}, 0)\\) representations of the Lorentz group are called ****Weyl [spinors]({{< relref "spinors" >}})****

    <!--list-separator-->

    -  3.7.7 Van der Waerden notation

        <!--list-separator-->

        -  \\(\chi\_L = \chi\_a\\)

        <!--list-separator-->

        -  \\(\chi\_R = \chi^{\dot{a}}\\)

        <!--list-separator-->

        -  The so-called <span class="underline"><span class="underline">spinor metric</span></span> enables the transformation of a right-chiral spinor into a left-chiral one and vice versa

            <!--list-separator-->

            -  \\(\epsilon^{ab}  = ( (0, \; 1), \; (-1, \; 0))\\)

            <!--list-separator-->

            -  \\(\chi\_L^C \equiv \epsilon \chi\_L^{\star}\\) where \\(\star\\) denotes complex conjugation and \\(C\\) denotes <span class="underline"><span class="underline">charge conjugation</span></span>

                <!--list-separator-->

                -  It can be shown that, beginning with a left-chiral spinor \\(\chi\_L\\), a right chiral spinor can be generated by acting with the spinor metric and the resulting spinor is named \\(\chi\_L^C\\)

        <!--list-separator-->

        -  \\(\epsilon \chi\_L = \epsilon \chi\_a = \epsilon^{ac} \chi\_c = \chi^a\\)

        <!--list-separator-->

        -  \\(\epsilon \chi\_R = \epsilon \chi^{\dot{a}} = \epsilon\_{\dot{a} \dot{c}} \chi^{\dot{c}} = \chi\_{\dot{a}}\\)

        <!--list-separator-->

        -  \\(\chi\_R = \epsilon \chi\_L^\star\\)

        <!--list-separator-->

        -  \\(\chi\_L = \epsilon \chi\_R^\star\\)

        <!--list-separator-->

        -  The transformation behavior of a transposed spinor with lower, undotted index is exactly the opposite of a spinor with upper, undotted index

            <!--list-separator-->

            -  Terms of the form \\((\chi^a)^T \chi\_a\\) and \\((\chi^{\dot{a}})^T \chi\_{\dot{a}}\\) are invariant under Lorentz transformations

            <!--list-separator-->

            -  Terms combining left-chiral and right-chiral [spinors]({{< relref "spinors" >}}) are not Lorentz invariant

            <!--list-separator-->

            -  Terms involving the complex conjugate of a right-chiral spinor with a left-chiral spinor or terms involving the complex conjugate of a left-chiral spinor with right-chiral [spinors]({{< relref "spinors" >}}) are Lorentz invariant

        <!--list-separator-->

        -  We can write the two transformation operators as one object \\(\Lambda\\)

            <!--list-separator-->

            -  $&chi;\_R &rarr; &chi;'\_R = &Lambda;{<sup>\dot{a}</sup>}{<sub>\dot{b}</sub>} &chi;<sup>\dot{b}</sup> = \left( e^{i \vec{\theta} \frac{\vec{\sigma}}{2} \* \vec{\phi} \frac{\vec{\sigma}}{2} } \right)<sup>\dot{a}</sup><sub>\\;\\,\dot{b}</sub> &chi;<sup>\dot{b}</sup> $

            <!--list-separator-->

            -  $&chi;\_L &rarr; &chi;'\_L = &Lambda;{<sub>a</sub>}{<sup>b</sup>} &chi;<sub>b</sub> = \left( e^{i \vec{\theta} \frac{\vec{\sigma}}{2} + \vec{\phi} \frac{\vec{\sigma}}{2} } \right)<sub>a</sub><sup>\\;\\,b</sup> &chi;<sub>b</sub> $

            <!--list-separator-->

            -  \\(\Lambda\_{(\frac{1}{2},0)} = \Lambda{\_{a}}{^{b}}\\)

            <!--list-separator-->

            -  \\(\Lambda\_{(0,\frac{1}{2})} = \Lambda{^{\dot{a}}}{\_{\dot{b}}}\\)

    <!--list-separator-->

    -  3.7.8 The (1/2, 1/2) representation

        <!--list-separator-->

        -  This is the vector representation

        <!--list-separator-->

        -  A 4-vector is a rank-2 spinor

        <!--list-separator-->

        -  A spinor with 2 indices that transforms according to this representation

        <!--list-separator-->

        -  A rank-2 tensor has two vector indices and a vector has two spinor indices. Therefore, the most basic object that can be Lorentz transformed is a spinor

    <!--list-separator-->

    -  3.7.9 [spinors]({{< relref "spinors" >}}) and parity

        <!--list-separator-->

        -  Nature isn't always symmetric under parity transformations

        <!--list-separator-->

        -  the \\((0,\frac{1}{2})\\) representation becomes the \\((\frac{1}{2}, 0)\\) representation and vice versa under parity transformations

        <!--list-separator-->

        -  A Dirac spinor combines two Weyl [spinors]({{< relref "spinors" >}}), a left-chiral (\\(\chi\_L\\)) and a right-chiral (\\(\xi\_R\\)) spinor, into a single object

            <!--list-separator-->

            -  \\(\Psi = ( \chi\_L, \xi\_R)^T = (\chi\_a, \xi^{\dot{a}})^T\\)

            <!--list-separator-->

            -  There is a special case called a Majorana spinor

                <!--list-separator-->

                -  \\(\Psi\_M = ( \chi\_L, \chi\_R)^T\\)

        <!--list-separator-->

        -  The Dirac and Majorana [spinors]({{< relref "spinors" >}}) are not 4-vectors because they transform according to the \\((\frac{1}{2}, 0) \oplus (0, \frac{1}{2})\\) whereas 4-vectors transform according to the \\((\frac{1}{2}, 0) \otimes (0, \frac{1}{2}) = (\frac{1}{2}, \frac{1}{2})\\) representation

        <!--list-separator-->

        -  Parity transformations convert \\((\frac{1}{2}, 0) \oplus (0, \frac{1}{2})\\) represented objects into \\((0, \frac{1}{2}) \oplus (\frac{1}{2}, 0)\\)

        <!--list-separator-->

        -  \\(\Psi \rightarrow \Psi^P \Rightarrow ( \chi\_L, \xi\_R)^T \rightarrow ( \xi\_R, \chi\_L)^T\\)

    <!--list-separator-->

    -  3.7.10 [spinors]({{< relref "spinors" >}}) and charge conjugation

        <!--list-separator-->

        -  The transformations that yield \\(\chi\_L \rightarrow \chi\_R\\) and \\(\xi\_R \rightarrow \xi\_L\\) are not part of the Lorentz group

        <!--list-separator-->

        -  \\(\Psi \rightarrow \Psi^C \Rightarrow ( \chi\_L, \xi\_R)^T \rightarrow ( \xi\_L, \chi\_R)^T\\)

        <!--list-separator-->

        -  This operator simultaneously flips all labels / properties we use to describe fundamental particles

    <!--list-separator-->

    -  3.7.11 Infinite-dimensional representations

        <!--list-separator-->

        -  Infinite-dimensional representations of the Lorentz group are required for the purpose of transforming physical fields

        <!--list-separator-->

        -  Finite-dimensional representations were shown to act on ****constant**** one, two, and four-component objects; however, since the fundamental objects in physics are changing in time, we need to understand how those dynamic objects transform

            <!--list-separator-->

            -  These fall into the class

                <!--list-separator-->

                -  \\(\Phi\_a \rightarrow \Phi'\_a = M\_{ab}(\Lambda) \Phi\_b\\)

        <!--list-separator-->

        -  When the object \\(\Phi\\) changes in space and time and is thus considered as a function of coordinates \\(\Phi(x)\\) (where \\(x\\) represents the four traditional spacetime coordinates) the impact of any given transformation on the coordinates, \\(x^\mu \rightarrow \Lambda^\mu\_\nu x^\nu\\), must be taken into account

            <!--list-separator-->

            -  \\(\Phi\_a(x) \rightarrow M\_{ab}(\Lambda) \Phi\_b (\Lambda x)\\)

            <!--list-separator-->

            -  Wigner convention: \\(\Phi\_a(x) \rightarrow M\_{ab}(\Lambda) \Phi\_b (\Lambda^{-1} x)\\)

        <!--list-separator-->

        -  The transformation will thus be separated into two parts

            <!--list-separator-->

            -  One part, given by one of the finite-dimensional representations, will act on the field in question itself, \\(\Phi\_a\\)

            <!--list-separator-->

            -  The other part will act on the coordinates as given by an infinite-dimensional vector space and thus this second part will require an infinite-dimensional representation

        <!--list-separator-->

        -  Infinite-dimensional representations of the Lorentz group are given by differential operators

            <!--list-separator-->

            -  \\(M^{\mathrm{inf}}\_{\mu \nu} = i(x^\mu \partial^\nu \* x^\nu \partial^\mu)\\)

            <!--list-separator-->

            -  \\(\Phi(\Lambda x) = e^{-i \frac{\omega^{\mu \nu}}{2} M^{\mathrm{inf}}\_{\mu \nu}} \Phi(x)\\)

        <!--list-separator-->

        -  The representation that combines the finite\* and infinite-dimensional representation of the generators \\(M\_{\mu \nu} = M^{\mathrm{fin}}\_{\mu \nu} + M^{\mathrm{inf}}\_{\mu \nu}\\) is called the <span class="underline"><span class="underline">field representation</span></span>

        <!--list-separator-->

        -

<!--list-separator-->

-  3.8 The Poincare Group

    <!--list-separator-->

    -  Rotations plus boosts plus translations = Lorentz group plus translations = Poincare group

    <!--list-separator-->

    -  Generators of the Poincare group are the generators of the Lorentz group ()\\(J\_i\\), \\(K\_i\\)) plus the generators of translations in Minkowski space \\(P\_μ\\).

    <!--list-separator-->

    -  It is useful to ****label**** the representations by using the ****fixed scalar values**** of the ****Casimir operators****. Recall that a Casimir operator is, of course, an operator that is constructed from generators such that it commutes with all other generators.

<!--list-separator-->

-  3.9 Elementary particles

    <!--list-separator-->

    -  The labels for the irreps of the Poincare group in mathematics correspond to the means by which elementary particles are labelled in physics

        <!--list-separator-->

        -  mass (m)

        <!--list-separator-->

        -  spin (j)

    <!--list-separator-->

    -  Other labels, called charges, follow from the <span class="underline"><span class="underline">internal symmetries</span></span>

    <!--list-separator-->

    -  Taken together all of these labels constitute what is considered to be a necessary and sufficient set to determine all information about all particles to describe their behaviors in all known conducted and presently conceivable experiments

        <!--list-separator-->

        -  mass and spin derive from the global invariance of physical laws to Poincare transformations

        <!--list-separator-->

        -  electric, weak, and strong charge derive from the internal symmetries of interactions

    <!--list-separator-->

    -  spin \\(0\\): described by a <span class="underline"><span class="underline">scalar</span></span> \\(\Phi\\) that transforms according to the \\((0,0)\\) spin \\(0\\) representation

        <!--list-separator-->

        -  Higgs particle

    <!--list-separator-->

    -  spin \\(\frac{1}{2}\\): described by <span class="underline"><span class="underline">spinor</span></span> \\(\Psi\\) that transforms according to the \\((\frac{1}{2}, 0) \oplus (0, \frac{1}{2})\\) spin \\(\frac{1}{2}\\) representation

        <!--list-separator-->

        -  electrons and quarks

    <!--list-separator-->

    -  spin \\(1\\): described by <span class="underline"><span class="underline">vector</span></span> \\(A\\) that transforms according to the \\((\frac{1}{2}, \frac{1}{2})\\) spin 1 representation or vector representation

        <!--list-separator-->

        -  photons

    <!--list-separator-->

    -  spin \\(2\\): graviton?

<!--list-separator-->

-  3.10 Appendix: Rotations in a complex vector space

    <!--list-separator-->

    -  \\(a \cdot a = (Ua) \cdot (Ua)\\) is the condition for a transformation of a complex vector space containing the arbitrary element \\(a\\) to preserve the inner product

    <!--list-separator-->

    -  Because of the fact that \\(a \cdot a = a^\dagger a\\) this implies that \\((Ua) \cdot (Ua) = a^\dagger U^\dagger U a = a^\dagger a\\) and for the last equality to hold then \\(U^\dagger U = 1\\). The \\(U\\) that satisfy the last statement of the criterion are called <span class="underline"><span class="underline">unitary</span></span>. This is the origin of the use of the word unitary in <span class="underline"><span class="underline">unitary groups</span></span>.

    <!--list-separator-->

    -  The <span class="underline"><span class="underline">special</span></span> unitary groups \\(SU(n)\\) additionally satisfy the criterion that \\(\mathrm{det}(U) = 1\\).

<!--list-separator-->

-  3.11 Appendix: Manifolds

    <!--list-separator-->

    -  A manifold is a set that can be given \\(n\\) independent coordinates in some neighborhood of any point

    <!--list-separator-->

    -  For spherical coordinates of the 2-sphere, we need at least two coordinate systems to cover the pole at \\(\phi=0\\) and the semicircle at \\(\theta = 0\\) or \\(2\pi\\).


### 4. The Framework (15) {#4-dot-the-framework--15}

<!--list-separator-->

-  Overview

    <!--list-separator-->

    -  We imagine we can get the correct equations of nature by extremizing (minimizing) something. What are the fundamental representations of a view of physical dynamics through the lens of optimization?

    <!--list-separator-->

    -  We don't attempt to answer such a broad question directly, but we can begin to work on ruling out candidates via the statement of justifiable constraints.

        <!--list-separator-->

        -  The statement of the optimization problem must yield <span class="underline"><span class="underline">equivalent laws of nature</span></span> in <span class="underline"><span class="underline">different reference frames</span></span>. This can be imposed via requiring invariance to Lorentz transformations.

            <!--list-separator-->

            -  This implies the object must be a scalar that transforms according to the \\((0,0)\\) representation of the Lorentz group

        <!--list-separator-->

        -  Given several equivalent statements of the optimization problem, we would prefer to select among the simplest

    <!--list-separator-->

    -  We find that the name of the optimization problem is the <span class="underline"><span class="underline">action</span></span>, which is the integral of the <span class="underline"><span class="underline">Lagrangian</span></span>. The Lagrangian assigns numbers to the various realizations of the temporal evolution of a system. The dynamical equations that emerge from extremization (minimization) of the Lagrangian are called the <span class="underline"><span class="underline">Euler-Lagrange equations</span></span>.

<!--list-separator-->

-  4.1 Lagrangian formalism

    <!--list-separator-->

    -  4.1.1 Fermat's principle

        <!--list-separator-->

        -  Light always chooses the path between two points in space that minimizes the time it takes to travel between them

            <!--list-separator-->

            -  let us refer to a general path as \\(q(t)\\)

        <!--list-separator-->

        -  Pierre de Maupertius

            <!--list-separator-->

            -  Whenever any action occurs in nature, the quantity of action employed by this change is the least possible

        <!--list-separator-->

        -  The (functional) action of path \\(q(t)\\)

            <!--list-separator-->

            -  \\(S\_{\mathrm{light}} [\mathbf{q}(t)] = \int dt\\)

            <!--list-separator-->

            -  Note that \\(S\\) is a function of a function, \\(\mathbf{q}(t)\\). This makes \\(S\\) a <span class="underline"><span class="underline">functional</span></span>

            <!--list-separator-->

            -  In order to extremize the functional, \\(S\\), we need to use the <span class="underline"><span class="underline">variational calculus</span></span>

    <!--list-separator-->

    -  4.1.2 Variational calculus \* the Basic idea

        <!--list-separator-->

        -  Extrema are characterized by the structure of their neighborhoods

        <!--list-separator-->

        -  Example extremum neighborhood of a function

            <!--list-separator-->

            -  \\(f(x) = 3x^2 + x\\)

            <!--list-separator-->

            -  Consider a point \\(x = a\\) and the neighborhood swept out by a small deviation from \\(a\\), \\(\epsilon\\), \\(f(a + \epsilon) = 3(a + \epsilon)^2 + (a + \epsilon)\\)

            <!--list-separator-->

            -  If \\(a\\) is a minimum, first order variations in \\(\epsilon\\) must vanish. Otherwise, \\(\epsilon < 0\\) would make \\(f(a+\epsilon) < f(a)\\) and then \\(a\\) would not be a true minimum

            <!--list-separator-->

            -  Collecting the terms that are linear in \\(\epsilon\\) and enforcing the constraint that they be equal to zero

                <!--list-separator-->

                -  \\(6a\epsilon + \epsilon = 0 \Rightarrow a = \* \frac{1}{6} = x\_{\mathrm{min}}\\)

        <!--list-separator-->

        -  \\(S[q(t)] = \int \mathcal{L} \, dt\\)

            <!--list-separator-->

            -  \\(\mathcal{L}\\) is the Lagrangian and it is generally a function of position and velocity, which may be written \\(\mathcal{L}(q(t), \partial\_t q(t))\\)

<!--list-separator-->

-  4.2 Restrictions

    <!--list-separator-->

    -  The lowest possible, non-trivial order derivative of a given theory is determined by the condition that the Lagrangian must be Lorentz invariant, because otherwise we would get different equations of motions for different frames of reference

    <!--list-separator-->

    -  Theories containing higher-order derivatives produce [Ostrogradsky instabilities](<https://en.wikipedia.org/wiki/Ostrogradsky%5Finstability>)

    <!--list-separator-->

    -  Locality alone only rules out an infinite number of derivatives. A non-local interaction is of the form \\(\Phi(x-h)\Phi(x)\\). The Taylor expansion of \\(\Phi(x-h)\\) contains an infinite series of derivatives of \\(\Phi\\) with respect to its coordinates, which demonstrates the first claim that locality rules out infinite derivation.

    <!--list-separator-->

    -  Lagrangians for particle theories involve solving for particle paths

    <!--list-separator-->

    -  Lagrangians for field theories involve solving for field configurations

    <!--list-separator-->

    -  For theories describing free non-interacting fields or particles, we must truncate non-linear terms at second order (i.e. we allow for the inclusion of \\(\Phi^0, \Phi^1, \Phi^2\\) but not higher order terms such as \\(\Phi^2 \partial\_\mu \Phi\\))

<!--list-separator-->

-  4.3 Particle theories vs field theories

    <!--list-separator-->

    -  Note that \\(\mathcal{L}\\) is used to refer to a particle theory Lagrangian and that \\(\mathscr{L}\\) is used to refer to a field theory Lagrangian

    <!--list-separator-->

    -  Particle theories

        <!--list-separator-->

        -  describe physical systems in terms of positions of particles depending on time \\(\vec{q} = \vec{q}(t)\\)

        <!--list-separator-->

        -  \\(\mathcal{L} = \mathcal{L} (\vec{q}, \partial\_t \vec{q}, t)\\)

        <!--list-separator-->

        -  Example: \\(\mathcal{L} = \frac{1}{2} m \dot{\vec{q}}^2\\)

    <!--list-separator-->

    -  Field theories

        <!--list-separator-->

        -  Instead of describing the locations of individual particles, field theories involve the action of fields \\(\Phi(\vec{x}, t)\\) on space and time

        <!--list-separator-->

        -  \\(\mathscr{L} = \mathscr{L}(\Phi(\vec{x}, t), \partial\_\mu \Phi(\vec{x},t), \vec{x})\\)

        <!--list-separator-->

        -  Example: \\(\mathscr{L} = \frac{1}{2} (\partial\_\mu \Phi \partial^\mu \Phi \* m^2 \Phi^2)\\) is the Lagrangian that leads to the Klein-Gordon equation

        <!--list-separator-->

        -  Field theories place space and time into a representation that does not distinguish between the two

        <!--list-separator-->

        -  For particle theories, the solutions of the equations of motion provide the correct paths of the particles that minimize the action functional from which they are derived.

        <!--list-separator-->

        -  For field theories, the solutions of the equations of motion provide the correct field configurations that minimize the action functional from which they are derived.

<!--list-separator-->

-  4.4 Euler-lagrange equation

    <!--list-separator-->

    -  Consider fixing the function \\(q(t) = a(t)\\) and varying it by a small amount \\(\epsilon(t)\\) at each point in time. We assume that \\(0 = \epsilon(t\_1) = \epsilon(t\_2)\\) as a means of fixing the boundaries \\(q(t\_1) = a(t\_1)\\) and \\(q(t\_2) = a(t\_2)\\)

    <!--list-separator-->

    -  For a particle theory, the Euler-Lagrange equation is \\(\frac{\partial \mathcal{L(q,\dot{q},t)}}{\partial q} \* \frac{d}{dt} \left( \frac{\partial \mathcal{L(q,\dot{q},t)}}{\partial \dot{q}} \right) = 0\\)

    <!--list-separator-->

    -  For a field theory we consider the Lagrangian density \\(\mathscr{L}\\) from which we derive the Lagrangian by integrating over all coordinates except for time

        <!--list-separator-->

        -  \\(\mathcal{L} = \int d^3 x \mathscr{L}(\Phi^i, \partial\_\mu \Phi^i)\\)

        <!--list-separator-->

        -  \\(S = \int dt \mathcal{L} = \int d^4 x \mathscr{L}(\Phi^i, \partial\_\mu \Phi^i)\\)

        <!--list-separator-->

        -  \\(\frac{\partial \mathscr{L}}{\partial \Phi^i} \* \partial\_\mu \left( \frac{\partial \mathscr{L}}{\partial (\partial\_\mu \Phi^i)} \right) = 0\\)

<!--list-separator-->

-  4.5 Noether's theorem

    <!--list-separator-->

    -  Overview

        <!--list-separator-->

        -  Each symmetry of the Lagrangian is directly related to one conserved quantity

        <!--list-separator-->

        -  Each of the natural quantities one might use to describe the physical world because they are invariant in time and thus one measurement is valid indefinitely are directly related to symmetries of the Lagrangian.

    <!--list-separator-->

    -  4.5.1 Noether's theorem for particle theories

        <!--list-separator-->

        -  The action is what needs to be invariant in order for the dynamics to stay the same

        <!--list-separator-->

        -  We can always add the total time derivative of an arbitrary function \\(G\\) to the Lagrangian without changing the action

            <!--list-separator-->

            -  \\(\delta S \rightarrow \delta S' = \delta S + \int\_{t\_1}^{t\_2} dt \frac{d}{dt} \delta G = \delta S + \frac{\partial G}{\partial q} \delta q \vert\_{t\_1}^{t\_2} = \delta S\\)

                <!--list-separator-->

                -  because we assume that \\(q\\) does not vary at the boundary implying \\(\delta q (t\_1) = \delta q(t\_2)=0\\)

            <!--list-separator-->

            -  This leads to the condition

                <!--list-separator-->

                -  \\(\delta \mathcal{L} = \frac{d G}{dt}\\) as opposed to \\(\delta \mathcal{L}=0\\)

        <!--list-separator-->

        -  It is possible to show using the preceding condition with the Euler-Lagrange equation there is a quantity conserved in time

            <!--list-separator-->

            -  \\(\frac{d}{dt} \left( \frac{\partial \mathcal{L}}{\partial \dot{q}} \delta q + G    \right) = 0\\)

            <!--list-separator-->

            -  so that if we define the term under the temporal derivative as \\(J\\) then \\(J\\) must be constant, thus conserved, since its derivative is zero

        <!--list-separator-->

        -  It is possible to show, for example, that conservation of momentum $\vec{p} = m \dot{\vec{q}} $ derives from the invariance to spatial translations $ \vec{q} &rarr; \vec{q}' = \vec{q} + \vec{a}$ of the Lagrangian \\(\mathcal{L} = \frac{1}{2} m \dot{\vec{q}}^2\\)

        <!--list-separator-->

        -  Invariance under rotations can be shown from the same Lagrangian to lead to conservation of angular momentum.

        <!--list-separator-->

        -  Invariance under time translations yields a conserved quantity called the Hamiltonian and corresponds to the conservation of total energy.

        <!--list-separator-->

        -  Invariance to boosts (momentum translation) corresponds to conservation of a lesser known quantity \\(J\_{\mathrm{boost}} = pt \* \frac{1}{2} mvt \* mq\\)

            <!--list-separator-->

            -  $ q &rarr; q + vt &rArr; m \dot{q} &rarr; m(\dot{q} + v)$

    <!--list-separator-->

    -  4.5.2 Noether's theorem for field theories \* spacetime symmetries

        <!--list-separator-->

        -  Overview

            <!--list-separator-->

            -  There are two kinds of symmetries

                <!--list-separator-->

                -  The Lagrangian can be invariant under spacetime transformations such as rotations

                <!--list-separator-->

                -  The field itself can be invariant to transformations. These are called <span class="underline"><span class="underline">internal symmetries</span></span>.

        <!--list-separator-->

        -  Observer \\(S'\\) sees field \\(\Psi'(x')\\) whereas observer \\(S\\) sees field \\(\Psi(x)\\).

        <!--list-separator-->

        -  Only the sum of the two conserved quantities that result from \\(x \rightarrow x'\\) and \\(\Psi \rightarrow \Psi'\\) is conserved

        <!--list-separator-->

        -  Symmetry for a field Lagrangian density implies

            <!--list-separator-->

            -  \\(\mathscr{L}(\Phi(x\_\mu), \partial\_\mu \Phi(x\_\mu), x\_\mu) = \mathscr{L}(\Phi'(x'\_\mu), \partial\_\mu \Phi'(x'\_\mu), x'\_\mu)\\)

            <!--list-separator-->

            -  \\(\delta \Phi = \epsilon\_{\mu \nu} S^{\mu \nu} \Phi(x) \* \frac{\partial \Phi(x)}{\partial x\_\mu} \delta x\_\mu\\)

        <!--list-separator-->

        -  Consideration of spacetime translations leads to the definition of the energy-momentum tensor

            <!--list-separator-->

            -  \\(T^{\nu}\_{\mu} = \frac{\partial \mathscr{L}}{\partial (\partial\_\nu \Phi)} \frac{\partial(\Phi)}{\partial x\_\mu} \* \delta^{\nu}\_{\mu} \mathscr{L}\\)

            <!--list-separator-->

            -  Application of the Euler-Lagrange equations for the Lagrangian density to its variation yields the continuity equation \\(\partial\_\nu T^{\nu}\_{\mu} = 0\\)

            <!--list-separator-->

            -  The invariance under spacetime translations ultimately yields both the conservation of total energy (for invariance to translations in the time component) and conservation of the total momentum (for invariance to translations in the spatial components)

                <!--list-separator-->

                -  \\(E = \int d^3 x T^0\_0\\)

                <!--list-separator-->

                -  \\(P\_i = \int d^3 x T^0\_i\\)

    <!--list-separator-->

    -  4.5.3 Rotations and boosts

        <!--list-separator-->

        -  Defining the Noether current in terms of the energy-momentum tensor \\((J^\nu)^{\sigma \mu} = T^{\mu \nu} x^\sigma \* T^{\sigma \nu} x^\mu\\) we have

            <!--list-separator-->

            -  \\(\partial (J^\nu)^{\sigma \mu} = 0\\)

        <!--list-separator-->

        -  These conditions lead to the conserved quantities of orbital angular momentum of the field

            <!--list-separator-->

            -  \\(L^i\_{\mathrm{orbit}} = \frac{1}{2} \epsilon^{ijk} Q^{jk} = \frac{1}{2} \epsilon^{ijk} \int d^3 x (T^{k0} x^j \* T^{j0} x^k)\\)

        <!--list-separator-->

        -  and another quantity

            <!--list-separator-->

            -  \\(Q^{0i} = \int d^3 x (T^{i0}x^0 \* T^{00}x^i)\\)

    <!--list-separator-->

    -  4.5.4 Spin

        <!--list-separator-->

        -  \\(\delta \Phi = \epsilon\_{\mu \nu} S^{\mu \nu} \Phi(x)\\)

        <!--list-separator-->

        -  recall that the finite-dimensional representations are responsible for mixing of the field components

        <!--list-separator-->

        -  The complete conserved quantity is

            <!--list-separator-->

            -  \\(L^i = \frac{1}{2} \epsilon^{ijk} Q^{jk} = \frac{1}{2} \epsilon^{ijk} \int d^3 x \left( \frac{\partial \mathscr{L}}{\partial (\partial\_0 \Phi)} S^{jk} \Phi(x) + (T^{k0} x^j \* T^{j0} x^k) \right)\\)

            <!--list-separator-->

            -  where \\(L\_i = L^i\_{\mathrm{spin}} + L^i\_{\mathrm{orbit}}\\)

            <!--list-separator-->

            -  The first part \\(L^i\_{\mathrm{spin}}\\) is thought of as form of <span class="underline"><span class="underline">internal</span></span> angular momentum

            <!--list-separator-->

            -  The orbital angular momentum describes how two or more particles revolve around each other whereas the internal angular momentum describes the <span class="underline"><span class="underline">spin</span></span> of a single particle

    <!--list-separator-->

    -  4.5.5 Noether's theorem for field theories \* internal symmetries

        <!--list-separator-->

        -  Internal symmetries are incredibly important for interacting field theories

        <!--list-separator-->

        -  \\(\Phi\_i \rightarrow \Phi'\_i = \Phi\_i + \delta \Phi\_i\\)

        <!--list-separator-->

        -  We get another quantity called Noether current \\(\partial\_\mu J^\mu = 0\\)

            <!--list-separator-->

            -  \\(J^\mu = \frac{\partial \mathscr{L}}{\partial (\partial\_\mu \Phi\_i)} \delta \Phi\_i\\)

            <!--list-separator-->

            -  The conserved quantity is \\(\partial\_t \int d^3 x J^0 = 0\\)

        <!--list-separator-->

        -  Invariance to displacements of the field itself given by \\(\Phi\_i \rightarrow \Phi'\_i = \Phi\_i \* i \epsilon\_i\\) with generators \\(-i\epsilon \frac{\partial}{\partial \Phi}\\) leads to the conservation of conjugate momentum \\(\Pi\\) with conjugate momentum density \\(\pi = J\_0 = \frac{\partial \mathscr{L}}{\partial (\partial\_0 \Phi)}\\) which is different from the physical momentum whose conservation derives from invariance under spatial translations

        <!--list-separator-->

        -

<!--list-separator-->

-  4.6 Appendix: conserved quantity from boost invariance for particle theories

<!--list-separator-->

-  4.7 Appendix: conserved quantity from boost invariance for field theories


## Part III: The equations of nature {#part-iii-the-equations-of-nature}


### 5. Measuring nature {#5-dot-measuring-nature}

<!--list-separator-->

-  Overview

    <!--list-separator-->

    -  Conserved quantities are what physicists commonly use to describe physical systems, because no matter how complicated the system changes, the conserved quantities stay the same.

<!--list-separator-->

-  5.1 The operators of quantum mechanics

    <!--list-separator-->

    -  \\([\hat{p\_i}, \hat{x\_j}] = i \delta\_{ij}\\)

    <!--list-separator-->

    -  5.1.1 Spin and angular momentum

        <!--list-separator-->

        -  orbital angular momentum is identified with the infinite dimensional representation of the generator

        <!--list-separator-->

        -  spin is identified with the finite dimensional representation of the generators

<!--list-separator-->

-  5.2 The operators of quantum field theory

    <!--list-separator-->

    -  Conjugate momentum density \\(\pi(x)\\) is identified with the generator of displacements of the field \\(-i \frac{\partial}{\partial \Phi(x)}\\)

    <!--list-separator-->

    -  \\([\Phi\_i(x), \pi\_j(y)] = i \delta(x-y) \delta\_{ij}\\)


### 6. Free Theory {#6-dot-free-theory}

<!--list-separator-->

-  Overview

    <!--list-separator-->

    -  Derive the equations for a physical theory of free <span class="underline"><span class="underline">(non-interacting) fields</span></span> <span class="underline"><span class="underline">from symmetry</span></span>

        <!--list-separator-->

        -  Derive the Klein-Gordon equation from the \\((0,0)\\) representation of the Lorentz group

        <!--list-separator-->

        -  Derive the Dirac equation using the \\((\frac{1}{2},0) \oplus (0, \frac{1}{2})\\) representation of the Lorentz group

        <!--list-separator-->

        -  Derive the Proca equation from the vector \\((\frac{1}{2}, \frac{1}{2})\\) representation of the Lorentz group (in the massless limit this reduces to Maxwell's equations)

<!--list-separator-->

-  6.1 Lorentz covariance and invariance

    <!--list-separator-->

    -  We require the equations of motion we derive for the standard model of particle physics to look the same in all inertial frames, because if this was not the case we would have a different equation for each possible frame of reference.

    <!--list-separator-->

    -  \\(A\_\mu \rightarrow A'\_\mu\\) is Lorentz covariant but \\(A\_1 + A\_3\\) is not

    <!--list-separator-->

    -  To make sure we only end up with Lorentz covariant equations, we require the action \\(S\\) to be Lorentz invariant.

<!--list-separator-->

-  6.2 Klein-Gordon equation

    <!--list-separator-->

    -  The simples case is that of scalars that transform according to the \\((0,0)\\) representation of the Lorentz group

    <!--list-separator-->

    -  A  general Lagrangian density compatible with the given restrictions of Lorentz invariance is

        <!--list-separator-->

        -  \\(\mathscr{L} = A \Phi^0 + B\Phi + C\Phi^2 + D \partial\_\mu \Phi + E \partial\_\mu \Phi \partial^\mu \Phi + F \Phi \partial\_\mu \Phi\\)

        <!--list-separator-->

        -  \\(S = \int d^Dx \,\, \mathscr{L}\\) where \\(d^D x\\) refers to integration over all \\(D\\) dimensions of spacetime. This is also written sometimes as \\(S = \int d^\mu x \,\, \mathscr{L}\\) or implicitly as \\(S = \int d x \,\, \mathscr{L}\\)

        <!--list-separator-->

        -  Lorentz invariance restricts the Lagrangian to be a scalar and therefore all odd powers in \\(\partial\_\mu\\) are forbidden (i.e. D=F=0).

        <!--list-separator-->

        -  Constants in the Lagrangian do not have an effect on the equations of motion derived from the Euler-Lagrange equations therefore A=0.

        <!--list-separator-->

        -  The impact of the linear term in the Lagrangian on the equations of motion derived from the Euler-Lagrange equations can be absorbed into a constant and so \\(B=0\\).

        <!--list-separator-->

        -  Taken together these constraints on the general Lagrangian density leaves

            <!--list-separator-->

            -  \\(\mathscr{L} = C \Phi^2 + E \partial\_\mu \Phi \partial^\mu \Phi\\)

            <!--list-separator-->

            -  In a free theory there are no non-linear terms involving distinct fields. The latter are taken to arise in the context of interactions leading to terms such as \\(\Phi\_1 \Phi\_2\\)

        <!--list-separator-->

        -  \\(C\\) and \\(E\\) are able to be combined into one constant. It is conventional to include a factor of \\(\frac{1}{2}\\) leading to the Lagrangian density

            <!--list-separator-->

            -  \\(\mathscr{L} = \frac{1}{2} (\partial\_\mu \Phi \partial^\mu \Phi \* m^2 \Phi^2)\\)

        <!--list-separator-->

        -  Placing this Lagrangian density into the Euler-Lagrange equation yields the equation of motion named the ****Klein-Gordon equation****

            <!--list-separator-->

            -  \\((\partial\_\mu \partial^\mu + m^2) \Phi = 0\\)

        <!--list-separator-->

        -  This equation describes free spin \\(0\\) fields or particles

    <!--list-separator-->

    -  6.2.1 Complex Klein-Gordon field

        <!--list-separator-->

        -  For spin \\(0\\) fields, we are able to construct a Lorentz-invariant Lagrangian without using the complex conjugate field. This does not work in the case of spin \\(\frac{1}{2}\\) fields \\(\Psi\\), which leads to the introduction of an antiparticle for each spin \\(\frac{1}{2}\\) particle that corresponds to a given field and its complex conjugate.

        <!--list-separator-->

        -  Including the complex conjugate of the spin \\(0\\) field in the Lagrangian is the same as considering two non-interacting scalar fields of equal mass.

        <!--list-separator-->

        -  The only known, experimentally-verified, spin \\(0\\) field is the Higgs field

    <!--list-separator-->

    -  The Klein-Gordon Lagrangian does not model any known physical field and therefore it is only used as a mathematical toy example

<!--list-separator-->

-  6.3 Dirac equation

    <!--list-separator-->

    -  We will use the \\((\frac{1}{2},0) \oplus (0, \frac{1}{2})\\) representation of the Lorentz group to find the equation of motion for free spin \\(\frac{1}{2}\\) fields or particles.

    <!--list-separator-->

    -  The objects transforming under this representation are called Dirac [spinors]({{< relref "spinors" >}}), which combine right-chiral and left-chiral [spinors]({{< relref "spinors" >}}) into one object

        <!--list-separator-->

        -  \\(\Psi = (\chi\_L, \xi\_R)^T = (\chi\_a, \xi^{\dot{a}})^T\\)

    <!--list-separator-->

    -  A general Lorentz-invariant Lagrangian density for Dirac [spinors]({{< relref "spinors" >}})

        <!--list-separator-->

        -  \\(\mathscr{L} = A \Psi^\dagger \gamma\_0 \Psi + B \Psi^\dagger \gamma\_0 \gamma^\mu \partial\_\mu \Psi\\)

        <!--list-separator-->

        -  It is common to see the introduction of a notation \\(\bar{\Psi} = \Psi^\dagger \gamma\_0\\) in which case \\(\mathscr{L} = A \bar{\Psi} \Psi + B \bar{\Psi} \gamma^\mu \partial\_\mu \Psi\\)

    <!--list-separator-->

    -  If we s set the constants \\(A = -m\\) and \\(B=i\\) we get the Dirac Lagrangian

        <!--list-separator-->

        -  \\(\mathscr{L} = -m \bar{\Psi} \Psi + i \bar{\Psi} \gamma^\mu \partial\_\mu \Psi = \bar{\Psi} (i \gamma^\mu \partial\_\mu -m)\Psi\\)

        <!--list-separator-->

        -  Note that there are two distinct fields. Though it could be written in terms of two real fields, \\(\Psi = \Psi\_1 + i\Psi\_2\\), it is more common to use two complex fields \\(\Psi\\) and \\(\bar{\Psi}\\)

    <!--list-separator-->

    -  Substituting into the Euler-Lagrange equation we get the equation of motion for each complex spinor field \\(\Psi\\) and \\(\bar{\Psi}\\)

        <!--list-separator-->

        -  \\((i \partial^\mu \bar{\Psi} \gamma\_\mu + m \bar{\Psi}) = 0\\)

        <!--list-separator-->

        -  \\((i \gamma\_\mu \partial^\mu -m) \Psi = 0\\)

<!--list-separator-->

-  6.4 Proca equation

    <!--list-separator-->

    -  We will use the vector \\((\frac{1}{2}, \frac{1}{2})\\) representation of the Lorentz group to find the equation of motion for spin 1 particles (both massive and massless)

    <!--list-separator-->

    -  \\(\mathscr{L}\_{\mathrm{Proca}} = C\_1 \partial^\mu A^\nu \partial\_\mu A\_\nu + C\_2 \partial^\mu A^\nu \partial\_\nu A\_\mu + C\_3 A^\mu A\_\mu + C\_4 \partial^\mu A\_\mu\\)

    <!--list-separator-->

    -  This yields the equations of motion

        <!--list-separator-->

        -  For massive spin 1: \\(m^2 A^\rho = \frac{1}{2} \partial\_\sigma(\partial^\sigma A^\rho \* \partial^\rho A^\sigma)\\)

        <!--list-separator-->

        -  For massless spin 1: \\(0 = \frac{1}{2} \partial\_\sigma(\partial^\sigma A^\rho \* \partial^\rho A^\sigma)\\)

        <!--list-separator-->

        -  These are the inhomogeneous Maxwell equations in the absence of electric currents

    <!--list-separator-->

    -  It is common to define the electromagnetic tensor

        <!--list-separator-->

        -  \\(F^{\sigma \rho} = \partial^\sigma A^\rho \* \partial^\rho A^\sigma\\)

    <!--list-separator-->

    -  In terms of this electromagnetic tensor the inhomogeneous Maxwell equations read

        <!--list-separator-->

        -  \\(\partial\_\rho F^{\sigma \rho} = 0\\)

    <!--list-separator-->

    -  Lagrangian for massless spin 1: \\(\mathscr{L}\_{\mathrm{Maxwell}} = \frac{1}{2} (\partial^\mu A^\nu \partial\_\mu A\_\nu \* \partial^\mu A^\nu \partial\_\nu A\_\mu) = \frac{1}{4} F^{\mu \nu} F\_{\mu \nu}\\)

    <!--list-separator-->

    -  Lagrangian for massive spin 1: \\(\mathscr{L}\_{\mathrm{Proca}} = \frac{1}{4} F^{\mu \nu} F\_{\mu \nu} + m^2 A\_\mu A^\mu\\)


### 7. Interaction theory {#7-dot-interaction-theory}

<!--list-separator-->

-  Summary

    <!--list-separator-->

    -  Local \\(U(1)\\) symmetry

        <!--list-separator-->

        -  \\(\mathscr{L} = m \bar{\Psi}\Psi + i \bar{\Psi} \gamma\_\mu \partial^\mu \Psi + A\_\mu \bar{\Psi} \gamma^\mu \Psi + \partial^\mu A^\nu \partial\_\mu A\_\nu \* \partial^\mu A^\nu \partial\_\nu A\_\mu\\)

    <!--list-separator-->

    -  Local \\(SU(2)\\) symmetry

        <!--list-separator-->

        -  Doublet \\(\bar{\Psi} = (\bar{\psi}\_1 \; \bar{\psi}\_2)\\) containing two spin \\(\frac{1}{2}\\) fields and three spin \\(1\\) fields \\(W^\mu\_j\\)

        <!--list-separator-->

        -  \\(\mathscr{L} = i \bar{\Psi} \gamma\_\mu \partial^\mu \Psi + \bar{\Psi} \gamma\_\mu \sigma\_j W^\mu\_j \Psi \* \frac{1}{4} (W\_{\mu \nu})\_i (W^{\mu \nu})\_i\\)

            <!--list-separator-->

            -  requires massless spin 1 and spin \\(\frac{1}{2}\\) fields

        <!--list-separator-->

        -  Experiments show the the spin 1 fields are not massless and that the electron mass is much bigger than the electron neutrino mass. The Higgs mechanism allows for the introduction of a locally \\(SU(2)\\) invariant Lagrangian that includes the necessary mass terms to match the theory to experiments.

    <!--list-separator-->

    -  Local \\(SU(3)\\) symmetry

        <!--list-separator-->

        -  Triplet \\(Q = (q\_1, \; q\_2 \; q\_3)^T\\) containing 3 spin \\(\frac{1}{2}\\) fields interpreted as quarks carrying color charge

        <!--list-separator-->

        -  The eight corresponding gluons are indeed massless which fits the theory

        <!--list-separator-->

        -  \\(\mathscr{L} = \* \frac{1}{4} F^A\_{\alpha \beta} F^{\alpha \beta}\_A + \bar{Q}(i D\_\mu \gamma^\mu \* m)Q\\)

<!--list-separator-->

-  7.1 U(1) interactions

    <!--list-separator-->

    -  7.1.1 internal symmetry of free spin \frac{1}{2} fields

    <!--list-separator-->

    -  The Lagrangian for a free spin \\(\frac{1}{2}\\) particle is

        <!--list-separator-->

        -  \\(\mathscr{L}\_{\mathrm{Dirac}} = -m \bar{\Psi} \Psi + i \bar{\Psi} \gamma^\mu \partial\_\mu \Psi = \bar{\Psi} (i \gamma^\mu \partial\_\mu -m)\Psi\\)

    <!--list-separator-->

    -  The Lagrangian is Lorentz invariant as required in the process of its derivation. However there is also a symmetry to field transformations

        <!--list-separator-->

        -  \\(\Psi \rightarrow \Psi' = e^{ia} \Psi\\)

        <!--list-separator-->

        -  \\(\bar{\Psi} \rightarrow \bar{\Psi}' = e^{-ia} \bar{\Psi}\\)

    <!--list-separator-->

    -  This forms the global internal \\(U(1)\\) symmetry. In its current form the Dirac Lagrangian is not locally \\(U(1)\\) invariant

        <!--list-separator-->

        -  $\mathscr{L'}<sub>\mathrm{Dirac}</sub> = -m \bar{\Psi} &Psi; + i \bar{\Psi} &gamma;\_&mu; &part;^&mu; &Psi; + i^2 (&part;^&mu; a(x)) \bar{\Psi} &gamma;\_&mu; &part;^&mu; &Psi; $

        <!--list-separator-->

        -

<!--list-separator-->

-  7.2 SU(2) interactions [progress indicators]({{< relref "progress_indicators" >}})

<!--list-separator-->

-  7.3 Mass terms and unification of SU(2) and U(1)

<!--list-separator-->

-  7.4 Parity violation

<!--list-separator-->

-  7.5 Lepton mass terms

<!--list-separator-->

-  7.6 Quark mass terms

<!--list-separator-->

-  7.7 Isospin

    <!--list-separator-->

    -  7.7.1 Labelling states

<!--list-separator-->

-  7.8 SU(3) interactions

<!--list-separator-->

-  7.9 The interplay between fermions and bosons


## Part IV: Applications {#part-iv-applications}


### 8. Quantum Mechanics {#8-dot-quantum-mechanics}

<!--list-separator-->

-  8.1 Particle theory identifications

<!--list-separator-->

-  8.2 Relativistic energy-momentum relation

<!--list-separator-->

-  8.3 The quantum formalism

<!--list-separator-->

-  8.4 The Schrodinger equation

    <!--list-separator-->

    -  Schrodinger equation with external field

<!--list-separator-->

-  8.5 From wave equations to particle motion

    <!--list-separator-->

    -  8.5.1 Example: free particle

    <!--list-separator-->

    -  8.5.2 Example: particle in a box

    <!--list-separator-->

    -  8.5.3 Dirac notation

    <!--list-separator-->

    -  8.5.4 Example: particle in a box, again

    <!--list-separator-->

    -  8.5.5 Spin

<!--list-separator-->

-  8.6 Heisenberg's uncertainy principle

<!--list-separator-->

-  8.7 Comments on interpretations

<!--list-separator-->

-  8.8 Appendix: Interpretation of the Dirac Spinor components

<!--list-separator-->

-  8.9 Appendix: Solving the Dirac equation

<!--list-separator-->

-  8.10 Appendix: Dirac [spinors]({{< relref "spinors" >}}) in different bases

    <!--list-separator-->

    -  8.10.1 Solutions of the Dirac equation in the mass basis


### 9. Quantum field theory {#9-dot-quantum-field-theory}

<!--list-separator-->

-  9.1 Field theory identifications

<!--list-separator-->

-  9.2 Free spin 0 field theory

<!--list-separator-->

-  9.3 Free spin \\(\frac{1}{2}\\) theory

<!--list-separator-->

-  9.4 Free spin \\(1\\) theory

<!--list-separator-->

-  9.5 Interacting field theory

    <!--list-separator-->

    -  9.5.1 Scatter amplitudes

    <!--list-separator-->

    -  9.5.2 Time evolution of states

    <!--list-separator-->

    -  9.5.3 Dyson series

    <!--list-separator-->

    -  9.5.4 Evaluating the series

<!--list-separator-->

-  9.6 Appendix: most general solution of the Klein-Gordon equation


### 10. Classical mechanics {#10-dot-classical-mechanics}

<!--list-separator-->

-  10.1 Relativistic mechanics

<!--list-separator-->

-  10.2 The Lagrangian of non-relativistic mechanics


### 11. Electrodynamics {#11-dot-electrodynamics}

<!--list-separator-->

-  11.1 The homogeneous Maxwell equations

<!--list-separator-->

-  11.2 The Lorentz force

<!--list-separator-->

-  11.3 Coulomb potential


### 12. Gravity {#12-dot-gravity}


### 13. Closing words {#13-dot-closing-words}


## Part V: Appendices {#part-v-appendices}


### A. Vector calculus {#a-dot-vector-calculus}


### B. Calculus {#b-dot-calculus}

<!--list-separator-->

-  B.5 Index notation

    <!--list-separator-->

    -  B.5.5 Important symbols

        <!--list-separator-->

        -  The Levi-Civita symbol is totally anti-symmetric

            <!--list-separator-->

            -  In four dimensions

                <!--list-separator-->

                -  \\(\epsilon\_{ijkl} = 1\\) if \\((i,j,k,l)\\) is an even permutation

                <!--list-separator-->

                -  \\(\epsilon\_{ijkl} = -1\\) if \\((i,j,k,l)\\) is an uneven permutation

                <!--list-separator-->

                -  \\(\epsilon\_{ijkl} = 0\\) otherwise

    <!--list-separator-->

    -


### C. Linear algebra {#c-dot-linear-algebra}


### D. Additional mathematical notions {#d-dot-additional-mathematical-notions}
