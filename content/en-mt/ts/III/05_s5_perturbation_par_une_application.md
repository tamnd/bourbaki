---
book: ts
book_title: Théories spectrales
chapter: III
chapter_title: APPLICATIONS LINÉAIRES COMPACTES ET PERTURBATIONS
section: 5
section_title: Perturbation par une application linéaire compacte
lang: en
source: ts-iii-v-fr
book_pages: TS III.71-TS III.82, TS III.125-TS III.128
pdf_pages: 0085-0096, 0139-0142
extraction: native
subsections:
    - "no": 1
      title: Morphismes stricts et propreté
      page: 71
      pdf_page: 85
    - "no": 2
      title: Perturbation des applications linéaires injectives ou surjectives
      page: 72
      pdf_page: 86
    - "no": 3
      title: Perturbation des applications de Fredholm
      page: 73
      pdf_page: 87
    - "no": 4
      title: Perturbation des endomorphismes de Riesz
      page: 75
      pdf_page: 89
    - "no": 5
      title: La théorie de Frédéric Riesz
      page: 77
      pdf_page: 91
    - "no": 6
      title: Alternative de Fredholm
      page: 79
      pdf_page: 93
statements: 19
exercises: 11
content_sha256: 00c0f0e72c676ebd456b4c6b9377c906b9ac16d553f5dd1629b67d663477cbc7
translated_from: content/fr/ts/III/05_s5_perturbation_par_une_application.md
source_lang: fr
translation_method: machine
source_content_sha256: b8520dc9762a5d703ee1e574286038de68c8d1f192be8cc257fab0dd44fafa29
translation_model: gpt-5-mini, gpt-5-6-mini
translation_run: translate-en-mt-44a5ece8
glossary_version: 34
glossary_terms_sha256: d5db462f73fd37eddc35ade743bda4190b921b575c314665fa556fd6807c5d36
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 5. PERTURBATION BY A COMPACT LINEAR MAPPING

### 1. Strict morphisms and properness

#### Lemma 1 {#ts-iii-s5-lem-1 .statement tag=02TK}

Let E and F be topological vector spaces, $u$ a continuous linear mapping of E into F and U a neighbourhood of 0 in E. Suppose that $u$ induces a homeomorphism of U onto a closed subset of F. Then the image I of $u$ is closed and $u$ induces a homeomorphism of E onto I.

The set $u(U)$ is a neighbourhood of 0 in I; it is closed in F, hence the subgroup I of F is locally closed at 0, and consequently it is closed (TG, III, p. 7, prop. 4).

Since Ker($u$) meets U only at 0, we have Ker($u$) $=\{0\}$ and the mapping $u$ is injective. Let V be a closed neighbourhood of 0 in E contained in U. Since $u(\mathring{V})$ is a neighbourhood of 0 in $u$(V), there exists a balanced neighbourhood W of 0 in F such that $u(V)\cap W\subset u(\mathring{V})$. The set $\overset{-1}{u}(W)$ is balanced, hence connected. It contains 0 and is contained in $\mathring{V}\cup (E$ - V). Since $\mathring{V}$ and E- V are disjoint open subsets of E, the set $\overset{-1}{u}(W)$ is contained in $\mathring{V}$, whence $W\cap I\subset u(\mathring{V})$. Consequently $u(\mathring{V})$ is a neighbourhood of 0 in I. This implies that $u$ induces a homeomorphism of E onto I.

#### Proposition 1 {#ts-iii-s5-prop-1 .statement tag=02TL}

Let E be a separated locally convex space, F a locally convex space and $u$ a continuous linear mapping of E into F. The following conditions are equivalent:

(i) The mapping $u$ is a strict morphism, its kernel is of finite dimension and its image is closed in F ;

(ii) There exists a closed neighbourhood V of 0 in E such that the restriction of $u$ to V is proper (TG, I, p. 72).

