---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 1
section_title: Artinian Modules and Noetherian Modules
lang: en
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.1-A VIII.23
pdf_pages: 0018-0040
extraction: native
subsections:
    - "no": 1
      title: Artinian Modules and Noetherian Modules
      page: 1
      pdf_page: 18
    - "no": 2
      title: Artinian Rings and Noetherian Rings
      page: 4
      pdf_page: 21
    - "no": 3
      title: Countermodule
      page: 8
      pdf_page: 25
    - "no": 4
      title: Polynomials with Coefficients in a Noetherian Ring
      page: 9
      pdf_page: 26
statements: 32
exercises: 28
content_sha256: 77443c27be06346c288e3d1177382bf078e623074399997285ec822cf3e2f114
---

## § 1. ARTINIAN MODULES AND NOETHERIAN MODULES

### 1. Artinian Modules and Noetherian Modules

#### Definition 1 {#alg-viii-s1-def-1 .statement tag=0001}

Let A be a ring. We call an A-module M Artinian (resp. Noetherian) if it satisfies the following equivalent conditions:

(i) Every nonempty set of submodules of M, ordered by inclusion, has a minimal (resp. maximal) element.

(ii) Every decreasing (resp. increasing) sequence of submodules of M is stationary.

The equivalence of conditions (i) and (ii) follows from Set Theory, III, §6, No. 5, p. 190, Proposition 6.

An A-module M is Artinian (resp. Noetherian) if and only if M, viewed as a module over the ring of homotheties $A_M$, is Artinian (resp. Noetherian).

Let M be an Artinian (resp. Noetherian) A-module. Every nonempty set of submodules of M, ordered by inclusion, that is left directed (resp. right directed) has a least element (resp. a greatest element) (Set Theory, III, §1, No. 10, p. 145, Proposition 10).

Let M be an Artinian (resp. Noetherian) A-module and $(M_i)_{i\in I}$ a family of submodules of M. The intersections (resp. sums) of finite subfamilies of the family $(M_i)_{i\in I}$ form a nonempty left (resp. right) directed set of submodules of M. Therefore, there exists a finite subset J of I such that $\bigcap_{i\in I}M_i=\bigcap_{i\in J}M_i$ (resp. $\sum_{i\in I}M_i=\sum_{i\in J}M_i)$.

#### Example 1 {#alg-viii-s1-n1-exa-1 .statement tag=0002}

A finite-dimensional vector space over a field is Artinian and Noetherian.

#### Example 2 {#alg-viii-s1-n1-exa-2 .statement tag=0003}

Let M be an A-module. If there exists an infinite family $(M_i)_{i\in I}$ of nonzero submodules of M whose sum is direct, then M is neither Artinian nor Noetherian: indeed, for every strictly decreasing (resp. strictly increasing) infinite sequence $(J_n)$ of subsets of I, the infinite sequence $(\sum_{i\in J_n}M_i)$ of submodules of M is strictly decreasing (resp. strictly increasing). In particular, an infinite-dimensional vector space over a field is neither Artinian nor Noetherian.

#### Example 3 {#alg-viii-s1-n1-exa-3 .statement tag=0004}

We will see further on that the $\mathbf{Z}$-module $\mathbf{Z}$ is Noetherian but not

Artinian (VIII, p. 5, Example 3$).*$

#### Example 4 {#alg-viii-s1-n1-exa-4 .statement tag=0005}

Let $p$ be a prime number and $M_p$ the $p$-primary component of the torsion $\mathbf{Z}$-module $\mathbf{Q}/\mathbf{Z}$ (VII, §2, No. 2, p. 7). Every submodule of $M_p$ is equal to either $M_p$ or $p^{-n}\mathbf{Z}/\mathbf{Z}$ for an integer $n\in \mathbf{N}$ (VII, §2, p. 54, Exercise 3). Consequently, $M_p$ is an Artinian but not Noetherian $\mathbf{Z}$-module.

#### Proposition 1 {#alg-viii-s1-prop-1 .statement tag=0006}

An A-module M has finite length (II, §1, No. 10, p. 212) if and only if it is both Artinian and Noetherian.

Suppose that M has finite length $d$. Then every strictly increasing or strictly decreasing sequence of submodules of M has at most $d+ 1$ terms (I, §4, No. 7, p. 44). Consequently, M is Artinian and Noetherian.

