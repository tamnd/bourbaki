---
book: ts
book_title: Théories spectrales
chapter: I
chapter_title: ALGÈBRES NORMÉES
section: 4
section_title: Calcul fonctionnel holomorphe
lang: en
source: ts-i-ii-fr
book_pages: TS I.49-TS I.88, TS I.172-TS I.177
pdf_pages: 0062-0101, 0185-0190
extraction: native
subsections:
    - "no": 1
      title: Germes de fonctions holomorphes
      page: 49
      pdf_page: 62
    - "no": 2
      title: Énoncé du théorème principal
      page: 51
      pdf_page: 64
    - "no": 3
      title: Suites adaptées et formes différentielles associées
      page: 52
      pdf_page: 65
    - "no": 4
      title: Construction des applications $\Theta_{\boldsymbol{a}}$
      page: 58
      pdf_page: 71
    - "no": 5
      title: Propriétés des applications $\Theta_{\boldsymbol{a}}$
      page: 61
      pdf_page: 74
    - "no": 6
      title: Théorèmes d’approximation
      page: 67
      pdf_page: 80
    - "no": 7
      title: Existence et unicité du calcul fonctionnel holomorphe
      page: 70
      pdf_page: 83
    - "no": 8
      title: Substitution dans le calcul fonctionnel
      page: 72
      pdf_page: 85
    - "no": 9
      title: Calcul fonctionnel holomorphe en une variable
      page: 74
      pdf_page: 87
    - "no": 10
      title: Exponentielle et logarithme
      page: 78
      pdf_page: 91
    - "no": 11
      title: Partitions de l’espace des caractères
      page: 79
      pdf_page: 92
    - "no": 12
      title: Partitions du spectre d’un élément
      page: 81
      pdf_page: 94
    - "no": 13
      title: Calcul fonctionnel holomorphe dans une algèbre normable complète réelle ou complexe
      page: 85
      pdf_page: 98
    - "no": 14
      title: Cas d’une algèbre sans élément unité
      page: 88
      pdf_page: 101
statements: 55
exercises: 18
content_sha256: bfd3dd87c3f14314ac07c57cc45fa868c6aacf7968e0d4fd61ff3372c2d96b1d
translated_from: content/fr/ts/I/04_s4_calcul_fonctionnel_holomorphe.md
source_lang: fr
translation_method: machine
source_content_sha256: c9001c326aa1e0c5c534ba4c11cbd814c51f66f6a0e2b17538081e873d9f5b50
translation_model: gpt-5-6-mini, gpt-5-mini, gpt-5.4
translation_run: translate-en-mt-921bb1a3
glossary_version: 34
glossary_terms_sha256: 788820ef53501261e218b02462eec1bb99eaf6ed632f9a6c69c6f6ff8b893cd5
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 4. HOLOMORPHIC FUNCTIONAL CALCULUS

### 1. Germs of holomorphic functions

Let E and F be complex Banach spaces. We recall (cf. VAR, R1, p. 26, 3.2.1, p. 22, 3.1 and p. 88, App.) that a holomorphic mapping defined on an open set U of E and with values in F is a mapping $f: U\rightarrow F$ such that, for every $x\in U$, there exists a convergent series

$$
f_x=\sum_{k\geqslant 0}f_{x,k}
$$

satisfying $f(x+y) =f_x(y)$ for every $y\in E$ sufficiently close to 0, where $f_{x,k}: E\rightarrow \mathbf{C}$ is a continuous homogeneous polynomial of degree $k$ on E with values in F, that is to say a mapping of the form

$$
f_{x,k}(y) =\widetilde{f}_{x,k}(y, . . . , y)
$$

where $\widetilde{f}_{x,k}: E^k\rightarrow F$ is a continuous $k$-multilinear mapping. We denote by $\mathscr{O}(U; F)$ the complex vector space of holomorphic functions on U with values in F endowed with the topology of compact convergence. It is a locally convex topological vector space, whose topology is defined by the semi-norms $f\mapsto$ sup$_{z\in K}\|f(z)\|$, where K runs through the set of compact subsets of U.

Let G be a complex Banach space and V an open subset of G. For every holomorphic mapping $\varphi : V\rightarrow$ U, the mapping $\varphi^*:f\mapsto f\circ \varphi$ is a continuous linear mapping from $\mathscr{O}(U; F)$ into $\mathscr{O}(V; F)$.

If H is a complex Banach space and $\varphi : F\rightarrow H$ is a continuous linear mapping, then the mapping $f\mapsto \varphi \circ f$ is a continuous linear mapping from $\mathscr{O}(U; F)$ into $\mathscr{O}(U; H)$, denoted by $\varphi_*$.

Let $n$ be a natural number and put $E =\mathbf{C}^n$. Let K be a compact subset of $\mathbf{C}^n$ and $\mathscr{U}$ the decreasing directed set of open neighbourhoods of K. If $U,U'\in \mathscr{U}$ and $U'\subset U$, the restriction mapping of functions from $\mathscr{O}(U; F)$ into $\mathscr{O}(U'; F)$ is continuous. The inductive limit of the spaces $\mathscr{O}(U; F)$ for these mappings is denoted by $\mathscr{O}(K; F)$. The elements of $\mathscr{O}(K; F)$ are called germs of holomorphic functions in a neighbourhood of K and with values in F.

The space $\mathscr{O}(K; F)$ is endowed with the inductive limit topology of the locally convex topologies of the $\mathscr{O}(U; F)$ (EVT, II, p. 31, example II). Let X be a locally convex topological vector space and $\varphi :\mathscr{O}(K; F)\rightarrow X$ a mapping. For every open neighbourhood U of K, the mapping $\mathscr{O}(U; F)\rightarrow X$ deduced from $\varphi$ by composition with the canonical mapping $\mathscr{O}(U; F)\rightarrow \mathscr{O}(K; F)$ is denoted by $\varphi^U$. The mapping $\varphi$ is continuous if and only if $\varphi^U$ is continuous for every U (EVT, II, p. 29, prop. 5, (iii)).

Let $m$ be a natural number. Let L be a compact subset of $\mathbf{C}^m$ and V an open neighbourhood of L. Let $\varphi : V\rightarrow \mathbf{C}^n$ be a holomorphic mapping such that $\varphi (L)\subset K$. The continuous linear mappings

$-1$

$$
\mathscr{O}(U; F)^{\varphi}\leftarrow^{^*}\rightarrow \mathscr{O}(\overset{-1}{\varphi}(U); F)^{\varphi^{\varphi}}\leftarrow^{^{(U)}}\rightarrow \mathscr{O}(L; F)
$$

for U an open neighbourhood of K, induce a continuous linear mapping $\varphi^*:\mathscr{O}(K; F)\rightarrow \mathscr{O}(L; F)$ (loc. cit.).

Let H be a complex Banach space and $\varphi : F\rightarrow H$ a continuous linear mapping. The continuous linear mappings

$$
\mathscr{O}(U; F)^{\varphi}\leftarrow_{_*}\rightarrow \mathscr{O}(U; H)^{\varphi}\leftarrow^{^U}\rightarrow \mathscr{O}(K; F)
$$

where U runs through the set of open neighbourhoods of K in $\mathbf{C}^n$, induce a continuous linear mapping $\varphi_*$ from $\mathscr{O}(K; F)$ into $\mathscr{O}(K; H)$ (loc. cit.). We shall sometimes write $\varphi \circ f=\varphi_*(f)$.

For every open neighbourhood U of K, the restriction to K is a continuous linear mapping $\mathscr{O}(U; F)\rightarrow \mathscr{C}(K; F)$; these mappings induce a continuous linear mapping $\mathscr{O}(K; F)\rightarrow \mathscr{C}(K; F)$, called evaluation of germs of holomorphic functions on K.

Soit A a unital complex Banach algebra. The spaces $\mathscr{O}(U; A)$ and $\mathscr{O}(K; A)$ are unital algebras. If $A\not=\{0\}$, one can canonically identify $\mathscr{O}(U;\mathbf{C})$ (resp. $\mathscr{O}(K;\mathbf{C})$) with the subalgebra $\mathscr{O}(U;\mathbf{C})\cdot 1$ of $\mathscr{O}(U; A)$ (resp. with the subalgebra $\mathscr{O}(K;\mathbf{C})\cdot 1$ of $\mathscr{O}(K; A)$). We shall put $\mathscr{O}(U) =\mathscr{O}(U;\mathbf{C})$ and $\mathscr{O}(K) =\mathscr{O}(K;\mathbf{C})$.

### 2. Statement of the principal theorem

Let X be a set. If $m\leqslant n$, we shall denote by $\pi_{m,n}$ the mapping from $X^n$ into $X^m$ such that $\pi_{m,n}(\boldsymbol{x}) = (x_1, . . . , x_m)$ for every $\boldsymbol{x}= (x_1, . . . , x_n)\in X^n$.

Let A be a unital Banach algebra over $\mathbf{C}$. For every integer $n\geqslant 1$ and every $\boldsymbol{a}\in A^n$, we denote by Sp$^n(\boldsymbol{a})$ the simultaneous spectrum Sp$^{\{1,...,n\}}_A(\boldsymbol{a})$ (def. 2 of I, p. 42). It is a compact subset of $\mathbf{C}^n$. For every integer $m$ such that $1\leqslant m\leqslant n$, one has $\pi_{m,n}$(Sp$^n(\boldsymbol{a})$) $=$ Sp$^m(\pi_{m,n}(\boldsymbol{a}))$ (I, p. 41, n$^o6$). The continuous linear mapping

$\pi_{m,n}^*:\mathscr{O}$(Sp$^m(\pi_{m,n}(\boldsymbol{a})); A$)$\longrightarrow \mathscr{O}$(Sp$^n(\boldsymbol{a}); A$)

is a morphism of unital algebras.

Let A be a commutative unital Banach algebra over $\mathbf{C}$. Let $n\geqslant 1$ be an integer. A holomorphic functional calculus in $n$ variables on A is the data, for every $\boldsymbol{a}\in A^n$, of a mapping

$\Theta_{\boldsymbol{a}}:\mathscr{O}$(Sp$^n(\boldsymbol{a}); A$)$\longrightarrow A$

satisfying the conditions:

(CF1) For every $\boldsymbol{a}\in A^n$, the mapping $\Theta_{\boldsymbol{a}}$ is a continuous morphism of unital algebras.

(CF2) If $\boldsymbol{a}= (a_1, . . . , a_n)$, and if $z_1, . . . , z_n$ denote the germs in the neighbourhood of Sp$^n(\boldsymbol{a})$ of the coordinate functions on $\mathbf{C}^n$, one has

$$
\Theta_{\boldsymbol{a}}(z_1) =a_1, . . . ,\Theta_{\boldsymbol{a}}(z_n) =a_n
$$

#### Remark {#ts-i-s4-n2-rem-1 .statement tag=029U}

If the radical of the algebra A is zero, one can omit the continuity condition in (CF1) (cf. prop. 9 of I, p. 40).

A holomorphic functional calculus on A is the data, for every integer $n\geqslant 1$, of a holomorphic functional calculus in $n$ variables on A, satisfying:

(CF3) Whatever the integers $m$ and $n$ such that $1\leqslant m\leqslant n$, and whatever $\boldsymbol{a}\in A^n$ and $f\in \mathscr{O}$(Sp$^m(\pi_{m,n}(\boldsymbol{a}); A)$, one has

$$
\Theta_{\boldsymbol{a}}(\pi^*_{m,n}(f)) = \Theta_{\pi_{m,n}(\boldsymbol{a})}(f)
$$

The object of this paragraph is to prove the following theorem:

#### Theorem 1 {#ts-i-s4-thm-1 .statement tag=029V}

Let A be a commutative complex unital Banach algebra. There exists a unique holomorphic functional calculus on A.

The proof of this theorem will occupy nos. $^{os}3$ to 7.

### 3. Adapted sequences and associated differential forms

In this number, and up to number 5, we denote by A a commutative complex unital Banach algebra and $n$ an integer $\geqslant 1$.

When we shall speak of infinitely differentiable functions on an open subset of $\mathbf{C}^n$, it will be a question of infinitely differentiable functions for the underlying structure of real manifold. The notions of differential calculus used will be relative to this structure.

#### Definition 1 {#ts-i-s4-def-1 .statement tag=029W}

Let $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$, let $h:\mathbf{C}^n\rightarrow \mathbf{C}$ be a mapping and let $u_1, . . . , u_n$ be mappings of $\mathbf{C}^n$ into A. We say that the sequence $(h, u_1, . . . , u_n)$ is adapted to $\boldsymbol{a}$ if

(i) The mapping $h$ is infinitely differentiable, of compact support, and equal to 1 in the neighbourhood of Sp$^n(\boldsymbol{a})$ ;

(ii) The mappings $u_1, . . . ,u_n$ are infinitely differentiable ;

(iii) For every $\boldsymbol{z}= (z_1, . . . , z_n)\in \mathbf{C}^n$, one has

$$
h(\boldsymbol{z}) + (z_1-a_1)u_1(\boldsymbol{z}) +\cdots + (z_n-a_n)u_n(\boldsymbol{z}) = 1 \tag{1}
$$

The differential form of degree $2n$ on $\mathbf{C}^n$, with coefficients in A, defined by

$$
\omega =\bigwedge_{i=1}^n(du_i\wedge dz_i)
$$

is called the differential form associated with $(h, u_1, . . . , u_n)$.

If $(h, u_1, . . . , u_n)$ is adapted to $\boldsymbol{a}$, then, by differentiating (1), one obtains the equality

$$
dh=-\sum_{i=1}^nu_idz_i-\sum_{i=1}^n(z_i-a_i)du_i \tag{2}
$$

whence, for every $i$ such that $1\leqslant i\leqslant n$, the relation

$$
dh\wedge dz_i\wedge \bigwedge_{j\not=i}(du_j\wedge dz_j) =-(z_i-a_i)\omega \tag{3}
$$

#### Lemma 1 {#ts-i-s4-lem-1 .statement tag=029X}

Let U be an open subset of $\mathbf{C}^n$ and K a compact subset of U. There exists an infinitely differentiable mapping $h$ of $\mathbf{C}^n$ into $\mathbf{C}$, equal to 1 on K and with compact support contained in U.

Let V be a relatively compact open neighbourhood of K such that $\overline{V}$ is contained in U (TG, I, p. 65, prop. 10). There exists an infinitely differentiable function $h$ of $\mathbf{C}^n$ into $\mathbf{C}$ whose support is contained in V and which is equal to 1 on K (VAR, R1, p. 40, 5.3.6). This function has the required properties.

#### Example {#ts-i-s4-n3-exa-1 .statement tag=029Y}

Suppose that $n= 1$. Let $a\in A$. For every open neighbourhood U of Sp($a$), there exists an infinitely differentiable mapping $h$ of $\mathbf{C}$ into $\mathbf{C}$ with compact support contained in U, equal to 1 in the neighbourhood of Sp($a$) (VAR, R1, p. 40, 5.3.6). Put

$$
u(z) = (1-h(z))(z-a)^{-1}
$$

for $z\in \mathbf{C}-$ Sp($a$) and $u(z) = 0$ if $z\in$ Sp($a$). The pair $(h, u)$ is adapted to $a$ and the associated differential form is $\omega =du\wedge dz$.

#### Lemma 2 {#ts-i-s4-lem-2 .statement tag=029Z}

Let $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$. There exist infinitely differentiable mappings $v_1, . . . , v_n$ of $\mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$ into A such that

$$
(z_1-a_1)v_1(\boldsymbol{z}) +\cdots + (z_n-a_n)v_n(\boldsymbol{z}) = 1
$$

for every $\boldsymbol{z}= (z_1, . . . , z_n)\in \mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$.

Let $\boldsymbol{w}= (w_1, . . . , w_n)\in \mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$. By definition of the simultaneous spectrum, there exist $b_1, . . . , b_n$ in A such that

$$
(w_1-a_1)b_1+\cdots + (w_n-a_n)b_n= 1
$$

(I, p. 41, n$^o6$). There exists an open neighbourhood $W_{\boldsymbol{w}}$ of $\boldsymbol{w}$ such that the element $(z_1-a_1)b_1+\cdots + (z_n-a_n)b_n$ of A is invertible if $\boldsymbol{z}= (z_1, . . . , z_n)$ belongs to $W_{\boldsymbol{w}}$. For every integer $j$ such that $1\leqslant j\leqslant n$ and every $\boldsymbol{z}$ in $W_{\boldsymbol{w}}$, let

$$
u_j(\boldsymbol{z}) =b_j(\sum_{i=1}^n(z_i-a_i)b_i)^{-1}
$$

The functions $u_1, u_2, . . . , u_n$ from $W_{\boldsymbol{w}}$ into A thus defined are infinitely differentiable in $W_{\boldsymbol{w}}$, and we have

$$
(z_1-a_1)u_1(\boldsymbol{z}) +\cdots + (z_n-a_n)u_n(\boldsymbol{z}) = 1
$$

for every $\boldsymbol{z}$ in $W_{\boldsymbol{w}}$.

Since the family $(W_{\boldsymbol{w}})_{\boldsymbol{w}\in\mathbf{C}^{n-}Sp^n(\boldsymbol{a})}$ is an open covering of $\mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$, there exists a locally finite open covering $\mathscr{W}= (W_{\lambda})_{\lambda\in L}$ (TG, I, p. 70, th. 5) and, for every $\lambda \in L$, functions $u_{1\lambda}, . . . , u_{n\lambda}$, with values in A, defined and infinitely differentiable in $W_{\lambda}$, such that $(z_1-a_1)u_{1\lambda}(\boldsymbol{z}) +\cdots + (z_n-a_n)u_{n\lambda}(\boldsymbol{z}) = 1$ for every $\boldsymbol{z}$ in $W_{\lambda}$. Let $(f_{\lambda})_{\lambda\in L}$ be a partition of unity subordinate to the covering $\mathscr{W}$ formed by infinitely differentiable functions (VAR, R1, p. 40, 5.3.6). Let $i$ be an integer such that $1\leqslant i\leqslant n$. For every $\lambda \in L$, let $u'_{i\lambda}$ be the mapping from $\mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$ into A obtained by extending by 0 the function $f_{\lambda}u_{i\lambda}$ in $(\mathbf{C}^n-$ Sp$^n(\boldsymbol{a}))-W_{\lambda}$. The functions $u'_{i\lambda}$ are infinitely differentiable. The family (Supp($u'_{i\lambda}$))$_{\lambda\in L}$ being locally finite, the function $v_i=\sum_{\lambda\in L}u'_{i\lambda}$ is defined and infinitely differentiable in

$\mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$.

Let $\boldsymbol{z}\in \mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$. Denote by $L'$ the finite set of the $\lambda \in L$ such that $\boldsymbol{z}\in W_{\lambda}$. Then

$$
\sum_{i=1}^n(z_i-a_i)v_i(\boldsymbol{z}) =\sum_{\lambda\in L'}\sum_{i=1}^n(z_i-a_i)u'_{i\lambda}(\boldsymbol{z})
$$

$$
=\sum_{\lambda\in L'}f_{\lambda}(\boldsymbol{z})\sum_{i=1}^n(z_i-a_i)u_{i\lambda}(\boldsymbol{z}) =(\sum_{\lambda\in L'}f_{\lambda}(\boldsymbol{z}))\cdot 1 = 1
$$

#### Lemma 3 {#ts-i-s4-lem-3 .statement tag=02A0}

Let $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$. Let $h$ be a mapping from $\mathbf{C}^n$ into $\mathbf{C}$, infinitely differentiable, equal to 1 in a neighbourhood of Sp$^n(\boldsymbol{a})$ and with compact support. There exist infinitely differentiable mappings $u_1, . . . , u_n$ from $\mathbf{C}^n$ into A such that the sequence $(h, u_1, . . . , u_n)$ is adapted to $\boldsymbol{a}$.

Let $v_1, . . . ,v_n$ be infinitely differentiable mappings from $\mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$ into A, such that

$$
\sum_{j=1}^n(z_j-a_j)v_j(\boldsymbol{z}) = 1
$$

for $\boldsymbol{z}$ in $\mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$ (lemma 2). Let $i$ be an integer such that $1\leqslant i\leqslant n$. Put $u_i(\boldsymbol{z}) = (1-h(\boldsymbol{z}))v_i(\boldsymbol{z})$ if $\boldsymbol{z}\in \mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$ and $u_i(\boldsymbol{z}) = 0$ if $\boldsymbol{z}\in$ Sp$^n(\boldsymbol{a})$. The mappings $u_i$ are infinitely differentiable in $\mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$ and vanish in a neighbourhood of Sp$^n(\boldsymbol{a})$, hence are infinitely differentiable in $\mathbf{C}^n$. Equality (1) holds in Sp$^n(\boldsymbol{a})$ because the functions $u_i$ vanish on Sp$^n(\boldsymbol{a})$ and $h$ is equal to 1 in a neighbourhood of Sp$^n(\boldsymbol{a})$. It also holds on $\mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$ by construction.

#### Lemma 4 {#ts-i-s4-lem-4 .statement tag=02A1}

Let $\boldsymbol{a}\in A^n$. Let $(h, u_1, . . . , u_n)$ be a sequence adapted to $\boldsymbol{a}$ and $\omega$ the associated differential form.

a) For $i= 1,2, . . . , n$, there exists a differential form $\beta_i$ on $\mathbf{C}^n$, of degree $n-1$, with coefficients in A, such that

$(z_i-a_i)\omega =d(h\beta_i\wedge dz_1\wedge  \cdots  \wedge dz_n)$ ;

b) The differential form $\omega$ has compact support contained in the support of $h$;

c) There exists a differential form $\beta$ on $\mathbf{C}^n$, of degree $n-1$, with coefficients in A, such that

$$
(n+ 1)h\omega -\omega =d(h\beta \wedge dz_1\wedge  \cdots  \wedge dz_n)
$$

Let $i$ be an integer such that $1\leqslant i\leqslant n$. There exists $\varepsilon_i\in  \{-1,1\}$ such that

$$
\varepsilon_i\bigwedge_{j\not=i}du_j\wedge dz_1\wedge  \cdots  \wedge dz_n=dz_i\wedge \bigwedge_{j\not=i}(du_j\wedge dz_j)
$$

Put $\beta_i=\varepsilon_i\bigwedge_{j\not=i}du_j$, so that the term on the left in this formula is $\beta_i\wedge dz_1\wedge  \cdots  \wedge dz_n$ and that $d\beta_i= 0$. Thus

$$
d(h\beta_i\wedge dz_1\wedge  \cdots  \wedge dz_n)=dh\wedge \beta_i\wedge dz_1\wedge  \cdots  \wedge dz_n=
$$

$$
dh\wedge dz_i\wedge \bigwedge_{j\not=i}(du_j\wedge dz_j) = (z_i-a_i)\omega
$$

by formula (3), whence assertion a).

