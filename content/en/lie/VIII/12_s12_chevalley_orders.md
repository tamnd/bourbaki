---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 12
section_title: Chevalley orders
lang: en
source: lie-vii-ix
book_pages: 173-189
pdf_pages: 0181-0197
extraction: native
subsections:
    - "no": 1
      title: LATTICES AND ORDERS
      page: 173
      pdf_page: 181
    - "no": 2
      title: DIVIDED POWERS IN A BIGEBRA
      page: 173
      pdf_page: 181
    - "no": 3
      title: INTEGRAL VARIANT OF THE POINCARÉ-BIRKHOFF-WITT THEOREM
      page: 174
      pdf_page: 182
    - "no": 4
      title: 'EXAMPLE: POLYNOMIALS WITH INTEGER VALUES'
      page: 176
      pdf_page: 184
    - "no": 5
      title: SOME FORMULAS
      page: 178
      pdf_page: 186
    - "no": 6
      title: BIORDERS IN THE ENVELOPING ALGEBRA OF A SPLIT REDUCTIVE LIE ALGEBRA
      page: 180
      pdf_page: 188
    - "no": 7
      title: CHEVALLEY ORDERS
      page: 185
      pdf_page: 193
    - "no": 8
      title: ADMISSIBLE LATTICES
      page: 187
      pdf_page: 195
statements: 34
exercises: 0
content_sha256: 70a1fda9bcbbb0cd2eeac99519c309fa26bdd55024e115fc44209044500844e5
---

## § 12. CHEVALLEY ORDERS

### 1. LATTICES AND ORDERS

Let V be a $\mathbf{Q}$-vector space. A lattice in V is a free $\mathbf{Z}$-submodule $\mathscr{V}$ of V such that the $\mathbf{Q}$-linear map $\alpha_{\mathscr{V},V}:\mathscr{V}\otimes_{\mathbf{Z}}\mathbf{Q}\rightarrow V$ induced by the injection of $\mathscr{V}$ into V is bijective. When V is finite dimensional, this is the same as saying that $\mathscr{V}$ is a $\mathbf{Z}$-submodule of finite type which generates the $\mathbf{Q}$-vector space V (recall that a torsion-free $\mathbf{Z}$-module of finite type is free by Algebra, Chap. VII, §4, no. 4, Cor. 2); moreover, in this case our definition is a special case of that of Commutative Algebra, Chap. VII, §4, no. 1, Def. 1 (loc. cit., Example 3). If W is a vector subspace of V, and $\mathscr{V}$ is a lattice in V, then $\mathscr{V}\cap W$ is a lattice in W.

If V is a $\mathbf{Q}$-algebra, an order in V is a lattice $\mathscr{V}$ in the underlying vector space that is a $\mathbf{Z}$-subalgebra of V; the map $\alpha_{\mathscr{V},V}$ is then an isomorphism of $\mathbf{Q}$-algebras. If V is a unital $\mathbf{Q}$-algebra, a unital order in V is an order in V containing the unit element.

Assume that V is a $\mathbf{Q}$-bigebra, with coproduct $c$ and counit $\gamma$. If $\mathscr{V}$ is a lattice in the vector space V, the canonical map $i:\mathscr{V}\otimes_{\mathbf{Z}}\mathscr{V}\rightarrow V\otimes_{\mathbf{Q}}V$ is injective; a biorder in V is a unital order $\mathscr{V}$ in the unital algebra V such that $\gamma (\mathscr{V})\subset \mathbf{Z}$ and $c(\mathscr{V})\subset i(\mathscr{V}\otimes_{\mathbf{Z}}\mathscr{V})$; the maps

$\gamma_{\mathscr{V}}:\mathscr{V}\rightarrow \mathbf{Z}$ and $c_{\mathscr{V}}:\mathscr{V}\rightarrow \mathscr{V}\otimes_{\mathbf{Z}}\mathscr{V}$

induced by $\gamma$ and $c$ give $\mathscr{V}$ the structure of a $\mathbf{Z}$-bigebra, and the map $\alpha_{\mathscr{V},V}$ is then an isomorphism of $\mathbf{Q}$-bigebras.

### 2. DIVIDED POWERS IN A BIGEBRA

Let A be a unital $k$-algebra, $x\in A,d\in k,n\in \mathbf{N}$. Put

$$
x(x-d). . .(x-d(n-1))^{n-1}
$$

$$
x^{(n,d)}==\prod(x-id)/(i+ 1) \tag{1}
$$

$n$!

$i=0$

In particular, $x^{(0,d)}= 1,x^{(1,d)}=x$. We agree that $x^{(n,d)}= 0$ for $n$ an integer $<0$. Put

$x^{(n)}=x^{(n,0)}=xn^n$! (2)

$(nx)=x^{(n,1)}=x(x-1). . .n($!$x-n+ 1)$. (3)

#### Proposition 1 {#lie-viii-s12-prop-1 .statement tag=017V}

Let A be a bigebra, with coproduct $c$, and $x$ a primitive element (Chap. II, §1, no. 2) of A. Then

$$
c(x^{(n,d)}) =\sum x^{(p,d)}\otimes x^{(q,d)} \tag{4}
$$

$p\in \mathbf{N},q\in \mathbf{N},p+q=n$

The proposition is trivial for $n\leq 0$. We argue by induction on $n$. If formula (4) is true for $n$, then

$$
(n+ 1)c(x^{(n+1,d)}) =c(x-dn)c(x^{(n,d)})
$$

$$
= (x\otimes 1 + 1\otimes x-dn1\otimes 1)c(x^{(n,d)})
$$

$$
=\sum_{p+q=n}[xx^{(p,d)}\otimes x^{(q,d)}+x^{(p,d)}\otimes xx^{(q,d)}-(p+q)dx^{(p,d)}\otimes x^{(q,d)}]
$$

$$
=\sum_{p+q=n}(x-pd)x^{(p,d)}\otimes x^{(q,d)}+\sum_{p+q=n}x^{(p,d)}\otimes (x-qd)x^{(q,d)}
$$

$$
=\sum_{p+q=n}(p+ 1)x^{(p+1,d)}\otimes x^{(q,d)}+\sum_{p+q=n}(q+ 1)x^{(p,d)}\otimes x^{(q+1,d)}
$$

$$
=\sum_{r+s=n+1}rx^{(r,d)}\otimes x^{(s,d)}+\sum_{r+s=n+1}sx^{(r,d)}\otimes x^{(s,d)}
$$

$$
= (n+ 1)\sum_{r+s=n+1}x^{(r,d)}\otimes x^{(s,d)}
$$

hence formula (4) for $n+ 1$.

### 3. INTEGRAL VARIANT OF THE POINCARÉ-BIRKHOFF-WITT THEOREM

Let $\mathfrak{g}$ be a finite dimensional $\mathbf{Q}$-Lie algebra, $U(\mathfrak{g})$ its enveloping bigebra. If I is a totally ordered set, $\mathbf{x}= (x_i)_{i\in I}$ a family of elements of $\mathfrak{g}$, and $\mathbf{n}=$ $(n_i)_{i\in I}\in \mathbf{N}^{(I)}$ a multi-index, put

$\mathbf{x}^{(\mathbf{n})}=\prod x\overset{ni}{n_{i}}$!$^{^i}$, (5)

$i\in I$

the product being calculated in $U(\mathfrak{g})$ in accordance with the ordered set I.

#### Theorem 1 {#lie-viii-s12-thm-1 .statement tag=017W}

Let $\mathscr{U}$ be a biorder in the bigebra $U(\mathfrak{g})$. Let $\mathscr{G}=\mathscr{U}\cap \mathfrak{g}$, which is an order in the Lie algebra $\mathfrak{g}$. Let $(x_i)_{i\in I}$ be a basis of $\mathscr{G}$. Give I a total order, and assume that we are given, for all $\mathbf{n}\in \mathbf{N}^I$, an element $[\mathbf{n}]$ of $\mathscr{U}$ such that $[\mathbf{n}]-\mathbf{x}^{(\mathbf{n})}$ has filtration $<|\mathbf{n}|$ in $U(\mathfrak{g})$. Then, the family of the $[\mathbf{n}]$ for $\mathbf{n}\in \mathbf{N}^I$ is a basis of the $\mathbf{Z}$-module $\mathscr{U}$.

For $p\in \mathbf{N}$, let $U_p(\mathfrak{g})$ be the set of elements of $U(\mathfrak{g})$ of filtration $\leq p$; then the images in $U_p(\mathfrak{g})/U_{p-1}(\mathfrak{g})$ of the $\mathbf{x}^{(\mathbf{n})}$ such that $|\mathbf{n}|=p$ form a basis of this $\mathbf{Q}$-vector space (Chap. I, §2, no. 7, Th. 1); hence the $[\mathbf{n}]$ form a basis of the $\mathbf{Q}$-vector space $U(\mathfrak{g})$. It remains to prove the following assertion (in which we put $M =\mathbf{N}^I):$

