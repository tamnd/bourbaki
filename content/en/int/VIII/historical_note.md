---
book: int
book_title: Integration
chapter: VIII
chapter_title: CONVOLUTION AND REPRESENTATIONS
section: 0
section_title: Historical Note
kind: historical
lang: en
source: int-vii-ix
pdf_pages: 0175-0182
extraction: ocr
statements: 0
exercises: 0
content_sha256: 8310a10c50a658cc062070acbfc343e395a3fba746d5379e0f041cac27733c15
---

# HISTORICAL NOTE

(Chapters VII and VIII)

(N.B. — The Roman numerals refer to the bibliography at the end of this note.)

The concepts of length, area and volume are, with the Greeks, essentially based on their invariance under displacements: « Things that coincide (εφαρμόξοντα) are equal » (Eucl. El., Book I, ‘Common notion’ 4); and it is by an ingenious use of this principle that all of the formulas giving the areas or volumes of the classical ‘figures’ (polygons, conic sections, polyhedra, spheres, etc.) are obtained, sometimes by methods of finite decomposition, sometimes by ‘exhaustion’ (*). In modern language, one can say that what the Greek geometers did was to prove the existence of ‘set functions’, additive and invariant under displacements, but defined only for sets of a very special type. The integral calculus may be regarded as responding to the need for enlarging the domain of definition of these set functions, and, from Cavalieri to H. Lebesgue, it is this preoccupation that was to be at the forefront of the research of analysts; as for the property of invariance under displacements, it passed to a secondary status, having become a trivial consequence of the general formula for change of variables in double or triple integrals and the fact that an orthogonal transformation has determinant equal to $\pm 1$. Even in non-euclidean geometries (though the group of displacements is different there), the point of view remains the same: in a general way, Riemann de-

(*) It can be shown that if two plane polygons P, P' have the same area, there are two polygons R ⊃ P, R' ⊃ P' each of which can be decomposed into a finite number of polygons R_i (resp. R'_i) (1 ≤ i ≤ m) without common interior point, such that R_i and R'_i can be deduced from each other by means of a displacement (depending on i) and such that R (resp. R') is the union of a finite family of polygons S_j (resp. S'_j) (0 ≤ j ≤ n), without common interior point, with S_0 = P, S'_0 = P', and S'_j obtainable from S_j by a displacement for 1 ≤ j ≤ n. However, M. DEHN proved (Ueber den Rauminhalt, Math. Ann., 55 (1902), 465–478) that this property is no longer valid for the volume of polyhedra, and that the exhaustion methods employed from EUDOXUS onward were therefore unavoidable.

fined the infinitesimal elements of area or volume (or their analogues for dimensions $\geqslant 3$) beginning with a $ds^2$ by the classical euclidean formulas, and their invariance under the transformations that leave the $ds^2$ invariant is therefore almost a tautology.

It is only around 1890 that there appeared other, less immediate extensions of the concept of measure invariant under a group, with the development of the theory of *integral invariants*, notably by H. Poincaré and E. Cartan; H. Poincaré considered only one-parameter groups operating in a portion of space, whereas E. Cartan was above all interested in groups of displacements, but operating in spaces other than the one where they are defined. For example, he thus determined among other things (II) the invariant (under the group of displacements) measure on the space of lines of $\mathbf{R}^2$ or of $\mathbf{R}^3$ (*); moreover, he noted that in a general way the integral invariants for a Lie group are none other than particular differential invariants and that it is therefore possible to determine them all by the methods of Lie. However, it does not seem that anyone had thought of considering nor of using an invariant measure on the group itself, prior to the fundamental work of A. Hurwitz in 1897 (V). Seeking to form polynomials (on $\mathbf{R}^n$) invariant under the orthogonal group, Hurwitz starts from the remark that for a finite group of linear transformations, the problem is immediately solved by taking the *average* of the transforms $s \cdot \mathrm{P}$ of any polynomial P by all of the elements $s$ of the group, which gave him the idea, for the orthogonal group, of replacing the average by an integral with respect to an invariant measure; he gave explicitly the expression of the latter with the help of the parametric representation by means of the Euler angles, but immediately observed (independently of E. Cartan) that the methods of Lie yielded the existence of an invariant measure for every Lie group. Perhaps due to the decline of invariant theory at the beginning of the 20th century, Hurwitz's ideas received scarcely any immediate echo, and were not exploited until 1924 onward, with the extension to compact groups, by I. Schur and H. Weyl, of the classical theory of Frobenius on the linear representations of finite groups. The former restricted himself to the case of the orthogonal group, and showed how Hurwitz's method permitted extending the classical orthogonality relations of the characters, an idea that H. Weyl combined with the work of E. Cartan on semi-simple Lie algebras, to obtain explicit expressions for the characters of the irreducible representations of compact Lie groups and the theorem on complete reducibility (XI *a*)), then, by a bold extension of the concept of 'regular representation', the celebrated Peter-Weyl theorem, a perfect analogue of the decomposition of the regular representation into its