Conversely, suppose that M is Artinian and Noetherian. Let $\mathscr{S}$ be the set of submodules of M of finite length. The zero submodule is an element of $\mathscr{S}$, and since M is Noetherian, $\mathscr{S}$ has a maximal element N. Let us give a proof by contradiction and suppose that $M\not= N$. The set of submodules of M distinct from N and containing N then has a minimal element P because M is Artinian. The module $P/N$ has length 1, and since N is a module of finite length, the same holds for P (II, §1, No. 10, p. 212, Proposition 16). This contradicts the definition of N.

#### Proposition 2 {#alg-viii-s1-prop-2 .statement tag=0007}

An A-module M is Noetherian if and only if every submodule of M is finitely generated.

Begin by assuming that every submodule of M is finitely generated. Let $(P_n)_{n\in\mathbf{N}}$ be an increasing sequence of submodules of M, and let P be its union. This is a submodule of M. By assumption, there exists a finite subset F of M generating the module P; let $n\in \mathbf{N}$ be an integer such that $F\subset P_n$. We then have $P_n= P$, and the sequence $(P_n)_{n\in\mathbf{N}}$ is stationary. This proves that the module M is Noetherian.

The converse is a consequence of the following more precise statement.

#### Lemma 1 {#alg-viii-s1-lem-1 .statement tag=0008}

Let M be a Noetherian A-module and E a subset of M. There exists a finite subset F of E generating the same submodule as E.

Indeed, by VIII, p. 2, there exists a finite subset F of E such that $\sum_{x\in E}Ax=\sum_{x\in F}Ax$.

#### Proposition 3 {#alg-viii-s1-prop-3 .statement tag=0009}

Let M be an A-module and N a submodule of M. Then M is Artinian (resp. Noetherian) if and only if N and $M/N$ are.

We will give the proof in the case of Artinian modules; the case of Noetherian modules is analogous.

Suppose that M is Artinian. Since every submodule of N is a submodule of M, the module N is Artinian. Let $(P_n)_{n\in\mathbf{N}}$ be a decreasing sequence of submodules of $M/N$. There exists a decreasing sequence $(Q_n)_{n\in\mathbf{N}}$ of submodules of M containing N such that $P_n= Q_n/N$ for every $n\in \mathbf{N}$ (I, §4, No. 6, p. 41, Theorem 4). Since M is Artinian, the sequence $(Q_n)$ is stationary, hence so is the sequence $(P_n)$. Consequently, the module $M/N$ is Artinian.

Conversely, suppose that the modules N and $M/N$ are Artinian, and consider a decreasing sequence $(P_n)$ of submodules of M. The sequence $P'_n= N\cap P_n$ of submodules of N is stationary. Likewise, the sequence $P''_n= (N + P_n)/N$ of submodules of $M/N$ is stationary. Hence, there exists an integer $m\in \mathbf{N}$ such that we have $P'_n= P'_m$ and $P''_n= P''_m$ for every integer $n\geqslant m$. The sequence $(P_n)$ is then stationary by the following lemma. **Lemma 2.** — Let M be an A-module and N, P, and Q submodules of M. Suppose that we have $P\subset Q$, $N\cap P = N\cap Q$, and N + P = N + Q. We then have P = Q.

Let $x$ be an element of Q. It belongs to N + P; hence, there exists an element $y$ of P such that $x-y\in N$. Since Q contains P, the difference $x-y$ belongs to $N\cap Q$ and therefore to P. Consequently, $x$ belongs to P.

#### Corollary {#alg-viii-s1-n1-cor-1 .statement tag=000A}

Let M be an A-module and $(M_i)_{i\in I}$ a finite family of submodules of M.

a) If the modules $M_i$ are Artinian (resp. Noetherian), then so is their sum $\sum_{i\in I}M_i$.

b) If the modules $M/M_i$ are Artinian (resp. Noetherian), then so is the module $M/\bigcap_{i\in I}M_i$.

By induction, it suffices to treat the case when $I =\{1,2\}$. The module $M_2/(M_1\cap M_2)$, quotient of $M_2$, is isomorphic to the submodule $(M_1+M_2)/M_1$ of $M/M_1$ (I, §4, No. 6, p. 41, Theorem 4).

In part a), we assume that $M_1$ and $(M_1+ M_2)/M_1$ are Artinian (resp. Noetherian); the same then holds for $M_1+ M_2$ (Proposition 3).

