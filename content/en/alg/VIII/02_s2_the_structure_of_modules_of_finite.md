---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 2
section_title: The Structure of Modules of Finite Length
lang: en
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.25-A VIII.43
pdf_pages: 0042-0060
extraction: native
subsections:
    - "no": 1
      title: Local Rings
      page: 25
      pdf_page: 42
    - "no": 2
      title: Weyr–Fitting Decomposition
      page: 27
      pdf_page: 44
    - "no": 3
      title: Indecomposable Modules and Primordial Modules
      page: 30
      pdf_page: 47
    - "no": 4
      title: Semiprimordial Modules
      page: 32
      pdf_page: 49
    - "no": 5
      title: The Structure of Modules of Finite Length
      page: 37
      pdf_page: 54
statements: 37
exercises: 20
content_sha256: 914e243aae55024b8374f15d6c940a29370810a3872e09be2dd123eef9d21a5a
---

## § 2. THE STRUCTURE OF MODULES OF FINITE LENGTH

### 1. Local Rings

#### Proposition 1 {#alg-viii-s2-prop-1 .statement tag=001P}

Let A be a nonzero ring, and let $\mathfrak{r}$ be the set of noninvertible elements of A. The following properties are equivalent:

(i) The set $\mathfrak{r}$ is a two-sided ideal of A.

(ii) The set $\mathfrak{r}$ is stable under addition.

(iii) The ring A has a unique maximal left ideal.

(iv) For every $a\in A$, one of the elements $a$ and $1-a$ is invertible.

(v) For every $a\in A$, one of the elements $a$ and $1-a$ is left invertible.

The implication (i) $\Rightarrow$ (ii) follows from the definition of an ideal. Since 1 does not belong to $\mathfrak{r}$, we have (ii) $\Rightarrow$ (iv).

We have $\mathfrak{r}\not= A$, and the set $\mathfrak{r}$ contains every left ideal of A not equal to A. If $\mathfrak{r}$ is a left ideal of A, it is therefore the unique maximal left ideal of A. This proves that (i) implies (iii).

Suppose that A has a unique maximal left ideal $\mathfrak{m}$. Take $b\in A-\mathfrak{m}$. The left ideal $Ab$ is not contained in any maximal left ideal of A, hence is equal to A (I, §8, No. 6, p. 104, Theorem 1), and $b$ is left invertible. For every $a\in A$, one of the elements $a$ and $1-a$ belongs to A $-\mathfrak{m}$ because $\mathfrak{m}$ is an ideal that does not contain 1. Thus, (iii) implies (v).

Suppose that property (v) holds. Let $b$ be a left invertible element of A. Let $c\in A$ be such that $cb= 1$. We have $(1-bc)b= 0$ and $b\not= 0$; hence, $1-bc$ is not left invertible. By property (v), $bc$ is left invertible and, a fortiori, $c$ is left invertible. But then $c$ is invertible; $b$ is its inverse, so $b$ is invertible. It follows that (v) implies (iv).

It remains to prove that (iv) implies (i). Suppose that (iv) holds. Then $\mathfrak{r}$ is a two-sided ideal of A by the following assertions a) through d):

a) We have $0\in \mathfrak{r}$ because the ring A is nonzero.

b) The product of two elements of A, one belonging to $\mathfrak{r}$ and the other to A $-\mathfrak{r}$, belongs to $\mathfrak{r}$.

c) The set $\mathfrak{r}$ is stable under addition.

Indeed, let $a$ and $b$ be elements of $\mathfrak{r}$ such that $s=a+b$ is invertible. By b), the elements $s^{-1}a$ and $s^{-1}b$ of A belong to $\mathfrak{r}$; since $s^{-1}b= 1-s^{-1}a$, this contradicts the assumption that (iv) holds.

d) The set $\mathfrak{r}$ is stable under multiplication.

Indeed, let $a$ and $b$ be two elements of $\mathfrak{r}$. The element $a'=-a(1-b)$ belongs to $\mathfrak{r}$ by b), so that the element $ab$, which is equal to $a+a'$, belongs to $\mathfrak{r}$ by c); assertion d) follows.

#### Definition 1 {#alg-viii-s2-def-1 .statement tag=001Q}

A local ring is a nonzero ring that has the equivalent properties of Proposition 1.

A ring A is local if and only if the opposite ring $A^o$ is local.

If A is a local ring, then the set $\mathfrak{r}$ of noninvertible elements of A is a two-sided ideal of A; it contains every left or right ideal of A not equal to A. The ring $A/\mathfrak{r}$ is therefore a field, which we call the residue field of A. The set $\mathfrak{r}$ is the unique maximal left (resp. right, two-sided) ideal of A; we simply say that $\mathfrak{r}$ is the maximal ideal of A.

#### Example 1 {#alg-viii-s2-n1-exa-1 .statement tag=001R}

Every field is a local ring.

#### Example 2 {#alg-viii-s2-n1-exa-2 .statement tag=001S}

Let A be a nonzero ring in which every element is invertible or nilpotent. Then A is a local ring. Indeed, if $a\in A$ is not invertible, then by assumption, there exists an integer $n\geqslant 0$ such that $a^{n+1}= 0$, and $1-a$ has inverse $1 +a+\cdots +a^n$.

