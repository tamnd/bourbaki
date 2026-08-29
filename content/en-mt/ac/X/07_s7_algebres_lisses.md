---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 7
section_title: Algèbres lisses
lang: en
source: ac-x-fr
book_pages: AC X.170-AC X.173
pdf_pages: 0082-0103, 0169-0172
extraction: ocr
subsections:
    - "no": 1
      title: Dérivations et relèvements d’homomorphismes
      page: 0
      pdf_page: 82
    - "no": 2
      title: Algèbres formellement lisses
      page: 84
      pdf_page: 83
    - "no": 3
      title: Exemples d’algèbres formellement lisses
      page: 87
      pdf_page: 86
    - "no": 4
      title: Relèvements d’homomorphismes dans les algèbres filtrées complètes
      page: 89
      pdf_page: 88
    - "no": 5
      title: Quotients formellement lisses d’algèbres
      page: 90
      pdf_page: 89
    - "no": 6
      title: Extension du corps de base dans les algèbres régulières (caractéristique non nulle)
      page: 0
      pdf_page: 91
    - "no": 7
      title: Un critère pour les algèbres locales formellement lisses
      page: 95
      pdf_page: 94
    - "no": 8
      title: Existence de rétractions pour les applications linéaires
      page: 0
      pdf_page: 96
    - "no": 9
      title: Le critère jacobien
      page: 98
      pdf_page: 97
    - "no": 10
      title: Algèbres lisses
      page: 102
      pdf_page: 101
statements: 39
exercises: 15
content_sha256: aaa34242d598f6821b0738736697b9b060d8724ab44b075a978f529e09bfce6c
translated_from: content/fr/ac/X/07_s7_algebres_lisses.md
source_lang: fr
translation_method: machine
source_content_sha256: d68b9c7325c87d31bf9721e3dce35c4be0ff95e79d61fe0491564111f5babb1e
translation_model: gpt-5.4
translation_run: translate-en-mt-fbad9c28
glossary_version: 34
glossary_terms_sha256: 7ad2e504feccae5814964a4eaf70d43128c4b2c9898079c403de2f942943e150
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 7. SMOOTH ALGEBRAS

### 1. Derivations and liftings of homomorphisms

Let $k$ be a ring, $C$ a $k$-algebra and $N$ an ideal of $C$ of square zero. Let $\pi : C \to C/N$ denote the canonical homomorphism; since $N^2 = \{0\}$, the structure of $C$-module on $N$ arises from a structure of $C/N$-module.

Let $A$ be a $k$-algebra and $\varphi : A \to C/N$ a homomorphism of $k$-algebras. Endow $N$ with the structure of $A$-module deduced from $\varphi$. By a *lifting of $\varphi$* (to $C$) is meant any homomorphism of $k$-algebras $\tilde{\varphi} : A \to C$ such that $\pi \circ \tilde{\varphi} = \varphi$. Let $\tilde{\varphi}$ be such a lifting, and $\delta$ a mapping of $A$ into $N$; let $\delta + \tilde{\varphi}$ denote the mapping $x \mapsto \delta(x) + \tilde{\varphi}(x)$ of $A$ into $C$.

#### Proposition 1 {#ac-x-s7-prop-1 .statement}

*If $\varphi$ admits a lifting, the mapping $(\delta, \tilde{\varphi}) \mapsto \delta + \tilde{\varphi}$ defines a simply transitive operation of the group of $k$-derivations of $A$ into $N$ on the set of liftings of $\varphi$.*

Let $\tilde{\varphi}_0 : A \to C$ be a lifting of $\varphi$. The mapping $\delta \mapsto \delta + \tilde{\varphi}_0$ induces a bijection of the set of mappings of $A$ into $N$ onto the set of mappings $\tilde{\varphi} : A \to C$ such that $\pi \circ \tilde{\varphi} = \varphi$. Fix $\delta$, and put $\tilde{\varphi} = \delta + \tilde{\varphi}_0$. In order that $\tilde{\varphi}$ be a homomorphism of $k$-algebras, it is necessary and sufficient that $\delta$ be a $k$-derivation of $A$ into $N$: indeed, for $x, y$ in $A$ and $\lambda$ in $k$, one has the relations

$$
\begin{align*}
\tilde{\varphi}(x + y) - \tilde{\varphi}(x) - \tilde{\varphi}(y) &= \delta(x + y) - \delta(x) - \delta(y) \\
\tilde{\varphi}(\lambda x) - \lambda \tilde{\varphi}(x) &= \delta(\lambda x) - \lambda \delta(x) \\
\tilde{\varphi}(xy) - \tilde{\varphi}(x)\tilde{\varphi}(y) &= \delta(xy) - \delta(x)\delta(y) - \delta(x)\tilde{\varphi}_0(y) - \tilde{\varphi}_0(x)\delta(y) \\
&= \delta(xy) - \varphi(x)\delta(y) - \varphi(y)\delta(x),
\end{align*}
$$

the last equality resulting from the fact that $N$ is of square zero. The proposition follows from this.

#### Example {#ac-x-s7-n1-exa-1 .statement}

Let $B$ be a $k$-algebra, $N$ a $B$-module. Endow the $k$-module $B \oplus N$ with the structure of a $k$-algebra defined by $(b, x)(b', x') = (bb', bx' + b'x)$ (*cf.* A, III, p. 127), so that $N$ is a square-zero ideal of $B \oplus N$. Let $\varphi : A \to B$ be a homomorphism of $k$-algebras. Then the liftings of $\varphi$ to $B \oplus N$ are the mappings $x \mapsto (\varphi(x), \delta(x))$, where $\delta$ runs through the set of $k$-derivations of $A$ into $N$ (*cf. loc. cit.*, prop. 12).

Let $\Omega_k(A)$ be the module of $k$-differentials of the ring $A$, and let $d : A \longrightarrow \Omega_k(A)$ be the universal $k$-derivation (A, III, p. 133 and 134); let us recall (*loc. cit.*) that for every $A$-module $M$, the mapping $v \mapsto v \circ d$ is an $A$-linear isomorphism of $\mathrm{Hom}_A(\Omega_k(A), M)$ onto the $A$-module of $k$-derivations of $A$ into $M$.

Let J be an ideal of A. By A, III, p. 137, one has an exact sequence of $A/J$-linear mappings

$$
J/J^2 \xrightarrow{\bar{d}} (\Lambda/J) \otimes_A \Omega_k(\Lambda) \longrightarrow \Omega_k(A/J) \to 0,
$$

where $\bar{d}$ is the homomorphism induced by passing to quotients from the restriction of $d$ to J.

Let $\rho : A \to A/J^2$ and $\pi : A/J^2 \to A/J$ denote the canonical surjections. Let $v : (A/J) \otimes_A \Omega_k(A) \longrightarrow J/J^2$ be a $k$-linear mapping; to it one associates a $k$-linear mapping $H_v : A \to A/J^2$ by putting $H_v(x) = \rho(x) - v(1 \otimes dx)$. If $v$ is a retraction of $\bar{d}$, $H_v$ vanishes on J, hence induces by passing to the quotient a $k$-linear mapping $h_v : A/J \to A/J^2$. On the other hand, given a $k$-linear mapping $h : A/J \to A/J^2$, let us denote by $\psi_h : A/J \oplus J/J^2 \longrightarrow A/J^2$ the mapping $(x, y) \mapsto h(x) + y$.

#### Proposition 2 {#ac-x-s7-prop-2 .statement}

Endow the $k$-module $\Lambda/J \oplus J/J^2$ with the structure of a $k$-algebra defined in the above example. The mappings $v \mapsto h_v$ and $h \mapsto \psi_h$ induce bijections between the following sets :

(i) the set of $A/J$-linear retractions $v$ of $\bar{d}$ ;
(ii) the set of homomorphisms of $k$-algebras $h : A/J \to A/J^2$ such that $\pi \circ h = \mathrm{Id}_{A/J}$ ;
(iii) the set of isomorphisms of $k$-algebras $\psi : A/J \oplus J/J^2 \longrightarrow A/J^2$ such that $\pi \circ \psi = \mathrm{pr}_1$ and $\psi(0, z) = z$ for $z \in J/J^2$.

Apply Prop. 1 with $C = A/J^2$ and $N = J/J^2$. Let $\varphi : A \to A/J$ be the canonical surjection ; the homomorphism $\rho$ is a lifting of $\varphi$ to $A/J^2$. The $A$-module $\mathrm{Hom}_{A/J}((A/J) \otimes_A \Omega_k(A), J/J^2)$ is identified with $\mathrm{Hom}_A(\Omega_k(A), J/J^2)$ ; after Prop. 1, the mapping $v \mapsto H_v$ is a bijection of this set onto the set of liftings of $\varphi$ to $A/J^2$. For $x \in J$, one has $1 \otimes dx = \bar{d}(\rho(x))$ ; for $H_v$ to vanish on J, it is necessary and sufficient that $v \circ \bar{d}$ be the identity mapping of $J/J^2$. This proves that the mapping $v \mapsto h_v$ induces a bijection between the first two sets described in the statement.

The mapping $h \mapsto \psi_h$ is a bijection of the set of $k$-linear homomorphisms of $A/J$ into $A/J^2$ onto the set of $k$-linear homomorphisms $\psi : A/J \oplus J/J^2 \longrightarrow A/J^2$ such that $\psi(0, z) = z$ for $z \in J/J^2$ ; moreover, for $\pi \circ \psi_h = \mathrm{pr}_1$ to hold, it is necessary and sufficient that $\pi \circ h = \mathrm{Id}_{A/J}$, that is to say $z \equiv h(\pi(z)) \pmod{J/J^2}$ for every $z \in A/J^2$. Suppose these conditions satisfied. For $h$ to be a ring homomorphism, it is necessary and sufficient that the same be true of $\psi_h$ ; moreover, the homomorphism $\psi_h$ is bijective : the inverse mapping associates to an element $z$ of $A/J^2$ the pair $(\pi(z), z - h(\pi(z)))$. This proves that the mapping $h \mapsto \psi_h$ induces a bijection between the last two sets described in the statement.

### 2. Formally smooth algebras

Let $k$ be a ring and $A$ a linearly topologized $k$-algebra (III, § 4, No. 2, Def. 1).

#### Definition 1 {#ac-x-s7-def-1 .statement}

One says that $A$ is formally smooth over $k$, or is a formally smooth $k$-algebra, if it satisfies the following condition: whatever the $k$-algebra $C$ and the square-zero ideal $N$ of $C$ may be, every continuous homomorphism from $A$ into the $k$-algebra $C/N$, endowed with the discrete topology, can be lifted to a continuous homomorphism from $A$ into the $k$-algebra $C$, endowed with the discrete topology.

Recall that a homomorphism from $A$ into a $k$-algebra endowed with the discrete topology is continuous if and only if its kernel is open.

Let $k$ be a ring, $A$ a $k$-algebra and $J$ an ideal of $A$. Endow $A$ with the $J$-adic topology. Let $C$ be a $k$-algebra, $N$ a square-zero ideal of $C$; endow $C$ and $C/N$ with the discrete topology. Let $\varphi : A \to C/N$ be a continuous homomorphism of algebras. Every lifting $\tilde{\varphi} : A \to C$ of $\varphi$ is continuous: in fact there exists an integer $n$ such that $\varphi(J^n)$ is zero, and one has $\tilde{\varphi}(J^n) \subset N$, whence $\tilde{\varphi}(J^{2n}) \subset N^2 = 0$. It follows in particular that, if $A$ is formally smooth for the $J$-adic topology, it is also formally smooth for the $J'$-adic topology for every ideal $J'$ containing $J$.

We shall say that a $k$-algebra $A$ is formally smooth if it is formally smooth when endowed with the discrete topology, that is to say, the $(0)$-adic topology; it is then formally smooth for the $J$-adic topology whatever the ideal $J$ of $A$ may be.

#### Remark 1 {#ac-x-s7-n2-rem-1 .statement}

Let $k$ be a ring, $A$ a $k$-algebra and $J$ an ideal of $A$. If the $k$-algebra $A/J$ is formally smooth (for the discrete topology), the identity mapping of $A/J$ admits a lifting to $A/J^2$; consequently the sets described in Prop. 2 are non-empty. In particular, the sequence

$$
0 \to J/J^2 \xrightarrow{\bar{d}} (A/J) \otimes_A \Omega_k(A) \longrightarrow \Omega_k(A/J) \to 0
$$

is exact and split.

#### Remark 2 {#ac-x-s7-n2-rem-2 .statement}

Let $k$ be a ring, $A$ a linearly topologized formally smooth $k$-algebra, $M$ an $A$-module whose annihilator is open in $A$. Then every derivation $\delta$ of $k$ into $M$ extends to a derivation of $A$ into $M$. Indeed, put $B = A/Ann(M)$; the mapping $\lambda \mapsto (\lambda 1_B, \delta(\lambda))$ defines a ring homomorphism from $k$ into $B \oplus M$ (No. 1, Example), that is, a $k$-algebra structure on $B \oplus M$. The canonical surjection $\varphi : A \to B$ is continuous, and therefore admits a lifting $\tilde{\varphi} : A \to B \oplus M$; by loc. cit., $pr_2 \circ \tilde{\varphi}$ is a derivation of $A$ into $M$ which extends $\delta$.

#### Proposition 3 {#ac-x-s7-prop-3 .statement}

Let $k$ be a ring.

a) Let $A$ and $B$ be linearly topologized $k$-algebras and $\rho : A \to B$ a continuous homomorphism of $k$-algebras. If $A$ is formally smooth over $k$ and $B$ formally smooth over $A$, then $B$ is formally smooth over $k$.

