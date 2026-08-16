---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 5
section_title: Automorphisms of a semi-simple Lie algebra
lang: en
source: lie-vii-ix
book_pages: 106-115, 233-237
pdf_pages: 0114-0123, 0241-0245
extraction: native+ocr
subsections:
    - "no": 1
      title: AUTOMORPHISMS OF A FRAMED SEMI-SIMPLE LIE ALGEBRA
      page: 106
      pdf_page: 114
    - "no": 2
      title: AUTOMORPHISMS OF A SPLIT SEMI-SIMPLE LIE ALGEBRA
      page: 107
      pdf_page: 115
    - "no": 3
      title: AUTOMORPHISMS OF A SPLITTABLE SEMI-SIMPLE LIE ALGEBRA
      page: 111
      pdf_page: 119
    - "no": 4
      title: ZARISKI TOPOLOGY ON Aut($\mathfrak{g}$)
      page: 113
      pdf_page: 121
    - "no": 5
      title: LIE GROUP CASE
      page: 115
      pdf_page: 123
statements: 25
exercises: 13
errata:
    - says: Chap. VII, §13, no. 1
      read: Chap. VIII, §13, no. 1
      why: Chapter VII has five sections and no section 13. The sentence says that the groups Aut$_0(\mathfrak{g})$ and Aut$_e(\mathfrak{g})$ can be distinct, and the place that shows it is no. 1 of section 13 of this chapter, on the algebras of type $A_l$, which computes Aut$_0(\mathfrak{g}) =\varphi (\mathbf{G}\mathbf{L}(l+ 1, k))$, identifies the quotient Aut$_0(\mathfrak{g})/$Aut$_e(\mathfrak{g})$ with $\mathbf{P}\mathbf{G}\mathbf{L}(l+ 1, k)/\mathbf{P}\mathbf{S}\mathbf{L}(l+ 1, k)$, and over the reals finds it isomorphic to $\mathbf{Z}/2\mathbf{Z}$ when $l+1$ is even. Chapter VII names neither group anywhere.
content_sha256: 4cb0cd2d76b32556fcf2dcae97fad2bc7fee6d517c3dcfb35b54bd9480118d79
---

## § 5. AUTOMORPHISMS OF A SEMI-SIMPLE LIE ALGEBRA

In this paragraph, $\mathfrak{g}$ denotes a semi-simple Lie algebra.

### 1. AUTOMORPHISMS OF A FRAMED SEMI-SIMPLE LIE ALGEBRA

Recall (Chap. VII, §3, no. 1) that Aut($\mathfrak{g}$) denotes the group of automorphisms of $\mathfrak{g}$. If $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{g}$, we denote by Aut($\mathfrak{g},\mathfrak{h}$) the group of automorphisms of $\mathfrak{g}$ that leave $\mathfrak{h}$ stable. Assume that $\mathfrak{h}$ is splitting, and let R be the root system of $(\mathfrak{g},\mathfrak{h})$. If $s\in$ Aut($\mathfrak{g},\mathfrak{h}$), the contragredient map of $s|\mathfrak{h}$ is an element of A(R) (the group of automorphisms of R) which we shall denote by $\varepsilon (s)$ in this paragraph. Thus

$\varepsilon :$ Aut($\mathfrak{g},\mathfrak{h}$)$\rightarrow A(R)$

is a homomorphism of groups.

For any root system R and any basis B of R, we denote by Aut(R$,B)$ the group of automorphisms of R that leave B stable. Recall (Chap. VI, §1, no. 5, Prop. 16 and §4, no. 2, Cor. of Prop. 1) that A(R) is the semi-direct product of Aut(R$,B)$ and W(R), and that $A(R)/W(R)$ is canonically isomorphic to the group of automorphisms of the Dynkin graph of R.

#### Proposition 1 {#lie-viii-s5-prop-1 .statement tag=011N}

Let $(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$ be a framed semi-simple Lie algebra, and R the root system of $(\mathfrak{g},\mathfrak{h})$. Let G be the set of $s\in$ Aut($\mathfrak{g},\mathfrak{h}$) that leave B stable, and such that $s(X_{\alpha}) =X_{\varepsilon(s)\alpha}$ for all $\alpha \in B ($in other words the set of automorphisms of $(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B}))$. Then the restriction of $\varepsilon$ to G is an isomorphism from G to Aut(R$,B)$.

If $s\in G$, it is clear that $\varepsilon (s)\in$ Aut(R$,B)$. On the other hand, the map

$\varepsilon |G : G\rightarrow$ Aut(R$,B)$

is bijective by Th. 2 of §4, no. 4.

### 2. AUTOMORPHISMS OF A SPLIT SEMI-SIMPLE LIE ALGEBRA

Let E be a commutative group, and $A =\bigoplus_{\gamma\in E}A^{\gamma}$ an E-graded algebra. For any homomorphism $\varphi$ from the group E to the multiplicative group $k^*$, let $f(\varphi )$ be the $k$-linear map from A to A whose restriction to each $A^{\gamma}$ is the homothety with ratio $\varphi (\gamma )$; it is clear that $f(\varphi )$ is an automorphism of the graded algebra A, and that $f$ is a homomorphism from the group Hom(E$, k^*)$ to the group of automorphisms of the graded algebra A.

Let $\mathfrak{h}$ be a splitting Cartan subalgebra of $\mathfrak{g}$, and R the root system of $(\mathfrak{g},\mathfrak{h})$. Recall that P(R) (resp. Q(R)) denotes the group of weights (resp. radical weights) of R. Put

$T_P=$ Hom(P(R)$, k^*)T_Q=$ Hom(Q(R)$, k^*)$.

