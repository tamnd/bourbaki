---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: GROUPES DE LIE
section: 0
section_title: Historical Note
kind: historical
lang: en
source: lie-ii-iii-fr
pdf_pages: 0284-0318
extraction: ocr
statements: 0
exercises: 0
content_sha256: d264a5fb7e52b2fc4fd8837bcfa0fb9b251e9a9910d4a441c8ec27ebb5092814
translated_from: content/fr/lie/III/historical_note.md
source_lang: fr
translation_method: machine
source_content_sha256: ecc1bb94d90a11516c78ea848cb14d893324cffe01469163c2bbc23a54c61eaa
translation_model: nemotron-3-ultra-free, gpt-5-6-mini, laguna-s-2.1-free, mimo-v2.5-free, hy3-free
translation_run: translate-en-mt-a8a58a65
glossary_version: 34
glossary_terms_sha256: 435582aab0cf5f75cbe062b2eecc00fdace59ef98560ebeb88e4aee3bca9a5fd
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

# HISTORICAL NOTE
Chapters I to III

I. Genesis

The theory, called for nearly a century 'theory of Lie groups', was built essentially by a single mathematician: Sophus Lie.
Before addressing its history, we shall briefly summarize various earlier researches that prepared its development.

a) Transform groups (Klein–Lie, 1869–1872)

Around 1860, the theory of permutation groups of a finite set develops and begins to be used (Serret, Kronecker, Mathieu, Jordan). On the other hand, the theory of invariants, then in full expansion, familiarizes mathematicians with certain infinite sets of geometric transforms stable under composition (notably linear or projective transforms). But, before Jordan's 1868 work (VII) on 'groups of motions' (closed subgroups of the group of displacements of 3-dimensional Euclidean space), it does not seem that a conscious link was established between these two currents of ideas.

In 1869, the young Félix Klein (1849–1925), a student of Plücker, becomes friends in Berlin with the Norwegian Sophus Lie (1842–1899), a few years older, whom their common interest in Plücker's 'geometry of lines' and notably the theory of line complexes brings together. It is around this period that Lie conceives one of his most original ideas, the introduction of the notion of invariant in Analysis and in differential geometry; one of its sources is his observation that the classical methods of integration 'by quadratures' of differential equations all rest on the fact that the equation is invariant under a 'continuous' family of transforms. It is from 1869 that dates the first work (written by Klein) in which Lie uses this idea; he studies the 'Reye complex' (set of lines cutting the faces of a tetrahedron in 4 points having a given cross-ratio) and the curves and surfaces admitting as tangents lines of this complex (III a)): his method rests on the invariance of the Reye complex under the commutative 3-parameter group (maximal torus of $\mathbf{PGL}(4, \mathbf{C})$) leaving the vertices of the tetrahedron invariant.

This same idea dominates the work written jointly by Klein and Lie while they are in Paris in the spring of 1870 (I a)); they essentially determine the connected commutative subgroups of the projective group of the plane $\mathbf{PGL}(3, \mathbf{C})$, and study the geometric properties of their orbits (under the name of curves or surfaces V); this gives them, by a uniform process, properties of various curves, algebraic or transcendental, such as $y = cx^m$ or logarithmic spirals. Their testimonies agree in emphasizing the profound impression that the theories of Galois and Jordan produced on them (Jordan's commentary on Galois had appeared in Math. Annalen in 1869; moreover, Lie had heard of Galois theory as early as 1863). Klein, who in 1871 begins to take an interest in non-Euclidean geometries, sees in it the beginning of his search for a principle of classification of all known geometries, a search that was to lead him in 1872 to the 'Erlangen program'. For his part, Lie, in a letter of 1873 to A. Mayer (III, vol. V, p. 584), dates from his stay in Paris the origin of his ideas on transform groups, and in a work of 1871 (III b)), he already uses the term 'transform group' and explicitly poses the problem of the determination of all subgroups ('continuous or discrete') of $\mathbf{GL}(n, \mathbf{C})$.

It must be said that both Klein and Lie had to experience some difficulty in inserting themselves into this new mathematical universe, and Klein speaks of Jordan's 'Treatise', newly published, as a 'book sealed with seven seals' (II, p. 51); he writes elsewhere concerning (I a) and b)): 'It is to Lie that belongs everything relating to the heuristic idea of a continuous group of operators, in particular everything touching on the integration of differential equations or partial differential equations. All the notions that he later developed in his theory of continuous groups were already present in germ in him, but however so little elaborated, that I had to convince him of many details, for example at the beginning the very existence of the V curves, in the course of long conversations' (II, p. 415).

b) Infinitesimal transforms

The conception of an 'infinitely small' transform goes back at least to the beginnings of the Infinitesimal Calculus; it is known that Descartes discovers the instantaneous center of rotation by admitting that 'in the infinitely small' every plane motion can be assimilated to a rotation; the development of Analytical Mechanics, in the 18th century, is entirely founded on similar ideas. In 1851, Sylvester, seeking to form invariants of the linear group $\mathbf{GL}(3, \mathbf{C})$ or of certain of its subgroups, gives to the parameters $z_j$ appearing in these matrices 'infinitely small' increments of the form $\alpha_j dt$, and expresses that a function $f((z_j))$ is invariant by writing the equation $f((z_j + \alpha_j dt)) = f((z_j))$; this gives for $f$ the linear partial differential equation $Xf = 0$, where

$$
Xf = \sum_j \alpha_j \frac{\partial f}{\partial z_j},
$$

$X$ being thus a differential operator, “derivative in the direction of the directing parameters $\alpha_j$” (V, Vol. 3, p. 326 and 327); Sylvester seems to feel that there is here a general principle of rather wide scope, but does not appear to have returned to the question. A little later, Cayley (VI, Vol. II, p. 164–178) proceeds in the same way for the invariants of $\mathbf{SL}(2, \mathbf{C})$ in certain representations of this group and shows that they are the solutions of two first-order partial differential equations $Xf = 0, Yf = 0$, where $X$ and $Y$ are obtained as above from the “infinitesimal” transformations

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

In modern terms, this is explained by the fact that $X$ and $Y$ generate the Lie algebra $\mathfrak{sl}(2, \mathbf{C})$; moreover Cayley calculates explicitly the bracket $XY - YX$ and shows that it too comes from an “infinitesimal” transformation.

In his 1868 memoir on groups of movements (VII), Jordan uses from beginning to end the concept of “infinitesimal transformation”, but exclusively from a geometrical point of view. It is doubtless with him that the idea of a one-parameter group “generated” by an infinitesimal transformation appears: for Jordan, it is the set of transformations obtained by “suitably repeating” the infinitesimal transformation (*loc. cit.*, p. 243). Klein and Lie, in their 1871 memoir, use the same expression “repeated infinitesimal transformation” (I b)), but the context shows that they mean by this an integration of a differential system. If the one-parameter group they consider is formed of the transformations $x' = f(x, y, t),\ y' = g(x, y, t)$, the corresponding “infinitesimal transformation” is given by

$$
dx = p(x, y)\ dt,\quad dy = q(x, y)\ dt
$$

where $p(x, y) = \frac{\partial f}{\partial t}(x, y, t_0),\ q(x, y) = \frac{\partial g}{\partial t}(x, y, t_0)$, and $t_0$ corresponds to the identical transformation of the group. Since Klein and Lie know explicitly the functions $f$ and $g$, they have no difficulty in verifying that the functions

$$
t \mapsto f(x, y, t) \quad \text{ and } \quad t \mapsto g(x, y, t)
$$

give in parametric form the integral curve of the differential equation

$$
q(\xi, \eta)\ d\xi = p(\xi, \eta)\ d\eta
$$

passing through the point $(x, y)$, but they give no general reason for this; moreover they no longer use this fact in the sequel of their memoir.

c) Contact transformations

In the following two years, Lie appears to abandon the theory of transformation groups (although he remains in very close contact with Klein, who publishes his “Programme” in 1872) in order to study contact transformations, the integration of first-order partial differential equations and the relations between these two theories. We shall not make the historical account of these questions here, and shall confine ourselves to mentioning a few points which appear to have played an important role in the genesis of the theory of transformation groups.

The notion of contact transformation generalizes both point transformations and transformations by reciprocal polars. Roughly speaking, a contact transformation¹ in $\mathbf{C}^n$ is an isomorphism of an open set $\Omega$ of the variety $T'(\mathbf{C}^n)$ of cotangent vectors to $\mathbf{C}^n$ onto another open set $\Omega'$ of $T'(\mathbf{C}^n)$ transforming the canonical 1-form of $\Omega$ into that of $\Omega'$. In other words, if $(x_1, \ldots, x_n, p_1, \ldots, p_n)$ denote the canonical coordinates of $T'(\mathbf{C}^n)$, a contact transformation is an isomorphism $(x_i, p_i) \mapsto (X_i, P_i)$ satisfying the relation $\sum_{i=1}^n P_i\, dX_i = \sum_{i=1}^n p_i\, dx_i$. Such transformations occur in the study of the integration of partial differential equations of the form

$$
F\left(x_1, x_2, \ldots, x_n, \frac{\partial z}{\partial x_1}, \ldots, \frac{\partial z}{\partial x_n}\right) = 0.
$$

Lie becomes familiar in the course of his research on these questions with the manipulation of Poisson brackets

$$
(f, g) = \sum_{i=1}^n \left( \frac{\partial f}{\partial x_i} \frac{\partial g}{\partial p_i} - \frac{\partial g}{\partial x_i} \frac{\partial f}{\partial p_i} \right)
$$

and of brackets² $[X, Y] = XY - YX$ of differential operators of type (1); he interprets the Poisson bracket (3) as the effect on $f$ of a transformation of type (1) associated with $g$, and observes on this occasion that the Jacobi identity for the Poisson brackets signifies that the bracket of the differential operators corresponding to $g$ and $h$ is associated with the bracket $(g, h)$. The search for functions $g$ such that $(F, g) = 0$, which occurs in Jacobi’s method for integrating

¹ Here it is a question of “homogeneous” contact transformations. Previously, the consideration of equations of type (2), but where $z$ occurs in $F$, had led Lie to consider contact transformations with $2n + 1$ variables $z, x_1, \ldots, x_n, p_1, \ldots, p_n$, where it is a question of finding $2n + 2$ functions $Z, P_i, X_i$ $(1 \leq i \leq n)$ and $\rho$ (the latter $\neq 0$ at every point) such that $dZ - \sum_i P_i\, dX_i = \rho(dz - \sum_i p_i\, dx_i)$.