(*) if $u\in \mathscr{U}, (a_{\mathbf{n}})\in \mathbf{Z}^{(M)}$, and $d\in$ **N --**$\{0\}$ are such that

$$
du=\sum_{\mathbf{n}\in M}a_{\mathbf{n}}[\mathbf{n}] \tag{6}
$$

then $d$ divides each $a_{\mathbf{n}}$.

For each integer $r\geq 0$, introduce the iterated coproduct

$$
c_i:\mathscr{U}\rightarrow \mathbf{T}^r(\mathscr{U}) =\mathscr{U}\otimes \mathscr{U}\otimes  \cdots  \otimes \mathscr{U}
$$

by definition, $c_0$ is the counit of $\mathscr{U},c_1=$ Id$_{\mathscr{U}},c_2=c$ (the coproduct of $\mathscr{U})$, and, for $r\geq 2,c_{r+1}$ is defined as the composite $p\circ (c_r\otimes 1)\circ c:$

$$
\mathscr{U}\longrightarrow^c\mathscr{U}\otimes_{\mathbf{Z}}\mathscr{U}^c\longrightarrow^{^r\otimes 1}\mathbf{T}^r(\mathscr{U})\otimes_{\mathbf{Z}}\mathscr{U}\longrightarrow^p\mathbf{T}^{r+1}(\mathscr{U})
$$

where $p$ is defined by using the multiplication in the algebra $\mathbf{T}(\mathscr{U})$. Further, consider the canonical projection $\pi$ of $\mathscr{U}$ onto $\mathscr{U}^+=$ Ker $c_0$, and the composite

$$
c^+_r=\mathbf{T}^r(\pi )\circ c_r:\mathscr{U}\rightarrow \mathbf{T}^r(\mathscr{U}^+)
$$

#### Lemma 1 {#lie-viii-s12-lem-1 .statement tag=017X}

Let $\mathbf{n}\in \mathbf{N}^I$. If $|\mathbf{n}|< r$, then $c^+_r([\mathbf{n}]) = 0$. If $|\mathbf{n}|=r$, then

$$
c^+_r([\mathbf{n}]) =\sum_{\varphi}x_{\varphi(1)}\otimes x_{\varphi(2)}\otimes  \cdots  \otimes x_{\varphi(r)} \tag{7}
$$

where $\varphi$ belongs to the set of maps from $\{1,2, . . . , r\}$ to I which take each value $i\in In_i$ times.

By Prop. 1,

$$
c_r(\mathbf{x}^{(\mathbf{n})}) =\sum\mathbf{x}^{(\mathbf{p}_1)}\otimes  \cdots  \otimes \mathbf{x}^{(\mathbf{p}_r)}
$$

where the summation extends over the set of sequences $(\mathbf{p}_1, . . . ,\mathbf{p}_r)$ of $r$ elements of M such that $\mathbf{p}_1+\cdots +\mathbf{p}_r=\mathbf{n}$. In view of Chap. II, §1, no. 3, Prop. 6, the map $c^+_r$, extended by linearity to a map from $U(\mathfrak{g})$ to $\mathbf{T}^r(U^+(\mathfrak{g}))$, vanishes on $U_{r-1}(\mathfrak{g})$. It follows that, for $r\geq  |\mathbf{n}|$,

$$
c^+_r([\mathbf{n}]) =c^+_r(\mathbf{x}^{(\mathbf{n})}) =\sum\pi (\mathbf{x}^{(\mathbf{p}_1)})\otimes  \cdots  \otimes \pi (\mathbf{x}^{(\mathbf{p}_r)}) \tag{8}
$$

For $r >|\mathbf{n}|$, the relation $\mathbf{p}_1+\cdots +\mathbf{p}_r=\mathbf{n}$ implies that at least one of the $\mathbf{p}_i$ is zero, so $c^+_r([\mathbf{n}]) = 0$. For $r=|\mathbf{n}|$, the only non-zero terms of the third member of (8) are those for which $|\mathbf{p}_1|=\cdots =|\mathbf{p}_r|= 1$, hence (7).

We return to the proof of Th. 1. We retain the notations of (*) and prove, by descending induction on $|\mathbf{n}|$, that $d$ divides $a_{\mathbf{n}}$, which is clear when $|\mathbf{n}|$ is sufficiently large. If $d$ divides $a_{\mathbf{n}}$ for $|\mathbf{n}|> r$ then, putting

$$
u'=u-\sum_{|\mathbf{n}|>r}(a_{\mathbf{n}}/d)[\mathbf{n}]\in \mathscr{U}
$$

we have

$$
du'=\sum_{|\mathbf{n}|\leq r}a_{\mathbf{n}}[\mathbf{n}] \tag{9}
$$

For any map $\varphi$ from $\{1,2, . . . , r\}$ to I, put

$$
e_{\varphi}=x_{\varphi(1)}\otimes  \cdots  \otimes x_{\varphi(r)}
$$

and $a_{\varphi}=a_{\mathbf{n}}$ where $\mathbf{n}=$ (Card$\varphi^{-1}(i))_{i\in I}$. By Lemma 1, (9) implies that