(i) $=\Rightarrow$ (ii) : Suppose that $u$ satisfies condition (i). Since the kernel of $u$ is of finite dimension, it has a topological supplement $E_1$ in E (III, p. 55, prop. 1), and there exists a compact neighbourhood C of 0 in Ker($u$). Identify E with $E_1\times$ Ker($u$); the set $V = E_1\times C$ is then a closed neighbourhood of 0 in E. The restriction of $u$ to V is composed of the projection of $E_1\times C$ onto $E_1$ which is proper (TG, I, p. 77, cor. 5) and of the restriction $u_1$ of $u$ to $E_1$. Now $u_1$ is a homeomorphism of $E_1$ onto a closed subspace of F, hence is proper (TG, I, p. 72, prop. 2). The composite of two proper mappings is proper (TG, I, p. 73, prop. 5, a)), hence the restriction of $u$ to V is proper.

(ii) $=\Rightarrow$ (i) : Let V be a closed neighbourhood of 0 in E such that the restriction $v$ of $u$ to V is proper. The set $V\cap$ Ker($u$) $=\overset{-1}{v}(\{0\})$ is then compact (TG, I, p. 75, th. 1); consequently, the vector space Ker($u$) is locally compact, hence of finite dimension (EVT, I, p. 15, th. 3). Let $E_1$ be a topological supplement of Ker($u$) in E (prop. 1 of III, p. 55); put $V_1= E_1\cap V$. The set $V_1$ is closed in V. The mapping $u|V_1$ is proper (TG, I, p. 74, cor. 1) and injective, hence is a homeomorphism of $V_1$ onto a closed subset of F (TG, I, p. 72, prop. 2). By Lemma 1, the restriction of $u$ to $E_1$ is a homeomorphism of $E_1$ onto a closed subspace of F, hence $u$ is a strict morphism with closed image.

### 2. Perturbation of injective or surjective linear mappings

#### Theorem 1 {#ts-iii-s5-thm-1 .statement tag=02TM}

Let E and F be separated locally convex spaces and $u$ a strict morphism of E into F, whose kernel is of finite dimension and whose image is closed. Let $h$ be a compact linear mapping of E into F. The linear mapping $u+h$ is a strict morphism, its kernel is of finite dimension and its image is closed.

According to prop. 1 of III, p. 71, there exists a closed neighbourhood V of 0 in E such that the restriction of $u$ to V is proper. Since $h$ is compact, there exists a closed neighbourhood W of 0 contained in V such that the set $h(W)$ is relatively compact. Put $C =h(W)$. The restriction of $u$ to W is proper (TG, I, p. 74, cor. 1). The mapping $\alpha :x\mapsto (u(x), h(x))$ from W into $F\times C$ is proper because the mapping pr$_1\circ \alpha =u|W$ from W into F is proper (TG, I, p. 73, prop. 5, d)). The mapping $\beta : (y, z)\mapsto (y+z, z)$ from $F\times C$ into $F\times C$ is a homeomorphism, and the mapping pr$_1$ from $F\times C$ into F is proper (TG, I, p. 77, cor. 5). The composed mapping pr$_1\circ \beta \circ \alpha$ from W into F is therefore proper (TG, I, p. 73, prop. 5, a)). But this mapping is none other than the restriction of $u+h$ to W. According to the prop. 1 of III, p. 71$,u+h$ is a strict morphism, its kernel is of finite dimension and its image is closed.

#### Lemma 2 {#ts-iii-s5-lem-2 .statement tag=02TN}

Let E and F be Fréchet spaces and $u\in \mathscr{L}(E; F)$. The following conditions are equivalent:

(i) The cokernel of $u$ is of finite dimension ;

(ii) The mapping $^tu: F'_c\rightarrow E'_c$ is a strict morphism with closed image whose kernel is of finite dimension.

(i) $=\Rightarrow$ (ii) : Suppose that the cokernel of $u$ is of finite dimension. The mapping $u$ is then a strict morphism (lemma 6 of III, p. 52). According to prop. 2 of EVT, IV, p. 27, the image of $^tu$ is closed in $E'$ endowed with the weak topology, and fortiori in $E'_c$. The kernel of $^tu$ is the orthogonal of the image of $u($loc. cit.) ; it is therefore of finite dimension. Finally, $^tu$ is a strict morphism from $F'_c$ into $E'_c$ according to theorem 1 of EVT, IV, p. 28.

(ii) $=\Rightarrow$ (i) : Suppose that $^tu: F'_c\rightarrow E'_c$ is a strict morphism. According to EVT, IV, p. 28, th. 1, the image of $u$ is closed. The kernel of $^tu$ is the orthogonal of Im($u$) (EVT, IV, p. 27, prop. 2) ; if this kernel is of finite dimension, the image of $u$ is of finite codimension in F.