#### Example 3 {#alg-viii-s2-n1-exa-3 .statement tag=001T}

Let X be a $C^r$ manifold (VAR, R, 5.1.5) and $x$ a point of X. Let $\mathscr{O}_x$ be the ring of germs at $x$ of $C^r$ functions with values in the field of scalars K. Then $\mathscr{O}_x$ is a commutative local ring, and its maximal ideal consists of the

germs of the functions that are zero at $x.*$

#### Example 4 {#alg-viii-s2-n1-exa-4 .statement tag=001U}

Let A be a commutative local ring and $B = A[[X_i]]_{i\in I}$ an algebra of formal power series with coefficients in A (III, §2, No. 11, p. 456). By Proposition 6 of IV, §4, No. 4, p. 30, the ring B is local, and its maximal ideal consists of the formal power series with constant term in the maximal ideal of A. In particular, if A is a field, the maximal ideal of $A[[X_i]]_{i\in I}$ consists of the formal power series with constant term zero.

#### Example 5 {#alg-viii-s2-n1-exa-5 .statement tag=001V}

Let $p$ be a prime number. We denote by $\mathbf{Z}_{(p)}$ the subring of the field $\mathbf{Q}$ of rational numbers consisting of the fractions $a/b$ with $a\in \mathbf{Z},b\in \mathbf{Z}$, and $b$ not divisible by $p*$(cf. Comm. Alg., II, §2, No. 1, p. 60) . Then $\mathbf{Z}$ is

$*(_{p)}$

a commutative local ring, with maximal ideal $p\mathbf{Z}_{(p)}$. The ring $\mathbf{Z}_p$ of $p$-adic integers (V, §12, No. 3, p. 96) is a commutative local ring, with maximal ideal $p\mathbf{Z}_p$ (VIII, p. 40, Exercise 9).

#### Example 6 {#alg-viii-s2-n1-exa-6 .statement tag=001W}

Let K be a commutative field of characteristic $p >0$ and G a $p$-group (I, §6, No. 5, p. 76, Definition 9). The algebra K[G] of the group G over K (III, §2, No. 6, p. 446) is a local ring; its maximal ideal is the set of elements $(a_g)_{g\in G}$ of K[G] such that $\sum_{g\in G}a_g= 0$ (VIII, p. 41, Exercise 10).

### 2. Weyr–Fitting Decomposition

Let A be a ring, M an A-module, and $u$ an endomorphism of M. For any integer $p\geqslant 0$, we denote the kernel of $u^p$ by $N_p$. The sequence of submodules $(N_p)$ is increasing, and its union is a submodule $N_{\infty}$ of M that is stable under $u$. For every integer $p\geqslant 0$, we have $N_{p+1}=\overset{-1}{u}(N_p)$, and the relation $N_p= N_{p+1}$ therefore implies $N_{p+1}= N_{p+2}$. Consequently, either the sequence $(N_p)$ is strictly increasing, or there exists an integer $p\geqslant 0$ such that $N_0, . . . ,N_p$ are distinct and $N_p= N_{\infty}$.

For any integer $q\geqslant 0$, denote the image of $u^q$ by $I_q$. The sequence of submodules $(I_q)$ is decreasing, and its intersection is a submodule $I_{\infty}$ of M that is stable under $u$. For every integer $q\geqslant 0$, we have $u(I_q) = I_{q+1}$, and the relation $I_q= I_{q+1}$ therefore implies $I_{q+1}= I_{q+2}$. Consequently, either the sequence $(I_q)$ is strictly decreasing, or there exists an integer $q\geqslant 0$ such that $I_0, . . . ,I_q$ are distinct and $I_q= I_{\infty}$.

#### Proposition 2 {#alg-viii-s2-prop-2 .statement tag=001X}

a) Suppose that the sequence $(N_p)$ is stationary. Then we have $N_{\infty}\cap I_{\infty}= 0$, the restriction of $u$ to $I_{\infty}$ is injective, and $u$ induces a nilpotent endomorphism of $N_{\infty}$.

b) Suppose that the sequence $(I_p)$ is stationary. Then we have M = $N_{\infty}+ I_{\infty}$ and $u(I_{\infty}) = I_{\infty}$.

c) (“Weyr–Fitting decomposition”—sometimes called the “Fitting decomposition”) Suppose that the sequences $(N_p)$ and $(I_p)$ are stationary. Then M is a direct sum of submodules $N_{\infty}$ and $I_{\infty}$ that are stable under $u$, and $u$ induces a nilpotent endomorphism of $N_{\infty}$ and an automorphism of $I_{\infty}$.

Let $p$ be a natural number such that $N_p= N_{\infty}$, and let $v=u^p$. By construction, $v$ and $v^2$ have the same kernel $N_{\infty}$, and $I_p$ is the image of $v$. For $x$ in $N_{\infty}\cap I_p$, there exists a $y\in M$ such that $x=v(y)$ and therefore $v^2(y) =v(x) = 0$; hence, we have $y\in N_{\infty}$ and consequently $x= 0$. In particular, we have $N_{\infty}\cap I_{\infty}= 0$. Since the kernel $N_1$ of $u$ is contained in $N_{\infty}$, the restriction of $u$ to $I_{\infty}$ is injective; on the other hand, we have $u^p(N_{\infty}) = 0$. This proves a).