$$
dc^+_r(u') =\sum_{\varphi\in I^r}a_{\varphi}e_{\varphi} \tag{10}
$$

so $c^+_r(u')\in \mathbf{T}^r(\mathscr{U}^+)\cap \mathbf{Q}\mathbf{T}^r(\mathscr{G})$. But the submodule $\mathscr{G}$ of $\mathscr{U}^+$ is a direct factor (Algebra, Chap. VII, §4, no. 3, Cor. of Th. 1), so the submodule $\mathbf{T}^r(\mathscr{G})$ is a direct factor of $\mathbf{T}^r(\mathscr{U}^+)$, and hence $c^+_r(u')\in \mathbf{T}^r(\mathscr{G})$. On the other hand, the $x_i$ form a basis of $\mathscr{G}$ by hypothesis, so the $e_{\varphi}$ form a basis of $\mathbf{T}^r(\mathscr{G})$. Then (10) proves that $d$ divides the $a_{\varphi}$, that is, the $a_{\mathbf{n}}$ for $|\mathbf{n}|=r$. This proves (*).

### 4. EXAMPLE: POLYNOMIALS WITH INTEGER VALUES

Let V be a finite dimensional $\mathbf{Q}$-vector space, $V^*$ its dual, $\mathscr{V}$ a lattice in V, $\mathscr{V}^*$ the dual $\mathbf{Z}$-module of $\mathscr{V}$, which can be identified canonically with a lattice in $V^*,\mathbf{S}(V)$ the symmetric algebra of V, and

$$
\lambda :\mathbf{S}(V)\rightarrow A(V^*)
$$

the canonical bijection from $\mathbf{S}(V)$ to the algebra of polynomial functions on $V^*($Algebra, Chap. IV, §5, no. 11, Remark 1). If we identify $A(V^*\times V^*)$ with $A(V^*)\otimes_{\mathbf{Q}}A(V^*)$, then $\lambda$ transforms the coproduct of $\mathbf{S}(V)$ into the map $A(V^*)\rightarrow A(V^*\times V^*)$ which associates to the polynomial function $\varphi$ on $V^*$ the polynomial function

$$
(x, y) \rightarrow \varphi (x+y)
$$

on $V^*\times V^*($Algebra, Chap. IV, §5, no. 11, Remark 2).

Denote by $(^{\mathscr{V}}_{\mathbf{Z}})$ the subset of $\mathbf{S}(V)$ consisting of the elements which correspond to polynomial maps from $V^*$ to $\mathbf{Q}$ that take integer values on $\mathscr{V}^*$.

#### Proposition 2 {#lie-viii-s12-prop-2 .statement tag=017Y}

(i) $(^{\mathscr{V}}_{\mathbf{Z}})$ is a biorder in the bigebra $\mathbf{S}(V)$, and $(^{\mathscr{V}}_{\mathbf{Z}})\cap V =\mathscr{V}$.

(ii) The $\mathbf{Z}$-algebra $(^{\mathscr{V}}_{\mathbf{Z}})$ is generated by the $(^h_n)$ for $h\in \mathscr{V}, n\in \mathbf{N}$.

(iii) If $(h_1, . . . , h_r)$ is a basis of $\mathscr{V}$, the elements

$$
(h)(h_1)(h_r)
$$

= $\cdots$,

$$
\mathbf{n}n_1n_r
$$

where $\mathbf{n}= (n_1, . . . , n_r)$ belongs to $\mathbf{N}^r$, form a basis of the $\mathbf{Z}$-module $(^{\mathscr{V}}_{\mathbf{Z}})$.

For $m\in \mathbf{N}$, put $\mathbf{S}_m(V) =\sum_{i\leq m}\mathbf{S}^i$(V), $\mathbf{S}_m(\mathscr{V}) =\sum_{i\leq m}\mathbf{S}^i(\mathscr{V})$. By Algebra, Chap. IV, §5, no. 9, Prop. 15 and Remark,

$\mathbf{S}_m(\mathscr{V})\subset \mathbf{S}_m(V)\cap (\mathscr{V}\mathbf{Z})\subset m1$!$\mathbf{S}_m(\mathscr{V})$

so $(^{\mathscr{V}}_{\mathbf{Z}})\cap V =\mathscr{V}$. Since $\mathbf{S}_m(\mathscr{V})$ is a lattice in $\mathbf{S}_m$(V), $\mathbf{S}_m(V)\cap (_{\mathbf{Z}}^{\mathscr{V}})$ is also a lattice in $\mathbf{S}_m(V)$. On the other hand, $\mathbf{S}_m(V)\cap (^{\mathscr{V}}_{\mathbf{Z}})$ is a direct factor of $\mathbf{S}_{m+1}(V)\cap (_{\mathbf{Z}}^{\mathscr{V}})$ (since the quotient is torsion-free), hence it admits a complement which is a free $\mathbf{Z}$-module. It follows that $(^{\mathscr{V}}_{\mathbf{Z}})$ is a free $\mathbf{Z}$-module. It is clear that this is a unital order in the algebra $\mathbf{S}(V)$. Let $(u_n)_{n\in\mathbf{N}}$ be a basis of the $\mathbf{Z}$-module $(^{\mathscr{V}}_{\mathbf{Z}})$. This is also a basis of the $\mathbf{Q}$-module $\mathbf{S}(V)$ and, for all

$$
\varphi \in \mathbf{S}(V\times V) =\mathbf{S}(V)\otimes_{\mathbf{Q}}\mathbf{S}(V)
$$

there exists a unique sequence $(v_n)$ of elements of $\mathbf{S}(V)$ such that $\varphi =\sum u_n\otimes v_n$. As above, identify $\mathbf{S}(V)$ with $A(V^*)$ and $\mathbf{S}(V)\otimes \mathbf{S}(V)$ with $A(V^*\times V^*)$. If $\varphi \in (^{\mathscr{V}\times\mathscr{V}}_{\mathbf{Z}})$, the polynomial function $x \rightarrow \varphi (x, y)$ belongs to $(^{\mathscr{V}}_{\mathbf{Z}})$ for all $y\in \mathscr{V}^*$. It follows that $v_n(y)\in \mathbf{Z}$ for all $n$ and all $y\in \mathscr{V}^*$, in other words that $v_n\in (^{\mathscr{V}}_{\mathbf{Z}})$. This proves that the coproduct maps $(^{\mathscr{V}}_{\mathbf{Z}})$ to $(_{\mathbf{Z}}^{\mathscr{V}})\otimes_{\mathbf{Z}}(_{\mathbf{Z}}^{\mathscr{V}})$. If $h\in \mathscr{V}$ and $n\in \mathbf{N}$, then $(_n^h)$ maps $u\in \mathscr{V}^*$ to the integer $(^{u(h)}_n)$, so $(^h_n)\in (_{\mathbf{Z}}^{\mathscr{V}})$. Assertion (iii) is now obtained by applying Th. 1 to the commutative Lie algebra V, and (ii) follows.

#### Corollary {#lie-viii-s12-n4-cor-1 .statement tag=017Z}

Let X be an indeterminate. The polynomials $(^X_n)$, where $n\in \mathbf{N}$, form a basis of the $\mathbf{Z}$-module consisting of the polynomials $P\in k[X]$ such that $P(\mathbf{Z})\subset \mathbf{Z}$.

If $P(\mathbf{Z})\subset \mathbf{Z}$, the Lagrange interpolation formula (Algebra, Chap. IV, §2, no. 1, Prop. 6) shows that the coefficients of P belong to $\mathbf{Q}$; thus, we can assume that $k=\mathbf{Q}$ and apply Prop. 2 with $V =\mathbf{Q},\mathscr{V}=\mathbf{Z}$.

### 5. SOME FORMULAS

In this number, A denotes a unital associative algebra. If $x\in A$, we write ad $x$ instead of ad$_Ax$.

#### Lemma 2 {#lie-viii-s12-lem-2 .statement tag=0180}

If $x, y\in A$ and $n\in \mathbf{N}$,

(ad$nx$! $)^ny=\sum(-1)^qxp^p$! $yxq^q$! = $\sum(-1)^qx^{(p)}yx^{(q)}$. (11)

$p+q=np+q=n$

Indeed, if we denote by $L_x$ and $R_x$ the maps $z \rightarrow xz$ and $z \rightarrow zx$ from A to A, we have, since $L_x$ and $R_x$ commute,

$n1$!(ad $x)^n=n1$!$(L_x-R_x)^n=\sum_{p+q=n}(-1)^qp1$! $L^p_xq1$! $R^q_x$.

#### Lemma 3 {#lie-viii-s12-lem-3 .statement tag=0181}

Let $x, h\in A$ and $\lambda \in k$ be such that (ad $h)x=\lambda x$. For all $n\in \mathbf{N}$, and all $P\in k[X]$, we have

$$
P(h)x^{(n)}=x^{(n)}P(h+n\lambda ) \tag{12}
$$

Since ad $h$ is a derivation of A and since (ad $h)x$ commutes with $x$, we have

(ad $h)x^n=nx^{n-1}$((ad $h)x) =n\lambda x^n$, (13) so

(ad $h)x^{(n)}=n\lambda x^{(n)}$.

Thus, formula (12) follows from the special case

$$
P(h)x=xP(h+\lambda ) \tag{14}
$$

by replacing $x$ by $x^{(n)}$ and $\lambda$ by $n\lambda$. It suffices to prove (14) when $P = X^m$, by induction on $m$. It is clear when $m= 0,1$. If (14) is true for $P = X^m$, then

$$
h^{m+1}x=h.h^mx=hx(h+\lambda )^m=x(h+\lambda )^{m+1}
$$

which proves (12).

#### Lemma 4 {#lie-viii-s12-lem-4 .statement tag=0182}

Let $x, y, h\in A$ be such that

$$
[y, x] =h,[h, x] = 2x,[h, y] =-2y \tag{15}
$$

(i) For $m, n\in \mathbf{N}$, we have

$$
_{(n)(m)}\sum_{(m-p)}(m+n-p-1-h)_{(n-p)}
$$

$xy$ = $yx$. (16)

$$
p
$$

$p\geq 0$

(ii) Let $A'$ be the $\mathbf{Z}$-subalgebra of A generated by the $x^{(m)}$ and the $y^{(m)}$ for $m\in \mathbf{N}$. Then $(^h_n)\in A'$ for all $n\in \mathbf{N}$.

Formula (16) can be written in the equivalent form

$$
_{(n)(m)}\sum_{(m-p)}(m+n-p-1-h)_{(n-p)}
$$

(ad $x)y$ = $yx.(17_m)$

$$
p
$$

$p\geq 1$

This is trivial for $m= 0$. We argue by induction on $m$. From $(17_m)$, we obtain

$(m+$ 1)(ad $x^{(n)})y^{(m+1)}=$ (ad $x^{(n)})y^{(m)}.y+y^{(m)}$.(ad $x^{(n)})y$ (18)

$$
_{(m-p)}(m+n-p-1-h)_{(n-p)(m)}-
$$

$$
=\sum yxy+y(n-1-h)x^{(n1)}
$$

$$
p
$$

$p\geq 1$

(§1, no. 1, Lemma 1). Now, applying the same lemma, and then Lemma 3,

we have

$$
(m+n-p-1-h)_{(n-p)}
$$

$$
xy
$$

$$
p
$$

$$
(m+n-p-1-h)_{(n-p)}-_-
$$

= $(yx+ (n-p-1-h)x^{(np1)})$

$$
p
$$

$$
(m+n-p+ 1-h)_{(n-p)}
$$

$$
=yx
$$

$$
p
$$

$$
(m+n-p-1-h)_{--}
$$

+ $(n-p-1-h)x^{(np1)}$.

$$
p
$$

Inserting this into (18), we obtain

$(m+$ 1)(ad $x^{(n)})y^{(m+1)}$

$$
_-(m+n-p+ 1-h)_-
$$

$$
=\sum(m-p+ 1)y^{(mp+1)}x^{(np)}
$$

$$
p
$$

$p\geq 1$

$$
_-(m+n-p-1-h)_{--}
$$

$+\sum y^{(mp)}(n-p-1-h)x^{(np1)}$

$$
p
$$

$p\geq 1$

$$
+y^{(m)}(n-1-h)x^{(n-1)}
$$

$$
_-(m+n-p+ 1-h)_-
$$

$=\sum(m-p+ 1)y^{(mp+1)}x^{(np)}$

$$
p
$$

$p\geq 1$

$$
_{(m-p)}(m+n-p-1-h)_{--}
$$

$+\sum y(n-p-1-h)x^{(np1)}$.

$$
p
$$

$p\geq 0$ Changing $p$ to $p-1$ in the second sum, and regrouping the terms, we obtain

$(m+$ 1)(ad $x^{(n)})y^{(m+1)}=\sum_{p\geq 1}y^{(m-p+1)}A_px^{(n-p)}$ (19)

with

$$
(m+n-p+ 1-h)(m+n-p-h)
$$

$A_p= (m-p+ 1)+ (n-p-h)$.

$$
pp-1
$$

Putting $z=m+n-p-h$, this can also be written as

$A_p=p1$!$(m-p+ 1)(z+ 1)z(z-1). . .(z-p+ 2)$

+ 1 $(z-m)z(z-1). . .(z-p+ 2)$

$(p-$ 1)!

$=p1$! $z(z-1). . .(z-p+ 2)[(m-p+ 1)(z+ 1) +p(z-m)]$

$$
(z)((m+ 1) +n-p-1-h)
$$

$$
= (m+ 1)= (m+ 1)
$$

$$
pp
$$

Inserting this into (19), we obtain $(17_{m+1})$, hence (i).

Assume that $(^h_p)\in A'$ for $p < n$. Then, for all $P\in \mathbf{Q}[T]$ of degree $< n$ such that $P(\mathbf{Z})\subset \mathbf{Z}$, we have $P(h)\in A'$ (no. 4, Cor. of Prop. 2). Hence, in view of (16) with $m=n$,

$$
(h)(n-1-h)
$$

$(-1)^n$ =

$$
nn
$$

$$
^{n-1}_-(2n-p-1-h)_-'
$$

$=-x^{(n)}y^{(n)}+\sum y^{(np)}x^{(np)}\in A$ ;

$$
p
$$

$p=0$

hence (ii) by induction on $n$.

### 6. BIORDERS IN THE ENVELOPING ALGEBRA OF A SPLIT REDUCTIVE LIE ALGEBRA

Let $\mathfrak{g}$ be a reductive Lie algebra over $\mathbf{Q},\mathfrak{h}$ a splitting Cartan subalgebra of $\mathfrak{g}$, and $R = R(\mathfrak{g},\mathfrak{h}) ($§2, no. 1, Remark 5).

#### Definition 1 {#lie-viii-s12-def-1 .statement tag=0183}

A lattice $\mathscr{H}$ in $\mathfrak{h}$ is said to be permissible (relative to $\mathfrak{g})$ if, for all $\alpha \in R$, we have $H_{\alpha}\in \mathscr{H}$ and $\alpha (\mathscr{H})\subset \mathbf{Z}$.

#### Remark 1 {#lie-viii-s12-n6-rem-1 .statement tag=0184}

Let B be a basis of R. A lattice $\mathscr{H}$ in $\mathfrak{h}$ is permissible if and only if $H_{\alpha}\in \mathscr{H}$ and $\alpha (\mathscr{H})\subset \mathbf{Z}$ for all $\alpha \in B$.

#### Remark 2 {#lie-viii-s12-n6-rem-2 .statement tag=0185}

Let $\mathfrak{c}$ be the centre of $\mathfrak{g}$. Then, a lattice $\mathscr{H}$ in $\mathfrak{h}$ is permissible if and only if $Q(R^{\vee})\subset \mathscr{H}\subset P(R^{\vee})\oplus \mathfrak{c}$. The lattice $\mathscr{H}\cap \mathscr{D}\mathfrak{g}$ is then permissible in the Cartan subalgebra $\mathfrak{h}\cap \mathscr{D}\mathfrak{g}$ of $\mathscr{D}\mathfrak{g}$. There may exist permissible lattices $\mathscr{H}$ such that $\mathscr{H}\not= (\mathscr{H}\cap \mathscr{D}\mathfrak{g})\oplus (\mathscr{H}\cap \mathfrak{c})$ (cf. §13, no. 1.IX).

#### Remark 3 {#lie-viii-s12-n6-rem-3 .statement tag=0186}

If $\mathfrak{g}$ is semi-simple, the permissible lattices in $\mathfrak{h}$ are the subgroups $\mathscr{H}$ of $\mathfrak{h}$ such that $Q(R^{\vee})\subset \mathscr{H}\subset P(R^{\vee})$.

In the remainder of this number, we assume fixed a split reductive Lie algebra $(\mathfrak{g},\mathfrak{h})$, a basis B of $R = R(\mathfrak{g},\mathfrak{h})$ and, for each $\alpha \in B$, a pair $(x_{\alpha}, y_{\alpha})$ with

$$
y_{\alpha}\in \mathfrak{g}^{-\alpha},x_{\alpha}\in \mathfrak{g}^{\alpha},[y_{\alpha}, x_{\alpha}] =H_{\alpha} \tag{20}
$$

If we denote by $\mathfrak{n}_+$ (resp. $\mathfrak{n}_-)$ the subalgebra of $\mathfrak{g}$ generated by the $x_{\alpha}$ (resp. the $y_{\alpha})$, we know (§3, no. 3, Prop. 9 (iii)) that

$$
\mathfrak{g}=\mathfrak{n}_-\oplus \mathfrak{h}\oplus \mathfrak{n}_+ \tag{21}
$$

$$
U(\mathfrak{g}) = U(\mathfrak{n}_-)\otimes_{\mathbf{Q}}U(\mathfrak{h})\otimes_{\mathbf{Q}}U(\mathfrak{n}_+) \tag{22}
$$

(where $U(\mathfrak{g}), . .$. are the enveloping algebras of $\mathfrak{g}, . . .)$.

Denote by $\mathscr{U}_+$ the $\mathbf{Z}$-subalgebra of $U(\mathfrak{n}_+)$ generated by the $x^{(n)}_{\alpha}$ for $\alpha \in B$ and $n\in \mathbf{N}$. Let W be the Weyl group of $R, R_+$ the set of positive roots relative to B.

#### Lemma 5 {#lie-viii-s12-lem-5 .statement tag=0187}

(i) $\mathscr{U}_+$ is a lattice in the vector space $U(\mathfrak{n}_+)$.

(ii) For all $\alpha \in B$, we have $\mathscr{U}_+\cap U(\mathfrak{g}^{\alpha}) =\bigoplus_{n\in\mathbf{N}}\mathbf{Z}x^{(n)}_{\alpha}$.

By definition, $\mathscr{U}_+$ is generated as a $\mathbf{Z}$-module by the elements

$x(\varphi \mathbf{n})$ = $1\leq \prod i\leq rx(\varphi n((ii)$))

where $r\in \mathbf{N},\varphi = (\varphi (i))\in B^r$, and $\mathbf{n}= (n(i))\in \mathbf{N}^r$. Give the algebra $U(\mathfrak{n}_+)$ the graduation of type Q(R) for which each $\mathfrak{g}^{\alpha}(\alpha \in R_+)$ is homogeneous of degree $\alpha$. A monomial $x^{(\mathbf{n})}_{\varphi}$ of the preceding type is homogeneous of degree

$$
\sum_{1\leq i\leq r}n(i)\varphi (i)\in Q(R)
$$

The monomials of this kind having a given degree $q$ are finite in number, and generate over $\mathbf{Q}$ the homogeneous component of $U(\mathfrak{n}_+)$ of degree $q$. This proves (i).

If $\alpha \in B,\mathscr{U}_+\cap U(\mathfrak{g}^{\alpha})$ is contained in the sum of the homogeneous components of degrees which are multiples of $\alpha$; thus, by the preceding, $\mathscr{U}_+\cap U(\mathfrak{g}^{\alpha})$ is generated by the $x^{(\mathbf{n})}_{\varphi}$ such that $\sum n(i)\varphi (i)\in \mathbf{N}\alpha$, which forces $\varphi (i) =\alpha$ for all $i$ (since B is a basis of R), so

$x^{(\mathbf{n})}_{\varphi}=x^{(n(1))}_{\alpha}. . . x^{(n(r))}_{\alpha}=(n(1) +n$(1)!$\cdots . . . n+(nr$)!$(r$))! $x^{(n(1)+\cdot \cdot \cdot+n(r))}_{\alpha}$.

Thus, $\mathscr{U}_+\cap \mathscr{U}(\mathfrak{g}^{\alpha})\subset \bigoplus_n\mathbf{Z}x^{(n)}_{\alpha}$, hence (ii). Q.E.D.

In the remainder of this paragraph, if E and F are $\mathbf{Z}$-submodules of $U(\mathfrak{g})$, we denote by $E.F$ the $\mathbf{Z}$-submodule of $U(\mathfrak{g})$ generated by the products $ab$, where $a\in E, b\in F$.

#### Proposition 3 {#lie-viii-s12-prop-3 .statement tag=0188}

Let $\mathscr{H}$ be a permissible lattice in $\mathfrak{h}$. Let $\mathscr{U}_+,\mathscr{U}_-,\mathscr{U}_0$ be the $\mathbf{Z}$-subalgebras of $U(\mathfrak{g})$ generated respectively by the elements $x_{\alpha}^{(n)}$ $(\alpha \in B,n\in \mathbf{N}),y_{\alpha}^{(n)}(\alpha \in B, n\in \mathbf{N}),(^h_n)(h\in \mathscr{H}, n\in \mathbf{N})$. Let $\mathscr{U}$ be the $\mathbf{Z}$-subalgebra of $U(\mathfrak{g})$ generated by $\mathscr{U}_+,\mathscr{U}_-,\mathscr{U}_0$.

(i) $\mathscr{U}$ is a biorder in the bigebra $U(\mathfrak{g})$.

(ii) We have $\mathscr{U}=\mathscr{U}_-.\mathscr{U}_0.\mathscr{U}_+,\mathscr{U}\cap \mathfrak{h}=\mathscr{H}$ and, for all $\alpha \in B$,

$$
\mathscr{U}\cap \mathfrak{g}^{\alpha}=\mathbf{Z}x_{\alpha},V\cap \mathfrak{g}^{-\alpha}=\mathbf{Z}y_{\alpha}
$$

By Lemma 5 and Prop. $2,\mathscr{U}_+,\mathscr{U}_-,\mathscr{U}_0$ are orders in the $\mathbf{Q}$-algebras $U(\mathfrak{n}_+),U(\mathfrak{n}_-),U(\mathfrak{h})$, respectively, and

$$
(\pm h+q)
$$

$\in \mathscr{U}_0$ for $h\in \mathscr{H}, q\in \mathbf{Z}, p\in \mathbf{N}$. (23)

$$
p
$$

Put $\mathscr{L}=\mathscr{U}_-.\mathscr{U}_0.\mathscr{U}_+\subset U(\mathfrak{g})$. By (22), $\mathscr{L}$ is a lattice in $U(\mathfrak{g})$. By construction,

$$
\mathscr{U}_-.\mathscr{L}\subset \mathscr{L} \tag{24}
$$

$$
\mathscr{L}.\mathscr{U}_+\subset \mathscr{L} \tag{25}
$$

while Lemma 3 and (23) imply that

$$
\mathscr{U}_0.\mathscr{L}\subset \mathscr{L} \tag{26}
$$

$$
\mathscr{L}.\mathscr{U}_0\subset \mathscr{L} \tag{27}
$$

Let $\alpha \in B, n\in \mathbf{N}, r\in \mathbf{N}, \varphi = (\varphi (i))\in B^r$, and

$$
(m(1), . . . , m(r))\in \mathbf{N}^r
$$

We show that

$$
x^{(n)}_{\alpha}y_{\varphi(1)}^{(m(1))}. . . y_{\varphi(r)}^{(m(r))}\in \mathscr{L} \tag{28}
$$

or equivalently, in view of (25), that

$$
[x^{(n)}_{\alpha}, y^{(m(1))}_{\varphi(1)}. . . y_{\varphi(r)}^{(m(r))}]\in \mathscr{L} \tag{29}
$$

We argue by induction on $r$. The bracket to be studied is the sum of the terms

$(m(1))(m(k))(n)(m(k+1))(m(k+2))(m(r))$

$y_{\varphi(1)}. . . y_{\varphi(k)}[x_{\alpha}, y_{\varphi(k+1)}]y_{\varphi(k+2)}. . . y_{\varphi(r)}$. (30) For $\alpha \not=\varphi (k+ 1),x_{\alpha}$ and $y_{\varphi(k+1)}$ commute, so $[x^{(n)}_{\alpha}, y^{(m(k+1))}_{\varphi(k+1)}] = 0$. If $\alpha =\varphi (k+ 1)$, the expression (30) is, by (17), the sum of expressions of the form

$(m(1))(m(k))(m(k+1)-p)(q-h)(n-p)(m(k+2))(m(r))$

$$
y_{\varphi(1)}. . . y_{\varphi(k)}y_{\varphi(k+1)}x_{\alpha}y_{\varphi(k+2)}. . . y_{\varphi(r)} \tag{31}
$$

$$
p
$$

where $q\in \mathbf{Z}, p\in$ **N --** $\{0\}, h\in \mathscr{H}$. The induction hypothesis, together with (24) and (26), proves that the expression (31) belongs to $\mathscr{L}$. We have thus proved (28).

By (28), $x^{(n)}_{\alpha}\mathscr{U}_-\subset \mathscr{L}$; thus, by (25) and (27), $x^{(n)}_{\alpha}\mathscr{L}\subset \mathscr{L}$, so $\mathscr{U}_+.\mathscr{L}\subset \mathscr{L}$ and

$$
\mathscr{L}.\mathscr{L}\subset \mathscr{U}_-.\mathscr{U}_0.\mathscr{L}\subset \mathscr{U}_-.\mathscr{L}\subset \mathscr{L}
$$

Thus, $\mathscr{L}$ is a $\mathbf{Z}$-subalgebra of $U(\mathfrak{g})$, so $\mathscr{U}=\mathscr{L}$. If $c$ is the coproduct of $U(\mathfrak{g}),c(\mathscr{U})\subset \mathscr{U}\otimes_{\mathbf{Z}}\mathscr{U}$ (no. 2, Prop. 1). Let $\gamma$ be the counit of $U(\mathfrak{g})$. Since $\gamma (x^{(n)}_{\alpha}) =\gamma (y^{(n)}_{\alpha}) =\gamma ((^h_n))= 0$ for $n >0$, we have $\gamma (\mathscr{U})\subset \mathbf{Z}$. This proves (i). On the other hand,

$$
\mathscr{U}\cap \mathfrak{h}=\mathscr{L}\cap \mathfrak{h}=\mathscr{U}_0\cap \mathfrak{h}=\mathscr{H}
$$

by Prop. 2 of no. 4; similarly,

$$
\mathscr{U}\cap \mathfrak{g}^{\alpha}=\mathscr{U}_+\cap \mathfrak{g}^{\alpha}=\mathbf{Z}x_{\alpha}
$$

by Lemma 5. This proves (ii).

#### Remark 4 {#lie-viii-s12-n6-rem-4 .statement tag=0189}

By Prop. 5 of §4, no. 4, there exists a unique automorphism $\theta$ of $\mathfrak{g}$ such that $\theta (x_{\alpha}) =y_{\alpha}$ and $\theta (y_{\alpha}) =x_{\alpha}$ for all $\alpha \in B$, and $\theta (h) =-h$ for all $h\in \mathfrak{h}$; we have $\theta^2= 1$. By construction of $\mathscr{U}$, we see that the automorphism of $U(\mathfrak{g})$ that extends $\theta$ leaves $\mathscr{U}$ stable.

#### Corollary 1 {#lie-viii-s12-prop-3-cor-1 .statement tag=018A}

Put $\mathscr{G}=\mathscr{U}\cap \mathfrak{g}$. Then $\mathscr{G}$ is an order in the Lie algebra $\mathfrak{g}$, stable under $\theta$. We have $\mathscr{G}=\mathscr{H}+\sum_{\alpha\in R}(\mathscr{G}\cap \mathfrak{g}^{\alpha})$. For all $\alpha \in B$ and all $n\in \mathbf{N}$, the maps (ad $x_{\alpha})^n/n$!, (ad $y_{\alpha})^n/n$! leave $\mathscr{U}$ and $\mathscr{G}$ stable.

The first assertion is clear. The second follows by considering the graduation of type Q(R) on $U(\mathfrak{g})$ and $\mathscr{U}$. The third follows from Lemma 2 of no. 5.

#### Corollary 2 {#lie-viii-s12-prop-3-cor-2 .statement tag=018B}

Let $w\in W$. There exists an elementary automorphism $\varphi$ of $\mathfrak{g}$ that commutes with $\theta$, leaves $\mathscr{G}$ and $\mathscr{U}$ stable, and extends $w$.

It suffices to treat the case in which $w$ is of the form $s_{\alpha}(\alpha \in B)$. Note first of all that ad $x_{\alpha}$ and ad $y_{\alpha}$ are locally nilpotent on $U(\mathfrak{g})$, in other words that for all $u\in U(\mathfrak{g})$ there exists an integer $n$ such that (ad $x_{\alpha})^nu=$ (ad $y_{\alpha})^nu= 0$.

This enables us to define the automorphisms $e^{adx_{\alpha}}=\sum_{n=0}^{\infty}\frac{1}{n!}$(ad $x_{\alpha})^n$ and $e^{ady_{\alpha}}$ of $U(\mathfrak{g})$; we verify immediately that these automorphisms of $U(\mathfrak{g})$ leave $\mathscr{U}$ stable. Put $\varphi_1=e^{adx_{\alpha}}e^{ady_{\alpha}}e^{adx_{\alpha}},\varphi_2=e^{ady_{\alpha}}e^{adx_{\alpha}}e^{ady_{\alpha}}$. We have $\varphi_1|\mathfrak{g}=$ $\varphi_2|\mathfrak{g}($§2, no. 2, formula (1)), so $\varphi_1=\varphi_2$. Put $\varphi_1=\varphi_2=\varphi$. We have $\theta \varphi \theta^{-1}=\varphi$, so $\theta$ and $\varphi$ commute. On the other hand, $\varphi |\mathfrak{h}=w$ by §2, no. 2, Lemma 1.

#### Corollary 3 {#lie-viii-s12-prop-3-cor-3 .statement tag=018C}

Let $\alpha \in R$. If $x\in \mathscr{G}\cap \mathfrak{g}^{\alpha}$ and $n\in \mathbf{N}$, we have $x^{(n)}\in \mathscr{U}$, and (ad $x)^n/n$! leaves $\mathscr{G}$ and $\mathscr{U}$ stable.

This is clear if $\alpha \in B$, by construction of $\mathscr{U}$ and Cor. 1. In the general case, there exists $w\in W$ such that $w(\alpha )\in B$ (Chap. VI, §1, no. 5, Prop. 15). By Cor. 2, there exists an automorphism $\varphi$ of $\mathfrak{g}$ that leaves $\mathscr{G}$ and $\mathscr{U}$ stable and takes $\mathfrak{g}^{\alpha}$ to $\mathfrak{g}^{w(\alpha)}$, hence the corollary by transport of structure.

#### Corollary 4 {#lie-viii-s12-prop-3-cor-4 .statement tag=018D}

There exists a Chevalley system $(X_{\alpha})_{\alpha\in R}$ in $(\mathfrak{g},\mathfrak{h}) ($§2, no. 4, Def. 3) such that $X_{\alpha}=x_{\alpha}$ and $X_{-\alpha}=y_{\alpha}$ for $\alpha \in B$. For every Chevalley system $(X'_{\alpha})_{\alpha\in R}$ having these properties, and for all $\alpha \in R,X'_{\alpha}$ is a basis of $\mathscr{G}\cap \mathfrak{g}^{\alpha}$.

For $\alpha \in B$, put $X_{\alpha}=x_{\alpha}, X_{-\alpha}=y_{\alpha}$. For $\alpha \in R_+$ **--** B, choose a $w\in W$ such that $w(\alpha )\in B$ and an automorphism $\varphi$ of $\mathfrak{g}$ such that $\theta \varphi =\varphi \theta ,\varphi (\mathscr{G}) =\mathscr{G}$ and $\varphi (h) =w^{-1}(h)$ for $h\in \mathfrak{h}$ (Cor. 2); put $X_{\alpha}=\varphi (x_{w(\alpha)}), X_{-\alpha}=\varphi (y_{w(\alpha)})$. Then

$$
[X_{-\alpha}, X_{\alpha}] =\varphi ([y_{w(\alpha)}, x_{w(\alpha)}]) =\varphi (H_{w(\alpha)}) =w^{-1}(H_{w(\alpha)}) =H_{\alpha}
$$

$$
\theta (X_{\alpha}) =\theta \varphi (x_{w(\alpha)}) =\varphi \theta (x_{w(\alpha)}) =\varphi (y_{w(\alpha)}) =X_{-\alpha}
$$

so $(X_{\alpha})_{\alpha\in R}$ is a Chevalley system. Moreover,

$$
\mathscr{G}\cap \mathfrak{g}^{\alpha}=\varphi (\mathscr{G}\cap \mathfrak{g}^{w(\alpha)}) =\varphi (\mathbf{Z}x_{w(\alpha)}) =\mathbf{Z}X_{\alpha} \tag{32}
$$

$$
\mathscr{G}\cap \mathfrak{g}^{-\alpha}=\varphi (\mathscr{G}\cap \mathfrak{g}^{-w(\alpha)}) =\varphi (\mathbf{Z}y_{w(\alpha)}) =\mathbf{Z}X_{-\alpha} \tag{33}
$$

Let $(X'_{\alpha})_{\alpha\in R}$ be a Chevalley system such that $X'_{\alpha}=x_{\alpha}, X'_{-\alpha}=y_{\alpha}$ for $\alpha \in B$. Let S be the set of $\alpha \in R$ such that $X'_{\alpha}=\pm X_{\alpha}$. By §2, no. 4, Prop. 7, S is a closed set of roots. Since $S\supset B\cup (-B)$, we have S = R (Chap. VI, §1, no. 6, Prop. 19). Thus, by (32) and (33), we have $\mathscr{G}\cap \mathfrak{g}^{\alpha}=\mathbf{Z}X'_{\alpha}$ for all $\alpha \in R$.

#### Remark 5 {#lie-viii-s12-n6-rem-5 .statement tag=018E}

Let $(X_{\alpha})_{\alpha\in R}$ be the Chevalley system constructed above. If $\alpha , \beta , \alpha +\beta \in R$ and if we put $[X_{\alpha}, X_{\beta}] = N_{\alpha ,\beta}X_{\alpha+\beta}$, we have $[X_{\alpha}, X_{\beta}]\in$ $\mathscr{G}\cap \mathfrak{g}^{\alpha+\beta}$, and we recover the fact that $N_{\alpha ,\beta}\in \mathbf{Z}$ (cf. §2, no. 4, Prop. 7).

#### Remark 6 {#lie-viii-s12-n6-rem-6 .statement tag=018F}

We have obtained in passing a new proof of the existence of Chevalley systems (cf. §4, no. 4, Cor. of Prop. 5), independent of Lemma 4, §2.

### 7. CHEVALLEY ORDERS

Let $(\mathfrak{g},\mathfrak{h})$ be a split reductive Lie algebra over $\mathbf{Q}, R$ its root system. Choose:

$a)$ a permissible lattice $\mathscr{H}$ in $\mathfrak{h}$ (no. 6, Def. 1);

$b)$ for all $\alpha \in R$, a lattice $\mathscr{G}^{\alpha}$ in $\mathfrak{g}^{\alpha}$.

Put $\mathscr{G}=\mathscr{H}\oplus \sum_{\alpha\in R}\mathscr{G}^{\alpha}$. This is a lattice in $\mathfrak{g}$. Denote by $\mathscr{U}$ the $\mathbf{Z}$-subalgebra

of $U(\mathfrak{g})$ generated by the $(^h_n)(h\in \mathscr{H}, n\in \mathbf{N})$ and the $x^{(n)}(x\in \mathscr{G}^{\alpha}, \alpha \in R$, $n\in \mathbf{N})$. Finally, for $\alpha \in R$ and $x\in \mathfrak{g}^{\alpha}$ **--** $\{0\}$, put

$w_{\alpha}(x) =$ (exp ad $x$)(exp ad $y$)(exp ad $x)$,

where $y$ is the unique element of $\mathfrak{g}^{-\alpha}$ such that $[y, x] =H_{\alpha}$. With these notations:

#### Theorem 2 {#lie-viii-s12-thm-2 .statement tag=018G}

The following conditions are equivalent:

(i) There exists a Chevalley system $(X_{\alpha})_{\alpha\in R}$ of $(\mathfrak{g},\mathfrak{h})$ such that $\mathscr{G}_{\alpha}=\mathbf{Z}X_{\alpha}$ for all $\alpha \in R$.

(ii) $\mathscr{U}\cap \mathfrak{g}=\mathscr{G}$ and $[\mathscr{G}^{\alpha},\mathscr{G}^{-\alpha}] =\mathbf{Z}H_{\alpha}$ for all $\alpha \in R$.

(iii) For all $\alpha \in R, x\in \mathscr{G}^{\alpha}, n\in \mathbf{N}$, the endomorphism (ad $x)^n/n$! of $\mathfrak{g}$ maps $\mathscr{G}$ to $\mathscr{G}$, and $[\mathscr{G}^{\alpha},\mathscr{G}^{-\alpha}] =\mathbf{Z}H_{\alpha}$.

(iv) For all $\alpha \in R$ and every basis $x$ of $\mathscr{G}^{\alpha},w_{\alpha}(x)$ maps $\mathscr{G}$ to $\mathscr{G}($that is, maps $\mathscr{G}^{\beta}$ to $\mathscr{G}^{s_{\alpha}(\beta)}$ for all $\beta \in R)$.

(i) $=\Rightarrow$ (ii): let $(X_{\alpha})_{\alpha\in R}$ be a Chevalley system in $(\mathfrak{g},\mathfrak{h})$ such that $\mathscr{G}^{\alpha}=$ $\mathbf{Z}X_{\alpha}$ for all $\alpha \in R$, and let B be a basis of R. For $\alpha \in B$, put $x_{\alpha}=X_{\alpha}, y_{\alpha}=$ $X_{-\alpha}$. Let $\mathscr{U}'$ be the biorder associated by Prop. 3 of no. 6 to $\mathscr{H}$, the $x_{\alpha}$ and the $y_{\alpha}$. It is clear that $\mathscr{U}'\subset \mathscr{U}$. By Cor. 3 and 4 of Prop. $3,x^{(n)}\in \mathscr{U}'$ for all $\alpha \in R,x\in \mathscr{G}^{\alpha}$ and $n\in \mathbf{N}$. Thus $\mathscr{U}=\mathscr{U}'$, which proves (ii).

(ii) $=\Rightarrow$ (iii): this is clear by Lemma 2 of no. 5.

(iii) $=\Rightarrow$ (iv): let $\alpha \in R$ and let $x$ be a basis of $\mathscr{G}^{\alpha}$. Since $[\mathscr{G}^{\alpha},\mathscr{G}^{-\alpha}] =\mathbf{Z}H_{\alpha}$, the unique $y\in \mathfrak{g}^{-\alpha}$ such that $[y, x] =H_{\alpha}$ belongs to $\mathscr{G}^{-\alpha}$. Since exp ad $x$ and exp ad $y$ leave $\mathscr{G}$ stable by (iii), so does $w_{\alpha}(x)$.

(iv) $=\Rightarrow$ (i): let B be a basis of R. Choose a basis $x_{\alpha}$ of $\mathscr{G}^{\alpha}$ for all $\alpha \in B$. Let $y_{\alpha}\in \mathscr{G}^{-\alpha}$ be such that $[y_{\alpha}, x_{\alpha}] =H_{\alpha}$. By §1, no. 5, formulas (5), we have $y_{\alpha}=w_{\alpha}(x_{\alpha}).x_{\alpha}$ so $y_{\alpha}$ is a basis of $\mathscr{G}^{-\alpha}$ by (iv). Let $\mathscr{G}'$ be the order in $\mathfrak{g}$ defined by $\mathscr{H}$, the $x_{\alpha}$ and the $y_{\alpha}$ (no. 6, Cor. 1 of Prop. 3). Then $\mathscr{G}'$ is stable under the (ad $x_{\alpha})^n/n$!, (ad $y_{\alpha})^n/n$! (loc. cit.), and hence under the $w_{\alpha}(x_{\alpha})$.

Now let $\beta \in R$. There exist $\alpha_0, \alpha_1, . . . , \alpha_r\in B$ such that

$$
\beta =s_{\alpha_r}s_{\alpha_{r-1}}. . . s_{\alpha_1}(\alpha_0)
$$

(Chap. VI, §1, no. 5, Prop. 15). Then $w_{\alpha_r}(x_{\alpha_r}).w_{\alpha_{r-1}}(x_{\alpha_{r-1}}). . . w_{\alpha_1}(x_{\alpha_1})$ maps $\mathscr{G}^{\alpha_0}$ to $\mathscr{G}^{\beta}$ by (iv), and maps $\mathscr{G}'\cap \mathfrak{g}^{\alpha_0}$ to $\mathscr{G}'\cap \mathfrak{g}^{\beta}$ by the preceding. Since $\mathscr{G}'\cap \mathfrak{g}^{\alpha_0}=\mathscr{G}^{\alpha_0}$ (Prop. 3 (ii)), we have $\mathscr{G}'\cap \mathfrak{g}^{\beta}=\mathscr{G}^{\beta}$. Thus

$$
\mathscr{G}'=\mathscr{H}\oplus \sum_{\beta\in R}(\mathscr{G}'\cap \mathfrak{g}^{\beta}) =\mathscr{H}\oplus \sum_{\beta\in R}\mathscr{G}^{\beta}=\mathscr{G}
$$

