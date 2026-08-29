---
book: ts
book_title: Théories spectrales
chapter: I
chapter_title: ALGÈBRES NORMÉES
section: 1
section_title: Spectres et caractères
lang: en
source: ts-i-ii-fr
book_pages: TS I.1-TS I.15, TS I.153-TS I.154
pdf_pages: 0014-0028, 0166-0167
extraction: native
subsections:
    - "no": 1
      title: Algèbres unifères
      page: 1
      pdf_page: 14
    - "no": 2
      title: Spectre d’un élément dans une algèbre unifère
      page: 2
      pdf_page: 15
    - "no": 3
      title: Résolvante
      page: 3
      pdf_page: 16
    - "no": 4
      title: Spectre d’un élément dans une algèbre
      page: 4
      pdf_page: 17
    - "no": 5
      title: Sous-algèbres pleines
      page: 5
      pdf_page: 18
    - "no": 6
      title: Caractères d’une algèbre unifère commutative
      page: 6
      pdf_page: 19
    - "no": 7
      title: Cas des algèbres sans élément unité
      page: 9
      pdf_page: 22
    - "no": 8
      title: Idéaux primitifs
      page: 11
      pdf_page: 24
statements: 33
exercises: 8
content_sha256: ba4faed48a44431108215f0ef740029a61d76cccd70f4a61007ff33d6daafaad
translated_from: content/fr/ts/I/01_s1_spectres_et_caracteres.md
source_lang: fr
translation_method: machine
source_content_sha256: 705ff1d1d239ae09b6a762f05fe80c3ebe2750db91e7b18bf20b0b956e8064c8
translation_model: gpt-5.4, gpt-5-6-mini
translation_run: translate-en-mt-792e7eaa
glossary_version: 34
glossary_terms_sha256: 396f3efaa9469dbbc12664ab3810b1da18ecd02197556f703811c129b92ec137
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 1. SPECTRA AND CHARACTERS

In this paragraph, the letter K denotes a commutative field. If E and F are vector spaces over K, we write $E\otimes F = E\otimes_KF$.

### 1. Unital algebras

