---
book: ac
book_title: Commutative Algebra
chapter: I
chapter_title: FLAT MODULES
section: 4
section_title: Flat modules and "Tor" functors
lang: en
source: ac-i-vii
book_pages: 37-38, 50
pdf_pages: 0057-0058, 0070-0070
extraction: ocr
statements: 3
exercises: 1
content_sha256: 9fd11944f9ccd26af40fbfd7087174fd30283103e635ee58c967ecaf0bfa5f58
---

## 4. FLAT MODULES AND "TOR" FUNCTORS

For the benefit of readers conversant with Homological Algebra (*), we shall indicate quickly how the theory of flat modules is related to that of Tor functors.

#### Proposition 1 {#ac-i-s4-prop-1 .statement}

Let E be a right A-module. The following four properties are equivalent:

(a) E is flat.
(b) For every left A-module F and every integer n $\geq 1$, $\mathrm{Tor}_n^A(E, F) = 0$.
(c) For every left A-module F, $\mathrm{Tor}_1^A(E, F) = 0$.
(d) For every finitely generated left ideal $a$ of A,
$$
\mathrm{Tor}_1^A(E, A_s/a) = 0.
$$

We show that (a) implies (b). Let
$$
\cdots \to L_n \to L_{n-1} \to \cdots \to L_0 \to F \to 0
$$
be a free resolution of F. As E is flat, the sequence
$$
(1) \quad \cdots \to E \otimes L_n \to E \otimes L_{n-1} \to \cdots \to E \otimes L_0 \to E \otimes F \to 0
$$
is exact. As the $\mathrm{Tor}_n^A(E, F)$ are isomorphic to homology groups of the complex (1), they are zero for $n \geq 1$. It is trivial that (b) implies (c) and (c) implies (d). We show finally that (d) implies (a). The exact sequence
$$
0 \to a \to A, \to A_s/a \to 0
$$
gives the exact sequence
$$
\mathrm{Tor}_1^A(E, A_s/a) \to E \otimes_A a \to E \otimes_A A.
$$
As (d) holds, the canonical homomorphism
$$
E \otimes_A a \to E \otimes_A A = E
$$
is injective, which means that E is flat (§ 2, no. 3, Proposition 1).

Proposition 1 provides a characterization of flat modules which is often useful in applications. We shall restrict ourselves, by way of an example, to giving a

(*) See the part of this Treatise devoted to categories and, in particular, Abelian categories (in preparation). Until this is published, the reader can consult H. CARTAN-S. EILENBERG, Homological Algebra, Princeton, 1956, or R. GODEMENT, Théorie des Faisceaux, Paris (Hermann), 1958.

$$
\operatorname{Tor}_1^A(E', F) \to \operatorname{Tor}_1^A(E, F) \to \operatorname{Tor}_1^A(E'', F)
$$

shows that $\operatorname{Tor}_1^A(E, F) = 0$ for every left A-module F, hence E is flat. If E and E'' are flat, the exact sequence

$$
\operatorname{Tor}_2^A(E'', F) \to \operatorname{Tor}_1^A(E', F) \to \operatorname{Tor}_1^A(E, F)
$$

shows that $\operatorname{Tor}_1^A(E', F) = 0$, hence E' is flat.

#### Proposition 2 {#ac-i-s4-prop-2 .statement}

*Let R, S be two rings, $\rho : \mathbf{R} \to \mathbf{S}$ a homomorphism and F a left R-module. The following two properties are equivalent:*
(a) $\operatorname{Tor}_1^R(\rho_*(E), F) = 0$ for every right S-module E.
(b) *The left S-module $\varphi^*(F) = F_{(S)} = S \otimes_R F$ is flat and $\operatorname{Tor}_1^R(\rho_*(S_d), F) = 0$.*

Suppose that (a) holds. Taking $E = S_d$, we see that $\operatorname{Tor}_1^R(\rho_*(S_d), F) = 0$. We show also that $F_{(S)}$ is a flat S-module. For that, we note that, if E is a right S-module, the additive group $E \otimes_S F_{,,}$ is identified with $\rho_*(E) \otimes_R F$. Then if there is an exact sequence of right S-modules

$$
0 \to E' \to E \to E'' \to 0
$$

we obtain, using (a), an exact sequence

$$
0 \to \rho_*(E') \otimes_R F \to \rho_*(E) \otimes_R F \to \rho_*(E'') \otimes_R F \to 0
$$

or also

$$
0 \to E' \otimes_S F_{(S)} \to E \otimes_S F_{(S)} \to E'' \otimes_S F_{(S)} \to 0
$$

which proves that $F_{(S)}$ is flat.

Conversely, if (b) holds, we have first of all, for every *free* right S-module $L = S_d^{(I)}$, $\operatorname{Tor}_1^R(\rho_*(L), F) = (\operatorname{Tor}_1^R(\rho_*(S_d), F))^{(I)} = 0$. Every right S-module E can be written in the form $E = L/H$ for a suitable free S-module L; then we have the exact sequence

(2) $0 = \operatorname{Tor}_1^R(\rho_*(L), F) \to \operatorname{Tor}_1^R(\rho_*(E), F) \to \rho_*(H) \otimes_R F \to \rho_*(L) \otimes_R F.$

But as $F_{,,}$ is flat, the homomorphism $H \otimes_S F_{(S)} \to L \otimes_S F_{(S)}$ is injective and is identified with the homomorphism

$$
\rho_*(H) \otimes_R F \to \rho_*(L) \otimes_R F.
$$

Then it follows from (2) that $\operatorname{Tor}_1^R(\rho_*(E), F) = 0$.

#### Remark {#ac-i-s4-n0-rem-1 .statement}

Proposition 2 also follows from the existence of the exact sequence

$$
E \otimes_S \operatorname{Tor}_1^R(\rho_*(S_d), F) \to \operatorname{Tor}_1^R(\rho_*(E), F) \to \operatorname{Tor}_1^S(E, S_d \otimes_R F) \to 0
$$

arising from the spectral sequence of the "associativity" of the Tor functors.

### Exercises {#ac-i-s4-exercises}

See the [exercises for § 4](exercises/s4/).