This apparently more general case reduces moreover easily to the “homogeneous” case (IV, Vol. 2, p. 135–146).

² These had already appeared in Jacobi-Clebsch's theory of "complete systems" of first-order partial differential equations $X_j f = 0$ $(1 \leq j \leq r)$, an equivalent notion to that of a "completely integrable system" of Frobenius: the fundamental theorem (equivalent to the "Frobenius theorem") characterizing these systems is that the brackets $[X_i, X_j]$ must be linear combinations (with variable coefficients) of the $X_k$.

The partial differential equation (2) becomes, for Lie, that of an infinitesimal contact transformation leaving the given equation invariant. Finally, Lie is led to study sets of functions $(u_j)_{1 \leq j \leq m}$ of the $x_i$ and $p_i$ such that the brackets $(u_j, u_k)$ are functions of the $u_h$, and he calls "groups" these sets (already considered in substance by Jacobi).

II. Continuous groups and infinitesimal transformations

Suddenly, in the autumn of 1873, Lie resumed the study of transformation groups and obtained decisive results. As far as one can follow the course of his thought in some letters to A. Mayer from 1873–1874 (III, vol. 5, p. 584–608), he starts from a "continuous group" of transformations on $n$ variables

$$
x'_i = f_i(x_1, \ldots, x_n, a_1, \ldots, a_r) \quad (1 \leq i \leq n)
$$

depending effectively¹ on $r$ parameters $a_1, \ldots, a_r$; he observes that, if the transformation (4) is the identity for the values $a_1^0, \ldots, a_r^0$ of the parameters,² then the Taylor expansions of the $x_i$, limited to the first order:

$$
f_i(x_1, \ldots, x_n, a_1^0 + z_1, \ldots, a_r^0 + z_r) = x_i + \sum_{k=1}^r z_k X_{ki}(x_1, \ldots, x_n) + \cdots \quad (1 \leq i \leq n)
$$

give a "generic" infinitesimal transformation depending linearly on the $r$ parameters $z_j$

$$
dx_i = \left( \sum_{k=1}^r z_k X_{ki}(x_1, \ldots, x_n) \right) dt \quad (1 \leq i \leq n).
$$

Proceeding as in his memoir with Klein, Lie integrates the differential system

$$
\frac{d\xi_1}{\sum_k z_k X_{k1}(\xi_1, \ldots, \xi_n)} = \cdots = \frac{d\xi_n}{\sum_k z_k X_{kn}(\xi_1, \ldots, \xi_n)} = dt,
$$

which gives him, for every point $(z_1, \ldots, z_r)$, a one-parameter group

$$
t \mapsto x'_i = g_i(x_1, \ldots, x_n, z_1, \ldots, z_r, t) \quad (1 \leq i \leq n)
$$

¹ By this Lie understands that the $f_i$ cannot be expressed using fewer than $r$ functions of the $a_j$, or that the Jacobian matrix $(\partial f_i / \partial a_j)$ has rank $r$ "in general".
² In his early notes, Lie believed he could prove a priori the existence of the identity and inverse in any set of transformations (4) closed under composition; he later recognized that his proof was incorrect, and Engel provided him with a counterexample reproduced in (IV, vol. 1, § 44). However, Lie showed how to reduce "continuous" systems (4) closed under composition to groupoids of transformations: such a system is of the form $G \circ h$, where $G$ is a groupoid of transformations and $h$ a transformation of the system (IV, vol. 1, th. 26, p. 163 and vol. 3, th. 46, p. 572) such that $g_i(x_1, \ldots, x_n, z_1, \ldots, z_r, 0) = x_i$ for all $i$. He showed in a clever way, by using the fact that the transformations (4) form a set closed under composition, that the one-parameter group (8) is a subgroup of the given group (III d)). The new idea, key to the entire theory, is to carry the Taylor expansions of the functions (4) to the second order. The course of his reasoning is rather confused and heuristic ((III d)) and (III, vol. 5, p. 600–601)); it can be presented as follows. For sufficiently small $z_j$, one can set $t = 1$ in (8), and thus obtain new parameters $z_1, \ldots, z_r$ for the transformations of the group (this is in fact the first appearance of "canonical parameters"). By definition, seen from (7)

$$
\frac{\partial g_i}{\partial t} = \sum_k z_k X_{ki}(x'_1, \ldots, x'_n),
$$

from which

$$
\frac{\partial^2 g_i}{\partial t^2} = \sum_{k,j} z_k \frac{\partial X_{kt}}{\partial x_j} (x'_1, \ldots, x'_n) \frac{\partial x'_j}{\partial t}
$$
$$
= \sum_{k,j} z_k \frac{\partial X_{kt}}{\partial x_j} (x'_1, \ldots, x'_n) \left( \sum_h z_h X_{hj}(x'_1, \ldots, x'_n) \right)
$$

which gives

$$
x'_i = x_i + \left( \sum_k z_k X_{ki}(x_1, \ldots, x_n) \right)t
$$
$$
+ \frac{1}{2} \left( \sum_{k,h,j} z_k z_h \frac{\partial X_{kt}}{\partial x_j} (x_1, \ldots, x_n) X_{hj}(x_1, \ldots, x_n) \right)t^2 + \cdots,
$$

from which, for $t = 1$, the Taylor expansions with respect to the parameters $z_j$

(9) $$ x'_i = x_i + \left( \sum_k z_k X_{ki} \right) + \frac{1}{2} \left( \sum_{k,h,j} z_k z_h X_{hj} \frac{\partial X_{ki}}{\partial x_j} \right) + \cdots \quad (1 \leq i \leq n). $$

Let us write in brief these relations $x' = G(x, z)$ between vectors

$$
x = (x_1, \ldots, x_n), \qquad x' = (x'_1, \ldots, x'_n), \qquad z = (z_1, \ldots, z_r);
$$

the fundamental property of stability of this set of transformations under composition is written as

(10) $$ G(G(x, u), v) = G(x, H(u, v)) $$

where $H = (H_1, \ldots, H_r)$ is independent of $x$; it is immediate that $H(u, 0) = u$, $H(0, v) = v$, from which the expansions follow

(11) $$ H_i(u, v) = u_i + v_i + \frac{1}{2} \sum_{h,k} c_{ikh} u_h v_k + \cdots, $$

the unwritten terms being nonlinear in $u$ or in $v$. Transforming (10) using (9) and (11), and then comparing the terms in $u_h v_k$ on both sides, Lie obtains the relations

$$
(12) \quad \sum_{j=1}^n \left( X_{hj} \frac{\partial X_{ki}}{\partial x_j} - X_{kj} \frac{\partial X_{hi}}{\partial x_j} \right) = \sum_{l=1}^r c_{lhk} X_{li} \qquad (1 \leq h, k \leq r, 1 \leq i \leq n).
$$

His practice of the theory of partial differential equations leads him to write these conditions in a simpler form: following the model of (1), he associates to each of the $r$ infinitesimal transforms obtained by setting $z_k = 1$, $z_h = 0$ for $h \neq k$ in (6), the differential operator

$$
(13) \qquad A_k(f) = \sum_{i=1}^n X_{ki} \frac{\partial f}{\partial x_i},
$$

and rewrites the conditions (12) in the form

$$
(14) \qquad [A_h, A_k] = \sum_l c_{lhk} A_l,
$$

the cornerstone of his theory. Until then, he had used the terms 'infinitesimal transform' and 'infinitesimal transform' (*e.g.* (III c)) interchangeably; the simplicity of the relations (14) leads him to call the operator (13) the 'symbol' of the infinitesimal transform $dx_i = X_{ki} dt$ ($1 \leq i \leq n$) (III e)) and very soon it is the operator (13) itself that he will call '*infinitesimal transform*' ((III e)) and (III, vol. 5, p. 589)).

He then becomes aware of the close links uniting the theory of 'continuous groups' with his earlier research on contact transforms and partial differential equations. This bringing together fills him with enthusiasm: '*My earlier works were, so to speak, ready in advance to found the new theory of transform groups*' he writes to Mayer in 1874 (III, vol. 5, p. 586).

In the following years, Lie continues the study of transform groups. Besides the general theorems summarized below (§ III), he obtains a certain number of more particular results: determination of the transform groups of the line and the plane, of the subgroups of small codimension of the projective groups, of groups with at most 6 parameters, etc. He does not for all that abandon differential equations. In fact, it even seems that, for him, the theory of transform groups was to be an instrument for integrating differential equations, where the transform group would play a role analogous to that of the galois group of an algebraic equation.\footnote{These researches have had only little influence on the general theory of differential equations, the automorphism group of such an equation being most often trivial. On the other hand, for certain types of equations (for example linear), interesting results have been obtained subsequently by Picard, Vessiot, then, more recently, Ritt and Kolchin.} Note that these researches also lead him to introduce certain sets of transforms with an infinity of parameters, which he calls 'infinite and continuous groups'¹; he reserves the name 'finite and continuous groups' for transform groups with a finite number of parameters of the type (4) above.

III. The 'dictionary' of Lie groups-Lie algebras

The theory of 'finite and continuous groups', developed by Lie in numerous memoirs from 1874 onward, is systematically presented in the imposing treatise 'Theorie der Transformationsgruppen' ((IV), 1888–1893), written in collaboration with F. Engel²; it forms the subject of the first volume and the last five chapters of the third, the second being devoted to contact transforms.

As the title indicates, this work deals only with transform groups, in the sense of equations (4), where the space of 'variables' $x_i$ and the space of 'parameters' $a_j$ play initially equally important roles. Moreover, the concept of 'abstract' group is not clearly distinguished at this time; when in 1883 (III g)) Lie observes that, with the notations of (10), the equation $w = \mathrm{H}(u, v)$ giving the parameters of the composite of two transforms of the group defines a new group, he considers it as a transform group on the parameter space, thus obtaining what he calls the 'parameter group' (he even obtains two of them, which are none other than the group of left translations and the group of right translations³).

