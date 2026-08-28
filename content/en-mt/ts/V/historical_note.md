---
book: ts
book_title: Théories spectrales
chapter: V
chapter_title: REPRÉSENTATIONS UNITAIRES
section: 0
section_title: Historical Note
kind: historical
lang: en
source: ts-iii-v-fr
book_pages: TS V.517-TS V.540
pdf_pages: 0530-0553
extraction: native
subsections:
    - "no": 1
      title: Découverte du spectre continu
      page: 517
      pdf_page: 530
    - "no": 2
      title: Opérateurs compacts
      page: 521
      pdf_page: 534
    - "no": 3
      title: Indice de Fredholm et perturbations
      page: 523
      pdf_page: 536
    - "no": 4
      title: Opérateurs partiels et théorème spectral
      page: 526
      pdf_page: 539
    - "no": 5
      title: Jonction entre analyse harmonique et théorie des groupes
      page: 528
      pdf_page: 541
    - "no": 6
      title: Groupes localement compacts commutatifs
      page: 533
      pdf_page: 546
    - "no": 7
      title: Algèbres d’opérateurs
      page: 536
      pdf_page: 549
    - "no": 8
      title: Représentations des groupes localement compacts
      page: 539
      pdf_page: 552
statements: 0
exercises: 0
content_sha256: 1f42e006f997885593b0e632f8b3c56f3053ebc4b3a331465f61e84ffcb3c41b
translated_from: content/fr/ts/V/historical_note.md
source_lang: fr
translation_method: machine
source_content_sha256: e7e785486ed1d63a42ea81c99924dbe4ab6c8b535bbf7ffbba15087c80657189
translation_model: gpt-5-mini, gpt-5.4
translation_run: translate-en-mt-fd4d27cb
glossary_version: 34
glossary_terms_sha256: ee8d75711b6fb565266b57bf0ce76f9c0e67261163d4db8d6705a935c9b1cd01
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

# HISTORICAL NOTE

(Chapters I to V)

The notions of eigenvalue and Fourier series were already well known in 1830, permeating many fields of Analysis throughout the xix$^e$ century (cf. ÉHM, p. 114, 260, 275). But spectral theory and harmonic analysis, in the sense in which we understand them in this book, only began to take their present form about a century later — at the same time as their junction with the study of group representations around 1930, and then with that of normed algebras around 1940.

We shall confine ourselves here to tracing the main lines of their development in the period extending from 1906 — the date at which Hilbert introduced the notion of “continuous spectrum” in his work on integral equations — to the years 1945–1950, when the theories presented here acquired essentially the form that they have retained up to the present day.

### 1. Discovery of the continuous spectrum

In the Note on Topological Vector Spaces (cf. ÉHM, p. 262–263), we have described how I. Fredholm came, around 1900 — pursuing work of C. Neumann, V. Volterra and H. Poincaré — to consider the equation

$$
u(x)-\lambda \int_IK(x, y)u(y)dy=f(x) \tag{1}
$$

with unknown function $u: I\rightarrow \mathbf{C}$, in the case where the interval $I\subset \mathbf{R}$ is compact and where the kernel K is continuous on $I\times I$. A skilful use of “infinite determinants”, based on ideas of Poincaré and H. von Koch, enabled him to obtain families of solutions whose dependence on the complex variable $\lambda$ is meromorphic, and then to prove the celebrated “alternative” concerning the existence of solutions (cf. III, p. 81, th. 5). But Fredholm immediately specialized his results to the case $\lambda =-1$, without exploiting the fact that equation (1) is an eigenvalue problem[^1].

When the kernel K is symmetric, we have also seen how Hilbert, in his first memoir on integral equations [**31**], recognized the relationship between Fredholm’s problem and the research of the “principal axes” of a quadratic form. Starting from this reduction for finite “sections” (discretizations) of the kernel K, he obtained by passing to the limit the formula

$$
\int_IK(s, t)x(s)x(t)dt=\sum_{n=1}^{\infty}\frac{1}{\lambda_n}\int_I\varphi_n(s)x(s)ds \tag{2}
$$

where the $\lambda_n$ are the eigenvalues of the kernel K, the $\varphi_n$ form an orthonormal system of associated eigenvectors[^2], and where the equality is valid as soon as $x$ is square integrable on I (cf. ÉHM, p. 264).

The principal obstacles that presented themselves to Hilbert concerned the passage from finite sums to the integrals in formula (2). He deduced from this formula the existence of the eigenvalues — however, he gave for the latter a variational characterization independent of the passage to the limit, inspired by the classical method for determining eigenvalues in finite dimension (cf. n$^o4$ of IV, p. 153). E. Schmidt would show in 1905, drawing inspiration from the work of H. Schwarz, how to obtain (2) without passing through the “infinite determinants” on which the methods of Fredholm and Hilbert depended (cf. ÉHM, p. 265).

But as early as 1906, Hilbert [**32**] turned to the more general problem of the reduction of a quadratic form

$$
B(x, x) =\sum_{p,q=0}^{\infty}b_{pq}x_px_q,x= (x_p)_{p\in\mathbf{N}}
$$

on $E =\ell^2_{\mathbf{C}}(\mathbf{N})$. He was of course keeping in mind that by passing to the coefficients in an orthonormal basis of E, problem (1) reduces to the search for solutions of the “infinite linear system”

$$
x_p+\sum_{q=0}^{\infty}b_{pq}x_q=f_p(p\in \mathbf{N})
$$

He nevertheless points out that for Fredholm’s problem, the quadratic forms involved are very particular ones, for which $B(x_n, x_n)$ tends to $B(x, x)$ as soon as $x_n$ converges weakly to $x$; he calls them “completely continuous” (vollstetig).

Hilbert insists on the essential difference that distinguishes them from the quadratic forms bounded on E, and decides to undertake the more general reduction of the latter. Once again, his method is to start from the reduction of the “finite sections”

$$
(x_0, . . . , x_n)\mapsto \sum_{p,q=0}^nb_{pq}x_px_q
$$

of the form B, and then to let $n$ tend to infinity. For this passage to the limit, he takes advantage of the ideas on integration introduced by T. Stieltjes in his work on continued fractions [**71**]. He shows that every bounded quadratic form can, after an orthogonal transformation of the variables, be put in the form

