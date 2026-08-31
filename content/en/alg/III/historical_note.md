---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 0
section_title: Historical Note
kind: historical
lang: en
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 655-710
pdf_pages: 0679-0734
extraction: ocr
statements: 0
exercises: 0
content_sha256: 78bd01af38161bc2db08e20c490bf7e6e244d8a0155ef6b475f75af266d69127
---

# HISTORICAL NOTE

(Chapters II and III)

(N.B. Numbers in brackets refer to the bibliography at the end of this Note.)

Linear algebra is both one of the oldest and one of the newest branches of mathematics. On the other hand, at the origins of mathematics are the problems which are solved by a single multiplication or division, that is by calculating a value of a function $f(x) = ax$, or by solving an equation $ax = b$: these are typical problems of linear algebra and it is impossible to deal with them, indeed even to pose them correctly, without "thinking linearly".

On the other hand, not only these questions but almost everything concerning equations of the first degree had long been relegated to elementary teaching, when the modern development of the notions of field, ring, topological vector space, etc. came to isolate and emphasize the essential notions of linear algebra (for example duality); then the essentially linear character of almost the whole of modern mathematics was perceived, of which "linearization" is itself one of the distinguishing traits, and linear algebra was given the place it merits. To give its history, from our present point of view, would therefore be a task as difficult as it is important; and we must therefore be content to give a brief summary.

From the above it is seen that linear algebra was no doubt born in response to the needs of practical calculators; thus we see the rule of three† and the rule of false position, more or less clearly stated, playing an important role in all the manuals of practical arithmetic, from the Rhind papyrus of the Egyptians to those used in our primary schools, by way of Āryabhaṭa, the Arabs, Leonard of

† Cf. J. Tropfke, Geschichte der Elementar-Mathematik, 1. Band, 2te Ausgabe, Berlin-Leipzig (W. de Gruyter), 1921, pp. 150–155.

Pisa and the countless "calculation books" of the Middle Ages and the Renaissance; but they never constituted more than a small part, for the use of practical men, of the most advanced scientific theories.

As for mathematicians proper, the nature of their research on linear algebra depends on the general structure of their science. Ancient Greek mathematics, as expounded in the *Elements* of Euclid, developed two abstract theories of a linear character, on the one hand that of magnitudes ([2], Book V; cf. Historical Note to *General Topology*, IV) and on the other hand that of integers ([2], Book VII). With the Babylonians we find methods much more akin to our elementary algebra; they know how to solve, and most elegantly ([1], pp. 181–183), systems of equations of the first degree. For a very long time, nevertheless, the progress of linear algebra is mainly confined to that of algebraic calculations and they should be considered from this point of view, foreign to this Note; to reduce a linear system to an equation of the type $ax = b$, it suffices, in the case of a single unknown, to know the rules (already, in substance, stated by Diophantus) for taking terms from one side to the other and combining similar terms; and, in the case of several unknowns, it suffices to know also how to eliminate them successively until only one is left. Also the Treatises on algebra, until the XVIIIth century, think that all is accomplished as far as the first degree is concerned, when they have expounded these rules; as for a system of as many equations as unknowns (they do not consider others) where the left hand sides are not linearly independent forms, they are content to observe in passing that this indicates a badly posed problem. In the treatises of the XIXth century and even certain more recent works, this point of view is only modified by the progress of notation, which allows writing systems of $n$ equations in $n$ unknowns, and by the introduction of determinants which allow formulae of an explicit solution to be given in the "general case"; this progress, the credit for which would have belonged to Leibniz ([7], p. 239) had he developed and published his ideas on this subject, is mainly due to the mathematicians of the XVIIIth and early XIXth centuries.

But we must first study various currents of ideas which, much more than the study of linear equations, contributed to the development of linear algebra in the sense in which we understand it. Inspired by the study of Appollonius, Fermat [4(a)], having conceived, even before Descartes [5], the principle of analytic geometry, has the idea of classifying plane curves according to their degree (which, having become little by little familiar to all mathematicians, can be considered to have been definitely grasped towards the end of the XVIIth century) and formulates the fundamental principle that an equation of the first degree, in the plane, represents a line and an equation of the second degree a conic: a principle from which he deduces immediately some "very beautiful" consequences relating to geometric loci. At the same time, he enunciates [4(b)] the classification of problems into problems with a single solution, problems which reduce to an equation in two unknowns, an equation in three unknowns, etc.; and he adds: the first consist of determining a point, the second a line or plane locus, the others a surface, etc. ("... such a problem does not seek only a point or a line, but the whole of a surface appropriate to the question; here surfaces as loci have their genesis and similarly for the rest", loc. cit., p. 186; here already is the germ of n-dimensional geometry). This paper, formulating the principle of dimension in algebra and algebraic geometry, indicates a fusion of algebra and geometry in absolute conformity with modern ideas, but which, as has already been seen, took more than two centuries to penetrate into men's minds.

At least these ideas soon result in the expansion of analytic geometry which reaches its fulness in the XVIIIth century with Clairaut, Euler, Cramer, Lagrange and many others. The linear character of the formulae for transformation of coordinates in the plane and in space, which Fermat cannot have failed already to have perceived, is put in relief for example by Euler ([8(a)], Chapters II–III and Appendix to Chapter IV), who here lays the foundation of the classification of plane curves and that of surfaces according to their degree (invariant precisely because of the linearity of these formulae); he it is also (loc. cit., Chapter XVIII) who introduces the word "affinity" to describe the relation between curves which can be derived one from the other by a transformation $x' = ax, y' = by$ (but without perceiving anything geometrically invariant in this definition which remains bound to a particular choice of axes). A little later we see Lagrange [9(a)] devoting a whole memoir, which long remained justly famous, to typically linear and multilinear problems of analytic geometry in three dimensions. Around about this time, in relation to the linear problem constituted by the search for a plane curve passing through given points, the notion of determinant takes shape, first in a somewhat empirical way, with Cramer [10] and Bezout [11]; this notion is then developed by several authors and its essential properties are definitively established by Cauchy [13] and Jacobi [16(a)].

On the other hand, whilst mathematicians had a slight tendency to despise equations of the first degree, the solution of differential equations was considered a capital problem; it was natural that, among these equations, linear equations, with constant coefficients or otherwise, should early be distinguished and their study contributed to emphasize linearity and related properties. This is certainly seen in the work of Lagrange [9(b)] and Euler [8(b)], at least as far as homogeneous equations are concerned; for these authors see no point in saying that the general solution of the non-homogeneous equation is the sum of a particular solution and the general solution of the corresponding homogeneous equation and they make no use of this principle (known however to d'Alembert); we note here also that, when they state that the general solution of the homogeneous linear equation of order $n$ is a linear combination of $n$ particular solutions, they do not add that these must be linearly independent and make no effort to make the latter notion explicit; it seems that only the teaching of Cauchy at the École Polytechnique throws some light ([14], pp. 573–574) on these points as on many others. But already Lagrange (*loc. cit.*) introduces also (purely by calculation, it is true, and without giving it a name) the adjoint equation $L^*(y) = 0$ of a linear differential equation $L(y) = 0$, an example typical of duality by virtue of the relation

$$
\int z L(y)\, dx = \int L^*(z) y\, dx,
$$

valid for $y$ and $z$ zero at the extremities of the interval of integration; more precisely, and 30 years before Gauss defined explicitly the transpose of a linear substitution in 3 variables, we see here the first example without doubt of a "functional operator" $L^*$ the transpose or "adjoint" of an operator $L$ given by means of a bilinear function (here the integral $\int yz\, dx$).

At the same time and again with Lagrange [9(c)], linear substitutions, in 2 and 3 variables at first, were in the process of conquering arithmetic. Clearly the set of values of a function $F(x, y)$, when $x$ and $y$ are given all integral values, does not change when a linear substitution with integral coefficients, of determinant 1, is performed on $x$ and $y$; on this fundamental observation Lagrange founds the theory of representations of numbers by forms and that of the reduction of forms; and Gauss, by a step whose boldness it has become difficult for us to appreciate, isolates the notion of equivalence and that of class of forms (cf. Historical Note to I); on this subject, he recognizes the necessity of certain elementary principles relating to linear substitutions and introduces in particular the notion of transpose or adjoint ([12(a)], p. 304). From this moment onwards, the arithmetic study and the algebraic study of quadratic forms, in 2, 3 and later $n$ variables, that of bilinear forms which are closely related to them and more recently the generalization of these notions to an infinity of variables were, right up to the present, to constitute one of the most fertile sources of progress for linear algebra (cf. Historical Note to IX).

But a perhaps still more decisive progress was the creation by Gauss, in the same *Disquisitiones* (cf. Historical Note to I), of the theory of finite commutative groups, which occur there in four different ways, in the additive group of integers modulo $m$ (for $m$ an integer), in the multiplicative group of integers prime to $m$ modulo $m$, in the group of classes of binary quadratic forms and finally in the multiplicative group of $m$-th roots of unity; and, as we have already noted, it is clearly as commutative groups, or rather as modules over $\mathbf{Z}$, that Gauss treats all these groups and studies their structure, their relations of isomorphism, etc. In the module of "complex integers" $a + bi$, he is later seen studying an infinite module over $\mathbf{Z}$, whose isomorphism he no doubt perceived with the module of periods (discovered by him in the complex domain) of elliptic functions; in any case this idea already appears neatly in Jacobi's work, for example in his famous proof of the impossibility of a function with 3 periods and his views on the problem of inversion of Abelian integrals [16(b)], to result soon in the theorems of Kronecker (cf. Historical Note to General Topology, VII).

Here, another current joins those whose course and occasional meanders we have sought to trace, which had long remained underground. As will later be expounded in more detail (Historical Note to IX), "pure" geometry in the sense understood in the last century, that is essentially projective geometry of the plane and space without using coordinates, had been created in the XVIIth century by Desargues [6], whose ideas, appreciated in their true value by a Fermat and put into practice by a Pascal, had then been buried in oblivion, eclipsed by the brilliant progress of analytic geometry; it was revived towards the end of the XVIIIth century, with Monge, then Poncelet and his rivals Brianchon and Chasles, sometimes completely and voluntarily separated from analytic methods, sometimes (especially in Germany) closely intermixed with them. Now projective transformations, from whatever point of view they are considered (synthetic or analytic), are of course just linear substitutions on the projective or "barycentric" coordinates; the theory of conics (in the XVIIth century) and later that of quadrics, with whose projective properties this school is principally concerned for a long time, are just that of quadratic forms, whose close connection with linear algebra we have already pointed out earlier. To these notions is added that of polarity: also created by Desargues, the theory of poles and polars becomes, in the hands of Monge and his successors and soon under the name of the principle of duality, a powerful tool for transforming geometric theorems; if it cannot be affirmed that its relation with adjoint differential equations was perceived during that period (they are indicated by Pincherle at the end of the century), then at least Chasles did not fail [17] to perceive its relation with the notion of reciprocal spherical triangles, introduced into spherical trigonometry by Viète ([3], p. 428) and Snellius as early as the XVIth century. But duality in projective geometry is only an aspect of duality of vector spaces, taking account of the modifications imposed when passing from the affine space to the projective space (which is a quotient space of it, under the relation "scalar multiplication").

The XIXth century, more than any period in our history, was rich in mathematicians of the first order; and it is difficult in a few pages, even restricting ourselves to the most salient features, to describe all that is produced in their hands by the coming together of these movements of ideas. Between the purely synthetic methods on the one hand, a species of Procrustean bed where their orthodox protagonists put themselves to torture, and the analytic methods related to a system of coordinates arbitrarily imposed on the space, the need is soon felt for a geometric calculus, dreamed of but not created by Leibniz and imperfectly sketched by Carnot: first appears addition of vectors, implicit in Gauss's work in his geometric representation of imaginary numbers and the applications he makes of this to elementary geometry (cf. Historical Note to General Topology, VIII), developed by Bellavitis under the name of "method of equipollences" and taking its definitive form with Grassmann, Möbius and Hamilton; at the same time, under the name of "barycentric calculus", Möbius gives a version of it suitable for the needs of projective geometry [18].

At the same period, and by the same men, the step, so natural (once engaged on this path), already announced by Fermat, is taken from the plane and "ordinary" space to $n$-dimensional space; indeed an inevitable step, since the algebraic phenomena which can in two or three variables be interpreted geometrically are still valid for an arbitrary number of variables; thus to impose, in using geometric language, the limitation to 2 or 3 dimensions, would be for the modern mathematician just as tiresome a yoke as that which always prevented the Greeks from extending the notion of number to ratios of incommensurable magnitudes. Hence the language and ideas relating to $n$-dimensional space appear almost simultaneously on all sides, obscurely in the work of Gauss, clearly in the work of the mathematicians of the following generation; and their greater or less assurance in using them was perhaps less due to their mathematical inclinations than to their philosophical or even purely practical outlook. In any case, Cayley and Grassmann, around 1846, handle these concepts with the greatest of ease (and this, says Cayley quite contrary to Grassmann ([22(a)], p. 321), "without recourse to any metaphysical notion"); Cayley is never far away from the analytic interpretation and coordinates, whereas in Grassmann's work from the start, addition of vectors in $n$-dimensional space and the geometric aspect take the upper hand, to result in the developments of which we shall speak in a moment.

Meantime the impulse given by Gauss was pushing mathematicians, in two different ways, towards this study of algebras or "hypercomplex systems". On the one hand, it was inevitable to try to extend the domain of real numbers otherwise than by introducing the "imaginary unit" $i = \sqrt{-1}$ and perhaps thus open up vaster domains just as fertile as that of the complex numbers. Gauss himself was convinced ([12(b)], p. 178) of the impossibility of such an extension, as long as one wants to preserve the principal properties of complex numbers, that is, in modern language, those which make it into a commutative field; and, either under his influence or independently, his contemporaries seem to have shared this conviction, which was only justified much later by Weierstrass [23] in a precise theorem. But, once multiplication of complex numbers is interpreted by rotations in the plane, then, if it is proposed to extend this idea to three dimensional space, (since the rotations in space form a non-Abelian group) non-commutative multiplications have to be envisaged; this is one of Hamilton's† guiding ideas in his discovery of quaternions [20], the first example of a non-commutative field. The singular nature of this example (the only one, as Frobenius was later to show, which can be constructed over the

† Cf. the interesting preface of his Lectures on quaternions [20] where he retraces the whole history of his discovery.

field of real numbers) somewhat restricts its import, in spite of or perhaps even because of the formation of a school of fanatical "quaternionists": a strange phenomenon, which was later reproduced around the work of Grassmann, and then by the vulgarizers who draw from Hamilton and Grassmann what is called "vector calculus". The abandoning a little later of associativity, by Graves and Cayley who construct the "Cayley numbers", opens up no very interesting path. But after Sylvester had introduced matrices and (without giving it a name) had clearly defined their rank [21], again it was Cayley [22(b)] who created the calculus of matrices, not without observing (an essential fact often lost sight of later) that a matrix is only an abridged notation for a linear substitution, just as Gauss denoted the form $aX^2 + 2bXY + cY^2$ by $(a, b, c)$. This is just one aspect, the most interesting for us of course, of the abundant production by Sylvester and Cayley on determinants and everything connected with them, a production full of ingenious identities and impressive calculations.

Also (amongst other things) Grassmann discovers an algebra over the reals, the exterior algebra which still bears his name. His work, earlier even than that of Hamilton [19(a)], created in an almost complete moral solitude, remained for a long time little known, no doubt because of its originality, because also of the philosophical mists, in which it begins by enveloping itself and which for example at first deterred Möbius. Moved by preoccupations analogous to those of Hamilton but of greater import (and which, as he soon sees, are the same as those of Leibniz), Grassmann constructs a vast algebraico-geometric edifice, resting on a geometric or "intrinsic" conception (already more or less axiomatized) of $n$-dimensional vector space; among the more elementary results at which he arrives, we quote for example the definition of linear independence of vectors, that of dimension and the fundamental relation

$$
\dim V + \dim W = \dim(V + W) + \dim(V \cap W)
$$

(loc. cit., p. 209; cf. [19(b)], p. 21). But it is especially exterior multiplication, then inner multiplication, of multivectors which provide him with the tools with which he easily treats first the problems of linear algebra proper and then those relating to the Euclidean structure, that is orthogonality of vectors (where he finds the equivalent of duality, which he does not possess).