A unital algebra over K is defined to be a pair $(A, e)$ where A is an algebra over K with a unit element and $e$ the unit element of A. Since $e$ is uniquely determined by A, we shall sometimes say, by abuse of language, that A is a unital algebra. If $(A, e)$ and $(A', e')$ are unital algebras, a unital morphism of $(A, e)$ into $(A', e')$ is defined to be a morphism $\varphi$ of A into $A'$ such that $\varphi (e) =e'$. A unital subalgebra of $(A, e)$ is a pair $(A', e)$, where $A'$ is a subalgebra of A containing $e$.

We shall often denote the unit element by 1.

#### Lemma 1 {#ts-i-s1-lem-1 .statement tag=024R}

Let A be an algebra. For every idempotent $j$ of A, the subspace $jAj$ of A is the set of $x\in A$ such that $xj=jx=x$. It is a subalgebra of A having $j$ as unit element.

The proof is elementary.

### 2. Spectrum of an element in a unital algebra

#### Definition 1 {#ts-i-s1-def-1 .statement tag=024S}

Let A be a unital algebra over K, and let $e$ be its unit element. For every $x\in A$, the spectrum of $x$ relative to A is the set of $\lambda \in K$ such that $\lambda e-x$ is not invertible.

The spectrum of $x$ will be denoted by Sp$_A(x)$, or Sp($x$) if no confusion can result. The complement of Sp$_A(x)$ in K is called the resolvent set of $x$.

#### Remark 1 {#ts-i-s1-n2-rem-1 .statement tag=024T}

If $A =\{0\}$, then Sp(0) $=\emptyset$.

#### Remark 2 {#ts-i-s1-n2-rem-2 .statement tag=024U}

If $A\not=\{0\}$, then Sp($\lambda e$) $=\{\lambda \}$ for every $\lambda \in K$.

#### Remark 3 {#ts-i-s1-n2-rem-3 .statement tag=024V}

For $x\in A$ to be invertible, it is necessary and sufficient that $0\notin$ Sp($x$).

#### Remark 4 {#ts-i-s1-n2-rem-4 .statement tag=024W}

Let $R\in K(X)$ be a rational fraction and let $x\in A$ be an element which can be substituted in R, that is to say (A, IV, p. 20), that there exist P and $Q\in K[X]$ such that $R = P/Q$ and $Q(x)$ is invertible; one can then form the element $R(x) = P(x)\cdot Q(x)^{-1}= Q(x)^{-1}\cdot P(x)$ of A; it does not depend on the choice of P and Q. One has $0\notin$ Q(Sp($x$)), so that every element of Sp($x$) can be substituted in R.

One has R(Sp($x$))$\subset$ Sp(R($x$)). For let $\lambda \in$ Sp($x$); there exists a polynomial $P_1$ such that $R(\lambda )-R(X) = (\lambda -X)P_1(X)/Q(X)$; then, $R(\lambda )e-$ $R(x) = (\lambda e-x)(P_1(x)/Q(x))$, so that $R(\lambda )-R(x)$ is not invertible, hence $R(\lambda )\in$ Sp(R($x$)).

Conversely, suppose that the field K is algebraically closed. Suppose first that R is not constant and let us prove that one has Sp(R($x$)) $=$ R(Sp($x$)). Let $\mu\in$ Sp(R($x$)). Since R is not constant, $P-\mu Q$ is not the zero polynomial; let $\mu Q-P =\alpha \prod(\lambda_i-X)$ be a decomposition into factors of degree 1, so that $\mu e-R(x) =$ $\alpha \prod(\lambda_ie-x)Q(x)^{-1}$. Since $\mu e-R(x)$ is not invertible, there exists $i$ such that $\lambda_ie-x$ is not invertible, hence $\lambda_i\in$ Sp($x$), and then $R(\lambda_i) =\mu\in$ R(Sp($x$)).

When R is constant, the equality Sp(R($x$)) $=$ R(Sp($x$)) also holds, provided that Sp($x$) is nonempty.

#### Remark 5 {#ts-i-s1-n2-rem-5 .statement tag=024X}

Suppose that the algebra A is nonzero. Let $x\in A$ be a nilpotent element. Let $n$ be an integer such that $x^n= 0$. The spectrum of $x^n$ reduces to 0, hence the same is true of the spectrum of $x$ by Remark 4.

#### Remark 6 {#ts-i-s1-n2-rem-6 .statement tag=024Y}

Let A and B be unital algebras over K and $\varphi : A\rightarrow B$ a unital morphism. For every $x\in A$, one has Sp$_B(\varphi (x))\subset$ Sp$_A(x)$.

#### Remark 7 {#ts-i-s1-n2-rem-7 .statement tag=024Z}

Let A be a unital algebra, R its radical (A, VIII, p. 150, Def. 2), and let $\varphi$ be the canonical morphism of A onto $B = A/R$. If $x\in A$, one has Sp$_B(\varphi (x)) =$ Sp$_A(x)$. In fact, it is enough to prove that if $\varphi (x)$ is invertible in B, then $x$ is invertible in A. Now, if $y\in A$ is such that $\varphi (x)\varphi (y) =\varphi (y)\varphi (x) =\varphi (e)$, one has $xy\in e+ R,yx\in e+ R$, hence $xy$ and $yx$ are invertible (A, VIII, p. 151, Th. 1) and consequently $x$ is invertible. In particular, if $x\in R$, one has Sp$_A(x) =\{0\}$ if $A\not=\{0\}$.

#### Remark 8 {#ts-i-s1-n2-rem-8 .statement tag=0250}

Let $(B_i)_{i\in I}$ be a family of unital algebras, with $B_i= (A_i, e_i)$ for $i\in I$. Put $A =\prod_iA_i,e= (e_i)_{i\in I}$. Then $(A, e)$ is a unital algebra called the product of the $B_i$. If $x= (x_i)_{i\in I}\in A$, one has Sp$_A(x) =\bigcup_i$ Sp$_{A_i}(x_i)$.

#### Example 1 {#ts-i-s1-n2-exa-1 .statement tag=0251}

Let X be a set and let $A = K^X$ be the algebra of functions with values in K defined on X. The spectrum of an element $f$ of A is the set of values of $f$.

#### Example 2 {#ts-i-s1-n2-exa-2 .statement tag=0252}

Let A be a unital algebra of finite rank over K. For $x\in A$ to be invertible, it is necessary and sufficient that the linear mapping $y\mapsto xy$ of A into A should have nonzero determinant. It follows that the spectrum of $x$ is the set of roots of the characteristic polynomial of $x$ (A, III, p. 110). If A is the endomorphism algebra of a finite-dimensional vector space V over K, the spectrum of $x$ is therefore the set of eigenvalues of $x$. This is not always so when V is of infinite dimension (cf. I, p. 153, exercise 2).

### 3. Resolvent

#### Definition 2 {#ts-i-s1-def-2 .statement tag=0253}

Let A be a unital algebra over K and $x\in A$. For every $\lambda \in K$ - Sp($x$), one sets

$$
R(x, \lambda ) = (\lambda e-x)^{-1}
$$

The mapping of K - Sp($x$) into A given by $\lambda \mapsto R(x, \lambda )$ is called the resolvent of $x$.

For fixed $x$, the values of $R(x, \lambda )$ are pairwise permutable. If $\lambda , \mu\in K$, one has:

$$
(\lambda -\mu)e= (\lambda e-x)-(\mu e-x)
$$

hence, if $\lambda , \mu\in K$ - Sp($x$), one has the relation

$$
(\lambda -\mu)R(x, \lambda )R(x, \mu) = R(x, \mu)-R(x, \lambda ) \tag{1}
$$

If $x, y\in A$ and $\lambda \in K$, one has:

$$
y-x= (\lambda e-x)-(\lambda e-y)
$$

hence, if $\lambda \in K$ - (Sp($x$)$\cup$ Sp($y$)), one has the relation

$$
R(y, \lambda )(y-x)R(x, \lambda ) = R(y, \lambda )-R(x, \lambda ) \tag{2}
$$

### 4. Spectrum of an element in an algebra

Let A be an algebra over K. Recall (A, III, p. 4) that one defines on the vector space $\widetilde{A} = K\times A$ an algebra structure such that:

$$
(\lambda , a)(\mu, b) = (\lambda \mu, \lambda b+\mu a+ab)
$$

Let $e= (1,0)$. Then $(\widetilde{A}, e)$ is a unital algebra said to be deduced from A by adjunction of a unit element. The algebra A is identified with the two-sided ideal $\{0\} \times A$ of $\widetilde{A}$; the algebra A is commutative if and only if $\widetilde{A}$ is.

If $A'$ is a second algebra over K, $(\widetilde{A}', e')$ the unital algebra deduced from $A'$ by adjunction of a unit element, and $\varphi$ a morphism of A into $A'$, there exists one and only one unital morphism of $(\widetilde{A}, e)$ into $(\widetilde{A}', e')$ extending $\varphi$.

Let A be an algebra over K and $x\in$ A. The spectrum of $x$ relative to A is defined to be the spectrum of $x$ relative to the unital algebra $\widetilde{A}$ deduced from A by adjunction of a unit element. This set will be denoted by Sp$'_A(x)$, or Sp$'(x)$ if no confusion results. One has $0\in$ Sp$'_A(x)$ whatever $x\in A$ may be.

If $\varphi$ is a morphism of A into an algebra B, one has Sp$'_B(\varphi (x))\subset$ Sp$'_A(x)$.

#### Remark 1 {#ts-i-s1-n4-rem-1 .statement tag=0254}

Let $(A,1)$ be a unital algebra. If $x\in A$, one has

Sp$'_A(x) =$ Sp$_A(x)\cup  \{0\}$. Indeed, one verifies that $(e-1)\cdot A = A\cdot (e-1) = 0$, hence that $\widetilde{A}$ is the unital algebra product of A and $K(e-1)$. Our assertion therefore follows from Remark 8 of I, p. 3.

#### Remark 2 {#ts-i-s1-n4-rem-2 .statement tag=0255}

It follows from Remark 1 that, if B is an algebra over K and if $x\in B$, one has:

Sp$'_B(x) =$ Sp$_{\widetilde{B}}(x) =$ Sp$_{\widetilde{B}}(x)\cup  \{0\}=$ Sp$'_{\widetilde{B}}(x)$.

#### Remark 3 {#ts-i-s1-n4-rem-3 .statement tag=0256}

If $x$ belongs to the radical of A (A, VIII, p. 430, def. 3), one has Sp$'_A(x) =\{0\}$. This follows from Remark 7 of I, p. 3.

#### Proposition 1 {#ts-i-s1-prop-1 .statement tag=0257}

Let A be an algebra and $x, y\in A$. One has Sp$'(xy) =$ Sp$'(yx)$.

By passing to $\widetilde{A}$, we reduce to the case where A possesses a unit element $e$. It is then enough to prove that, if $\lambda \not= 0$ is such that $xy-\lambda e$ admits an inverse $u$, then $yx-\lambda e$ is invertible. Put $z=yux-e$. Since $xyu=\lambda u+e$, one has

$$
(yx-\lambda e)z=y(xyu)x-yx-\lambda yux+\lambda e
$$

$$
=y(\lambda u+e)x-yx-\lambda yux+\lambda e=\lambda e
$$

and analogously $z(yx-\lambda e) =\lambda e$. Since $\lambda \not= 0$, one sees that $yx-\lambda e$ is invertible.

If A is a unital algebra and if $x, y\in A$, the preceding proposition implies that Sp($xy$)$\cup \{0\}=$ Sp($yx$)$\cup \{0\}$, but one can have Sp($xy$)$\not=$ Sp($yx$) (cf. I, p. 153, exer. 3).

### 5. Full subalgebras

Let A be a unital algebra over K.

#### Definition 3 {#ts-i-s1-def-3 .statement tag=0258}

A full subalgebra of A is called a unital subalgebra B such that every element of B which is invertible in A is invertible in B.

In other words, B is a full subalgebra of A if and only if Sp$_B(x) =$ Sp$_A(x)$ for every $x\in B$.

The intersection of a family of full subalgebras of A is a full subalgebra of A.

Let M be a subset of A. The intersection of the full subalgebras of A containing M is the smallest full subalgebra of A containing M; it is called the full subalgebra of A generated by M. The commutant $M'$ of M in A is a full subalgebra of A (for, if $x$ is invertible in A and commutes with M, then $x^{-1}$ commutes with M). Hence the bicommutant $M''$ of M is a full subalgebra of A which contains the full subalgebra of A generated by M.

If the elements of M are pairwise commuting, one has $M\subset M'$ and $M''\subset M'''$; the algebra $M''$ is therefore commutative and the same is then true of the full algebra generated by M.

A maximal commutative subalgebra of A is a full subalgebra, since it is equal to its commutant.

#### Lemma 2 {#ts-i-s1-lem-2 .statement tag=0259}

Let $(x_{\lambda})_{\lambda\in\Lambda}$ be a family of pairwise commuting elements of A. The full subalgebra generated by $(x_{\lambda})$ is the set of elements of the form $R((x_{\lambda}))$, where $R\in K((X_{\lambda}))$ runs through the set of rational fractions in which the family $(x_{\lambda})$ is substitutable.

Let B be the full subalgebra of A generated by the family $(x_{\lambda})$, and let us denote by $B_1$ the set of elements of the form $R((x_{\lambda}))$, where $R((X_{\lambda}))$ is a rational fraction in which $(x_{\lambda})$ can be substituted. Explicitly, $B_1$ is the set of elements of A of the form $P((x_{\lambda}))Q((x_{\lambda}))^{-1}$, where $P,Q\in K[(X_{\lambda})]$ and $Q((x_{\lambda}))$ is invertible in A. The set $B_1$ is a unital subalgebra of A containing the family $(x_{\lambda})$. It is a full subalgebra: if $P((x_{\lambda}))Q((x_{\lambda}))^{-1}$ is invertible in A, then $P((x_{\lambda}))$ is invertible in A and the inverse $Q((x_{\lambda}))P((x_{\lambda}))^{-1}$ of $P((x_{\lambda}))Q((x_{\lambda}))^{-1}$ belongs to $B_1$. Hence $B\subset B_1$. On the other hand, if $P,Q\in K[(X_{\lambda})]$, and if $Q((x_{\lambda}))$ is invertible in A, then $P((x_{\lambda}))\in B$ and $Q((x_{\lambda}))\in B$, hence $Q((x_{\lambda}))^{-1}\in B$ and $P((x_{\lambda}))Q((x_{\lambda}))^{-1}\in B$, hence $B_1\subset B$.

### 6. Characters of a commutative unital algebra

#### Definition 4 {#ts-i-s1-def-4 .statement tag=025A}

Let A be a commutative unital algebra over K. A unital character is a unital morphism of A into K.

When no confusion can result from this, we shall simply say character instead of unital character. The set of unital characters of A is denoted by $\mathsf{X}(A)$. If A is the zero algebra, then $\mathsf{X}(A)$ is empty.

Let A and B be commutative unital algebras over K and $h$ a unital morphism of A into B. The map $\chi \mapsto \chi \circ h$ of $\mathsf{X}(B)$ into $\mathsf{X}(A)$ is denoted by $\mathsf{X}(h)$. If $k$ is a morphism of B into a commutative unital algebra, one has $\mathsf{X}(k\circ h) =\mathsf{X}(h)\circ \mathsf{X}(k)$. The map $\mathsf{X}$(Id$_A$) is the identity map of $\mathsf{X}(A)$.

If $h$ is surjective, $\mathsf{X}(h)$ is a bijection of $\mathsf{X}(B)$ onto the set of characters of A which vanish on the kernel of $h$.

Let $(A_1, e_1), . . . ,(A_n, e_n)$ be commutative unital algebras over K and let A be the unital algebra $A_1\times  \cdots  \times A_n$, with unit element $(e_1, . . . , e_n)$. For each $i$, identify $A_i$ with an ideal of A and let $\pi_i$ be the canonical mapping of A onto $A_i$. Then $\mathsf{X}(\pi_i)$ is a bijection of $\mathsf{X}(A_i)$ onto the set $\mathsf{X}_i$ of characters of A vanishing on $\prod_{j\not=i}A_j$. The sets $\mathsf{X}_i$ are pairwise disjoint. On the other hand, let $\chi \in \mathsf{X}(A)$. Since $1 =\sum\chi (e_i)$, there exists $i$ such that $\chi (e_i)\not= 0$. For every $j\not=i$ and every $y\in A_j$, one has $\chi (e_i)\chi (y) =\chi (e_iy) =\chi (0) = 0$, hence $\chi (A_j) = 0$. Thus, $\chi$ vanishes on $\prod_{j\not=i}A_j$, so that $\mathsf{X}(A)$ is the union of the $\mathsf{X}_i$.

Let B be the unital algebra $A_1\otimes  \cdots  \otimes A_n$. Let $h_i$ denote the canonical morphism $A_i\rightarrow B$. Then

$$
\chi \mapsto (\chi \circ h_1, . . . , \chi \circ h_n)
$$

is a map from $\mathsf{X}(B)$ into $\mathsf{X}(A_1)\times  \cdots  \times \mathsf{X}(A_n)$, and

$$
(\chi_1, . . . , \chi_n)\mapsto \chi_1\otimes  \cdots  \otimes \chi_n
$$

is a map from $\mathsf{X}(A_1)\times  \cdots  \times \mathsf{X}(A_n)$ into $\mathsf{X}(B)$. One verifies that these maps are reciprocal bijections, by means of which one identifies $\mathsf{X}(B)$ with $\mathsf{X}(A_1)\times  \cdots  \times \mathsf{X}(A_n)$.

Let A be a commutative unital algebra over K. Let Y be the set of ideals of codimension 1 of A. For every $\chi \in \mathsf{X}(A)$, one has Ker($\chi$ )$\in Y$. The mapping $\chi \mapsto$ Ker($\chi$ ) is a bijection of $\mathsf{X}(A)$ onto Y. In fact, if $I\in Y$, there exists a unique isomorphism of the unital K-algebra $A/I$ onto K and the composite morphism

$$
A\longrightarrow A/I\longrightarrow K
$$

is the unique character of A with kernel I.

#### Definition 5 {#ts-i-s1-def-5 .statement tag=025B}

Let A be a commutative unital algebra over K. For every $x\in A$, let $\mathscr{G}_A(x)$, or simply $\mathscr{G}(x)$, denote the mapping $\chi \mapsto$ $\chi (x)$ of $\mathsf{X}(A)$ into K. It is called the Gelfand transform of $x$.

The mapping $\mathscr{G}$ is a unital morphism of A into the unital algebra $K^{\mathsf{X}(A)}$ of mappings from $\mathsf{X}(A)$ into K. It is called the Gelfand transform of A.

If $x\in$ A, the image of the Gelfand transform $\mathscr{G}_A(x)$ of $x$ is contained in Sp$_A(x)$. Indeed, let $\chi \in \mathsf{X}(A)$; since $\chi (x-\chi (x)e) =$ 0, the element $x-\chi (x)e$ is not invertible.

Let B be a commutative unital algebra over K and $h$ a unital morphism of A into B; then $\mathsf{X}(h) :\mathsf{X}(B)\rightarrow \mathsf{X}(A)$ defines a unital morphism $h_*: K^{\mathsf{X}(A)}\rightarrow K^{\mathsf{X}(B)}$, and the diagram:

$\mathscr{G}\leftarrow_A\mathsf{X}(A)$

A $\rightarrow K$ (3) $\rightarrow \leftarrow_h\rightarrow \leftarrow_{h_*}$

$\mathscr{G}\leftarrow_B\mathsf{X}(B)$

B $\rightarrow K$

is commutative. Indeed, for every $x\in A$ and every $\chi \in \mathsf{X}(B)$, we have:

$$
\mathscr{G}_B(h(x))(\chi ) =\chi (h(x)) = (\chi \circ h)(x)
$$

$$
= (\mathsf{X}(h)(\chi ))(x)
$$

$$
=\mathscr{G}_A(x)(\mathsf{X}(h)(\chi )) \tag{4}
$$

$$
=h_*(\mathscr{G}_A(x))(\chi )
$$

Now suppose that K is a topological field. One then endows $\mathsf{X}(A)$ with the topology of simple convergence on A (cf. EVT, III, p. 14, Example 1), and the topological space $\mathsf{X}(A)$ is called the space of characters of A. The topology of $\mathsf{X}(A)$ is therefore the least fine for which the functions $\mathscr{G}_A(x)$ for $x\in A$ are continuous, and the mapping $\chi \mapsto (\chi (a))_{a\in A}$ identifies the space $\mathsf{X}(A)$ with a subset of $K^A$.

When K = $\mathbf{R}$ or $\mathbf{C}$, this topology is the topology induced on $\mathsf{X}(A)\subset A^*$ by the weak topology $\sigma (A^*,A)$ on $A^*$ (EVT, II, p. 45, Def. 2); in this respect, we shall also say that it is the weak topology on $\mathsf{X}(A)$.

If $h$ is a unital morphism of A into B, the mapping $\mathsf{X}(h) :\mathsf{X}(B)\rightarrow \mathsf{X}(A)$ is continuous. If $h$ is surjective, the image of $\mathsf{X}(h)$, namely the set of characters of A vanishing on the kernel of $h$, is closed in $\mathsf{X}(A)$; on the other hand, the topology on $\mathsf{X}(h)(\mathsf{X}(B))$ deduced from that of $\mathsf{X}(B)$ by the bijection $\mathsf{X}(h)$ is the topology of simple convergence in A, that is to say the topology induced by that of $\mathsf{X}(A)$; in other words, $\mathsf{X}(h)$ is a homeomorphism of $\mathsf{X}(B)$ onto a closed subset of $\mathsf{X}(A)$.

If $A_1, . . . ,A_n$ are commutative unital algebras over K, the space $\mathsf{X}(A_1\times  \cdots  \times A_n)$ is thus identified with the topological sum of $\mathsf{X}(A_1), . . . ,\mathsf{X}(A_n)$. Analogously, $\mathsf{X}(A_1\otimes  \cdots  \otimes A_n)$ is identified with the topological product $\mathsf{X}(A_1)\times  \cdots  \times \mathsf{X}(A_n)$.

### 7. Case of algebras without unit element

#### Definition 6 {#ts-i-s1-def-6 .statement tag=025C}

Let A be a commutative algebra over K. A character of A is, by definition, an algebra morphism of A into K.

The set of characters of A will be denoted by $\mathsf{X}'(A)$.

The zero mapping is an algebra morphism. If A has a unit element $e$, a nonzero algebra morphism of A into K is unital, that is to say, is a unital character of K in the sense of Definition 4: indeed, in order that $\chi \in \mathsf{X}'(A)$ be nonzero, it is necessary and sufficient that $\chi (e) = 1$.

We shall put $\mathsf{X}(A) =\mathsf{X}'(A)-\{0\}$; from the foregoing, this notation is compatible with that introduced when A is unital.

If $h: A\rightarrow B$ is a morphism of commutative algebras, the mapping $\chi \mapsto \chi \circ h$ is a mapping $\mathsf{X}'(h) :\mathsf{X}'(B)\rightarrow \mathsf{X}'(A)$. It maps 0 to 0. If $k: B\rightarrow C$ is a morphism of commutative algebras, then one has $\mathsf{X}'(k\circ h) =\mathsf{X}'(h)\circ \mathsf{X}'(k)$. If $h$ is surjective, $\mathsf{X}'(h)$ is a bijection of $\mathsf{X}'(B)$ onto the set of characters of A vanishing on the kernel of $h$. Let $A_1, . . . ,A_n$ be commutative algebras, $A = A_1\times  \cdots  \times A_n$ and $\pi : A\rightarrow A_i$ the canonical morphism; then $\mathsf{X}'(\pi_i)$ is a bijection of $\mathsf{X}'(A_i)$ onto a subset $\mathsf{X}'_i$ of $\mathsf{X}'(A)$, namely the set of characters of A vanishing on $\prod_{j\not=i}A_j$; one sees as in No.$^o6$ that $\mathsf{X}'(A)$ is the union

of the $\mathsf{X}'_i$; on the other hand, $\mathsf{X}'_i\cap \mathsf{X}'_j=\{0\}$ for $i\not=j$; in particular the $\mathsf{X}'_i-\{0\}$ form a partition of $\mathsf{X}'(A)-\{0\}=\mathsf{X}(A)$.

For every $x\in A$, let $\mathscr{G}'_A(x)$, or simply $\mathscr{G}'(x)$, be the mapping $\chi \mapsto \chi (x)$ of $\mathsf{X}'(A)$ into K. The mapping $\mathscr{G}'$ is a morphism of A into the algebra $A_1$ of mappings $\mathsf{X}'(A)\rightarrow K$ vanishing at 0. Let B be a commutative algebra, $B_1$ the algebra of mappings $\mathsf{X}'(B)\rightarrow$ K vanishing at 0, and $h$ a morphism of A into B; then $\mathsf{X}'(h)$ defines a morphism $h_1: A_1\rightarrow B_1$, and one has $h_1\circ \mathscr{G}'_A=\mathscr{G}'_B\circ h$. One denotes by $\mathscr{G}_A(x)$, or simply $\mathscr{G}(x)$, the restriction of $\mathscr{G}'_A(x)$ to $\mathsf{X}(A)$, and calls it the Gelfand transform of $x$.

Let $\widetilde{A}$ be the unital algebra deduced from A by adjunction of a unit element. By restriction, every character of $\widetilde{A}$ defines a character of A; conversely, every character of A extends in a unique way to a character of $\widetilde{A}$. This defines a canonical bijection of $\mathsf{X}'(A)$ onto $\mathsf{X}(\widetilde{A})$, by which these two sets are identified. The character 0 of A is identified with the unique character of $\widetilde{A}$ with kernel A.

If $x\in A$ and $\chi \in \mathsf{X}'(A)$, one has $\chi (x)\in$ Sp$_{\widetilde{A}}(x)$, hence $\chi (x)\in$ Sp$'_A(x)$.

#### Lemma 3 {#ts-i-s1-lem-3 .statement tag=025D}

The mapping $\chi \mapsto$ Ker($\chi$ ) is a bijection of $\mathsf{X}(A)$ onto the set of regular ideals of codimension 1 of A.

Let us recall (A, VIII, p. 426, Definition 1) that an ideal I of A is said to be regular if the quotient algebra $A/I$ admits a unit element.

Let us prove the lemma. On the one hand, $\mathsf{X}(A)$ is identified with the set of characters of $\widetilde{A}$ which are not zero on A. On the other hand, by A, VIII, p. 428, Prop. 4, the mapping $I\mapsto A\cap I$ is a bijection of the set of maximal ideals of $\widetilde{A}$ distinct from A onto the set of regular maximal ideals of A. The lemma then follows from the results of No. 6.

Now suppose that K is a topological field. We then endow $\mathsf{X}'(A)$ with the topology of simple convergence on A; the notation $\mathsf{X}'(A)$ will henceforth denote the topological space thus obtained. When $K =\mathbf{R}$ or $\mathbf{C}$, we shall also call it the weak topology. For every $x\in A$, the function $\mathscr{G}'_A(x)$ on $\mathsf{X}'(A)$ is continuous.

If $h$ is a morphism from A into B, the mapping $\mathsf{X}'(h) :\mathsf{X}'(B)\rightarrow$ $\mathsf{X}'(A)$ is continuous. If $h$ is surjective, $\mathsf{X}'(h)$ is a homeomorphism of $\mathsf{X}'(B)$ onto its image, and this image is closed in $\mathsf{X}'(A)$.

Let $A = A_1\times  \cdots  \times A_n$; with the same notation as above, $\mathsf{X}'(\pi_i)$ is a homeomorphism of $\mathsf{X}'(A_i)$ onto $\mathsf{X}'_i$ and $\mathsf{X}'_i$ is closed in $\mathsf{X}'(A)$. Hence $\mathsf{X}'_i-\{0\}$ is open in $\mathsf{X}'(A)$; the $\mathsf{X}'(\pi_i)$ define a continuous mapping of the sum space S of the $\mathsf{X}'(A_i)$ onto $\mathsf{X}'(A)$, and one immediately verifies that a union of neighbourhoods of the points $0\in \mathsf{X}'(A_1), . . . ,0\in \mathsf{X}'(A_n)$ has for image a neighbourhood of $0\in \mathsf{X}'(A)$; from all this it follows that $\mathsf{X}'(A)$ is canonically identified with a quotient space of S. In particular, the space $\mathsf{X}(A)$ is identified with the sum space of the $\mathsf{X}(A_i)$.

The canonical bijection of $\mathsf{X}'(A)$ onto $\mathsf{X}(\widetilde{A})$ is a homeomorphism. Let B be a unital algebra over K and $B'$ the underlying algebra; then the space $\mathsf{X}(B)$ is identified with the subspace $\mathsf{X}(B')$ of $\mathsf{X}'(B')$.

### 8. Primitive Ideals

Let A be an algebra over K and E a vector space over K. A representation of A in E is a morphism from A into the algebra $\mathscr{L}(E)$ of endomorphisms of E. An injective representation is said to be faithful. Let $\pi_1$ and $\pi_2$ be representations of A in spaces $E_1,E_2$. A morphism from $\pi_1$ into $\pi_2$ is a K-linear mapping $u: E_1\rightarrow E_2$ such that $u(\pi_1(a)x) =\pi_2(a)u(x)$ for all $a\in A$ and $x\in E_1$. The representations are said to be equivalent if there exists a morphism from $\pi_1$ into $\pi_2$ which is an isomorphism of vector spaces. Its inverse is then a morphism from $\pi_2$ into $\pi_1$. A representation $\pi$ of A in E is said to be irreducible if $E\not=\{0\}$ and if the only vector subspaces of E stable under $\pi (A)$ are $\{0\}$ and E.

#### Example {#ts-i-s1-n8-exa-1 .statement tag=025E}

The zero mapping of A into $\mathscr{L}(E)$ is a representation, called trivial, of A. It is irreducible if and only if E is of dimension 1.

#### Lemma 4 {#ts-i-s1-lem-4 .statement tag=025F}

Let $\pi$ be a nontrivial irreducible representation of A in E. For every nonzero element $\xi$ of E, one has $\pi (A)\xi = E$.

The subspace $\pi (A)\xi$ of E is stable under $\pi (A)$. Suppose that it is zero. Then the nonzero subspace $K\xi$ of E would be stable under $\pi (A)$, and hence equal to E; but this would imply that $\pi$ is the zero representation. Thus one has $\pi (A)\xi = E$.

Let $\pi$ be a nontrivial irreducible representation of A in E. By this lemma, the annihilator R of $\xi$ in A is a regular left ideal (A, VIII, p. 425, No.$^o1$) of A, and the representation $\pi$ is equivalent to the representation defined by the A-pseudomodule $A/R$. Since $\pi$ is irreducible, the ideal R is a regular maximal left ideal.

#### Definition 7 {#ts-i-s1-def-7 .statement tag=025G}

Let A be an algebra over K. A primitive ideal of A is defined to be the kernel of a nontrivial irreducible representation of A.

If A is commutative, the primitive ideals of A are the regular maximal ideals of A. In fact, the nontrivial irreducible representations of A are, up to equivalence, the representations $\pi_R$ defined by the A-pseudomodules $A/R$, where R is a regular maximal ideal of A. The kernel of $\pi_R$ contains R. It is even equal to it since, by A, VIII, p. 426, Prop. 2, the commutativity of A implies that $A/R$ is a field. Hence Ker($\pi_R$) is regular maximal.

#### Lemma 5 {#ts-i-s1-lem-5 .statement tag=025H}

Let $\pi$ be an irreducible representation of A in a vector space E over K.

a) Let I be a two-sided ideal of A. If $\pi (I)\not=\{0\}$, then $\pi |I$ is irreducible;

b) Let $I_1$ and $I_2$ be two-sided ideals of A such that $\pi (I_1)\not= 0$ and $\pi (I_2)\not= 0$. Then $\pi (I_1I_2)\not= 0$.

The set of elements of E annihilated by $\pi (I)$ is stable under $\pi (A)$ and distinct from E, hence equal to 0. Therefore, if $\xi$ is a nonzero element of E, one has $\pi (I)\xi \not= 0$; since $\pi (I)\xi$ is stable under $\pi (A)$, one has $\pi (I)\xi = E$, which proves a). On the other hand, what precedes proves that $\pi (I_2)E = E$, $\pi (I_1)\pi (I_2)E = E$, hence $\pi (I_1I_2)\not= 0$, whence b).