$$
\sum_{p\in\mathbf{N}}\frac{1}{\lambda_p}x^2_p+\int_{s\in\mathbf{R}}\frac{1}{s}d\sigma (s, x) \tag{3}
$$

In this formula, the $\lambda_p$ are the eigenvalues of B and $x\mapsto \sigma (s, x)$ is (for fixed $s\in \mathbf{R}$) a positive separating quadratic form on E, whereas $s\mapsto \sigma (s, x)$ is[^3] (for fixed $x\in E$) a continuous increasing function which tends to 0 at $-\infty$ and to $\|x\|^2$ at $+\infty ($cf. ÉHM, p. 284, for Stieltjes’ notation).

Let S denote the set of points of $\overline{\mathbf{R}}$ admitting no neighbourhood in which $s\mapsto \sigma (s, x)$ remains constant for every $x$; then the integral in (3) can naturally be taken over S. Hilbert names the set S “continuous spectrum” (Streckenspektrum), the set of eigenvalues of B “point spectrum” (Punktspektrum), and their union “spectrum” (Spektrum). This term, coming from optics, had been used in 1897 by W. Wirtinger [**91**] in the study of differential equations with periodic coefficients.

Hilbert would quickly derive from his “spectral” methods a profound renewal of several problems of classical Analysis, concerning the study of ordinary differential equations (in particular of Sturm–Liouville type), partial differential equations or functions of a complex variable. We shall not give an account here of the abundance of results that followed in the first quarter of the xx$^e$ century and refer to the synthesis of E. Hellinger and O. Toeplitz [**29**]. We shall nevertheless mention some of these works on integral equations, where the seeds of later developments of the abstract theory will be found.

For Hilbert and his pupils, faithful to a German tradition in linear Algebra, the model remains the theorem of principal axes; hence it is still a matter of studying the spectra of bilinear or quadratic forms, in particular on the “Hilbert” space $E =\ell^2_{\mathbf{C}}(\mathbf{N})$. The fact that every continuous bilinear form B on E could be related to the continuous endomorphism A of E characterised by $\langle Ax, y\rangle = B(x, y)$ was known to Hilbert’s school, in particular after the work of E. Schmidt, M. Fréchet and F. Riesz in 1907–1908. But it was F. Riesz who showed, in an admirable book [**59**] of 1913, the interest of putting endomorphisms in the foreground in this context.

