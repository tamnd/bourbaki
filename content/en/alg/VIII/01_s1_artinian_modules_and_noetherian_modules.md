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
content_sha256: 2ca9c31a3787173eafc7e038fc5b4b835dd21d5ed994e6b8b9a822d2f614f151
---

## § 1. ARTINIAN MODULES AND NOETHERIAN MODULES

### 1. Artinian Modules and Noetherian Modules

#### Definition 1 {#alg-viii-s1-def-1 .statement}

Let A be a ring. We call an A-module M Artinian (resp. Noetherian) if it satisfies the following equivalent conditions:

(i) Every nonempty set of submodules of M, ordered by inclusion, has a minimal (resp. maximal) element.

(ii) Every decreasing (resp. increasing) sequence of submodules of M is stationary.

The equivalence of conditions (i) and (ii) follows from Set Theory, III, §6, No. 5, p. 190, Proposition 6.

An A-module M is Artinian (resp. Noetherian) if and only if M, viewed as a module over the ring of homotheties $A_M$, is Artinian (resp. Noetherian).

Let M be an Artinian (resp. Noetherian) A-module. Every nonempty set of submodules of M, ordered by inclusion, that is left directed (resp. right directed) has a least element (resp. a greatest element) (Set Theory, III, §1, No. 10, p. 145, Proposition 10).

Let M be an Artinian (resp. Noetherian) A-module and $(M_i)_{i\in I}$ a family of submodules of M. The intersections (resp. sums) of finite subfamilies of the family $(M_i)_{i\in I}$ form a nonempty left (resp. right) directed set of submodules of M. Therefore, there exists a finite subset J of I such that $\bigcap_{i\in I}M_i=\bigcap_{i\in J}M_i$ (resp. $\sum_{i\in I}M_i=\sum_{i\in J}M_i)$.

#### Example 1 {#alg-viii-s1-n1-exa-1 .statement}

A finite-dimensional vector space over a field is Artinian and Noetherian.

#### Example 2 {#alg-viii-s1-n1-exa-2 .statement}

Let M be an A-module. If there exists an infinite family $(M_i)_{i\in I}$ of nonzero submodules of M whose sum is direct, then M is neither Artinian nor Noetherian: indeed, for every strictly decreasing (resp. strictly increasing) infinite sequence $(J_n)$ of subsets of I, the infinite sequence $(\sum_{i\in J_n}M_i)$ of submodules of M is strictly decreasing (resp. strictly increasing). In particular, an infinite-dimensional vector space over a field is neither Artinian nor Noetherian.

#### Example 3 {#alg-viii-s1-n1-exa-3 .statement}

We will see further on that the $\mathbf{Z}$-module $\mathbf{Z}$ is Noetherian but not

Artinian (VIII, p. 5, Example 3$).*$

#### Example 4 {#alg-viii-s1-n1-exa-4 .statement}

Let $p$ be a prime number and $M_p$ the $p$-primary component of the torsion $\mathbf{Z}$-module $\mathbf{Q}/\mathbf{Z}$ (VII, §2, No. 2, p. 7). Every submodule of $M_p$ is equal to either $M_p$ or $p^{-n}\mathbf{Z}/\mathbf{Z}$ for an integer $n\in \mathbf{N}$ (VII, §2, p. 54, Exercise 3). Consequently, $M_p$ is an Artinian but not Noetherian $\mathbf{Z}$-module.

#### Proposition 1 {#alg-viii-s1-prop-1 .statement}

An A-module M has finite length (II, §1, No. 10, p. 212) if and only if it is both Artinian and Noetherian.

Suppose that M has finite length $d$. Then every strictly increasing or strictly decreasing sequence of submodules of M has at most $d+ 1$ terms (I, §4, No. 7, p. 44). Consequently, M is Artinian and Noetherian.

Conversely, suppose that M is Artinian and Noetherian. Let $\mathscr{S}$ be the set of submodules of M of finite length. The zero submodule is an element of $\mathscr{S}$, and since M is Noetherian, $\mathscr{S}$ has a maximal element N. Let us give a proof by contradiction and suppose that $M\not= N$. The set of submodules of M distinct from N and containing N then has a minimal element P because M is Artinian. The module $P/N$ has length 1, and since N is a module of finite length, the same holds for P (II, §1, No. 10, p. 212, Proposition 16). This contradicts the definition of N.

#### Proposition 2 {#alg-viii-s1-prop-2 .statement}

An A-module M is Noetherian if and only if every submodule of M is finitely generated.

Begin by assuming that every submodule of M is finitely generated. Let $(P_n)_{n\in\mathbf{N}}$ be an increasing sequence of submodules of M, and let P be its union. This is a submodule of M. By assumption, there exists a finite subset F of M generating the module P; let $n\in \mathbf{N}$ be an integer such that $F\subset P_n$. We then have $P_n= P$, and the sequence $(P_n)_{n\in\mathbf{N}}$ is stationary. This proves that the module M is Noetherian.

The converse is a consequence of the following more precise statement.

#### Lemma 1 {#alg-viii-s1-lem-1 .statement}

Let M be a Noetherian A-module and E a subset of M. There exists a finite subset F of E generating the same submodule as E.

Indeed, by VIII, p. 2, there exists a finite subset F of E such that $\sum_{x\in E}Ax=\sum_{x\in F}Ax$.

#### Proposition 3 {#alg-viii-s1-prop-3 .statement}

Let M be an A-module and N a submodule of M. Then M is Artinian (resp. Noetherian) if and only if N and $M/N$ are.

We will give the proof in the case of Artinian modules; the case of Noetherian modules is analogous.

Suppose that M is Artinian. Since every submodule of N is a submodule of M, the module N is Artinian. Let $(P_n)_{n\in\mathbf{N}}$ be a decreasing sequence of submodules of $M/N$. There exists a decreasing sequence $(Q_n)_{n\in\mathbf{N}}$ of submodules of M containing N such that $P_n= Q_n/N$ for every $n\in \mathbf{N}$ (I, §4, No. 6, p. 41, Theorem 4). Since M is Artinian, the sequence $(Q_n)$ is stationary, hence so is the sequence $(P_n)$. Consequently, the module $M/N$ is Artinian.

Conversely, suppose that the modules N and $M/N$ are Artinian, and consider a decreasing sequence $(P_n)$ of submodules of M. The sequence $P'_n= N\cap P_n$ of submodules of N is stationary. Likewise, the sequence $P''_n= (N + P_n)/N$ of submodules of $M/N$ is stationary. Hence, there exists an integer $m\in \mathbf{N}$ such that we have $P'_n= P'_m$ and $P''_n= P''_m$ for every integer $n\geqslant m$. The sequence $(P_n)$ is then stationary by the following lemma. **Lemma 2.** — Let M be an A-module and N, P, and Q submodules of M. Suppose that we have $P\subset Q$, $N\cap P = N\cap Q$, and N + P = N + Q. We then have P = Q.