Let $q$ be a natural number such that $I_q= I_{\infty}$, and let $w=u^q$. Then $w$ and $w^2$ have the same image $I_{\infty}$, and $N_q$ is the kernel of $w$. Let $x\in M$. We have $w(x)\in I_{\infty}$, so there exists a $y\in M$ such that $w(x) =w^2(y)$; we then have $x-w(y)\in N_q$, whence $M = N_q+ I_{\infty}$ and a fortiori $M = N_{\infty}+ I_{\infty}$. We have $u(I_{\infty}) =u(I_q) = I_{q+1}= I_{\infty}$. This proves b).

Assertion c) follows immediately from a) and b).

#### Remark 1 {#alg-viii-s2-n2-rem-1 .statement tag=001Y}

Let $p$ be an integer such that $N_p= N_{p+1}$; the proof given above shows that $N_{\infty}\cap I_p= 0$, and the restriction of $u$ to $I_p$ is injective. Likewise, let $q$ be an integer such that $I_q= I_{q+1}$; then we have $N_q+ I_{\infty}= M$, and the endomorphism of $M/N_q$ deduced from $u$ by passing to the quotient is surjective.

#### Remark 2 {#alg-viii-s2-n2-rem-2 .statement tag=001Z}

Suppose that M is a direct sum of two submodules N and I that are stable under $u$ and that $u$ induces a nilpotent endomorphism $u_N$ of N and an automorphism of I. We then have $N_{\infty}= N$ and $I_{\infty}= I$, and the sequences $(N_p)$ and $(I_p)$ are stationary. Moreover, the following integers are equal:

$\alpha )$ the least integer $p\geqslant 0$ such that $N_p= N_{\infty}$,

$\beta )$ the least integer $q\geqslant 0$ such that $I_q= I_{\infty}$,

$\gamma )$ the least integer $r\geqslant 0$ such that $(u_N)^r= 0$.

#### Remark 3 {#alg-viii-s2-n2-rem-3 .statement tag=0020}

The assumption of assertion a) is satisfied if the A-module M is Noetherian; the assumption of assertion b) is satisfied if M is Artinian; by Proposition 1 of VIII, p. 2, the assumption of assertion c) is satisfied if M has finite length.

#### Corollary 1 {#alg-viii-s2-prop-2-cor-1 .statement tag=0021}

Let A be a ring, and let M be an A-module.

a) If the module M is Noetherian, then every surjective endomorphism of M is bijective.

b) If the module M is Artinian, then every injective endomorphism of M is bijective.

c) If the module M has finite length, then every injective or surjective endomorphism of M is bijective.

d) If the ring A is commutative and the A-module M is finitely generated, then every surjective endomorphism of M is bijective.

Let $u$ be an endomorphism of the A-module M. We use the notation introduced at the beginning of this subsection. If the endomorphism $u$ is surjective, then we have $I_{\infty}= M$. Assertion a) then follows from Proposition 2, a) and Remark 3. Likewise, if the endomorphism $u$ is injective, we have $N_{\infty}= 0$. Assertion b) therefore follows from Proposition 2, b) and Remark 3. Assertion c) follows immediately from a) and b).

Now, suppose that the ring A is commutative, the A-module M is finitely generated, and the endomorphism $u$ is surjective. Let us prove that $u$ is injective. Let $x$ be an element of M such that $u(x) = 0$. Choose a finite generating family $(x_i)_{i\in I}$ of the A-module M and, for every $i\in I$, an element $y_i$ of M such that $u(y_i) =x_i$. There exist families $(a_i)_{i\in I}, (b_{ij})_{(i,j)\in I\times I}$, and $(c_{ij})_{(i,j)\in I\times I}$ of elements of A such that we have

$$
x=\sum_{i\in I}a_ix_i,y_j=\sum_{i\in I}b_{ij}x_i,u(x_j) =\sum_{i\in I}c_{ij}x_i
$$

for every $j\in I$. Let $A'$ be a Noetherian subring of A containing the elements $a_i,b_{ij}$, and $c_{ij}$ (VIII, p. 12, Corollary 3). Let $M'$ be the $A'$-submodule of M generated by the family $(x_i)_{i\in I}$. We have $u(x_j)\in M',y_j\in M'$, and $u(y_j) =x_j$ for every $j\in I$; hence $u$ defines, by restriction, a surjective endomorphism $u'$ of the $A'$-module $M'$. Since the ring $A'$ is Noetherian, the finitely generated $A'$-module $M'$ is Noetherian (VIII, p. 7, Proposition 4 a)). By a), the endomorphism $u'$ of $M'$ is bijective. By construction, $x$ belongs to $M'$, and we have $u'(x) =u(x) = 0$. We therefore have $x= 0$, which proves d).

#### Corollary 2 {#alg-viii-s2-prop-2-cor-2 .statement tag=0022}

In a left Noetherian ring, every left or right invertible element is invertible.