In part b), we assume that $M/M_2$ and $M_2/(M_1\cap M_2)$ are Artinian (resp. Noetherian); the same then holds for $M/(M_1\cap M_2)$ (loc. cit.).

#### Example 5 {#alg-viii-s1-n1-exa-5 .statement tag=000B}

Let $(M_i)_{i\in I}$ be a finite family of A-modules. If the modules $M_i$ are Artinian (resp. Noetherian), then so is their direct sum $\bigoplus_{i\in I}M_i$.

#### Remark {#alg-viii-s1-n1-rem-1 .statement tag=000C}

The definitions and results of this subsection extend to arbitrary abelian groups with operators by replacing the submodules in the statements with stable subgroups.

### 2. Artinian Rings and Noetherian Rings

#### Definition 2 {#alg-viii-s1-def-2 .statement tag=000D}

A ring A is said to be left Artinian (resp. left Noetherian) if the left A-module $A_s$ is Artinian (resp. Noetherian). Likewise, a ring A is said to be right Artinian (resp. right Noetherian) if the right A-module $A_d$ is Artinian (resp. Noetherian).

A ring A is right Artinian (resp. right Noetherian) if and only if its opposite ring $A^o$ is left Artinian (resp. left Noetherian). For a commutative ring A, the properties of being left Artinian and of being right Artinian coincide, and when they are hold, we say that the ring A is Artinian; we adopt an analogous convention for “Noetherian.” There exist noncommutative rings that are left Artinian but not right Artinian, and noncommutative rings that are left Noetherian but not right Noetherian (VIII, p. 14, Exercise 3).

Let A be a ring. By definition, the following properties are equivalent:

(i) The ring A is left Artinian.

(ii) Every nonempty set of left ideals of A, ordered by inclusion, has a minimal element.

(iii) Every decreasing sequence of left ideals of A is stationary.

Because of Proposition 2 of VIII, p. 3, the following properties are equivalent:

(i) The ring A is left Noetherian.

(ii) Every nonempty set of left ideals of A, ordered by inclusion, has a maximal element.

(iii) Every increasing sequence of left ideals of A is stationary.

(iv) Every left ideal of A is generated by a finite subset of A.

#### Example 1 {#alg-viii-s1-n2-exa-1 .statement tag=000E}

A field is a ring that is both left and right Artinian and Noetherian.

#### Example 2 {#alg-viii-s1-n2-exa-2 .statement tag=000F}

Let A be a ring and D a subring of A. Suppose that D is a field and that A is a finite-dimensional left vector space over D. Then the ring A is left Artinian and left Noetherian because every left ideal of A is a D-vector subspace of A. In particular, a finite-dimensional algebra over a commutative field is a ring that is both left and right Artinian and Noetherian.

#### Example 3 {#alg-viii-s1-n2-exa-3 .statement tag=000G}

A principal ideal domain (VII, §1, No. 1, p. 1, Definition 1) is Noetherian. An integral domain A that is not a field is not an Artinian ring: for every nonzero noninvertible element $a$ of A, the sequence of ideals $a^nA$ (for $n\in \mathbf{N})$ is strictly decreasing. In particular, the ring $\mathbf{Z}$ of integers is Noetherian but not Artinian.

#### Example 4 {#alg-viii-s1-n2-exa-4 .statement tag=000H}

Let M be an A-module that is the direct sum of an infinite family $(M_i)_{i\in I}$ of nonzero submodules. Let E be the endomorphism ring of M. For every $i\in I$, let $\mathfrak{a}_i$ (resp. $\mathfrak{b}_i)$ be the set of elements of E with kernel containing $\sum_{j\not=i}M_j$ (resp. with image contained in $M_i)$. Then $(\mathfrak{a}_i)$ is an infinite family of nonzero left ideals of E whose sum is direct, and $(\mathfrak{b}_i)$ is an infinite family of nonzero right ideals of E whose sum is direct. Consequently, the ring E is neither left nor right Artinian (resp. Noetherian) (VIII, p. 2, Example 2). In particular, the endomorphism ring of an infinite-dimensional vector space is neither left nor right Artinian (resp. Noetherian). **Theorem 1.** — Let A be a left Artinian ring. The A-module $A_s$ has finite length.

We will use the following lemma in the proof.

#### Lemma 3 {#alg-viii-s1-lem-3 .statement tag=000I}