Let $x$ be an element of Q. It belongs to N + P; hence, there exists an element $y$ of P such that $x-y\in N$. Since Q contains P, the difference $x-y$ belongs to $N\cap Q$ and therefore to P. Consequently, $x$ belongs to P.

#### Corollary {#alg-viii-s1-n1-cor-1 .statement}

Let M be an A-module and $(M_i)_{i\in I}$ a finite family of submodules of M.

a) If the modules $M_i$ are Artinian (resp. Noetherian), then so is their sum $\sum_{i\in I}M_i$.

b) If the modules $M/M_i$ are Artinian (resp. Noetherian), then so is the module $M/\bigcap_{i\in I}M_i$.

By induction, it suffices to treat the case when $I =\{1,2\}$. The module $M_2/(M_1\cap M_2)$, quotient of $M_2$, is isomorphic to the submodule $(M_1+M_2)/M_1$ of $M/M_1$ (I, §4, No. 6, p. 41, Theorem 4).

In part a), we assume that $M_1$ and $(M_1+ M_2)/M_1$ are Artinian (resp. Noetherian); the same then holds for $M_1+ M_2$ (Proposition 3).

In part b), we assume that $M/M_2$ and $M_2/(M_1\cap M_2)$ are Artinian (resp. Noetherian); the same then holds for $M/(M_1\cap M_2)$ (loc. cit.).

#### Example 5 {#alg-viii-s1-n1-exa-5 .statement}

Let $(M_i)_{i\in I}$ be a finite family of A-modules. If the modules $M_i$ are Artinian (resp. Noetherian), then so is their direct sum $\bigoplus_{i\in I}M_i$.

#### Remark {#alg-viii-s1-n1-rem-1 .statement}

The definitions and results of this subsection extend to arbitrary abelian groups with operators by replacing the submodules in the statements with stable subgroups.

### 2. Artinian Rings and Noetherian Rings

#### Definition 2 {#alg-viii-s1-def-2 .statement}

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

#### Example 1 {#alg-viii-s1-n2-exa-1 .statement}

A field is a ring that is both left and right Artinian and Noetherian.

#### Example 2 {#alg-viii-s1-n2-exa-2 .statement}

Let A be a ring and D a subring of A. Suppose that D is a field and that A is a finite-dimensional left vector space over D. Then the ring A is left Artinian and left Noetherian because every left ideal of A is a D-vector subspace of A. In particular, a finite-dimensional algebra over a commutative field is a ring that is both left and right Artinian and Noetherian.

#### Example 3 {#alg-viii-s1-n2-exa-3 .statement}

A principal ideal domain (VII, §1, No. 1, p. 1, Definition 1) is Noetherian. An integral domain A that is not a field is not an Artinian ring: for every nonzero noninvertible element $a$ of A, the sequence of ideals $a^nA$ (for $n\in \mathbf{N})$ is strictly decreasing. In particular, the ring $\mathbf{Z}$ of integers is Noetherian but not Artinian.

#### Example 4 {#alg-viii-s1-n2-exa-4 .statement}

Let M be an A-module that is the direct sum of an infinite family $(M_i)_{i\in I}$ of nonzero submodules. Let E be the endomorphism ring of M. For every $i\in I$, let $\mathfrak{a}_i$ (resp. $\mathfrak{b}_i)$ be the set of elements of E with kernel containing $\sum_{j\not=i}M_j$ (resp. with image contained in $M_i)$. Then $(\mathfrak{a}_i)$ is an infinite family of nonzero left ideals of E whose sum is direct, and $(\mathfrak{b}_i)$ is an infinite family of nonzero right ideals of E whose sum is direct. Consequently, the ring E is neither left nor right Artinian (resp. Noetherian) (VIII, p. 2, Example 2). In particular, the endomorphism ring of an infinite-dimensional vector space is neither left nor right Artinian (resp. Noetherian). **Theorem 1.** — Let A be a left Artinian ring. The A-module $A_s$ has finite length.

We will use the following lemma in the proof.

#### Lemma 3 {#alg-viii-s1-lem-3 .statement}

Let A be a ring and $n$ a natural number. An Artinian A-module M that is the sum of a family of submodules of length $\leqslant n$ has finite length.

We use induction on $n$. First, suppose $n= 1$. If M were not of finite length, then we could construct a sequence $(M_m)_{m\in\mathbf{N}}$ of submodules of M of length 1 with $M_m\not\subset \sum_{i<m}M_i$ for every $m\in \mathbf{N}$. We would then have $M_m\cap \sum_{i<m}M_i= 0$ for every $m$, and the sum of the family $(M_m)_{m\in\mathbf{N}}$ would be direct. However, this contradicts the fact that the A-module M is Artinian (VIII, p. 2, Example 2).

Now, suppose $n\geqslant 2$. Let $(M_i)_{i\in I}$ be a family of submodules of M of length $\leqslant n$ with sum M. For every $i\in I$, choose a submodule $M'_i$ of $M_i$ of length $\leqslant n-1$ such that $M_i/M'_i$ has length $\leqslant 1$. Set $M'=\sum M'_i$, and denote the image of $M_i$ in $M''= M/M'$ by $M''_i$. The modules $M''_i$ are of length $\leqslant 1$, and their sum is $M''$. The modules $M'$ and $M''$ are Artinian (VIII, p. 3, Proposition 3); by the induction hypothesis, they are of finite length. Hence, M has finite length (II, §1, No. 10, p. 212, Proposition 16).

Let us now prove Theorem 1. Let $\mathscr{S}$ denote the set of left ideals $\mathfrak{a}$ of A such that the module $A_s/\mathfrak{a}$ has finite length. Let $(\mathfrak{a}_i)_{i\in I}$ be a finite family of elements of $\mathscr{S}$. By Proposition 1 of VIII, p. 2, the A-module $A_s/\mathfrak{a}_i$ is Artinian and Noetherian for every $i\in I$. Consequently, $A_s/\bigcap_{i\in I}\mathfrak{a}_i$ is Artinian and Noetherian (VIII, p. 4, Corollary of Proposition 3), hence of finite length (VIII, p. 2, Proposition 1). This proves that $\mathscr{S}$ is a left directed set for the inclusion. Since the ring A is left Artinian, the set $\mathscr{S}$ has a least element $\mathfrak{b}$. We denote the length of the A-module $A_s/\mathfrak{b}$ by $n$.