From assertion a) and formula (1) one deduces the relation

$$
\omega =h\omega + (1-h)\omega =h\omega +\sum_{i=1}^n(z_i-a_i)u_i\omega
$$

$$
=h\omega +\sum_{i=1}^nu_id(h\beta_i\wedge dz_1\wedge  \cdots  \wedge dz_n)
$$

whence Supp($\omega$ )$\subset$ Supp($h$), which proves b).

Finally, put

$\beta =\sum_{i=1}^n\varepsilon_iu_i\bigwedge_{j\not=i}du_j=\sum_{i=1}^nu_i\beta_i$, and $\tau =h\beta dz_1\wedge  \cdots  \wedge dz_n$.

We have $d\beta =\sum_idu_i\wedge \beta_i$ and therefore

$$
d\beta \wedge dz_1\wedge  \cdots  \wedge dz_n=\sum_idu_i\wedge dz_i\wedge \bigwedge_{j\not=i}(du_j\wedge dz_j) =n\omega
$$

Thus

$$
d\tau =dh\wedge \beta \wedge dz_1\wedge  \cdots  \wedge dz_n+hd\beta \wedge dz_1\wedge  \cdots  \wedge dz_n
$$

$$
=\sum_{i=1}^nu_idh\wedge dz_i\wedge \bigwedge_{j\not=i}(du_j\wedge dz_j) +nh\omega
$$

$$
=-\sum_{i=1}^nu_i(z_i-a_i)\omega +nh\omega = (h-1)\omega +nh\omega = (n+ 1)h\omega -\omega
$$

taking account of formulas (3) and (1), whence c).

We now propose to study how the differential form $\omega$ associated with a sequence adapted to $\boldsymbol{a}$ varies as a function of this sequence. We shall say that sequences $(h, u_1, . . . , u_n)$ and $(h', u'_1, . . . , u'_n)$ adapted to $\boldsymbol{a}$ are linked if there exists a differential form $\psi$ of degree $n-1$ on $\mathbf{C}^n$, with coefficients in A and with support contained in the union of the supports of $h$ and of $h'$, such that the associated differential forms $\omega$ and $\omega '$ satisfy

$$
\omega -\omega '=d(\psi \wedge dz_1\wedge dz_2\wedge  \cdots  \wedge dz_n)
$$

Let us begin with an elementary modification:

#### Lemma 5 {#ts-i-s4-lem-5 .statement tag=02A2}

Let $\boldsymbol{a}\in A^n$, let $(h, u_1, . . . , u_n)$ be a sequence adapted to $\boldsymbol{a}$, and let $\omega$ be the associated differential form.

Let $w$ be an indefinitely differentiable mapping of $\mathbf{C}^n$ into A, and let $i$ and $j$ be distinct integers between 1 and $n$. Define $u'_1, . . . , u'_n$ by

$$
u'_i=u_i+ (z_j-a_j)w,u'_j=u_j-(z_i-a_i)w
$$

$u'_k=u_k$ for $k\not=i, j$.

Then the sequence $(h, u'_1, . . . , u'_n)$ is adapted to $\boldsymbol{a}$ and is linked to the sequence $(h, u_1, . . . , u_n)$.

Let us write $d\boldsymbol{z}=dz_1\wedge  \cdots  \wedge dz_n$. Since

$$
\sum_{k=1}^n(z_k-a_k)u'_k(\boldsymbol{z}) =\sum_{k=1}^n(z_k-a_k)u_k(\boldsymbol{z}) +w(\boldsymbol{z})(z_j-a_j)(z_i-a_i)
$$

$$
-w(\boldsymbol{z})(z_i-a_i)(z_j-a_j) = 1-h(\boldsymbol{z})
$$

for every $z\in \mathbf{C}^n$, the sequence $(h, u'_1, . . . , u'_n)$ is adapted to $\boldsymbol{a}$. Further, we have

$$
du'_i\wedge du'_j\wedge dz_1\wedge  \cdots  \wedge dz_n=
$$

$$
(du_i+w dz_j+ (z_j-a_j)dw)\wedge (du_j-w dz_i-(z_i-a_i)dw)\wedge d\boldsymbol{z}
$$

$$
=(du_i\wedge du_j-(z_i-a_i)du_i\wedge dw-(z_j-a_j)du_j\wedge dw)\wedge d\boldsymbol{z}
$$

There therefore exists $\varepsilon \in  \{-1,1\}$ such that $\varepsilon (\omega -\omega ')$ is equal to

$$
du'_i\wedge du'_j\wedge \bigwedge_{k\not=i,j}du'_k\wedge d\boldsymbol{z}-du_i\wedge du_j\wedge \bigwedge_{k\not=i,j}du_k\wedge d\boldsymbol{z}
$$

$$
=-((z_i-a_i)du_i\wedge dw+ (z_j-a_j)du_j\wedge dw)\wedge \bigwedge_{k\not=i,j}du_k\wedge d\boldsymbol{z}
$$

$$
=-(\sum_{k=1}^n(z_k-a_k)du_k)\wedge dw\wedge \bigwedge_{k\not=i,j}du_k\wedge d\boldsymbol{z}
$$

and, taking account of (2), this is equal to

$$
dh\wedge dw\wedge \bigwedge_{k\not=i,j}du_k\wedge d\boldsymbol{z}=d(h dw\wedge \bigwedge_{k\not=i,j}du_k\wedge d\boldsymbol{z})
$$

whence the result.

#### Lemma 6 {#ts-i-s4-lem-6 .statement tag=02A3}

Let $\boldsymbol{a}\in A^n$. All sequences adapted to $\boldsymbol{a}$ are linked.

Let $(h, u_1, . . . , u_n)$ and $(h', u'_1, . . . , u'_n)$ be sequences adapted to $\boldsymbol{a}$, and let us denote by $\omega$ and $\omega '$ the associated differential forms.

Define the indefinitely differentiable mappings

$$
w_{ij}=u'_iu_j-u_iu'_j,1\leqslant i\leqslant n,1\leqslant j\leqslant n
$$

$$
s_i=u'_ih-u_ih',1\leqslant i\leqslant n
$$

so that $w_{ji}=-w_{ij}$, and Supp($s_i$)$\subset$ Supp($h$)$\cup$ Supp($h'$).

Let $u''_i=u'_i-s_i,\boldsymbol{u}= (u_1, . . . , u_n)$ and $\boldsymbol{u}''= (u''_1, . . . , u''_n)$. Let us also denote by $\boldsymbol{v}_{ij}$ the mapping of $\mathbf{C}^n$ into $A^n$ whose $i$-th component is $(z_j-a_j)w_{ij}$, whose $j$-th component is $(z_i-a_i)w_{ji}=-(z_i-a_i)w_{ij}$, and whose other components are zero. Then we have

$$
\boldsymbol{u}''=\boldsymbol{u}+\sum_{i<j}\boldsymbol{v}_{ij}
$$

In fact, for every integer $k$ such that $1\leqslant k\leqslant n$, the $k$-th component of the right-hand side is

$$
u_k+\sum^{k-1}_{i=1}(z_i-a_i)w_{ki}+\sum_{j=k+1}^n(z_j-a_j)w_{kj}=u_k+\sum_{i=1}^n(z_i-a_i)w_{ki}
$$

$$
=u_k+u'_k\sum_{i=1}^n(z_i-a_i)u_i-u_k\sum_{i=1}^n(z_i-a_i)u'_i
$$

$$
=u_k+ (1-h)u'_k-(1-h')u_k=u'_k-s_k
$$

By induction, one deduces from Lemma 5, applied to the integers $i$ and $j$ and to the mappings $w_{ij}$, that the sequence $(h, u''_1, . . . , u''_n)$ is adapted to $\boldsymbol{a}$ and is linked to $(h, u_1, . . . , u_n)$. Let $\omega ''$ be the differential form associated with $(h, u''_1, . . . , u''_n)$. Since $u''_i=u'_i-s_i$, we have

$$
\omega ''-\omega '=d(u'_1-s_1)\wedge dz_1\wedge  \cdots  \wedge d(u'_n-s_n)\wedge dz_n-
$$

$$
du'_1\wedge dz_1\wedge  \cdots  \wedge du'_n\wedge dz_n
$$

which is expressed as a linear combination, with coefficients 1 or $-1$, of differential forms of the form

$$
\xi_{I_1,I_2}=\bigwedge_{i\in I_1}ds_i\wedge \bigwedge_{i\in I_2}du'_i\wedge dz_1\wedge  \cdots  \wedge dz_n
$$

where $I_1$ (resp. $I_2$) is a nonempty subset (resp. a subset) of $\{1, . . . , n\}$. Each differential form $\xi_{I_1,I_2}$ can also be written in the form

$$
d(\widetilde{\psi}\wedge dz_1\wedge  \cdots  \wedge dz_n)
$$

where the support of the differential form $\widetilde{\psi}$ is contained in the support of $s_i$ for every $i\in I_1$. Since $I_1$ is nonempty, this support is contained in Supp($h$)$\cup$ Supp($h'$). Consequently, $(h, u''_1, . . . , u''_n)$ is linked to $(h', u'_1, . . . , u'_n)$, and the lemma results on writing

$$
\omega -\omega '= (\omega -\omega '') + (\omega ''-\omega ')
$$

### 4. Construction of the mappings $\Theta_{\boldsymbol{a}}$

Let $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$ and let U be an open neighbourhood of Sp$^n(\boldsymbol{a})$. Let $h$ be an indefinitely differentiable mapping, equal to 1 in a neighbourhood of Sp$^n(\boldsymbol{a})$ and such that the support of $h$ is compact and contained in U (Lemma 1 of I, p. 52). By Lemma 3 of I, p. 54, there exist indefinitely differentiable mappings $(u_1, . . . , u_n)$ of $\mathbf{C}^n$ into A such that the sequence $(h, u_1, . . . , u_n)$ is adapted to $\boldsymbol{a}$. Let $\omega$ be the differential form associated with it; it has compact support contained in U (Lemma 4 of I, p. 54). There exists an indefinitely differentiable function $\psi$ with compact support in U and with values in A such that

$$
\omega =\psi  dx_1\wedge dy_1\wedge  \cdots  \wedge dx_n\wedge dy_n
$$

where $x_j+iy_j$ are the coordinate functions on $\mathbf{C}^n$, identified with $\mathbf{R}^{2n}$. Let $\mu$ be the Lebesgue measure on $\mathbf{R}^{2n}$.

Let $f\in \mathscr{C}(U; A)$. The differential form $f \omega |U$ on U is continuous and has compact support. The vector measure associated with this differential form (VAR, R2, 10.4.3 and 10.4.4) is the vector measure $f \psi \cdot \mu$; it is a measure with base $\mu$ (INT, VI, §2, n$^o4$, Def. 4), its support is compact and contained in the support of $\omega$. This measure is majorized with respect to the norm of A (INT, VI, §2, n$^o4$, Prop. 8); we denote by $\|f \omega \|$ the positive measure on $\mathbf{C}^n$ associated with it (INT, VI, §2, n$^o3$, Def. 3).

By INT, VI, §2, n$^o4$, Prop. 8, b), we have

$$
\|f \omega \|=\|f \psi \cdot \mu\|=\|f \psi \| \cdot \mu=\|f\| \|\omega \|
$$

In particular, the integral of the differential form $f \omega$ over U satisfies

$$
\|\int_Uf \omega \|\leqslant \int_U\|f\| \|\omega \|
$$

(INT, VI, §2, n$^o3$, Prop. 5).

#### Lemma 7 {#ts-i-s4-lem-7 .statement tag=02A4}

For every function $f\in \mathscr{O}(U; A)$, the integral $\int_Uf \omega$ is an element of A depending only on $\boldsymbol{a}$ and on the germ of $f$ in a neighbourhood of Sp$^n(\boldsymbol{a})$. It satisfies the inequality

(4) $\|\int f \omega \|\leqslant (\int\|\omega \|)$ sup $\|f(z)\|$,

U U $z\in$Supp($h$)

and

$$
\int_U(af)\omega =a\int_Uf \omega
$$

for every $a\in A$.

We have seen above that the integral is defined for $f\in \mathscr{C}(U; A)$ and satisfies

$\|\int f \omega \|\leqslant \int\|f\| \|\omega \|\leqslant (\int\|\omega \|)$ sup $\|f(z)\|$.

U U U $z\in$Supp($h$)

Moreover, for every $a\in A$ and every $f\in \mathscr{C}(U; A)$, we have

$$
\int_U(af)\omega =a\int_Uf \omega
$$

(INT, VI, §2, n$^o2$, Prop. 2 applied to multiplication by $a$).

Let $(h', u'_1, . . . , u'_n)$ be a sequence adapted to $\boldsymbol{a}$ such that Supp($h'$)$\subset U$. Let $\omega '$ be the associated differential form. By Lemma 6 of I, p. 57, there exists a differential form $\psi$ on $\mathbf{C}^n$ of degree $n-1$, with coefficients in A and with support contained in Supp($h$)$\cup$ Supp($h'$)$\subset U$, such that