b) The product $k$-algebra of a finite family of linearly topologized formally smooth $k$-algebras is formally smooth.

c) Let $A$ be a linearly topologized $k$-algebra, and $\hat{A}$ the separated completion algebra of $A$; in order that $A$ be formally smooth over $k$, it is necessary and sufficient that this be so for $\hat{A}$.

Let C be a $k$-algebra, N a square-zero ideal of C, and $\pi : C \to C/N$ the canonical surjection. Equip C and C/N with the discrete topology.

a) Let $\psi : B \to C/N$ be a continuous homomorphism of $k$-algebras. Since A is formally smooth over $k$, there exists a continuous homomorphism of $k$-algebras $\tilde{\varphi} : A \to C$ such that $\pi \circ \tilde{\varphi} = \psi \circ \rho$.

$$
\begin{array}{ccc}
 & & C \\
 & \swarrow_{\tilde{\varphi}} & \\
A \xrightarrow{\rho} B \xrightarrow{\psi} C/N & & \downarrow^{\pi}
\end{array}
$$

Consider C and C/N as A-algebras by means of $\tilde{\varphi}$, so that $\psi$ is a homomorphism of A-algebras; since B is formally smooth over A, there exists a continuous homomorphism of A-algebras $\tilde{\psi} : B \to C$ such that $\pi \circ \tilde{\psi} = \psi$, whence a).

b) It is enough to prove that the product of two formally smooth $k$-algebras $A_1$ and $A_2$ is formally smooth. Let $\varphi : A_1 \times A_2 \to C/N$ be a continuous homomorphism of $k$-algebras. Put $e_1 = \varphi(1,0)$, $e_2 = \varphi(0,1)$, so that $e_1$ and $e_2$ are orthogonal idempotents in C/N. Let $\varphi_1 : A_1 \to (C/N)e_1$ and $\varphi_2 : A_2 \to (C/N)e_2$ denote the mappings defined by $\varphi_1(a_1) = \varphi(a_1,0)$ and $\varphi_2(a_2) = \varphi(0,a_2)$; these are continuous homomorphisms of $k$-algebras, and one has $\varphi(a_1, a_2) = \varphi_1(a_1) + \varphi_2(a_2)$ for every $(a_1, a_2) \in A_1 \times A_2$. There exists an idempotent element $\tilde{e}_1$ of C such that $\pi(\tilde{e}_1) = e_1$ (A, VIII, § 9, No. 4, Prop. 7); put $\tilde{e}_2 = 1 - \tilde{e}_1$, so that $\pi(\tilde{e}_2) = e_2$. For $i = 1, 2$, the homomorphism $C\tilde{e}_i \to (C/N)e_i$ induced by $\pi$ is surjective, with kernel $N\tilde{e}_i$; since the $k$-algebra $A_i$ is formally smooth, the homomorphism $\varphi_i$ admits a continuous lifting $\tilde{\varphi}_i$ to $C\tilde{e}_i$. The mapping $(a_1, a_2) \mapsto \tilde{\varphi}_1(a_1) + \tilde{\varphi}_2(a_2)$ is a continuous lifting of $\varphi$ to C.

c) Let $i : A \to \widehat{A}$ denote the canonical homomorphism. For every ring D, endowed with the discrete topology, the mapping which associates to a continuous homomorphism $f : \widehat{A} \to D$ the continuous homomorphism $f \circ i : A \to D$ is bijective. Assertion c) follows from this.

Assertion c) of the proposition applies in particular when the topology of $\Lambda$ is the J-adic topology, where J is an ideal of finite type; the closure $\widehat{J}$ of J in $\widehat{A}$ is then equal to $JA$ and the topology of $\widehat{A}$ is the $\widehat{J}$-adic topology (III, § 2, No. 12, Cor. 2 of Prop. 16). Consequently, it is equivalent to say that A is formally smooth for the J-adic topology or that its separated completion $\widehat{A}$ is formally smooth for the J-adic topology.

#### Proposition 4 {#ac-x-s7-prop-4 .statement}

Let k be a ring, A and B $k$-algebras, J an ideal of A, K an ideal of B.

a) Let S be a multiplicative subset of A and T a subset of k whose image in A is contained in S. If A is formally smooth over k for the J-adic topology, S $^1\Lambda$ is formally smooth over $T^{-1}k$ for the $S^{-1}J$-adic topology.

b) Let $k'$ be a $k$-algebra. If $A$ is formally smooth over $k$ for the $J$-adic topology, the $k'$-algebra $A_{(k')}$ is formally smooth over $k'$ for the $JA_{(k')}$-adic topology.

c) Let $I$ denote the ideal of $A \otimes_k B$ generated by the images of $J \otimes_k B$ and $A \otimes_k K$. If $A$ and $B$ are formally smooth over $k$ for the $J$-adic and $K$-adic topologies respectively, the $k$-algebra $A \otimes_k B$ is formally smooth for the $I$-adic topology.

a) Under the hypotheses of a), let $C$ be a $T^{-1}k$-algebra, and $N$ an ideal of square zero of $C$; equip $C$ and $C/N$ with the discrete topology, and let $\pi : C \to C/N$ denote the canonical surjection. Let $\varphi : S^{-1}A \longrightarrow C/N$ be a homomorphism of $T^{-1}k$-algebras, continuous for the $S^{-1}J$-adic topology. Let $i$ denote the canonical homomorphism of $A$ into $S^{-1}A$. The mapping $\varphi \circ i$ is a homomorphism of $k$-algebras, continuous for the $J$-adic topology, and therefore admits a lifting $\tilde{\varphi}_0 : A \to C$. The elements of $\tilde{\varphi}_0(S)$ are invertible modulo $N$, hence invertible since $N$ is square zero. It follows that there exists a ring homomorphism $\tilde{\varphi} : S^{-1}A \to C$ such that $\tilde{\varphi} \circ i = \tilde{\varphi}_0$ (II, § 2, No. 1, Proposition 1); by Corollary 3 to Proposition 2 of loc. cit., $\tilde{\varphi}$ is $T^{-1}k$-linear. We have $\pi \circ \tilde{\varphi} \circ i = \varphi \circ i$, whence $\pi \circ \tilde{\varphi} = \varphi$ (loc. cit., Proposition 1), so that $\tilde{\varphi}$ is a lifting of $\varphi$.

b) Let us place ourselves under the hypotheses of b). Let $C$ be a $k'$-algebra, $N$ a square-zero ideal of $C$; let us endow $C$ and $C/N$ with the discrete topology. Let $\varphi : A_{(k')} \longrightarrow C/N$ be a homomorphism of $k'$-algebras, continuous for the $JA_{(k')}$-adic topology. Let $i : A \to A_{(k')}$ denote the canonical homomorphism. The mapping $\varphi \circ i$ is a homomorphism of $k$-algebras from $A$ into $C/N$, continuous for the $J$-adic topology; if $A$ is formally smooth over $k$ for the $J$-adic topology, $\varphi \circ i$ admits a lifting $\tilde{\psi} : A \to C$. The homomorphism of $k'$-algebras $\tilde{\varphi} : A_{(k')} \longrightarrow C$ deduced from $\tilde{\psi}$ is a lifting of $\varphi$.

c) Let us place ourselves under the hypotheses of c). The $B$-algebra $A \otimes_k B$ is formally smooth for the $J(A \otimes_k B)$-adic topology by b), hence for the $I$-adic topology; moreover the canonical homomorphism $B \to A \otimes_k B$ is continuous when $B$ is endowed with the $K$-adic topology and $A \otimes_k B$ with the $I$-adic topology. The assertion c) therefore results from prop. 3, a).

### 3. Examples of formally smooth algebras

Let $k$ be a ring.

1) Let $P$ be a projective $k$-module. The symmetric $k$-algebra $S_k(P)$ is formally smooth for the discrete topology, and $a fortiori$ for that defined by its grading. In fact, for every $k$-algebra $C$ and every ideal $N$ of $C$, the homomorphisms of algebras from $S_k(P)$ into $C$ (resp. $C/N$) are in bijective correspondence with the $k$-linear mappings from $P$ into $C$ (resp. $C/N$), and the canonical mapping $\mathrm{Hom}_k(P, C) \to \mathrm{Hom}_k(P, C/N)$ is surjective.

Consequently (prop. 3, c)), the $k$-algebra $\hat{S}_k(P) = \prod_{n \geq 0} S_k^n(P)$ is formally smooth (for the product topology of the discrete topologies on the $S_k^n(P)$): in fact it is the completion of the $k$-algebra $S_k(P)$ for the topology defined by the grading.

2) For every family of indeterminates $\mathbf{T} = (T_i)_{i \in I}$, the polynomial $k$-algebra $k[\mathbf{T}]$, and the formal power series $k$-algebra $k[[\mathbf{T}]]$ endowed with its canonical topology, are formally smooth; this follows from example 1. If $k$ is a field, the purely transcendental extension $k(\mathbf{T})$ is formally smooth (No. 2, Prop. 4 a)).

