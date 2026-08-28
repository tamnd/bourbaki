---
book: hist
book_title: Elements of the History of Mathematics
chapter: "1"
chapter_title: ELEMENTS OF THE HISTORY OF MATHEMATICS
section: 25
section_title: Lie Groups and Lie Algebras
lang: en
source: hist
pdf_pages: 0247-0267
extraction: ocr
statements: 0
exercises: 0
content_sha256: 758f790e5baf428b457b35b0bb0942e6c9333e16ace540ad6af8edad1dd35da6
---

## 25. LIE GROUPS AND LIE ALGEBRAS.

I. GENESIS.

The theory, which has been called for almost a century the “theory of Lie groups”, was essentially set up by one mathematician: Sophus Lie.
Before starting on its history, we will summarise briefly various earlier researches that prepared its development.

a) Transformations (Klein-Lie, 1869-1872).

Around 1860, the theory of permutation groups of a finite set is developing and begins to be used (Serret, Kronecker, Mathieu, Jordan). On the other hand, the theory of invariants, then in full flight, familiarises mathematicians with certain infinite sets of geometric transformations closed under composition (notably linear or projective transformations). But, before the work of 1868 of Jordan [174 b] on the “movement groups” (closed subgroups of the groups of displacements in Euclidean space of 3 dimensions), it does not seem as if any conscious link had been established between these two streams of ideas.

In 1869, the young Felix Klein (1849-1925), a pupil of Plücker, becomes the friend at Berlin of the Norwegian Sophus Lie (1842-1899), a few years older, being brought together by their common interest in the “geometry of straight lines” of Plücker and notably the theory of complexes of straight lines (p. 133). It is around this period that Lie conceives of one of his most original ideas, the introduction of the notion of invariant in Analysis and in differential geometry; one of the sources of this is his observation that the classical methods of integration “by quadratures” of differential equations all rely on the fact that the equation is invariant for a “continuous” family of transformations. It is from 1869 that is dated the first work (drawn up by Klein) where Lie uses this idea; he studies there the “Reye complex” (a set of straight lines intersecting the faces of a tetrahedron in 4 points having a given cross-ratio) and the curves and surfaces having as tangents straight lines of this complex ([202], vol. I, Abh. V, pp. 68-77): his method relies on the invariance of the Reye complex under the commutative group with 3 parameters (a maximal torus of $\mathbf{PGL}(4, \mathbf{C})$) leaving invariant the corners of the tetrahedron. This same idea dominates the work written together by Klein and Lie when they found themselves in Paris in the spring of 1870 ([182], v. I, pp. 416-420); they essentially determine there the connected commutative subgroups of the projective group of the plane $\mathbf{PGL}(3, \mathbf{C})$, and study the geometric properties of their orbits (under the name of V curves or surfaces); that gives them, by a uniform procedure, properties of varied curves, algebraic or transcendental, such as $y = cx^m$ or the logarithmic spirals. Their testimony agrees in underlining the profound impression that was produced on them by the theories of Galois and of Jordan (the commentary of Jordan on Galois had appeared in Math. Annalen in 1869; in any case, Lie had heard of the theory of Galois already in 1863). Klein, who in 1871, begins to be interested in non-Euclidean geometries, sees there the beginning of his research for a classification principle for all known geometries, research that was to lead him in 1872 to the "Erlangen programme". On his side, Lie in a letter of 1873 to A. Mayer ([202], vol. 5, p. 584), dates from his stay in Paris the origin of his ideas on transformations groups, and in a work of 1871 ([202], vol. I, Abh. XII, pp. 153-214), he uses already the term "transformation group" and states explicitly the problem of the determination of all the subgroups ("continuous or discontinuous") of $\mathbf{GL}(n, \mathbf{C})$. Truth to tell, Klein and Lie must both have had difficulty in penetrating this new mathematical universe, and Klein speaks of the "Treatise" of Jordan, newly appeared, as a "book sealed with seven seals" ([182], v. I, p. 51); he writes elsewhere in connection with ([182], v. I, pp. 424-459): "It is to Lie that belongs all that is concerned with the heuristic idea of a continuous group of operators, in particular all that touches on the integration of differential equations or partial differential equations. All the notions that he developed later in his theory of continuous groups were already to be found in embryo with him, but so little elaborated however, that I had to convince him of many details, for example at the beginning even the existence of the curves $V$, during the course of long conversations" ([182], v. I, p. 415).

b) Infinitesimal transformations.

The conception of an "infinitely small" transformation goes back to the beginnings of the infinitesimal Calculus; it is known that Descartes discovers the instantaneous centre of rotation by assuming that "in the infinitely small" every plane movement can be assimilated into a rotation; the elaboration of analytic Mechanics, in the XVIIIth century, is entirely founded on similar ideas. In 1851, Sylvester, seeking to form invariants of the linear group

$GL(3, \mathbf{C})$ or of certain of its subgroups, gives to the parameters $z_j$ occurring in these matrices "infinitely small" increments of the form $\alpha_j dt$, and expresses that a function $f((z_j))$ is invariant by writing down the equation $f((z_j + \alpha_j dt)) = f((z_j))$; this gives him a linear equation for $f$ with partial derivatives $Xf = 0$, where

$$
Xf = \sum_j \alpha_j \frac{\partial f}{\partial z_j},
$$

$X$ being thus a *differential operator*, "a derivative in the direction of directed parameters $\alpha_j$" ([304], vol. 3, pp. 326 and 327); Sylvester seems to feel that there is there a general principle of fairly wide scope, but does not seem to have returned to the question. A little later, Cayley ([58], v. II, pp. 164-178) proceeds in the same way for invariants of $SL(2, \mathbf{C})$ in certain representations of this group and shows that it is the solution of two partial differential equations of the first order $Xf = 0, Yf = 0$, where $X$ and $Y$ are obtained as above starting from "infinitely small" transformations

$$
\begin{pmatrix}
0 & 0 \\
dt & 0
\end{pmatrix}
\text{ and }
\begin{pmatrix}
0 & dt \\
0 & 0
\end{pmatrix}.
$$

In modern terms, this is explained by the fact that $X$ and $Y$ generate the Lie algebra $\mathfrak{sl}(2, \mathbf{C})$; besides Cayley calculates explicitly the bracket $XY - YX$ and shows that it also comes from an "infinitely small" transformation.

In his memoir of 1868 on groups of movements [174 b], Jordan uses from beginning to end the concept of "infinitely small transformation", but exclusively from a geometric point of view. There is no doubt that it is with him that the idea of a group with one parameter "generated" by an infinitely small transformation appears: for Jordan, it is the set of transformations obtained by "repeating suitably" the infinitely small transformation (*loc. cit.* p. 243). Klein and Lie, in their memoir of 1871, use the same expression "repeated infinitely small transformation" ([182], v. I, pp. 424-459), but the context shows that they mean by that an integral of a differential system. If the group with one parameter that they consider is made up of transformations $x' = f(x, y, t), y' = g(x, y, t)$, the corresponding "infinitely small transformation" is given by