Indeed, consider elements $x,y$ of a left Noetherian ring A such that $xy= 1$. Denote by $\boldsymbol{\delta }(x)$ and $\boldsymbol{\delta }(y)$, respectively, the endomorphisms $a\mapsto ax$ and $a\mapsto ay$ of the A-module $A_s$. We have $\boldsymbol{\delta }(y)\circ \boldsymbol{\delta }(x) = 1_{A_s}$; hence $\boldsymbol{\delta }(y)$ is surjective. By Corollary 1, a), $\boldsymbol{\delta }(y)$ is bijective. The endomorphism $\boldsymbol{\delta }(x)$ is then the inverse bijection of $\boldsymbol{\delta }(y)$, and we have $yx= (\boldsymbol{\delta }(x)\circ \boldsymbol{\delta }(y))(1) = 1$. The corollary follows.

### 3. Indecomposable Modules and Primordial Modules

Let A be a ring. Recall the following definition (VII, §4, No. 8, p. 23, Definition 3).

#### Definition 2 {#alg-viii-s2-def-2 .statement tag=0023}

An A-module M is called indecomposable if it is not the direct sum of a family of submodules distinct from 0 and M.

By the corollary of Proposition 12 of II, §1, No. 8, p. 209, the following properties are equivalent:

a) The A-module M is indecomposable.

b) The A-module M is nonzero, and every direct factor submodule of M is equal to 0 or M.

c) The A-module M is nonzero, and the ring End$_A(M)$ contains no idempotent disctinct from 0 and $1_M$.

In particular, since the endomorphism ring of the A-module $A_s$ is isomorphic to the opposite ring of A, we see that the A-module $A_s$ is indecomposable if and only if the ring A is nonzero and its only idempotents are 0 and 1.

#### Example {#alg-viii-s2-n3-exa-1 .statement tag=0024}

Suppose that the ring A is a principal ideal domain. The indecomposable finitely generated A-modules are the A-modules isomorphic to either A or $A/p^nA$, where $p$ is an irreducible element of A and $n$ an integer $>0$ (VII, §4, No. 8, p. 24, Proposition 8).

#### Proposition 3 {#alg-viii-s2-prop-3 .statement tag=0025}

A Noetherian or Artinian A-module M is the direct sum of a finite family of indecomposable submodules.

Let us first prove that every nonzero submodule P of M has an indecomposable direct factor. If this were not the case, then every direct factor submodule of P would be decomposable; proceeding by induction, we could then construct, for every $n\in \mathbf{N}$, nonzero submodules $N'_n$ and $N''_n$ of P such that $P = N'_0\oplus N''_0$ and $N'_{n-1}= N'_n\oplus N''_n$ for $n\geqslant 1$. But then, the sequence of submodules $N''_0+\cdots + N''_n$ would be strictly increasing, and that of the submodules $N'_n$ would be strictly decreasing. The module M would be neither Noetherian nor Artinian, contrary to the assumption.

Now, suppose that M is not the direct sum of a finite family of indecomposable submodules. By induction, we construct indecomposable submodules $P''_n$ of M and nonzero submodules $P'_n$ of M for every $n\in \mathbf{N}$ such that $M = P'_0\oplus P''_0$ and $P'_{n-1}= P'_n\oplus P''_n$ for $n\geqslant 1$. Indeed, M is nonzero, and the first part of the proof, applied to P = M, provides $P'_0$ and $P''_0$. Since the modules $P'_k$ and $P''_k$ are defined for $k < n$, by the first part of the proof, there exist submodules $P'_n$ and $P''_n$ such that $P'_{n-1}= P'_n\oplus P''_n$ with $P''_n$ indecomposable. The relation $M = P'_n\oplus P''_0\oplus  \cdots  \oplus P''_n$ then implies that $P'_n\not= 0$ because M is not the direct sum of a finite family of indecomposable modules.

The sequence of submodules $P''_0\oplus  \cdots  \oplus P''_n$ is strictly increasing, and the sequence of submodules $P'_n$ is strictly decreasing. This contradicts the assumption that M is Noetherian or Artinian.

The question of the uniqueness of the decomposition of a module as a direct sum of indecomposable submodules will be studied in the next subsection.

#### Definition 3 {#alg-viii-s2-def-3 .statement tag=0026}

A module is called primordial[^1] if its endomorphism ring is local.

By definition, a local ring is not reduced to 0; consequently, a primordial module is nonzero. Moreover, the A-module $A_s$ is primordial if and only if the ring A is local.

#### Proposition 4 {#alg-viii-s2-prop-4 .statement tag=0027}

a) A primordial module is indecomposable.

b) An indecomposable module of finite length is primordial.

Let M be an A-module. Suppose that M is primordial; let $e$ be an idempotent in the local ring End$_A(M)$. Since $e^2=e$, either $e$ is invertible and we have $e= 1$, or $1-e$ is invertible and we have $e= 0$. This proves that M is indecomposable (VIII, p. 30).

Now, suppose that M is indecomposable and of finite length. By Proposition 2, c) of VIII, p. 27, every endomorphism of M is invertible or nilpotent; the ring End$_A(M)$ is therefore local by Example 2 of VIII, p. 26.

The $\mathbf{Z}$-module $\mathbf{Z}$ is indecomposable, Noetherian, but not Artinian. Its endomorphism ring is isomorphic to $\mathbf{Z}$, hence is not local. Consequently, $\mathbf{Z}$ is not a primordial $\mathbf{Z}$-module.

$*$Let $p$ be a prime number. The endomorphism ring of the $\mathbf{Z}$-module $\mathbf{Q}_p/\mathbf{Z}_p$ is isomorphic to the local ring $\mathbf{Z}_p$ (cf. VII, §4, p. 65, Exercise 13); it is therefore a primordial $\mathbf{Z}$-module.