Riesz gives the modern definition of the spectrum of an element A of $\mathscr{L}(E)$[**59**, p. 139], remarks that it is a closed, bounded set, and shows that the resolvent $\lambda \mapsto (\lambda 1_E-A)^{-1}$ is holomorphic on the complement of the spectrum of A. Above all, he gives a central role to the algebra structure of $\mathscr{L}(E) :$ inspired by work of Volterra, he develops a first version of the functional calculus for symmetric endomorphisms, which enables him to recover simply the reduction results of Hilbert and Schmidt. If A is a symmetric element of $\mathscr{L}$ (E), Riesz shows how to define $f(A)$ for every function $f$ semi-continuous (lower or upper) from $\mathbf{R}$ to $\mathbf{R}$, and notes that $f\mapsto f(A)$ is what we call today an algebra morphism [**59**, p. 129–130]. Applying this idea to the characteristic function of an interval $[\xi ,+\infty [$, one obtains for every $\xi$ a symmetric endomorphism $A_{\xi}$ of E; using the Stieltjes integral, Riesz then shows a version of Hilbert’s relation (3):

$$
\langle Ax, y\rangle =\int_{\mathbf{R}}\xi  d\langle A_{\xi}x, y\rangle
$$

for $x, y\in E$, an equality which he even writes

$$
A =\int_{\mathbf{R}}\xi  dA_{\xi}
$$

The spectrum of A is then the set of values $\xi_0$ such that $A_{\xi}$ does not remain constant in any neighbourhood of $\xi_0$, and the point spectrum that of the points of discontinuity of $\xi \mapsto A_{\xi}$.

Shortly before concluding with the applications of the theory, Riesz notes [**59**, p. 146] that his results take a particularly simple form when the endomorphism A comes from one of Hilbert’s “completely continuous” bilinear forms: the spectrum reduces to the set of eigenvalues (to which 0 may possibly have to be added), the eigenvalues are organised in a sequence tending to 0, and each non-zero eigenvalue is of finite multiplicity (III, p. 90, prop. 5).

### 2. Compact operators

Riesz considerably amplifies these remarks less than three years later, in his memoir on functional equations [**60**] which develops, with a clarity intact after more than a century, the essential part of the spectral theory of compact operators on Banach spaces. The stated aim of this text is to reformulate Fredholm’s theory for equation (1) on a compact interval I, by considering the space $E =\mathscr{C}(I)$ endowed with the topology of uniform convergence. But as we have already indicated in an earlier note (ÉHM, p. 268), Riesz is clearly aware that his results apply to every Banach space — notion which would only be introduced in the following decade.

Inspired by Fréchet’s ideas on general topology, Riesz now considers the endomorphisms of E which send every bounded sequence to a relatively compact sequence. Like Hilbert, he still calls them “completely continuous” and notes that this new notion is equivalent, in the case of E = $\ell^2_{\mathbf{C}}(\mathbf{N})$, to the notion of complete continuity that he had used in his book of 1913[^4].

Riesz studies the endomorphisms of the form $B = 1_E-A$ where A is a completely continuous endomorphism of E, and deduces all their spectral properties from the fact that a locally compact normed vector space must be of finite dimension — a fact discovered, it seems, on the occasion. He easily proves that the kernel of B is of finite dimension and that its image is closed and of finite codimension. As E. Weyr [**87**] had done in finite dimension, he then considers the iterates $B^k$. He shows that the sequence of their kernels and that of their images are stationary, then introduces what we call today nilespace and conilespace of B, showing effectively that E is their topological direct sum. Applying this observation to the endomorphisms $B_{\lambda}= 1_E-\lambda A$ for $\lambda \in \mathbf{C}$, he deduces without difficulty the spectral properties of completely continuous endomorphisms of a Banach space, and this in an almost definitive form.

Among the principal results on the spectrum of these operators, only those that will require a more mature view of the notion of functional space, in particular of duality, seem to escape Riesz. For example, at the end of the 1920s, T. Hildebrandt [**33**] and J. Schauder [**63**] will show (in the now well-established setting of Banach spaces) that the adjoint of a completely continuous endomorphism is completely continuous.

Moreover, the notion of complete continuity of Riesz still depends on the use of sequences; Banach [**4**] freed himself from this in his 1932 book in order to consider mappings that transform every bounded subset into a relatively compact subset. The term « compact » linear mapping would only become established progressively in the second half of the xx$^e$ century, probably following E. Hille’s [**34**] book on operator semigroups.

Several questions posed in the 1930s would remain open for a long time. In this direction, let us mention the resolution [**18**] in 1973 of the « approximation problem » made famous by Banach and S. Mazur in 1932 and 1938 (see Remark 6 of III, p. 16 and Exercise 25 of III, p. 112).

At the same time, Lomonosov [**40**] proved the existence of nontrivial closed subspaces invariant under an endomorphism commuting with a nonzero compact endomorphism in a locally convex space (cor. 2 of III, p. 13). This result was one of the most significant advances on the problem of the existence of such a subspace for an arbitrary continuous endomorphism (« invariant subspace problem »). This problem is still open, at the present time, in the case of continuous endomorphisms of Hilbert spaces of countable type; P. Enflo [**19**] constructed in 1987 the first example of an endomorphism of a Banach space admitting no nontrivial closed invariant subspace.

### 3. Fredholm index and perturbations

The notion of index appeared in 1920 in a work of Fritz Noether on integral equations. In his address at the International Congress of 1904, Hilbert considered a problem posed by Riemann in potential theory: if one is given a bounded open domain Ω of the plane whose boundary is a simple smooth closed curve Γ, as well as three functions $a,b,f$ on Γ, the problem is to find a function $z: \Omega \rightarrow \mathbf{C}$, holomorphic on Ω and continuous on Ω, satisfying

$a\mathscr{R}(z) +b\mathscr{I}(z) =f$ sur $\Gamma$.

Parametrizing Γ by a real $s\in [0,2\pi ]$, Hilbert showed that the problem amounts to solving a « singular kernel » integral equation for $\varphi =\mathscr{R}(z)$, namely

$$
a(s)\varphi (s) +\int_0^{2\pi}K(s, t)\varphi (t)dt=f(s) \tag{4}
$$

Here the kernel $K(s, t)$ takes the form $b(s)$ cot($\frac{t-s}{2}$) $+ A(s, t)$ for a continuous function A. It is therefore singular along the diagonal, and the integral above is to be taken in the sense of the Cauchy principal value.

Noether [**53**] observes that contrary to integral equations satisfying the Fredholm alternative, in the case of a kernel K as above and of a nonzero second member $f$, it is possible that (4) admits families of nontrivial solutions. He shows that the space of solutions is governed by the integer

(5) $n=\frac{1}{2\pi}\int_{\Gamma}d$ (log($a-ib$)).

If $n <0$, there is no nontrivial solution, and if $n\geqslant 0$, equation (4) admits a family with $2n$ parameters of solutions. Noether uses the term « index » (Index) for the integer $n$ and recognizes in it a number of turns, a classical notion since the end of the xix$^e$ century in the study of functions of one complex variable.

Other works would subsequently study examples of equations requiring an extension of Fredholm theory. But it would be necessary to wait more than twenty years before the notion of Fredholm mapping was systematically developed, at the same time as the study of perturbations by compact operators matured.

In 1909, H. Weyl [**81**] had shown that if two bounded quadratic forms on $\ell^2_{\mathbf{C}}(\mathbf{N})$ have a completely continuous difference, then their essential spectra coincide (cf. III, p. 89, th. 2). Moreover, Riesz had remarked in his 1916 memoir, naturally without the modern language, that compact operators on a Banach space E form a two-sided ideal of $\mathscr{L}(E)$. It seems however that the path indicated by these two remarks was only explored from the 1940s onwards. In 1941, J. Calkin, motivated by the works of J. von Neumann on operator algebras (which we shall have to discuss shortly, see p. 537), points out the interest of studying congruences modulo this ideal in the setting of Hilbert spaces [**10**]. He shows how the structure of the algebra which now bears his name (cf. III, p. 75) makes it possible to recover Weyl’s result simply.

At the same time, around 1942, J. Dieudonné [**15**] had the idea of studying the perturbations of a continuous linear mapping $u$ between normed spaces, in the case where the perturbation is « small » in the sense of the operator norm. He restricts himself to the case where $u$ is a strict morphism whose kernel is of finite dimension or finite codimension, proves that the same is then true of every « small perturbation » of $u$, and shows that in the case of Fredholm mappings (cf. n$^o2$ of III, p. 40), the index is locally constant (th. 1 of III, p. 58), as well as several of the results presented in § 4 of III, p. 55.

These two ideas converge around 1950, when F. Atkinson [**3**], I. Gohberg [**26**], S. Mikhlin [**46**] and B. Yood [**93**] study perturbations by compact operators. They explicitly make the connection with the Noether index and bring out the notions of Fredholm mapping [**3**, p. 8] and Riesz mapping [**93**, §5]. The latter are the subject of systematic research in the following decade, in which the results presented in Chapter III take approximately their present form.

The usual setting of these theories is that of Banach spaces; however, various applications motivate their generalization to broader classes of topological vector spaces. Thus, the case of Fréchet spaces appears naturally in 1954 in work of H. Cartan and J-P. Serre [**13**] who prove the finiteness of the cohomology of a compact complex analytic manifold with coefficients in a coherent sheaf, the proof making use of deformation results proved by L. Schwartz [**66**] (cf. th. 2 of III, p. 73).

The invariance of the index under deformation is perfectly clear, in the case of formula (5), if one observes that the right-hand member (number of turns) is invariant under homotopy. Such topological expressions for the index will soon become famous for Fredholm mappings arising from differential geometry. If D is a differential operator on a compact variety X of class $C^{\infty}($cf. VAR, §14), and if D is “elliptic” (cf. [**2**, §1]), then an extension of D to suitable Sobolev spaces defines a Fredholm mapping. The search for a formula giving a topological expression for its index by means of the “characteristic classes” of X, suggested among others by work of I. Gelfand around 1960 [**23**, vol. I, p. 65], led in 1963 to the “index theorem” of M. Atiyah and I. Singer [**2**]. The latter gave rise to extraordinary developments at the confluence of analysis, topology and differential geometry. We cannot describe here the vast fields which they opened and which, still today very fertile, have not ceased to draw nourishment from Fredholm theory.

### 4. Partial operators and spectral theorem

The general Hilbert spectral theory was created largely in order to answer the problem of the mathematical foundations of Quantum Mechanics, notably under the impetus of von Neumann.

We refer to the work of M. Jammer [**35**] for a detailed description of the development of Quantum theory up to the fundamental article of W. Heisenberg which introduced Quantum Mechanics [**28**]. Less than five years were needed between its publication in the summer of 1924 and that of the article [**50**], in 1929, in which von Neumann presents, in a perfectly lucid and rigorous manner, all the fundamental results of the theory of Hermitian partial (often called “unbounded”) operators on Hilbert spaces.

By giving the first axiomatic presentation of Hilbert spaces [**49**], von Neumann crowns an idea long in gestation (cf. ÉHM, p. 267), and illuminates various isomorphisms between spaces of sequences or functions well known to Schmidt, Fréchet, Fischer and Riesz before 1910. This rise in abstraction enables von Neumann to make considerable conceptual advances.

Such is the idea of a partial operator, which seems to hover, still formless, over several of the works which take up again, after Hilbert, the Fredholm equations (see above, n$^o1$). Hilbert had noticed that many differential equations of Sturm–Liouville type, in particular in the case of an unbounded interval, could be reduced to Fredholm equations; but in order to apply integral methods, it was necessary to weaken the conditions imposed on the kernel and to leave the setting where the results of Fredholm, Hilbert and Schmidt could be applied. Over the years increasingly singular kernels are studied, until equations are considered for which the left-hand member has a meaning only if the unknown belongs to a subspace of $L^2(I)$. In this direction, mention must be made of work of E. Hilb [**30**] in 1908, of H. Weyl on Sturm–Liouville theory [**82**] in 1910, and above all of T. Carleman [**11**] in 1923, in a very general setting.

By unifying these problems, von Neumann casts an entirely new light on these classical works. He emphasizes in particular the fundamental distinction between symmetric operator and self-adjoint operator, and interprets the self-adjoint extensions of a symmetric operator in terms of abstract “boundary conditions”, generalizing the well-known boundary conditions which appeared, for example, in the Dirichlet and Neumann problems for the Laplace operator on a bounded open subset of $\mathbf{R}^n$.

At the same time, von Neumann [**51**] brings out the notion of normal operator[^5] as a natural setting for spectral theory, insisting on the role of the commutative algebra generated by the operator and its adjoint.

Relying on this precise mathematical formalism, which also revealed the equivalence between the viewpoints of Heisenberg and Schrödinger, and on the Copenhagen interpretation of experimental procedures and results, non-relativistic Quantum Mechanics thereby reached a state of perfection which has scarcely changed since then; the validity of this physical theory, despite its surprising consequences, even paradoxical in appearance, has since been constantly confirmed by experiment, and this with remarkable precision.

From a formal point of view, the foundations of spectral theory were established by von Neumann. At the same time, after the presentation of the first ideas of the latter, M. Stone had pursued similar researches between 1928 and 1930 and obtained related results. The clear and complete presentation of the known results which Stone published in 1932 [**72**] had an important influence on the diffusion of Hilbertian spectral theory.

Nevertheless, other improvements in the presentation were important for the diffusion of these results. Indeed, the spectral theorem (cf. Theorem 1 of IV, p. 266), as presented by von Neumann, was for a long time considered very difficult, largely because it was stated in the setting of vector-valued measures.

Later, P. Halmos [**27**], by emphasizing the interpretation of the spectral theorem by means of multiplication operators on the spaces $L^2$, revealed its essentially elementary aspect in the case of bounded operators. Quite recently, S. Woronowicz (in the somewhat different setting of regular operators of Hilbert modules over stellar algebras [**92**]) introduced a simplification by introducing the “bornification” (cf. No.$^o2$ of IV, p. 265), which makes it possible to treat normal partial operators as simply as self-adjoint operators.

Moreover, if D is a formally symmetric scalar differential operator on an open set U of $\mathbf{R}^n$, the study of the self-adjoint extensions of D to $L^2(U)$ is naturally linked with the study of distributions on U (in the case of the Laplacian, cf. No.$^o6$ of IV, p. 242). We refer to the work of J. Dieudonné [**16**, ch. vii] for the history of the latter — a winding history which is untangled shortly after the period just mentioned, with decisive contributions by S. Sobolev [**69**] in 1936, and by L. Schwartz [**65**] ten years later.

From a purely mathematical point of view, spectral theory interacts in a particularly fruitful manner with Riemannian Geometry. Thus, taking up a question of S. Bochner, M. Kac gives in 1966 a singularly striking presentation [**36**] of the problem of determining the geometric properties of a Riemannian manifold which can be deduced from the spectral properties of the Laplace operator. This question had been anticipated by the physicist A. Schuster [**64**] in 1882: To find out the different tunes sent out by a vibrating system is a problem which may or may not be solvable in certain special cases, but it would baffle the most skillful mathematician to solve the inverse problem and to find out the shape of a bell by means of the sounds which it is capable of giving out. (“To determine the harmonics emitted by a vibrating system is a problem which may or may not be solvable in certain particular cases, but the most skillful mathematician would be baffled if he had to solve the inverse problem and determine the shape of a bell from the sounds which it can emit”).

### 5. Junction between harmonic analysis and group theory

We have described, in the historical notes of the Book of Integration (cf. ÉHM, p. 275), how the questions connected with the heat equation led Fourier to the revolutionary conception of the representation of an arbitrary function as a sum of trigonometric functions.

We cannot retrace here the development of the theory of Fourier series and integrals throughout the xix$^e$ century, nor the profound influence which the questions raised by this theory had on the evolution of Analysis — to the point of overturning the conception of real numbers, contributing to the birth of set theory (cf. ÉHM, p. 42). But in order to understand the form of the ideas expounded in this Book, it is appropriate to describe the way in which harmonic analysis was linked after 1925 with group theory and with Hilbertian spectral theory.

The recognition of the link between Fourier’s ideas and the group structures of $\mathbf{R}/\mathbf{Z}$ and $\mathbf{R}$, as well as the generalization of these ideas to other groups, took place rather late.

One can naturally, in the beginnings of the theory of finite groups and their characters, identify results which today appear to contain the rudiments of finite Fourier analysis. For example, the dual of the group of invertible elements of $\mathbf{Z}/q\mathbf{Z}$, as well as the orthogonality relation which expresses the characteristic function of an element as a linear combination of characters, appear implicitly in 1837 in Dirichlet’s article [**17**] proving that there exist infinitely many prime numbers $p\equiv a$ mod$. q$ if $a$ is prime to $q$. It relies on ideas of Gauss, who had introduced the term “character” (character) in his study of binary quadratic forms with integer coefficients and fixed discriminant (cf. [**22**, § 230]).

But neither Gauss nor Dirichlet use the language of groups. It was Dedekind, presenting these works in 1879, who recognized their latent role and defined the notion of character for commutative groups. Dedekind’s remarks are considerably amplified by H. Weber, first in 1882 [**77**], then in 1886 [**78**, p. 112], where he introduced the dual group of a finite commutative group A and noted that it is isomorphic to A. His purpose was then to construct abelian extensions of the field $\mathbf{Q}$ with given galois group, and he did not consider the problem of harmonic analysis on such a group.

In the case of noncommutative groups, the foundations of the theory of representations of finite groups were solidly established towards the turn of the xx$^e$ century, following the work of G. Frobenius, W. Burnside and I. Schur (cf. ÉHM, p. 154). After 1905, it was clear that the orthogonality relations of characters played a crucial role in the organization of the theory. But their kinship with harmonic analysis remained hidden.

It was Hermann Weyl who joined these domains, when he conceived the idea of a general theory of representations for compact groups. In several major texts published between 1925 and 1927, he recognized the links that would unite such a theory with Fourier analysis and Hilbertian spectral theory, and he laid the foundations for many subsequent discoveries.

It was a letter from Schur that set Weyl on this path, thanks to their common interest in invariant theory. We have described, in the note on Haar measure (ÉHM, p. 289–291), how A. Hurwitz had conceived as early as 1897 the idea of using an “invariant integration” to determine the polynomials on $\mathbf{R}^n$ invariant under the orthogonal group. It seems that Schur did not know Hurwitz’s results before 1924, when he suddenly understood how invariant integration made it possible to extend to the group $\mathbf{O}(n)$ the theory of characters and the orthogonality relations that he had established for finite groups. Weyl immediately saw that Schur’s methods, joined to the work of Élie Cartan, made it possible to construct the irreducible representations of compact semisimple Lie groups. The series of three memoirs in which Weyl combined the ideas of Cartan and Schur, published in 1925 [**83**], already contained the essential part of the results of LIE, IX, §6-7; cf. ÉHM, p. 328–330.

But it was the following year, in a no less celebrated text written with his student F. Peter [**54**], that Weyl brought to light the links between the theory of representations of compact groups, Fourier analysis, and Hilbertian spectral theory. This text of fewer than twenty pages contains in germ very numerous future developments.

Peter and Weyl free themselves from every algebraic assumption on the structure of the group studied, supposing only that G is a compact topological group endowed with an invariant measure. The existence of such a measure was clear for connected Lie groups; soon A. Haar would establish it in general, partly motivated by the results presented here (cf. ÉHM, p. 291).

The starting point of their study is the orthogonality of matrix coefficients. Schur had remarked that by choosing a representative $\pi \in \widehat{G}$ for each equivalence class of irreducible representations, a G-invariant scalar product on the space E of $\pi$, and an orthonormal basis of E, one obtains a family of matrix coefficients which is orthonormal in $L^2(G)$. Peter and Weyl mean to show that such a family is total.

In the case of finite groups, the analogous result had been proved by Frobenius by studying the group algebra $\mathbf{C}[G]$. Peter and Weyl then consider the space $\mathscr{C}(G)$ of continuous functions on G and endow it with the convolution product. It seems that this is the first use of the convolution product as an abstract operation in explicit connection with the group structure (cf. ÉHM, p. 295). Peter and Weyl moreover call Gruppenzahl (“group number”) an element of the algebra $\mathscr{C}$(G), and denote by $xy$ the (convolution) product of two Gruppenzahlen. They also endow $\mathscr{C}(G)$ with the involution $f\mapsto \widetilde{f}$, where $\widetilde{f}(g) =f(g^{-1})$ for $g\in G$.

Having thus introduced the involutive algebra $\mathscr{C}$(G), the first observation made by Peter and Weyl is that every unitary representation $\pi$ of G gives rise to a representation $f\mapsto \pi (f)$ of $\mathscr{C}(G) ($cf. V, p. 400). The notion of hermitian element of $\mathscr{C}(G)$ is explicitly defined, and likewise (implicitly) that of positive element, which opens the way to the application of Hilbertian techniques.

Peter and Weyl no longer hesitate to qualify the operator $\pi (f)$ as the “Fourier coefficient” of $f$, and they pursue the parallel with Fourier theory by remarking that Schur’s orthogonality relations imply Bessel’s inequality

(6) $\sum_{\pi\in\widehat{G}}$ dim($\pi$ ) Tr($\pi (f)\pi (f)^*$)$\leqslant (f*\widetilde{f})(e) =\|f\|^2_2$.

Hilbert–Schmidt spectral theory then allows them to show that this is an equality (“Plancherel formula”). To every element $\varphi$ of $\mathscr{C}$ (G), Peter and Weyl associate the continuous kernel $K_{\varphi}: G\times G\rightarrow \mathbf{C}$ defined by $K_{\varphi}(x, y) =\varphi (xy^{-1})$. They then observe that if $\varphi$ is of the form $f*\widetilde{f}$ with $f\in \mathscr{C}(G)$,[^6] then $K_{\varphi}$ is a positive hermitian kernel in the sense of Hilbert–Schmidt theory. A variant of a Schmidt algorithm[^7] then allows them to construct an orthonormal basis of eigenfunctions of the kernel $K_{\varphi}$, and then to reduce the proof of the equality in (6) to the fact that the trace of the operator defined by $K_{\varphi}$ is equal to the sum of its eigenvalues.

Naturally, only the representations $\pi$ satisfying $\pi (f)\not = 0$ can occur in (6); the spectral theory for $K_{\varphi}$ shows the existence of such a representation if $f$ is not identically zero. Peter and Weyl deduce easily from this that the irreducible representations separate the points of G — a particular case of the Gelfand–Raikov theorem, which will be discussed later.

In the celebrated work of Frobenius, an equality analogous to (6) made it possible to prove that the regular representation of G contains all the irreducible representations. But it was a question of applying this equality by taking for $f$ the identity element of $\mathbf{C}[G]$; one then obviously had $\pi (f)\not = 0$ for every $\pi$. According to Peter and Weyl, the absence of an identity element for convolution explains many of the difficulties in their proof; they nevertheless remark, borrowing from the theory of Fourier series an idea destined to have a great future, that one can deduce the analogue of Frobenius' result by applying (6) to a sequence of functions forming an approximate unit for convolution (cf. No.$^o10$ of I, p. 120).

Analogously, starting from the equality resulting from (6), the polarized version

(7) $\sum_{\pi\in\widehat{G}}$ dim($\pi$ ) Tr($\pi (x)\pi (y)$) $= (x*y)(e)$

makes it possible to obtain, by taking for $y$ an approximate unit for convolution, a uniform approximation of every element of $\mathscr{C}(G)$ by linear combinations of matrix coefficients of irreducible representations. Methods had made it possible for Weyl to give a new proof [**84**] of the fundamental result of the theory of “almost periodic functions” of H. Bohr, to which we shall return shortly. Peter and Weyl point out that one can read there the first analytic application of the theory of representations of a non-compact group, here that of the translations of $\mathbf{R}$.

The young quantum theory very quickly provided Weyl with the opportunity to return to the representations of $\mathbf{R}$. At the end of 1927, he pointed out the interest of groups (finite or not) and representations for clarifying the foundations of this theory [**85**]. He returned to this the following year, in a celebrated book [**86**].

In his 1927 article, Weyl observes that if $u$ is a continuous self-adjoint operator on a Hilbert space, then $t\mapsto e^{itu}$ is a unitary representation of $\mathbf{R}$. But there exist unitary representations of $\mathbf{R}$ which are not of this form; taking up von Neumann’s idea on the role of partial symmetric operators in representing observable physical quantities, Weyl suggests that every unitary representation of $\mathbf{R}$ is of the form $t\mapsto e^{itu}$, where $u$ is a self-adjoint partial operator on a Hilbert space. This point of view enables him to reduce the analysis of the “canonical relations” of Heisenberg and Schrödinger, already studied in detail by von Neumann, to that of the links between two unitary representations of $\mathbf{R}$ on the same Hilbert space. Stone [**73**] shows in 1932 the result hoped for by Weyl (V, p. 428, Theorem 1), following on from his study of the spectral properties of self-adjoint operators.

### 6. Commutative locally compact groups

The interaction between harmonic analysis and group representations is therefore firmly established at the beginning of the 1930s. It is greatly strengthened in the following decade, each of the two subjects bringing about rapid progress in the other.

A very fertile field for this interaction was the study of almost periodic functions, introduced by H. Bohr in 1924 in the case of functions of a real variable [**9**]. According to one of the fundamental theorems of the latter, these are the bounded continuous functions which are uniform limits on $\mathbf{R}$ of linear combinations of functions $x\mapsto e^{i\lambda x},\lambda \in \mathbf{R}($cf. II, p. 292, exerc. 54). Bochner [**6**] had proved in 1926 that a function $f\in \mathscr{C}_b(\mathbf{R})$ is almost periodic if and only if its translates $x\mapsto f(x-a)$, for $a\in \mathbf{R}$, form a relatively compact subset of $\mathscr{C}_b(\mathbf{R})$ for the topology of uniform convergence. Bochner and von Neumann remarked that if G is a topological group, this characterization visibly provides a notion of almost periodic function (on the right or on the left) on G. At the beginning of the 1930s, the theory promised to develop rapidly, in particular under the impetus of von Neumann [**52**] and the methods of Peter and Weyl.

Another privileged field appears on the margin of the work of N. Wiener. The latter introduces, in a celebrated article [**88**] of 1932, methods of an algebraic nature in the study of the so-called Tauberian problems — that is to say, in the study of the asymptotic behaviour of a function (or a sequence) following a filter, given information concerning the behaviour of certain weighted averages. His approach was motivated by an idea of R. Schmidt.

One of the auxiliary results of Wiener’s work ([**88**, Lemma IIe]) was particularly striking and inspired numerous developments: if $f$ is a periodic function whose Fourier series is absolutely convergent, and if $f$ does not vanish, then the Fourier series of $1/f$ is absolutely convergent (cf. I, p. 38, example). As early as 1932, R. Paley and N. Wiener [**89**] outlined the link between this convergence result, the notion of dual group for a discrete commutative group, and the theory of almost periodic functions.

Against this analytical background, it is algebraic topology that leads L. Pontryagin to give the decisive impetus for the study of characters of locally compact abelian groups. He announces as early as 1932 [**55**] the interest of the notion of character group for putting into duality the homology groups of a compact subset of Euclidean space and those of its complement. In an article [**58**] published in 1934, he shows that the character group of a discrete group is compact, then establishes the duality theorems in this setting. Though Pontryagin uses the results of Peter and Weyl, as well as Haar measure whose existence had just been established in general, he aims mainly at applications to topology [**57**] and does not explicitly concern himself with harmonic analysis[^8]: the duality theorems are proved by a fine study of the structure of compact abelian groups.

Pontryagin’s work immediately arouses great interest. At von Neumann’s suggestion, E. van Kampen extends the duality the following year to all commutative locally compact groups [**37**]. Shortly afterwards, he gives a spectacular application of the new invariant analysis to the study of almost periodic functions [**38**], discovered independently by A. Weil at the same period [**79**]: if G is a locally compact commutative group, one obtains a compact group $\widetilde{G}$ by first endowing the dual group $\widehat{G}$ with the discrete topology, then defining $\widetilde{G}$ as the compact dual group of the discrete group thus obtained. The group G then embeds canonically in $\widetilde{G} ($cf. II, p. 292, exerc. 54) and a simple application of Peter–Weyl theory for continuous functions on $\widetilde{G}$ provides all the results known at the time on almost periodic functions on G.

At the same time, positive definite functions, well known in classical analysis, appear at this period in the study of unitary representations of $\mathbf{R}$. The notion of universally positive kernel had been studied by J. Mercer [**45**] shortly before 1910, in connection with the theory of integral equations, while its analogue for sequences gave rise to quite numerous works during the same period, connected in particular with the moment problem (cf. IV, p. 359, exerc. 21). Meanwhile, positive definite functions on $\mathbf{R}$, already studied systematically by M. Mathias [**43**] in 1923, had become in Bochner’s hands one of the fundamental tools of Fourier analysis and probability theory [**7**]. In 1933, Bochner [**8**] and Riesz [**61**] independently observe that every diagonal matrix coefficient of a unitary representation of $\mathbf{R}$ is a positive definite function on $\mathbf{R}$. This observation enables them to give a simpler proof of Stone’s theorem, and will have a decisive influence on the development of the general theory (cf. n$^o7$).

The results of this period are put in order by A. Weil, in a book completed before 1937 and published in 1940 [**80**]. He sets out there in detail the results of Peter–Weyl, Pontryagin and van Kampen. But in the case of commutative groups, whereas Pontryagin and van Kampen emphasized the structure of groups and the duality theorems, Weil systematically develops harmonic analysis, introducing the Fourier transform and proving Plancherel’s formula and Bochner’s theorem (V, p. 455, th. 5). He emphasizes in particular the role of convolution (under the name “composition product”) and that of positive definite functions, henceforth defined on an arbitrary group and related to diagonal matrix coefficients of representations, at least in the case of finite-dimensional representations.

The generality thus achieved in the commutative case will open a little later new horizons in number theory. As early as 1936, with a view to introducing algebraic methods into class field theory, C. Chevalley [**14**] introduces the group of idèles of a number field, which will appear later as the group of invertible elements of the ring of adèles (cf. AC, VII, p. 221–222, and ÉHM, p. 143). In 1950, J. Tate [**75**] will show that harmonic analysis for groups of adèles and idèles makes it possible to recover easily the functional equations of Hecke L-functions, foreshadowing extraordinary developments linking harmonic analysis on adelic groups and the study of automorphic forms.

But one may say that by the end of the 1930s, the principal results of invariant harmonic analysis had been obtained for compact groups and for commutative locally compact groups. In the commutative case, Weil’s proofs still depend (as do those of Pontryagin and van Kampen) on a fine knowledge of the structure of the group, that is to say, roughly speaking, on the classification results of § 2 of II, p. 244. The following decade will show how to free oneself from this, thanks to the new methods of the Gelfand school (cf. H. Cartan and R. Godement [**12**]).

### 7. Operator algebras

We have seen the role that Riesz, presenting in 1913 the work of the Hilbert school, assigns to the algebra $\mathscr{L}(E)$ of endomorphisms of a Hilbert space, as well as to the holomorphic functional calculus and to the abstract notion of spectrum. In his memoir of 1916, he already seems to announce normed algebras as a natural setting for spectral theory; after the work of Banach and his school in the 1920s, it is hardly surprising that this idea should have taken a central place. The notion of Banach algebra is introduced by M. Nagumo [**48**] in 1936, whereas S. Mazur [**44**], in 1938, shows that the only normed algebra over $\mathbf{C}$ which is a field is $\mathbf{C}$ itself (I, p. 26, cor. 2).

Towards the middle of the 1930s, in connection with spectral theory, occasions to consider abstractly algebras of operators on Hilbert spaces became more and more frequent. F. Murray and J. von Neumann, in a series of profound and influential works [**47**], systematically study the involutive subalgebras of $\mathscr{L}(E)$ equal to their bicommutant (“von Neumann algebras”). On the other hand, in 1936, S. Steen proposes introducing an axiomatic notion of “operator algebra” and studying in depth the associated structures [**70**]. Moreover, Stone [**74**], motivated by the study of spectral projectors, studies in 1937 the unital algebras whose every element is idempotent (“Boolean algebras”: cf. ÉHM, p. 146). He notes that if X is a locally compact topological space, the characteristic functions of the open subsets and those of the complements of the everywhere dense subsets generate, in $\mathscr{C}$ (X), a Boolean algebra A. He then proves that the ideals of A correspond naturally to the closed subsets of the space X, thus introducing an idea which will prove particularly fruitful.

From 1939 onwards, Gelfand’s viewpoint opens new perspectives on these relatively scattered results. His work seems to have been partly motivated by Wiener’s ideas, in particular by his theorem concerning absolutely convergent Fourier series, as well as by the methods of Peter and Weyl. Between 1939 and 1946, in collaboration with M. Naimark, D. Raikov and G. Shilov, Gelfand establishes the foundations of the theory of commutative Banach algebras and of that of star algebras (cf. [**23**], vol. I, p. 169–400). In particular, he gives the classical proof of Wiener’s theorem — generalized by P. Lévy [**39**] — which is found in this book (I, p. 38, example).

In Gelfand’s approach, the essential object to which a commutative Banach algebra A is related is the space X of maximal ideals of A. Indeed, by means of the Gelfand–Mazur theorem (I, p. 26, cor. 2), every element of A defines a function on X. The capital importance which this viewpoint will have in the subsequent development of algebraic geometry is well known (cf. ÉHM, p. 146–148). This approach was itself motivated by Stone’s work on Boolean algebras mentioned above.

It seems that it was L. Loomis, in a course published in 1953 [**41**, p. 53], who first presented Gelfand’s theory by emphasizing the space of characters of A, defining the Gelfand transform in the sense in which we understand it in this book. The clearest advantage of this viewpoint is undoubtedly that the topological properties of the space of characters follow immediately from the compactness of the unit ball of the dual of a Banach space for the weak topology.

From his first works, Gelfand had constructed the holomorphic functional calculus mapping in one variable in a Banach algebra, by means of Cauchy’s integral, and had deduced from it that an involutive Banach algebra admits a non-trivial decomposition into a product of rings when the space of its maximal ideals is not connected. The case of an arbitrary Banach algebra is not treated until 1953, when Shilov develops a form of the functional calculus in several variables [**68**].

As for star algebras, which Gelfand and Naimark had shown as early as 1942 can be realized as algebras of operators on a Hilbert space (cf. V, p. 442, th. 2), they soon became the object of abundant and profound studies, stimulated by applications to group representations, by the work of Murray and von Neumann, and by the mathematical formalization of Quantum Mechanics. Let us mention in particular the contributions of I. Segal, who was one of the pioneers of the systematic study of representations of star algebras, in connection with the study of the unitary dual of locally compact groups which we shall discuss in a few lines.

Though Gelfand, Naimark, Raikov and Shilov had established the essential foundations of the theory of star algebras before 1946, certain technical points were improved subsequently. Thus, R. Arens [**1**] showed how to avoid appealing to the existence of the “Shilov boundary” (cf. I, p. 171, exerc. 26) in order to prove that the Gelfand transform is an involutive morphism. Moreover, Gelfand and Naimark’s theory for unital star algebras initially added as an axiom the fact that $1 +x^*x$ is invertible for every $x$. They nevertheless conjectured that this axiom was unnecessary; the proof of this assertion, elementary but delicate, was only given around 1952, following work of M. Fukamiya [**21**] taken up by I. Kaplansky [**62**].

### 8. Representations of locally compact groups

Until 1939, the study of representations of topological groups was confined to the compact case and the commutative case. Physicists, for their part, had found in Quantum Mechanics numerous reasons for studying irreducible unitary representations in order to seek Hilbert spaces capable of modelling the states of elementary particles. P. Dirac, drawing on work of E. Majorana, had pointed out around 1936 the interest, from this point of view, of the Lorentz group $\mathbf{S}\mathbf{O}(3,1)$ and of the Poincaré group $\mathbf{S}\mathbf{O}(3,1)\ltimes \mathbf{R}^4$. Their methods remained far removed from those of the mathematicians of the time. But in 1939, E. Wigner opened a breach [**90**] when he classified the irreducible unitary representations of the Poincaré group by relying on the work of Murray and von Neumann.

It is to Gelfand that one owes, it seems, having perceived a general path towards the study of representations of locally compact groups. In a memoir written in 1942 (cf. [**23**], vol. II, p. 3–17), he points out with Raikov that such a theory is made possible by the link between unitary representations and functions of positive type. They prove the existence of a Hilbertian realisation for every function of positive type (V, p. 432, th 1) and deduce from this that irreducible unitary representations separate the points of G (V, p. 454, th. 4). The positive linear forms on the involutive algebra $L^1(G)$ play an essential role: Gelfand and Raikov show the link which unites them with functions of positive type (cf. V, p. 448, prop. 13). The enveloping star algebra of an involutive algebra is presented (without a name) in [**24**, § 48], although there is not yet a direct question of associating with G the algebra Stell(G) (cf. 9, déf. de I, p. 125).

After 1945, the study of unitary representations developed by great strides. The interaction with star algebras, as well as with the analysis of the foundations of quantum theory, quickly provided valuable general results: around 1947, Segal associated various[^9] star algebras with a locally compact group [**67**], and wove the link between their representations and those of the group considered. Shortly afterwards, G. Mackey brought out the notion of induced representation [**42**], which was to be omnipresent in the concrete results on unitary representations.

At the same time, the theory was considerably stimulated by the study of examples which reveal its variety and depth. Gelfand and Naimark, studying the example of $\mathbf{S}\mathbf{L}(2,\mathbf{C})$, brought out in 1947 a particular case of the notion of induced representation, then showed that it is the key to the study of the representations of this group [**23**, vol. II, p. 41– 124]. The same year, V. Bargmann studied [**5**] the group $\mathbf{S}\mathbf{L}(2,\mathbf{R})$ and discovered the existence of a countable family of square integrable representations, called “discrete series” (discrete series), as well as the orthogonality relations between their matrix coefficients (cf. prop. 8 of V, p. 424). As Godement immediately realised [**25**], Bargmann’s orthogonality relations are satisfied by all square integrable representations of locally compact groups.

Soon the study of particular classes of groups would again, and for a long time, take precedence over the abstract theory. Harish-Chandra, in particular, would begin the general study of representations of reductive Lie groups — an epic task which we cannot describe here, any more than the prodigious consequences which Langlands would foresee for number theory.

[^1]: Let us recall that it was Poincaré who, guided by the problem of the “vibrating membranes” where the notion of eigenvalue played an essential role, had introduced a parameter $\lambda$ in (1) and suggested studying the dependence on $\lambda$ of the solutions (cf. ÉHM, p. 262).
[^2]: For Hilbert, the relation defining values and eigenvectors is the equality $\varphi_n(t) =\lambda_n\int_IK(s, t)\varphi_n(s)ds$; the “eigenvalues” which he mentions are therefore the inverses of those sanctioned by modern terminology, and can be infinite. As we shall see, the change was proposed by F. Riesz in 1913.
[^3]: As Hilbert remarks, one can characterise $\sigma (s, x) =\sum_{p,q=0}^{\infty}\sigma_{pq}(s)x_px_q$ by the fact that it satisfies $\int_{\mathbf{R}}d\sigma (s, x) =\|x\|^2$ and that for every continuous function $u$ on $\mathbf{R}$, one has $\sum_{r=0}^{\infty}\int_{\mathbf{R}}u(s)d\sigma_{pr}(s)\int_{\mathbf{R}}u(s)d\sigma_{rq}(s) =\int_{\mathbf{R}}u(s)^2d\sigma_{pq}(s)$.
[^4]: This equivalence is still valid in the case of a reflexive Banach space, but the two notions are different in general: cf. III, p. 7, prop. 8.
[^5]: This notion was known to algebraists at the end of the xix$^e$ century, and used by Toeplitz [**76**] in an analytic setting in 1918.
[^6]: This is the general form of a positive element of $\mathscr{C}$(G), cf. n$^o2$ of I, p. 118.
[^7]: This is the algorithm which enabled Schmidt, drawing inspiration from the work of Schwarz and considering the “iterates” of the kernel $K_{\varphi}$, to simplify the results of Fredholm and Hilbert in his thesis of 1905.
[^8]: This does not mean that Pontryagin neglected Analysis: in a short note [**56**] of 1933, appended to a contribution by Stepanoff and Tychonoff concerning almost periodic functions on $\mathbf{R}$, he had reformulated their result by means of two Abelian groups in duality.
[^9]: As early as 1941, Segal proposed associating a Banach algebra with such a group G in order to study representations; but at that time he had rather in mind the algebra obtained from $L^1(G)$ by adjunction of a unit element. In 1947, in an influential article, he associated a star-algebra with G with a view to the decomposition of the regular representation; what he then introduced was rather the "reduced" star-algebra, quotient of Stell(G) by the kernel of the regular representation, than the universal star-algebra itself. The latter seems to appear in its modern guise in 1960 in a text of J. Fell [**20**].