and Cor. 4 of Prop. 3 concludes the proof.

#### Definition 2 {#lie-viii-s12-def-2 .statement tag=018H}

When conditions (i) to (iv) of Th. 2 are satisfied, $\mathscr{G}$ is said to be a Chevalley order in $(\mathfrak{g},\mathfrak{h})$.

#### Remark {#lie-viii-s12-n7-rem-1 .statement tag=018I}

Chevalley orders in $(\mathfrak{g},\mathfrak{h})$ always exist. Indeed, the Chevalley orders are the sets of the form $\mathscr{H}\oplus \sum_{\alpha\in R}\mathbf{Z}X_{\alpha}$, where $(X_{\alpha})_{\alpha\in R}$ is a Chevalley system in $(\mathfrak{g},\mathfrak{h})$ and $\mathscr{H}$ is a lattice in $\mathfrak{h}$ such that

$$
Q(R^{\vee})\subset \mathscr{H}\subset P(R^{\vee})\oplus \mathfrak{c}
$$

$(\mathfrak{c}$ being the centre of $\mathfrak{g})$.

#### Theorem 3 {#lie-viii-s12-thm-3 .statement tag=018J}

We retain the notations at the beginning of no. 7, and assume that $\mathscr{G}$ is a Chevalley order in $(\mathfrak{g},\mathfrak{h})$.