$$
\omega -\omega '=d(\psi \wedge dz_1\wedge  \cdots  \wedge dz_n)
$$

Let $f\in \mathscr{O}(U; A)$. Since the mapping $f$ is holomorphic, we have

$$
df=\sum^n\frac{\partial f}{\partial z_i}dz_i
$$

$i=1$

(VAR, R2, p. 24, 8.8.9) and hence

$$
f(\omega -\omega ') =f d(\psi \wedge dz_1\wedge  \cdots  \wedge dz_n) =d(f \psi \wedge dz_1\wedge  \cdots  \wedge dz_n)
$$

By Stokes' formula (VAR, R2, p. 48, 11.2.3), we then have

$$
\int_Uf(\omega -\omega ') = 0
$$

Thus the element $\int_Uf \omega$ does not depend on the choice of the sequence $(h, u_1, . . . , u_n)$.

To conclude, let us prove that $\int_Uf \omega$ depends only on the germ of $f$ in a neighbourhood of Sp$^n(\boldsymbol{a})$. Let U and $U'$ be open neighbourhoods of Sp$^n(\boldsymbol{a})$. Let $f\in \mathscr{O}(U; A)$ and $f'\in \mathscr{O}(U'; A)$ be such that $f$ and $f'$ coincide on an open neighbourhood $U''$ of Sp$^n(\boldsymbol{a})$. There exists a mapping $h$ of $\mathbf{C}^n$ into $\mathbf{C}$, indefinitely differentiable, equal to 1 in a neighbourhood of Sp$^n(\boldsymbol{a})$, and with compact support contained in $U''$ (Lemma 1 of I, p. 52), and there exists $(u_1, . . . , u_n)$ such that the sequence $(h, u_1, . . . , u_n)$ is adapted to $\boldsymbol{a}$ (Lemma 3 of I, p. 54). Let $\omega$ be the associated differential form. Since Supp($\omega$ )$\subset$ Supp($h$)$\subset U''$ (Lemma 4, b) of I, p. 54), we have

$$
\int_Uf \omega =\int_{U''}f \omega =\int_{U''}f'\omega =\int_{U'}f'\omega
$$

which completes the proof.

This lemma proves that there exists a unique a-linear mapping $\Theta_{\boldsymbol{a}}$ of $\mathscr{O}$(Sp$^n(\boldsymbol{a}); A$) into A such that

(5) $\Theta_{\boldsymbol{a}}(f) =n$! $_n\int\widetilde{f \omega}$

$$
(2i\pi )_U
$$

for every open set U and every representative $\widetilde{f}\in \mathscr{O}(U; A)$ of a germ $f\in \mathscr{O}$(Sp$^n(\boldsymbol{a}); A$). The linear mapping $\Theta_{\boldsymbol{a}}$ is continuous by inequality (4) and EVT, II, p. 29, Proposition 5.

### 5. Properties of the mappings $\Theta_{\boldsymbol{a}}$

We recall (VAR, R2, p. 46 and p. 47, 11.1.3, d)) that if K is a compact subset of $\mathbf{C}$, there exists a fundamental system of compact neighbourhoods V of K which are pieces of $\mathbf{C}$ (that is to say, for every $x\in V$, there exists a chart $(U, \varphi ,\mathbf{C})$ of $\mathbf{C}$ at $x$ such that $\varphi (U\cap K)$ is an open subset of a closed half-space of $\mathbf{C}$). We then denote by $\partial V$ the boundary of the piece V endowed with the orientation deduced from the orientation of $\mathbf{C}$ (VAR, R2, p. 47) and by $dz$ the differential of the injection $\partial V\rightarrow \mathbf{C}$.

#### Proposition 1 {#ts-i-s4-prop-1 .statement tag=02A5}

Let $a$ be an element of A, let U be an open neighbourhood of Sp($a$), and let $f\in \mathscr{O}(U; A)$. Let V be a compact neighbourhood of Sp($a$) contained in U and such that V is a piece of $\mathbf{C}$.

Then $z\mapsto f(z)(z-a)^{-1}$ is continuous on $\partial V$, the differential form $f(z)(z-a)^{-1}dz$ is integrable on $\partial V$, and one has

$$
\Theta_a(f) =\frac{1}{2i\pi}\int_{\partial V}f(z)(z-a)^{-1}dz
$$

Let $h$ be a mapping of $\mathbf{C}$ into $\mathbf{C}$, indefinitely differentiable, equal to 1 in a neighbourhood of Sp($a$) and with compact support contained in the interior of V (lemma 1 of I, p. 52). Let $u$ be a mapping of $\mathbf{C}$ into A such that $(h, u)$ is adapted to $a($cf. example 3 of I, p. 53). The associated differential form is $\omega =du\wedge dz$. We get $f \omega =f du\wedge dz=d(f u dz)$ since $f$ is holomorphic. Moreover, $u(z) = (z-a)^{-1}$ on the boundary of V. On the other hand, the differential form $f u dz$ is of class $C^1$ on U. Hence

$$
2i\pi \Theta_a(f) =\int_Vd(f u dz) =\int_{\partial V}f u dz=\int_{\partial V}f(z)(z-a)^{-1}dz
$$

by formula (5) and Stokes's formula for the piece V (VAR, R2, p. 47, 11.2.3).

#### Corollary {#ts-i-s4-n5-cor-1 .statement tag=02A6}

Let $a\in A$. One has $\Theta_a(1) = 1$.

Let $R> \varrho (a)$ be a real number. Let V be the closed disk with center 0 and radius R, so that Sp($a$)$\subset \mathring{V}$. It is a piece of $\mathbf{C}$ whose boundary $\partial V$ is the circle with center 0 and radius R. For $z\in \mathbf{C}-\mathring{V}$, one has the formula $(z-a)^{-1}=z^{-1}(1-z^{-1}a)^{-1}=\sum^{+\infty}_{j=1}z^{-j}a^{j-1}$. The series converges uniformly for $z\in \partial V$. Hence

$$
\Theta_a(1) =\frac{1}{2i\pi}\sum^{+\infty}_{j=1}a^{j-1}\int_{\partial V}z^{-j}dz= 1
$$

since

$$
\int_{\partial V}z^jdz= 0
$$

for every integer $j\not=-1$ and

$$
\int_{\partial V}z^{-1}dz= 2i\pi
$$

(VAR, R2, p. 44, 10.4.5, and p. 47, 11.2.1, example).

#### Lemma 8 {#ts-i-s4-lem-8 .statement tag=02A7}

Let U be an open set in $\mathbf{C}^n$. Let $\omega_1$ be a continuous differential form of degree $n$ in U with compact support and with values in A (resp. $\omega_2$ a continuous differential form of degree 2 in $\mathbf{C}$ with compact support and with values in $\mathbf{C}$). Let us denote by $\pi_1$ and $\pi_2$ the canonical projections of $U\times \mathbf{C}$ onto U and $\mathbf{C}$. The differential form $\pi_1^*\omega_1\wedge \pi_2^*\omega_2$ on $U\times \mathbf{C}$ is continuous with compact support and with values in A. We have

$$
\int_{U\times\mathbf{C}}\pi_1^*\omega_1\wedge \pi^*_2\omega_2=(\int_{\mathbf{C}}\omega_2)((\int_U\omega_1)
$$

Let $\mu_n$ be the Lebesgue measure on $\mathbf{C}^n$ and $\mu_1$ the Lebesgue measure on $\mathbf{C}$. There exist $\psi_1\in \mathscr{K}(U; A)$ and $\psi_2\in \mathscr{K}(\mathbf{C})$ such that the vector measure associated with $\omega_1$ is equal to $\psi_1\cdot \mu_n$, and the vector measure associated with $\omega_2$ is equal to $\psi_2\cdot \mu_1$. The vector measure associated with the differential form $\pi^*_1\omega_1\wedge \pi_2^*\omega_2$ is $(\psi_1\otimes \psi_2)\cdot \mu_n\otimes \mu_1$.

Let $\ell$ be a continuous linear form on A. After INT, VI, §2, n$^o2$, definition 2 and the definition of the product measure (INT, III, §4, n$^o1$, definition 1), it follows that

$$
\ell (\int_{U\times\mathbf{C}}\pi_1^*\omega_1\wedge \pi^*_2\omega_2)=\int_{U\times\mathbf{C}}\ell \circ (\psi_1\otimes \psi_2)\mu_n\otimes \mu_1
$$

$$
=\int\psi_2(z)\ell (\psi_1(x))d\mu_n(x)d\mu_1(z)
$$

$$
=(\int^{U\times\mathbf{C}}_{\mathbf{C}}\psi_2(z)d\mu_1(z))(\int_U\ell (\psi_1(x))d\mu_n(x))
$$

$$
=(\int_{\mathbf{C}}\psi_2\mu_1)\ell (\int_U\psi_1\mu_n)
$$

whence the result (INT VI, loc. cit.).

#### Lemma 9 {#ts-i-s4-lem-9 .statement tag=02A8}

Let $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$. Let $p\in \mathbf{N}$ and $\boldsymbol{a}'$ = $(a_{n+1}, . . . , a_{n+p})\in A^p$. Then we have $\Theta_{(\boldsymbol{a},\boldsymbol{a}')}\circ \pi_{n,n+p}^*= \Theta_{\boldsymbol{a}}$. In particular, we have $\Theta_{\boldsymbol{a}}(1) = 1$.