Let $x$ be an element of $A_s$ and $\mathfrak{a}$ its annihilator (II, §1, No. 12, p. 219). The A-module $Ax$ is isomorphic to $A_s/\mathfrak{a}$. If $Ax$ has finite length, then $\mathfrak{a}$ belongs to $\mathscr{S}$, so $\mathfrak{a}$ contains $\mathfrak{b}$ and $Ax$ has length $\leqslant n$. Thus, every monogenous left ideal of A of finite length has length $\leqslant n$. Let $\mathfrak{c}$ be the sum of these ideals; this is a left ideal of A, of finite length by Lemma 3. Every left ideal of A of finite length is a sum of monogenous left ideals of finite length and is therefore contained in $\mathfrak{c}$. Hence, $\mathfrak{c}$ is the largest left ideal of A of finite length.

If $\mathfrak{c}$ were distinct from A, then the set of left ideals of A containing $\mathfrak{c}$ and distinct from $\mathfrak{c}$ would have a minimal element $\mathfrak{c}'$. The A-module $\mathfrak{c}'/\mathfrak{c}$ would then have length 1, and $\mathfrak{c}'$ would have finite length, which contradicts the fact that $\mathfrak{c}$ is maximal. We therefore have $\mathfrak{c}= A$; the A-module $A_s$ has finite length.

#### Corollary {#alg-viii-s1-n2-cor-1 .statement}

Every left Artinian ring is left Noetherian.

Let A be a left Artinian ring. By Theorem 1, the A-module $A_s$ has finite length. We then apply Proposition 1 of VIII, p. 2.

Let A be a left (resp. right) Artinian ring; the length of the A-module $A_s$ (resp. $A_d)$ (I, §4, No. 7, p. 44) is called the left (resp. right) length of the ring A. When A is a commutative Artinian ring, these two lengths coincide and are simply called the length of A. When A is left and right Artinian but is not commutative, the left and right lengths of A are not necessarily equal (VIII, p. 14, Exercise 3).

#### Example 5 {#alg-viii-s1-n2-exa-5 .statement}

The left and right lengths of a field are equal to 1.

#### Proposition 4 {#alg-viii-s1-prop-4 .statement}

a) Let A be a left Noetherian ring and M a finitely generated left A-module. The module M is Noetherian, and every submodule of M is finitely generated.

b) Let A be a left Artinian ring and M a left A-module. The following properties are equivalent: the module M is finitely generated; the module M is Artinian; the module M has finite length; the module M is Noetherian.

Let us prove a). Every monogenous submodule of M is isomorphic to a quotient of $A_s$, hence is Noetherian by Proposition 3 of VIII, p. 3. The module M is a finite sum of such submodules; it is therefore Noetherian by the corollary (VIII, p. 4) of Proposition 3. Every submodule of M is then finitely generated (VIII, p. 3, Proposition 2)

Now, suppose that the ring A is left Artinian. We see, as in the previous section, that if the A-module M is finitely generated, then it is Artinian. If it is Artinian, then it has finite length: indeed, its monogenous submodules are isomorphic to quotients of $A_s$ and are therefore of finite length less than that of $A_s$, and the assertion follows from Lemma 3. Every module of finite length is Noetherian, and every Noetherian module is finitely generated. This proves b).

#### Proposition 5 {#alg-viii-s1-prop-5 .statement}

a) Let A be a left Artinian (resp. left Noetherian) ring, and let $\varphi : A\rightarrow B$ be a ring homomorphism that makes B into a finitely generated left A-module. The ring B is left Artinian (resp. left Noetherian).

b) Let A be a left Artinian (resp. left Noetherian) ring, and let $\mathfrak{a}$ be a two-sided ideal of A; the ring $A/\mathfrak{a}$ is left Artinian (resp. left Noetherian).

c) Let $(A_i)_{i\in I}$ be a family of left Artinian (resp. left Noetherian) rings. The ring $\prod_{i\in I}A_i$ is left Artinian (resp. left Noetherian).

We will treat the case of Artinian rings; the case of Noetherian rings is analogous.

Let us prove a). By Proposition 4, the ring $B_s$ is an Artinian left A-module and a fortiori an Artinian left B-module.

Assertion b) follows from assertion a) applied to the canonical homomorphism from A to $A/\mathfrak{a}$.

Let us prove c). Set $A =\prod_{i\in I}A_i$. By assumption, $(A_i)_s$ is an Artinian left $A_i$-module and a fortiori an Artinian left A-module. By Example 5 of VIII, p. 4, the A-module $A_s$ is Artinian.

#### Corollary {#alg-viii-s1-n2-cor-2 .statement}

The prime ideals of an Artinian commutative ring are its maximal ideals.

In any commutative ring, a maximal ideal is prime. Let A be an Artinian commutative ring. Let $\mathfrak{p}$ be a prime ideal of A. The ring $A/\mathfrak{p}$ is an integral domain and is Artinian (Proposition 5), hence is a field (VIII, p. 5, Example 3). Consequently, the ideal $\mathfrak{p}$ is maximal.

The polynomial ring $\mathbf{Q}[(X_n)_{n\in\mathbf{N}}]$ is an integral domain; it is not Noetherian (or Artinian) (VIII, p. 15, Exercise 9). It is a subring of its field of fractions, which is an Artinian (and Noetherian) ring.

### 3. Countermodule

#### Definition 3 {#alg-viii-s1-def-3 .statement}

Let A be a ring, M an A-module, and E = End$_A(M)$ the endomorphism ring of M. The countermodule of M is the left E-module with the same underlying additive group as M and external law $(c, x)\mapsto c(x)$.

Let Z be the center of the ring A. For every $a\in Z$, the homothety $a_M$ belongs to E. Consequently, E is canonically endowed with the structure of a Z-algebra. In particular, if M is a finitely generated Z-module, then the countermodule of M is finitely generated.

#### Lemma 4 {#alg-viii-s1-lem-4 .statement}

Let M be a left A-module with finitely generated countermodule. There exist a natural number $m$ and an injective $A_M$-linear mapping from $(A_M)_s$ to $M^m$.

Set E = End$_A(M)$. Let $(x_1, . . . , x_m)$ be a finite generating family of the E-module M. The mapping $\varphi :a\mapsto (ax_1, . . . , ax_m)$ from $(A_M)_s$ to $M^m$ is $A_M$-linear. Let $a$ be an element of $A_M$ such that $\varphi (a) = 0$. The set of elements $x$ of M such that $ax= 0$ is an E-submodule of M containing $x_1, . . . , x_m$ and is therefore equal to M, which implies $a= 0$.

#### Proposition 6 {#alg-viii-s1-prop-6 .statement}

Let M be an Artinian (resp. Noetherian) left A-module with finitely generated countermodule. The ring of homotheties $A_M$ of M is left Artinian (resp. left Noetherian).

