---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 3
section_title: Conjugacy theorems
lang: en
source: lie-vii-ix
book_pages: A VII.20-A VII.27, A VII.57-A VII.62
pdf_pages: 0030-0037, 0066-0071
extraction: native
subsections:
    - "no": 1
      title: ELEMENTARY AUTOMORPHISMS
      page: 20
      pdf_page: 30
    - "no": 2
      title: CONJUGACY OF CARTAN SUBALGEBRAS
      page: 22
      pdf_page: 32
    - "no": 3
      title: APPLICATIONS OF CONJUGACY
      page: 24
      pdf_page: 34
    - "no": 4
      title: CONJUGACY OF CARTAN SUBALGEBRAS OF SOLVABLE LIE ALGEBRAS
      page: 25
      pdf_page: 35
    - "no": 5
      title: LIE GROUP CASE
      page: 26
      pdf_page: 36
statements: 17
exercises: 18
content_sha256: 328dbc41ee606865fc60e4c126e9e7181b193c73a291316876d1391ffa9c93d1
---

## § 3. CONJUGACY THEOREMS

In this paragraph, the base field $k$ is of characteristic 0.

### 1. ELEMENTARY AUTOMORPHISMS

Let $\mathfrak{g}$ be a Lie algebra. Denote its group of automorphisms by Aut($\mathfrak{g}$). If $x\in \mathfrak{g}$ and if ad $x$ is nilpotent, $e^{adx}\in$ Aut($\mathfrak{g}$) (Chap. I, §6, no. 8).

#### Definition 1 {#lie-vii-s3-def-1 .statement tag=00V0}

A finite product of automorphisms of $\mathfrak{g}$ of the form $e^{adx}$ with ad $x$ nilpotent is called an elementary automorphism of $\mathfrak{g}$. The group of elementary automorphisms of $\mathfrak{g}$ is denoted by Aut$_e(\mathfrak{g})$.

If $u\in$ Aut($\mathfrak{g}$)$,ue^{adx}u^{-1}=e^{adu(x)}$. It follows that Aut$_e(\mathfrak{g})$ is a normal subgroup of Aut($\mathfrak{g}$). If $k=\mathbf{R}$ or $\mathbf{C}$, Aut$_e(\mathfrak{g})$ is contained in the group Int($\mathfrak{g}$) of inner automorphisms of $\mathfrak{g}$ (Chap. III, §6, no. 2, Def. 2).

$^*$ In the general case, Aut$_e(\mathfrak{g})$ is contained in the identity component of the algebraic group Aut($\mathfrak{g}$)$._*$

#### Lemma 1 {#lie-vii-s3-lem-1 .statement tag=00V1}

Let V be a finite dimensional vector space, $\mathfrak{n}$ a Lie subalgebra of $\mathfrak{a}=\mathfrak{g}\mathfrak{l}(V)$ consisting of nilpotent elements.

(i) The map $x \rightarrow$ exp $x$ is a bijection from $\mathfrak{n}$ to a subgroup N of $\mathbf{G}\mathbf{L}(V)$ consisting of unipotent elements (Chap. II, §6, no. 1, Remark 4). We have $\mathfrak{n}=$ log(exp$\mathfrak{n})$. The map $f \rightarrow f\circ$ log is an isomorphism from the algebra of polynomial functions on $\mathfrak{n}$ to the algebra of restrictions to N of polynomial functions on End(V).

(ii) If $x\in \mathfrak{n}$ and $a\in \mathfrak{a}$,

(exp ad$_{\mathfrak{a}}x).a=$ (exp $x)a$(exp($-x$)).