(*) The invariant measure on the space of lines of the plane had already been essentially determined in connection with problems in 'geometric probability', notably by CROFTON, whose works were probably not known to E. CARTAN at the time.

irreducible components in the theory of finite groups (XI, b)).

A year earlier, O. Schreier had founded the general theory of topological groups, and from then on it was clear that the arguments in the Peter–Weyl memoir would remain valid unchanged for every topological group on which an 'invariant measure' could be defined. Actually, the general concepts of topology and measure were at the time still in rapid development, and neither the category of topological groups on which one could hope to define an invariant measure, nor the sets for which this 'measure' was to be defined, seemed to be clearly delineated. The only obvious point was that one could not hope to extend to the general case the infinitesimal methods proving the existence of an invariant measure on a Lie group. Now, another current of ideas, growing out of work on Lebesgue measure, led precisely to more direct methods of attack. Hausdorff had proved, in 1914, that there does not exist an additive set function, not identically zero, that is defined for $\textbf{all}$ subsets of $\mathbf{R}^3$ and is invariant under displacements, and it was natural to investigate whether this result was also valid for $\mathbf{R}$ and $\mathbf{R}^2$: a problem that was solved by S. Banach in 1923 in a surprising way, by showing that, on the contrary, such a 'measure' did indeed exist (I); his method, highly ingenious, already rested on a construction by transfinite induction and on the consideration of the 'means' $\frac{1}{n} \sum_{k=1}^n f(x + \alpha_k)$ of the translates of a function by elements of the group (*). It was analogous ideas that enabled A. Haar, in 1933 (IV), to take the decisive step, by proving the existence of an invariant measure for locally compact groups with a countable base for open sets: guided by the method of approximating a volume, in classical integral Calculus, by a juxtaposition of arbitrarily small congruent cubes, he obtained, with the aid of the diagonal method, the invariant measure as a limit of a sequence of 'approximate measures', a procedure which is essentially the one we have used in Ch. VII, §1. This discovery had a very great impact, in particular because it immediately allowed J. von Neumann to solve, for compact groups, the famous "5th problem" of Hilbert on the characterization of Lie groups by purely topological properties (excluding all differential structure given in advance). However, it was immediately perceived that to make efficient use of the invariant measure, it was necessary to know not only its existence, but to also know that it was unique up to a constant factor; this point was first proved by J. von Neumann for compact groups, using a method of defining Haar measure via 'means' of continuous functions, analogous to those of Banach (VII a)); then J. von Neumann

(*) J. von NEUMANN showed, in 1929, that the underlying reason for the difference in behavior between $\mathbf{R}$ and $\mathbf{R}^2$ on the one hand, and the $\mathbf{R}^n$ for $n \geq 3$ on the other, was to be found in the commutativity of the group of rotations of the space $\mathbf{R}^2$.

(VII b)) and A. Weil (X), by different methods, simultaneously obtained uniqueness for the case of locally compact groups, with A. Weil indicating at the same time how Haar’s method could be extended to general locally compact groups. It was also A. Weil (loc. cit.) who obtained the condition for the existence of a relatively invariant measure on a homogeneous space, and showed, finally, that the existence of a ‘measure’ (endowed with reasonable properties) on a Hausdorff topological group, implied ipso facto that the group is locally precompact. This work essentially completed the general theory of Haar measure; the only recent addition to be cited is the concept of quasi-invariant measure, which was scarcely identified before around 1950, in connection with the theory of representations of locally compact groups in Hilbert spaces.

