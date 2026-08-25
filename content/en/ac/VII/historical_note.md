---
book: ac
book_title: Commutative Algebra
chapter: VII
chapter_title: DIVISORS
section: 0
section_title: Historical Note
kind: historical
lang: en
source: ac-i-vii
book_pages: 579-625
pdf_pages: 0597-0642
extraction: ocr
statements: 0
exercises: 0
content_sha256: 310b51f7681f87389ad268cda064f6af31cea24a76ec2275974603d2dfff3682
---

# HISTORICAL NOTE

(Numbers in brackets refer to the bibliography at the end of this Note.)

"Abstract" commutative algebra is a recent creation but its development can only be understood as a function of that of the theory of algebraic numbers and algebraic geometry, which gave birth to it.

It has been conjectured without too much improbability that the famous "proof" Fermat claimed to possess of the impossibility of the equation $x^p + y^p = z^p$ for $p$ an odd prime and $x, y, z$ integers $\neq 0$ depended on the decomposition

$$
(x + y)(x + \zeta y) \ldots (x + \zeta^{p-1} y) = z^p
$$

in the ring $\mathbf{Z}[\zeta]$ (where $\zeta \neq 1$ is a $p$-th root of unity) and on a divisibility argument in this ring, assuming it to be a principal ideal domain. In any case an analogous argument is found outlined by Lagrange ([2], vol. II, p. 531); it is by arguments of this type, with certain variations (notably changes of variable aimed at lowering the degree of the equation) that Euler ([1], vol. I, p. 488) (*) and Gauss ([3], vol. II, p. 387) show Fermat's Theorem for $p = 3$, Gauss (loc. cit.) and Dirichlet ([4], vol. I, p. 42) for $p = 5$ and Dirichlet the impossibility of the equation $x^{14} + y^{14} = z^{14}$ ([4], vol. I, p. 190). Finally, in his first research on the theory of numbers, Kummer believed he had obtained in this way a general proof and it was no doubt this mistake (which Dirichlet pointed out to him) that led him to his study of the arithmetic of cyclotomic fields from which he was eventually to succeed in deducing a correct version of his proof for prime numbers $p < 100$ [7d].

On the other hand, the celebrated memoir of Gauss of 1831 on biquadratic

(*) In the proof, Euler argues as if $\mathbf{Z}[\sqrt{-3}]$ were a principal ideal domain, which is not the case; however, his argument can be rendered correct by considering the conductor of $\mathbf{Z}[\rho]$ ($\rho$ a cube root of unity) on $\mathbf{Z}[\sqrt{-3}]$ (cf. Sommer, Introduction à la théorie des nombres algébriques (trans. A. Lévy), Paris (Hermann), 1911, p. 190).

residues, whose results are derived from a detailed study of divisibility in the ring $\mathbf{Z}[i]$ of "Gaussian integers" ([3], vol. II, p. 109), showed clearly the interest that the extension of divisibility to algebraic numbers could hold out for the classical problems of the theory of numbers (*); therefore it is not surprising that between 1830 and 1850 this theory was the subject of numerous works by German mathematicians, first Jacobi, Dirichlet and Eisenstein, and then, a little later, Kummer and his pupil and friend Kronecker. We shall not speak here of the theory of units, which is too specialized a branch of the theory of numbers, where progress was very rapid, Eisenstein obtaining the structure of the group of units for cubic fields and Kronecker for cyclotomic fields, just before Dirichlet in 1846 ([4], vol. I, p. 640) proved the general theorem, at which Hermite had almost arrived independently ([8], vol. I, p. 159). The question (central to the whole theory) of decomposition into prime factors appeared much more difficult. Since Lagrange had given examples of numbers of the form $x^2 + D y^2$ (x, y, D integers) with divisors which are not of the form $m^2 + D n^2$ ([2], vol. II, p. 465), it was effectively known that the ring $\mathbf{Z}[\sqrt{-D}]$ could not in general be expected to be a principal ideal domain and Euler's temerity was followed by considerable circumspection; when Dirichlet, for example, proves that the relation $p^2 - 5 q^2 = r^5$ ($p, q, r$ integers) is equivalent to

$$
p + q \sqrt{5} = (x + y \sqrt{5})^5
$$

for integers x, y, he restricts himself to pointing out that "there are analogous theorem for many other prime numbers [than 5]" ([4], vol. I, p. 31). In Gauss's memoir of 1831 and the work of Eisenstein on cubic residues [6a], it is certainly true that there are advanced studies on arithmetic in the principal ideal domains $\mathbf{Z}[i]$ and $\mathbf{Z}[\rho]$ ($\rho = (-1 + i \sqrt{3})/2$, a cube root of unity) in perfect analogy with the theory of rational integers and in these examples at least the close connection between arithmetic in quadratic fields and the theory of binary quadratic forms developed by Gauss was very apparent; but the general case lacked a "dictionary" which would have allowed quadratic fields to be treated by a simple translation from Gauss's theory (†).

In fact, it is not for quadratic fields but for cyclotomic fields (and for reasons which will only appear clearly much later (cf. p. 585)) that the problem was

(*) The research of Gauss on division on the lemniscate and elliptic functions related to this curve, not published during his lifetime, but dating from about 1800, must have led him from this time to consider the arithmetical properties of the ring $\mathbf{Z}[i]$, division by numbers in this ring playing an important role in the theory; see what Jacobi say on this subject ([5], vol. VI, p. 275) and also the calculations related to these questions found in Gauss's papers ([3], vol. II, p. 411; see also [3], vol. X_2, p. 33 et seq.).

† The reader will find an exact discription of this correspondence between quadratic forms and quadratic fields in Sommer, loc. cit., pp. 205–229.

first solved. From 1837 onwards, Kummer, originally an analyst, turns to the arithmetic of cyclotomic fields which was to occupy him almost exclusively for 25 years. Like his predecessors, he studies divisibility in the ring $\mathbf{Z}[\zeta]$, where $\zeta$ is a $p$-th root of unity $\neq 1$ ($p$ an odd prime); he quickly sees that here also rings are encountered which are not principal ideal domains, blocking all progress in the extension of the laws of arithmetic [7a] and it is only in 1845, after 8 years' efforts, that the light dawns, thanks to his definition of "ideal numbers" ([7c] and [7d]).

What Kummer does amounts exactly, in modern language, to defining the valuations on the field $\mathbf{Q}(\zeta)$: they are in one-to-one correspondence with his "ideal prime numbers", the "exponent" with which such a factor appears in the "decomposition" of a number $x \in \mathbf{Z}[\zeta]$ is just the value at $x$ of the corresponding valuation. As the conjugates of $x$ also belong to $\mathbf{Z}[\zeta]$ and their product $N(x)$ (the "norm" of $x (*)$) is a rational integer, the "ideal prime factors" to be defined must also be "factors" of the rational prime numbers and in order to define them it was sufficient just to say what were the "ideal prime divisors" of a prime number $q \in \mathbf{Z}$. For $q = p$ Kummer had already effectively proved [7a] that the principal ideal $(1 - \zeta)$ was prime and that its $(p - 1)$-th power was the principal ideal $(p)$; this case therefore raised no new problem. For $q \neq p$ the idea which seems to have guided Kummer is to replace the cyclotomic equation $\Phi_p(z) = 0$ by the congruence $\Phi_p(u) \equiv 0 \pmod{q}$, in other words to decompose the cyclotomic polynomial $\Phi_p(X)$ over the field $\mathbf{F}_q$ and to associate with each irreducible factor of this polynomial an "ideal prime factor". A simple case (explicitly mentioned in the Note [7b] where Kummer announces his results without proof) is that where $q \equiv 1 \pmod{p}$; if $q = mp + 1$ and $y \in \mathbf{F}_q$ is a primitive $(q - 1)$-th root of 1, then, in $\mathbf{F}_q[X]$,
$$
\Phi_p(X) = \prod_{k=1}^{q-1} (X - \gamma^{km})
$$

(*) The notion of norm of an algebraic number goes back to Lagrange: if $\alpha_i$ ($1 \leq i \leq n$) are the roots of a polynomial of degree $n$, he even considers the "norm form" $N(x_0, x_1, \ldots, x_{n-1}) = \prod_{i=1}^n (x_0 + \alpha_i x_1 + \cdots + \alpha_i^{n-1} x_{n-1})$ in the variables $x_i$

which was no doubt suggested to him by his research on the solution of equations and "Lagrange resolvents" ([2], vol. VII, p. 170). It is to be noted that it is the multiplicative property of the norm which leads Lagrange to his identity on binary quadratic forms, whence Gauss was able to obtain the "composition" of these forms ([2], vol. II, p. 522). On the other hand, when the theory of algebraic numbers comes into being about 1830, it is very often in the form of the solution of equations $N(x_0, \ldots, x_{n-1}) = \lambda$ (in particular with $\lambda = 1$ in research on units) or the study of "norm forms" (also called "decomposable forms") that the problems are presented; and even in recent works, the properties of these particular Diophantine equations are used fruitfully, notably in the theory of p-adic numbers (Skolem, Chabauty).

since $\gamma^{pm} = 1$. Then associating with each factor $X - \gamma^{km}$ an "ideal prime factor" $q_k$ of $q$, Kummer says that an element $x \in \mathbf{Z}[\zeta]$, of which P is the minimal polynomial over $\mathbf{Q}$, is divisible by $q_k$ if in $\mathbf{F}_q$, $P(\gamma^{km}) = 0$; to sum up, in modern language, he writes the quotient ring $\mathbf{Z}[\zeta]/q\mathbf{Z}[\zeta]$ as a direct composition of fields isomorphic to $\mathbf{F}_r$. For $q \not\equiv 1 \pmod{p}$, the irreducible factors of $\Phi_p(X)$ in $\mathbf{F}_q[X]$ are no longer of first degree and it would therefore be necessary to substitute for X in $P(X)$ "Galois imaginary" roots of the factors of $\Phi_p$ in $\mathbf{F}_q[X]$. Kummer avoids this difficulty by passing, as we would say today, to the decomposition field K of $q$; iff is the least integer such that $q^f \equiv 1 \pmod{p}$ and $p - 1 = ef$, K is just the subfield of $\mathbf{Q}(\zeta)$ consisting of the invariants of the subgroup of order f of the Galois group (cyclic of order $p - 1$) of $\mathbf{Q}(\zeta)$ over $\mathbf{Q}$; in other words it is the unique subfield of $\mathbf{Q}(\zeta)$ which is of degree e over $\mathbf{Q}$; it had been well known since Gauss's Disquisitiones, being generated by the "periods"

$$
\eta_k = \zeta_k + \zeta_{k+f} + \zeta_{k+2f} + \cdots + \zeta_{k+(e-1)f}
$$

$(0 \leq k \leq e-1, \zeta_v = \zeta^{g^v}$ where g is a primitive root of the congruence $z^{p-1} \equiv 1 \pmod{p}$), which form a normal basis for it. If $R(X)$ is the minimal polynomial (monic and with rational integer coefficients) of any of these "periods" $\eta$, Kummer, starting from Gauss's formulae, proves that, over the field $\mathbf{F}_r$, $R(X)$ also decomposes into distinct factors of the first degree $X - u_j$ ($1 \leq j \leq e$) and it is with each of the $u_j$ that he now associates an "ideal prime factor" $q_j$. To define "divisibility by $q_j$", Kummer writes every $x \in \mathbf{Z}[\zeta]$ in the form $x = \sum_{k=0}^{f-1} \gamma^k y_k$, where each $y_k \in K$ may itself be written uniquely as a polynomial of degree $\leq e - 1$ in $\eta$ with rational integer coefficients; he says that $x$ is divisible by $q_j$ if and only if, when $u_j$ is substituted for $\eta$ in each of the $y_k$, the elements of F, obtained are all zero. But it was also necessary to define the "exponent" of $q_j$ in $x$. For this, Kummer introduces what we would now call a uniformizer for $q_j$, that is an element $\rho_j \in K$ such that $N(\rho_j) \equiv 0 \pmod{q}$, $N(\rho_j) \not\equiv 0 \pmod{q^2}$ and finally such that $\rho_j$ is divisible by $q_j$ (in the sense defined above) but by none other of the ideal factors $\neq q$, of $q$. The existence of such a $\rho_j$ had effectively been proved by Kronecker in his dissertation the previous year ([9a], p. 23); then writing $\rho = N(\rho_j)/\rho_j$, Kummer says that the exponent of $q_j$ in $x$ is equal to h if $x\rho_j^h \equiv 0 \pmod{q^h}$ but $x\rho_j^{h+1} \not\equiv 0 \pmod{q^{h+1}}$; he begins of course by proving that the relation $x\rho_j' \equiv 0 \pmod{q}$ is equivalent to the fact that $x$ is divisible by $q_j$ (in the above sense). Once these definitions were made, the extension to $\mathbf{Z}[\zeta]$ of the usual laws of divisibility for "ideal numbers" no longer offered serious difficulty; and from his first memoir [7c] Kummer could even, using Dirichlet's "box method", show that the "classes" and "ideal factors" were finite in number (*).

(*) He does no more than reproduce an argument of Kronecker in his disser-

