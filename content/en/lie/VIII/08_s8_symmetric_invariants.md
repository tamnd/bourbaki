---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 8
section_title: Symmetric invariants
lang: en
source: lie-vii-ix
book_pages: 141-151, 250-253
pdf_pages: 0149-0159, 0258-0261
extraction: native+ocr
subsections:
    - "no": 1
      title: EXPONENTIAL OF A LINEAR FORM
      page: 141
      pdf_page: 149
    - "no": 2
      title: INJECTION OF $\boldsymbol{k}$[P] INTO S($\mathfrak{h}$)$^*$
      page: 142
      pdf_page: 150
    - "no": 3
      title: INVARIANT POLYNOMIAL FUNCTIONS
      page: 143
      pdf_page: 151
    - "no": 4
      title: PROPERTIES OF Aut0
      page: 148
      pdf_page: 156
    - "no": 5
      title: CENTRE OF THE ENVELOPING ALGEBRA
      page: 148
      pdf_page: 156
statements: 24
exercises: 18
content_sha256: 8859a6b0573d4c210f3a62d9f114b94021ab2d8e4f8b830402b7c871294dce5b
---

## § 8. SYMMETRIC INVARIANTS

In this paragraph, we denote by $(\mathfrak{g},\mathfrak{h})$ a split semi-simple Lie algebra, by R its root system, by W its Weyl group, and by P its group of weights.

### 1. EXPONENTIAL OF A LINEAR FORM

Let V be a finite dimensional vector space, $\mathbf{S}(V)$ its symmetric algebra. The coalgebra structure of $\mathbf{S}(V)$ defines on $\mathbf{S}(V)^*$ a commutative and associative algebra structure (Algebra, Chap. III, §11, pp. 579 to 582). The vector space $\mathbf{S}(V)^*$ can be identified canonically with $\prod_{m\geq 0}\mathbf{S}^m(V)^*$, and $\mathbf{S}^m(V)^*$ can

be identified canonically with the space of symmetric $m$-linear forms on V. The canonical injection of $V^*=\mathbf{S}^1(V)^*$ into $\mathbf{S}(V)^*$ defines an injective homomorphism from the algebra $\mathbf{S}(V^*)$ to the algebra $\mathbf{S}(V)^*$, whose image is $\mathbf{S}(V)^{*gr}=\sum_{m\geq 0}\mathbf{S}^m(V)^*($Algebra, Chap. III, §11, no. 5, Prop. 8). We identify

the algebras $\mathbf{S}(V^*)$ and $\mathbf{S}(V)^{*gr}$ by means of this homomorphism; we also identify $\mathbf{S}(V^*)$ with the algebra of polynomial functions on V (Chap. VII, App. I, no. 1).

The elements $(u_m)\in \prod_{m\geq 0}\mathbf{S}^m(V)^*$ such that $u_0= 0$ form an ideal J of

$\mathbf{S}(V)^*$; we give $\mathbf{S}(V)^*$ the J-adic topology (Commutative Algebra, Chap. III, §2, no. 5), in which $\mathbf{S}(V)^*$ is complete and $\mathbf{S}(V^*)$ is dense in $\mathbf{S}(V)^*$. If $(e^*_i)_{1\leq i\leq n}$ is a basis of $V^*$, and if $T_1, . . . ,T_n$ are indeterminates, the homomorphism from $k[T_1, . . . ,T_n]$ to $\mathbf{S}(V^*)$ that takes $T_i$ to $e^*_i(1\leq i\leq n)$ is an isomorphism of algebras, and extends to a continuous isomorphism from the algebra $k[[T_1, . . . ,T_n]]$ to the algebra $\mathbf{S}(V)^*$.

For all $\lambda \in V^*$, the family $\lambda^n/n$! is summable in $\mathbf{S}(V)^*$. Its sum is called the exponential of $\lambda$ and is denoted by exp($\lambda$ ) (conforming to Chap. II, §6, no. 1). Let $x_1, . . . , x_n\in V$; we have

$\langle$exp $\lambda , x_1. . . x_n\rangle =1\langle \lambda^n, x_1. . . x_n\rangle =\langle \lambda , x_1\rangle . . .\langle \lambda , x_n\rangle$

$n$!

by Algebra, Chap. III, §11, no. 5, formula (29). It follows immediately that exp($\lambda$ ) is the unique homomorphism from the algebra $\mathbf{S}(V)$ to $k$ that extends $\lambda$.

We have exp($\lambda +\mu$) $=$ exp($\lambda$ ) exp($\mu$) for all $\lambda , \mu\in V^*$ (Chap. II, §6, no. 1, Remark). Thus, the map exp$: V^*\rightarrow \mathbf{S}(V)^*$ is a homomorphism from the additive group $V^*$ to the multiplicative group of invertible elements of $\mathbf{S}(V)^*$. The family (exp $\lambda )_{\lambda\in V^*}$ is a free family in the vector space $\mathbf{S}(V)^*($Algebra, Chap. V, §7, no. 3, Th. 1).

#### Lemma 1 {#lie-viii-s8-lem-1 .statement tag=0154}

Let $\Pi$ be a subgroup of $V^*$ that generates the vector space $V^*$, and $m$ an integer $\geq 0$. Then pr$_m$(exp $\Pi )$ generates the vector space $\mathbf{S}^m(V^*)$.

By Algebra, Chap. I, §8, no. 2, Prop. 2, any product of $m$ elements of $V^*$ is a $k$-linear combination of elements of the form $x^m$ where $x\in \Pi$. But $x^m=m$! pr$_m$(exp $x)$. Q.E.D.

By transport of structure, every automorphism of V defines automorphisms of the algebras $\mathbf{S}(V)$ and $\mathbf{S}(V)^*$; this gives linear representations of $\mathbf{G}\mathbf{L}(V)$ on $\mathbf{S}(V)$ and $\mathbf{S}(V)^*$.

### 2. INJECTION OF $\boldsymbol{k}$[P] INTO S($\mathfrak{h}$)$^*$