This follows from Lemma 4 and Proposition 3 of VIII, p. 3.

#### Corollary {#alg-viii-s1-n3-cor-1 .statement}

Let A be a commutative ring.

a) Let M be a Noetherian A-module. The ring $A_M$ is Noetherian.

b) Let M be an A-module of finite length. The ring $A_M$ is Artinian.

Let M be an A-module. Under the assumptions of a) or b), the A-module M is finitely generated. Since A is commutative, $A_M$ is contained in the ring End$_A$(M), so that the countermodule of M is finitely generated. It then suffices to apply Proposition 6.

#### Remark {#alg-viii-s1-n3-rem-1 .statement}

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

#### Remark {#alg-viii-s1-n4-rem-1 .statement}

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

#### Theorem 2 {#alg-viii-s1-thm-2 .statement}

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

#### Corollary 2 {#alg-viii-s1-thm-2-cor-2 .statement}

Let A be a Noetherian commutative ring. A commutative A-algebra generated by finitely many elements is a Noetherian ring.

Such an algebra is isomorphic to an algebra of the form $A[X_1, . . . ,X_n]/\mathfrak{a}$, where $n\geqslant 0$ and $\mathfrak{a}$ is an ideal of $A[X_1, . . . ,X_n]$. We then apply Corollary 1 and Proposition 5 of VIII, p. 7.

#### Corollary 3 {#alg-viii-s1-thm-2-cor-3 .statement}

Every commutative ring is the union of a right directed family of Noetherian subrings.

Indeed, let A be a commutative ring. The subrings of A generated (as $\mathbf{Z}$-algebras) by finitely many elements are Noetherian by Corollary 2. They form a right directed family of subrings of A, with union A.

### Exercises {#alg-viii-s1-exercises}

1) Let A be a principal ideal domain that is not a field and P a system of representatives consisting of irreducible elements of A. An A-module M is Artinian if and only if it is a torsion module and there exists a finite subset S of P such that the following two conditions are satisfied:

(i) For every $\pi \in P$ S, the $\pi$-primary component $M_{\pi}$ of M (VII, §2, No. 2, p. 8) is reduced to 0.

(ii) For every $\pi \in S$, the set of elements of M annihilated by $\pi$, viewed as a vector space over the field $A/\pi A$, is finite-dimensional.

2) Let A be a ring, M an A-module of finite length $n$, and R a set of nilpotent endomorphisms of M that is stable under composition. a) If $n= 1$, then every element of R is zero. If $n >1$, prove that there exists a submodule N of M, distinct from 0 and M, that is stable under all elements of R. (We may assume that R has an element $s\not= 0$; choose one such that $s(M)$ has mimimum length, and prove that we have $srs= 0$ for every $r\in R$. Deduce that we can take $N =s(M)$ if $Rs=\{0\}$ and $N =\sum_{r\in R}r(s(M))$ if $Rs\not=\{0\}.)$[^1] b) Deduce from a) that there exists a Jordan–Hölder series $(M_i)_{0\leqslant i\leqslant n}$ of M such that we have $r(M_i)\subset M_{i+1}$ for all $r\in R$ and $0\leqslant i\leqslant n-1$. Deduce that we have $r_1\cdots r_n= 0$ for every sequence $(r_i)_{1\leqslant i\leqslant n}$ of $n$ elements of R.

3) a) Give an example of a commutative field K and an isomorphism $\varphi$ from K to one of its subfield $K'$ such that K is finite-dimensional over $K'$. On the additive group $A = K\times K$, we define a ring structure by setting $(x, y)(x', y') = (xx', xy'+y\varphi (x'))$ (II, §1, p. 382, Exercise 7). The only left ideals of A are $\{(0,0)\},\{0\} \times K$, and A, but for every $K'$-linear subspace E of $K,\{0\} \times E$ is a right ideal of A. Deduce that A is left Artinian and left Noetherian but neither right Artinian nor right Noetherian. b) Give an example of a module of finite length whose endomorphism ring is neither left Artinian nor left Noetherian. c) Using the same method as in a), give an example of a left and right Artinian ring whose left length is different from its right length.

4) Let $\rho : A\rightarrow B$ be a ring homomorphism. a) If, as a right A-module, B is free and nonzero, and if the ring B is left Artinian (resp. left Noetherian), then the ring A is left Artinian (resp. left Noetherian). b) Give an example where A is a commutative field, where B, viewed as a right vector space over A, is finite-dimensional, and where B is neither left Artinian nor left Noetherian (use Exercise 3).

5) Let $n$ be an integer $\geqslant 1$. A ring A is left Artinian (resp. left Noetherian) if and only if the matrix ring $\mathbf{M}_n(A)$ is. If A is left Artinian, then the left length of $\mathbf{M}_n(A)$ is equal to $n$ times that of A.

6) Let A be a ring and $e$ an idempotent in A. a) Let $\mathfrak{a}_1$ be a left ideal of the ring $eAe$ and $\mathfrak{a}$ the left ideal of A generated by $\mathfrak{a}_1$. We have $\mathfrak{a}_1=e\mathfrak{a}e=\mathfrak{a}\cap eAe$. b) For every left ideal $\mathfrak{a}$ of A, we have $\mathfrak{a}\cap eAe\subset e\mathfrak{a}e$; give an example where this is a strict inclusion (take a matrix ring for A). c) We have $\mathfrak{a}\cap eAe=e\mathfrak{a}e$ for every two-sided ideal $\mathfrak{a}$ of A. d) If the ring A is left Artinian (resp. left Noetherian), then so are the rings $eAe$ and $(1-e)A(1-e)$. e) Give an example where $eAe$ and $(1-e)A(1-e)$ are commutative fields and where A admits infinite strictly increasing sequences and infinite strictly decreasing sequences of two-sided ideals. (Choose an infinite-dimensional vector space V over a commutative field K, endow the additive group $A = K\times V\times K$ with the ring structure defined by $(\lambda , x, µ)(\lambda ', x', µ') = (\lambda \lambda ', \lambda x'+µ'x, µµ')$, and set $e= (1,0,0).)$

7) a) Let A be a ring and $\mathscr{I}$ the set of left ideals of A of the form $Ae$, where $e$ is an idempotent in A. Prove that the following properties are equivalent:

(i) Every nonempty subset of $\mathscr{I}$ has a minimal element.

(ii) Every nonempty subset of $\mathscr{I}$ has a maximal element.

(iii) There is no infinite family of nonzero ideals belonging to $\mathscr{I}$ whose sum is direct.