The other path opened up by Gauss in the study of hypercomplex systems is that starting from the complex integers $a + bi$; after these follow quite naturally algebras or more general hypercomplex systems, over the ring $\mathbf{Z}$ of integers and over the field $\mathbf{Q}$ of rationals, and first of all those already envisaged by Gauss which are generated by roots of unity, then algebraic number fields and modules of algebraic integers: the former are the principal topic in the work of Kummer, the study of the latter was undertaken by Dirichlet, Hermite, Kronecker and Dedekind. Here, in contrast to what happens with algebras over the reals, it is not necessary to abandon any of the characteristic properties of commutative fields and attention was confined to the latter throughout the XIXth century. But linear properties and for example the search for the basis for the integers of the field (indispensable for a general definition of the discriminant) play an essential role at many points; and with Dedekind at any rate the methods are destined to become typically "hypercomplex"; Dedekind himself moreover, without setting himself the problem of algebras in general, is conscious of this character of his works and of what relates them for example to the results of Weierstrass on hypercomplex systems over the reals ([24], in particular vol. 2, p. 1). At the same time the determination of the structure of the multiplicative group of units in an algebraic number field, effected by Dirichlet in some famous notes [15] and almost at the same time by Hermite, was vitally important in clarifying ideas on modules over $\mathbf{Z}$, their generating systems and, their bases (when such exist). Then the notion of ideal, defined by Dedekind in algebraic number fields (as a module over the ring of integers of the field), whilst Kronecker introduces in polynomial rings (under the name of "systems of modules") an equivalent notion, gives the first examples of modules over more general rings than $\mathbf{Z}$; and in the work of the same authors, and then Hilbert, in particular cases the notion of group with operators is slowly isolated, and the possibility of constructing always from such a group a module over a suitably defined ring.

At the same time, the arithmetico-algebraic study of quadratic bilinear forms and their "reduction" (or, what amounts to the same, of matrices and their "invariants") leads to the discovery of the general principles on the solution of systems of linear equations, principles which due to the lack of the notion of rank, had escaped Jacobi.\footnote{Concerning the classification of systems of $n$ equations in $n$ unknowns when the determinant is zero, he says ([16(a)], p. 370): "paullo prolixum videtur negotium" (it could not be elucidated briefly).} The problem of the solution in integers of systems of linear equations with integral coefficients is attacked and solved, first in a special case by Hermite and then in all its generality by H. J. Smith [25]; the results of the latter are found again, only in 1878, by Frobenius, in the framework of a vast programme of research instituted by Kronecker and in which Weierstrass also participates; incidentally during the course of these works, Kronecker gives definitive form to the theorems on linear systems with real (or complex) coefficients, which are also elucidated, in an obscure manual, with the minute care characteristic of him, by the famous author of *Alice in Wonderland*; as for Kronecker, he disdains to publish these results and leaves them to his colleagues and disciples; the word "rank" itself is only introduced by Frobenius. Also in the course of their teaching at the University of Berlin Kronecker [26] and Weierstrass introduce the "axiomatic" definition of determinants (as an alternating multilinear function of $n$ vectors in $n$-dimensional space, normed so that it takes the value 1 at the unit matrix), a definition equivalent to that derived from Grassmann’s calculus and to that adopted in this Treatise; again during his courses Kronecker, without feeling the need to give it a name and in a still non-intrinsic form, introduces the tensor product of spaces and the “Kronecker” product of matrices (the linear substitution induced on a tensor product by given linear substitutions applied to the factors).

This research cannot be separated from the theory of invariants created by Cayley, Hermite and Sylvester (the “invariant trinity” of which Hermite later speaks in his letters) and which, from a modern point of view, is above all a theory of representations of the linear group. Here there comes to light, as the algebraic equivalent of duality in projective geometry, the distinction between series of cogredient and contragredient variables, that is vectors in a space and vectors in the dual space; and, after attention has been turned first to forms of low degree and then of arbitrary degree, in 2 and 3 variables, almost without delay bilinear, then multilinear forms are examined in several series of “cogredient” or “contragredient” variables, which is equivalent to the introduction of tensors; the latter becomes explicit and is popularized when, under the inspiration of the theory of invariants, Ricci and Levi-Civitá, in 1900, introduce into differential geometry “tensor calculus” [28], which later came into great vogue following its use by the “relativist” physicists. Again the progressive intermingling of the theory of invariants, differential geometry and the theory of partial differential equations (especially the so-called problem of Pfaff and its generalizations) slowly leads geometers to consider alternating bilinear forms of differentials, in particular the “bilinear covariant” of a form of degree 1 (introduced in 1870 by Lipschitz and then studied by Frobenius), to result in the creation by E. Cartan [29] and Poincaré [30] of the calculus of exterior differential forms. Poincaré introduces the latter, in order to form his integral invariants, as the expressions which appear in multiple integrals, whilst Cartan, guided no doubt by his research on algebras, introduces them in a more formal way, but without failing to observe that the algebraic part of their calculus is identical with Grassmann’s exterior multiplication (whence the name which he adopts), thus definitively restoring the work of the latter to its rightful place. The translation, into the notation of tensor calculus, of exterior differential forms, moreover shows immediately their connection with skew-symmetric tensors, which, once a purely algebraic point of view is adopted, shows that they are for alternating multilinear forms what covariant tensors are for arbitrary multilinear forms; this aspect is further clarified with the modern theory of representations of the linear group; and thus, for example, the substantial identity between the definition of determinants given by Weierstrass and Kronecker and that resulting from Grassmann’s calculus is recognized.

We thus arrive at the modern period, where the axiomatic method and the notion of structure (at first vaguely perceived, and defined only recently) allow us to separate concepts which until then had been inextricably mixed, to formulate what was vague or left to intuition and to prove with proper generality theorems which were known only in special cases. Peano, one of the creators of the axiomatic method and also one of the first mathematicians fully to appreciate the work of Grassmann, gives as early as 1888 ([27], Chapter IX) the axiomatic definition of vector spaces (finite-dimensional or otherwise) over the field of real numbers and, in a completely modern notation, of linear mappings of one such space into another; a little later, Pincherle seeks to develop applications of linear algebra, thus conceived, to the theory of functions, in a direction it is true which has not been very fruitful; at least his point of view allows him to recognize “Lagrange’s adjoint” as a special case of the transposition of linear mappings: which appears soon, still more clearly, and for partial differential equations as well as for differential equations, in the course of the memorable works of Hilbert and his school on Hilbert space, and its applications to analysis. It is on that occasion that Toeplitz [31], also introducing (but by means of coordinates) the most general vector space over the reals, makes the fundamental observation that the theory of determinants is not needed to prove the principal theorems of linear algebra, which allows these to be extended without difficulty to infinite-dimensional spaces; and he also indicates that linear algebra thus understood can of course be applied to an arbitrary commutative base field.

On the other hand, with the introduction by Banach, in 1922, of the spaces bearing his name,\footnote{These are complete normed vector spaces over the field of real numbers or that of complex numbers.} spaces not isomorphic to their dual are encountered, albeit in a problem which is topological as much as it is algebraic. Already between a finite-dimensional vector space and its dual there is no “canonical” isomorphism, that is determined by its structure, which had long been reflected in the distinction between cogredient and contragredient. Nevertheless it seems beyond doubt that the distinction between a space and its dual was definitively established only after the work of Banach and its school; also in these works the importance of the notion of codimension comes to light. As for duality or “orthogonality” between the vector subspaces of a space and those of its dual, the way in which it is formulated today presents not just a superficial analogy with the modern formulation of the principal theorem of Galois theory (cf. *Algebra*, V) and with so-called Pontrjagin duality in locally compact Abelian groups; the latter goes back to Weber, who, in the course of arithmetical researches, lays in 1886 its foundations for finite groups; in Galois theory the “duality” between subgroups and subfields takes form in the work of Dedekind and Hilbert; and orthogonality between vector subspaces derives visibly, first from duality between linear varieties in projective geometry and also from the notion and properties of completely orthogonal varieties in a Euclidean space or a Hilbert space (whence its name). All these strands are reassembled in the contemporary period, in the hands of algebraists such as

E. Noether, Artin and Hasse and topologists such as Pontrjagin and Whitney (not without the ones influencing the others) to arrive, in each of these fields, at the stage of knowledge whose results are expounded in this Treatise.

At the same time a critical examination is made, which is destined to eliminate, on each point, the hypotheses which are not completely indispensable, and especially those which would close the way to certain applications. Thus the possibility is perceived of substituting rings for fields in the notion of vector spaces and, creating the general notion of module, of treating at the same time these spaces, Abelian groups, the particular modules already studied by Kronecker, Weierstrass, Dedekind and Steinitz and even groups with operators and for example of applying the Jordan-Hölder theorem to them; at the same time, with the distinction between right and left modules, we pass to the non-commutative, which arises from the modern development of the theory of algebras by the American school (Wedderburn, Dickson) and especially the German school (E. Noether, E. Artin).

BIBLIOGRAPHY

1. O. Neugebauer, Vorlesungen über Geschichte der antiken Mathematik, Vol. I: Vorgriechische Mathematik, Berlin (Springer), 1934.
2. Euclidis Elementa, 5 vols., ed. J. L. Heiberg, Lipsiae (Teubner), 1883–88.
2 bis. T. L. Heath, The thirteen books of Euclid’s Elements ..., 3 vols., Cambridge, 1908.
3. Francisci Vietae, Opera mathematica ..., Lugduni Batavorum (Elzevir), 1646.
4. P. Fermat, Oeuvres, vol. I, Paris (Gauthier-Villars), 1891: (a) Ad locos planos et solidos Isagoge (pp. 91–110; French transl. ibid., vol. III, p. 85); (b) Appendix ad methodum ... (pp. 184–188; French transl., ibid., vol. III, p. 159).
5. R. Descartes, La géométrie, Leyde (Jan Maire), 1637 (=Oeuvres, ed. Ch. Adam and P. Tannery, vol. VI, Paris (L. Cerf), 1902).
6. G. Desargues, Oeuvres ..., vol. I, Paris (Leiber), 1864: Brouillon proiect d’une atteinte aux éuénemens des rencontres d’un cône auec un plan (pp. 103–230).
7. G. W. Leibniz, Mathematische Schriften, ed. C. I. Gerhardt, vol. I, Berlin (Asher), 1849.
8. L. Euler: (a) Introductio in Analysin Infinitorum, vol. 2, Lausannae, 1748 (=Opera Omnia (1), vol. IX, Zürich-Leipzig-Berlin (O. Füssli and B. G. Teubner), 1945); (b) Institutionum Calculi Integralis, vol. 2, Petropoli, 1769 (=Opera Omnia (1), vol. XII, Leipzig-Berlin (B. G. Teubner), 1914).
9. J.-L. Lagrange, Oeuvres, Paris (Gauthier-Villars), 1867–1892: (a) Solutions analytiques de quelques problèmes sur les pyramides triangulaires, vol. III, pp. 661–692; (b) Solution de différents problèmes de calcul intégral, vol. I, p. 471; (c) Recherches d’arithmétique, vol. III, pp. 695–795.

10. G. Cramer, Introduction à l’analyse des lignes courbes, Geneva (Cramer and Philibert), 1750.

11. E. Bezout, Théorie générale des équations algébriques, Paris, 1779.

12. C. F. Gauss, Werke, Göttingen, 1870–1927: (a) Disquisitiones arithmeticae, vol. I; (b) Selbstanzeige zur Theoria residuorum biquadraticorum, Commentatio secunda, vol. II, pp. 169–178.

13. A.-L. Cauchy, Mémoire sur les fonctions qui ne peuvent obtenir que deux valeurs égales et de signes contraires par suite des transpositions opérées entre les variables qu’elles renferment, J. Ec. Polytech., cahier 17 (volume X), 1815, pp. 29–112 (=Oeuvres complètes (2), vol. I, Paris (Gauthier-Villars), 1905, pp. 91–169).

14. A.-L. Cauchy, in Leçons de calcul différentiel et de calcul intégral, rédigées principalement d’après les méthodes de M. A.-L. Cauchy by Abbé Moigno, vol. II, Paris, 1844.

15. P. G. Lejeune-Dirichlet, Werke, vol. I, Berlin (G. Reimer), 1889, pp. 619–644.

16. C. G. J. Jacobi, Gesammelte Werke, Berlin (G. Reimer), 1881–1891: (a) De formatione et proprietatibus determinantium, vol. III, pp. 355–392; (b) De functionibus duarum variabilium . . ., vol. II, pp. 25–50.

17. M. Chasles, Aperçu historique sur l’origine et le développement des méthodes en géométrie . . ., Bruxelles, 1837.

18. A. F. Möbius, Der baryzentrische Calcul . . ., Leipzig, 1827 (=Gesammelte Werke, vol. I, Leipzig (Hirzel), 1885).

19. H. Grassmann: (a) Die lineale Ausdehnungslehre, ein neuer Zweig der Mathematik, dargestellt und durch Anwendungen auf die übrigen Zweige der Mathematik, wie auch auf die Statik, Mechanik, die Lehre vom Magnetismus und die Kristallonomie erläutert, Leipzig (Wigand), 1844 (=Gesammelte Werke, vol. I, 1st Part, Leipzig (Teubner), 1894); (b) Die Ausdehnungslehre, vollständig und in strenger Form bearbeitet, Berlin, 1862 (=Gesammelte Werke, vol. I, 2nd Part, Leipzig (Teubner), 1896).

20. W. R. Hamilton, Lectures on quaternions, Dublin, 1853.

21. J. J. Sylvester, Collected Mathematical Papers, vol. I, Cambridge, 1904: No. 25, Addition to the articles . . ., pp. 145–151 (=Phil. Mag., 1850).

22. A. Cayley, Collected Mathematical Papers, Cambridge, 1889–1898: (a) Sur quelques théorèmes de la géométrie de position, vol. I, pp. 317–328 (=Crelle’s J., vol. XXXI (1846), pp. 213–227); (b) A memoir on the theory of matrices, vol. II, pp. 475–496 (=Phil. Trans., 1858).

23. K. Weierstrass, Mathematische Werke, vol. II, Berlin, (Mayer und Müller),

1895: Zur Theorie des aus $n$ Haupteinheiten gebildeten complexen Grössen, pp. 311–332.
24. R. Dedekind, Gesammelte mathematische Werke, 3 vols., Braunschweig (Vieweg), 1930–32.
25. H. J. Smith, Collected Mathematical Papers, vol. I, Oxford, 1894: On systems of linear indeterminate equations and congruences, p. 367 (=Phil. Trans., 1861).
26. L. Kronecker, Vorlesungen über die Theorie der Determinanten . . ., Leipzig (Teubner), 1903.
27. G. Peano, Calcolo geometrico secondo l’Ausdehnungstheorie di Grassmann preceduto dalle operazioni della logica deduttiva, Torino, 1888.
28. G. Ricci and T. Levi-Civita, Méthodes de calcul différentiel absolu et leurs applications, Math. Ann., vol. LIV (1901), p. 125.
29. E. Cartan, Sur certaines expressions différentielles et le problème de Pfaff, Ann. E.N.S. (3), vol. XVI (1899), pp. 239–332 (=Oeuvres complètes, vol. II_1, Paris (Gauthier-Villars), 1953, pp. 303–396).
30. H. Poincaré, Les méthodes nouvelles de la mécanique céleste, vol. III, Paris (Gauthier-Villars), 1899, Chapter XXII.
31. O. Toeplitz, Ueber die Auflösung unendlichvieler linearer Gleichungen mit unendlichvielen Unbekannten, Rend. Circ. Mat. Pal., vol. XXVIII (1909), pp. 88–96.

$x + y, x \cdot y, xy, x \top y, x \perp y$: I, § 1, no. 1.
$X \top Y, X + Y, XY$ (X, Y subsets): I, § 1, no. 1.
$X \top a, a \top X$ (X a subset, a an element): I, § 1, no. 1.

$$
\prod_{\alpha \in A} x_\alpha, \bigwedge_{\alpha} x_\alpha, \bigwedge x_\alpha, \bigwedge_{\alpha \in A} x, \bigwedge_{\alpha} x_\alpha, \bigwedge x_\alpha, \sum_{\alpha \in A} x_\alpha, \sum x_\alpha, \sum_{\alpha} x_\alpha, \prod_{\alpha \in A} x_\alpha, \prod x_\alpha,
$$

$$
\prod_{\alpha \in A} x_\alpha : \text{I, § 1, no. 2}.
$$

$$
\prod_{p \leq i \leq q} x_i, \prod_{i=p}^q x_i : \text{I, § 1, no. 2}.
$$

$x_p \top x_{p+1} \top \cdots \top x_q : \text{I, § 1, no. 3}$.

$$
\prod^n x, \perp x^n, nx \quad (n \in \mathbf{N}) : \text{I, § 1, no. 3}.
$$

$$
\prod_{0 \leq i < j \leq n} x_{ij}, \prod_{i < j} x_{ij} : \text{I, § 1, no. 5}.
$$

$$
\sum_{i=p}^q \sum_{j=r}^s x_{ij}, \sum_{j=r}^s \sum_{i=p}^q x_{ij} : \text{I, § 1, no. 5}.
$$

