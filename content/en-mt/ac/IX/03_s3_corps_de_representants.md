---
book: ac
book_title: Commutative Algebra
chapter: IX
chapter_title: ANNEAUX LOCAUX NOETHÉRIENS COMPLETS
section: 3
section_title: Corps de représentants
lang: en
source: ac-viii-ix-fr
book_pages: AC IX.28-AC IX.30, AC IX.75-AC IX.78
pdf_pages: 0140-0142, 0187-0190
extraction: ocr
subsections:
    - "no": 1
      title: Anneaux locaux d’égales caractéristiques
      page: 28
      pdf_page: 140
    - "no": 2
      title: Un théorème de relèvement
      page: 28
      pdf_page: 140
    - "no": 3
      title: Corps de représentants
      page: 29
      pdf_page: 141
statements: 7
exercises: 9
content_sha256: 6c19e36e8e9fe2a14bd3f138891e6c1cece185efb7ead4bcf2d5736981b90781
translated_from: content/fr/ac/IX/03_s3_corps_de_representants.md
source_lang: fr
translation_method: machine
source_content_sha256: f87346f41fd15cf679aaa4db67e841015ffb1e15814b135f808cfb3c36b391f2
translation_model: gpt-5-6-mini, gpt-5.4
translation_run: translate-en-mt-42a1da81
glossary_version: 34
glossary_terms_sha256: 41ba4583c5bb2c9231cfb0f9ac94252c23bb48f1776e6582e40604374d5a2f87
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 3. Fields of representatives

### 1. Local rings of equal characteristics

Let A be a ring. Recall (A, V, p. 2) that the characteristic of A is defined when A contains a subfield. It is equal to 0 if and only if A contains a subfield isomorphic to $\mathbf{Q}$; and equal to a prime number $p$ if and only if one has $p1_A = 0$. If the characteristic of A is defined, and if $f : A \to B$ is a nonzero homomorphism of rings, the characteristic of B is defined and it is equal to that of A.

Let A be a local ring, with maximal ideal $m$, and residue field $k$.

a) Suppose that $k$ has characteristic 0. Then A contains a field and the characteristic of A is equal to 0. Indeed, the canonical homomorphism from $\mathbf{Z}$ into A is injective, and for every nonzero integer $n$, $n1_A$ is invertible in A, because it does not belong to $m$.

b) Suppose that $k$ has characteristic $p \neq 0$. Then A contains a field if and only if $p1_A = 0$. In this case the characteristic of A is equal to $p$.

Suppose that A is an integral local ring, with field of fractions K and residue field $k$.

a’) The ring A contains a subfield if and only if the characteristics of $k$ and K are equal. In this case, the characteristic of A is equal to that of $k$ and K, and one says that A is a local ring of equal characteristics.

b’) Suppose that the fields $k$ and K do not have the same characteristic. Then there exists a prime number $p$ such that $k$ has characteristic $p$. Since one has $q1_A \neq 0$ for every prime number $q \neq p$, the field K has characteristic 0. One then says that A is a local ring of unequal characteristics.

### 2. A lifting theorem

#### Proposition 1 {#ac-ix-s3-prop-1 .statement}

Let $k_0$ be a field, A a $k_0$-algebra which is a separated and complete local ring, K a sub-$k_0$-extension of $\kappa_A$ which possesses a separating transcendence basis $(\xi_{\lambda})_{\lambda \in \Lambda}$ over $k_0$ (A, V, p. 130, déf. 1). For every $\lambda \in \Lambda$, let $x_{\lambda}$ be a representative of $\xi_{\lambda}$ in A. There exists a unique subfield L of A, containing $k_0$ and the elements $x_{\lambda}$, and such that the canonical homomorphism $\pi$ from A onto $\kappa_A$ induces an isomorphism of L onto K.

Let $\varphi$ be the $k_0$-homomorphism of the polynomial ring $k_0[(X_{\lambda})_{\lambda \in \Lambda}]$ into A which maps $X_{\lambda}$ onto $x_{\lambda}$ for every $\lambda \in \Lambda$. Let $u$ be a nonzero element of $k_0[(X_{\lambda})_{\lambda \in \Lambda}]$; one has $\pi(\varphi(u)) \neq 0$, because the family $(\xi_{\lambda})_{\lambda \in \Lambda}$ is algebraically free over $k_0$ in $\kappa_A$; consequently, $\varphi(u)$ is invertible in the local ring A. It follows that $\varphi$ extends to a homomorphism $\psi$ of the field $k_1 = k_0((X_{\lambda})_{\lambda \in \Lambda})$ into A. Then A is a $k_1$-algebra, $\kappa_A$ is an extension of $k_1$ and K a sub-extension of $\kappa_A$ which is algebraic and separable over $k_1$. It remains to prove that there exists a unique subfield L of A containing $\psi(k_1)$ and such that $\pi(L) = K$.

a) *Existence of L*: Let S be the set of subfields L of A, containing $\psi(k_1)$ and such that $\pi(L) \subset K$; it is inductive for the inclusion relation. Let L be a maximal element of S; we consider K as an extension (algebraic and separable, by A, V, p. 40, prop. 9) of L. Let $\xi \in K$ and let $P \in L[X]$ be its minimal polynomial over L. Since $\xi$ is a simple root of P, Hensel's lemma (III, § 4, no. 5, cor. 1 of th. 2) ensures the existence of an element x of A such that $\pi(x) = \xi$ and $P(x) = 0$. The subring $L[X]$ of A belongs to S; by the maximal character of L, we therefore have $x \in L$, whence $\xi \in \pi(L)$. Finally one has $\pi(L) = K$.