#### Theorem 2 {#ts-iii-s5-thm-2 .statement tag=02TO}

Let E and F be Fréchet spaces, $u: E\rightarrow F$ a continuous linear mapping whose cokernel is of finite dimension, and $h: E\rightarrow F$ a compact linear mapping. The linear mapping $u+h$ is a strict morphism, its cokernel is of finite dimension and its image is closed.

According to lemma 6 of III, p. 52, it suffices to show that the cokernel of $u+h$ is of finite dimension. Now, according to prop. 9 of III, p. 9, the mapping $^th$ from $F'_c$ into $E'_c$ is compact ; theorem 2 results from theorem 1 and lemma 2.

### 3. Perturbation of Fredholm mappings

#### Theorem 3 {#ts-iii-s5-thm-3 .statement tag=02TP}

Let E be a locally convex space, F a separated locally convex space, $u$ a Fredholm mapping from E into F and $h$ a compact linear mapping from E into F. Then $u+h$ is a Fredholm mapping, and one has ind($u+h$) $=$ ind($u$).

We shall prove the theorem in three steps.

A) Suppose that E and F are Banach spaces. Proposition 2 of III, p. 42 shows that the linear mapping $u$ is a strict morphism with closed image whose kernel and cokernel are of finite dimension. Since E and F are Banach spaces, Theorems 1 and 2 of III, p. 73 imply that, for every $t\in [0,1]$, the linear mapping $u_t=u+th$ has these same properties, and is therefore a Fredholm mapping (III, p. 42, Proposition 2). The mapping $t\mapsto u_t$ of $[0,1]$ into the set $\mathscr{F}(E; F)$ of Fredholm mappings of E into F is continuous. By Theorem 1 of III, p. 58, the mapping $t\mapsto$ ind($u_t$) is locally constant. Since the interval $[0,1]$ of $\mathbf{R}$ is connected, this mapping is constant. Hence ind($u$) $=$ ind($u+h$).

B) Suppose that E = F and $u= 1_E$. By Proposition 5 of III, p. 5, there exist a Banach space G, a continuous linear mapping $p: E\rightarrow G$ and a compact linear mapping $q: G\rightarrow E$ such that $h=q\circ p$. The endomorphism $p\circ q$ of G is compact. By A), $1_G+p\circ q$ is a Fredholm endomorphism of G of index zero. But then $1_E+h= 1_E+q\circ p$ is a Fredholm endomorphism of E of index zero (III, p. 49, Proposition 10, f )).

C) General case. Let $v$ be a quasi-inverse of $u$. The endomorphisms $u\circ v$ and $(u+h)\circ v$ of F differ from $1_F$ by compact linear mappings. By B), they are Fredholm endomorphisms of F of index zero. It follows that $u+h$ is a Fredholm endomorphism (III, p. 40, n$^o2$) of the same index as $u($III, p. 43, n$^o3$, formula (2)).

#### Corollary 1 {#ts-iii-s5-thm-3-cor-1 .statement tag=02TQ}

Let E and F be separated locally convex spaces and $u\in \mathscr{L}(E; F)$. In order that $u$ be a Fredholm mapping, it is necessary and sufficient that there exist a mapping $v\in \mathscr{L}(F; E)$ such that the linear mappings $1_E-v\circ u$ and $1_F-u\circ v$ be compact.

Since a continuous linear mapping of finite rank is compact, the stated condition is necessary.

Let $v$ be an element of $\mathscr{L}(F; E)$ such that the linear mappings $1_E-v\circ u$ and $1_F-u\circ v$ are compact. By Theorem 3$,v\circ u$ and $u\circ v$ are Fredholm mappings. Let $p$ and $q$ be quasi-inverses of $v\circ u$ and $u\circ v$ respectively. Put $w=p\circ v$ and $w'=v\circ q$. With the notations of No.$^o2$ of III, p. 40, one has $w\circ u\equiv 1_E$ and $u\circ w'\equiv 1_F$, whence $w\equiv w\circ u\circ w'\equiv w'$. It follows that $w$ is a quasi-inverse of $u$.

#### Corollary 2 {#ts-iii-s5-thm-3-cor-2 .statement tag=02TR}