$$
\prod_{0 \leq i_1 < i_2 < \cdots < i_p \leq n} x_{i_1 i_2 \cdots i_p}, \prod_{i_1 < i_2 < \cdots < i_p} x_{i_1 i_2 \cdots i_p} : \text{I, § 1, no. 5}.
$$

$0, 1 : \text{I, § 2, no. 1}$.

$\gamma_a, \delta_a, \gamma(a), \delta(a) : \text{I, § 2, no. 2}$.

$E_S$ (S a subset of a commutative monoid E): I, § 2, no. 4.

$\mathbf{Z}, +$ (addition in $\mathbf{Z}$): I, § 2, no. 5.

$\leq$ (order relation on $\mathbf{Z}$): I, § 2, no. 5.

$\mathbf{N}^* : \text{I, § 2, no. 5}$.

$\prod^n$ (for $n \in \mathbf{Z}$): I, § 2, no. 7.

$
-x, x - y, x + y - z, x - y - z, x - y + z - t : \text{I, § 2, no. 8}.
$

$nx$ ($n \in \mathbf{Z}$): I, § 2, no. 8.

$x^n$ ($n \in \mathbf{Z}$): I, § 2, no. 8.

$
\frac{1}{x}, \frac{x}{y}, x/y : \text{I, § 2, no. 8}.
$ $\alpha.x, x.\alpha, x^\alpha$ ($\alpha$ an operator): I, § 3, no. 1.
$\alpha \perp x, \alpha \perp X, \Xi \perp X$ ($\alpha$ an operator, $\Xi$ a set of operators): I, § 3, no. 1.
$\mathfrak{S}_F$: I, § 4, no. 1.
$(G:H), G/H$ (H a subgroup of G): I, § 4, no. 4.
$x \equiv y$ (mod. H), $x \equiv y$ (H) (H a normal subgroup): I, § 4, no. 4.
Ker $f$, Im $f$ ($f$ a group homomorphism): I, § 4, no. 5.
$$
\prod_{i \in I} G_i \quad (G_i \text{ groups}): \text{I, } § 4, \text{ no. 8}.
$$
$G_1 \times_H G_2$: I, § 4, no. 8.
$$
\prod_{i \in I} G_i \quad (G_i \text{ groups}): \text{I, } § 4, \text{ no. 9}.
$$
$x \equiv y$ (mod. $a$), $x \equiv y$ ($a$) ($a, x, y$ rational integers): I, § 4, no. 10.
$v_p(a)$ ($p$ a prime number, $a$ a rational integer): I, § 4, no. 10.
Aut(G), Int(G), Int(x) (G a group, $x \in G$): I, § 5, no. 3.
$N_G(A), N(A)$ (G a group, $A \subset G$): I, § 5, no. 3.
$C_G(A), C(A)$ (G a group, $A \subset G$): I, § 5, no. 3.
E/G, G|E (G a group operating on E): I, § 5, no. 4.
G|E/H (G, H groups operating on E by commuting actions): I, § 5, no. 4.
$\mathfrak{S}_n$: I, § 5, no. 7.
$\tau_{x,y}$ (transposition of support $\{x, y\}$): I, § 5, no. 7.
$\varepsilon(\sigma), \varepsilon_\sigma$ ($\sigma$ a permutation): I, § 5, no. 7.
$\mathcal{U}_E, \mathcal{U}_n$: I, § 5, no. 7.
$F \xrightarrow{i} E \xrightarrow{\rho} G$ (E, F, G groups): I, § 6, no. 1.
$F \times_\tau G, \mathcal{E}_\tau$ ($\tau$ a homomorphism of G into Aut(F)): I, § 6, no. 1.
$gf$ ($f \in F, g \in G$): I, § 6, no. 1.
$(f, g) \cdot_\tau (f', g')$ ($f, f'$ in F, $g, g'$ in G): I, § 6, no. 1.
$(x, y), (A, B)$ ($x, y$ elements, A, B subsets of a group G): I, § 6, no. 2.
D(G): I, § 6, no. 2.
$C^n(G)$: I, § 6, no. 3.
$D^n(G)$: I, § 6, no. 4.
$E^G$ (G a group operating on E): I, § 6, no. 5.
$M_n(X), M(X)$ (X a set): I, § 7, no. 1.
$l(w)$ ($w$ an element of M(X)): I, § 7, no. 1.
$ww', w.w'$ ($w, w'$ elements of M(X)): I, § 7, no. 1.
$l(w)$ ($w$ a word over X): I, § 7, no. 2.
$ww', w.w'$ ($w, w'$ words over X): I, § 7, no. 2.
Mo(X) (X a set): I, § 7, no. 2.
$l(\sigma)$ ($\sigma$ a decomposition): I, § 7, no. 3.
$*G_i, G_1 * G_2$ ($G_1, G_2, G_i$ groups): I, § 7, no. 3.
$\langle \tau_1, \ldots, \tau_n; r_1, \ldots, r_m \rangle$ ($\tau_j$ generators, $r_i$ relators): I, § 7, no. 6.
$\langle \tau_1, \ldots, \tau_n; u_1 = v_1, \ldots, u_m = v_m \rangle$ ($\tau_j$ generators, $u_i, v_i$ elements of a free group): I, § 7, no. 6.
$\mathbf{Z}^{(X)}, \mathbf{N}^{(X)}$ (X a set): I, § 7, no. 7.

0, 1 (elements of a ring): I, § 8, no. 1.
A^0 (A a ring): I, § 8, no. 3.
(a) (a an element of A): I, § 8, no. 6.
$\sum_{\lambda} a_\lambda$ (a_\lambda ideals): I, § 8, no. 6.
$x \equiv y \pmod{a}$, $x \equiv y$ (a) (a an ideal): I, § 8, no. 7.
A/a (a a two-sided ideal): I, § 8, no. 7.
ab (a, b two-sided ideals): I, § 8, no. 9.
A[S^{-1}] (S a subset of a ring A): I, § 8, no. 12.
$F_p$ (p a prime number): I, § 9, no. 1.
$\mathbf{Q}$: I, § 9, no. 4.
$\mathbf{Q}_+$: I, § 9, no. 4.
|x|, sgn x (x a rational number): I, § 9, no. 4.
in(G): I, § 4, Exercise 13.
D_n: I, § 6, Exercise 4.
Q: I, § 6, Exercise 4.
A \approx B: I, § 6, Exercise 39.
e(G): I, § 7, Exercise 39.
d_n(X): I, § 7, Exercise 39.
A_s, A_d (A a ring): II, § 1, no. 1.
$\sum_{i \in I} x_i ((x_i)_{i \in I})$ a family of elements of a module of finite support: II, § 1, no. 1.
Hom_A(E, F), Hom(E, F), (E, F, A-modules): II, § 1, no. 2.
End_A(E), End(E), Aut(E), GL(E) (E an A-module): II, § 1, no. 2.
Hom_A(u, v), Hom(u, v) (u, v linear mappings): II, § 1, no. 2.
1_E (E a module): II, § 1, no. 2.
0 (zero module): II, § 1, no. 3.
Ker u, Im u, Coim u, Coker u (u a linear mapping): II, § 1, no. 3.
$\prod_i f_i$ (f_i: E_i \to F_i linear mappings): II, § 1, no. 5.
$\bigoplus_{i \in I} E_i, E_p \oplus E_{p+1} \oplus \cdots \oplus E_q ((E_i)_{i \in I}$ a family of A-modules): II, § 1, no. 6.
$\sum_{i \in I} f_i$ (f_i: E_i \to F_i linear mappings): II, § 1, no. 6.
$\bigoplus_{i \in I} f_i, f_p \oplus f_{p+1} \oplus \cdots \oplus f_q$ (f_i: E_i \to F_i linear mappings): II, § 1, no. 6.
E^{(1)} (E a module): II, § 1, no. 6.
$\bigoplus_{i \in I} M_i$ ((M_i)_{i \in I} a family of submodules): II, § 1, no 7.
long_A(M), long(M) (M an A-module of finite length): II, § 1, no. 10.
$\delta_{st}$ (Kronecker symbol): II, § 1, no. 11.
$\sum_{t \in T} \xi_t \cdot t$ (T a set, $\xi_t$ elements of a ring): II, § 1, no. 11.

Ann(S), Ann(x) (S a subset of a module, x an element of a module): II, § 1, no. 12.
$\rho_*(E), E_{[B]}$ (E an A-module, $\rho : B \to A$ a ring homomorphism): II, § 1, no. 13.
$\rho_*(u)$ ($\rho : B \to A$ a ring homomorphism, u an A-linear mapping): II, § 1, no. 13.
E* (E a module): II, § 2, no. 3.
$\langle x, x^* \rangle$ (x an element of a left module E, $x^*$ an element of its dual E*): II, § 2, no. 3.
$\langle x^*, x \rangle$ (x an element of a right module E, $x^*$ an element of its dual E*): II, § 2, no. 3.
$t_u$ (u a linear or semi-linear mapping): II, § 2, no. 5.
$\tilde{u}$ (u an isomorphism): II, § 2, no. 5.
$E \otimes_A F, E \otimes_A F$ (E a right A-module, F a left A-module): II, § 3, no. 1.
$x \otimes y$ (x $\in$ E (a right module), y $\in$ F (a left module)): II, § 3, no. 1.
$u \otimes v$ (u, v linear mappings): II, § 3, no. 2.
$u \otimes v$ (u, v semi-linear mappings): II, § 3, no. 3.
$s_{A_d}$ (A ring): II, § 3, no. 4.
$\mathcal{L}_2(E, F; G)$ (E, F, G modules over a commutative ring): II, § 3, no. 5.
$\bigotimes_{\lambda \in L} G_\lambda, \bigotimes_{\lambda \in L} x_\lambda$ (($G_\lambda$) a family of $\mathbf{Z}$-modules, $x_\lambda \in G_\lambda$ for all $\lambda$): II, § 3, no. 9.
$\bigotimes_{\lambda \in L} v_\lambda$ ($v_\lambda : G_\lambda \to G'_\lambda$ $\mathbf{Z}$-linear mappings): II, § 3, no. 9.
$\bigotimes_{(c,p,q)} G_\lambda, \bigotimes_{(c,p,q)} x_\lambda, \bigotimes_{(c)} x_\lambda$: II, § 3, no. 9.
$\bigotimes_{(c)} v_\lambda$ ($v_\lambda$ $\mathbf{Z}$-linear mappings): II, § 3, no. 9.
$E_1 \otimes_{A_1} E_2 \otimes_{A_2} E_3 \otimes \cdots \otimes_{A_{n-2}} E_{n-1} \otimes_{A_{n-1}} E_n$: II, § 3, no. 9.
$x_1 \otimes x_2 \otimes \cdots \otimes x_n$: II, § 3, no. 9.
$u_1 \otimes u_2 \otimes \cdots \otimes u_n$ ($u_i$ linear mappings): II, § 3, no. 9.
$\mathcal{L}_n(E_1, \ldots, E_n; G)$ ($E_1, \ldots, E_n, G$ modules over a commutative ring): II, § 3, no. 9.
Tr(u) (u an endomorphism of a module over a commutative ring): II, § 4, no. 3.
$\rho^*(E), E_{(B)}$ (E an A-module, $\rho : A \to B$ a ring homomorphism): II, § 5, no. 1.
$\rho^*(u), u_{(B)}$ ($\rho : A \to B$ a ring homomorphism, u an A-module homomorphism): II, § 5, no. 1.
dim_K E, dim E, [E : K] (E a vector K-space): II, § 7, no. 2.
dim_A E, dim E (E an A-module any two bases of which are equipotent): II, § 7, no. 2.
codim_E F, codim F (F a vector subspace of a vector space E): II, § 7, no. 3.
rg(u) (u a linear mapping of vector spaces): II, § 7, no. 4.
rg(u) (u an element of a tensor product of vector spaces): II, § 7, no. 8.
dim_K E, dim E (E an affine space over a field K): II, § 9, no. 1.
$a + t, t + a$ (a a point, t a translation of an affine space): II, § 9, no. 1.

$b - a$ ($a, b$ points of an affine space): II, § 9, no. 1.

$\sum_{c \in I} \lambda_i x_i$ (($x_i$)$_{i \in I}$ a family of points of an affine space, $(\lambda_i)_{i \in I}$ a family of scalars, of finite support, such that $\sum_i \lambda_i = 1$ or $\sum_i \lambda_i = 0$): II, § 9, no. 1.

$\mathbf{P}(V), \Delta(V)$ (V a vector space): II, § 9, no. 5.
$\mathbf{P}_n(K), \Delta_n(K)$ (K a field): II, § 9, no. 5.
$\dim_K \mathbf{P}(V), \dim \mathbf{P}(V)$ (V a vector K-space): II, § 9, no. 5.
$\tilde{K}, \infty$ (K a field): II, § 9, no. 9.
$\mathbf{PGL}(V), \mathbf{PGL}_n(K), \mathbf{PGL}(n, K)$ (K a field, V a vector space): II, § 9, no. 10.
$^tM$ ($M$ a matrix): II, § 10, no. 1.
$M' + M''$ ($M', M''$ matrices over a commutative group): II, § 10, no. 2.
$f(M', M''), M'M''$ ($M', M''$ matrices): II, § 10, no. 2.
$E_{ij}$ (matrix units): II, § 10, no. 3.
$\sigma(M), M^\sigma$ ($M$ a matrix, $\sigma$ a ring homomorphism): II, § 10, no. 3.
$M(x), x$ (x an element of a finitely generated free module): II, § 10, no. 4.
$M(u)$ (u a homomorphism of a free module into a free module): II, § 10, no. 4.
$M(x), M(u)$ (matrices relative to decompositions as direct sums): II, § 10, no. 5.
$M(u)$ (u a semi-linear mapping): II, § 10, no. 6.
$\mathbf{M}_n(A), I_n, 1_n$ (A a ring): II, § 10, no. 7.
$\mathbf{GL}_n(A), \mathbf{GL}(n, A)$ (A a ring): II, § 10, no. 7.
$^tX^{-1}$ (X an invertible square matrix): II, § 10, no. 7.
$\operatorname{diag}(a_i)_{i \in I}, \operatorname{diag}(a_1, a_2, \ldots, a_n)$: II, § 10, no. 7.
$X_1 \otimes X_2$ ($X_1, X_2$ matrices over a commutative ring): II, § 10, no. 10.
$\operatorname{Tr}(X)$ (X a square matrix over a commutative ring): II, § 10, no. 11.
$\operatorname{rg}(X)$ (X a matrix over a field): II, § 10, no. 12.
$\deg(x)$ (x an element of a graded group): II, § 11, no. 1.
$M(\lambda_0)$ (M a graded module, $\lambda_0$ an element of the monoid of degrees): II, § 11, no. 2.
$\operatorname{Homgr}_A(M, N)$ (M, N graded modules over a graded ring A): II, § 11, no. 6.
$\operatorname{Engr}_A(M), M^{*\operatorname{gr}}$ (M a graded module): II, § 11, no. 6.
$M:N$ (M, N modules): II, § 1, Exercise 24.

$$
\begin{bmatrix}
a & b \\
d & c
\end{bmatrix}
$$ (a, b, c, d points on a projective line): II, § 9, Exercise 11.

$\mathbf{SL}(E)$ (E a vector space): II, § 10, Exercise 12.
$\mathbf{PSL}(E)$ (E a vector space): II, § 10, Exercise 14.
$x.y, xy$ (multiplication in an algebra): III, § 1, no. 1.
$E^0$ (E an algebra): III, § 1, no. 1.
$\operatorname{Hom}_{A-\operatorname{alg.}}(E, F)$ (E, F A-algebras): III, § 1, no. 1.
$E/b$ (b a two-sided ideal of an algebra E): III, § 1, no. 2.
$\hat{E}$ (E an algebra): III, § 1, no. 2.
$\eta_c, \eta_E, \eta$ (E an algebra, c a unit): III, § 1, no. 3.

T(u), N(u): III, § 2, no. 3.
$\bar{u}$ : III, § 2, no. 4.
$H$ : III, § 2, no. 5.
Lib_A(I), Libas_A(I), Libasc_A(I): III, § 2, no. 7.
$U((x_i)_{i \in I})$ : III, § 2, no. 8.
$A[(x_i)_{i \in I}], A[x_i]_{i \in I}$ : III, § 2, no. 9.
$A[(X_i)_{i \in I}]$ : III, § 2, no. 9.
$A[X_1, \ldots, X_n]$ : III, § 2, no. 9.
$A[X], A[X, Y], A[X, Y, Z]$ : III, § 2, no. 9.
X^\nu (\nu \text{ a multiindex}): III, § 2, no. 9.

\sum_s \xi_s e_s, \sum_s \xi_s . s (s \text{ elements of a monoid}): III, § 2, no. 10.
$A[[X_i]]_{i \in I}$ : III, § 2, no. 11.
$\sum_\nu \alpha_\nu X^\nu$ : III, § 2, no. 11.
\omega(u), \omega_K(u) (u \text{ a formal power series}): III, § 2, no. 11.

\bigotimes_{i \in I} E_i, E_1 \otimes_A E_2 \otimes \cdots \otimes_A E_n, E_1 \otimes E_2 \otimes \cdots \otimes E_n (E_i \text{ A-algebras}): III, § 4, no. 1.
E^{\otimes n} (E \text{ an algebra}): III, § 4, no. 1.

\bigotimes_{i \in I} E_i (I \text{ an infinite set, } E_i \text{ algebras}): III, § 4, no. 5.

\bigotimes_{i \in I} u_i, \bigotimes_{i \in I} x_i (u_i \text{ algebra homomorphisms, } x_i \text{ elements, I infinite}): III, § 4, no. 5.

\epsilon \bigotimes_{i \in I} E_i, \epsilon \bigotimes_{i \in I} f_i, \epsilon G^{\otimes n} (E_i, G \text{ graded algebras, } f_i \text{ graded algebra homomorphisms, } \epsilon \text{ a system of commutation factors}): III, § 4, no. 7.

g \bigotimes_{i \in I} E_i, E^g \otimes_A F, gG^{\otimes n}, g \bigotimes_{i \in I} f_i, f_1 \otimes f_2, gf^{\otimes n}: III, § 4, no. 7.

\bigotimes^n M, T^n(M), \mathrm{Tens}^n(M), T^n_A(M), T(M), \mathrm{Tens}(M), T_A(M) (M an A-module): III, § 5, no. 1.
T(u), T^n(u) (u \text{ a linear mapping}): III, § 5, no. 2.
T_J^1(M), T_q^p(M) (M a module): III, § 5, no. 6.
$\alpha_q^f(z), e_f^g$ : III, § 5, no. 6.
$\alpha_{v_p}^{\lambda \cdots \mu}$ : III, § 5, no. 6.
c_j^i: III, § 5, no. 6
S(M), S_A(M), \mathrm{Sym}(M): III, § 6, no. 1.
\mathfrak{g}', \mathfrak{g}'_M, \mathfrak{g}'_n: III, § 6, no. 1.
S^n(M), S^n(u), S(u) (M a module, u a linear mapping): III, § 6, nos. 1 and 2.
$s.z$ : III, § 6, no. 3.
e^\alpha (\alpha \text{ a multiindex}): III, § 6, no. 6.
\wedge(M), \wedge_A(M), \mathrm{Alt}(M): III, § 7, no. 1.
$\mathfrak{g}'', \mathfrak{g}''_M, \mathfrak{g}''_n$ : III, § 7, no. 1.

$\wedge^n(M)$: III, § 7, no. 1.
$u \wedge v, x_1 \wedge x_2 \wedge \cdots \wedge x_n$: III, § 7, no. 1.
$\wedge(u), \wedge^n(u)$ ($u$ a linear mapping): III, § 7, no. 2.
$x_H$ (H a subset of $\{1, n\}$): III, § 7, no. 3.
$u(x_1, \ldots, \hat{x}_j, \ldots, x_n)$: III, § 7, no. 4.
$a.z$: III, § 7, no. 4.
$A'_n(M), A''_n(M)$: III, § 7, no. 4.
$e_J$: III, § 7, no. 8.
$\rho_{J, K}$: III, § 7, no. 8.
$\det(u)$ ($u$ an endomorphism): III, § 8, no. 1.
$\det(x_1, x_2, \ldots, x_n)$ ($x_j$ vectors in an $n$-dimensional free A-module): III, § 8, no. 1.
$\det(X)$ ($X$ a matrix): III, § 8, no. 3.
$\det(\xi_{ij})_{1 \leq i \leq n, 1 \leq j \leq n}, \det(\xi_{ij})$: III, § 8, no. 3.

$$
\begin{vmatrix}
\xi_{11} & \cdots & \xi_{1n} \\
\vdots & \ddots & \vdots \\
\xi_{n1} & \cdots & \xi_{nn}
\end{vmatrix}
$$
: III, § 8, no. 3.

$X_{H, K}, X^{H}$ ($X$ a matrix): III, § 8, nos 5 and 6.
$\mathrm{SL}_n(A), \mathrm{SL}(n, A)$: III, § 8, no. 9.
$p.x$ ($p \in A[X]$, $x$ an element of an A-module): III, § 8, no. 10.
$M_u, M[X]$ ($M$ an A-module, $u$ an endomorphism): III, § 8, no. 10.
$\chi_u(X)$ ($u$ an A-module endomorphism): III, § 8, no. 11.
$\mathrm{Tr}_{M/K}(a), N_{M/K}(a), \mathrm{Pc}_{M/K}(a; X)$ ($A$ a K-algebra, $M$ an A-module, $a \in A$) : III, § 9, no. 1.
$\mathrm{Tr}_{A/K}(a), N_{A/K}(a), \mathrm{Pc}_{A/K}(a; X)$ ($A$ a K-algebra, $a \in A$) : III, § 9, no. 3.
$D_{A/K}(x_1, \ldots, x_n)$ ($x_j$ elements of a K-algebra A): III, § 9, no. 5.
$[u, v]_g, [u, v]$ ($u, v$ elements of a graded algebra): III, § 10, no. 4.
$P(D), P(d_1, \ldots, d_n)$ ($P$ a polynomial, $d_j$ derivations): III, § 10, no. 4.
$\mathrm{ad}_e(a), \mathrm{ad}(a)$ ($a$ a homogeneous element of a graded algebra): III, § 10, no. 6.
$D_K(B, F)$ ($B$ a K-algebra, $F$ a (B, B)-bimodule): III, § 10, no. 7.
$D_{A, \rho}(B, F), D_A(B, F)$: III, § 10, no. 7.
$D_s$ ($s$ an endomorphism): III, § 10, no. 9.
$\Omega_K(A), d_{A/K}(x), dx$ ($x$ an element of a K-algebra A): III, § 10, no. 11.
$D_iP, \partial P/\partial X_i$ ($P$ a polynomial): III, § 10, no. 11.
$\Omega(u), \Omega_0(u)$ ($u$ a ring homomorphism): III, § 10, no. 12.
$\Omega_u$ ($u$ a K-algebra homomorphism): III, § 10, no. 12.
$M^{*gr}$ ($M$ a graded module): III, § 11.
$u.v, u._mv$ ($u, v$ symmetric multilinear mappings): III, § 11, no. 2.
$u \wedge v$ ($u, v$ alternating multilinear mappings): III, § 11, no. 2.
$\theta_T, \theta_S, \theta_\Lambda$: III, § 11, no. 5.

$u \perp x, i(x)$ : III, § 11, no. 6.
$x \perp u, i'(x)$ : III, § 11, no. 6.
$x \perp u, i(u)$ : III, § 11, no. 7.
$u \perp x, i'(u)$ : III, § 11, no. 7.
$G_p(E), G_{n,p}(K)$ : III, § 11, no. 13.
a(x, y, z): III, Appendix, no. 1.
ME: III, § 2, Exercise 13.
E \* F: III, § 5, Exercise 6.
R[a]: III, § 6, Exercise 4.
K[X; \sigma, d]: III, § 10, Exercise 3.
\tilde{X}: III, § 11, Exercise 9.

Abelian group: I, § 4, no. 2.
Absolute value of a rational number: I, § 9, no. 4.
Action of one set on another: I, § 3, no. 1.
Action, canonical: I, § 3, no. 1.
Action, distributive: I, § 3, no. 4.
Action, induced: I, § 3, no. 2.
Action, quotient: I, § 3, no. 3.
Action, right, left, derived from a law of composition: I, § 3, no. 1.
Actions which commute: I, § 5, no. 4.
Addition: I, § 1, no. 1.
Addition of rational integers: I, § 2, no. 5.
Additively (law written): I, § 1, no. 1.
Adjoint of a matrix: III, § 11, Exercise 9.
Adjunction of a unit element (algebra derived by): III, § 1, no. 2.
Affine function: II, § 9, no. 4.
Affine group: II, § 9, no. 4.
Affine line, plane, hyperplane: II, § 9, no. 3.
Affine mapping: II, § 9, no. 4.
Affine space: II, § 9, no. 1.
Affine subset, linear variety: II, § 9, no. 3.
Affinely free, affinely related family: II, § 9, no. 3.
Affinely independent points: II, § 9, no. 3.
Algebra, A-Algebra: III, § 1, no. 1.
Algebra, alternative: III, Appendix, no. 1.
Algebra, alternating graded: III, § 4, no. 9.
Algebra, anticommutative graded: III, § 4, no. 9.
Algebra, associative: III, § 1, no. 1.
Algebra, Cayley: III, § 2, no. 4.
Algebra, commutative: III, § 1, no. 1.

Algebra derived from an algebra by the adjunction of a unit element: III, § 1, no. 2.
Algebra, exterior, of a module: III, § 7, no. 1.
Algebra, free: III, § 2, no. 7.
Algebra, free associative: III, § 2, no. 7.
Algebra, free associative and commutative: III, § 2, no. 7.
Algebra, free, of a module: III, § 2, Exercise 13.
Algebra generated by generators subject to relations: III, § 2, no. 8.
Algebra, graded, over a graded ring: III, § 3, no. 1.
Algebra, total, of a monoid: III, § 2, no. 10.
Algebra obtained by extension of scalars: III, § 1, no. 5.
Algebra obtained by restriction of scalars: III, § 1, no. 5.
Algebra of a group, of a magma, of a monoid: III, § 2, no. 6.
Algebra of dual numbers: III, § 2, no. 3.
Algebra of formal power series: III, § 2, no. 11.
Algebra of Hamiltonian quaternions: III, § 2, no. 5.
Algebra of octonians of type $(\alpha, \beta, \gamma, \delta)$: III, Appendix, no. 3.
Algebra of quaternions: III, § 2, no. 5.
Algebra of quaternions of type $(\alpha, \beta, \gamma)$, of type $(\alpha, \gamma)$: III, § 2, no. 5.
Algebra, opposite: III, § 1, no. 1.
Algebra, product: III, § 1, no. 4.
Algebra, quadratic: III, § 2, no. 3.
Algebra, quadratic, of type $(\alpha, \beta)$: III, § 2, no. 3.
Algebra, quotient: III, § 1, no. 4.
Algebra, Rees: III, § 6, Exercise 4.
Algebra, restricted, of a monoid: III, § 2, no. 10.
Algebra, symmetric, of a module: III, § 6, no. 1.
Algebra, tensor, of a module: III, § 5, no. 1.
Algebra, unital: III, § 1, no. 1.
Algebra, universal, defined by a generating system related by a family of relators: III, § 2, no. 8.
Algebra, universal, generated by a set subjected to identities: III, § 2, no. 8.
Algebra, universal unital associative, defined by a generating system related by a family of relators: III, § 2, no. 8.
Algebras, linearly disjoint: III, § 4, no. 4.
Alternating graded algebra: III, § 4, no. 9.
Alternating group: III, § 5, no. 7.
Alternating multilinear mapping: III, § 7, no. 4.
Alternative algebra: III, Appendix, no. 1.
Amalgamated sum: I, § 7, no. 3.
Annihilated by a scalar (element): II, § 1, no. 12.
Annihilator, left, right: I, § 8, no. 6.
Annihilator, of a subset, of an element of a module: II, § 1, no. 12.

Antiautomorphism: III, § 1, no. 1.
Anticocommutative graded cogebra: III, § 11, no. 3.
Anticocommutative skew graded bigebra: III, § 11, no. 4.
Anticommutative graded algebra: III, § 4, no. 9.
Anticommutative skew graded bigebra: III, § 11, no. 4.
Antiderivation, K-antiderivation: III, § 10, no. 2.
Antiendomorphism of a ring: II, § 10, no. 6.
Associated (B-module) with an A-module and a ring homomorphism B → A:
II, § 1, no. 13.
Associated (faithful module) with a module: II, § 1, no. 12.
Associated (law of action) with an action: I, § 3, no. 1.
Associated (linear mapping) with an affine linear mapping: II, § 9, no. 4.
Associated (vectorspace) with a module over an integral domain: II, § 7, no. 10.
Associated (vector subspace) with a homogeneous element of an exterior algebra: III, § 7, no. 2.
Associated (vector subspace) with a homogeneous element of a symmetric algebra: III, § 6, no. 2.
Associated (vector subspace) with a homogeneous element of a tensor algebra: III, § 5, no. 2.
Associative algebra: III, § 1, no. 1.
Associative algebra, free: III, § 2, no. 7.
Associative and commutative algebra, free: III, § 2, no. 7.
Associative law: I, § 1, no. 3.
Associativity relations in a multiplication table: III, § 1, no. 7.
Associativity theorem: I, § 1, no. 3.
Associator: III, Appendix, no. 1.
Attached (affine space) to a vector space: II, § 9, no. 3.
Augmentation: III, § 10, no. 8.
Automorphism, inner of a group: I, § 5, no. 3.
Automorphism, inner, of a ring: I, § 8, no. 4.
Automorphism with no fixed point: I, § 6, Exercise 23.

Barycentre of m points, barycentre of a family of weighted points: II, § 9, no. 2.
Barycentric coordinate: II, § 9, no. 3.
Bases dual to one another: II, § 2, no. 7.
Basic family in a group: I, § 7, no. 6.
Basis dual of a basis of a module: II, § 2, no. 6.
Basis, Hamel: II, § 7, no. 1.
Basis of a module: II, § 1, no. 11.
Basis of an algebra: III, § 1, no. 7.
Basis of T_I^J(M) associated with a basis of M: III, § 5, no. 6.

Basis of type $(\alpha, \beta)$ of a quadratic algebra: III, § 2, no. 3.
Basis of type $(\alpha, \beta, \gamma)$, of type $(\alpha, \gamma)$, of a quaternion algebra: III, § 2, no. 5.
Basis, projective: II, § 9, Exercise 10.
Biadditive, $\mathbf{Z}$-bilinear mapping: II, § 3, no. 1.
Bicentralizer: I, § 1, no. 5.
Bicentralizer of a subalgebra: III, § 1, no. 2.
Bicyclic group: I, § 6, Exercise 26.
Bidual of a module: II, § 2, no. 7.
Bigebra, anticommutative, anticocommutative, skew graded: III, § 11, no. 4
Bigebra, cocommutative, commutative, graded: III, § 11, no. 4.
Bigebra, graded bigebra, skew graded bigebra, III, § 11, no. 4.
Bigebra of a monoid: III, § 11, no. 4.
Bigraded group, ring, module: II, § 11, no. 2.
Bigraduation: II, § 11, no. 1.
Bilinear mapping: II, § 3, no. 5.
Bimodule, (A, B)-bimodule: II, § 1, no. 14.
Bimodule over algebras: III, § 4, no. 3.
Binomial formula: I, § 8, no. 2.
Block product of matrices: II, § 10, no. 5.
Boolean ring: I, § 9, Exercise 8.
Bordered matrix: II, § 10, no. 1.
Bracket, $\varepsilon$-bracket of two derivations: III, § 10, no. 4.

Cancellable, left, right, cancellable, element: I, § 2, no 2.
Cartan-Brauer-Hua Theorem: I, § 9, Exercise 18.
Cayley algebra: III, § 2, no. 4.
Cayley extension of an algebra: III, § 2, no. 5.
Cayley-Hamilton theorem: III, § 8, no. 11.
Cayley norm, trace: III, § 2, no. 4.
Cayley octonians: III, Appendix, no. 3.
Central element: I, § 1, no. 5.
Central extension: I, § 6, no. 1.
Central homothety: II, § 1, no. 2.
Central ring homomorphism: II, § 5, no. 3.
Central series, lower: I, § 6, no. 3.
Centralizer: I, § 5, no. 3.
Centralizer of a subalgebra of an associative algebra: III, § 1, no. 2.
Centralizer of a subset: I, § 1, no. 5.
Centralizer of a subset of a field: II, § 7, no. 7.
Centralizer subalgebra: III, § 1, no. 2.
Centralizing element: I, § 5, no. 3.
Centralizing subset: I, § 5, no. 3.
Centre: I, § 1, no. 5.

Centre of an algebra: III, § 1, no. 2.
Centre of a projective linear mapping: II, § 9, no. 10.
Change of coordinates, formulae of: II, § 10, no. 8.
Characteristic of a field: I, § 9, Exercise 4.
Characteristic polynomial of a matrix: III, § 8, no. 11.
Characteristic subgroup: I, § 5, no. 3.
Class, conjugacy: I, § 5, no. 4.
Class, nilpotency, of a group: I, § 6, no. 3.
Class, solvability, of a group: I, § 6, no. 4.
Coassociative cogebra: III, § 11, no. 2.
Cocommutative bigebra: III, § 11, no. 4.
Cocommutative cogebra: III, § 11, no. 2.
Codiagonal mapping: II, § 1, no. 6.
Codimension of an affine linear variety: II, § 9, no. 3.
Codimension of a vector subspace: II, § 7, no. 3.
Coefficients of a formal power series: III, § 2, no. 11.
Coefficients of a linear combination: II, § 1, no. 1.
Coefficients of a polynomial: III, § 2, no. 9.
Coefficients of a system of linear equations: II, § 2, no. 8.
Cofactor of an element of a square matrix: III, § 8, no. 6.
Cogebra, A-cogebra: III, § 11, no. 1.
Cogebra, anticocommutative graded: III, § 11, no. 3.
Cogebra, coassociative: III, § 11, no. 2.
Cogebra, cocommutative: III, § 11, no. 2.
Cogebra, counital: III, § 11, no. 2.
Cogebra, graded: III, § 11, no. 1.
Cogebra, opposite: III, § 11, no. 1.
Coimage of a linear mapping: II, § 1, no. 3.
Coincidence group: I, § 4, no. 8.
Cokernel of a linear mapping: II, § 1, no. 3.
Column of a matrix: II, § 10, no. 1.
Combination, linear: II, § 2, no. 5.
Combinations, formal linear (module of): II, § 1, no. 11.
Commutation factor: III, § 10, no. 1.
Commutative algebra: III, § 1, no. 1.
Commutative field: I, § 9, no. 1.
Commutative graded bigebra: III, § 11, no. 4.
Commutative group, free, over X: I, § 7, no. 5.
Commutative group with operators: I, § 4, no. 2.
Commutative law: I, § 1, no. 5.
Commutative magma: I, § 1, no. 5.
Commutative monoid, free, over X: I, § 7, no. 7.
Commutative ring: I, § 8, no. 1.

Commutativity relations in a multiplication table: III, § 1, no. 7.
Commutativity theorem: I, § 1, no. 5.
Commutator group: I, § 6, no. 2.
Commutator of two elements: I, § 6, no. 2.
Commute, actions which: I § 5, no. 4.
Commute, elements which: I, § 1, no. 5.
Compatible (equivalence relation) with a law of composition: I, § 1, no. 6.
Compatible (equivalence relation) with an action: I, § 3, no. 3.
Compatible (graduation) with a coproduct: III, § 11, no. 1.
Compatible (graduation) with an algebra structure: III, § 3, no. 1.
Compatible (graduation) with a ring, module, structure: II, § 11, no. 2.
Compatible law of composition and equivalence relation: I, § 1, no. 6.
Compatible, left, right (equivalence relation), with a law of composition: I, § 3, no. 3.
Compatible (mapping) with an action: I, § 3, no. 1.
Compatible (mapping) with the operation of a monoid: I, § 5, no. 1.
Compatible module or multinode structure: II, § 1, no. 14.
Complementary minors: III, § 8, no. 6.
Component, homogeneous, of an element in a graded group: II, § 11, no. 1.
Component of an element in a direct sum: II, § 1, no. 8.
Component of an element with respect to a basis: II, § 1, no. 11.
Component, S-connected: I, § 7, Exercise 18.
Component submodule of a direct sum: II, § 1, no. 6.
Composition in M(X): I, § 7, no. 1.
Composition, law of: I, § 1, no. 1.
Composition of a family with finite support: I, § 2, no. 1.
Composition of an ordered sequence: I, § 1, no. 2.
Composition of the empty family: I, § 2, no. 1.
Composition of words: I, § 7, no. 2.
Composition series: I, § 4, no. 7.
Condition, maximal (resp. minimal) (set of subgroups satisfying the): I, § 4, Exercise 15.
Congruence modulo a rational integer: I, § 4, no. 10.
Congruent (elements) modulo an ideal: I, § 8, no. 7.
Conjugacy class in a group: I, § 5, no. 4.
Conjugate elements in a group: I, § 5, no. 4.
Conjugate elements under the operation of a group: I, § 5, no. 4.
Conjugate subsets in a group: I, § 5, no. 4.
Conjugation, conjugate in a Cayley algebra: III, § 2, no. 4.
Conjugation, conjugate in a quadratic algebra: III, § 2, no. 3.
Constants of structure of an algebra with respect to a basis: III, § 1, no. 7.
Contraction of two indices in a mixed tensor: III, § 5, no. 6.
Contragredient of an invertible square matrix: II, § 10, no. 7.

Contragradient of an isomorphism: II, § 2, no. 5.
Contravariant tensor: III, § 5, no. 6.
Coordinate, barycentric: II, § 9, no. 3.
Coordinate form: II, § 2, no. 6.
Coordinate of an element with respect to a basis: II, § 1, no. 11.
Coordinates, homogeneous (system of), of a point in a projective space: II, § 9, no. 6.
Coordinates of a tensor over M with respect to a basis of M: III, § 5, no. 6.
Coproduct: III, § 11, no. 1.
Coset (right, left) modulo a subgroup: I, § 4, no. 4.
Cotranspose of an endomorphism: III, § 8, no. 6.
Counital cogebra: III, § 11, no. 2.
Counit: III, § 11, no. 2.
Covariant tensor: III, § 5, no. 6.
Cramer formulae, system: III, § 8, no 7.
Cross-ratio: II, § 9, Exercise 11.
Crossed homomorphism: I, § 6, Exercise 7.
Crossed product: III, § 2, Exercise 11.
Cyclic group: I, § 4, no. 10.
Cycle of a permutation: I, § 5, no. 7.

Decomposable $p$-vector: III, § 11, no. 13.
Decomposition, direct, of a ring: I, § 8, no. 11.
Decomposition, reduced decomposition of an element in an amalgamated sum of monoids: I, § 7, no. 3.
Defined (group) by generators and relations: I, § 7, no. 6.
Defined (monoid) by generators and relations: I, § 7, no. 2.
Degree of a homogeneous element in a graded group: II, § 11, no. 1.
Degree of a polynomial with respect to the indeterminates X_j such that $j \in J$: III, § 2, no. 9.
Degree, total degree, of a monomial: III, § 2, no. 9.
Degree, total degree, of an element of a free algebra, of a free associative algebra: III, § 2, no. 7.
Degree, total degree, of a polynomial: III, § 2, no. 9.
Denominator: I, § 2, no. 4.
$\varepsilon$-derivation, inner: III, § 10, no. 6.
Derivation, K-derivation: III, § 10, no. 2.
(K, $\varepsilon$)-derivation of degree $\delta$, $\varepsilon$-derivation of degree $\delta$: III, § 10, no. 2.
$\varepsilon$-derivation of a graded algebra, $\varepsilon$-derivation of a ring: III, § 10, no. 2.
Derivation of a ring A into a ring B: III, § 10, no. 2.
Derivative, partial: III, § 10, no. 11.
Derived (element) from an element of the free algebra by substituting elements for the indeterminates: III, § 2, no. 8.

Derived (element) from an element of the free associative algebra by substituting elements for the indeterminates: III, § 2, no. 8.
Derived group of a group: I, § 6, no. 2.
Derived (left action, right action) from a law of composition: I, § 3, no. 1.
Derived series of a group: I, § 6, no. 4.
Determinant, Cauchy: III, § 8, Exercise 5.
Determinant of a matrix: III, § 8, no. 3.
Determinant of an endomorphism: III, § 8, no. 1.
Determinant of a sequence of vectors: III, § 8, no. 1.
Determinant, Vandermonde: III, § 8, no. 6.
Diagonal elements of a square matrix: II, § 10, no. 7.
Diagonal matrix of matrices: II, § 10, no. 7.
Diagonal of a square matrix, diagonal matrix: II, § 10, no. 7.
Diagram, exact: II, § 1, no. 4.
Differences, group of: I, § 2, no. 4.
Differences, monoid of: I, § 2, no. 4.
K-differential: III, § 10, no. 11.
Differential of an element: III, § 10, no. 11.
Dihedral group: I, § 6, Exercise 4.
Dilatation: II, § 10, Exercise 11.
Dimension of a free module: II, § 7, no. 2.
Dimension of an affine linear variety: II, § 9, no. 3.
Dimension of an affine space: II, § 9, no. 1.
Dimension of a projective space: II, § 9, no. 5.
Dimension of a vector space: II, § 7, no. 2.
Dimorphism: II, § 1, no. 13.
Direct decomposition of a ring: I, § 8, no. 11.
Direct factor: I, § 4, no. 9.
Direct limit: see Limit, direct.
Direct product: I, § 4, no. 9.
Direct product, internal: I, § 4, no. 9.
Direct sum: I, § 4, no. 9.
Direct system: see System direct.
Direction of an affine linear variety: II, § 9, no. 3.
Direction parameters of an affine line: II, § 9, no. 3.
Direction vector of an affine line: II, § 9, no. 3.
Discriminant ideal of an algebra: III, § 9, no. 5.
Discriminant of a finite sequence in an algebra: III, § 9, no. 5.
Distributive action: I, § 3, no. 4.
Distributive, left distributive, right distributive, law: I, § 3, no. 4.
Distributive (mapping) with respect to an index: I, § 3, no. 4.
Distributivity of one law of composition with respect to another: I, § 3, no. 5.
Divisor, left, right: I, § 8, no. 1.

Divisor of zero, left, right: I, § 8, no. 1.
Domain, integral, domain of integrity: I, § 9, no. 2.
Double coset with respect to two subgroups: I, § 5, no. 4.
Dual bases: II, § 2, nos. 6 and 7.
Dual, graded, of a graded module: II, § 11, no. 6.
Dual numbers, algebra of: III, § 2, no. 3.
Dual of a module: II, § 2, no. 3.

Element, central: I, § 1, no. 5.
Element centralizing a subset: I, § 5, no. 3.
Element derived from an element of the free algebra by substituting elements for indeterminates: III, § 2, no. 8.
Element derived from an element of the free associative algebra by substituting elements for indeterminates: III, § 2, no. 8.
Element, free, of a module: II, § 1, no. 11.
Element, homogeneous (homogeneous of degree $n$), of a graded group: II, § 11, no. 1.
Element, identity: I, § 2, no. 1.
Element invariant under an operator: I, § 3, no. 2.
Element, isobaric, of a graded group: II, § 11, no. 1.
Element, left cancellable, right cancellable, cancellable: I, § 2, no. 2.
Element, left invertible, right invertible, invertible: I, § 2, no. 3.
Element, left regular, right regular, regular: I, § 2, no. 2.
Element normalizing a subset: i, § 5, no. 3.
Element, $p$-regular: I, § 6, Exercise 28.
Element, $p$-unipotent: I, § 6, Exercise 28.
Element, primitive, in a free group: I, § 7, Exercise 26.
Element, primitive, of a graded bigebra: III, § 11, no. 8.
Element resulting from substituting elements for indeterminates in a free group: I, § 7, no. 5.
Element, s-neighbouring: I, § 7, Exercise 18.
Element, torsion, of a module: II, § 7, no. 10.
Element, unit: I, § 2, no. 1.
Element, unit, of an algebra: III, § 1, no. 1.
Element, zero: I, § 2, no. 1.
Elements congruent modulo an ideal: I, § 8, no. 7.
Elements, conjugate, in a group: I, § 5, no. 4.
Elements, conjugate, under the operation of a group: I, § 5, no. 4.
Elements, diagonal, of a square matrix: II, § 10, no. 7.
Elements, linearly dependent (linearly independent) in a module: II, § 1, no. 11.
Elements, orthogonal: II, § 2, no. 4.
Elements, permutable, elements which commute: I, § 1, no. 5.

Empty matrix: II, § 10, no. 1.
Endomorphism: I, § 1, no. 1.
Endomorphism of a module: II, § 1, no. 2.
Endomorphism of a ring: I, § 8, no. 4.
Endomorphism, unimodular: III, § 8, no. 1.
Endomorphisms, equivalent, similar: III, § 8, Exercise 26.
Ends, number of ends: I, § 7, Exercise 37.
Envelope, injective, of a module: II, § 2, no. 1.
Equation, linear, homogeneous linear equation, homogeneous linear equation associated with a linear equation: II, § 2, no. 8.
Equation of a hyperplane: II, § 7, no. 5.
Equation, scalar linear: II, § 2, no. 8.
Equations, linear (system of): II, § 2, no. 8.
Equations (system of) of a vector subspace: II, § 7, no. 5.
Equivalent composition series: I, § 4, no. 7.
Equivalent endomorphisms: III, § 8, Exercise 26.
Equivalent matrices: II, § 10, no. 9.
Even permutation: I, § 5, no. 7.
Exact diagram: II, § 1, no. 4.
Exact sequence: II, § 1, no. 4.
Expansion by a column: III, § 8, no. 6.
Expansion by a row: III, § 8, no. 6.
Expansion, Laplace: III, § 8, no. 6.
Extension, Cayley, of an algebra: III, § 2, no. 5.
Extension, central: I, § 6, no. 1.
Extension, essential, of a module: II, § 2, Exercise 15.
Extension of laws of operation: I, § 5, no. 1.
Extension of one group by another: I, § 6, no. 1.
Extension of one module by another: II, § 1, no. 4.
Extension of scalars (module obtained by): II, § 5, no. 1.
Extension of scalars (algebra obtained by): III, § 1, no. 5.
Extension, trivial: I, § 6, no. 1.
Extension, trivial, of a module: II, § 1, no. 9.
Exterior algebra of a module: III, § 7, no. 1.
Exterior power, $p$-th, of an endomorphism: III, § 7, no. 4.
Exterior power, $p$-th, of a matrix: III, § 8, no. 5.
Exterior power, $p$-th, of a module: III, § 7, no. 4.
Exterior product of a $p$-vector and a $q$-vector: III, § 7, no. 1.
External law of composition: I, § 3, no. 1.

Factor, direct, of a group: I, § 4, no. 9.
Factor, direct, of a module: II, § 1, no. 9.
Factor of a product: I, § 1, no. 2.

Factors, system of: III, § 2, Exercise 11.
Faithfully (monoid operating): I, § 5, no. 1.
Faithful module: III, § 1, no. 12.
Family, affinely free, affinely related, of points in an affine space: II, § 9, no. 3.
Family, basic, free, generating, in a group: I, § 7, no. 6.
Family, free, related, of elements of a module: II, § 1, no. 11.
Family, generating, of an algebra: III, § 1, no. 2.
Family, orthogonal, of projectors: II, § 1, no. 8.
Family, projectively free, projectively related, of points in a projective space: II, § 9, no. 7.
Fibre product: I, § 4, no. 8.
Field: I, § 9, no. 1.
Field, commutative, skew field: I, § 9, no. 1.
Field of fractions of an integral domain: I, § 9, no. 2.
Field of left fractions: I, § 9, Exercise 15.
Field of rational numbers: I, § 9, no. 4.
Field, projective: II, § 9, no. 9.
Finer composition series: I, § 4, no. 7.
Finite group: I, § 4, no. 1.
Finitely generated group: I, § 7, Exercise 16.
Finitely generated module: II, § 1, no. 7.
Fixer of a subset of a set: I, § 5, no. 2.
Fixing a subset of a set (operator, set of operators): I, § 5, no. 2.
Form, canonical bilinear: II, § 2, no. 3.
Form, coordinate: II, § 2, no. 6.
Form, linear: II, § 2, no. 3.
Form, $n$-linear: II, § 3, no. 9.
$n$-form: III, § 11, no. 7.
Formula, binomial: I, § 8, no. 2.
Formula, Leibniz: III, § 10, no. 4.
Formulae, Cramer’s: III, § 8, no. 7.
Formulae of change of coordinates: II, § 10, no. 8.
Formulae, transitivity, of norms and traces: III, § 9, no. 4.
Fractions (field of) of an integral domain: I, § 9, no. 2.
Fractions, group of, of a monoid: I, § 2, no. 4.
Fractions, monoid of, with denominators in S: I, § 2, no. 4.
Fractions, ring of, with denominators in S: I, § 8, no. 12.
Fractions, total ring of: I, § 8, no. 12.
Free algebra, associative algebra, associative and commutative algebra: III, § 2, no. 7.
Free algebra of a module: III, § 2, Exercise 13.
Free commutative group: I, § 7, no. 5.

Free commutative monoid: I, § 7, no. 7.
Free element, family, module, subset, system: II, § 1, no. 11, and (by an abuse of language) II, § 9, no. 7.
Free family in a group: I, § 7, no. 6.
Free group: I, § 7, no. 5.
Free magma: I, § 7, no. 1.
Free monoid: I, § 7, no. 2.
Free product of algebras: III, § 5, Exercise 6.
Free product of groups: I, § 7, no. 3.
Free vector in an affine space: II, § 9, no. 1.
Freely, group operating: I, § 5, no. 4.
Function, linearly affine, affine function: II, § 9, no. 4.

Generated by a family of ordered pairs (equivalent relation): I, § 1, no. 6.
Generated by a subset (ideal): I, § 8, no. 6, and III, § 1, no. 2.
Generated by a subset (stable subgroup): I, § 4, no. 3.
Generated by a subset (stable subset): I, § 1, no. 4.
Generated by a subset (subalgebra): III, § 1, no. 2.
Generated by a subset (subfield): I, § 9, no. 1.
Generated by a subset (submagma): I, § 1, no. 4.
Generated by a subset (subring): I, § 8, no. 5.
Generated by a subset (unital submagma, submonoid): I, § 2, no. 1.
Generating family of a group: I, § 7, no. 6.
Generating family of an algebra: III, § 1, no. 2.
Generating set, system, of a field: I, § 9, no. 1.
Generating set, system, of a magma: I, § 1, no. 4.
Generating set, system, of a module: II, § 1, no. 7.
Generating set, system, of an ideal: I, § 8, no. 6.
Generating set, system, of a ring: I, § 8, no. 5.
Generating set, system, of a stable subgroup: I, § 4, no. 3.
Generating set, system, of a stable subset: I, § 1, no. 4.
Generating set, system, of a unital submagma, of a submonoid: I, § 2, no. 1.
Generators of a presentation: I, § 7, no. 6.
Graded algebra over a graded ring: III, § 3, no. 1.
Graded bigebra: III, § 11, no. 4.
Graded bigebra, skew: III, § 11, no. 4.
Graded cogebrba: III, § 11, no. 1.
Graded group, module, ring: II, § 11, nos. 1 and 2.
Graded homomorphism: II, § 11, no. 2.
Graded subalgebra: III, § 3, no. 2.
Graded subring, submodule, ideal: II, § 11, no. 3.
Graded tensor product of type $\Delta_0$: III, § 4, no. 8.

Graduation compatible with a coproduct: III, § 11, no. 1.
Graduation compatible with an algebra structure: III, § 3, no. 1.
Graduation induced, quotient graduation: II, § 11, no. 3.
Graduation of type Δ: II, § 11, no. 1.
Graduation, partial, total graduation: II, § 11, nos. 1 and 2.
Graduation, trivial: II, § 11, no. 1.
Grassmannian: III, § 11, no. 13.
Grassmann relations: III, § 11, no. 13.
Greatest common divisor (g.c.d.) of two integers: I, § 8, no. 11.
Group: I, § 2, no. 3.
Group, additive, of a ring: I, § 8, no. 1.
Group, affine: I, § 9, no. 4.
Group, alternating: I, § 5, no. 7.
Group, bicyclic: I, § 6, Exercise 26.
Group, bigraded: II, § 11, no. 2.
Group, coincidence, of two homomorphisms: I, § 4, no. 8.
Group commutator: I, § 6, no. 2.
Group, cyclic: I, § 4, no. 10.
Group defined by generators and relations: I, § 7, no. 6.
Group, derived: I, § 6, no. 2.
Group, dihedral: I, § 6, Exercise 4.
Group, finite, infinite group: I, § 4, no. 1.
Group, finitely generated: I, § 7, Exercise 16.
Group, finitely presented: I, § 7, Exercise 16.
Group, free commutative, over a set: I, § 7, no. 7 and II, § 1, no. 11.
Group, free, over a set: I, § 7, no. 5.
Group, graded: II, § 11, no. 1.
Group, linear: II, § 2, no. 6.
Group, minimal simple: I, § 6, Exercise 27.
Group, monogenous: I, § 4, no. 10.
Group, multiplicative, of a ring: I, § 8, no. 1.
Group, nilpotent, nilpotent group of class $n$: I, § 6, no. 3.
Group of differences, group of fractions: I, § 2, no. 4.
Group of exponential type: I, § 7, Exercise 39.
Group operating faithfully: I, § 5, no. 1.
Group operating freely: I, § 5, no. 4.
Group operating simply transitively: I, § 5, no. 6.
Group operating transitively: I, § 5, no. 5.
$p$-group: I, § 6, no. 5.
Group, projective: II, § 9, no. 10.
Group, residually finite: I, § 5, Exercise 5.
Group, solvable, solvable group of class $n$: I, § 6, no. 4.
Group, special linear: III, § 8, no. 9.

Group, supersolvable: I, § 6, Exercise 26.
Group, symmetric: I, § 4, no. 1.
Group, unimodular: III, § 8, no. 9.
Group with operators, Abelian, commutative: I, § 4, no. 2.
Group with operators: I, § 4, no. 2.
Group with operators, product: I, § 4, no. 8.
Group with operators, product (or internal product), of a family of quotient groups: I, § 4, no. 8.
Group with operators, quotient: I, § 4, no. 4.
Group with operators, simple: I, § 4, no. 4.
Groupoid: I, § 4, Exercise 23.

Hall’s Theorem: I, § 6, Exercise 10.
Hamel basis: II, § 7, no. 1.
Hamiltonian quaternions: III, § 2, no. 5.
Homogeneous element in a graded group: II, § 11, no. 1.
Homogeneous G-set: I, § 5, no. 5.
Homogeneous linear equation, linear system: II, § 2, no. 8.
Homogeneous subset of degree $p$ in a formal power series: III, § 2, no. 11.
Homogeneous subset of degree $p$ with respect to certain indeterminates in a formal power series: III, § 2, no. 11.
Homomorphism, algebra: III, § 1, no. 1.
Homomorphism, A-module, A-homomorphism: II, § 1, no. 2.
Homomorphism, central ring: II, § 5, no. 3.
Homomorphism, crossed: I, § 6, Exercise 7.
Homomorphism, essential: II, § 2, Exercise 15.
Homomorphism for two laws of composition: I, § 1, no. 1.
Homomorphism, graded: II, § 11, no. 2.
Homomorphism, graded algebra: III, § 3, no. 1.
Homomorphism, group: I, § 4, no. 1.
Homomorphism, monoid: I, § 2, no. 1.
Homomorphism, M-set: I, § 5, no. 1.
Homomorphism, multinode: II, § 1, no. 14.
Homomorphism of groups with operators: I, § 4, no. 2.
$\phi$-homomorphism: I, § 3, no. 1.
Homomorphism, projection: I, § 4, no. 8.
Homomorphism, ring: I, § 8, no. 4.
Homomorphism, trivial: I, § 2, no. 1.
Homomorphism, unital: I, § 2, no. 1.
Homomorphism, unital algebra: III, § 1, no. 1.
Homothety: I, § 4, no. 2 and II, § 1, no. 1.
Homothety, central: II, § 1, no. 2 and III, § 9, Exercise 6.
Hyperplane, affine: II, § 9, no. 3.

Hyperplane at infinity: II, § 9, no. 8.
Hyperplane passing through 0 in a vector space: II, § 7, no. 3.
Hyperplane, projective: II, § 9, no. 7.
Hyperplane, projective, taken as hyperplane at infinity: II, § 9, no. 10.

Ideal, discriminant: III, § 9, no. 5.
Ideal, graded: II, § 11, no. 3 and III, § 3, no. 2.
Ideal, irreducible two-sided: I, § 8, Exercise 11.
Ideal, left, right ideal, two-sided ideal in an algebra: III, § 1, no. 2.
Ideal, left, right ideal, two-sided ideal in a ring: I, § 8, no. 6.
Ideal, maximal: I, § 8, no. 6.
Ideal, prime: I, § 9, no. 3.
Ideal, principal: I, § 8, no. 6.
Ideal of relators: III, § 2, no. 8.
Ideal, zero: I, § 8, no. 6.
Idempotent: I, § 1, no. 4.
Identities, Jacobi, between minors of a determinant: III, § 11, Exercise 9.
Identities, polynomials: III, § 2, no. 9.
Identity element: I, § 2, no. 1.
Identity, Jacobi: III, § 10, no. 6.
Identity, Redei: III, § 8, Exercise 25.
Image (inverse image) of a projective linear variety under a projective mapping: II, § 9, no. 10.
Image of a homomorphism: II, § 1, no. 3.
Indeterminate, indeterminate of index i: I, § 7, no. 5 and III, § 2, no. 7.
Index of a subgroup: I, § 4, no. 4.
Induced action: I, § 3, no. 2.
Induced graduation: II, § 11, no. 3.
Induced K'-structure: II, § 8, no. 1.
Induced law: I, § 1, no. 4.
Infinity, hyperplane at: II, § 9, no. 8.
Infinity, points at: II, § 9, no. 8.
Inner automorphism of a group: I, § 5, no. 3.
Inner automorphism of a ring: I, § 8, no. 4.
Inner product, left, right: III, § 11, nos. 6 and 7.
Integer, negative, positive, strictly negative, strictly positive: I, § 2, no. 5.
Integer, rational: I, § 2, no. 5.
Integers, rational, modulo a (ring of): I, § 8, no. 11.
Integers, relatively prime: I, § 8, no. 11.
Integral domain: I, § 9, no. 2.
Integrity, domain of: I, § 9, no. 2.
Internal direct product, restricted sum: I, § 4, no. 9.
Invariant element: I, § 5, no. 2.

Invariant subgroup, stable subgroup: I, § 4, no. 4.
Inverse, left inverse, right inverse, element: I, § 2, no. 3.
Inverse, left, right inverse, of a linear mapping: II, § 1, no. 9.
Inverse limit: see Limit, inverse.
Inverse system: see System, inverse.
Inversion in a bigebra: III, § 11, Exercise 4.
Inversion of a permutation: I, § 5, no. 7.
Invertible, left invertible, right invertible, element: I, § 2, no. 3.
Invertible, left, right invertible, linear mapping: II, § 1, no. 9.
Invertible square matrix: II, § 10, no. 7.
Irreducible ideal: I, § 8, Exercise 11.
Isobaric element: II, § 11, no. 1.
Isomorphic magmas: I, § 1, no. 1.
Isomorphism, magma: I, § 1, no. 1.

Jacobi identity: III, § 10, no. 6.
Jordan-Hölder series: I, § 4, no. 7.
Jordan-Hölder Theorem: I, § 4, no. 7.
Juxtaposition: I, § 7, no. 2.

Kernel of a group homomorphism: I, § 4, no. 5.
Kernel of a linear mapping: II, § 1, no. 3.
Kronecker symbol: II, § 1, no. 11.
Krull’s Theorem: I, § 8, no. 6.

Laplace expansion: III, § 8, no. 6.
Law and equivalence relation, compatible: I, § 1, no. 6.
Law, associative: I, § 1, no. 3.
Law, commutative: I, § 1, no. 5.
Law, group: I, § 4, no. 1.
Law, induced: I, § 1, no. 4.
Law, left distributive, right distributive, distributive with respect to another I, § 3, nos. 4 and 5.
Law not everywhere defined: I, § 1, no. 1.
Law of composition: I, § 1, no. 1.
Law of left, right, operation of a monoid on a set: I, § 5, no. 1.
Law of right, left action associated with an action: I, § 3, no. 1.
Law, opposite: I, § 1, no. 1.
Law, quotient: I, § 1, no. 6.
Law written additively, multiplicatively: I, § 1, no. 1.
Least common multiple (l.c.m.) of two integers: I, § 8, no. 11.
Leibniz formula: III, § 10, no. 4.
Lemma, Zassenhaus’s: I, § 4, no. 7.

Length of a decomposition in an amalgamated sum: I, § 7, no. 3.
Length of a group: I, § 4, no. 7.
Length of a module: II, § 1, no. 10.
Length of an element in a free group: I, § 7, Exercise 19.
Length of an element in a free magma: I, § 7, no. 1.
Length of a word: I, § 7, no. 2.
Limit, direct, of $A_\alpha$-algebras: III, § 1, no. 6.
Limit, direct, of $A_\alpha$-modules: II, § 6, no. 2.
Limit, direct, of actions: I, § 10, no. 4.
Limit, direct, of graded algebras: III, § 3, no. 3.
Limit, direct, of groups, of groups with operators, of monoids: I, § 10, no. 3.
Limit, direct, of magmas: I, § 10, no. 3.
Limit, direct, of rings: I, § 10, no. 3.
Limit, inverse, of $A_\alpha$-algebras: III, § 1, no. 6.
Limit, inverse, of $A_\alpha$-modules: II, § 6, no. 1.
Limit, inverse, of groups, of groups with operators, of monoids: I, § 10, no. 1.
Limit, inverse, of magmas: I, § 10, no. 1.
Limit, inverse, of rings: I, § 10, no. 1.
Line, affine: II, § 9, nos. 1 and 3.
Line (passing through 0) in a vector space: II, § 7, no. 3.
Line, projective: II, § 9, no. 5.
Linear equation, system: II, § 2, no. 8.
Linear equation, system, homogeneous: II, § 2, no. 8.
Linear form: II, § 2, no. 3.
Linear group: II, § 2, no. 6.
Linear group, special: III, § 8, no. 9.
Linear mapping: II, § 1, no. 2.
Linear mapping, function, affine: II, § 9, no. 4.
Linear mapping, projective: II, § 9, no. 10.
Linear problem: II, § 2, no. 8.
Linear variety: II, § 9, nos. 3, 7 and 11.
Linear variety, affine: II, § 9, no. 3.
Linear variety, projective: II, § 9, nos. 7 and 11.
Linearly dependent, linear independent, elements: II, § 1, no. 11.
Linearly disjoint subalgebras: III, § 4, no. 4.
Linearity, principle of extension by: II, § 1, no. 7.

Magma: I, § 1, no. 1.
Magma, associative: I, § 1, no. 3.
Magma, commutative: I, § 1, no. 5.
Magma, defined by generators and relations: I, § 7, no. 1.
Magma, free, over a set: I, § 7, no. 1.
Magma of mappings into a magma: I, § 1, no. 1.

Magma, opposite: I, § 1, no. 1.
Magma, product: I, § 1, no. 1.
Magma, quotient: I, § 1, no. 6.
Magma, unital: I, § 2, no. 1.
Magmas, isomorphic: I, § 1, no. 1.
Mapping, affine linear, affine: II, § 9, no. 4.
Mapping, alternating multilinear: III, § 7, no. 4.
Mapping, biadditive, $\mathbf{Z}$-bilinear: II, § 3, no. 1.
Mapping, C-bilinear: II, § 3, no. 5.
Mapping compatible with an action: I, § 3, no. 1.
Mapping compatible with the operation of a monoid: I, § 5, no. 1.
Mapping distributive with respect to a variable: I, § 3, no. 4.
Mapping, linear, A-linear: II, § 1, no. 2.
Mapping, linear, $A_s(T) \to E$ determined by a mapping $T \to E$: II, § 1, no. 11.
Mapping, linear, associated with an affine mapping: II, § 9, no. 4.
Mapping, multiadditive, $\mathbf{Z}$-multilinear: II, § 3, no. 9.
Mapping, C-multilinear: II, § 3, no. 9.
Mapping, orbital: I, § 5, no. 4.
Mapping, projective linear, projective: II, § 9, no. 10.
Mapping, right invertible linear, left invertible linear: II, § 1, no. 9.
Mapping, semi-linear: II, § 1, no. 13.
Mapping, symmetric multilinear: III, § 6, no. 3.
Matrices differing only by the order of the columns, rows: II, § 10, no. 9.
Matrices, equivalent: II, § 10, no. 9.
Matrices, similar square: II, § 10, no. 9.
Matrix, contragredient, of an invertible matrix: II, § 10, no. 7.
Matrix, diagonal: II, § 10, no. 7.
Matrix, empty: II, § 10, no. 1.
Matrix, invertible: II, § 10, no. 7.
Matrix, lower triangular, upper triangular: II, § 10, no. 7.
Matrix, matrix of type $(p, q)$: II, § 10, no. 1.
Matrix, monomial: II, § 10, no. 7.
Matrix obtained by bordering a matrix: II, § 10, no. 1.
Matrix obtained by suppressing columns, rows: II, § 10, no. 1.
Matrix of a linear mapping with respect to two bases: II, § 10, no. 4.
Matrix of a linear system: II, § 10, no. 4.
Matrix of an element with respect to a basis: II, § 10, no. 4.
Matrix of an endomorphism with respect to a basis: II, § 10, no. 7.
Matrix of a permutation: II, § 10, no. 7.
Matrix of a semi-linear mapping with respect to two bases: II, § 10, no. 6.
Matrix of passing from one basis to another: II, § 10, no. 8.
Matrix, scalar: II, § 10, no. 7.

Matrix, square, square matrix of order $n$: II, § 10, no. 7.
Matrix, unimodular: III, § 8, no. 4.
Matrix units: II, § 10, no. 3.
Matrix with only zeros below (above) the diagonal: II, § 10, no. 7.
Matrix, zero: II, § 10, no. 2.
Maximal ideal: I, § 8, no. 6.
G-mean: I, § 6, Exercise 8.
Minimal normal stable subgroups: I, § 4, Exercise 15.
Minimal simple group: I, § 6, Exercise 27.
Minor, minor of order $p$ of a matrix: III, § 8, no. 5.
Minors, complementary: III, § 8, no. 6.
Mixed tensor: III, § 5, no. 6.
Module, bigraded: II, § 11, no. 2.
Module, divisible: II, § 7, Exercise 33.
Module, dual: II, § 2, no. 3.
Module, faithful: II, § 1, no. 12.
Module, faithful, associated with a module: II, § 1, no. 12.
Module, free: II, § 1, no. 11.
Module, graded free: II, § 11, no. 2.
Module, graded, graded module with positive degrees: II, § 11, no. 2.
Module, graded quotient: II, § 11, no. 3.
Module, indecomposable: II, § 2, Exercise 21.
Module, injective: II, § 2, Exercise 11.
Module, left, right module, A-module: II, § 1, no. 1.
Module, monogeneus: II, § 1, no. 12.
Module of finite length: II, § 1, no. 10.
Module of formal linear combinations: II, § 1, no. 11.
Module of linear relations: II, § 1, no. 11.
Module over an algebra: III, § 4, no. 3.
Module, product: II, § 1, no. 5.
Module, projective: II, § 2, no. 2.
Module, quotient: II, § 1, no. 3.
Module, reflexive: II, § 2, no. 7.
Module, torsion-free, over an integral domain: II, § 7, no. 10.
Module, torsion, over an integral domain: II, § 7, no. 10.
Monogeneus group: I, § 4, no. 10.
Monogenous module: II, § 1, no. 2.
Monoid: I, § 2, no. 1.
Monoid defined by generators and relations: I, § 7, no. 2.
Monoid, free, over a set: I, § 7, no. 2.
Monoid of differences: I, § 2, no. 4.
Monoid of fractions with denominators in S: I, § 2, no. 4.
Monoid operating faithfully on a set: I, § 5, no. 1.

Monoidal sum: I, § 7, no. 3.
Monomial: III, § 2, no. 9.
Morphism, algebra: III, § 1, no. 1.
Morphism, A-module: II, § 1, no. 2.
Morphism, cogebra: III, § 11, no. 1.
Morphism, graded bigebra, left graded bigebra morphism: III, § 11, no. 4.
Morphism, graded cogebra: III, § 11, no. 1.
Morphism, magma: I, § 1, no. 1.
Morphism, monoid: I, § 2, no. 1.
Morphism of extensions: I, § 6, no. 1.
Morphism, ring: I, § 8, no. 4.
Morphism, unital algebra: III, § 4, no. 5.
Morphism, unital magma: I, § 2, no. 1.
ϕ-morphism (ϕ a homomorphism of one monoid of operators into another):
    I, § 5, no. 1.
ϕ-morphism (ϕ a mapping of one set of operators into another): I, § 3, no. 1.
M-morphism (M a monoid of operators): I, § 5, no. 1.
Ω-morphism (Ω a set of operators): I, § 3, no. 1.
Multiadditive, Z-multilinear, mapping: II, § 3, no. 9.
Multidegree in the free algebra of a monoid: III, § 2, Exercise 13.
Multiindex: I, § 7, no. 7.
Multilinear form: II, § 3, no. 9.
C-multilinear mapping: II, § 3, no. 9.
Multimodule: II, § 1, no. 14.
Multimodule, quotient: II, § 1, no. 14.
Multiple, left, right: I, § 8, no. 1.
Multiplication: I, § 1, no. 1.
Multiplication in an algebra. III, § 1, no. 1.
Multiplication table: III, § 1, no. 7.
Multiplicative group of a ring: I, § 8, no. 1.

Negative of an element: I, § 2, no. 3.
Negative rational integer: I, § 2, no. 5.
Negative rational number: I, § 9, no. 4.
S-neighbouring element: I, § 7, Exercise 18.
Nielson-Schreier Theorem: I, § 7, Exercise 20.
Nilpotent group, nilpotent group of class n: I, § 6, no. 3.
Norm, Cayley: III, § 2, no. 4.
Norm in a quadratic algebra: III, § 2, no. 3.
Norm of an element in a K-algebra relative to K: III, § 9, no. 3.
Norm of a scalar relative to a module: III, § 9, no. 1.
Normal stable subgroup: I, § 4, no. 4.

Normal subgroup: I, § 4, no. 4.
Normalizer: I, § 5, no. 3.
Normalizing (element, subset) a subset: I, § 5, no. 3.
Null element: I, § 2, no. 1.
Number, prime: I, § 4, no. 10.
Number, rational: I, § 9, no. 4.
Number (rational), negative, positive, strictly negative, strictly positive: I, § 9, no. 4.
Numerator: I, § 2, no. 4.

Octonions, Cayley: III, Appendix, no. 3.
Octonions of type ($\alpha, \beta, \gamma, \delta$) (algebra of): III, Appendix, no. 3.
Odd permutation: I, § 5, no. 7.
Operation by left, right, translation: I, § 5, no. 1.
Operation, left, right (laws of): I, § 5, no. 1.
Operation, left, right, of a monoid: I, § 5, no. 1.
Operation, simply transitive: I, § 5, no. 6.
Operation, transitive: I, § 5, no. 5.
Operation, trivial: I, § 5, no. 2.
Operator: I, § 3, no. 1.
Opposite algebra: III, § 1, no. 1.
Opposite cogebra: III, § 11, no. 1.
Opposite law: I, § 1, no. 1.
Opposite magma: I, § 1, no. 1.
Opposite to an M-set, $M^0$-set: I, § 5, no. 1.
Opposite ring: I, § 8, no. 3.
Orbit: I, § 5, no. 4.
Orbital mapping: I, § 5, no. 4.
Order, element of infinite: I, § 4, no. 10.
Order of a cycle: I, § 5, no. 7.
Order of a formal power series with respect to certain indeterminates: III, § 2, no. 11.
Order of a group: I, § 4, no. 1.
Order of an element in a group: I, § 4, no. 10.
Order of a square matrix: II, § 10, no. 7.
Order, total order, of a formal power series: III, § 2, no. 11.
Ordered sequence: I, § 1, no. 2.
Ordered sequences, similar: I, § 1, no. 2.
Origin: I, § 2, no. 1.
Origin, choice of, in an affine space: II, § 9, no. 1.
Orthogonal elements, sets: II, § 2, no. 3.
Orthogonal family of projectors: II, § 1, no. 8.
Orthogonal, submodule, to a subset of E (resp. E$^*$): II, § 2, no. 4.

Parallel linear varieties: II, § 9, no. 3.
Parallelogram: II, § 9, Exercise 1.
Parameters, direction, of an affine line: II, § 9, no. 3.
Partial derivative: III, § 10, no. 11.
Partial graduation: II, § 11, no. 1.
Passage, matrix of: II, § 10, no. 8.
Permutable elements: I, § 1, no. 5.
Permutation, even, odd: I, § 5, no. 7.
Plane, affine: II, § 9, nos. 1 and 3.
Plane passing through 0 in a vector space: II, § 7, no. 3.
Plane, projective: II, § 9, no. 5.
Point of an affine space: II, § 9, no. 1.
Point of a projective space: II, § 9, no. 5.
Points, affinely independent: II, § 9, no. 3.
Points at infinity: II, § 9, no. 8.
Polynomial, characteristic, of an element in a K-algebra: III, § 9, no. 3.
Polynomial, characteristic, of an endomorphism: III, § 8, no. 11.
Polynomial, characteristic, of a scalar with respect to a module: III, § 9, no. 1.
Polynomial containing no term in X^v: III, § 2, no. 9.
Polynomial identities: III, § 2, no. 9.
Polynomial of degree n: III, § 2, no. 9.
Polynomial relators: III, § 2, no. 9.
Polynomial with no constant term: III, § 2, no. 9.
Polynomial with respect to a family of indeterminates, with coefficients in a ring: III, § 2, no. 9.
Positive rational integer: I, § 2, no. 5.
Positive rational number: I, § 9, no. 4.
Power, exterior, of a linear mapping: III, § 7, no. 4.
Power, exterior, of a matrix: III, § 8, no. 5.
Power, exterior, of a module: III, § 7, no. 4.
Power, n-th, under an associative law: I, § 1, no. 3.
Power, symmetric, of a linear mapping, of a module: III, § 6, no. 3.
Power, tensorial, of a linear mapping: III, § 5, no. 2.
Power, tensorial, of a module: III, § 5, no. 1.
Presentation of a group: I, § 7, no. 6.
Presentation of an algebra: III, § 2, no. 8.
Presented, finitely (group): I, § 7, Exercise 16.
Preservation when passing to the quotient: I, § 1, no. 6.
Prime ideal: I, § 9, no. 3.
Prime number: I, § 4, no. 10.
Prime, relatively (integers): I, § 8, no. 10.
Primitive element in a free group: I, § 7, Exercise 26.

Primitive element in a free magma generated by a single element: I, § 7, Exercise 7.
Primitive element of a graded bigebra: III, § 11, no. 8.
Principal G-set, homogeneous: I, § 5, no. 6.
Principal ideal: I, § 8, no. 6.
Principal series: I, § 4, Exercise 17.
Principal set under G, homogeneous: I, § 5, no. 6.
Principle of extension by linearity: II, § 1, no. 7.
Problem, linear: II, § 2, no. 8.
Product algebra: III, § 1, no. 4.
Product, block, of matrices: II, § 10, no. 5.
Product, crossed: III, § 2, Exercise 11.
Product, exterior, of a $p$-vector and a $q$-vector: III, § 7, no. 1.
Product, external semi-direct, of G by F relative to $\tau$: I, § 6, no. 1.
Product, fibre, of groups with operators: I, § 4, no. 8.
Product, fibre, of modules: II, § 1, Exercise 4.
Product, free, of algebras: III, § 5, Exercise 6.
Product, free, of groups: I, § 7, no. 5.
Product, graded tensor, of two graded modules: II, § 11, no. 5.
Product, graded tensor, of graded algebras: III, § 4, nos. 7 and 9.
Product group, internal product group, of a family of quotient groups: I, § 4, no. 8.
Product group with operators: I, § 4, no. 8.
Product, internal direct, direct product, product, of subgroups: I, § 4, no. 9.
Product magma: I, § 1, no. 1.
Product of K'-structures: II, § 8, no. 3.
Product of laws of composition: I, § 1, no. 1.
Product of matrices calculated according to a mapping: II, § 10, no. 2.
Product of matrices calculated in a ring: II, § 10, no. 3.
Product of modules: II, § 1, no. 5.
Product of multimodules: II, § 1, no. 14.
Product of an operator and an element: I, § 3, no. 1.
Product of an ordered sequence: I, § 1, no. 2.
Product of two elements: I, § 1, no. 1.
Product of two-sided ideals: I, § 8, no. 9.
Product, (right, left) inner: III, § 11, nos. 6 and 7.
Product ring: I, § 8, no. 10.
Product, symmetric, of multilinear mappings: III, § 11, no. 2.
Product, tensor, of a family of $\mathbf{Z}$-modules relative to a triple $(c, p, q)$: II, § 3, no. 9.
Product, tensor, of algebras: III, § 4, no. 1.
Product, tensor, of an infinite family of algebras: III, § 4, no. 5.
Product, tensor, of bases of algebras: III, § 4, no. 5.

Product, tensor, of cogebras: III, § 11, no. 1.
Product, tensor, of two bases: II, § 3, no. 7.
Product, tensor, of two elements: II, § 3, no. 1.
Product, tensor, of two linear mappings: II, § 3, no. 2.
Product, tensor, of two matrices over a commutative ring: II, § 10, no. 10
Product, tensor, of two modules: II, § 3, no. 1.
Product, tensor, of two multimodules: II, § 3, no. 4.
Product, tensor, of two semi-linear mappings: II, § 3, no. 3.
Projection homomorphism: I, § 4, no. 8.
Projective field: II, § 9, no. 9.
Projective group: II, § 9, no. 10.
Projective hyperplane, plane: II, § 9, no. 7.
Projective line: II, § 9, no. 5.
Projective mapping: II, § 9, no. 10.
Projective module: II, § 2, no. 2.
Projective space: II, § 9, nos. 5 and 11.
Projectively free, projectively related, family: II, § 9, no. 7.
Projector: II, § 1, no. 8.
Pseudomodule, left, right: II, Appendix, no. 2.
Pseudo-ring: I, § 8, no. 1.
Pseudo-ring with zero square: I, § 8, no. 3.
Pure $p$-vector: III, § 11, no. 13.
Pure quaternion: III, § 2, Exercise 3.

Quadratic algebra: III, § 2, no. 3.
Quasi-group: I, § 3, Exercise 6.
Quaternion, pure: III, § 2, Exercise 3.
Quaternion algebra: III, § 2, no. 5.
Quaternionic group: I, § 6, Exercise 4.
Quotient algebra: III, § 1, no. 2.
Quotient graduation: II, § 11, no. 3.
Quotient group with operators: I, § 4, no. 4.
Quotient law: I, § 1, no. 6.
Quotient magma: I, § 1, no. 11.
Quotient module, vector space: II, § 1, no. 3.
Quotient multinode: II, § 1, no. 14.
Quotient of an action: I, § 3, no. 3.
Quotient ring: I, § 8, no. 7.
Quotients of a composition series of a group with operators: I, § 4, no. 7.

Rank of a free group: I, § 7, Exercise 14.
Rank of a linear mapping of vector spaces: II, § 7, no. 4.
Rank of a linear system over a field: II, § 7, no. 6.

Rank of a matrix over a field: II, § 10, no. 12.
Rank of an affine linear mapping: II, § 9, no. 4.
Rank of an element in a tensor product of vector spaces: II, § 7, no. 8.
Rank of a semi-linear mapping of vector spaces: II, § 7, no. 4.
Rank of a subset of a module over an integral domain: II, § 7, no. 10.
Rank of a subset of a vector space: II, § 7, no. 2.
Ratio of a homothety: II, § 1, no. 1.
Rational integer: I, § 2, no. 5.
Rational number: I, § 9, no. 4.
Rational numbers, field of : I, § 9, no. 4.
Rational over a subfield (linear form): II, § 8, no. 4.
Rational over a subfield (linear mapping): II, § 8, no. 3.
Rational over a subfield (subspace, vector): II, § 8, no. 2.
Reduced decomposition of an element of an amalgamated sum: I, § 7, no. 3.
Reflexive module: II, § 2, no. 7.
Regular, left regular, right regular, element: I, § 2, no. 2.
p-regular element: I, § 6, Exercise 28.
Related system, subset: II, § 1, no. 11, and § 9, no. 7.
Relation, equivalence, compatible with a law of composition: I, § 1, no. 6.
Relation, equivalence, compatible with an action: I, § 3, no. 3.
Relation, equivalence, generated by a family of ordered pairs: I, § 1, no. 6.
Relation, equivalence, left, right, compatible with a law of composition: I, § 3, no. 3.
Relations, commutativity, in a multiplication table: III, § 1, no. 7.
Relations, Grassmann: III, § 11, no. 13.
Relations, module of linear: II, § 1, no. 11.
Relatively prime integers: I, § 8, no. 11.
Relator: I, § 7, no. 6 and III, § 2, no. 8.
Relator, universal: III, § 2, no. 8.
Relators, ideal of: III, § 3, no. 8.
Relators of a presentation: I, § 7, no. 6 and III, § 2, no. 8.
Relators, polynomial: III, § 2, no. 9.
Residue of a semi-group: I, § 2, Exercise 11.
Residually finite group: I, § 5, Exdrcise 5.
Restricted algebra of a monoid: III, § 2, no. 10.
Restricted sum, internal: I, § 4, no. 9.
Restricted sum of groups: I, § 4, no. 9.
Restricted sum of groups with respect to subgroups: I, § 4, no. 9.
Restriction of scalars (algebra obtained by): III, § 1, no. 5.
Resulting (element) from substituting elements for indeterminates: I, § 7, no. 5.
Retraction of an extension: I, § 6, no. 1.

Right hand side of a linear equation, right hand sides of a linear system: II, § 2, no. 8.
Ring: I, § 8, no. 1.
Ring, Boolean: I, § 9, Exercise 8.
Ring, commutative: I, § 8, no. 1.
Ring (graded, graded with positive degrees, bigraded): II, § 11, no. 2.
Ring, graded quotient: II, § 11, no. 3.
Ring obtained by the adjunction of a unit element: II, Appendix, no. 1.
Ring of endomorphisms of a commutative group: I, § 8, no. 4.
Ring of fractions with denominators in S: I, § 8, no. 12.
Ring of integers modulo n: I, § 8, no. 11.
Ring of polynomials which are not commutative relative to an endomorphism and a derivation: III, § 10, Exercise 3.
Ring, opposite: I, § 8, no. 3.
Ring, product: I, § 8, no. 10.
Ring, quotient: I, § 8, no. 7.
Ring, total, of fractions: I, § 8, no. 2.
Ring, zero: I, § 8, no. 3.
Row of a matrix: II, § 10, no. 1.
Rule, sign: I, § 8, no. 1.

Scalar: II, § 1, no. 1.
Scalar linear equation: II, § 2, no. 8.
Scalar matrix: II, § 10, no. 7.
Schreier’s Theorem on composition series: I, § 4, no. 7.
Section of an extension: I, § 6, no. 2.
Semi-direct product of groups: I, § 6, no. 1.
Semi-group, left, right: I, § 2, Exercise 11.
Semi-homomorphism, algebra, algebra ρ-homomorphism: III, § 1, no. 5.
Semi-linear mapping: II, § 1, no. 13.
Sequence, exact: II, § 1, no. 4.
Sequence, ordered: I, § 1, no. 2.
Sequence, split exact: II, § 1, no. 9.
Sequences, similar ordered: I, § 1, no. 2.
Series, algebra of formal power: III, § 2, no. 11.
Series, composition: I, § 4, no. 6.
Series, derived: I, § 6, no. 4.
Series, equivalent decomposition: I, § 4, no. 7.
Series, finer composition: I, § 4, no. 7.
Series, formal power: III, § 2, no. 11.
Series, Jordan-Hölder: I, § 4, no. 7.
Series, lower central: I, § 6, no. 3.
Series, normal: I, § 4, Exercise 17.

Series, principal: I, § 4, Exercise 17.
G-set, homogeneous (G a group of operators): I, § 5, no. 5.
G-set, homogeneous principal, homogeneous principal set under G: I, § 5, no. 6.
Set, generating, of a group: I, § 4, no. 3.
Set, generating, of a magma: I, § 1, no. 4.
M-set (M a monoid of operators): I, § 5, no. 1.
M^0-set opposite to an M-set: I, § 5, no. 1.
Set of degrees of a graded group: II, § 11, no. 1.
Set of subgroups satisfying the maximal condition, the minimal condition: I, § 4, Exercise 15.
Sets, orthogonal: II, § 2, no. 4.
G-sets, weakly equivalent: I, § 5, Exercise 26.
Shift, shifting: II, § 11, no. 2.
Signature of a permutation: I, § 5, no. 7.
Sign of a rational number: I, § 9, no. 4.
Similar endomorphisms: III, § 8, Exercise 26.
Similar matrices: II, § 10, no. 9.
Similar ordered sequences: I, § 1, no. 2.
Simple group: I, § 4, no. 4.
Simply transitive operation: I, § 5, no. 6.
Skew field: I, § 9, no. 1.
Skew graded bigebra: III, § 11, no. 4.
Skew-symmetric tensor: III, § 7, no. 4.
Skew-symmetrized tensor: III, § 7, no. 4.
Skew tensor product of graded algebras: III, § 4, nos. 7 and 8.
Solution of a linear equation, of a linear system: II, § 2, no. 8.
Solution, trivial, zero solution of a homogeneous linear equation: II, § 2, no. 8.
Solvable group, solvable group of class n: I, § 6, no. 4.
Space, affine, attached to a vector space: II, § 9, no. 1.
Space, canonical projective, associated with a vector space: II, § 9, no. 8.
Space, projective: II, § 9, nos. 5 and 11.
Space, projective, derived from a vector space: II, § 9, no. 5.
Space, quotient vector, quotient space: II, § 1, no. 3.
Space, right, left, vector, over a field: II, § 1, no. 1.
Space, vector, associated with a module over an integral domain: II, § 7, no. 10.
Space, vector, obtained by taking an origin in an affine space: II, § 9, no. 1.
Space, vector, of translations of an affine space: II, § 9, no. 1.
Split exact sequence: II, § 1, no. 10.
Stabilizing (operator, set of operators) a subset: I, § 5, no. 2.
Stabilizing, strictly (operator, set of operators), a subset: I, § 5, no. 2.
Stable subgroup of a group with operators: I, § 4, no. 3.

Stable subset: I, § 1, no. 4.
Strictly negative, strictly positive, rational integer: I, § 2, no. 5.
Strictly negative, strictly positive, rational number: I, § 9, no. 4.
Strict stabilizer: I, § 5, no. 2.
Strictly stabilizing a subset: I, § 5, no. 2.
Strict transporter: I, § 5, no. 2.
Strongly associative subset: III, Appendix, no. 1.
Structures, module (multimodule), compatible: II, § 1, no. 14.
Structure, projective space: II, § 9, no. 11.
K'-structure, induced: II, § 8, no. 2.
K'-structure on a vector K-space: II, § 8, no. 1.
K'-structure, product: II, § 8, no. 3.
Subalgebra: III, § 1, no. 2.
Subalgebra generated by a subset: III, § 1, no. 2.
Subalgebra, graded: III, § 3, no. 2.
Subfield: I, § 9, no. 1.
Subfield generated by a subset: I, § 9, no. 1.
Subgroup, characteristic: I, § 5, no. 3.
Subgroup, invariant stable, invariant subgroup: I, § 4, no. 4.
Subgroup, normal stable, normal subgroup: I, § 4, no. 4.
Subgroup, stable, generated by a subset: I, § 4, no. 3.
Subgroup, stable subgroup: I, § 4, no. 3.
Subgroup, Sylow, Sylow $p$-subgroup: I, § 6, no. 6.
Submagma: I, § 1, no. 4.
Submagna generated by a subset: I, § 1, no. 4.
Submagma, unital: I, § 2, no. 1.
Submagma, unital, generated by a subset: I, § 2, no. 1.
Submatrix: II, § 10, no. 1.
Submodule: II, § 1, no. 3.
Submodule, component, of a direct sum of modules: II, § 1, no. 6.
Submodule generated by a family: II, § 1, no. 7.
Submodule, graded: II, § 11, no. 3.
Submodule, irreducible: II, § 2, Exercise 16.
Submodule, orthogonal (or totally orthogonal) to a subset of E (resp. E*) II, § 2, no. 4.
Submodule, torsion, of a module over an integral domain: II, § 7, no. 10.
Submodule, zero: II, § 1, no. 3.
Submodules, supplementary: II, § 1, no. 9.
Submultimodule: II, § 1, nos. 14.
Subring: I, § 8, no. 5.
Subring generated by a subset: I, § 8, no. 5.
Subring, graded: II, § 11, no. 3.
Subset, affine: II, § 9, no. 3.

Subset centralizing a subset: I, § 5, no. 3.
Subset, free, related subset: II, § 1, no. 11.
Subset, homogeneous, of degree $p$ with respect to certain indeterminates in a formal power series: III, § 2, no. 11.
Subset normalizing a subset: I, § 5, no. 3.
Subset, stable: I, § 1, no. 4 and § 3, no. 2.
Subset, stable, generated by a subset: I, § 1, no. 4 and § 3, no. 2.
Subset, strongly associative: III, Appendix, no. 1.
Subset, symmetric: I, § 4, no. 1.
Subsets, conjugate: I, § 5, no. 4.
Subspaces associated with a homogeneous element of the exterior algebra: III, § 7, no. 2.
Subspace associated with a homogeneous element of the symmetric algebra: III, § 6, no. 2.
Subspace associated with a homogeneous element of the tensor algebra: III, § 5, no. 2.
Subspaces associated with an element of a tensor product of vector spaces: II, § 7, no. 8.
Subspace rational over a subfield: II, § 8, no. 2.
Subspace, vector, subspace: II, § 1, no. 3.
Sum, amalgamated, of modules: II, § 1, Exercise 5.
Sum, amalgamated, of monoids: II, § 7, no. 3.
Sum, direct: I, § 4, no. 9.
Sum, direct, of a family of submodules: II, § 1, no. 8.
Sum, external direct, of a family of submodules: II, § 1, no. 6.
Sum, internal restricted, of subgroups: I, § 4, no. 9.
Sum, monoidal: I, § 7, no. 3.
Sum of a family of elements of finite support: I, § 2, no. 1.
Sum of a family of left ideals, of right ideals: I, § 8, no. 6.
Sum of a family of submodules: II, § 1, no. 7.
Sum of an ordered sequence: I, § 1, no. 2.
Sum of two elements: I, § 1, no. 1.
Sum of two matrices: II, § 10, no. 2.
Sum, restricted, of groups with respect to subgroups, restricted sum of groups: I, § 4, no. 9.
Supersolvable group: I, § 6, Exercise 26.
Supplementary submodules: II, § 1, no. 9.
Support of a cycle: I, § 5, no. 7.
Support of a family: I, § 2, no. 1.
Suppress columns, rows, in a matrix: II, § 10, no. 1.
Sylow subgroup: I, § 6, no. 6.
Symbol, Kronecker: II, § 1, no. 11.
Symmetric algebra of a module: III, § 6, no. 1.

Symmetric group: I, § 4, no. 1.
Symmetric multilinear mapping: III, § 6, no. 3.
Symmetric power of a linear mapping: III, § 6, no. 3.
Symmetric power of a module: III, § 6, no. 3.
Symmetric product of two multilinear mapping: III, § 11, no. 2.
Symmetric subset in a group: I, § 4, no. 1.
Symmetric tensor: III, § 6, no. 3.
Symmetrization of a tensor: III, § 6, no. 3.
System, direct, of graded algebras: III, § 3, no. 3.
System, direct, of magmas: I, § 10, no. 3.
System, direct, of modules: II, § 6, no. 2.
System, direct, of rings (groups, fields): I, § 10, no. 3.
System, free, related system: II, § 1, no. 11.
System, generating, of a group: I, § 4, no. 3.
System, generating, of a magma: I, § 1, no. 4.
System, generating, of a module: II, § 1, no. 7.
System, generating, of a projective space: II, § 9, no. 8.
System, generating, of a unital magma: I, § 2, no. 1.
System, generating, of an algebra: III, § 1, no. 2.
System, inverse, of algebras: III, § 1, no. 6.
System, inverse, of magmas: II, § 10, no. 1.
System, inverse, of modules: II, § 6, no. 1.
System, inverse, of rings (groups, fields): I, § 10, no. 1.
System of equations of a vector subspace: II, § 7, no. 5.
System of factors: III, § 2, Exercise 11.
System of homogeneous coordinates of a point: II, § 9, no. 6.
System of linear equations, linear system, homogeneous linear system: II, § 2, no. 8.
System, trivial, of commutation factors: III, § 4, no. 7.

Table, diagonal, lower triangle, upper triangular, of matrices: II, § 10, no. 7.
Table, multiplication, of an algebra: III, § 1, no. 7.
Table, square, of matrices: II, § 10, no. 5.
Tensor algebra of a module: III, § 5, no. 1.
Tensor, contravariant, covariant tensor, mixed tensor: III, § 5, no. 6.
Tensor of type (I, J): III, § 5, no. 6.
Tensor, skew-symmetric: III, § 7, no. 4.
Tensor, symmetric: III, § 6, no. 3.
Tensorial power of a linear mapping: III, § 5, no. 2.
Tensorial power of a module: III, § 5, no. 1.
Term, constant, of a formal power series: III, § 2, no. 11.
Term, constant, of a polynomial: III, § 2, no. 9.
Term in X^α in a polynomial: III, § 2, no. 9.

Term of a formal power series: III, § 2, no. 11.
Term of a polynomial: III, § 2, no. 9.
Term of a sum: I, § 1, no. 2.
Term of degree $p$ with respect to certain indeterminates in a formal power series: III, § 2, no. 11.
Term of total degree $p$ in a formal power series: III, § 2, no. 11.
Theorem, associativity: I, § 1, no. 3.
Theorem, Cayley-Hamilton: III, § 8, no. 11.
Theorem, commutativity: I, § 1, no. 5.
Theorem, Desargues’s: II, § 9, Exercise 15.
Theorem, Erdős-Kaplansky: II, § 7, Exercise 3.
Theorem, fundamental, of projective geometry: II, § 9, Exercise 16.
Theorem, Hall’s: I, § 6, Exercise 7.
Theorem, Jordan-Hölder: I, § 4, no. 7.
Theorem, Kaplansky’s: II, § 2, Exercise 2.
Theorem, Krull’s: I, § 8, no. 6.
Theorem, Nielsen-Schreier: I, § 7, Exercise 20.
Theorem of the complete quadrilateral: II, § 9, Exercise 13.
Theorem, Pappus’s: II, § 9, Exercise 14.
Theorem, Schreier’s: I, § 4, no. 7.
Torsion element, module, submodule: II, § 7, no. 10.
Torsion-free module: II, § 7, no. 10.
Total algebra of a monoid: III, § 2, no. 10.
Total graduation: II, § 11, no. 1.
Totally orthogonal (submodule) to a subset: II, § 2, no. 4.
Trace, Cayley: III, § 2, no. 4.
Trace in a quadratic algebra: III, § 2, no. 3.
Trace of a matrix: II, § 10, no. 11.
Trace of an element in a K-algebra: III, § 9, no. 3.
Trace of an endomorphism: II, § 4, no. 3.
Trace of a scalar with respect to a module: III, § 9, no. 1.
Transitive operation: I, § 5, no. 5.
Transitivity formulae: III, § 9, no. 4.
Translation in an affine space, space of translations: II, § 9, no. 1.
Translation, left, right: I, § 2, no. 2.
Translation, left, right (monoid operating on itself by): I, § 5, no. 1.
Transporter, strict transporter: I, § 5, no. 2.
Transpose of a linear mapping, of a semi-linear mapping: II, § 2, no. 5.
Transpose of a matrix: II, § 10, no. 1.
Transposition: I, § 5, no. 7.
Transvection: II, § 10, Exercise 11.
Triangular, lower, upper triangular, matrix: II, § 10, no. 7.
Trivial extension: I, § 6, no. 1.

Trivial graduation: II, § 11, no. 1.
Trivial homomorphism: I, § 2, no. 1.
Trivial operation: I, § 5, no. 2.
Trivial solution of a homogeneous linear equation: II, § 2, no. 8.
Trivial system of commutation factors: III, § 4, no. 7.
Two-sided ideal: I, § 8, no. 6 and III, § 1, no. 2.
Type, exponential, group of: I, § 7, Exercise 39.
Type Δ, graduation of: II, § 11, no. 1.

Unimodular endomorphism: III, § 8, no. 1.
Unimodular group: III, § 8, no. 9.
Unimodular matrix: III, § 8, no. 3.
p-unipotent element: I, § 6, Exercise 28.
Unit element of an algebra: III, § 1, no. 1.
Unit, left, right, in a groupoid: I, § 4, Exercise 23.
Unit, unit element of a magma: I, § 2, no. 1.
Unital algebra: III, § 1, no. 1.
Unital algebra homomorphism, morphism: III, § 1, no. 1.
Unital homomorphism: I, § 2, no. 1.
Unital magma: I, § 2, no. 1.
Units, matrix: II, § 10, no. 3.
Universal algebra defined by a generating system related by a family of relators: III, § 2, no. 8.
Universal algebra subjected to identities: III, § 2, no. 8.
Universal relator: III, § 2, no. 8.
Unknowns of a linear system: II, § 2, no. 8.

Value, absolute, of a rational number: I, § 9, no. 4.
Value of an element of a free algebra: III, § 2, no. 8.
Vandermonde determinant: III, § 8, no. 6.
Variety, affine linear, affine linear variety generated by a family: II, § 9, no. 3.
Variety, linear: II, § 9, nos. 3, 7 and 11.
Variety, projective linear, projective linear variety generated by a family: II, § 9, nos. 7 and 11.
Varieties, parallel linear: II, § 9, no. 3.
Vector: II, § 1, no. 1.
Vector, direction, of an affine line: II, § 9, no. 3.
Vector, free, of an affine space: II, § 9, no. 1.
p-vector: III, § 7, no. 1.
p-vector, pure: III, § 11, no. 13.
Vector rational over a subfield: II, § 8, no. 2.
Vector space: II, § 1, no. 1.

Word: I, § 7, no. 2.

Weight of a homogeneous element: II, § 11, no. 1.
With no fixed point (automorphism): I, § 6, Exercise 23.

Zassenhaus’s Lemma: I, § 4, no. 7.
Zero: I, § 2, no. 1.
Zero matrix: II, § 10, no. 22.
Zero ring: I, § 8, no. 3.
Zero solution of a linear equation: II, § 2, no. 8.
Zero submodule: II, § 1, no. 3.

N. Bourbaki, Elements of Mathematics, Algebra, Chapters 1-3

This is the soft-cover reprint of the English translation of 1974 (available from Springer since 1989) of the first 3 chapters of Bourbaki's "Algebrec". It gives a thorough exposition of the fundamentals of general, linear and multilinear algebra. The first chapter introduces the basic objects: groups, actions, rings, fields. The second chapter studies the properties of modules and linear maps, especially with respect to the tensor product and duality constructions. The third chapter investigates algebras, in particular tensor algebras. Determinants, norms, traces and derivations are also studied.