The map $p \rightarrow$ exp $p$ from P to $\mathbf{S}(\mathfrak{h})^*$ is a homomorphism from the additive group P to $\mathbf{S}(\mathfrak{h})^*$ equipped with its multiplicative structure (no. 1). Consequently, there exists a unique homomorphism $\psi$ from the algebra $k[P]$ of the monoid P to the algebra $\mathbf{S}(\mathfrak{h})^*$ such that

$\psi (e^{\lambda}) =$ exp($\lambda$ )$(\lambda \in P)$

(in the notations of §7, no. 7). By no. $1,\psi$ is injective. By transport of structure, $\psi (w(e^{\lambda})) =w(\psi (e^{\lambda}))$ for all $\lambda \in P$ and all $w\in W$. Hence, if $k[P]^W$ (resp. $\mathbf{S}(\mathfrak{h})^{*W})$ denotes the set of elements of $k[P]$ (resp. $\mathbf{S}(\mathfrak{h})^*)$ invariant under W, we have $\psi (k[P]^W)\subset \mathbf{S}(\mathfrak{h})^{*W}$.

#### Proposition 1 {#lie-viii-s8-prop-1 .statement tag=0155}

Let $S^m(\mathfrak{h}^*)^W$ be the set of elements of $S^m(\mathfrak{h}^*)$ invariant under W. Then pr$_m(\psi (k[P]^W)) =\mathbf{S}^m(\mathfrak{h}^*)^W$.

It is clear from the preceding that pr$_m(\psi (k[P]^W))\subset \mathbf{S}^m(\mathfrak{h}^*)^W$. Every element of $\mathbf{S}^m(\mathfrak{h}^*)$ is a $k$-linear combination of elements of the form

pr$_m$(exp $\lambda ) =$ (pr$_m\circ \psi )(e^{\lambda})$

where $\lambda \in P$ (Lemma 1). Hence every element of $\mathbf{S}^m(\mathfrak{h}^*)^W$ is a linear combination of elements of the form

$\sum_{w\in W}w$((pr$_m\circ \psi )(e^{\lambda})) =$ (pr$_m\circ \psi )(\sum_{w\in W}w(e^{\lambda}))$,

each of which belongs to pr$_m(\psi (k[P]^W))$.

#### Proposition 2 {#lie-viii-s8-prop-2 .statement tag=0156}

Let E be a finite dimensional $\mathfrak{g}$-module. Let $U(\mathfrak{h}) =\mathbf{S}(\mathfrak{h})$ be the enveloping algebra of $\mathfrak{h}$. If $u\in U(\mathfrak{h})$, then

Tr($u_E$) $=\langle \psi$(ch $E), u\rangle$.

It suffices to treat the case in which $u=h_1. . . h_m$ with $h_1, . . . , h_m\in \mathfrak{h}$. For all $\lambda \in P$, let $d_{\lambda}=$ dim $E^{\lambda}$. Then ch $E =\sum_{\lambda}d_{\lambda}e^{\lambda}$, so $\psi$(ch $E) =\sum_{\lambda}d_{\lambda}$ exp($\lambda$ ) and hence

$$
\langle \psi(\mathrm{ch}\,E),u\rangle
 = \sum_{\lambda} d_\lambda\langle\exp\lambda,h_1\ldots h_m\rangle
$$
$$
= \sum_{\lambda} d_\lambda\lambda(h_1)\ldots\lambda(h_m)\qquad\text{(no. 1)}
$$
$$
= \mathrm{Tr}\,u_E.
$$

#### Corollary 1 {#lie-viii-s8-prop-2-cor-1 .statement tag=01J7}

— Let $\mathrm{U}(\mathfrak g)$ be the enveloping algebra of $\mathfrak g$. Let the homomorphism
$$
\zeta:\mathrm{U}(\mathfrak g)^*\longrightarrow\mathrm{U}(\mathfrak h)^*=\mathrm{S}(\mathfrak h)^*
$$
be the transpose of the canonical injection
$$
\mathrm{U}(\mathfrak h)\longrightarrow\mathrm{U}(\mathfrak g).
$$
The following diagram commutes
$$
\begin{array}{ccccc}
\mathscr{R}(\mathfrak g)&\xrightarrow{\mathrm{ch}}&\mathbf{Z}[P]\\
\Big\downarrow{\scriptstyle\mathrm{Tr}}&&\Big\downarrow{\scriptstyle\psi}\\
\mathrm{U}(\mathfrak g)^*&\xrightarrow{\zeta}&\mathrm{S}(\mathfrak h)^*
\end{array}
$$

This is simply a reformulation of Prop. 2.

#### Corollary 2 {#lie-viii-s8-prop-2-cor-2 .statement tag=01J8}

— Let $m$ be an integer $\geqslant 0$. Every element of $\mathrm{S}^m(\mathfrak h^*)^W$ is a linear combination of polynomial functions on $\mathfrak h$ of the form $x\mapsto\mathrm{Tr}(\rho(x)^m)$, where $\rho$ is a finite dimensional linear representation of $\mathfrak g$.

By Prop. 1, $\mathrm{S}^m(\mathfrak h^*)^W=(\mathrm{pr}_m\circ\psi)(k[P]^W)$. Now $\mathbf{Z}[P]^W=\mathrm{ch}\,\mathscr{R}(\mathfrak g)$ (§7, no. 7, Th. 2 (ii)). Thus, by Chap. VI, §3, no. 4, Lemma 3, $\psi(k[P]^W)$ is the $k$-vector subspace of $\mathrm{S}(\mathfrak h)^*$ generated by $\psi(\mathrm{ch}\,\mathscr{R}(\mathfrak g))=\zeta(\mathrm{Tr}\,\mathscr{R}(\mathfrak g))$. Consequently, $\mathrm{S}^m(\mathfrak h^*)^W$ is the vector subspace of $\mathrm{S}^m(\mathfrak h^*)$ generated by $(\mathrm{pr}_m\circ\zeta\circ\mathrm{Tr})(\mathscr{R}(\mathfrak g))$. But, if $\rho$ is a finite dimensional linear representation of $\mathfrak g$,

$$
((\mathrm{pr}_m\circ\zeta\circ\mathrm{Tr})(\rho))(x)
=\left\langle(\zeta\circ\mathrm{Tr})(\rho),\frac{x^m}{m!}\right\rangle
=\frac{1}{m!}\mathrm{Tr}(\rho(x)^m)
$$