(iv) There is no infinite family $(e_i)$ of nonzero idempotents in A such that $e_ie_j= 0$ for $i\not=j$. b) Give an example of a ring A in which every nonempty set of monogenous left ideals has a maximal element and a minimal element (so that the equivalent conditions of a) are satisfied) even though A is neither left Artinian nor left Noetherian (use Exercise 3). c) Let M be a module. If every nonempty set of finitely generated submodules of M has a maximal element, then M is Noetherian. d) Give an example of a non-Artinian module in which every nonempty set of finitely generated submodules has a minimal element.

8) Let A be a ring, B and D two subrings of A. Prove that if D is a field and the ring B is left Artinian, $B\cap D$ is a field.

9) Let A be a nonzero commutative ring, and let I be an infinite set. The rings $A[(X_i)_{i\in I}]$ and $A[[(X_i)_{i\in I}]]$ are neither Artinian nor Noetherian.

10) Let A be a ring and $\mathfrak{a}$ and $\mathfrak{b}$ two-sided ideals of A. If the rings $A/\mathfrak{a}$ and $A/\mathfrak{b}$ are left Artinian (resp. left Noetherian), then so is the ring $A/\mathfrak{a}\cap \mathfrak{b}$; by contrast, the ring $A/\mathfrak{a}\mathfrak{b}$ is not necessarily left Artinian (resp. left Noetherian).

11) Let $A,B$ be rings, M a finitely generated left A-module, P a finitely generated right A-module, and N an $(A$, B)-bimodule. If the right B-module N is Artinian (resp. Noetherian), then so are the right B-modules Hom$_A(M,N)$ and $P\otimes_AN$.

12) Let K be a commutative field. Denote by $(e_n)_{n\in\mathbf{N}}$ the canonical basis of the vector space $V = K^{(\mathbf{N})}$. We define the sequence $(u_n)_{n\in\mathbf{N}}$ of endomorphisms of V by setting

$u_0(e_0) = 0u_0(e_1) = 0u_0(e_{n+1}) =e_n$ for $n\geqslant 1$

$u_m(e_0) =e_mu_m(e_n) = 0$ for $m\geqslant 1$ and $n\geqslant 1$.

Let A be the unital K-subalgebra of End$_K(V)$ generated by the sequence $(u_n)_{n\in\mathbf{N}}$. Prove that the left A-module V is Artinian, finitely generated (and even monogenous), but not Noetherian.

13) a) Let $\rho : A\rightarrow B$ be a ring homomorphism. Assume that A is left Noetherian and that there exists a finite subset S of B whose elements commute with one another and with the elements of $\rho$(A), such that the ring B is generated by $\rho (A)$ and S. Then B is left Noetherian. b) Let A be a nonzero commutative ring. Give an example of an associative unital A-algebra, generated by finitely many elements, that is a neither left nor right Noetherian ring (consider the free associative algebra Libas$_A(I)$ (III, §2, No. 7, p. 449, Definition 2), where I is a set of cardinality $\geqslant 2)$.

14) Let V be a vector space of countable infinite dimension over a field K. The set $\mathscr{I}$ of endomorphisms of V of finite rank is a two-sided ideal of the ring B = End$_K(V)$. Prove that the only two-sided ideals of the ring $A = B/\mathscr{I}$ are $\{0\}$ and A, but that A is neither left nor right Noetherian.

$\P 15)$ Let A be a commutative ring and M a finitely generated A-module. a) Suppose that for every increasing sequence $(\mathfrak{a}_n)_{n\in\mathbf{N}}$ of ideals of A, the sequence $(\mathfrak{a}_nM)_{n\in\mathbf{N}}$ is stationary. Prove that the A-module M is Noetherian. (Reduce to the case when the A-module M is faithful and when for every ideal $\mathfrak{a}\not= 0$ of A, the A-module $M/\mathfrak{a}M$ is Noetherian. There then exists a submodule $N_0$ of M that is maximal among the submodules $N\subset M$ such that $M/N$ is faithful. Prove that the A-module $M/N_0$ is Noetherian and then that the ring A is Noetherian, and conclude.) b$)^*$Suppose that for every decreasing sequence $(\mathfrak{a}_n)_{n\in\mathbf{N}}$ of ideals of A, the sequence $(\mathfrak{a}_nM)_{n\in\mathbf{N}}$ is stationary. Prove that the A-module M is Artinian. (Reduce to the case when the A-module M is faithful. Prove that A then has only finitely many maximal ideals and, drawing on the proof of Proposition 1 of VIII, p. 173, that the radical of A is nilpotent. Deduce that there exists a finite sequence $(\mathfrak{m}_1,\mathfrak{m}_2,\cdots ,\mathfrak{m}_n)$ of maximal ideals of A whose product annihilates M. Conclude by induction on $n.)_*$

16) a) Let A be a commutative ring and $\rho : A\rightarrow B$ an injective ring homomorphism that makes B into a finitely generated left A-module. Suppose that for every increasing (resp. decreasing) sequence $(\mathfrak{a}_n)_{n\in\mathbf{N}}$ of ideals of A, the sequence $(\mathfrak{a}_nB)_{n\in\mathbf{N}}$ is stationary (which is the case if the ring B is right Noetherian (resp. right Artinian)). Prove that the ring A is Noetherian (resp. Artinian) (use Exercise 15). b) Give an example of a left and right Artinian and Noetherian ring B and a subring A of B such that B is finitely generated as a left and right A-module and that the ring A is neither left nor right Noetherian or Artinian (choose a suitable integral domain C, with field of fractions K, take B to be the matrix ring $\mathbf{M}_3(K)$ and A to be the subring of B consisting of the matrices $(a_{ij})_{1\leqslant i,j\leqslant 3}$ with $a_{ij}= 0$ for $1\leqslant i < j\leqslant 3$ and $a_{22}\in C.)$

17) Let E be a monoid, $e$ its identity element, S a subset of E, and $S'$ the submonoid of E generated by S. We say that S admits a calculus of left fractions on E if the following two (tautological when E is commutative) conditions are satisfied:

(i) For every $a\in E$ and every $s\in S$, there exist $b\in E$ and $t\in S'$ such that $ta=bs$.