The history of the convolution product is more complex. From the beginning of the 19th century, it was observed that if, for example, F(x, t) is a solution of a partial differential equation in x and t, linear and with constant coefficients, then

$$
\int_{-\infty}^{+\infty} F(x - s, t) f(s) \, ds
$$

is also a solution of the same equation; since before 1820, Poisson, among others, had used this idea to write the solutions of the heat equation in the form

(1)
$$
\int_{-\infty}^{+\infty} \exp \left( - \frac{(x - s)^2}{4t} \right) f(s) \, ds.
$$

A little later, the expression

(2)
$$
\frac{1}{2\pi} \int_{-\pi}^{+\pi} \frac{\sin \frac{2n+1}{2}(x-t)}{\sin \frac{x-t}{2}} f(t) \, dt
$$

for the partial sum of a Fourier series, and the study, by Dirichlet, of the limit of this integral as n tends to $+\infty$, provided the first example of a ‘regularization’ $f \mapsto \rho_n * f$ on the torus $\mathbf{T}$ (actually, by a sequence of non-positive ‘kernels’, which greatly complicates the study); under the name of ‘singular integrals’, the analogous integral expressions were a subject of choice among analysts at the end of the 19th century and the beginning of the 20th, from P. du Bois-Reymond to H. Lebesgue. On $\mathbf{R}$, Weierstrass made use of the integral (1) in the proof of his theorem on approximation by polynomials, and gave in this connection the general principle of regularization by a sequence of positive ‘kernels’ $\rho_n$ of the form $x \mapsto c_n \rho(x/n)$. On $\mathbf{T}$, the most famous example of regularization by positive kernels was given a little later by Fejér, and from this moment on, it is the standard procedure that was to be the basis of most of the 'summation methods' for series of functions.

However, these works, due to the dissymmetry of the roles played by the 'kernel' and the function regularized, scarcely revealed the algebraic properties of the convolution product. We are indebted above all to Volterra for having placed the emphasis on this point. He made a general study of the 'composition' $F * G$ of two functions of two variables

$$
(F * G)(x, y) = \int_x^y F(x, t)G(t, y)\, dt,
$$

which he viewed as a generalization, 'by passage from finite to infinite', of the product of two matrices (IX). Very early he singled out the case (called 'of closed cycle' because of its interpretation in the theory of heredity) where F and G depend only on $y - x$; the same is then true of $H = F * G$, and if one sets $F(x, y) = f(y - x)$, $G(x, y) = g(y - x)$, then

$$
H(x, y) = h(y - x),
$$

where

$$
h(t) = \int_0^t f(t - s)g(s)\, ds,
$$

so that, for $t \geq 0$, $h$ coincides with the convolution of the functions $f_1, g_1$ equal, respectively, to $f$ and $g$ when $t \geq 0$, and to 0 when $t < 0$.

Nevertheless, the algebraic formalism developed by Volterra did not reveal the connections with the group structure of $\mathbf{R}$ and the Fourier transformation. This is not the place to relate the history of the latter; but it is appropriate to note that from Cauchy on, the analysts who treated the Fourier integral devoted themselves above all to finding ever wider conditions for the validity of various 'inversion' formulas, and somewhat neglected its algebraic properties. One could certainly not say the same regarding this of the works of Fourier himself (or of those of Laplace on the analogous integral $\int_0^{+\infty} e^{-st} f(t)\, dt$); but these transformations had been introduced essentially in connection with linear problems, and it is therefore not very surprising that it was a long time before anyone thought of considering the product of two Fourier transforms (with exception made for products of trigonometric series or of power series, but the connection with the convolution of discrete measures obviously could not have been perceived in the 19th century). The first mention of this product and of convolution over $\mathbf{R}$ is probably to be found in a memoir of Tchebychef (VIII), in connection with questions in probability theory. In fact, in this theory the convolution $\mu * \nu$ of two 'laws of probability' on $\mathbf{R}$ (positive measures of total mass 1 ) is none other than the 'composed' probability law of $\mu$ and $\nu$ (for the addition of the corresponding 'random variables'). To be sure, for Tchebychef it is still only a question of the convolution of probability laws having a density (with respect to Lebesgue measure), hence of the convolution of functions; moreover, it only comes up in his work in an episodic way, and it was to be so in the several rare works in which it appeared before the period 1920–1930. In 1920, P. J. Daniell, in a note (III) little noticed at the time, defined the convolution of two arbitrary measures on $\mathbf{R}$ and the Fourier transform of such a measure, and observed explicitly that the Fourier transform carried convolution over to an ordinary product—a formalism that, from 1925 on, was to be used intensively by probabilists, especially following P. Lévy. But the fundamental importance of convolution in the theory of groups was only fully recognized by H. Weyl in 1927; he noticed that for a compact group, the convolution of functions plays the role of multiplication in the algebra of a finite group, allowing him to subsequently define the 'regular representation'; at the same time, he found in regularization the equivalent of the unity element of the algebra of a finite group. It remained to make the synthesis of all of these points of view, accomplished in the book of A. Weil (X), preparing the way for the later generalizations which were to constitute, on the one hand I. Gelfand's theory of normed algebras, and on the other the convolution of distributions.