for all $x\in\mathfrak h$.

### 3. INVARIANT POLYNOMIAL FUNCTIONS

Let $\mathfrak a$ be a finite dimensional Lie algebra. In accordance with the conventions of no. 1, we identify the algebra $\mathrm{S}(\mathfrak a^*)$, the algebra $\mathrm{S}(\mathfrak a)^{*gr}$, and the algebra of polynomial functions on $\mathfrak a$. For all $a\in\mathfrak a$, let $\theta(a)$ be the derivation of $\mathrm{S}(\mathfrak a)$ such that $\theta(a)x=[a,x]$ for all $x\in\mathfrak a$. We know (Chap. I, §3, no. 2) that $\theta$ is a representation of $\mathfrak a$ on $\mathrm{S}(\mathfrak a)$. Let $\theta^*(\mathfrak a)$ be the restriction of ${}^t\theta(a)$ to $\mathrm{S}(\mathfrak a^*)$. Then $\theta^*$ is a representation of $\mathfrak a$. If $f\in\mathrm{S}^n(\mathfrak a^*)$, then $\theta^*(a)f\in\mathrm{S}^n(\mathfrak a^*)$ and, for $x_1,\ldots,x_n\in\mathfrak a$,

$$
(\theta^*(a)f)(x_1,\ldots,x_n)
=-\sum_{1\leqslant i\leqslant n}
f(x_1,\ldots,x_{i-1},[a,x_i],x_{i+1},\ldots,x_n).
\tag{1}
$$

We deduce easily from (1) that $\theta^*(a)$ is a derivation of $\mathbf{S}(\mathfrak{a}^*)$. An element of $\mathbf{S}(\mathfrak{a})$ (resp. $\mathbf{S}(\mathfrak{a}^*))$ that is invariant under the representation $\theta$ (resp. $\theta^*)$ of $\mathfrak{a}$ is called an invariant element of $\mathbf{S}(\mathfrak{a})$ (resp. $\mathbf{S}(\mathfrak{a}^*))$.

#### Lemma 2 {#lie-viii-s8-lem-2 .statement tag=0157}

Let $\rho$ be a finite dimensional linear representation of $\mathfrak{a}$, and $m$ an integer $\geq 0$. The function $x \rightarrow$ Tr($\rho (x)^m$) on $\mathfrak{a}$ is an invariant polynomial function.

Put $g(x_1, . . . , x_m) =$ Tr($\rho (x_1). . . \rho (x_m)$) for $x_1, . . . , x_m\in \mathfrak{a}$. If $x\in \mathfrak{a}$, we have

$$
-(\theta^*(x)g)(x_1, . . . , x_m)
$$

$=\sum_{1\leq i\leq m}$ Tr($\rho (x_1). . . \rho (x_{i-1})[\rho (x), \rho (x_i)]\rho (x_{i+1}). . . \rho (x_m)$)

= Tr($\rho (x)\rho (x_1). . . \rho (x_m)$)$-$ Tr($\rho (x_1). . . \rho (x_m)\rho (x)$) $= 0$,

so $\theta^*(x)g= 0$. Let $h$ be the symmetric multilinear form defined by

1 $\sum$

$$
h(x_1, . . . , x_m) =g(x_{\sigma(1)}, . . . , x_{\sigma(m)})
$$

$m$!

$\sigma \in \mathfrak{S}_m$

For all $x\in \mathfrak{a}$, we have $\theta^*(x)h= 0$ and Tr($\rho (x)^m$) $=h(x, . . . , x)$, hence the lemma.

#### Lemma 3 {#lie-viii-s8-lem-3 .statement tag=0158}

Let E be a finite dimensional $\mathfrak{g}$-module, and $x\in E$. Then $x$ is an invariant element of the $\mathfrak{g}$-module E if and only if (exp $a_E).x=x$ for every nilpotent element $a$ of $\mathfrak{g}$.

The condition is clearly necessary. Assume now that it is satisfied. Let $a$ be a nilpotent element of $\mathfrak{g}$. There exists an integer $n$ such that $a^n_E= 0$. For all $t\in k$, we have

1 1 $_{--}$

0 = exp($ta_E$)$.x-x=ta_Ex+t^2a^2_Ex+\cdots +t^{n1}a^{n1}x$,

2! $(n-$ 1)! $^E$

so $a_Ex= 0$. But the Lie algebra $\mathfrak{g}$ is generated by its nilpotent elements (§4, no. 1, Prop. 1). Hence $x$ is an invariant element of the $\mathfrak{g}$-module E. Q.E.D.

For any $\xi \in \mathbf{G}\mathbf{L}(\mathfrak{g})$, let $\mathbf{S}(\xi )$ be the automorphism of $\mathbf{S}(\mathfrak{g})$ that extends $\xi$, and $\mathbf{S}^*(\xi )$ the restriction to $\mathbf{S}(\mathfrak{g}^*)$ of the contragredient automorphism of $\mathbf{S}(\xi )$. Then $\mathbf{S}$ and $\mathbf{S}^*$ are representations of $\mathbf{G}\mathbf{L}(\mathfrak{g})$. If $a$ is a nilpotent element of $\mathfrak{g},\theta (a)$ is locally nilpotent on $\mathbf{S}(\mathfrak{g})$ and $\mathbf{S}$(exp ad $a) =$ exp$\theta (a)$, so

$\mathbf{S}^*$(exp ad $a) =$ exp$\theta^*(a)$. (2)

#### Proposition 3 {#lie-viii-s8-prop-3 .statement tag=0159}

Let $f$ be a polynomial function on $\mathfrak{g}$. The following conditions are equivalent:

(i) $f\circ s=f$ for all $s\in$ Aut$_e(\mathfrak{g})$;

(ii) $f\circ s=f$ for all $s\in$ Aut$_0(\mathfrak{g})$;

(iii) $f$ is invariant.

The equivalence of (i) and (iii) follows from formula (2) and Lemma 3. It follows from this that (iii) implies (ii) by extension of the base field. The implication (ii) $=\Rightarrow$ (i) is clear.