3) Let $f \in k[T]$ be a polynomial in one indeterminate. To say that the $k$-algebra $k[T]/(f)$ is formally smooth is to say that the following property is satisfied: *for every $k$-algebra $C$ and every square-zero ideal $N$ of $C$, every root of $f$ in $C/N$ can be lifted to a root of $f$ in $C$*. This is so when $f$ and its derivative $f'$ generate the unit ideal. In fact, let $\alpha$ be a root of $f$ in $C/N$ and let $a$ be an element of $C$ lifting $\alpha$. Then $f(a)$ belongs to $N$ and consequently $f'(a)$ is invertible in $C$; the element $b = a - f'(a)^{-1} f(a)$ lifts $\alpha$. Since $f'(a)^{-1} f(a)$ is square zero, one has

$$
f(b) = f(a) - f'(a) f'(a)^{-1} f(a) = 0 .
$$

**Theorem 1** (I. S. Cohen). *Let $k$ be a field and $K$ a separable extension of $k$. Then $K$ is a formally smooth $k$-algebra.*

Let $C$ be a $k$-algebra, $N$ a square-zero ideal of $C$, $\pi : C \to C/N$ the canonical homomorphism and $\varphi : K \to C/N$ a homomorphism of $k$-algebras. We have to construct a lifting of $\varphi$. Let us distinguish two cases.

A) Suppose first that $k$ is of characteristic 0. Consider the pairs $(K', \tilde{\varphi}')$, where $K'$ is a subextension of $K$ and $\tilde{\varphi}' : K' \to C$ a lifting of the restriction of $\varphi$ to $K'$. The set of these pairs, endowed with the order defined by the extension relation, is inductive; by Zorn's theorem (E, III, p. 20, th. 2), there exists a maximal pair $(K', \tilde{\varphi}')$. Let us prove that $K'$ is equal to $K$. Let $x \in K - K'$. If $x$ is transcendental over $K'$, the $K'$-algebra $K'(x)$ is formally smooth (example 2). If $x$ is algebraic over $K'$, its minimal polynomial $f \in K'[T]$ is relatively prime to its derivative (A, V, p. 37, prop. 4), and $K'(x)$ is identified with the $K'$-algebra $K'[T]/(f)$, hence is a formally smooth $K'$-algebra (example 3). In both cases, $K'(x)$ is formally smooth over $K'$, and there exists an extension of $\tilde{\varphi}'$ to $K'(x)$ which lifts the restriction of $\varphi$ to $K'(x)$, which contradicts the maximal character of $(K', \tilde{\varphi}')$.

B) Suppose that $k$ is of characteristic $p \neq 0$. Consider the ring homomorphism $F : C \to C$ such that $F(x) = x^p$; one has $F(x) = 0$ for $x \in N$, so that there exists a unique ring homomorphism $\lambda : C/N \to C$ such that $\lambda \circ \pi = F$. One has $\pi(\lambda(\pi(x))) = \pi(x^p) = \pi(x)^p$; since $\pi$ is surjective, one has therefore $\pi(\lambda(z)) = z^p$ for every element $z$ of $C/N$. Moreover, let $f : K \to K^p$ denote the isomorphism $y \mapsto y^p$ and $f^{-1} : K^p \to K$ the reciprocal isomorphism. Let $g : K^p \to C$ be the composite of the sequence of ring homomorphisms

$$
\begin{array}{ccccccccc}
K^p & \xrightarrow{f^{-1}} & K & \xrightarrow{\varphi} & C/N & \xrightarrow{\lambda} & C .
\end{array}
$$

For every $x \in K$, we have $g(x^p) = \lambda(\varphi(x))$. Since $\lambda(\alpha z) = \alpha^p \lambda(z)$ for $\alpha \in k$ and $z \in C/N$, the mapping $g$ is $k^p$-linear. Since the extension $K$ of $k$ is separable, $k(K^p)$ is identified with $k \otimes_{k^p} K^p$ (A, V, p. 119, remark); consequently there exists a unique homomorphism of $k$-algebras $h : k(K^p) \to C$ which coincides with $g$ on $K^p$.

Let $(a_i)_{i \in I}$ be a $p$-basis of $K$ over $k(K^p)$ (A, V, p. 98, theorem 2); for every $i \in I$, choose an element $b_i$ of $C$ such that $\pi(b_i) = \varphi(a_i)$. We have $h(a_i^p) = g(a_i^p) = \lambda(\varphi(a_i)) = \lambda(\pi(b_i)) = b_i^p$ for every $i \in I$. By A, V, p. 94, remark, there exists a homomorphism of $k$-algebras $\tilde{\varphi} : K \to C$, extending $h$ and such that $\tilde{\varphi}(a_i) = b_i$ for every $i$. We have $\pi(\tilde{\varphi}(a_i)) = \pi(b_i) = \varphi(a_i)$ for every $i$ and $\pi(\tilde{\varphi}(x^p)) = \pi(h(x^p)) = \pi(g(x^p)) = \pi(\lambda(\varphi(x))) = \varphi(x^p)$ for every $x \in K$. Hence $\pi \circ \tilde{\varphi} = \varphi$, which completes the proof.

#### Corollary {#ac-x-s7-n3-cor-1 .statement}

Let $k$ be a field, $K$ a separable extension of $k$ and $A$ a linearly topologized $K$-algebra. If $A$ is formally smooth over $K$, it is formally smooth over $k$.

This follows from the theorem and prop. 3 a) of No. 2.

#### Remark 1 {#ac-x-s7-n3-rem-1 .statement}

Let $k$ be a field. Every étale $k$-algebra (A, V, p. 28, def. 1) is formally smooth (*loc. cit.*, p. 34, th. 4, d) and No. 2, prop. 3, b)).

#### Remark 2 {#ac-x-s7-n3-rem-2 .statement}

We shall see below (cor. 2 of th. 2 of No. 5) that a field extension which is formally smooth is absolutely regular, hence separable (§ 6, No. 4, example 2).

### 4. Liftings of homomorphisms in complete filtered algebras

Let $k$ be a ring, $C$ a $k$-algebra, $(C_n)_{n \in \mathbf{Z}}$ a decreasing filtration of $C$, compatible with the structure of $k$-algebra and such that $C_0 = C$ (III, § 2, No. 1). Suppose that $C$ is separated and complete for the topology defined by this filtration, so that the canonical mapping $C \to \varprojlim C/C_n$ is a homeomorphism (*loc. cit.*, No. 6). Let $m$ be an integer $> 0$; denote by $\pi : C \to C/C_m$ the canonical surjection.

#### Proposition 5 {#ac-x-s7-prop-5 .statement}

Let $A$ be a formally smooth linearly topologized $k$-algebra. Every continuous homomorphism of $k$-algebras $\varphi : \Lambda \to C/C_m$ admits a continuous lifting to $C$.

For every integer $n > m$, let us denote by $\pi_n : C/C_n \to C/C_{n-1}$ the canonical surjection. Since $C$ is identified with the projective limit of the $C/C_n$, to give a continuous lifting of $\varphi$ to $C$ amounts to the same as giving a family $(\varphi_n)_{n > m}$ of continuous homomorphisms of $k$-algebras $\varphi_n : A \to C/C_n$, satisfying $\pi_n \circ \varphi_n = \varphi_{n-1}$. This reduces us, by induction on $m$, to proving the statement when $C_{m+1} = 0$. The ideal $C_m$ is then square zero (for $2m \geq m+1$), whence the proposition since $A$ is formally smooth.

#### Example {#ac-x-s7-n4-exa-1 .statement}

Let $C$ be a $k$-algebra and $N$ a nilpotent two-sided ideal of $C$. The proposition applies to the algebra $C$ endowed with the $N$-adic filtration. If $A$ is a formally smooth linearly topologized $k$-algebra, one obtains that every continuous homomorphism of $A$ into the $k$-algebra $C/N$, endowed with the discrete topology, lifts to a continuous homomorphism of $A$ into the $k$-algebra $C$, endowed with the discrete topology.

### 5. Formally smooth quotients of algebras

#### Theorem 2 {#ac-x-s7-thm-2 .statement}

Let k be a ring, A a k-algebra, and J an ideal of A such that the k-algebra A/J is formally smooth. Endow A with the J-adic topology. The following conditions are equivalent:

(i) the topological k-algebra A is formally smooth;
(ii) the $\Lambda/J$-module $J/J^2$ is projective and the canonical homomorphism ($\S$ 5, n° 2)
$$
\beta : S_{A/J}(J/J^2) \to \mathrm{gr}_J(A)
$$
is bijective;
(iii) the $A/J$-module $J/J^2$ is projective and there exists an isomorphism of topological k-algebras of the separated completion of A onto the completed algebra of the graded algebra $S_{A/J}(J/J^2)$.

If A is noetherian, these conditions are also equivalent to:

(iv) the ideal J is completely secant.

Let us first observe that (iii) implies (i): indeed, under the hypotheses of (iii), the algebra $S_{A/J}(J/J^2)$, endowed with the topology associated with its graduation, is formally smooth over $A/J$ (No. 3, example 1), hence over k (No. 2, prop. 3, a)); assertion (i) then follows from prop. 3, c) of No. 2.

Let $\hat{A}$ denote the separated completion of the algebra A and $\hat{J}$ the separated completion of J. The canonical homomorphism $i : A \to \hat{A}$ induces an isomorphism $A/J \to \hat{A}/\hat{J}$ (III, § 2, No. 12, formula (21)). Let $\varphi : A/J \to \hat{A}$ be a lifting of this isomorphism (No. 4, Prop. 5). Let $\lambda : \hat{J} \to J/J^2$ denote the surjection deduced from the canonical isomorphism $J/J^2 \to \hat{J}/\hat{J}^2$ (III, § 2, No. 12, formula (21)). Let $a$ be an element of A, $\bar{a}$ its class in $A/J$, and $z$ an element of $\hat{J}$; one has $\varphi(\bar{a}) \equiv i(a) \pmod{\hat{J}}$, whence $\varphi(\bar{a})z \equiv i(a)z \pmod{\hat{J}^2}$ and $\lambda(\varphi(\bar{a})z) = \lambda(i(a)z) = \bar{a}\lambda(z)$. In other words, $\lambda$ is A/J-linear when $\hat{J}$ is endowed with the structure of an A/J-module deduced from $\varphi$.

Suppose that the homomorphism $\lambda$ admits an A/J-linear section $\sigma : J/J^2 \to \hat{J}$. Let S denote the graded k-algebra $S_{A/J}(J/J^2)$ and $\hat{S}$ its completion. Let
$$
\theta : S \to \hat{A}
$$
be the homomorphism of k-algebras such that $\theta(x) = \varphi(x)$ for $x$ in $S^0 = A/J$, and $\theta(x) = \sigma(x)$ for $x$ in $S^1 = J/J^2$. Since $\theta$ maps $S^1$ into $\hat{J}$, it maps $S^n$ into $\hat{J}^n$ and therefore extends to a continuous homomorphism $\hat{\theta} : \hat{S} \to \hat{A}$. The mapping $\mathrm{gr}_1(\theta) : J/J^2 \to \hat{J}/\hat{J}^2$ is the composite of $\sigma$ with the canonical surjection $\hat{J} \to \hat{J}/\hat{J}^2$; since $\sigma$ is a section of $\lambda$, $\mathrm{gr}_1(\theta)$ coincides with the canonical isomorphism of $J/J^2$ onto $\hat{J}/\hat{J}^2$. It follows that $\mathrm{gr}(\theta) : S \to \mathrm{gr}_{\hat{J}}(\hat{A})$ is the composite of the canonical surjection $\beta$ with the canonical isomorphism $\mathrm{gr}_J(A) \to \mathrm{gr}_{\hat{J}}(\hat{A})$ (III, § 2, No. 12, formula (22)).

