---
book: alg
book_title: Algebra
chapter: VII
chapter_title: MODULES OVER PRINCIPAL IDEAL DOMAINS
section: 0
section_title: Historical Note
kind: historical
lang: en
source: alg-iv-vii
source_edition: 2003, Springer
pdf_pages: 0432-0460
extraction: ocr
statements: 0
exercises: 0
content_sha256: 0badcac98496c7f98609a5c39885b447949598116e8182f2d00bd1c60192a86d
---

# HISTORICAL NOTE

(Chapters VI and VII)

(N.B. — Roman numerals in parentheses refer to the bibliography at the end of this note.)

Elementary arithmetical operations, in particular operations with fractions, inevitably lead to a number of empirical observations about divisibility between integers. But neither the Babylonians (although they were such experts in algebra), nor the Egyptians (despite their acrobatic skill at manipulating fractions) seem to have been acquainted with the general rules governing these properties, and the initiative in this respect is due to the Greeks. Their arithmetical work, a masterly exposition of which can be found in Books VII and IX of Euclid (I), is in no way inferior to their most beautiful discoveries in other branches of Mathematics. The existence of the gcd of two integers is proved right at the beginning of Book VII by the procedure known as the « Euclidean algorithm » \* ; it serves as the basis for all the subsequent developments (properties of prime numbers, existence and calculation of Icm, etc.), based on arguments not substantially different from those in Chap. VI, 9 1 above ; and the crowning glory is formed by the two remarkable theorems proving the existence of infinity of prime numbers (Book IX, Prop. 20) and giving a procedure for constructing even perfect numbers (cf. VII, p. 53, Ex. 24 ; this procedure in fact gives all the even perfect numbers, as would be proved by Euler). It is only the existence and uniqueness of prime factorisation that is not proved in a general manner ; however Euclid does prove explicitly that every integer is divisible by a prime number (Book VII, Prop. 31), as well as the following two propositions (Book IX, Prop. 13 and 14) :

« If as many numbers as we like are in a progression, beginning with 1, with constant ratio [i.e. geometric], and if the number following 1 is prime, then the

\* If $a_1$ and $a_2$ are two integers, such that $a_1 \geq a_2$, one defines $a_n$ (for $n \geq 3$) recursively as the remainder on dividing $a_{n-2}$ by $a_{n-1}$; if $m$ is the smallest index such that $a_m = 0$, then $a_1$, $a_2$, is the gcd of $a_1$ and $a_2$. This is the transposition into the integers of the method of successive subtractions (sometimes also called ἀνθυφαιρεσις) for finding a common measure for two lengths. The latter no doubt goes back to the Pythagoreans, and seems to have been the basis of a pre-Eudoxean theory of irrational numbers.

largest number will not be divisible by any number except those appearing in the progression » (in other words, a power $p^n$ of a prime number $p$ can be divisible only by powers of $p$ of exponent $\leq n$).

« If a number is the smallest which is divisible by [given] prime numbers, it will not be divisible by any other prime number with the exception of those initially [given as] dividing it » (in other words, a product of distinct primes $p_1, \ldots, p_k$ has no prime factor other than $p_1, \ldots, p_k$).

Thus it seems that if Euclid does not state the general theorem, it is only for want of an adequate terminology and notation for arbitrary powers of an integer.*

Although a careful study makes it seem likely that Euclid's text is made up of several successive layers, each corresponding to a stage in the development of Arithmetic **, it seems that this evolution took place entirely between the beginning of the 5th and the middle of the 4th centuries B.C., and one must admire the skill and the logical confidence which it represents: the next comparable progress made in Arithmetic would not occur for two millenia.

It was the so-called « indeterminate » or « Diophantine » problems which were at the root of subsequent developments in Number Theory. The term « Diophantine equations », as it is used today, is not entirely justified historically; it is generally understood to mean polynomial equations (or systems of equations) with integer coefficients, for which only integer solutions are sought: a problem which is usually impossible if the equations are « determinate », that is have only finitely many (real or complex) solutions, but which on the other hand often admits solutions when there are more unknowns than equations. Now, while Diophantus does indeed seem to have been the first to consider « indeterminate » problems, he looks for integer solutions only in exceptional cases, and is usually content to find a single solution in the rational numbers (II). That was a type of problem which he was usually able to solve by algebraic calculations, where the

\* In support of this thesis, one can also remark that the proof of the theorem on perfect numbers is basically just another special case of the unique prime factorisation theorem. Moreover, all the evidence shows that from this period onwards the factorisation of an explicit number into primes was well known and in current use; but no complete proof of the factorisation theorem is to be found before that given by Gauss at the beginning of the Disquisitiones ((VIII) t. I, p. 15).

** Cf. B. L. van der Waerden, Die Arithmetik der Pythagoreer, Math. Ann., vol. CXX (1947-49), p. 127. An example of a passage left over from a previous version is provided by Prop. 21 to 34 of Book IX, which deals with the most elementary properties of divisibility by 2, and no doubt goes back to a period when the general theory of prime numbers had not been developed. Moreover, it is known that the categories Even and Odd played a major rôle in the metaphysical speculations of the early Pythagoreans, to whom it is naturally tempting to attribute this segment.

arithmetical nature of the unknowns was not relevant *; also the theory of divisibility plays only a minor rôle (the word for prime number is used only once ((11), Book V, problem 9, vol. 1, pp. 334-335), and the notion of coprime numbers is invoked only in connection with the theorem which asserts that the quotient of two coprime numbers can be a square only if each of them is a square) **.

The study of integer solutions of indeterminate equations only begins properly with the Chinese and Hindu mathematicians of the early middle ages. The former seem to have been led to considerations of this nature by the practical problems of drawing up calendars (where the determination of the common periods of various cycles of astronomical phenomena constitutes precisely a linear « Diophantine » problem); at any rate they were responsible (certainly between the 4th and the 7th century A.D.) for a rule for solving simultaneous linear congruences (cf. VI, p. 33, Ex. 25). As for the Hindus, whose Mathematics flourished between the 5th and the 13th centuries, not only did they know how to deal methodically (by applying the Euclidean algorithm) with systems of linear Diophantine equations in arbitrarily many unknowns ***. but they were the first to attack and solve quadratic problems, among them certain special cases of « Fermat's equation » Nx^2 + 1 = y^2 ((111), vol. II, pp. 87-307).

This is not the place for us to pursue the history of the theory of Diophantine equations of degree > 1, which, by way of the work of Fermat, Euler, Lagrange and Gauss, was to lead to the theory of algebraic integers in the 19th century. As we have already noted (cf. Historical Note to Chap. II and 111), the study of linear systems, which no longer seemed to present problems worthy of interest, was rather neglected during this period: in particular there was no search for general existence conditions for an arbitrary system, nor for a description of the set of solutions. Nevertheless Hermite, in his Number-theoretical research in the 19th

\* While Diophantus' work on indeterminate problems is always reduced to problems in a single unknown, via a numerical choice of the other unknowns in such a way as to make a solution to his final equation possible, it seems that the main reason for using this method was his notation, which did not allow him to calculate with several unknowns at once; in any case he keeps track of the numerical substitutions he has made throughout the calculation, and modifies them later if need be, by writing down a compatibility condition for the substituted variables, and solving this auxiliary problem first. In other words, he handles these substituted numerical values like we handle parameters, so much so that what he actually does amounts to finding a rational parametric representation of a given algebraic variety, or of a subvariety of it (cf. (II bis)).

** Various indications, however, point to more advanced arithmetical knowledge in Diophantus: he knew for example that the equation x^2 - y^2 = n has no rational solutions if n is an integer of the form 4k + 3 (Book V, problem 9 and Book VI, problem 14 ((II), vol. 1, pp. 332-335 and p. 425; cf. also (II bis), pp. 105-110)).

*** Astronomical problems were also among those which led the Hindus to consider this type of equation (cf. (III), vol. II, pp. 100, 117 and 135).