Let A be a ring and $n$ a natural number. An Artinian A-module M that is the sum of a family of submodules of length $\leqslant n$ has finite length.

We use induction on $n$. First, suppose $n= 1$. If M were not of finite length, then we could construct a sequence $(M_m)_{m\in\mathbf{N}}$ of submodules of M of length 1 with $M_m\not\subset \sum_{i<m}M_i$ for every $m\in \mathbf{N}$. We would then have $M_m\cap \sum_{i<m}M_i= 0$ for every $m$, and the sum of the family $(M_m)_{m\in\mathbf{N}}$ would be direct. However, this contradicts the fact that the A-module M is Artinian (VIII, p. 2, Example 2).

Now, suppose $n\geqslant 2$. Let $(M_i)_{i\in I}$ be a family of submodules of M of length $\leqslant n$ with sum M. For every $i\in I$, choose a submodule $M'_i$ of $M_i$ of length $\leqslant n-1$ such that $M_i/M'_i$ has length $\leqslant 1$. Set $M'=\sum M'_i$, and denote the image of $M_i$ in $M''= M/M'$ by $M''_i$. The modules $M''_i$ are of length $\leqslant 1$, and their sum is $M''$. The modules $M'$ and $M''$ are Artinian (VIII, p. 3, Proposition 3); by the induction hypothesis, they are of finite length. Hence, M has finite length (II, §1, No. 10, p. 212, Proposition 16).

Let us now prove Theorem 1. Let $\mathscr{S}$ denote the set of left ideals $\mathfrak{a}$ of A such that the module $A_s/\mathfrak{a}$ has finite length. Let $(\mathfrak{a}_i)_{i\in I}$ be a finite family of elements of $\mathscr{S}$. By Proposition 1 of VIII, p. 2, the A-module $A_s/\mathfrak{a}_i$ is Artinian and Noetherian for every $i\in I$. Consequently, $A_s/\bigcap_{i\in I}\mathfrak{a}_i$ is Artinian and Noetherian (VIII, p. 4, Corollary of Proposition 3), hence of finite length (VIII, p. 2, Proposition 1). This proves that $\mathscr{S}$ is a left directed set for the inclusion. Since the ring A is left Artinian, the set $\mathscr{S}$ has a least element $\mathfrak{b}$. We denote the length of the A-module $A_s/\mathfrak{b}$ by $n$.

Let $x$ be an element of $A_s$ and $\mathfrak{a}$ its annihilator (II, §1, No. 12, p. 219). The A-module $Ax$ is isomorphic to $A_s/\mathfrak{a}$. If $Ax$ has finite length, then $\mathfrak{a}$ belongs to $\mathscr{S}$, so $\mathfrak{a}$ contains $\mathfrak{b}$ and $Ax$ has length $\leqslant n$. Thus, every monogenous left ideal of A of finite length has length $\leqslant n$. Let $\mathfrak{c}$ be the sum of these ideals; this is a left ideal of A, of finite length by Lemma 3. Every left ideal of A of finite length is a sum of monogenous left ideals of finite length and is therefore contained in $\mathfrak{c}$. Hence, $\mathfrak{c}$ is the largest left ideal of A of finite length.

If $\mathfrak{c}$ were distinct from A, then the set of left ideals of A containing $\mathfrak{c}$ and distinct from $\mathfrak{c}$ would have a minimal element $\mathfrak{c}'$. The A-module $\mathfrak{c}'/\mathfrak{c}$ would then have length 1, and $\mathfrak{c}'$ would have finite length, which contradicts the fact that $\mathfrak{c}$ is maximal. We therefore have $\mathfrak{c}= A$; the A-module $A_s$ has finite length.

#### Corollary {#alg-viii-s1-n2-cor-1 .statement tag=000J}

Every left Artinian ring is left Noetherian.

Let A be a left Artinian ring. By Theorem 1, the A-module $A_s$ has finite length. We then apply Proposition 1 of VIII, p. 2.

Let A be a left (resp. right) Artinian ring; the length of the A-module $A_s$ (resp. $A_d)$ (I, §4, No. 7, p. 44) is called the left (resp. right) length of the ring A. When A is a commutative Artinian ring, these two lengths coincide and are simply called the length of A. When A is left and right Artinian but is not commutative, the left and right lengths of A are not necessarily equal (VIII, p. 14, Exercise 3).