The variables $x_i$ and the parameters $a_j$ in equations (4) are in principle assumed complex (except in Chapters XIX–XXIV of volume 3), and the functions $f_i$ analytic; Lie and Engel are of course aware of the fact that these functions are not in general defined for all complex values of the $x_i$ and the $a_j$ and that, consequently, the composition of such transforms raises serious difficulties (IV, vol. 1, p. 15–17, p. 33–40 and passim); and although, subsequently, they almost always express themselves as if the composition of the transforms they study were possible without restriction, this is no doubt only for the convenience of the statements, and they explicitly reinstate the 'local' point of view whenever necessary (cf. loc. cit., p. 168 or 189 for example or ibid., vol. 3, p. 2, footnote); in other words, the mathematical object

¹ They are called today "Lie pseudo-groups"; care must be taken not to confuse them with the "Banach" Lie groups defined in this volume.
² From 1886 to 1898, Lie held at Leipzig the chair left vacant by Klein and had Engel as assistant; this circumstance fostered the emergence of an active mathematical school as well as the diffusion of Lie's ideas, which were quite little known until then (due, in particular, to the fact that his first memoirs were most often written in Norwegian, and published in the Comptes Rendus de l'Académie de Christiania, little disseminated elsewhere). It is thus that at a time when it was hardly customary for young French mathematicians to go study in Germany, E. Vessiot and A. Tresse spent a year of study at Leipzig, with Sophus Lie.
³ The analogous notion for permutation groups had been introduced and studied by Jordan in his "Treatise".

which they study is close to what we call in this treatise a piece of composition law. They do not hesitate, on occasion, to consider global groups, for example the 4 series of classical groups (IV, Vol. 3, p. 682), but do not appear to have asked the question of what a "global group" may be in general; it suffices for them to be able to obtain, for the "parameters" of the classical groups (the "variables" of these groups introduce no difficulty, since they are linear transforms of $\mathbf{C}^n$), systems of "local" parameters in the neighbourhood of the identical transform, without their worrying about the domain of validity of the formulas they write.

They do, however, pose a problem that clearly goes beyond local theory¹: the study of "mixed" groups, that is, groups having a finite number of connected components, such as the orthogonal group (IV, Vol. 1, p. 7). They present this study as that of a set of transforms stable under composition and passing to the inverse which is the union of sets $H_j$ each of which is described by systems of functions $(f_i^{(j)})$ as in (4); the number of (essential) parameters of each $H_j$ is even supposed a priori to depend on $j$, but they show that in fact this number is the same for all $H_j$. Their main result is then the existence of a finite continuous group $G$ such that $H_j = G \circ h_j$ for an $h_j \in H_j$ and for every $j$; they also establish that $G$ is normal in the mixed group and remark that the determination of the invariants of the latter reduces to that of the invariants of $G$ and of a discontinuous group (IV, Vol. 1, Chap. 18).

The general theory developed in (IV) leads (without this being said in a very systematic way by the authors) to forging a "dictionary" carrying over the properties of "finite continuous groups" to those of the set of their infinitesimal transforms. It is based on the "three theorems of Lie", each of which consists of an assertion and its converse.

The first theorem (IV, Vol. 1, p. 33 and 72 and Vol. 3, p. 563) asserts firstly that if in (4) the parameters are effective, the functions $f_i$ satisfy a system of partial differential equations of the form

$$
\frac{\partial f_i}{\partial a_j} = \sum_{k=1}^r \xi_{kji}(f(x, a)) \psi_{kj}(a) \qquad (1 \leq i \leq n)
$$

where the matrix $(\xi_{kji})$ is of maximum rank and $\det(\psi_{kj}) \neq 0$; conversely, if the functions $f_i$ have this property, the formulas (4) define a transformation groupoid.

The second theorem (IV, Vol. 1, p. 149 and 158, and Vol. 3, p. 590) gives relations

¹ Let us recall (Historical Note of Alg., Chap. VIII, p. 170) that following a Note of H. Poincaré (XIV, Vol. V, p. 77–79) various authors have studied the group of invertible elements of a finite-dimensional associative algebra. It is interesting to note in this connection that E. Study, in his works on this subject, introduces a symbolism which amounts in substance to envisaging the abstract group defined by the parameter group.

between the $\xi_{kli}$ on the one hand, the $\psi_{ij}$ on the other: the conditions on the $\xi_{kli}$ are written in the form

$$
(16) \quad \sum_{k=1}^{n} \left( \xi_{ik} \frac{\partial \xi_{jl}}{\partial x_k} - \xi_{jk} \frac{\partial \xi_{il}}{\partial x_k} \right) = \sum_{k=1}^{r} c_{ij}^{kc} \xi_{kl} \qquad (1 \leq i, j \leq r, 1 \leq l \leq n)
$$

where the $c_{ij}^{k}$ are constants ($1 \leq i, j, k \leq r$) antisymmetric in $i, j$. The conditions on the $\psi_{ij}$, in the form given by Maurer (X), are:

$$
(17) \quad \frac{\partial \psi_{kl}}{\partial a_m} - \frac{\partial \psi_{km}}{\partial a_l} = \frac{1}{2} \sum_{1 \leq i, j \leq r} c_{ij}^{k} (\psi_{il} \psi_{jm} - \psi_{jl} \psi_{im}) \qquad (1 \leq k, l, m \leq r).
$$

By introducing the matrix $(\alpha_{ij})$ contragradient to $(\psi_{ij})$ and the infinitesimal transforms

$$
(18) \quad X_k = \sum_{i=1}^{n} \xi_{kli} \frac{\partial}{\partial x_i}, \qquad A_k = \sum_{j=1}^{r} \alpha_{kj} \frac{\partial}{\partial a_j} \qquad (1 \leq k \leq r),
$$

one can write (16) and (17) respectively as:

$$
(19) \quad [X_i, X_j] = \sum_{k=1}^{r} c_{ij}^{k} X_k \qquad (1 \leq i, j \leq r).
$$
$$
(20) \quad [A_i, A_j] = \sum_{k=1}^{r} c_{ij}^{k} A_k
$$

Conversely, if one takes $r$ infinitesimal transforms $X_k$ ($1 \leq k \leq r$) linearly independent and satisfying the conditions (19), the one-parameter subgroups generated by these transforms generate a transformation group with $r$ essential parameters.

Finally, the third theorem (IV, t. 1, p. 170 and 297 and t. 3, p. 597) reduces the determination of the systems of infinitesimal transformations $(X_k)_{1 \leq k \leq r}$ satisfying (19) to a purely algebraic problem: one must have

$$
(21) \quad c_{ij}^{k} + c_{ji}^{k} = 0
$$
$$
(22) \quad \sum_{l=1}^{r} (c_{il}^{m} c_{jk}^{l} + c_{kl}^{m} c_{ij}^{l} + c_{jl}^{m} c_{ki}^{l}) = 0 \qquad (1 \leq i, j, k, m \leq r).
$$

Conversely,¹ if (21) and (22) are satisfied, there exists a system of infinitesimal transformations satisfying the relations (19), hence a group of transformations with $r$ parameters (in other words, the linear combinations with constant coefficients of the $X_k$ form a Lie algebra, and conversely every finite-dimensional Lie algebra can be obtained in this way).

These results are completed by the study of questions of isomorphism. Two groups of transformations are said to be *similar* if one passes from one to the other by an invertible transformation of coordinates on the variables and an invertible transformation of coordinates on the parameters: from the beginning of his research, Lie had naturally encountered this notion in connection with the definition of "canonical parameters". He shows that two groups are similar if, by a transformation on the "variables", one can bring the infinitesimal transformations of one onto those of the other (IV, t. 1, p. 329). A necessary condition for this to be the case is that the Lie algebras of the two groups be isomorphic, what Lie expresses by saying that the groups are "zusammengesetzt"; but this condition is not sufficient, and an entire chapter (IV, t. 1, chap. 19) is devoted to obtaining additional conditions ensuring that the groups are "similar". The theory of permutation groups, for its part, furnished the notion of "holoedric isomorphism" of two such groups (isomorphism of the underlying "abstract" groups); Lie transposes this notion to transformation groups, and shows that two such groups are "holoedrically isomorphic" if and only if their Lie algebras are isomorphic (IV, t. 1, p. 418). In particular, every transformation group is holoedrically isomorphic to each of its parameter groups, and this shows that, when one wishes to study the structure of the group, the "variables" on which it acts are of little importance and that, in fact, everything reduces to the Lie algebra.¹

By analogy with the theory of permutation groups, Lie introduces the notions of subgroups, normal subgroups, "meriedric isomorphisms" (surjective homomorphisms), and shows that they correspond to those of subalgebras, ideals, and surjective homomorphisms of Lie algebras; he had moreover encountered very early a particularly important example of "meriedric isomorphism", the adjoint representation, and recognized its links with the center of the group (III e)). For these results, as for the fundamental theorems, the essential tool is the Jacobi–Clebsch theorem giving the complete integrability of a differential system (one of the forms of the so-called "Frobenius" theorem); he moreover gives a new proof of it using one-parameter groups (IV, t. 1, chap. 6).

The notions of transitivity and primitivity, so important for permutation groups, also presented themselves naturally for "finite and continuous" transformation groups, and the Lie–Engel treatise makes a detailed study of them (IV, t. 1, chap. 13 and passim); the relations with the stabiliser subgroups of a point and the notion of homogeneous space are glimpsed (insofar as they could be without adopting a global point of view) (IV, t. 1, p. 425).

Finally, the "dictionary" is completed, in (IV), by the introduction of the notions of derived group and solvable group (called "integrable group" by Lie; this terminology, suggested by the theory of differential equations, remained in use until the work of H. Weyl) (IV, t. 1, p. 261 and t. 3, p. 678–679); the relation between commutators and brackets had moreover been perceived by Lie as early as 1883 (III, t. 5, p. 358).

Other proofs of the fundamental theorems

In (VIII) F. Schur shows that in canonical coordinates the $\psi_{ik}$ of (15) satisfy the differential equations

$$
\frac{d}{dt}(t\psi_{ik}(ta)) = \delta_{ik} + \sum_{j,l} c_{jl}^k ta_l \psi_{ij}(ta).
$$

These integrate and give a formula equivalent to the formula

$$
\varpi(\mathbf{X}) = \sum_{n \geq 0} \frac{1}{(n+1)!} (\mathrm{ad}(\mathbf{X}))^n
$$