(iii) Let $V'$ be a finite dimensional vector space, $\mathfrak{n}'$ a Lie subalgebra of $\mathfrak{g}\mathfrak{l}(V')$ consisting of nilpotent elements, $\rho$ a homomorphism from $\mathfrak{n}$ to $\mathfrak{n}'$. Let $\pi$ be the map exp $x \rightarrow$ exp $\rho (x)$ from exp$\mathfrak{n}$ to exp$\mathfrak{n}'$. Then $\pi$ is a group homomorphism.

By Engel’s theorem, we can identify V with $k^n$ in such a way that $\mathfrak{n}$ is a subalgebra of $\mathfrak{n}(n, k)$ (the Lie subalgebra of $\mathbf{M}_n(k)$ consisting of the lower triangular matrices with zeros on the diagonal). For $s\geq 0$, let $\mathfrak{n}_s(n, k)$ be the set of $(x_{ij})_{1\leq i,j\leq n}\in \mathbf{M}_n(k)$ such that $x_{ij}= 0$ for $i-j < s$. Then

$$
[\mathfrak{n}_s(n, k),\mathfrak{n}_{s'}(n, k)]\subset \mathfrak{n}_{s+s'}(n, k)
$$

(Chap. II, §4, no. 6, Remark), and the Hausdorff series defines a polynomial map $(a, b) \rightarrow H(a, b)$ from $\mathfrak{n}(n, k)\times \mathfrak{n}(n, k)$ to $\mathfrak{n}(n, k)$ (Chap. II, §6, no. 5, Remark 3); this map makes $\mathfrak{n}(n, k)$ into a group (Chap. II, §6, no. 5, Prop. 4). By Chap. II, §6, no. 1, Remark 4, the maps $x \rightarrow$ exp $x$ from $\mathfrak{n}(n, k)$ to $1 +\mathfrak{n}(n, k)$ and $y \rightarrow$ log $y$ from $1 +\mathfrak{n}(n, k)$ to $\mathfrak{n}(n, k)$ are inverse bijections and are polynomial; by Chap. II, §6, no. 5, Prop. 3, these maps are isomorphisms of groups if $\mathfrak{n}(n, k)$ is given the group law $(a, b) \rightarrow H(a, b)$ and if $1 +\mathfrak{n}(n, k)$ is considered as a subgroup of $\mathbf{G}\mathbf{L}_n(k)$. Assertions (i) and (iii) of the lemma now follow. Let $x\in \mathfrak{n}$. Denote by $L_x,R_x$ the maps $u \rightarrow xu, u \rightarrow ux$ from $\mathfrak{a}$ to $\mathfrak{a}$, which commute and are nilpotent. We have ad$_{\mathfrak{a}}x= L_x-R_x$, so, for all $a\in \mathfrak{a}$,

(exp ad$_{\mathfrak{a}}x)a=$ (exp(L$_x-R_x))a=$ (exp $L_x$)(exp $R_{-x})a$ (1)

$$
\sum L^i_xR^j_{-x}
$$

= $a=$ (exp $x)a$(exp($-x$)).

$i$! $j$!

$i,j\geq 0$

With the notation in Lemma $1,\pi$ is called the linear representation of exp $\mathfrak{n}$ compatible with the given representation $\rho$ of $\mathfrak{n}$ on $V'$. When $k$ is $\mathbf{R}$, $\mathbf{C}$, or a non-discrete complete ultrametric field, $\rho = L(\pi )$ by the properties of exponential maps (Chap. III, §4, no. 4, Cor. 2 of Prop. 8).

#### Proposition 1 {#lie-vii-s3-prop-1 .statement tag=00V2}

Let $\mathfrak{g}$ be a Lie algebra, $\mathfrak{n}$ a subalgebra of $\mathfrak{g}$ such that ad$_{\mathfrak{g}}x$ is nilpotent for all $x\in \mathfrak{n}$. Then $e^{ad_{\mathfrak{g}}\mathfrak{n}}$ is a subgroup of Aut$_e(\mathfrak{g})$.

This follows immediately from Lemma 1 (i).

In particular, if $\mathfrak{n}$ is the nilpotent radical of $\mathfrak{g},e^{ad_{\mathfrak{g}}\mathfrak{n}}$ is the group of special automorphisms of $\mathfrak{g}$ (Chap. I, §6, no. 8, Def. 6).

#### Remark 1 {#lie-vii-s3-n1-rem-1 .statement tag=00V3}

Let V be a finite dimensional vector space, $\mathfrak{g}$ a Lie subalgebra of $\mathfrak{a}=\mathfrak{g}\mathfrak{l}$(V), $x$ an element of $\mathfrak{g}$ such that ad$_{\mathfrak{g}}x$ is nilpotent. Then there exists a nilpotent element $n$ of $\mathfrak{a}$ such that ad$_{\mathfrak{a}}n$ extends ad$_{\mathfrak{g}}x$. Indeed, let $s, n$ be the semi-simple and nilpotent components of $x$; then ad$_{\mathfrak{a}}s$ and ad$_{\mathfrak{a}}n$ are the semi-simple and nilpotent components of ad$_{\mathfrak{a}}x$ (Chap. I, §5, no. 4, Lemma 2), so ad$_{\mathfrak{a}}s$ and ad$_{\mathfrak{a}}n$ leave $\mathfrak{g}$ stable, and ad$_{\mathfrak{a}}s|\mathfrak{g}$ and ad$_{\mathfrak{a}}n|\mathfrak{g}$ are the semi-simple and nilpotent components of ad$_{\mathfrak{g}}x$; consequently, ad$_{\mathfrak{g}}x=$ ad$_{\mathfrak{a}}n|\mathfrak{g}$, which proves our assertion. In view of Lemma 1 (ii), every elementary automorphism of $\mathfrak{g}$ extends to an automorphism of $\mathfrak{a}$ of the form $u \rightarrow mum^{-1}$ where $m\in \mathbf{G}\mathbf{L}(V)$.

#### Remark 2 {#lie-vii-s3-n1-rem-2 .statement tag=00V4}

Let V be a finite dimensional vector space. For all $g\in \mathbf{S}\mathbf{L}$(V), let $\varphi (g)$ be the automorphism $x \rightarrow gxg^{-1}$ of $\mathfrak{g}\mathfrak{l}(V)$. Then

Aut$_e(\mathfrak{g}\mathfrak{l}(V)) =\varphi (\mathbf{S}\mathbf{L}(V))$.

Indeed, by (1), Aut$_e(\mathfrak{g}\mathfrak{l}(V))$ is contained in $\varphi (\mathbf{S}\mathbf{L}$(V)), and the opposite inclusion follows from Algebra, Chap. III, §8, no. 9, Prop. 17 and (1). An analogous argument shows that Aut$_e(\mathfrak{s}\mathfrak{l}(V))$ is the set of restrictions of elements of $\varphi (\mathbf{S}\mathbf{L}(V))$ to $\mathfrak{s}\mathfrak{l}(V)$.

### 2. CONJUGACY OF CARTAN SUBALGEBRAS

Let $\mathfrak{g}$ be a Lie algebra, $\mathfrak{h}$ a nilpotent subalgebra of $\mathfrak{g}$ and R the set of non-zero weights of $\mathfrak{h}$ in $\mathfrak{g}$, in other words the set of linear forms $\lambda \not= 0$ on $\mathfrak{h}$ such that $\mathfrak{g}^{\lambda}(\mathfrak{h})\not= 0$, cf. §1, no. 3, Prop. 9 (iii). Assume that

$$
\mathfrak{g}=\mathfrak{g}^0(\mathfrak{h})\oplus \sum_{\lambda\in R}\mathfrak{g}^{\lambda}(\mathfrak{h})
$$

which is the case if $k$ is algebraically closed (§1, no. 3, Prop. 9 (i)). For $\lambda \in R$ and $x\in \mathfrak{g}^{\lambda}(\mathfrak{h})$, ad $x$ is nilpotent (§1, no. 3, Prop. 10 (iv)). Denote by $E(\mathfrak{h})$ the subgroup of Aut$_e(\mathfrak{g})$ generated by the $e^{adx}$ where $x$ is of the form above. If $u\in$ Aut($\mathfrak{g}$), it is immediate that $uE(\mathfrak{h})u^{-1}= E(u(\mathfrak{h}))$.

#### Lemma 2 {#lie-vii-s3-lem-2 .statement tag=00V5}

(i) Let $\mathfrak{h}_r$ be the set of $x\in \mathfrak{h}$ such that $\mathfrak{g}^0(x) =\mathfrak{g}^0(\mathfrak{h})$; this is the set of $x\in \mathfrak{h}$ such that $\lambda (x)\not= 0$ for all $\lambda \in R$, and $\mathfrak{h}_r$ is open and dense in $\mathfrak{h}$ in the Zariski topology.

(ii) Put $R =\{\lambda_1, \lambda_2, . . . , \lambda_p\}$ where the $\lambda_i$ are mutually distinct. Let F be the map from $\mathfrak{g}^0(\mathfrak{h})\times \mathfrak{g}^{\lambda_1}(\mathfrak{h})\times  \cdots  \times \mathfrak{g}^{\lambda_p}(\mathfrak{h})$ to $\mathfrak{g}$ defined by the formula

$$
F(h, x_1, . . . , x_p) =e^{adx_1}. . . e^{adx_p}h
$$

Then F is a dominant polynomial map (App. I).

Assertion (i) is clear. We prove (ii). Let $n=$ dim $\mathfrak{g}$. If $\lambda \in R$ and $x\in \mathfrak{g}^{\lambda}(\mathfrak{h})$, we have (ad $x)^n= 0$. It follows that $(y, x) \rightarrow e^{adx}y$ is a polynomial map from $\mathfrak{g}\times \mathfrak{g}^{\lambda}(\mathfrak{h})$ to $\mathfrak{g}$; it follows by induction that F is polynomial. Let $h_0\in \mathfrak{h}_r$ and let DF be the tangent linear map of F at $(h_0,0, . . . ,0)$; we show that DF is surjective. For $h\in \mathfrak{g}^0(\mathfrak{h}), F(h_0+h,0, . . . ,0) =h_0+h$, so DF($h,0, . . . ,0$) $=h$ and Im(DF) $\supset \mathfrak{g}^0(\mathfrak{h})$. On the other hand, for $x\in \mathfrak{g}^{\lambda_1}(\mathfrak{h})$,

$_{adx}$ (ad $x)^2$

$F(h_0, x,0, . . . ,0) =eh_0=h_0+$ (ad $x).h_0+h_0+\cdots$

2!

so DF(0$, x,0, . . . ,0) =$ (ad $x).h_0=-$(ad $h_0)x$; since ad $h_0$ induces an automorphism of $\mathfrak{g}^{\lambda_1}(\mathfrak{h})$, Im(DF) $\supset \mathfrak{g}^{\lambda_1}(\mathfrak{h})$. Similarly,

Im(DF) $\supset \mathfrak{g}^{\lambda_i}(\mathfrak{h})$

for all $i$, hence the surjectivity of DF. Prop. 4 of App. I now shows that F is dominant.

#### Proposition 2 {#lie-vii-s3-prop-2 .statement tag=00V6}

Assume that $k$ is algebraically closed. Let $\mathfrak{g}$ be a Lie algebra, $\mathfrak{h}$ and $\mathfrak{h}'$ Cartan subalgebras of $\mathfrak{g}$. There exist $u\in E(\mathfrak{h})$ and $u'\in E(\mathfrak{h}')$ such that $u(\mathfrak{h}) =u'(\mathfrak{h}')$.

We retain the notation of Lemma 2. From the fact that $\mathfrak{h}$ and $\mathfrak{h}'$ are Cartan subalgebras, it follows that $\mathfrak{g}^0(\mathfrak{h}) =\mathfrak{h}$ and $\mathfrak{g}^0(\mathfrak{h}') =\mathfrak{h}'$. By Lemma 2 and Prop. 3 of App. $I, E(\mathfrak{h})\mathfrak{h}_r$ and $E(\mathfrak{h}')\mathfrak{h}'_r$ contain open dense subsets of $\mathfrak{g}$ in the Zariski topology. Thus $E(\mathfrak{h})\mathfrak{h}_r\cap E(\mathfrak{h}')\mathfrak{h}'_r\not=\emptyset$. In other words, there exist $u\in E(\mathfrak{h}), u'\in E(\mathfrak{h}'), h\in \mathfrak{h}_r, h'\in \mathfrak{h}'_r$ such that $u(h) =u'(h')$; then

$$
u(\mathfrak{h}) =u(\mathfrak{g}^0(\mathfrak{h})) =\mathfrak{g}^0(u(h)) =\mathfrak{g}^0(u'(h')) =u'(\mathfrak{h}')
$$

#### Corollary {#lie-vii-s3-n2-cor-1 .statement tag=00V7}

$E(\mathfrak{h}) = E(\mathfrak{h}')$.

Let $u, u'$ be as in Prop. 2. Then

$$
E(\mathfrak{h}) =uE(\mathfrak{h})u^{-1}= E(u(\mathfrak{h})) = E(u'(\mathfrak{h}')) =u'E(\mathfrak{h}')u^{'-1}= E(\mathfrak{h}')
$$