Note carefully that, if $f$ satisfies the conditions of Prop. $3,f$ is not in general invariant under Aut($\mathfrak{g}$) (Exerc. 1 and 2).

#### Theorem 1 {#lie-viii-s8-thm-1 .statement tag=015A}

Let $I(\mathfrak{g}^*)$ be the algebra of invariant polynomial functions on $\mathfrak{g}$. Let $i:\mathbf{S}(\mathfrak{g}^*)\rightarrow \mathbf{S}(\mathfrak{h}^*)$ be the restriction homomorphism.

(i) The map $i|I(\mathfrak{g}^*)$ is an isomorphism from the algebra $I(\mathfrak{g}^*)$ to the algebra $\mathbf{S}(\mathfrak{h}^*)^W$.

(ii) For any integer $n\geq 0$, let $I^n(\mathfrak{g}^*)$ be the set of homogeneous elements of $I(\mathfrak{g}^*)$ of degree $n$. Then $I^n(\mathfrak{g}^*)$ is the set of linear combinations of functions on $\mathfrak{g}$ of the form $x \rightarrow$ Tr($\rho (x)^n$), where $\rho$ is a finite dimensional linear representation of $\mathfrak{g}$.

(iii) Let $l=$ rk($\mathfrak{g}$). There exist $l$ algebraically independent homogeneous elements of $I(\mathfrak{g}^*)$ that generate the algebra $I(\mathfrak{g}^*)$.

$a)$ Let $f\in I(\mathfrak{g}^*)$ and $w\in W$. There exists $s\in$ Aut$_e(\mathfrak{g},\mathfrak{h})$ such that $s|\mathfrak{h}=w($§2, no. 2, Cor. of Th. 2). Since $f$ is invariant under $s$ (Prop. $3),i(f)$ is invariant under $w$. Hence $i(I(\mathfrak{g}^*))\subset \mathbf{S}(\mathfrak{h}^*)^W$.

$b)$ We prove that, if $f\in I(\mathfrak{g}^*)$ is such that $i(f) = 0$, then $f= 0$. Extending the base field if necessary, we can assume that $k$ is algebraically closed. By Prop. $3,f$ vanishes on $s(\mathfrak{h})$ for all $s\in$ Aut$_e(\mathfrak{g})$. Hence $f$ vanishes on every Cartan subalgebra of $\mathfrak{g}$ (Chap. VII, §3, no. 2, Th. 1), and in particular on the set of regular elements of $\mathfrak{g}$. But this set is dense in $\mathfrak{g}$ for the Zariski topology (Chap. VII, §2, no. 2).

$c)$ Let $n$ be an integer $\geq 0$. Let $L^n$ be the set of linear combinations of functions of the form $x \rightarrow$ Tr($\rho (x)^n$) on $\mathfrak{g}$, where $\rho$ is a finite dimensional linear representation of $\mathfrak{g}$. By Lemma $2, L^n\subset I^n(\mathfrak{g}^*)$. Thus

$$
i(L^n)\subset i(I^n(\mathfrak{g}^*))\subset \mathbf{S}^n(\mathfrak{h}^*)^W
$$

By Cor. 2 of Prop. $2,\mathbf{S}^n(\mathfrak{h}^*)^W\subset i(L^n)$. Hence $i(I^n(\mathfrak{g}^*)) =\mathbf{S}^n(\mathfrak{h}^*)^W$, which proves (i), and $i(L^n) =i(I^n(\mathfrak{g}^*))$ so $L^n= I^n(\mathfrak{g}^*)$ by $b)$. Thus (ii) is proved.

$d)$ Assertion (iii) follows from (i) and Chap. V, §5, no. 3, Th. 3.

#### Corollary 1 {#lie-viii-s8-thm-1-cor-1 .statement tag=015B}

Assume that $\mathfrak{g}$ is simple. Let $m_1, . . . , m_l$ be the exponents of the Weyl group of $\mathfrak{g}$. There exist elements $P_1, . . . ,P_l$ of $I(\mathfrak{g}^*)$, homogeneous of degrees

$$
m_1+ 1, . . . , m_l+ 1
$$

which are algebraically independent and generate the algebra $I(\mathfrak{g}^*)$.

This follows from Th. 2 (i) and Chap. V, §6, no. 2, Prop. 3.

#### Corollary 2 {#lie-viii-s8-thm-1-cor-2 .statement tag=015C}

Let B be a basis of R, $R_+$ (resp. $R_-)$ the set of positive (resp. negative) roots of $(\mathfrak{g},\mathfrak{h})$ relative to B$,\mathfrak{n}_+=\sum_{\alpha\in R_+}\mathfrak{g}^{\alpha},\mathfrak{n}_-=\sum_{\alpha\in R_-}\mathfrak{g}^{\alpha}$, $\mathbf{S}(\mathfrak{h})$ the symmetric algebra of $\mathfrak{h}$, and J the ideal of $\mathbf{S}(\mathfrak{g})$ generated by $\mathfrak{n}_+\cup \mathfrak{n}_-$.

(i) $\mathbf{S}(\mathfrak{g}) =\mathbf{S}(\mathfrak{h})\oplus J$.

(ii) Let $j$ be the homomorphism from the algebra $\mathbf{S}(\mathfrak{g})$ to the algebra $\mathbf{S}(\mathfrak{h})$ defined by the preceding decomposition of $\mathbf{S}(\mathfrak{g})$. Let $I(\mathfrak{g})$ be the set of invariant elements of $\mathbf{S}(\mathfrak{g})$. Let $\mathbf{S}(\mathfrak{h})^W$ be the set of elements of $\mathbf{S}(\mathfrak{h})$ invariant under the operation of W. Then $j|I(\mathfrak{g})$ is an isomorphism from $I(\mathfrak{g})$ to $\mathbf{S}(\mathfrak{h})^W$.