¹ This converse was not obtained without difficulty. The first proof that Lie gives (III e)) consists of passing to the adjoint group and is in fact valid only if the center of the given Lie algebra is reduced to $0$. He then gives two general proofs (IV, vol. 2, chap. XVII and vol. 3, p. 599-604); it is rather significant that the first is based on contact transformations and that Lie finds it more natural than the second.

¹ One can observe a similar evolution in the theory of "abstract" groups, in particular finite ones. They were initially defined as transformation groups, but already Cayley remarked that the essential point is the way in which the transformations compose with each other, and not the nature of the concrete representation of the group as a permutation group of particular objects.

from our Chapter III, § 6, No. 4, Proposition 12; in particular, in canonical coordinates, the $\psi_{ij}$ extend to entire functions of the $a_k$. F. Schur deduces from this a result making precise an earlier remark of Lie: if, in definition (4) of transformation groups, one assumes only that the $f_i$ are of class $C^2$, then the group is holohedrically isomorphic to an analytic group.\footnote{Lie had already stated without proof a result of this kind (III i)). He had been led to it by his researches on the foundations of geometry (“Helmholtz problem”), where he had remarked that the hypotheses of analyticity are not natural.}

Following his researches on the integration of differential systems, E. Cartan (XII, t. II_2, p. 371) introduces in 1904 the Pfaffian forms

$$
\omega_k = \sum_{i=1}^r \psi_{ki} da_i \quad (1 \leq i \leq r)
$$

(with the notations of (15)), later called *Maurer-Cartan forms*. The conditions (17) of Maurer can then be written

$$
d\omega_k = -\frac{1}{2} \sum_{i,j} c_{ij}^k \omega_i \wedge \omega_j;
$$

The result of F. Schur was to lead Hilbert, in 1900, to ask whether the same conclusion remained valid if one assumes only the $f_i$ continuous (“5th Hilbert problem”). This problem has given rise to numerous researches. The most complete result in this vein is the following theorem, proved by A. Gleason, D. Montgomery and L. Zippin: every locally compact topological group possesses an open subgroup which is a projective limit of Lie groups; it implies that every locally euclidean group is a Lie group. For more details on this question, cf. D. MONTGOMERY and L. ZIPPIN (XLI).

E. Cartan shows that one can develop the theory of finite and continuous groups from the $\omega_k$ and establishes the equivalence of this point of view and that of Lie. But, for him, the interest of this method is especially that it adapts to the “infinite and continuous groups” whose theory he pushes much further than Lie had done, and that it permits him to erect his theory of the generalized “moving frame”.

IV. The theory of Lie algebras

Once the correspondence between transformation groups and Lie algebras is acquired, the theory takes a markedly more algebraic turn and is centred on a deep study of Lie algebras.$^1$

A first and short period, from 1888 to 1894, marked by the works of Engel, his student Umlauf and especially Killing and E. Cartan, leads to a series of spectacular results on complex Lie algebras. We have seen above that the notion of solvable Lie algebra is due to Lie himself, who had proved (in the complex case) the reduction theorem of solvable linear Lie algebras to triangular form (IV, t. 1, p. 270).$^2$ Killing observes (XI) that there exists in a Lie algebra a greatest solvable ideal (today called the radical), and that the quotient of the Lie algebra by its radical has zero radical; he calls *semisimple* the Lie algebras of zero radical, and proves that they are products of simple algebras (this last notion had already been introduced by Lie, who had proved the simplicity of the “classical” Lie algebras (IV, t. 3, p. 682)).

On the other hand, Killing introduces, in a Lie algebra, the characteristic equation $\det(\mathrm{ad}(x) - \omega.1) = 0$, already met by Lie while studying the Lie subalgebras of dimension 2 containing a given element of a Lie algebra. We refer to other Historical Notes of this Book for the analysis of the methods by which Killing, by deeply studying the properties of the roots of the characteristic equation “generic” for a semisimple algebra, arrives at the most remarkable of his results, the *complete* determination of simple Lie algebras (complex).$^3$

$^1$ The term “Lie algebra” was introduced by H. Weyl in 1934: in his works of 1925, he had used the expression “infinitesimal group”. Previously, one speaks simply of the “infinitesimal transformations $X_1 f, \ldots, X_r f$” of the group, which Lie and Engel frequently abbreviate by saying “the group $X_1 f, \ldots, X_r f$”!

$^2$ Almost at the beginning of his researches, Lie had encountered solvable linear groups, and even in fact nilpotent ones (III $f$).

$^3$ Except that he finds two exceptional algebras of dimension 52, of which he does not notice the isomorphism. (It concerns solely complex simple Lie algebras, for no more general problem was envisaged at that time; Killing's methods are in fact valid for any algebraically closed field of characteristic 0).

Killing proves that the derived algebra of a solvable algebra is “of rank 0” (which means that ad $x$ is nilpotent for every element $x$ of the algebra). A short time later, Engel proves that the algebras “of rank 0” are solvable (this statement is in substance what we have called the Engel theorem in Chapter I, § 4, No. 2). In his thesis, E. Cartan introduces moreover what is now called the “Killing form”, and establishes the two fundamental criteria which characterize by means of this form solvable Lie algebras and semisimple Lie algebras.

Killing had asserted (XI, IV) that the derived algebra of a Lie algebra is a sum of a semisimple algebra and its radical, which is nilpotent, but his proof was incomplete. A little later, E. Cartan announced without proof (XII, t. I₁, p. 104) that more generally every Lie algebra is a sum of its radical and a semisimple subalgebra; the only result in this direction established indisputably at that time is an Engel theorem asserting the existence, in any non-solvable Lie algebra, of a simple Lie subalgebra of dimension 3. The first published proof (for complex Lie algebras) of Cartan's statement is due to E. E. Levi (XVIII); another proof (valid also in the real case) was given by J. H. C. Whitehead in 1936 (XXVI a)). In 1942 A. Malcev complemented this result with the uniqueness theorem for "Levi sections" up to conjugation.

From his very first works, Lie had posed the problem of the isomorphism of any Lie algebra with a linear Lie algebra. He believed he had resolved it affirmatively by considering the adjoint representation (and deducing thus a proof of his "third theorem"), (III e)); he soon recognized that his proof was correct only for Lie algebras with null center; after him, the question remained open for a very long time, and was resolved affirmatively by Ado in 1935 (XXVII). On the other hand, Lie had posed in substance the problem of determining the linear representations of minimal dimension of simple Lie algebras, and had solved it for the classical algebras; in his Thesis, Cartan also solves this problem for the exceptional simple algebras¹; the methods he uses for this purpose will be generalized by him twenty years later to obtain all the irreducible representations of real or complex simple Lie algebras.

The property of complete reducibility of a linear representation seems to have been encountered for the first time (in a geometric form) by Study. In an unpublished manuscript, but cited in (IV, t. 3, p. 785–788), he proves this property for the linear representations of the Lie algebra of $\mathbf{SL}(2, \mathbf{C})$, and obtains partial results for $\mathbf{SL}(3, \mathbf{C})$ and $\mathbf{SL}(4, \mathbf{C})$. Lie and Engel conjectured on this occasion that the theorem of complete reducibility holds for $\mathbf{SL}(n, \mathbf{C})$ for any $n$. The complete reducibility of the linear representations

¹ Cartan's point of view consists in studying Lie algebras which are non-trivial extensions of a simple Lie algebra and a (commutative) radical of minimal dimension.

of semisimple Lie algebras was established by H. Weyl in 1925¹ by an argument of global nature (see later). The first algebraic proof was obtained in 1935 by Casimir and van der Waerden (XXXII); other algebraic proofs were subsequently given by R. Brauer (XXXI) (the one we have reproduced) and J. H. C. Whitehead (XXVI, b)).

Finally, in the course of his research on the exponential mapping (cf. infra), H. Poincaré (XIV, t. 3) considers the associative algebra of differential operators of all orders, generated by the operators of a Lie algebra; he shows in substance that, if $(X_i)_{1 \leq i \leq n}$ is a basis of the Lie algebra, the associative algebra generated by the $X_i$ has as basis certain symmetric functions of the $X_i$ (sums of non-commutative "monomials" deduced from a given monomial by all permutations of the factors). The essential part of his proof is algebraic in nature, and allows obtaining the structure of the enveloping algebra that we have defined abstractly in chap. I. Analogous proofs were given in 1937 by G. Birkhoff (XXIX b)) and E. Witt (XXX).²

Most of the works cited above are limited to real or complex Lie algebras, which alone correspond to Lie groups in the usual sense. The study of Lie algebras over a field other than $\mathbf{R}$ or $\mathbf{C}$ is approached by Jacobson (XXVIII a)), who shows that the greater part of the classical results (i.e., those of chap. I) remain valid over a field of characteristic zero.

V. Exponential and Hausdorff formula

The first research concerning the exponential mapping are due to E. Study and F. Engel; Engel (IX b)) notes that the exponential map is not surjective for $\mathbf{SL}(2, \mathbf{C})$ (for example $\begin{pmatrix} -1 & a \\ 0 & -1 \end{pmatrix}$ is not an exponential if $a \neq 0$), but that it is for $\mathbf{GL}(n, \mathbf{C})$, and therefore also for $\mathbf{PGL}(n, \mathbf{C})$ (this latter property had already been noted by Study for $n = 2$); thus $\mathbf{SL}(2, \mathbf{C})$ and $\mathbf{PGL}(2, \mathbf{C})$ give an example of two locally isomorphic groups, which are nonetheless very different from the global point of view. Engel also shows that the exponential map is surjective in the other classical groups, augmented by the homotheties; these works are taken up and continued by Maurer, Study, and others, without bringing substantial novelties.

¹ H. Weyl remarks on this occasion that the construction given by E. Cartan of the irreducible representations implicitly uses this property.
² The first use of the higher-order differential operators generated by the $X_i$ is undoubtedly the employment of the "Casimir operator" for the proof of the theorem of complete reducibility. After 1950, the research of Gelfand and his school, and of Harish-Chandra, on the linear representations of infinite dimension, brought these operators to the forefront.