We can consider $\mathfrak{g}=\mathfrak{g}^0+\sum_{\alpha\in R}\mathfrak{g}^{\alpha}$ as a Q(R)-graded algebra. The preceding remarks define a canonical homomorphism from $T_Q$ to Aut($\mathfrak{g},\mathfrak{h}$), which will be denoted by $f$ in this paragraph. In the other hand, the canonical injection from Q(R) to P(R) defines a homomorphism from $T_P$ to $T_Q$, which will be denoted by $q:$

$T_P\longrightarrow^qT_Q\longrightarrow^f$ Aut($\mathfrak{g},\mathfrak{h}$).

If $s\in$ Aut($\mathfrak{g},\mathfrak{h}$), let $s^*$ be the restriction of $^t(s|\mathfrak{h})^{-1}$ to Q(R). Then, for all $\varphi \in T_Q$,

$$
f(\varphi \circ s^*) =s^{-1}\circ f(\varphi )\circ s \tag{1}
$$

Indeed, let $\gamma \in Q(R)$ and $x\in \mathfrak{g}^{\gamma}$; then $sx\in \mathfrak{g}^{s^*\gamma}$ and

$$
f(\varphi \circ s^*)x= (\varphi \circ s^*)(\gamma ).x=s^{-1}(\varphi (s^*\gamma )sx) = (s^{-1}\circ f(\varphi )\circ s)(x)
$$

#### Proposition 2 {#lie-viii-s5-prop-2 .statement tag=011O}

The sequence of homomorphisms

1 $\longrightarrow T_Q\longrightarrow^f$ Aut($\mathfrak{g},\mathfrak{h}$)$\longrightarrow^{\varepsilon}$ A(R) $\longrightarrow$ 1

is exact.

$a)$ Let $\varphi \in$ Ker $f$. Then $\varphi (\alpha ) = 1$ for all $\alpha \in R$. Since R generates the group $Q(R),\varphi$ is the identity element of $T_Q$.

$b)$ Let $\varphi \in T_Q$. The restriction of $f(\varphi )$ to $\mathfrak{h}=\mathfrak{g}^0$ is the identity, so

Im $f\subset$ Ker$\varepsilon$.

$c)$ Let $s\in$ Ker$\varepsilon$. Then $s|\mathfrak{h}=$ Id$_{\mathfrak{h}}$. For all $\alpha \in R$, we have $s(\mathfrak{g}^{\alpha}) =\mathfrak{g}^{\alpha}$, and there exists a $t_{\alpha}\in k^*$ such that $sx=t_{\alpha}x$ for all $x\in \mathfrak{g}^{\alpha}$. Writing down the condition that $s\in$ Aut($\mathfrak{g}$), we obtain the relations

$t_{\alpha}t_{-\alpha}= 1$ for all $\alpha \in R$

$t_{\alpha}t_{\beta}=t_{\alpha+\beta}$ when $\alpha , \beta , \alpha +\beta \in R$.

Under these conditions, there exists $\varphi \in T_Q$ such that $\varphi (\alpha ) =t_{\alpha}$ for all $\alpha \in R$ (Chap. VI, §1, no. 6, Cor. 2 of Prop. 19). Then $s=f(\varphi )$. Hence, Ker $\varepsilon \subset$ Im $f$.

$d)$ The image of Aut($\mathfrak{g},\mathfrak{h}$) under $\varepsilon$ contains W(R) by §2, no. 2, Cor. of Th. 2, and contains Aut(R$,B)$ by Prop. 1. Hence this image is equal to A(R).

#### Corollary 1 {#lie-viii-s5-prop-2-cor-1 .statement tag=011P}

Let $(B,(X_{\alpha})_{\alpha\in B})$ be a framing of $(\mathfrak{g},\mathfrak{h})$. Let G be the set of $s\in$ Aut($\mathfrak{g},\mathfrak{h}$) that leave the framing invariant. Then Aut($\mathfrak{g},\mathfrak{h}$) is the semi-direct product of G and $\varepsilon^{-1}(W(R))$.

Indeed, $G\cap \varepsilon^{-1}(W(R)) =\{1\}$ by Prop. 1, and

Aut($\mathfrak{g},\mathfrak{h}$) $= G.\varepsilon^{-1}(W(R))$

since $\varepsilon$ is surjective (Prop. 2).

#### Corollary 2 {#lie-viii-s5-prop-2-cor-2 .statement tag=011Q}

The group $\varepsilon^{-1}(W(R))$ operates simply-transitively on the set of framings of $(\mathfrak{g},\mathfrak{h})$.

Indeed, Aut($\mathfrak{g},\mathfrak{h}$) operates transitively on the set of framings of $(\mathfrak{g},\mathfrak{h})$ by §4, no. 4, Th. 2. Cor. 2 now follows from Cor. 1.

#### Corollary 3 {#lie-viii-s5-prop-2-cor-3 .statement tag=011R}

Let B be a basis of R. The group Ker $\varepsilon =f(T_Q)$ operates simply-transitively on the set of framings of $(\mathfrak{g},\mathfrak{h})$ of the form $(B,(X_{\alpha})_{\alpha\in B})$.

This follows immediately from Prop. 2.

Let $\alpha \in R,X_{\alpha}\in \mathfrak{g}^{\alpha},X_{-\alpha}\in \mathfrak{g}^{-\alpha}$ be such that $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$. We have seen (§2, no. 2, Th. 2) that, for all $t\in k^*$, the restriction of the elementary automorphism

$$
\theta_{\alpha}(t) =e^{adtX_{\alpha}}e^{adt^{-1}X_{-\alpha}}e^{adtX_{\alpha}}
$$

to $\mathfrak{h}$ is the transpose of $s_{\alpha}$; so $\varepsilon (\theta_{\alpha}(t)) =s_{\alpha}$ and consequently $\theta_{\alpha}(t)\theta_{\alpha}(-1)\in$ Ker $\varepsilon$.

#### Lemma 1 {#lie-viii-s5-lem-1 .statement tag=011S}