#### Lemma 6 {#ts-i-s1-lem-6 .statement tag=025I}

Let $I_1$ and $I_2$ be two-sided ideals of A, I a primitive ideal of A. If I contains $I_1I_2($in particular, if I contains $I_1\cap I_2)$, then I contains $I_1$ or $I_2$.

Let $\pi$ be an irreducible representation with kernel I. If $I\not\supset I_1$ and $I\not\supset I_2$, Lemma 5, b) proves that $\pi (I_1I_2)\not= 0$, whence $I\not\supset I_1I_2$.

#### Lemma 7 {#ts-i-s1-lem-7 .statement tag=025J}

Suppose that A admits a unit element. Let I be a maximal two-sided ideal of A. Then I is a primitive ideal.

There exists a maximal left ideal R of A containing I (A, I, p. 99, Theorem 1). Let $\pi$ be the canonical representation of A in $A/R$, which is irreducible and nonzero. Since IA $\subset R$, the kernel $I'$ of $\pi$ contains I, hence $I'= I$ and I is primitive.

Let J(A) be the set of primitive ideals of A. For every subset M of A, we denote by V(M) the set of primitive ideals of A containing M; if I is the two-sided ideal of A generated by M, one has V(M) = V(I). If M is reduced to a single element $x$, one writes $V(x)$ instead of $V(\{x\})$. The mapping $M\mapsto V(M)$ is decreasing for the inclusion relations. One has :