We shall not pursue the history of Kummer’s later works on cyclotomic fields, concerning the determination of the class number and the application to the proof of Fermat’s theorem in certain cases. Let us just mention the way in which, in 1859, he extends his method to obtain (at least partially) the “ideal prime numbers” in a “Kummerian field” $\mathbf{Q}(\zeta, \mu)$, where $\mu$ is a root of the irreducible polynomial $P(X) = X^p - \alpha$, where $\alpha \in \mathbf{Z}[\zeta]$ [7e]. It is interesting that Kummer envisages the problem precisely by considering $\mathbf{Q}(<+)$ as a cyclic extension of the field $\mathbf{Q}(\zeta)$ taken as “base field” (†): he starts with an “ideal prime number” $q$ of $\mathbf{Z}[\zeta]$ which he assumes divides neither $p$ nor $\alpha$ and this time he examines (in modern terms) the polynomial $\overline{P}(X) = X^p - \bar{\alpha}$ in the residue field $k$ of the valuation on $\mathbf{Q}(\zeta)$ corresponding to $q$ ($\bar{\alpha}$ being the canonical image of $a$ in $k$). As $\mathbf{Q}(\zeta)$ is the field of the $p$-th roots of unity, $\overline{P}$ is, either irreducible over $k$, or the product of factors of the first degree. In the first case, Kummer says that $q$ remains prime in $\mathbf{Z}[\zeta, \mu]$; in the second, he introduces elements $w_i$ ($1 \leq i \leq p$) of $\mathbf{Z}[\zeta]$ whose images in $k$ are the roots of $\overline{P}$ and he associates with each index $i$ an ideal prime factor $r_i$ of $q$; then writing $W_i(X) = \prod_{j \neq i} (X - w_j)$, he says that, for a polynomial $f$ with coefficients in $\mathbf{Z}[\zeta], f(\mu)$ contains the factor $r_i$ $m$ times if
$$
f(w_i) W_i^m(w_i) \equiv 0 \pmod{q^m}
$$
but
$$
f(w_i) W_i^{m+1}(w_i) \not\equiv 0 \pmod{q^{m+1}}.
$$
To sum up, he obtains in this way the valuations on $\mathbf{Q}(\zeta, \mu)$ which are unramified over $\mathbf{Q}$, which are sufficient for the applications he has in view.

\*   \*   \*

Kummer had had the chance to meet, in studying particular fields to which his research on Fermat’s Theorem had led at first, a number of fortuitous circumstances which made their study much more accessible. The extension to the tation, relating to the classes of solutions of equations of the form
$$
N(x_0, x_1, \ldots, x_{n-1}) = a
$$
([9a], p. 25). On the other hand, Kummer makes several allusions to results obtained by Dirichlet on equations of this type (for any algebraic number field); but these results have neither been published nor found among Dirichlet’s papers.

(†) In his memoir on quadratic forms with coefficients in the ring of Gaussian integers ([4], vol. I, pp. 533–618) Dirichlet had in various places been led to consider the relative norm of the field $\mathbf{Q}(\sqrt{D}, i)$ over its quadratic subfield $\mathbf{Q}(\sqrt{D})$. Similarly, Eisenstein, studying the 8-th roots of unity, considers the field they generate as a quadratic extension of $\mathbf{Q}(i)$ and uses the norm relative to this sub-field ([&], p. 253). But the work of Kummer is the first example of profound arithmetical study of a “relative field”.

general case of Kummer’s results presented considerable difficulties and was to take years of effort.

With Kronecker and Dedekind, who play the principal roles there, the history of the theory of algebraic numbers, during the 40 years following Kummer’s discovery, is not dissimilar (but happily without the same acrimony) to that of the rivalry of Newton and Leibniz 180 years earlier concerning the invention of Infinitesimal Calculus. Pupil and later colleague of Kummer in Berlin, Kronecker (whose thesis, as we have seen, had served as an essential point in Kummer’s theory) was greatly interested in “ideal numbers” with the aim of applying them to his own research; and we admire his astonishing penetration when we see him, as early as 1853 ([9b], p. 10) announce the general theorem on the structure of Abelian extensions of $\mathbf{Q}$ and, what is perhaps still more remarkable, create, in the years which follow, the theory of complex multiplication and discover the first germ of class field theory ([9c] and [9d]). A letter from Kronecker to Dirichlet in 1857 ([9], vol. 5, pp. 418–421) shows that he already possessed at that time a generalization of Kummer’s theory, which moreover Kummer himself confirms in one of his own works ([7e], p. 57) and Kronecker will make many an allusion to this theory in his memoirs between 1860 and 1880 (*).

But although at that time none of the mathematicians of the German school of the Theory of Numbers was unaware of the existence of these works of Kronecker, the latter seems only to have communicated the principles of his methods to a restricted circle of friends and pupils and when he finally decided to publish them in his memoir of 1881 on the discriminant [9e] and above all in his great “Festschrift” of 1882 [9f], Dedekind could not refrain from expressing his surprise ([10], vol. III, p. 427), having imagined the processes were completely different, from the echoes he had heard ([10], vol. III, p. 287). Kronecker moreover was far from possessing to the same degree Dedekind’s remarkable gifts of exposition and clarity and it is therefore not surprising that it is chiefly the methods of the latter, already published in 1871, which have formed the framework of the theory of algebraic numbers; however interesting it may be, Kronecker’s method of the “adjunction of indeterminates”, where the Theory of Numbers is concerned, is scarcely more in our eyes than a variant of Dedekind’s (cf. Chapter VII, § 1, Exercise 31) and it is chiefly in another direction, oriented towards Algebraic Geometry, that Kronecker’s ideas acquire all their importance for the history of Commutative Algebra, as we shall see later.

For reasons which could only clearly be seen much later, a first preliminary to any attempt at a general theory was of course the clarification of the notion of algebraic integer. This is obtained about 1845–50, although it is difficult

(*) On the evolution of his ideas on this subject, see the very interesting introduction to his memoir of 1881 on the discriminant ([9e], p. 195).

enough to date its appearance precisely; it seems probable that it is the idea of a system stable under addition and multiplication (or, more precisely, what we now call a Z-algebra of finite rank) which, more or less consciously, led to the general definition of algebraic integers: in fact this definition is inevitably hit upon when a Z-algebra of the form $\mathbf{Z}[\theta]$ is restricted to being of finite rank, by analogy with the ring $\mathbf{Z}[\zeta]$ generated by a root of unity, which was always at the centre of arithmeticians’ preoccupations at this time. At any rate, when, independently, Dirichlet ([4], vol. I, p. 640), Hermite ([8], vol. I, pp. 115 and 146) and Eisenstein ([6c], p. 236) introduce the notion of algebraic integer, they do not appear to consider that they are dealing with a new concept nor to judge that it will be useful to make a detailed study thereof; only Eisenstein shows effectively (*loc. cit.*) that the sum and product of two algebraic integers are algebraic integers, without moreover claiming that this result is original.

A much more subtle point was the determination of the rings in which a generalization of Kummer’s theory could be expected. The latter, in his first note [7b], does not hesitate to affirm that he can regain by his method Gauss’s theory of binary quadratic forms by considering the rings $\mathbf{Z}[\sqrt{D}]$ (D an integer); he never developed this idea, but it certainly seems that neither he nor any one else before Dedekind perceived that unique composition into “ideal” prime factors is impossible in the ring $\mathbf{Z}[\sqrt{D}]$ when $D \equiv 1 \pmod{4}$ (although the example of the cube roots of unity showed that the ring $\mathbf{Z}[\rho]$ considered from the time of Gauss is distinct from $\mathbf{Z}[\sqrt{-3}]$) (*). Before Dedekind and Kronecker, the only rings studied are always of the type $\mathbf{Z}[\theta]$ or sometimes certain particular rings of the type $\mathbf{Z}[\theta, \theta']$ (†). As far as Kronecker is concerned, it is possible that the idea of considering *all* the integers of an algebraic extension was first suggested to him by the study of the field of algebraic functions, where this ring arises naturally as the set of functions which are “finite at infinite distance”; in any case he insists in his memoir of 1881 on the discriminant (written and announced at the Academy of Berlin as early as 1862) on this characterization of the “integers” in these fields [9e]. Dedekind gives no indication as to the origin of his own ideas on this point, but in his very first publication on number fields in 1871 the ring of all integers of such a field plays a capital role in his theory; it is also Dedekind who clarifies the relation between such a ring and its subrings with the same field of fractions, by the introduction of the notion of *conductor* [10c].

(*) Although Kronecker must have been led to study the arithmetic of the rings $\mathbf{Z}[\sqrt{-D}]$ ($D > 0$) by his work on complex multiplication, he published nothing on this subject and the characterization of the integers of any quadratic field $\mathbf{Q}(\sqrt{D})$ is given explicitly for the first time by Dedekind in 1871 ([10c], pp. 105–106).

(†) We have seen earlier the example of the ring $\mathbf{Z}[\zeta, \mu]$ introduced by Kummer [7e]. Earlier, Eisenstein had been led to envisage a subring generated by two elements of the ring of integers in the field of the 21st roots of unity [6b].

But here was not the only difficulty. To generalize the ideas of Kummer, it was necessary first to get rid of passing via the decomposition field, which naturally could have no analogue in the case of a non-Abelian field. This detour seems moreover at first sight very surprising and artificial, for, starting with the irreducible polynomial $\Phi_p(X)$ of $\mathbf{Z}[X]$, one may wonder why Kummer does not push his ideas to their logical conclusion and what prevents him from using the theory of "Galois imaginary" numbers which were well known at the time. The obstacle comes more clearly to light in an unfortunate attempt at generalization made as early as 1865 by Selling, a pupil of Dedekind: given an irreducible polynomial $P \in \mathbf{Z}[X]$, Selling decomposes the corresponding polynomial $\overline{P}(X)$ into irreducible factors in $\mathbf{F}_q[X]$; the roots of this polynomial therefore belong to a finite extension $F$, of $\mathbf{F}_q$; but Selling, in order to define in Kummer's way the exponent of an "ideal prime factor" of $q$ in an integer of the splitting field of $P(X)$, does not hesitate to speak, *in the field* $\mathbf{F}_r$, of congruences modulo a *power of* $q$ ([11], p. 26); and a little later when he tries to approach the question of ramification, he "adjoins" to $\mathbf{F}_r$ "imaginary roots" of an equation of the form $x^h = q$ ([11], p. 34). Clearly these bold steps (which would be justified were the finite field $\mathbf{F}_q$ replaced by the $q$-adic field) could at that time only end in nonsense. Fortunately, Dedekind in 1857 [10a], under the name of "theory of higher congruences", took up again in another form the theory of finite fields (*): he interprets the elements of the latter as "residues" of the polynomials of $\mathbf{Z}[X]$ with respect to a "double modulus" consisting of the linear combinations with coefficients in $\mathbf{Z}[X]$ of a prime number $p$ and an irreducible monic polynomial $P \in \mathbf{Z}[X]$ (which is no doubt for him, as for Kronecker, the origin of the general idea of *module* at which they were to arrive independently a little later). According to his own testimony ([10d], p. 218) it seems that Dedekind had begun by attacking the problem of the "ideal factors" of $p$ in a field $\mathbf{Q}(\xi)$, where $P \in \mathbf{Z}[X]$ is the minimal polynomial of $\xi$, as follows (certainly at least in the "unramified" case, that is when the polynomial $p$ in $\mathbf{F}_p[X]$ corresponding to $P$ has no multiple root): he writes, in $\mathbf{Z}[X]$,

$$
P = P_1 P_2 \ldots P_h + p \cdot G
$$

where the $\overline{P}_i$ are irreducible and distinct in $\mathbf{F}_p[X]$; it may be assumed that $G$ is not divisible (in $\mathbf{Z}[X]$) by any of the $P_i$ and for all $i$ he writes $W_i = \prod_{j \neq i} P_j$; then, if $f \in \mathbf{Z}[X]$, it will be said that $f(\xi)$ contains the "ideal factor" $p_i$ of $p$

(*) It is known that certain results of this theory, published first by Galois, had been obtained (in the language of congruences) by Gauss about 1800; after the death of Gauss, Dedekind was charged with the publication of part of his works and had rediscovered in particular in the papers left by Gauss the memoir on finite fields ([3], vol. II, pp. 212–240).

corresponding to $P_i$ $k$ times if

$$
f W_i^k \equiv 0 \pmod{p^k, P}
$$

and

$$
f W_i^{k+1} \not\equiv 0 \pmod{p^{k+1}, P}.
$$

The relationship with the method followed by Kummer for "Kummerian fields" is here manifest and Kummer's original definition for cyclotomic fields can, in this way, easily be recovered (see for example the work of Zolotareff [14] who, at first independently of Dedekind, developed these ideas a little later).

However, neither Dedekind nor Kronecker who appears also to have made analogous attempts, could progress further in this direction, both of them halted by the difficulties presented by ramification ([10d], p. 218 and [9f], p. 325) (*). If the ring of integers $\mathbf{A}$ of the number field $K$ under consideration admits a basis (over $\mathbf{Z}$) consisting of the powers of the same integer $\theta$, it is not difficult to generalize the above method for ramified prime numbers in $\mathbf{Z}[\theta]$ (as Zolotareff indicates *loc. cit.*)). But there are fields $K$ where no basis of this type exists in the ring $\mathbf{A}$; and Dedekind even finished by discovering that there are cases where certain prime numbers $p$ (the "extraordinary factors of the discriminant" of the field $K$) are such that, *for all* $0 \in \mathbf{A}$, applying the above method of the minimal polynomial of $0$ over $\mathbf{Q}$ leads to attributing top multiple ideal factors when in fact $p$ is unramified in $\mathbf{A}$ ($\dagger$); he admits that he was held up for a long time by this unforeseen difficulty, before managing to surmount it by the creation from scratch of the theory of modules and ideals, in a masterly exposition (and already in a wholly modern style, in contrast with the discursive style of his contemporaries) in what is without doubt his masterpiece, the famous "11th supplement" to Dirichlet's book on the Theory of Numbers [10f]. This work saw three successive versions, but already in the first (published as the "10th supplement" to the second edition of Dirichlet's book in 1871 [4 bis]) the essentials of the method are present and almost at one stroke the theory of algebraic numbers passes from sketches and earlier gropings to a fully mature discipline already possessing its essential tools: from the beginning, the ring of all integers of a number field is placed at the centre of the theory; Dedekind proves the existence of a basis of this ring over $\mathbf{Z}$ and

(*) Zolotareff circumvents the difficulty by a refinement of his method which appears of little more than anecdotal interest [14].

($\dagger$) Kronecker claims to have come across the same phenomenon in a subfield of the field of the 13th roots of unity which he does not describe more precisely ([9f], p. 384). The example of an extraordinary factor of the discriminant given by Dedekind is treated in detail in Hasse, Zahlentheorie (Berlin, Akad. Verlag, 1949), p. 333; a little later, Hasse gives an example of a field $K$ where there is no extraordinary factor of the discriminant, but where there exists no $\theta \in \mathbf{A}$ such that $\mathbf{A} = \mathbf{Z}[\theta]$ (*loc. cit.*, p. 335).