Let $\alpha \in R$ and $t\in k^*$. Let $\varphi$ be the homomorphism $\lambda  \rightarrow t^{\lambda(H_{\alpha})}$ from Q(R) to $k^*$. Then $f(\varphi ) =\theta_{\alpha}(t)\theta_{\alpha}(-1)$.

Let $\rho$ be the representation of $\mathfrak{s}\mathfrak{l}(2, k)$ on $\mathfrak{g}$ associated to $X_{\alpha}$. Let $\pi$ be the representation of $\mathbf{S}\mathbf{L}(2, k)$ compatible with $\rho$. Introduce the notations $\theta (t), h(t)$ of §1, no. 5. Since $\rho (H) =$ ad $H_{\alpha}$, the elements of $\mathfrak{g}^{\lambda}$ are of weight $\lambda (H_{\alpha})$ for $\rho$. By §2, no. $2,\theta_{\alpha}(t)\theta_{\alpha}(-1) =\pi (\theta (t)\theta (-1)) =\pi (h(t))$. Hence the restriction of $\theta_{\alpha}(t)\theta_{\alpha}(-1)$ to $\mathfrak{g}^{\lambda}$ is the homothety of ratio $t^{\lambda(H_{\alpha})}($§1, no. 5, Prop. 6), hence the lemma.

#### Proposition 3 {#lie-viii-s5-prop-3 .statement tag=011T}

The image of the composite homomorphism

$T_P\longrightarrow^qT_Q\longrightarrow^f$ Aut($\mathfrak{g},\mathfrak{h}$)

is contained in Aut$_e(\mathfrak{g})$.

Let B be a basis of R. Then $(H_{\alpha})_{\alpha\in B}$ is a basis of $R^{\vee}$, and the dual basis of $(H_{\alpha})_{\alpha\in B}$ in $\mathfrak{h}^*$ is a basis of the group P(R). Hence the group $T_P$ is generated by the homomorphisms $\lambda  \rightarrow t^{\lambda(H_{\alpha})}(t\in k^*, \alpha \in B)$. If $\varphi$ is the restriction of such a homomorphism to Q(R), Lemma 1 proves that $f(\varphi )\in$ Aut$_e(\mathfrak{g})$, hence the proposition.

Let $\overline{k}$ be an algebraic closure of $k$. The map which associates to any automorphism $s$ of $\mathfrak{g}$ the automorphism $s\otimes 1$ of $\mathfrak{g}\otimes_k\overline{k}$ is an injective homomorphism from Aut($\mathfrak{g}$) to Aut($\mathfrak{g}\otimes_k\overline{k}$). We denote by Aut$_0(\mathfrak{g})$ the normal subgroup of Aut($\mathfrak{g}$) which is the inverse image of Aut$_e(\mathfrak{g}\otimes_k\overline{k})$ under this homomorphism; this is the set of automorphisms of $\mathfrak{g}$ that become elementary on extending the base field from $k$ to $\overline{k}$. It is clear that Aut$_e(\mathfrak{g})$ is independent of the choice of $\overline{k}$, and that Aut$_e(\mathfrak{g})\subset$ Aut$_0(\mathfrak{g})$. The groups Aut$_0(\mathfrak{g})$ and Aut$_e(\mathfrak{g})$ can be distinct (Chap. VII, §13, no. 1). If $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{g}$, put

Aut$_e(\mathfrak{g},\mathfrak{h}) =$ Aut$_e(\mathfrak{g})\cap$ Aut($\mathfrak{g},\mathfrak{h}$), Aut$_0(\mathfrak{g},\mathfrak{h}) =$ Aut$_0(\mathfrak{g})\cap$ Aut($\mathfrak{g},\mathfrak{h}$).

#### Lemma 2 {#lie-viii-s5-lem-2 .statement tag=011U}

Let $\mathfrak{h}$ be a splitting Cartan subalgebra of $\mathfrak{g}$, and $s\in$ Aut$_0(\mathfrak{g},\mathfrak{h})$. Assume that the restriction of $s$ to $\sum_{\alpha\in R}\mathfrak{g}^{\alpha}$ does not have 1 as an eigenvalue.

Then $\varepsilon (s) = 1$.

By extension of $k$, we are reduced to the case where $s\in$ Aut$_e(\mathfrak{g},\mathfrak{h})$. The dimension of the nilspace of $s-1$ is at least dim $\mathfrak{h}$ (Chap. VII, §4, no. 4, Prop. 9). Hence $(s-1)|\mathfrak{h}$ is nilpotent. Since $s|\mathfrak{h}\in A(R^{\vee}),s|\mathfrak{h}$ is of finite order, and hence semi-simple (Chap. V, Appendix, Prop. 2). Consequently, $(s-1)|\mathfrak{h}= 0$, which proves that $\varepsilon (s) = 1$.

#### Lemma 3 {#lie-viii-s5-lem-3 .statement tag=011V}

(i) Let $m= (P(R) : Q(R))$. If $\varphi$ is the $m$th power of an element of $T_Q$, then $\varphi \in q(T_P)$.

(ii) If $k$ is algebraically closed, $q(T_P) = T_Q$.

There exist a basis $(\lambda_1, . . . , \lambda_l)$ of P(R) and integers $n_1\geq 1, . . . , n_l\geq 1$ such that $(n_1\lambda_1, . . . , n_l\lambda_l)$ is a basis of Q(R). We have $m=n_1. . . n_l$. Let $\psi \in T_Q$ and put $\psi (n_1\lambda_1) =t_1, . . . , \psi (n_l\lambda_l) =t_l$. For $i= 1, . . . , l$, put $m_i=$ $\prod_{j\not=i}n_j$. Let $\chi$ be the element of $T_P$ such that $\chi (\lambda_1) =t^m_{1^1}, . . . , \chi (\lambda_l) =t^m_{l^l}$. Then