$$
V(\emptyset ) = J(A),V(A) =\emptyset \tag{5}
$$

$$
V(\bigcup_{i\in I}M_i)= V(\sum_{i\in I}M_i)=\bigcap_{i\in I}V(M_i) \tag{6}
$$

for every family $(M_i)_{i\in I}$ of subsets of A. On the other hand, by lemma 6,

$$
V(I_1\cap I_2) = V(I_1I_2) = V(I_1)\cup V(I_2) \tag{7}
$$

for every two-sided ideals $I_1,I_2$ of A. Formulas (5) to (7) show that the subsets V(M) of J(A) are the closed subsets of a topology called the Jacobson topology on J(A).

Let T be a subset of J(A), and let Υ(T) be the intersection of the elements of T, so that Υ(T) is a two-sided ideal of A. Then the closure of T in J(A) is the smallest closed subset of J(A) containing T, that is to say V(Υ(T)). In particular, T is closed if and only if T = V(Υ(T)).

#### Proposition 2 {#ts-i-s1-prop-2 .statement tag=025K}

Let $I_1$ and $I_2$ be distinct points of J(A). Then one of these two points is not adherent to the other.

For, for example, one has $I_1\not\subset I_2$. The set $V(I_1)$ of the $I\in J(A)$ such that $I_1\subset I$ is closed in J(A), and it contains $I_1$ but not $I_2$.

