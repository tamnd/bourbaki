---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 9
section_title: Modules dualisants
lang: en
source: ac-x-fr
pdf_pages: 0124-0140, 0174-0177
extraction: ocr
subsections:
    - "no": 1
      title: Modules dualisants
      page: 0
      pdf_page: 124
    - "no": 2
      title: Quotient par une suite régulière
      page: 128
      pdf_page: 127
    - "no": 3
      title: Changement d’anneaux
      page: 130
      pdf_page: 129
    - "no": 4
      title: Structure des modules dualisants
      page: 133
      pdf_page: 132
    - "no": 5
      title: Dualité des modules de type fini
      page: 134
      pdf_page: 133
    - "no": 6
      title: 'Exemple : le cas de la dimension 1'
      page: 0
      pdf_page: 136
statements: 31
exercises: 12
content_sha256: 70b41f4e0959618816afc0363d5324215a447233f0a954a4c83161f076065312
translated_from: content/fr/ac/X/09_s9_modules_dualisants.md
source_lang: fr
translation_method: machine
source_content_sha256: e91759ba70639eaebfa25698b669acf6e3da97d31ed7579081129197fa443e8f
translation_model: gpt-5.4
translation_run: translate-en-mt-c2b0a5e6
glossary_version: 34
glossary_terms_sha256: 9df319c0388461b762c85fbeca7f05404f1e48bf468eb449ae14176d34562212
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 9. DUALIZING MODULES

### 1. Dualizing modules

#### Definition 1 {#ac-x-s9-def-1 .statement}

Let $A$ be a noetherian ring. One says that a $\Lambda$-module $\Omega$ is dualizing if it is finitely generated and if, for every maximal ideal $m$ of $\Lambda$, the $A/m$-vector space $\mathrm{Ext}_A^i(A/m, \Omega)$ is zero for $i \neq \mathrm{ht}(m)$ and of dimension 1 for $i = \mathrm{ht}(m)$.

For every maximal ideal $m$ of $A$ and every integer $i$, the $A/m$-vector space $\mathrm{Ext}_A^i(A/m, \Omega)$ is canonically isomorphic to $\mathrm{Ext}_{A_m}^i(A/m, \Omega_m)$ ($\S$ 3, No. 2, prop. 2). Consequently, for a finitely generated $A$-module $\Omega$ to be dualizing, it is necessary and sufficient that the $A_m$-module $\Omega_m$ be dualizing for every maximal ideal $m$ of $A$.

#### Example 1 {#ac-x-s9-n1-exa-1 .statement}

If the ring $A$ is local and artinian, the dualizing $A$-modules are the finitely generated injective $A$-modules $\Omega$ such that $\mathrm{Hom}_A(\kappa_A, \Omega)$ is of dimension 1 ($\S$ 3, No. 3, prop. 6), that is to say the Matlis $A$-modules ($\S$ 8, No. 3).

#### Example 2 {#ac-x-s9-n1-exa-2 .statement}

For a noetherian ring $A$ to be Gorenstein, it is necessary and sufficient that the $A$-module $A$ be dualizing ($\S$ 3, No. 7, prop. 11). In particular, the $A$-module $A$ is dualizing when $A$ is regular.

#### Remark 1 {#ac-x-s9-n1-rem-1 .statement}

Let $A$ be a local noetherian ring and $\Omega$ a finitely generated $A$-module. The residue field $\kappa_{\widehat{A}}$ identifies with $\kappa_A$, and the $\widehat{A}$-module $\widehat{\Omega}$ with $\widehat{A} \otimes_A \Omega$ (III, $\S$ 3, No. 4, th. 3). It then follows from A, X, p. 111, prop. 10 that the $\kappa_A$-vector space $\mathrm{Ext}_A^i(\kappa_A, \Omega)$ is canonically isomorphic to $\mathrm{Ext}_{\widehat{A}}^i(\kappa_{\widehat{A}}, \widehat{\Omega})$. Consequently, for the $A$-module $\Omega$ to be dualizing, it is necessary and sufficient that the $\widehat{A}$-module $\widehat{\Omega}$ be dualizing.

#### Remark 2 {#ac-x-s9-n1-rem-2 .statement}

Let $\Omega$ be a dualizing $A$-module; for every projective $A$-module $L$ of rank 1, the $A$-module $\Omega \otimes_A L$ is dualizing (A, X, p. 108, prop. 7, b)). We shall see below (No. 4, prop. 6) that every dualizing $A$-module is isomorphic to a module of this form.

#### Proposition 1 {#ac-x-s9-prop-1 .statement}

Let $A$ be a noetherian ring and $\Omega$ a dualizing $A$-module.

a) $A$ is a Macaulay ring, and the $A$-module $\Omega$ is Macaulay.

b) One has $\mathrm{di}_A(\Omega) = \dim(\Omega) = \dim(A)$.

Suppose first that the ring $A$ is local, and let $d$ denote its dimension. Prop. 6 of § 3, No. 3 implies $\mathrm{di}_A(\Omega) = d$, hence $\mathrm{prof}(A) = d$ by prop. 9 of § 3, No. 6, so that $A$ is a Macaulay ring. Moreover, one has $\mathrm{prof}(\Omega) = d$ by definition of depth; since one has $\mathrm{prof}(\Omega) \leq \dim(\Omega) \leq d$, one deduces the proposition in this case.

In the general case, the $A_m$-module $\Omega_m$ is dualizing for every maximal ideal $m$ of $A$, hence $A_m$ is a Macaulay ring and $\Omega_m$ an $A_m$-module which is Macaulay by what precedes, which implies a). Moreover one has $\mathrm{di}_{A_m}(\Omega_m) = \dim(\Omega_m) = \dim(A_m)$ for every maximal ideal $m$, whence b) by passing to the least upper bound (§ 3, No. 2, prop. 3).

#### Proposition 2 {#ac-x-s9-prop-2 .statement}

*Let A be a noetherian ring, $\Omega$ a dualizing A-module. For every prime ideal $p$ of A, the $A_p$-module $\Omega_p$ is dualizing.*

Consider a saturated chain $p \subset p_1 \subset \ldots \subset p_r$ of prime ideals of A such that the ideal $p_r$ is maximal. Reasoning by induction on $r$, one may suppose that the $A_{p_1}$-module $\Omega_{p_1}$ is dualizing. Replacing A by $A_{p_1}$ and $p$ by $pA_{p_1}$, one is reduced to the case where the ring A is local and where the chain $p \subset m_A$ is saturated.

Put then $d = \dim(A) = \mathrm{ht}(m_A)$. One has $\dim(A_p) = \mathrm{ht}(p) = d - 1$ since A is a Macaulay ring (§ 2, No. 2, cor. of prop. 2). For every integer $i$, the $A_p$-module $\mathrm{Ext}^i_{A_p}(\kappa(p), \Omega_p)$ is isomorphic to $\mathrm{Ext}^i_A(A/p, \Omega)_p$ (§ 3, No. 2, prop. 2); it is therefore enough to prove that the $A/p$-module $\mathrm{Ext}^i_A(A/p, \Omega)$ vanishes for $i \neq d - 1$ and is of rank one for $i = d - 1$.

Let $x$ be an element of $m_A - p$, and $\overline{x}$ its class in $A/p$. Consider the exact sequence of A-modules

$$
0 \to A/p \xrightarrow{\overline{x}} A/p \longrightarrow A/(p + xA) \to 0 .
$$

The A-module $A/(p + xA)$ is of finite length since its support is reduced to $m_A$; since the A-module $\Omega$ is dualizing, one has $\mathrm{Ext}^i_A(A/(p + xA), \Omega) = 0$ for $i \neq d$ ($§ 8$, No. 5, example 3). It then follows from the exact sequence of extension modules associated with the sequence above and with $\Omega$ that the homothety of ratio $x$ in the A-module $\mathrm{Ext}^i_A(A/p, \Omega)$ is surjective for $i \neq d - 1$, which implies that this module is zero (Nakayama lemma). In particular $\mathrm{Ext}^d_A(A/p, \Omega)$ is zero, and one obtains an exact sequence

$$
0 \to \mathrm{Ext}^{d-1}_A(A/p, \Omega) \xrightarrow{x} \mathrm{Ext}^{d-1}_A(A/p, \Omega) \longrightarrow \mathrm{Ext}^d_A(A/(p + xA), \Omega) \to 0 .
$$

One has $\mathrm{long}_A(\mathrm{Ext}^i_A(A/(p + xA), \Omega)) = \mathrm{long}_A(A/(p + xA))$ (*loc. cit.*); the proposition then follows from the following lemma, applied to the ring $B = A/p$ and the B-module $M = \mathrm{Ext}^{d-1}_A(A/p, \Omega)$:

#### Lemma 1 {#ac-x-s9-lem-1 .statement}

*Let B be a local noetherian integral ring of dimension 1, and M a finitely generated torsion-free B-module. Suppose that one has $\mathrm{long}_B(M/xM) = \mathrm{long}_B(B/xB)$ for every nonzero element x of B. Then the B-module M is of rank 1.*

For let $r$ be the rank of M; there exists a free submodule L of M of rank $r$ such that $M/L$ is a torsion module (VII, § 4, No. 1, corollary of proposition 1), hence of finite length (VII, § 2, No. 5, lemma 1). The annihilator of $M/L$ is not reduced to 0, and therefore contains a nonzero element $x$ of $m_B$. Consider the commutative diagram

$$
\begin{array}{cccccccc}
0 & \to & L & \longrightarrow & M & \longrightarrow & M/L & \to 0 \\
& & \downarrow_{x_L} & & \downarrow_{x_M} & & \downarrow_0 & \\
0 & \to & L & \longrightarrow & M & \longrightarrow & M/L & \to 0 .
\end{array}
$$

By the snake lemma (A, X, p. 4, proposition 2), one deduces from it an exact sequence

$$
0 \to M/L \longrightarrow L/xL \longrightarrow M/xM \longrightarrow M/L \to 0 ,
$$

whence $\operatorname{long}(M/xM) = \operatorname{long}(L/xL)$. Since $\operatorname{long}(M/xM) = \operatorname{long}(B/xB)$ by hypothesis and $\operatorname{long}(L/xL) = r \operatorname{long}(B/xB)$, one deduces that $r = 1$.

#### Corollary 1 {#ac-x-s9-lem-1-cor-1 .statement}

*For every multiplicative subset S of A, the S$^{-1}$A-module S$^{-1}\Omega$ is dualizing.*

#### Corollary 2 {#ac-x-s9-lem-1-cor-2 .statement}

*The support of $\Omega$ is equal to Spec(A).*

Indeed a dualizing module over a local ring is nonzero by definition.

#### Corollary 3 {#ac-x-s9-lem-1-cor-3 .statement}

*Let M be a finitely generated A-module, and let i be an integer. The A-module $\operatorname{Ext}_A^i(M, \Omega)$ is finitely generated, and its support is of codimension $\geqslant i$ in Spec(A).*

The first assertion follows from A, X, p. 108, corollary. Let $\mathfrak{p}$ be a prime ideal of the support of $\operatorname{Ext}_A^i(M, \Omega)$. One has $\operatorname{Ext}_A^i(M, \Omega)_\mathfrak{p} \neq 0$, hence $\operatorname{Ext}_{A_\mathfrak{p}}^i(M_\mathfrak{p}, \Omega_\mathfrak{p}) \neq 0$ (§ 3, No. 2, proposition 2), which implies $\operatorname{di}_{A_\mathfrak{p}}(\Omega_\mathfrak{p}) \geqslant i$. Since $\Omega_\mathfrak{p}$ is a dualizing $A_\mathfrak{p}$-module (proposition 2), one has $\operatorname{di}_{A_\mathfrak{p}}(\Omega_\mathfrak{p}) = \dim(A_\mathfrak{p})$ (proposition 1), whence the corollary.

#### Proposition 3 {#ac-x-s9-prop-3 .statement}

*Let A be a local noetherian ring, $\Omega$ a dualizing A-module and M a finitely generated A-module.

a) *One has $\operatorname{Ext}_A^i(M, \Omega) = 0$ for $i < \dim(A) - \dim_A(M)$.*

b) *Put $c = \dim(A) - \dim_A(M)$. If M is nonzero, the A-module $\operatorname{Ext}_A^c(M, \Omega)$ is nonzero.*

c) *One has $\operatorname{Ext}_A^i(M, \Omega) = 0$ for $i > \dim(A) - \operatorname{prof}_A(M)$.*

Assume M nonzero and denote by F its support. By proposition 9 of § 1, No. 5, the conjunction of assertions a) and b) is equivalent to $\operatorname{prof}_F(\Omega) = c$. But since $\Omega$ is Cohen-Macaulay and its support is equal to Spec(A) (proposition 1 and corollary 2 of proposition 2), one has

$$
\operatorname{prof}_F(\Omega) = \operatorname{codim}(F, \operatorname{Spec}(A)) = c
$$

(§ 2, No. 1, corollary of proposition 1 and No. 2, corollary of proposition 2).

Let us prove c) by induction on the depth of M. If $\operatorname{prof}_A(M) = 0$, one indeed has $\operatorname{Ext}_A^i(M, \Omega) = 0$ for $i > \dim(A)$, since $\operatorname{di}_A(\Omega) = \dim(A)$ (proposition 1). Assume $\operatorname{prof}_A(M) > 0$; then there exists an element $x$ of $\mathfrak{m}_A$ such that the homothety of ratio $x$ is injective in M. One has $\operatorname{prof}_A(M/xM) = \operatorname{prof}_A(M) - 1$ (§ 1, No. 4, proposition 7).

Consider the exact sequence of extension modules

$$
\operatorname{Ext}_A^i(M, \Omega) \xrightarrow{x} \operatorname{Ext}_A^i(M, \Omega) \longrightarrow \operatorname{Ext}_A^{i+1}(M/xM, \Omega)
$$

associated with the exact sequence

$$
0 \to M \xrightarrow{x} M \longrightarrow M/xM \to 0 .
$$

For $i > \dim(A) - \operatorname{prof}_A(M)$, the $A$-module $\operatorname{Ext}_A^{i+1}(M/xM, \Omega)$ is zero by the induction hypothesis; therefore the homothety with ratio $x$ is surjective in $\operatorname{Ext}_A^i(M, \Omega)$, which implies that this $A$-module is zero (Nakayama's lemma). This proves c).

#### Corollary {#ac-x-s9-n1-cor-1 .statement}

*If $M$ is Macaulay, then $\operatorname{Ext}_A^i(M, \Omega) = 0$ for $i \neq c$; the $A$-module $\operatorname{Ext}_A^c(M, \Omega)$ is Macaulay, and its support is equal to that of $M$.*

The first assertion follows from Prop. 3, a) and c). Let $p \in \operatorname{Supp}(M)$; by Prop. 1 of § 2, No. 1, applied to $M$ and to $A$, we have

$$
\dim(A_p) - \dim_{A_p}(M_p) = \dim(A) - \dim_A(M) = c ;
$$

since the $A_p$-module $\Omega_p$ is dualizing (Prop. 2), it follows from Prop. 3, b) that the $A_p$-module $\operatorname{Ext}_A^c(M_p, \Omega_p)$ is not zero. Hence the support of $\operatorname{Ext}_A^c(M, \Omega)$ is equal to that of $M$.

Finally, let us prove, by induction on $\dim(M)$, that the $A$-module $\operatorname{Ext}_A^c(M, \Omega)$ is Macaulay. The assertion is true when $\dim(M) = 0$, since every module of finite length is Macaulay. Suppose $\dim(M) > 0$ and choose an element $x$ of $\mathfrak{m}_A$ such that the homothety $x_M$ is injective. The $A$-module $M/xM$ is Macaulay ($§ 2$, No. 3, Prop. 4), of dimension $\dim(M) - 1$. In view of the foregoing, the exact sequence of extension modules associated with the exact sequence $0 \to M \xrightarrow{x} M \longrightarrow M/xM \to 0$ reduces to

$$
0 \to \operatorname{Ext}_A^c(M, \Omega) \xrightarrow{x} \operatorname{Ext}_A^c(M, \Omega) \longrightarrow \operatorname{Ext}_A^{c+1}(M/xM, \Omega) \to 0 ;
$$

Prop. 4 of § 2, No. 3 and the induction hypothesis then imply that $\operatorname{Ext}_A^c(M, \Omega)$ is Macaulay, whence the corollary.

### 2. Quotient by a regular sequence

#### Proposition 4 {#ac-x-s9-prop-4 .statement}

*Let $A$ be a noetherian ring, $J$ an ideal of $A$ generated by an $A$-regular sequence $x$, and $\Omega$ a finitely generated $A$-module.

a) If the $A$-module $\Omega$ is dualizing, the sequence $x$ is $\Omega$-regular and the $A/J$-module $\Omega/J\Omega$ is dualizing;

b) If the $A/J$-module $\Omega/J\Omega$ is dualizing, if $J$ is contained in the radical of $A$, and if the sequence $x$ is $\Omega$-regular, the $A$-module $\Omega$ is dualizing.*

Reasoning by induction on the length of the sequence $x$, we are reduced to the case where the latter consists of a single element $x$. Suppose that the $A$-module $\Omega$ is dualizing. For every maximal ideal $m$ of $A$ containing $x$, one has $\dim(A_m/xA_m) = \dim(A_m) - 1$