#### Example 5 {#alg-viii-s1-n2-exa-5 .statement tag=000K}

The left and right lengths of a field are equal to 1.

#### Proposition 4 {#alg-viii-s1-prop-4 .statement tag=000L}

a) Let A be a left Noetherian ring and M a finitely generated left A-module. The module M is Noetherian, and every submodule of M is finitely generated.

b) Let A be a left Artinian ring and M a left A-module. The following properties are equivalent: the module M is finitely generated; the module M is Artinian; the module M has finite length; the module M is Noetherian.

Let us prove a). Every monogenous submodule of M is isomorphic to a quotient of $A_s$, hence is Noetherian by Proposition 3 of VIII, p. 3. The module M is a finite sum of such submodules; it is therefore Noetherian by the corollary (VIII, p. 4) of Proposition 3. Every submodule of M is then finitely generated (VIII, p. 3, Proposition 2)

Now, suppose that the ring A is left Artinian. We see, as in the previous section, that if the A-module M is finitely generated, then it is Artinian. If it is Artinian, then it has finite length: indeed, its monogenous submodules are isomorphic to quotients of $A_s$ and are therefore of finite length less than that of $A_s$, and the assertion follows from Lemma 3. Every module of finite length is Noetherian, and every Noetherian module is finitely generated. This proves b).

#### Proposition 5 {#alg-viii-s1-prop-5 .statement tag=000M}

a) Let A be a left Artinian (resp. left Noetherian) ring, and let $\varphi : A\rightarrow B$ be a ring homomorphism that makes B into a finitely generated left A-module. The ring B is left Artinian (resp. left Noetherian).

b) Let A be a left Artinian (resp. left Noetherian) ring, and let $\mathfrak{a}$ be a two-sided ideal of A; the ring $A/\mathfrak{a}$ is left Artinian (resp. left Noetherian).

c) Let $(A_i)_{i\in I}$ be a family of left Artinian (resp. left Noetherian) rings. The ring $\prod_{i\in I}A_i$ is left Artinian (resp. left Noetherian).

We will treat the case of Artinian rings; the case of Noetherian rings is analogous.

Let us prove a). By Proposition 4, the ring $B_s$ is an Artinian left A-module and a fortiori an Artinian left B-module.

Assertion b) follows from assertion a) applied to the canonical homomorphism from A to $A/\mathfrak{a}$.

Let us prove c). Set $A =\prod_{i\in I}A_i$. By assumption, $(A_i)_s$ is an Artinian left $A_i$-module and a fortiori an Artinian left A-module. By Example 5 of VIII, p. 4, the A-module $A_s$ is Artinian.

#### Corollary {#alg-viii-s1-n2-cor-2 .statement tag=000N}

The prime ideals of an Artinian commutative ring are its maximal ideals.

In any commutative ring, a maximal ideal is prime. Let A be an Artinian commutative ring. Let $\mathfrak{p}$ be a prime ideal of A. The ring $A/\mathfrak{p}$ is an integral domain and is Artinian (Proposition 5), hence is a field (VIII, p. 5, Example 3). Consequently, the ideal $\mathfrak{p}$ is maximal.

The polynomial ring $\mathbf{Q}[(X_n)_{n\in\mathbf{N}}]$ is an integral domain; it is not Noetherian (or Artinian) (VIII, p. 15, Exercise 9). It is a subring of its field of fractions, which is an Artinian (and Noetherian) ring.

### 3. Countermodule

#### Definition 3 {#alg-viii-s1-def-3 .statement tag=000O}

Let A be a ring, M an A-module, and E = End$_A(M)$ the endomorphism ring of M. The countermodule of M is the left E-module with the same underlying additive group as M and external law $(c, x)\mapsto c(x)$.

Let Z be the center of the ring A. For every $a\in Z$, the homothety $a_M$ belongs to E. Consequently, E is canonically endowed with the structure of a Z-algebra. In particular, if M is a finitely generated Z-module, then the countermodule of M is finitely generated.

#### Lemma 4 {#alg-viii-s1-lem-4 .statement tag=000P}

Let M be a left A-module with finitely generated countermodule. There exist a natural number $m$ and an injective $A_M$-linear mapping from $(A_M)_s$ to $M^m$.