#### Proposition 3 {#ts-i-s1-prop-3 .statement tag=025L}

Let $I\in J(A)$. In order that $\{I\}$ be closed in J(A), it is necessary and sufficient that I be a maximal primitive ideal.

In fact, the closure of $\{I\}$ consists of the primitive ideals of A containing I.

The relation

“ $\pi_1,\pi_2$ are representations of A which are isomorphic ”

is an equivalence relation with respect to $\pi_1$ and $\pi_2$. For every representation $\pi$ of A, we shall denote by cl($\pi$ ) the equivalence class of $\pi$, which is therefore a representation of A isomorphic to $\pi$, such that two representations $\pi_1$ and $\pi_2$ are isomorphic if and only if cl($\pi_1$) $=$ cl($\pi_2$). One says that cl($\pi$ ) is the class of $\pi$.

Let $\mathfrak{c}$ be the cardinal of A. Let $\pi$ be a nonzero irreducible representation of A in a K-vector space E. Let $\xi$ be a nonzero element of E. Since $\pi (A)\xi = E$ (lemma 4), the dimension of E is $\leqslant \mathfrak{c}$ (A, II, p. 97, corollaire). The relation

“ $\lambda$ is a class of irreducible representations of A

in a K-vector space of dimension $\leqslant \mathfrak{c}$ ”