In 1899, H. Poincaré (XIV, t. 3, p. 169–172 and 173–212), approaches the study of the exponential mapping from a different point of view. His memoirs appear to have been hastily written, because in several places he asserts that every element of a connected group is an exponential, whereas he gives examples of the contrary elsewhere. His results bear principally on the adjoint group: he shows that a semisimple element of such a group $G$ can be the exponential of infinitely many elements of the Lie algebra $\mathfrak{L}(G)$, whereas a non-semisimple element may not be an exponential. If $\operatorname{ad}(X)$ does not have a nonzero multiple eigenvalue of $2\pi i$, then $\exp$ is étale at $X$. He also proves that, if $U$ and $V$ describe loops in $\mathfrak{L}(G)$, and if one defines by continuity $W$ such that $e^U.e^V = e^W$, one does not necessarily return to the initial determination of $W$. He uses a residue formula which comes essentially to

$$
\Phi(\mathrm{ad}\ X) = \frac{1}{2\pi i} \int \frac{\Phi(\xi)\ d\xi}{\xi - \mathrm{ad}\ X}
$$

where $\operatorname{ad}(X)$ is a semisimple element whose nonzero eigenvalues are of multiplicity 1, $\Phi$ a power series with a sufficiently large radius of convergence, the integral being taken over a loop enclosing the eigenvalues of $\operatorname{ad} X$; he also studies what happens when $X$ tends toward a transform having multiple eigenvalues.

The search for expressions of $W$ in terms of $U$ and $V$ in the formula $e^U.e^V = e^W$ had already, shortly before Poincaré's work, been the subject of two memoirs by Campbell (XIII). As Baker writes a little later, "... Lie's theory obviously suggests that the product $e^Ue^V$ is of the form $e^W$ where $W$ is a series of alternants in $U$ and $V$ ...". Subsequent work on this subject aims at clarifying this assertion and giving an explicit formula (or a construction method) for $W$ (the "Hausdorff formula"). After Campbell and Poincaré, Pascal, Baker (XV), and Hausdorff (XVI) return to the question; each considers the proofs of his predecessors to be unconvincing; the main difficulty resides in what is to be understood by "alternants": are they elements of the particular Lie algebra one is considering, or are they universal "symbolic" expressions? Neither Campbell, nor Poincaré, nor Baker express themselves clearly on this point. Hausdorff's memoir, on the other hand, is perfectly precise; he works first in the algebra of associative (noncommutative) formal series in a finite number of indeterminates and considers $U, V, W$ as elements of this algebra. He demonstrates the existence of $W$ by a differential equation argument analogous to that of his predecessors. The same argument serves him to prove the convergence of the series when the indeterminates are replaced by elements of a finite-dimensional Lie algebra. As Baker had remarked, and independently Poincaré, this result can serve to give a proof of Lie's third theorem; it elucidates the correspondence between groups and Lie algebras, for example as regards the commutator group.

In 1947, Dynkin (XXXIX) takes up the question again, and obtains the explicit coefficients of the Hausdorff formula, by considering from the outset a normed Lie algebra (finite-dimensional or not, over $\mathbf{R}, \mathbf{C}$ or an ultrametric field).¹

VI. Linear representations and global Lie groups

None of the works we have just spoken of frankly addressed the problem of the definition and study of global Lie groups. The first steps in this direction are due to H. Weyl. He draws inspiration from two theories, which had until then developed independently: that of linear representations of complex semisimple Lie algebras, due to E. Cartan, and that of linear representations of finite groups, due to Frobenius and which had just been transposed to the orthogonal group by I. Schur, using an idea of Hurwitz. The latter had shown (XVII) how one can form invariants for the orthogonal group or the unitary group by replacing the averaging operation over a finite group by integration relative to an invariant measure. He had also remarked that, by applying this method to the unitary group, one obtains invariants for the general linear group, the first example of the "unitarian trick". In 1924, I. Schur (XX) uses this method to show the complete reducibility of the representations of the orthogonal group $\mathbf{O}(n)$ and of the unitary group $\mathbf{U}(n)$, by the construction of an invariant positive non-degenerate Hermitian form; he deduces, by the "unitarian trick", the complete reducibility of the holomorphic representations of $\mathbf{O}(n, \mathbf{C})$, and of $\mathbf{SL}(n, \mathbf{C})$, establishes orthogonality relations for the characters of $\mathbf{O}(n)$ and of $\mathbf{U}(n)$ and determines the characters of $\mathbf{O}(n)$. H. Weyl immediately extends this method to complex semisimple Lie algebras (XXI). Given such an algebra $\mathfrak{g}$, he shows that it possesses a "compact real form" (which amounts to saying that it arises by extension of scalars from $\mathbf{R}$ to $\mathbf{C}$ of an algebra $g_0$ over $\mathbf{R}$ whose adjoint group $G_0$ is compact). Moreover, he shows that the fundamental group of $G_0$ is finite, hence that the universal covering² of $G_0$ is compact. He deduces, by a suitable adaptation of Schur's method, the complete reducibility of the representations of $\mathfrak{g}$, and also gives, by a global method, the determination of the characters of the representations of $\mathfrak{g}$. In a letter to I. Schur (Sitzungsber. Berlin,

¹ In the ultrametric case, the classical method of majorants cannot be extended without precautions, because of the asymptotic behaviour of the $p$-adic absolute value of $1/n$ as $n$ tends to infinity.

² H. Weyl does not explicitly define this notion, with which he had been familiar since the writing of his course on Riemann surfaces (1913). It is O. Schreier (XXII) who, in 1926–1927, gives, for the first time, the definition of a topological group and that of a "continuous" group (i.e. locally homeomorphic to a Euclidean space), as well as the construction of the universal covering of such a group.

1924, 338–343), H. Weyl summarises the results of Cartan, which Schur did not know (cf. (XX), p. 299, footnote) and compares the two points of view: Cartan's method provides all holomorphic representations of the simply connected group of Lie algebra g; in the case of the orthogonal group, one thus obtains representations of a two-sheeted covering (later called the spinor group), which escape Schur; on the other hand, Schur's method has the advantage of proving complete reducibility and of giving explicitly the characters.

After the works of H. Weyl, E. Cartan adopts a frankly global point of view in his research on symmetric spaces and Lie groups. It is this point of view which is at the basis of his 1930 exposition (XII, t. I2, p. 1165–1225) of the theory of "finite and continuous" groups. There one finds in particular the first proof of the global variant of the 3rd fundamental theorem (existence of a Lie group with given Lie algebra); Cartan also shows that every closed subgroup of a real Lie group is a Lie group (Chap. III, § 8, No. 2, Theorem 2) which generalises a result of J. von Neumann on closed subgroups of the linear group (XXIII). In this Memoir, von Neumann also showed that every continuous representation of a complex semisimple group is real analytic.

After these works, the theory of Lie groups in the "classical" sense (that is, of finite dimension over $\mathbf{R}$ or $\mathbf{C}$) is more or less fixed in its broad outlines. The first detailed exposition of it is given by Pontrjagin in his book on topological groups (XXXVI); there he keeps a point of view still rather close to that of Lie, but carefully distinguishing the local from the global. He is followed by Chevalley's book (XXXVIII) which also contains the first systematic discussion of the theory of analytic manifolds and exterior differential calculus; Lie's "infinitesimal transformations" appear there as vector fields and the Lie algebra of a Lie group G is identified with the space of left-invariant vector fields on G. He leaves aside the "local groups" aspect and the "transformation groups" aspect.

VII. Extensions of the notion of Lie group

In our day, the vitality of Lie theory manifests itself through the diversity of its applications (in topology, differential geometry, arithmetic, etc.), as well as through the creation of parallel theories where the underlying differential manifold structure is replaced by a neighbouring structure (manifold $p$-adique, algebraic, scheme, formal scheme, ...). We do not have to give here the history of all these developments, and we shall confine ourselves to those dealt with in Chap. III: Lie groups $p$-adiques.

a) Banach Lie groups

These are Lie groups "of infinite dimension". From the local point of view, one replaces a neighbourhood of 0 in a Euclidean space by a neighbourhood of 0 in a Banach space. This is what G. Birkhoff does in 1936 (XXIX a)), thus arriving at the notion of a complete normed Lie algebra and its correspondence with a "groupuscule" defined on an open set of a Banach space. Around 1950, Dynkin completes these results by an extension to this case of the Hausdorff formula (cf. supra).

The definitions and results of Birkhoff and Dynkin are local. Until a recent date, it does not seem that anyone has sought to make explicit the corresponding global theory, no doubt for lack of applications.¹

¹ If, despite this lack of applications, we have included the "Banach" groups in Chap. III, it is because Banach manifolds are increasingly used in analysis (and for the study of finite-dimensional manifolds themselves), and because, moreover, this generalization presents no additional difficulty.

b) Lie groups $p$-adiques

Such groups are encountered for the first time in 1907 in the work of Hensel (XIX) on $p$-adic analytic functions (defined by developments in power series). The latter studies in particular the exponential and the logarithm; despite the $a$ priori surprising behaviour of the series that define them (for example the exponential series does not converge everywhere), their fundamental functional properties remain valid, which provides a local isomorphism between the additive group and the multiplicative group of $\mathbf{Q}_p$ (or, more generally, of any complete ultrametric field of characteristic zero).

It is also a question of commutative groups (but non-linear this time) in the work of A. Weil (XXXIII) and E. Lutz (XXXIV) on elliptic curves $p$-adiques (1936). Besides arithmetic applications, one finds there the construction of a local isomorphism of the group with the additive group, based on the integration of an invariant differential form. This method applies equally to abelian varieties, as C. Chabauty remarks shortly after, who uses it without further explanation to prove a particular case of the "Mordell conjecture" (XXXV).

From this moment on, it was clear that the local theory of Lie groups applied almost without change to the case $p$-adique. The fundamental theorems of the "dictionary" between Lie groups and Lie algebras are established in 1942 in the thesis of R. Hooke (XXXVII), a student of Chevalley; this work also contains the $p$-adic analogue of E. Cartan's theorem on closed subgroups of real Lie groups.

More recently, M. Lazard (XLII, b) develops a more precise form of the "dictionary" for compact analytic groups over $\mathbf{Q}_p$. He shows that the existence of an analytic structure $p$-adique on a compact group G is closely linked to that of certain filtrations on G, and gives various applications of it (for example to the cohomology of G). One of Lazard's tools is an improvement of Dynkin's results on the convergence of the Hausdorff series $p$-adique (XLII a)).

VIII. Free Lie algebras

It remains for us to speak of a series of works on Lie algebras where the link with the theory of Lie groups is very tenuous; these researches, on the other hand, have important applications in the theory of "abstract" groups and more especially of nilpotent groups.