Since one has $\pi_{n,n+p}=\pi_{n,n+1}\circ \cdots \circ \pi_{n+p-1,n+p}$, it is enough to prove the first assertion when $p= 1$, which we henceforth suppose. We write simply $\pi =\pi_{n,n+1}$. It is then enough to prove that, for every open neighbourhood U of Sp$^n(\boldsymbol{a})$, and every function $f\in \mathscr{O}(U; A)$, one has $\Theta_{(\boldsymbol{a},a_{n+1})}(f\circ \pi ) = \Theta_{\boldsymbol{a}}(f)$. Let $g=f\circ \pi$. Let $h$ (resp. $h'$) be a mapping of $\mathbf{C}^n$ into $\mathbf{C}$ (resp. of $\mathbf{C}$ into $\mathbf{C}$), indefinitely differentiable, equal to 1 in a neighbourhood of Sp$^n(\boldsymbol{a})$ (resp. of Sp($\boldsymbol{a}'$)), with compact support contained in U (resp. in $\mathbf{C}$). There exist mappings $(u_1, . . . , u_n)$ of $\mathbf{C}^n$ into A, indefinitely differentiable, such that the sequence $(h, u_1, . . . , u_n)$ is adapted to $\boldsymbol{a}$ (lemma 3 of I, p. 54), and an indefinitely differentiable mapping $u_{n+1}$ of $\mathbf{C}$ into A such that the pair $(h', u_{n+1})$ is adapted to $a_{n+1}($loc. cit.)

For $\boldsymbol{z}\in \mathbf{C}^n$ and $z_{n+1}\in \mathbf{C}$, write $h''(\boldsymbol{z}, z_{n+1}) =h(\boldsymbol{z})h'(z_{n+1})$ and $u''_{n+1}(\boldsymbol{z}, z_{n+1}) =h(\boldsymbol{z})u_{n+1}(z_{n+1})$. The functions $h''$ and $u''_{n+1}$ are indefinitely differentiable in $\mathbf{C}^{n+1}$. The function $h''$ is equal to 1 in a neighbourhood of Sp$^{n+1}(\boldsymbol{a}, a_{n+1})$, and has compact support contained in $U\times \mathbf{C}$. For every $\boldsymbol{w}= (\boldsymbol{z}, z_{n+1})\in \mathbf{C}^{n+1}$, one has

$$
(z_1-a_1)(u_1\circ \pi )(\boldsymbol{w}) +\cdots + (z_n-a_n)(u_n\circ \pi )(\boldsymbol{w})
$$

$$
+ (z_{n+1}-a_{n+1})u''_{n+1}(\boldsymbol{w}) = 1-h(\boldsymbol{z}) +h(\boldsymbol{z})(1-h'(z_{n+1}))
$$

$$
= 1-h''(\boldsymbol{w})
$$

which proves that the sequence $(h'', u_1\circ \pi , . . . , u_n\circ \pi , u''_{n+1})$ is adapted to $(\boldsymbol{a}, a_{n+1})$. Let $\omega$ be the associated differential form.

The differential form $du_1\wedge dz_1\wedge  \cdots  \wedge du_n\wedge dz_n\wedge dh$ on $\mathbf{C}^n$ is of degree $2n+ 1$, hence is zero. Therefore

$$
\omega =d(u_1\circ \pi )\wedge dz_1\wedge  \cdots  \wedge d(u_n\circ \pi )\wedge dz_n\wedge du''_{n+1}\wedge dz_{n+1}
$$

$$
= (h\circ \pi )d(u_1\circ \pi )\wedge dz_1\wedge  \cdots  \wedge d(u_n\circ \pi )\wedge dz_n\wedge du_{n+1}\wedge dz_{n+1}
$$

Since $g=f\circ \pi$, formula (5) and lemma 8 imply

$\Theta_{\boldsymbol{a},\boldsymbol{a}'}(g) =$ (2$(ni\pi +$ 1)!$)^{n+1}\int_{U\times\mathbf{C}}g\omega =$ (2$(ni\pi +$ 1)!$)^{n+1}(\int_{\mathbf{C}}du_{n+1}\wedge dz_{n+1})$

$$
\times (\int_Uf h du_1\wedge dz_1\wedge  \cdots  \wedge du_n\wedge dz_n)
$$

On the one hand, one has

$$
\int_{\mathbf{C}}du_{n+1}\wedge dz_{n+1}= 2i\pi \Theta^{\mathbf{C}}_{a_{n+1}}(1) = 2i\pi \cdot 1
$$

by corollary 5. On the other hand, part c) of lemma 4 of I, p. 54 and the fact that the integral of a closed form is zero (VAR, R2, p. 48, 11.2.4) imply

$$
(n+ 1)\int_Uf hdu_1\wedge dz_1\wedge  \cdots  \wedge du_n\wedge dz_n=
$$

$\int_Uf du_1\wedge dz_1\wedge  \cdots  \wedge du_n\wedge dz_n=(2i\pi n$!$)^n\Theta_{\boldsymbol{a}}(f)$.

Thus one obtains

$\Theta_{\boldsymbol{a},\boldsymbol{a}'}(g) =$ (2$(ni\pi +$ 1)!$)^{n+1}\times ((2ni\pi +$ 1)!$)^n\Theta_{\boldsymbol{a}}(f)\times 2i\pi = \Theta_{\boldsymbol{a}}(f)$.

Finally, the formula $\Theta_{\boldsymbol{a}}(1) = 1$ results from the foregoing and from the corollary of Prop. 1.

#### Lemma 10 {#ts-i-s4-lem-10 .statement tag=02A9}

Let $\boldsymbol{a}\in A^n$. Let $g$ be a polynomial function on $\mathbf{C}^n$ with coefficients in A and let $f\in \mathscr{O}$(Sp$^n(\boldsymbol{a}); A$). Then $\Theta_{\boldsymbol{a}}(gf) =g(\boldsymbol{a})\Theta_{\boldsymbol{a}}(f)$. In particular, $\Theta_{\boldsymbol{a}}(g) =g(\boldsymbol{a})$.

By Lemma 9, it is enough to prove the first assertion.

Let $z_1, . . . , z_n$ denote the coordinate functions on $\mathbf{C}^n$. Since the mapping $\Theta_{\boldsymbol{a}}$ is A-linear, it is enough to prove the assertion of the lemma when $g=z_1^{e_1}\cdots z^{e_n}_n$, where $(e_1, . . . , e_n)\in \mathbf{N}^n$. Arguing by induction on $e_1+\cdots +e_n$, we are reduced to the case where there exists an integer $i$ such that $1\leqslant i\leqslant n$ and $g=z_i$.

Let U be an open neighbourhood of Sp$^n(\boldsymbol{a})$. Let $(h, u_1, . . . , u_n)$ be a sequence adapted to $\boldsymbol{a}$ such that the support of $h$ is contained in U (Lemma 1 of I, p. 52 and Lemma 3 of I, p. 54), and let $\omega$ be the associated differential form. By Lemma 4, a) of I, p. 54, there exists a differential form $\beta$ such that

$$
(z_i-a_i)\omega =d(h\beta \wedge dz_1\wedge  \cdots  \wedge dz_n)
$$

Consequently, for every function $f\in \mathscr{O}(U; A)$, one has

$$
(z_i-a_i)f \omega =f d(h\beta \wedge dz_1\wedge  \cdots  \wedge dz_n) =d(f h\beta \wedge dz_1\wedge  \cdots  \wedge dz_n)
$$

since $f$ is holomorphic, so that $df\wedge dz_1\wedge  \cdots  \wedge dz_n= 0$. Applying Stokes's formula (VAR, R2, p. 48, 11.2.4), we obtain $\int_U(z_i-a_i)f \omega = 0$, whence

$\Theta_{\boldsymbol{a}}(z_if) =(2i\pi n$!$)^n\int_Uz_if \omega =(2ni\pi$!$)^n\int_Ua_if \omega =a_i\Theta_{\boldsymbol{a}}(f)$

by formula (5). The result follows.

#### Proposition 2 {#ts-i-s4-prop-2 .statement tag=02AA}

Let $\varrho_1, . . . , \varrho_n$ be real numbers $>0$ and let $U\subset \mathbf{C}^n$ be the polydisc product of the open discs with center 0 and radius $\varrho_i$. Let

$$
\sum c(k_1, . . . , k_n)X^{k_1}_1\cdots X^{k_n}_n\in A[[X_1, . . . ,X_n]]
$$

$(k_1,...,k_n)\in \mathbf{N}^n$

be a formal series with coefficients in A. Suppose that this series converges in U, and let $f$ denote the holomorphic function in U of which it is the sum.

Let $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$ be such that $\varrho (a_i)< \varrho_i$ for $1\leqslant i\leqslant n$. Then Sp$^n(\boldsymbol{a})\subset U$, the family $(c(k_1, . . . , k_n)a^{k_1}_1\cdots a^{k_n}_n)$ of elements of A is absolutely summable, and

$$
\Theta_{\boldsymbol{a}}(f) =\sum c(k_1, . . . , k_n)a^{k_1}_1\cdots a^{k_n}_n
$$

$(k_1,...,k_n)\in \mathbf{N}^n$

For every character $\chi$ of A and every integer $i$ such that $1\leqslant i\leqslant n$, one has $|\chi (a_i)|\leqslant \varrho (a_i)< \varrho_i$, hence Sp$^n(\boldsymbol{a})\subset U$ by definition of the simultaneous spectrum. Let $z_1, . . . , z_n$ be the restrictions to U of the coordinate functions on $\mathbf{C}^n$. Then the family $(c(k_1, . . . , k_n)z_1^{k_1}\cdots z^{k_n}_n)$ is summable in $\mathscr{O}(U; A)$ and has sum $f$. In view of lemma 10 and the continuity of the mapping $\Theta^U_{\boldsymbol{a}}$, the family $(c(k_1, . . . , k_n)a^{k_1}_1. . . a^{k_n}_n)$ is therefore summable in A and has sum $\Theta_{\boldsymbol{a}}(f)$. For $1\leqslant i\leqslant n$, let $\lambda_i$ be a real number such that $\varrho (a_i)< \lambda_i< \varrho_i$. There exists $M_i<+\infty$ such that $\|a^k_i\|\leqslant M_i\lambda^k_i$ for every integer $k\geqslant 0$. One then has

$$
\sum\|c(k_1, . . . , k_n)\| \|a^{k_1}_1\cdots a^{k_n}_n\|\leqslant
$$

$(k_1,...,k_n)\in \mathbf{N}^n$

$M_1\cdots M_n\sum\|c(k_1, . . . , k_n)\|\lambda^{k_1}_1\cdots \lambda^{k_n}_n$

$(k_1,...,k_n)\in \mathbf{N}^n$ which is finite by hypothesis, hence the family $(c(k_1, . . . , k_n)a^{k_1}_1\cdots a^{k_n}_n)$ is absolutely summable.

#### Corollary {#ts-i-s4-n5-cor-2 .statement tag=02AB}

Assume that A is nonzero. Let $\boldsymbol{a}\in \mathbf{C}^n\subset A^n$. One has Sp$^n_A(\boldsymbol{a}) =\{\boldsymbol{a}\}$. For every germ $f\in \mathscr{O}(\{\boldsymbol{a}\}; A)$, one has $\Theta_{\boldsymbol{a}}(f) =f(\boldsymbol{a})$.

#### Proposition 3 {#ts-i-s4-prop-3 .statement tag=02AC}

Let B be a commutative unital Banach algebra and $\varphi$ a continuous unital morphism of A into B. Let $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$. Put $\boldsymbol{b}= (\varphi (a_1), . . . , \varphi (a_n))$, so that Sp$^n_B(\boldsymbol{b})\subset$ Sp$^n_A(\boldsymbol{a})$. For every $f\in \mathscr{O}$(Sp$^n_A(\boldsymbol{a}); A$), one has

$$
\varphi (\Theta_{\boldsymbol{a}}(f)) = \Theta_{\boldsymbol{b}}(\varphi_*(f))
$$

where $\varphi_*(f)$ denotes the germ of $\varphi \circ f$ in a neighbourhood of Sp$^n_B(\boldsymbol{b})$.

It is enough to prove that for every open neighbourhood U of Sp$^n_A(\boldsymbol{a})$ and every $f\in \mathscr{O}(U; A)$, one has $\varphi (\Theta_{\boldsymbol{a}}(f)) = \Theta_{\boldsymbol{b}}(\varphi \circ f)$, where $\varphi \circ f\in \mathscr{O}(U; B)$. Let $(h, u_1, . . . , u_n)$ be a sequence adapted to $\boldsymbol{a}$, where the support of $h$ is contained in U (lemma 1 of I, p. 52 and lemma 3 of I, p. 54). Let $\omega$ denote the associated differential form. For every $\boldsymbol{z}\in \mathbf{C}^n$, one has

$$
\sum_{j=1}^n(z_j-b_j)\varphi (u_i(\boldsymbol{z})) =\varphi (\sum_{j=1}^n(z_j-a_j)u_j(\boldsymbol{z}))= 1-h(\boldsymbol{z})
$$

so that the sequence $(h, \varphi \circ u_1, . . . , \varphi \circ u_n)$ is adapted to $\boldsymbol{b}$. Let $\omega '$ denote the associated differential form. Let $\mu$ denote Lebesgue measure on $\mathbf{C}^n$. Let $f\in \mathscr{O}(U; A)$. Let us write $\psi \cdot \mu$ for the vector measure associated with the differential form $f \omega$. The vector measure associated with the differential form

$$
(\varphi \circ f)\omega '= (\varphi \circ f)d(\varphi \circ u_1)\wedge dz_1\wedge  \cdots  \wedge d(\varphi \circ u_n)\wedge dz_n
$$

is equal to $(\varphi \circ \psi )\cdot \mu$. Therefore, by formula (5), and INT, VI, §2, n$^o2$, prop. 2, one has

$\Theta_{\boldsymbol{b}}(\varphi \circ f) =(2i\pi n$!$)^n\int_U(\varphi \circ f)\mu=(2ni\pi$!$)^n\varphi (\int_U\psi  \mu)=\varphi (\Theta_{\boldsymbol{a}}(f))$,

as was required.

#### Corollary 1 {#ts-i-s4-prop-3-cor-1 .statement tag=02AD}

Let $\chi \in \mathsf{X}(A)$ and $\boldsymbol{a}\in A^n$. For every germ $f\in \mathscr{O}$(Sp$^n(\boldsymbol{a})$), one has $\chi (\Theta_{\boldsymbol{a}}(f)) =f(\chi (a_1), . . . , \chi (a_n))$.

This is a consequence of Proposition 3, applied to the continuous unital morphism $\chi : A\rightarrow \mathbf{C}$ (Theorem 1 of I, p. 29), and of the corollary to Proposition 2, applied to the Banach algebra $\mathbf{C}$.

#### Remark {#ts-i-s4-n5-rem-1 .statement tag=02AE}

Suppose that the algebra A is without radical. Let $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$. By Proposition 8 of I, p. 38, the mapping $\Theta^U_{\boldsymbol{a}}$ is the unique mapping $\varphi$ from $\mathscr{O}(U)$ into A such that $\chi (\varphi (f)) =f(\chi (a_1), . . . , \chi (a_n))$ for every $\chi \in \mathsf{X}(A)$ and every function $f\in \mathscr{O}(U)$.

#### Corollary 2 {#ts-i-s4-prop-3-cor-2 .statement tag=02AF}

Let $p$ be an integer $\geqslant$ 1. For every family $(f_1, . . . , f_p)$ of elements of $\mathscr{O}$(Sp$^n(\boldsymbol{a})$), one has

Sp$^p((\Theta_{\boldsymbol{a}}(f_1), . . . ,\Theta_{\boldsymbol{a}}(f_p))) = (f_1, . . . , f_p$)(Sp$^n(\boldsymbol{a})$).

In particular, for every $f\in \mathscr{O}$(Sp$^n(\boldsymbol{a})$), one has Sp(Θ$_{\boldsymbol{a}}(f)$) $=f$(Sp$^n(\boldsymbol{a})$).

This follows from Corollary 1 and the definition of the joint spectrum.

#### Example {#ts-i-s4-n5-exa-1 .statement tag=02AG}

Let A be the complex Banach algebra of functions on the unit circle with absolutely convergent Fourier series (I, p. 19, Example 8). Let $\varphi \in$ A. Let $f$ be a germ of a holomorphic function in a neighbourhood of the set of values of $\varphi$. Then $\psi = \Theta_{\varphi}(f)$ is an absolutely convergent Fourier series which for every $u\in \mathbf{U}$ satisfies $\psi (u) =f(\varphi (u))$ (Corollary 1, applied to the characters $\varphi \mapsto \varphi (u)$). In other words, the function $f\circ \varphi$ on the unit circle also has an absolutely convergent Fourier series (“theorem of P. Lévy”). This result generalises Wiener's theorem (I, p. 38, Example 4), which concerns the case of the function $f(z) = 1/z$ on $\mathbf{C}-\{0\}$ when $\varphi$ does not vanish.

### 6. Approximation Theorems

In this No., A is a commutative complex unital Banach algebra.

#### Proposition 4 {#ts-i-s4-prop-4 .statement tag=02AH}

Let L be a polynomially convex compact subset of $\mathbf{C}^n$ and let U be an open neighbourhood of L. For every function $f\in \mathscr{O}(U; A)$, there exists a sequence of polynomial functions on $\mathbf{C}^n$ with coefficients in A which converges to $f|L$ in $\mathscr{C}(L; A)$.

One may suppose that L is not empty and that A is nonzero. Let P (resp. $P_0$) be the set of restrictions to L of polynomial functions on $\mathbf{C}^n$ with coefficients in A (resp. with coefficients in $\mathbf{C}$). Let B (resp. $B_0$) be the Banach algebra closure of P (resp. of $P_0$) in $\mathscr{C}(L; A)$. Let $\iota$ denote the injection of A onto the normed subalgebra of B consisting of the constant functions.

Let $z_1, . . . , z_n$ be the restrictions to L of the coordinate functions on $\mathbf{C}^n$; they are elements of $B_0$, and, setting $\boldsymbol{z}= (z_1, . . . , z_n)$, one has Sp$^n_{B_0}(\boldsymbol{z}) = L$ by Proposition 15 of I, p. 47.

Let $f\in \mathscr{O}(U; A)$. By composition with $\iota$, the function $f$ defines an element $f_B=\iota \circ f$ of $\mathscr{O}(U; B)$. Since Sp$^n_B(\boldsymbol{z})\subset$ Sp$^n_{B_0}(\boldsymbol{z})\subset U$, one can form the element $b= \Theta_{\boldsymbol{z}}(f_B)$ of B. Let $\boldsymbol{w}= (w_1, . . . , w_n)\in L$, and let $\varphi$ be the continuous unital morphism $g\mapsto g(\boldsymbol{w})$ of B into A. One has $\varphi \circ \iota =$ Id$_A$, so that $\varphi \circ f_B=f$. Since $\varphi (z_i) =w_i$, prop. 3 of I, p. 66 implies $\varphi (\Theta_{\boldsymbol{z}}(f_B)) = \Theta_{\boldsymbol{w}}(\varphi \circ f_B)$. Hence

$$
b(\boldsymbol{w}) =\varphi (b) =\varphi (\Theta_{\boldsymbol{z}}(f_B)) = \Theta_{\boldsymbol{w}}(\varphi \circ f_B) = \Theta_{\boldsymbol{w}}(f) =f(\boldsymbol{w})
$$

by the corollary of prop. 2 of I, p. 65. Thus one has $f|L =b$; in particular, $f|L$ belongs to B. This proves the proposition.

#### Theorem 2 (Oka–Weil) {#ts-i-s4-thm-2 .statement tag=02AI}

Let K be a polynomially convex compact subset of $\mathbf{C}^n$ and P the set of germs in a neighbourhood of K of polynomial functions on $\mathbf{C}^n$ with coefficients in A. Then P is dense in $\mathscr{O}(K; A)$. More precisely, every element of $\mathscr{O}(K; A)$ is the limit of a sequence of elements of P.

Consider an element of $\mathscr{O}(K; A)$, germ of a function $f\in$ $\mathscr{O}(U; A)$, where U is an open neighbourhood of K. By lemma 7 of I, p. 48, there exists a compact neighbourhood L of K contained in U which is polynomially convex. Let V be the interior of L; it is a neighbourhood of K.

By the preceding proposition, there exists a sequence $(P_k)$ of polynomial functions on $\mathbf{C}^n$ with coefficients in A which converges to $f|L$ in $\mathscr{C}(L; A)$. In particular, the sequence $(P_k)$ converges to $f|V$ in $\mathscr{O}(V; A)$.

By definition of the topology on $\mathscr{O}(K; A)$ (cf. EVT, II, p. 29, prop. 5), the canonical mapping of $\mathscr{O}(V; A)$ into $\mathscr{O}(K; A)$ is continuous. Consequently, the sequence of germs in a neighbourhood of K of the functions $P_k$ converges to the germ of $f$ in a neighbourhood of K in the space $\mathscr{O}(K; A)$, which was to be proved.

#### Corollary 1 {#ts-i-s4-thm-2-cor-1 .statement tag=02AJ}

Let U be an open neighbourhood of K. Let $u_1$ and $u_2$ be continuous mappings of $\mathscr{O}(U; A)$ into a topological space X factoring through $\mathscr{O}(K; A)$. Then $u_1=u_2$ if and only if $u_1$ and $u_2$ coincide on the set of restrictions to K of polynomial functions on $\mathbf{C}^n$ with coefficients in A.

#### Corollary 2 {#ts-i-s4-thm-2-cor-2 .statement tag=02AK}

Let E be a Banach space. Let K be a polynomially convex compact subset of $\mathbf{C}^n$. Let P be the set of germs in a neighbourhood of K of polynomial functions on $\mathbf{C}^n$ with values in E. Then every element of $\mathscr{O}(K; E)$ is the limit of a sequence of elements of P.

Let E be provided with the multiplication defined by $ab= 0$ for all $a$ and $b$ in E (example 1 of I, p. 17). It is a commutative Banach algebra. Let A be the commutative unital Banach algebra obtained from E by adjunction of a unit element. Since the canonical mapping $\mathscr{O}(K; A)\rightarrow \mathscr{O}(K; E)$ is continuous, the assertion results from the Oka-Weil theorem applied to the algebra A.

For $n= 1$ and $A =\mathbf{C}$, one also has the following result, which will be made more precise by corollary 2 of I, p. 150.

#### Theorem 3 (Runge) {#ts-i-s4-thm-3 .statement tag=02AL}

Let K be a compact subset of $\mathbf{C}$, and Q the set of germs of rational functions holomorphic in a neighbourhood of K. Then Q is dense in $\mathscr{O}(K)$.

By the definition of the topology on $\mathscr{O}(K)$, it is enough to prove that for every open neighbourhood U of K, and every compact subset L of U, every function $f\in \mathscr{O}(U)$ is the limit of rational functions continuous on L. One may suppose that L is a compact neighbourhood of K.

Let $Q'$ be the set of restrictions to L of rational functions on $\mathbf{C}$ which are continuous on L, and let C be the closure of $Q'$ in $\mathscr{C}(L)$. It is an algebra with no radical.

Let $z\in C$ be the identical mapping of L. Then C is the full closed subalgebra of $\mathscr{C}(L)$ generated by $z$ (lemma 2 of I, p. 6). Hence Sp$_C(z) =$ Sp$_{\mathscr{C}(L)}(z) = L$. One can therefore form the element $c= \Theta_z(f)$ of C. Since C has no radical, application of cor. 1 of I, p. 66 to the characters $g\mapsto g(w)$ of C, for every $w\in L$, shows that $c$ coincides with the restriction of $f$ to L. By definition of C, this proves that $f|L$ is the uniform limit on L of elements of $Q'$, and this completes the proof of the theorem.

### 7. Existence and uniqueness of the holomorphic functional calculus

We assume that A is a commutative complex unital Banach algebra.

#### Definition 2 {#ts-i-s4-def-2 .statement tag=02AM}

Let $n\geqslant 1$ be an integer and let $\boldsymbol{a}\in A^n$. Let U be an open neighbourhood of Sp$^n(\boldsymbol{a})$. One says that a family $\boldsymbol{a}'$ is an envelope of $(\boldsymbol{a},U)$ if $\boldsymbol{a}'\in \mathbf{C}^{n+p}$ extends $\boldsymbol{a}$ and if $U\times \mathbf{C}^p$ contains the polynomially convex envelope of Sp$^{n+p}(\boldsymbol{a}')$.

#### Lemma 11 {#ts-i-s4-lem-11 .statement tag=02AN}

Let $n\geqslant 1$ be an integer. Let $\boldsymbol{a}\in A^n$. For every open neighbourhood U of Sp$^n(\boldsymbol{a})$, there exists an envelope of $(\boldsymbol{a},U)$.

Let $(a_{\lambda})_{\lambda\in\Lambda}$ be a family of elements of A extending the family $\boldsymbol{a}$ and generating the unital Banach algebra A topologically. Let $\pi$ be the canonical projection of $\mathbf{C}^{\Lambda}$ onto $\mathbf{C}^n$ and let $U'=\pi^{-1}(U)$. Then $U'$ is a neighbourhood of Sp$^{\Lambda}((a_{\lambda}))$, and Sp$^{\Lambda}((a_{\lambda}))$ is polynomially convex (I, p. 44, lemma 4). By lemma 6 of I, p. 47, there exists a finite subset $\Lambda_0$ of Λ containing $\{1,2, . . . , n\}$ such that pr$_{\Lambda_0}(U')$ contains the polynomially convex envelope S of pr$_{\Lambda_0}$(Sp$^{\Lambda}((a_{\lambda})_{\lambda\in\Lambda})$) $=$ Sp$^{\Lambda_0}((a_{\lambda})_{\lambda\in\Lambda_0})$. Let $p\geqslant 0$ be the integer such that $\Lambda_0$ has cardinal $n+p$, and let $j$ be a bijection of $\{1, . . . , n+p\}$ onto $\Lambda_0$ which coincides with the identical mapping on $\{1, . . . , n\}$. Since the projection of S is contained in U, the family $(a_{j(k)})_{1\leqslant k\leqslant n+p}$ is an envelope of $(\boldsymbol{a},U)$.

#### Proposition 5 {#ts-i-s4-prop-5 .statement tag=02AO}

The data of the mappings $\Theta_{\boldsymbol{a}}$, for $n\geqslant 1$ and $\boldsymbol{a}\in A^n$, constitute a holomorphic functional calculus on A, that is to say that conditions (CF1), (CF2) and (CF3) of I, p. 51 are satisfied.

Let $n\geqslant 1$ be an integer and $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$. The mapping $\Theta_{\boldsymbol{a}}$ satisfies $\Theta_{\boldsymbol{a}}(z_i) =a_i$ for every $i$ such that $1\leqslant i\leqslant n$ by lemma 10 of I, p. 64, which proves property (CF2). Lemma 9 of I, p. 63 implies property (CF3) of the mappings $\Theta_{\boldsymbol{a}}$.

The mapping $\Theta_{\boldsymbol{a}}$ is A-linear and continuous (I, p. 61, n$^o5$). It satisfies $\Theta_{\boldsymbol{a}}(1) = 1$ (lemma 9 of I, p. 63). To verify condition (CF1), it remains to establish that $\Theta_{\boldsymbol{a}}$ is an algebra morphism. For this, we shall prove that $\Theta^U_{\boldsymbol{a}}$ is an algebra morphism for every open neighbourhood U of Sp$^n(\boldsymbol{a})$.

Suppose first that U contains the polynomially convex hull K of Sp$^n(\boldsymbol{a})$. Let $f_1$ and $f_2$ be elements of $\mathscr{O}(U; A)$. There exists a sequence $(f_{1,k})$ (resp. $(f_{2,k})$) of polynomial functions converging to $f_1$ (resp. to $f_2$) in $\mathscr{O}(K; A)$ (theorem 2 of I, p. 68), hence in $\mathscr{O}$(Sp$^n(\boldsymbol{a}); A$). For every integer $k$, one has

$$
\Theta^U_{\boldsymbol{a}}(f_{1,k})\Theta^U_{\boldsymbol{a}}(f_{2,k}) = \Theta^U_{\boldsymbol{a}}(f_{1,k}f_{2,k})
$$

by lemma 10 of I, p. 64, whence $\Theta^U_{\boldsymbol{a}}(f_1)\Theta^U_{\boldsymbol{a}}(f_2) = \Theta^U_{\boldsymbol{a}}(f_1f_2)$ on passing to the limit.

Consider the general case. Let $\boldsymbol{a}'\in \mathbf{C}^{n+p}$ be an envelopment of $(\boldsymbol{a},U)$ (lemma 11) and $\pi : U\times \mathbf{C}^p\rightarrow U$ the canonical projection. Since $U\times \mathbf{C}^p$ contains the polynomially convex hull of Sp$^{n+p}(\boldsymbol{a}')$, one has

$$
\Theta^{U\times\mathbf{C}^p}_{\boldsymbol{a}'}(f_1\circ \pi )\Theta^{U\times\mathbf{C}^p}_{\boldsymbol{a}'}(f_2\circ \pi ) = \Theta^{U\times\mathbf{C}^p}_{\boldsymbol{a}'}(f_1f_2\circ \pi )
$$

for $f_1$ and $f_2$ in $\mathscr{O}(U; A)$ by the first case. Since, for every function $f\in \mathscr{O}(U; A)$, one has $\Theta^{U\times\mathbf{C}^p}_{\boldsymbol{a}'}(f\circ \pi ) = \Theta^U_{\boldsymbol{a}}(f)$ (condition (CF3) proved above), the conclusion follows, and hence condition (CF1).

We can now prove theorem 1 of I, p. 51. Prop. 5 shows that the family of mappings $(\Theta_{\boldsymbol{a}})_{\boldsymbol{a}}$ is a holomorphic functional calculus on A. It therefore only remains to establish the uniqueness of the holomorphic functional calculus on A.

Let $(\Psi_{\boldsymbol{a}})_{\boldsymbol{a}}$ be a family of mappings defined for every integer $n\geqslant 1$ and every $\boldsymbol{a}\in A^n$ and satisfying conditions (CF1), (CF2), (CF3) of the holomorphic functional calculus on A (I, p. 51). It suffices to prove that for every integer $n\geqslant 1$, for every $\boldsymbol{a}\in A^n$ and for every open neighbourhood U of $\boldsymbol{a}$, one has $\Theta^U_{\boldsymbol{a}}= \Psi^U_{\boldsymbol{a}}$.

Let $n\geqslant 1$ and $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$. Let U be an open neighbourhood of Sp$^n(\boldsymbol{a})$. Suppose first that U contains the polynomially convex hull K of Sp$^n(\boldsymbol{a})$. The morphisms $\Theta^U_{\boldsymbol{a}}$ and $\Psi^U_{\boldsymbol{a}}$ coincide on polynomial functions by properties (CF1) and (CF2). By the corollary to theorem 2 of I, p. 68 and the continuity property (CF1), these morphisms are therefore equal.

Let us prove the general case. Let $\boldsymbol{a}'\in \mathbf{C}^{n+p}$ be an envelopment of $(\boldsymbol{a},U)$ and $\pi : U\times \mathbf{C}^p\rightarrow U$ the canonical projection. One has

$$
\Theta^U_{\boldsymbol{a}}= \Theta^{U\times\mathbf{C}^p}_{\boldsymbol{a}'}\circ \pi^*= \Psi^{U\times\mathbf{C}^p}_{\boldsymbol{a}'}\circ \pi^*= \Psi^U_{\boldsymbol{a}}
$$

by property (CF3) and the preceding case. This concludes the proof of theorem 1 of I, p. 51.

Let us remark that theorem 2 of I, p. 68 also entails the following uniqueness result:

#### Proposition 6 {#ts-i-s4-prop-6 .statement tag=02AP}

Let $\boldsymbol{a}\in A^n$. Suppose that Sp$^n(\boldsymbol{a})$ is polynomially convex. Let $z_1, . . . , z_n$ be the germs in a neighbourhood of Sp$^n(\boldsymbol{a})$ of the coordinate functions on $\mathbf{C}^n$. Then the mapping $\Theta_{\boldsymbol{a}}$ is the unique continuous unital algebra morphism $\varphi$ from $\mathscr{O}$(Sp$^n(\boldsymbol{a}); A$) into A such that $\varphi (z_1) =a_1, . . . , \varphi (z_n) =a_n$.

Lemma 10 of I, p. 64 and the corollary to proposition 2 of I, p. 65 justify the following notations for the holomorphic functional calculus. Let $n\geqslant 1$ and $\boldsymbol{a}\in A^n$. For every germ $f\in \mathscr{O}(K; A)$ (resp. for every holomorphic function $f\in \mathscr{O}(U; A)$ on an open neighbourhood U of Sp$^n(\boldsymbol{a})$), one sets

$$
f(\boldsymbol{a}) = \Theta_{\boldsymbol{a}}(f) \tag{6}
$$

This notation is consistent with the notation introduced in A, IV, p. 4, n$^o3$, if $f$ is a polynomial, by properties (CF1) and (CF2).

Properties (CF2) and (CF3) of I, p. 51 may then be written

$$
z_i(\boldsymbol{a}) =a_i,1\leqslant i\leqslant n,(f\circ \pi_{m,n})(\boldsymbol{a}) =f(\pi_{m,n}(\boldsymbol{a}))
$$

### 8. Substitution in the functional calculus

With the notations introduced above, the statements of cor. 1 of I, p. 66 and of cor. 2 of I, p. 67 become respectively

$\chi (g(\boldsymbol{a})) =g(\chi (a_1), . . . , \chi (a_n))$, Sp($g(\boldsymbol{a})$) $=g$(Sp$^n(\boldsymbol{a})$)

for $f\in \mathscr{O}$(Sp$^n(\boldsymbol{a}); A$)$,\chi \in \mathsf{X}(A)$ and $g\in \mathscr{O}$(Sp$^n(\boldsymbol{a})$).

We shall now prove a more general substitution property.

#### Theorem 4 {#ts-i-s4-thm-4 .statement tag=02AQ}

Let A be a commutative complex unital Banach algebra, let $n\geqslant 1$ be an integer, and let $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$. Let $\boldsymbol{f}=$ $(f_1, . . . , f_p)$, where $f_1, . . . , f_p$ are elements of $\mathscr{O}$(Sp$^n(\boldsymbol{a})$). The image of Sp$^n(\boldsymbol{a})$ under the mapping $\boldsymbol{z}\mapsto \boldsymbol{f}(\boldsymbol{z}) = (f_1(\boldsymbol{z}), . . . , f_p(\boldsymbol{z}))$ is equal to Sp$^p(\boldsymbol{f}(\boldsymbol{a}))$.

For every $g\in \mathscr{O}$(Sp$^p(\boldsymbol{f}(\boldsymbol{a})); A$), the composite germ $g\circ \boldsymbol{f}$ is an element of $\mathscr{O}$(Sp$^n(\boldsymbol{a}); A$) and one has $g(\boldsymbol{f}(\boldsymbol{a})) = (g\circ \boldsymbol{f})(\boldsymbol{a})$.

The first assertion concerning the image of Sp$^n(\boldsymbol{a})$ follows from cor. 2 of I, p. 67. To prove the second, we shall use the following lemma.

#### Lemma 12 {#ts-i-s4-lem-12 .statement tag=02AR}

Let K be the polynomially convex envelope of Sp$^p(\boldsymbol{f}(\boldsymbol{a}))$. One has $g(\boldsymbol{f}(\boldsymbol{a})) = (g\circ \boldsymbol{f})(\boldsymbol{a})$ for every germ $g\in \mathscr{O}(K; A)$.

Let Ψ be the mapping from $\mathscr{O}(K; A)$ into A such that $\Psi (g) = (g\circ \boldsymbol{f})(\boldsymbol{a})$. It is a continuous unital morphism such that $\Psi (z_j) =f_j(\boldsymbol{a})$, where $z_j$ is the germ of the $j$-th coordinate function on $\mathbf{C}^p$. When $g$ is the germ of a polynomial function, one therefore has $\Psi (g) =g(\boldsymbol{f}(\boldsymbol{a}))$. By th. 2 of I, p. 68, this formula remains valid for every $g\in \mathscr{O}(K; A)$.

Let us now prove the theorem. Let V be an open neighbourhood of Sp$^p(\boldsymbol{f}(\boldsymbol{a}))$ and $\widetilde{g}\in \mathscr{O}(V; A)$ a holomorphic function whose germ in a neighbourhood of Sp$^p(\boldsymbol{f}(\boldsymbol{a}))$ is equal to $g$. Let $\boldsymbol{b}\in \mathbf{C}^{p+q}$ be an envelopment of $(\boldsymbol{f}(\boldsymbol{a}),V)$ (Lemma 11 of I, p. 70) and $\pi : V\times \mathbf{C}^q\rightarrow V$ the canonical projection.

Let $\widetilde{f}_1, . . . ,\widetilde{f}_p$ be holomorphic functions whose germs are $f_1, . . . , f_p$ and let U be an open neighbourhood of Sp$^n(\boldsymbol{a})$ such that $(\widetilde{f}_1, . . . ,\widetilde{f}_p)(U)\subset V$. Let $\pi '$ be the canonical projection of $U\times \mathbf{C}^q$ onto U. Let us denote by $z_{n+1}, . . . , z_{n+q}$ the last $q$ coordinate functions on $\mathbf{C}^{n+q}$. Put $h=\widetilde{g}\circ (\widetilde{f}_1, . . . ,\widetilde{f}_p)$ and

$$
\boldsymbol{c}= (a_1, . . . , a_n, b_{p+1}, . . . , b_{p+q})\in A^{n+q}
$$

The mapping $\widetilde{g}\circ \pi$ is holomorphic in the open neighbourhood $V\times \mathbf{C}^q$ of the polynomially convex envelope L of Sp$^{p+q}(\boldsymbol{b})$. By Lemma 12, applied to $\boldsymbol{c}$, to the germs in a neighbourhood of L of the functions

$$
(\widetilde{f}_1\circ \pi ', . . . ,\widetilde{f}_p\circ \pi ', z_{n+1}, . . . , z_{n+q})
$$

and to the germ of $\widetilde{g}\circ \pi$, we have

$$
(g\circ \pi )((f_1\circ \pi ')(\boldsymbol{c}), . . . ,(f_p\circ \pi ')(\boldsymbol{c}), z_{n+1}(\boldsymbol{c}), . . . , z_{n+q}(\boldsymbol{c}))= (h\circ \pi ')(\boldsymbol{c})
$$

Since $\pi '(\boldsymbol{c}) =\boldsymbol{a}$, we have $(h\circ \pi ')(\boldsymbol{c}) =h(\boldsymbol{a})$ and $(f_i\circ \pi ')(\boldsymbol{c}) =f_i(\boldsymbol{a})$ for $1\leqslant i\leqslant p$ (property (CF3) of the holomorphic functional calculus). Since, moreover, $z_{n+j}(\boldsymbol{c}) =b_{p+j}$ for $1\leqslant j\leqslant q$ (property (CF2)), we have

$$
(g\circ \pi )(f_1(\boldsymbol{a}), . . . , f_p(\boldsymbol{a}), b_{p+1}, . . . , b_{p+q}) =h(\boldsymbol{a})
$$

whence we deduce $g(f_1(\boldsymbol{a}), . . . , f_p(\boldsymbol{a})) =h(\boldsymbol{a})$ by applying property (CF3) again.

### 9. Holomorphic Functional Calculus in One Variable

#### Theorem 5 {#ts-i-s4-thm-5 .statement tag=02AS}

Let A be a unital Banach algebra, not necessarily commutative. Let $a$ be an element of A and $z$ the germ of the identity function of $\mathbf{C}$ in a neighbourhood of Sp$_A(a)$. There exists a unique continuous unital morphism $\varphi_a$ of $\mathscr{O}$(Sp$_A(a)$) into A such that $\varphi_a(z) =a$.

The image of $\varphi_a$ is contained in the full closed subalgebra of A generated by $a$. In particular, it is contained in the bicommutant of $a$.

Let us prove the existence of the morphism $\varphi_a$. Let B be the full closed subalgebra of A generated by $a$. It is commutative, and we have Sp$_B(a) =$ Sp$_A(a)$ (I, p. 5, No$^o5$). The mapping $\Theta_a$ of the holomorphic functional calculus on B is a continuous unital morphism of $\mathscr{O}$(Sp$_B(a)$) into B such that $\Theta_a(z) =a$ (Theorem 1 of I, p. 51). The morphism composed of $\Theta_a$ and the canonical injection of B into A is a continuous unital morphism $\varphi_a$ of $\mathscr{O}$(Sp$_A(a)$) into A such that the image of $z$ is $a$.

Let us prove uniqueness. Let $\varphi '_a$ be a continuous unital morphism from $\mathscr{O}$(Sp$_A(a)$) into A such that $\varphi '_a(z) =a$. Then $\varphi_a$ and $\varphi '_a$ coincide on the set of germs of polynomials in a neighbourhood of Sp$_A(a)$, hence on the set of germs of rational fractions holomorphic in a neighbourhood of Sp$_A(a)$. But these germs are dense in $\mathscr{O}$(Sp$_A(a)$) (I, p. 69, th. 3). This implies that $\varphi_a=\varphi '_a$.

The construction of $\varphi_a$ proves that its image is contained in the commutative subalgebra B, which is contained in the bicommutant of $a($I, p. 6).

If the radical of the algebra A is zero, the uniqueness of the morphism $\varphi_a$ is valid without requiring that it be continuous (cf. prop. 9 of I, p. 40). This is not so in general, cf. G. R. Allan, Embedding the algebra of formal power series in a Banach algebra, Proc. London Math. Soc. (3) 25 (1972), 329–340.

For every Banach algebra A, every element $a$ of A and every germ $f\in \mathscr{O}$(Sp$_A(a)$), one denotes by $f(a)$ the element $\varphi_a(f)$ of theorem 5. If A is a commutative Banach algebra, this element $f(a)$ coincides with the element $f(a)$ furnished by the holomorphic functional calculus on a commutative Banach algebra (theorem 1 of I, p. 51).

Let B be the closed full subalgebra of A generated by $a$, so that Sp$_A(a) =$ Sp$_B(a)$. The element $f(a)$ of A belongs to B, and coincides with the element $f(a)$ calculated relative to the algebra B.

#### Proposition 7 {#ts-i-s4-prop-7 .statement tag=02AT}

Let A and B be unital Banach algebras and $\varphi$ a continuous unital morphism from A into B. Let $a\in$ A. Then Sp$_B(\varphi (a))\subset$ Sp$_A(a)$ and one has $\varphi (f(a))$ = $f(\varphi (a))$ for every $f\in \mathscr{O}$(Sp$_A(a)$). In particular, for every $\chi \in \mathsf{X}(A)$, one has $\chi (f(a)) =f(\chi (a))$.

This results from prop. 3 of I, p. 66.

#### Proposition 8 {#ts-i-s4-prop-8 .statement tag=02AU}

Let A be a unital Banach algebra and $a\in A$. Let $f\in \mathscr{O}$(Sp($a$)). One has $f$(Sp$_A(a)$) $=$ Sp$_A(f(a))$. Moreover, for every $g\in \mathscr{O}$(Sp$_A(f(a))$), one has $g\circ f\in \mathscr{O}$(Sp$_A(a)$) and $g(f(a)) = (g\circ f)(a)$.

This results from th. 4.

#### Proposition 9 {#ts-i-s4-prop-9 .statement tag=02AV}

Let A be a unital Banach algebra and $a\in A$. Let U be an open neighbourhood of Sp$_A(a)$ and $f\in \mathscr{O}(U)$. Let moreover V be a compact neighbourhood of Sp$_A(a)$ contained in U such that V is a piece of U with oriented boundary $\partial V$.

For every integer $n\geqslant 0$, the mapping $z\mapsto f(z)(z-a)^{-n-1}$ is continuous on $\partial V$, the differential form $z\mapsto f(z)(z-a)^{-n-1}dz$ is integrable on $\partial V$ and one has

(7) $f^{(n)}(a) =2ni\pi$! $\int_{\partial V}f(z)(z-a)^{-n-1}dz$

where $f^{(n)}\in \mathscr{O}(U)$ is the $n$-th derivative of $f$.

We proceed by induction on $n$. When $n= 0$, the result follows from Prop. 1 of I, p. 61. Suppose now that the assertion of the proposition is true for the integer $n\geqslant 0$. Let $g\in \mathscr{O}(\mathbf{C}-$ Sp$_A(a); A)$ be the holomorphic function defined by $g(z) = (z-a)^{-n-1}f(z)$. The differential form $g'(z)dz$ = $dg$ is of class $C^1$; since the piece V is compact, Stokes's formula (VAR, R2, p. 47, 11.2.3) implies

$$
\int_{\partial V}g'(z)dz=\int_{\partial V}dg= 0
$$

Since $g'(z) = (z-a)^{-n-1}f'(z)-(n+1)(z-a)^{-n-2}f(z)$, we deduce

$$
\int_{\partial V}f'(z)(z-a)^{-n-1}dz= (n+ 1)\int_{\partial V}f(z)(z-a)^{-n-2}dz
$$

Applying the induction hypothesis to $f'$, we therefore obtain

$2ni\pi$! $f^{(n+1)}(a) = (n+ 1)\int_{\partial V}f(z)(z-a)^{-n-2}dz$,

which is the assertion of the proposition for the integer $n+ 1$. This completes the proof.

#### Proposition 10 {#ts-i-s4-prop-10 .statement tag=02AW}

Let A be a unital Banach algebra and U an open subset of $\mathbf{C}$.

a) The set Ω of $a\in A$ such that Sp$_A(a)\subset U$ is open in A;

b) Let $f\in \mathscr{O}(U)$. The mapping $a\mapsto f(a)$ of Ω into A is holomorphic, and in particular continuous.

Let $a\in \Omega$. There exists a compact neighbourhood V of Sp$_A(a)$ contained in U which is a piece of U (VAR, R2, p. 46 and p. 47, 11.1.3, d)).

Since the resolvent of $a$ tends to 0 at infinity (Theorem 1, c) of I, p. 24), the mapping $z\mapsto  \|(z-a)^{-1}\|$ is bounded on $\mathbf{C}-\mathring{V}$. Let M denote its least upper bound. If $h\in A$ is such that $\|h\|\leqslant (2M)^{-1}$ and if $z\in \mathbf{C}-\mathring{V}$, we have

$$
z-(a+h) = (1-h(z-a)^{-1})(z-a)
$$

and $\|h(z-a)^{-1}\|\leqslant \frac{1}{2}$, hence $z-(a+h)$ is invertible and its inverse satisfies

$$
(z-(a+h))^{-1}= (z-a)^{-1}\sum_{n=0}^{\infty}(h(z-a)^{-1})^n \tag{8}
$$

with $\|(h(z-a)^{-1})^n\|\leqslant 2^{-n}$ (Prop. 2 of I, p. 22). Thus Sp$_A(a+h)$ is contained in V, hence in U, which proves that Ω is open in A.

Let $f\in \mathscr{O}(U)$. Let $m$ denote the least upper bound of $|f(z)|$ for $z\in \partial V$. Let $a\in A$. For every $h\in A$ such that $\|h\|\leqslant (2M)^{-1}$, we have

$$
f(a+h) =\frac{1}{2i\pi}\int_{\partial V}f(z)(z-(a+h))^{-1}dz
$$

(Prop. 9). The series (8) converges uniformly on the boundary of V, hence

$$
f(a+h) =\sum_{n=0}^{+\infty}f_{a,n}(h)
$$

where the mapping $f_{a,n}$ of A into A is defined by

$$
f_{a,n}(h) =\frac{1}{2i\pi}\int_{\partial V}f(z)(z-a)^{-1}(h(z-a)^{-1})^ndz
$$

For every $n\in \mathbf{N}$, the function $f_{a,n}$ is a continuous homogeneous polynomial function of degree $n$. Moreover, we obtain

$$
\|f_{a,n}(h)\|\leqslant \frac{mM}{\pi}(\int_{\partial V}\|dz\|)2^{-(n+1)}
$$

(INT, VI, §2, No.$^o3$, Prop. 5). The series $\sum_nf_{a,n}(h)$ is therefore absolutely convergent for $\|h\|\leqslant (2M)^{-1}$. This proves that the mapping which associates $f(a)$ with $a$ is holomorphic on Ω (VAR, R1, p. 26, 3.2.1).

#### Proposition 11 {#ts-i-s4-prop-11 .statement tag=02AX}

Let A be a unital Banach algebra, $a\in A$ and U an open neighbourhood of Sp$_A(a)$. Let $\delta$ denote the distance from Sp$_A(a)$ to $\mathbf{C}-$ U. Let $f\in \mathscr{O}(U)$.

a) For every real number $\eta$ such that $0< \eta  < \delta$, there exists a real number $C\geqslant 0$ such that $\|f^{(n)}(a)\|\leqslant Cn$!$\eta^{-n}$ for every integer $n\in \mathbf{N}$;

b) If $b\in A$ commutes with $a$ and if $\varrho (b)< \delta$, one has Sp$_A(a+b)\subset U$, and