century, was led to make use of several Lemmas on linear Diophantine equations, notably a « reduced form » for a linear transformation with integer coefficients ((XIII), pp. 164 and 265); finally, after Heger in 1858 had given the existence condition for a system whose rank is equal to the number of equations, H. J. Smith in 1861 defined the invariant factors of an integer matrix, and obtained the general theorem that such a matrix reduces to the « normal form » which we gave in VII, p. 22, Cor. 1 (XVII).

But meanwhile, following its introduction by Gauss (cf. Historical Notes to Chap. I, II and III), and the important part it played in the subsequent development of Number Theory, the notion of an abelian group was gradually being made precise. In his particularly deep study, presented in the Disquisitiones, of the finite abelian group of classes of quadratic forms of a given discriminant, Gauss soon realised that certain of these groups are not cyclic: « in this case, » he says, « one basis [that is to say, one generator] cannot suffice, it is necessary to take two or a greater number which, through multiplication and composition*, can produce all the classes » ((VIII), vol. I, pp. 374-375). It is not certain that Gauss intended these words to describe the decomposition of the group as a direct product of cyclic groups; nevertheless, in the same article of the Disquisitiones, he proves that there exists an element in the group whose order is the lcm of the orders of all the elements — in other words he obtains the existence of the largest invariant factor of the group ((VIII), vol. 1, p. 373); and on the other hand, the notion of direct product was known to him, for, in a manuscript dating from 1801, but not published during his lifetime, he sketches a general proof of the decomposition of a finite abelian group into a direct product of p-groups** ((VIII), vol. II, p. 226). In any case, in 1868 Schering, the editor of Gauss' collected works, inspired by these results (notably by this manuscript which he had just found), proved (still for the group of classes of quadratic forms) the general decomposition theorem (XVIII) by a method which, as repeated in abstract terms two years later by Kronecker (XX), is essentially that which we have used above (VII, p. 18, Th. 1). As for torsion-free abelian groups, we have already said (cf. Historical Note to Chap. II and III) how the theory of elliptic functions and abelian integrals, developed by Gauss, Abel and Jacobi, gradually led to attention being paid to their structure; the first and best known example of a decomposition of an infinite group into a direct sum of cyclic groups was given in 1846 by Dirichlet in his paper on the units of an algebraic number field (XI). But it was not until 1879 that the connection between the theory of finitely generated abelian groups and Smith's theorem was recognised and explicitly used by Frobenius and Stickelberger ((XXIII), § 10).

\* Gauss uses additive notation for the law of composition of classes, thus by « multiplication » he means the product of a class by an integer.
** Abel also proved this property en passant in his note on abelian equations ((IX), vol. I, pp. 494-497).

Around the same period the theory of similarity of matrices (with real or complex entries) was also reaching completion. The notion of an eigenvalue of a linear transformation appeared explicitly in the theory of systems of linear differential equations with constant coefficients, applied by Lagrange (VIa) to the theory of small oscillations and by Lagrange (VIb) and Laplace (VIIa) to the « secular » perturbations of the planets. It is implicit in many other problems which were also attacked around the middle of the 18th century, such as that of finding the axes of a conic or a quadric (first solved by Euler (Va)), or the study (also developed by Euler (Vb)) of the principal axes of inertia of a solid body (discovered by De Segner in 1755); we know now that it is also involved (in a more disguised form) in the beginnings of the theory of partial differential equations, in particular the equation of a vibrating string. But (leaving this last case aside) the relationship between these various problems was barely recognised before Cauchy (X). Moreover, as most of them involve the use of symmetric matrices, it was principally because of the latter that eigenvalues were initially studied; we will return to this point in more detail in the Historical Notes following the chapters of this treatise devoted to hermitian operators; let us simply note here that, as early as 1826, Cauchy proved the invariance of the eigenvalues of such matrices under similarity, and proved that they are real for a $3 \times 3$ symmetric matrix (Xa), a result which he generalised three years later (Xb) to arbitrary real symmetric matrices.* The general notion of a projection, introduced by Mobius in 1827, rapidly led to the problem of classifying such transformations (in 2 and 3 dimensions first of all), which is nothing other than the problem of classifying the corresponding matrices up to similarity; but for a long time this question was treated only by the « synthetic » methods which were in vogue in the mid 19th century, and its (in any case rather slow) progress does not seem to have affected the theory of eigenvalues in any way. The same is not true of another geometric question, the classification of « pencils » of conics or quadrics, which from the modern point of view amounts to the study of the elementary divisors of the matrix $U + \lambda V$, where $U$ and $V$ are two symmetric matrices; it was certainly in this spirit that Sylvester attacked this problem in 1851, carefully examining (in order to find « canonical forms » for the pencil under consideration) what happens to the minors of the matrix $U + \lambda V$ when a value for $\lambda$ is substituted which annihilates the determinant (XIV). The purely algebraic aspect of the theory of eigenvalues was progressing simultaneously; so it was that several authors (including Sylvester himself) proved around 1850 that the eigenvalues of $U^n$ are the n-th powers of the eigenvalues of $U$, while Cayley

