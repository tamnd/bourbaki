---
book: fvr
book_title: Functions of a Real Variable
chapter: VI
chapter_title: GENERALIZED TAYLOR EXPANSIONS EULER-MACLAURIN SUMMATION FORMULA
section: 0
section_title: Historical Note
kind: historical
lang: en
source: fvr-i-vii
pdf_pages: 0314-0318
extraction: ocr
statements: 0
exercises: 0
content_sha256: f46444e85c3eb79a4d7395b05440c907d0dc354d8369c5239ce60b393fc50854
---

# HISTORICAL NOTE

(Chapters V and VI)

(N.B. Roman numerals refer to the bibliography to be found at the end of this note.)

The distinction between the “infinitely small” (or “infinitely large”) of different orders appeared implicitly in the first writings on the Differential Calculus, and for example in those of Fermat; it became fully articulated with Newton and Leibniz, with the theory of “differences of higher order”; and no time was lost before observing that in the most simple cases, the limit (or “true value”) of an expression of the form $f(x)/g(x)$ at a point where $f$ and $g$ both tend to 0 is given by the Taylor expansion of these functions on a neighbourhood of the point considered (“l’Hôpital’s rule”, probably due to Johann Bernoulli).

Apart from in the elementary case, the principal problem of “asymptotic evaluation” which presented itself to the mathematicians from the end of the XVII$^{th}$ century was the calculation, exact or approximate, of sums of the form $\sum_{k=1}^n f(k)$ when $n$ is very large; such a calculation was truly needed as much for interpolation and for the numerical evaluation of the sum of a series, as in the Calculus of Probabilities, where the “functions of large numbers” such as $n!$ or $\binom{a}{n}$ play a preponderant rôle. Already Newton, to obtain approximate values for $\sum_{k=1}^n \frac{1}{a+k}$ when $n$ is large, indicated a method which reduces (in this particular case) to the calculation of the first terms in the Euler-Maclaurin formula (I). Towards the end of the century, Jakob Bernoulli, in the course of his research in the Calculus of Probabilities, set himself to determine the sums $S_k(n) = \sum_{p=1}^{n-1} p^k$, polynomials in $n$ of which he discovered the general law of formation (without giving a proof) $^4$, so introducing for the first time, in the expression for the coefficients of these polynomials, the numbers which bear his name, and the induction relation which allows one to calculate them ((II), p. 97). In 1730, Stirling obtained an asymptotic expansion for $\sum_{k=1}^n \log(x+ka)$, as $n$ increases indefinitely, by a procedure for calculating the coefficients recursively.

$^4$ They are the primitives of the “Bernoulli polynomials” $B_k(x)$.

The decisive works of Euler on series and on related questions date from 1730 to 1745. Putting $S(n) = \sum_{k=1}^{n} f(k)$, he applied the Taylor formula to the function $S(n)$, which gave him

$$
f(n) = S(n) - S(n-1) = \frac{dS}{dn} - \frac{1}{2!} \frac{d^2 S}{dn^2} + \frac{1}{3!} \frac{d^3 S}{dn^3} - \cdots,
$$

an equation which he “inverted” by the method of undetermined coefficients, looking for a solution of the form

$$
S(n) = \alpha \int f(n)\, dn + \beta\, f(n) + \gamma \frac{df}{dn} + \delta \frac{d^2 f}{dn^2} + \cdots;
$$

he thus obtained, term-by-term,

$$
S(n) = \int f(n)\, dn + \frac{f(n)}{2} + \frac{1}{12} \frac{df}{dn} - \frac{1}{720} \frac{d^3 f}{dn^3} + \frac{1}{30\,240} \frac{d^5 f}{dn^5} - \cdots
$$

without in the first place being able to determine the law of formation of the coefficients (III $a$ and $d$). But about 1735, in analogy with the decomposition of a polynomial into linear factors, he did not hesitate to write the formula