hence the corollary.

Because of this result, if $k$ is algebraically closed we shall denote simply by E the group $E(\mathfrak{h})$, where $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{g}$.

In general, Aut$_e(\mathfrak{g})\not= E$ (for example, if $\mathfrak{g}$ is nilpotent, E reduces to the identity element, even though non-trivial elementary automorphisms exist provided $\mathfrak{g}$ is non-commutative). However, it can be shown (Chap. VIII, §10, Exerc. 5) that Aut$_e(\mathfrak{g}) = E$ for $\mathfrak{g}$ semi-simple.

#### Theorem 1 {#lie-vii-s3-thm-1 .statement tag=00V8}

Assume that $k$ is algebraically closed. Let $\mathfrak{g}$ be a Lie algebra. The group E is normal in Aut($\mathfrak{g}$) and operates transitively on the set of Cartan subalgebras of $\mathfrak{g}$.

Let $\mathfrak{h}$ be a Cartan subalgebra of $\mathfrak{g}$, and $v\in$ Aut($\mathfrak{g}$). Then

$$
vE(\mathfrak{h})v^{-1}= E(v(\mathfrak{h})) = E(\mathfrak{h})
$$

so $E(\mathfrak{h}) = E$ is normal in Aut($\mathfrak{g}$). If $\mathfrak{h}'$ is another Cartan subalgebra of $\mathfrak{g}$, then, in the notation of Prop. $2,u^{'-1}u(\mathfrak{h}) =\mathfrak{h}'$, and $u^{'-1}u\in E$.

