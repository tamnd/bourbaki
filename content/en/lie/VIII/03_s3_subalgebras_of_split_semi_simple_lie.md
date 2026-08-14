---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 3
section_title: Subalgebras of split semi-simple Lie algebras
lang: en
source: lie-vii-ix
book_pages: A VIII.86-A VIII.95, A VIII.229-A VIII.231
pdf_pages: 0094-0103, 0237-0239
extraction: native
subsections:
    - "no": 1
      title: SUBALGEBRAS STABLE UNDER ad $\mathfrak{h}$
      page: 86
      pdf_page: 94
    - "no": 2
      title: IDEALS
      page: 89
      pdf_page: 97
    - "no": 3
      title: BOREL SUBALGEBRAS
      page: 90
      pdf_page: 98
    - "no": 4
      title: PARABOLIC SUBALGEBRAS
      page: 92
      pdf_page: 100
    - "no": 5
      title: NON-SPLIT CASE
      page: 94
      pdf_page: 102
statements: 28
exercises: 14
content_sha256: bb4fbba66794d2448e767216a487cc2435a0d8e55bfa7858277f92188f613d3e
---

## § 3. SUBALGEBRAS OF SPLIT SEMI-SIMPLE LIE ALGEBRAS

In this paragraph, we denote by $(\mathfrak{g},\mathfrak{h})$ a split semi-simple Lie algebra, and by R its root system.

### 1. SUBALGEBRAS STABLE UNDER ad $\mathfrak{h}$

#### Lemma 1 {#lie-viii-s3-lem-1 .statement tag=00ZO}

Let V be a vector subspace of $\mathfrak{g}$ and R(V) the set of $\alpha \in R$ such that $\mathfrak{g}^{\alpha}\subset V$. Then, $(V\cap \mathfrak{h}) +\sum_{\alpha\in R(V)}\mathfrak{g}^{\alpha}$ is the largest vector subspace of V stable under ad $\mathfrak{h}$.

A vector subspace W of V is stable under ad $\mathfrak{h}$ if and only if

$$
W = (W\cap \mathfrak{h}) +\sum_{\alpha\in R}(W\cap \mathfrak{g}^{\alpha})
$$

(Algebra, Chap. VII, §2, no. 2, Cor. 1 of Th. 1). The largest vector subspace of V stable under ad $\mathfrak{h}$ is thus $(V\cap \mathfrak{h}) +\sum_{\alpha\in R}(V\cap \mathfrak{g}^{\alpha})$. But $V\cap \mathfrak{g}^{\alpha}=\mathfrak{g}^{\alpha}$ for $\alpha \in R(V)$, and $V\cap \mathfrak{g}^{\alpha}= 0$ for $\alpha  /\in R(V)$ since dim $\mathfrak{g}^{\alpha}= 1$. Q.E.D.

For any subset P of R, put

$$
\mathfrak{g}^P=\sum_{\alpha\in P}\mathfrak{g}^{\alpha}\mathfrak{h}_P=\sum_{\alpha\in P}\mathfrak{h}_{\alpha}
$$

If $P\subset R$ and $Q\subset R$, we clearly have

$$
[\mathfrak{h},\mathfrak{g}^P]\subset \mathfrak{g}^P \tag{1}
$$

$$
[\mathfrak{g}^P,\mathfrak{g}^Q] =\mathfrak{g}^{(P+Q)\cap R}+\mathfrak{h}_{P\cap(-Q)} \tag{2}
$$

Recall (Chap. VI, §1, no. 7, Def. 4) that a subset P of R is said to be closed if the conditions $\alpha \in P, \beta \in P, \alpha +\beta \in R$ imply $\alpha +\beta \in P$, in other words if $(P + P)\cap R\subset P$.

#### Lemma 2 {#lie-viii-s3-lem-2 .statement tag=00ZP}

Let $\mathfrak{h}'$ be a vector subspace of $\mathfrak{h}$ and P a subset of R. Then $\mathfrak{h}'+\mathfrak{g}^P$ is a subalgebra of $\mathfrak{g}$ if and only if P is a closed subset of R and

$$
\mathfrak{h}'\supset \mathfrak{h}_{P\cap(-P)}
$$

Indeed,

$$
[\mathfrak{h}'+\mathfrak{g}^P,\mathfrak{h}'+\mathfrak{g}^P] = [\mathfrak{h}',\mathfrak{g}^P] + [\mathfrak{g}^P,\mathfrak{g}^P] =\mathfrak{h}_{P\cap(-P)}+ [\mathfrak{h}',\mathfrak{g}^P] +\mathfrak{g}^{(P+P)\cap R}
$$

Hence $\mathfrak{h}'+\mathfrak{g}^P$ is a subalgebra of $\mathfrak{g}$ if and only if

$\mathfrak{h}_{P\cap(-P)}\subset \mathfrak{h}'$ and $\mathfrak{g}^{(P+P)\cap R}\subset \mathfrak{g}^P$

which proves the lemma.

#### Proposition 1 {#lie-viii-s3-prop-1 .statement tag=00ZQ}

(i) The subalgebras of $\mathfrak{g}$ stable under ad$\mathfrak{h}$ are the vector subspaces of the form $\mathfrak{h}'+\mathfrak{g}^P$, where P is a closed subset of R and $\mathfrak{h}'$ is a vector subspace of $\mathfrak{h}$ containing $\mathfrak{h}_{P\cap(-P)}$.

(ii) Let $\mathfrak{h}',\mathfrak{h}''$ be vector subspaces of $\mathfrak{h}$ and $P,Q$ closed subsets of R, with $\mathfrak{h}'\supset \mathfrak{h}_{P\cap(-P)},\mathfrak{h}''\subset \mathfrak{h}'$ and $Q\subset P$. Then $\mathfrak{h}''+\mathfrak{g}^Q$ is an ideal of $\mathfrak{h}'+\mathfrak{g}^P$ if and only if