Let E and F be separated locally convex spaces and $u\in \mathscr{L}(E; F)$. The following conditions are equivalent:

(i) The mapping $u$ is a Fredholm mapping of index zero;

(ii) There exists an isomorphism $v$ of E onto F such that $u-v$ is of finite rank ;

(iii) There exists an isomorphism $v$ of E onto F such that $u-v$ is compact.

(i) $=\Rightarrow$ (ii) : Suppose that $u$ is a Fredholm mapping of index zero. There exist decompositions into topological direct sums $E = E_1\oplus E_2$ and $F = F_1\oplus F_2$ with $E_2$ and $F_2$ finite-dimensional such that $u$ vanishes on $E_2$ and defines by restriction an isomorphism $u_1$ of $E_1$ onto $F_1($III, p. 42, prop. 2). If ind($u$) $= 0$, then the dimensions of $E_2$ and $F_2$ are equal and there exists an isomorphism $v$ of E onto F extending $u_1$. The kernel of $u-v$ contains $E_1$, hence $u-v$ is of finite rank.

We have (ii) $=\Rightarrow$ (iii) since every continuous linear mapping of finite rank from E into F is compact, and (iii) $=\Rightarrow$ (i) according to th. 3.

### 4. Perturbation of Riesz endomorphisms

Let E be a Banach space. Recall (cf. III, p. 5, prop. 3) that the set $\mathscr{L}^c(E)$ of compact endomorphisms of E is a closed two-sided ideal of the Banach algebra $\mathscr{L}(E)$. The quotient Banach algebra is called the Calkin algebra of E; it is denoted by $\mathscr{C}$alk(E). We denote by $\pi$ the canonical homomorphism of $\mathscr{L}(E)$ onto $\mathscr{C}$alk(E). According to Cor. 1 of III, p. 74, an endomorphism $u$ of E is a Fredholm endomorphism if and only if $\pi (u)$ is invertible in the algebra $\mathscr{C}$alk(E).

#### Proposition 2 {#ts-iii-s5-prop-2 .statement tag=02TS}

Let $u\in \mathscr{L}(E)$ be such that $\|1_E-\pi (u)\|<1$ in the algebra $\mathscr{C}$alk(E). Then $u$ is a Riesz endomorphism of E.

Let $r\geqslant 1$ be an integer such that $\|1_E-\pi (u)\|^r<\frac{1}{2}$. Let $P\in \mathbf{C}[X]$ be the polynomial $\frac{1-(1-X)^r}{X}$. Let $v= 1_E-(1_E-u)^r$. We thus have $v=uP(u)$ and $\|1_E-\pi (v)\|<\frac{1}{2}$. Since the endomorphisms $u$ and $P(u)$ of E commute, it suffices to prove that $v$ is a Riesz endomorphism of E (III, p. 49, prop. 9).

Since $\|1_E-\pi (v)\|<1/2$, there exists, by definition of the quotient norm in the space $\mathscr{C}$alk(E), a compact endomorphism $h$ of E and an endomorphism $w$ of E such that $v= 1_E+h+w$ and $\|w\|<\frac{1}{2}$. According to Corollary 1 of I, p. 22, the element $1_E+w$ is an automorphism of E. Since $h$ is compact, $v= (1_E+w) +h$ is a Fredholm endomorphism of E of index 0 (Cor. 2 of III, p. 74). For every integer $n\geqslant 0$, denote by $N_n$ the kernel of $v^n$. To prove that $v$ is a Riesz endomorphism of E, it suffices to prove that there exists an integer $n\geqslant 0$ such that $N_n= N_{n+1}($III, p. 46, def. 2 and III, p. 46, remark).

Reason by contradiction by supposing the sequence $(N_n)$ strictly increasing. For every $n\in \mathbf{N}$, let $p_n$ be the canonical mapping of E onto the normed space $E/N_n$. Let $c$ be a real number such that $2\|w\|< c <1$. Let $n\in \mathbf{N}$. Since $N_{n+1}$ is different from $N_n$, there exists an element $x_n\in N_{n+1}$ such that $\|p_n(x_n)\|=c$ and such that $\|x_n\|<1$ (indeed, there exists $y\in N_{n+1}/N_n$ of norm $c$ so, for every $\varepsilon  >0$, there exists $x_n\in N_{n+1}$ such that $p_n(x_n) =y$ and $\|x_n\|\leqslant c+\varepsilon$ ).