Assertion (i) is clear. The Killing form defines an isomorphism from the vector space $\mathfrak{g}^*$ to the vector space $\mathfrak{g}$, which extends to an isomorphism $\xi$ from the $\mathfrak{g}$-module $\mathbf{S}(\mathfrak{g}^*)$ to the $\mathfrak{g}$-module $\mathbf{S}(\mathfrak{g})$. We have $\xi (I(\mathfrak{g}^*)) = I(\mathfrak{g})$. The orthogonal complement of $\mathfrak{h}$ with respect to the Killing form is $\mathfrak{n}_++\mathfrak{n}_-($§2, no. 2, Prop. 1). If we identify $\mathfrak{h}^*$ with the orthogonal complement of $\mathfrak{n}_++\mathfrak{n}_$-in $\mathfrak{g}^*$, then $\xi (\mathfrak{h}^*) =\mathfrak{h}$, so $\xi (\mathbf{S}(\mathfrak{h}^*)) =\mathbf{S}(\mathfrak{h})$ and $\xi (\mathbf{S}(\mathfrak{h}^*)^W) =\mathbf{S}(\mathfrak{h})^W$. Finally, $\xi^{-1}(J)$ is the set of polynomial functions on $\mathfrak{g}$ that vanish on $\mathfrak{h}$. This proves that $\xi$ transforms the homomorphism $i$ of Th. 1 into the homomorphism $j$ of Cor. 2. Thus assertion (ii) follows from Th. 1 (i).

#### Proposition 4 {#lie-viii-s8-prop-4 .statement tag=015D}