$$
dx = p(x, y) dt, \quad dy = q(x, y) dt
$$

where $p(x, y) = \frac{\partial f}{\partial t}(x, y, t_0), q(x, y) = \frac{\partial g}{\partial t}(x, y, t_0)$, where $t_0$ corresponds to the identical transformation of the group. As Klein and Lie know the functions $f$ and $g$ explicitly, they have no problem in checking that the functions

$$
t \mapsto f(x, y, t) \text{ and } t \mapsto g(x, y, t)
$$

give in a parametric form the integral curve of the differential equation

$$
q(\xi, \eta) d\xi = p(\xi, \eta) d\eta
$$

going through the point $(x, y)$, but do not give any general reason for that; besides they do not use this fact again in the rest of their memoir.

c) Contact transformations.

In the following two years, Lie seems to abandon the theory of transformation groups (although he remains in very close contact with Klein, who publishes in 1872 his "Programme") in order to study contact transformations, the integration of partial differential equations of the first order and the relations between these two theories. We do not have to spell out the history of these questions here, and we will limit ourselves to mentioning a few points that seem to have played an important role in the genesis of the theory of transformation groups.

The notion of contact transformation generalises at the same time the point transformations and the transformations by reciprocal polars. Grosso modo, a contact transformation$^1$ in $C^n$ is an isomorphism of an open set $\Omega$ of the variety $T'(C^n)$ of cotangent vectors to $C^n$ onto another open set $\Omega'$ of $T'(C^n)$ transforming the canonical 1-form of $\Omega$ into that of $\Omega'$. In other words, if $(x_i, \ldots, x_n, p_1, \ldots, p_n)$ describes the canonical co-ordinates of $T'(C^n)$, a contact transformation is an isomorphism $(x_i, p_i) \mapsto (X_i, P_i)$ satisfying the relation $\sum_{i=1}^n P_i dX_i = \sum_{i=1}^n p_i dx_i$. Such transformations occur in the study of partial differential equations of the form

$$
F \left( x_1, x_2, \ldots, x_n, \frac{\partial z}{\partial x_1}, \ldots, \frac{\partial z}{\partial x_n} \right) = 0
$$

Lie becomes familiar during the course of his research on these questions with the handling of Poisson parentheses

$$
(f, g) = \sum_{i=1}^n \left( \frac{\partial f}{\partial x_i} \frac{\partial g}{\partial p_i} - \frac{\partial g}{\partial x_i} \frac{\partial f}{\partial p_i} \right)
$$

and brackets$^2$ $[X, Y] = XY - YX$ of differential operators of type (25.1); he interprets the Poisson parenthesis (25.3) as the effect on $f$ of a transforma-

$^1$ It is a case here of "homogeneous" contact transformations. Previously, the consideration of equations of type (25.2), but where $z$ occurs in $F$, had led Lie to consider contact transformations with $2n + 1$ variables $z, x_1, \ldots, x_n, p_1, \ldots, p_n$, where it is a case of finding $2n + 2$ functions $Z, P_i, X_i (1 \leq i \leq n)$ and $\rho$ (this latter $\neq 0$ at all points) such that $dZ - \sum_i P_i dX_i = \rho(dz - \sum_i p_i dx_i)$. This case which appears to be more general is reduced easily in fact to the "homogeneous" case ([203], v. 2, pp. 135-146).

$^2$ These occurred already in the theory of Jacobi-Clebsch in "complete systems" of partial differential equations of the first order $X_j f = 0 (1 \leq j \leq r)$, a notion equivalent to that of "completely integrable system" of Frobenius: the fundamental theorem (equivalent to the "Frobenius theorem") which characterises these systems is that the brackets $[X_i, X_j]$ must be linear combinations (with variable coefficients) of the $X_k$.

tion of type (25.1) associated with $g$, and observes on this occasion that the Jacobi identity for Poisson parentheses means that the bracket of differential operators corresponding to $g$ and $h$ is associated with the parenthesis $(g, h)$. The search for functions $g$ such that $(F, g) = 0$, which occurs in the method of Jacobi for integrating the partial differential equation (25.2), becomes for Lie that for an infinitesimal contact transformation leaving the given equation invariant. Finally, Lie is led to study the set of functions $(u_j)_{1 \leq j \leq m}$ of the $x_i$ and the $p_i$ such that the parentheses $(u_j, u_k)$ are functions of the $u_h$, and calls these sets "groups" (already considered in substance by Jacobi).

II. CONTINUOUS GROUPS AND INFINITESIMAL TRANSFORMATIONS.

Suddenly, in the autumn of 1873, Lie takes up again the study of transformation groups and obtains decisive results. For as much as it is possible to follow the unravelling of his thoughts in a few letters to A. Mayer from the years 1873-1874 ([202], vol. 5, pp. 585-608), he starts from a "continuous group" of transformations on $n$ variables

$$
x'_i = f_i(x_1, \ldots, x_n, a_1 \ldots, a_r) \quad (1 \leq i \leq n)
$$

depending effectively$^3$ on $r$ parameters $a_1, \ldots, a_r$; he observes that if the transformation (25.4) is the identity for the values $a_1^0, \ldots, a_r^0$ of the parameters,$^4$ then the Taylor expansions of the $x_i$, limited to the first order:

$$
f_i(x_1, \ldots, x_n, a_1^0 + z_1, \ldots, a_r^0 + z_r) = x_i + \sum_{k=1}^r z_k X_{ki}(x_1, \ldots, x_n) + \ldots (1 \leq i \leq n)
$$

give a "generic" infinitely small transformation depending linearly on the $r$ parameters $z_j$

$$
dx_i = \left( \sum_{k=1}^r z_k X_{ki}(x_1, \ldots, x_n) \right) dt \quad (1 \leq i \leq n).
$$

Proceeding as in his memoir with Klein, Lie integrates the differential system

$^3$ Lie means by that that the $f_i$ can not be expressed by means of less than $r$ functions of the $a_j$, or equally that the Jacobian matrix $(\partial f_i / \partial a_j)$ is of rank $r$ "in general".

$^4$ In his first notes, Lie believes himself able to prove *a priori* the existence of the identity and of the inverse in all sets of transformations (4) closed under composition; he recognises later that his proof was incorrect, and Engel supplies him with a counterexample reproduced in ([203], v. I, §44). However Lie shows how to reduce the "continuous" systems (4) closed under composition to groupuscules of transformations: such a system is of the form $G \circ h$, where $G$ is a groupuscule of transformations and $h$ is a transformation of the system ([203], v. I, th. 26, p. 163, and v. 3, th. 46, p. 572).