$(P + Q)\cap R\subset Q$ and $\mathfrak{h}_{P\cap(-Q)}\subset \mathfrak{h}''\subset \bigcap_{\alpha\in P,\alpha  /\in Q}$ Ker $\alpha$.

Assertion (i) follows immediately from Lemmas 1 and 2. Let $\mathfrak{h}',\mathfrak{h}'',P,Q$ be as in (ii). Then

$$
[\mathfrak{h}'+\mathfrak{g}^P,\mathfrak{h}''+\mathfrak{g}^Q] =\mathfrak{h}_{P\cap(-Q)}+ [\mathfrak{h}',\mathfrak{g}^Q] + [\mathfrak{h}'',\mathfrak{g}^P] +\mathfrak{g}^{(P+Q)\cap R}
$$

Hence, $\mathfrak{h}''+\mathfrak{g}^Q$ is an ideal of $\mathfrak{h}'+\mathfrak{g}^P$ if and only if

$$
\mathfrak{h}_{P\cap(-Q)}\subset \mathfrak{h}'',[\mathfrak{h}'',\mathfrak{g}^P]\subset \mathfrak{g}^Q,\mathfrak{g}^{(P+Q)\cap R}\subset \mathfrak{g}^Q
$$

This implies (ii).

#### Proposition 2 {#lie-viii-s3-prop-2 .statement tag=00ZR}

Let $\mathfrak{a}$ be a subalgebra of $\mathfrak{g}$ stable under ad$\mathfrak{h}$, and let $\mathfrak{h}'\subset \mathfrak{h}$, $P\subset R$ be such that $\mathfrak{a}=\mathfrak{h}'+\mathfrak{g}^P$.

(i) Let $\mathfrak{k}$ be the set of $x\in \mathfrak{h}'$ such that $\alpha (x) = 0$ for all $\alpha \in P\cap (-P)$. The radical of $\mathfrak{a}$ is $\mathfrak{k}+\mathfrak{g}^Q$, where Q is the set of $\alpha \in P$ such that $-\alpha  /\in P$. Moreover, $\mathfrak{g}^Q$ is a nilpotent ideal of $\mathfrak{a}$.

(ii) $\mathfrak{a}$ is semi-simple if and only if $P =-P$ and $\mathfrak{h}'=\mathfrak{h}_P$.

(iii) $\mathfrak{a}$ is solvable if and only if $P\cap (-P) =\emptyset$. In that case $[\mathfrak{a},\mathfrak{a}] =\mathfrak{g}^S$, where