### 3. APPLICATIONS OF CONJUGACY

#### Theorem 2 {#lie-vii-s3-thm-2 .statement tag=00V9}

Let $\mathfrak{g}$ be a Lie algebra.

(i) The Cartan subalgebras of $\mathfrak{g}$ are all of the same dimension, namely rk($\mathfrak{g}$), and the same nilpotency class.

(ii) An element $x\in \mathfrak{g}$ is regular if and only if $\mathfrak{g}^0(x)$ is a Cartan subalgebra of $\mathfrak{g}$; every Cartan subalgebra is obtained in this way.

To prove (i), we can assume that $k$ is algebraically closed (cf. §2, Prop. 3 and Prop. 6), in which case it follows from Th. 1 of no. 2. Assertion (ii) follows from (i) and §2, Th. 1 (i) and (iv).

#### Proposition 3 {#lie-vii-s3-prop-3 .statement tag=00VA}

Let $\mathfrak{g}$ be a Lie algebra, $\mathfrak{g}'$ a subalgebra of $\mathfrak{g}$. The following conditions are equivalent:

(i) $\mathfrak{g}'$ contains a regular element of $\mathfrak{g}$, and rk($\mathfrak{g}$) $=$ rk($\mathfrak{g}'$);

(ii) $\mathfrak{g}'$ contains a Cartan subalgebra of $\mathfrak{g}$;