Set E = End$_A(M)$. Let $(x_1, . . . , x_m)$ be a finite generating family of the E-module M. The mapping $\varphi :a\mapsto (ax_1, . . . , ax_m)$ from $(A_M)_s$ to $M^m$ is $A_M$-linear. Let $a$ be an element of $A_M$ such that $\varphi (a) = 0$. The set of elements $x$ of M such that $ax= 0$ is an E-submodule of M containing $x_1, . . . , x_m$ and is therefore equal to M, which implies $a= 0$.

#### Proposition 6 {#alg-viii-s1-prop-6 .statement tag=000Q}

Let M be an Artinian (resp. Noetherian) left A-module with finitely generated countermodule. The ring of homotheties $A_M$ of M is left Artinian (resp. left Noetherian).

This follows from Lemma 4 and Proposition 3 of VIII, p. 3.

#### Corollary {#alg-viii-s1-n3-cor-1 .statement tag=000R}

Let A be a commutative ring.

a) Let M be a Noetherian A-module. The ring $A_M$ is Noetherian.

b) Let M be an A-module of finite length. The ring $A_M$ is Artinian.

Let M be an A-module. Under the assumptions of a) or b), the A-module M is finitely generated. Since A is commutative, $A_M$ is contained in the ring End$_A$(M), so that the countermodule of M is finitely generated. It then suffices to apply Proposition 6.

#### Remark {#alg-viii-s1-n3-rem-1 .statement tag=000S}

Let A be a ring. An Artinian left A-module M with finitely generated countermodule has finite length: indeed, the ring of homotheties $A_M$ of M is left Artinian (Proposition 6), and M is an Artinian module over $A_M$; by VIII, p. 7, Proposition 4, the module M has finite length over $A_M$ and therefore also over A.

In particular, every finitely generated Artinian module over a commutative ring has finite length. By contrast, a finitely generated Artinian module over a noncommutative ring is not necessarily of finite length (VIII, p. 16, Exercise 12).

### 4. Polynomials with Coefficients in a Noetherian Ring

Let A be a ring, $\sigma$ an endomorphism of the ring A, and $d$ an endomorphism of the additive group of A satisfying the relation

$$
d(ab) =\sigma (a)d(b) +d(a)b \tag{1}
$$

for all $a, b\in A$. In other words, $d$ is a derivation from the ring A to the $(A$, A)-bimodule obtained by endowing the additive group of A with the left law of action $(a, x)\mapsto \sigma (a)x$ and the right law of action $(x, a)\mapsto xa$. We have $d(1) = 0$ (III, §10, No. 5, p. 557, Proposition 3).

Recall (IV, §1, No. 1, p. 2) that A[X] denotes the $\mathbf{Z}$-module $A\otimes_{\mathbf{Z}}\mathbf{Z}[X]$ of polynomials in one variable with coefficients in A. We endow it with its natural structure of a left A-module. The family $(X^n)_{n\in\mathbf{N}}$ is a basis for A[X] over A. We identify A with its image under the mapping $a\mapsto a\otimes 1$. **Proposition 7.** — Let A$,\sigma ,d$ be as above. There exists a unique ring structure on the group A[X] with the following properties:

a) The addition in this ring is the usual addition of A[X].

b) The multiplication in this ring extends that of A.

c) The product in this ring of a sequence $(a,X, . . . ,X)$, consisting of an element $a$ of A followed by $n$ terms equal to X, is the polynomial $aX^n$.

d) In this ring, we have $Xa=\sigma (a)X +d(a)$ for every $a\in A$.

Let E be the endomorphism ring of the additive group A[X]. The mapping that sends $a\in A$ to the homothety $a_M$ of the left A-module M = A[X] is a ring homomorphism from A to E. Consider the elements $u,\sigma_M$, and $d_M$ of E defined by $u(\sum b_nX^n) =\sum b_nX^{n+1},\sigma_M(\sum b_nX^n) =\sum\sigma (b_n)X^n$, $d_M(\sum b_nX^n) =\sum d(b_n)X^n$. For every $a\in A$, we have

$$
u a_M=a_Mu ,\sigma_Ma_M=\sigma (a)_M\sigma_M,d_Ma_M=\sigma (a)_Md_M+ (d(a)_M) \tag{2}
$$

Set

$$
X_M=\sigma_Mu+d_M \tag{3}
$$

It follows from (2) that for every $a\in A$, we have

$$
X_Ma_M=\sigma (a)_MX_M+ (d(a)_M) \tag{4}
$$