(i) $\mathscr{U}$ is a biorder in $U(\mathfrak{g})$.

(ii) Let B be a basis of R, and $(X_{\alpha})_{\alpha\in B\cup(-B)}$ a family of elements of $\mathfrak{g}$ such that $\mathscr{G}^{\alpha}=\mathbf{Z}X_{\alpha}$ for $\alpha \in B\cup (-B)$. The $\mathbf{Z}$-algebra $\mathscr{U}$ is generated by the $(^h_n)$ and the $X_{\alpha}^{(n)}(h\in \mathscr{H}, \alpha \in B\cup (-B), n\in \mathbf{N})$. If $\mathfrak{g}$ is semi-simple and $\mathscr{H}= Q(R^{\vee})$, the $\mathbf{Z}$-algebra $\mathscr{U}$ is generated by the $X_{\alpha}^{(n)}(\alpha \in B\cup (-B), n\in \mathbf{N})$.

(iii) Let B be a basis of R, $R_+$ the corresponding set of positive roots, $R_-=-R_+,\mathfrak{n}_+=\sum_{\alpha\in R_+}\mathfrak{g}^{\alpha},\mathfrak{n}_-=\sum_{\alpha\in R_-}\mathfrak{g}^{\alpha}$. Then,

$$
\mathscr{U}= (\mathscr{U}\cap U(\mathfrak{n}_-)).(\mathscr{U}\cap U(\mathfrak{h})).(\mathscr{U}\cap U(\mathfrak{n}_+))
$$