Let $m,n$ be two integers such that $m > n\geqslant 0$. We have

$$
\|h(x_m)-h(x_n)\|=\|v(x_m-x_n)-(1_E+w)(x_m-x_n)\|
$$

$$
\geqslant \|(v-1_E)(x_m-x_n)\| - \|w(x_m-x_n)\|
$$

$$
\geqslant \|(v-1_E)(x_m-x_n)\| -2\|w\| \tag{1}
$$

since $\|x_m\|\leqslant 1$ and $\|x_n\|\leqslant 1$. Moreover, note that

$$
(v-1_E)(x_m-x_n) =v(x_m-x_n) +x_n-x_m
$$

But since $n < m$ and $v(N_{m+1})\subset N_m$, we have $v(x_m-x_n) +x_n\in N_m$, whence

$$
\|v(x_m-x_n) +x_n-x_m\|\geqslant \|p_m(x_m)\|=c
$$

The inequality (1) therefore gives the lower bound

$$
\|h(x_m)-h(x_n)\|\geqslant c-2\|w\|>0 \tag{2}
$$

The sequence $(h(x_m))_{m\in\mathbf{N}}$ therefore has no value of adherence in E, which contradicts the fact that the image by $h$ of the unit ball of E is relatively compact, since $h$ is compact (remark 1 of III, p. 2).

#### Corollary 1 {#ts-iii-s5-prop-2-cor-1 .statement tag=02TT}

Let E be a separated locally convex space and let $u\in \mathscr{L}(E)$. In order that $u$ be a Riesz endomorphism, it is necessary and sufficient that there exist an element $v$ of $\mathscr{L}(E)$ which commutes with $u$ and such that $1_E-u\circ v$ is compact.

Since every continuous linear mapping of finite rank is compact, the condition is necessary (III, p. 47, prop. 6 d)). Let us prove that it is sufficient. Let $v$ be an element of $\mathscr{L}(E)$ which commutes with $u$ and such that the endomorphism $h= 1_E-u\circ v$ of E is compact. There exist a Banach space G, a continuous linear mapping $p: E\rightarrow G$ and a compact linear mapping $q: G\rightarrow E$ such that $h=q\circ p($III, p. 5, prop. 5). The endomorphism $p\circ q$ of G is compact. According to prop. 2, the linear mapping $1_G-p\circ q$ is a Riesz endomorphism of G. But then $u\circ v= 1_E-q\circ p$ is a Riesz endomorphism of E (III, p. 49, prop. 10, g)). Since $u$ and $v$ commute, $u$ is a Riesz endomorphism of E (III, p. 49, prop. 9).

#### Corollary 2 {#ts-iii-s5-prop-2-cor-2 .statement tag=02TU}

Let E be a separated locally convex space, $u$ a Riesz endomorphism of E and $h\in \mathscr{L}(E)$ a compact linear mapping. If $u$ and $h$ commute, then $u+h$ is a Riesz endomorphism of E.

Let $v$ be the canonical quasi-inverse of $u$. It commutes with $u$ and with $h($III, p. 47, prop. 6), hence with $u+h$. The endomorphism $1_E-(u+h)\circ v$ of E is the sum of the continuous linear mapping of finite rank $1_E-u\circ v$ and the compact linear mapping $-h\circ v$, hence is compact. It follows that $u+h$ is a Riesz endomorphism of E (corollary 1).

#### Proposition 3 {#ts-iii-s5-prop-3 .statement tag=02TV}

Let E be a Banach space. Let $u$ be an endomorphism of E, and let A be its commutant in $\mathscr{L}(E)$. The closure B of $\pi (A)$ in the algebra $\mathscr{C}$alk(E) is a Banach algebra. In order that $u$ be a Riesz endomorphism of E, it is necessary and sufficient that $\pi (u)$ be invertible in B.

Since $\pi (A)$ is a unital subalgebra of $\mathscr{C}$alk(E), its closure B is a Banach algebra. If $u$ is a Riesz endomorphism of E, the element $\pi (u)$ possesses an inverse in $\pi (A)$ (cor. 1), hence in B. Conversely, suppose that $\pi (u)$ has an inverse $s$ in B. By definition of B, there exists an element $v$ of A such that