$$
\frac{d\xi_1}{\sum_k z_k X_{k1}(\xi_1, \ldots, \xi_n)} = \cdots = \frac{d\xi_n}{\sum_k z_k X_{kn}(\xi_1, \ldots, \xi_n)} = dt,
$$
which gives him, for each point $(z_1, \ldots, z_r)$, a group with one parameter
$$
t \mapsto x_i' = g_i(x_1, \ldots, x_n, z_1, \ldots, z_r, t) \quad (1 \leq i \leq n)
$$
such that $g_i(x_1, \ldots, x_n, z_1, \ldots, z_r, 0) = x_i$ for every $i$. He shows in an ingenious way, using the fact that the transformations (25.4) make up a set closed under composition, that the group with one parameter (25.8) is a subgroup of the given group ([202], vol. 5, Abh. VII, pp. 32-63). The new idea, key to the whole theory, is to proceed on to the second order in the Taylor expansions of the functions (25.4). The thread of his argument is fairly confused and heuristic ([202], vol. 5, Abh. VII, pp. 32-63 and [202], vol. 5, pp. 600-601); it can be set out as follows. For the $z_j$ that are fairly small, one can put $t = 1$ in (25.8), and thus are obtained new parameters $z_1, \ldots, z_r$ for the transformations of the group (it is in fact the first appearance of the "canonical parameters"). By definition, we have with regard to (25.7)
$$
\frac{\partial g_i}{\partial t} = \sum_k z_k X_{ki}(x_1', \ldots, x_n'),
$$
from where
$$
\frac{\partial^2 g_i}{\partial t^2} = \sum_{k,j} z_k \frac{\partial X_{ki}}{\partial x_j}(x_1', \ldots, x_n') \frac{\partial x_j'}{\partial t} =
\sum_{k,j} z_k \frac{\partial X_{ki}}{\partial x_j}(x_1', \ldots, x_n') \left( \sum_h z_h X_{hj}(x_1', \ldots, x_n') \right)
$$
which gives
$$
x_i' = x_i + (\sum_k z_k X_{ki}(x_1, \ldots, x_n)) t
$$
$$
+ \frac{1}{2} \left( \sum_{k,h,j} z_k z_h \frac{\partial X_{ki}}{\partial x_j}(x_1, \ldots, x_n) X_{hj}(x_1, \ldots, x_n) \right) t^2 + \ldots,
$$
from where, for $t = 1$, the Taylor expansions with respect to the parameters $z_j$
$$
x_i' = x_i + \left( \sum_k z_k X_{ki} \right) + \frac{1}{2} \left( \sum_{k,h,j} z_k z_h X_{hj} \frac{\partial X_{ki}}{\partial x_j} \right) + \ldots (1 \leq i \leq n).
$$
Let us write these relations in brief as $x' = G(x, z)$ between vectors
$$
x = (x_1, \ldots, x_n), \; x' = (x_1', \ldots, x_n'), \; z = (z_1, \ldots, z_r);
$$

the fundamental property of closure of the sets of these transformations under composition is written as

$$
G(G(x, u), v) = G(x, H(u, v))
$$

where $H = (H_1, \ldots, H_r)$ is independent of $x$; it is immediate that $H(u, 0) = u, H(0, v) = v$, whence the expansions

$$
H_i(u, v) = u_i + v_i + \frac{1}{2} \sum_{h,k} c_{ikh} u_h v_k + \ldots,
$$

the terms not written down being non linear either in $u$ or in $v$. Transforming (25.10) with the help of (25.9) and (25.11), then comparing the terms in $u_h v_k$ of the two members, Lie obtains the relations

$$
\sum_{j=1}^n \left( X_{hj} \frac{\partial X_{ki}}{\partial x_j} - X_{kj} \frac{\partial X_{hi}}{\partial x_j} \right) = \sum_{l=1}^r c_{lhk} X_{li} \quad (1 \leq h, k \leq r, 1 \leq i \leq n).
$$

His expertise with the theory of partial differential equations leads him to write these conditions in a simpler form: following the model of (25.1), he associates with each of these $r$ infinitely small transformations obtained by putting $z_k = 1, z_h = 0$ for $h \neq k$ in (25.6), the differential operator

$$
A_k(f) = \sum_{i=1}^n X_{ki} \frac{\partial f}{\partial x_i},
$$

and rewrites the conditions (25.12) in the form

$$
[A_h, A_k] = \sum_l c_{lhk} A_l,
$$

a keystone of his theory. Until then, he had used indiscriminately the terms "infinitely small transformation" and "infinitesimal transformation" (*e.g.* [202], vol. 5, Abh. I, pp. 1-4); the simplicity of the relations (25.14) leads him to call the operator (25.13) the "symbol" of the infinitesimal transformation $dx_i = X_{ki} dt$ ($1 \leq i \leq n$) ([202], vol. 5, Abh. III, pp. 42-75) and very rapidly, it is the operator (25.13) itself that he will call *infinitesimal transformation* ([202], vol. 5, Abh. III, pp. 42-75 and [202], vol. 5, p. 589).

He then becomes aware of the tight links which unite the theory of "continuous groups" with his previous research on contact transformations and partial differential equations. This link fills him with enthusiasm: *"My old work was so to speak all ready in advance to found the new theory of groups of transformations"* he wrote to Mayer in 1874 ([202], vol. 5, p. 586).

In the following years, Lie pursued the study of transformation groups. Apart from the general theorems summarised here (§ III), he obtains a certain number of more particular results: the determination of transformation groups of the straight line and of the plane, subgroups of small codimension in projective groups, groups with at most 6 parameters, etc.. For all that he does not abandon differential equations. In fact, it even appears that for him, the theory of transformation groups was to be an instrument for integrating differential equations, where the transformation group would play a role analogous to that of the Galois group of an algebraic equation.$^5$ Let us note that this research leads him likewise to introducing certain sets of transformations with an infinity of parameters, which he calls “infinite and continuous groups”;$^6$ he keeps the name “finite and continuous groups” for the transformation groups with a finite number of parameters of type (25.4) above.

III. THE “DICTIONARY” LIE GROUPS — LIE ALGEBRAS.

The theory of “finite and continuous” groups, developed by Lie in numerous memoirs starting in 1874, is set out systematically in the imposing treatise “Theorie der Transformationsgruppen” ([203], 1888-1893), written in collaboration with F. Engel;$^7$ it is the object of the first volume and of the last five chapters of the third, the second being consecrated to contact transformations.

As the title indicates, there was never any question in this work of anything other than transformation groups, in the meaning of the equations (25.4), where the space of “variables” $x_i$ and the space of “parameters” $a_j$ initially both play equally important roles. Besides the concept of “abstract” group is not clearly expressed at this time; when in 1883 ([202], vol. 5, Abh. XII, pp. 311-313) Lie remarks that with the notation of (25.10), the equation $w = H(u, v)$, which gives the parameters of the product of two transformations of the group, defines a new group, it is as a *transformation group* on the space of parameters that he is considering it, obtaining thus what he calls the

$^5$ This research only had a small influence on the general theory of differential equations, the group of automorphisms of such an equation being most often trivial. On the contrary, for certain types of equations (for example linear ones), interesting results were obtained subsequently by Picard, Vessiot, then, more recently, Ritt and Kolchin.

$^6$ They are called today “Lie pseudo-groups”; we must be careful not to confuse them with the “Banach” Lie groups.

$^7$ From 1886 to 1898, Lie occupied at Leipzig the chair left vacant by Klein and had Engel as assistant; this circumstance favoured the flowering of an active mathematical school as well as the diffusion of the ideas of Lie, fairly poorly known until then (because, notably, of the fact that his first memoirs were most often written in Norwegian, and published in the Comptes Rendus of the Academy of Christiania, poorly propagated elsewhere). It is thus that at a time when it was hardly usual for young French mathematicians to go to study in Germany, E. Vessiot and A. Tresse spent a year of study at Leipzig, with Sophus Lie.

"group of parameters" (he even obtains two of them, which are none other than the group of left translations and the group of right translations).8

The variables $x_i$ and the parameters $a_j$ in the equations (25.4) are assumed complex in principle (except in chaps. XIX-XXIV of v. 3), and the functions $f_i$ analytic; Lie and Engel are of course conscious of the fact that these functions are not in general defined for all complex values of the $x_i$ and the $a_j$ and that, in consequence, the composition of such transformations raises serious difficulties ([203], v. I, pp. 15-17, pp. 33-40 and passim); and although, later, they express themselves almost always as if composition of the transformations that they study were always possible without restriction, it is no doubt only for the convenience of the statements, and they re-establish explicitly the "local" point of view each time that it is necessary (cf. loc. cit., pp. 168 or 189 for example or ibid., v. 3, p. 2, note at the bottom of the page); in other words, the mathematical object that they are studying is near to what we would now call a partial operation law. They do not fail to consider, on occasion, global groups, for example the 4 series of classical groups ([203], v. 3, p. 682), but do not seem to have set themselves the question of what in general a "global group" can be; it suffices for them to be able to obtain, for the "parameters" of the classical groups (the "variables" of these groups do not introduce any difficulty, since it is a case of linear transformations of $\mathbf{C}^n$), systems of "local" parameters in the neighbourhood of the identical transformation, without their being concerned about the domain of validity of the formulae that they write down. They set themselves however one problem that stands out clearly from the local theory:9 the study of "mixed" groups, that is to say groups having a finite number of connected components, such as the orthogonal group ([203], v. I, p. 7). They present this study as that of a set of transformations closed under composition and taking inverses, which is the union of sets $H_j$ such that each is described by systems of functions $f_i^{(j)}$ as in (25.4); the number of (essential) parameters of each $H_j$ is even assumed $a$ priori to depend on $j$, but they show in fact that this number is the same for all the $H_j$. Their main result is then the existence of a finite continuous group $G$ such that $H_j = G \circ h_j$ for an $h_j \in H_j$ and for all $j$; they establish also that $G$ is normal in the mixed group and remark that the determination of the invariants of this latter reduces to that of the invariants of $G$ and of a discontinuous group ([203], v. I, chap. 18).

The general theory developed in [203] finishes up (without that being stated in a very systematic way by the authors) by forging a "dictionary" making the translation from properties of "finite continuous" groups to those

8 The analogous notion for groups of permutations had been introduced and studied by Jordan in his "Traité".
9 Let us remember that (p. 119), following a Note of H. Poincaré ([251], v. V, pp. 77-79) various authors have studied the group of invertible elements of an associative algebra of finite dimension. It is interesting to note in this connection that E. Study, in his work on this subject, introduces a symbolism that reduces in substance to considering the abstract group defined by the group of parameters.

of the set of their infinitesimal transformations. It is based on the "three theorems of Lie", each one of which is made up of an assertion and its converse.

The first theorem ([203], v. I, pp. 33 and 72 and v. 3, p. 563) affirms in the first instance that if in (25.4) the parameters are effective, the functions $f_i$ satisfy a system of partial differential equations of the form

$$
\frac{\partial f_i}{\partial a_j} = \sum_{k=1}^r \xi_{ki}(f(x, a)) \psi_{kj}(a) \quad (1 \leq i \leq n)
$$

where the matrix $(\xi_{kl})$ is of maximum rank and $\det(\psi_{kj}) \neq 0$; reciprocally, if the functions $f_i$ have this property, the formulae (25.4) define a groupuscule of transformations.

The second theorem ([203], v. I, pp. 149 and 158, and v. 3, p. 590) gives relations between the $\xi_{ki}$ on the one hand, the $\psi_{ij}$ on the other: the conditions on the $\xi_{ki}$ can be written in the form

$$
\sum_{k=1}^n \left( \xi_{ik} \frac{\partial \xi_{jl}}{\partial x_k} - \xi_{jk} \frac{\partial \xi_{il}}{\partial x_k} \right) = \sum_{k=1}^r c_{ij}^k \xi_{kl} \quad (1 \leq i, j \leq r, 1 \leq l \leq n)
$$

where the $c_{ij}^k$ are constants $(1 \leq i, j, k \leq r)$ anti-symmetric in $i, j$. The conditions on the $\psi_{ij}$ in the form given by Maurer, are:

$$
\frac{\partial \psi_{kl}}{\partial a_m} - \frac{\partial \psi_{km}}{\partial a_l} = \frac{1}{2} \sum_{1 \leq i, j \leq r} c_{ij}^k (\psi_{il} \psi_{jm} - \psi_{jl} \psi_{im}) (1 \leq k, l, m \leq r).
$$

By introducing the matrix $(\alpha_{ij})$ contragredient to $(\psi_{ij})$ and the infinitesimal transformations

$$
X_k = \sum_{i=1}^n \xi_{ki} \frac{\partial}{\partial x_i}, \quad A_k = \sum_{j=1}^r \alpha_{kj} \frac{\partial}{\partial a_j} \quad (1 \leq k \leq r),
$$

(25.16) and (25.17) can be written respectively:

$$
[X_i, X_j] = \sum_{k=1}^r c_{ij}^k X_k \quad (1 \leq i, j \leq r)
$$
$$
[A_i, A_j] = \sum_{k=1}^r c_{ij}^k A_k.
$$

Conversely, if given $r$ infinitesimal transformations $X_k (1 \leq k \leq r)$, linearly independent and satisfying conditions (25.19), the one parameter subgroups generated by these transformations generate a group of transformations with $r$ essential parameters.

Finally, the third theorem ([203], v. I, pp. 170 and 297 and v. 3, p. 597) reduces the determination of systems of infinitesimal transformations $(X_k)_{1 \leq k \leq r}$ satisfying (25.19) to a purely algebraic problem: we must have

$$
c_{ij}^k + c_{ji}^k = 0 \tag{25.21}
$$
$$
\sum_{l=1}^r (c_{il}^m c_{jk}^l + c_{kl}^m c_{ij}^l + c_{jl}^m c_{ki}^l) = 0 \quad (1 \leq i, j, k, m \leq r). \tag{25.22}
$$

Conversely,$^{10}$ if (25.21) and (25.22) are satisfied, there exists a system of infinitesimal transformations satisfying relations (25.19), from whence a group of transformations with $r$ parameters (in other words, the linear combinations with constant coefficients of the $X_k$ make up a Lie algebra, and conversely every Lie algebra of finite dimension can be obtained in this way).

These results are completed by the study of isomorphism questions. Two groups of transformations are said to be *similar* if it is possible to pass from one to the other by an invertible transformation of co-ordinates on the variables and an invertible transformation of co-ordinates on the parameters: from the beginning of his research, Lie had met this notion in a natural way in connection with the definition of the "canonical parameters". He shows that two groups are similar if, by means of a transformation on the "variables", one can bring the infinitesimal transformations of the one onto those of the other ([203], v. I, p. 329). A necessary condition for this to be so is that the Lie algebras of the two groups be isomorphic, which Lie expresses by saying that the groups are *"gleichzusammengesetzt"*, but this condition is not sufficient, and a whole chapter ([203], v. I, chap. 19) is devoted to obtaining supplementary conditions insuring that the groups should be "similar". On the other hand the theory of permutation groups supplied the notion of the "holoedric isomorphism" of two such groups (isomorphism of the underlying "abstract" groups); Lie transposes this notion to groups of transformations, and shows that two such groups are "holoedric isomorphic" if and only if their Lie algebras are isomorphic ([203], v. I, p. 418). In particular, every group of transformations is holoedrically isomorphic to each of its groups of parameters, and that shows that, when one wishes to study the structure of the group, the "variables" on which they operate do not matter much and that in fact everything reduces to the Lie algebra.$^{11}$

Always by analogy with the theory of permutation groups. Lie introduces the notions of subgroups, normal subgroups, "meriedric isomorphisms" (surjective homomorphisms), and shows that they correspond to that of sub-algebras, ideals and surjective homomorphisms of Lie algebras; besides he

$^{10}$ This converse was not obtained without trouble. The first proof that Lie gives of it ([202], vol. 5, Abh. III, pp. 42-75) consists in passing over to the adjoint group and is in fact only valid if the centre of the given Lie algebra is reduced to 0. He later gives two general proofs of it ([203], v. 2, chap. XVII and v. 3, pp. 599-604); it is fairly significant that the first is based on contact transformations and that Lie finds it more natural than the second.

$^{11}$ It can be noticed that there is a similar evolution in the theory of "abstract" groups, in particular finite ones. They were first defined as groups of transformations, but already Cayley remarked that what is essential is the manner in which the transformations are composed together, and not the nature of the concrete representation of the group of permutations of particular objects.

had met very early on a particularly important example of "meriedric isomorphism", the adjoint representation, and had recognised its links with the centre of the group ([202], vol. 5, Abh. III, pp. 42-75). For these results, as for the fundamental theorems, the essential tool is the theorem of Jacobi-Clebsch giving the complete integrability of a differential system (one of the forms of the theorem called "of Frobenius"); he gives a new proof of it, as it happens, using groups with one parameter ([203], v. I, chap. 6).

The notions of transitivity and of primitivity, so important for groups of permutations, arise also naturally for the "finite and continuous" groups of transformations, and the treatise of Lie-Engel makes a detailed study of them ([203], v. I, chap. 13 and passim); the relations with the subgroups stabilising a point and the notion of homogeneous space are observed (for as much as they could be without putting oneself in a global point of view) ([203], v. I, p. 425).

Finally, the "dictionary" is completed, in [203], by the introduction of the notions of derived group and soluble group (called "integrable group" by Lie; this terminology, suggested by the theory of differential equations, will remain in use until the work of H. Weyl) ([203], v. I, p. 261 and v. 3, pp. 678-679); the relation between commutators and brackets had besides been observed by Lie already in 1883 ([202], vol. 5, p. 358).

Other proofs of fundamental theorems.

In [278 b], F. Schur shows that in canonical co-ordinates the $\psi_{ik}$ of (15) satisfy the differential equations

$$
\frac{d}{dt}(t\psi_{ik}(ta)) = \delta_{ik} + \sum_{j,l} c^k_{jl} ta_l \psi_{ji}(ta).
$$

These integrate and give a formula equivalent to the formula

$$
\varpi(X) = \sum_{n \geq 0} \frac{1}{(n+1)!} (\mathrm{ad}(X))^n
$$

for the right differential $\varpi(X)$ of the exponential map at the point $X$; in particular, in canonical co-ordinates, the $\psi_{ij}$ are extended into entire functions of the $a_k$. F. Schur deduces from this a result making precise an earlier remark of Lie: if, in the definition (25.4) of groups of transformations, it is only assumed that the $f_i$ are in the class $C^2$, then the group is holoedrically isomorphic to an analytic group.$^{12}$ Following his research on the integration

$^{12}$ Lie had already stated without proof a result of this kind ([202], vol. 6, Abh. V, pp. 230-236). He had been led to it by his research on the foundations of geometry ("problem of Helmhotz"), where he had remarked that the hypotheses of analyticity are not natural.

of differential systems, E. Cartan ([52 a], v. II_2, p. 371) introduces in 1904 the Pfaffian forms

$$
\omega_k = \sum_{i=1}^r \psi_{ki} da_i \quad (1 \leq i \leq r)
$$

(with the notation of (25.15)), later called *Maurer-Cartan forms*. The conditions (25.17) of Maurer can then be written

$$
d\omega_k = -\frac{1}{2} \sum_{i,j} c_{ij}^k \omega_i \wedge \omega_j;
$$

E. Cartan shows that it is possible to develop the theory of finite continuous groups starting with the $\omega_k$ and establishes the equivalence of this point of view and that of Lie. But, for him, the interest in this method is especially that it adapts itself to "infinite and continuous" groups for which he pushes the theory much further that had been done by Lie, and that it allows the setting up of his theory of the generalised "mobile marker".

IV. THE THEORY OF LIE ALGEBRAS.

Once the correspondence between groups of transformations and Lie algebras is acquired, the theory is going to take a clearly more algebraic turn and will be centred on a deep study of Lie algebras.$^{13}$

A first and short period, from 1888 to 1894, marked by the work of Engel, of his pupil Umlauf and especially Killing and E. Cartan, ended up with a series of spectacular results on complex Lie algebras. We have seen above that the notion of soluble Lie algebra was due to Lie himself, who had proved (in the complex case) the reduction theorem for soluble linear Lie algebras to triangular form ([203], v. I, p. 270).$^{14}$ Killing observes [180] that there exists in a Lie algebra a biggest soluble ideal (that is called the radical today), and that the quotient of the Lie algebra by its radical has null radical; he calls the Lie algebras with null radical *semisimple*, and proves that they are the product of simple algebras (this last notion had already been introduced by

$^{13}$ The term "Lie algebra" was introduced by H. Weyl in 1934: in his work of 1925, he had used the expression "infinitesimal group". Beforehand, one simply speaks of "infinitesimal transformations $X_1 f, \ldots, X_r f$" of the group, which Lie and Engel frequently shorten by saying "the group $X_1 f, \ldots, X_r f$".

$^{14}$ Almost at the beginning of his research, Lie had met soluble linear groups, and even in fact nilpotent ones ([202], vol. 5, Abh. IV, pp. 78-133).

Lie, who had proved the simplicity of the "classical" Lie algebras ([203], v. 3, p. 682)).

On the other hand, Killing introduces, in a Lie algebra, the characteristic equation $\det(\mathrm{ad}(x) - \omega.1) = 0$, already met by Lie in studying the Lie subalgebras of dimension 2 containing a given element of a Lie algebra. We refer to other historical Notes for the analysis of the methods whereby Killing, in studying in a penetrating manner the properties of the roots of the "generic" characteristic equation for a semisimple algebra, ends up with the most remarkable of his results, the *complete* determination of the simple (complex) Lie algebras.$^{15}$

Killing proves that the derived algebra of a soluble algebra is "of rank 0" (which means that $\mathrm{ad}\, x$ is nilpotent for every element $x$ of the algebra). Soon after, Engel proves that the algebras "of rank 0" are soluble (this statement is in substance what is called today Engel's theorem). In his thesis, E. Cartan introduces on the other hand what is now called the "Killing form", and establishes the two fundamental criteria that characterise by means of this form the soluble Lie algebras and the semisimple Lie algebras.

Killing had affirmed ([180], IV) that the derived algebra of a Lie algebra is the sum of a semisimple algebra and of its radical, which is nilpotent, but his proof was incomplete. A little later, E. Cartan announced without proof ([52 a], v. I_1, p. 104) that more generally every Lie algebra is the sum of its radical and of a semisimple subalgebra; the only result in this direction that is indisputably established at this time is a theorem of Engel affirming the existence, in every non-soluble Lie algebra, of a simple Lie subalgebra of dimension 3. The first published proof (for complex Lie algebras) of the statement of Cartan is due to E. E. Levi [200]; another proof (equally valid for the real case) was given by J. H. C. Whitehead in 1936 [334 a]. In 1942, A. Malcev completed this result by the uniqueness theorem on the "Levi sections" up to conjugation.

Already from his first work, Lie had set himself the problem of the isomorphism of every Lie algebra with a linear Lie algebra. He had thought that he had solved it affirmatively by considering the adjoint representation (and so deducing a proof of his "third theorem") ([202], vol. 5, Abh. III, pp. 42-75); he recognised rapidly that his proof was only correct for Lie algebras with null centre; after him, the question remained open for a long time, and was solved affirmatively by Ado in 1935 [2 a]. On the other hand, Lie had substantially set himself the problem of determining the linear representations of minimal dimension of the simple Lie algebras, and had solved it for the classical algebras; in his Thesis, Cartan had also resolved this problem

$^{15}$ Up to the following that he finds two exceptional algebras of dimension 52, for which he does not notice the isomorphism. (It is a case only of simple complex Lie algebras, as a more general problem was not considered at this time; the methods of Killing are valid in fact for every algebraically closed field of characteristic 0).

for the exceptional simple algebras;$^{16}$ the methods that he employs in this context will be generalised by him twenty years later in order to obtain all the irreducible representations of simple real or complex Lie algebras.

The property of complete reducibility of a linear representation seems to have been met for the first time (in a geometric form) by Study. In an unpublished manuscript, but quoted in ([203], v. 3, pp. 785-788) he proves this property for the linear representation of the Lie algebra of $\mathrm{SL}(2, \mathbf{C})$, and obtains partial results for $\mathrm{SL}(3, \mathbf{C})$ and $\mathrm{SL}(4, \mathbf{C})$. Lie and Engel conjecture on this occasion that the complete reducibility theorem is valid for $\mathrm{SL}(n, \mathbf{C})$ whatever $n$ may be. The complete reducibility of the linear representations of semisimple Lie algebras was established by H. Weyl in 1925$^{17}$ by an argument of a global nature (see later). The first algebraic proof was obtained in 1935 by Casimir and van der Waerden [55]; other algebraic proofs were given afterwards by R. Brauer [34 b] and J. H. C. Whitehead [334 b].

Finally, during his research on the exponential map (cf. infra). H. Poincaré ([251], v. III) considers the associative algebra of differential operators of all orders, generated by the operators of a Lie algebra; he shows, substantially that, if $(X_i)_{1 \leq i \leq n}$ is a basis of a Lie algebra, the associative algebra generated by the $X_i$ has as basis certain symmetric functions of the $X_i$ (sums of the non-commutative "monomials" obtained from a given monomial by all permutations of its factors). The essential part of his proof is algebraic in nature, and allows him to obtain the structure of the enveloping algebra. Analogous proofs have been given in 1937 by G. Birkhoff [22 b] and E. Witt [337 b].$^{18}$

The majority of the work quoted above is limited to real or complex Lie algebras, which are the only ones corresponding to Lie groups in the usual sense. The study of Lie algebras over a field other than $\mathbf{R}$ or $\mathbf{C}$ is tackled by Jacobson [172 a] who shows that the greater part of the classical results remain valid over a field of characteristic zero.

$^{16}$ The point of view of Cartan consisted in studying the non-trivial Lie algebra extensions of a simple Lie algebra and a (commutative) radical of minimal dimension.
$^{17}$ H. Weyl remarks on this occasion that the construction given by E. Cartan of the irreducible representation implicitly uses this property.
$^{18}$ The first use of differential operators of higher order generated by the $X_i$ is without doubt the use of the "Casimir operator" for the proof of the complete reducibility theorem. After 1950, the researches of Gelfand and his school, and of Harish-Chandra, on the linear representations of infinite dimension, have brought these operators to the front rank.

The first research concerning the exponential map is due to E. Study and F. Engel; Engel [104 b] remarks that the exponential is not surjective for $\mathrm{SL}(2, \mathbf{C})$ (for example $\begin{pmatrix} -1 & a \\ 0 & -1 \end{pmatrix}$) is not an exponential if $a \neq 0$, but that it is for $\mathrm{GL}(n, \mathbf{C})$, thus also for $\mathrm{PGL}(n, \mathbf{C})$ (this latter property had already been noted by Study for $n = 2$); thus $\mathrm{SL}(2, \mathbf{C})$ and $\mathrm{PGL}(2, \mathbf{C})$ give an example of two groups that are locally isomorphic, but which are nonetheless very different from a global point of view. Engel shows also that the exponential is surjective in the other classical groups, augmented by homotheties; this work is taken up again and continued by Maurer, Study and others, without bringing in substantial new results.

In 1899, H. Poincaré ([251], v. III, pp. 169-172 and 173-212), tackles the study of the exponential map from a different point of view. His memoirs seem to have been hurriedly written, for in several places he affirms that every element of a connected group is an exponential, whereas he gives examples to the contrary elsewhere. His results refer mainly to the adjoint group: he shows that a semisimple element of such a group $G$ can be the exponential of an infinity of elements of the Lie algebra $L(G)$, whereas a non-semisimple element may be not an exponential. If $\mathrm{ad}(X)$ does not have an eigenvalue which is a non-zero multiple of $2\pi i$, then exp is étale in $X$. He proves also that, if $U$ and $V$ describe loops in $L(G)$, and if $W$ is defined by continuity such that $e^U . e^V = e^W$, we do not return necessarily to the initial determination of $W$. He uses a formula for residues that reduces essentially to

$$
\Phi(\mathrm{ad}\, X) = \frac{1}{2\pi i} \int \frac{\Phi(\xi) d\xi}{\xi - \mathrm{ad}\, X}
$$

where $\mathrm{ad}(X)$ is a semisimple element whose non-zero eigenvalues have multiplicity 1, $\Phi$ is an entire series with a sufficiently large radius of convergence, the integral being taken over a loop enclosing the eigenvalues of $\mathrm{ad}\, X$; he studies also what happens when $X$ tends towards a transformation having multiple eigenvalues.

The search for expressions for $W$ as a function of $U$ and $V$ in the formula $e^U . e^V = e^W$ had already, a little before the work of Poincaré, been the subject of two memoirs of Campbell [46 a and b]. As is written a little later by Baker "...the theory of Lie suggests in an obvious way that the product $e^U e^V$ is of the form $e^W$ where $W$ is an alternating series in $U$ and $V$ ...". The subsequent work on this subject aimed to make this assertion precise and to give an explicit formula (or a method of construction) for $W$ ("Hausdorff formula"). After Campbell and Poincaré, Pascal, Baker [13] and Hausdorff [152 a] return to the question; each considers that the proofs of his predecessor are not convincing; the main difficulty resides in what is meant by "alternating": is it a case of elements of the particular Lie algebra under consideration, or of universal "symbolic" expressions? Neither Campbell, nor Poincaré, nor Baker express themselves clearly on this point. The memoir of Hausdorff, on the contrary, is perfectly precise; he works at first in the algebra of formal associative (non commutative) series in a finite number of indeterminates and considers $U, V, W$ as elements of this algebra. He proves the existence of $W$ by an argument on differential equations analogous to those of his predecessors. The same argument is used by him to prove the convergence of the series when the indeterminates in it are replaced by elements of a Lie algebra of finite dimension. As Baker had remarked, and Poincaré independently, this result can be used to give a proof of the third theorem of Lie; he clarifies the correspondence between groups and Lie algebras, for example as far as the group of commutators is concerned.

In 1947, Dynkin [98 a] takes up the question again, and obtains the explicit coefficients of the Hausdorff formula, by considering from the beginning a normed Lie algebra (of finite dimension or not, over $\mathbf{R}, \mathbf{C}$ or an ultrametric field).19

VI. LINEAR REPRESENTATIONS AND GLOBAL LIE GROUPS.

None of the work of which we have been speaking tackled frankly the problem of the definition and the study of global Lie groups. The first steps along this path go back to H. Weyl. He is inspired by two theories, which until then had developed independently: that of linear representations of semisimple complex Lie algebras, due to E. Cartan, and that of linear representations of finite groups, due to Frobenius and which had just been transposed to the orthogonal group by I. Schur using an idea of Hurwitz. This latter had shown [168] how invariants can be constructed for the orthogonal groups or the unitary groups by replacing the operation of the mean on a finite group by integration relative to an invariant measure. He had also remarked that in applying this method to the unitary group, invariants for the general linear group are obtained, a first example of the "unitarian trick". In 1924, I. Schur [279 e] used this procedure to show the complete reducibility of the representations of the orthogonal group $O(n)$ and of the unitary group $U(n)$, by the construction of a positive non-degenerate invariant hermitian form; he deduces from this, by the "unitarian trick", the complete reducibility of the holomorphic representations of $O(n, \mathbf{C})$ and of $SL(n, \mathbf{C})$, establishes orthogonality relations for the characters of $O(n)$ and of $U(n)$ and determines the characters of $O(n)$. H. Weyl also extends this method to complex semisimple Lie algebras [331 b]. Given such an algebra $g$, he shows that it possesses a "real compact form" (which amounts to saying that it comes from an algebra

19 In the ultrametric case, the classical method of majorants can not be extended without precautions, because of the asymptotic behaviour of the $p$-adic valuation of $1/n$ when $n$ tends to infinity.

$g_0$ over $\mathbf{R}$, whose adjoint group $G_0$ is compact, by extending the scalars from $\mathbf{R}$ to $\mathbf{C}$. Furthermore he shows that the fundamental group of $G_0$ is finite, thus that the universal cover$^{20}$ of $G_0$ is compact. He deduces from this, by an appropriate adaptation of the procedure of Schur, the complete reducibility of the representations of $g$, and gives also, by global means, the determination of the characters of the representations of $g$. In a letter to I. Schur [331 a], H. Weyl summarises the results of Cartan, that Schur did not know (cf. [279 e], p. 299, note at the foot of the page) and compares the two points of view: the method of Cartan supplies all the holomorphic representations of the simply connected group of the Lie algebra $g$; in the case of the orthogonal group, the representations of a cover in two sheets (later called the spinor group), which had escaped Schur’s notice, are also obtained; from another side, Schur’s method has the advantage of proving complete reducibility and of giving the characters explicitly.

After the work of H. Weyl, E. Cartan adopts an openly global point of view in his research on symmetric spaces and Lie groups. It is this point of view that is at the basis of his exposé of 1930 ([52 a], v. I_2, pp. 1165-1225) of the theory of “finite and continuous” groups. There is found in particular the first proof of the global variant of the third fundamental theorem (existence of a Lie group with given Lie algebra); Cartan shows also that every closed subgroup of a real Lie group is a Lie group, which generalises a result of J. von Neumann on the closed subgroups of the linear group [324 b]. In this Memoir, von Neumann showed also that every continuous representation of a complex semisimple group is real analytic.

After this work, the theory of Lie groups in the “classical” sense (that is to say of finite dimension over $\mathbf{R}$ or $\mathbf{C}$) is more or less fixed in its main lines. The first detailed exposé of it is given by Pontrjagin in his book on topological groups [253]; he keeps there to a point of view still fairly close to that of Lie, but in distinguishing carefully the local from the global. It is followed by the book of Chevalley [62 d] which contains also the first systematic discussion of the theory of analytic varieties and of the exterior differential calculus; the “infinitesimal transformations” of Lie appear there as fields of vectors and the Lie algebra of a Lie group $G$ is identified with the space of fields of vectors invariant on the left under $G$. He leaves to one side the “groupuscule” aspect and the “groups of transformations” aspect.

$^{20}$ H. Weyl does not define this notion, with which he was familiar since the drawing up of his lecture on Riemann surfaces (1913), explicitly. It is O. Schreier [276 a and b] who, in 1926-1927, gives, for the first time, the definition of a topological group and that of a “continuous” group (i.e. locally homeomorphic to a Euclidean space), as well as the construction of the universal cover of such a group.

VII. EXTENSIONS OF THE NOTION OF A LIE GROUP.

In our day, the vitality of Lie theory is manifested by the diversity of its applications (in topology, differential geometry, arithmetic, etc.) as well as by the creation of parallel theories where the structure of the underlying differential variety is replaced by a neighbouring structure ($p$-adic, algebraic variety, schema, formal schema, ...). We do not need to provide here the history of all these developments, and we will limit ourselves to two of them: Banach Lie groups and $p$-adic Lie groups.

a) *Banach Lie groups*.

It is a case of Lie groups "of infinite dimension". From the local point of view, a neighbourhood of 0 in an Euclidean space is replaced by a neighbourhood of 0 in a Banach space. It is what is done by G. Birkhoff in 1936 [22 a], ending up thus with the notion of a *complete normed Lie algebra* and with its correspondence with a "groupuscule" defined on an open set of a Banach space. Around 1950, Dynkin completes these results by an extension to this case of the Hausdorff formula (cf. *supra*).

The definitions and results of Birkhoff and Dynkin are local. Until recent days, it does not seem that an attempt has been made to make explicit the corresponding global theory, no doubt because of the lack of applications.

b) *$p$*-adic *Lie groups*.

Such groups are met for the first time in 1907 in the work of Hensel [157 e] on the $p$-adic analytic functions (defined by expansions in entire series). He studies notably the exponential and the logarithm; in spite of the *a priori* surprising behaviour of the series that define them (for example the exponential series does not converge everywhere), their functional properties remain valid, which supplies a *local isomorphism* between the additive group and the multiplicative group of $\mathbf{Q}_p$ (or, more generally, of every complete ultrametric field of characteristic zero).

It is equally about commutative groups (but not linear this time) that the work of A. Weil [330 a] and E. Lutz [210] on the elliptic $p$-adic curves (1936) is concerned. Other than the arithmetic applications, there can be found the construction of a local isomorphism of the group with the additive group, based on the integration of an invariant differential form. This method can be equally applied to abelian varieties, as is remarked shortly afterwards by C. Chabauty who uses it without any more explanation in order to prove a particular case of the "Mordell conjecture" [61].

From this moment, it was clear that the local theory of Lie groups can be applied almost without change to the $p$-adic case. The fundamental theorems of the "dictionary" Lie groups-Lie algebras are established in 1942 in the thesis of R. Hooke [166], a pupil of Chevalley; this work contains also the $p$-adic analogue of the theorem of E. Cartan on the closed subgroups of real Lie groups.

More recently, M. Lazard [195 b] develops a more precise form of the "dictionary" for compact analytic groups over $\mathbf{Q}_p$. He shows that the existence of an analytic $p$-adic structure on a compact group $G$ is tightly linked to that of certain filtrations on $G$, and gives various applications of it (for example to the cohomology of $G$). One of Lazard's tools is an improvement of Dynkin's results on the convergence of the $p$-adic Hausdorff series [195 a].

VIII. FREE LIE ALGEBRAS.

It remains for us to speak of a series of works on *Lie algebras* where the link with the theory of *Lie groups* is very tenuous; these researches have on the other hand important applications in the theory of "abstract" groups and more especially nilpotent groups.

The origin of this is the work of P. Hall [144], which appeared in 1932. There is however there no question of Lie algebras: P. Hall has in view the study of a certain class of $p$-groups, those that he calls "regular". But that leads him to examine in detail iterated commutators and the lower central series of a group; he establishes on this occasion a variant of the Jacobi identity, as well as the "Hall formula"

$$
(xy)^n = x^n y^n (x, y)^{n(n-1)/2} \ldots
$$

Soon after (in 1935-1937) the fundamental works of W. Magnus [215 a and b] and E. Witt [337 b] appear. In [215 a] Magnus uses the same algebra of formal series $\hat{A}$ as Hausdorff (since called the "Magnus algebra"); he embeds the free group $F$ in it and uses the natural filtration of $\hat{A}$ in order to obtain a decreasing sequence $(F_n)$ of subgroups of $F$; it is one of the first examples of *filtration*. He conjectures that the $F_n$ coincide with the terms of the lower central series of $F$. This conjecture is proved in his second memoir [215 b]; it is also there that he explicitly makes the link between his ideas and those of P. Hall, and that he defines the free Lie algebra $L$ (as a sub algebra of $A$) of which he shows in substance that it is identified with the graded $F$. In [337 b], Witt completes this result on several points. He shows notably that the enveloping algebra of $L$ is a free associative algebra and deduces from that immediately the rank of the homogeneous components of $L$ ("Witt formulae").

As for the determination of the basis of $L$ known by the name of "Hall basis", it seems that it only appears for the first time in 1950, in a note of M. Hall [143], although it is implicit in the works of P. Hall and W. Magnus quoted above.