An injective module is indecomposable if and only if it is primordial (X, §1, n$^o9$, p. 21, proposition $14).*$

### 4. Semiprimordial Modules

#### Definition 4 {#alg-viii-s2-def-4 .statement tag=0028}

A module is called semiprimordial if it is the direct sum of a family of primordial submodules.

#### Example 1 {#alg-viii-s2-n4-exa-1 .statement tag=00SE}

$*$Every simple module is primordial (VIII, p. 45); every semisimple module is therefore semiprimordial (VIII, p. 55, Definition 1).

#### Example 2 {#alg-viii-s2-n4-exa-2 .statement tag=01L7}

If A is a left Noetherian ring, then every injective A-module is semiprimordial (X, §1, n$^o9$, p. 21, proposition 14 and X, §1, n$^o10$, p. 22, théorème 3, b)).$*$

#### Theorem 1 (Azumaya) {#alg-viii-s2-thm-1 .statement tag=00RX}

Let A be a ring, L a primordial A-module, and M a semiprimordial A-module. There exists a unique cardinal, denoted by [M : L], with the following property:

For every decomposition $M =\bigoplus_{i\in I}M_i$ of M as a direct sum of primordial modules, the set of indices $i\in I$ such that $M_i$ is isomorphic to L has cardinal [M : L].

The proof is based on the following four lemmas.

#### Lemma 1 {#alg-viii-s2-lem-1 .statement tag=0029}

Let M be an A-module, $M'$ a primordial submodule of M, and $M''$ a submodule of M supplementary to $M'$. Let $u$ be an endomorphism of M. Then $u$ or $1_M-u$ induces an isomorphism from $M'$ to a submodule of M supplementary to $M''$.

Let $p$ be the projection from M onto $M'$ with kernel $M''$, and let $v$ be the restriction of $p\circ u$ to $M'$. First, suppose that $v$ is an automorphism of $M'$. Since $v$ is injective, the restriction of $u$ to $M'$ is injective, and we have $u(M')\cap M''= 0$. Since $v$ is surjective, we have $u(M')\oplus M''= M$. Consequently, $u$ induces an isomorphism from $M'$ to a submodule supplementary to $M''$ in M. Now, suppose that $v$ is not an automorphism of $M'$. Then $1_{M'}-v$ is an automorphism of $M'$ because $M'$ is primordial. Now, $1_{M'}-v$ is the restriction of $p\circ (1_M-u)$ to $M'$. The previous reasoning proves that $1_M-u$ induces an isomorphism from $M'$ to a submodule of M supplementary to $M''$.

#### Lemma 2 {#alg-viii-s2-lem-2 .statement tag=002A}

Let M be an A-module that is the direct sum of a family $(M_i)_{i\in I}$ of primordial submodules, and let $u$ be an endomorphism of M. Set $v= 1_M-u$ and $M_J=\bigoplus_{i\in J}M_i$ for every subset J of I. Then one of the following two properties holds:

a) There exists an index $i\in I$ such that $u$ induces an isomorphism from $M_i$ to a direct factor submodule of M.

b) For every finite subset J of I$,v$ induces an isomorphism from $M_J$ to a submodule supplementary to $M_{I-J}$.

If property b) holds, then $v$ is injective.