$\infty (n)$

$f(a+b) =\sum fn$!$(a)b^n$,

$n=0$

where the series converges absolutely.

Let $\eta$ be a real number such that $0< \eta  < \delta$. Put $\varepsilon =\delta -\eta  >0$. Let K be the compact neighbourhood of Sp$_A(a)$ formed by the points of $\mathbf{C}$ whose distance from Sp$_A(a)$ is $\leqslant \varepsilon /2$. Since $f$ is holomorphic in every open disk of radius $\eta +\varepsilon /2$ whose center belongs to K, there exists, by Cauchy's inequalities (VAR, R1, p. 29, 3.3.4), a real number $C\geqslant 0$ such that

sup$_{z\in K}|f^(\overset{n)}{n}$!$(z)|\leqslant \frac{C}{\eta^n}$

for every integer $n\geqslant 0$. Then assertion a) results from Prop. 1 of I, p. 61 applied to $f^{(n)}$ and to a piece V contained in K.

Let $b$ be an element of A commuting with $a$ such that $\varrho (b)< \delta$. Replacing A by the full closed subalgebra B generated by $a$ and $b$, which satisfies Sp$_A(a) =$ Sp$_B(a)$ and Sp$_A(a+b) =$ Sp$_B(a+b)$, one is reduced, in order to prove b), to the case where A is commutative.