Let \overline{A} denote the ring A/xA; let m be a maximal ideal of A containing x, and let \overline{m} be its image in \overline{A}. The A-module A/m is annihilated by x, and is identified with \overline{A}/\overline{m} ; hence for every integer i \geqslant 1 there is an isomorphism Ext^i_A(A/m, \Omega) \longrightarrow \operatorname{Ext}^{i-1}_{\overline{A}}(\overline{A}/\overline{m}, \Omega/x\Omega) (§ 3, n° 4, prop. 7). One has

$$
\operatorname{ht}(\overline{m}) = \dim(\overline{A}_m) = \dim(A_m/xA_m) = \dim(A_m) - 1 = \operatorname{ht}(m) - 1
$$

(VIII, § 3, n° 1, cor. 2, a)). Now the maximal ideals of \overline{A} are the ideals \overline{m}, where m is a maximal ideal of A containing x; and if moreover x belongs to the radical of A, every maximal ideal of A contains x. The proposition follows.

#### Corollary 1 {#ac-x-s9-prop-4-cor-1 .statement}

**Let A be an integral noetherian ring. Every dualizing A-module is torsion-free and of rank 1.**

Let \Omega be a dualizing A-module; it is torsion-free by prop. 4. Let K be the field of fractions of A; the K-vector space K \otimes_A \Omega is dualizing (n° 1, prop. 2), hence of dimension 1.

#### Corollary 2 {#ac-x-s9-prop-4-cor-2 .statement}

**Let A be a local Macaulay ring, \Omega a finitely generated A-module, and x a maximal secant sequence of elements of m_A, generating an ideal J. The following conditions are equivalent:**

(i) the A-module \Omega is dualizing ;
(ii) the A-module \Omega is a Macaulay module of dimension equal to \dim(A), and \Omega/J\Omega is an indecomposable injective module over the artinian local ring A/J ;
(iii) the sequence x is \Omega-regular and \Omega/J\Omega is an indecomposable injective module over the artinian local ring A/J ;
(iv) the sequence x is \Omega-regular, one has \operatorname{long}_A(\Omega/J\Omega) = \operatorname{long}_A(A/J) and the \kappa_A-vector space \operatorname{Hom}_A(\kappa_A, \Omega/J\Omega) is of dimension 1.

(i) \Rightarrow (ii) : if \Omega is dualizing, it is Macaulay and of dimension \dim(A) (n° 1, prop. 1). The sequence x is A-regular since A is a Macaulay ring; by prop. 4, the A/J-module \Omega/J\Omega is dualizing, and hence is a Matlis A/J-module (n° 1, example 1).

(ii) \Rightarrow (iii) : under assumption (ii), one has \dim(\Omega) = \dim(A) and \dim(\Omega/J\Omega) = \dim(A/J) = 0, so that the sequence x is secant for \Omega, hence \Omega-regular (§ 2, n° 3, th. 1).

(iii) \Rightarrow (i) : under the assumptions of (iii), the A/J-module \Omega/J\Omega is a Matlis A-module, and hence is dualizing (n° 1, example 1) ; by prop. 4 the A-module \Omega is dualizing.

(iii) \Leftrightarrow (iv) : this follows from the remark in § 8, n° 3.

### 3. Change of rings

#### Proposition 5 {#ac-x-s9-prop-5 .statement}

Let $\rho : A \to B$ be a homomorphism of noetherian rings, making $B$ into a flat $A$-module. Assume that for every maximal ideal $n$ of $B$, the ring $\kappa(\rho^{-1}(n)) \otimes_A B$ is a Gorenstein ring. Let $\Omega$ be a dualizing $A$-module ; the $B$-module $\Omega_{(B)}$ is dualizing.

Let $n$ be a maximal ideal of $B$, and $p$ its inverse image in $A$. The $A_p$-module $B_n$ is flat, the $A_p$-module $\Omega_p$ is dualizing, $\Omega_{(B)} \otimes_B B_n$ is identified with $\Omega_p \otimes_{A_p} B_n$ and $\kappa_{A_p} \otimes_{A_p} B_n$, which is identified with a ring of fractions of $\kappa(p) \otimes_A B$, is a Gorenstein ring. It is therefore enough to prove the proposition when $\rho$ is a local homomorphism of local rings, which we shall henceforth assume.

Let us first treat the case where the rings $A$ and $B$ are artinian. Put $C = B/\mathfrak{m}_A B$. Since $B$ is flat over $A$, the $B$-module $\mathrm{Hom}_B(C, \Omega_{(B)})$ is isomorphic to $\mathrm{Hom}_A(\kappa_A, \Omega) \otimes_A B$ (I, § 2, n° 10, prop. 11), hence to $\mathrm{Hom}_A(\kappa_A, \Omega) \otimes_{\kappa_A} C$. One deduces a sequence of isomorphisms

$$
\mathrm{Hom}_B(\kappa_B, \Omega_{(B)}) \longrightarrow \mathrm{Hom}_C(\kappa_C, \mathrm{Hom}_B(C, \Omega_{(B)})) \longrightarrow \mathrm{Hom}_C(\kappa_C, \mathrm{Hom}_A(\kappa_A, \Omega) \otimes_{\kappa_A} C)
$$
$$
\longrightarrow \mathrm{Hom}_A(\kappa_A, \Omega) \otimes_{\kappa_A} \mathrm{Hom}_C(\kappa_C, C) .
$$

The $\kappa_A$-vector space $\mathrm{Hom}_A(\kappa_A, \Omega)$ is of dimension 1 since $\Omega$ is dualizing, and the same holds for the $\kappa_C$-vector space $\mathrm{Hom}_C(\kappa_C, C)$ since $C$ is a Gorenstein ring; consequently the $\kappa_B$-vector space $\mathrm{Hom}_B(\kappa_B, \Omega_{(B)})$ is of dimension 1.

Let $M$ be a $B$-module of finite length; let us prove by induction on $\mathrm{long}_B(M)$ that one has $\mathrm{long}_B(\mathrm{Hom}_B(M, \Omega_{(B)})) \leqslant \mathrm{long}_B(M)$. The assertion is clear if $M = 0$, and it follows from the preceding if $M = \kappa_B$. Suppose $\mathrm{long}_B(M) \geqslant 2$. There exists an exact sequence of $B$-modules
$$
0 \to M' \to M \to \kappa_B \to 0
$$
with $\mathrm{long}_B(M') < \mathrm{long}_B(M)$. One deduces from this an exact sequence
$$
0 \to \mathrm{Hom}_B(\kappa_B, \Omega_{(B)}) \to \mathrm{Hom}_B(M, \Omega_{(B)}) \to \mathrm{Hom}_B(M', \Omega_{(B)}) ,
$$
and one concludes by applying the induction hypothesis to $M'$.

Let $N$ be the kernel of the canonical surjection of $\kappa_A \otimes_A B$ onto $\kappa_B$. Put $m = \mathrm{long}_B(\kappa_A \otimes_A B)$; one has $\mathrm{long}_B(N) = m - 1$. Consider the exact sequence of $B$-modules
$$
0 \to \mathrm{Hom}_B(\kappa_B, \Omega_{(B)}) \longrightarrow \mathrm{Hom}_B(\kappa_A \otimes_A B, \Omega_{(B)}) \longrightarrow \mathrm{Hom}_B(N, \Omega_{(B)})
$$
$$
\longrightarrow \mathrm{Ext}_B^1(\kappa_B, \Omega_{(B)}) \longrightarrow \mathrm{Ext}_B^1(\kappa_A \otimes_A B, \Omega_{(B)}) .
$$

The $B$-modules $\mathrm{Hom}_B(\kappa_A \otimes_A B, \Omega_{(B)})$ and $\mathrm{Ext}_B^1(\kappa_A \otimes_A B, \Omega_{(B)})$ are respectively isomorphic to $\mathrm{Hom}_A(\kappa_A, \Omega) \otimes_A B$ and $\mathrm{Ext}_A^1(\kappa_A, \Omega) \otimes_A B$, that is to say to $\kappa_A \otimes_A B$ and to 0. The lengths of the $B$-modules $\mathrm{Hom}_B(\kappa_B, \Omega_{(B)})$ and $\mathrm{Hom}_B(\kappa_A \otimes_A B, \Omega_{(B)})$ are 1 and $m$, and that of $\mathrm{Hom}_B(N, \Omega_{(B)})$) is $\leqslant m - 1$; one deduces from this that the $B$-module $\mathrm{Ext}_B^1(\kappa_B, \Omega_{(B)})$ is zero. By Prop. 6 of § 3, No. 3, the $B$-module $\Omega_{(B)}$ is injective; consequently it is a dualizing module (No. 1, Example 1).

Let us pass to the general case. Put $C = \kappa_A \otimes_A B$; by hypothesis this is a Gorenstein ring, hence a Macaulay ring ($§ 3, n° 7$, prop. 10). By prop. 1 of No. 1, $A$ is a Macaulay ring, and the $A$-module $\Omega$ is Macaulay. Hence $B$ is a Macaulay ring, and the $B$-module $\Omega_{(B)}$ is Macaulay ($§ 2, n° 7$, cor. 1 of prop. 9). Put $r = \dim(A)$, $s = \dim(C)$. There exists a sequence $(x_1, \ldots, x_r)$ of elements of $\mathfrak{m}_A$ regular for the $A$-modules $A$ and $\Omega$, and a sequence $(y_1, \ldots, y_s)$ of elements of $\mathfrak{m}_B$ regular for the $B$-module $C$; let $x$ denote the ideal of $A$ and $\mathfrak{g}$ the ideal of $B$ generated by them respectively. The sequence $(y_1, \ldots, y_s, \rho(x_1), \ldots, \rho(x_r))$ is regular for the $B$-modules $B$ and $\Omega_{(B)}$ ($§ 1, n° 6$, prop. 11), and the $A$-module $B/\mathfrak{g}$ is flat (*loc. cit.*, prop. 10). Put $A' = A/x$, $B' = B/(xB + \mathfrak{g})$ and let $\rho' : A' \to B'$ denote the homomorphism deduced from $\rho$ by passing to quotients. The rings $A'$ and $B'$ are artinian, the $A'$-module $B'$ is flat, the ring $\kappa_{A'} \otimes_{A'} B'$, which is identified with $C/\mathfrak{g}$, is a Gorenstein ring ($§ 3, n° 7$, example 2) and the $A'$-module $\Omega_{(A')}$ is dualizing (No. 2, prop. 4). By the first part of the proof, the $B'$-module $\Omega_{(B')}$ is dualizing. It then follows from *loc. cit.* that the $B$-module $\Omega_{(B)}$ is dualizing.