\* An attempt to prove this result in the particular case of the « secular » perturbations of the planets had previously been made by Laplace (VIIb) in 1784. As for the third degree equation giving the axes of a real quadric, Euler had stated without proof that it has real roots, and an attempted proof by Lagrange in 1773 (VIe) was incomplete; this point was first proved rigourously by Hachette and Poisson in 1801 (Journal de l'École Polytechnique, cahier 11 (year X), pp. 170-172).

announced in 1858, in the paper in which he introduced matrix arithmetic (XVI), the « Cayley-Hamilton Theorem » for an arbitrary square matrix *, though he contented himself with a direct proof for 2 x 2 and 3 x 3 matrices. Finally Weierstrass in 1868, using Sylvester's methods, obtained « canonical forms » for a « pencil » $U + XV$ where this time $U$ and V are square matrices, not necessarily symmetric, subject only to the condition that $\det(U + XV)$ not be identically zero; he deduced from that the definition of the elementary divisors of an arbitrary square (complex) matrix, and proved that they characterise the latter up to similarity (XIX); these results, incidentally, were partially (and apparently independently) recovered by Jordan two years later ** (XXI). Here again it was Frobenius who showed in 1879 that Weierstrass' theorem can easily be deduced from Smith's theorem extended to polynomials ((XXII), § 13); his procedure is the basis of the proof of this theorem which we have given above (VII, p. 35).

We have just referred to the theory of divisibility for polynomials in one variable; the question of division of polynomials must naturally have arisen in the earliest days of algebra, as the inverse operation to multiplication (the latter being known even to Diophantus, at least for polynomials of low degrees); but one can imagine that it is barely possible to attack this problem in a general fashion before a coherent notation for the various powers of the variable has been established. In fact we find very few examples of the « Euclidean » division procedure for polynomials, as we know it, before the middle of the 16th century ***; and S. Stevin (essentially, using exponent notation) seems to have been the first to have had the idea of deducing the extension of the « Euclidean algorithm » to find the gcd of two polynomials ((IV, vol. I, pp. 54-56). Apart from that, the theory of divisibility had been restricted to the rational integers until the mid 18th century. It was Euler in 1770 who began a new chapter in Arithmetic by somewhat rashly extending the notion of divisibility to the integers of a quadratic extension: seeking to determine the divisors of a number of the form $x^2 + cy^2$ (x, y and c rational integers), he put

$$
x - y \sqrt{-c} = (p + q \sqrt{-c})(r + s \sqrt{-c}) \quad (p, q, r, s \text{ rational integers})
$$

and, taking norms of each side, he had no hesitation in asserting that all the divisors of $x^2 + cy^2$ are obtained in this way as $p^2 + cq^2$ (Vc). In other words,

\* Hamilton, incidently, had proved this theorem for 3 x 3 matrices some years previously ((XV), pp. 566-567).

** Jordan did not mention the invariance of the normal form which he obtained. It is interesting to note as an aside that he dealt with the problem not for complex matrices, but for matrices over a finite field. On the other hand, let us point out that Grassmann had given a method for reducing a (complex) matrix to triangular form as early as 1862, and explicitly mentioned the connection between this reduction and the classification of projections (Ges. Math. Werke, vol. I2, Leipzig (Teubner), 1896, pp. 249-254).

*** Cf. for example H. Bosmans, Sur le « libro del Algebra » de Pedro Nuñez, Bibl. Math. (3), vol. VIII (1907-1908), pp. 154-169.

Euler argued as if the ring $\mathbf{Z}[\sqrt{-c}]$ were a principal ideal domain; a little later he used an analogous argument to apply the method of « infinite descent » to the equation $x^3 + y^3 = z^3$ (he reduced the problem to that of finding a cube root of $p^2 + 3q^2$, which he does by putting $p + q \sqrt{-3} = (r + s \sqrt{-3})^3$). But Lagrange proved as early as 1773 (VIc) that the divisors of numbers of the form $x^2 + cy^2$ are not all of this form, the first example of the fundamental difficulty which was to appear much more clearly in the studies of Gauss and his successors into divisibility in cyclotomic fields *; it is not possible, in general, to extend the essential properties of divisibility of rational integers, such as the existence of gcd's and the uniqueness of prime factorisation, directly to these fields. This is not the place to describe how Kummer, for cyclotomic fields (XII)**, and then Dedekind and Kronecker for arbitrary algebraic number fields, succeeded in overcoming this formidable obstacle by the invention of ideal theory, one of the most decisive advances of modern algebra. But Dedekind, ever curious about the foundations of various Mathematical theories, was not content with this success; and by analysing the mechanism of the divisibility relations he laid the foundations of the theory of lattice ordered groups, in a paper (unknown to his contemporaries, and lost in obscurity for 30 years) which is without doubt one of the earliest works of axiomatic Algebra (XXIV); modulo notation, his work was very close to the modern form of this theory, as we have presented it in Chap. VI, 91.

\* Gauss seems to have hoped at one time that the ring of integers in the field of n-th roots of unity would be a principal ideal domain; in a manuscript unpublished in his lifetime ((VIII), vol. II, pp. 387-397), he proves the existence of a Euclidean division process in the field of cube roots of unity, and gives some indications of an analogous process in the field of 5th roots of unity; he uses these results to prove by an « infinite descent » argument more correct than Euler’s that the equation $x^3 + y^3 = z'$ has no solution in the field of cube roots of unity, indicates that one can extend the method to the equation $x^5 + y^5 = z^5$, but stops short of the equation $x^7 + y^7 = z^7$, saying that here it is impossible to reject apriori the case where x, y and z are not divisible by 7.

** In his earliest work on « ideal numbers », Kummer explicitly indicated the possibility of applying his method, not only to cyclotomic fields, but also to quadratic fields, and hence of recovering Gauss' results on binary quadratic forms ((XII), pp. 324-325).

(Vd): for every polynomial $f$ with real coefficients, he attempted to prove the existence of a factorisation $f = f_1 f_2$ into two (non constant) polynomials with *real* coefficients, which would give him a proof of the « fundamental theorem » by induction on the degree off. It even suffices, as he noticed, to stop at the first odd degree factor, and consequently all the difficulties are reduced to the consideration of the case where the degree $n$ off is even. Euler then restricts himself to the case when the desired factors each have degree $n/2$, and he indicates that by a suitable process of elimination one can express the unknown coefficients of $f_1$ and $f_2$ as rational functions of a root of an equation with real coefficients, whose extreme terms have *opposite signs* and which consequently has at least one real root. But Euler's proof was only a sketch, and skipped over a number of essential points; it was not till *1772* that Lagrange succeeded in resolving the difficulties raised by this proof (*VIId*) by means of an extremely long and minute analysis, in which he demonstrated a remarkable virtuosity in the use of the « Galois methods » which he had recently created (cf. Historical Note to Chap. IV and V).

All the same, Lagrange, like Euler and all his contemporaries, had no hesitation in arguing formally within a « field of roots » of a polynomial (that is, in his language, to consider « imaginary roots » of this polynomial); the Mathematics of his period had provided no justification for this type of argument. Gauss, who was from the outset resolutely hostile to the unrestricted formalism of the 18th century, came out strongly against this abuse in his dissertation ((VIII), vol. *III*, p. 3). But it would have been unlike him not to have sensed that it was a case of a superficially faulty presentation of an argument which was intrinsically correct. We find him also, a few years later ((VIII), vol. *III*, p. 33; cf. also *(VIIIbis)*), taking up a simpler form of Euler's argument, which had been suggested in *1759* by Foncenex (who, however, had been unable to use it to any advantage), to obtain a new proof of the « fundamental theorem » in which he carefully avoids all mention of « imaginary » roots: the latter being replaced by skilful adjunction and specialisation of indeterminates. It is essentially this proof of Gauss that we have given in the text (VI, p. 26, Th. 3), with simplifications made possible by the use of algebraic extensions.

The rôle of Topology in the « fundamental theorem » was thus reduced to the single theorem that a polynomial with real coefficients cannot change sign in an interval without having a zero (Bolzano's Theorem for polynomials). This theorem is also at the root of all the criteria for separation of the real roots of a polynomial (with real coefficients), which was one of the favourite Algebraic topics in the 19th century *. In the course of this research it becomes obvious that it is the order structure of $\mathbf{R}$, much more than its topology, which plays the

\* On these topics, which we will not discuss in the present work, the reader may consult for example J.-A. Serret, Cours d'Algèbre supérieure, 3rd ed., Paris (Gauthier-Villars), 1866, or B. L. van der Waerden, Moderne Algebra, vol. I (1st ed.), Berlin (Springer) 1930, pp. 223-235.

essential rôle *; for example Bolzano's Theorem for polynomials remains true in the field of all real algebraic numbers. This train of ideas resulted in the abstract theory of ordered fields, created by E. Artin and O. Schreier (XXV); one of its most remarkable results is certainly the discovery that the existence of an order relation on a field is related to purely algebraic properties of the field. This is the theory presented in § 2 of Chap. VI.

\* The tendency to attach overwhelming importance to the order structure of the real numbers can also be seen in their definition by means of Dedekind « cuts », which is basically a process which can be applied to all ordered sets (cf. VI, p. 35, Ex. 30 onwards).

Bibliography

(I) Euclidis Elementa, 5 vol., ed. J. L. Heiberg, Lipsiae (Teubner), 1883-88.
(I bis) T. L. Heath, The thirteen books of Euclid's Elements..., 3 vol., Cambridge, 1908.
(II) Diophanti Alexandrini Opera Omnia..., 2 vol., ed. P. Tannery, Lipsiae (Teubner), 1893-95.
(II bis) T. L. Heath, Diophantus of Alexandria, 2nd ed., Cambridge, 1910.
(III) B. Datta and A. N. Singh, History of Hindu Mathematics, 2 vol., Lahore (Motilal Banarsí Das), 1935-38.
(IV) S. Stevin, Les œuvres mathématiques..., ed. A. Girard, Leyde (Elsevier), 1634, vol. I.
(V) L. Euler : a) Introductio in Analysin Infinitorum (Opera Omnia, (1), t. IX, Zürich-Leipzig-Berlin (O. Füssli and B. G. Teubner), 1945, p. 384); b) Theoria motus corporum solidorum seu rigidorum (Opera Omnia (2), t. III, Zurich-Leipzig-Berlin (O. Fussli and B. G. Teubner), 1948, p. 200-201); c) Vollständige Anleitung zur Algebra (Opera Omnia (1), t. I, Leipzig-Berlin (Teubner), 1911, p. 422); d) Recherches sur les racines imaginaires des équations (Opera Omnia (1), t. VI, Leipzig-Berlin (Teubner), 1921, p. 78).
(VI) J.-L. Lagrange, Œuvres, Paris (Gauthier-Villars), 1867-1892 : a) Solutions de divers problemes de Calcul integral, t. I, p. 520; b) Recherches sur les équations séculaires du mouvement des nœuds, t. VI, p. 655-666; c) Recherches d'arithmétique, t. III, p. 695-795; d) Sur la forme des racines imaginaires des équations, t. III, p. 479; e) Nouvelle solution du probleme de rotation d'un corps quelconque qui n'est animé par aucune force accélératrice, t. III, p. 579-616.
(VII) P. S. Laplace : a) Mémoire sur les solutions particulières des equations différentielles et sur les inegalites seculaires des planetes (Œuvres, t. VIII, Paris (Gauthier-Villars), 1891, p. 325-366); b) Mémoire sur les inégalités seculaires des planetes et des satellites (Œuvres, t. XI, Paris (Gauthier-Villars), 1895, p. 49-92).
(VIII) C. F. Gauss, Werke, t. I (Gottingen, 1870), t. II (ibid., 1876) et t. III (ibid., 1876).
(VIII bis) Die vier Gauss'schen Beweise für die Zerlegung ganzer algebraischer Functionen in reelle Factoren ersten oder zweiten Grades (Ostwald's Klassiker, n° 14, Leipzig (Teubner), 1904).
(IX) N. H. Abel, Œuvres, t. I, ed. Sylow and Lie, Christiania, 1881.
(X) A. L. Cauchy : a) Leçons sur les applications du Calcul infinitésimal a la Géométrie (Œuvres complètes (2), t. V, Paris (Gauthier-Villars), 1903, p. 248); b) Sur l'équation a l'aide de laquelle on determine les inégalités séculaires des planetes (Œuvres complètes (2), t. IX, Paris (Gauthier-Villars), 1891, p. 174).
(XI) P. G. Lejeune-Dirichlet, Werke, t. I, Berlin (G. Reimer), 1889, p. 619-644.
(XII) E. Kummer, Zur Theorie der complexen Zahlen, J. de Crelle, t. XLIII (1847), p. 319 (Collected papers, vol. I, Heidelberg (Springer V.), 1975, p. 203).
(XIII) Ch. Hermite, Œuvres, t. I, Paris (Gauthier-Villars), 1905.
(XIV) J. J. Sylvester, Collected Mathematical Papers, vol. I, Cambridge, 1904 : An enumeration of the contacts of lines and surfaces of the second order, p. 219 (= Phil. Mag., 1851).
(XV) W. R. Hamilton, Lectures on Quaternions, Dublin, 1853.
(XVI) A. Cayley, Collected Mathematical Papers, Cambridge, 1889-1898 : A memoir on the theory of matrices, t. II. p. 475-496 (= Phil. Trans., 1858).