$$
\chi (n_i\lambda_i) =t^m_{i^i}^{n_i}=t^m_i= (\psi^m)(n_i\lambda_i)
$$

so $\chi |Q(R) =\psi^m$. This proves (i). If $k$ is algebraically closed, every element of $k^*$ is the $m$th power of an element of $k^*$, so every element of $T_Q$ is the $m$th power of an element of $T_Q$; hence, (ii) follows from (i).

#### Proposition 4 {#lie-viii-s5-prop-4 .statement tag=011W}

We have $f(T_Q)\subset$Aut$_0(\mathfrak{g},\mathfrak{h})$ and $\varepsilon^{-1}(W(R)) =$ Aut$_0(\mathfrak{g},\mathfrak{h})$.

$a)$ Let $\varphi \in T_Q$ and let $\overline{k}$ be an algebraic closure of $k$. By Lemma $3,\varphi$ extends to an element of Hom(P(R)$, k^*)$. By Prop. 3,

$f(\varphi )\otimes 1\in$ Aut$_e(\mathfrak{g}\otimes_k\overline{k},\mathfrak{h}\otimes_k\overline{k})$.

Hence $f(\varphi )\in$ Aut$_0(\mathfrak{g},\mathfrak{h})$, and Ker $\varepsilon \subset$ Aut$_0(\mathfrak{g},\mathfrak{h})$.

$b)$ The image of Aut$_e(\mathfrak{g},\mathfrak{h})$ under $\varepsilon$ contains W(R) (§2, no. 2, Cor. of Th. 2). In view of $a)$, we see that $\varepsilon^{-1}(W(R))\subset$ Aut$_0(\mathfrak{g},\mathfrak{h})$.

$c)$ It remains to prove that Aut$_0(\mathfrak{g},\mathfrak{h})\subset \varepsilon^{-1}(W(R))$. In view of $b)$, it suffices to prove that $\varepsilon$(Aut$_0(\mathfrak{g},\mathfrak{h}))\cap$ Aut(R$,B)$, where B denotes a basis of R, reduces to $\{1\}$.

Let $s\in$ Aut$_0(\mathfrak{g},\mathfrak{h})$ be such that $\varepsilon (s)\in$ Aut(R$,B)$. The subgroup of A(R) generated by $\varepsilon (s)$ has a finite number of orbits on R. Let U be such an orbit, of cardinal $r$, and $\mathfrak{g}^U=\sum_{\beta\in U}\mathfrak{g}^{\beta}$. Let $\beta_1\in U$, and put $\beta_i=\varepsilon (s)^{i-1}\beta_1$ for

$1\leq i\leq r$, so that $U =\{\beta_1, . . . , \beta_r\}$. Let $X_{\beta_1}$ be a non-zero element of $\mathfrak{g}^{\beta_1}$, and put $X_{\beta_i}=s^{i-1}X_{\beta_1}$ for $1\leq i\leq r$. There exists $c_U\in k^*$ such that $s^rX_{\beta_1}=$ $c_UX_{\beta_1}$, hence $s^rX_{\beta_i}=c_UX_{\beta_i}$ for all $i$, and consequently $s^r|\mathfrak{g}^U=c_U.1$. Let $\varphi \in T_Q$, and $s'=s\circ f(\varphi )$, which by $a)$ is an element of Aut$_0(\mathfrak{g},\mathfrak{h})$. We have ${s'}^r|\mathfrak{g}^U=c'_U.1$, where

$$
c'_U=c_U\prod_{i=1}^r\varphi (\beta_i) =c_U\varphi (\sum_{i=1}^r\beta_i)
$$

Put $B =\{\alpha_1, . . . , \alpha_l\}$ and $\sum_{i=1}^r\beta_i=\sum_{j=1}^lm^U_j\alpha_j$. Since $\varepsilon (s)\in$ Aut(R$,B)$, the

$m^U_j$ are integers of the same sign and not all zero. We have

$$
c'_U=c_U\prod_{j=1}^l\varphi (\alpha_j)^{m^U_j}
$$

Now $\varphi$ can be chosen so that $c'_U\not= 1$ for every orbit U; indeed, this reduces to choosing elements $\varphi (\alpha_1) =t_1, . . . , \varphi (\alpha_l) =t_l$ of $k^*$ which are not annihilated by a finite number of polynomials in $t_1, . . . , t_l$, not identically zero. For such a choice of $\varphi ,\varepsilon (s') = 1$ by Lemma 2, so