The origin of it is the work of P. Hall (XXIV), published in 1932. There is, however, no question of Lie algebras in it: P. Hall has in view the study of a certain class of $p$-groups, those which he calls "regular". But this leads him to examine in detail the iterated commutators and the descending central series of a group; he establishes on this occasion a variant of the Jacobi identity (cf. Chap. II, § 4, No. 4, formula (20)) as well as the "Hall formula"

$$
(xy)^n = x^n y^n (x, y)^{n(1-n)/2} \ldots \quad \text{(cf. Chap. II, § 5, Exerc. 9).}
$$

Shortly afterwards (in 1935–1937) appear the fundamental works of W. Magnus (XXV a) and b)) and E. Witt (XXX). In (XXV a)) Magnus uses the same formal power series algebra $\hat{A}$ as Hausdorff (called since "Magnus algebra"); he embeds the free group F in it and uses the natural filtration of $\hat{A}$ to obtain a decreasing sequence $(F_n)$ of subgroups of F; this is one of the first examples of a filtration. He conjectures that the $F_n$ coincide with the terms of the descending central series of F. This conjecture is proved in his second memoir (XXV b)); it is also there that he explicitly makes the connection between his ideas and those of P. Hall, and that he defines the free Lie algebra L (as a subalgebra of $\hat{A}$) of which he shows in substance that it identifies with the graded of F. In (XXX), Witt completes this result on several points. He shows in particular that the enveloping algebra of L is a free associative algebra and immediately deduces the rank of the homogeneous components of L ("Witt formulas").

As regards the determination of the basis of $L$ known as the "Hall basis" (cf. Chap. II, § 2, no. 11), it seems that it first appeared only in 1950, in a note of M. Hall (XL), although it is implicit in the works of P. Hall and W. Magnus cited above.

I. F. KLEIN and S. LIE: a) Sur une certaine famille de courbes et surfaces, C. R. Acad. Sci., t. LXX (1870), p. 1222–1226 et p. 1275–1279 (= (II, p. 416–420) et (III, t. 1, p. 78–85)); b) Über diejenigen ebenen Kurven, welche durch ein geschlossenen System von einfach unendlich vielen vertauschbaren linearen Transformationen in sich übergehen, Math. Ann., t. IV (1871), p. 50–84 (= (II, p. 424–459) et (III, t. 1, Abh. XIV, p. 229–266)).

II. F. KLEIN, Gesammelte mathematische Abhandlungen, Bd. I, Berlin (Springer), 1921.

III. S. LIE, Gesammelte Abhandlungen, 7 vol., Leipzig (Teubner): a) Über die Reziprozitätsverhältnisse des Reyeschen Komplexes, t. I, Abh. V, p. 68–77 (= Gött. Nach. (1870), p. 53–66); b) Über eine Klasse geometrischer Transformationen, t. I, Abh. XII, p. 153–214 (= Christiana For. (1871), p. 182–245); c) Kurzes Resume mehrerer neuer Theorien, t. V, Abh. I, p. 1–4 (= Christiana For. (1872), p. 24–27); d) Über partielle Differentialgleichungen erster Ordnung, t. V, Abh. VII, p. 32–63 (= Christiana For. (1873), p. 16–51); e) Theorie der Transformationsgruppen II, t. V, Abh. III, p. 42–75 (= Archiv f. Math., t. I (1876), p. 152–193); f) Theorie der Transformationsgruppen III, t. V, Abh. IV, p. 78–133 (= Archiv f. Math., t. III (1878), p. 93–165); g) Untersuchungen über Differentialgleichungen III, t. V, Abh. XII, p. 311–313 (= Christiana For. (1883), n° 10, 1–4); h) Untersuchungen über Transformationsgruppen II, t. V, Abh. XXII, p. 507–551 (= Archiv f. Math., t. X (1886), p. 353–413); i) Beiträge zur allgemeinen Transformationstheorie, t. VI, Abh. V, p. 230–236 (= Leipziger Ber. (1888), p. 14–21).

IV. S. LIE und F. ENGEL, Theorie der Transformationsgruppen, 3 vol., Leipzig (Teubner), 1888–1893.

V. J. J. SYLVESTER, Collected Mathematical Papers, 4 vol., Cambridge, 1904–1911.

VI. A. CAYLEY, Collected Mathematical Papers, 13 vol., Cambridge, 1889–1898.

VII. C. JORDAN, Mémoire sur les groupes de mouvements, Annali di Math., t. XI (1868–1869), p. 167–215 et p. 332–345 (= Œuvres, t. IV, p. 231–302).

VIII. F. SCHUR: a) Zur Theorie der aus Haupteinheiten gebildeten Komplexen, Math. Ann., t. XXXIII (1889), p. 49–60; b) Neue Begründung der Theorie der endlichen Transformationsgruppen, Math. Ann., t. XXXV (1890), p. 161–197; c) Zur Theorie der endlichen Transformationsgruppen, Math. Ann., t. XXXVIII (1891), p. 273–286; d) Über den analytischen Character der eine endliche continuierliche Transformationsgruppe darstellende Funktionen, Math. Ann., t. XLI (1893), p. 509–538.

IX. F. ENGEL: a) Über die Definitionsgleichung der continuierlichen Transformationsgruppen, Math. Ann., t. XXVII (1886), p. 1–57; b) Die Erzeugung der endlichen Transformationen einer projektiven Gruppe durch die infinitesimalen Transformationen der Gruppe, I, Leipziger Ber., XLIV (1892), p. 279–296, II (mit Beiträgen von E. Study), ibid., XLV (1893), p. 659–696.

X. L. Maurer, Über allgemeinere Invarianten-Systeme, Sitzungsber. München, XVIII (1888), p. 103–150.

XI. W. Killing, Die Zusammensetzung der stetigen endlichen Transformationsgruppen: I) Math. Ann., t. XXXI (1888), p. 252–290; II) ibid., t. XXXIII (1889), p. 1–48; III) ibid., t. XXXIV (1889), p. 57–122; IV) ibid., t. XXXVI (1890), p. 161–189.

XII. E. Cartan, Œuvres complètes, 6 vol., Paris (Gauthier-Villars), 1952–54.

XIII. J. E. Campbell: a) On a law of combination of operators bearing on the theory of continuous transformation groups, Proc. London Math. Soc., (1), t. XXVIII (1897), p. 381–390; b) On a law of combination of operators (second paper), ibid., t. XXIX (1898), p. 14–32.

XIV. H. Poincaré, Œuvres, 11 vol., Paris (Gauthier-Villars), 1916–1956.

XV. H. F. Baker, Alternants and continuous groups, Proc. London Math. Soc., (2), t. III (1905), p. 24–47.

XVI. F. Hausdorff, Die symbolische Exponentialformel in der Gruppentheorie, Leipziger Ber., t. LVIII (1906), p. 19–48.

XVII. A. Hurwitz, Über die Erzeugung der Invarianten durch Integration, Gött. Nachr. (1897), p. 71–90 (= Math. Werke, t. II, p. 546–564).

XVIII. E. E. Levi, Sulla struttura dei Gruppi finiti e continui, Atti Acc. Sci. Torino, t. XL (1905), p. 551–565 (= Opere, t. I, p. 101–115).

XIX. K. Hensel, Über die arithmetischen Eigenschaften der Zahlen, Jahresber. der D.M.V., t. XVI (1907), p. 299–319, 388–393, 474–496.

XX. I. Schur, Neue Anwendungen der Integralrechnung auf Probleme der Invariantentheorie, Sitzungsber. Berlin, 1924, p. 189–208, 297–321, 346–355.

XXI. H. Weyl, Theorie der Darstellung kontinuierlicher halb-einfacher Gruppen durch lineare Transformationen, I, Math. Zeitschr., t. XXIII (1925), p. 271–309; II, ibid., t. XXIV (1926), p. 328–376; III, ibid., t. XXIV (1926), p. 377–395 (= Werke, t. 2 p 543–647).

XXII. O. Schreier: a) Abstrakte kontinuierliche Gruppen, Abh. math. Sem. Hamburg, t. IV (1926), p. 15–32; b) Die Verwandtschaft stetiger Gruppen in grossen, ibid., t. V (1927), p. 233–244.

XXIII. J. von Neumann, Zur Theorie der Darstellung kontinuierlicher Gruppen, Sitzungsber. Berlin, 1927, p. 76–90 (= Collected Works, t. I, p. 134–148).

XXIV. P. Hall, A contribution to the theory of groups of prime power order, Proc. London Math. Soc., (3), t. IV (1932), p. 29–95.

XXV. W. Magnus: a) Beziehungen zwischen Gruppen und Idealen in einen speziellen Ring, Math. Ann., t. CXI (1935), p. 259–280; b) Über Beziehungen zwischen höheren Kommutatoren, J. Crelle, t. CLXXVII (1937), p. 105–115.

XXVI. J. H. C. Whitehead: a) On the decomposition of an infinitesimal group, Proc. Camb. Phil. Soc., t. XXXII (1936), p. 229–237 (= Mathematical Works, I, p. 281–289); b) Certain equations in the algebra of a semisimple infinitesimal group, Quart. Journ. of Math., (2), t. VIII (1937), p. 220–237 (= Mathematical Works, I, p. 291–308).

XXVII. I. Ado: a) Note on the representation of finite and continuous groups by means of linear substitutions (in Russian), Bull. Phys. Math. Soc. Kazan, t. VII (1935), p. 3–43; b) The representation of Lie algebras by matrices (in Russian), Uspehi Mat. Nauk, t. II (1947), p. 159–173 (English translation: Amer. Math. Soc. Transl., (1), vol. 9, p. 308–327).

XXVIII. N. Jacobson: a) Rational methods in the theory of Lie algebras, Ann. of Math., t. XXXVI (1935), p. 875–881; b) Classes of restricted Lie algebras of characteristic $p$, II, Duke Math. Journal, t. X (1943), p. 107–121.

XXIX. G. Birkhoff: a) Continuous groups and linear spaces, Rec. Math. Moscou, t. I (1936), p. 635–642; b) Representability of Lie algebras and Lie groups by matrices, Ann. of Math., t. XXXVIII (1937), p. 526–532.