$$
\|s-\pi (v)\|<\frac{1}{\|\pi(u)\|}
$$

whence $\|1_E-\pi (u\circ v)\|<1$. According to prop. 2, the linear mapping $u\circ v$ is a Riesz endomorphism of E. The same is true of $u$ since $u$ and $v$ commute (III, p. 49, prop. 9).

### 5. The theory of Frédéric Riesz

Let E be a separated locally convex space and let $h$ be a compact endomorphism of E. Let $\lambda \in K$. The endomorphism $\lambda h$ is compact, hence $1_E-\lambda h$ is a Riesz endomorphism of E (cor. 2 of prop. 2 of III, p. 75); denote by $N_{\lambda}$ and $I_{\lambda}$ its null space and its conull space. According to prop. 6 of III, p. 47, the following properties hold:

(i) The vector subspaces $I_{\lambda}$ and $N_{\lambda}$ of E are closed and stable under $h$;

(ii) The locally convex space E is the topological direct sum of $I_{\lambda}$ and $N_{\lambda}$;

(iii) The mapping $1_E-\lambda h$ defines by restriction an automorphism of $I_{\lambda}$;

(iv) The vector space $N_{\lambda}$ is finite-dimensional, and there exists an integer $n_{\lambda}\geqslant 0$ such that $(1_E-\lambda h)^{n_{\lambda}}(x) = 0$ for every $x\in N_{\lambda}$.

These properties determine the spaces $I_{\lambda}$ and $N_{\lambda}$ uniquely (A, VIII, p. 26, remark 2).

#### Lemma 3 {#ts-iii-s5-lem-3 .statement tag=02TW}

Let X be a topological space whose topology possesses a countable basis. Every discrete subset of X is countable.

Let $\mathscr{B}$ be a countable basis of the topology of X and let D be a discrete subset of X. For each element $x$ of D, there exists an element $B_x$ of $\mathscr{B}$ such that $B_x\cap D =\{x\}$. The mapping from D into $\mathscr{B}$ defined by $x\mapsto B_x$ is injective, whence the lemma.

#### Theorem 4 {#ts-iii-s5-thm-4 .statement tag=02TX}

Let E be a separated locally convex space and let $h$ be a compact endomorphism of E. The set Σ of the $\lambda \in K$ such that $1_E-\lambda h$ is not an automorphism of E is a countable, closed and discrete subset of the field K.

The set Σ is also the set of $\lambda \in K$ such that $1_E-\lambda h$ is not injective and the set of $\lambda \in K$ such that $1_E-\lambda h$ is not surjective.

There exist a Banach space G, a continuous linear mapping $p: E\rightarrow G$ and a compact linear mapping $q: G\rightarrow E$ such that $h=q\circ p($III, p. 5, prop. 5). The endomorphism $h'=p\circ q$ of G is compact, and for $1_E-\lambda h$ to be an automorphism of E it is necessary and sufficient that $1_G-\lambda h'$ be an automorphism of G (prop. 10 of III, p. 49, e)). It is therefore enough for us to prove the theorem when E is a Banach space, which we henceforth suppose.

Let $\lambda \in K$. Since the index of a Riesz endomorphism is zero, it amounts to the same thing to say that the mapping $1_E-\lambda h$ is an automorphism of E, or that it is injective, or again that it is surjective.

The set Σ is closed in K since the set of automorphisms of E is open in $\mathscr{L}(E)$. Let $\lambda$ be an element of Σ. We have $\lambda \not = 0$. Denote by N the nilspace of $h$ and by I its conilspace, and denote by $h_I$ and $h_N$ the endomorphisms of I and N which $h$ defines by passing to the subspaces. Then $1_I-\lambda h_I$ is an automorphism of I, and there exists a neighbourhood U of $\lambda$ in K such that $1_I-\mu h_I$ is an automorphism of I for every $\mu\in U$. The endomorphism $1_N-\lambda h_N$ of N is nilpotent; for every $\mu\not =\lambda$, we have

$$
1_N-\mu h_N=\frac{\lambda-\mu}{\lambda}(1_N+\frac{\mu}{\lambda-\mu}(1_N-\lambda h_N))
$$