(XVII) H. J. SMITH, Collected Mathematical Papers, vol. I, Oxford, 1894 ; On systems of linear indeterminate equations and congruences, p. 367 (Phil. Trans., 1861).
(XVIII) E. SCHERING, Die fundamental Classen der zusammensetzbaren arithmetischen Formen, Abh. Ges. Göttingen, t. XIV (1868-69), p. 13.
(XIX) K. WEIERSTRASS, Mathematische Werke, Bd. II, Berlin (Mayer und Müller), 1895 : Zur Theorie der bilinearen und quadratischen Formen, p. 19.
(XX) L. KRONECKER, Auseinandersetzungen einiger Eigenschaften der Klassenanzahl idealer complexer Zahlen, Monats. Abhandl. Berlin (1870), p. 881 (= Werke, t. I, Leipzig (Teubner), 1895, p. 273).
(XXI) C. JORDAN, Traité des substitutions et des équations algébriques. Paris (Gauthier-Villars), 1870, p. 114-125.
(XXII) G. FROBENIUS, Theorie der linearen Formen mit ganzen Coefficienten, Gesammelte Abhandlungen, vol. I, Heidelberg (Springer V.), 1968, p. 482 (= J. de Crelle, 1879).
(XXIII) G. FROBENIUS und L. STICKELBERGER, Ueber Gruppen von vertauschbaren Elementen, J. de Crelle, t. LXXXVI (1879), p. 217 (= Frobenius, Ges. Abh., vol. I, p. 545).
(XXIV) R. DEDEKIND, Gesammelte mathematische Werke, t. II, Braunschweig (Vieweg), 1932 : Ueber Zerlegungen von Zahlen durch ihre grössten gemeinsamen Teiler, p. 103.
(XXV) a) E. ARTIN und O. SCHREIER, Algebraische Konstruktion reeler Korper, Abh. Math. Sem. Univ. Hamburg, t. V (1927), p. 83 ; b) E. ARTIN, Ueber die Zerlegung definiter Funktionen in Quadrate (ibid., p. 100) ; c) E. ARTIN und O. SCHREIER, Eine Kennzeichnung der reell abgeschlossenen Korper (ibid., p. 225).

Index of notation

A[(X_i)_{i \in I}], A[X_1, ..., X_n], X^\nu : IV, p. 1.
$deg u$ : IV, p. 3.
$f \circ g$ : IV, p. 4.
D_i P, D_{x_i} P, \frac{\partial P}{\partial X_i}, P'_{x_i}, D^\nu, DP, \frac{dP}{dX}, P' : IV, p. 6.
$\Delta^\nu$ : IV, p. 7.
K((X_i)_{i \in I}), deg r : IV, p. 19 and 20.
D_i f, D_{x_i} f, \frac{\partial f}{\partial X_i}, f'_{x_i}, Df, \frac{df}{dX}, f' : IV, p. 23.
$A[[X_i)_{i \in I}]], A[[I]]$ : IV, p. 24.
$\omega$ : IV, p. 25.
u(x), u((x_i)_{i \in I}), u(x_1, ..., x_n) : IV, p. 29.
$A", D", D_i$ : IV, p. 31 and 32.
D_i u, D_{x_i} u, \frac{\partial u}{\partial X_i}, u'_{x_i}, Du, \frac{du}{dX} : IV, p. 32.
$A\{I\}, f \circ g$ : IV, p. 29 and 36.
$T_1$ : IV, p. 36.
exp X, e^X, e(X), l(X) : IV, p. 39 and 40.
$exp f, log g$ : IV, p. 40.
M^H, Tr_{H/G} : IV, p. 41 and 42.
TS^n(M), TS(M) : IV, p. 42.
$\mathfrak{S}_{p|q}, \mathfrak{S}_{p,q}, \mathfrak{S}_{p_1|\cdots|p_n}$ : IV, p. 43.
\gamma_k(x), x \in M : IV, p. 45.
$\varphi_M, \psi_M$ : IV, p. 52.
Pol_A^q(M, N), Pol^q(M, N) : IV, p. 55.
Map(M, N), Pol_A(M, N), Pol(M, N) : IV, p. 57.
s_k, s_{k,n}, A[X_1, ..., X_n]^{\text{sym}} : IV, p. 61.
$S(\alpha), M(\alpha)$ : IV, p. 65 and 66.
s_k, A[[X]]^{\text{sym}} : IV, p. 67 and 68.
$\mathcal{B}_k$ : IV, p. 70.
M(f, g, p, q), res_{p,q}(f, g), res(f, g) : IV, p. 76.
dis(f), f monic polynomial : IV, p. 81.
dis_m(f), f polynomial of degree \leq m : IV, p. 83.
\Gamma(E), \Gamma_p(E), \gamma_p, \Gamma(h) : IV, p. 92, ex. 2.
$Q, F_p$ : V, p. 1.
S^{pf} : V, p. 4.