XXX. E. Witt, Treue Darstellung Lieschen Ringe, J. Crelle, t. CLXXVII (1937), p. 152–160.
XXXI. R. Brauer, Eine Bedingung für vollständige Reduzibilität von Darstellungen gewöhnlicher und infinitesimaler Gruppen, Math. Zeitschr., t. XLI (1936), p. 330–339.
XXXII. H. Casimir–B. L. van der Waerden, Algebraischer Beweis der vollständigen Reduzibilität der Darstellungen halbeinfacher Liescher Gruppen, Math. Ann., t. CXI (1935), p. 1–12.
XXXIII. A. Weil, On elliptic functions $p$-adiques, C. R. Acad. Sci., t. CCIII (1936), p. 22.
XXXIV. E. Lutz, On the equation $y^2 = x^3 - Ax - B$ in the fields $p$-adiques, J. Crelle, t. CLXXVII (1937), p. 237–247.
XXXV. C. Chabauty, On the rational points of algebraic curves of genus upper to the unity, C. R. Acad. Sci., t. CCXII (1941), p. 882–884.
XXXVI. L. S. Pontrjagin, Topological Groups, Princeton Univ. Press, 1939.
XXXVII. R. Hooke, Linear $p$-adic groups and their Lie algebras, Ann. of Math., t. XLIII (1942), p. 641–655.
XXXVIII. C. Chevalley, Theory of Lie Groups, Princeton University Press, 1946.
XXXIX. E. Dynkin: a) Calculus of the coefficients of the Campbell–Hausdorff formula (in Russian), Dokl. Akad. Nauk, t. LVII (1947), p. 323–326; b) Normed Lie algebras and analytic groups (in Russian), Uspehi Mat. Nauk, t. V (1950), p. 135–186 (English translation: Amer. Math. Soc. Transl., (1), vol. 9, p. 470–534).
XL. M. Hall, A basis for free Lie rings and higher commutators in free groups, Proc. Amer. Math. Soc., t. I (1950), p. 575–581.
XLI. D. Montgomery–L. Zippin, Topological Transformation Groups, New York (Interscience), 1955.
XLII. M. Lazard: a) Some calculuses concerning the Hausdorff formula, Bull. Soc. Math. France, t. XCI (1963), p. 435–451; b) Analytic groups $p$-adiques, Publ. Math. I.H.E.S., n° 26 (1965), p. 389–603.

The reference numbers indicate successively the chapter, the paragraph and the number.

K : II.Conventions
g, U = Ug, σ : g → Ug: II.1
ε, c, u, π_u, η_u, c_u^+ : II.1.1
E, E^+ : II.1.1
P(E), π, η, c^+ : II.1.6
S(g), c_s, η : II.1.5
f_E : U(P(E)) → E : II.1.6
M(X), l(w), Lib(X) = Lib_K(X) : II.2.1
L(X) = L_K(X) : II.2.2
φ : X → L(X) : II.2.2
(a, r) : II.2.3
L(u) : II.2.5
Lib^δ(X), L^δ(X), L^n(X) : II.2.6
P_n : II.2.7
c^n(g) : II.2.7
H, d_y : II.2.10
w̄ = Ψ(w) : II.2.11
A(X) = A_K(X), A^+(X), Mo(X) : II.3
π : II.3.2
(G_α), (G_α^+) : II.4.1
v : II.4.2
gr(G), gr_α(G) : II.4.3
F(X), A(X), A^n(X) : II.5
Â(X), ω : II.5.1
ε(a) : II.5.2
l(x), exp(x), log(y) : II.6.1
e(X), l(X) : II.6.1
L̂(X) : II.6.2
a ⊕ b : II.6.2
H, H_n, H_{rs} : II.6.4 \tilde{H}, \Omega : II.7.2
A, \exp_A, \log_A, \hat{P}(A^1, A) : II.7.3
v, \theta = \frac{1}{p - 1} : II.8
S(n) : II.8.1
h(x, y) : II.8.3
G_R : II.8.4
\mu(n) : II.App.
e, e_G, \gamma(g), \delta(g), \mathrm{Int}(g), f' : III.Conventions
\mathbf{GL}(E), \mathbf{GL}(n, K) : III.1.1, III.3.10
G^\vee : III.1.2
\tau(g), \rho(x) : III.1.5
(G, g, \theta, m) : III.1.10
T(m) : III.2.1
T(G), T(\varphi) : III.2.2
t \* t' : III.3.1, III.3.18
U(G), U^+(G), U_s(G), U_s^+(G) : III.3.1, III.3.18
T_g^{(s)}(G), T_g^{(\infty)}(G), \mathcal{T}^{(\infty)}(G) : III.3.1, III.3.18
t \* f : III.3.4, III.3.18
D_t : III.3.5, III.3.18
L_t, R_t : III.3.6, III.3.18
L(G) : III.3.7, III.3.18
L(\varphi) : III.3.8, III.3.18
\langle t, f \rangle : III.3.9, III.3.18
\mathbf{SL}(E) : III.3.10
Ad, Ad(g) : III.3.12
[\alpha]^2 : III.3.14
\mathrm{mod}\ (\omega)_\mu^!, \mathrm{mod}\ \varphi : III.3.16
f^{-1}.df : III.3.17, III.3.18
H : III.4.2
g^t, \varpi(x) : III.4.3
x.y, x^{[n]} : III.5
c_{\alpha\beta\gamma}, B(x, y) : III.5.1
e_\alpha : III.5.2
\Psi_j, \Psi_{p,m}, \binom{t}{i} : III.5.3
E(x), L(x) : III.5.4
P_{M,x,y} : III.6.2
\mathrm{Ad}(a) = \mathrm{Int}(a) : III.6.2
\exp, \exp_G : III.6.4
\mathrm{Ad}(G) = \mathrm{Int}(L(G)) : III.6.4
L(\rho) : III.6.5 \tilde{G}: III.6.10
A, m, p: III.7
G(a): III.7.4
h_n: III.7.5
G_f, \log_G, \log: III.7.6
\overline{D}^i G, \overline{C}^i G: III.9.1
Z_G(A), Z_G(a), \delta_G(A), \delta_G(a): III.9.3
N_G(A), N_G(a), n_G(a): III.9.4
R, N, r, n: III.9.7
\pi_1 \otimes \cdots \otimes \pi_n, T(\pi), S(\pi), \wedge(\pi), T^n(\pi), S^n(\pi), \wedge^n(\pi): III.App.

The reference numbers indicate successively the chapter, the paragraph and the number (or, exceptionally, the exercise).

adjoint (group — of a real or complex Lie group): III.6.4
adjoint (representation —): III.3.12
alternating (degree $n$ —): II.2.6
ascending (central series of a group —): II.4, exerc. 18
free associative (algebra —): II.3
associated (infinitesimal operation law — to an operation law): III.3.7
basic (basis of a Lie algebra —): II.2.3
basic (commutators —): II.5.4
Bieberbach (theorem —): III.4, exerc. 13
bicébra: II.1.2
biinvariant (section —): III.3.13
binomial (polynomial —): II.5, exerc. 4
canonical (left differential form —): III.3.13, III.3.18
central (filtration of a group —): II.4.4
centralizer: III.9.3
field of pointwise distributions: III.3.5, III.3.18
nilpotency class: II.2.7
cogebra: II.1.1
compatible (group and manifold structures —): III.1.1
complex (Lie group —): III.1.1, III.8.1
complexification of a real Lie group: III.6.10
conjugate (Lie group of a complex Lie group —): III.1.1
contragredient (of an analytic representation —): III.3.11
convolved (with a pointwise distribution and a function —): III.3.4
convolution (product of —): III.3.1, III.3.18
counit of a cogebra: II.1.1
$C^r$ — connected (subset of a Lie group —): III.6.2
partial derivative (in the algebra of a free group —): II.5, exerc. 2
second kind (canonical chart of —): III.4.3
second kind (system of canonical coordinates of —): III.4.3 differential left (of a mapping into a Lie group —): III.3.17, III.3.18
elimination (theorem of —): II.2.9
entire (filtration of a group —): II.4.1
enveloping (cogebra —): II.1.4
homogeneous space of Lie: III.1.6
exhaustive (filtration —): II.4.1
exponential: II.6.1, III.4.3, III.6.4
left foliation associated with a Lie subalgebra: III.4.1
real (filtration of a group —): II.4.1
filtered (cogebra —): II.1.3
order function associated with a filtration: II.4.2
G-vector bundle: III.1.8
total grading of L(I): II.2.6
associated graded (group of a filtered group —): II.4.3
associated graded (Lie algebra —): II.4.4
Lie group: III.1.10
Lie group defined by a Lie algebra: III.4.2
Hall (basis of —): II.2.11
Hall (set of —): II.2.10
Hall (formula of —): II.5, exerc. 9
Hausdorff (function of —): II.7.2, II.8.3
Hausdorff (group of —): II.6.2
Hausdorff (inversion of the formula of —): II.6, exerc. 4
Hausdorff (series of —): II.6.4
inverse image (Lie group structure —): III.1.9
induced (Lie group structure —): III.4.5
infinitesimal (automorphism —): III.10.1
integral (subgroup of a Lie group —): III.6.2
left-invariant (field of pointwise distributions —): III.3.6
invariant (section —): III.3.13
Jordan (theorem of —): III.4, exerc. 11
free (Lie algebra —): II.2.2
free (magma —): II.2.1
free ($p$-Lie algebra —): II.3, exerc. 4
Lie (algebra of a Lie group —): III.3.7
Lie (algebra of a Lie group —): III.3.18
Lie (group —): III.1.1
locally isomorphic (Lie groups —): III.1.10
logarithm: II.6.1, III.7.6
infinitesimal operation law: III.3.7, III.3.18
length of an element of a free magma: II.2.1
Magnus (algebra of —): II.5.1
Magnus (group of —): II.5.2
Maurer–Cartan (formulas of —): III.3.14, III.3.18
Möbius (function of —): II.App.
Möbius (inversion formula of —): II.App.
piece of an operation law: III.1.11
morphism of Lie groups: III.1.2
morphism of Lie groups: III.1.10
multigrading of L(I): II.2.6
nilpotent (Lie algebra —): II.27
normable (algebra —): II.7
normalizer: III.9.4
normed (Lie algebra —): II.7, II.8.2
order of an element (in a filtered group —): II.4.2
p-adic (Lie group —): III.1.1, III.8.1
P-integral: II.4, exerc. 14
P-envelope (of a nilpotent group —): II.4, exerc. 15
permutable (elements —): III.9.3
polynomial (mapping —): II.2.4
Lie polynomial: II.2.4
first kind (canonical chart of —): III.4.3
first kind (system of canonical coordinates of —): III.4.3
presentation of a Lie algebra: II.2.3
almost simple (Lie group —): III.9.8
primitive (element of a cogebra —): II.1.2
product (of Lie groups —): III.1.4
tensor product of representations: III.App.
P-saturated (of a subgroup of a nilpotent group —): II.4, exerc. 14
P-torsion (group of —, torsion-free group —): II.4, exerc. 14
t-th power (mapping —): III.4.3
Lie quasi-subgroup: III.1.3
quotient of a Lie group: III.1.6
roots of a solvable Lie algebra: III.9, exerc. 17
radical of a Lie group: III.9.7
real (Lie group —): III.1.1, III.8.1, III.8.2
relations: II.2.3
analytic linear representation of a Lie group: III.1.2
scalar restriction (Lie group derived from a Lie group by —): III.1.1
universal covering of a connected Lie group: III.1.9
section of a vector bundle: III.1.8
semi-direct (product of Lie groups —): III.1.4
semisimple (Lie group —): III.9.8
separated (filtration —): II.4.1 formal Lie series: II.6.3
Lie subgroup: III.1.3
Lie sub-Lie group: III.1.10
standard (group —): III.7.3
descending central series of a Lie algebra: II.2.7
tangent (law of composition —): III.2.1
tangent (Lie subalgebra —): III.4.5
constant term of an element of the Magnus algebra: II.5.2
lower unitriangular (group —): II.4.6
trivial (G-vector bundle —): III.1.8
right (resp. left) trivialization of T(G): III.2.1, III.2.2
type (N) (real Lie group of —): III.9, exerc. 29
unipotent (endomorphism —): III.9.5
u-primitive (element of a cogebra —): II.1.1
CHAPTER II. — FREE LIE ALGEBRAS .......................... 7