is collectivizing in $\lambda$ (E, II, p. 3). In fact, every vector space of dimension $\leqslant \mathfrak{c}$ is isomorphic to a space $K^B$ where B is a subset of A (A, II, p. 25, déf. 10), and the assertion then follows from E, II, p. 47.

We denote by $\widehat{A}$ the set of classes of irreducible, non-trivial, representations of A. From what precedes, for every non-trivial irreducible representation $\pi$ of A, there exists a unique representation $\widehat{\pi}\in \widehat{A}$ which is isomorphic to $\pi$.

The mapping of $\widehat{A}$ into J(A) which associates to $\pi$ its kernel is surjective. If A is commutative, it follows from the fact that the primitive ideals are the regular maximal ideals that this mapping is a bijection.

We endow $\widehat{A}$ with the inverse image topology of that of J(A) by the mapping $\widehat{A}\rightarrow J(A)$.

#### Proposition 4 {#ts-i-s1-prop-4 .statement tag=025M}

If A possesses a unit element, the spaces J(A) and $\widehat{A}$ are quasi-compact.

It is enough to give the proof for J(A). Let $(T_j)$ be a family of closed subsets of J(A) whose intersection is empty. If the sum $\sum_j\Upsilon (T_j)$ were not equal to A, this sum would be contained in a maximal two-sided ideal I. The ideal I would be primitive (Lemma 7); since the subset $T_j$ is closed, hence equal to $V(\Upsilon (T_j))$, one would have $I\in T_j$ for every $j$, which contradicts the hypothesis. Thus one has $\sum_j\Upsilon (T_j) = A$, and therefore one can write $1 =x_1+\cdots +x_n$ with $n\geqslant 1$ and $x_i\in \Upsilon (T_{j_i})$ for every $i$. This implies that $\Upsilon (T_{j_1})+\cdots +\Upsilon (T_{j_n}) = A$, whence $T_{j_1}\cap  \cdots  \cap T_{j_n}=\emptyset$.