#### Corollary {#ac-x-s9-n3-cor-1 .statement}

*Let $A$ be a noetherian ring admitting a dualizing module $\Omega$; let $B$ be a polynomial algebra over $A$ in a finite number of indeterminates. The $B$-module $\Omega_{(B)}$ is dualizing.*

Indeed, for every prime ideal $\mathfrak{p}$ of $A$, the ring $\kappa(\mathfrak{p}) \otimes_A A[X]$ is identified with $\kappa(\mathfrak{p})[X]$, which is regular, hence Gorenstein.

#### Proposition 6 {#ac-x-s9-prop-6 .statement}

*Let $\Lambda$ be a noetherian local ring and $\Omega$ a dualizing $A$-module. Let $B$ be a finite $A$-algebra; suppose that the $A$-module $B$ is Macaulay. The $B$-module $\mathrm{Ext}_A^i(B, \Omega)$ is zero for $i \neq \dim(A) - \dim(B)$ and dualizing for $i = \dim(A) - \dim(B)$.

We have $\dim(B) = \dim_A(B) \leq \dim(\Lambda)$ (VIII, § 2, No. 3, Theorem 1 c)); let $c = \dim(A) - \dim(B)$. We have $\mathrm{Ext}_A^i(B, \Omega) = 0$ for $i \neq c$ since the $A$-module $B$ is Macaulay (No. 1, Corollary to Proposition 3). Let us prove that the $B$-module $\mathrm{Ext}_A^c(B, \Omega)$ is dualizing.

Suppose first that $\dim(B) = 0$. The spectrum $X$ of $B$ is finite and formed of maximal ideals (IV, § 2, No. 5, Proposition 9); the canonical mapping $B \to \prod_{n \in X} B_n$ is an isomorphism (*loc. cit.*, Corollary 1). The $B$-module $\Omega' = \mathrm{Ext}_A^c(B, \Omega)$ is therefore the direct sum of the modules $\mathrm{Ext}_A^c(B_n, \Omega)$; since $\mathrm{Ext}_A^c(B_n, \Omega)$ has support in $\{n\}$, it identifies with $\Omega'_n$. We have $\dim(B_n) = 0$ for every $n$; to prove that the $B$-module $\Omega'$ is dualizing, it is therefore enough to prove that this is so for the $B_n$-module $\mathrm{Ext}_A^c(B_n, \Omega)$ for every $n \in X$, which brings us back to the case where the ring $B$ is *local*. In this case, by Example 6 of § 8, No. 5, the $B$-module $\mathrm{Ext}_A^c(B, \Omega)$ is isomorphic to $\mathrm{Hom}_A(B, I)$, where $I$ is a Matlis $A$-module; it is consequently a Matlis $B$-module (§ 8, No. 6, Corollary to Proposition 5), hence a dualizing $B$-module (No. 1, Example 1).

Now suppose that $\dim(B) > 0$ and reason by induction on $\dim(B)$. We have $\mathrm{prof}_A(B) = \dim_A(B) = \dim(B)$, whence $\mathrm{prof}_A(B) > 0$; on the other hand we have $\mathrm{prof}(A) = \dim(A) > 0$ (No. 1, Proposition 1), and consequently $\mathrm{prof}_A(A \oplus B) > 0$. There therefore exists an element $x$ of $\mathfrak{m}_A$ such that the homotheties $x_A$ and $x_B$ are injective.

Consider the exact sequence of extension modules associated with the exact sequence $0 \to B \xrightarrow{x_B} B \longrightarrow B/xB \to 0$ and with the $A$-module $\Omega$. The $A$-module $B/xB$ is Macaulay ($§ 2$, No. 1, Example 3), of dimension $\dim(B) - 1$ (VIII, $§ 3$, No. 2, Proposition 3) ; we therefore have $\mathrm{Ext}_A^i(B/xB, \Omega) = 0$ for $i \neq c + 1$ (No. 1, Corollary to Proposition 3). Since we have $\mathrm{Ext}_A^i(B, \Omega) = 0$ for $i \neq c$, we obtain an exact sequence of $B$-modules

$$
0 \to \mathrm{Ext}_A^c(B, \Omega) \xrightarrow{x} \mathrm{Ext}_A^c(B, \Omega) \longrightarrow \mathrm{Ext}_A^{c+1}(B/xB, \Omega) \to 0 .
$$

By the induction hypothesis, the $B/xB$-module $\mathrm{Ext}_A^{c+1}(B/xB, \Omega)$ is dualizing. Since the $A$-algebra $B$ is finite, the image of $m_A$ in $B$ is contained in the radical of $B$ (V, $§ 2$, No. 1, Proposition 1) ; by Proposition 4 of No. 2, the $B$-module $\mathrm{Ext}_A^c(B, \Omega)$ is dualizing.

#### Corollary 1 {#ac-x-s9-prop-6-cor-1 .statement}

*Let A be a noetherian ring, $\Omega$ a dualizing A-module, and B a finite A-algebra; suppose that the A-module B is Macaulay. The B-module $\mathrm{Ext}_A(B, \Omega)$ is dualizing.*

Let $\Omega'$ denote the $B$-module $\mathrm{Ext}_A(B, \Omega)$. Let $n$ be a maximal ideal of $B$; its inverse image in $A$ is a maximal ideal $m$ (V, $§ 2$, No. 1, prop. 1). The $A_m$-algebra $B_m = A_m \otimes_A B$ is finite, and is a Macaulay $A_m$-module; by the proposition, the $B_m$-module $\Omega'_m$, which identifies with $\mathrm{Ext}_{A_m}(B_m, \Omega_m)$ ($§ 3$, No. 2, prop. 2), is dualizing. Since $B_n$ is a ring of fractions of $B_m$, the $B_n$-module $\Omega'_n$ is dualizing, whence the corollary.

#### Remark {#ac-x-s9-n3-rem-1 .statement}

Let us retain the assumptions of cor. 1 and suppose further that the canonical homomorphism $\rho : A \to B$ is injective. Then one has $\dim(A_m) = \dim(B_m)$ for every maximal ideal $m$ of $A$ (VIII, $§ 2$, No. 3, th. 1 a)). By prop. 6 and cor. 1, $\mathrm{Ext}_A^i(B, \Omega)$ is zero for $i \neq 0$, and the $B$-module $\mathrm{Hom}_A(B, \Omega)$ is dualizing.

#### Corollary 2 {#ac-x-s9-prop-6-cor-2 .statement}

*If a noetherian ring $A$ has a dualizing module, every finitely generated $A$-algebra which is a Macaulay ring has a dualizing module.*

This results from cor. 1 and the cor. of prop. 5.

#### Corollary 3 {#ac-x-s9-prop-6-cor-3 .statement}