Let us now prove the implication (ii) $\Rightarrow$ (iii). Under assumption (ii), the A/J-module $J/J^2$ is projective, and therefore $\lambda$ admits an A/J-linear section; the homomorphism $\hat{\theta} : \hat{S} \to \hat{A}$ associated with this section by the preceding construction induces by

Let us prove (i) ⇒ (ii). Suppose that the topological k-algebra A is formally smooth. Let us first prove that the A/J-module J/J^2 is projective. Let M be a Λ/J-module and $f : M \to J/J^2$ a surjective A/J-linear mapping; the question is to prove that f admits a Λ/J-linear section.

Let π denote the canonical surjection $A/J^2 \to A/J$. By Remark 1 of No. 2, there exists an isomorphism of k-algebras ψ : A/J ⊕ J/J^2 → A/J^2 such that π(ψ(y, z)) = y and ψ(0, z) = z for $y \in A/J$, $z \in J/J^2$. Consider the k-algebra (A/J) ⊕ M (No. 1, Example) and the mapping u : (A/J) ⊕ M → A/J^2 such that u(x, m) = ψ(x, f(m)). This is a surjective homomorphism of k-algebras, whose kernel is the submodule Ker f of M, and therefore is square zero. The canonical surjection ρ : A → A/J^2 is continuous; since the topological k-algebra A is formally smooth, there exists a homomorphism of k-algebras ŝ : A → (A/J)⊕M such that u◦ŝ = ρ. Since pr_1 = π◦ψ = π◦u, one has pr_1◦ŝ = π◦u◦ŝ = π◦ρ, so that pr_1◦ŝ is the canonical surjection of A onto A/J. Hence one has ŝ(J) ⊂ M and consequently ŝ(J^2) = 0, so that ŝ induces an A/J-linear mapping s : J/J^2 → M. One has u◦ŝ = ρ and pr_2◦ψ^{-1}◦u(y, m) = f(m) for $y \in A/J$ and $m \in M$. Let $x \in J$, and ū its class in J/J^2; one has f(s(ū)) = f(pr_2(ŝ(x))) = pr_2(ψ^{-1}(ū)) = ū. Thus s is a section of f.

It remains to prove that the homomorphism β is injective. Since the A/J-module J/J^2 is projective, λ admits an A/J-linear section; let θ : S → Ā denote the associated homomorphism. The homomorphism gr(θ) is identified with β. Let m be an integer; let Σ_m denote the graded k-algebra quotient of S by the ideal $\sum_{i>m} S^i$ and $\theta_m : \Sigma_m \to A/J^{m+1}$ the homomorphism deduced from θ. The composite of θ_m with the canonical surjection A/J^{m+1} → A/J is the canonical projection of Σ_m onto S^0 = A/J; hence the kernel of θ_m is a nilpotent two-sided ideal. By the example of No. 4, there exists a lifting ψ_m : A → Σ_m of the canonical surjection A → A/J^{m+1}. Since the composite of ψ_m with the canonical projection of Σ_m onto A/J is the canonical surjection, ψ_m(J) consists of elements of degree > 0. By passing to associated graded algebras, one deduces from ψ_m a graded k-linear mapping gr(ψ_m) : gr_J(A) → Σ_m such that gr_m(θ)◦gr_m(ψ_m) = Id_{J^m/J^{m+1}}. It follows that gr_m(θ), hence also β_m, is injective, which completes the proof of (ii).

Finally, when A is noetherian, conditions (ii) and (iv) are equivalent (§ 5, No. 2, Th. 1).

#### Corollary 1 {#ac-x-s7-thm-2-cor-1 .statement}

Let k be a field and A a noetherian local k-algebra such that the extension κ_A of k is separable. The following conditions are equivalent:

(i) the k-algebra A is formally smooth for the $m_A$-adic topology;
(ii) the ring A is regular;
(iii) the k-algebra Λ is absolutely regular (§ 6, No. 4, Def. 1) ;
(iv) the k-algebra Ā is isomorphic to κ_A[[T_1, ..., T_n]], with n = dim A.

#### Corollary 2 {#ac-x-s7-thm-2-cor-2 .statement}

Let $k$ be a field, $A$ a noetherian $k$-algebra and $J$ an ideal of $A$ contained in the radical of $A$. Suppose that the $k$-algebra $A$ is formally smooth for the $J$-adic topology. Then it is absolutely regular.

Let indeed $k'$ be a finite extension of $k$ and $A'$ the $A$-algebra $A_{(k')}$; it is a question of proving that, for every maximal ideal $m'$ of $A'$, the noetherian local ring $A'_{m'}$ is regular. Now one has $JA' \subset m'$: in fact, the inverse image of $m'$ in $A$ is a maximal ideal of $A$ (V, § 2, No. 1, prop. 1), hence contains $J$. The $k'$-algebra $A'$ is formally smooth for the $JA'$-adic topology (No. 2, prop. 4, b)), and the $k'$-algebra $A'_{m'}$ is formally smooth for the $JA'_{m'}$-adic topology (No. 2, prop. 4, a)), hence also for the $m'A'_{m'}$-adic topology. Let $k_0$ be the prime subfield of $k'$. Then $A'_{m'}$ is formally smooth over $k_0$ for the $m'A'_{m'}$-adic topology (cor. to th. 1 of No. 3); since $\kappa(m')$ is separable over $k_0$, the ring $A'_{m'}$ is regular (cor. 1).

#### Corollary 3 {#ac-x-s7-thm-2-cor-3 .statement}

Let $k$ be a ring and $A$ a formally smooth $k$-algebra.

a) The $A$-module $\Omega_k(A)$ is projective.

b) Suppose that the ring $A \otimes_k A$ is noetherian. Let $\mu : A \otimes_k A \to A$ denote the homomorphism such that $\mu(x \otimes y) = xy$; then the ideal $\mathrm{Ker}(\mu)$ is completely secant.

The $k$-algebras $A$ and $A \otimes_k A$ are formally smooth (No. 2, prop. 4, c)), and $A$ is isomorphic to the quotient of $A \otimes_k A$ by the kernel $I$ of $\mu$. By definition one has $\Omega_k(A) = I/I^2$. Thus a) and b) result from th. 2.

### 6. Extension of the base field in regular algebras (nonzero characteristic)

Let $k$ be a ring and $\rho : A \to B$ a homomorphism of $k$-algebras. From $\rho$ one deduces an $A$-linear mapping $\Omega(\rho) : \Omega_k(A) \to \Omega_k(B)$, and consequently a $B$-linear mapping $\Omega_0(\rho) : B \otimes_A \Omega_k(A) \to \Omega_k(B)$ (A, III, p. 135). Let $T = (T_i)_{i \in I}$ be a family of indeterminates, and $t = (t_i)_{i \in I}$ a family of elements of $B$; for every polynomial $f = \sum_{\alpha \in \mathbf{N}^{(I)}} c_\alpha T^\alpha$ of $A[T]$, let $d^\Lambda f(t)$ denote the element $\sum_\alpha t^\alpha \otimes dc_\alpha$ of $B \otimes_A \Omega_k(A)$.

#### Lemma 1 {#ac-x-s7-lem-1 .statement}

Suppose that the $A$-algebra $B$ admits a generating family $t = (t_i)_{i \in I}$, with defining relations $f_\lambda \in A[T]$ ($\lambda \in \Lambda$). The $B$-linear homomorphism
$$
\psi : (B \otimes_A \Omega_k(A)) \oplus B^{(I)} \longrightarrow \Omega_k(B)
$$
defined by $\psi(\alpha, (b_i)) = \Omega_0(\rho)(\alpha) + \sum_{i \in I} b_i dt_i$, is surjective; its kernel is generated by the elements $r_\lambda = \left( d^\Lambda f_\lambda(t), \left( \frac{\partial f_\lambda}{\partial T_i}(t) \right)_{i \in I} \right)$ for $\lambda \in \Lambda$.

Consider the sequence of B-modules and B-linear mappings

$$
B^{(\Lambda)} \xrightarrow{\varphi} (B \otimes_{\Lambda} \Omega_k(A)) \oplus B^{(1)} \xrightarrow{\psi} \Omega_k(B) \longrightarrow 0,
$$

where $\varphi$ is the homomorphism such that $\varphi(e_\lambda) = n_\lambda$; it is a matter of proving that this sequence is exact. By A, II, p. 36, th. 1, it is enough to prove that, for every B-module M, the sequence

$$
0 \to \mathrm{Hom}_B(\Omega_k(B), M) \xrightarrow{\mathrm{Hom}(\psi, 1)} \mathrm{Hom}_B((B \otimes_A \Omega_k(A)) \oplus B^{(1)}, M) \xrightarrow{\mathrm{Hom}(\varphi, 1)} \mathrm{Hom}_B(B^{(\Lambda)}, M)
$$

is exact. In view of the universal property of the module of differentials (A, III, p. 134), this sequence is identified with

$$
0 \to D_k(B, M) \xrightarrow{\psi'} D_k(A, M) \oplus M^1 \xrightarrow{\varphi'} M^\Lambda
$$

where $\psi'(D) = (D \circ \rho, (D(t_i)))$ and $\varphi'(\Delta, (m_i)) = (f^\Delta_\lambda(t) + \sum_i \frac{\partial f_\lambda}{\partial T_i}(t) m_i)_{\lambda \in \Lambda}$ (in accordance with A, V, p. 121, for every polynomial $f = \sum_{\alpha \in \mathbf{N}^{(1)}} c_\alpha T^\alpha$ of $A[T]$, $f^\Delta(t)$ denotes the element $\sum_\alpha t^\alpha \Delta(c_\alpha)$). But the exactness of this sequence follows from loc. cit., prop. 1, in view of the fact that a derivation $D : B \to M$ is $k$-linear if and only if this is so for $D \circ \rho$.

Let A be a ring. There exists a unique structure of $\mathbf{Z}$-algebra on A; one writes simply $\Omega(\Lambda)$ for the A-module $\Omega_{\mathbf{Z}}(A)$. If $\rho : k \to A$ is a homomorphism of rings, there is a canonical exact sequence of A-modules (A, III, p. 136, prop. 21)

$$
A \otimes_k \Omega(k) \to \Omega(A) \to \Omega_k(A) \to 0.
$$

Suppose that A contains a subfield, and let P be the prime subfield of A; then $\Omega(P)$ is zero and the canonical homomorphism of A-modules $\Omega(A) \to \Omega_P(A)$ is bijective. If moreover A is of characteristic $p \neq 0$ (which means by definition that $p$ is a prime number, that $p1_A = 0$ and $1_A \neq 0$), then P is identified with $\mathbf{F}_p$. Moreover, every derivation of A vanishes on the subring $A^p$; for every subring $k$ of A contained in $A^p$ (and, in particular, for every perfect subfield $k$ of A), the canonical mapping $\Omega(A) \to \Omega_k(A)$ is bijective.