deduces from it the definition of the discriminant of the field as the square of the determinant formed by the elements of a basis of the ring of integers and their conjugates; however he only gives in the 11th supplement the characterization of ramified prime numbers (as prime factors of the discriminant) for quadratic fields ([10f], p. 202), whereas he was in possession of the general theorem from 1871 onwards (*). The central result of the work is the existence and uniqueness theorem for the decomposition of ideals into prime factors, for which Dedekind starts by developing an elementary theory of “modules”; in fact, in the 11th supplement, he reserves this name for sub-Z-modules of a number field, but the conception he forms of them and the results he shows are already expounded in a way which is immediately applicable to general modules (†); amongst other things must be noted, as early as 1871, the introduction of the notion of “transporter” which plays an important role (as well as the “ascending chain condition”) in the first proof of the unique factorization theorem. In the two following editions, Dedekind was also to give two other proofs of this theorem which he justly considered as the cornerstone of his theory. It should be noted here that it is in the third proof that fractional ideals are made use of (already introduced as early as 1859 by Kummer for cyclotomic fields) and the fact that they form a group is established; we shall return later to the second proof (p. 594).

All these results (except for the language) were no doubt already known to Kronecker about 1860 as particular cases of his more general conceptions of which we speak later (whereas Dedekind recognizes that he only surmounted the last difficulties of his theory in 1869–70 ([10e], p. 351)) (‡); as far as number fields are concerned, it must in particular be underlined that, already at this time, Kronecker knew that the whole theory is applicable without essential change starting with a “base field” k which is itself a number field (other than $\mathbf{Q}$), a point of view to which the theory of complex multiplication led naturally; he had thus recognized, for certain fields k, the existence of algebraic extensions $K \neq k$ unramified over k ([9f], p. 269), a fact which cannot hold for $k = \mathbf{Q}$ (as follows from minorations of Hermite and Minkowski for the discriminant). Dedekind was never to develop this last point of view (although he indicates its possibility in his memoir of 1882 on the different) and the first systematic exposition of “relative field” theory is due to Hilbert [16d].

(*) He only gives the proof of this theorem in his memoir of 1882 on the different [10e].
(†) In his memoir of 1882 on algebraic curves (jointly with H. Weber) [10 bis], he uses the theory of modules over the ring $\mathbf{C}[X]$ in the same way.
(‡) Kronecker had however not succeeded in obtaining by his methods the complete characterization of ramified ideals in the case of number fields. On the other hand he does have this characterization for fields of algebraic functions of one variable and proves moreover that in this case there is no “extraordinary factor” of the discriminant [9e].

Finally, in 1882 [10e], Dedekind completes the theory by introducing the different, which gives him a new definition of the discriminant and allows him to define precisely the exponents of the ideal prime factors in the decomposition of the latter. It is also about this time that he becomes interested in the particular features presented by Galois extensions, introducing the notions of decomposition group and inertia group (in his memoir [10g] which was only published in 1894) and even (in papers not published during his lifetime ([10], vol. 11, pp. 410–411)) a sketch of ramification groups, which Hilbert (independently of Dedekind) was to develop a little later ([16c] and [16d]).

Thus, about 1895, the theory of algebraic numbers had completed the first stage of its development; the tools forged during this formation period will allow it almost immediately to enter the next stage, general class field theory (or, what amounts to the same, the theory of Abelian extensions of number fields) which carries on to our own day and which we shall not describe here. From the point of view of Commutative Algebra, it may be said that at the same time the history of Dedekind domains is practically completed, setting aside their axiomatic characterization, and also the structure of finitely generated modules over these domains (which, in the case of number fields, will only be substantially elucidated by Steinitz in 1912 [20b]) (*).

\*   \*   \*

The later progress in Commutative Algebra arises chiefly from quite different problems, issuing from Algebraic Geometry (which will moreover influence the Theory of Numbers directly even before the "abstract" developments of the present period).

We shall not concern ourselves here with the detailed history of Algebraic Geometry which, until the death of Riemann, scarcely touches our subject. Let it suffice to recall that it was mainly concerned with the study of algebraic curves in the complex projective plane, usually approached by projective geometric methods (with or without the use of coordinates). There was a parallel development, with Abel, Jacobi, Weierstrass and Riemann, of the theory of "algebraic functions" of one complex variable and their integrals; mathematicians were obviously conscious of the connection between this theory and the geometry of plane algebraic curves and even on occasions were known to "apply Analysis to Geometry"; but the methods used for the study of algebraic functions were chiefly of a "transcendental" nature, even before Riemann (†); this character is still further accentuated in the work of the latter,

(*) A start to the study of modules over a ring of algebraic numbers had already been made by Dedekind [10h].

(†) It must be noted however that Weierstrass, in his research on Abelian functions (which goes back to 1857 but was only expounded in his lectures about 1865 and only published in his complete Works ([17], vol. IV)), gives, in contrast with the introduction of "Riemann surfaces" and arbitrary analytic functions defined on such a surface. Almost immediately after the death of Riemann, Roch and above all Clebsch recognized the possibility of obtaining from the profound results obtained by Riemann's transcendental methods numerous striking applications to the projective geometry of curves, which was of course to incite contemporary geometers to give purely "geometric" proofs of these results; this programme, incompletely followed by Clebsch and Gordan, was completed by Brill and M. Noether several years later [13], with the aid of the study of systems of variable points on a given curve and auxiliary curves (the "adjoints") passing through such systems of points. But even for his contemporaries, Riemann's transcendental methods (and notably his use of topological notions and of "Dirichlet's principle") appeared to rest on uncertain foundations; and although Brill and Noether are rather more careful than most contemporary "synthetic" geometers (see below p. 593), their geometric-analytic methods are not safe from all reproach. It is essentially to give the theory of plane algebraic curves a solid basis that Dedekind and Weber published in 1882 their great memoir on this subject [10 bis]: "The researchpublished below", they say, "is intended to lay thefoundations of the theory & algebraicfunctions of one variable, one of Riemann's principal creations, in a way which is at the same time simple, rigorous and entirely general. In earlier research on this subject, in general restrictive hypotheses have been made on the singularities of thefunctions considered and the would-be exceptional cases are, either mentioned in passing as limiting cases, or entirely neglected. Similarly, certainfundamental theorem on continuity or analyticity are accepted, whose "evidence" depends on geometric intuitions of a varied nature" ([10 bis], p. 181) (*).

to Riemann, a purely algebraic definition of the genus of a curve, as the least integer $p$ such that there are rational functions on the curve with poles at $p + 1$ given arbitrary points. It is interesting to point out that, seeking to obtain elements which serve as functions with only one pole on the curve, Weierstrass, before finally using for this purpose transcendental functions, had, according to Kronecker ([9e], p. 197), urged the latter to extend to algebraic functions of one variable the results he had at that time just obtained for number fields ("ideal prime factors" effectively playing the role desired by Weierstrass).

(*) It is well known that, in spite of the efforts of Dedekind, Weber and Kronecker, the laxness in the conception of what constituted a correct proof, already visible in the German school of Algebraic Geometry of the years 1870–1880, was only to be aggravated more and more in the work of French and above all Italian geometers of the next two generations, who, following the German geometers and developing their methods, attack the theory of algebraic surfaces: a "scandal" often denounced (chiefly since 1920) by algebraists, but to a certain extent justified by the brilliant successes achieved by these "non-rigorous" methods, contrasting with the fact that, until about 1940, the orthodox successors of Dedekind had shown themselves incapable of formulating with sufficient flexibility and power the algebraic notions which would have allowed correct proofs to be given of these results.

The essential idea of their work is to model the theory of algebraic functions of one variable on the theory of algebraic numbers as Dedekind had just developed it; to do this, they must first look at it from an “affine” point of view (in contrast with their contemporaries, who invariably considered algebraic curves as imbedded in complex projective space): they therefore start with a finite algebraic extension K of the field $\mathbf{C}(X)$ of rational functions and the ring A of “integral algebraic functions” in K, i.e. the elements of this field which are integral over the polynomial ring $\mathbf{C}[X]$; their fundamental result, which they obtain without using any topological consideration (*), is that A is a Dedekind domain, to which may be applied mutatis mutandis (and even, as Dedekind and Weber remark, without yet clearly seeing the reason ([10], vol. I, p. 268), in a simpler way) all the results of the “11th supplement”. Having done this, they prove that their theorems are in fact birationally invariant (in other words, depend only on the field K) and in particular do not depend on the choice of the “line at infinity” made at the beginning. What is no doubt still more interesting for us, is that, in order to define the points of the “Riemann surface” corresponding to K (and in particular the “points at infinity”, which cannot correspond to ideals of A), they are led to introduce the notion of place of the field K: They find themselves in the same situation as Gelfand will find himself in 1940 when founding the theory of normed algebras, knowing a set K of elements which are not given to start with as functions and yet one wants to consider as such; and, to obtain the defining set of hypothetical functions, they have for the first time the idea (which Gelfand followed and which has become commonplace through being used at every turn in modern mathematics) of associating with a point x a set E and with a set $\mathcal{F}$ of mappings of E to a set G the mapping $f \mapsto f(x)$ of $\mathcal{F}$ to G, in other words of considering, in the expression $f(x)$, $f$ as variable and $x$ as fixed, in contrast with the classical tradition. Finally, they have no difficulty, starting from the notion of place, in defining “positive divisors” (“Polygon” in their terminology) which include the ideals of A as particular cases and correspond to the “systems of points” of Brill and Noether; but, although they write principal divisors and divisors of differentials as “quotients” of positive divisors, they do not give the general definition of divisors and it is only in 1902 that Hensel and Landsberg introduce, by analogy with fractional ideals, this notion which will always embarrass the champions of purely “geometric” methods (obliged in spite of themselves to define them with the name “virtual systems”, but uneasy at not being able to give them a “concrete” interpretation).

The same year 1882 also sees appear Kronecker’s great memoir awaited for more than 20 years [9f]. Much more ambitious than the work of Dedekind-

(*) They underline that, thanks to this fact, all their results would remain valid if the field $\mathbf{C}$ were replaced by the field of all algebraic numbers ([10], vol. I, p. 240).

Weber, it is also unfortunately much more vague and obscure. Its central theme is (in modern language) the study of the ideals of a finite integral algebra over one of the polynomial rings $\mathbf{C}[X_1, \ldots, X_n]$ or $\mathbf{Z}[X_1, \ldots, X_n]$; Kronecker limits himself $a\ priori$ to those ideals which are finitely generated (the fact that they all are was only to be proved (for the ideals of $\mathbf{C}[X_1, \ldots, X_n]$)) some years later by Hilbert in the course of his work on invariants [16a]). As far as $\mathbf{C}[X_1, \ldots, X_n]$ or $\mathbf{Z}[X_1, \ldots, X_n]$ is concerned, this naturally led to associating with each ideal of one of these rings the "algebraic variety" consisting of the zeros common to all the elements of the ideal; and the study of geometry in 2 and 3 dimensions during the 19th century was to lead intuitively to the idea that every variety is a union of a finite number of "irreducible" varieties whose "dimensions" are not necessarily all the same. It seems that the proof of this fact is the aim Kronecker sets himself, although he nowhere says so explicitly and no definition of "irreducible variety" can be found in his memoir, nor of "dimension". In fact, he limits himself to indicating summarily how a general elimination method (*) gives, starting with a system of generators of the ideal considered, a finite number of algebraic varieties for each of which, in a suitable coordinate system, a certain number of coordinates are arbitrary and the others are "algebraic functions" of them (†). But if it is indeed the decomposition into irreducible varieties at which Kronecker is aiming, it must be recognized that he only arrives there in the elementary case of a principal ideal, where he proves effectively, extending a classical lemma of Gauss on $\mathbf{Z}[X]$ ([3], vol. I, p. 34), that the domains $\mathbf{C}[X_1, \ldots, X_n]$ and $\mathbf{Z}[X_1, \ldots, X_n]$ are factorial; and, in the general case, it is questionable whether Kronecker was in possession of the notion of prime ideal (what he calls "Primmodulsystem" is an ideal which is indecomposable as a product of two others ([9f], p. 336); this is all the more astonishing as the definition already given by Dedekind in 1871 was perfectly general).

It must however be said that Kronecker's elimination method, suitably applied, certainly leads to the decomposition of an algebraic variety into its irreducible components: this is clearly established by E. Lasker at the beginning of his great memoir of 1905 on polynomial ideals [19]; he defines correctly the

(*) By a linear change of coordinates, it may be assumed that the generators $F_i$ ($1 \leq i \leq r$) of the ideal are polynomials where the term of highest degree in $X_1$ is of the form $c_i X_1^{m_i}$, where $c_i$ is a constant $\neq 0$. It may also be assumed that the $F_i$ have no common factor. Consider then for $2r$ indeterminates $u_i, v_i$ ($1 \leq i \leq r$) the polynomials $\sum_{i=1}^r u_i F_i$ and $\sum_{i=1}^r v_i F_i$ as *polynomials in* $X_1$; form their Sylvester resultant, which is a polynomial in the $u_i$ and $v_i$ with coefficients in $\mathbf{C}[X_2, \ldots, X_n]$ (resp. $\mathbf{Z}[X_2, \ldots, X_n]$); by annihilating these coefficients, a system of equations is obtained whose solutions $(x_2, \ldots, x_n)$ are precisely the projections of the solutions $(x_1, \ldots, x_n)$ of the system of equations $F_i(x_1, x_2, \ldots, x_r) = 0$ ($1 \leq i \leq r$). The application of the method may then be continued by induction on $n$.

(†) It is this number of arbitrary coordinates that he calls the *dimension* ("Stufe").