*Every presentable Macaulay ring (in particular, every complete local Macaulay ring) has a dualizing module.*

For let indeed $R$ be a regular ring and $A$ a Macaulay ring quotient of $R$. The $R$-module $A$ is a Macaulay module ($§ 2$, No. 5, example 5), and $R$ has a dualizing module (No. 1, example 2); hence the same is true of $A$ by cor. 1. Moreover, it has already been observed that a complete local noetherian ring is presentable ($§ 4$, No. 4, prop. 6, c)).

More generally, every Macaulay ring quotient of a Gorenstein ring has a dualizing module. Conversely, one can prove that a local Macaulay ring which has a dualizing module is a quotient of a Gorenstein local ring (exercise 1).

### 4. Structure of Dualizing Modules

#### Lemma 2 {#ac-x-s9-lem-2 .statement}

Let $A$ be a noetherian ring, $M$ and $N$ finitely generated $A$-modules, $u : M \to N$ a homomorphism. Let $x$ be an element of the radical of $A$, such that the homothety $x_N$ is injective. If the homomorphism $\overline{u} : M/xM \to N/xN$ induced by $u$ is injective (resp. surjective, resp. bijective), the same is true of $u$.

The assertion concerning the surjectivity of $u$ results from Nakayama's lemma (II, § 3, No. 2, cor. 1 of prop. 4), without any assumption on $x_N$. Consider the commutative diagram with exact rows

$$
\begin{array}{ccccccc}
M & \xrightarrow{x_M} & M & \longrightarrow & M/xM \\
\downarrow u & & \downarrow u & & \downarrow \overline{u} \\
0 & \longrightarrow & N & \xrightarrow{x_N} & N & \longrightarrow & N/xN ;
\end{array}
$$

by means of the snake lemma (I, § 1, No. 4, prop. 2), one deduces from it an exact sequence $\mathrm{Ker}\, u \xrightarrow{x} \mathrm{Ker}\, u \longrightarrow \mathrm{Ker}\, \overline{u}$. If $\overline{u}$ is injective, the homothety with ratio $x$ is surjective in $\mathrm{Ker}\, u$, which implies $\mathrm{Ker}\, u = 0$ by Nakayama's lemma.

#### Proposition 7 {#ac-x-s9-prop-7 .statement}

Let $A$ be a noetherian ring and $\Omega$ a dualizing $A$-module.

a) One has $\mathrm{Ext}_A^i(\Omega, \Omega) = 0$ for $i > 0$.

b) The canonical homomorphism $\gamma : A \to \mathrm{End}_A(\Omega)$ is bijective.

c) Every dualizing $A$-module is of the form $\Omega \otimes_A L$ where $L$ is a projective $A$-module of rank 1.

A) Let us first treat the case where the ring $A$ is local. In this case condition c) means simply that two dualizing modules are isomorphic.

Let $\Omega'$ be a dualizing $A$-module. One has $\mathrm{prof}_A(\Omega') = \dim_A(\Omega') = \dim(A)$ (No. 1, prop. 1), therefore $\mathrm{Ext}_A^i(\Omega', \Omega) = 0$ for $i \neq 0$ (No. 1, prop. 3, c)), whence a).

Let us prove b) and c) by induction on the integer $\dim(A)$ (equal to $\mathrm{prof}(A)$). If it is zero, the ring $A$ is artinian, $\Omega'$ and $\Omega$ are Matlis $A$-modules (No. 1, Example 1); hence they are isomorphic ($\S$ 8, No. 1, Prop. 1) and the canonical mapping $A \to \mathrm{End}_A(\Omega)$ is bijective ($\S$ 8, No. 2, Prop. 3, c)). Suppose $\dim(A) > 0$ and let $x$ be a cancellable element of $\mathfrak{m}_A$. The homothety $x_\Omega$ is injective (No. 2, Prop. 4), and we have an exact sequence

$$
0 \to \Omega \xrightarrow{x_\Omega} \Omega \longrightarrow \Omega/x\Omega \to 0 .
$$

Since $\mathrm{Ext}_A^1(\Omega', \Omega)$ is zero and $\mathrm{Hom}_A(\Omega', \Omega/x\Omega)$ is identified with $\mathrm{Hom}_{A/xA}(\Omega'/x\Omega', \Omega/x\Omega)$, we deduce an exact sequence

$$
(1)\quad 0 \to \mathrm{Hom}_A(\Omega', \Omega) \xrightarrow{x} \mathrm{Hom}_A(\Omega', \Omega) \xrightarrow{p} \mathrm{Hom}_{A/xA}(\Omega'/x\Omega', \Omega/x\Omega) \to 0 ,
$$

where $p$ is the canonical mapping. By Prop. 4, the $A/xA$-modules $\Omega/x\Omega$ and $\Omega'/x\Omega'$ are dualizing, hence isomorphic by the induction hypothesis. Let $\overline{u}$ be an isomorphism of $\Omega'/x\Omega'$ onto $\Omega/x\Omega$. In view of the exact sequence (1), there exists an $A$-homomorphism $u : \Omega' \to \Omega$ such that $p(u) = \overline{u}$; by Lemma 2, $u$ is bijective, which proves c). By the induction hypothesis, the canonical homomorphism $A/xA \longrightarrow \mathrm{End}_{A/xA}(\Omega/x\Omega)$ is bijective. In view of the exact sequence (1), this homomorphism is identified with the homomorphism $\overline{\gamma} : A/xA \longrightarrow \mathrm{End}_A(\Omega)/x\mathrm{End}_A(\Omega)$ induced by $\gamma$; it then follows from Lemma 2 that $\gamma$ is bijective, whence b).

B) Let us pass to the general case. For every maximal ideal $m$ of $A$ and every integer $i > 0$, we have $\mathrm{Ext}^i_{A_m}(\Omega_m, \Omega_m) = 0$ by what precedes, hence $\mathrm{Ext}^i_A(\Omega, \Omega)_m = 0$ ($§ 3$, No. 2, Prop. 2), which implies $\mathrm{Ext}^i_A(\Omega, \Omega) = 0$ (II, $§ 3$, No. 3, Cor. 2 of Th. 1). Analogously, the homomorphism $\gamma_m : A_m \to \mathrm{End}_A(\Omega)_m$ is bijective for every maximal ideal $m$ of $A$, hence $\gamma$ is bijective (*loc. cit.*, Th. 1).

Let us finally prove c). Let $\Omega'$ be a dualizing $A$-module. Denote by $L$ the $A$-module $\mathrm{Hom}_A(\Omega', \Omega)$, and by $v : \Omega' \otimes_A L \to \Omega$ the homomorphism such that $v(x \otimes f) = f(x)$ for $x \in \Omega'$, $f \in L$. Let $m$ be a maximal ideal of $A$. The $A_m$-module $L_m$ is identified with $\mathrm{Hom}_{A_m}(\Omega'_m, \Omega_m)$; by the case already treated it is free of rank one, and every isomorphism $h : \Omega'_m \to \Omega_m$ is a generator of it. When one identifies $L_m$ with $A_m$ by means of the generator $h$, the homomorphism $v_m : \Omega'_m \otimes_{A_m} L_m \to \Omega_m$ is identified with $h$, hence is bijective. Since this holds for every maximal ideal $m$ of $A$, the $A$-module $L$ is projective of rank one (II, $§ 5$, No. 3, Theorem 2), and the homomorphism $v$ is bijective (II, $§ 3$, No. 3, Theorem 1).

#### Corollary 1 {#ac-x-s9-prop-7-cor-1 .statement}

*In order that $A$ be a Gorenstein ring, it is necessary and sufficient that the $A$-module $\Omega$ be projective of rank 1*.

This follows from Example 2 of No. 1 and Proposition 7 c).

#### Corollary 2 {#ac-x-s9-prop-7-cor-2 .statement}

*Suppose that the ring $A$ is presentable. The set of prime ideals $p$ of $A$ such that $A_p$ is a Gorenstein ring is open in $\mathrm{Spec}(A)$*.

Let $p$ be a prime ideal of $A$ such that $A_p$ is a Gorenstein ring. Then it is a Macaulay ring; replacing $A$ if necessary by $A_f$, where $f$ is a suitable element of $A - p$, one is reduced to the case where $A$ is a Macaulay ring ($§ 4$, No. 4, Proposition 7, c)). Let $\Omega$ be a dualizing $A$-module (No. 3, Corollary 3 of Proposition 6). Then $\Omega_p$ is a dualizing module over the Gorenstein ring $A_p$ (No. 1, Proposition 2), hence is free of rank 1 (Corollary 1). It follows that there exists an element $g$ of $A - p$ such that the $A_g$-module $\Omega_g$ is free of rank 1 (II, $§ 5$, No. 1, Corollary of Proposition 2). Thus $A_g$ is a Gorenstein ring (Corollary 1) and the same is true of $A_q$ for every prime ideal $q$ of $A$ not containing $g$ ($§ 3$, No. 7, Example 1), which proves the corollary.