Let $\mathfrak{a}$ be a semi-simple Lie algebra, $l$ its rank. Let I (resp. $I')$ be the set of elements of $\mathbf{S}(\mathfrak{a}^*)$ (resp. $\mathbf{S}(\mathfrak{a}))$ invariant under the representation induced by the adjoint representation of $\mathfrak{a}$. Let Z be the centre of the enveloping algebra of $\mathfrak{a}$.

(i) I and $I'$ are graded polynomial algebras (Chap. V, §5, no. 1) of transcendance degree $l$.

(ii) Z is isomorphic to the algebra of polynomials in $l$ indeterminates over $k$.

The canonical filtration of the enveloping algebra of $\mathfrak{a}$ induces a filtration of Z. By Chap. I, §2, no. 7, Th. 1 and p. 25, gr Z is isomorphic to $I'$. In view of Commutative Algebra, Chap. III, §2, no. 9, Prop. 10, it follows that (i) $=\Rightarrow$ (ii).

On the other hand, Th. 1 and its Cor. 2 show that (i) is true whenever $\mathfrak{a}$ is split. The general case reduces to that case in view of the following lemma:

#### Lemma 4 {#lie-viii-s8-lem-4 .statement tag=01JY}

$^2$ Let $A =\bigoplus_{n\geq 0}A^n$ be a graded $k$-algebra, $k'$ an extension of $k$, and $A'= A\otimes_kk'$. Assume that $A'$ is a graded polynomial algebra over $k'$. Then A is a graded polynomial algebra over $k$.

We have ${A'}^0=k'$, so $A^0=k$. Put $A_+=\bigoplus_{n\geq 1}A^n$ and $P = A_+/A^2_+$. Then P is a graded vector space, and there is a graded linear map $f: P\rightarrow A_+$ of

$^2$ In Lemmas 4, 5 and $6,k$ can be any (commutative) field. degree zero such that the composite with the canonical projection $A_+\rightarrow P$ is the identity on P. Give $\mathbf{S}(P)$ the graded structure induced by that of P (Algebra, Chap. III, p. 506). The homomorphism of $k$-algebras $g:\mathbf{S}(P)\rightarrow A$ that extends $f$ (Algebra, Chap. III, p. 497) is a graded homomorphism of degree 0; an immediate induction on the degree shows that $g$ is surjective.

#### Lemma 5 {#lie-viii-s8-lem-5 .statement tag=015E}

A is a graded polynomial algebra if and only if P is finite dimensional and $g$ is bijective.

If P is finite dimensional, $\mathbf{S}(P)$ is clearly a graded polynomial algebra, and so is A if $g$ is bijective. Conversely, assume that A is generated by algebraically independent homogeneous elements $x_1, . . . , x_m$ of degrees $d_1, . . . , d_m$. Let $\overline{x}_i$ be the image of $x_i$ in P. It is immediate that the $\overline{x}_i$ form a basis of P; since $\overline{x}_i$ is of degree $d_i$, it follows that $\mathbf{S}(P)$ and A are isomorphic; in particular, dim $\mathbf{S}(P)^n=$ dim $A^n$ for all $n$. Since $g$ is surjective, it is necessarily bijective.

Lemma 4 is now immediate. Indeed, Lemma 5, applied to the $k'$-algebra $A'$, shows that $g\otimes 1 :\mathbf{S}(P)\otimes k'\rightarrow A\otimes k'$ is bijective, and hence so is $g$.

#### Proposition 5 {#lie-viii-s8-prop-5 .statement tag=015F}

We retain the notations of Prop. 4, and denote by $\mathfrak{p}$ the ideal of $\mathbf{S}(\mathfrak{a}^*)$ generated by the homogeneous elements of I of degree $\geq 1$. Let $x\in \mathfrak{a}$. Then $x$ is nilpotent if and only if $f(x) = 0$ for all $x\in \mathfrak{p}.^3$

Extending the base field if necessary, we can assume that $\mathfrak{a}=\mathfrak{g}$ is splittable. Assume that $x$ is nilpotent. For any finite dimensional linear representation $\rho$ of $\mathfrak{g}$, and any integer $n\geq 1$, we have Tr($\rho (x)^n$) $= 0$, so $f(x) = 0$ for all homogeneous $f\in I(\mathfrak{g}^*)$ of degree $\geq 1$ (Th. 1 (ii)), and hence $f(x) = 0$ for all $f\in \mathfrak{p}$. Conversely, if $f(x) = 0$ for all $f\in \mathfrak{p}$, then Tr((ad $x)^n) = 0$ for all $n\geq 1$ (Th. 1 (ii)), so $x$ is nilpotent.

#### Remark 1 {#lie-viii-s8-n3-rem-1 .statement tag=01L5}

$^*$Let $P_1, . . . ,P_l$ be algebraically independent homogeneous elements of I that generate the algebra I. Then $(P_1, . . . ,P_l)$ is an $\mathbf{S}(\mathfrak{a}^*)$-regular sequence (Chap. V, §5, no. 5). Indeed, extending the base field if necessary, we can assume that $\mathfrak{a}=\mathfrak{g}$ is splittable. Now let N = dim $\mathfrak{g}$, and let

$$
(Q_1, . . . ,Q_{N-l})
$$

be a basis of the orthogonal complement of $\mathfrak{h}$ in $\mathfrak{g}^*$. Let $\mathfrak{m}$ be the ideal of $\mathbf{S}(\mathfrak{g}^*)$ generated by $P_1, . . . ,P_l,Q_1, . . . ,Q_{N-l}$. Then $\mathbf{S}(\mathfrak{g}^*)\mathfrak{m}$ is isomorphic to $\mathbf{S}(\mathfrak{h}^*)/J$, where J is the ideal of $\mathbf{S}(\mathfrak{h}^*)$ generated by $i(P_1), . . . , i(P_l)$. By Th. 1 and Chap. V, §5, no. 2, Th. $2,\mathbf{S}(\mathfrak{h}^*)/J$ is a finite dimensional vector space, and hence so is $\mathbf{S}(\mathfrak{g}^*)/\mathfrak{m}$. By a result of Commutative Algebra, it follows that $(P_1, . . . ,P_l,Q_1, . . . ,Q_{N-l})$ is an $\mathbf{S}(\mathfrak{g}^*$)-regular sequence, and a fortiori so is $(P_1, . . . ,P_l)$.

$^3$ It can be shown (B. KOSTANT, Lie group representations on polynomial rings,

Amer. J. Math., Vol. LXXXV (1963), pp. 327-404, Th. 10 and 15) that $\mathfrak{p}$ is a

prime ideal of $\mathbf{S}(\mathfrak{a}^*)$ and that $\mathbf{S}(\mathfrak{a}^*)/\mathfrak{p}$ is integrally closed.

#### Remark 2 {#lie-viii-s8-n3-rem-2 .statement tag=01L6}

The algebra $\mathbf{S}(\mathfrak{a}^*)$ is a graded free module over I. Indeed, this follows from Prop. 4, Remark 1, and Chap. V, §5, no. 5, Lemma $5._*$

### 4. PROPERTIES OF Aut0

#### Lemma 6 {#lie-viii-s8-lem-6 .statement tag=015G}

Let V be a finite dimensional vector space, G a finite group of automorphisms of V, and $v$ and $v'$ elements of V such that $v'\in /Gv$. There exists a G-invariant polynomial function $f$ on V such that $f(v')\not=f(v)$.

Indeed, for each $s\in G$ there exists a polynomial function $g_s$ on V equal to 1 at $v$ and to 0 at $sv'$. Then the function $g= 1-\prod_{s\in G}g_s$ is equal to 0 at

$v$ and to 1 on $Gv'$. The polynomial function $f=\prod_{t\in g}t.g$ is G-invariant, equal to 0 at $v$ and to 1 at $v'$.

#### Proposition 6 {#lie-viii-s8-prop-6 .statement tag=015H}

Let $\mathfrak{a}$ be a semi-simple Lie algebra and $s\in$ Aut($\mathfrak{a}$). The following conditions are equivalent:

(i) $s\in$ Aut$_0(\mathfrak{a})$;

(ii) for any invariant polynomial function $f$ on $\mathfrak{a}$, we have $f\circ s=f$.

By extending scalars if necessary, we can assume that $k$ is algebraically closed. The implication (i) $=\Rightarrow$ (ii) follows from Prop. 3. We assume that condition (ii) is satisfied and prove (i). In view of Prop. 3, and §5, no. 3, Cor. 1 of Prop. 5, we can assume that $s\in$ Aut($\mathfrak{g},\mathfrak{h}$) and that $s$ leaves stable a Weyl chamber C. Let $x\in C\cap \mathfrak{h}_{\mathbf{Q}}$. We have $sx\in C$. If $g$ is a W-invariant polynomial function on $\mathfrak{h}$, we have $g(x) =g(sx)$ (Th. 1 (i)). By Lemma 6, it follows that $sx\in Wx$. Since $sx\in C$, we have $x=sx$ (Chap. V, §3, no. 3, Th. 2). Then $s|\mathfrak{h}=$ Id$_{\mathfrak{h}}$, and $s\in$ Aut$_0(\mathfrak{g},\mathfrak{h}) ($§5, no. 2, Prop. 4).

#### Corollary {#lie-viii-s8-n4-cor-1 .statement tag=015I}

The group Aut$_0(\mathfrak{a})$ is open and closed in Aut($\mathfrak{a}$) in the Zariski topology.

Prop. 6 shows that Aut$_0(\mathfrak{a})$ is closed. Let $\overline{k}$ be an algebraic closure of $k$. The group Aut($\mathfrak{a}\otimes \overline{k}$)$/$Aut$_0(\mathfrak{a}\otimes \overline{k})$ is finite (§5, no. 3, Cor. 1 of Prop. 5); a fortiori, the group Aut($\mathfrak{a}$)$/$Aut$_0(\mathfrak{a})$ is finite. Since the cosets of Aut($\mathfrak{a}$) in Aut($\mathfrak{a}$) are closed, it follows that Aut$_0(\mathfrak{a})$ is open in Aut($\mathfrak{a}$).

### 5. CENTRE OF THE ENVELOPING ALGEBRA

In this number, we choose a basis B of R. Let $R_+$ be the set of positive roots relative to B. Let $\rho =\frac{1}{2}\sum_{\alpha\in R_+}\alpha$, and $\delta$ the automorphism of the algebra $\mathbf{S}(\mathfrak{h})$ that takes every $x\in \mathfrak{h}$ to $x-\rho (x)$, and hence the polynomial function $p$ on $\mathfrak{h}^*$ to the function $\lambda  \rightarrow p(\lambda -\rho )$.

#### Theorem 2 {#lie-viii-s8-thm-2 .statement tag=015J}

Let U be the enveloping algebra of $\mathfrak{g}$, Z its centre, $V\subset U$ the enveloping algebra of $\mathfrak{h}($identified with $\mathbf{S}(\mathfrak{h}))$, $U^0$ the commutant of V in U, $\varphi$ the *Harish-Chandra homomorphism* (§6, no. 4) from $U^0$ to $V$ relative to $B$.

Let $S(\mathfrak h)^W$ be the set of elements of $S(\mathfrak h)$ invariant under the action of $W$. Then $(\delta\circ\varphi)|_Z$ is an isomorphism from $Z$ to $S(\mathfrak h)^W$, independent of the choice of $B$.

a) Let $P_{++}$ be the set of dominant weights of $R$, $w\in W$, $\lambda\in P_{++}$, $\mu=w\lambda$. Then $Z(\mu-\rho)$ is isomorphic to a submodule of $Z(\lambda-\rho)$ (§6, no. 3, Cor. 2 of Prop. 6), and $\varphi(u)(\lambda-\rho)=\varphi(u)(\mu-\rho)$ for all $u\in Z$ (§6, no. 4, Prop. 7). Thus, the polynomial functions $(\delta\circ\varphi)(u)$ and $(\delta\circ\varphi)(u)\circ w$ on $\mathfrak h^*$ coincide on $P_{++}$. But $P_{++}$ is *dense* in $\mathfrak h^*$ in the Zariski topology: this can be seen by identifying $\mathfrak h^*$ with $k^B$ by means of the basis consisting of the fundamental weights $\varpi_\alpha$, and by applying Prop. 9 of *Algebra*, Chap. IV, §2, no. 3. Hence

$$
(\delta\circ\varphi)(u)=(\delta\circ\varphi)(u)\circ w,
$$

which proves that $(\delta\circ\varphi)(Z)\subset S(\mathfrak h)^W$.

b) Let $\eta$ be the isomorphism from $I(\mathfrak g)$ to $S(\mathfrak h)^W$ defined in no. 3, Cor. 2 of Th. 1. Consider the canonical isomorphism from the $\mathfrak g$-module $U$ to the $\mathfrak g$-module $S(\mathfrak g)$ (Chap. I, §2, no. 8), and let $\theta$ be its restriction to $Z$. Then $\theta(Z)=I(\mathfrak g)$. Let $z$ be an element of $Z$ with filtration $\leqslant f$ in $U$.

$$
\begin{array}{ccc}
Z & \xrightarrow{\theta} & I(\mathfrak g)\\
\Big\downarrow{\scriptstyle\varphi} & & \Big\downarrow{\scriptstyle\eta}\\
S(\mathfrak h) & \xrightarrow{\delta} & S(\mathfrak h).
\end{array}
$$

Introduce the notations of §6, no. 4, and put

$$
z=
\sum_{\sum q_i+\sum m_i+\sum p_i\leqslant f}
\lambda_{(q_i),(m_i),(p_i)}
u((q_i),(m_i),(p_i)).
$$

Let $v((q_i),(m_i),(p_i))$ be the monomial
$X_{\alpha_1}^{q_1}\cdots X_{\alpha_n}^{q_n}H_1^{m_1}\cdots H_l^{m_l}X_{\alpha_1}^{p_1}\cdots X_{\alpha_n}^{p_n}$
calculated in $S(\mathfrak g)$. Denoting by $S_d(\mathfrak g)$ the sum of the homogeneous components of $S(\mathfrak g)$ of degrees $0,1,\ldots,d$, we have

$$
\theta(z)\equiv
\sum_{\sum q_i+\sum m_i+\sum p_i=f}
\lambda_{(q_i),(m_i),(p_i)}v((q_i),(m_i),(p_i))
\pmod{S_{f-1}(\mathfrak g)}
$$

so

$$
(\eta\circ\theta)(z)\equiv
\sum_{\sum m_i=f}
\lambda_{(0),(m_i),(0)}v((0),(m_i),(0))
\pmod{S_{f-1}(\mathfrak h)}
$$

and consequently

$$
(\eta\circ\theta)(z)\equiv\varphi(z)
\pmod{S_{f-1}(\mathfrak h)}.
\tag{3}
$$

c) We show that $\delta\circ\varphi:Z\longrightarrow S(\mathfrak h)^W$ is bijective. The canonical filtrations on $U$ and $S(\mathfrak g)$ induce filtrations on $Z$, $I(\mathfrak g)$ and $S(\mathfrak h)^W$, and $\theta$, $\eta$ are compatible with these filtrations, so that gr($\eta \circ \theta$ ) is an isomorphism from the vector space gr(Z) to the vector space gr($\mathbf{S}(\mathfrak{h})^W$). By (3), gr($\varphi$ ) $=$ gr($\eta \circ \theta$ ), and it is clear that gr($\delta$ ) is the identity. Hence gr($\delta \circ \varphi$ ) is bijective, so