therefore $1_N-\mu h_N$ is an automorphism of N. Consequently, the set $U\cap \Sigma$ is reduced to the single element $\lambda$ and the set Σ is discrete. It is countable by the lemma 3.

### 6. Fredholm Alternative

#### Proposition 4 (Fredholm Alternative) {#ts-iii-s5-prop-4 .statement tag=02TY}

Let E be a Banach space and let $h$ be a compact endomorphism of E. Let $\lambda$ be an element of K $-\{0\}$. Let F be the kernel of $1_E-\lambda h$ and G the kernel of $1_{E'}-\lambda^th$.

a) The spaces F and G have the same finite dimension $n\geqslant 0$;

b) For $y\in E$, there exists $x\in E$ such that $x-\lambda h(x) =y$ if and only if $\langle y, \ell \rangle = 0$ for all $\ell \in G$;

c) For $\ell \in E'$, there exists $f\in E'$ such that $f-\lambda^th(f) =\ell$ if and only if $\langle x, f\rangle = 0$ for all $x\in F$.

In particular, one and only one of the following conditions is valid:

(i) The space F is nonzero ;

(ii) For every $y\in E$, there exists $x\in E$ such that $x-\lambda h(x) =y$.

Replacing $h$ by $\lambda h$, we reduce to the case where $\lambda = 1$.

The endomorphism $^th$ is compact by corollary 1 of III, p. 9. The endomorphisms $w= 1_E-h$ of E and $w'= 1_{E'}-^th$ of $E'$ are therefore Riesz endomorphisms (cor. 2 of prop. 2 of III, p. 75). In particular, their kernels F and G have finite dimension. Since $w'=^tw$ and the index of $w$ is zero, the dimension of F is equal to that of G by formula (3) of III, p. 43.

For an element $y$ of E, the equation $x-h(x) =y$ has a solution $x\in E$ if and only if $x$ belongs to the image of $w$. Since the dual of the cokernel of $w$ identifies with the kernel G of Ker($^tw$) (EVT, IV, p. 27, prop. 2), this is the case if and only if $\langle y, \ell \rangle = 0$ for all $\ell \in G$.

For an element $\ell$ of $E'$, the equation $f-^th(f) =\ell$ has a solution $f\in E'$ if and only if $f$ belongs to the image of $w'$. Since the image of $^tw$ is the orthogonal of the kernel F of $w$ (EVT, IV, p. 27, prop. 2) this is the case if and only if $\langle x, f\rangle = 0$ for all $x\in F$.

#### Example {#ts-iii-s5-n6-exa-1 .statement tag=02TZ}

Let X be a compact space, $\mu$ a measure on X, real or complex according as K is equal to $\mathbf{R}$ or $\mathbf{C}$, and $N : X\times X\rightarrow K$ a continuous function.

Let E denote the Banach space $\mathscr{C}(X; K)$. Suppose given a function $a\in E$ and $\lambda \in K-\{0\}$. Let us study the problem of the existence and uniqueness of the solutions $f\in E$ of the integral equation

$$
f(x)-\lambda \int_XN(x, y)f(y)d\mu(y) =a(x)(x\in X) \tag{3}
$$

For this, introduce the set $F_{\lambda}$ of the solutions $f\in E$ of the associated homogeneous equation

$$
f(x)-\lambda \int_XN(x, y)f(y)d\mu(y) = 0(x\in X) \tag{4}
$$

and the set $G_{\lambda}$ of the solutions $g\in E$ of the transposed homogeneous equation of (4), that is to say

$$
g(y)-\lambda \int_XN(x, y)g(x)d\mu(x) = 0(y\in X) \tag{5}
$$

If it is not empty, the set of the solutions of (3) is an affine subspace of E with direction $F_{\lambda}$.

For $f\in E$ and $x\in X$, put

$$
h(f)(x) =\int_XN(x, y)f(y)d\mu(y)
$$

the mapping $f\mapsto h(f)$ thus defined is a compact endomorphism of the Banach space E (cor. of prop. 2 of III, p. 26). The dual $E'$ of E consists of the measures on X, real or complex according as K is equal to $\mathbf{R}$ or $\mathbf{C}$ (INT, III, p. 47, § 1, n$^o3$, def. 2). The transpose $^th$ of $h$ is the endomorphism of $E'$ characterized by the relation $\langle f,^th(m)\rangle =\langle h(f), m\rangle$ for $f\in E$ and $m\in E'$, that is to say