Since $\varrho (b)< \delta$, one can choose $\eta$ such that $\varrho (b)< \eta  < \delta$. Let $V_1$ be the set of points of $\mathbf{C}$ whose distance from Sp$_A(a)$ is $< \delta -\eta$, and $V_2$ the open disk with center 0 and radius $\eta$ in $\mathbf{C}$. Let $g$ be the mapping $(z_1, z_2)\mapsto z_1+z_2$ of $V_1\times V_2$ into U. Then $h=f\circ g$ is the mapping $(z_1, z_2)\mapsto f(z_1+z_2)$ of $V_1\times V_2$ into $\mathbf{C}$. One has Sp$^2_A(a, b)\subset V_1\times V_2$, hence Sp$_A(a+b)\subset U$ (cf. cor. 2 of I, p. 67), and moreover $f(a+b) =h(a, b)$ by th. 4 of I, p. 72. Now, in the space $\mathscr{O}(V_1\times V_2)$, one has

$h(z_1, z_2) =\sum_{n\geqslant 0}f^{(n}\overset{)}{n}($!$z_1)z_2^n$,

(VAR, R1, p. 29, 3.3.4) hence the series

$\sum f^(\overset{n)}{n}$!$(a)b^n$

$n\geqslant 0$ converges in A and its sum is $h(a, b) =f(a+b)$. Moreover, this series is absolutely convergent by assertion a).

### 10. Exponential and logarithm

The complex exponential function of $\mathbf{C}$ into $\mathbf{C}$ is denoted by exp (FVR, III, p. 8, def. 2). It is differentiable and satisfies exp$'=$ exp (FVR, III, p. 9, (26)), hence is holomorphic in $\mathbf{C}$. Let A be a unital Banach algebra and $a$ an element of A. By prop. 2 of I, p. 65 and formula (9) of FVR, III, p. 16, one has