§ 1. Enveloping bialgebra of a Lie algebra ..................... 7
    1. Primitive elements of a cogebras ............................ 7
    2. Primitive elements of a bialgebra ............................ 9
    3. Filtered bialgebras ........................................ 10
    4. Enveloping bialgebra of a Lie algebra ................. 10
    5. Structure of the cogebras $U(\mathfrak{g})$ in characteristic 0 .......... 12
    6. Structure of filtered bialgebras in characteristic 0 ........ 15

§ 2. Free Lie algebras ....................................... 17
    1. Reminders on free algebras ............................ 17
    2. Construction of the free Lie algebra ..................... 18
    3. Presentations of a Lie algebra ........................ 19
    4. Lie polynomials and substitutions .......................... 19
    5. Functorial properties ................................... 20
    6. Gradings ................................................ 21
    7. Lower central series .................................. 23
    8. Derivations of free Lie algebras .................... 25
    9. Elimination theorem ..................................... 25
   10. Hall sets in a free magma ...................... 27
   11. Hall bases of a free Lie algebra .................. 30

§ 3. Enveloping algebra of the free Lie algebra ............... 32
    1. Enveloping algebra of $L(X)$ ............................... 32
    2. Projector from $A^+(X)$ onto $L(X)$ .......................... 34
    3. Dimension of the homogeneous components of $L(X)$ ........... 35

§ 4. Central filtrations ........................................ 38
    1. Real filtrations ......................................... 38
    2. Order function ........................................... 38
    3. Graded algebra associated to a filtered algebra ............. 39

4. Filtrations centrales sur un groupe ......................... 40
5. Un exemple de filtration centrale ......................... 42
6. Filtrations centrales entières ............................. 44

§ 5. Magnus algebras ........................................ 45
    1. Magnus algebras ....................................... 45
    2. Magnus group ......................................... 46
    3. Magnus group and free group ....................... 46
    4. Lower central series of a free group .......... 48
    5. $p$-filtration of free groups .................... 50

§ 6. The Hausdorff series ...................................... 51
    1. Exponential and logarithm in filtered algebras .. 51
    2. Hausdorff group ...................................... 52
    3. Formal Lie series .................................. 54
    4. The Hausdorff series .................................... 55
    5. Substitutions in the Hausdorff series ............... 57

§ 7. Convergence of the Hausdorff series (real or complex case) ............. 60
    1. Continuous polynomials with values in $\mathfrak{g}$ ................ 60
    2. Groupoid defined by a complete normed Lie algebra 61
    3. Exponential in complete normed associative algebras 64

§ 8. Convergence of the Hausdorff series (ultrametric case) ............. 66
    1. $p$-adic bounds for the series exp, log and H .......... 66
    2. Normed Lie algebras .................................. 67
    3. Group defined by a complete normed Lie algebra .... 68
    4. Exponential in complete normed associative algebras 69

Appendix. — Möbius function ................................. 71

Exercises from § 1 .................................................. 73
Exercises from § 2 .................................................. 75
Exercises from § 3 .................................................. 79
Exercises from § 4 .................................................. 79
Exercises from § 5 .................................................. 84
Exercises from § 6 .................................................. 90
Exercises from § 7 .................................................. 92
Exercises from § 8 .................................................. 92
Exercises from the Appendix .......................................... 94

CHAPTER III. — LIE GROUPS............................................. 95

§ 1. Lie groups......................................................... 95
    1. Definition of a Lie group................................. 95
    2. Morphisms of Lie groups................................. 99
    3. Lie subgroups............................................ 100
    4. Semi-direct products of Lie groups..................... 101
    5. Quotient of a manifold by a Lie group............... 103
    6. Homogeneous spaces and quotient groups..................... 105
    7. Orbits.......................................................... 108
    8. Vector bundles with operators............................... 109
    9. Local definition of a Lie group......................... 112
   10. Groupoids.................................................. 114
   11. Pieces of operation laws................................. 118

§ 2. Group of tangent vectors to a Lie group.................. 120
    1. Tangent composition laws................................. 120
    2. Group of tangent vectors to a Lie group............. 122
    3. Case of groupoids.......................................... 124

§ 3. Passage from a Lie group to its Lie algebra.................. 125
    1. Convolution of punctual distributions on a Lie group 125
    2. Functorial properties..................................... 127
    3. Case of a group operating on a manifold.................... 130
    4. Convolution of punctual distributions and functions... 131
    5. Fields of punctual distributions defined by the action of a group on a manifold............................................. 135
    6. Invariant fields of punctual distributions on a Lie group......................................................... 136
    7. Lie algebra of a Lie group............................ 138
    8. Functorial properties of the Lie algebra................ 141
    9. Lie algebra of the group of invertible elements of an algebra............................................................. 143
   10. Lie algebras of certain linear groups................ 144
   11. Linear representations.................................... 147
   12. Adjoint representation....................................... 151
   13. Invariant tensors and forms............................... 155
   14. Maurer–Cartan formulas................................... 156
   15. Construction of invariant differential forms.......... 158
   16. Haar measure on a Lie group........................ 159
   17. Left differential......................................... 162
   18. Lie algebra of a Lie group chunk..................... 163

§ 4. Passage from Lie algebras to Lie groups ......................... 166
    1. Passage from Lie algebra morphisms to Lie group morphisms ............................................. 166
    2. Passage from Lie algebras to Lie groups ............... 168
    3. Exponential mappings ............................................. 171
    4. Functoriality of exponential mappings .................... 175
    5. Induced structure on a subgroup ............................. 176
    6. Primitives of differential forms with values in a Lie algebra .................................................. 178
    7. Passage from infinitesimal operation laws to operation laws ......................................................... 182

§ 5. Formal calculations in Lie groups ................................. 184
    1. The coefficients c_{αβγ} .................................................. 185
    2. Bracket in the Lie algebra .......................................... 186
    3. Powers ................................................................. 187
    4. Exponential .............................................................. 190

§ 6. Real or complex Lie groups ........................................ 192
    1. Passage from Lie algebra morphisms to Lie group morphisms ............................................. 192
    2. Integral subgroups .................................................. 193
    3. Passage from Lie algebras to Lie groups ............... 198
    4. Exponential mapping ............................................... 199
    5. Application to linear representations ......................... 203
    6. Normal integral subgroups ................................. 204
    7. Primitives of differential forms with values in a Lie algebra .................................................. 206
    8. Passage from infinitesimal operation laws to operation laws ......................................................... 206
    9. Exponential mapping in the linear group ............... 208
   10. Complexification of a real finite-dimensional Lie group 210

§ 7. Lie groups over an ultrametric field ............................. 214
    1. Passage from Lie algebras to Lie groups ............... 214
    2. Exponential mappings ............................................. 216
    3. Standard groups ....................................................... 216
    4. Filtration of standard groups ..................................... 218
    5. Powers in standard groups ............................. 219
    6. Logarithm mapping .................................................. 221

§ 8. Lie groups over R or Q_p .................................................. 225
    1. Continuous morphisms ..................................................... 225
    2. Closed subgroups ..................................................... 227

§ 9. Commutators, centralizers, normalizers in a Lie group .... 230
    1. Commutators in a topological group ......................... 230
    2. Commutators in a Lie group ............................... 231
    3. Centralizers ....................................................... 233
    4. Normalizers ....................................................... 234
    5. Nilpotent Lie groups ............................................ 235
    6. Solvable Lie groups ........................................... 240
    7. Radical of a Lie group .......................................... 241
    8. Semisimple Lie groups ......................................... 242

§ 10. The automorphism group of a Lie group .................. 247
    1. Infinitesimal automorphisms ...................................... 247
    2. The automorphism group of a Lie group (real or complex case) ................................................................. 250
    3. The automorphism group of a Lie group (ultrametric case) ................................................................. 255

Appendix. — Operations on linear representations ............. 256

Exercises of § 1 ........................................................................ 257
Exercises of § 3 ........................................................................ 258
Exercises of § 4 ........................................................................ 261
Exercises of § 5 ........................................................................ 265
Exercises of § 6 ........................................................................ 266
Exercises of § 7 ........................................................................ 272
Exercises of § 8 ........................................................................ 275
Exercises of § 9 ........................................................................ 276
Exercises of § 10 ...................................................................... 284

Historical note (Chapter I to III) ............................................... 286

Bibliography ........................................................................... 306

Index of notations ............................................................... 309

Terminological index ............................................................ 312