$$
\int_Xf(x)d(^th(m))(x) =\int_Xh(f)(x)dm(x)
$$

$$
=\int_X(\int_XN(x, y)f(y)d\mu(y))dm(x)
$$

$$
=\int_X(\int_XN(x, y)dm(x))f(y)d\mu(y) \tag{6}
$$

for $m\in E'$ and $f\in E$ (INT, III, p. 84, § 4, n$^o1$, th. 2).

#### Lemma 4 {#ts-iii-s5-lem-4 .statement tag=02U0}

The linear mapping from $G_{\lambda}$ into $E'$ defined by $g\mapsto g\cdot \mu$ is injective, and its image is the kernel of $1_{E'}-\lambda^th$.

If $g\in G_{\lambda}$ satisfies $g\cdot \mu= 0$, then formula (5) implies $g= 0$, hence the mapping $g\mapsto g\cdot \mu$ is injective.

Let $m\in E'$ be a measure belonging to the kernel of $1_{E'}-\lambda^th$. According to relation (6), one has

$$
\int_Xf(x)dm(x) =\lambda \int_X(\int_XN(x, y)dm(x))f(y)d\mu(y) \tag{7}
$$

for every continuous function $f: X\rightarrow K$. The measure $m$ is therefore equal to the measure $g\cdot \mu$, where $g$ is the continuous function from X into K defined by

$$
g(y) =\lambda \int_XN(x, y)dm(x) \tag{8}
$$

for every $y\in X$. Formula (8) then implies that the function $g$ belongs to $G_{\lambda}$.

Conversely, let $g: X\rightarrow K$ be a continuous function belonging to $G_{\lambda}$ and put $m=g\cdot \mu$. For every continuous function $f: X\rightarrow K$, we therefore have

$$
\int_Xf(y)dm(y) =\int_Xg(y)f(y)d\mu(y)
$$

$$
=\lambda \int_X(\int_XN(x, y)g(x)d\mu(x))f(y)d\mu(y)
$$

$$
=\lambda \int_Xf(x)dm(x)
$$

so that $^th(m) =\lambda m$. This proves Lemma 4.

By applying Proposition 4 and Theorem 4 of III, p. 78. to the endomorphism $h$, one then obtains the following statements.

#### Theorem 5 {#ts-iii-s5-thm-5 .statement tag=02U1}

Let $\lambda \in K$.

a) The sets $F_{\lambda}$ and $G_{\lambda}$ are finite-dimensional vector subspaces of $\mathscr{C}(X; K)$ and their dimensions are equal ;

b) In order that equation (3) have at least one solution $f\in \mathscr{C}(X,K)$, it is necessary and sufficient that one have $\int_Xa(x)g(x)d\mu(x) = 0$ for every function $g\in G_{\lambda}$. The set of solutions of (3) is then an affine subspace of $\mathscr{C}(X; K)$ with direction $F_{\lambda}$;

c) One of the following conditions, which exclude each other, is satisfied :

(i) For every function $a\in \mathscr{C}(X; K)$, there exists a unique

solution $f\in \mathscr{C}(X; K)$ of the integral equation (3) ;

(ii) The homogeneous equation (4) possesses a nonzero solution

$$
f\in \mathscr{C}(X; K)
$$

#### Corollary {#ts-iii-s5-n6-cor-1 .statement tag=02U2}

The set of the $\lambda \in K$ for which the space $F_{\lambda}$ is not zero is a countable, closed and discrete subset of K.

## EXERCISES {#ts-iii-s5-exercises}

In the following exercises, when E is a Banach space, one denotes by $\mathscr{C}$alk(E) the Calkin algebra $\mathscr{L}(E)/\mathscr{L}^c(E)$. One denotes by $\pi$ the canonical projection of $\mathscr{L}(E)$ into $\mathscr{C}$alk(E).

If E is a complex Hilbert space, $\mathscr{C}$alk(E) is provided with the involution deduced from the involution of $\mathscr{L}(E)$ by passing to the quotient.

See the [exercises for § 5](exercises/s5/).