$\infty n$

(9) exp($a$) $=\sum an$!.

$n=0$

Since $\|a^n\|\leqslant \|a\|^n$, one sees that $\|$exp($a$)$\|\leqslant$ exp($\|a\|$) and that series (9) converges uniformly in every ball of A. The mapping $a\mapsto$ exp($a$) of A into A is holomorphic (prop. 10 of I, p. 76). The exponential of $a\in A$ is also sometimes denoted by $e^a$.

When $a$ is an endomorphism of a Banach space E, the exponential exp($a$) resulting in the Banach algebra $\mathscr{L}(E)$ coincides with that defined in FVR, IV, p. 27, def. 1, by loc. cit. prop. 7 (3).

For every element $b$ of A which commutes with $a$, one also has

exp($a+b$) $=\sum^{\infty}bn^n$! exp($a$),

$n=0$

(prop. 11 of I, p. 77), whence

(10) exp($a+b$) $=$ exp($a$)$\cdot$ exp($b$).

In particular, exp($a$) is invertible and

(11) exp($a$)$^{-1}=$ exp($-a$).

Let B be the set of $z\in \mathbf{C}$ such that $-\pi  <\mathscr{I}z < \pi$. Let F be the complement in $\mathbf{C}$ of the interval $\mathbf{R}_-$. The restriction of the exponential to B induces by passing to subspaces a bijection of B onto F (FVR, III, p. 10, n$^o7$), whose reciprocal bijection will be denoted by log.

If $a\in A$ is such that Sp$_A(a)\subset F$, one can form the element log($a$) of A. One has Sp$_A$(log($a$))$\subset B$, and

(12) exp(log($a$)) $=a$ after prop. 8 of I, p. 75. Conversely, let $b$ be an element of A such that Sp$_A(b)\subset B$. One has Sp$_A$(exp($b$))$\subset F$ and

(13) log(exp($b$)) $=b$

(loc. cit.).

In particular, if $a\in A$ is such that $\varrho (a)<1$, one has Sp$_A(1-a)\subset F$ and one can form log(1 $-a$). For $n\geqslant 1$, the $n$-th derivative of $z\mapsto$ log(1$-z$) is $z\mapsto  -(n-$1)!(1$-z$)$^{-n}$ The power series expansion of $z\mapsto$ log(1 $-z$) at the point 0 is therefore

log(1 $-z$) $=-\sum^{\infty}\frac{z^n}{n}$,

$n=1$

valid for $|z|<1$ (VAR, R1, p. 30, 3.3.9). After prop. 2 of I, p. 65, one obtains

(14) log(1 $-a$) $=-\sum_{n=1}^{\infty}\frac{a^n}{n}$.

#### Proposition 12 {#ts-i-s4-prop-12 .statement tag=02AY}

Let A be a commutative unital Banach algebra. The image of the exponential mapping is the identity component of the group G of invertible elements of A.

Formulas (10) and (11) prove that exp(A) is a subgroup of G. By what precedes (see formula (12)), this subgroup contains the open ball with center 1 and radius 1. It is therefore an open subgroup, and hence a closed subgroup, of G. On the other hand, A is connected and the mapping $a\mapsto$ exp($a$) is continuous, so that exp(A) is connected. Therefore exp(A) is the identity component of G.

### 11. Partitions of the character space

#### Proposition 13 {#ts-i-s4-prop-13 .statement tag=02AZ}

Let A be a commutative unital Banach algebra. Let $U_1$ and $U_2$ be open sets of $\mathsf{X}(A)$ forming a partition of $\mathsf{X}(A)$. Then there exists a unique idempotent $j$ of A such that the Gelfand transform $\mathscr{G}(j)$ is equal to 1 on $U_1$ and to 0 on $U_2$.

Let us identify the space $\mathsf{X}(A)$ with a compact subset of $\mathbf{C}^A$ by the mapping $\chi \mapsto (\chi (a))_{a\in A}($cf. No.$^o6$ of I, p. 6 and corollary of Theorem 1 of I, p. 29). The subsets $U_1$ and $U_2$ of the uniform space $\mathbf{C}^A$ are compact and disjoint. By TG, II, p. 31, Proposition 4, there exists a finite subset M of A and disjoint open subsets $V_1$ and $V_2$ of $\mathbf{C}^M$ such that

$$
p(U_1)\subset V_1,p(U_2)\subset V_2
$$

where $p$ is the canonical projection of $\mathbf{C}^A$ onto $\mathbf{C}^M$.

Let $a_1, . . . , a_n$ be the distinct elements of M, and identify $\mathbf{C}^M$ with $\mathbf{C}^n$. We have Sp$^n_A(a_1, . . . , a_n)\subset p(\mathsf{X}(A))\subset V_1\cup V_2$ since $U_1\cup U_2=\mathsf{X}(A)$. Let $f$ be the function on $V_1\cup V_2$ equal to 1 on $V_1$ and to 0 on $V_2$. We have $f\in \mathscr{O}(V_1\cup V_2)$. Put $j=f(a_1, . . . , a_n)$. Since $f^2=f$, we have $j^2=j$. By corollary 1 of I, p. 66, we have $\chi (j) = 1$ if $\chi \in U_1$ and $\chi (j) = 0$ if $\chi \in U_2$, which proves the existence of the required idempotent.

Moreover, if $j_1$ is an idempotent of A, the relations $j^2=j$ and $j_1^2=j_1$ imply $(j-j_1)(j+j_1-1) = 0$. If $\mathscr{G}(j_1) =\mathscr{G}(j)$, the Gelfand transform of $j+j_1-1$ has its values in $\{-1,1\}$, hence $j+j_1-1$ is invertible (Proposition 6 of I, p. 37), whence $j=j_1$.

#### Corollary {#ts-i-s4-n11-cor-1 .statement tag=02B0}

Let A be a commutative unital Banach algebra. The following assertions are equivalent:

a) The space of characters $\mathsf{X}(A)$ is not connected;

b) There exists an idempotent element of A different from 0 and 1;

c) The algebra A is isomorphic to the product of two non-zero Banach algebras.

The proposition proves that a) implies b). If $j$ is an idempotent of A, let $I_1=jA$ and $I_2= (1-j)A$. Then $I_1$ and $I_2$ are closed ideals of A, and $I_1+ I_2= A$. If $j \notin  \{0,1\}$, the ideals $I_1$ and $I_2$ are distinct from A. On the other hand, the ideal $I_1$ (resp. $I_2$) is the set of elements $x$ of A such that $jx=x$ (resp. $(1-j)x=x$), hence $I_1\cap I_2=\{0\}$. The algebra A is therefore identified with the product $A/I_1\times A/I_2$. Thus assertion b) implies c). Finally, if A is isomorphic to $A_1\times A_2$, the space $\mathsf{X}(A)$ is identified with the sum space of $\mathsf{X}(A_1)$ and of $\mathsf{X}(A_2)$ (I, p. 6, n$^o6$), hence c) implies a).

#### Proposition 14 {#ts-i-s4-prop-14 .statement tag=02B1}

Let A be a commutative Banach algebra without radical. In order that A admit a unit element, it is necessary and sufficient that $\mathsf{X}(A)$ be compact.

The condition is necessary (I, p. 29, corollaire). Suppose $\mathsf{X}(A)$ compact. Let $\widetilde{A}$ be the Banach algebra deduced from A by adjunction of a unit element, and identify $\mathsf{X}'(A)$ with $\mathsf{X}(\widetilde{A})$. The complement of $\mathsf{X}(A)$ in $\mathsf{X}(\widetilde{A})$ reduces to the character $\chi_0$ of $\widetilde{A}$ whose kernel is A. The subsets $\mathsf{X}(A)$ and $\{\chi_0\}$ are open in $\mathsf{X}(\widetilde{A})$. By Prop. 13, there exists an element $j\in A$ such that $\chi (j) = 1$ for $\chi \in \mathsf{X}(A)$, and $\chi_0(j) = 0$. Hence $j\in A$.

Let then $x$ be in A. We have $\chi (jx) =\chi (x)$ for every $\chi \in \mathsf{X}(A)$, hence $jx=x$ since A is without radical. Thus, $j$ is a unit element of A.

#### Proposition 15 {#ts-i-s4-prop-15 .statement tag=02B2}

Let A be a commutative Banach algebra, let $I_1$ be an ideal of A and $F_1$ the set of $\chi \in \mathsf{X}(A)$ which are zero on $I_1$. Let $F_2$ be a subset of $\mathsf{X}(A)$ disjoint from $F_1$, closed for the Jacobson topology, and compact for the weak topology. Then there exists $u\in I_1$ such that $\mathscr{G}(u) = 1$ on $F_2$.

Let $I_2$ be the intersection of the kernels of the characters belonging to $F_2$. The Banach algebra $A/I_2$ is semisimple (Prop. 8 of I, p. 38). Since $F_2$ is closed for the Jacobson topology, the only elements of $\mathsf{X}(A)$ vanishing on $I_2$ are those of $F_2($cf. I, p. 13). Hence $F_2$, endowed with the topology induced by the weak topology of $\mathsf{X}(A)$, is identified with $\mathsf{X}(A/I_2)$ endowed with the weak topology (I, p. 9, n$^o7$). Since $F_2$ is weakly compact, the algebra $A/I_2$ has a unit element (Prop. 14).

One then has $I_1+ I_2= A$. For otherwise, $(I_1+ I_2)/I_2$ would be a proper ideal, hence contained in the kernel of a nonzero character of $A/I_2($I, p. 30, Th. 2). The latter would define, by composition with the canonical projection $A\rightarrow A/I_2$, a nonzero character $\chi$ of A which would vanish on $I_1$ and $I_2$, and would therefore belong to $F_1\cap F_2$, contrary to the hypothesis.

Since $I_1+ I_2= A$, there exists $u\in I_1$ whose class in $A/I_2$ is a unit element of $A/I_2$. Then $\chi (u) = 1$ for every $\chi \in F_2$, which concludes the proof.

#### Corollary {#ts-i-s4-n11-cor-2 .statement tag=02B3}

Let A be a commutative Banach algebra. Let $F_1$ and $F_2$ be two disjoint subsets of $\mathsf{X}(A)$, closed for the Jacobson topology. Assume that $F_2$ is weakly compact. Then there exists $u\in A$ such that $\mathscr{G}(u) = 1$ on $F_2$ and $\mathscr{G}(u) = 0$ on $F_1$.

### 12. Partitions of the spectrum of an element

Let A be a unital Banach algebra, $x\in A$, and K = Sp$_A(x)$. Let Π denote the set of subsets of K which are open and closed in K. Let B be the full closed subalgebra of A generated by $x$; it is commutative.

For every $H\in \Pi$, there exists a unique element $f_H$ of $\mathscr{O}(K)$ equal to 1 in a neighbourhood of H and to 0 in a neighbourhood of K - H. Put $j_H=f_H(x)$. The element $j_H$ is an idempotent of A, said to be associated with $x$ and H, and one has the following formulae:

$$
j_{H\cap H'}=j_Hj_{H'}=j_{H'}j_H(H,H'\in \Pi ) \tag{15}
$$

$$
j_{H\cup H'}=j_H+j_{H'}-j_{H'}j_H(H,H'\in \Pi ) \tag{16}
$$

$$
j_{\emptyset}= 0,j_K= 1
$$

Let $H\in \Pi$. Define $A_H=j_HAj_H$. This is a closed subalgebra of A, admitting the unit element $j_H($cf. Lemma 1 of I, p. 2). Put also $B_H=j_HBj_H$ and $x_H=xj_H=j_Hx=j_Hxj_H\in B_H$.

Let $g_H$ be the element of $\mathscr{O}(K)$ defined by $g_H(z) =z$ in a neighbourhood of H and $g_H(z) = 0$ in a neighbourhood of K - H. One has $g_H(z) =f_H(z)z$ on K, and therefore $x_H=g_H(x)$. It follows that, if $H\not= K$, one has

Sp$_A(x) =g_H(K) = H\cup  \{0\}$.

Let $\lambda \in \mathbf{C}-$ H. Let $h_{H,\lambda}$ denote the element of $\mathscr{O}(K)$ equal to $(\lambda -z)^{-1}$ in a neighbourhood of H and to 0 in a neighbourhood of K - H. We have $h_{H,\lambda}=f_Hh_{H,\lambda}$ and $(\lambda f_H-g_H)h_{H,\lambda}=f_H$. If we set $R_H(x, \lambda ) =h_{H,\lambda}(x)$, then $R_H(x, \lambda )\in B_H$ and

$$
R_H(x, \lambda )(\lambda j_H-x_H) = (\lambda j_H-x_H)R_H(x, \lambda ) =j_H \tag{17}
$$

$$
R_H(x, \lambda )j_{K-H}=j_{K-H}R_H(x, \lambda ) = 0
$$

In particular, $\lambda \in \mathbf{C}-$ Sp$_{A_H}(x_H)$.

Let now $\lambda \in H$. Suppose that $\lambda j_H-x_H$ has an inverse $y$ in $A_H$. Using the formulas $j_Hy=y$ (since $y\in A_H$) and $j_{K-H}R_{K-H}(x, \lambda ) = R_{K-H}(x, \lambda )$ (since $R_{K-H}(x, \lambda )\in A_{K-H}$), we find

$$
(\lambda -x)(y+ R_{K-H}(x, \lambda )) = (\lambda -x)(j_Hy+j_{K-H}R_{K-H}(x, \lambda )) =
$$

$$
(\lambda j_H-xj_H)y+ (\lambda j_{K-H}-xj_{K-H})R_{K-H}(x, \lambda ) =j_H+j_{K-H}= 1
$$

(by formula (17) applied to K - H). One verifies analogously that

$$
(y+ R_{K-H}(x, \lambda ))(\lambda -x) = 1
$$

This proves that $\lambda -x$ has in A the inverse $y+ R_{K-H}(x, \lambda )$, which is absurd. Thus we have $\lambda \in$ Sp$_{A_H}(x_H)$. We therefore conclude that

(18) Sp$_{A_H}(x_H) = H$. In particular, if H is nonempty, the idempotent $j_H$ is nonzero.

Formulas (17) and (18) prove that the function $\lambda \mapsto R_H(x, \lambda )$, defined in $\mathbf{C}-$ H, is the resolvent of $x_H$ relative to $A_H$.

#### Proposition 16 {#ts-i-s4-prop-16 .statement tag=02B4}

We retain the preceding notation. Let $(H_i)_{1\leqslant i\leqslant n}$ be a partition of Sp$_A(x)$ into elements of Π.

a) The algebra B is canonically identified with the algebra $B_{H_1}\times \cdots \times B_{H_n}$;

b) We have $x_{H_i}x_{H_j}= 0$ for $i\not=j$, and

$$
x=x_{H_1}+x_{H_2}+\cdots +x_{H_n}
$$

c) We have

$$
R(x, \lambda ) = R_{H_1}(x, \lambda ) +\cdots + R_{H_n}(x, \lambda ) \tag{19}
$$

for every $\lambda \in \mathbf{C}-$ Sp$_A(x)$. In particular, if $H\in \Pi$, the resolvent $\lambda \mapsto R(x, \lambda )$ is equal in a neighbourhood of H to the sum of $R_H(x, \lambda )$ and a holomorphic function.

The relation 1 = $j_{H_1}+\cdots +j_{H_n}$ is a decomposition of 1 into pairwise orthogonal idempotents of B, hence the algebra B is canonically identified with the product algebra $B_{H_1}\times  \cdots  \times B_{H_n}$ (A, I, p. 105, prop. 10).

Assertion b) follows from the corresponding relations for the functions $g_{H_i}$; assertion c) is a consequence of a) and of the equality $R(x_H, \lambda ) = R_H(x, \lambda )$.

#### Proposition 17 {#ts-i-s4-prop-17 .statement tag=02B5}

Let $\mu$ be an isolated point of Sp$_A(x)$. Then

a) For every $\lambda \in \mathbf{C}-$ Sp$_A(x)$, we have

$R(x, \lambda ) = R_{\{\mu\}}(x, \lambda ) + R_{Sp_A(x)-\{\mu\}}(x, \lambda )$ ;

b) The function which associates to $\lambda$ $R_{Sp_A(x)-\{\mu\}}(x, \lambda )$ is holomorphic in $\mathbf{C}-$ Sp$_A(x)$ and in a neighbourhood of $\mu$; moreover, the function which associates to $\lambda$ $R_{\{\mu\}}(x, \lambda )$ is holomorphic in $\mathbf{C}-\{\mu\}$;