Consider the mapping $\varphi : A[X]\rightarrow E$ defined by

$$
\varphi \sum a_nX^n=\sum(a_n)_M(X_M)^n \tag{5}
$$

This is a group homomorphism. An induction argument shows that we have $(X_M)^n(1) = X^n$ for every $n\in \mathbf{N}$. We therefore have $\varphi (P)(1) = P$ for every $P\in A[X]$, which proves that the homomorphism $\varphi$ is injective. We denote its image by B. The set B is a subgroup of E; it contains 1, and it is stable under left multiplication by $a_M$ for $a\in A$ and by $X_M$ (see (4)). It is therefore a subring of E. The unique ring structure on A[X] derived from that on B by transfer of structure via $\varphi$ has the properties of Proposition 7, where property d) results from relation (4).

If A[X] is endowed with a ring structure that has the properties of Proposition 7, then the left homothety $\boldsymbol{\gamma }_X$ of this ring (I, §8, No. 1, p. 97) necessarily sends $bX^n$ to $\sigma (b)X^{n+1}+d(b)X^n$ for $b\in A$ and $n\in \mathbf{N}$, hence is equal to $X_M$. The homothety $\boldsymbol{\gamma }_a$ is necessarily equal to $a_M$ for every $a\in A$. Consequently, we have $\boldsymbol{\gamma }_P=\varphi (P)$ for every $P\in A[X]$; the uniqueness in Proposition 7 follows.

The set A[X], endowed with the unique ring structure with the properties of Proposition 7, is denoted by $A[X]_{\sigma ,d}$ and called the polynomial ring in X with coefficients in A, relative to $\sigma$ and $d$. We simply denote it by $A[X]_{\sigma}$ when $d$ is the zero mapping and by A[X] when, moreover, $\sigma$ is the identity mapping on A. This notation is compatible with that introduced in IV, §1, No. 1, p. 1 for a commutative ring A.

#### Remark {#alg-viii-s1-n4-rem-1 .statement tag=000T}

The ring $A[X]_{\sigma ,d}$ has the following universal property: given a ring $A'$, a ring homomorphism $f: A\rightarrow A'$, and an element $x$ of $A'$ such that $xf(a) =f(\sigma (a))x+f(d(a))$ for every $a\in A$, there exists a unique ring homomorphism $g: A[X]_{\sigma ,d}\rightarrow A'$ that extends $f$ and maps X onto $x$.

The uniqueness is clear. Let us therefore show that the mapping $g: A[X]_{\sigma ,d}\rightarrow A'$ defined by $g(\sum a_nX^n) =\sum f(a_n)x^n$ has the required properties. It extends $f$, maps X onto $x$, and is a group homomorphism. We have $g(1) = 1$. For $a\in A$ and $Q =\sum a_nX^n$ in $A[X]_{\sigma ,d}$, we have

$$
g(aQ) =g\sum aa_nX^n=\sum f(aa_n)x^n=f(a)\sum f(a_n)x_n=g(a)g(Q)
$$

as well as

$g$(XQ) $=g\sum\sigma (a_n)X^{n+1}+d(a_n)X^n$

$$
=\sum(f(\sigma (a_n))x^{n+1}+f(d(a_n))x^n) =x\sum f(a_n)x^n=g(X)g(Q)
$$

It follows that we have $g(P)g(Q) =g$(PQ) for $P,Q$ in $A[X]_{\sigma ,d}$ and therefore that $g$ is a ring homomorphism.

#### Theorem 2 {#alg-viii-s1-thm-2 .statement tag=000U}

Let A be a left Noetherian ring, and let $\sigma$ be an automorphism of A and $d$ an endomorphism of the additive group of A satisfying relation (1). The ring $A[X]_{\sigma ,d}$ is left Noetherian.

Set $B = A[X]_{\sigma ,d}$. For any integer $n\geqslant 0$, we denote by $B_n$ the set of elements of B of the form $a_0+a_1X +\cdots +a_nX^n$. It is a left A-submodule of B. The mapping $\varphi_n: B_n\rightarrow A_s$ defined by $\varphi_n(a_0+a_1X +\cdots +a_nX^n) =a_n$ is A-linear.

Let $\mathfrak{b}$ be a left ideal of B. For every integer $n\geqslant 0$, the set $\mathfrak{a}_n=\varphi_n(\mathfrak{b}\cap B_n)$ is a left ideal of A. Since we have $Xa=\sigma (a)X +d(a)$ for every $a\in A$, we have