(ii) For every $a\in E,b\in E$, and $s\in S$ such that $as=bs$, there exists a $t\in S'$ such that $ta=tb$. a) Suppose that there exists a homomorphism $u$ from E to a monoid $E'$ such that every element of $u(S)$ is invertible in $E'$ and that for every $a, b$ in E with $u(a) =u(b)$, there exists an $s\in S'$ such that $sa=sb$. Then S admits a calculus of left fractions on E. b) Suppose that S admits a calculus of left fractions on E. In $E\times S'$, we denote by $(a, s)\sim (b, t)$ the relation “there exist $c$ and $d$ in E such that we have $ca=db$ and $cs=dt\in S'$.” This is an equivalence relation. We set $S^{-1}E = (E\times S')/\sim$, and we denote by $\varepsilon : E\rightarrow S^{-1}E$ the mapping that sends $a\in E$ to the class of $(a, e)$. There exists a unique monoid structure on $S^{-1}E$ such that $\varepsilon$ is a unital homomorphism, that $\varepsilon (s)$ is invertible for every $s\in S$, and that for $(a, s)\in E\times S'$, the class of $(a, s)$ in $S^{-1}E$ is equal to $\varepsilon (s)^{-1}\varepsilon (a)$. We say that $S^{-1}E$ is the monoid of left fractions of E associated with S. It coincides with that defined in I, §2, No. 4, p. 18 when the monoid E is commutative. c) Let $a, b$ be in E. We have $\varepsilon (a) =\varepsilon (b)$ if and only if there exists an $s\in S'$ such that $sa=sb$. The mapping $\varepsilon$ is injective (resp. bijective) if and only if every element of S is right regular (resp. invertible). d) Let $f$ be a unital homomorphism from E to a monoid F such that every element of $f(S)$ is invertible in F. There is a unique homomorphism $f: S^{-1}E\rightarrow F$ such that $f=f\circ s$. If $f$ is injective, then $f$ is injective. e) We say that S admits a calculus of right fractions on E if it admits a calculus of left fractions on the opposite monoid $E^o$ of E. In this case, define the monoid of right fractions ES$^{-1}$ of E associated with S, observe that we have (ES$^{-1})^o= S^{-1}(E^o)$, and rewrite b) for the monoids of right fractions. If S admits a calculus of left and right fractions on E, then the monoids $S^{-1}E$ and ES$^{-1}$ are canonically isomorphic.

18) a) Let A be a ring, S a subset of A, and $S'$ the smallest subset of A containing 1 and S and stable under multiplication. We say that S admits a calculus of left fractions on A if the following two (tautological when A is commutative) conditions are satisfied:

(i) For every $a\in A$ and every $s\in S$, there exist $b\in A$ and $t\in S'$ such that $ta=bs$.

(ii) For every $a\in A$ and $s\in S$ such that $as= 0$, there exists a $t\in S'$ such that $ta= 0$.

This is equivalent to saying that S admits a calculus of left fractions on the monoid obtained by endowing the set A with only multiplication (Exercise 17). Prove that on the multiplicative monoid $S^{-1}A$, there then exists a unique addition such that $S^{-1}A$, endowed with this addition and its multiplication, is a ring and that the canonical mapping $\varepsilon : A\rightarrow S^{-1}A$ (loc. cit.) is a ring homomorphism. We say that $S^{-1}A$ is the ring of left fractions of A associated with S. When A is commutative, this coincides with the ring defined in I, §8, No. 12, p. 113. b) The set S admits a calculus of left fractions on A if and only if there exist a ring B and a ring homomorphism $u: A\rightarrow B$ such that every element of $u(S)$ is invertible in B and that for every $a\in u^{-1}$(0), there exists an $s\in S$ such that $sa= 0$. c) Suppose that S admits a calculus of left fractions on A. The kernel of the canonical homomorphism $\varepsilon : A\rightarrow S^{-1}A$ is the set of $a\in A$ for which there exists an $s\in S$ with $sa= 0$.

Let $f$ be a homomorphism from A to a ring B such that every element of $f(S)$ is invertible in B. There exists a unique homomorphism $f: S^{-1}A\rightarrow F$ such that $f=f\circ s$. If $f$ is injective, then $f$ is injective. d) Formulate the statements analogous to a), b), c) for a calculus of right fractions; if S admits a calculus of right fractions on A, we denote the ring of right fractions of A by AS$^{-1}$. In this case, we have (AS$^{-1})^o= S^{-1}(A^o)$. If S admits a calculus of left and right fractions on A, then the rings $S^{-1}A$ and AS$^{-1}$ are canonically isomorphic. e) Let A be a nonzero ring without zero divisors. Then A admits a field of left fractions (I, §9, p. 177, Exercise 15) if and only if the set S of nonzero elements of A admits a calculus of left fractions on A, and in this case, $S^{-1}A$ is the field of left fractions of A.

19) Let A be a ring, S a subset of A that admits a calculus of left fractions on A (Exercise 18), and $S'$ the smallest subset of A containing 1 and S and stable under multiplication. We denote by $S^{-1}A$ the ring of left fractions of A associated with S and by $\varepsilon : A\rightarrow S^{-1}A$ the canonical homomorphism. a) Let M be an A-module. We denote the $S^{-1}$ A-module $S^{-1}A\otimes_AM$ by $S^{-1}M$, and we call it the module of left fractions of M associated with S. Prove that every element of $S^{-1}M$ can be written as $\varepsilon (s)^{-1}\otimes x$ with $x\in M$ and $s\in S'$, and that for $x, y$ in M and $s, t$ in $S'$, the relation $\varepsilon (s)^{-1}\otimes x=\varepsilon (t)^{-1}\otimes y$ is equivalent to the existence of a pair $(c, d)$ of elements of A such that we have $cx=dy$ and $cs=dt\in S'$. b) We denote by $\varepsilon_M$ the canonical A-linear mapping $x\mapsto 1\otimes x$ from M to $S^{-1}M$. Its image generates the $S^{-1}$A-module $S^{-1}M$; its kernel consists of the elements $x\in M$ for which there exists an $s\in S'$ such that $sx= 0$. The mapping $\varepsilon_M$ is injective (resp. bijective) if and only if for every $s\in S$, the homothety $x\mapsto sx$ of M is injective (resp. bijective). c) We have $S^{-1}M = 0$ if and only if for every $x\in M$, there exists an $s\in S$ such that $sx= 0$. d) Let N be a submodule of M. The canonical $S^{-1}$A-linear mapping from $S^{-1}N$ to $S^{-1}M$ is injective. $(^*$In other words, the right A-module $S^{-1}A$ is flat.$_*)$ We identify $S^{-1}N$ with its image in $S^{-1}M$ under this mapping. The submodule $\varepsilon^-_M^1(S^{-1}N)$ of M consists of the elements $x\in M$ for which there exists an $s\in S'$ with $sx\in N$. We say that it is the left saturation of N for S. e) The mapping $N'\mapsto \varepsilon^-_M^1(N')$ is an isomorphism from the ordered set of $S^{-1}A$-submodules of $S^{-1}M$ onto the ordered set of A-submodules of M that are left saturated, (i.e., equal to their saturation) for S. The inverse isomorphism is $N\mapsto S^{-1}N$. f ) If the A-module M is Noetherian, then the $S^{-1}$A-module $S^{-1}M$ is Noetherian. If the A-module M is Artinian, then the $S^{-1}$A-module $S^{-1}M$ is Artinian and the mapping $\varepsilon_M: M\rightarrow S^{-1}M$ is surjective. g) If the ring A is left Noetherian (resp. left Artinian), then so is the ring $S^{-1}A$. h) Formulate the statements analogous to those of this exercise for the modules of right fractions of right modules.