$$
S = ((P + P)\cap R)\cup  \{\alpha \in P|\alpha (\mathfrak{h}')\not= 0\}
$$

(iv) $\mathfrak{a}$ is reductive in $\mathfrak{g}$ if and only if $P =-P$.

(v) $\mathfrak{a}$ consists of nilpotent elements if and only if $\mathfrak{h}'= 0$. Then $P\cap (-P) =$ $\emptyset$, and $\mathfrak{a}$ is nilpotent.

We prove (v). If $\mathfrak{a}$ consists of nilpotent elements, $\mathfrak{a}$ is clearly nilpotent, and $\mathfrak{h}'= 0$ since the elements of $\mathfrak{h}$ are semi-simple. Assume that $\mathfrak{h}'= 0$. By Prop. 1 (i), $P\cap (-P) =\emptyset$. By Chap. VI, §1, no. 7, Prop. 22, there exists a chamber C of R such that $P\subset R_+(C)$. Hence, there exists an integer $n >0$ with the following properties: if $\alpha_1, . . . , \alpha_n\in P$ and $\beta \in R\cup  \{0\}$, then

$$
\alpha_1+\cdots +\alpha_n+\beta  /\in R\cup  \{0\}
$$

This implies that every element of $\mathfrak{g}^P$ is nilpotent, hence (v).

We prove (iii). If $P\cap (-P) =\emptyset ,\mathfrak{g}^P$ is a subalgebra of $\mathfrak{g}$ (Prop. 1 (i)), and is nilpotent by (v). Now

$$
[\mathfrak{a},\mathfrak{a}] = [\mathfrak{h}',\mathfrak{g}^P] + [\mathfrak{g}^P,\mathfrak{g}^P] = [\mathfrak{h}',\mathfrak{g}^P] +\mathfrak{g}^{(P+P)\cap R}\subset \mathfrak{g}^P
$$

so $\mathfrak{a}$ is solvable and $[\mathfrak{a},\mathfrak{a}]$ is given by the formula in the proposition. If $P\cap (-P)\not=\emptyset$, let $\alpha \in P$ be such that $-\alpha \in P$. Then $\mathfrak{h}_{\alpha}+\mathfrak{g}^{\alpha}+\mathfrak{g}^{-\alpha}$ is a simple subalgebra of $\mathfrak{a}$ so $\mathfrak{a}$ is not solvable.

We prove (i). Since P is closed, $(P + Q)\cap R\subset P$. If $\alpha \in P, \beta \in Q$ and $\alpha +\beta \in R$, we cannot have $\alpha +\beta \in  -P$, for, P being closed, this would imply that $-\beta =-(\alpha +\beta ) +\alpha \in P$ whereas $\beta \in Q$; thus, $(P + Q)\cap R\subset Q$. This proves that $\mathfrak{g}^Q$ is an ideal of $\mathfrak{a}$, nilpotent by (v). We have $P\cap (-Q) =\emptyset$, and $P\cap (-P) = P\cap \complement Q$, so $\mathfrak{h}_{P\cap(-Q)}\subset \mathfrak{k}\subset \bigcap_{\alpha\in P,\alpha  /\in Q}$ Ker$\alpha$. By Prop. 1 (ii),

$\mathfrak{k}+\mathfrak{g}^Q$ is an ideal of $\mathfrak{a}$. Since $Q\cap (-Q) =\emptyset$, this ideal is solvable by (iii). It is therefore contained in the radical $\mathfrak{r}$ of $\mathfrak{a}$. Since $\mathfrak{r}$ is stable under every derivation of $\mathfrak{a},\mathfrak{r}$ is stable under ad $\mathfrak{h}$. Hence there exists a subset S of P such that $\mathfrak{r}= (\mathfrak{r}\cap \mathfrak{h}) +\mathfrak{g}^S$. Suppose that $\alpha \in S$ and that $-\alpha \in P$. Then $\mathfrak{h}_{\alpha}= [\mathfrak{g}^{\alpha},\mathfrak{g}^{-\alpha}]\subset \mathfrak{r}$, so $\mathfrak{g}^{-\alpha}= [\mathfrak{h}_{\alpha},\mathfrak{g}^{-\alpha}]\subset \mathfrak{r}= 0$, so that $-\alpha \in S$; by (iii), this contradicts the fact that $\mathfrak{r}$ is solvable. Consequently, $S\subset Q$. Finally, if $x\in \mathfrak{r}\cap \mathfrak{h}$ and if $\alpha \in P\cap (-P)$, then $[x,\mathfrak{g}^{\alpha}]\subset \mathfrak{g}^{\alpha}\cap \mathfrak{r}= 0$, so $\alpha (x) = 0$; this shows that $x\in \mathfrak{k}$. Hence $\mathfrak{r}\subset \mathfrak{k}+\mathfrak{g}^Q$ and the proof of (i) is complete.

We prove (iv). By (i), the adjoint representation of $\mathfrak{a}$ on $\mathfrak{g}$ is semi-simple if and only if ad$_{\mathfrak{g}}x$ is semi-simple for all $x\in \mathfrak{k}+\mathfrak{g}^Q$ (Chap. I, §6, no. 5, Th. 4); by (v), this is the case if and only if $Q =\emptyset$, in other words $P =-P$.

We prove (ii). If $\mathfrak{a}$ is semi-simple, $P =-P$ by (i), so $\mathfrak{h}_P\subset \mathfrak{h}'$; further, $\mathfrak{a}= [\mathfrak{a},\mathfrak{a}]\subset \mathfrak{h}_P+\mathfrak{g}^P$ and consequently $\mathfrak{h}'=\mathfrak{h}_P$. If $P =-P$ and $\mathfrak{h}'=\mathfrak{h}_P,\mathfrak{a}$ is reductive by (iv), and $\mathfrak{a}=\sum_{\alpha\in P}\mathfrak{s}_{\alpha}$, so $\mathfrak{a}= [\mathfrak{a},\mathfrak{a}]$ and $\mathfrak{a}$ is semi-simple.

#### Proposition 3 {#lie-viii-s3-prop-3 .statement tag=00ZS}

Let $\mathfrak{a}$ be a semi-simple subalgebra of $\mathfrak{g}$ stable under ad($\mathfrak{h}$) and let P be the subset of R such that $\mathfrak{a}=\mathfrak{h}_P+\mathfrak{g}^P$.

(i) $\mathfrak{h}_P$ is a splitting Cartan subalgebra of $\mathfrak{a}$.

(ii) The root system of $(\mathfrak{a},\mathfrak{h}_P)$ is the set of restrictions to $\mathfrak{h}_P$ of elements of P.

Since $\mathfrak{h}_P$ is stable under ad $\mathfrak{h}$, its normalizer in $\mathfrak{a}$ is stable under ad $\mathfrak{h}$, and hence is of the form $\mathfrak{h}_P+\mathfrak{g}^Q$ where $Q\subset P$ (Lemma 1). If $\alpha \in Q$,

$$
\mathfrak{g}^{\alpha}= [\mathfrak{h}_{\alpha},\mathfrak{g}^{\alpha}]\subset [\mathfrak{h}_P,\mathfrak{g}^{\alpha}]\subset \mathfrak{h}_P
$$

which is absurd. Thus $Q =\emptyset$ and $\mathfrak{h}_P$ is its own normalizer in $\mathfrak{a}$. This proves that $\mathfrak{h}_P$ is a Cartan subalgebra of $\mathfrak{a}$. If $x\in \mathfrak{h}_P$, ad$_{\mathfrak{g}}x$, and a fortiori ad$_{\mathfrak{a}}x$, are triangularizable. Thus (i) is proved, and (ii) is clear.

By Prop. 1 (i), the subalgebras of $\mathfrak{g}$ containing $\mathfrak{h}$ are the sets $\mathfrak{h}+\mathfrak{g}^P$ where P is a closed subset of R. By Chap. VII, §3, Prop. 3, every Cartan subalgebra of $\mathfrak{h}+\mathfrak{g}^P$ is a Cartan subalgebra of $\mathfrak{g}$.

#### Proposition 4 {#lie-viii-s3-prop-4 .statement tag=00ZT}

Let $\mathfrak{a}$ be a subalgebra of $\mathfrak{g}$ containing $\mathfrak{h},x$ an element of $\mathfrak{a},s$ and $n$ its semi-simple and nilpotent components. Then $s\in \mathfrak{a}$ and $n\in \mathfrak{a}$.

We have (ad $x)\mathfrak{a}\subset \mathfrak{a}$, so (ad $s)\mathfrak{a}\subset \mathfrak{a}$ and (ad $n)\mathfrak{a}\subset \mathfrak{a}$. Since $\mathfrak{a}$ is its own normalizer in $\mathfrak{g}$ (Chap. VII, §2, no. 1, Cor. 4 of Prop. $4),s\in \mathfrak{a}$ and $n\in \mathfrak{a}$.

#### Proposition 5 {#lie-viii-s3-prop-5 .statement tag=00ZU}

Let P be a closed subset of R.

(i) $\mathfrak{h}+\mathfrak{g}^P$ is solvable if and only if $P\cap (-P) =\emptyset$. In that case, $[\mathfrak{h}+\mathfrak{g}^P,\mathfrak{h}+\mathfrak{g}^P] =\mathfrak{g}^P$.

(ii) $\mathfrak{h}+\mathfrak{g}^P$ is reductive if and only if $P =-P$.

Assertion (i) follows from Prop. 2 (iii). If $P =-P,\mathfrak{h}+\mathfrak{g}^P$ is reductive (Prop. 2 (iv)). Assume that $\mathfrak{a}=\mathfrak{h}+\mathfrak{g}^P$ is reductive. Then

$$
\mathfrak{g}^P= [\mathfrak{h},\mathfrak{g}^P]\subset [\mathfrak{a},\mathfrak{a}]\subset \mathfrak{h}+\mathfrak{g}^P
$$

so $[\mathfrak{a},\mathfrak{a}]$ is of the form $\mathfrak{h}'+\mathfrak{g}^P$ with $\mathfrak{h}'\subset \mathfrak{h}$; since $[\mathfrak{a},\mathfrak{a}]$ is semi-simple, $P =-P$ (Prop. 2 (ii)).

### 2. IDEALS

#### Proposition 6 {#lie-viii-s3-prop-6 .statement tag=00ZV}

Let $R_1, . . . ,R_p$ be the irreducible components of R. For $i= 1, . . . , p$, put $\mathfrak{g}_i=\mathfrak{h}_{R_i}+\mathfrak{g}^{R_i}$. Then $\mathfrak{g}_1, . . . ,\mathfrak{g}_p$ are the simple components of $\mathfrak{g}$.

The $\mathfrak{g}_i$ are ideals of $\mathfrak{g}$ (Prop. 1 (ii)). It is clear that $\mathfrak{g}$ is the direct sum of the $\mathfrak{g}_i$, hence the product of the $\mathfrak{g}_i$. Let $\mathfrak{a}$ and $\mathfrak{b}$ be complementary ideals of $\mathfrak{g}$. Then $\mathfrak{a}$ and $\mathfrak{b}$ are semi-simple and stable under ad $\mathfrak{h}$, so there exist subsets $P,Q$ of R such that $\mathfrak{a}=\mathfrak{h}_P+\mathfrak{g}^P,\mathfrak{b}=\mathfrak{h}_Q+\mathfrak{g}^Q$. Then $\mathfrak{h}_P,\mathfrak{h}_Q$ are orthogonal complements of each other in $\mathfrak{h}$ for the Killing form, so P and Q are unions of irreducible components of R. This proves that the $\mathfrak{g}_i$ are minimal ideals of $\mathfrak{g}$.

#### Corollary 1 {#lie-viii-s3-prop-6-cor-1 .statement tag=01IZ}

$\mathfrak{g}$ is simple if and only if R is irreducible (in other words, its Dynkin graph is connected).

This follows from Prop. 6.

A Lie algebra $\mathfrak{a}$ is said to be absolutely simple if, for every extension $k'$ of $k$, the $k'$-Lie algebra $\mathfrak{a}_{(k')}$ is simple.

#### Corollary 2 {#lie-viii-s3-prop-6-cor-2 .statement tag=00ZW}

A splittable simple Lie algebra is absolutely simple.

This follows from Cor. 1.

If $\mathfrak{g}$ is of type $A_l(l\geq 1)$ or $B_l(l\geq 1)$ or $C_l(l\geq 1)$ or $D_l(l\geq 3),\mathfrak{g}$ is said to be a classical splittable simple Lie algebra. If $\mathfrak{g}$ is of type $E_6, E_7, E_8, F_4$, or $G_2,\mathfrak{g}$ is said to be an exceptional splittable simple Lie algebra.

### 3. BOREL SUBALGEBRAS

#### Proposition 7 {#lie-viii-s3-prop-7 .statement tag=00ZX}

Let $\mathfrak{b}=\mathfrak{h}+\mathfrak{g}^P$ be a subalgebra of $\mathfrak{g}$ containing $\mathfrak{h}$. The following conditions are equivalent:

(i) $\mathfrak{b}$ is a maximal solvable subalgebra of $\mathfrak{g}$;

(ii) there exists a chamber C of R such that $P = R_+(C)$;

(iii) $P\cap (-P) =\emptyset$ and $P\cup (-P) = R$.

(i) $=\Rightarrow$ (ii): If $\mathfrak{b}$ is solvable, $P\cap (-P) =\emptyset$. Then there exists a chamber C of R such that $P\subset R_+(C)$ (Chap. VI, §1, no. 7, Prop. 22). Then $\mathfrak{h}+\mathfrak{g}^{R_+(C)}$ is a solvable subalgebra of $\mathfrak{g}$ containing $\mathfrak{b}$, hence equal to $\mathfrak{b}$ if $\mathfrak{b}$ is maximal.

(ii) $=\Rightarrow$ (iii): This is clear.

(iii) $=\Rightarrow$ (i): Assume that $P\cap (-P) =\emptyset$ and that $P\cup (-P) = R$. Then $\mathfrak{b}$ is solvable. Let $\mathfrak{b}'$ be a solvable subalgebra of $\mathfrak{g}$ containing $\mathfrak{b}$. There exists a subset Q of R such that $\mathfrak{b}'=\mathfrak{h}+\mathfrak{g}^Q$. Then $Q\cap (-Q) =\emptyset$ and $Q\supset P$, so Q = P and $\mathfrak{b}'=\mathfrak{b}$.

#### Definition 1 {#lie-viii-s3-def-1 .statement tag=00ZY}

A subalgebra of $\mathfrak{g}$ containing $\mathfrak{h}$ and satisfying the equivalent condition in Prop. 7 is called a Borel subalgebra of $(\mathfrak{g},\mathfrak{h})$.

A subalgebra $\mathfrak{b}$ of a splittable algebra $\mathfrak{g}$ is called a Borel subalgebra of $\mathfrak{g}$ if there exists a splitting Cartan subalgebra $\mathfrak{h}'$ of $\mathfrak{g}$ such that $\mathfrak{b}$ is a Borel subalgebra of $(\mathfrak{g},\mathfrak{h}')$.

Let $(\mathfrak{g},\mathfrak{h})$ be a split reductive Lie algebra. Let $\mathfrak{g}=\mathfrak{c}\times \mathfrak{s}$ with $\mathfrak{c}$ commutative and $\mathfrak{s}$ semi-simple. A subalgebra of $\mathfrak{g}$ of the form $\mathfrak{c}\times \mathfrak{b}$, where $\mathfrak{b}$ is a Borel subalgebra of $(\mathfrak{s},\mathfrak{h}\cap \mathfrak{s})$, is called a Borel subalgebra of $(\mathfrak{g},\mathfrak{h})$.

With the notations of Prop. 7, we also say that $\mathfrak{b}$ is the Borel subalgebra of $\mathfrak{g}$ defined by $\mathfrak{h}$ and C (or by $\mathfrak{h}$ and the basis of R associated to C).

#### Remark {#lie-viii-s3-n3-rem-1 .statement tag=00ZZ}

The map which associates $R_+(C)$ to a chamber C of R is injective (Chap. VI, §1, no. 7, Cor. 1 of Prop. 20). Consequently, $C \rightarrow \mathfrak{h}+\mathfrak{g}^{R_+(C)}$ is a bijection from the set of chambers of R to the set of Borel subalgebras of $(\mathfrak{g},\mathfrak{h})$. Thus, the number of Borel subalgebras of $(\mathfrak{g},\mathfrak{h})$ is equal to the order of the Weyl group of R (Chap. VI, §1, no. 5, Th. 2).

#### Proposition 8 {#lie-viii-s3-prop-8 .statement tag=0100}

Let $\mathfrak{b}$ be a subalgebra of $\mathfrak{g},k'$ an extension of $k$. Then $\mathfrak{b}\otimes_kk'$ is a Borel subalgebra of $(\mathfrak{g}\otimes_kk',\mathfrak{h}\otimes_kk')$ if and only if $\mathfrak{b}$ is a Borel subalgebra of $(\mathfrak{g},\mathfrak{h})$.

This is clear from condition (iii) of Prop. 7.

#### Proposition 9 {#lie-viii-s3-prop-9 .statement tag=0101}

Let $\mathfrak{b}$ be the Borel subalgebra of $(\mathfrak{g},\mathfrak{h})$ defined by a chamber C of R. Let $\mathfrak{n}=\mathfrak{g}^{R_+(C)}=\sum_{\alpha\in R,\alpha >0}\mathfrak{g}^{\alpha}$. Let $l=$ dim$\mathfrak{h}$.

(i) If $h\in \mathfrak{h}$ and $x\in \mathfrak{n}$, the characteristic polynomial of ad$_{\mathfrak{g}}(h+x)$ is $T^l\prod_{\alpha\in R}(T-\alpha (h))$.

(ii) The largest nilpotent ideal of $\mathfrak{b}$ is equal to $\mathfrak{n}$ and to $[\mathfrak{b},\mathfrak{b}]$. This is also the set of elements of $\mathfrak{b}$ nilpotent in $\mathfrak{g}$.

(iii) Let B be the basis of R associated to C. For all $\alpha \in B$, let $X_{\alpha}$ be a non-zero element of $\mathfrak{g}^{\alpha}$. Then $(X_{\alpha})_{\alpha\in B}$ generates the Lie algebra $\mathfrak{n}$. We have $[\mathfrak{n},\mathfrak{n}] =\sum_{\alpha\in R,\alpha >0,\alpha  /\in B}\mathfrak{g}^{\alpha}$.

There exists a total order on $\mathfrak{h}^*_{\mathbf{Q}}$ compatible with its vector space structure and such that the elements of $R_+(C)$ are $>0$ (Chap. VI, §1, no. 7). Let $h, x$ be as in (i) and $y\in \mathfrak{g}^{\alpha}$. Then $[h+x, y] =\alpha (h)y+z$ where $z\in \sum_{\beta >\alpha}\mathfrak{g}^{\beta}$. Then,

with respect to a suitable basis of $\mathfrak{g}$, the matrix of ad$_{\mathfrak{g}}(h+x)$ has the following properties:

1) it is lower triangular;

2) the diagonal entries of the matrix are the number $0 (l$ times) and the $\alpha (h)$ for $\alpha \in R$.

This proves (i). It also shows that the characteristic polynomial of ad$_{\mathfrak{b}}(h+x)$ is $T\prod_{\alpha\in R_+(C)}^l(T-\alpha (h))$. It follows from the preceding that the

set of elements of $\mathfrak{b}$ nilpotent in $\mathfrak{g}$, as well as the largest nilpotent ideal of $\mathfrak{b}$, are equal to $\mathfrak{n}$. We have $\mathfrak{n}= [\mathfrak{b},\mathfrak{b}]$ by Prop. 5 (i). Finally, assertion (iii) follows from §2, Prop. 4 (ii) and Chap. VI, §1, no. 6, Prop. 19.

#### Corollary {#lie-viii-s3-n3-cor-1 .statement tag=0102}

Let $\mathfrak{b}$ be a Borel subalgebra of $\mathfrak{g}$.

(i) Every Cartan subalgebra of $\mathfrak{b}$ is a splitting Cartan subalgebra of $\mathfrak{g}$.

(ii) If $\mathfrak{h}_1,\mathfrak{h}_2$ are Cartan subalgebras of $\mathfrak{b}$, there exists $x\in [\mathfrak{b},\mathfrak{b}]$ such that $e^{ad_{\mathfrak{g}}x}\mathfrak{h}_1=\mathfrak{h}_2$.

Assertion (i) follows from Prop. 9 (i) and Chap. VII, §3, no. 3, Prop. 3. Assertion (ii) follows from Prop. 9 (ii) and Chap. VII, §3, no. 4, Th. 3.

#### Proposition 10 {#lie-viii-s3-prop-10 .statement tag=0103}

Let $\mathfrak{b},\mathfrak{b}'$ be Borel subalgebras of $\mathfrak{g}$. There exists a splitting Cartan subalgebra of $\mathfrak{g}$ contained in $\mathfrak{b}\cap \mathfrak{b}'$.

Let $\mathfrak{h}$ be a Cartan subalgebra of $\mathfrak{b},\mathfrak{n}= [\mathfrak{b},\mathfrak{b}],\mathfrak{n}'= [\mathfrak{b}',\mathfrak{b}'],\mathfrak{p}=\mathfrak{b}\cap \mathfrak{b}'$, and $\mathfrak{s}$ a vector subspace of $\mathfrak{g}$ complementary to $\mathfrak{b}+\mathfrak{b}'$. Denote by $\mathfrak{s}^{\bot},\mathfrak{b}^{\bot},\mathfrak{b}^{'\bot}$ the orthogonal complements of $\mathfrak{s},\mathfrak{b},\mathfrak{b}'$ with respect to the Killing form of $\mathfrak{g}$. Put $l=$ dim$\mathfrak{h}, n=$ dim$\mathfrak{n}, p=$ dim$\mathfrak{p}$. Then dim$\mathfrak{b}=$ dim$\mathfrak{b}'=l+n$,