### 5. Duality of modules of finite type

In this number we consider a noetherian ring $A$ *of finite dimension* which possesses a dualizing module $\Omega$. Then $\mathrm{di}_A(\Omega) = \dim(A) < +\infty$ (No. 1, Prop. 1). *Choose an injective resolution of finite length* $e : \Omega \to (I, \delta)$. For every complex $C$ of $A$-modules, let $D(C)$ denote the complex $\mathrm{Homgr}_A(C, I)$. This applies in particular to every $A$-module $M$, regarded as a complex concentrated in degree 0; we then have $D(M)^i = \mathrm{Hom}_A(M, I^i)$ for every integer $i$. Recall that in A, X, p. 100, Theorem 1, we constructed a canonical isomorphism

$$
\varphi(M, I) : H(D(M)) \longrightarrow \mathrm{Ext}_A(M, \Omega)
$$

*Examples.* 1) The complex $D(A) = \mathrm{Homgr}_A(A, 1)$ is identified with $I$. The map $e : \Omega \to D(A)$ is by definition a homologism.

2) The homomorphism $e \in \mathrm{Homgr}_A(\Omega, I)^0$ is an element of $D(\Omega)^0$; the a-linear map $\tilde{e} : A \to D(\Omega)$ such that $\tilde{e}(1) = e$ is a homologism (No. 4, Prop. 7, a) and b)).

3) Let S be a multiplicative subset of A. The $S^{-1}A$-module $S^{-1}\Omega$ is dualizing (No. 1, Cor. 1 of Prop. 2); the $S^{-1}A$-modules $S^{-1}I^i$ are injective (Cor. 1 of Prop. 3 of § 3, No. 2) and the morphism $e' : S^{-1}\Omega \to S^{-1}I$ deduced from $e$ is an injective resolution of $S^{-1}\Omega$, to which one may therefore apply the foregoing. For every complex C of finite type (and in particular every $A$-module M of finite type), the canonical homomorphism from $S^{-1}D(C)$ into $\mathrm{Homgr}_{S^{-1}A}(S^{-1}C, S^{-1}I) = D(S^{-1}C)$ is bijective.

4) Let A be a Dedekind ring, K its field of fractions. The A-module A is dualizing and admits the injective resolution I of length 1 defined by the exact sequence

$$
0 \to A \xrightarrow{e} K \xrightarrow{\delta} K/A \to 0
$$

where $\delta$ is the canonical surjection. For every A-module M, the complex $D(M)$ is the complex concentrated in degrees 0 and 1

$$
\ldots \longrightarrow 0 \longrightarrow \mathrm{Hom}_A(M, K) \xrightarrow{d} \mathrm{Hom}_A(M, K/A) \longrightarrow 0 \longrightarrow \ldots
$$

with $d = \mathrm{Hom}_A(1_M, \delta)$. We have an exact sequence

$$
0 \to \mathrm{Hom}_A(M, A) \longrightarrow D(M)^0 \xrightarrow{d} D(M)^1 \longrightarrow \mathrm{Ext}_A^1(M, A) \to 0 .
$$

For every morphism of complexes $f : C \to C'$, we denote by $D(f) : D(C') \to D(C)$ the morphism of complexes $\mathrm{Homgr}_A(f, 1_I)$. If $f$ is a homologism, $D(f)$ is a homologism (A, X, p. 86, Prop. 4, b)). If $C' \xrightarrow{f} C \xrightarrow{g} C''$ is an exact sequence of complexes, the sequence of complexes $D(C'') \xrightarrow{D(g)} D(C) \xrightarrow{D(f)} D(C')$ is exact (A, X, p. 83, Prop. 2, a)).

Let M be an A-module. To each element $m$ of M, let us associate the map $\alpha_M(m) : f \mapsto f(m)$ from $D(M)$ into I; this is an element of $D(D(M))_0 = \mathrm{Homgr}_A(D(M), I)_0$. It follows from the definitions that $\alpha_M(m)$ is a morphism of complexes, hence an element of $Z_0(D(D(M)))$.

Thus one defines a morphism of complexes:

$$
\alpha_M : M \to D(D(M)),
$$

whence, by passing to homology, a homomorphism of A-modules

$$
\alpha_M : M \to H_0(D(D(M))).
$$

#### Theorem 1 {#ac-x-s9-thm-1 .statement}

**Let $M$ be a finitely generated $A$-module. Then $\alpha_M$ is a homologism: we have $H_i(D(D(M))) = 0$ for $i \neq 0$ and the homomorphism $\alpha_M$ is bijective.**

Let us first take $M = A$. The mapping $e : \Omega \to D(A)$ is a homomorphism (Example 1), hence so also is the mapping $D(e) : D(D(A)) \to D(\Omega)$. The mapping $\tilde{e} : A \to D(\Omega)$ is a homomorphism (Example 2), and we have $D(e) \circ \alpha_A = \tilde{e}$; thus $\alpha_A$ is a homomorphism, which proves the theorem in this case. It follows that $\alpha_M$ is a homomorphism when the $A$-module $M$ is a finitely generated free module.

Let us pass to the general case; we shall prove by induction on the integer $n$ the following assertion:

$(A_n)$ *for every finitely generated $A$-module $M$, the homomorphism $H_i(\alpha_M)$ is bijective for $i \leq n$.*

This also means that $H_i(D(D(M)))$ is zero for $i \neq 0$ and $i \leq n$, and that $\alpha_M$ is bijective if $n \geq 0$. Observe that $(A_n)$ holds for $n < -d$, where $d$ is the length of the complex $I$; in fact the $A$-module $D(D(M))_i$ is equal to $\bigoplus_p \mathrm{Hom}_A(\mathrm{Hom}_A(M, I^p), I^{p-i})$, and is therefore zero for $i < -d$ and $i > d$.

Let us prove the implication $(A_n) \Rightarrow (A_{n+1})$. Let $M$ be a finitely generated $A$-module. There exists a finitely generated free $A$-module $L$ and an exact sequence $0 \to N \xrightarrow{u} L \xrightarrow{v} M \to 0$.

The sequence $0 \to D(M) \xrightarrow{D(v)} D(L) \xrightarrow{D(u)} D(N) \to 0$ is exact; analogously, if we put $u' = D(D(u))$ and $v' = D(D(v))$, the sequence $0 \to D(D(N)) \xrightarrow{u'} D(D(L)) \xrightarrow{v'} D(D(M)) \to 0$ is exact.

Since $H_i(D(D(L)))$ is zero for $i \neq 0$, we have isomorphisms

$$
H_i(D(D(M)))) \longrightarrow H_{i-1}(D(D(N))) \quad \text{for } i \neq 0, 1 ;
$$

this yields the implication $(A_n) \Rightarrow (A_{n+1})$ for $n \neq -1$ and $n \neq 0$. Consider the commutative diagram with exact rows

$$
\begin{array}{ccccccccc}
0 & \to & N & \xrightarrow{u} & L & \xrightarrow{v} & M & \to & 0 \\
& & \downarrow{\alpha_N} & & \downarrow{\alpha_L} & & \downarrow{\alpha_M} & & \\
0 & \to & H_1(D(D(M))) & \longrightarrow & H_0(D(D(N))) & \xrightarrow{H_0(u')} & H_0(D(D(L))) & \xrightarrow{H_0(v')} & H_0(D(D(M))) \longrightarrow H_{-1}(D(D(N)))
\end{array}
$$

where $\alpha_L$ is bijective. If $(A_0)$ holds, the homomorphism $\alpha_N$ is likewise bijective, hence $H_0(u')$ is injective and one obtains $H_1(D(D(M))) = 0$, whence $(A_1)$. If $(A_{-1})$

Thus $(A_n)$ is true for every $n$, which proves the theorem.

Let $M$ be a finitely generated $A$-module; put $c = \dim(A) - \dim_A(M)$. Let $D'(M)$ denote the subcomplex of $D(M)$ equal to $\bigoplus_{i < c} D(M)^i \bigoplus Z^c(D(M))$, and

$$
j : D'(M) \to D(M)
$$

the canonical injection. From the canonical surjection $Z^c(D(M)) \to H^c(D(M))$ and the isomorphism $\varphi(M, I)$ one deduces a morphism of complexes

$$
p : D'(M)(-c) \to \mathrm{Ext}_A^c(M, \Omega)
$$

since $H^i(D(M))$ is zero for $i < c$ (No. 1, prop. 3 a)), $(D'(M)(-c), p)$ is a left resolution of $\mathrm{Ext}_A^c(M, \Omega)$. By A, X, p. 100, th. 1, one has a canonical isomorphism

$$
\varphi^0(D'(M)(-c), I) : H_0(D(D'(M))) \to \mathrm{Ext}_A^c(\mathrm{Ext}_A^c(M, \Omega), \Omega)
$$