Suppose that property a) does not hold, and let us establish property b) by induction on the cardinal of J. There is nothing to prove if $J =\emptyset$. Therefore, assume that J is nonempty, choose an element $i$ of J, and set $J'= J-\{i\}$. By the induction hypothesis, $v$ induces an isomorphism from $M_{J'}$ to a submodule of M supplementary to $M_{I-J'}= M_{I-J}\oplus M_i$; consequently, the submodule $M''=v(M_{J'})\oplus M_{I-J}$ is supplementary to $M_i$. By Lemma 1 and the assumption on $u$, the endomorphism $v$ induces an isomorphism from $M_i$ to a submodule of M supplementary to $M''$; consequently, $v$ induces an isomorphism from $M_J= M_i\oplus M_{J'}$ to a submodule supplementary to $M_{I-J}$.

The last assertion follows from the fact that M is the union of the submodules $M_J$, where J runs through the finite subsets of I.

#### Lemma 3 {#alg-viii-s2-lem-3 .statement tag=002B}

Let M be an A-module that is the direct sum of a family $(M_i)_{i\in I}$ of primordial submodules, and let $p$ be a nonzero projector of M. There exists an index $i\in I$ such that $p$ induces an isomorphism from $M_i$ to a direct factor submodule of $p(M)$.

Since $p$ is nonzero, $1_M-p$ is not injective. By Lemma 2, there exists an index $i\in I$ such that $p$ induces an isomorphism from $M_i$ to a direct factor submodule of M. Every projector of M with image $p(M_i)$ defines, by restriction, a projector of $p(M)$ with image $p(M_i)$, so $p(M_i)$ is a direct factor submodule of $p(M)$.

#### Lemma 4 {#alg-viii-s2-lem-4 .statement tag=002C}

Let M be an A-module that is the direct sum of a family $(M_i)_{i\in I}$ of primordial submodules, let L be a primordial A-module, and let N be a direct factor submodule of M. Suppose that N is the direct sum of a family $(N_j)_{j\in J}$ of submodules isomorphic to L, and denote by $I_L$ the set of indices $i\in I$ such that $M_i$ is isomorphic to L. We then have

(1) Card(J) $\leqslant$ Card(I$_L)$.

Let $N_0$ be a submodule of M supplementary to N. The module M is the direct sum of $N_0$ and the family $(N_j)_{j\in J}$. For every $j\in J$, denote by $p_j$ the projector of M with image $N_j$ associated with this decomposition (II, §1, No. 8, p. 209, Proposition 12). For every $i\in I$, denote by $J(i)$ the set of indices $j\in J$ such that $p_j$ induces an isomorphism from $M_i$ to $N_j$. This set is finite: indeed, if $x$ is a nonzero element of $M_i$ and K is a finite subset of J such that $x$ belongs to $N_0+\sum_{k\in K}N_k$, then we have $p_j(x) = 0$ for $j\in J$- K, so that $J(i)$ is contained in K.

Let $j\in J$. By Lemma 3, there exists an index $i\in I$ such that $p_j$ induces an isomorphism from $M_i$ to a direct factor submodule of $N_j$. Since $M_i$ is nonzero and $N_j$ is primordial and therefore indecomposable (VIII, p. 31, Proposition 4), we have $p_j(M_i) = N_j$, and $j$ belongs to $J(i)$. Since the module $M_i$ is isomorphic to $N_j$ and hence to L, the index $i$ belongs to $I_L$. This proves that J is the union of the family of finite sets $(J(i))_{i\in I_L}$. If the set J is infinite, then the set $I_L$ is infinite, and we have (Set Theory, III, §6, No. 3, p. 188, Corollary 3)

Card(J) $\leqslant \sum_{i\in I_L}$ Card(J($i$))$\leqslant$ Card(I$_L)$.

Now, suppose that the set J is finite, and let us prove the lemma by induction on the cardinal of J. If J is empty, there is nothing to prove. Therefore, suppose that J is nonempty, and choose an element $j$ of J. By the above, there exists an index $i\in I_L$ such that $p_j$ induces an isomorphism from $M_i$ to $N_j$. Set $I'= I-\{i\}$ and $J'= J-\{j\}$. The module M is the direct sum of $M_i$ and the kernel of $p_j$. It is also the direct sum of $M_i$ and the submodule $M'=\oplus_{i'\in I'}M_{i'}$. Hence, there exists (II, §1, No. 9, p. 210, Corollary of Proposition 13) an isomorphism $\varphi$ from Ker $p_j= N_0\oplus_{j'\in J'}N_{j'}$ to $M'$. Set $N'=\varphi (\sum_{j'\in J'}N_{j'})$. The submodule $N'$ of $M'$ is a direct factor and is the direct sum of the family $(\varphi (N_{j'}))_{j'\in J'}$ of primordial submodules isomorphic to L. Let us apply the induction hypothesis to $M'$ and $N':$ we have Card(J$')\leqslant$ Card(I$_L-\{i\})$ and therefore inequality (1).

Let us prove Theorem 1. Let $(M_i)_{i\in I}$ and $(N_j)_{j\in J}$ be two families of primordial submodules with direct sum M. Let $I_L$ (resp. $J_L)$ be the set of $i\in I$ (resp. $j\in J)$ such that $M_i$ (resp. $N_j)$ is isomorphic to L. We have Card(J$_L)\leqslant$ Card(I$_L)$ by Lemma 4. By interchanging the roles of I and J, we obtain the inverse inequality and thus the theorem.

The cardinal [M : L] defined in Theorem 1 is called the primordial multiplicity of L in M.

#### Corollary 1 {#alg-viii-s2-lem-4-cor-1 .statement tag=002D}

Let M and N be semiprimordial modules. Then M and N are isomorphic if and only if we have [M : L] = [N : L] for every primordial module L.

#### Corollary 2 {#alg-viii-s2-lem-4-cor-2 .statement tag=00QY}

Let M be a semiprimordial module. Let $(M_i)_{i\in I}$ and $(M'_j)_{j\in J}$ be families of primordial submodules of M such that

$$
M =\bigoplus_{i\in I}M_i=\bigoplus_{j\in J}M'_j
$$

Then there exist an automorphism $u$ of M and a bijection $\varphi$ from I to J such that we have $u(M_i) = M'_{\varphi(i)}$ for every $i\in I$.

For any primordial module L, let $I_L$ (resp. $J_L)$ be the set of indices $i\in I$ (resp. $j\in J)$ such that $M_i$ (resp. $M'_j)$ is isomorphic to L. The nonempty sets of the form $I_L$ (resp. $J_L)$ form a partition of I (resp. J), and for every L, we have

Card(I$_L) =$ Card(J$_L) = [M : L]$;

the corollary follows.

#### Corollary 3 {#alg-viii-s2-lem-4-cor-3 .statement tag=002E}

Let M, N, and P be semiprimordial modules. Suppose that $M\oplus P$ is isomorphic to $N\oplus P$ and that [P : L] is finite for every primordial module L. Then M and N are isomorphic.

By assumption, we have

[M : L] + [P : L] = [N : L] + [P : L]

for every primordial module L. Since [P : L] is finite, it follows by induction from (Set Theory, III, §3, No. 4, p. 162, Proposition 8) that we have [M : L] = [N : L] for every primordial module L. The modules M and N are therefore isomorphic by Corollary 1.

#### Corollary 4 {#alg-viii-s2-lem-4-cor-4 .statement tag=002F}

Let M and N be semiprimordial modules. Suppose that there exists an integer $d >0$ such that $M^d$ is isomorphic to $N^d$. Then the modules M and N are isomorphic.

Let L be a primordial module. By assumption, we have

$$
d[M : L] =d[N : L]
$$

We therefore have the equality [M : L] = [N : L]: indeed, we have $d\mathfrak{a}=\mathfrak{a}$ for every infinite cardinal $\mathfrak{a}($Set Theory, III, §6, No. 3, p. 188, Corollary 4). The modules M and N are then isomorphic by Corollary 1.

#### Corollary 5 {#alg-viii-s2-lem-4-cor-5 .statement tag=002G}

Let M be a semiprimordial module that is the direct sum of a finite family $(M_i)_{i\in I}$ of primordial submodules. For any subset J of I, write $M_J=\bigoplus_{i\in J}M_i$. Let N be a direct factor submodule of M.

a) There exists a subset J of I such that $M_J$ is a submodule supplementary to N.

b) Let J be a subset of I. If $M_J$ is supplementary to N, then the module N is isomorphic to $M_{I-J}$ and is semiprimordial.

We denote by K the set of indices $i\in I$ such that $N\cap M_i= 0$; let us use induction on the cardinal of K. The corollary is clear if M = N. Suppose $M\not= N$. Let $p$ be a projector of M with kernel N. Denote its image by P. It is nonzero, and by Lemma 3, there exists a $j\in I$ such that $p$ induces an isomorphism from $M_j$ to a direct factor submodule of P. We have $N\cap M_j= 0$. Set $N'= N\oplus M_j$. We have $N'= N\oplus p(M_j)$. A submodule supplementary to $p(M_j)$ in P is also supplementary to $N'$ in M, so that $N'$ is a direct factor submodule of M. The set of indices $i\in I$ such that $N'\cap M_i= 0$ is contained in K $-\{j\}$. By the induction hypothesis, there exists a subset $J'$ of I such that $M_{J'}$ is a submodule supplementary to $N'$ in M. Set $J = J'\cup  \{j\}$. Then $M_J$ is a submodule supplementary to N in M.

Let J be a subset of I such that $M_J$ is a submodule supplementary to M in N. Since $M_J$ is also supplementary to $M_{I-J}$, the modules N and $M_{I-J}$ are isomorphic and N is semiprimordial.

#### Corollary 6 {#alg-viii-s2-lem-4-cor-6 .statement tag=002H}

Every finitely generated projective module over a local ring is free.[^2]

Let A be a local ring. The A-module $A_s$ is primordial (VIII, p. 31). If M is a finitely generated projective A-module, then there exist an A-module N and a natural number $n$ such that $M\oplus N$ is isomorphic to $A^n_s$ (II, §2, No. 2, p. 232, Corollary 1). It follows from Corollary 5 that the module M is itself isomorphic to $A^m_s$ for an integer $m$ such that $0\leqslant m\leqslant n$, hence is free.

#### Remark {#alg-viii-s2-n4-rem-1 .statement tag=002I}

Let M and $M'$ be semiprimordial A-modules. It immediately follows from Lemma 4 of VIII, p. 33 that $M'$ is isomorphic to a direct factor submodule of M if and only if we have $[M': L]\leqslant [M : L]$ for every primordial A-module L. In particular, if L is a primordial A-module, [M : L] is the greatest of the cardinals $\mathfrak{a}$ for which there exists a direct factor submodule of M isomorphic to $L^{(\mathfrak{a})}$.

The relation [M : L] = 0 therefore means that there exists no direct factor submodule of M isomorphic to L. This does not exclude the existence of a submodule of M isomorphic to L; it suffices to consider the example where $A =\mathbf{Z}, L =\mathbf{Z}/2\mathbf{Z}$, and $M =\mathbf{Z}/4\mathbf{Z}:$ the $\mathbf{Z}$-modules L and M are primordial and not isomorphic, so that [M : L] = 0 and L is isomorphic to the submodule $2\mathbf{Z}/4\mathbf{Z}$ of M.

### 5. The Structure of Modules of Finite Length

#### Theorem 2 (Krull–Remak–Schmidt) {#alg-viii-s2-thm-2 .statement tag=00RY}

Let A be a ring and M an A-module of finite length.

a) There exists a finite family $(M_i)_{i\in I}$ of indecomposable submodules of M such that $M =\bigoplus_{i\in I}M_i$, and the module M is semiprimordial.

b) Let $(M_i)_{i\in I}$ and $(M'_j)_{j\in J}$ be two finite families of indecomposable submodules of M such that $M =\bigoplus_{i\in I}M_i=\bigoplus_{j\in J}M'_j$. There exist a bijection $\sigma$ from I to J and an automorphism $u$ of M such that we have $u(M_i) = M'_{\sigma(i)}$ for every $i\in I$.

c) Let N be a direct factor submodule of M, and let $(M_i)_{i\in I}$ be a finite family of indecomposable submodules of M with direct sum M. There exists a subset J of I such that $\bigoplus_{i\in I-J}M_i$ is supplementary to N. The module N is isomorphic to $\bigoplus_{j\in J}M_j$.

d) Let N be an A-module. If there exists an integer $d >0$ such that the modules $M^d$ and $N^d$ are isomorphic, then the modules M and N are isomorphic.

e) Let N and P be A-modules of finite length. If the modules $M\oplus P$ and $N\oplus P$ are isomorphic, then M and N are isomorphic.