20) Prove that a left Noetherian ring A without zero divisors admits a field of left fractions (Exercise 18) (if $a$ and $s$ are nonzero elements of A, use the fact that the sequence of ideals $(As+ Asa+\cdots + Asa^n)_{n\in\mathbf{N}}$ is stationary to prove that $Aa\cap As$ is not reduced to 0).

21) Let A be a ring, $\sigma$ an endomorphism of the ring A, and $d$ a nilpotent endomorphism of the additive group of A satisfying the relation $d(ab) =\sigma (a)d(b) +d(a)b$. a) Show that the set $S =\{X\}$ admits a calculus of left fractions (Exercise 18) on the ring $B = A[X]_{\sigma ,d}$ (VIII, p. 11). If $\sigma$ is injective, then the canonical homomorphism from B to $S^{-1}B$ is injective and we identify B with a subring of $S^{-1}B$. If $\sigma$ is bijective, then S also admits a calculus of right fractions on B, and every element of $S^{-1}B$ can be written uniquely as $\sum_{n\in\mathbf{Z}}a_nX^n$, where $(a_n)_{n\in\mathbf{Z}}$ is a family of elements of A with finite support. For $a\in A$, write the element $X^{-1}a$ of $S^{-1}B$ in this form. b) Prove that the multiplication in the ring $A[X]_{\sigma ,d}$ extends by continuity to a multiplication on the set A[[X]] of formal power series in X with coefficients in A. The additive group A[[X]] endowed with this multiplication is a ring that we denote by $A[[X]]_{\sigma ,d}$ (or simply $A[[X]]_{\sigma}$ if $d= 0)$. Give an example where a formal power series $u\in A[[X]]$ with constant term equal to 1 has neither a left nor a right inverse in the ring $A[[X]]_{\sigma ,d}$. c) Show that the invertible elements of $A[[X]]_{\sigma}$ are those whose constant term is invertible in A. d) Formulate and prove the analog of a) after replacing the ring $A[X]_{\sigma ,d}$ with the ring $A[[X]]_{\sigma ,d}$. e) Suppose that A is a field and $\sigma$ an automorphism of A. Then $S^{-1}A[[X]]_{\sigma}$ (where $S =\{X\})$ is a field, and each of its elements can be written uniquely as $\sum_{n\in\mathbf{Z}}a_nX^n$, where $(a_n)_{n\in\mathbf{Z}}$ is a family of elements of A having only finitely many nonzero terms with index $<0$. We denote this field by $A((X))_{\sigma}$. f ) Suppose that A is a commutative field. Describe the center of the field $A((X))_{\sigma}$. Deduce an example of a field of infinite degree over its center.

22) Let G be a group and H a normal subgroup of G such that the quotient group $G/H$ is isomorphic to $\mathbf{Z}$. Let $g$ be an element of G whose canonical image in $G/H$ generates $G/H$. Let C be a commutative ring, A the algebra C[H] of H over C (III, §2, No. 6, p. $446), (e_h)_{h\in H}$ its canonical basis, and $\sigma$ the automorphism of A that sends $e_h$ to $e_{ghg^{-1}}$. a) Prove that there exists a unique homomorphism $u$ from the ring $B = A[X]_{\sigma}$ to the ring C[G] that extends the canonical injection of A = C[H] into C[G] and sends X to the element $e_g$ of the canonical basis of C[G]. b) Set $S =\{X\}$. Prove that $u$ extends to an isomorphism from the ring $S^{-1}B$ (cf. Exercise 21) to C[G]. Deduce that if the ring C[H] is left Noetherian, then so is the ring C[G].

23) Let A be a ring, I a set, $\boldsymbol{\sigma }= (\sigma_i)_{i\in I}$ a family of endomorphisms of the ring A, and $\boldsymbol{d}= (d_i)_{i\in I}$ a family of endomorphisms of the additive group of A, satisfying the relations

$$
\sigma_i\circ \sigma_j=\sigma_j\circ \sigma_i\sigma_i\circ d_j=d_j\circ \sigma_id_i\circ d_j=d_j\circ d_i
$$

for $i\in I,j\in I,i\not=j$ and

$$
d_i(ab) =\sigma_i(a)d_i(b) +d_i(a)b
$$

for $i\in I,a\in A,b\in A$. a) Prove that there exists a unique ring B whose additive group is the additive group $A[\mathbf{X}]$ of polynomials with coefficients in A in the family of variables $\mathbf{X}= (X_i)_{i\in I}$ and whose product has the following properties:

(i) The elements $X_i(i\in I)$ of B are pairwise permutable.

(ii) For every $a\in A$ and every multi-index $\boldsymbol{\nu }= (\nu_i)_{i\in I}\in \mathbf{N}^{(I)}$, the product in B, in this order, of $a$ and a finite sequence of $\nu_i$ elements equal to $X_i$ for each $i\in I$ is the polynomial $a\mathbf{X}^{\boldsymbol{\nu }}$.

(iii) For every $a\in A$ and every $i\in I$, we have the relation $X_ia=\sigma_i(a)X_i+d_i(a)$ in the ring B. b) The ring B is denoted by $A[\mathbf{X}]_{\boldsymbol{\sigma },\mathbf{d}}$. It has the following universal property: given a ring C, a ring homomorphism $f: A\rightarrow C$, and a family $(x_i)_{i\in I}$ of elements of C that are pairwise permutable such that $x_if(a) =f(\sigma_i(a))x_i+f(d_i(a))$ for every $a\in A$ and every $i\in I$, there exists a unique ring homomorphism $g: B\rightarrow C$ extending $f$ such that $g(X_i) =x_i$ for $i\in I$. c) Let J be a subset of I. Denote the ring $A[(X_i)_{i\in J}]_{(\sigma_i)_{i\in J},(d_i)_{i\in J}}$ by $B'$. For every $i\in I$ J, there exist a unique endomorphism $\sigma_i'$ of the ring $B'$ and a unique endomorphism $d'_i$ of the additive group of $B'$ such that

$\sigma_i'(a) =\sigma_i(a)d'_i(a) =d_i(a)$ for $a\in A$,

$\sigma_i'(X_j) = X_jd'_i(X_j) = 0$ for $j\in J$,

$d'_i$(PQ) $=\sigma '_i(P)d'_i(Q) +d'_i(P)Q$ for $P\in B,Q\in B$.