Let A be a ring of characteristic $p \neq 0$ and $(f_i)_{1 \leq i \leq n}$ a finite sequence of elements of A. Let $A_n$ denote the quotient ring of the polynomial ring $A[T_1, \ldots, T_n]$ by the ideal generated by the polynomials $T_i^p - f_i$, for $1 \leq i \leq n$.

#### Lemma 2 {#ac-x-s7-lem-2 .statement}

Suppose the ring A local and noetherian. Then $A_n$ is local and noetherian. The following conditions are equivalent:

(i) $A_n$ is regular;
(ii) A is regular and the elements $1 \otimes df_i$ of the $\kappa_A$-vector space $\kappa_A \otimes_A \Omega(A)$ are linearly independent.

A) Let us first treat the case $n = 1$, setting $T_1 = T$, $f_1 = f$. Let $a$ denote the class of $f$ in $\kappa_A$, and distinguish two cases according as $a$ does or does not belong to $\kappa_A^p$. If $a \notin \kappa_A^p$, then the polynomial $T^p - a$ is irreducible in $\kappa_A$ (A, V, p. 24, lemma 1), and $\kappa_A \otimes_A A_1$ is isomorphic to the field $\kappa_A[T]/(T^p - a)$. The ideal $m_A A_1$ of $A_1$ is therefore maximal, so that the ring $A_1$ is local (V, § 2, No. 1, prop. 1). If $A$ is regular, $A_1$ is regular (VIII, § 5, No. 1, prop. 1). By A, V, p. 99, prop. 6, the element $da$ of $\Omega(\kappa_A)$ is not zero; since it is the image under the canonical mapping $\kappa_A \otimes_A \Omega(A) \to \Omega(\kappa_A)$ of $1 \otimes df$, the latter is not zero. This proves the lemma in this case.

Suppose now that $a$ belongs to $\kappa_A^p$. There therefore exists an element $g$ of $A$ such that $f - g^p \in m_A$. Put $h = f - g^p$. Since $T^p - f = (T - g)^p - h$, the $A$-algebra $A_1$ is isomorphic to $A[T]/(T^p - h)$. By VIII, § 5, No. 4, prop. 4, the ring $A_1$ is local and, in order that it be regular, it is necessary and sufficient that $A$ be regular and that $h$ should not belong to $m_A^2$. Now, since $\kappa_A$ is formally smooth over the prime field (No. 3, th. 1), the canonical mapping

$$
\bar{d} : m_A / m_A^2 \to \kappa_A \otimes_A \Omega(A)
$$

is injective (No. 2, remark 1); but the image under $\bar{d}$ of the class of $h$ modulo $m_A^2$ is equal to $1 \otimes dh = 1 \otimes d(f - g^p) = 1 \otimes df$. This proves the lemma in this second case and completes the proof of the case $n = 1$.

B) Suppose $n > 1$. The ring $A_1$ is local and noetherian by the case already treated. The $A_1$-algebra $A_n$ is identified with the quotient of $A_1[T_2, \ldots, T_n]$ by the ideal generated by the $T_i^p - f_i$, $i \geq 2$; by the induction hypothesis, it is a local ring and condition (i) is equivalent to the conjunction of the following two:

(i') $A_1$ is regular;
(ii') the elements $1 \otimes df_2, \ldots, 1 \otimes df_n$ of the $\kappa_{A_1}$-vector space $\kappa_{A_1} \otimes_{A_1} \Omega(A_1)$ are linearly independent.

But (i') is equivalent, as we have just seen, to
(ii'') $A$ is regular and the element $1 \otimes df_1$ of the $\kappa_A$-vector space $\kappa_A \otimes_A \Omega(A)$ is not zero.

By lemma 1, the canonical homomorphism $A_1 \otimes_A \Omega(A) \to \Omega(A_1)$ induces an isomorphism of $((A_1 \otimes_A \Omega(A))/A_1(1 \otimes df_1)) \oplus A_1$ onto $\Omega(A_1)$, and consequently an injective homomorphism of $(\kappa_{A_1} \otimes_A \Omega(A))/\kappa_{A_1}(1 \otimes df_1)$ into $\kappa_{A_1} \otimes_{A_1} \Omega(A_1)$. Since $\kappa_{A_1} \otimes_A \Omega(A)$ is identified with $\kappa_{A_1} \otimes_{\kappa_A} (\kappa_A \otimes_A \Omega(A))$, assertion (ii'') is therefore equivalent to:
(ii''') the elements $1 \otimes df_2, \ldots, 1 \otimes df_n$ are linearly independent in $(\kappa_A \otimes_A \Omega(A))/\kappa_A(1 \otimes df_1)$.

But the conjunction of (ii') and (ii'') is equivalent to (ii), which proves the lemma.

#### Proposition 6 {#ac-x-s7-prop-6 .statement}

Let $k$ be a field of characteristic $p \neq 0$, $k'$ a purely inseparable extension of $k$, of finite degree and of height $\leqslant 1$, and $A$ a regular local $k$-algebra. Then $A_{(k')}$ is a local ring and the following conditions are equivalent:

(i) the ring $A_{(k')}$ is regular;
(ii) the $\kappa_A$-linear mapping

$$
\kappa_A \otimes_{{k'}^p} \Omega_{{k'}^p}({k'}^p) \longrightarrow \kappa_A \otimes_A \Omega(A)
$$

deduced from the canonical injection ${k'}^p \to A$ is injective.

Let indeed $(x_i)_{i \in I}$ be a finite $p$-base of $k'$ over $k$ (A, V, p. 98); for each $i \in I$, put $f_i = x_i^p \in k$. The $k$-algebra $k'$ is identified with the quotient of $k[(T_i)_{i \in I}]$ by the ideal generated by the polynomials $T_i^p - f_i$, hence the $A$-algebra $A_{(k')}$ with the quotient of $A[(T_i)_{i \in I}]$ by the ideal generated by the polynomials $T_i^p - f_i 1_A$.

Moreover, $(f_i)_{i \in I}$ is a $p$-base of ${k'}^p$ over $k^p$, and the ${k'}^p$-vector space $\Omega_{k^p}({k'}^p)$ has as basis the family of the $df_i$ (A, V, p. 97, th. 1). Proposition 6 then follows from lemma 2.

### 7. A criterion for formally smooth local algebras

#### Proposition 7 {#ac-x-s7-prop-7 .statement}

Let $k_0$ be a ring, $k$ a $k_0$-algebra, $A$ a $k$-algebra, $m$ a maximal ideal of $A$. Suppose that $k$ and $A/m$ are formally smooth over $k_0$. In order that $A$ be formally smooth over $k$ for the $m$-adic topology, it is necessary and sufficient that the following two conditions be satisfied:

(i) the canonical homomorphism $S_{A/m}(m/m^2) \to \mathrm{gr}_m(A)$ is bijective;
(ii) the $A/m$-linear mapping

$$
\omega : A/m \otimes_k \Omega_{k_0}(k) \longrightarrow A/m \otimes_A \Omega_{k_0}(A)
$$

deduced from the canonical mapping $k \to A$ is injective.

Let us denote by $d_k : k \to \Omega_{k_0}(k)$ and $d_A : A \to \Omega_{k_0}(A)$ the universal $k_0$-derivations.

Suppose first that $A$ is formally smooth over $k$ for the $m$-adic topology. Then $A$ is formally smooth over $k_0$ for the $m$-adic topology (No. 2, Prop. 3, a)), which is equivalent to (i) (No. 5, Theorem 2). Moreover, the $k_0$-derivation $\lambda \mapsto 1 \otimes d_k(\lambda)$ of $k$ into $A/m \otimes_k \Omega_{k_0}(k)$ can be extended to a $k_0$-derivation of $A$ into $A/m \otimes_k \Omega_{k_0}(k)$ (No. 2, Remark 2). There therefore exists an $A$-linear mapping $u : \Omega_{k_0}(A) \to A/m \otimes_k \Omega_{k_0}(k)$ such that $u(d_A(\lambda 1_A)) = 1 \otimes d_k(\lambda)$ for every $\lambda \in k$. The $A/m$-linear mapping $A/m \otimes_A \Omega_{k_0}(A) \longrightarrow A/m \otimes_k \Omega_{k_0}(k)$ deduced from $u$ is a retraction of $\omega$, which proves (ii).

Suppose conversely that conditions (i) and (ii) are satisfied. Then $A$ is formally smooth over $k_0$ for the $m$-adic topology (No. 5, Theorem 2) and the $A$-module $\Omega_{k_0}(A)$ is projective (No. 5, Corollary 3 of Theorem 2). Let us fix an integer $r \geqslant 0$ and consider the $A/m^r$-linear mapping

$$
\omega_r : A/m^r \otimes_k \Omega_{k_0}(k) \longrightarrow A/m^r \otimes_A \Omega_{k_0}(A)
$$

deduced from the canonical mapping $k \to A$. Let $(\lambda_i)_{i \in I}$ be a family of elements of $k$ such that the $d_k(\lambda_i)$ form a basis of the vector space $\Omega_{k_0}(k)$ over $k$; by (ii), the elements $1 \otimes d_A(\lambda_i 1_A)$ are linearly independent in $A/\mathfrak{m} \otimes_{\Lambda} \Omega_{k_0}(A)$. By II, § 3, No. 2, Cor. 1 and 2 of Prop. 5, the $1 \otimes d_A(\lambda_i 1_A)$ form a basis of a direct factor of the $A/\mathfrak{m}^r$-module $A/\mathfrak{m}^r \otimes_{\Lambda} \Omega_{k_0}(A)$. There therefore exists an $A/\mathfrak{m}^r$-linear mapping
$$
u_r : A/\mathfrak{m}^r \otimes_{\Lambda} \Omega_{k_0}(A) \longrightarrow A/\mathfrak{m}^r \otimes_k \Omega_{k_0}(k)
$$
such that $u_r(1 \otimes d_A(\lambda_i 1_A)) = 1 \otimes d_k(\lambda_i)$ for all $i$, hence $u_r \circ \omega_r = \mathrm{Id}$.

Let us now verify that $A$ is formally smooth over $k$ for the $\mathfrak{m}$-adic topology. Let $C$ be a $k$-algebra, $N$ a square-zero ideal of $C$, and $\pi : C \to C/N$ the canonical surjection; endow $C$ and $C/N$ with the discrete topology. Let $\varphi : A \to C/N$ be a continuous homomorphism of $k$-algebras. Since $A$ is formally smooth over $k_0$ for the $\mathfrak{m}$-adic topology, there exists a continuous homomorphism of $k_0$-algebras $\tilde{\varphi}_0 : A \to C$ such that $\pi \circ \tilde{\varphi}_0 = \varphi$. By Prop. 1 of No. 1, the homomorphisms of $k_0$-algebras $\tilde{\varphi} : A \to C$ such that $\pi \circ \tilde{\varphi} = \varphi$ are the mappings $x \mapsto v(d_A(x)) + \tilde{\varphi}_0(x)$, where $v$ runs through $\mathrm{Hom}_{\Lambda}(\Omega_{k_0}(A), N)$. It remains to choose $v$ in such a way that $\tilde{\varphi}$ is a homomorphism of $k$-algebras. The mapping $\lambda \mapsto \lambda 1_C - \tilde{\varphi}_0(\lambda 1_A)$ is a $k_0$-derivation of $k$ into $N$ (*loc. cit.*), and therefore can be written $h \circ d_k$ with $h \in \mathrm{Hom}_k(\Omega_{k_0}(k), N)$.

Choose an integer $r$ such that the kernel of $\varphi$ contains $\mathfrak{m}^r$. The $A$-module $N$ is annihilated by $\mathfrak{m}^r$, and it is enough to take for $v$ the composite of the sequence of homomorphisms
$$
\Omega_{k_0}(A) \longrightarrow A/\mathfrak{m}^r \otimes_{\Lambda} \Omega_{k_0}(A) \xrightarrow{u_r} A/\mathfrak{m}^r \otimes_k \Omega_{k_0}(k) \xrightarrow{h'} N ,
$$
where $h'$ is deduced from $h$. In fact, for $\lambda \in k$ one has:
$$
v(d_A(\lambda 1_A)) = h'u_r(1 \otimes d_A(\lambda 1_A)) = h'(1 \otimes d_k(\lambda)) = h(d_k(\lambda)) = \lambda 1_C - \tilde{\varphi}_0(\lambda 1_A) .
$$

#### Remark 1 {#ac-x-s7-n7-rem-1 .statement}

When $A$ is noetherian, condition (i) means that the local ring $A_{\mathfrak{m}}$ is regular (VIII, § 5, No. 2, Theorem 1).

#### Proposition 8 {#ac-x-s7-prop-8 .statement}

*Let $k$ be a field and $A$ a noetherian local $k$-algebra. The following conditions are equivalent*:

(i) *A is formally smooth over $k$ for the $\mathfrak{m}_A$-adic topology* ;
(ii) *A is regular and the $\kappa_A$-linear mapping*
$$
\omega : \kappa_A \otimes_k \Omega(k) \longrightarrow \kappa_A \otimes_{\Lambda} \Omega(A)
$$
*deduced from the canonical injection $k \to A$ is injective* ;
(iii) *A is absolutely regular* ;
(iv) *for every purely inseparable extension $k'$ of $k$, of finite degree and of height $\leqslant 1$, the local ring $A_{(k')}$ is regular*.

(ii) $\Leftrightarrow$ (i): it is enough to apply Prop. 7 and Remark 1 above, taking for $k_0$ the prime subfield of $k$; in fact, $k$ and $\kappa_A$ are formally smooth over $k_0$ (No. 3, Theorem 1).
(i) $\Rightarrow$ (iii): this follows from Corollary 2 of Theorem 2 (No. 5).

If k is of characteristic 0, it follows from Corollary 1 of Theorem 2 (No. 5) that (iv) implies (i), whence the proposition in this case. Suppose k of characteristic $p \neq 0$ and prove (iv) ⇒ (ii). Let $k'$ be a purely inseparable extension of k, of finite degree and of height $\leq 1$. If A and $A_{(k')}$ are regular, the canonical mapping $\kappa_A \otimes_{k'} \Omega_{k^p}({k'}^p) \longrightarrow \kappa_A \otimes_A \Omega(\Lambda)$ is injective (No. 6, Prop. 6). By Theorem 1, b) of A, V, p. 97, applied to the extension k of $k^p$, the k-vector space $\Omega(k)$, which coincides with $\Omega_{k^p}(k)$, is the increasing filtered union of the subspaces $k \otimes_{{k'}^p} \Omega_{k^p}({k'}^p)$, where $k'$ runs through the set of finite purely inseparable extensions of k of height $\leq 1$ contained in a fixed algebraic closure of k. Assertion (ii) follows.

#### Remark 2 {#ac-x-s7-n7-rem-2 .statement}

Let k be a field and A a k-algebra such that the ring $A_{(k')}$ is regular for every purely inseparable extension $k'$ of k, of finite degree and of height $\leq 1$; then A is absolutely regular. In fact, let $k'$ be such an extension; for every maximal ideal m of A, the ring $k' \otimes_k A_m$ is identified with a ring of fractions of $A_{(k')}$, and is therefore regular. By Prop. 8 above and Prop. 6 of § 6, No. 4, the algebra A is absolutely regular.

### 8. Existence of retractions for linear mappings

#### Proposition 9 {#ac-x-s7-prop-9 .statement}

Let A be a ring, M a finitely generated A-module, N a projective A-module, and $u : M \to N$ an A-linear mapping.

a) Let $\mathfrak{p}$ be a prime ideal of A. The following conditions are equivalent :

(i) there exist $f \in A - \mathfrak{p}$ and $v \in \mathrm{Hom}_{A_f}(N_f, M_f)$ with $v \circ u_f = \mathrm{Id}_{M_f}$;
(ii) there exists $v \in \mathrm{Hom}_{A_\mathfrak{p}}(N_\mathfrak{p}, M_\mathfrak{p})$ with $v \circ u_\mathfrak{p} = \mathrm{Id}_{M_\mathfrak{p}}$;
(iii) the $\kappa(\mathfrak{p})\text{-linear } 1 \otimes u : \kappa(\mathfrak{p}) \otimes_A M \to \kappa(\mathfrak{p}) \otimes_A N$ mapping is injective;
(iv) there exist an integer $m \geq 0$, elements $x_1, \ldots, x_m$ of M and linear forms $y_1, \ldots, y_m$ on N such that the images of the $x_i$ in $M_\mathfrak{p}$ generate the $A_\mathfrak{p}$-module $M_\mathfrak{p}$ and that one has $\det(<y_j, u(x_i)>)\notin \mathfrak{p}$;

If condition (iv) is satisfied, one has $m = [\kappa(\mathfrak{p}) \otimes_A M : \kappa(\mathfrak{p})]$ and the elements $1 \otimes x_i$ form a basis of the $\kappa(\mathfrak{p})$-vector space $\kappa(\mathfrak{p}) \otimes_A M$.

b) The set U of prime ideals $\mathfrak{p}$ of A satisfying the conditions of a) is an open set of Spec(A), and the following conditions are equivalent:

(i) one has $U = \mathrm{Spec}(A)$;
(ii) U contains all the maximal ideals of A;
(iii) there exists $v \in \mathrm{Hom}_A(N, M)$ with $v \circ u = \mathrm{Id}_M$;
(iv) u is injective and Coker(u) is a projective A-module.

Let us prove a).

(i) ⇒ (ii) ⇒ (iii): these implications are clear.

(iii) ⇒ (iv): put $m = [\kappa(\mathfrak{p}) \otimes_A M : \kappa(\mathfrak{p})]$ and let $(x_1, \ldots, x_m)$ be a sequence of elements of M such that the elements $1 \otimes x_i$ form a basis of the $\kappa(\mathfrak{p})$-vector space $\kappa(\mathfrak{p}) \otimes_A M$. The images of the $x_i$ in $M_\mathfrak{p}$ generate the $A_\mathfrak{p}$-module $M_\mathfrak{p}$ (Nakayama lemma). If condition (iii) is satisfied, the elements $1 \otimes u(x_i)$ of the $\kappa(\mathfrak{p})$-vector space $\kappa(\mathfrak{p}) \otimes_A N$ are linearly independent.

Moreover, there exist an A-module N', a set I, and an isomorphism of A-modules $\theta : N \oplus N' \to A^{(I)}$, from which one deduces an isomorphism of $\kappa(p)$-vector spaces
$$
\overline{\theta} : (\kappa(p) \otimes_{\Lambda} N) \oplus (\kappa(p) \otimes_A N') \to \kappa(p)^{(I)} .
$$
The elements $t_i = \overline{\theta}(1 \otimes u(x_i), 0)$ of $\kappa(p)^{(I)}$ form a finite free family. There therefore exist elements $\alpha_1, \ldots, \alpha_m$ of I such that one has $\det(\mathrm{pr}_{\alpha_j}(t_i)) \neq 0$; the linear forms $y_j : z \mapsto \mathrm{pr}_{\alpha_j}(\theta(z, 0))$ on N are suitable.

Suppose condition (iv) fulfilled. Let $(a_{ij}) \in M_m(A)$ denote the matrix of coefficients $a_{ij} = <y_j, u(x_i)>$. Let g be an element of $A - p$ such that the images of the $x_i$ generate the $\Lambda_g$-module $M_g$ (II, § 5, No. 1, Prop. 2), and let $f = g \det(a_{ij})$. Since $\det(a_{ij})$ is invertible in $A_f$, the images of the elements $u(x_i)$ in $N_f$ are linearly independent; consequently the images of the $x_i$ in $M_f$ form a basis of this $A_f$-module. This proves the last assertion of a). Let us now prove (i). Let $w \in \mathrm{Hom}_A(N, M)$ denote the mapping $z \mapsto \sum_j <y_j, z> x_j$. We have
$$
w \circ u(x_i) = \sum_j a_{ij} x_j ;
$$
since the images of the $x_i$ form a basis of $M_f$ and the matrix $(a_{ij})$ is invertible in $M_m(A_f)$, the endomorphism $(w \circ u)_f$ of $M_f$ is bijective, and the mapping $v = (w \circ u)_f^{-1} \circ w_f \in \mathrm{Hom}_{A_f}(N_f, M_f)$ satisfies condition (i).

Let us prove b). The fact that U is open follows from condition (i) of a).

(iii) $\Rightarrow$ (i) $\Rightarrow$ (ii): this is clear.

(iv) $\Rightarrow$ (iii): under the hypotheses of (iv), the sequence $0 \to M \xrightarrow{u} N \longrightarrow \mathrm{Coker}(u) \to 0$ is exact and split, whence (iii).

(ii) $\Rightarrow$ (iv): let us introduce, as above, an isomorphism of A-modules $\theta : N \oplus N' \to A^{(I)}$. Let $u'$ denote the mapping of M into $A^{(I)}$ defined by $u'(x) = \theta(u(x), 0)$. There exists a finite subset J of I such that the image of $u'$ is contained in the submodule $A^J$ of $A^{(I)}$. Let $u'' : M \to \Lambda^J$ denote the mapping deduced from $u'$. Under hypothesis (ii), for every maximal ideal m of A, the $A_m$-linear mapping $u'_m$ of $M_m$ into $A_m^{(I)}$ admits a retraction, and therefore the same is true of $u''_m$; thus $u''_m$ is injective and its image is a direct factor in $A_m^J$, so that its cokernel is a projective $A_m$-module. The A-module $\mathrm{Coker}(u'')$ is finitely presented by construction; it is therefore projective (II, § 5, No. 2, Th. 1). The homomorphism $u''$ is injective (II, § 3, No. 3, Th. 1); consequently, $u$ is injective. The A-module $\mathrm{Coker}(u')$ is isomorphic, on the one hand to $\mathrm{Coker}(u) \oplus N'$, on the other hand to $\mathrm{Coker}(u'') \oplus A^{(I-J)}$. Since the A-modules $A^{(I-J)}$, $\mathrm{Coker}(u'')$ and $N'$ are projective, the same is true of $\mathrm{Coker}(u)$, which completes the proving of (iv).

### 9. The Jacobian criterion

Let k be a ring, A a k-algebra, J an ideal of A and $\bar{d} : J/J^2 \to \Lambda/J \otimes_A \Omega_k(A)$ the canonical mapping. For each A/J-algebra R, one denotes by
$$
\bar{d}_R : R \otimes_{\Lambda/J} J/J^2 \longrightarrow R \otimes_A \Omega_k(A)
$$

the R-linear mapping induced by $\bar{d}$. If the $k$-algebra $A/J$ is formally smooth, $\bar{d}$ has an A-linear retraction (No. 2, Remark 1) and $\bar{d}_R$ has an R-linear retraction for every R.

More generally:

#### Lemma 3 {#ac-x-s7-lem-3 .statement}

Let K be an ideal of A containing J. Suppose that there exists an integer m such that $J \cap K^m$ is contained in JK (this condition is satisfied if A is noetherian). If $A/J$ is formally smooth over k for the K/J-adic topology, the mapping $\bar{d}_{A/K} : A/K \otimes_{A/J} J/J^2 \longrightarrow A/K \otimes_A \Omega_k(A)$ has an A-linear retraction.

Let C denote the $k$-algebra $A/(JK + K^m)$; the ideal N = $(J + K^m)/(JK + K^m)$ of C is square zero and the quotient ring C/N identifies with $A/(J + K^m)$. Endow C and C/N with the discrete topology, and A/J with the K/J-adic topology. The canonical homomorphism $A/J \to A/(J + K^m)$ is continuous; it therefore has a lifting $\varphi : A/J \to A/(JK + K^m)$.

The mapping $a \mapsto a1_C - \varphi(a1_{A/J})$ of A into N is then a $k$-derivation (No. 1, Prop. 1), hence is written $a \mapsto u(da)$ with $u \in \mathrm{Hom}_A(\Omega_k(A), N)$. But the assumption $J \cap K^m \subset JK$ implies $J \cap (JK + K^m) = JK$, so that the canonical mapping $\psi : J/JK \to N$ is bijective; there therefore exists $v \in \mathrm{Hom}_{A/K}(A/K \otimes_A \Omega_k(A), J/JK)$ such that, for a in A, one has $a1_C = \varphi(a1_{A/J}) + \psi(v(1 \otimes da))$. Taking a in J, one sees that $v(1 \otimes da)$ is equal to the class of a in J/JK. Since $A/K \otimes_{A/J} J/J^2$ identifies with $J/JK$, $v$ is the required retraction.

The fact that the condition on K is satisfied when the algebra A is noetherian follows from III, § 3, No. 1, Cor. 2 of Prop. 1.

#### Lemma 4 {#ac-x-s7-lem-4 .statement}

Suppose that A is formally smooth over k for the J-adic topology. In order that $A/J$ be formally smooth over k, it is necessary and sufficient that the canonical mapping $\bar{d}$ have an A-linear retraction.

It is already known that if $A/J$ is formally smooth over $k$, the mapping $\bar{d}$ admits an A-linear retraction (No. 2, Remark 1). Conversely, suppose that $\bar{d}$ has an A-linear retraction. Let $\pi : A/J^2 \to A/J$ be the canonical surjection; by Prop. 2 of No. 1, there exists a ring homomorphism $h : A/J \to A/J^2$ such that $\pi \circ h = \mathrm{Id}_{A/J}$. Let C be a $k$-algebra, N an ideal of C which is square zero, and $\rho : C \to C/N$ the canonical surjection; endow C and C/N with the discrete topology. Let $u : A/J \to C/N$ be a continuous homomorphism of $k$-algebras. Since A is formally smooth over $k$ for the J-adic topology, there exists a homomorphism of $k$-algebras $v : A \to C$ making the diagram

$$
\begin{array}{ccc}
A & \xrightarrow{v} & C \\
\downarrow & & \downarrow \rho \\
A/J & \xrightarrow{u} & C/N
\end{array}
$$

commutative, where the vertical arrows represent the canonical surjections. One has $v(J) \subset \mathbf{N}$, hence $v(J^2) \subset \mathbf{N}^2 = \{0\}$, and $v$ defines, by passing to quotients, a homomorphism $\bar{v} : A/J^2 \to C$ which satisfies $\rho \circ \bar{v} = u \circ \pi$. Then $\bar{v} \circ h$ is a lifting of $u$ to $C$.

#### Theorem 3 {#ac-x-s7-thm-3 .statement}

Let $k$ be a ring, $A$ a formally smooth $k$-algebra, and $J$ a finitely generated ideal of $A$; put $B = A/J$.

a) Let $\mathfrak{p}$ be a prime ideal of $B$ and let $q$ be the (prime) ideal of $A$ such that $\mathfrak{p} = q/J$. The following conditions are equivalent:
(i) the $k$-algebra $B_{\mathfrak{p}}$ is formally smooth;
(ii) there exists $f \in B - \mathfrak{p}$ such that the $k$-algebra $B_f$ is formally smooth;
(iii) the $\kappa(\mathfrak{p})$-linear mapping
$$
\bar{d}_{\kappa(\mathfrak{p})} : \kappa(\mathfrak{p}) \otimes_B J/J^2 \to \kappa(\mathfrak{p}) \otimes_A \Omega_k(\Lambda)
$$
is injective;
(iv) there exist an integer $m \geqslant 0$, elements $f_1, \ldots, f_m$ of $J$, whose images $(f_1)_q, \ldots, (f_m)_q$ generate the ideal $J_q$, and $k$-derivations $D_1, \ldots, D_m$ of $A$ such that $\det(D_j(f_i)) \notin q$.

b) The set of prime ideals $\mathfrak{p}$ of $B$ which satisfy the equivalent conditions of a) is open in $\mathrm{Spec}(B)$. In order that $B$ be formally smooth over $k$, it is necessary and sufficient that every prime (resp. maximal) ideal of $B$ satisfy these conditions.

c) Suppose that $A$ is noetherian. The conditions of a) are also equivalent to:
(v) the $k$-algebra $B_{\mathfrak{p}}$ is formally smooth for the $\mathfrak{p}B_{\mathfrak{p}}$-adic topology.
Moreover, under the conditions of (iv), the ideal $J_q$ is completely secant and the sequence $((f_1)_q, \ldots, (f_m)_q)$ is completely secant for $A_q$.

Put $M = J/J^2$ and $N = B \otimes_A \Omega_k(A)$. The $B$-module $M$ is of finite type, and the $B$-module $N$ is projective (No. 5, Corollary 3 of Theorem 2). For every multiplicative subset $S$ of $A$, the $k$-algebra $S^{-1}A$ is formally smooth (No. 2, Proposition 4, a)). By Lemma 4, conditions (i) and (ii) are therefore equivalent respectively to
(i') the mapping $\bar{d}_{B_{\mathfrak{p}}} : M_{\mathfrak{p}} \to N_{\mathfrak{p}}$ has a $B_{\mathfrak{p}}$-linear retraction;
(ii') there exists $f \in B - \mathfrak{p}$ such that the mapping $\bar{d}_{B_f} : M_f \to N_f$ has a $B_f$-linear retraction.

Prop. 9 of No. 8 applied to the ring $B$ and to the homomorphism $\bar{d} : M \to N$ implies the equivalence of conditions (i'), (ii'') and (iii), and also entails the assertions of b) (using again Lemma 4). Moreover, (iii) is equivalent to:
(iii') the mapping $\kappa(q) \otimes_A J \to \kappa(q) \otimes_A \Omega_k(A)$ deduced from $d : J \to \Omega_k(A)$ is injective,
whereas (iv) may be written:
(iv') there exist an integer $m \geqslant 0$, elements $f_1, \ldots, f_m$ of $J$ whose images generate the ideal $J_q$ of $A_q$, and elements $y_1, \ldots, y_m$ of $\mathrm{Hom}_A(\Omega_k(A), A)$ such that $\det(<y_j, df_i>) \notin q$.

Since the $A$-module $\Omega_k(A)$ is projective (No. 5, Cor. 3 of Th. 2), Prop. 9 of No. 8, applied to the ring $A$ and to the homomorphism $d : J \to \Omega_k(A)$, yields the equivalence of (iii') and (iv').

Finally, suppose the ring $A$ noetherian. It is clear that (i) implies (v). Under assumption (v), Lemma 3 shows that the mapping

$$
\bar{d}_{\kappa(q)} : \kappa(q) \otimes_{B_p} J_q / J_q^2 \longrightarrow \kappa(q) \otimes_{A_q} \Omega_k(A_q)
$$

is injective, whence (iii).

Under the conditions of (iv), one has $m = [\kappa(q) \otimes_A J : \kappa(q)]$ (No. 9, Prop. 8). By Th. 2 of No. 5, the ideal $J_q$ is completely secant, and the sequence $((f_1)_q, \ldots, (f_m)_q)$ is completely secant for $A_q$ ($§ 1$, No. 3, Cor. 2 of Th. 1). This proves c).

#### Corollary 1 {#ac-x-s7-thm-3-cor-1 .statement}

*Let $k_0$ be a ring, $k$ a noetherian $k_0$-algebra formally smooth, and $B$ a local $k$-algebra essentially of finite type. If the $k_0$-algebra $B$ is formally smooth for the $\mathfrak{m}_B$-adic topology, it is formally smooth.*

There exist an integer $n \geqslant 0$, a multiplicative subset $S$ of $k[T_1, \ldots, T_n]$, and a surjective $k$-homomorphism $S^{-1} k[T_1, \ldots, T_n] \to B$. The algebra $S^{-1} k[T_1, \ldots, T_n]$ is noetherian and formally smooth over $k$ (No. 3, Example 2 and No. 2, Prop. 4, a)), hence over $k_0$ (No. 2, Prop. 3, a)). The corollary then follows from Th. 3, c).

#### Corollary 2 {#ac-x-s7-thm-3-cor-2 .statement}

*Let $k_0$ be a ring, $k$ a noetherian $k_0$-algebra formally smooth, and $B$ a $k$-algebra essentially of finite type. The set $U$ of prime ideals $\mathfrak{p}$ of $B$ such that the $k_0$-algebra $B_{\mathfrak{p}}$ is formally smooth (for the discrete topology or the $\mathfrak{p}B_{\mathfrak{p}}$-adic topology) is open in $\operatorname{Spec}(B)$ and the following conditions are equivalent:

(i) *one has* $U = \operatorname{Spec}(B)$ ;
(ii) $U$ *contains all the maximal ideals of* $B$ ;
(iii) *the* $k_0$*-algebra* $B$ *is formally smooth*.

This follows as above from Th. 3.

#### Remark 1 {#ac-x-s7-n9-rem-1 .statement}

Corollaries 1 and 2 apply in particular when $k_0$ is a field and one is in one of the following two cases:
a) $B$ is an algebra essentially of finite type over a separable extension of $k_0$ (th. 1 of No. 3);
b) $B$ is a complete noetherian local $k_0$-algebra whose residue field $\kappa_B$ is a separable extension of $k_0$ (in this case one takes for $k$ an algebra of formal power series over $\kappa_B$ of which $B$ is a quotient (No. 3 and IX, § 3, No. 3)).
In each of these cases, it follows from cor. 2, having regard to prop. 8 of No. 7 and prop. 6, b) of § 6, No. 4, that the $k_0$-algebra $B$ is formally smooth if and only if it is absolutely regular.

**Corollary 3 (Zariski).** — *Let $k$ be a field, $A$ a regular local $k$-algebra, and $J$ an ideal of $A$ distinct from $A$. Suppose that the $k$-algebra $A$ is essentially of finite type or complete. In order that the local ring $A/J$ be regular, it is necessary and sufficient that there exist an integer $m \geqslant 0$, elements $f_1, \ldots, f_m$ of $J$ generating $J$, and derivations $D_1, \ldots, D_m$ of $A$ such that $\det(D_j(f_i)) \notin \mathfrak{m}_A$. The elements $(f_1, \ldots, f_m)$ then form part of a system of coordinates of $A$ and the ideal $J$ is prime.*

Let $k_0$ be the prime subfield of $k$. The $k_0$-algebra $A$ is absolutely regular ($§ 6$, No. 4, example 1), hence formally smooth (remark 1 above). For the same reasons, to say that $A/J$ is regular is equivalent to saying that it is a formally smooth $k_0$-algebra. The first assertion therefore follows from th. 3, which also implies that the sequence $(f_1, \ldots, f_m)$ is completely secant for $A$. One then applies prop. 2 of VIII, $§ 5$, No. 3.

#### Remark 2 {#ac-x-s7-n9-rem-2 .statement}

Under the hypotheses of cor. 3, the $A$-module $\Omega(A)$ is projective (No. 5, cor. 3 of th. 2), hence free; every derivation of $A$ into $\kappa_A$ therefore lifts to a derivation of $A$. The condition of the statement may therefore be expressed as follows: there exist a generating system $(f_1, \ldots, f_m)$ of $J$ and derivations $D_1, \ldots, D_m$ of $A$ into $\kappa_A$, such that $\det(D_j(f_i)) \neq 0$.

#### Corollary 4 (Zariski) {#ac-x-s7-thm-3-cor-4 .statement}

*Let $k$ be a field and $A$ a $k$-algebra essentially of finite type or a complete noetherian local ring. The set of prime ideals $\mathfrak{p}$ of $A$ such that the local ring $A_{\mathfrak{p}}$ is regular is open in $\mathrm{Spec}(A)$*.

It is enough to apply Remark 1, taking for $k_0$ the prime subfield of $k$.

### 10. Smooth algebras

#### Lemma 5 {#ac-x-s7-lem-5 .statement}

*Let $\rho : A \to B$ be a local homomorphism of noetherian local rings. Suppose that $B$ is essentially of finite type over $A$. For the $A$-algebra $B$ to be formally smooth, it is necessary and sufficient that the $A$-module $B$ be flat and that the $\kappa_A$-algebra $\kappa_A \otimes_A B$ be absolutely regular.*

There exists an integer $n \geqslant 0$, a prime ideal $q$ of $A[T_1, \ldots, T_n]$, and a surjective homomorphism $h$ of $A[T_1, \ldots, T_n]_q$ onto $B$. Let $C$ denote the local $A$-algebra $A[T_1, \ldots, T_n]_q$; it is formally smooth (No. 3, Example 2 and No. 2, Prop. 4, a)) and flat over $A$, and one can identify $B$ with the $A$-algebra $C/J$, where $J = \mathrm{Ker}(h)$.

Put $\overline{C} = \kappa_A \otimes_A C$ and $\overline{B} = \kappa_A \otimes_A B$. Suppose that $B$ is formally smooth over $A$. Then the $\kappa_A$-algebra $\overline{B}$ is formally smooth (No. 2, Prop. 4, b)), hence absolutely regular (No. 5, Cor. 2 of Th. 2). Moreover, since $\overline{C}/J\overline{C}$ can be identified with $\overline{B}$ and the $\kappa_A$-algebra $\overline{C}$ is formally smooth, the ideal $J\overline{C}$ of $\overline{C}$ is completely secant (No. 5, Th. 2). It then follows from § 5, No. 6, Prop. 6 that the $A$-module $B$ is flat.

Suppose conversely that $B$ is flat over $A$ and that the $\kappa_A$-algebra $\overline{B}$ is absolutely regular. Then the local $\kappa_A$-algebra $\overline{B}$ is formally smooth (Remark 1 of No. 9 with $k = k_0 = \kappa_A$). Put $\overline{J} = \kappa_A \otimes_A J$; since $B$ is a flat $A$-module, the canonical mapping $\overline{J} \to J\overline{C}$ is bijective and $\overline{B}$ can be identified with $\overline{C}/\overline{J}$. It follows (Remark 1 of No. 2) that the canonical mapping

$$
\overline{J}/\overline{J}^2 \longrightarrow \overline{B} \otimes_{\overline{C}} \Omega_{\kappa_A}(\overline{C})
$$

is injective and admits a retraction. Now $\overline{J}/\overline{J}^2$ is identified with $\kappa_A \otimes_A J/J^2$, hence with $\overline{B} \otimes_B J/J^2$; on the other hand, the $\overline{C}$-module $\Omega_{\kappa_A}(\overline{C})$ is canonically isomorphic to $\overline{C} \otimes_C \Omega_A(C)$ (A, III, p. 136, prop. 20), hence $\overline{B} \otimes_{\overline{C}} \Omega_{\kappa_A}(\overline{C})$ is canonically isomorphic to $\overline{B} \otimes_C \Omega_A(C)$. Passing to the quotient by the maximal ideal of $\overline{B}$, one obtains an injective homomorphism

$$
\kappa_B \otimes_B J/J^2 \longrightarrow \kappa_B \otimes_C \Omega_A(C)
$$

which is none other than $d_{\kappa_B}$. Thus B is formally smooth over A (th. 3).

#### Theorem 4 {#ac-x-s7-thm-4 .statement}

Let A be a noetherian ring and B an A-algebra essentially of finite type. The following conditions are equivalent:

(i) the A-algebra B is formally smooth ;
(ii) for every $q \in \mathrm{Spec}(B)$, the A-algebra $B_q$ is formally smooth (resp. formally smooth for the $qB_q$-adic topology) ;
(iii) the A-module B is flat and, for every $p \in \mathrm{Spec}(A)$, the $\kappa(p)\text{-algebra} \ \kappa(p) \otimes_A B$ is absolutely regular ;
(iv) the A-module B is flat and, for every regular A-algebra R, the ring $R \otimes_A B$ is regular ;
(v) the A-module B is flat and the kernel of the homomorphism $\mu : B \otimes_A B \to B$ such that $\mu(x \otimes y) = xy$ is a completely secant ideal.

The equivalence of (i) and (ii) follows from cor. 2 of th. 3 (No. 9).

(i)⇒(v) : suppose the A-algebra B formally smooth. Let q be a prime ideal of B, and p its inverse image in A. The $A_p$-algebra $B_q$ is formally smooth (prop. 4, a) of No. 2), hence flat (lemma 5) ; consequently the A-module B is flat (II, § 3, No. 4, prop. 15). On the other hand, the ring $B \otimes_A B$ is noetherian (§ 6, No. 1, cor. of prop. 2), hence the ideal $\mathrm{Ker}\,\mu$ is completely secant by cor. 3 of th. 2 (No. 5).

(v)⇒(iii) : suppose condition (v) satisfied. Put $I = \mathrm{Ker}(\mu)$. Let $p \in \mathrm{Spec}(A)$. The mapping

$$
1 \otimes \mu : \kappa(p) \otimes_A (B \otimes_A B) \to \kappa(p) \otimes_A B
$$

is identified with the mapping

$$
\mu_p : (\kappa(p) \otimes_A B) \otimes_{\kappa(p)} (\kappa(p) \otimes_A B) \to \kappa(p) \otimes_A B
$$

deduced from the multiplication of the $\kappa(p)\text{-algebra} \ \kappa(p) \otimes_A B$. The ideal $\mathrm{Ker}(\mu_p)$ is identified with $I(\kappa(p) \otimes_A (B \otimes_A B))$. It is completely secant since the A-module B is flat (§ 5, No. 6, prop. 6). Assertion (iii) then follows from prop. 8 of § 6, No. 5.

(iii)⇒(ii) : let q be a prime ideal of B, and p its inverse image in A. Under the hypotheses of (iii), the $A_p$-module $B_q$ is flat, and the $\kappa(p)\text{-algebra} \ \kappa(p) \otimes_{A_p} B_q$, which is identified with a ring of fractions of $\kappa(p) \otimes_A B$, is absolutely regular (§ 6, No. 4, prop. 6). It follows from lemma 5 that $B_q$ is formally smooth over $A_p$, hence over A (No. 2, prop. 3 and 4).

(iii)⇒(iv) : let us place ourselves under the hypotheses of (iii). Let R be a regular A-algebra. The R-module $R \otimes_A B$ is flat (I, § 2, No. 7, cor. 2 to prop. 8). Let r be a prime ideal of R and p its inverse image in A ; the ring $\kappa(r) \otimes_R (R \otimes_A B)$, which is identified with $\kappa(r) \otimes_{\kappa(p)} (\kappa(p) \otimes_A B)$, is regular (§ 6, No. 4, cor. 2 of prop. 7). The ring $R \otimes_A B$ is therefore regular (§ 4, No. 5, cor. of prop. 9).

(iv) ⇒ (iii) : let $p$ be a prime ideal of $A$ and let $k$ be an extension of $\kappa(p)$; under the hypotheses of (iv), the ring $k \otimes_{\kappa(p)} (\kappa(p) \otimes_A B)$, which is identified with $k \otimes_A B$, is regular, whence (iii).

#### Definition 2 {#ac-x-s7-def-2 .statement}

Let $A$ be a noetherian ring. An $A$-algebra $B$ is said to be smooth if it is essentially of finite type and if it satisfies the equivalent conditions of theorem 4.

#### Proposition 10 {#ac-x-s7-prop-10 .statement}

Let $A$ be a noetherian ring.

a) Let $A'$ be a noetherian $A$-algebra and $B$ a smooth $A$-algebra. Then the $A'$-algebra $A' \otimes_A B$ is smooth.

b) Let $B$ be a smooth $A$-algebra and $C$ a smooth $B$-algebra. Then the $A$-algebra $C$ is smooth.

c) Let $B$ and $C$ be two smooth $A$-algebras. Then the $A$-algebra $B \otimes_A C$ is smooth.

This follows from Prop. 4 of No. 2 and from the analogous statements for algebras essentially of finite type (§ 6, No. 1).

#### Example 1 {#ac-x-s7-n10-exa-1 .statement}

The smooth algebras over a field $k$ are the $k$-algebras essentially of finite type and absolutely regular.

#### Example 2 {#ac-x-s7-n10-exa-2 .statement}

Let $A$ be a noetherian ring, $T = (T_i)_{i \in I}$ a finite family of indeterminates. The $A$-algebra $A[T]$ is smooth. More generally, let $F_1, \ldots, F_m$ be elements of $A[T]$, and let $B$ be the $A$-algebra $A[T]/(F_1, \ldots, F_m)$. If at every maximal ideal $n$ of $B$ the class (mod. $n$) of the matrix $\left( \frac{\partial F_j}{\partial T_i} \right)$ is of rank $m$, the $A$-algebra $B$ is smooth (Theorem 3 of No. 9).

## EXERCISES {#ac-x-s7-exercises}

See the [exercises for § 7](exercises/s7/).