(6) $\varphi_{n+1}$(XQ) $=\sigma (\varphi_n(Q))$

for every $Q\in B_n$ and therefore $\sigma (\mathfrak{a}_n)\subset \mathfrak{a}_{n+1}$. Consequently, the sequence $\mathfrak{a}'_n=\sigma^{-n}(\mathfrak{a}_n)$ of ideals of A is increasing. Since the ring A is left Noetherian, there exists an integer $m\geqslant 0$ such that we have $\mathfrak{a}'_n=\mathfrak{a}'_{n+1}$ for $n\geqslant m$. Since $\sigma$ is surjective, we have the relation

$$
\sigma (\mathfrak{a}_n) =\mathfrak{a}_{n+1} \tag{7}
$$

for every integer $n\geqslant m$.

Let $\mathfrak{c}$ be the left ideal of B generated by $\mathfrak{b}\cap B_m$. Since the left A-module $B_m$ is finitely generated and the ring A is left Noetherian, the left A-module $\mathfrak{b}\cap B_m$ is finitely generated (VIII, p. 7, Proposition 4 a)). The left ideal $\mathfrak{c}$ is therefore generated by a finite subset of B. It is clear that it is contained in $\mathfrak{b}$. Let us prove that it is equal to $\mathfrak{b}$ by proving by induction that for every integer $n\geqslant 0$, we have

$$
\mathfrak{b}\cap B_n\subset \mathfrak{c} \tag{8}
$$

Relation (8) is true by construction for $n\leqslant m$. From now on, we assume that $n$ is an integer $\geqslant m$ such that $\mathfrak{b}\cap B_n\subset \mathfrak{c}$. Let P be an element of $\mathfrak{b}\cap B_{n+1}$. Then $\varphi_{n+1}(P)$ belongs to $\mathfrak{a}_{n+1}=\sigma (\mathfrak{a}_n)$, and there consequently exists an element Q of $\mathfrak{b}\cap B_n$ such that $\varphi_{n+1}(P) =\sigma (\varphi_n(Q))$. Set $R = P-$ XQ. Because of relation (6), we have $\varphi_{n+1}(R) = 0$, that is, $R\in B_n$. Since P and Q belong to the left ideal $\mathfrak{b}$ of B, the same is true for R; hence, R and Q belong to $\mathfrak{b}\cap B_n$, which is contained in the ideal $\mathfrak{c}$ by the induction hypothesis. Consequently, P belongs to $\mathfrak{c}$. This proves that we have $\mathfrak{b}\cap B_{n+1}\subset \mathfrak{c}$.

It follows that $\mathfrak{b}$ is equal to $\mathfrak{c}$; it is therefore a finitely generated ideal of B. This proves that the ring B is left Noetherian.

If the endomorphism $\sigma$ of the ring A is not an automorphism, then the ring $A[X]_{\sigma ,d}$ is not necessarily left Noetherian, even when A is a Noetherian commutative ring (VIII, p. 22, Exercise 26).

Corollary 1 (Hilbert). — Let A be a Noetherian commutative ring. For every integer $n\geqslant 0$, the polynomial algebra $A[X_1, . . . ,X_n]$ is a Noetherian ring.

This follows by induction from Theorem 2, taking Proposition 8 of III, §2, No. 9, p. 453, into account.

#### Corollary 2 {#alg-viii-s1-thm-2-cor-2 .statement tag=000V}

Let A be a Noetherian commutative ring. A commutative A-algebra generated by finitely many elements is a Noetherian ring.

Such an algebra is isomorphic to an algebra of the form $A[X_1, . . . ,X_n]/\mathfrak{a}$, where $n\geqslant 0$ and $\mathfrak{a}$ is an ideal of $A[X_1, . . . ,X_n]$. We then apply Corollary 1 and Proposition 5 of VIII, p. 7.

#### Corollary 3 {#alg-viii-s1-thm-2-cor-3 .statement tag=000W}

Every commutative ring is the union of a right directed family of Noetherian subrings.

Indeed, let A be a commutative ring. The subrings of A generated (as $\mathbf{Z}$-algebras) by finitely many elements are Noetherian by Corollary 2. They form a right directed family of subrings of A, with union A.

### Exercises {#alg-viii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