Set $\boldsymbol{\sigma }'= (\sigma_i')_{i\in I J}$ and $\boldsymbol{d}'= (d'_i)_{i\in I J}$. The canonical bijection from $A[(X_i)_{i\in I}]$ to $A[(X_j)_{j\in J}][(X_i)_{i\in I J}]$ is an isomorphism from the ring $B = A[(X_i)_{i\in I}]_{\boldsymbol{\sigma },\boldsymbol{d}}$ to the ring $B'[(X_i)_{i\in I J}]_{\boldsymbol{\sigma }',\boldsymbol{d}'}$. d) If the ring A is left Noetherian, then the set I is finite, and if for every $i\in I$, the endomorphism $\sigma_i$ of A is bijective, then the ring $B = A[\mathbf{X}]_{\boldsymbol{\sigma },\boldsymbol{d}}$ is left Noetherian. e) Suppose that for every $i\in I$, the morphism $\sigma_i$ is the identity mapping on A. Let E be the endomorphism ring of the additive group of A. Show that there exists a unique ring homomorphism $\psi$ from $B = A[\mathbf{X}]_{\boldsymbol{\sigma },\boldsymbol{d}}$ to E such that $\psi (X_i) =d_i$ for $i\in I$ and that for all $a\in A$, the morphism $\psi (a)$ is the left homothety $b\mapsto ab$ of A. f ) Keep the assumptions of e). Suppose, moreover, that A is a polynomial ring $C[(T_i)_{i\in I}]$ with coefficients in a (not necessarily commutative) ring C and that for every $i\in I$, the morphism $d_i$ is the derivation $P\mapsto_{\partial}^{\partial}_T^{P_i}$ of A. Prove that if C is nonzero and without torsion on $\mathbf{Z}$, the homomorphism $\psi : B\rightarrow E$ is injective. Prove that if C is a ring of characteristic $p >0$ (V, §1, No. 2, p. 2), the kernel of $\psi$ is the left ideal of B generated by the element $X^p_i(i\in I)$.

$\P 24)$ Let G be a group, $e$ its identity element, and A a nonzero commutative ring. Denote the algebra of the group G over A by A[G] (III, §2, No. 6, p. 446). a) Let I be a finite set, $(G_i)_{i\in I}$ a family of subgroups of G, and $(g_i)_{i\in I}$ a family of elements of G. Prove that if G is the union of the family $(g_iG_i)_{i\in I}$, one of the subgroups $G_i$ has finite index in G. b) Suppose that every conjugacy class in G distinct from $\{e\}$ is infinite and that the ring A is an integral domain. Prove that if $\mathfrak{a}$ and $\mathfrak{b}$ are two nonzero two-sided ideals of the ring A[G], we have $\mathfrak{a}\mathfrak{b}\not= 0$. (Choose elements $a=\sum a_gg$ and $b=\sum b_gg$ in $\mathfrak{a}$ and $\mathfrak{b}$ with $a_e\not= 0$ and $b_e\not= 0$. Using a), prove that, if necessary replacing $a$ with $hah^{-1}$ for suitable $h\in G$, we may assume that $a_gb_{g^{-1}}= 0$ for every $g\not=e$ in G.) $*$c) Prove that the ring A[G] is left (resp. right) Artinian if and only if the ring A is

Artinian and the group G is finite. (If A[G] is left Artinian, deduce from Theorem 1 of VIII, p. 6 that the group G has finite length; to prove that it is finite, reduce to the case when A is a field and G a simple group, and then use b) and Proposition 1 of VIII, p. 173$).*$

25) Keep the notation of Exercise 24. a) For any subgroup H of G, let $I_H$ be the kernel of the canonical surjection $\mathbf{Z}[G]\rightarrow \mathbf{Z}^{(G/H)}$. Then the mapping $H\mapsto I_H$ is the increasing injection from the set of subgroups of G to the set of the left ideals of $\mathbf{Z}[G]$; if H is a normal subgroup of G, the ideal $I_H$ is two-sided. b) Suppose that the ring A[G] is left Noetherian. It is then also right Noetherian. For every subgroup H of G, the ring A[H] is left Noetherian; in particular, the ring A is Noetherian. If H is normal in G, then the ring $A[G/H]$ is left Noetherian. Every subgroup of G admits a finite generating system. c) Prove that the following properties are equivalent:

(i) The group G admits a composition series whose quotients are finite or isomorphic to $\mathbf{Z}$.

(ii) The group G admits a composition series $(G_i)_{0\leqslant i\leqslant n}$ such that $G_1$ has finite index in G and $G_i/G_{i+1}$ is isomorphic to $\mathbf{Z}$ for $0\leqslant i\leqslant n-1$.

When they are satisfied and the ring A is Noetherian, the ring A[G] is left Noetherian (use Exercise 22).

26) Let K be a commutative field, A the polynomial ring K[T], and $\sigma$ the endomorphism $P(T)\mapsto P(T^2)$ of the ring A. The ring $A[X]_{\sigma}$ is not left Noetherian even though the ring A is Noetherian.

27) Let D be a field, $\sigma$ an automorphism of $D,d$ an endomorphism of the additive group of D satisfying relation (1) of VIII, p. 9, and A the ring $D[X]_{\sigma ,d}$ (VIII, p. 11). Given a nonzero element $P =\sum_na_nX^n$ of A, the greatest integer $n$ such that $a_n\not= 0$ is called the degree of P and denoted by deg(P). We set deg(0) $=-\infty$. a) Let $F,G$ be elements of A with $G\not= 0$; show that there exist well-determined elements $Q,R$ (resp. $Q',R')$ of A such that F = QG + R and deg(R) $<$ deg(G) (resp. F = GQ$'+ R'$ and deg(R$')<$ deg(G)). b) Deduce that every left (resp. right) ideal of A is monogenous. If $F,G,H,K$ are elements of A satisfying AF + AG = AH and AF $\cap$ AG = AK, then we have deg(F) + deg(G) = deg(H) + deg(K) (observe that the D-vector space $A/$AF has dimension deg(F)). c) The ideal AF of A is maximal if and only if F is irreducible, that is, is not the product of two nonconstant polynomials.

28) Let B be a ring, A a subring of B, and $x$ an element of B such that we have $A + Ax= A +xA$ and that the ring B is generated by $A\cup  \{x\}$. a) Let M be a Noetherian left A-module; prove that the B-module $M_{(B)}= B\otimes_AM$ is Noetherian. In particular, if the ring A is left Noetherian, then so is B. b) Suppose that the A-module M has finite length $n$; prove that every B-submodule of $M_{(B)}$ admits a generating subset of cardinality $\leqslant n$ (adapt the proof of Theorem 1 of VIII, p. 6).

[^1]: This proof was communicated to us by A. Rosenberg.