dim$\mathfrak{s}^{\bot}=$ dim($\mathfrak{b}+\mathfrak{b}'$) $= 2(l+n)-p$,

and so

dim($\mathfrak{s}^{\bot}\cap \mathfrak{p}$)$\geq$ dim$\mathfrak{s}^{\bot}+$ dim$\mathfrak{p}-$ dim$\mathfrak{g}$ (3)

$$
= 2(l+n)-p+p-(l+ 2n) =l
$$

By Prop. 1 of §2, no. $2,\mathfrak{n}\subset \mathfrak{b}^{\bot},\mathfrak{n}'\subset \mathfrak{b}^{'\bot}$. The elements of $\mathfrak{p}\cap \mathfrak{n}$ are nilpotent in $\mathfrak{g}$ (Prop. 9 (ii)), and belong to $\mathfrak{b}'$, and hence to $\mathfrak{n}'$ (Prop. 9 (ii)). Consequently, $\mathfrak{p}\cap \mathfrak{n}\subset \mathfrak{n}\cap \mathfrak{n}'\subset \mathfrak{b}^{\bot}\cap \mathfrak{b}^{'\bot}$, so $\mathfrak{s}^{\bot}\cap \mathfrak{p}\cap \mathfrak{n}= 0$. In view of (3), we see that $\mathfrak{s}^{\bot}\cap \mathfrak{p}$ is a complement of $\mathfrak{n}$ in $\mathfrak{b}$. Let $z$ be an element of $\mathfrak{h}$ regular in $\mathfrak{g}$; there exists $y\in \mathfrak{n}$ such that $y+z\in \mathfrak{s}^{\bot}\cap \mathfrak{p}$; by Prop. 9 (i), ad$_{\mathfrak{g}}(y+z)$ has the same characteristic polynomial as ad$_{\mathfrak{g}}z$, so $x=y+z$ is regular in $\mathfrak{g}$ and a fortiori in $\mathfrak{b}$ and $\mathfrak{b}'$ (Chap. VII, §2, no. 2, Prop. 9). Since $\mathfrak{g},\mathfrak{b},\mathfrak{b}'$ have the same rank, $\mathfrak{b}^0(x) =\mathfrak{g}^0(x) ={\mathfrak{b}'}^0(x)$ is simultaneously a Cartan subalgebra of $\mathfrak{b}$, of $\mathfrak{g}$ and of $\mathfrak{b}'$ (Chap. VII, §3, no. 3, Th. 2). Finally, this Cartan subalgebra of $\mathfrak{g}$ is splitting by the Cor. of Prop. 9.

#### Corollary {#lie-viii-s3-n3-cor-2 .statement tag=0104}

The group Aut$_e(\mathfrak{g})$ operates transitively on the set of pairs $(\mathfrak{t},\mathfrak{b})$ where $\mathfrak{t}$ is a splitting Cartan subalgebra of $\mathfrak{g}$ and $\mathfrak{b}$ is a Borel subalgebra of $(\mathfrak{g},\mathfrak{t})$.

Let $(\mathfrak{t}_1,\mathfrak{b}_1)$ and $(\mathfrak{t}_2,\mathfrak{b}_2)$ be two such pairs. There exists a splitting Cartan subalgebra $\mathfrak{t}$ of $\mathfrak{g}$ contained in $\mathfrak{b}_1\cap \mathfrak{b}_2$ (Prop. 10). By the Cor. of Prop. 9, we are reduced to the case in which $\mathfrak{t}_1=\mathfrak{t}_2=\mathfrak{t}$. Let S be the root system of $(\mathfrak{g},\mathfrak{t})$. There exists bases $B_1,B_2$ of S such that $\mathfrak{b}_i$ is associated to $B_i(i= 1,2)$, and there exists $s\in W(S)$ which transforms $B_1$ into $B_2$. Finally, there exists $a\in$ Aut$_e(\mathfrak{g})$ such that $a|\mathfrak{t}=s($§2, no. 2, Cor. of Th. 2). Then $a(\mathfrak{t}) =\mathfrak{t}$ and $a(\mathfrak{b}_1) =\mathfrak{b}_2$.

### 4. PARABOLIC SUBALGEBRAS

#### Proposition 11 {#lie-viii-s3-prop-11 .statement tag=0105}

Let $\mathfrak{p}=\mathfrak{h}+\mathfrak{g}^P$ be a subalgebra of $\mathfrak{g}$ containing $\mathfrak{h}$. The following conditions are equivalent:

(i) $\mathfrak{p}$ contains a Borel subalgebra of $(\mathfrak{g},\mathfrak{h})$;

(ii) there exists a chamber C of R such that $P\supset R_+(C)$;

(iii) P is parabolic, in other words (Chap. VI, §1, no. 7, Def. 4), $P\cup (-P) =$ R.

Conditions (i) and (ii) are equivalent by Prop. 7. Conditions (ii) and (iii) are equivalent by Chap. VI, §1, no. 7, Prop. 20.

#### Definition 2 {#lie-viii-s3-def-2 .statement tag=0106}

A subalgebra of $\mathfrak{g}$ containing $\mathfrak{h}$ and satisfying the equivalent conditions of Prop. 11 is called a parabolic subalgebra of $(\mathfrak{g},\mathfrak{h})$. A parabolic subalgebra of $\mathfrak{g}$ is a parabolic subalgebra of $(\mathfrak{g},\mathfrak{h}')$ where $\mathfrak{h}'$ is a splitting Cartan subalgebra of $\mathfrak{g}$.

This definition extends immediately to the case in which $(\mathfrak{g},\mathfrak{h})$ is a split reductive Lie algebra.

#### Remark {#lie-viii-s3-n4-rem-1 .statement tag=0107}

Let B be a basis of R, and $\mathfrak{b}$ the corresponding Borel subalgebra. If $\Sigma \subset B$, denote by $Q_{\Sigma}$ the set of roots that are linear combinations of elements of $\Sigma$ with coefficients $\leq 0$; put $\mathfrak{p}(\Sigma ) = R_+(B)\cup Q_{\Sigma}$ and $\mathfrak{p}_{\Sigma}=\mathfrak{h}\oplus \mathfrak{g}^{P(\Sigma)}$. By Chap. VI, §1, no. 7, Lemma 3 and Prop. $20,\mathfrak{p}_{\Sigma}$ is a parabolic subalgebra containing $\mathfrak{b}$ and every parabolic subalgebra of $\mathfrak{g}$ containing $\mathfrak{b}$ is obtained in this way.

#### Lemma 3 {#lie-viii-s3-lem-3 .statement tag=0108}

Let V be a finite dimensional real vector space, S a root system in $V^*,\mathscr{P}$ the set of parabolic subsets of S; let $\mathscr{H}$ be the set of Ker $\alpha$ for $\alpha \in S$, and $\mathscr{F}$ the set of facets of V relative to $\mathscr{H}$ (Chap. V, §1, no. 2, Def. 1).

If $P\in \mathscr{P}$, let F(P) be the set of $v\in V$ such that $\alpha (v)\geq 0$ for all $\alpha \in P$. If $F\in \mathscr{F}$, let P(F) be the set of $\alpha \in R$ such that $\alpha (v)\geq 0$ for all $v\in F$.

Then $F \rightarrow P(F)$ is a bijection from $\mathscr{F}$ to $\mathscr{P}$; for all $F\in \mathscr{F}$, F(P(F)) is the closure of F.

$a)$ Let $P\in \mathscr{P}$. There exists a chamber C of S and a subset $\Sigma$ of the basis B(C) such that $P = S_+(C)\cup Q$ where Q is the set of linear combinations of elements of $\Sigma$ with non-positive integer coefficients (Chap. VI, §1, no. 7, Prop. 20). Put

$$
B(C) =\{\alpha_1, . . . , \alpha_l\}, \Sigma =\{\alpha_1, . . . , \alpha_m\}
$$

If $v\in V$, we have the following equivalences:

$\alpha (v)\geq 0$ for all $\alpha \in P$

$$
\Leftarrow \Rightarrow \alpha_1(v)\geq 0, . . . \alpha_l(v)\geq 0, \alpha_1(v)\leq 0, . . . , \alpha_m(v)\leq 0
$$

$$
\Leftarrow \Rightarrow \alpha_1(v) =\cdots =\alpha_m(v) = 0, \alpha_{m+1}(v)\geq 0, . . . , \alpha_l(v)\geq 0
$$

so F(P) is the closure of the set

$$
\{v\in V|\alpha_1(v) =\cdots =\alpha_m(v) = 0, \alpha_{m+1}(v)>0, . . . , \alpha_l(v)>0\}
$$

a set which is a facet F relative to $\mathscr{H}$ since every element of S is a linear combination of $\alpha_1, . . . , \alpha_l$ in which the coefficients are either all $\geq 0$ or all $\leq 0$. Moreover, if $\beta =u_1\alpha_1+\cdots +u_l\alpha_l\in S$,

$$
\beta \in P(F)\Leftarrow \Rightarrow u_{m+1}\geq 0, . . . , u_l\geq 0
$$

$\Leftarrow \Rightarrow \beta \in S_+(C)$ or $(-\beta \in S_+(C)$ and $u_{m+1}=. . .=u_l= 0)$

$$
\Leftarrow \Rightarrow \beta \in S_+(C)\cup Q = P
$$

so P(F) = P.

$b)$ Let $F\in \mathscr{F}$. It is clear that $P(F)\in \mathscr{P}$. On the other hand, F is contained in the closure of a chamber relative to $\mathscr{H}$ (Chap. V, §1, no. 3, formulas (6)), and so is a facet relative to the set of walls of this chamber (Chap. V, §1, no. 4, Prop. 9). Consequently, F is of the form $\{v\in V|\alpha (v)\geq 0$ for all $\alpha \in T\}$, where T is a subset of S which we can clearly take to be equal to P(F). Thus, F = F(P(F)). Q.E.D.