by composing it with the homomorphism $H_0(D(j)) : H_0(D(D(M))) \to H_0(D(D'(M)))$

one therefore obtains a homomorphism

$$
H_0(D(D(M))) \to \mathrm{Ext}_A^c(\mathrm{Ext}_A^c(M, \Omega), \Omega),
$$

whence finally, by composition with $\alpha_M$, a canonical homomorphism

$$
\beta_M : M \to \mathrm{Ext}_A^c(\mathrm{Ext}_A^c(M, \Omega), \Omega).
$$

#### Corollary {#ac-x-s9-n5-cor-1 .statement}

If the $A$-module $M$ is Macaulay, the homomorphism $\beta_M$ is bijective.

If $M$ is Macaulay, the $A$-module $H^i(D(M))$ is zero for $i \neq c$ (No. 1, cor. of prop. 3), so that the canonical injection $j : D'(M) \to D(M)$ is a homologism; hence the morphism of complexes $D(j) : D(D(M)) \to D(D'(M))$ is a homologism (A, X, p. 86, prop. 4). Thus $H_0(D(j))$ is bijective; on the other hand $\alpha_M$ is bijective by th. 1, whence the corollary.

When the $A$-module $M$ is of finite length, the $A$-module $\mathrm{Ext}_A^c(M, \Omega)$ identifies with the Matlis dual of $M$ ($cf.$ § 8, No. 5, example 3 and th. 3), and one recovers prop. 4 of § 8, No. 4.

### 6. Example: the case of dimension 1

In this number, one considers an integral noetherian ring $A$ of dimension 1 admitting a dualizing module $\Omega$. Let $K$ denote the field of fractions of $A$, and $V$ the $K$-vector space $K \otimes_A \Omega$.

The canonical homomorphism $\Omega \to V$ is injective, and the K-vector space V is of dimension 1 (No. 2, cor. 1 of prop. 4); let us identify $\Omega$ with a sub-A-module of V.

#### Proposition 8 {#ac-x-s9-prop-8 .statement}

*The A-module $V/\Omega$ is a Matlis module.*

Consider the exact sequence

$$
0 \to \Omega \to V \to V/\Omega \to 0 ;
$$

the A-module V is injective (A, X, p. 18, example 1), and one has $\mathrm{di}_A(\Omega) = 1$ (No. 1, prop. 1). One deduces on the one hand that $V/\Omega$ is injective (§ 3, No. 1, prop. 1), on the other hand that, for every maximal ideal $m$ of A, the $A/m$-vector space $\mathrm{Hom}_A(A/m, V/\Omega)$ is isomorphic to $\mathrm{Ext}_A^1(A/m, \Omega)$, hence of dimension 1. Since $V/\Omega$ is a torsion module, its associated prime ideals are maximal; this proves the proposition (§ 8, No. 4).

Let M be an A-module; in accordance with *loc. cit.*, we shall denote by D(M) the A-module $\mathrm{Hom}_A(M, V/\Omega)$. One can apply the constructions of No. 5 by taking for I the complex

$$
\cdots 0 \to V \xrightarrow{p} V/\Omega \to 0 \cdots
$$

where V is placed in degree 0, and p denotes the canonical surjection. The complex $\mathbf{D}(M)$ is

$$
\cdots 0 \to \mathrm{Hom}_A(M, V) \xrightarrow{p_M} \mathbf{D}(M) \to 0 \cdots ,
$$

with $p_M = \mathrm{Hom}(1_M, p)$. One has a canonical isomorphism of graded A-modules $\varphi(M, I) : \mathrm{H}(\mathbf{D}(M)) \to \mathrm{Ext}_A(M, \Omega)$ (A, X, p. 100, th. 1).

When M is a torsion module, the module $\mathbf{D}(M)^0 = \mathrm{Hom}_A(M, V)$ is zero, and $\varphi(M, I)$ is an isomorphism of $\mathbf{D}(M)$ onto $\mathrm{Ext}_A^1(M, \Omega)$; the morphism $\alpha_M : M \to \mathbf{D}(\mathbf{D}(M))$ is none other than the canonical homomorphism of A-modules

$$
\alpha_M : M \to \mathbf{D}(\mathbf{D}(M))
$$

defined in § 8, No. 3, which is an isomorphism when M is of finite type (that is to say, of finite length). In this case one recovers the situation of *loc. cit*.

Let us return to the general case, and suppose the A-module M to be of finite type. Then $\mathbf{D}(M)$ is a torsion module, hence the A-module $\mathbf{D}(\mathbf{D}(M))^{-1} = \mathrm{Hom}_A(\mathbf{D}(M), V)$ is zero. On the other hand the A-module $\mathrm{Hom}_A(\mathbf{D}(M)^0, V) = \mathrm{Hom}_A(\mathrm{Hom}_A(M, V), V)$ identifies naturally with $K \otimes_A M$, in such a way that the homomorphism

$$
\mathrm{Hom}(1, p) : \mathrm{Hom}_A(\mathrm{Hom}_A(M, V), V) \to \mathbf{D}(\mathrm{Hom}_A(M, V))
$$

identifies with the mapping

$$
j : K \otimes_A M \to \mathbf{D}(\mathrm{Hom}_A(M, V))
$$

such that $j(\lambda \otimes m)(f) = p(\lambda f(m))$ for $\lambda \in K,\ m \in M,\ f \in \mathrm{Hom}_A(M, V)$. Theorem 1 of No. 5 therefore translates into the exactness of the sequence

$$
0 \longrightarrow M \xrightarrow{(i, \alpha_M)} (K \otimes_A M) \oplus D(D(M)) \xrightarrow{(j, -D(p_M))} D(\mathrm{Hom}_A(M, V)) \longrightarrow 0,
$$

where $i$ denotes the canonical mapping of $M$ into $K \otimes_A M$. The kernel of $i$ identifies with the torsion submodule $T(M)$ of $M$, and its cokernel with $(K/A) \otimes_A M$. Consider the commutative diagram with exact rows

$$
\begin{array}{ccccccccc}
0 & \to & T(M) & \longrightarrow & M & \xrightarrow{i} & K \otimes_A M & \longrightarrow & (K/A) \otimes_A M \longrightarrow 0 \\
& & \downarrow{\alpha_M} & & & & \downarrow{j} & & \\
0 & \to & D(\mathrm{Ext}_A^1(M, \Omega)) & \longrightarrow & D(D(M)) & \xrightarrow{D(p_M)} & D(\mathrm{Hom}_A(M, V)) & \longrightarrow & D(\mathrm{Hom}_A(M, \Omega)) \longrightarrow 0
\end{array}
$$

where the second row is obtained by Matlis duality from the exact sequence

$$
0 \to \mathrm{Hom}_A(M, \Omega) \longrightarrow \mathrm{Hom}_A(M, V) \xrightarrow{p_M} \mathrm{Hom}_A(M, V/\Omega) \longrightarrow \mathrm{Ext}_A^1(M, \Omega) \to 0.
$$

Theorem 1 then means that the homomorphisms of $A$-modules

$$
\gamma^0(M) : T(M) \longrightarrow D(\mathrm{Ext}_A^1(M, \Omega)) \quad \text{and} \quad \gamma^1(M) : (K/A) \otimes_A M \longrightarrow D(\mathrm{Hom}_A(M, \Omega))
$$

deduced from $\alpha_M$ and $j$ respectively, are bijective. Since the $A$-module $T(M)$ is of finite length, the $A$-module $\mathrm{Ext}_A^1(M, \Omega)$ is of finite length and identifies with the Matlis dual of $D(T(M))$, and one has $[\mathrm{Ext}_A^1(M, \Omega)] = [T(M)]$ in the group $Z_0(A)$ and $\mathrm{long}_A(\mathrm{Ext}_A^1(M, \Omega)) = \mathrm{long}_A(T(M))$ (§ 8, No. 4, Proposition 4). On the other hand, when one takes $M = A$, one obtains a canonical isomorphism $\gamma^1(A) : K/A \to D(\Omega)$.

Let $B$ be a subring of $K$ containing $A$, finite over $A$. For every maximal ideal $m$ of $A$, one has $\mathrm{prof}_{A_m}(B_m) = \dim_{A_m}(B_m) = 1$ (§ 1, No. 1, Remark 2 and VIII, § 2, No. 3, Theorem 1), so that $B$ is a Macaulay A-module. Consequently the $B$-module $\Omega_B = \mathrm{Hom}_A(B, \Omega)$ is dualizing (No. 3, Remark). The canonical mapping of $\Omega_B = \mathrm{Hom}_A(B, \Omega)$ into $\Omega = \mathrm{Hom}_A(A, \Omega)$ is injective; its image is formed by the elements $\omega$ of $\Omega$ such that the B-submodule $B\omega$ of $V$ is contained in $\Omega$. Thus $\Omega_B$ identifies with the greatest B-submodule of $\Omega$. The $A$-module $B/A$ is of finite length; the exact sequence

$$
0 \to \Omega_B \to \Omega \to \mathrm{Ext}_A^1(B/A, \Omega) \to 0
$$

makes it possible to identify $\Omega/\Omega_B$ with $\mathrm{Ext}_A^1(B/A, \Omega)$, hence from what precedes with $D(B/A)$. In particular, one has $[B/A] = [\Omega/\Omega_B]$ in $Z_0(A)$ and $\mathrm{Ann}_A(B/A) = \mathrm{Ann}_A(\Omega/\Omega_B)$ (§ 8, No. 4, prop. 4).

The ideal $c = \mathrm{Ann}_A(B/A)$ is the transporter $A : B$, that is to say (VII, § 1, No. 1) the set of elements $x$ of $K$ such that $xB \subset A$. It is a (nonzero) ideal of

A and of B; it is in fact the largest ideal of B contained in A. Since $\Omega_B : \Omega \subset \Omega : \Omega = A$ (No. 4, prop. 7, b)), one has $\operatorname{Ann}_A(\Omega/\Omega_B) = \Omega_B : \Omega$, whence finally
$$
c = \operatorname{Ann}_A(B/A) = \operatorname{Ann}_A(\Omega/\Omega_B) = \Omega_B : \Omega .
$$
Since $\Omega_B$ is a B-module, the relation $x \Omega \subset \Omega_B$ is equivalent to $xB\Omega \subset \Omega_B$, so that one also has $c = \Omega_B : B\Omega$.