$$
1 - \frac{\sin s}{\sin \alpha} = \left(1 - \frac{s}{\alpha}\right) \left(1 - \frac{s}{\pi - \alpha}\right)
$$
$$
\left(1 - \frac{s}{-\pi - \alpha}\right) \left(1 - \frac{s}{2\pi - \alpha}\right) \left(1 - \frac{s}{-2\pi - \alpha}\right) \cdots
$$

and on equating the coefficients of the expansions of both sides as entire series he obtained in particular (for $\alpha = \pi / 2$) the famous expressions for the series $\sum_{k=1}^{\infty} \frac{1}{n^{2k}}$

in terms of powers of $\pi$ (III $b$) $^5$. Several years later he perceived at last that the coefficients of these powers of $\pi$ are given by the same equations as those of his summation formula, and recognised their connection with the numbers introduced by Bernoulli, and with the coefficients of the series expansion of $z/(e^z - 1)$ (III $g$).

Independently of Euler, Maclaurin had arrived about the same time at the same summation formula, by a slightly less hazardous way, close to that which we have followed in the text; he effectively iterated the “Taylor” formula which expresses $f(x)$ in terms of the differences $f^{(2k+1)}(x+1) - f^{(2k+1)}(x)$, a formula which he obtained by “inverting” the Taylor expansions of these differences by the method of

$^5$ In 1743 Euler, in response to various contemporary critics, gave a somewhat more plausible derivation of the “Eulerian expansions” of the trigonometric functions; for example, the expansion of $\sin x$ as an infinite product is derived from the expression $\sin x = \frac{1}{2i}(e^{ix} - e^{-ix})$ and the fact that $e^{ix}$ is the limit of the polynomial $\left(1 + \frac{ix}{n}\right)^n$ (III $e$).

undetermined coefficients (IV); but he did not perceive the law of formation of the coefficients, discovered by Euler.

But Maclaurin, like Euler and all the mathematicians of his time, presented all these formulae as series expansions, whose convergence was not even studied. Not that the notion of a convergent series was totally neglected at this period; one had known since Jakob Bernoulli that the harmonic series is divergent, and Euler had even made this result clear by evaluating the sum of the first $n$ terms of this series with the help of his summation formula (III c and d); it was also Euler who remarked that the ratio of two consecutive Bernoulli numbers increases indefinitely, and consequently that an entire series having these numbers as coefficients cannot converge ((III f), p. 357) $^6$. But the tendency towards formal calculus was the stronger, and Euler’s extraordinary intuition even so did not prevent him from descending into the absurd, as when, for example, he wrote $0 = \sum_{n=-\infty}^{+\infty} x^n$ ((III f), p. 362) $^7$.

We have already seen (Historical Note to chap. IV) how the mathematicians at the beginning of the XIX$^{th}$ century, weary of this unbridled and unfounded formalism, brought Analysis back to the ways of rigour. Once the concept of a convergent series was made precise, the need appeared for simple criteria for showing the convergence of integrals and series by comparison with known integrals or series; Cauchy gave a number of such criteria in his Analyse algébrique (Va), while Abel, in a posthumous memoir (VI), obtained the logarithmic convergence criteria. Cauchy, on the other hand (V b), elucidated the paradox of such series as that of Stirling, obtained by applying the Euler-Maclaurin formula (and often called “semiconvergent series”): he showed that if (in view of Euler’s remark on the Bernoulli numbers) the general term $u_k(n)$ of such a series, for a fixed value of $n$, increases indefinitely with $k$, nonetheless for a fixed value of $k$ the partial sum $s_k(n) = \sum_{h=1}^k u_h(n)$ gives an asymptotic expansion (as $n$ tends to $+\infty$) of the function “represented” by the series, correspondingly more precise as $k$ is larger.

In the majority of the calculations of Classical Analysis it is possible to obtain a general law of formation for the asymptotic expansions of a function having a number of arbitrarily large terms; this fact has contributed to creating a lasting confusion (at least in the language) between series and asymptotic expansions; so much so that H. Poincaré, when he took the trouble, in 1886 (VIII), to codify the elementary rules of asymptotic expansions (following the integer powers of $1/x$ on a neighbourhood of $+\infty$), still employed the vocabulary of the theory of series. It was only with the appearance of asymptotic expansions coming from analytic number theory that a