$$
\varepsilon(s)=\varepsilon(s')\varepsilon(f(\varphi))^{-1}=1.
$$

#### Corollary {#lie-viii-s5-n2-cor-1 .statement tag=01J0}

— Let $B$ be a basis of $R$. The group $\operatorname{Aut}(\mathfrak g,\mathfrak h)$ is isomorphic to the semi-direct product of the groups $\operatorname{Aut}(R,B)$ and $\operatorname{Aut}_0(\mathfrak g,\mathfrak h)$.

This follows from Prop. 1, Cor. 1 of Prop. 2, and Prop. 4.

#### Remark {#lie-viii-s5-n2-rem-1 .statement tag=011X}

Let $\varepsilon',\varepsilon''$ be the restrictions of $\varepsilon$ to $\operatorname{Aut}_0(\mathfrak g,\mathfrak h)$, $\operatorname{Aut}_e(\mathfrak g,\mathfrak h)$. Let $f'$ be the homomorphism from $T_P$ to $\operatorname{Aut}_e(\mathfrak g,\mathfrak h)$ induced by $f$ via the canonical injection from $Q(R)$ to $P(R)$. In the preceding we have established the following commutative diagram:
$$
\begin{array}{ccccccccc}
1&\longrightarrow&T_Q&\xrightarrow{\ f\ }&\operatorname{Aut}(\mathfrak g,\mathfrak h)&\xrightarrow{\ \varepsilon\ }&A(\mathbf R)&\longrightarrow&1\\
&&\uparrow&&\uparrow&&\uparrow&&\\
1&\longrightarrow&T_Q&\xrightarrow{\ f\ }&\operatorname{Aut}_0(\mathfrak g,\mathfrak h)&\xrightarrow{\ \varepsilon'\ }&W(\mathbf R)&\longrightarrow&1\\
&&\uparrow^{q}&&\uparrow&&\uparrow&&\\
&&T_P&\xrightarrow{\ f'\ }&\operatorname{Aut}_e(\mathfrak g,\mathfrak h)&\xrightarrow{\ \varepsilon''\ }&W(\mathbf R)&\longrightarrow&1
\end{array}
$$
in which the vertical arrows other than $q$ denote the canonical injections. We have seen (Prop. 2 and 4) that the first two rows are exact. In the third row, the homomorphism $\varepsilon''$ is surjective (§2, no. 2, Cor. of Th. 2); it can be shown that its kernel is $f'(T_P)$ (§7, Exerc. 26 d)).

### 3. AUTOMORPHISMS OF A SPLITTABLE SEMI-SIMPLE LIE ALGEBRA

#### Proposition 5 {#lie-viii-s5-prop-5 .statement tag=01J1}

— Assume that $\mathfrak g$ is splittable. The group $\operatorname{Aut}_0(\mathfrak g)$ operates simply-transitively on the set of framings of $\mathfrak g$.

Let $e_1=(\mathfrak g,\mathfrak h_1,B_1,(X^1_\alpha)_{\alpha\in B_1})$, $e_2=(\mathfrak g,\mathfrak h_2,B_2,(X^2_\alpha)_{\alpha\in B_2})$ be two framings of $\mathfrak g$. There exists at least one element of $\operatorname{Aut}_0(\mathfrak g)$ that transforms $e_1$ into $e_2$ (Prop. 1 and Prop. 4). Let $\overline{k}$ be an algebraic closure of $k$. There exists an element of $\operatorname{Aut}_e(\mathfrak g\otimes_k\overline{k})$ that transforms $\mathfrak h_1\otimes_k\overline{k}$ into $\mathfrak h_2\otimes_k\overline{k}$ (Chap. VII, §3, no. 2, Th. 1). Hence, by Prop. 4 and Cor. 2 of Prop. 2, there exists an element $\varphi$ of $\operatorname{Aut}_e(\mathfrak g\otimes_k\overline{k})$ that transforms the framing $(\mathfrak g\otimes_k\overline{k},\mathfrak h_1\otimes_k\overline{k},B_1,(X^1_\alpha)_{\alpha\in B_1})$ of $\mathfrak g\otimes_k\overline{k}$ into the framing $(\mathfrak g\otimes_k\overline{k},\mathfrak h_2\otimes_k\overline{k},B_2,(X^2_\alpha)_{\alpha\in B_2})$. Since $\mathfrak h_1$ and the $X^1_\alpha$ (resp. $\mathfrak h_2$ and the $X^2_\alpha$) generate $\mathfrak g_1$ (resp. $\mathfrak g_2$), we have $\varphi(\mathfrak g_1)=\mathfrak g_2$, so $\varphi$ is of the form $\psi\otimes 1$ where $\psi\in\operatorname{Aut}_0(\mathfrak g)$, and $\psi$ transforms $e_1$ into $e_2$.

#### Corollary 1 {#lie-viii-s5-prop-5-cor-1 .statement tag=01J2}

— Let $(\mathfrak g,\mathfrak h,B,(X_\alpha)_{\alpha\in B})$ be a framing of $\mathfrak g$, and $G$ the group (isomorphic to $\operatorname{Aut}(R,B)$) of automorphisms of $\mathfrak g$ that leave this framing invariant. Then $\operatorname{Aut}(\mathfrak g)$ is the semi-direct product of $G$ and $\operatorname{Aut}_0(\mathfrak g)$.

Indeed, every element of $\operatorname{Aut}(\mathfrak g)$ transforms $(\mathfrak g,\mathfrak h,B,(X_\alpha)_{\alpha\in B})$ into a framing of $\mathfrak g$. By Prop. 5, every coset of $\operatorname{Aut}(\mathfrak g)$ modulo $\operatorname{Aut}_0(\mathfrak g)$ meets $G$ in exactly one point.

\hfill Q.E.D.

It follows from Cor. 1 that the group Aut($\mathfrak{g}$)$/$Aut$_0(\mathfrak{g})$ can be identified with Aut(R$,B)$, and is isomorphic to the group of automorphisms of the Dynkin graph of R.

#### Corollary 2 {#lie-viii-s5-prop-5-cor-2 .statement tag=01J3}

Aut($\mathfrak{g}$) $=$ Aut$_0(\mathfrak{g})$ when $\mathfrak{g}$ is a splittable simple Lie algebra of type $A_1,B_n(n\geq 2)$, $C_n(n\geq 2)$, $E_7,E_8,F_4,G_2$. The quotient Aut($\mathfrak{g}$)$/$Aut$_0(\mathfrak{g})$ is of order 2 when $\mathfrak{g}$ is of type $A_n(n\geq 2)$, $D_n(n\geq 5)$, $E_6$; it is isomorphic to $\mathfrak{S}_3$ when $\mathfrak{g}$ is of type $D_4$.

This follows from Cor. 1 and Chap. VI, Plates I to IX.

#### Remark 1 {#lie-viii-s5-n3-rem-1 .statement tag=011Z}

Let $e_1= (\mathfrak{g},\mathfrak{h}_1,B_1,(X_{\alpha}^1)_{\alpha\in B_1}),e_2= (\mathfrak{g},\mathfrak{h}_2,B_2,(X_{\alpha}^2)_{\alpha\in B_2})$, $e'_2= (\mathfrak{g},\mathfrak{h}_2,B_2,(Y_{\alpha}^2)_{\alpha\in B_2})$ be framings of $\mathfrak{g}$, and $s$ (resp. $s')$ an element of Aut$_0(\mathfrak{g})$ that transforms $e_1$ to $e_2$ (resp. $e'_2)$. Then $s|\mathfrak{h}_1=s'|\mathfrak{h}_1$. Indeed, $s^{'-1}s\in$ Aut$_0(\mathfrak{g},\mathfrak{h}_1)$ and $s^{'-1}s(B_1) = B_1$, so $\varepsilon (s^{'-1}s) = 1$.

#### Remark 2 {#lie-viii-s5-n3-rem-2 .statement tag=0120}

Let X be the set of pairs $(\mathfrak{h},B)$ where $\mathfrak{h}$ is a splitting Cartan subalgebra of $\mathfrak{g}$ and B a basis of the root system of $(\mathfrak{g},\mathfrak{h})$. If $x= (\mathfrak{h},B)$ and $x'= (\mathfrak{h}',B')$ are two elements of X, there exists $s\in$ Aut$_0(\mathfrak{g})$ that transforms $x$ into $x'$ (Prop. 5), and the restriction $s_{x',x}$ of $s$ to $\mathfrak{h}$ does not depend on the choice of $s$ (Remark 1). In particular, $s_{x'',x'}\circ s_{x',x}=s_{x'',x}$ if $x, x', x''\in X$, and $s_{x,x}= 1$. The set of families $(h_x)_{x\in X}$ satisfying the conditions

$a)h_x\in \mathfrak{h}$ if $x= (\mathfrak{h},B)$

$b)s_{x',x}(h_x) =h_{x'}$ if $x, x'\in X$

is in a natural way a vector space $\mathfrak{h}(\mathfrak{g})$ which we sometimes call the canonical Cartan subalgebra of $\mathfrak{g}$. For $x= (\mathfrak{h},B)$ and $x'= (\mathfrak{h}',B'),s_{x',x}$ takes B to $B'$, and hence the root system of $(\mathfrak{g},\mathfrak{h})$ to that of $(\mathfrak{g},\mathfrak{h}')$; it follows that the dual $\mathfrak{h}(\mathfrak{g})^*$ of $\mathfrak{h}(\mathfrak{g})$ is naturally equipped with a root system $R(\mathfrak{g})$ and with a basis $B(\mathfrak{g})$ of $R(\mathfrak{g})$. We sometimes say that $R(\mathfrak{g})$ is the canonical root system of $\mathfrak{g}$ and that $B(\mathfrak{g})$ is its canonical basis. The group Aut($\mathfrak{g}$) operates on $\mathfrak{h}(\mathfrak{g})$ leaving $R(\mathfrak{g})$ and $B(\mathfrak{g})$ stable; the elements of Aut($\mathfrak{g}$) that operate trivially on $\mathfrak{h}(\mathfrak{g})$ are those of Aut$_0(\mathfrak{g})$.

#### Proposition 6 {#lie-viii-s5-prop-6 .statement tag=0121}

Let $\mathfrak{h}$ be a splitting Cartan subalgebra of $\mathfrak{g}$. We have, with the notations in no. 1, Aut$_0(\mathfrak{g}) =$ Aut$_e(\mathfrak{g})$.Ker $\varepsilon =$ Aut$_e(\mathfrak{g}).f(T_Q)$.

By §3, no. 3, Cor. of Prop. 10, Aut$_0(\mathfrak{g}) =$ Aut$_e(\mathfrak{g})$.Aut$_0(\mathfrak{g},\mathfrak{h})$. On the other hand, $\varepsilon$(Aut$_e(\mathfrak{g},\mathfrak{h}))\supset W(R)$ by §2, no. 2, Cor. of Th. 2, so Aut$_0(\mathfrak{g},\mathfrak{h}) =$ Aut$_e(\mathfrak{g},\mathfrak{h})$.Ker$\varepsilon$.

#### Remark 3 {#lie-viii-s5-n3-rem-3 .statement tag=0122}

Prop. 6 shows that the canonical homomorphism

$\iota : T_Q/$Im(T$_P)\rightarrow$ Aut$_0(\mathfrak{g})/$Aut$_e(\mathfrak{g})$,

induced by the diagram in no. 2, is surjective. In particular, Aut$_e(\mathfrak{g})$ contains the derived group of Aut$_0(\mathfrak{g})$; we shall see (§11, no. 2, Prop. 3) that they are actually equal. Moreover, it can be shown that $\iota$ is injective, in other words that

$f(T_Q)\cap$ Aut$_e(\mathfrak{g}) =f'(T_P)$,

(cf. §7, Exerc. $26d))$.

#### Proposition 7 {#lie-viii-s5-prop-7 .statement tag=0123}

Let $\mathfrak{g}$ be a splittable semi-simple Lie algebra, $\mathfrak{b}$ a Borel subalgebra of $\mathfrak{g}$, and $\mathfrak{p}_1$ and $\mathfrak{p}_2$ distinct parabolic subalgebras of $\mathfrak{g}$ containing $\mathfrak{b}$. Then $\mathfrak{p}_1$ and $\mathfrak{p}_2$ are not conjugate under Aut$_0(\mathfrak{g})$.

We can assume that $k$ is algebraically closed. Let $s\in$ Aut$_0(\mathfrak{g})$ be such that $s(\mathfrak{p}_1) =\mathfrak{p}_2$. Let $\mathfrak{h}$ be a Cartan subalgebra of $\mathfrak{g}$ contained in $\mathfrak{b}\cap s(\mathfrak{b}) ($§3, no. 3, Prop. 10). Since $\mathfrak{h}$ and $s(\mathfrak{h})$ are Cartan subalgebras of $s(\mathfrak{b})$, there exists $u\in [\mathfrak{b},\mathfrak{b}]$ such that $e^{adu}(\mathfrak{h}) =s(\mathfrak{h})$ (Chap. VII, §3, no. 4, Th. 3). Replacing $s$ by $e^{-adu}s$, we are reduced to the case in which $s(\mathfrak{h}) =\mathfrak{h}$, and $s$ then induces on $\mathfrak{h}$ an element $\sigma$ of the Weyl group W of $(\mathfrak{g},\mathfrak{h})$ (Prop. 4). Let C be the Weyl chamber corresponding to $\mathfrak{b}$. Then $\mathfrak{p}_1$ and $\mathfrak{p}_2$ correspond to facets $F_1$ and $F_2$ of $\mathfrak{h}_{\mathbf{R}}$ contained in the closure of C. We have $\sigma (F_1) = F_2$. Since $\sigma \in W$, this implies that $F_1= F_2$ (Chap. V, §3, no. 3, Th. 2) so $\mathfrak{p}_1=\mathfrak{p}_2$.

#### Remark 4 {#lie-viii-s5-n3-rem-4 .statement tag=0124}

Let $\mathfrak{g}$ be a splittable semi-simple Lie algebra, $\mathscr{P}$ the set of parabolic subalgebras of $\mathfrak{g}$, a set on which Aut$_0(\mathfrak{g})$ operates. Retain the notations of Remark 2. Let $\Sigma$ be a subset of $B(\mathfrak{g})$. Giving $\Sigma$ is equivalent to giving, for every $x= (\mathfrak{h},B)\in X$, a subset $\Sigma_x$ of B, such that $s_{x',x}$ takes $\Sigma_x$ to $\Sigma_{x'}$ for any $x, x'\in X$. Let $\mathfrak{p}_x$ be the parabolic subalgebra of $\mathfrak{g}$ corresponding to $\Sigma_x$ (§3, no. 4, Remark). The orbit of $\mathfrak{p}_x$ under Aut$_0(\mathfrak{g})$ is the set of $\mathfrak{p}_{x'}$ for $x'\in X$. This defines a map from $\mathfrak{P}(B(\mathfrak{g}))$ to $\mathscr{P}/$Aut$_0(\mathfrak{g})$. This map is surjective by the Remark of §3, no. 4, and injective by Prop. 7.