Let $(h_i)_{i\in I}$ be a basis of $\mathscr{H}$. For all $\alpha \in R$, let $X_{\alpha}$ be a basis of $\mathscr{G}^{\alpha}$. Give the set $I\cup R$ a total order (we assume that $I\cap R =\emptyset )$. For $\lambda \in I\cup R$ and $n\in \mathbf{N}$, put $e^{\langle n\rangle}_{\lambda}=(^{h_{\lambda}}_n)$ if $\lambda \in I,e^{\langle n\rangle}_{\lambda}=X_{\lambda}^{(n)}$ if $\lambda \in R$. Then the products $\prod_{\lambda\in I\cup R}e^{\langle n_{\lambda}\rangle}_{\lambda}$, where $(n_{\lambda})$ belongs to $\mathbf{N}^{I\cup R}$, form a basis of the $\mathbf{Z}$-module $\mathscr{U}$. The

products $\prod_{\lambda\in I}(^{h_{\lambda}}_{n_{\lambda}})$, where $(n_{\lambda})$ belongs to $\mathbf{N}^I$, form a basis of the $\mathbf{Z}$-module $\mathscr{U}\cap U(\mathfrak{h})$. The products $\prod_{\lambda\in R_+}X_{\lambda}^{(n_{\lambda})}$, where $(n_{\lambda})$ belongs to $\mathbf{N}^{R_+}$, form a basis of the $\mathbf{Z}$-module $\mathscr{U}\cap U(\mathfrak{n}_+)$.