If $P\in \mathscr{P}$, the facet F such that P = P(F) is said to be associated to P; we denote it by F(P). We extend these conventions to the case in which $(\mathfrak{g},\mathfrak{h})$ is split reductive.

#### Proposition 12 {#lie-viii-s3-prop-12 .statement tag=0109}

Let $\mathscr{H}$ be the set of hyperplanes of $\mathfrak{h}_{\mathbf{R}}$ consisting of the kernels of the roots in R. Let $\mathscr{F}$ be the set of facets of $\mathfrak{h}_{\mathbf{R}}$ relative to $\mathscr{H}$. Let $\mathscr{S}$ be the set of parabolic subalgebras of $(\mathfrak{g},\mathfrak{h})$. For every $\mathfrak{p}=\mathfrak{h}+\mathfrak{g}^P\in \mathscr{S}$, let $F(\mathfrak{p})$ be the facet associated to P. Then $\mathfrak{p} \rightarrow F(\mathfrak{p})$ is a bijection from $\mathscr{S}$ to $\mathscr{F}$. If $\mathfrak{p}_1,\mathfrak{p}_2\in \mathscr{P}$,

$$
\mathfrak{p}_1\supset \mathfrak{p}_2\Leftarrow \Rightarrow F(\mathfrak{p}_1)\subset F(\mathfrak{p}_2)
$$