$$
\delta \circ \varphi : Z\rightarrow \mathbf{S}(\mathfrak{h})^W
$$

is bijective (Commutative Algebra, Chap. III, §2, no. 8, Cor. 1 and 2 of Th. 1).

$d)$ Recall the notations in $a)$. Let E be a simple $\mathfrak{g}$-module of highest weight $\lambda$, and $\chi$ its central character (§6, no. 1, Def. 2). Let $\varphi '$ and $\delta '$ be the homomorphisms analogous to $\varphi$ and $\delta$ relative to the basis $w(B)$. The highest weight of E relative to $w(B)$ is $w(\lambda )$. By §6, no. 4, Prop. 7,

$$
\varphi (u)(\lambda ) =\chi (u) =\varphi '(u)(w\lambda )
$$

for all $u\in Z$, so, by $a)$,

$$
(\delta \circ \varphi )(u)(w\lambda +w\rho ) = (\delta \circ \varphi )(u)(\lambda +\rho ) =\varphi (u)(\lambda ) =\varphi '(u)(w\lambda )
$$

$$
= (\delta '\circ \varphi ')(u)(w\lambda +w\rho )
$$

Thus, the polynomial functions $(\delta \circ \varphi )(u)$ and $(\delta '\circ \varphi ')(u)$ coincide on $w(P_{++}) +w\rho$, and hence are equal.

#### Corollary 1 {#lie-viii-s8-thm-2-cor-1 .statement tag=015K}

For all $\lambda \in \mathfrak{h}^*$, let $\chi_{\lambda}$ be the homomorphism $z \rightarrow (\varphi (z))(\lambda )$ from Z to $k$.