notion of irreducible variety (in $\mathbf{C}^n$) as an algebraic variety V such that a product of two polynomials can only be zero on the whole of the variety V if one of them is and he also gives a definition which is independent of the choice of axes. In the interesting historical considerations he inserts in this work, Lasker shows that he is interested, not only in the purely algebraic tendencies of Kronecker and Dedekind, but also in the problems raised by the geometric methods of the school of Clebsch and M. Noether and notably in the famous theorem proved by the latter in 1873 [12]. He is essentially concerned, as we would say today, with determining the ideal $\mathfrak{a}$ of polynomials of $\mathbf{C}[X_1, \ldots, X_n]$ which are zero at the points of a given set M of $\mathbf{C}^n$; usually M was the "algebraic variety" of zeros common to polynomialsf, finite in number and for a long time it seems that it was accepted (of course without justification) that, at least for $n = 2$ or $n = 3$, the ideal $\mathfrak{a}$ was simply generated by thef, (*). M. Noether had shown that even for $n = 2$ and for two polynomials $f_1, f_2$ this is generally false and he had given sufficient conditions for $\mathfrak{a}$ to be generated by $f_1$ and $f_2$. Ten years later, Netto proves that, with no hypothesis on $f_1$ and $f_2$, a power of $\mathfrak{a}$ is always contained in the ideal generated by $f_1$ and $f_2$ [15], a theorem which Hilbert generalized in 1893 in his celebrated Nullstellensatz [16b]. No doubt inspired by this result, Lasker, in his memoir, introduces the general notion of primary ideal (†) in the rings $\mathbf{C}[X_1, \ldots, X_n]$ and $\mathbf{Z}[X_1, \ldots, X_n]$ (after having given for these rings the definition of prime ideal, by transcribing Dedekind's definition) and shows (*) the existence of a primary decomposition

(*) See the remarks of M. Noether at the beginning of his memoir [13]. It is interesting to note on this subject that, according to Lasker, Cayley, about 1860, had conjectured that for every twisted algebraic curve in $\mathbf{C}^3$ there were a finite number of polynomials generating the ideal of polynomials of $\mathbf{C}[X, Y, Z]$ which are zero on the curve (in other words, a particular case of Hilbert's finiteness theorem [16a]).

(†) Examples of primary ideals which are not powers of prime ideals had been encountered by Dedekind in "orders", i.e. rings of algebraic numbers with a given number field as field of fractions ([10], vol. III, p. 306). Kronecker also gives as an example of an ideal "indecomposable" as a product of two other non-trivial ideals, the ideal of $\mathbf{Z}[X]$ generated by $p^2$ and $X^2 + p$, where $p$ is a prime number (an ideal which is primary for the prime ideal generated by $X$ and $p$ ([9f], p. 341)).

(‡) Lasker proceeds by induction on the maximal dimension $h$ of the irreducible components of the variety V of zeros of the ideal $\mathfrak{a}$ under consideration. In modern terms, he considers first the prime ideals $\mathfrak{p}_i$ ($1 \leq i \leq r$) containing $\mathfrak{a}$, which correspond to the irreducible components of maximal dimension $h$ of V. With each $\mathfrak{p}_i$ he associates the saturation $q_i$ of $\mathfrak{a}$ with respect to $\mathfrak{p}_i$ (cf. Chapter IV, § 2, no. 3, Proposition 5); he then considers the transporter $b_i = \mathfrak{a} : q_i$ of $q_i$ in $\mathfrak{a}$, takes in $\sum b_i$ an element c belonging to none of the $\mathfrak{p}_i$ and shows on the one hand that $\mathfrak{a}$ is the intersection of the $q_i$ and $\mathfrak{a} + (c) = \mathfrak{a}'$ and on the other that the variety V' of for every ideal in these rings (*). He does not seem to be concerned with questions of uniqueness in this decomposition; it is Macaulay who, a little later [21] introduces the distinction between "immersed" and "non-immersed" primary ideals and shows that the latter are determined uniquely, but not the former. It should finally be noted that Lasker also extends his results to the ring of convergent power series in a neighbourhood of a point, by using Weierstrass's "preparation theorem". This part of his memoir is no doubt the first place this ring had been considered from a purely algebraic point of view and the methods which Lasker develops on this occasion were strongly to influence Krull when in 1938 he created the general theory of local rings (cf. [29d], p. 204 and passim).

\*   \*   \*

The movement of ideas which will give birth to modern Commutative Algebra begins to take shape about 1910. If the general notion of field was reached by the beginning of the 20th century, in contrast the first work where the general notion of ring is defined is probably that of Fraenkel in 1914 [23]. At this time, there were already as examples of rings, not only the integral domains of the Theory of Numbers and Algebraic Geometry, but also rings of power series (formal and convergent) and finally algebras (commutative or not) over a base field. However, for the theory of fields as well as that of rings, the catalyst role seems to have been played by Hensel's theory of $p$-adic numbers, which Fraenkel and also Steinitz [20a] mention specially as the starting point of their research.

Hensel's first publication on this subject goes back to 1897; he there starts from the analogy shown by Dedekind and Weber between the points of a Riemann surface of an algebraic function field K and the prime ideals of a number field $k$; he proposes to carry over to the Theory of Numbers "Puiseux expansions" (classical from the middle of the 19th century) which, in a neighbourhood of any point of the Riemann surface of K, allow every element $x \in \mathbf{K}$ to be expressed in the form of a convergent series of powers of the "uniformizer" at the point considered (a series with only a finite number of terms

zeros of $a'$ has only irreducible components of dimension $\leq h - 1$, which allows him to conclude by induction.

(*) It is interesting to note that Dedekind's second proof of the unique decomposition theorem proceeds by first establishing the existence of a unique reduced Primary decomposition; and in a passage not published in the 11th supplement, Dedekind observes explicitly that this part of the proof is valid not only for the ring A of all integers of a number field K, but also for all the "orders" of K ([10], vol. III, p. 303). It is only then, after showing explicitly that A is "completely integrally closed" (to within terminology) that he proves, using this fact, that the primary ideals of the above decomposition are in fact powers of prime ideals ([10], vol. III, p. 307).

with negative exponent). Hensel’s shows similarly that, if $\mathfrak{p}$ is a prime ideal of $k$ lying above a prime number $p$, a “$p$-adic series” may be associated with every $x \in k$, of the form $\sum_i \alpha_i p^i$ (or $\sum_i \alpha_i p^{i/e}$ when $\mathfrak{p}$ is ramified over $p$), the $\alpha_i$ being taken in a given representative system of the field of residues of the ideal $\mathfrak{p}$; but his great originality lies in having had the idea of considering such “expansions” even when they correspond to *no element* of $k$, by analogy with the expansions in integral series of transcendental functions on a Riemann surface [18a].

Throughout the rest of his career, Hensel devotes himself to polishing and perfecting little by little his new calculus; and if his manner seems to us hesitant or ponderous, it must not be forgotten that at the beginning at least he had at his disposal none of the topological or algebraic tools of modern mathematics which would have facilitated his task. In his first publications he moreover scarcely speaks of topological notions and on the whole for him the ring of $p$-adic integers ($\mathfrak{p}$ a prime ideal in the ring of integers $\mathbf{A}$ of a number field $k$) is, in modern terms, the inverse limit of the rings $\mathbf{A}/\mathfrak{p}^n$ for $n$ increasing indefinitely, in a purely algebraic sense; and to establish the properties of this ring and its field of fractions, it is necessary at each step to use more or less painfully *ad hoc* arguments (for example to prove that the $p$-adic integers form an integral domain). The idea of introducing topological notions into a $p$-adic field does not appear in Hensel’s works before 1905 [18d]; and it is only in 1907, after having published the book where he reexpounds the theory of algebraic numbers according to his ideas [18f]), that he arrives at the definition and essential properties of $p$-adic absolute values [18e], starting with which he will be able to develop, modeling it on Cauchy’s theory, a new “$p$-adic analysis” which he will be able to apply fruitfully in the Theory of Numbers (notably by using the $p$-adic exponential and logarithm) and whose importance has been growing ever since.

Hensel had well seen, from the beginning, the simplifications his theory brought to classical expositions, by allowing the problems to be “localized” and the work to be carried out in a field where not only are the divisibility properties trivial, but also, thanks to the fundamental lemma which he discovered as early as 1902 [18c], the study of polynomials whose “reduced” polynomials mod $p$ have no multiple roots is reduced to the study of polynomials over a finite field. He had given as early as 1897 [18b] striking examples of these simplifications, notably on questions related to the discriminant (in particular, a short proof of the criterion he had given a few years earlier for the existence of “extraordinary divisors”). But for a long time it seems that the $p$-adic numbers inspired considerable distrust in contemporary mathematicians; a current attitude no doubt towards ideas that are “too abstract”, but which was also justified in part by the rather excessive enthusiasm of their author (so frequent in mathematics among zealots of new theories). Not content to apply his theory fruitfully to algebraic numbers, Hensel, impressed as all his contemporaries were, by the proofs of the transcendence of $e$ and $\pi$ and perhaps misled by the adjective "transcendental" applied both to numbers and to functions, had come to think that there existed a connection between his p-adic numbers and transcendental real numbers and he had thought for a moment that he had obtained a simple proof of the transcendence of $e$ and even of $e^e$ ([18d], p. 556) (*).

Soon after 1910, the situation changes, with the rising of the next generation, influenced by the ideas of Frtchet and F. Riesz on topology and by those of Steinitz on algebra, and from the start devoted to "abstraction"; it will know how to assimilate and put in their true place Hensel's works. As early as 1913, Kürschak [22] gives a general definition of the notion of absolute value, recognizes the importance of ultrametric absolute values (of which the p-adic absolute value was an example), proves (by modelling the proof on the case of real numbers) the existence of the completion of a field with respect to an absolute value and above all shows generally the possibility of extending an absolute value to any algebraic extension of the given field. But he had not seen that the ultrametric character of an absolute value was already revealed in the prime field; this point was established by Ostrowski, to whom also is due the determination of all the absolute values on the field $\mathbf{Q}$ and the fundamental theorem characterizing fields with a non-ultrametric absolute value as subfields of $\mathbf{C}$ [24]. In the years from 1920 to 1935, the theory will be completed by a more detailed study of absolute values which are not necessarily discrete, including amongst others the examination of various circumstances which arise in passing to an algebraic or transcendental extension (Ostrowski, Deuring, F. K. Schmidt); on the other hand, in 1931, Krull introduces and studies the general notion of valuation [29b] which will be greatly used in the years that follow by Zariski and his school of Algebraic Geometry (†). We must also mention here, although it lies outside our scope, the deeper studies on the structure of complete valued fields and complete local rings, which date from the same period (Hasse-Schmidt, Witt, Teichmuller, I. Cohen).

\*   \*   \*

The work of Fraenkel mentioned above (p. 594) only treated a very special

(*) This research at all cost of a narrow parallelism between p-adic series and Taylor series also leads Hensel to pose himself strange problems: he proves for example that every p-adic integer may be written in the form of a series $\sum_{k=0}^{\infty} a_k p^k$ where the $a_k$ are rational numbers chosen so that the series converges not only in $\mathbf{Q}_p$, but also in $\mathbf{R}$ (perhaps by analogy with Taylor series which converge at several places at once?) ([16e] and [16f]).

(†) An example of a valuation of height 2 had already been introduced incidentally by H. Jung in 1925 [27].

type of ring (Artinian with only a single prime ideal, which is moreover assumed to be principal). With the exception of Steinitz’s work on fields [20a], the first important works on the study of general commutative rings are E. Noether’s two great memoirs on ideal theory: that of 1921 [25a], devoted to primary decomposition, which takes up again in all generality and completes on many points the results of Lasker and Macaulay; and that of 1927 characterizing Dedekind domains axiomatically [25b]. Just as Steinitz had shown for fields, it is seen in these memoirs how a small number of abstract ideas, such as the notion of irreducible ideal, the chain conditions and the idea of an integrally closed domain (the last two, as we have seen, already brought to light by Dedekind) can by themselves lead to general results which seemed inextricably bound up with results of pure computation in the cases where they had previously been known.

With these memoirs of E. Noether, joined to the slightly later works of Artin-van der Waerden on divisorial ideals [31] and Krull relating these ideals to essential valuations [29b], the long study of the decomposition of ideals started a century earlier (*) is thus complete, at the same time as modern Commutative Algebra is being inaugurated.

The innumerable later research works on Commutative Algebra are grouped most easily according to several important directions of development:

(A) Local rings and topologies

Although the germ was contained in all the earlier works on the Theory of Numbers and Algebraic Geometry, the general idea of localization came to light very slowly. The general notion of ring of fractions is only defined in 1926 by H. Grell, a pupil of E. Noether, and only for integral domains [28]; its extension to more general rings will only be given in 1944 by C. Chevalley for Noetherian rings and in 1948 by Uzkov in the general case. Until about 1940, Krull and his school are practically alone in using in general arguments the consideration of the local rings A, of an integral domain A; these rings will only begin to appear explicitly in Algebraic Geometry with the works of Chevalley and Zariski starting in 1940 (†).

The general study of local rings themselves only begins in 1938 with Krull’s

(*) Following the definition of divisorial ideals, a considerable number of research works (Priifer, Krull, Lorenzen, etc.) were undertaken on ideals which are invariant under other operations $a \mapsto a'$ satisfying axiomatic conditions analogous to the properties of the operation $a \mapsto A$: (A: a) which gives birth to divisorial ideals; the results obtained in this way have as yet found no application in Algebraic Geometry nor in the Theory of Numbers.

(†) In the works of Hensel and his pupils on the Theory of Numbers, the local rings A, are systematically neglected to the benefit of their completions, no doubt because of the possibility of applying Hensel’s lemma to the latter.

great memoir [29d]. The most important results of this work concern dimension theory and regular rings, of which we shall not speak here; but here for the first time appears the completion of any arbitrary Noetherian local ring and also a still imperfect form of the graded ring associated with a local ring (*); the latter will only be defined about 1948 by P. Samuel [36] and independently in research on Algebraic Topology by Leray and H. Cartan. Krull, in the above mentioned work, hardly uses topological language; but already in 1928[29a], he had proved that, in a Noetherian ring $\mathbf{A}$, the intersection of the powers of an ideal $\mathbf{a}$ is the set of $x \in \mathbf{A}$ such that $x(1 - a) = 0$ for some $a \in \mathbf{a}$; it is easily deduced from this that, for every ideal $m$ of $\mathbf{A}$, the $m$-adic topology on $\mathbf{A}$ induces on an ideal $\mathbf{a}$ the $m$-adic topology on $\mathbf{a}$; in his memoir of 1938, Krull completes this result by proving that in a Noetherian local ring every ideal is closed. These theorems were soon afterwards extended by Chevalley to Noetherian semi-local rings and then by Zariski to the rings which bear his name [33b]; to Chevalley also goes back the introduction of "linear compactness" in topological rings, as also the determination of the structure of complete semi-local rings [32b].