Let B and $(X_{\alpha})_{\alpha\in B\cup(-B)}$ be as in (ii), and such that $[X_{-\alpha}, X_{\alpha}] =H_{\alpha}$. Let $\mathscr{U}'$ be the $\mathbf{Z}$-subalgebra of $U(\mathfrak{g})$ generated by the $(_n^h)$ and the $X_{\alpha}^{(n)}$ $(h\in \mathscr{H}, \alpha \in B\cup (-B), n\in \mathbf{N})$. We have seen in the proof of Th. 2, (i) $=\Rightarrow$ (ii), that $\mathscr{U}'$ is equal to $\mathscr{U}$ and is a biorder in $U(\mathfrak{g})$. This proves (i) and the first assertion of (ii); the second follows from Lemma 4 (ii). Assertion (iii) follows from Th. 1 (no. 3) and Prop. 3 (no. 6).

### 8. ADMISSIBLE LATTICES

Generalizing the terminology adopted for vector spaces, an endomorphism $u$ of a module M is said to be diagonalizable if there exists a basis of M such that the matrix of $u$ relative to this basis is diagonal.

#### Lemma 6 {#lie-viii-s12-lem-6 .statement tag=018K}

Let M be a free $\mathbf{Z}$-module of finite type, $u$ an endomorphism of M, and $v$ the endomorphism $u\otimes 1$ of $M\otimes_{\mathbf{Z}}\mathbf{Q}$. Assume that $(^v_n)(M)\subset M$ for all $n\in \mathbf{N}$. Then $u$ is diagonalizable.

$a)$ For any polynomial $P\in \mathbf{Q}[T]$ such that $P(\mathbf{Z})\subset \mathbf{Z}$, we have $P(v)(M)\subset M$ (no. 4, Cor. of Prop. 2), so det $P(v)\in \mathbf{Z}$.

$b)$ Denote by $\chi_v(t) =t^d+\alpha_1t^{d-1}+\cdots$ the characteristic polynomial of $v$. Let $k\in \mathbf{Z}, n\in \mathbf{N}$. Applying $a)$ to the polynomial $(^{T-k}_n)$, we see that the number