A module of finite length is both Artinian and Noetherian (VIII, p. 2, Proposition 1). Moreover, for a module of finite length, being indecomposable or primordial amounts to the same (VIII, p. 31, Proposition 4). Assertion a) then follows from Proposition 3 of VIII, p. 30. Assertions b), c), and e) follow from, respectively, Corollaries 2, 5, and 3 of Theorem 1 of VIII, p. 32. Finally, assertion d) follows from Corollary 4 of VIII, p. 35 because under the assumptions of d), the module N has finite length and is therefore semiprimordial by a).

#### Theorem 3 {#alg-viii-s2-thm-3 .statement tag=002J}

Let K be a commutative field, A a K-algebra, and M and N modules of finite length. Let $K'$ be a nonzero commutative K-algebra such that the $A_{(K')}$-modules $M_{(K')}$ and $N_{(K')}$ are isomorphic. Then the A-modules M and N are isomorphic.

a) First, suppose that the algebra $K'$ has finite degree $d$ over K. Then the A-module $M_{(K')}$ is isomorphic to $M^d$ and the A-module $N_{(K')}$ is isomorphic to $N^d$, so that the A-modules $M^d$ and $N^d$ are isomorphic. By Theorem 2, d), the A-modules M and N are isomorphic.

b) Now, suppose that the K-algebra $K'$ is generated by finitely many elements. Choose a maximal ideal $\mathfrak{m}$ of $K'$, and set $K''= K'/\mathfrak{m}$. By Hilbert’s Nullstellensatz (VIII, p. 462, Corollary 1 of Theorem 1$), K''$ is a finite-degree extension of K. By extension of scalars from $K'$ to $K''$, we deduce from the $A_{(K')}$-linear isomorphism $M_{(K')}\rightarrow N_{(K')}$ an $A_{(K'')}$-linear isomorphism $M_{(K'')}\rightarrow N_{(K'')}$. By part a) of the proof, the A-modules M and N are isomorphic.

c) Finally, let us treat the general case. Let $u: M_{(K')}\rightarrow N_{(K')}$ be an isomorphism of $A_{(K')}$-modules and $v: N_{(K')}\rightarrow M_{(K')}$ the inverse isomorphism. Denote by $\mathscr{E}$ the set of K-subalgebras of $K'$ generated by finitely many elements. If E is such a subalgebra, then $A_{(E)}$ is identified with a subring of $A_{(K')}$, and $M_{(E)}$ and $N_{(E)}$ are identified with $A_{(E)}$-submodules of $M_{(K')}$ and $N_{(K')}$, respectively (II, §7, No. 7, p. 306); moreover, $M_{(K')}$ and $N_{(K')}$ are unions of right directed families $(M_{(E)})_{E\in\mathscr{E}}$ and $(N_{(E)})_{E\in\mathscr{E}}$, respectively. The A-modules M and N are of finite length, hence finitely generated; let S be a finite generating subset of the A-module M and T a finite generating subset of the A-module N. There exists a K-algebra $E\in \mathscr{E}$ such that we have $u(1\otimes s)\in N_{(E)}$ for every $s\in S$ and $v(1\otimes t)\in M_{(E)}$ for every $t\in T$. It follows by linearity that we have $u(M_{(E)})\subset N_{(E)}$ and $v(N_{(E)})\subset M_{(E)}$. The maps $u$ and $v$ then induce inverse bijections from $M_{(E)}$ to $N_{(E)}$ and from $N_{(E)}$ to $M_{(E)}$. These bijections are clearly $A_{(E)}$-linear. Thus, the $A_{(E)}$-modules $M_{(E)}$ and $N_{(E)}$ are isomorphic. By part b) of the proof, the A-modules M and N are isomorphic.

#### Remark {#alg-viii-s2-n5-rem-1 .statement tag=002K}

Let E and F be two finite-dimensional vector spaces over a commutative field K, and let $K'$ be an extension of K. Let $u$ be an endomorphism of E and $v$ an endomorphism of F, and let $u_{(K')}$ and $v_{(K')}$ be the endomorphisms of $E_{(K')}$ and $F_{(K')}$ obtained by extension of scalars. It follows from Corollaries 1 and 2 of VII, §5, No. 3, p. 32 that the endomorphisms $u$ and $v$ are similar if and only if the endomorphisms $u_{(K')}$ and $v_{(K')}$ are. This also follows from Theorem 3 above applied to the algebra A = K[X] and the A-modules $M = E_u$ and $N = F_v$ (VII, §5, No. 1, p. 29).

### Exercises {#alg-viii-s2-exercises}

See the [exercises for § 2](exercises/s2/).

[^1]: Note added in translation: some authors use the terminology “module with local endomorphism ring” for “primordial module.”
[^2]: It can be shown that every projective module over a local ring is free (VIII, p. 42, Exercise 18).