### 4. ZARISKI TOPOLOGY ON Aut($\mathfrak{g}$)

#### Proposition 8 {#lie-viii-s5-prop-8 .statement tag=0125}

Let V be the set of endomorphisms of the vector space $\mathfrak{g}$. Then Aut($\mathfrak{g}$) is closed in V for the Zariski topology (Chap. VII, App. I).

Let K be the Killing form of $\mathfrak{g}$. If $s\in$ Aut($\mathfrak{g}$),

$$
[sx, sy] = [x, y] \tag{2}
$$

$$
K(sx, sy) = K(x, y) \tag{3}
$$

for all $x, y\in \mathfrak{g}$. Conversely, let $s$ be an element of V satisfying (2) and (3) for all $x, y\in \mathfrak{g}$. Then Ker($s$) $= 0$, so $s$ is bijective and $s\in$ Aut($\mathfrak{g}$). But, for all $x, y\in \mathfrak{g}$, the maps $s \rightarrow [sx, sy]$ and $s \rightarrow K(sx, sy)$ from V to $\mathfrak{g}$ and $k$ are polynomial.

#### Proposition 9 {#lie-viii-s5-prop-9 .statement tag=0126}

Let $\mathfrak{h}$ be a splitting Cartan subalgebra of $\mathfrak{g}$.