$a_n=$ det $(v-k)=1_d$ det($v-k$) det($v-k-1$)$. .$. det($v-k-n+ 1$)

$n(n$!)

$$
=\frac{(-1)^n}{4}\chi_v(k)\chi_v(k+ 1). . . \chi_v(k+n-1)
$$

$(n$!)

is an integer. Take $k-1<-\alpha_1/d$. Then

$$
\chi_v(k+n-1) =n^d+ (\alpha_1+ (k-1)d)n^{d-1}+\cdots
$$

and

$$
|a_n|=\frac{|\chi_v(k + n- 1)|}{d}|a_{n-1}|
$$

$$
n
$$

hence, if $a_n\not= 0$ for all $n\in \mathbf{N}$, the sequence of the $|a_n|$ is strictly decreasing for $n$ sufficiently large, which is absurd. It follows that $v$ has an integer eigenvalue $\lambda$. Put $M'=$ Ker($u-\lambda .1$) and $M''= M/M'$. Then $M'$ is the intersection with M of a vector subspace of $M\otimes_{\mathbf{Z}}\mathbf{Q}$, so the $\mathbf{Z}$-module $M''$ is torsion-free of finite type, and consequently free of rank $< d$. Arguing by induction on $d$ and applying the induction hypothesis to the endomorphism of $M''$ induced by $u$, we conclude that all the eigenvalues of $v$ in an algebraically closed extension of $\mathbf{Q}$ are integers.

$c)$ We show that $v$ is diagonalizable. Let $\lambda$ be an eigenvalue of $v$ and let $x\in M\otimes_{\mathbf{Z}}\mathbf{Q}$ be such that $(v-\lambda )^2x= 0$. We have $v(vx-\lambda x) =\lambda (vx-\lambda x)$, so

$n1$!$(v-\lambda -n+ 1)(v-\lambda -n+ 2). . .(v-\lambda -1)(v-\lambda )x$

$$
=\frac{(-1)^{n-1}}{n}(vx-\lambda x)
$$

By $a)$, this implies that $vx-\lambda x\in nM$ for all $n\in \mathbf{N}$, so $(v-\lambda )x= 0$.

$d)$ Let $\lambda$ be an eigenvalue of $v$ and let $\lambda -a, \lambda +b$ be an interval in $\mathbf{Z}$ containing all the eigenvalues of $v$. Consider the polynomial

$$
(T-\lambda -1)(T-\lambda -2). . .(T-\lambda -b)
$$

$$
P(T) = (-1)^b
$$

$b$!

$$
(T-\lambda + 1)(T-\lambda + 2). . .(T-\lambda +a)
$$

$$
\times
$$

$a$!

We have $P(\mathbf{Z})\subset \mathbf{Z},P(\lambda ) = 1,P(\mu) = 0$ for $\mu\in \mathbf{Z}\cap (\lambda -a, \lambda +b)$ and $\mu\not=\lambda$. By $a), P(v)(M)\subset M$. By $c), P(v)$ is a projection of $M\otimes_{\mathbf{Z}}\mathbf{Q}$ onto the eigenspace corresponding to $\lambda$. Q.E.D.

#### Remark 1 {#lie-viii-s12-n8-rem-1 .statement tag=018L}

If we only assume that $v$ is diagonalizable with integer eigenvalues, $u$ is not necessarily diagonalizable (for example, take $M =\mathbf{Z}^2$ and $u(x, y) =$ $(y, x)$ for all $(x, y)\in M)$.

Let $\mathfrak{g},\mathfrak{h},R,\mathscr{H},\mathscr{G}^{\alpha},\mathscr{G},\mathscr{U}$ be as in no. 7, and assume that $\mathscr{G}$ is a Chevalley order in $(\mathfrak{g},\mathfrak{h})$.

#### Definition 3 {#lie-viii-s12-def-3 .statement tag=018M}

Let E be a $\mathfrak{g}$-module. A lattice $\mathscr{E}$ in E is said to be admissible (relative to $\mathscr{G})$ if the following conditions are satisfied:

(i) $\mathscr{U}$ maps $\mathscr{E}$ to $\mathscr{E}$;

(ii) $\mathscr{E}$ is stable under $(^h_n)$ and $x^{(n)}$ for all $\alpha \in R, x\in \mathscr{G}^{\alpha}, n\in \mathbf{N}, h\in \mathscr{H}$.

#### Remark 2 {#lie-viii-s12-n8-rem-2 .statement tag=018N}

Let $\rho$ be the adjoint representation of $\mathfrak{g}$ on $U(\mathfrak{g})$. Let $\alpha , x, n, h$ be as in (ii) above. We have $\rho (x^{(n)}).\mathscr{U}\subset \mathscr{U}$ by Lemma 2. On the other hand, if $p\in \mathbf{N}$,

$((h))_{(n)}($ ad $h)_{(n)}(n\alpha (h))_{(n)}$

$\rho x$ = $x$ = $x$

$$
ppp
$$

(no. 5, formula (13)), so $\rho ((^h_p)).\mathscr{U}\subset \mathscr{U}$. This proves that $\mathscr{U}$ is an admissible lattice in $U(\mathfrak{g})$, and it follows that $\mathscr{G}$ is an admissible lattice in $\mathfrak{g}$ (for the adjoint representation).

#### Remark 3 {#lie-viii-s12-n8-rem-3 .statement tag=018O}

Let E be a finite dimensional $\mathfrak{g}$-module, $\mathscr{E}$ an admissible lattice in E, $\mathfrak{c}$ the centre of $\mathfrak{g}$. By Lemma 6, every element of $\mathfrak{c}$ defines a diagonalizable endomorphism of E. Hence E is semi-simple (Chap. I, §6, no. 5, Th. 4). Thus, E is a direct sum of simple $\mathscr{D}\mathfrak{g}$-modules on which $\mathfrak{c}$ induces homotheties. By Lemma $6,\mathscr{E}=\oplus (\mathscr{E}\cap E^{\lambda})$ and, for all weights $\lambda$ of E, we have

$$
\lambda (\mathscr{H})\subset \mathbf{Z}
$$

#### Remark 4 {#lie-viii-s12-n8-rem-4 .statement tag=018P}

If $\mathfrak{g}$ is semi-simple and $\mathscr{H}= Q(R^{\vee})$, conditions (i) and (ii) of Def. 3 are equivalent, by Th. 3 (ii), to

(iii) $\mathscr{E}$ is stable under $x^{(n)}$ for all $\alpha \in R, x\in \mathscr{G}^{\alpha}, n\in \mathbf{N}$.

#### Remark 5 {#lie-viii-s12-n8-rem-5 .statement tag=018Q}

Let B be a basis of R; in conditions (i) and (ii) above, “$\alpha \in$ R” can be replaced by “$\alpha \in B\cup (-$B)” (loc. cit).

#### Theorem 4 {#lie-viii-s12-thm-4 .statement tag=018R}

Let E be a finite dimensional $\mathfrak{g}$-module. The following conditions are equivalent:

(i) E has an admissible lattice;

(ii) every element of $\mathscr{H}$ defines a diagonalizable endomorphism of E with integer eigenvalues.

(i) $=\Rightarrow$ (ii): this follows from Remark 3.

(ii) $=\Rightarrow$ (i): we assume that condition (ii) is satisfied and prove (i). By Th. 4 of Chap. I, §6, no. 5, we can assume that the elements of $\mathfrak{c}$ define homotheties of E, and that E is a simple $\mathscr{D}\mathfrak{g}$-module. Let B be a basis of R, and $\mathfrak{g}=\mathfrak{n}_-\oplus \mathfrak{h}\oplus \mathfrak{n}_+$ the corresponding decomposition of $\mathfrak{g}$. Let $\lambda$ be the highest weight of the $\mathscr{D}\mathfrak{g}$-module E, and let $e\in E^{\lambda}$ **--** $\{0\}$. Put $\mathscr{E}=\mathscr{U}.e$. It is clear that $\mathscr{U}.\mathscr{E}\subset \mathscr{E}$. Since E is simple, $U(\mathfrak{g}).e= E$ and hence $\mathscr{E}$ generates E as a $\mathbf{Q}$-vector space. For $h\in \mathscr{H}$ and $n\in \mathbf{N}$, we have $(^h_n)e=(^{\lambda(h)}_n)e\in \mathbf{Z}e$, so

$$
(\mathscr{U}\cap U(\mathfrak{h})).e=\mathbf{Z}e
$$

Since $U(\mathfrak{n}_+).e= 0$, we have $\mathscr{E}= (\mathscr{U}\cap U(\mathfrak{n}_-)).e$ by Prop. 3. It now follows from Th. 3 (iii) that $\mathscr{E}$ is a $\mathbf{Z}$-module of finite type.

#### Corollary {#lie-viii-s12-n8-cor-1 .statement tag=018S}

If $\mathfrak{g}$ is semi-simple and $\mathscr{H}= Q(R^{\vee})$, every finite dimensional $\mathfrak{g}$-module has an admissible lattice.