We shall specialise the preceding discussion to the case where B is the integral closure of A; the assumption that B be a finitely generated A-module is satisfied when the ring A is Japanese (IX, § 4, No. 1, def. 1), which is the case when it is local and complete (*loc. cit.*, No. 2, th. 2), or when it is essentially of finite type over a field (*loc. cit.*, No. 1, remark 2 and example). The ring B is then a Dedekind ring (VII, § 2, No. 2, th. 1), and the torsion-free B-modules $\Omega_B$, $B\Omega$ and $c$ are projective of rank 1 (VII, § 4, No. 10, prop. 22). The relation $c = \Omega_B : B\Omega$ then signifies that the linear mapping $c \otimes_B B\Omega \to \Omega_B$ deduced from the action of K on V is an isomorphism (II, § 5, No. 6, prop. 11). In particular one has $\Omega_B = c(B\Omega) = c\Omega$.

#### Proposition 9 {#ac-x-s9-prop-9 .statement}

*Let B be the integral closure of A, and $c = A : B$. Suppose that B is a finitely generated A-module. One has the inequality $[B/c] \leq 2[B/A]$ in $Z_0(A)$. For there to be equality, it is necessary and sufficient that A be a Gorenstein ring.*

One has $[B/c] = [B/A] + [A/c]$, so that the inequality under consideration is equivalent to $[A/c] \leq [B/A]$.

A) For every maximal ideal $m$ of A, the integral closure of $A_m$ is $B_m$ (V, § 1, No. 5, cor. 1), and one has $c_m = A_m : B_m$. Moreover, by definition, one has $[B/c] = \sum_m \operatorname{long}_{A_m}(B_m/c_m)[m]$ and $[B/A] = \sum_m \operatorname{long}_{A_m}(B_m/A_m)[m]$. This reduces us to proving the proposition when the ring A is *local*, which we shall henceforth assume. In this case the ordered group $Z_0(A)$ identifies canonically with $\mathbf{Z}$, in such a way that the class of a module of finite length is its length. The ring B is semilocal and the B-module $B\Omega$ is free of rank 1 (II, § 5, No. 3, prop. 5).

B) If A is a Gorenstein ring, the A-module $\Omega$ is free of rank 1 (No. 4, cor. 1 of prop. 7); let us choose a generator $\omega$ of $\Omega$. One has $\Omega = A\omega$ and $\Omega_B = c\Omega = c\omega$, and consequently $\operatorname{long}(A/c) = \operatorname{long}(\Omega/\Omega_B) = \operatorname{long}(B/A)$.

C) Suppose the residue field $\kappa_A$ is infinite. For every maximal ideal $n$ of B, let $L(n)$ denote the $B/n$-vector space (of dimension 1) $B\Omega/nB\Omega$, and $\operatorname{pr}_n$ the canonical projection of $\bigoplus_n L(n)$ onto $L(n)$. Let $\varphi : \Omega \longrightarrow \bigoplus_n L(n)$ be the restriction to $\Omega$ of the canonical homomorphism $B\Omega \longrightarrow \bigoplus_n L(n)$. The image of $\varphi$ is a $\kappa_A$-vector subspace of $\bigoplus_n L(n)$; it is not contained in $\operatorname{Ker} \operatorname{pr}_n$, for otherwise one would have $\Omega \subset nB\Omega$ and consequently $B\Omega \subset nB\Omega$, which is contradictory. Thus the image of $\varphi$ is not contained in the union of the $\operatorname{Ker} \operatorname{pr}_n$ (A, V, p. 40, lemma 1); there therefore exists an element $\omega$ of $\Omega$ whose image in $B\Omega/nB\Omega$ is non-zero for every $n$, which implies that $\omega$ generates the B-module $B\Omega$ (II, § 3, No. 3, prop. 11).

Let $a \in A$; if $a\omega$ belong to $\Omega_B$, one has $aB\omega \subset \Omega_B$, hence $a\Omega \subset \Omega_B$, which implies that $a \in c$. The mapping $a \mapsto a\omega$ therefore induces an injection of $A/c$ into $\Omega/\Omega_B$; consequently one has $\operatorname{long}(A/c) \leq \operatorname{long}(\Omega/\Omega_B) = \operatorname{long}(B/A)$.

If $\operatorname{long}(A/c) = \operatorname{long}(B/A)$, one has $A\omega + \Omega_B = \Omega$. One may suppose that the ideal $c$ is contained in $m_A$ (otherwise $A$ is equal to $B$, hence is a Gorenstein ring). Since $\Omega_B = c\Omega$ is contained in $m_A\Omega$, it follows from Nakayama's lemma that $\omega$ generates $\Omega$. Thus the $A$-module $\Omega$ is monogenous, hence free of rank 1, which means that $A$ is a Gorenstein ring (No. 4, cor. 1 of prop. 7).

D) Let us treat the general case. Let us denote by $A'$ the ring $A[X]$, that is to say (IX, App., No. 2) the local ring of the polynomial ring $A[X]$ at the prime ideal $m_A A[X]$; it is a flat, integral $A$-algebra of dimension 1, whose residue field $\kappa_{A'}$ is identified with $\kappa_A(X)$ and whose field of fractions is identified with $K(X)$ (*loc. cit.*). By the corollary to proposition 5 of No. 3, the $A'$-module $A' \otimes_A \Omega$ is dualizing. Put $B' = A' \otimes_A B$; this is the integral closure of $A'$ in $K(X)$ (V, § 1, No. 3, proposition 13 and No. 5, proposition 16). The conductor $c' = A' : B'$ is equal to $cA'$ (I, § 2, No. 10, formula (11)). For every $A$-module $M$ of finite length, one has $\operatorname{long}_{A'}(A' \otimes_A M) = \operatorname{long}_A(M)$: in fact, since the $A$-algebra $A'$ is flat, it is enough to prove this relation when $M$ is simple, that is to say isomorphic to $\kappa_A$; but in this case $A' \otimes_A \kappa_A$ is identified with $\kappa_{A'}$, whence our assertion. Thus one has

$$
\operatorname{long}_A(B/c) = \operatorname{long}_{A'}(B'/c') \quad \text{and} \quad \operatorname{long}_A(B/A) = \operatorname{long}_{A'}(B'/A') .
$$

The ring $A'$ satisfies the hypotheses of the proposition, and its residue field is infinite. By part C) of the proof, one has $\operatorname{long}_{A'}(B'/c') \leq 2 \operatorname{long}_{A'}(B'/A')$, and equality implies that $A'$ is a Gorenstein ring; but this last condition implies that $A$ is a Gorenstein ring (§ 3, No. 8, corollary 1 to proposition 12).

## EXERCISES {#ac-x-s9-exercises}

See the [exercises for § 9](exercises/s9/).