This follows immediately from Lemma 3.

#### Example {#lie-viii-s3-n4-exa-1 .statement tag=010A}

The facets corresponding to the parabolic subalgebras of $(\mathfrak{g},\mathfrak{h})$ containing a Borel algebra $\mathfrak{b}$ are the facets contained in the closure of the chamber associated to $\mathfrak{b}$ (cf. the Remark above).

#### Proposition 13 {#lie-viii-s3-prop-13 .statement tag=010B}

Let $\mathfrak{p}=\mathfrak{h}+\mathfrak{g}^P$ be a parabolic subalgebra of $(\mathfrak{g},\mathfrak{h})$, Q the set of $\alpha \in P$ such that $-\alpha  /\in P$, and $\mathfrak{s}=\mathfrak{h}+\mathfrak{g}^{P\cap(-P)}$. Then $\mathfrak{p}=\mathfrak{s}\oplus \mathfrak{g}^Q,\mathfrak{s}$ is reductive in $\mathfrak{g}$, and $\mathfrak{g}^Q$ is the largest nilpotent ideal of $\mathfrak{p}$ and the nilpotent radical of $\mathfrak{p}$. The centre of $\mathfrak{p}$ is zero.

By Prop. $2,\mathfrak{s}$ is reductive in $\mathfrak{g}$ and $\mathfrak{g}^Q$ is a nilpotent ideal of $\mathfrak{p}$. If $\mathfrak{n}$ is the largest nilpotent ideal of $\mathfrak{p},\mathfrak{g}^Q\subset \mathfrak{n}\subset \mathfrak{h}+\mathfrak{g}^Q$ (Prop. 2 (i)); if $x\in \mathfrak{n}\cap \mathfrak{h}$, ad$_{\mathfrak{p}}x$ is nilpotent, so $\alpha (x) = 0$ for all $\alpha \in P$, and hence $x= 0$; this proves that $\mathfrak{n}=\mathfrak{g}^Q$. Since $[\mathfrak{h},\mathfrak{g}^Q] =\mathfrak{g}^Q$, the nilpotent radical of $\mathfrak{p}$ contains $\mathfrak{g}^Q$ and consequently is equal to $\mathfrak{g}^Q$. Let $z=h+\sum_{\alpha\in P}u_{\alpha}$ (where $h\in \mathfrak{h}, u_{\alpha}\in \mathfrak{g}^{\alpha})$ be an