(i) The group $f(T_Q)$ is closed in Aut($\mathfrak{g}$) in the Zariski topology.

(ii) The group $f(q(T_P))$ is dense in $f(T_Q)$ in the Zariski topology.

Assertion (i) follows from the equality $f(T_Q) =$ Aut($\mathfrak{g},\mathfrak{h}$)$\cap$Ker$\varepsilon$ (Prop. 2). Put $m= (P(R) : Q(R))$. Let F be a polynomial function on V; we assume that F vanishes on the $m$th power of every element of $f(T_Q)$, and show that $F|f(T_Q) = 0$; in view of Lemma 3, this will prove (ii).

The set $V'$ of elements of V inducing the identity on $\mathfrak{h}$ and leaving each $\mathfrak{g}^{\alpha}$ stable can be identified with $k^R$. Let $F'$ be the restriction of F to $V'=k^R$; this is a polynomial function. We have $f(T_Q)\subset V'$. Let $B = (\alpha_1, . . . , \alpha_l)$ be a basis of R. For all $t= (t_1, . . . , t_l)\in k^{*B}$, let $\varphi (t)$ be the homomorphism from Q(R) to the group $k^*$ that extends $t$. Then $F'(f(\varphi (t)))$ can be written as a finite sum

$$
\sum_{n_1,...,n_l\in\mathbf{Z}}c_{n_1,...,n_l}t^n_{1^1}. . . t^n_{l^l}= H(t_1, . . . , t_l)
$$

By assumption,

$$
0 = H(t^m_1, . . . , t^m_l) =\sum_{n_1,...,n_l\in\mathbf{Z}}c_{n_1,...,n_l}t^{mn}_{1^1}. . . t^{mn}_{l^l}
$$

for all $t_1, . . . , t_l\in k^*$. The $c_{n_1,...,n_l}$ are thus the coefficients of a polynomial in $l$ variables which vanishes on $k^{*l}$; hence they are all zero.

#### Proposition 10 {#lie-viii-s5-prop-10 .statement tag=0127}

Assume that $\mathfrak{g}$ is splittable.

(i) The group Aut$_e(\mathfrak{g})$ is dense in Aut$_0(\mathfrak{g})$ in the Zariski topology.

(ii) The groups Aut$_e(\mathfrak{g})$ and Aut$_0(\mathfrak{g})$ are connected in the Zariski topology.