(B) Passage from the local to the global

Since Weierstrass, an analytic function of one variable (and in particular an algebraic function) has habitually been associated with the set of its "expansions" at all the points of the Riemann surface where it is defined. In the introduction to his book on the Theory of Numbers ([18f], p. V), Hensel similarly associates with each element of an algebraic number field $k$ the set of elements corresponding to it in the completions of $k$ with respect to all the absolute values on $k$ ($\dagger$). It may be said that it is this point of view which, in modern Commutative Algebra, has replaced the decomposition formula of an ideal as a product of prime ideals (extending in a certain sense Kummer's initial point of view). Hensel's remark amounts implicitly to embedding $k$ in the product of all its completions; this is what Chevalley does explicitly in 1936 with his theory of

(*) If $m$ is the maximal ideal of the Noetherian local ring $\mathbf{A}$ under consideration and $(\alpha_i)_{1 \leq i \leq r}$, a minimal system of generators of $m$, Krull defines for $x \neq 0$ in $\mathbf{A}$ the "initial forms" of $x$ as follows: if $j$ is the greatest integer such that $x \in m^j$, the initial forms of $x$ are all the homogeneous polynomials of degree $j$, $P(X_1, \ldots, X_r)$ with coefficients in the residue field $k = \mathbf{A}/m$, such that $x \equiv P(\alpha_1, \ldots, a,) \pmod{m^{j+1}}$. With each ideal $\mathbf{a}$ of $\mathbf{A}$ he associates the graded ideal of $k[X_1, \ldots, X_r]$ generated by the initial forms of all the elements of $\mathbf{a}$ ("Leitideal"); these two notions for him take the place of the associated graded ring.

($\dagger$) Hensel takes, as non-ultrametric absolute values on a field $K$ of degree $n$ over $\mathbf{Q}$, the functions $x \mapsto |x^{(i)}|$ (where the $x^{(i)}$ for $1 \leq i \leq n$ are the conjugates of $x$) currently used since Dirichlet; Ostrowski was to show a little later that these functions are essentially the only non-ultrametric absolute values on $K$.

"idèles" [32a], which perfects earlier analogous ideas of Priifer and von Neumann (the latter confining themselves to embedding $k$ in the product of its $p$-adic completions)(*). Although this is somewhat outside our scope, it is important to mention here that, thanks to an appropriate topology on the group of idèles, all the techniques of locally compact groups (including Haar measure) can thus be very effectively applied to the Theory of Numbers.

In a more general context, Krull's theorem [29b] characterizing an integrally closed domain as an intersection of valuation rings (which amounts also to embedding the domain under consideration in a product of valuation rings) often facilitates the study of these rings, although the method is only really tractable for essential valuations of Krull domains. Moreover Krull frequently exhibits [29e] (quite elementary) examples of the "passage from the local to the global" method consisting of showing a property of an integral domain $A$ by verifying it for the "localized" rings $A_i$, of $A$ at all its prime ideals ($\dagger$); more recently, Serre perceived that this method works for arbitrary commutative rings $A$, that it is applicable also to $A$-modules and that it is even sufficient often to "localize" at the maximal ideals of $A$ (Chapter II, §3, Theorem 1): a point of view which is closely connected with ideas about "spectra" and sheaves defined over these spectra (see below, p. 602).

(C) Integers and integral closure
We have seen that the notion of algebraic integer, first introduced for number fields, had already been extended by Kronecker and Dedekind to algebraic function fields, although in this case it might appear rather artificial (not corresponding to a projective notion). E. Noether's memoir of 1927, followed by the work of Krull starting in 1931, showed the interest that these notions present for more general rings ($\ddagger$). Krull in particular is responsible for the

(*) Because of this remark by Hensel, the non-ultrametric absolute values on a number field $K$ have habitually been called (by an abuse of language) the "places at infinity" of $K$, by analogy with the process by which Dedekind and Weber define the "points at infinity" of the Riemann surface of an affine curve (cf. p. 591).

($\dagger$) In speaking of the "passage from the local to the global", there is often an allusion to much more difficult questions, connected with class field theory, and the best known examples of which are those treated in Hasse's memoirs ([26a] and [26b]) on quadratic forms over an algebraic number field $k$; he shows there among other things that for an equation $f(x_1, \ldots, x_n) = a$ to have a solution in $k^n$ ($f$ a quadratic form, $a \in k$), it is necessary and sufficient that it have a solution in each of the completions of $k$. According to Hasse, the idea of this type of theorem had been suggested to him by his master Hensel [26c]. The extension of this "principle of Hasse" to groups other than the orthogonal group is one of the objectives of the modern theory of "adelizations" of algebraic groups.

($\ddagger$) Krull and E. Noether limit themselves to integral domains, but the extension of their methods to the general case is not difficult; the most interesting memoir theorems on the lifting of prime ideals to integral algebras [29c], as also for extending the theory of decomposition and inertia groups of Dedekind-Hilbert [29b]. As for E. Noether, we owe to her the general formulation of the normalization lemma (*) (from which follows amongst other things Hilbert’s Nullstellensatz) as also the first general criterion (transcribing the classical arguments of Kronecker and Dedekind) for the integral closure of an integral domain to be finite over that domain.

Finally, it should be pointed out here that one of the reasons for the present importance of the notion of integrally closed domain is due to Zariski’s studies on algebraic varieties; he discovered that “normal” varieties (that is those whose local rings are integrally closed domains) are distinguished by particularly pleasant properties, notably the fact that they have no “singularity of codimension 1”; and it has then been seen that analogous phenomena are true for “analytic spaces”. Therefore “normalization” (that is the operation which, for the local rings of a variety, consists of taking their integral closures) has become a powerful weapon in the arsenal of modern Algebraic Geometry.

(D) The study of modules and the influence of Homological Algebra

One of the striking characteristics of the work of E. Noether and W. Krull in Algebra is the tendency to “linearization”, extending the analogous development given to field theory by Dedekind and Steinitz; in other words, ideals are considered above all as modules and so all the constructions of Linear Algebra (quotient, product and more recently tensor product and formation of homomorphism modules) are brought to bear on them, producing in general modules which are no longer ideals. It is thus quickly seen that in many questions (for commutative or non-commutative rings), interest should not be confined to the study of ideals of a ring A, but on the contrary the theorems should be stated in general for A-modules (sometimes subjected to certain finiteness conditions).

The intervention of Homological Algebra has strongly reinforced the above tendency, since this branch of Algebra is essentially concerned with questions of a linear nature. We shall not retrace its history here; but it is interesting to point out that several fundamental notions of Homological Algebra (such as that of projective module and that of Tor functor) came into being on the occasion of a close study of the behaviour of modules over a Dedekind domain relative to the tensor product, a study undertaken by H. Cartan in 1948.

on this subject is that where I. Cohen and Seidenberg extend Krull’s lifting theorems, indicating exactly the limits of their validity [35]. It should be mentioned that E. Noether had explicitly mentioned the possibility of such generalizations in her memoir of 1927 ([25b], p. 30).

(*) A particular case had already been asserted by Hilbert in 1893 ([16b], p. 316).

Conversely, it could be foreseen that the new classes of modules introduced naturally by Homological Algebra as “universal annihilators” of the Ext functors (projective modules and injective modules) and the Tor functors (flat modules) would throw new light on Commutative Algebra. It happens that chiefly projective modules and still more flat modules have shown themselves useful: the importance of the latter arises above all from the remark, made first by Serre [38b], that localization and completion introduce flat modules naturally, thus “explaining” in a much more satisfactory way the properties of these operations already known and rendering them much easier to use. It should moreover be mentioned (as we shall see in later chapters) that the applications of Homological Algebra are far from being limited to this and that it is playing a more and more important role in Algebraic Geometry.

(E) The notion of spectrum
The most recent in date of the new notions of Commutative Algebra has a complex history. Hilbert’s spectral theorem introduced ordered sets of orthogonal projectors of a Hilbert space, forming a “Boolean algebra” (or rather a Boolean lattice) (*), in one-to-one correspondence with a Boolean lattice of classes of measurable subsets (for a suitable measure) of $\mathbf{R}$. No doubt his earlier work on operators on Hilbert spaces, about 1935, led M. H. Stone to study Boolean lattices generally and notably to look for “representations” of them by subsets of a set (or classes of subsets with respect to a certain equivalence relation). He observes that a Boolean lattice becomes a *commutative* ring (moreover of a very special type), if multiplication is defined on it by $xy = \inf(x, y)$ and addition by $x + y = \sup(\inf(x, y'), \inf(x', y))$. In the particular case where the Boolean lattice in question is the set $\mathfrak{P}(X)$ of all subsets of afinite set $X$, it is immediately seen that the elements of $X$ are in a natural one-to-one correspondence with the maximal ideals of the corresponding “Boolean” ring; and Stone obtains precisely his general representation theorem for a Boolean lattice by similarly considering the set of maximal ideals of the corresponding ring and associating with each element of the Boolean lattice the set of maximal ideals which contains it [30a].

On the other hand, the set of both open and closed subsets of a topological space was a well-known classical example of a Boolean lattice. In a second paper [30b], Stone showed that in fact every Boolean lattice is also isomorphic to a Boolean lattice of this nature. For this it was of course necessary to define a *topology* on the set of maximal ideals of a “Boolean” ring; which was very

(*) A *Boolean lattice* is a lattice-ordered set $E$, with a least element $a$ and a greatest element $\omega$, where each of the laws sup and inf is *distributive* with respect to the other and, for all $a \in E$, there exists a unique $a' \in E$ such that $\inf(a, a') = a$ and $\sup(a, a') = w$ (cf. *Set Theory*, Chapter III, § 1, Exercise 17).

simply accomplished by taking as closed sets for each ideal $a$ the set of maximal ideals containing $a$.

We shall not speak here of the influence of these ideas on Functional Analysis, where they played an important role in the birth of the theory of normed algebras developed by I. Gelfand and his school. But in 1945, Jacobson observes [34] that the process of defining a topology, invented by Stone, can in fact be applied to any ring $A$ (commutative or not) provided the set of ideals taken is not the set of maximal ideals but the set of two-sided "primitive" ideals (i.e. the two-sided ideals $b$ such that $A/b$ is a primitive ring); for a commutative ring, these of course turn out to be the maximal ideals. On his part, Zariski, in 1944 [33a], uses an analogous method to define a topology on the set of *places* of an algebraic function field. However, these topologies remained for the majority of algebraists mere curiosities, by reason of the fact that they are not usually Hausdorff and a quite understandable repugnance was felt about working on such unusual objects. This distrust was only overcome when A. Weil showed, in 1952, that every algebraic variety can be given a natural topology of the above type and that this topology allows the definition, in perfect analogy with the case of differentiable or analytic manifolds, of the notion of *fibre bundle* [37]; soon afterwards, Serre had the idea of extending to these varieties thus topologized the theory of *coherent sheaves*, thanks to which the topology renders in the case of "abstract" varieties the same services as the usual topology when the base field is $\mathbf{C}$, notably as far as applying the methods of Algebraic Topology is concerned ([38a] and [38b]).

From then on it was natural to use this geometric language throughout Commutative Algebra. It was quickly seen that considering maximal ideals is usually insufficient to obtain useful assertions (*) and that the adequate notion is that of the set of *prime* ideals of the ring topologized in the same manner. With the introduction of the notion of spectrum, there now exists a dictionary allowing every theorem of Commutative Algebra to be expressed in a geometric language very close to that of the Algebraic Geometry of the Weil-Zariski period; which has moreover immediately brought about a considerable enlargement of the scope of the latter, so that Commutative Algebra is scarcely more than the most elementary part of it [39].

(*) The inconvenience of limiting attention to the "maximal spectrum" arises from the fact that, if $\phi : A \to B$ is a ring homomorphism and $n$ a maximal ideal of $B$, $\phi^{-1}(n)$ is not necessarily a maximal ideal of $A$, whereas for every prime ideal $p$ of $B$, $\phi^{-1}(p)$ is a prime ideal of $A$. Hence in general a mapping of the set of maximal ideals of $B$ to the set of maximal ideals of $A$ cannot naturally be associated with $\phi$.

1. L. Euler, Vollständige Anleitung zur Algebra (=Opera Omnia (1), vol. I, Leipzig-Berlin (Teubner), 1911).
2. J. L. Lagrange, Oeuvres, 14 volumes, Paris (Gauthier-Villars), 1867–1892.
3. C. F. Gauss, Werke, 12 volumes, Gottingen, 1870-1927.
4. P. G. Lejeune-Dirichlet, Werke, 2 volumes, Berlin (Reimer), 1889–1897.
4 (bis). P. G. Lejeune-Dirichlet, Vorlesungen über Zahlentheorie, 2te Aufl., Braunschweig (Vieweg), 1871.
5. C. G. J. Jacobi, Gesammelte Werke, 7 volumes, Berlin (Reimer), 1881–1891.
6. G. Eisenstein: (a) Beweis der Reciprocitatsgesetzefur die cubischen Reste in der Theorie der aus dritten Wurzeln der Einheit zusammengesetzen Zahlen, Crelle’s Journal, 27 (1844), pp. 289–310; (b) Zur Theorie der quadratischen Zerfallung der Primzahlen 8n + 3, 7n + 2 und 7n + 4, Crelle’s Journal, 37 (1848), pp. 97–126; (c) Über einige allgemeine Eigenschaften der Gleichung von welcher die Teilung der ganzen Lemniscate abhangt, nebst Anwendungen derselben auf die Zahlentheorie, Crelle’s Journal, 39 (1850), pp. 160–179 and 224–287.
7. E. Kummer: (a) Sur les nombres complexes qui sont formés avec les nombres entiers réels et les racines de l’unité, J. de Math., (1), 12 (1847), pp. 185–212; (b) Zur Theorie der complexen Zahlen, Crelle’s Journal, 35 (1847), pp. 319–326; (c) Ueber die Zerlegung der aus Wurzeln der Einheit gebildeten complexen Zahlen in Primfactoren, Crelle’s Journal, 35 (1847), pp. 327–367; (d) Mémoire sur les nombres complexes composés de racines de l’unité et des nombres entiers, J. de Math., (1), 16 (1851), pp. 377–498; (e) Über die allgemeinen Reciprocitatsgesetze unter den Resten und Nichtresten der Potenzen deren Grad eine Primzahl ist (Abh. der Kon. Akad. der Wiss. zu Berlin (1859), Math. Abhandl., pp. 19–159).
8. C. Hermite, Oeuvres, 4 Volumes, Paris (Gauthier-Villars), 1905–1917.
9. L. Kronecker, Werke, 5 volumes, Leipzig (Teubner), 1895–1930: (a) De unitatibus complexis, vol. I, pp. 5–71 (= Inaug. Diss., Berolini, 1845); (b) Über die algebraisch auflosbaren Gleichungen I, vol. IV, pp. 1–11 (= Monatsber. der Kon. Preuss. Akad. der Wiss., 1853, pp. 365–374); (c) Über die elliptischen Functionen fur welche complexe Multiplication stattfindet vol. IV, pp. 177–183 (= Monatsber. der Kon. Preuss. Akad. der Wiss., 1857, pp. 455–460); (d) Uber die complexe Multiplication der elliptischen Functionen, vol. IV, pp. 207–217 (= Monatsber. der Kön. Preuss. Akad. der Wiss., 1862, pp. 363–372); (e) Über die Discriminante algebraischer Functionen einer Variabeln, vol. II, pp. 193–236 (= Crelle’s Journal, 91 (1881), pp. 301–334); (f) Grundzuge einer arithmetischen Theorie der algebraischen Grössen, vol. II, pp. 237–387 (=Crelle’s Journal, 92 (1882), pp. 1–122).

10. R. Dedekind, Gesammelte mathematische Werke, 3 volumes, Braunschweig (Vieweg), 1932: (a) Abriss einer Theorie der höheren Kongruenzen in bezug auf einen reellen Primzahl-Modulus, vol. I, pp. 40–66 (=Crelle’s Journal, 54 (1857), pp. 1–26; (b) Sur la Théorie des Nombres entiers algébriques, vol. III, pp. 262–296 (=Bull. Sci. Math., (1), 11 (1876), pp. 278–288 and (2), 1 (1877), pp. 17–41, 69–92, 144–164, 207–248); (c) Uber die Anzahl der Ideal-Klassen in den verschiedenen Ordnungen eines endlichen Korpers, vol. I, pp. 105–157 (=Festschrift der Technischen Hochschule in Braunschweig zur Säkularfeier des Geburtstages von C. F. Gauss, Braunschweig, 1877, pp. 1–55); (d) Über den Zusammenhang zwischen der Theorie der Ideals und der Theorie der höheren Kongruenzen, vol. I, pp. 202–230 (=Abh. Kön. Ges. Wiss. zu Gottingen, 23 (1878), pp. 1–23); (e) Uber die Discriminantend endlicher Korper, vol. I, pp. 351–396 (=Abh. Kön. Ges. Wiss. zu Gdttingen, 29 (1882), pp. 1–56); (f) Uber die Theorie der ganzen algebraischen Zahlen, vol. III, pp. 1–222 (=Supplement XI von Dirichlets Vorlesungen über Zahlentheorie, 4 Aufl. (1894), pp. 434–657); (g) Zur Theorie der Ideale, vol. 11, pp. 43–48 (=Nachr. Gottingen, 1894, pp. 272–277); (h) Uber eine Erweiterung des Symbols (a, b) in der Theorie der Moduln, vol. II, pp. 59–85 (=Nachr. Göttingen, 1895, pp. 183–208).

10(bis). R. Dedekind-H. Weber, Theorie der algebraischen Funktionen einer Veränderlichen, Crelle’s Journal, 92 (1882), pp. 181–290 (=R. Dedekind, Ges. Math. Werke, vol. I, pp. 238–349).

11. E. Selling, Ueber die idealen Primfactoren der complexen Zahlen, welche aus den Wurzeln einer beliebigen irreductiblen Gleichung rational gebildet sind, Zeitschr.fur Math. und Phys., 10 (1865), pp. 17–47.

12. M. Noether, Uber einen Satz aus der Theorie der algebraischen Funktionen, Math. Ann., 6 (1873), pp. 351–359.

13. A. Brill-M. Noether, Ueber algebraischen Funktionen, Math. Ann., 7 (1874), pp. 269–310.

14. G. Zolotareff, Sur la théorie des nombres complexes, J. de Math. (3), 6 (1880), pp. 51–84 and 129–166.

15. E. Netto, Zur Theorie der Elimination, Acta Math., 7 (1885), pp. 101–104.

16. D. Hilbert: (a) Uber die Theorie der algebraischen Formen, Math. Ann., 36 (1890), pp. 473–534; (b) Uber die vollen Invariantensysteme, Math. Ann., 42 (1893), pp. 313–373; (c) Grundzuge einer Theorie des Galoischen Zahlkorpers, Gött. Nachr., (1894), pp. 224–236; (d) Zahlbericht, Jahresber. der D. M. V., 4 (1897), pp. 175–546 (translated into French by A. Lévy and Th. Got under the title “Théorie des corps de nombres algébriques”, Paris (Hermann), 1913).

17. K. Weierstrass, Mathematische Werke, 7 volumes, Berlin (Mayer und Muller), 1894–1927.

18. K. HENSEL: (a) Über eine neue Begriindung der Theorie der algebraischen Zahlen, Jahresber. der D. M. V., 6 (1899), pp. 83–88; (b) Ueber die Fundamentalgleichung und die ausserwesentlichen Diskriminantentheiler eines algebraischen Korpers, Gött. Nachr., (1897), pp. 254–260; (c) Neue Grundlagen der Arithmetik, Crelle’s Journal, 127 (1902), pp. 51–84; (d) Über die arithmetische Eigenschaften der algebraischen und transcendenten Zahlen, Jahresber. der D. M. V., 14 (1905), pp. 545–558; (e) Ueber die arithmetischen Eigenschaften der Zahlen, Jahresber. der D. M. V., 16 (1907), pp. 299–319, 388–393, 474–496; (f) Theorie der algebraischen Zahlen, Leipzig (Teubner), 1908.

19. E. LASKER, Zur Theorie der Moduln und Ideale, Math. Ann., 60 (1905), pp. 20–116.

20. E. STEINITZ: (a) Algebraische Theorie der Korper, Crelle’s Journal, 137 (1910), pp. 167–308; (b) Rechteckige Systeme und Moduln in algebraischen Zahlkörpern, Math. Ann. 71 (1912), pp. 328–354 and 72 (1912), pp. 297–345.

21. F. S. MACAULAY, On the resolution of a given modular system into primary systems including some properties of Hilbert numbers, Math. Ann., 74 (1913), pp. 66–121.

22. J. KÜRSCHAK, Über Limesbildung und allgemeine Körpertheorie, Crelle’s Journal, 142 (1913), pp. 211–253.

23. A. FRAENKEL, Uber die Teiler der Null und die Zerlegung von Ringen, Crelle’s Journal, 145 (1914), p p 139–176.

24. A. OSTROWSKI, Über einige Lösungen der Funktionalgleichung $\phi(x)\phi(y) = \phi(x.y)$, Acta Math., 41 (1917), pp. 271–284.

25. E. NOETHER: (a) Idealtheorie in Ringbereichen, Math. Ann., 83 (1921), pp. 24–66; (b) Abstrakter Aufbau der Idealtheorie in algebraischen Zahl- und Funktionenkörpern, Math. Ann., 96 (1927), pp. 26–61.

26. H. HASSE: (a) Ueber die Darstellbarkeit von Zahlen durch quadratischen Formen im Korper der rationalen Zahlen, Crelle’s Journal, 152 (1923), pp. 129–148; (b) Ueber die Äquivalenz quadratischer Formen im Korper der rationalen Zahlen, Crelle’s Journal, 152 (1923), pp. 205–224; (c) Kurt Hensels entscheidender Anstoss zur Entdeckung des Lokal-Global-Prinzips, Crelle’s Journal, 209 (1960), pp. 3–4.

27. H. JUNG, Algebraischen Flachen, Hannover (Helwing), 1925.

28. H. GRELL, Beziehung zwischen den Idealen verschiedener Ringe, Math. Ann., 97 (1927), pp. 490–523.

29. W. KRULL: (a) Primidealketten in allgemeine Ringbereichen, Sitz. Ber. Heidelberg Akad. Wiss., 1928; (b) Allgemeine Bewertungstheorie, Crelle’s Journal, 167 (1931), pp. 160–196; (c) Beiträge zur Arithmetik kommutativer Integritatsbereiche, III, Math. Zeitschr., 42 (1937), pp. 745–766; (d) Dimensionstheorie in Stellenringen, Crelle’s Journal, 179 (1938), pp. 204–226; (e) Idealtheorie, Berlin (Springer), 1935.

30. M. H. Stone: (a) The theory of representations for Boolean algebras, Trans. Amer. Math. Soc., 40 (1936), pp. 37–111; (b) Applications of the theory of Boolean rings to general topology, Trans. Amer. Math. Soc., 41 (1937), pp. 375–481.
31. B. L. van der Waerden, Moderne Algebra, vol. II, Berlin (Springer), 1931.
32. C. Chevalley: (a) Généralisation de la théorie du corps de classes pour les extensions infinies, J. de Math., (9), 15 (1936), pp. 359–371; (b) On the theory of local rings, Ann. of Math., 44 (1943), pp. 690–708.
33. O. Zariski: (a) The compactness of the Riemann manifold of an abstract field of algebraic functions, Bull. Amer. Math. Soc., 50 (1944), pp. 683–691 ; (b) Generalized semi-local rings, Summa Bras. Math., 1 (1946), pp. 169–195.
34. N. Jacobson, A topology for the set of primitive ideals in an arbitrary ring, Proc. Nat. Acad. Sci. U.S.A., 31 (1945), pp. 333–338.
35. I. Cohen-A. Seidenberg, Prime ideals and integral independence, Bull. Amer. Math. Soc., 52 (1946), pp. 252–261.
36. P. Samuel, La notion de multiplicité en Algèbre et en Gtomtrie algébrique, J. de Math., (9), 30 (1951), pp. 159–274.
37. A. Weil, Fibre-spaces in Algebraic Geometry (Notes by A. Wallace), Chicago Univ., 1952.
38. J. P. Serre: (a) Faisceaux algébriques cohérents, Ann. of Math., 61 (1955), pp. 197–278; (b) Géométrie algébrique et géométrie analytique, Ann. Inst. Fourier, 6 (1956), pp. 1–42.
39. A. Grothendieck, Éléments de géométrie algébrique, Publ. math. Inst. Htes Et. Scient., 1960.

The reference numbers indicate the chapter, section and sub-section (or exercise) in that order.

1, (E a set), U . V, UV (U, V additive subgroups), $a^0$ (a an ideal): Preliminary conventions of Chapter I
E : F : 1.2.10
$A[S^{-1}], a/s$ (A a ring, S a subset of A, $a \in A$, s a product of elements of S): 11.2.1 $i_A^S$: 11.2.1
$S^{-1}A, A_p$ (S a multiplicative subset, p a prime ideal): 11.2.1
$M[S^{-1}], m/s, i_M^S$ (M an A-module, S a subset of A, $m \in M$, s a product of elements of S): 11.2.2
$S^{-1}M, M_p$ (M an A-module, S a multiplicative subset of A, p a prime ideal of A): 11.2.2
$S^{-1}u, u_p$ (u an A-module homomorphism): 11.2.2
$r(a)$ (a an ideal): 11.2.6
$V(M), V(f)$ (M a subset of the ring A, $f \in A$): 11.4.3
$\operatorname{Spec}(A)$: 11.4.3
$X_f$ ($f \in A, X = \operatorname{Spec}(A)$): II.4.3
$\mathfrak{g}(Y)$ (Y a subset of $\operatorname{Spec}(A)$): 11.4.3
$ah$ (h a ring homomorphism): 11.4.3
$\operatorname{Supp}(M)$ (M an A-module): 11.4.4
$A, M_f, u_f$ (A a ring, M an A-module, u an A-homomorphism, $f \in A$): II.5.1
$\operatorname{rg}_p(P)$ (P a projective module): 11.5.3
$\operatorname{rg}(P)$ (P a projective module): 11.5.3
$P(A), \operatorname{cl}(M)$ (A a ring, M a projective A-module of rank 1): 11.5.4
$\mathfrak{C}, \mathfrak{C}(A)$: 11.5.7
$\det(u), \chi_u$ (u an endomorphism of a projective module of rank n): 11.5. Ex. 9
$A^{(d)}, M^{(d,k)}, M^{(d)}$ (A a graded ring, M a graded A-module): III.1.3
$A_{(p)}, M_{(p)}$ (A a graded ring, p a graded prime ideal of A, M a graded A-module): 111.1.4 gr_n(G), gr(G) (G a filtered group): 111.2.3
gr(h) (h a homomorphism compatible with the filtrations): 111.2.4
\mathbf{Z}_n (n an integer > 1): 111.2.12
\hat{\mathbf{Z}}: 111.2.13
A\{X_1, \ldots, X_p\} (A a linearly topologized ring): 111.4.2
f(b_1, \ldots, b_p) (f a restricted formal power series): 111.4.2
f \circ g, M_f, M_f(\mathbf{X}), J_f, J_f(\mathbf{X}), \mathbf{X}, \mathbf{1}, (\mathbf{f}, \mathbf{g} systems of formal power series, \mathbf{g} without constant term): 111.4.4
f(x) (f a system of formal power series, x a system of topological nilpotent elements): 111.4.5
m \times n (m an ideal): 111.4.5
Ass_A(M), Ass(M) (M an A-module): IV. 1.1
Ass_f(M): IV.1. Ex. 17
A^G (A an algebra, G a group operating on A): V.1.9
G^Z(p'), G^Z, A^Z(p'), A^Z (G a group operating on a ring A', p' a prime ideal of A'): V.2.2
G^T(p'), G^T, A^T(p'), A^T (A group operating on a ring A', p' a prime ideal of A): v.2.2
K^Z(p'), K^Z, K^T(p'), K^T (K the field of fractions of an integrally closed domain A, p' a prime ideal of the integral closure of A in a quasi-Galois extension of K): V.2.3
Y^p (where p = (p_1, \ldots, p_m), the p_i being integers \geqslant 0): V.3.1
m(A), \kappa(A), U(A) (A a local ring): VI
R, a: VI.2.1
+\infty: VI.3.1
\Gamma_A, v_A: VI.3.2
a(M) (M a major set): VI.3.5
h(G) (G a totally ordered group): VI.4.4
\mathcal{T}_v (v a valuation): VI.5.2
e(v'/v), e(A'/A), e(L/K): VI.8.1
f(v'/v), f(A'/A), f(L/K): VI.8.1
\varepsilon(G, H) (G a totally ordered group, H a subgroup of G of finite index): VI.8.4
\varepsilon(v'/v) (v a valuation, v' an extension of v): VI.8.4
\operatorname{mod}(x), \operatorname{mod}_K(x) (K a non-discrete locally compact field, x \in K): VI.9.1
r(G) (rational rank of a commutative group): VI.10.2
d(K'/K), s(v'/v), r(v'/v) (v a valuation on K, v' an extension of v to a transcendental extension K' of K): VI.10.3
I(A), D(A) (A an integral domain): VIII.1.1
a \prec b, \operatorname{div}(a), \operatorname{div}(x) (a, b fractional ideals, x an element of the field of fractions): VII.1.1
\tilde{a} (a a fractional ideal): VII.1.1
d_1 \leq d_2 (d_1, d_2 divisors): VII.1.1 $b : a$ (a, $b$ fractional ideals): VII.1.1
$J(A)$ (A an integral domain): VII.1.2
$P(A)$ (A a Krull domain): VII.I.3
$p^{(n)}$ ($p$ a divisorial prime ideal): VII.1.4
$v_p$ ($p$ a prime ideal of height 1 in a Krull domain): VII.1.10
$F(A), C(A)$ (A a Krull domain): VII.1.10
$e(\mathfrak{P}/p)$ ($p \in P(A), \mathfrak{P} \in P(B), A \subset B, \mathfrak{P} \cap A = p$) VII.1.10
$i$ (homomorphism from $D(A)$ to $D(B)$, or of $C(A)$ to $C(B)$): VII.1.10
$\bar{i}$ (homomorphism from $C(A)$ to $C(B)$): VII.1.10
$A, A,, \Delta(K)$ (rings of restricted adèles): VII.2.4
$\mathfrak{P}^*, \mathfrak{P}^*(A)$ (A an integral domain): VII.3.2
$M^*$ (dual lattice of a lattice $M$): VII.4.2
$l_p(T), \chi(T)$ (T a torsion A-module, $p$ a prime ideal of height 1): VII.4.5
$F(A), T(A), cl(M)$: VII.4.5
$\chi(M, M')$ (M, $M'$ lattices): VII.4.6
$c(d)$ (da divisor): VII.4.7
$c(M), r(M), \gamma(M)$ (M a lattice): VII.4.7
$\mathfrak{P}|p, e_{\mathfrak{P}/p}, f_{\mathfrak{P}/p}, f(\mathfrak{P}/p)$ (A $\subset$ B Krull domains such that B is a finite A-algebra $P \in P(A), \mathfrak{P} \in P(B), \mathfrak{P} \cap A = p$): VII.4.8
$N_{B/A}, N, i_{B/A}$: VII.4.8

The reference numbers indicate the chapter, section and sub-section (or exercise) in that order.

Adèle, restricted, principal restricted adtle : VII.2.4
m-adic filtration: 111.2.1
— topology: 111.2.5
n-adic integers: 111.2.12
Algebra, Azumaya: II.1.7
— finitely generated : 111.1.1
— integral, finite, over a ring: V. 1.1
Algebraic closure of a field in an algebra : V. 1.2
Algebraically closed field in an algebra: V. 1.2
— dependent, independent, elements: 111.1.1
— free, related, family: 111.1.1
Almost all $p \in P(A)$ (property valid for) : VII.4.3
— nilpotent endomorphism: IV. 1.4
Approximation theorem for absolute values : VI.7.3
— theorem for valuations: VI.7.2
Artin-Rees Lemma: 111.3.1
Associated (filtered module) with a graded module: 111.2.1
— (filtered ring) with a graded ring: 111.2.1
— (filtration) with a graduation: III.2.1
— (graded homomorphism) with a homomorphism compatible with filtrations: 111.2.4
— (graded module) with a filtered module: 111.2.3
— (graded ring) with a filtered ring: 111.2.3
— (mapping) with a ring homomorphism: 11.4.3
— (prime ideal) with a module: IV. 1.1
— ring, place, valuation: VI.3.3

Canonical decomposition of a place: VI.2.3
— factorization of a valuation: VI.3.2
— homomorphism of the decomposition group of a prime ideal $\mathfrak{p}'$ of $\mathbf{A}'$ into the automorphism group of $\mathbf{A}'/\mathfrak{p}'$: V.2.2
Class, divisor, attached to a finitely generated module : VII.4.7
Classes, divisor (monoid of) : VII.1.2
Closure, algebraic, of a field in an algebra : V.1.2
— integral, of an integral domain : V.1.2
— integral, of a ring in an algebra: V.1.2
Commutative diagram: I.1.2
Compatible (filtration) with a ring structure, module structure: 111.2.1
— (homomorphism) with filtrations: 111.2.4
Complete system of extensions of a valuation: VI.8.2
Completely integrally closed domain : V.1.4
Component, irreducible (of a topological space) : 11.4.1
Conditions, Hensel's: 111.4.5
Conductor of a submodule : V.1.5
Content of a polynomial over a pseudo-Bezoutian domain: VII.1.Ex.23
— of a torsion module: VII.4.5
Criterion, Eisenstein’s irreducibility: VII.3.Ex.20

Decomposition, canonical, of a place : VI.2.3
— complete, of a prime ideal: V.2.2
— field of a prime ideal: V.2.2
— group, ring, of a prime ideal: V.2.2
— of an ideal in a Dedekind domain into prime factors: VII.2.3
— primary: IV.2.2 and Ex.20
— reduced primary: IV.2.3 and Ex.20
Decreasing filtration: 111.2.1
Dedekind domain: VII.2.1
Defined (topology) by a filtration: 111.2.5
Defining ideal: III.3.2
Degree, residue class, of one valuation over another: VI.8.1
Dependence, integral (equation of) : V.1.1
Derived (module filtration) from a ring filtration: 111.2.1
Diagram, commutative: I.1.2
— snake : I.1.4
Discrete filtration: 111.2.1
— valuation: VI.3.6
Distinguished polynomial : VII.3.8
Divisor, principal divisor: VII.1.1
— determinantal: VII.4.Ex.11
— finitely generated: VII.1.Ex.11

Divisorial fractional ideal : VII. 1.1
Divisors, equivalent: VII. 1.2
Domain, Bezoutian (or Bezout) : VII.1.Ex.20
— completely integrally closed : V. 1.4
— Dedekind: VII.2.1
— factorial: VII.3.1
— integrally closed : V. 1.2
— integrally closed, of finite character: VII.1.Ex.25, 26 and 28
— integrally Noetherian: V.3.Ex.6
— Krull: VII.1.3
— local integral, of dimension 1 : VI.4.Ex.7
— Pruferian (or Prufer): VII.2.Ex.12
— pseudo-Bezoutian: VII. 1.Ex.21
— pseudo-principal: VII. 1.Ex.21
— pseudo-Pruferian: VII.2.Ex.19
— regularly integrally closed: VII. 1.Ex.30
Dominating (local ring) a local ring: VI. 1.1
Dual, algebraic toric, of a module: VI.5.Ex.9
— lattice: VII.4.2
— topological toric: VI.5.Ex.10

Element, topologically nilpotent: 111.4.3
Elements, algebraically dependent, independent: III.1.]
— strongly relatively prime: 111.4.1
Endomorphism, almost nilpotent: IV. 1.4
Equivalent divisors: VII. 1.2
— valuations: VI.3.2
Essential graded ideal: III.1.4
— valuations: VII.1.4
Euclidean ordered field: VI.2.Ex.4
Exhaustive filtration: III.2.1
Extension, quasi-Galois: V.2.2

Factor, invariant: VII.4.Ex. 11 and 14
Factorial domain: VII.3.1
Factorization, canonical, of a valuation : VI.3.2
Faithfully flat module: 1.3.1
Family, algebraically free, related : 111.1.1
— formally free: 111.2.9
Field, algebraically closed in an algebra : V. 1.2
— decomposition: V.2.3
— projective: VI.2.1
— residue, of a local ring: II.3.1

Field, residue, of a place: VI.2.3
— residue, of a valuation: VI.3.2
— value, of a place: VI.2.2
Filtered group, ring, module: 111.2.1
Filtration, m-adic: 111.2.1
— associated with a graduation: 111.2.1
— compatible with a ring structure, module structure: 111.2.1
— discrete: 111.2.5
— m-good: 111.3.1
— increasing, decreasing, separated, exhaustive: 111.2.1
— induced, product, quotient: III.2.1
— module, derived from a ring filtration: III.2.1
— trivial: 111.2
Finite algebra over a ring : V. 1.1
— (place) at an element: VI.2.2
Finitely generated algebra: 111.1.1
Finitely presented: 1.2.8
Flat for M, M-flat (module): 1.2.2
— module: 1.2.3
Formally free family: 111.2.9
Fractional ideal: VII.1.1
Function, order: 111.2.2

Gaussian integer: V. 1.1
Gauss’s lemma: VII.3.5
Gelfand-Mazur Theorem: V1.6.4.
Generated by a subset (multiplicative subset): 11.2.1
Generators, formal system of: 111.2.9
m-good filtration: 111.3.1
Group, decomposition: V.2.2
— filtered: 111.2.1
— inertia: V.2.2
— of classes of invertible modules: 11.5.7
— of operators, locally finite : V. 1.9
— operating on a ring: V. 1.9
— order, of a valuation: VI.3.2
— ordered, of height $n$, of height $+\infty$: VI.4.4

Height $\leq 1$ (prime ideal of) : VII.1.6
— of an ordered group, of a valuation : VI.4.4
Henselian ring : III.4.Ex.3
Hensel’s conditions: 111.4.5
— Theorem: 111.4.3

Homomorphism, canonical, of the decomposition group of a prime ideal $p'$
— from $A'$ to the automorphism group of $A'/p'$: V.2.2
— compatible with filtrations: III.2.4
— graded, associated with a homomorphism compatible with filtrations: 111.2.4
— local: 11.3.1
— pseudo-injective, pseudo-surjective, pseudo-zero, pseudo-bijective: VII.4.4

Ideal, determinantal: VII.4.Ex.10 and 14
— essential graded : III.1.4
— immersed prime: IV.2.3
— integral, fractional ideal : VII.1.1
— invertible fractional: 11.5.7
— lying above an ideal : V.2.1
— minimal prime: 11.2.6
— of a place: VI.2.3
— of a valuation: VI.3.2
— prime: II.1.1
— prime, associated with a module : IV.1.1
— prime, decomposing completely: V.2.2
— prime, of height $\leq 1$: VII.1.6
— primary, p-primary: IV.2.1 and Ex.20
— unramified: V.2.Ex.18 and 19
Ideally Hausdorff module: 111.5.1
Ideals, relatively prime: 11.1.2
Identity, Cauchy's: VII.3.Ex.18
Immersed prime ideal: IV.2.3
Improper valuation: VI.3.1
Increasing filtration: III.2.1
Independent valuation rings: VI.7.2
— valuations: VI.7.2
Index, initial, of a subgroup of an ordered group, initial ramification index of a valuation: VI.8.4
— ramification: VI.8.1
Induced filtration: 111.2.1
Induction, Noetherian (principle of): II.4.2
Inertia field: V.2.3
— ring, group: V.2.2
Initial ramification index: VI.8.4
Integer, algebraic: V.1.1
— Gaussian: V.1.1
— over a ring: V.1.1

Invertible fractional ideal: 11.5.7
— submodule: 11.5.6
Irreducible component: 11.4.1
— set: 11.4.1
— space: 11.4.1
Isolated subgroup: VI.4.2

Jacobson ring: V.3.4

Module graded, associated with a filtered module: 111.2.3
— ideally Hausdorff 111.5.1
— of fractions defined by a subset of a ring: 11.2.2
— projective, of rank $n$: 11.5.3
— pseudo-coherent: I.2.Ex.11
— pseudo-zero: VII.4.4
Monoid, divisor class: VII.1.2
Morphism for laws of composition not everywhere defined: VI.2.1
Multiplicative subset: 11.2.1

Nilradical of a ring: 11.2.6
Noetherian space: 11.4.2
Non-degenerate submodule: 11.5.5
Normalization lemma: V.3.1
Normed discrete valuation: VI.3.6
Nullstellensatz: V.3.3

Order group of a valuation: VI.3.2
— of an element for a valuation: VI.3.2
— reduced, of a formal power series: VII.3.8
Ordered pair of rings with the linear extension property: 1.3.7
Ostrowski’s theorem: VI.6.4

Place, finite at $x$: VI.2.2
— of a field: VI.2.2
— trivial: VI.2.2
Point, generic, of an irreducible space: II.4.Ex.2
Polygon, Newton: VI.4.Ex.11
Polynomial, distinguished: VII.3.8
— minimal: V.1.3
Preparation theorem: VII.3.8
Presentation of a module, — finite: 1.2.8
n-presentation: I.2.Ex.6
Presented, finitely (module): 1.2.8
Primary decomposition: IV.2.2 and Ex.20
— p-primary, ideal, submodule: IV.2.1 and Ex.20
Prime ideal: II.1.1
— spectrum: 11.4.3
Principal divisor: VII.1.1
— restricted adèle: VII.2.4
Principle of Noetherian induction: 11.4.2
Product filtration: III.2.1
Projective field: VI.2.1

Pseudo-injective, pseudo-surjective, pseudo-zero, pseudo-bijective (homomorphism): VII.4.4
Pseudo-isomorphism: VII.4.4
Pseudo-zero module: VII.4.4

Quasi-Galois extension: V.2.2
Quotient filtration: III.2.1

Radical of an ideal: 11.2.6
Rank at p of a projective module: 11.5.3
— of a projective module: 11.5.3
— rational, of a commutative group: VI.10.2
— residue: VI.8.5
Rational rank of a commutative group: VI.10.2
Reduced order: VII.3.8
— primary decomposition: IV.2.3
— ring: 11.2.6
— series: VII.3.8
Reflexive lattice: VII.4.2
Related local rings: VI.1.Ex.1
Relatively prime ideals: II.1.2
Representative system of extremal elements: VII.3.3
Residue class degree of a valuation: VI.8.1
— field: 11.3.1
— rank of a valuation: VI.8.5
Resolution, finite free, of a module: VII.4.7
Restricted adèle: VIII.2.4
— formal power series: 111.4.2
Ring, absolutely flat: I.2.Ex.17
— coherent (left, right): I.2.Ex.17
— decomposition: V.2.2
— filtered: 111.2.1
— filtered, associated with a graded ring: 111.2.1
— graded, associated with a filtered ring: 111.2.3
— inertia: V.2.2
— integrally closed in an algebra: V.1.2
— Jacobson: V.3.4
— linearly topologized: 111.4.2
— local: 11.3.1
— local, dominating a local ring: VI.1.1
— local, of A at p, of p (p a prime ideal): 11.3.1
— of a place: VI.2.3
— of a valuation: VI.3.2

Ring of fractions defined by a subset of a ring: 11.2.1
— reduced: 11.2.6
— semi-local: 11.3.5
— total, of fractions: 11.2.1
— unramified: V.2.Ex.19
— valuation, valuation ring of a field : VI. 1.1
— Zariski: 111.3.3
Rings, independent valuation: VI.7.2

Saturation of a submodule with respect to a multiplicative subset (with respect to a prime ideal) : 11.2.4
Semi-local ring: 11.3.5
Series, reduced: VII.3.8
— restricted formal power: 111.4.2
Set, irreducible: 11.4.1
— major, in a totally ordered group: VI.3.5
Space, irreducible: 11.4.1
— Noetherian: 11.4.2
Special topology: 11.4.3
Spectrum, prime, of a ring: 11.4.3
Strongly Laskerian module: IV.2.Ex.28
— primary submodule: IV.2.Ex.27
— relatively prime elements: 111.4.1
Subgroup, isolated, of an ordered group: VI.4.2
Submodule, invertible :II.5.6
— non-degenerate: 11.5.5
— primary, p-primary: IV.2.1
Subset, multiplicative, of a ring: 11.2.1
— multiplicative, generated by a subset: 11.2.1
— saturated multiplicative: II.2.Ex.1
Support of a module: 11.4.4
System, complete, of extensions of a valuation: VI.8.2
— formal, of generators: 111.2.9
— representative, of extremal elements: VII.3.3

Theorem, approximation, for absolute values: VI.7.3
— approximation, for valuations: VI.7.2
— Gelfand-Mazur: VI.6.4
— Hensel’s: III.4.3
— Hilbert’s zeros (Nullstellensatz): V.3.3
— Krull’s: 111.3.1
— Krull-Akizuki: VII.3.5
— Ostrowski’s: VI.6.3

Theorem, preparation: VII.3.8
— Stickelberger's : VI.8.Ex.18
— Zariski's Principal: V.3.Ex.7
Topologically nilpotent element: 111.4.3
Topology defined by a filtration: 111.2.5
— spectral: 11.4.3
— Zariski: 11.4.3
Transporter: 1.2.10
Trivial filtration: 111.2.1
— place: VI.2.2

Ultrametric absolute value: VI.6.1
Uniformizer for a discrete valuation: VI.3.6
Unramified valuation: VI.8.1

Valuation, valuation of an element $x$: VI.3.1 and 2
— discrete, normed discrete valuation: VI.3.6
— essential: VII.1.4 and Ex.26
— improper: VI.3.1
— ring: VI.1.1
— unramified: VI.8.1
Valuations, equivalent: VI.3.2
— independent: VI.7.2
Value field of a place: VI.2.2
— ultrametric absolute: VI.6.1

Weakly associated (prime ideal) with a module: IV.1.Ex.17

Zariski, ring: 111.3.3
— topology: 11.4.3 semi-local ring
    ↑
local ring
    ↑
---------------------------
integrally closed domain ↔ valuation ring
    ↑
completely integrally closed domain ↔ valuation ring of height 1
    ↑
Krull domain
    ↑
integral
Noetherian ring

In the case of Noetherian rings this table reduces to the following:

integrally closed domain        semi-local ring
    ↑                        ↑
Dedekind domain   factorial domain   local ring
    ↑                        ↑
principal ideal domain ↔ discrete valuation ring

In this table and the following, each row corresponds to a property a ring may possess and each column to a ring derived from the ring $\mathbf{A}$ ($p$ denoting a prime ideal of $\mathbf{A}$, $S$ a multiplicative subset of $\mathbf{A}$ not containing 0 and $\mathbf{A}'$ the integral closure of $\mathbf{A}$ in a finite algebraic extension $L$ of the field of fractions $K$ of $\mathbf{A}$). The ring $\mathbf{A}$ is assumed to possess the property indicated in the row; the word "yes") (resp. "no", "?"') at the intersection of this row and a column means that it is true (resp. false, still unknown) that every ring constructed from $\mathbf{A}$ by the process indicated by the column has the property indicated by the row.

The references indicate the place in this Book or the Book Algebra where the result in question is proved, and similarly for the two following works where results not mentioned in the text or in the exercises are concerned:

(1) A. Grothendieck, Éléments de géométrie algébrique, Chapter IV (Publ. Inst. Htes etudes Scient., nos. 20 and 24, 1964).
(2) M. Nagata, Local rings, Interscience (New York), 1962.

<table>
  <tr>
    <th></th>
    <th>A/p</th>
    <th>S^{-1}\mathbf{A}</th>
    <th>\mathbf{A}[X]</th>
    <th>\mathbf{A}[[X]]</th>
    <th>\mathbf{A}'</th>
  </tr>
  <tr>
    <td>A a principal ideal domain</td>
    <td>YES</td>
    <td>YES</td>
    <td>NO<br><i>Alg. VII,</i><br>§ 1, Ex. 1</td>
    <td>NO</td>
    <td>NO<br><i>Alg. VII,</i><br>1, Ex. 12</td>
  </tr>
  <tr>
    <td>A a Dedekind domain</td>
    <td>YES</td>
    <td>YES</td>
    <td>NO<br><i>Alg. VII,</i><br>§ 1, Ex. 1</td>
    <td>NO<br>VII, § 1,<br>Ex. 9</td>
    <td>YES<br>VII, § 2,<br>Cor. 2 to Prop. 9)</td>
  </tr>
</table> <table>
  <tr>
    <th></th>
    <th>A/p</th>
    <th>S^{-1}A</th>
    <th>A[X]</th>
    <th>A[[X]]</th>
    <th>A'</th>
  </tr>
  <tr>
    <td>A a factorial domain</td>
    <td>NO<br>'§ 1, Ex. !</td>
    <td><b>YES</b><br>VII, § 3, Prop. 3</td>
    <td><b>YES</b><br>VII, § 3, Th. 2</td>
    <td>NO<br>VII, § 3, Ex. 9</td>
    <td><b>NO</b><br><i>Alg.</i> VII, § 1, Ex. 12</td>
  </tr>
  <tr>
    <td>A a Noetherian integrally closed domain</td>
    <td>NO<br>'§ 1, Ex. !</td>
    <td><b>YES</b><br>'§ 1, Cor. to Prop. 16</td>
    <td><b>YES</b><br>'§ 1, Cor. 1 to Prop. 13</td>
    <td><b>YES</b><br>V, § 1, Prop. 14</td>
    <td>?</td>
  </tr>
  <tr>
    <td>A a field or a discrete valuation ring</td>
    <td><b>YES</b><br>VI, § 3, no. 6</td>
    <td><b>YES</b><br>VI, § 3, no. 6</td>
    <td><b>NO</b><br><i>Alg.</i> VII, § 1, Ex. 1</td>
    <td>NO<br>VII, § 1, Ex. 9</td>
    <td><b>NO</b><br>V, § 2, Ex. 6</td>
  </tr>
  <tr>
    <td>A a field or a valuation ring of height 1</td>
    <td><b>YES</b><br>VI, § 4</td>
    <td><b>YES</b><br>VI, § 4, Prop. 1</td>
    <td><b>NO</b><br><i>Alg.</i> VII, § 1, Ex. 1</td>
    <td>NO<br>VII, § 1, Ex. 9</td>
    <td><b>NO</b><br>V, § 2, Ex. 6</td>
  </tr>
  <tr>
    <td>A a valuation ring</td>
    <td><b>YES</b><br>VI, § 1, Th. 1</td>
    <td><b>YES</b><br>VI, § 1, Th. 1</td>
    <td><b>NO</b><br><i>Alg.</i> VII, § 1, Ex. 1</td>
    <td>NO<br>VII, § 1, Ex. 9</td>
    <td><b>NO</b><br>V, § 2, Ex. 6</td>
  </tr>
  <tr>
    <td>A a complete valuation ring</td>
    <td><b>YES</b><br>VI, § 5, Prop. 1</td>
    <td><b>YES</b><br>VI, § 7, Prop. 3</td>
    <td><b>NO</b><br><i>Alg.</i> VII, § 1, Ex. 1</td>
    <td>NO<br>VII, § 1, Ex. 9</td>
    <td><b>NO</b><br>V, § 2, Ex. 6</td>
  </tr>
  <tr>
    <td>A a Krull domain</td>
    <td>NO<br>V, § 1, Ex. 9</td>
    <td><b>YES</b><br>VII, § 1, Prop. 6</td>
    <td><b>YES</b><br>VII, § 1, Prop. 13</td>
    <td><b>YES</b><br>VII, § 1, Ex. 9</td>
    <td><b>YES</b><br>VII, § 1, Prop. 12</td>
  </tr>
</table>

In this table $a$ denotes an ideal of $\mathbf{A}$ distinct from $\mathbf{A}$, $S$ a multiplicative subset of $\mathbf{A}$ and $\mathbf{A}'$ the integral closure of $\mathbf{A}$ which is assumed to be an integral domain.

<table>
  <tr>
    <th></th>
    <th>A/a</th>
    <th>S^{-1}A</th>
    <th>A[X]</th>
    <th>A[[X]]</th>
    <th>A'</th>
  </tr>
  <tr>
    <td>A local</td>
    <td>YES</td>
    <td>NO<br>II, §2, Prop. 11</td>
    <td>NO</td>
    <td>YES<br>Alg. IV, §5, Prop. 4</td>
    <td>NO<br>V, 42, Ex. 20</td>
  </tr>
  <tr>
    <td>A local and complete</td>
    <td>?<br>YES if $\Lambda$ is Noetherian (III, §3, Prop. 6)</td>
    <td>NO<br>II, §2, Prop. 11</td>
    <td>NO</td>
    <td>YES<br>III, §2, Prop. 6</td>
    <td>?<br>YES if $\Lambda$ is Noetherian (1)</td>
  </tr>
  <tr>
    <td>A semi-local</td>
    <td>YES</td>
    <td>NO<br>IV, §2, Ex. 23(c)</td>
    <td>NO</td>
    <td>YES<br>Alg. IV, §5, Prop. 4</td>
    <td>YES if $\mathbf{A}$ is Noetherian<br>V, §2, Ex. 7</td>
  </tr>
  <tr>
    <td>A semi-local and complete</td>
    <td>?<br>YES if $\mathbf{A}$ is Noetherian (III, §3, Prop. 6)</td>
    <td>NO<br>IV, 42, Ex. 23(c)</td>
    <td>NO</td>
    <td>YES<br>III, §2, Prop. 6</td>
    <td>—</td>
  </tr>
  <tr>
    <td>A Noetherian</td>
    <td>YES<br>Alg. VIII, §2, Prop. 6</td>
    <td>YES<br>II, §2, Cor. 2 to Prop. 10</td>
    <td>YES<br>III, §2, Cor. 1 to Th. 2</td>
    <td>YES<br>III, §2, Cor. 6 to Th. 2</td>
    <td>NO<br>V, §1, Ex. 21<br>YES if $\mathbf{A}$ is locally complete (1)<br>$\mathbf{A}'$ is always a Krull domain (2)</td>
  </tr>
</table> (a) Let $\mathbf{A}$ be a ring and $m$ an ideal of $\mathbf{A}$ distinct from $\mathbf{A}$. Let $\mathbf{A}$ be given the $m$-adic topology and let $\hat{\mathbf{A}}$ denote its Hausdorff completion.

$$
\begin{array}{ll}
\mathbf{A} \text{ Hausdorff} & \text{YES} \\
\mathbf{A} \text{ Noetherian} & \text{YES (III, § 3, Proposition 8)} \\
\mathbf{A} \text{ local} & \text{YES (III, § 2, Proposition 19)} \\
\mathbf{A} \text{ semi-local} & \text{YES (III, § 2, Corollary to Proposition 19)} \\
\mathbf{A} \text{ a Zariski ring} & \text{YES (III, § 3, Proposition 8)}
\end{array}
$$

(b) Suppose now that $\mathbf{A}$ is local and Noetherian and that $m$ is its maximal ideal.

$$
\begin{array}{ll}
\mathbf{A} \text{ an integral domain} & \text{NO (III, § 3, Exercise 15 (b))} \\
\mathbf{A} \text{ an integrally closed domain} & \text{NO (2)} \\
& \text{YES for excellent rings (1)} \\
\mathbf{A} \text{ a discrete valuation ring} & \text{YES (VI, § 5, Proposition 5)} \\
\mathbf{A} \text{ reduced} & \text{NO (2)} \\
& \text{YES for excellent rings (1)}
\end{array}
$$