element of the centre of $\mathfrak{p}$. For all $h'\in \mathfrak{h}, 0 = [h', z] =\sum\alpha (h')u_{\alpha}$, so $u_{\alpha}= 0$ for all $\alpha \in P$; it follows that $[h,\mathfrak{g}^{\beta}] = 0$ for all $\beta \in P$, so $h= 0$.

### 5. NON-SPLIT CASE

#### Proposition 14 {#lie-viii-s3-prop-14 .statement tag=010C}

Let $k'$ be an extension of $k$ and $\mathfrak{g}'=\mathfrak{g}\otimes_kk'$. Let $\mathfrak{m}$ be a subalgebra of $\mathfrak{g}$ and $\mathfrak{m}'=\mathfrak{m}\otimes_kk'$. If $\mathfrak{m}'$ is a parabolic (resp. Borel ) subalgebra of $\mathfrak{g}',\mathfrak{m}$ is a parabolic (resp. Borel ) subalgebra of $\mathfrak{g}$.

By Prop. 8 and 11, it suffices to prove that $\mathfrak{m}$ contains a splitting Cartan subalgebra of $\mathfrak{g}$. Let $\mathfrak{b}$ be a Borel subalgebra of $\mathfrak{g}$. Then $\mathfrak{b}'=\mathfrak{b}\otimes_kk'$ is a Borel subalgebra of $\mathfrak{g}'$, so $\mathfrak{m}'\cap \mathfrak{b}'$ contains a Cartan subalgebra of $\mathfrak{g}'$ (Prop. 10). Let $\mathfrak{t}$ be a Cartan subalgebra of $\mathfrak{m}\cap \mathfrak{b}$. Then $\mathfrak{t}\otimes_kk'$ is a Cartan subalgebra of $\mathfrak{m}'\cap \mathfrak{b}'$, and hence of $\mathfrak{g}'$ (Chap. VII, §3, no. 3, Prop. 3). Consequently, $\mathfrak{t}$ is a Cartan subalgebra of $\mathfrak{g}$, and it is splitting since it is contained in $\mathfrak{b}$.

#### Definition 3 {#lie-viii-s3-def-3 .statement tag=010D}

Let $\mathfrak{a}$ be a semi-simple (or more generally reductive) Lie algebra and $\overline{k}$ an algebraic closure of $k$. A subalgebra $\mathfrak{m}$ of $\mathfrak{a}$ is said to be parabolic (resp. Borel ) if $\mathfrak{m}\otimes_k\overline{k}$ is a parabolic (resp. Borel ) subalgebra of $\mathfrak{a}\otimes_k\overline{k}$.

If $\mathfrak{a}$ is splittable, Prop. 14 shows that this definition is equivalent to Definition 2 (resp. to Definition 1).

#### Proposition 15 {#lie-viii-s3-prop-15 .statement tag=010E}

Let $\mathfrak{a}$ be a reductive Lie algebra, $k'$ an extension of $k$, and $\mathfrak{m}$ a subalgebra of $\mathfrak{a}$. Then $\mathfrak{m}$ is a parabolic (resp. Borel ) subalgebra of $\mathfrak{a}$ if and only if $\mathfrak{m}\otimes_kk'$ is a parabolic (resp. Borel ) subalgebra of $\mathfrak{a}\otimes_kk'$.

This follows immediately from Prop. 14.

### Exercises {#lie-viii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