By Prop. $3,f(q(T_P))\subset$ Aut$_e(\mathfrak{g})$. For all $s\in$ Aut$_e(\mathfrak{g})$, the closure of $s.f(q(T_P))$ in the Zariski topology contains $s.f(T_Q)$ by Prop. 9. Hence the closure of Aut$_e(\mathfrak{g})$ contains Aut$_e(\mathfrak{g}).f(T_Q) =$ Aut$_0(\mathfrak{g})$ (Prop. 6). This proves (i).

Let Aut$_e(\mathfrak{g}) =\Omega \cup \Omega '$ be a partition of Aut$_e(\mathfrak{g})$ formed by relatively open subsets in the Zariski topology, and with $\Omega \not=\emptyset$. If $\omega \in \Omega$ and if $x$ is a nilpotent element of $\mathfrak{g}$, the map $\tau :t \rightarrow \omega$ exp($t$ ad $x)$ from $k$ to Aut$_e(\mathfrak{g})$ is polynomial, hence continuous in the Zariski topology; consequently, $\tau (k)$ is connected; since $\omega \in \tau (k)$, we have $\tau (k)\subset \Omega$. Thus, $\Omega$.(exp ad $kx)\subset \Omega$, so $\Omega$.Aut$_e(\mathfrak{g})\subset \Omega$ and $\Omega =$ Aut$_e(\mathfrak{g})$. This proves that Aut$_e(\mathfrak{g})$ is connected. It follows, by (i), that Aut$_0(\mathfrak{g})$ is connected. Q.E.D.

We shall see (§8, no. 4, Cor. of Prop. 6) that Aut$_0(\mathfrak{g})$ is closed in V in the Zariski topology, and that it is the connected component of the identity element of Aut($\mathfrak{g}$). On the other hand, Aut$_e(\mathfrak{g})$ is not in general closed in the Zariski topology.

$^*$Assume that $(\mathfrak{g},\mathfrak{h})$ is split. The group Aut$_0(\mathfrak{g})$ is the group $G(k)$ of $k$-points of a connected semi-simple algebraic group G with trivial centre (adjoint group). The group $f(T_Q)$ is equal to $H(k)$, where H is the Cartan subgroup of G with Lie algebra $\mathfrak{h}$. The inverse image $\widetilde{H}$ of H in the universal covering $\widetilde{G}$ of G (in the algebraic sense) has $T_P$ as its group of $k$-points. The image of $\widetilde{G}(k)$ in $G(k) =$ Aut$_0(\mathfrak{g})$ is the group Aut$_e(\mathfrak{g})._*$

### 5. LIE GROUP CASE

#### Proposition 11 {#lie-viii-s5-prop-11 .statement tag=0128}

Assume that $k$ is $\mathbf{R},\mathbf{C}$ or a non-discrete complete ultrametric field. Let $\mathfrak{h}$ be a splitting Cartan subalgebra of $\mathfrak{g}$.

(i) Aut($\mathfrak{g},\mathfrak{h}$) is a Lie subgroup of Aut($\mathfrak{g}$) with Lie algebra ad$\mathfrak{h}$.

(ii) $f(T_Q)$ and $(q\circ f)(T_P)$ are open subgroups of Aut($\mathfrak{g},\mathfrak{h}$).

(iii) Aut$_e(\mathfrak{g})$ is an open subgroup of Aut($\mathfrak{g}$).

(iv) If $k=\mathbf{R}$ or $\mathbf{C}$, Aut$_e(\mathfrak{g})$ is the identity component of Aut($\mathfrak{g}$), in other words Int($\mathfrak{g}$).

By Chap. III, §3, no. 8, Cor. 2 of Prop. 29, and no. 10, Prop. 36, Aut($\mathfrak{g},\mathfrak{h}$) is a Lie subgroup of Aut($\mathfrak{g}$) whose Lie algebra is the set of ad $x(x\in \mathfrak{g})$ such that (ad $x)\mathfrak{h}\subset \mathfrak{h}$, in other words ad$\mathfrak{h}$.

Let $H\in \mathfrak{h}$. There exists $\varepsilon  >0$ with the following properties: for $t\in k$ and $|t|< \varepsilon$, exp($t\gamma (H)$) is defined for all $\gamma \in P(R)$, and the map $\gamma  \rightarrow$ exp($t\gamma (H)$) is a homomorphism $\sigma_t$ from P(R) to $k^*$. For $|t|< \varepsilon$, exp($t$ ad H) is defined, induces the identity on $\mathfrak{h}$ and induces on $\mathfrak{g}^{\alpha}$ the homothety with ratio $\sigma_t(\alpha )$; hence exp $t$ ad $H\in (q\circ f)(T_P)$. This proves, in view of (i), that $(q\circ f)(T_P)$ contains a neighbourhood of 1 in Aut($\mathfrak{g},\mathfrak{h}$), and consequently is an open subgroup of Aut($\mathfrak{g},\mathfrak{h}$). A fortiori$,f(T_Q)$ is an open subgroup of Aut($\mathfrak{g},\mathfrak{h}$).

For all $\alpha \in R$, exp ad $\mathfrak{g}^{\alpha}\subset$ Aut$_e(\mathfrak{g})$. In view of (ii), Aut$_e(\mathfrak{g})$ contains a neighbourhood of 1 in Aut($\mathfrak{g}$), which proves (iii).

Assume that $k=\mathbf{R}$ or $\mathbf{C}$. Then Aut$_e(\mathfrak{g})$ is contained in the identity component C of Aut($\mathfrak{g}$) (Chap. VII, §3, no. 1), and is open in Aut($\mathfrak{g}$) by (iii). Thus Aut$_e(\mathfrak{g}) = C$. Finally, C = Int($\mathfrak{g}$) by Chap. III, §9, no. 8, Prop. 30 (i).

### Exercises {#lie-viii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