b) *Uniqueness of L*: Let L and L’ be two subfields of A containing $\psi(k_1)$ and such that $\pi(L) = \pi(L') = K$. Let $\xi \in K$, and let $x \in L$ and $x' \in L'$ be the elements such that $\pi(x) = \pi(x') = \xi$. If $P \in k_1[X]$ is the minimal polynomial of $\xi$ over $k_1$, then $\xi$ is a simple root of P, and one has $P(x) = P(x') = 0$. By Hensel's lemma (*loc. cit.*) one has $x = x'$. Therefore $L = L'$.

#### Remark {#ac-ix-s3-n2-rem-1 .statement}

\* The preceding proof applies more generally to the case where one assumes only that A is a henselian local ring*. The proof of uniqueness uses the hypothesis that the local ring A is separated, but not that it is complete.

### 3. Fields of representatives

#### Definition 1 {#ac-ix-s3-def-1 .statement}

*Let A be a local ring. A field of representatives of A is any subfield K of A such that the canonical homomorphism of A onto $\kappa_A$ induces an isomorphism of K onto $\kappa_A$ (in other words, such that $A = K + m_A$).*

There can exist a field of representatives of A only if A has a characteristic. This condition is sufficient when A is separated and complete. More precisely, one has the following theorem:

#### Theorem 1 {#ac-ix-s3-thm-1 .statement}

*Let A be a separated and complete local ring of characteristic p.*

a) *Assume $p = 0$ and let $(x_\lambda)_{\lambda \in \Lambda}$ be a family of elements of A whose classes modulo $m_A$ form a transcendence basis of $\kappa_A$ over $\mathbf{Q}$. There exists a unique field of representatives of A containing the elements $x_\lambda$.*

b) *Assume $p \neq 0$. Let $(x_\lambda)_{\lambda \in \Lambda}$ be a family of elements of A whose classes modulo $m_A$ form a p-basis of $\kappa_A$ (A, V, p. 95). There exists a unique field of representatives of A containing the elements $x_\lambda$. It is a Cohen subring of A.*

Assume that one has $p = 0$, so that A is a $\mathbf{Q}$-algebra. Every transcendence basis of $\kappa_A$ over $\mathbf{Q}$ being separating, assertion a) follows from prop. 1 of no. 1 applied to the case $k_0 = \mathbf{Q}$, $K = \kappa_A$.

Assume now that one has $p \neq 0$. Then one has $p1_A = 0$, and every Cohen subring C of A satisfies $pC = 0$. In other words, there is identity between the notions of field of representatives and of Cohen subring of A. Assertion b) then follows from § 2, no. 2, th. 1.

#### Corollary 1 {#ac-ix-s3-thm-1-cor-1 .statement}

Let $A$ be a separated and complete local ring, whose residue field is an algebraic extension of $\mathbf{Q}$. Then there exists a unique field of representatives of $A$.
In fact the ring $A$ is of characteristic 0 (no. 1).

#### Corollary 2 {#ac-ix-s3-thm-1-cor-2 .statement}

Let $A$ be a separated and complete local ring of characteristic $p \neq 0$. Assume that the residue field $\kappa_A$ is perfect. Then there exists a unique field of representatives of $A$, namely the set of multiplicative representatives.
Cor. 2 follows immediately from th. 1 and prop. 7 of § 2, no. 4.

#### Theorem 2 {#ac-ix-s3-thm-2 .statement}

Let $A$ be a complete noetherian local ring of dimension $d$ containing a field. Let $K$ be a coefficient field of $A$, and let $m$ be the dimension of the vector space $m_A/m_A^2$ over the field $K$.
a) There exists an ideal $a$ of $K[[T_1, ..., T_m]]$ such that the $K$-algebra $A$ is isomorphic to $K[[T_1, ..., T_m]]/a$.
b) There exists a sub-$K$-algebra $A'$ of $A$, isomorphic to $K[[T_1, ..., T_d]]$ and such that $A$ is a finite algebra over $A'$.
c) Suppose that the noetherian local ring $A$ is regular, i.e. $d = m$. Then there exists a $K$-isomorphism of $A$ onto $K[[T_1, ..., T_d]]$.
Let $t_1, ..., t_m$ be elements of $m_A$ whose classes modulo $m_A^2$ generate the vector space $m_A/m_A^2$ over $K$. By lemma 3 of § 2, No. 5, there exists a surjective $K$-homomorphism of $K[[T_1, ..., T_m]]$ into $A$, mapping $T_i$ to $t_i$ for $1 \leq i \leq m$. This proves $a$.
Analogously, assertion $b$ follows from lemma 4 of loc. cit. and from the existence of a maximal secant sequence for $A$ (VIII, § 3, No. 2, th. 1).
Finally, assertion $c$ is nothing but cor. 3 of th. 1 of VIII, § 5, No. 2.

## EXERCISES {#ac-ix-s3-exercises}

See the [exercises for § 3](exercises/s3/).