$K[S]$ : V, p. 4.
$S^{p^{-f}}, A^{p^{-\infty}}$: V, p. 5 and 6.
[A : K]: V, p. 10.
K(x_i), K(x), K(x_1, ..., x_n): V, p. 10.
h(L), [A : K], $\mathcal{H}(A)$: V, p. 31.
$E_s$ : V, p. 44.
$[E:K]_s, [E:K],$ : V, p. 31 and 46.
$N_{A/K}(x), \mathrm{Tr}_{A/K}(x), D_{A/K}(x_1, ..., x_n)$ : V, p. 47.
$Gal(N/K)$ : V, p. 58.
$k(\Delta), g(E)$ : V, p. 67.
K_{ab}: V, p. 77.
$\mu_m(K), \mu_\infty(K), \mathbf{Z}[1/p]$: V, p. 78.
$\mu_{l^\infty}(K)$: V, p. 79.
$\varphi(n)$: V, p. 79.
R_n(K), \Phi_n, \chi_n: V, p. 81.
K(A^{1/n}), \langle \sigma, a \rangle: V, p. 88.
$\mathfrak{g}, K(\mathfrak{g}^{-1}(A))$, [u, a]: V, p. 91.
F_q(\Omega), F_q: V, p. 95.
Z_l, Z: V, p. 96.
$\sigma_q$: v, p. 97.
$\varphi_n$: V, p. 97.
deg.tr_K E: V, p. 110.
f^A: V, p. 127.
$\chi(f), f$ a linear mapping: V, p. 132.
$x|y, x|y$ : VI, p. 5.
$(x)$ : VI, p. 6.
$x \equiv x' (\bmod y)$ : VI, p. 6.
sup_F(x_i) (F a subset of an ordered set E): VI, p. 8.
gcd(x_i), lcm(x_i): VI, p. 8.
x^+, x^-, |x| (x an element of a lattice ordered group): VI, p. 12.
sgn(x): VI, p. 20.
$\sqrt{a}$ (a an element $\geq 0$ of an ordered field) VI, p. 24.
|z| (z an element of K(i). where K is an ordered field and i^2 = -1): VI, p. 27.
GL+(E) (E an oriented vector space): VI, p. 29.
M(\alpha), M_\alpha (M a module over A, \alpha \in A): VII, p. 7.
(Z/nZ)^*: U(p^n): VII, p. 12.
c_L(x), L a free module over a principal ideal domain A, x \in L: VII, p. 16.
m(0), m(p^n) (p irreducible, n an integer $\geq 1$): VII, p. 24.
D(M) (M a module over a principal ideal domain A, N^0: VII, p. 25 to 27.
$c_M: M \to D(D(M))$ : VII, p. 26.
M_u (M a module, u an endomorphism of M): VII, p. 28.
V_\alpha (V a vector space, \alpha \in K): VII, p. 30.
$\chi_u, \chi_v$: VII, p. 30.
$U_{m,\alpha}$ : VII, p. 35.
u_s, u_j (u an endomorphism): VII, p. 43 and 45.
f_s, f_u (f an automorphism): VII, p. 46.

Index of terminology

Abelian closure : V, p. 77.
Abelian extension : V, p. 77.
Absolutely semi-simple endomorphism : VII, p. 42.
Addition of inequalities : VI, p. 2.
Adjunction (extension obtained by) : V, p. 11.
Algebraic closure : V, p. 22.
Algebraic element in an algebra : V, p. 16.
Algebraic extension : V, p. 17.
Algebraic number : V, p. 20.
Algebraically closed field : V, p. 20.
Algebraically dependent family, subset : V, p. 106.
Algebraically disjoint extensions : V, p. 112.
Algebraically free family of extensions : V, p. 115.
Algebraically free family, subset : IV, p. 4, V, p. 106.
Archimedean ordered group : VI, p. 35, Ex. 31.
Artin’s theorem : V, p. 65.
Artin-Schreier theorem : VI, p. 22.
Artin-Schreier theory : V, p. 91.
Associated elements : VI, p. 5.

Bezout's identity : VII, p. 2.
Budan-Fourier rule : VI, p. 42, Ex. 21.

Characteristic exponent of a field : V, p. 7.
Characteristic of a ring : V, p. 2.
Characteristic submodule : VII, p. 67, Ex. 16.
Chinese remainder theorem : VI, p. 33, Ex. 25.
Closed (field, algebraically) : V, p. 20.
Closed (field, separably) : V, p. 45.
Closed half-line : VI, p. 28.
Closed (relatively algebraically) field : V, p. 19.
Closure (abelian) of a field : V, p. 77.
Closure (algebraic) of a field : V, p. 22.
Closure (algebraic separable) : V, p. 45.
Closure (perfect) : V, p. 5.
Closure (relative algebraic) : V, p. 19.

Closure (relative p-radical) : V, p. 25.
Closure (relative separable algebraic) : V, p. 43.
Coefficients of a formal power series : IV, p. 24.
Coefficients of a polynomial : IV, p. 1.
Compatible (order relation) with a group, monoid structure : VI, p. 1.
Compatible (order relation) with a ring structure : VI, p. 19.
Compatible (preorder relation) with a commutative monoid structure : VI, p. 3.
Complementary orientation : VI, p. 29.
Composite extension : V, p. 12.
Composition of series : IV, p. 97, Ex. 15.
Conjugacy class in $\Omega$ : V, p. 52.
Conjugate elements : V, p. 52 ;
Conjugate extensions : V, p. 52.
Constant polynomial, term : IV, p. 1.
Content : VII, p. 16.
Coprime elements : VI, p. 13.
Coproduct in TS(M) : IV, p. 50.
Cubic extension : V, p. 10.
Cyclic extension : V, p. 85.
Cyclic vector space (for u) : VII, p. 29.
Cyclotomic extension : V, p. 81.
Cyclotomic polynomial : V, p. 81.

Decomposable module : VII, p. 23.
Decomposition algebra (universal) of a polynomial : IV, p. 73.
Decomposition theorem: VI, p. 11.
Dedekind's theorem : V, p. 27.
Degree (inseparable) of an extension : V, p. 46.
Degree of an algebra over a field : V, p. 10.
Degree of an algebraic element : V, p. 16.
Degree (total) of a polynomial : IV, p. 3.
Degree (total) of a rational fraction : IV, p. 20.
Degree (separable) of an extension : V, p. 31.
Derivation (partial) in a p-radical extension of height $\leq 1$ : V, p. 103.
Derivative (partial) of a formal power series : IV, p. 32.
Derivative (partial) of a polynomial : IV, p. 6.
Descartes'rule : VI, p. 42, Ex. 21.
Diagonal, diagonalizable set of endomorphisms : VII, p. 40.
Diagonalizable, diagonalized algebra : V, p. 28.
Direct basis : VI, p. 29.
Direction vector : VI, p. 28.
Direction of a half-line : VI, p. 28.
Discriminant of a monic polynomial : IV, p. 81.
Discriminant of a polynomial : IV, p. 83.
Discriminant of a sequence of elements : V, p. 47.
Disjoint (algebraically) extensions : V, p. 112.

Disjoint (linearly) extensions : V, p. 14.
Divided power in TS(M) : IV, p. 45.
Divided power of a series : IV, p. 96, Ex. 13.
Divisibility relation : VI, p. 5.
Division (euclidean) : IV, p. 10.
Divisor (greatest common) : IV, p. 12, VI, p. 8.
Divisor of an element : VI, p. 5.
Divisors (elementary) of a module : VII, p. 24.
Double root : IV, p. 15.

Eigenspace : VII, p. 30.
Eigenvalue : VII, p. 30.
Elementary divisor of a module : VII, p. 24.
Elementary symmetric polynomial : IV, p. 61.
Etale algebra : V, p. 28.
Euclid's lemma : VI, p. 15.
Euclidean domain : VII, p. 49, Ex. 7.
Euler's identity : VI, p. 8, IV, p. 89, Ex. 6.
Euler-Lagrange theorem : VI, p. 26.
Expansion at the origin of a rational fraction : IV, p. 30, V, p. 39.
Exponential of a formal power series : IV, p. 39.
Exponential type (sequence of) : IV, p. 91, Ex. 1.
Extension of a field : V, p. 9.
Extension (principle of) of algebraic identities : IV, p. 18.

Finite extension : V, p. 10.
Finitely generated extension : V, p. 11.
Form of degree n : IV, p. 2.
Formal power series : IV, p. 24.
Formal power series (generalized) : IV, p. 38.
Fractions (fields of rational) : IV, p. 19.
Frobenius homomorphism : V, p. 4, V, p. 92.

Galois extension : V, p. 57.
Galois group of an extension, of a polynomial : V, p. 58.
Galois theory : V, p. 67.
Gamma algebra of a module : IV, p. 92, Ex. 2.
Gaussian integer : VII, p. 1.
Generated (extension) : V, p. 11.
Generated (Galois extension) : V, p. 57.
Generated (quasi-Galois extension) : V, p. 55.
Generating family of an extension : V, p. 11.
Greatest common divisor (GCD) of elements : VI, p. 8.
Greatest common divisor of polynomials : IV, p. 12.
Greatest common divisor of principal ideals : VII, p. 3.

Half-line (closed, open) : VI, p. 28.
Half-lines (opposite) : VI, p. 28.
Hankel determinants : IV, p. 90, Ex. 1.
Height of a p-radical element : V, p. 24.
Height of a p-radical extension : V, p. 26.
Height of an element of K(T) : V, p. 148, Ex. 11.
Hermite interpolation formula : IV, p. 88, Ex. 13.
Hermite reduced form : VII, p. 68, Ex. 21.
Homogeneous component of a formal power series : IV, p. 25.

Imperfect field : V, p. 7.
Imperfection (degree of) : V, p. 170, Ex. 1.
Indecomposable module : VII, p. 23.
Indeterminate : IV, p. 1.
Index of a linear mapping : V, p. 132.
Indicator (Euler's) : V, p. 79.
Indivisible element : VII, p. 17.
Inflation homomorphism : V, p. 70.
Inseparable degree : V, p. 46.
Integral ideal : VI, p. 6.
Invariant factors of a linear mapping : VII, p. 22.
Invariant factors of a module : VII, p. 20.
Invariant factors of a submodule : VII, p. 19.
Invariants (similarity) of an endomorphism : VII, p. 32.
Irreducible element : VI, p. 17.
Irreducible polynomial : IV, p. 13.
Isobaric polynomial : IV, p. 3.

Jordan decomposition : VII, p. 43.
Jordan decomposition (multiplicative) : VII, p. 46.
Jordan matrix : VII, p. 35.

Kummer extension : V, p. 162, Ex. 7.
Kummer theory : V, p. 88.

Lagrange interpolation formula : IV, p. 16.
Law (polynomial) : IV, p. 94, Ex. 9.
Leading coefficient : IV, p. 3.
Least common multiple (LCM) of elements : VI, p. 8.
Least common multiple of principal ideals : VII, p. 3.
Lefschetz's principle : V, p. 117.
Lexicographic product of ordered groups : VI, p. 7.
Linear topology : IV, p. 28.
Linearly disjoint extensions : V, p. 13.
Linearly topologized algebra : IV, p. 28.

Logarithm of a formal power series : IV, p. 40
Logarithmic derivative : IV, p. 41.
Liiroth's theorem : V, p. 149, Ex. 11.

Mac Laner's criterion : V, p. 43, V, p. 123.
Maximal ordered field : VI, p. 25.
Minimal polynomial of an element : V, p. 16.
Minimal polynomial of an endomorphism : VII, p. 29.
Minkowski's lemma : VII, p. 50, Ex. 9.
Monic polynomial : IV, p. 3.
Monogenous extension : V, p. 11.
Monomials, IV, p. 1.
Multiple factor (polynomial without) : IV, p. 14.
Multiple of an element : VI, p. 5.
Multiple root : IV, p. 15.
Multiplicity (geometric) of an eigenvalue : VII, p. 30.
Multiplicity of a root : IV, p. 15.
Multiplicity of an elementary divisor : VII, p. 24.

Negative element : VI, p. 4.
Negative n-vector : VI, p. 29.
Negative basis : VI, p. 29.
Newton polygon : V, p. 150, Ex. 2.
Newton's relations : IV, p. 70, IV, p. 75.
Nilpotent component : VII, p. 45.
Normal basis, normal basis theorem : V, p. 73.
Normal extension : V, p. 53.
$Norm$ : V, p. 47.

Open half-line : VI. p. 28.
Opposite half-lines : VI, p. 28.
Order of a (generalized) formal power series : IV, p. 25, IV, p. 38
Order of a root : IV, p. 15.
Orderable field : VI, p. 39, Ex. 8.
Ordered extension : VI, p. 21.
Ordered field : VI, p. 20.
Ordered group, monoid : VI, p. 1.
Ordered ring : VI, p. 19.
Orientation of a vector space : VI, p. 29.
Oriented affine space, vector space : VI, p. 29.

p-adic integers (ring of) : V, p. 96
p-basis : V, p. 98.
p-basis (absolute) : V, p. 98.
p-free family : V, p. 98.

p-radical closure : V, p. 25.
p-radical element : V, p. 24.
p-radical extension : IV, p. 19.
p-torsion group : VII, p. 10.
n-primary component : VII, p. 8.
π-primary module : VII, p. 7.
Perfect closure of a ring : V, p. 5.
Perfect field : V, p. 7.
Perfect ring of characteristic p : V, p. 5.
Polynomial, polynomial algebra : IV, p. 1.
Polynomial function : IV, p. 4.
Polynomial law : IV, p. 94, Ex. 9.
Polynomial mapping : IV, p. 57.
Polynomial mapping (homogeneous) : IV, p. 55.
Positive basis : VI, p. 29.
Positive element : VI, p. 4.
Positive n-vector : VI, p. 29.
Power series (generalized formal) : IV, p. 24, IV, p. 38
Preordered group, monoid : VI, p. 3.
Primary extension : V, p. 139.
Prime field, subfield : V, p. 1.
Primitive element (theorem of the) : V, p. 40.
Primitive root of unity : V, p. 81.
Principal fractional ideal : VI, p. 6.
Principal ideal domain : VII, p. 1.
Principal ideal ring : VII, p. 49, Ex. 6.
Product (lexicographic) of ordered groups : VI, p. 7.
Product of ordered groups : VI, p. 7.
Product orientation : VI, p. 29.
Puiseux's theorem : V, p. 150, Ex. 2.
Pure basis : V, p. 106.
Pure extension : V, p. 106.
Pure submodule : VII, p. 55, Ex. 7.
Pythagorean field : VI, p. 39, Ex. 8.

Quadratic extension : V, p. 10.
Quadratic reciprocity (theorem of) : V, p. 166, Ex. 23.
Quasi-Galois extension : V, p. 53.
Quotient in euclidean division : IV, p. 11.
Quotient orientation : VI, p. 29.

Rational fraction : IV, p. 19.
Rational function : IV, p. 21.
Reduced ring : V, p. 34.
Regular algebra : V, p. 140.
Regular extension : V, p. 141.
Relative algebraic closure of a field in an extension : V, p. 19.

Relatively algebraically closed field in an extension field : V, p. 19.
Relatively prime polynomials : IV, p. 12.
Remainder in euclidean division : IV, p. 11.
Representatives (system of) of irreducible elements : VII, p. 3.
Restriction homomorphism : V, p. 60, V, p. 70.
Resultant of two polynomials : IV, p. 76.
Root of a polynomial : IV, p. 14.
Root of unity : V, p. 78.
Rule of signs : VI, p. 19.

Semi-simple (absolutely) component : VII, p. 45.
Semi-simple (absolutely) endomorphism : VII, p. 42.
Semi-simple endomorphism : VII, p. 41.
Semi-simple module : VII, p. 9.
Separable algebra : V, p. 119.
Separable algebraic closure (relative) : V, p. 44.
Separable algebraic extension : V, p. 36.
Separable closure : V, p. 44.
Separable degree : V, p. 31.
Separable element : V, p. 39.
Separable extension : V, p. 121.
Separable polynomial : V, p. 37.
Separably closed field : V, p. 45.
Separating transcendence basis : V, p. 136.
Series on E with values in F : IV, p. 96, Ex. 11.
Set (\Gamma-) : V, p. 75.
Sign of an element : VI, p. 20.
Similar endomorphisms, matrices : VII, p. 29.
Similarity invariants of on endomorphism : VII, p. 32.
Simple module : VII, p. 25.
Simple root : IV, p. 15.
Splitting field, extension : V, p. 21.
Subextension : V, p. 9.
Subfield : V, p. 1.
Substitutable element in a rational fraction : IV, p. 21.
Substitution in a formal power series : IV, p. 29.
Substitution in a polynomial : IV, p. 4.
Substitution in a rational fraction : IV, p. 21.
Symmetric (elementary) polynomials : IV, p. 61.
Symmetric formal power series : IV, p. 67.
Symmetric polynomial : IV, p. 61.
Symmetric product of symmetric tensors : IV, p. 43.
Symmetric rational fraction : IV, p. 67.
Symmetric tensor : IV, p. 42.
Symmetrized tensor : IV, p. 43.

Tangent linear mapping : IV, p. 36.
Taylor's formula for formal power series : IV, p. 31.

Taylor's formula for polynomials : IV, p. 8.
Term, constant term, of a formal power series : IV, p. 24.
Term, constant term, of a polynomial : IV, p. 1.
Trace : V, p. 47.
Transcendence basis : V, p. 109.
Transcendence degree : V, p. 110.
Transcendental element : V, p. 16.
Transcendental extension : V, p. 17.
Translation homomorphism : V, p. 70.
Triangularisable endomorphism : VII, p. 35.
Trivial extension : V, p. 9.

Ulm-Zippin theorem : VII, p. 59, Ex. 14.
Unipotent component : VII, p. 46.
Unipotent endomorphism : VII, p. 46.
Units of a ring : VI, p. 5.
Universal decomposition of a monic polynomial : IV, p. 73.

Weight : IV, p. 3.
Wilson's formula : V, p. 94.

Zero of a polynomial : IV, p. 14.

Table of contents

Chapter IV. — Polynomials and rational fractions ............ IV.1

§ 1. Polynomials ..................................................... IV.1
    1. Definition of polynomials .................................. IV.1
    2. Degrees ..................................................... IV.2
    3. Substitutions .............................................. IV.4
    4. Differentials and derivations ............................. IV.6
    5. Divisors of zero in a polynomial ring .................... IV.9
    6. Euclidean division of polynomials in one indeterminate .... IV.10
    7. Divisibility of polynomials in one indeterminate .......... IV.11
    8. Irreducible polynomials ................................... IV.13

§ 2. Zeros of polynomials ......................................... IV.14
    1. Roots of a polynomial in one indeterminate. Multiplicity ..................................................... IV.14
    2. Differential criterion for the multiplicity of a root ..... IV.17
    3. Polynomial functions on an infinite integral domain ...... IV.17

§ 3. Rational fractions ............................................. IV.19
    1. Definition of rational fractions ........................... IV.19
    2. Degrees ..................................................... IV.20
    3. Substitutions .............................................. IV.21
    4. Differentials and derivations ............................. IV.23

§ 4. Formal power series .......................................... IV.24
    1. Definition of formal power series. Order .................. IV.24
    2. Topology on the set of formal power series. Summable families ..................................................... IV.25
    3. Substitutions .............................................. IV.28
    4. Invertible formal power series ............................ IV.30
    5. Taylor's formula for formal power series .................. IV.31
    6. Derivations in the algebra of formal power series ....... IV.32
    7. The solution of equations in a formal power series ring .. IV.35
    8. Formal power series over an integral domain .............. IV.38
    9. The field of fractions of the ring of formal power series in one indeterminate over a field ....................... IV.38
   10. Exponential and logarithm .................................. IV.39

§ 5. Symmetric tensors and polynomial mappings ......................... IV.41
    1. Relative traces .................................................. IV.41
    2. Definition of symmetric tensors ................................. IV.42
    3. Product for symmetric tensors .................................. IV.43
    4. Divided powers .................................................. IV.45
    5. Symmetric tensors over a free module .......................... IV.47
    6. The functor TS .................................................. IV.48
    7. Coproduct for symmetric tensors ................................. IV.50
    8. Relations between TS(M) and S(M) .............................. IV.52
    9. Homogeneous polynomial mappings ................................. IV.54
   10. Polynomial mappings ............................................. IV.57
   11. Relations between S(M*), TS(M)*gr and Pol(M, A) ......... IV.59

§ 6. Symmetric functions ............................................. IV.61
    1. Symmetric polynomials .......................................... IV.61
    2. Symmetric rational fractions ................................. IV.67
    3. Symmetric formal power series ................................. IV.67
    4. Sums of powers ................................................ IV.70
    5. Symmetric functions in the roots of a polynomial .......... IV.72
    6. The resultant .................................................. IV.75
    7. The discriminant ............................................... IV.81

Exercises on § 1 .................................................... IV.86
Exercises on § 2 .................................................... IV.87
Exercises on § 3 .................................................... IV.89
Exercises on § 4 .................................................... IV.90
Exercises on § 5 .................................................... IV.91
Exercises on § 6 .................................................... IV.98
Table ............................................................... IV.103

CHAPTER V. — COMMUTATIVE FIELDS .................................. V.1

§ 1. Prime fields. Characteristic .................................. V.1
    1. Prime fields .................................................. V.1
    2. Characteristic of a ring and of a field ..................... V.2
    3. Commutative rings of characteristic p ....................... V.3
    4. Perfect rings of characteristic $p$ ....................... V.5
    5. Characteristic exponent of a field. Perfect fields ........ V.7
    6. Characterization of polynomials with zero differential .. V.7

§ 2. Extensions .................................................... V.9
    1. The structure of an extension ............................... V.9
    2. Degree of an extension ...................................... V.10
    3. Adjunction .................................................. V.10
    4. Composite extensions ......................................... V.12
    5. Linearly disjoint extensions ............................... V.13

§ 3. Algebraic extensions ......................................... V.15
    1. Algebraic elements of an algebra ........................... V.15

2. Algebraic extensions ..................................................... V.17
3. Transitivity of algebraic extensions. Fields that are relatively algebraically closed in an extension field ............ V.19

§ 4. Algebraically closed extensions ............................................. V.19
    1. Algebraically closed fields ............................................. V.19
    2. Splitting extensions .................................................. V.21
    3. Algebraic closure of a field .......................................... V.22

§ 5. p-radical extensions .......................................................... V.24
    1. p-radical elements ..................................................... V.24
    2. p-radical extensions .................................................. V.25

§ 6. Etale algebra ................................................................. V.26
    1. Linear independence of homomorphisms ......................... V.26
    2. Algebraic independence of homomorphisms .................. V.28
    3. Diagonalizable algebras and etale algebras ............... V.28
    4. Subalgebras of an etale algebra ................................. V.30
    5. Separable degree of a commutative algebra ................. V.31
    6. Differential characterization of etale algebras ........... V.33
    7. Reduced algebras and etale algebras .......................... V.34

§ 7. Separable algebraic extensions ............................................. V.36
    1. Separable algebraic extensions .................................. V.36
    2. Separable polynomials ............................................... V.37
    3. Separable algebraic elements ...................................... V.39
    4. The theorem of the primitive element ......................... V.40
    5. Stability properties of separable algebraic extensions ... V.41
    6. A separability criterion ........................................... V.42
    7. The relative separable algebraic closure .................... V.43
    8. The separable closure of a field ................................. V.45
    9. Separable and inseparable degrees of an extension of finite degree ..................................................... V.46

§ 8. Norms and traces ............................................................. V.47
    1. Recall ............................................................................. V.47
    2. Norms and traces in etale algebras ............................. V.47
    3. Norms and traces in extensions of finite degree .......... V.50

§ 9. Conjugate elements and quasi-Galois extensions ......................... V.52
    1. Extension of isomorphisms ......................................... V.52
    2. Conjugate extensions. Conjugate elements .................. V.52
    3. Quasi-Galois extensions ............................................. V.53
    4. The quasi-Galois extension generated by a set ............. V.55

§ 10. Galois extensions ............................................................ V.56
    1. Definition of Galois extensions .................................. V.56
    2. The Galois group ..................................................... V.58
    3. Topology of the Galois group ...................................... V.60

4. Galois descent .................................................. V.62
5. Galois cohomology ............................................. V.64
6. Artin’s theorem ............................................... V.65
7. The fundamental theorem of Galois theory ............... V.67
8. Change of base field ......................................... V.69
9. The normal basis theorem .................................... V.72
10. Finite $\Gamma$-sets and etale algebras .................. V.75
11. The structure of quasi-Galois extensions ................. V.76

§ 11. Abelian extensions ........................................ V.77
    1. Abelian extensions and the abelian closure ............ V.77
    2. Roots of unity ........................................... V.78
    3. Primitive roots of unity ................................ V.79
    4. Cyclotomic extensions .................................... V.81
    5. Irreducibility of cyclotomic polynomials ............... V.83
    6. Cyclic extensions ......................................... V.85
    7. Duality of $\mathbf{Z}/n\mathbf{Z}$-modules ............ V.86
    8. Kummer theory ........................................... V.88
    9. Artin-Schreier theory .................................... V.91

§ 12. Finite fields .............................................. V.93
    1. The structure of finite fields .......................... V.93
    2. Algebraic extensions of a finite field .................. V.94
    3. The Galois group of the algebraic closure of a finite field .................................................. V.96
    4. Cyclotomic polynomials over a finite field ............. V.97

§ 13. $p$-radical extensions of height $\leq 1$ .......... V.98
    1. $p$-free subsets and $p$-bases ..................... V.98
    2. Differentials and $p$-bases .......................... V.100
    3. The Galois correspondence between subfields and Lie algebras of derivations ................................. V.104

§ 14. Transcendental extensions ................................ V.106
    1. Algebraically free families. Pure extensions ............ V.106
    2. Transcendence bases ...................................... V.107
    3. The transcendence degree of an extension ............... V.110
    4. Extension of isomorphisms ................................ V.111
    5. Algebraically disjoint extensions ....................... V.112
    6. Algebraically free families of extensions ............... V.115
    7. Finitely generated extensions ........................... V.117

§ 15. Separable extensions ...................................... V.118
    1. Characterization of the nilpotent elements of a ring ... V.118
    2. Separable algebras ....................................... V.119
    3. Separable extensions ..................................... V.121
    4. Mac Lane's separability criterion ....................... V.122
    5. Extensions of a perfect field ........................... V.125
    6. The characterization of separability by automorphisms V.125

§ 16. Differential criteria of separability ............................................. V.127
    1. Extension of derivations : the case of rings .................... V.127
    2. Extension of derivations : the case of fields ................. V.128
    3. Derivations in fields of characteristic zero .................. V.130
    4. Derivations in separable extensions ............................. V.131
    5. The index of a linear mapping ..................................... V.132
    6. Differential properties of finitely generated extensions . V.133
    7. Separating transcendence bases ................................... V.136

§ 17. Regular extensions ................................................................. V.137
    1. Complements on the relative separable algebraic closure ..................................................... V.137
    2. The tensor product of extensions ................................. V.139
    3. Regular algebras ............................................................. V.140
    4. Regular extensions .......................................................... V.141
    5. Characterization of regular extensions ......................... V.142
    6. Application in composite extensions .......................... V.143

Exercises on § 1 ............................................................................. V.145
Exercises on § 2 ............................................................................. V.146
Exercises on § 3 ............................................................................. V.147
Exercises on § 4 ............................................................................. V.150
Exercises on § 5 ............................................................................. V.150
Exercises on § 6 ............................................................................. V.151
Exercises on § 7 ............................................................................. V.151
Exercises on § 8 ............................................................................. V.153
Exercises on § 9 ............................................................................. V.153
Exercises on § 10 ........................................................................... V.154
Exercises on § 11 .......................................................................... V.160
Exercises on § 12 .......................................................................... V.166
Exercises on § 13 .......................................................................... V.170
Exercises on § 14 .......................................................................... V.171
Exercises on § 15 .......................................................................... V.175
Exercises on § 16 .......................................................................... V.177
Exercises on § 17 .......................................................................... V.180
Historical note (chapters IV and V) ............................................. V.182
Bibliography .................................................................................. V.197

CHAPTER VI. — ORDERED GROUPS AND FIELDS ............................. VI.1

§ 1. Ordered groups. Divisibility ..................................................... VI.1
    1. Definition of ordered monoids and groups ....................... VI.1
    2. Pre-ordered monoids and groups ................................. VI.3
    3. Positive elements ............................................................... VI.3
    4. Filtered groups ................................................................. VI.4
    5. Divisibility relations in a field ..................................... VI.5
    6. Elementary operations on ordered groups .................. VI.7
    7. Increasing homomorphisms of ordered groups ............. VI.7

8. Suprema and infima in an ordered group ......................... VI.8
9. Lattice-ordered groups ............................................. VI.10
10. The decomposition theorem ....................................... VI.11
11. Positive and negative parts ...................................... VI.12
12. Coprime elements .................................................. VI.13
13. Irreducible elements ............................................... VI.17

§ 2. Ordered fields ............................................................ VI.19
    1. Ordered rings ....................................................... VI.19
    2. Ordered fields ..................................................... VI.20
    3. Extensions of ordered fields ..................................... VI.21
    4. Algebraic extensions of ordered fields ........................ VI.23
    5. Maximal ordered fields ........................................... VI.25
    6. Characterization of maximal ordered fields. Euler-Lagrange theorem ..................................................... VI.26
    7. Vector spaces over an ordered field ............................. VI.28

Exercises on § 1 ............................................................. VI.30
Exercises on § 2 ............................................................. VI.37

CHAPTER VII. — MODULES OVER PRINCIPAL IDEAL DOMAINS ........ VII.1

§ 1. Principal ideal domains ............................................. VII.1
    1. Definition of a principal ideal domain ......................... VII.1
    2. Divisibility in principal ideal domains ....................... VII.1
    3. Decomposition into irreducible factors in principal ideal domains ..................................................... VII.3
    4. Divisibility of rational integers ................................. VII.5
    5. Divisibility of polynomials in one indeterminate over a field ..................................................... VII.5

§ 2. Torsion modules over a principal ideal domain ................. VII.6
    1. Modules over a product of rings ................................. v11.6
    2. Canonical decomposition of a torsion module over a principal ideal domain ........................................... VII.7
    3. Applications : I. Canonical decompositions of rational numbers and of rational functions in one indeterminate .... VII.10
    4. Applications : II. The multiplicative group of units of the integers modulo $a$ ........................................... VII.12

§ 3. Free modules over a principal ideal domain .................... VII.14

§ 4. Finitely generated modules over a principal ideal domain ... VII.15
    1. Direct sums of cyclic modules ................................... VII.15
    2. Content of an element of a free module ....................... VII.16
    3. Invariant factors of a submodule ............................... VII.18
    4. Structure of finitely generated modules ....................... VII.19
    5. Calculation of invariant factors ............................... VII.20

6. Linear mappings of free modules. and matrices over a principal ideal domain .................................................. VII.21
7. Finitely generated abelian groups .................................................. VII.22
8. Indecomposable modules. Elementary divisors ............ VII.23
9. Duality in modules of finite length over a principal ideal domain ............................................................. VII.25

§ 5. Endomorphisms of vector spaces ............................................. VII.28
    1. The module associated to an endomorphism ................. VII.28
    2. Eigenvalues and eigenvectors .................................. VII.30
    3. Similarity invariants of an endomorphisms ............... VII.31
    4. Triangularisable endomorphism ................................. VII.34
    5. Properties of the characteristic polynomial : trace and determinant .................................................. VII.36
    6. Characteristic polynomial of the tensor product of two endomorphisms .................................................. VII.39
    7. Diagonalisable endomorphisms .................................. VII.40
    8. Semi-simple and absolutely semi-simple endomorphisms .......................................................... VII.41
    9. Jordan decomposition ............................................... VII.43

Exercises on § 1 ............................................................................. VII.48
Exercises on § 2 ............................................................................. VII.54
Exercises on § 3 ............................................................................. VII.59
Exercises on § 4 ............................................................................. VII.62
Exercises on § 5 ............................................................................. VII.70
Historical note (Chapters VI and VII) ........................................... VII.73
Bibliography .................................................................................. VII.83
Index of notations ........................................................................ 445
Index of terminology .................................................................... 447
Table of contents .......................................................................... 455