c) One has

lim$_{n\rightarrow+\infty}\|(x-\mu)^nj_{\{\mu\}}\|^{1/n}= 0$

and, for $\lambda \in \mathbf{C}-\{\mu\}$, the formula

$$
R_{\{\mu\}}(x, \lambda ) =\sum_{n=0}^{\infty}(\lambda -\mu)^{-n-1}(x-\mu)^nj_{\{\mu\}} \tag{20}
$$

The foregoing implies assertions a) and b). Let us prove c). Replacing $x$ by $x-\mu$, we are reduced to the case where $\mu= 0$. Put $H =\{0\}$; this is an open and closed subset of Sp$_A(x)$. By formula (18), the spectrum of $x_H$ in $A_H$ is $\{0\}$, hence $x_H$ is quasi-nilpotent, that is to say, $\|x^nj_H\|^{1/n}=\|(xj_H)^n\|^{1/n}$ tends to 0 as $n$ tends to $+\infty$. Moreover, for $\lambda \not= 0$, one has in $A_H$

$$
(\lambda j_H-x_H)^{-1}=\sum_{n=0}^{\infty}\lambda^{-n-1}x^n_H
$$

(Theorem 1 of I, p. 24, d)), whence (20).

#### Corollary 1 {#ts-i-s4-prop-17-cor-1 .statement tag=02B6}

Let $\mu$ be an isolated point of Sp$_A(x)$ and $p$ a strictly positive integer. In order that $\mu$ be a pole of order $p$ of the resolvent of $x($cf. VAR, R1, p. 30, 3.3.9), it is necessary and sufficient that $(x-\mu)^{p-1}j_{\{\mu\}}\not= 0$ and $(x-\mu)^pj_{\{\mu\}}= 0$.

#### Corollary 2 {#ts-i-s4-prop-17-cor-2 .statement tag=02B7}

Let $\mu$ be an isolated point of Sp$_A(x)$. Let Γ be the oriented boundary of an open disk Δ with center $\mu$ such that

Sp$_A(x)\cap (\Gamma \cup \Delta ) =\{\mu\}$.

Then the idempotent $j_{\{\mu\}}$ associated with $x$ and $\{\mu\}$ is given by

$$
j_{\{\mu\}}=\frac{1}{2i\pi}\int_{\Gamma}(z-x)^{-1}dz
$$

*In other words, the idempotent $j_{\{\mu\}}$ is the residue at $\mu$ of the resolvent of $x.*$

For $z\in \mathbf{C}-$ Sp$_A(x)$, one has

$$
(z-u)^{-1}= R(x, z) = R_{\{\mu\}}(x, z) + R_H(x, z)
$$

where H = Sp$_A(x)-\{\mu\}$ (formula (19)). The function $z\mapsto R_H(x, z)$ is holomorphic in $\mathbf{C}-$ H and in a neighbourhood of $\{\mu\}$ (Prop. 17, b)), hence

$$
\frac{1}{2i\pi}\int_{\Gamma}R_H(x, z)dz= 0
$$

(VAR, R2, p. 48, 11.2.5). The function $z\mapsto R_{\{\lambda\}}(x, z)$ is the resolvent of the element $j_{\{\mu\}}xj_{\{\mu\}}$ of the unital algebra $A_{\{\mu\}}$. One then has

$$
j_{\{\mu\}}=\frac{1}{2i\pi}\int_{\Gamma}R_{\{\mu\}}(x, z)dz
$$

by Prop. 9 of I, p. 75 applied to $A_{\{\mu\}}$ and to the constant function 1 in a neighbourhood of $\Delta \cup \Gamma$. The corollary follows.

### 13. Holomorphic functional calculus in a complete normable real or complex algebra

Let E be a real topological vector space. The complexified topological vector space $\mathbf{C}\otimes E$ of E (TVS, II, p. 65) is denoted by $E_{(\mathbf{C})}$ and E is identified with a real topological vector subspace of $E_{(\mathbf{C})}$ by the mapping $x\mapsto 1\otimes x$.

#### Proposition 18 {#ts-i-s4-prop-18 .statement tag=02B8}

The complex topological vector space $E_{(\mathbf{C})}$ is normable (resp. complete) if and only if E is normable (resp. complete).

The underlying real topological vector space of $E_{(\mathbf{C})}$ is isomorphic to $E\times E$. Hence $E_{(\mathbf{C})}$ is complete if and only if E is complete, and E is normable if $E_{(\mathbf{C})}$ is so.

Suppose conversely that E is normable. Let $p$ be a norm defining the topology of E and B the unit ball of $p$. There exists a closed balanced neighbourhood V of 0 in $E_{(\mathbf{C})}$ contained in $B +iB$ (TVS, II, p. 66). The sets $\lambda V$, where $\lambda$ ranges over $\mathbf{R}^*_+$, therefore form a fundamental system of neighbourhoods of 0 in $E_{(\mathbf{C})}$. The gauge of V is a norm on $E_{(\mathbf{C})}$ defining the topology of $E_{(\mathbf{C})}$, therefore $E_{(\mathbf{C})}$ is normable.

#### Remark {#ts-i-s4-n13-rem-1 .statement tag=02B9}

Let E and F be normable topological vector spaces over K. The vector space $\mathscr{L}(E; F)$ of continuous linear mappings from E into F, endowed with the topology of bounded convergence, is a normable topological vector space (TVS, III, p. 14).

Let E and F be normable topological vector spaces over $\mathbf{R}$. The $\mathbf{C}$-linear mapping $\varphi :\mathscr{L}(E; F)_{(\mathbf{C})}\rightarrow \mathscr{L}(E_{(\mathbf{C})}; F_{(\mathbf{C})})$ defined by $\varphi (\lambda \otimes u) =\lambda u_{(\mathbf{C})}$ is an isomorphism of complex topological vector spaces. In particular, the dual of $E_{(\mathbf{C})}$ is identified with the complexified dual of E and the normable algebra $\mathscr{L}(E_{(\mathbf{C})})$ with the complexified of the normable algebra $\mathscr{L}(E)$.

Let S be a compact subset of $\mathbf{C}$ stable under complex conjugation. Consider the $\mathbf{C}$-algebra $\mathscr{O}(S)$ of germs of holomorphic functions with complex values in a neighbourhood of S, endowed with the complex locally convex space structure defined in No. 1 of I, p. 49. If U is an open neighbourhood of S in $\mathbf{C}$, and $h: U\rightarrow \mathbf{C}$ a holomorphic function, the image V of U under complex conjugation is an open neighbourhood of S in $\mathbf{C}$ and $h^*:w\mapsto \overline{h(\overline{w})}$ is a holomorphic function on V. By passing to the inductive limit one deduces a continuous involution $f\mapsto f^*$ in the algebra $\mathscr{O}(S)$. In particular, one has:

$$
(f+g)^*=f^*+g^*(f g)^*=f^*g^*(\lambda f)^*=\lambda f^*
$$

for $f, g$ in $\mathscr{O}(S)$ and $\lambda$ in $\mathbf{C}$.

The set of germs $f\in \mathscr{O}(S)$ such that $f=f^*$ is denoted by $\mathscr{O}_{\mathbf{R}}(S)$. It is a closed full sub-$\mathbf{R}$-algebra of $\mathscr{O}(S)$.

#### Proposition 19 {#ts-i-s4-prop-19 .statement tag=02BA}

Let $z$ denote the germ in $\mathscr{O}(S)$ of the identity mapping of $\mathbf{C}$. Then $\mathscr{O}_{\mathbf{R}}(S)$ is the smallest closed full sub-$\mathbf{R}$-algebra of $\mathscr{O}(S)$ containing $z$.

We have $z^*=z$; hence $z$ belong to $\mathscr{O}_{\mathbf{R}}(S)$. Let B be a full closed sub-$\mathbf{R}$-algebra of $\mathscr{O}(S)$ containing $z$. The mapping $f\mapsto f+f^*$ of $\mathscr{O}(S)$ into $\mathscr{O}_{\mathbf{R}}(S)$ is continuous and surjective, and the set of germs of rational functions holomorphic in a neighbourhood of S is dense in $\mathscr{O}(S)$ (Theorem 3 of I, p. 69). To prove that B contains $\mathscr{O}_{\mathbf{R}}(S)$, it therefore suffices to prove that if $f$ is the germ of such a rational function, then $f+f^*\in B$.

There exist polynomials P and Q in $\mathbf{C}[X]$ such that Q vanishes at no point of S and such that one has $f=\frac{P(z)}{Q(z)}$. Let $P^*$ and $Q^*$ denote the polynomials obtained by replacing the coefficients of P and Q by their conjugates. One then has $P(z)^*= P^*(z)$ and $Q(z)^*= Q^*(z)$. Since S is stable under complex conjugation, the polynomial $Q^*$ vanishes at no point of S. The germs $Q^*(z)$ and (QQ$^*$)$(z)$ are therefore invertible in $\mathscr{O}(S)$, and

$f+f^*=\frac{P(z)}{Q(z)}+\frac{P^*(z)}{Q^*(z)}=$ (PQ(QQ$^*+ P_*$)$(^*Q)(z)z$).

Since the polynomials PQ$^*+ P^*Q$ and QQ$^*$ have real coefficients and B is a full sub-$\mathbf{R}$-algebra of $\mathscr{O}(S)$ containing $z$, the element $f+f^*$ belong to B. This concludes the proof of the proposition.

Let A be a complete normable unital algebra over $\mathbf{R}$. Let $x$ be an element of A. The spectrum of the element $1\otimes x$ of the algebra $A_{(\mathbf{C})}$ is called the complex spectrum of $x$, and is denoted by Sp$_{A_{(\mathbf{C})}}(x)$. Its intersection with the set $\mathbf{R}$ is none other than the spectrum Sp$_A(x)$ of $x$ relative to A, which is sometimes called the real spectrum of $x$. The complex spectrum Sp$_{A_{(\mathbf{C})}}(x)$ is a compact subset of $\mathbf{C}$, stable under complex conjugation. It is not empty when the algebra A is not reduced to 0.

Let $x$ be an element of A. The spectral radius of $1\otimes x\in A_{(\mathbf{C})}$ is equal to the spectral radius $\varrho (x)$ of $x$. It is the smallest real number $r\geqslant 0$ such that $|\lambda |\leqslant r$ for every $\lambda \in$ Sp$_{A_{(\mathbf{C})}}(x)$. One has

$\varrho (x) =$ lim$_{n\rightarrow+\infty}\|x^n\|^{1/n}=$ inf$_{n>0}\|x^n\|^{1/n}$

for every norm on A which defines the topology of A. In fact, one may suppose that the norm on A is the restriction of a norm on $A_{(\mathbf{C})}$ which defines the topology of $A_{(\mathbf{C})}$ and apply Prop. 1 of I, p. 20.

Let us denote by $u\mapsto \overline{u}$ the endomorphism of the $\mathbf{R}$-algebra $A_{(\mathbf{C})}$ which maps $\lambda \otimes a$ to $\overline{\lambda}\otimes a$. It is continuous.

#### Lemma {#ts-i-s4-n13-lem-1 .statement tag=02BB}

For every $f\in \mathscr{O}$(Sp$_{A_{(\mathbf{C})}}(x)$), one has $f^*(1\otimes x) =\overline{f(1 \otimes x)}$.

The mappings $f\mapsto f(1\otimes x)$ and $f\mapsto \overline{f^*(1 \otimes x)}$ are continuous unital homomorphisms of $\mathbf{C}$-algebras from $\mathscr{O}$(Sp($x$)) into $A_{(\mathbf{C})}$ which map $z$ to $1\otimes x$; they are therefore equal (I, p. 74, th. 5).

#### Proposition 20 {#ts-i-s4-prop-20 .statement tag=02BC}

For every $f\in \mathscr{O}_{\mathbf{R}}$(Sp$_{A_{(\mathbf{C})}}(x)$), there exists a unique element $f(x)$ of A such that $f(1\otimes x) = 1\otimes f(x)$ in $A_{(\mathbf{C})}$. The mapping $f\mapsto f(x)$ from $\mathscr{O}_{\mathbf{R}}$(Sp$_{A_{(\mathbf{C})}}(x)$) into A is the unique continuous unital homomorphism of $\mathbf{R}$-algebras which maps to $x$ the germ in $\mathscr{O}_{\mathbf{R}}$(Sp$_{A_{(\mathbf{C})}}(x)$) of the identical mapping of $\mathbf{C}$.

Let us put S = Sp$_{A_{(\mathbf{C})}}(x)$. By the above lemma, for every germ $f\in \mathscr{O}_{\mathbf{R}}$(Sp($x$)), one has $f(1\otimes x) =\overline{f(1 \otimes x)}$. The first assertion follows from this. Let us denote by $z$ the germ in $\mathscr{O}_{\mathbf{R}}(S)$ of the identical mapping of $\mathbf{C}$. The mapping $f\mapsto f(x)$ is a continuous unital homomorphism of the $\mathbf{R}$-algebra $\mathscr{O}_{\mathbf{R}}$(Sp($x$)) into A, which maps $z$ to $x$. It is the only one by prop. 19, since every morphism having these properties is uniquely determined on every full closed sub-$\mathbf{R}$-algebra of $\mathscr{O}(S)$ containing $z$.

Let $f\in \mathscr{O}_{\mathbf{R}}$(Sp$_{A_{(\mathbf{C})}}(x)$). The element $f(x)$ belongs to every full closed subalgebra of A containing $x$ (prop. 19), and therefore belongs to the bicommutant of $x$ in A. The complex spectrum of $f(x)$ is equal to $f$(Sp($x$)) (I, p. 75, prop. 8). For every $g\in \mathscr{O}_{\mathbf{R}}(f$(Sp$_{A_{(\mathbf{C})}}(x)$)), one has $g\circ f\in \mathscr{O}_{\mathbf{R}}$(Sp$_{A_{(\mathbf{C})}}(x)$) and (loc. cit.) $(g\circ f)(x) =g(f(x))$.

Let U be an open subset of $\mathbf{C}$, stable under complex conjugation. The set Ω of elements $x$ of A whose complex spectrum is contained in U is open in A (I, p. 76, Prop. 10). Let $f$ be a holomorphic function on U such that $f^*=f$. The mapping $x\mapsto f(x)$ of Ω into A is analytic (loc. cit.).

Let A, B be complete normable unital associative algebras over $\mathbf{R}$ and let $\varphi : A\rightarrow$ B be a continuous unital algebra morphism. Let $x\in A$. The complex spectrum of $\varphi (x)$ is contained in that of $x$ and, for every $f\in \mathscr{O}_{\mathbf{R}}$(Sp$_{A_{(\mathbf{C})}}(x)$), one has $f(\varphi (x)) =\varphi (f(x))$. This results at once from the analogous statement in the complex case (I, p. 75, Prop. 8).

### 14. Case of an Algebra without Unit Element

Let A be a complete normable algebra, not necessarily unital, over $K =\mathbf{R}$ or $\mathbf{C}$. Let $(\widetilde{A}, e)$ denote the unital algebra obtained from A by adjunction of a unit element. It is normable and complete.

Let $x$ be an element of A. If $K =\mathbf{C}$, let Sp$'(x) =$ Sp$_{\widetilde{A}}(x)$ denote the spectrum of $x$ relative to $\widetilde{A}$, and consider a germ $f\in \mathscr{O}$(Sp$'(x)$). If $K =\mathbf{R}$, let Sp$'(x)$ denote the complex spectrum of the element $x$ of $\widetilde{A}$, and consider a germ $f\in \mathscr{O}_{\mathbf{R}}$(Sp$'(x)$). In both cases, 0 belongs to Sp$'(x)$, and the element $f(x)$ of $\widetilde{A}$ belongs to A if and only if $f$ satisfies $f(0) = 0$. In fact, the projection $\pi :\widetilde{A}\rightarrow Ke$ is a continuous morphism whose kernel is A, and one has $\pi (f(x)) =f(\pi (x)) =f(0)$.

## EXERCISES {#ts-i-s4-exercises}

In the exercises below, all the algebras considered are over $\mathbf{C}$, unless there is explicit mention to the contrary.

See the [exercises for § 4](exercises/s4/).