(iii) every Cartan subalgebra of $\mathfrak{g}'$ is a Cartan subalgebra of $\mathfrak{g}$.

(i) $=\Rightarrow$ (ii): Assume that rk($\mathfrak{g}$) $=$ rk($\mathfrak{g}'$), and that there exists $x\in \mathfrak{g}'$ regular in $\mathfrak{g}$. Put $\mathfrak{h}=\mathfrak{g}^0(x),\mathfrak{h}'={\mathfrak{g}'}^0(x) =\mathfrak{h}\cap \mathfrak{g}'$. Then

rk($\mathfrak{g}'$)$\leq$ dim$\mathfrak{h}'\leq$ dim$\mathfrak{h}=$ rk($\mathfrak{g}$) $=$ rk($\mathfrak{g}'$)

so $\mathfrak{h}=\mathfrak{h}'\subset \mathfrak{g}'$. This proves (ii).

(ii) $=\Rightarrow$ (iii): Assume that $\mathfrak{g}'$ contains a Cartan subalgebra $\mathfrak{h}$ of $\mathfrak{g}$, and let $\mathfrak{h}_1$ be a Cartan subalgebra of $\mathfrak{g}'$. To prove that $\mathfrak{h}_1$ is a Cartan subalgebra of $\mathfrak{g}$, we can assume that $k$ is algebraically closed. Let $E(\mathfrak{h})$ and $E'(\mathfrak{h})$ be the groups of automorphisms of $\mathfrak{g}$ and $\mathfrak{g}'$ associated to $\mathfrak{h}$ (no. 2). By Th. 1, there exists $f\in E'(\mathfrak{h})$ such that $f(\mathfrak{h}) =\mathfrak{h}_1$. Now every element of $E'(\mathfrak{h})$ is induced by an element of $E(\mathfrak{h})$; indeed, it suffices to verify this for $e^{adx}$, with $x\in {\mathfrak{g}'}^{\lambda}(\mathfrak{h}),\lambda \not= 0$, in which case it follows from the inclusion ${\mathfrak{g}'}^{\lambda}(\mathfrak{h})\subset \mathfrak{g}^{\lambda}(\mathfrak{h})$. Thus $\mathfrak{h}_1$ is a Cartan subalgebra of $\mathfrak{g}$.

(iii) $=\Rightarrow$ (i): Assume that condition (iii) is satisfied. Let $\mathfrak{h}$ be a Cartan subalgebra of $\mathfrak{g}'$. Since this is a Cartan subalgebra of $\mathfrak{g}$, it contains a regular element of $\mathfrak{g}$ (Th. 2 (ii)), and on the other hand rk($\mathfrak{g}$) $=$ dim($\mathfrak{h}$) $=$ rk($\mathfrak{g}'$).

#### Corollary {#lie-vii-s3-n3-cor-1 .statement tag=00VB}

Let $\mathfrak{h}$ be a nilpotent subalgebra of $\mathfrak{g}$. The subalgebra $\mathfrak{g}^0(\mathfrak{h})$ has properties (i), (ii), (iii) in Prop. 3.

Indeed, Prop. 11 of §2, no. 3, shows that $\mathfrak{g}^0(\mathfrak{h})$ has property (ii).

#### Proposition 4 {#lie-vii-s3-prop-4 .statement tag=00VC}

Let $\mathfrak{g}$ be a Lie algebra, $l$ the rank of $\mathfrak{g},c$ the nilpotency class of the Cartan subalgebras of $\mathfrak{g}$, and $x\in \mathfrak{g}$. There exists an $l$-dimensional subalgebra of $\mathfrak{g}$ whose nilpotency class is $\leq c$ and which contains $x$.

Let T be an indeterminate. Let $k'=k(T)$ and $\mathfrak{g}'=\mathfrak{g}\otimes_kk'$. If $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{g},\mathfrak{h}\otimes_kk'$ is a Cartan subalgebra of $\mathfrak{g}'$, hence the rank of $\mathfrak{g}'$ is $l$ and the nilpotency class of the Cartan subalgebras of $\mathfrak{g}'$ is $c$.

Choose a regular element $y$ of $\mathfrak{g}$. With the notations of §2, no. 2, we have $a_l(y)\not= 0$. Denote also by $a_l$ the polynomial function on $\mathfrak{g}'$ that extends $a_l$. Then the element $a_l(x+ Ty)$ of $k[T]$ has dominant coefficient $a_l(y)$. In particular, $x+ Ty$ is regular in $\mathfrak{g}'$. Let $\mathfrak{h}'$ be the nilspace of ad($x+ Ty$) in $\mathfrak{g}'$. Then dim $\mathfrak{h}'=l$ and the nilpotency class of $\mathfrak{h}'$ is $c$. Put $\mathfrak{k}=\mathfrak{h}'\cap (\mathfrak{g}\otimes_kk[T])$; then $\mathfrak{k}\otimes_{k[T]}k(T) =\mathfrak{h}'$.

Let $\varphi$ be the homomorphism from $k[T]$ to $k$ such that $\varphi (T) = 0$, and let $\psi$ be the homomorphism $1\otimes \varphi$ from $\mathfrak{g}\otimes_kk[T]$ to $\mathfrak{g}$. Then $\psi (\mathfrak{k})$ is a subalgebra of $\mathfrak{g}$ whose nilpotency class is $\leq c$ and which contains $\psi (x+ Ty) =x$.

In the free $k$[T]-module $\mathfrak{g}\otimes_kk[T],\mathfrak{k}$ is a submodule of rank $l$, and $(\mathfrak{g}\otimes_kk[T])/\mathfrak{k}$ is torsion free, so the submodule $\mathfrak{k}$ is a direct summand of $\mathfrak{g}\otimes_kk[T] ($Algebra, Chap. VII, §4, no. 2, Th. 1). Hence dim$_k\psi (\mathfrak{k}) =l$, which completes the proof.

### 4. CONJUGACY OF CARTAN SUBALGEBRAS OF SOLVABLE LIE ALGEBRAS

Let $\mathfrak{g}$ be a solvable Lie algebra. Denote by $\mathscr{C}^{\infty}(\mathfrak{g})$ the intersection of the terms of the descending central series of $\mathfrak{g}$ (Chap. I, §1, no. 5). This is a characteristic ideal of $\mathfrak{g}$, and is the smallest ideal $\mathfrak{m}$ of $\mathfrak{g}$ such that $\mathfrak{g}/\mathfrak{m}$ is nilpotent. Since $\mathscr{C}^{\infty}(\mathfrak{g})\subset [\mathfrak{g},\mathfrak{g}],\mathscr{C}^{\infty}(\mathfrak{g})$ is a nilpotent ideal of $\mathfrak{g}$ (Chap. I, §5, no. 3, Cor. 5 of Th. 1). By Prop. 1 of no. 1, the set of $e^{adx}$, for $x\in \mathscr{C}^{\infty}(\mathfrak{g})$, is a subgroup of Aut($\mathfrak{g}$) contained in the group of special automorphisms (Chap. I, §6, no. 8, Def. 6).

#### Theorem 3 {#lie-vii-s3-thm-3 .statement tag=00VD}

Let $\mathfrak{g}$ be a solvable Lie algebra, and let $\mathfrak{h},\mathfrak{h}'$ be Cartan subalgebras of $\mathfrak{g}$. There exists $x\in \mathscr{C}^{\infty}(\mathfrak{g})$ such that $e^{adx}\mathfrak{h}=\mathfrak{h}'$.

We argue by induction on dim$\mathfrak{g}$, the case where $\mathfrak{g}= 0$ being trivial. Let $\mathfrak{n}$ be a minimal non-zero commutative ideal of $\mathfrak{g}$. Let $\varphi :\mathfrak{g}\rightarrow \mathfrak{g}/\mathfrak{n}$ be the canonical morphism. Then $\varphi (\mathscr{C}^{\infty}\mathfrak{g}) =\mathscr{C}^{\infty}(\mathfrak{g}/\mathfrak{n})$ (Chap. I, §1, no. 5, Prop. 4). Since $\varphi (\mathfrak{h})$ and $\varphi (\mathfrak{h}')$ are Cartan subalgebras of $\mathfrak{g}/\mathfrak{n}($§2, no. 1, Cor. 2 of Prop. 4), there exists, by the induction hypothesis, an $x\in \mathscr{C}^{\infty}(\mathfrak{g})$ such that $e^{ad\varphi(x)}\varphi (\mathfrak{h}) =\varphi (\mathfrak{h}')$. Replacing $\mathfrak{h}$ by $e^{adx}\mathfrak{h}$, we can assume that $\varphi (\mathfrak{h}) =\varphi (\mathfrak{h}')$, in other words that

$$
\mathfrak{h}+\mathfrak{n}=\mathfrak{h}'+\mathfrak{n}
$$

Then $\mathfrak{h}$ and $\mathfrak{h}'$ are Cartan subalgebras of $\mathfrak{h}+\mathfrak{n}$. If $\mathfrak{h}+\mathfrak{n}\not=\mathfrak{g}$, the assertion to be proved follows from the induction hypothesis. Assume from now on that $\mathfrak{h}+\mathfrak{n}=\mathfrak{h}'+\mathfrak{n}=\mathfrak{g}$.

By the minimality of $\mathfrak{n}, [\mathfrak{g},\mathfrak{n}] =\{0\}$ or $[\mathfrak{g},\mathfrak{n}] =\mathfrak{n}$. If $[\mathfrak{g},\mathfrak{n}] =\{0\}$, then $\mathfrak{n}\subset \mathfrak{h}$ and $\mathfrak{n}\subset \mathfrak{h}'($§2, no. 1, Prop. 5), so $\mathfrak{h}=\mathfrak{h}+\mathfrak{n}=\mathfrak{h}'+\mathfrak{n}=\mathfrak{h}'$. It remains to consider the case where $[\mathfrak{g},\mathfrak{n}] =\mathfrak{n}$, so $\mathfrak{n}\subset \mathscr{C}^{\infty}(\mathfrak{g})$. The ideal $\mathfrak{n}$ is a simple $\mathfrak{g}$-module; since $\mathfrak{g}=\mathfrak{h}+\mathfrak{n}$, and since $[\mathfrak{n},\mathfrak{n}] =\{0\}$, it follows that $\mathfrak{n}$ is a simple $\mathfrak{h}$-module. If $\mathfrak{h}\cap \mathfrak{n}\not=\{0\}$, then $\mathfrak{n}\subset \mathfrak{h}$, so $\mathfrak{g}=\mathfrak{h}$ and $\mathfrak{h}'=\mathfrak{h}$. Assume now that $\mathfrak{h}\cap \mathfrak{n}=\{0\}$. Then $\mathfrak{g}=\mathfrak{h}\oplus \mathfrak{n}$ and hence $\mathfrak{g}=\mathfrak{h}'\oplus \mathfrak{n}$, since $\mathfrak{h}$ and $\mathfrak{h}'$ have the same dimension.

For all $x\in \mathfrak{h}$, let $f(x)$ be the unique element of $\mathfrak{n}$ such that $x-f(x)\in \mathfrak{h}'$; if $x, y\in \mathfrak{h}$,

$$
[x, y]-[x, f(y)]-[f(x), y] = [x-f(x), y-f(y)]\in \mathfrak{h}'
$$

so $f([x, y]) = [x, f(y)] + [f(x), y]$. By §1, no. 3, Cor. of Prop. 9, there exists $a\in \mathfrak{n}$ such that $f(x) = [x, a]$ for all $x\in \mathfrak{h}$. We have (ad $a)^2(\mathfrak{g})\subset$ (ad $a)(\mathfrak{n}) = 0$, so, for all $x\in \mathfrak{h}$,

$$
e^{ada}x=x+ [a, x] =x-f(x)
$$

Thus $e^{ada}(\mathfrak{h}) =\mathfrak{h}'$. Since $a\in \mathscr{C}^{\infty}(\mathfrak{g})$, this completes the proof.

#### Lemma 3 {#lie-vii-s3-lem-3 .statement tag=00VE}

Let $\mathfrak{g}$ be a Lie algebra, $\mathfrak{r}$ its radical, $\varphi$ the canonical homomorphism from $\mathfrak{g}$ to $\mathfrak{g}/\mathfrak{r},v$ an elementary automorphism of $\mathfrak{g}/\mathfrak{r}$. There exists an elementary automorphism $u$ of $\mathfrak{g}$ such that $\varphi \circ u=v\circ \varphi$.

We can assume that $v$ is of the form $e^{adb}$, where $b\in \mathfrak{g}/\mathfrak{r}$ and ad $b$ is nilpotent. Let $\mathfrak{s}$ be a Levi subalgebra of $\mathfrak{g}$ (Chap. I, §6, no. 8, Def. 7) and let $a$ be the element of $\mathfrak{s}$ such that $\varphi (a) =b$. Since ad$_{\mathfrak{s}}a$ is nilpotent, ad$_{\mathfrak{g}}a$ is nilpotent (Chap. I, §6, no. 3, Cor. of Prop. 3), and $u=e^{ad_{\mathfrak{g}}a}$ is an elementary automorphism of $\mathfrak{g}$ such that $\varphi \circ u=v\circ \varphi$.

#### Proposition 5 {#lie-vii-s3-prop-5 .statement tag=00VF}

Let $\mathfrak{g}$ be a Lie algebra, $\mathfrak{r}$ its radical, $\mathfrak{h}$ and $\mathfrak{h}'$ Cartan subalgebras of $\mathfrak{g}$, and $\varphi$ the canonical homomorphism from $\mathfrak{g}$ to $\mathfrak{g}/\mathfrak{r}$. The following conditions are equivalent:

(i) $\mathfrak{h}$ and $\mathfrak{h}'$ are conjugate by an elementary automorphism of $\mathfrak{g}$;

(ii) $\varphi (\mathfrak{h})$ and $\varphi (\mathfrak{h}')$ are conjugate by an elementary automorphism of $\mathfrak{g}/\mathfrak{r}$.

(i) $=\Rightarrow$ (ii): This is clear.

(ii) $=\Rightarrow$ (i): We assume that condition (ii) is satisfied and prove (i). By Lemma 3, we are reduced to the case where $\varphi (\mathfrak{h}) =\varphi (\mathfrak{h}')$. Put $\mathfrak{k}=$ $\mathfrak{h}+\mathfrak{r}=\mathfrak{h}'+\mathfrak{r}$, which is a solvable subalgebra of $\mathfrak{g}$. Then $\mathfrak{h}$ and $\mathfrak{h}'$ are Cartan subalgebras of $\mathfrak{k}$, so there exists $x\in \mathscr{C}^{\infty}(\mathfrak{k})$ such that $e^{ad_{\mathfrak{k}}x}\mathfrak{h}=\mathfrak{h}'$ (Th. 3). Since $\mathfrak{k}/\mathfrak{r}$ is nilpotent, $\mathscr{C}^{\infty}(\mathfrak{k})\subset \mathfrak{r}$; on the other hand, $\mathscr{C}^{\infty}(\mathfrak{k})\subset [\mathfrak{k},\mathfrak{k}]\subset [\mathfrak{g},\mathfrak{g}]$, so $x\in \mathfrak{r}\cap [\mathfrak{g},\mathfrak{g}]$; by Chap. I, §5, no. 3, Th. 1, ad$_{\mathfrak{g}}x$ is nilpotent, so $e^{ad_{\mathfrak{g}}x}$ is an elementary automorphism of $\mathfrak{g}$ transforming $\mathfrak{h}$ to $\mathfrak{h}'$.

### 5. LIE GROUP CASE

#### Proposition 6 {#lie-vii-s3-prop-6 .statement tag=00VG}

Assume that $k$ is $\mathbf{R},\mathbf{C}$ or a non-discrete complete ultrametric field of characteristic 0. Let $G$ be a finite dimensional Lie group over $k,e$ its identity element, $\mathfrak{g}$ its Lie algebra, $\mathfrak{h}$ a Cartan subalgebra of $\mathfrak{g},\mathfrak{h}_r$ the set of regular elements of $\mathfrak{g}$ belonging to $\mathfrak{h}$.

(i) Let $\mathfrak{s}$ be a vector space complement of $\mathfrak{h}$ in $\mathfrak{g},\mathfrak{s}_0$ a neighbourhood of 0 in $\mathfrak{s}$ on which an exponential map is defined, and $h_0\in \mathfrak{h}_r$. The map $(s, h) \rightarrow F(s, h) =$ (exp ad $s).h$ from $\mathfrak{s}_0\times \mathfrak{h}$ to $\mathfrak{g}$ is étale at $(0, h_0)$.

(ii) The map $(g, h) \rightarrow F'(g, h) =$ (Ad $g).h$ from $G\times \mathfrak{h}_r$ to $\mathfrak{g}$ is a submersion. In particular, its image $\Omega$ is open. For all $x\in \Omega ,\mathfrak{g}^0(x)$ is a Cartan subalgebra of $\mathfrak{g}$ conjugate to $\mathfrak{h}$ under Ad(G). $\bigcup$

(iii) Let $h_0\in \mathfrak{h}_r$. For any neighbourhood U of $e$ in G, the set $_{a\in U}$(Ad $a)(\mathfrak{h}_r)$

is a neighbourhood of $h_0$ in $\mathfrak{g}$.

Let $h_0$ and $\mathfrak{s}$ be as in (i). Let T be the tangent linear map of F at $(0, h_0)$. Then $F(0, h) =h$ for all $h\in \mathfrak{h}$, so $T(0, h) =h$ for all $h\in \mathfrak{h}$. On the other hand, for $\mathfrak{s}_0$ sufficiently small, the tangent linear map at 0 of the map $s \rightarrow$ exp ad $s$ from $\mathfrak{s}_0$ to End($\mathfrak{g}$) is the map $s \rightarrow$ ad $s$ from $\mathfrak{s}$ to End($\mathfrak{g}$). Thus $T(s,0) = [s, h_0]$ for all $s\in \mathfrak{s}$. Now the map from $\mathfrak{g}/\mathfrak{h}$ to $\mathfrak{g}/\mathfrak{h}$ induced by ad $h_0$ by passage to the quotient is bijective. It follows that T is bijective, hence (i). Since exp ad $s=$ Ad exp $s$ for all $s\in \mathfrak{s}$ sufficiently close to 0, (iii) and the first assertion of (ii) follow. Every $x\in \Omega$ is of the form (Ad $a)(h)$ with $a\in G$ and $h\in \mathfrak{h}_r$, so $\mathfrak{g}^0(x) =$ (Ad $a)(\mathfrak{g}^0(h)) =$ (Ad $a)(\mathfrak{h})$ is a subalgebra of $\mathfrak{g}$ conjugate to $\mathfrak{h}$ under Ad(G).

### Exercises {#lie-vii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