Haar measure and convolution have rapidly become essential tools in the tendency towards algebraization that so strongly marks modern Analysis; we shall have occasion to develop numerous applications of them in later Books. The only one that we have treated in these chapters concerns the 'variation' of the closed subgroups (and notably of the discrete subgroups) of a locally compact group. This theory, starting from a result of K. Mahler in the Geometry of numbers, was inaugurated in 1950 by C. Chabauty, and has just been considerably developed and deepened by Macbeath and Swierczkowski (VII), whose principal results we have reproduced here.

(I) S. Banach, Sur le problème de la mesure, Fund. Math., 4 (1923), pp. 7–33.

(II) E. Cartan, Le principe de dualité et certaines intégrales multiples de l’espace tangentiel et de l’espace réglé, Bull. Soc. Math. France, 24 (1896), pp. 140–177 (= Œuvres complètes, v. II₁, pp. 265–302).

(III) P. J. Daniell, Stieltjes–Volterra products, Congr. Intern. des Math., Strasbourg, 1920, pp. 130–136.

(IV) A. Haar, Der Massbegriff in der Theorie der kontinuierlichen Gruppen, Ann. of Math., (2), 34 (1933), pp. 147–169 (= Gesammelte Arbeiten, pp. 600–622).

(V) A. Hurwitz, Ueber die Erzeugung der Invarianten durch Integration, Gött. Nachr., 1897, pp. 71–90 (= Math. Werke, v. II, pp. 546–564).

(VI) A. M. Macbeath, S. Swierczkowski, Limits of lattices in a compactly generated group, Canad. J. Math., 12 (1960), pp. 427–437.

(VII) J. von Neumann, a) Zum Haarschen Mass in topologischen Gruppen, Comp. Math., 1 (1934), pp. 106–114 (= Collected Works, v. II, n° 22); b) The uniqueness of Haar’s measure, Mat. Sbornik, 1 (43) (1936), pp. 721–734 (= Collected Works, v. IV, n° 6).

(VIII) P. Tchebychef, Sur deux théorèmes relatifs aux probabilités, Acta. Math., 14 (1890), pp. 305–315) (= Œuvres, v. II, pp. 481–491).

(IX) V. Volterra, Leçons sur les fonctions de lignes, Paris (Gauthier-Villars), 1913.

(X) A. Weil, L’intégration dans les groupes topologiques et ses applications, Actual. Scient. et Ind., n° 869, Paris, Hermann, 1940 (2e éd., ibid., n° 869-1145, Paris, Hermann, 1953).

(XI) H. Weyl, a) Theorie des Darstellung kontinuierlicher halbeinfacher Gruppen durch lineare Transformationen, Math. Zeit., 23 (1925), pp. 271–309, 24 (1926), pp. 328–395 and 789–791 (= Selecta, Basel–Stuttgart (Birkhäuser), 1956, pp. 262–366); b) (with F. Peter) Die Vollständigkeit der primitiven Darstellungen einer geschlossenen kontinuierlichen Gruppe, Math. Ann., 97 (1927), pp. 737–755 (= Selecta, pp. 387–404).