$^6$ Since the series which Euler considered here was introduced with a view to numerical calculation, he took only the sum of the terms which start decreasing and from the index where the terms begin to increase he replaced them by a remainder whose origin he did not indicate (the remainder in the Euler-Maclaurin formula in its general form did not appear until Cauchy).
$^7$ It is ironic that this formula follows one page after a passage where Euler warned against the unconsidered use of divergent series!

istinction between the concept of an asymptotic expansion and a series was established, by reason of the fact that, in the majority of the problems which ory treats, one cannot obtain more than a very small number of terms explicitly (often only one) of the expansion sought.

These problems have also familiarised mathematicians with the use of comparison scales other than those of the (real or integer) powers of the variable. This notion is due above all to the works of P. du Bois-Reymond (VII) who, first, treated systematically the comparison of functions in a neighbourhood of a point, and, in very few works, recognised the “nonarchimedean” character of comparison scales, at the same time as he studied in a general manner integration and differentiation comparison relations, and deduced a host of interesting consequences (VII b). These sometimes lack clarity and rigour, and it is to G.H. Hardy (IX) that a presentation of du Bois-Reymond’s results is due: his principal contribution consisted in recognising and proving the existence of a set of “elementary functions”, functions, on which the usual operations of Analysis (notably differentiation) are applicable to the comparison relations $^8$.

———
not our remit to develop in these chapters the methods which allow one to obtain asymptotic expansions of functions belonging to certain particular categories, as for example certain types of integrals depending on a parameter, which appear quite frequently in analysis; on this point (and in particular on the important methods of Laplace and Darboux) the reader may consult the book of Hardy (IX) already mentioned, which contains a very complete bibliography.

(I) I. NEWTON, in St. P. RIGAUD, Correspondence of scientific men, Oxford, 1841, t. II, p. 309-310.
(II) Jakob Bernoulli, Ars conjectandi, Bâle, 1713.
(III) L. EULER, Opera omnia (1), t. XIV; Commentationes analyticae . . . , Leipzig-Berlin (Teubner), 1924: a) Methodus generalis summandi progressiones, p. 42-72 (=Comm. Acad. petrop , t. VI (1732-33)); b) De summis serierum reciprocarum, p. 73-86 (=Comm. Acad. petrop., t. VII (1734-35)); c) De progressionibus harmonicis observationes, p. 87-100 (ibid.); d) Inventio summae cujusque seriei . . . , p. 108-123 (=Comm. Acad. petrop., t. VIII (1736)); e) De summis serierum reciprocarum . . . dissertatio altera . . . , p. 138-155 (=Misc. Berol., t. VII (1743)); f) Consideratio progressionis . . . , p. 350-363 (=Comm. Acad. petrop., t. XI (1739)); g) De seriebus quibusdam considerationes, p. 407-462 (=Comm. Acad. petrop., t. XII (1740)).
(IV) C. MACLAURIN, A complete treatise of fluxions, Edinburgh, 1742.
(V) A. L. CAUCHY: a) Cours d’Analyse de l’Ecole Royale Polytechnique, 1re partie, 1821 (=Œuvres, (2), t. III, Paris (Gauthier-Villars), 1897; b) Œuvres, (1), t. VIII, p. 18-25, Paris (Gauthier-Villars), 1893.
(VI) N. H. ABEL, Œuvres, t. II, p. 197-205, éd. Sylow and Lie, Christiania, 1881.
(VII) P. DU BOIS-REYMOND: a) Sur la grandeur relative des infinis des fonctions, Ann. di Mat. (2), t. IV (1871), p. 338-353; b) Ueber asymptotische Werthe, infinitäre Approximationen und infinitäre Auflösung von Gleichungen, Math. Ann., t. VIII (1875), p. 362-414.
(VIII) H. POINCARÉ, Sur les intégrales irrégulières des équations linéaires, Acta Math., t. VIII (1886), p. 295-344.
(IX) G. H. HARDY, Orders of infinity, Cambridge tracts, n° 12, 2nd ed., Cambridge University Press, 1924.