(i) If $k$ is algebraically closed, every homomorphism from Z to $k$ is of the form $\chi_{\lambda}$ for some $\lambda \in \mathfrak{h}^*$.

(ii) Let $\lambda , \mu\in \mathfrak{h}^*$. Then $\chi_{\lambda}=\chi_\mu$ if and only if $\mu+\rho \in W(\lambda +\rho )$.

If $k$ is algebraically closed, every homomorphism from $\mathbf{S}(\mathfrak{h})^W$ to $k$ extends to a homomorphism from $\mathbf{S}(\mathfrak{h})$ to $k($Commutative Algebra, Chap. V, §1, no. 9, Prop. 22, and §2, no. 1, Cor. 4 of Th. 1), and every homomorphism from $\mathbf{S}(\mathfrak{h})$ to $k$ is of the form $f \rightarrow f(\lambda )$ for some $\lambda \in \mathfrak{h}^*$ (Chap. VII, App. I, Prop. 1). Hence, if $\chi$ is a homomorphism from Z to $k$, there exists (Th. 2) a $\mu\in \mathfrak{h}^*$ such that, for all $z\in Z$,

$$
\chi (z) = ((\delta \circ \varphi )(z))(\mu) = (\varphi (z))(\mu-\rho )
$$

hence (i).

Let $\lambda , \mu\in \mathfrak{h}^*$ and assume that $\chi_{\lambda}=\chi_\mu$. Then, for all $z\in Z$,

$$
((\delta \circ \varphi )(z))(\lambda +\rho ) = (\varphi (z))(\lambda ) =\chi_{\lambda}(z) =\chi_\mu(z) = ((\delta \circ \varphi )(z))(\mu+\rho )
$$

in other words, the homomorphisms from $\mathbf{S}(\mathfrak{h})$ to $k$ defined by $\lambda +\rho$ and $\mu+\rho$ coincide on $\mathbf{S}(\mathfrak{h})^W$; thus, assertion (ii) follows from Commutative Algebra, Chap. V, §2, no. 2, Cor. of Th. 2.

#### Corollary 2 {#lie-viii-s8-thm-2-cor-2 .statement tag=015L}

Let $E,E'$ be finite dimensional simple $\mathfrak{g}$-modules, and $\chi , \chi '$ their central characters. If $\chi =\chi '$, E and $E'$ are isomorphic.

Let $\lambda , \lambda '$ be the highest weights of $E,E'$. By §6, no. 4, Prop. $7,\chi_{\lambda}=\chi =$ $\chi '=\chi_{\lambda'}$, so there exists $w\in W$ such that $\lambda '+\rho =w(\lambda +\rho )$. Since $\lambda +\rho$ and $\lambda '+\rho$ belong to the chamber defined by B, we have $w= 1$. Thus, $\lambda =\lambda '$, hence the corollary.

#### Proposition 7 {#lie-viii-s8-prop-7 .statement tag=015M}

For any class $\gamma$ of finite dimensional simple $\mathfrak{g}$-modules, let $U_{\gamma}$ be the isotypical component of type $\gamma$ of the $\mathfrak{g}$-module U (for the adjoint representation of $\mathfrak{g}$ on U). Let $\gamma_0$ be the class of the trivial $\mathfrak{g}$-module of dimension 1. Let $[U,U]$ be the vector subspace of U generated by the brackets of pairs of elements of U.

(i) U is the direct sum of the $U_{\gamma}$.

(ii) $U_{\gamma_0}= Z$, and $\sum_{\gamma\not=\gamma_0}U_{\gamma}= [U,U]$.

(iii) Let $u \rightarrow u^{\natural}$ be the projection of U onto Z defined by the decomposition $U = Z\oplus [U,U]$. If $u\in U$ and $v\in U$, we have $(uv)^{\natural}= (vu)^{\natural}$. If $u\in U$ and $z\in Z$, we have $(uz)^{\natural}=u^{\natural}z$.

(iv) Let $\varphi$ be the Harish-Chandra homomorphism. Let $\lambda \in P_{++}$, and let E be a finite dimensional simple $\mathfrak{g}$-module of highest weight $\lambda$. For all $u\in U$, we have

1 $\natural$

Tr($u_E$) $= (\varphi (u))(\lambda )$.

dim E

The $\mathfrak{g}$-module U is a direct sum of finite dimensional submodules. This implies (i).

It is clear that $U_{\gamma_0}= Z$. Let $U'$ be a vector subspace of U defining a subrepresentation of class $\gamma$ of the adjoint representation. Then either $[\mathfrak{g},U'] = U'$ or $[\mathfrak{g},U'] = 0$. Thus, if $\gamma \not=\gamma_0$ then $[\mathfrak{g},U'] = U'$, so $\sum_{\gamma\not=\gamma_0}U_{\gamma}\subset [U,U]$. On the other hand, if $u\in U$ and $x_1, . . . , x_n\in \mathfrak{g}$, then

$$
[x_1. . . x_n, u] = (x_1. . . x_nu-x_2. . . x_nux_1)+(x_2. . . x_nux_1-x_3. . . x_nux_1x_2)
$$

$$
+\cdots + (x_nux_1. . . x_{n-1}-ux_1. . . x_n)\in [\mathfrak{g},U]
$$

Hence $[U,U]\subset [\mathfrak{g},\sum_{\gamma}U_{\gamma}]=[\mathfrak{g},\sum_{\gamma\not=\gamma_0}U_{\gamma}]\subset \sum_{\gamma\not=\gamma_0}U_{\gamma}$. This proves (ii). Under these conditions, (iii) follows from Chap. I, §6, no. 9, Lemma 5.

Finally, let $E, \lambda$ be as in (iv). Then

Tr($u_E$) $=$ Tr(($u^{\natural}$)$_E)$ since $u-u^{\natural}\in [U,U]$

= Tr($\varphi (u^{\natural})(\lambda ).1$) (§$6$, no$.4$, Prop$.7)$

= (dim $E).\varphi (u^{\natural})(\lambda )$.

### Exercises {#lie-viii-s8-exercises}

See the [exercises for § 8](exercises/s8/).