Suppose that the algebra A is commutative and unital. The Jacobson topology on J(A) is the topology induced on J(A) by the Zariski topology of the prime spectrum of A (AC, II, Definition 4, p. 125).

Suppose that A is commutative and that K is a topological field. The canonical isomorphism of K onto $\mathscr{L}(K)$ makes it possible to identify an element of $\mathsf{X}(A)$ with a representation of A in the vector space K, which defines an injective mapping of $\mathsf{X}(A)$ into $\widehat{A}$. One can therefore identify $\mathsf{X}(A)$ with a subset of $\widehat{A}$.

#### Proposition 5 {#ts-i-s1-prop-5 .statement tag=025N}

The topology induced on $\mathsf{X}(A)$ by that of $\widehat{A}$ is coarser than the topology of $\mathsf{X}(A)$.

In fact, let T be a closed subset of $\widehat{A}$. Then T is the set of $\pi \in \widehat{A}$ whose kernel contains a subset M of A. Therefore $T\cap \mathsf{X}(A)$ is the set of $\chi \in \mathsf{X}(A)$ which vanish on M, that is, a closed subset of $\mathsf{X}(A)$. Hence the proposition.

In general, the topology of $\mathsf{X}(A)$ does not coincide with the topology induced by the topology of $\widehat{A}($cf. I, p. 193, Exercise 6, c)).

## EXERCISES {#ts-i-s1-exercises}

See the [exercises for § 1](exercises/s1/).
