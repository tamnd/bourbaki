---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 7
section_title: Finite dimensional modules over a split semi-simple Lie algebra
lang: en
source: lie-vii-ix
book_pages: 124-140, 238-250
pdf_pages: 0132-0148, 0246-0258
extraction: native+ocr
subsections:
    - "no": 1
      title: WEIGHTS OF A FINITE DIMENSIONAL SIMPLE $\mathfrak{g}$-MODULE
      page: 124
      pdf_page: 132
    - "no": 2
      title: HIGHEST WEIGHT OF A FINITE DIMENSIONAL SIMPLE $\mathfrak{g}$-MODULE
      page: 126
      pdf_page: 134
    - "no": 3
      title: MINUSCULE WEIGHTS
      page: 130
      pdf_page: 138
    - "no": 4
      title: TENSOR PRODUCTS OF $\mathfrak{g}$-MODULES
      page: 132
      pdf_page: 140
    - "no": 5
      title: DUAL OF A $\mathfrak{g}$-MODULE
      page: 134
      pdf_page: 142
    - "no": 6
      title: REPRESENTATION RING
      page: 136
      pdf_page: 144
    - "no": 7
      title: CHARACTERS OF $\mathfrak{g}$-MODULES
      page: 139
      pdf_page: 147
statements: 46
exercises: 27
content_sha256: 373094899a42a9ee7668fe8b6fc892ffbcc2dc272b6bd645e1900eefba1aaec5
---

## § 7. FINITE DIMENSIONAL MODULES OVER A SPLIT SEMI-SIMPLE LIE ALGEBRA

In this paragraph, we retain the general notations of §6. We denote by P (resp. Q) the group of weights of R (resp. radical weights of R). We denote by $P_+$ (resp. $Q_+)$ the set of elements of P (resp. Q) that are positive for the order relation defined by B. We denote by $P_{++}$ the set of dominant weights of R relative to B (Chap. VI, §1, no. 10). An element $\lambda$ of $\mathfrak{h}^*$ belongs to P (resp. to $P_{++})$ if and only if all the $\lambda (H_{\alpha}),\alpha \in B$, are integers (resp. integers $\geq 0)$. We have $P_{++}\subset P_+$ (Chap. VI, §1, no. 6). If $w\in W$, we denote by $\varepsilon (w)$ the determinant of $w$, which is equal to 1 or $-1$. We put $\rho =\frac{1}{2}\sum_{\alpha\in R_+}\alpha$.

### 1. WEIGHTS OF A FINITE DIMENSIONAL SIMPLE $\mathfrak{g}$-MODULE

#### Proposition 1 {#lie-viii-s7-prop-1 .statement tag=0138}

Let V be a finite dimensional $\mathfrak{g}$-module.

(i) All the weights of V belong to P.

(ii) $V =\bigoplus_{\mu\in P}V^\mu$.

(iii) For all $\mu\in \mathfrak{h}^*,V^\mu$ is the set of $x\in V$ such that $h.x=\mu(h)x$ for all $h\in \mathfrak{h}$.

For all $\alpha \in B$, there exists a homomorphism from $\mathfrak{s}\mathfrak{l}(2, k)$ to $\mathfrak{g}$ that takes $H$ to $H_{\alpha}$. Thus, by §1, no. 2, Cor. of Prop. $2, (H_{\alpha})_V$ is diagonalizable and its eigenvalues are integers. Hence, the set of $(H_{\alpha})_V$, for $\alpha \in B$, is diagonalizable (Algebra, Chap. VII, §5, no. 6, Prop. 13). Consequently, for all $h\in \mathfrak{h},h_V$ is diagonalizable. By Chap. VII, §1, no. 3, Prop. $9, V =\bigoplus_{\mu\in\mathfrak{h}^*}V^\mu$. On the other hand, if $V^\mu\not= 0$, the preceding shows that $\mu(H_{\alpha})\in \mathbf{Z}$ for all $\alpha \in B$, so $\mu\in P$. This proves (i) and (ii). We see in the same way that $\mathfrak{h}_V$ is diagonalizable, hence (iii).

#### Corollary {#lie-viii-s7-n1-cor-1 .statement tag=0139}

Let $\rho$ be a finite dimensional representation of $\mathfrak{g}$ and $\Phi$ the bilinear form associated to $\rho$.

(i) If $x, y\in \mathfrak{h}_{\mathbf{Q}}$, then $\Phi (x, y)\in \mathbf{Q}$ and $\Phi (x, x)\in \mathbf{Q}_+$.

(ii) If $\rho$ is injective, the restriction of $\Phi$ to $\mathfrak{h}$ is non-degenerate.

Assertion (i) follows from Prop. 1 since the elements of P have rational values on $\mathfrak{h}_{\mathbf{Q}}$. If $\rho$ is injective, $\Phi$ is non-degenerate (Chap. I, §6, no. 1, Prop. 1), so the restriction of $\Phi$ to $\mathfrak{h}$ is non-degenerate (Chap. VII, §1, no. 3, Prop. 10 (iii)).

#### Lemma 1 {#lie-viii-s7-lem-1 .statement tag=013A}

Let V be a $\mathfrak{g}$-module and $\rho$ the corresponding representation of $\mathfrak{g}$.

(i) If $a$ is a nilpotent element of $\mathfrak{g}$, and if $\rho (a)$ is locally nilpotent,

$$
\rho (e^{ada}b) =e^{\rho(a)}\rho (b)e^{-\rho(a)}
$$

for all $b\in \mathfrak{g}$.

(ii) If $\alpha \in R$ and if the images under $\rho$ of the elements of $\mathfrak{g}^{\alpha}$ and $\mathfrak{g}^{-\alpha}$ are locally nilpotent, the set of weights of V is stable under the reflection $s_{\alpha}$.

With the assumptions in (i), we have $\rho$((ad $a)^nb) =$ (ad $\rho (a))^n\rho (b)$ for all $n\geq 0$, so $\rho (e^{ada}b) =e^{ad\rho(a)}\rho (b)$. On the other hand,

$$
e^{ad\rho(a)}\rho (b) =e^{\rho(a)}\rho (b)e^{-\rho(a)}
$$

is assertion (ii) of Chap. VII, §3, no. 1, Lemma 1.

We now adopt the assumptions in (ii). Let $\theta_{\alpha}=e^{adX_{\alpha}}e^{adX_{-\alpha}}e^{adX_{\alpha}}$. By (i), there exists $S\in \mathbf{G}\mathbf{L}(V)$ such that $\rho (\theta_{\alpha}b) = S\rho (b)S^{-1}$ for all $b\in \mathfrak{g}$. Now $\theta_{\alpha}|\mathfrak{h}$ is the transpose of $s_{\alpha}($§2, no. 2, Lemma 1). Let $\lambda$ be a weight of V. There exists a non-zero element $x$ of V such that $\rho (h)x=\lambda (h)x$ for all $h\in \mathfrak{h}$. Then

$$
\rho (h)S^{-1}x= S^{-1}\rho (^ts_{\alpha}h)x= S^{-1}\lambda (^ts_{\alpha}h)x= (s_{\alpha}\lambda )(h)S^{-1}x
$$

for all $h\in \mathfrak{h}$. Consequently, $s_{\alpha}\lambda$ is a weight of V.

#### Proposition 2 {#lie-viii-s7-prop-2 .statement tag=013B}

Let V be a finite dimensional $\mathfrak{g}$-module and $s\in$ Aut$_0(\mathfrak{g})$.

(i) There exists $S\in \mathbf{G}\mathbf{L}(V)$ such that $(s(x))_V= Sx_VS^{-1}$ for all $x\in \mathfrak{g}$.

(ii) If $s\in$ Aut$_e(\mathfrak{g})$, S can be chosen to be an element of $\mathbf{S}\mathbf{L}(V)$ leaving stable all the $\mathfrak{g}$-submodules of V.

Assertion (ii) follows from Lemma 1 (i). Now let $s\in$ Aut$_0(\mathfrak{g})$ and denote by $\rho$ the representation of $\mathfrak{g}$ defined by V. By (ii), the representations $\rho$ and $\rho \circ s$ become equivalent after extension of scalars. They are therefore equivalent (Chap. I, §3, no. 8, Prop. 13), hence the existence of S.

#### Remark 1 {#lie-viii-s7-n1-rem-1 .statement tag=013C}

Let S satisfy the condition in Prop. 2 (i), and let $\mathfrak{h}'=s(\mathfrak{h})$; denote by $s^*$ the isomorphism $\lambda  \rightarrow \lambda \circ s^{-1}$ from $\mathfrak{h}^*$ to $\mathfrak{h}^{'*}$. It is clear that

$$
S(V^{\lambda}) = V^{s^*\lambda}
$$

In particular:

#### Corollary 1 {#lie-viii-s7-prop-2-cor-1 .statement tag=013D}

The isomorphism $s^*$ takes the weights of V with respect to $\mathfrak{h}$ to those of V with respect to $\mathfrak{h}'$; corresponding weights have the same multiplicity.

#### Corollary 2 {#lie-viii-s7-prop-2-cor-2 .statement tag=013E}

Let $w\in W$. For all $\lambda \in \mathfrak{h}^*$, the vector subspaces $V^{\lambda}$ and $V^{w\lambda}$ have the same dimension. The set of weights of V is stable under W.

Indeed, $w$ is of the form $s^*$ with $s\in$ Aut$_e(\mathfrak{g},\mathfrak{h}) ($§2, no. 2, Cor. of Th. 2).

#### Remark 2 {#lie-viii-s7-n1-rem-2 .statement tag=01L8}

By Cor. 1 of Prop. 2 and §5, no. 3, Remark 2, it makes sense to speak of the weights of V with respect to the canonical Cartan subalgebra of $\mathfrak{g}$, and of their multipicities.

#### Remark 3 {#lie-viii-s7-n1-rem-3 .statement tag=013F}

Lemma 1 (i) and Prop. 2 remain valid, with the same proof, even if $\mathfrak{g}$ is not assumed to be splittable.

### 2. HIGHEST WEIGHT OF A FINITE DIMENSIONAL SIMPLE $\mathfrak{g}$-MODULE

#### Theorem 1 {#lie-viii-s7-thm-1 .statement tag=013G}

A simple $\mathfrak{g}$-module is finite dimensional if and only if it has a highest weight belonging to $P_{++}$.

We denote by V a simple $\mathfrak{g}$-module and by $\mathscr{X}$ its set of weights.

a) Assume that V is finite dimensional. Then $\mathscr{X}$ is finite and non-empty (Prop. 1) and so has a maximal element $\omega$. Let $\alpha \in B$. Then $\omega +\alpha  /\in \mathscr{X}$, which proves that $\omega$ is the highest weight of V (§6, no. 2, Lemma 2). On the other hand, there exists a homomorphism from $\mathfrak{s}\mathfrak{l}(2, k)$ to $\mathfrak{g}$ that takes $H$ to $H_{\alpha}$; by §1, Prop. 2 (i), $\omega (H_{\alpha})$ is an integer $\geq 0$, so $\omega \in P_{++}$.

b) Assume that V has a highest weight $\omega \in P_{++}$. Let $\alpha \in B$ and let $e$ be a primitive element of weight $\omega$ in V. Put $e_j=X_{-\alpha}^je$ for $j\geq 0$,

$m=\omega (H_{\alpha})\in \mathbf{N}$, and N = $\sum_{j=0}^mke_j$. By §1, no. 2, Prop. $1,X_{\alpha}e_{m+1}$ = 0.

If $\beta \in B$ and $\beta \not=\alpha$, then $[X_{\beta}, X_{-\alpha}] = 0$ so $X_{\beta}e_{m+1}=X_{\beta}X_{-\alpha}^{m+1}e$ = $X_{-\alpha}^{m+1}X_{\beta}e= 0$. If $e_{m+1}\not= 0$, we conclude that $e_{m+1}$ is primitive, which is absurd (§6, Prop. 3 (i)); so $e_{m+1}= 0$. Thus, by §1, no. 2, Cor. of Prop. 1, N is stable under the subalgebra $\mathfrak{s}_{\alpha}$ generated by $H_{\alpha}, X_{\alpha}$ and $X_{-\alpha}$. Now $\mathfrak{s}_{\alpha}$ is reductive in $\mathfrak{g}$, so the sum of the finite dimensional subspaces of V that are stable under $\mathfrak{s}_{\alpha}$ is a $\mathfrak{g}$-submodule of V (Chap. I, §6, no. 6, Prop. 7); since this sum is non-zero, it is equal to V. It follows from this that $(X_{\alpha})_V$ and $(X_{-\alpha})_V$ are locally nilpotent. In view of Lemma 1 (ii), $\mathscr{X}$ is stable under $s_{\alpha}$, and this holds for all $\alpha$. Hence $\mathscr{X}$ is stable under W. Now every orbit of W on P meets $P_{++}$ (Chap. VI, §1, no. 10). On the other hand, if $\lambda \in \mathscr{X}\cap P_{++}$, then $\lambda =\omega -\sum_{\alpha\in B}n_{\alpha}\alpha =\sum_{\alpha\in B}n'_{\alpha}\alpha$ with $n_{\alpha}\in \mathbf{N}$ and $n'_{\alpha}\geq 0$ for all $\alpha \in B$

(Chap. V, §3, no. 5, Lemma 6). So $\mathscr{X}\cap P_{++}$ is finite and hence so is $\mathscr{X}$. Since each weight has finite multiplicity (§6, no. 1, Prop. 1 (ii)), V is finite dimensional.

#### Corollary 1 {#lie-viii-s7-thm-1-cor-1 .statement tag=013H}

If $\lambda \in \mathfrak{h}^*$ and $\lambda  /\in P_{++}$, the $\mathfrak{g}$-module $E(\lambda ) ($§6, no. 3) is infinite dimensional.

#### Corollary 2 {#lie-viii-s7-thm-1-cor-2 .statement tag=013I}

The $\mathfrak{g}$-modules $E(\lambda )$ for $\lambda \in P_{++}$ constitute a set of representatives of the classes of finite dimensional simple $\mathfrak{g}$-modules.

The $\mathfrak{g}$-modules $E(\lambda )$, where $\lambda$ is a fundamental weight, are called the fundamental $\mathfrak{g}$-modules; the corresponding representations are called the fundamental representations of $\mathfrak{g}$; they are absolutely irreducible (§6, no. 2, Prop. 3 (iv)).

If V is a finite dimensional $\mathfrak{g}$-module and $\lambda \in P_{++}$, the isotypical component of V of type $E(\lambda )$ is called the isotypical component of highest weight $\lambda$ of V.

#### Remark 1 {#lie-viii-s7-n2-rem-1 .statement tag=013J}

Let $\lambda \in P_{++},\rho_{\lambda}$ the representation of $\mathfrak{g}$ on $E(\lambda ),s\in$ Aut($\mathfrak{g}$), and $\sigma$ the canonical image of $s$ in Aut(R$,B) ($§5, no. 3, Cor. 1 of Prop. 5). Then $\rho_{\lambda}\circ s$ is equivalent to $\rho_{\sigma \lambda}$; indeed, if $s\in$ Aut$_0(\mathfrak{g}),\rho_{\lambda}\circ s$ and $\rho_{\sigma \lambda}$ are equivalent to $\rho_{\lambda}$ (Prop. 2); and, if $s$ leaves $\mathfrak{h}$ and B stable, $\rho_{\lambda}\circ s$ is simple of highest weight $\sigma \lambda$.

In particular, the fundamental representations are permuted by $s$, and this permutation is the identity if and only if $s\in$ Aut$_0(\mathfrak{g})$.

#### Proposition 3 {#lie-viii-s7-prop-3 .statement tag=013K}

Let V be a finite dimensional $\mathfrak{g}$-module and $\mathscr{X}$ its set of weights. Let $\lambda \in \mathscr{X},\alpha \in R$, I the set of $t\in \mathbf{Z}$ such that $\lambda +t\alpha \in \mathscr{X},p$ (resp. $-q)$ the largest (resp. smallest) element of I. Let $m_t$ be the multiplicity of $\lambda +t\alpha$.

(i) I = $-q, p$ and $q-p=\lambda (H_{\alpha})$.

(ii) For any integer $u\in 0, p+q,\lambda + (p-u)\alpha$ and $\lambda + (-q+u)\alpha$ are conjugate under $s_{\alpha}$, and $m_{-q+u}=m_{p-u}$.

(iii) If $t\in \mathbf{Z}$ and $t <(p-q)/2$, $(X_{\alpha})_V$ maps $V^{\lambda+t\alpha}$ injectively into $V^{\lambda+(t+1)\alpha}$.

(iv) The function $t \rightarrow m_t$ is increasing on $-q,(p-q)/2$ and decreasing on $(p-q)/2, p$.

Let $\alpha \in B$. Give V the $\mathfrak{s}\mathfrak{l}(2, k$)-module structure defined by the elements $X_{\alpha}, X_{-\alpha}, H_{\alpha}$ of $\mathfrak{g}$. Every non-zero element of $V^{\lambda+p\alpha}$ is then primitive. Consequently, $(\lambda +p\alpha )(H_{\alpha})\geq 0$ and $(X_{-\alpha})^rV^{\lambda+p\alpha}\not= 0$ for

$$
0\leq r\leq (\lambda +p\alpha )(H_{\alpha}) =\lambda (H_{\alpha}) + 2p
$$

(§1, no. 2, Prop. 2). It follows that $V^{\lambda+t\alpha}\not= 0$ for $p\geq t\geq p-(\lambda (H_{\alpha}) + 2p)$, so $p+q\geq \lambda (H_{\alpha}) + 2p$. Applying this result to $-\alpha$ gives

$$
p+q\geq \lambda (H_{-\alpha}) + 2q=-\lambda (H_{\alpha}) + 2q
$$

Hence $q-p=\lambda (H_{\alpha})$ and $\lambda +t\alpha \in \mathscr{X}$ for $p\geq t\geq  -q$, which proves (i).

We have $s_{\alpha}(\alpha ) =-\alpha$, and $s_{\alpha}(\mu)\in \mu+k\alpha$ for all $\mu\in \mathfrak{h}^*$. Since W leaves $\mathscr{X}$ stable (Cor. 2 of Prop. $2),s_{\alpha}$ leaves $\{\lambda -q\alpha , \lambda -q\alpha +\alpha , . . . , \lambda +p\alpha \}$ stable and takes $\lambda -q\alpha +u\alpha$ to $\lambda +p\alpha -u\alpha$ for all $u\in k$. Using Cor. 2 of Prop. 2 again, we see that $m_{-q+u}=m_{p-u}$ for every integer $u\in 0, p+q$. This proves (ii).

By §1, Cor. of Prop. $2, (X_{\alpha})_V|V^{\lambda+t\alpha}$ is injective for $t <(p-q)/2$. Now $(X_{\alpha})_V$ maps $V^{\lambda+t\alpha}$ to $V^{\lambda+(t+1)\alpha}$. Hence $m_{t+1}\geq m_t$ for $t <(p-q)/2$. Changing $\alpha$ to $-\alpha$, we see that $m_{t+1}\leq m_t$ for $t >(p-q)/2$. This proves (iii) and (iv).

#### Corollary 1 {#lie-viii-s7-prop-3-cor-1 .statement tag=013L}

If $\lambda \in \mathscr{X}$ and $\lambda (H_{\alpha})\geq 1$, then $\lambda -\alpha \in \mathscr{X}$. If $\lambda +\alpha \in \mathscr{X}$ and $\lambda (H_{\alpha}) = 0$, then $\lambda \in \mathscr{X}$ and $\lambda -\alpha \in \mathscr{X}$.

This follows immediately from Prop. 3 (i).

#### Corollary 2 {#lie-viii-s7-prop-3-cor-2 .statement tag=01J4}

Let $\mu\in P_{++}$ and $\nu \in Q_+$. If $\mu+\nu \in \mathscr{X}$, then $\mu\in \mathscr{X}$.

Write $\nu =\sum_{\alpha\in B}c_{\alpha}.\alpha$, where $c_{\alpha}\in \mathbf{N}$ for all $\alpha \in B$. The corollary is clear

when $\sum_{\alpha\in B}c_{\alpha}= 0$; assume that $\sum_{\alpha\in B}c_{\alpha}>0$ and argue by induction on $\sum_{\alpha\in B}c_{\alpha}$. Let $(\cdot  | \cdot )$ be a W-invariant non-degenerate positive symmetric bilinear form on $\mathfrak{h}^*_{\mathbf{R}}$. Then $(\nu |\sum_{\alpha\in B}c_{\alpha}.\alpha )>0$, so there exists $\beta \in B$ such that $c_{\beta}\geq 1$ and

$(\nu |\beta )>0$, hence $\nu (H_{\beta})\geq 1$. Since $\mu\in P_{++}$, it follows that $(\mu+\nu )(H_{\beta})\geq 1$. By Cor. $1,\mu+ (\nu -\beta )\in \mathscr{X}$, and it suffices to apply the induction hypothesis.

#### Corollary 3 {#lie-viii-s7-prop-3-cor-3 .statement tag=013M}

Let $v\in V$ be primitive of weight $\omega$. Let $\Sigma$ be the set of $\alpha \in B$ such that $\omega (H_{\alpha}) = 0$. The stabilizer in $\mathfrak{g}$ of the line $kv$ is the parabolic subalgebra $\mathfrak{p}_{\Sigma}$ associated to $\Sigma ($§3, no. 4, Remark).

Replacing V by the $\mathfrak{g}$-submodule generated by $v$, if necessary, we can assume that V is simple. Let $\mathfrak{s}$ be the stabilizer. We have $(\mathfrak{n}_+)_Vv$ = 0, $(\mathfrak{h})_Vv\subset kv$. Let $\alpha \in B$ be such that $\omega (H_{\alpha}) = 0$. We have $\omega +\alpha  /\in \mathscr{X}$, hence $\omega -\alpha  /\in \mathscr{X}$ (Prop. 3 (i)) and consequently $(\mathfrak{g}^{-\alpha})_Vv= 0$. The preceding proves that $\mathfrak{p}_{\Sigma}\subset \mathfrak{s}$. If $\mathfrak{p}_{\Sigma}\not=\mathfrak{s}$, then $\mathfrak{s}=\mathfrak{p}_{\Sigma'}$, where $\Sigma '$ is a subset of B strictly containing $\Sigma$. Let $\beta \in \Sigma '$ **--** $\Sigma$. Then $\mathfrak{g}^{-\beta}$ stabilizes $kv$, and hence annihilates $v$. But, since $\omega (H_{\beta})>0$, this contradicts Prop. 3 (iii). Q.E.D.

A subset $\mathscr{X}$ of P is called R-saturated if it satisfies the following condition: for all $\lambda \in \mathscr{X}$ and all $\alpha \in R$, we have $\lambda -t\alpha \in \mathscr{X}$ for all integers $t$ between 0 and $\lambda (H_{\alpha})$. Since $s_{\alpha}(\lambda ) =\lambda -\lambda (H_{\alpha})\alpha$, we see that an R-saturated subset of P is stable under W. Let $\mathscr{Y}\subset P$. An element $\lambda$ of $\mathscr{Y}$ is called R-extremal in $\mathscr{Y}$ if, for all $\alpha \in R$, either $\lambda +\alpha  /\in \mathscr{Y}$ or $\lambda -\alpha  /\in \mathscr{Y}$.

#### Proposition 4 {#lie-viii-s7-prop-4 .statement tag=013N}

Let V be a finite dimensional $\mathfrak{g}$-module and $d$ an integer $\geq 1$. The set of weights of V of multiplicity $\geq d$ is R-saturated.

This follows immediately from Prop. 3.

#### Proposition 5 {#lie-viii-s7-prop-5 .statement tag=013O}

Let V be a finite dimensional simple $\mathfrak{g}$-module, $\omega$ its highest weight, $\mathscr{X}$ its set of weights. Choose a W-invariant non-degenerate positive symmetric bilinear form $(\cdot |\cdot )$ on $\mathfrak{h}^*_{\mathbf{R}}$, and let $\lambda  \rightarrow  \|\lambda \|= (\lambda |\lambda )^{1/2}$be the corresponding norm.

(i) $\mathscr{X}$ is the smallest R-saturated subset of P containing $\omega$.

(ii) The R-extremal elements of $\mathscr{X}$ are the W-transforms of $\omega$.

(iii) If $\mu\in \mathscr{X}$, we have $\|\mu\| \leq  \|\omega \|$. If, in addition, $\mu\not=\omega$, we have $\|\mu+\rho \|<\|\omega +\rho \|$. If $\mu$ is not R-extremal in $\mathscr{X}$, then $\|\mu\|<\|\omega \|$.

(iv) We have $\mathscr{X}= W.(\mathscr{X}\cap P_{++})$. An element $\lambda$ of $P_{++}$ belongs to $\mathscr{X}\cap P_{++}$ if and only if $\omega -\lambda \in Q_+$.

(i) Let $\mathscr{X}'$ be the smallest R-saturated subset of P containing $\omega$. We have $\mathscr{X}'\subset \mathscr{X}$ (Prop. 4). Assume that $\mathscr{X}\not=\mathscr{X}'$. Let $\lambda$ be a maximal element of $\mathscr{X}$ **--** $\mathscr{X}'$. Since $\lambda \not=\omega$, there exists $\alpha \in B$ such that $\lambda +\alpha \in \mathscr{X}$. Introduce $p$ and $q$ as in Prop. 3. Since $\lambda$ is maximal in $\mathscr{X}$ **--** $\mathscr{X}',\lambda +p\alpha \in \mathscr{X}'$. By Prop. 3 (ii), $\lambda -q\alpha \in \mathscr{X}'$ since $\mathscr{X}'$ is stable under W. Hence $\lambda +u\alpha \in \mathscr{X}'$ for every integer $u$ in the interval $-q, p$. This contradicts $\lambda  /\in \mathscr{X}'$ and proves (i).

(ii) It is clear that $\omega$ is an R-extremal element of $\mathscr{X}$; its W-transforms are therefore also R-extremal in $\mathscr{X}$. Let $\lambda$ be an R-extremal element of $\mathscr{X}$; we shall prove that $\lambda \in W.\omega$. Since there exists $w\in W$ such that $w\lambda \in P_{++}$ (Chap. VI, §1, no. 10), we can assume that $\lambda \in P_{++}$. Let $\alpha \in B$; introduce $p$ and $q$ as in Prop. 3. Since $\lambda$ is R-extremal, either $p= 0$ or $q= 0$. Since

$$
q-p=\lambda (H_{\alpha})\geq 0
$$

we cannot have $p >0$. Hence $p= 0$ and $\lambda =\omega$.

(iii) Let $\mu\in \mathscr{X}\cap P_{++}$. Then $\omega +\mu\in P_{++}$ and $\omega -\mu\in Q_+($§6, no. 1, Prop. 1), so $0\leq (\omega -\mu|\omega +\mu) = (\omega |\omega )-(\mu|\mu)$; hence, $(\mu|\mu)\leq (\omega |\omega )$, and this extends to all $\mu\in \mathscr{X}$ by using the Weyl group. If $\mu\in \mathscr{X}$ **--** $\{\omega \}$,

$$
(\mu+\rho |\mu+\rho ) = (\mu|\mu) + 2(\mu|\rho ) + (\rho |\rho )\leq (\omega |\omega ) + 2(\mu|\rho ) + (\rho |\rho )
$$

$$
= (\omega +\rho |\omega +\rho )-2(\omega -\mu|\rho )
$$

Now $\omega -\mu=\sum_{\alpha\in B}n_{\alpha}\alpha$ with integers $n_{\alpha}\geq 0$ not all zero, so $(\omega -\mu|\rho )>0$ since $(\rho |\alpha )>0$ for all $\alpha \in B$ (Chap. VI, §1, no. 10, Prop. 29 (iii)). If $\mu$ is not R-extremal in $\mathscr{X}$, there exists $\alpha \in R$ such that $\mu+\alpha \in \mathscr{X}$ and $\mu-\alpha \in \mathscr{X}$; then

$\|\mu\|<$ sup($\|\mu+\alpha \|,\|\mu-\alpha \|$)$\leq$ sup$_{\lambda\in\mathscr{X}}\|\lambda \|$

and this last upper bound is $\|\omega \|$ by the preceding.

(iv) We have $\mathscr{X}= W.(\mathscr{X}\cap P_{++})$ by Chap. VI, §1, no. 10. If $\lambda \in \mathscr{X}$, then $\omega -\lambda \in Q_+($§6, no. 1, Prop. 1). If $\lambda \in P_{++}$ and $\omega -\lambda \in Q_+$, then $\lambda \in \mathscr{X}$ (Cor. 2 of Prop. 3).

#### Corollary {#lie-viii-s7-n2-cor-1 .statement tag=013P}

Let $\mathscr{X}$ be a finite R-saturated subset of P. There exists a finite dimensional $\mathfrak{g}$-module whose set of weights is $\mathscr{X}$.

Since $\mathscr{X}$ is stable under $W,\mathscr{X}$ is the smallest R-saturated set containing $\mathscr{X}\cap P_{++}$. By Prop. 5 (i), $\mathscr{X}$ is the set of weights of $\bigoplus_{\lambda\in\mathscr{X}\cap P_{++}}E(\lambda )$.

#### Remark 2 {#lie-viii-s7-n2-rem-2 .statement tag=013Q}

Recall (Chap. VI, §1, no. 6, Cor. 3 of Prop. 17) that there exists a unique element $w_0$ of W that transforms B into $-B$; we have $w_0^2= 1$. and $-w_0$ respects the order relation on P. With this in mind, let V be a finite dimensional simple $\mathfrak{g}$-module, $\omega$ its highest weight. Then $w_0(\omega )$ is the lowest weight of V, and its multiplicity is 1.

### 3. MINUSCULE WEIGHTS

#### Proposition 6 {#lie-viii-s7-prop-6 .statement tag=013R}

Let $\lambda \in P$, and $\mathscr{X}$ the smallest R-saturated subset of P containing $\lambda$. Choose a norm $\| \cdot  \|$ as in Prop. 5. The following conditions are equivalent:

(i) $\mathscr{X}= W.\lambda$;

(ii) all the elements of $\mathscr{X}$ have the same norm;

(iii) for all $\alpha \in R$, we have $\lambda (H_{\alpha})\in  \{0,1,-1\}$.

Every non-empty R-saturated subset of P contains an element $\lambda$ satisfying the above conditions.

Introduce the condition:

(ii$')$ for all $\alpha \in R$ and for every integer $t$ between 0 and $\lambda (H_{\alpha})$,

$$
\|\lambda -t\alpha \| \geq  \|\lambda \|
$$

(i) $=\Rightarrow$ (ii) $=\Rightarrow$ (ii$'):$ This is clear.

(ii$') =\Rightarrow$ (iii): Assume that condition (ii$')$ is satisfied. Let $\alpha \in R$. We have $\|\lambda \|=\|\lambda -\lambda (H_{\alpha})\alpha \|$, so $\|\lambda -t\alpha \|<\|\lambda \|$ for every integer $t$ strictly between 0 and $\lambda (H_{\alpha})$; hence, there can be no such integers, so $|\lambda (H_{\alpha})| \leq 1$.

(iii) $=\Rightarrow$ (i): Assume that condition (iii) is satisfied. Let $w\in W$ and $\alpha \in R$. Then $(w\lambda )(H_{\alpha}) =\lambda (H_{w^{-1}\alpha})\in  \{0,1,-1\}$; thus, if $t$ is an integer between 0 and $(w\lambda )(H_{\alpha}),w\lambda -t\alpha$ is equal to $w\lambda$ or $s_{\alpha}(w\lambda )$. This proves that $W.\lambda$ is R-saturated, so $\mathscr{X}= W.\lambda$.

Let $\mathscr{Y}$ be a non-empty R-saturated subset of P. There exists in $\mathscr{Y}$ an element $\lambda$ of minimum norm. It is clear that $\lambda$ satisfies condition (ii$')$, hence the last assertion of the proposition.

#### Proposition 7 {#lie-viii-s7-prop-7 .statement tag=013S}

Let V be a finite dimensional simple $\mathfrak{g}$-module, $\mathscr{X}$ the set of weights of V, and $\lambda$ the highest element of $\mathscr{X}$ (cf. Prop. 5 (i)). Conditions (i), (ii) and (iii) of Prop. 6 are equivalent to:

(iv) for all $\alpha \in R$ and all $x\in \mathfrak{g}^{\alpha}$, we have $(x_V)^2= 0$.

If these conditions are satisfied, all the weights of V have multiplicity 1.

If (i) is satisfied, then $\mathscr{X}= W.\lambda$ and the weights all have the same multiplicity as $\lambda$ (Cor. 2 of Prop. 2), in other words, multiplicity 1. Moreover, if $w\in W$ and $\alpha \in R,w\lambda +t\alpha$ cannot be a weight of V unless $|t| \leq 1$; thus, if $x\in \mathfrak{g}^{\alpha}$,

$$
(x_V)^2(V^{w(\lambda)})\subset V^{w(\lambda)+2\alpha}= 0
$$

so $(x_V)^2= 0$, which proves that (i) $=\Rightarrow$ (iv).

Conversely, assume that (iv) is satisfied. Let $\alpha \in R$, and give V the $\mathfrak{s}\mathfrak{l}(2, k)$-module structure defined by the elements $X_{\alpha}, X_{-\alpha}, H_{\alpha}$ of $\mathfrak{g}$. Condition (iv), applied to $x=X_{\alpha}$, implies that the weights of the $\mathfrak{s}\mathfrak{l}(2, k$)-module V belong to $\{0,1,-1\}$ (cf. §1, no. 2, Cor. of Prop. 2). In particular, $\lambda (H_{\alpha})\in  \{0,1,-1\}$, so (iv) $=\Rightarrow$ (iii).

#### Proposition 8 {#lie-viii-s7-prop-8 .statement tag=013T}

Assume that $\mathfrak{g}$ is simple. Denote by $\alpha_1, . . . , \alpha_l$ the elements of B. Let $_1, . . . ,_l$ be the corresponding fundamental weights. Let $H$ = $n_1H_{\alpha_1}+\cdots +n_lH_{\alpha_l}$ be the highest root of $R^{\vee}$, and J the set of $i\in  \{1, . . . , l\}$ such that $n_i= 1$. Let $\lambda \in P_{++}$ **--** $\{0\}$. Then conditions (i), (ii) and (iii) of Prop. 6 are equivalent to each of the following conditions:

(v) $\lambda (H) = 1$;

(vi) there exists $i\in J$ such that $\lambda =_i$.

The $_i$, for $i\in J$, form a system of representatives in P(R) of the non-zero elements of $P(R)/Q(R)$.

Let $\lambda =u_{11}+\cdots +u_{ll}$, where $u_1, . . . , u_l$ are integers $\geq 0$ and not all zero. Then $\lambda (H) =u_1n_1+\cdots +u_ln_l$ and $n_1\geq 1, . . . , n_l\geq 1$, which gives the equivalence of (v) and (vi) immediately. On the other hand, $\lambda (H) =$ sup$_{\alpha\in R_+}\lambda (H_{\alpha})$, and $\lambda (H)>0$ since $\lambda$ is a non-zero element of $P_{++}$. Hence

condition (v) is equivalent to the condition $\lambda (H_{\alpha})\in  \{0,1\}$ for all $\alpha \in R$, in other words to condition (iii) of Prop. 6.

The last assertion of the proposition follows from Chap. VI, §2, no. 3, Cor. of Prop. 6.

#### Definition 1 {#lie-viii-s7-def-1 .statement tag=013U}

Assume that $\mathfrak{g}$ is simple. A minuscule weight of $(\mathfrak{g},\mathfrak{h})$ is an element of $P_{++}$ **--** $\{0\}$ which satisfies the equivalent conditions (i), (ii), (iii), (iv), (v) and (vi) of Prop. 6, 7 and 8.

#### Remark {#lie-viii-s7-n3-rem-1 .statement tag=013V}

Assume that $\mathfrak{g}$ is simple. Let $\Sigma^{'\vee}$ be the Coxeter graph of the affine Weyl group $W_a(R^{\vee})$. Recall that the vertices of $\Sigma^{'\vee}$ are the vertices of the Coxeter graph $\Sigma^{\vee}$ of $W(R^{\vee})$, together with a supplementary vertex 0. The group $A(R^{\vee})$ operates on $\Sigma^{'\vee}$ leaving 0 fixed. The group Aut($\Sigma^{'\vee}$) is canonically isomorphic to the semi-direct product of $A(R^{\vee})/W(R^{\vee})$ with a group $\Gamma_C$ (cf. Chap. VI, §2, no. 3, and Chap. VI, §4, no. 3); clearly (Aut $\Sigma^{'\vee})(0) =\Gamma_C(0)$; and $\Gamma_C(0)$ consists of 0 and the vertices of $\Sigma^{\vee}$ corresponding to the $_i$ for $i\in J$ (cf. Chap. VI, §2, Prop. 5 and Remark 1 of no. 3). In summary, the minuscule weights are the fundamental weights corresponding to the vertices of $\Sigma^{\vee}$ which can be obtained from 0 by the operation of an element of Aut($\Sigma^{'\vee}$).

With the notations of Chap. VI, Plates I to IX, we deduce from the preceding that the minuscule weights are the following:

For type $A_l(l\geq 1):_1, . . . ,_l$.

For type $B_l(l\geq 2):_l$.

For type $C_l(l\geq 2):_1$.

For type $D_l(l\geq 3):_1,_{l-1},_l$.

For type $E_6:_1,_6$.

For type $E_7:_7$.

For types $E_8,F_4,G_2$ there are no minuscule weights.

### 4. TENSOR PRODUCTS OF $\mathfrak{g}$-MODULES

Let $E,F$ be $\mathfrak{g}$-modules. For all $\lambda , \mu\in \mathfrak{h}^*, E^{\lambda}\otimes F^\mu\subset (E\otimes F)^{\lambda+\mu}$ (Chap. VII, §1, no. 1, Prop. 2 (ii)). If E and F are finite dimensional, then $E =\sum_{\lambda\in P}E^{\lambda}$

and $F =\sum_{\mu\in P}F^\mu$; consequently,

$$
(E\otimes F)^{\nu}=\sum_{\lambda ,\mu\in P,\lambda+\mu=\nu}E^{\lambda}\otimes F^\mu
$$

In other words, equipped with its graduation of type $P, E\otimes F$ is the graded tensor product of the graded vector spaces E and F.

#### Proposition 9 {#lie-viii-s7-prop-9 .statement tag=013W}

Let $E,F$ be finite dimensional simple $\mathfrak{g}$-modules, with highest weights $\lambda , \mu$, respectively.

(i) The component of $E\otimes F$ of highest weight $\lambda +\mu$ is a simple submodule, generated by $(E\otimes F)^{\lambda+\mu}= E^{\lambda}\otimes F^\mu$.

(ii) The highest weight of any simple submodule of $E\otimes F$ is $\leq \lambda +\mu$ (cf. §9, Prop. 2).

If $\alpha , \beta \in P$ and if $E^{\alpha}\otimes F^{\beta}\not= 0$, then $\alpha \leq \lambda$ and $\beta \leq \mu$. Consequently, $(E\otimes F)^{\lambda+\mu}$ is equal to $E^{\lambda}\otimes F^\mu$, and hence is of dimension 1, and $\lambda +\mu$ is the highest weight of $E\otimes F$. Every non-zero element of $E^{\lambda}\otimes F^\mu$ is primitive. By Prop. 4 of §6, no. 2, the length of the isotypical component of $E\otimes F$ of highest weight $\lambda +\mu$ is 1.

#### Remark {#lie-viii-s7-n4-rem-1 .statement tag=013X}

Retain the notations of Prop. 9. Let C be the isotypical component of $E\otimes F$ of highest weight $\lambda +\mu$. Then C depends only on E and F and not on the choice of $\mathfrak{h}$ and the basis B. In other words, let $\mathfrak{h}'$ be a splitting Cartan subalgebra of $\mathfrak{g}, R'$ the root system of $(\mathfrak{g},\mathfrak{h}')$, and $B'$ a basis of $R'$; let $\lambda ', \mu'$ be the highest weights of $E,F$ relative to $\mathfrak{h}'$ and $B'$; let $C'$ be the isotypical component of $E\otimes F$ of highest weight $\lambda '+\mu'$; then $C'= C$. Indeed, to prove this we can assume, by extension of the base field, that $k$ is algebraically closed. Then there exists $s\in$ Aut$_e(\mathfrak{g})$ that takes $\mathfrak{h}$ to $\mathfrak{h}', R$ to $R', B$ to $B'$. Let $S\in \mathbf{S}\mathbf{L}(E\otimes F)$ have the properties in Prop. 2 of no. 1. Then $S((E\otimes F)^{\lambda+\mu}) = (E\otimes F)^{\lambda'+\mu'}$ and S(C) = C. Hence $(E\otimes F)^{\lambda'+\mu'}\subset C'\cap S(C) = C'\cap C$, so $C'= C$. Thus, to 2 classes of finite dimensional simple $\mathfrak{g}$-modules we can associate canonically a third; in other words, we have defined on the set $\mathfrak{S}_{\mathfrak{g}}$ of classes of finite dimensional simple $\mathfrak{g}$-modules a composition law. With this structure, $\mathfrak{S}_{\mathfrak{g}}$ is canonically isomorphic to the additive monoid $P_{++}$.

#### Corollary 1 {#lie-viii-s7-prop-9-cor-1 .statement tag=01J5}

Let ( $_{\alpha})_{\alpha\in B}$ be the family of fundamental weights relative to B. Let $\lambda =\sum_{\alpha\in B}m_{\alpha\alpha}\in P_{++}$. For all $\alpha \in B$, let $E_{\alpha}$ be a simple $\mathfrak{g}$-module of highest weight $_{\alpha}$. In the $\mathfrak{g}$-module $\bigotimes_{\alpha\in B}(\bigotimes^{m_{\alpha}}E_{\alpha})$, the isotypical component of highest weight $\lambda$ is of length 1.

This follows from Prop. 9 by induction on $\sum_{\alpha\in B}m_{\alpha}$.

#### Corollary 2 {#lie-viii-s7-prop-9-cor-2 .statement tag=013Y}

Assume that $k$ is $\mathbf{R}$ or $\mathbf{C}$ or a non-discrete complete ultrametric field. Let G be a Lie group with Lie algebra $\mathfrak{g}$. Assume that, for any fundamental representation $\rho$ of $\mathfrak{g}$, there exists an analytic linear representation $\rho '$ of G such that $\rho = L(\rho ')$. Then, for any finite dimensional linear representation $\pi$ of $\mathfrak{g}$, there exists an analytic linear representation $\pi '$ of G such that $\pi = L(\pi ')$.

We use the notations of Cor. 1. There exists a representation $\sigma$ of G on $X =\bigotimes_{\alpha\in B}(\bigotimes^{m_{\alpha}}E_{\alpha})$ such that $L(\sigma )$ corresponds to the $\mathfrak{g}$-module structure of X (Chap. III, §3, no. 11, Cor. 3 of Prop. 41). Let C be the isotypical component of X of highest weight $\lambda$. In view of Chap. III, §3, no. 11, Prop. 40, it suffices to prove that C is stable under $\sigma (G)$. Let $g\in G$ and $\varphi =$ Ad($g$). Then $\sigma (g)a_X\sigma (g)^{-1}= (\varphi (a))_X$ for all $a\in \mathfrak{g}$. On the other hand, $\varphi$ is an automorphism of $\mathfrak{g}$ that takes $\mathfrak{h}$ to $\mathfrak{h}', R$ to $R'= R(\mathfrak{g},\mathfrak{h}'), B$ to a basis $B'$ of $R'$, and $_{\alpha}$ to the highest weight $'_{\alpha}$ of $E_{\alpha}$ relative to $\mathfrak{h}'$ and $B'$ (since $\varphi$ transforms $E_{\alpha}$ into a $\mathfrak{g}$-module isomorphic to $E_{\alpha})$. Hence $\varphi$ takes $\lambda$ to $\sum m_{\alpha}'_{\alpha}$. By the Remark above, $\sigma (g)(C) = C$.

#### Proposition 10 {#lie-viii-s7-prop-10 .statement tag=013Z}

Let $\lambda , \mu\in P_{++}$. Let $E,F,G$ be simple $\mathfrak{g}$-modules with highest weights $\lambda , \mu, \lambda +\mu$. Let $\mathscr{X}$ (resp. $\mathscr{X}',\mathscr{X}'')$ be the set of weights of E (resp. $F,G)$. Then $\mathscr{X}''=\mathscr{X}+\mathscr{X}'$.

We have $E =\bigoplus_{\nu\in P}E^{\nu},F =\bigoplus_{\sigma\in P}F^{\sigma}$, so $E\otimes F$ is the direct sum of the

$$
(E\otimes F)^{\tau}=\sum_{\nu+\sigma=\tau}E^{\nu}\otimes F^{\sigma}
$$

By Prop. 9, G can be identified with a $\mathfrak{g}$-submodule of $E\otimes F$, so $\mathscr{X}''\subset \mathscr{X}+\mathscr{X}'$. We have $G^{\tau}= G\cap (E\otimes F)^{\tau}$, and it is enough to show that, for $\nu \in \mathscr{X}$ and $\sigma \in \mathscr{X}'$, we have $G\cap (E\otimes F)^{\nu+\sigma}\not= 0$. Let $(e_1, . . . , e_n)$ (resp. $(f_1, . . . , f_p))$ be a basis of E (resp. F) consisting of elements each of which belong to some $E^{\nu}$ (resp. $F^{\sigma})$, and such that $e_1\in E^{\lambda}$ (resp. $f_1\in F^\mu)$. The $e_i\otimes f_j$ form a basis of $E\otimes F$. Suppose that the result to be proved is false. Then there exists a pair $(i, j)$ such that the coordinate of index $(i, j)$ of every element of G is zero. Let U be the enveloping algebra of $\mathfrak{g}, U'$ the dual of $U,c$ the coproduct of U. For all $u\in U$, let $x_i(u)$ (resp. $y_j(u))$ be the coordinate of $u(e_1)$ (resp. $u(f_1))$ of index $i$ (resp. $j)$; let $z_{ij}(u)$ be the coordinate of index $(i, j)$ of $u(e_1\otimes f_1)$. Then $x_i, y_j, z_{ij}\in U'$. Now $e_1$ generates the $\mathfrak{g}$-module E, so $x_i\not= 0$, and similarly $y_j\not= 0$. By the definition of the $\mathfrak{g}$-module $E\otimes F$ (Chap. I, §3, no. 2), if $c(u) =\sum u_s\otimes u'_s$, we have

$$
z_{ij}(u) =\sum_sx_i(u_s).y_j(u'_s) =\langle c(u), x_i\otimes y_j\rangle
$$

In other words, $z_{ij}$ is the product of $x_i$ and $y_j$ in the algebra $U'$. But this algebra is an integral domain (Chap. II, §1, no. 5, Prop. 10), so $z_{ij}\not= 0$. Since $u(e_1\otimes f_1)\in G$ for all $u\in U$, this is a contradiction.

### 5. DUAL OF A $\mathfrak{g}$-MODULE

Let $E,F$ be $\mathfrak{g}$-modules. Recall (Chap. I, §3, no. 3) that Hom$_k(E,F)$ has a canonical $\mathfrak{g}$-module structure. Let $\varphi$ be an element of weight $\lambda$ in Hom$_k(E,F)$. If $\mu\in \mathfrak{h}^*$, then $\varphi (E^\mu)\subset F^{\lambda+\mu}$ (Chap. VII, §1, no. 1, Prop. 2 (ii)). Thus, if E and F are finite dimensional, the elements of weight $\lambda$ in Hom$_k(E,F)$ are the graded homomorphisms of degree $\lambda$ in the sense of Algebra, Chap. II, §11, no. 2, Def. 4.

#### Proposition 11 {#lie-viii-s7-prop-11 .statement tag=0140}

Let E be a finite dimensional $\mathfrak{g}$-module, and consider the $\mathfrak{g}$-module $E^*=$ Hom$_k(E, k)$.

(i) An element $\lambda \in P$ is a weight of $E^*$ if and only if $-\lambda$ is a weight of E, and the multiplicity of $\lambda$ in $E^*$ is equal to that of $-\lambda$ in E.

(ii) If E is simple and has highest weight $\omega ,E^*$ is simple and has highest weight $-w_0(\omega )$ (cf. no. 2, Remark 2).

Consider $k$ as a trivial $\mathfrak{g}$-module whose elements are of weight 0. By what was said above, the elements of $E^*$ of weight $\lambda$ are the homomorphisms from E to $k$ which vanish on $E^\mu$ if $\mu\not=-\lambda$. This proves (i). If E is simple, $E^*$ is simple (Chap. I, §3, no. 3), and the last assertion follows from Remark 2 of no. 2.

#### Remark 1 {#lie-viii-s7-n5-rem-1 .statement tag=0141}

Let $E,E^*$ be as in Prop. 11, and $\sigma \in$ Aut($\mathfrak{g},\mathfrak{h}$) be such that $\varepsilon (\sigma ) =-w_0$ in the notations of §5, no. 1 (§5, no. 2, Prop. 2). Let $\rho , \rho '$ be the representations of $\mathfrak{g}$ associated to $E,E^*$. Then $\rho \circ \sigma$ is a simple representation of $\mathfrak{g}$ with highest weight $-w_0(\omega )$, so $\rho \circ \sigma$ is equivalent to $\rho '$.

#### Remark 2 {#lie-viii-s7-n5-rem-2 .statement tag=0142}

Assume that $w_0=-1$. Then, for any finite dimensional $\mathfrak{g}$-module E, E is isomorphic to $E^*$. Recall that, if $\mathfrak{g}$ is simple, $w_0=-1$ in the following cases: $\mathfrak{g}$ of type $A_1,B_l(l\geq 2), C_l(l\geq 2), D_l(l$ even $\geq 4), E_7,E_8,F_4,G_2$ (Chap. VI, Plates).

#### Lemma 2 {#lie-viii-s7-lem-2 .statement tag=0143}

Let $h^0=\sum_{\alpha\in R_+}H_{\alpha}$. Then $h^0=\sum_{\alpha\in B}a_{\alpha}H_{\alpha}$, where the $a_{\alpha}$ are integers $\geq 1$. Let $(b_{\alpha})_{\alpha\in B},(c_{\alpha})_{\alpha\in B}$ be families of scalars such that $b_{\alpha}c_{\alpha}=a_{\alpha}$ for all $\alpha \in B$. Put $x=\sum_{\alpha\in B}b_{\alpha}X_{\alpha}, y=\sum_{\alpha\in B}c_{\alpha}X_{-\alpha}$. There exists a homomorphism $\varphi$

from $\mathfrak{s}\mathfrak{l}(2, k)$ to $\mathfrak{g}$ such that $\varphi (H) =h^0, \varphi (X_+) =x, \varphi (X_-) =y$.

The fact that the $a_{\alpha}$ are integers $\geq 1$ follows from the fact that $(H_{\alpha})_{\alpha\in B}$ is a basis of the root system $(H_{\alpha})_{\alpha\in B}$ (cf. Chap. VI, §1, no. 5, Remark 5). We have:

$$
\alpha (h^0) = 2 \tag{1}
$$

for all $\alpha \in B$ (Chap. VI, §1, no. 10, Cor. of Prop. 29), so

$$
[h^0, x] =\sum_{\alpha\in B}b_{\alpha}\alpha (h^0)X_{\alpha}= 2x \tag{2}
$$

$$
[h^0, y] =\sum_{\alpha\in B}c_{\alpha}(-\alpha (h^0))X_{-\alpha}=-2y \tag{3}
$$

On the other hand,

$$
[x, y] =\sum_{\alpha ,\beta\in B}b_{\alpha}c_{\beta}[X_{\alpha}, X_{-\beta}] =\sum_{\alpha\in B}b_{\alpha}c_{\alpha}[X_{\alpha}, X_{-\alpha}] =-\sum_{\alpha\in B}a_{\alpha}H_{\alpha}=-h^0 \tag{4}
$$

hence the existence of the homomorphism $\varphi$.

#### Proposition 12 {#lie-viii-s7-prop-12 .statement tag=0144}

Let E be a finite dimensional simple $\mathfrak{g}$-module, $\omega$ its highest weight, and $\mathscr{B}$ the vector space of $\mathfrak{g}$-invariant bilinear forms on E. Let $m$ be the integer $\sum_{\alpha\in R_+}\omega (H_{\alpha})$, so that $m/2$ is the sum of the coordinates of $\omega$ with respect to B (Chap. VI, §1, no. 10, Cor. of Prop. 29). Let $w_0$ be the element of W such that $w_0(B) =-B$.

(i) If $w_0(\omega )\not=-\omega$, then $\mathscr{B}= 0$.

(ii) Assume that $w_0(\omega ) =-\omega$. Then $\mathscr{B}$ is of dimension 1, and every non-zero element of $\mathscr{B}$ is non-degenerate. If $m$ is even (resp. odd ), every element of $\mathscr{B}$ is symmetric (resp. alternating).

$a)$ Let $\Phi \in \mathscr{B}$. The map $\varphi$ from E to $E^*$ defined, for $x, y\in E$, by $\varphi (x)(y) =$ $\Phi (x, y)$ is a homomorphism of $\mathfrak{g}$-modules. If $\Phi \not= 0$, then $\varphi \not= 0$, so $\varphi$ is an isomorphism by Schur’s lemma, and hence $\Phi$ is non-degenerate. Consequently, the $\mathfrak{g}$-module E is isomorphic to the $\mathfrak{g}$-module $E^*$, so that $w_0(\omega ) =-\omega$. We have thus proved (i).

$b)$ Assume from now on that $w_0(\omega)=-\omega$. Then E is isomorphic to $E^*$. The vector space $\mathscr B$ is isomorphic to $\operatorname{Hom}_{\mathfrak g}(E,E^*)$, and hence to $\operatorname{Hom}_{\mathfrak g}(E,E)$ which is of dimension 1 (§6, no. 1, Prop. 1 (iii)). Hence $\dim \mathscr B=1$. Every non-zero element $\Phi$ of $\mathscr B$ is non-degenerate by a). Put $\Phi_1(x,y)=\Phi(y,x)$ for $x,y\in E$. By the preceding, there exists $\lambda\in k$ such that $\Phi_1(x,y)=\lambda\Phi(x,y)$ for all $x,y\in E$. Then $\Phi(y,x)=\lambda\Phi(x,y)=\lambda^2\Phi(y,x)$, so $\lambda^2=1$ and $\lambda=\pm1$. Thus, $\Phi$ is either symmetric or alternating.

$c)$ By Chap. VII, §1, no. 3, Prop. 9 (v), $E^\lambda$ and $E^\mu$ are orthogonal with respect to $\Phi$ if $\lambda+\mu\ne0$. Since $\Phi$ is non-degenerate, it follows that $E^\omega,E^{-\omega}$ are not orthogonal with respect to $\Phi$.

$d)$ There exists a homomorphism $\varphi$ from $\mathfrak{sl}(2,k)$ onto a subalgebra of $\mathfrak g$ that takes $H$ to
$$
\sum_{\alpha\in R_+}H_\alpha
$$
(Lemma 2). Consider E as an $\mathfrak{sl}(2,k)$-module via this homomorphism. Then the elements of $E^\lambda$ are of weight $\lambda\left(\sum_{\alpha\in R_+}H_\alpha\right)$. If $\lambda\in P$ is such that $E^\lambda\ne0$ and $\lambda\ne\omega,\lambda\ne-\omega$, then $-\omega<\lambda<\omega$, so
$$
-m=-\omega\left(\sum_{\alpha\in R_+}H_\alpha\right)<\lambda\left(\sum_{\alpha\in R_+}H_\alpha\right)<\omega\left(\sum_{\alpha\in R_+}H_\alpha\right)=m.
$$
Let G be the isotypical component of type V$(m)$ of the $\mathfrak{sl}(2,k)$-module E. By the preceding, G is of length 1 and contains $E^\omega,E^{-\omega}$. By c), the restriction of $\Phi$ to G is non-zero. By §1, no. 3, Remark 3, $\pi$ is even or odd according as this restriction is symmetric or alternating. In view of b), this completes the proof.

#### Definition 2 {#lie-viii-s7-def-2 .statement tag=01J6}

A finite dimensional irreducible representation $\rho$ of $\mathfrak g$ is said to be orthogonal (resp. symplectic) if there exists on E a non-degenerate symmetric (resp. alternating) bilinear form invariant under $\rho$.

### 6. REPRESENTATION RING

Let $\mathfrak a$ be a finite dimensional Lie algebra. Let $\mathscr F_{\mathfrak a}$ (resp. $\mathscr G_{\mathfrak a}$) be the set of classes of finite dimensional (resp. finite dimensional simple) $\mathfrak a$-modules. Let $\mathscr R(\mathfrak a)$ be the free abelian group $\mathbf Z^{(\mathscr G_{\mathfrak a})}$. For any finite dimensional simple $\mathfrak a$-module E, denote its class by $[E]$. Let F be a finite dimensional $\mathfrak a$-module; let
$$
(F_n,F_{n-1},\ldots,F_0)
$$
be a Jordan-Hölder series for F; the element
$$
\sum_{i=1}^{n}[F_i/F_{i-1}]
$$
of $\mathscr R(\mathfrak a)$ depends only on F and not on the choice of Jordan-Hölder series; we denote it by $[F]$. If
$$
0\longrightarrow F'\longrightarrow F\longrightarrow F''\longrightarrow0
$$
is an exact sequence of finite dimensional $\mathfrak a$-modules, then $[F]=[F']+[F'']$.

Let F be a finite dimensional semi-simple $\mathfrak{a}$-module; for all $E\in \mathfrak{S}_{\mathfrak{a}}$, let $n_E$ be the length of the isotypical component of F of type E; then [F] = $\sum_{E\in\mathfrak{S}_{\mathfrak{a}}}n_E.E$. If $F,F'$ are finite dimensional semi-simple $\mathfrak{a}$-modules, and if [F] = $[F']$, then F and $F'$ are isomorphic.

#### Lemma 3 {#lie-viii-s7-lem-3 .statement tag=0145}

Let G be an abelian group written additively, and $\varphi :\mathscr{F}_{\mathfrak{a}}\rightarrow G$ a map; by abuse of notation, we denote by $\varphi (F)$ the image under $\varphi$ of the class of any finite dimensional $\mathfrak{a}$-module F. Assume that, for any exact sequence

$$
0\longrightarrow F'\longrightarrow F\longrightarrow F''\longrightarrow 0
$$

of finite dimensional $\mathfrak{a}$-modules, we have $\varphi (F) =\varphi (F') +\varphi (F'')$. Then, there exists a unique homomorphism $\theta :\mathscr{R}(\mathfrak{a})\rightarrow G$ such that $\theta ([F]) =\varphi (F)$ for every finite dimensional $\mathfrak{a}$-module F.

There exists a unique homomorphism $\theta$ from $\mathscr{R}(\mathfrak{a})$ to G such that $\theta ([E]) =\varphi (E)$ for every finite dimensional simple $\mathfrak{a}$-module E. Let F be a finite dimensional $\mathfrak{a}$-module, and $(F_n,F_{n-1}, . . . ,F_0)$ a Jordan-Hölder series of F; if $n >0$, we have, by induction on $n$,

$$
\theta ([F]) =\sum_{i=1}^n\theta ([F_i/F_{i-1}]) =\sum_{i=1}^n\varphi (F_i/F_{i-1}) =\varphi (F)
$$

If $n= 0$ then [F] = 0 so $\theta ([F]) = 0$; on the other hand, by considering the exact sequence $0\longrightarrow 0\longrightarrow 0\longrightarrow 0\longrightarrow 0$ we see that $\varphi (0) = 0$.

#### Example {#lie-viii-s7-n6-exa-1 .statement tag=0146}

Take $G =\mathbf{Z}$ and $\varphi (F) =$ dim F. The corresponding homomorphism from $\mathscr{R}(\mathfrak{a})$ to $\mathbf{Z}$ is denoted by dim. Let $c$ be the class of a trivial $\mathfrak{a}$-module of dimension 1, and let $\psi$ be the homomorphism $n \rightarrow nc$ from $\mathbf{Z}$ to $\mathscr{R}(\mathfrak{a})$. It is immediate that

dim$\circ \psi =$ Id$_{\mathbf{Z}}$,

so that $\mathscr{R}(\mathfrak{a})$ is the direct sum of Ker dim and $\mathbf{Z}c$.

#### Lemma 4 {#lie-viii-s7-lem-4 .statement tag=0147}

There exists on the additive group $\mathscr{R}(\mathfrak{a})$ a unique multiplication distributive over addition such that $[E][F] = [E\otimes F]$ for all finite dimensional $\mathfrak{a}$-modules E, F. In this way $\mathscr{R}(\mathfrak{a})$ is given the structure of a commutative ring. The class of the trivial $\mathfrak{a}$-module of dimension 1 is the unit element of this ring.

The uniqueness is clear. There exists a commutative multiplication on $\mathscr{R}(\mathfrak{a}) =\mathbf{Z}^{(\mathfrak{S}_{\mathfrak{a}})}$ that is distributive over addition and such that $[E][F] = [E\otimes F]$ for all $E,F\in \mathfrak{S}_{\mathfrak{a}}$. Let $E_1,E_2$ be finite dimensional $\mathfrak{a}$-modules, $l_1$ and $l_2$ their lengths; we show that $[E_1][E_2] = [E_1\otimes E_2]$ by induction on $l_1+l_2$. This is clear if $l_1+l_2\leq 2$. On the other hand, let $F_1$ be a submodule of $E_1$ distinct from 0 and $E_1$. Then

$[F_1][E_2] = [F_1\otimes E_2]$ and $[E_1/F_1][E_2] = [(E_1/F_1)\otimes E_2]$ by the induction hypothesis. On the other hand, $(E_1\otimes E_2)/(F_1\otimes E_2)$ is isomorphic to $(E_1/F_1)\otimes E_2$. Hence

$$
[E_1][E_2] = ([E_1/F_1] + [F_1]).[E_2] = [(E_1/F_1)\otimes E_2] + [F_1\otimes E_2] = [E_1\otimes E_2]
$$

which proves our assertion. It follows immediately that the multiplication defined above is associative, so $\mathscr{R}(\mathfrak{a})$ has the structure of a commutative ring. Finally, it is clear that the class of the trivial $\mathfrak{a}$-module of dimension 1 is the unit element of this ring.

#### Lemma 5 {#lie-viii-s7-lem-5 .statement tag=0148}

There exists a unique involutive automorphism $X \rightarrow X^*$ of the ring $\mathscr{R}(\mathfrak{a})$ such that $[E]^*= [E^*]$ for every finite dimensional $\mathfrak{a}$-module E.

The uniqueness is clear. By Lemma 3, there exists a homomorphism $X \rightarrow X^*$ from the additive group $\mathscr{R}(\mathfrak{a})$ to itself such that $[E]^*= [E^*]$ for every finite dimensional $\mathfrak{a}$-module E. We have $(X^*)^*= X$, so this homomorphism is involutive. It is an automorphism of the ring $\mathscr{R}(\mathfrak{a})$ since $(E\otimes F)^*$ is isomorphic to $E^*\otimes F^*$ for all finite dimensional $\mathfrak{a}$-modules E and F. Q.E.D.

Let $U(\mathfrak{a})$ be the enveloping algebra of $\mathfrak{a}, U(\mathfrak{a})^*$ the vector space dual of $U(\mathfrak{a})$. Recall (Chap. II, §1, no. 5) that the coalgebra structure of $U(\mathfrak{a})$ defines on $U(\mathfrak{a})^*$ a commutative, associative algebra structure with unit element. For any finite dimensional $\mathfrak{a}$-module E, the map $u \rightarrow$ Tr($u_E$) from $U(\mathfrak{a})$ to $k$ is an element $\tau_E$ of $U(\mathfrak{a})^*$. If $0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0$ is an exact sequence of finite dimensional $\mathfrak{a}$-modules, then $\tau_E=\tau_{E'}+\tau_{E''}$. Hence, by Lemma 3 there exists a unique homomorphism, which we denote by Tr, from the additive group $\mathscr{R}(\mathfrak{a})$ to the group $U(\mathfrak{a})^*$ such that Tr[E] $=\tau_E$ for every finite dimensional $\mathfrak{a}$-module E. If $k$ denotes the trivial $\mathfrak{a}$-module of dimension 1, it is easy to check that Tr[$k]$ is the unit element of $U(\mathfrak{a})^*$. Finally, let E and F be finite dimensional $\mathfrak{a}$-modules. Let $u\in U(\mathfrak{a})$ and let $c$ be the coproduct of $U(\mathfrak{a})$. By definition of the U-module $E\otimes F$ (Chap. I, §3, no. 2), if $c(u) =\sum_iu_i\otimes u'_i$,

$$
u_{E\otimes F}=\sum_i(u_i)_E\otimes (u'_i)_F
$$

Consequently

$\tau_{E\otimes F}(u) =\sum_i$ Tr($u_i$)$_E$Tr($u'_i$)$_F=\sum_i\tau_E(u_i)\tau_F(u'_i)$

$$
= (\tau_E\otimes \tau_F)(c(u))
$$

This means that $\tau_E\tau_F=\tau_{E\otimes F}$. Thus, Tr$:\mathscr{R}(\mathfrak{a})\rightarrow U(\mathfrak{a})^*$ is a homomorphism of rings.

Let $\mathfrak{a}_1$ and $\mathfrak{a}_2$ be Lie algebras, $f$ a homomorphism from $\mathfrak{a}_1$ to $\mathfrak{a}_2$. Every finite dimensional $\mathfrak{a}_2$-module E defines by means of $f$ an $\mathfrak{a}_1$-module, hence elements of $\mathscr{R}(\mathfrak{a}_2)$ and $\mathscr{R}(\mathfrak{a}_1)$ that we denote provisionally by $[E]_2$ and $[E]_1$. By Lemma 3, there exists a unique homomorphism, denoted by $\mathscr{R}(f)$, from the group $\mathscr{R}(\mathfrak{a}_2)$ to the group $\mathscr{R}(\mathfrak{a}_1)$ such that $\mathscr{R}(f)[E]_2=[E]_1$ for every finite dimensional $\mathfrak{a}_2$-module E. Moreover, $\mathscr{R}(f)$ is a homomorphism of rings. If U(f) is the homomorphism from U($\mathfrak{a}_1$) to U($\mathfrak{a}_2$) extending $f$, the following diagram is commutative

$$
\begin{array}{ccc}
\mathscr{R}(\mathfrak{a}_2) & \xrightarrow{\mathscr{R}(f)} & \mathscr{R}(\mathfrak{a}_1)\\
\Big\downarrow\scriptstyle{\operatorname{Tr}} & & \Big\downarrow\scriptstyle{\operatorname{Tr}}\\
U(\mathfrak{a}_2)^* & \xrightarrow{t_{U(f)}} & U(\mathfrak{a}_1)^*.
\end{array}
$$

In what follows we take for $\mathfrak{a}$ the splittable semi-simple Lie algebra $\mathfrak{g}$. The ring $\mathscr{R}(\mathfrak{g})$ is called the *representation ring* of $\mathfrak{g}$. For all $\lambda\in P_{++}$, we denote by $[\lambda]$ the class of the simple $\mathfrak{g}$-module E($\lambda$) of highest weight $\lambda$.

### 7. CHARACTERS OF $\mathfrak{g}$-MODULES

Let $\Delta$ be a commutative monoid written additively, and $\mathbf{Z}[\Delta]=\mathbf{Z}^{(\Delta)}$ the algebra of the monoid $\Delta$ over $\mathbf{Z}$ (Algebra, Chap. III, §2, no. 6). Denote by $(e^\lambda)_{\lambda\in\Delta}$ the canonical basis of $\mathbf{Z}[\Delta]$. For all $\lambda,\mu\in\Delta$, we have $e^{\lambda+\mu}=e^\lambda e^\mu$. If 0 is the neutral element of $\Delta$, then $e^0$ is the unit element of $\mathbf{Z}[\Delta]$; it is denoted by 1.

Let E be a $\Delta$-graded vector space over a field $\kappa$, and let $(E^\lambda)_{\lambda\in\Delta}$ be its graduation. If each $E^\lambda$ is finite dimensional, the *character* of E, denoted by ch(E), is the element $(\dim E^\lambda)_{\lambda\in\Delta}$ of $\mathbf{Z}^{\Delta}$. If E itself is finite dimensional,

$$
\operatorname{ch}(E)=\sum_{\lambda\in\Delta}(\dim E^\lambda)e^\lambda\in\mathbf{Z}[\Delta].
\tag{5}
$$

Let E′, E, E″ be $\Delta$-graded vector spaces such that the E′${}^\lambda$, E${}^\lambda$, E″${}^\lambda$ are finite dimensional over $\kappa$, and $0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow0$ an exact sequence of graded homomorphisms of degree 0. It is immediate that

$$
\operatorname{ch}(E)=\operatorname{ch}(E')+\operatorname{ch}(E'').
\tag{6}
$$

In particular, if F$_1$, F$_2$ are $\Delta$-graded vector spaces such that the F$_1^\lambda$ and the F$_2^\lambda$ are finite dimensional over $\kappa$, then

$$
\operatorname{ch}(F_1\oplus F_2)=\operatorname{ch}(F_1)+\operatorname{ch}(F_2).
\tag{7}
$$

If F$_1$ and F$_2$ are finite dimensional, we also have

$$
\operatorname{ch}(F_1\otimes F_2)=\operatorname{ch}(F_1)\mathbin{.}\operatorname{ch}(F_2).
\tag{8}
$$

#### Example {#lie-viii-s7-n7-exa-1 .statement tag=01JX}

Assume that $\Delta=\mathbf{N}$. Let T be an indeterminate. There exists a unique isomorphism from the algebra $\mathbf{Z}[\mathbf{N}]$ to the algebra $\mathbf{Z}[T]$ that takes $e^n$ to $T^n$ for all $n\in\mathbf{N}$. For any finite dimensional $\mathbf{N}$-graded vector space E, the image of ch(E) in $\mathbf{Z}[T]$ is the Poincaré polynomial of E (Chap. V, §5, no. 1).

Let E be a $\mathfrak{g}$-module such that $E =\sum_{\lambda\in\mathfrak{h}^*}E^{\lambda}$ and such that each $E^{\lambda}$ is

finite dimensional. We know that $(E^{\lambda})_{\lambda\in\mathfrak{h}^*}$ is a graduation of the vector space E. In what follows we shall reserve the notation ch(E) for the character of E considered as a $\mathfrak{h}^*$-graded vector space. Thus, the character ch(E) is an element of $\mathbf{Z}^{\mathfrak{h}^*}$. If E is finite dimensional, ch(E) $\in \mathbf{Z}[P]$. By formula (6) and Lemma 3 of no. 6, there exists a unique homomorphism from the group $\mathscr{R}(\mathfrak{g})$ to $\mathbf{Z}[P]$ that takes E to ch(E), for any finite dimensional $\mathfrak{g}$-module E; this homomorphism will be denoted by ch. Relation (8) shows that ch is a homomorphism from the ring $\mathscr{R}(\mathfrak{g})$ to the ring $\mathbf{Z}[P]$.

#### Remark {#lie-viii-s7-n7-rem-1 .statement tag=0149}

Every element of P defines a simple $\mathfrak{h}$-module of dimension 1, hence a homomorphism from the group $\mathbf{Z}[P]$ to the group $\mathscr{R}(\mathfrak{h})$, which is an injective homomorphism of rings. It is immediate that the composite

$$
\mathscr{R}(\mathfrak{g})\longrightarrow \mathbf{Z}[P]\longrightarrow \mathscr{R}(\mathfrak{h})
$$

is the homomorphism defined by the canonical injection of $\mathfrak{h}$ into $\mathfrak{g}$ (no. 6).

The Weyl group W operates by automorphisms on the group P, and hence operates on $\mathbf{Z}^P$. For all $\lambda \in P$ and all $w\in W$, we have $we^{\lambda}=e^{w\lambda}$. Let $\mathbf{Z}[P]^W$ be the subring of $\mathbf{Z}[P]$ consisting of the elements invariant under W.

#### Lemma 6 {#lie-viii-s7-lem-6 .statement tag=014A}

If $\lambda \in P_{++}$, then ch[$\lambda ]\in \mathbf{Z}[P]^W$. The unique maximal term of ch[$\lambda ]$ (Chap. VI, §3, no. 2, Def. 1) is $e^{\lambda}$.

The first assertion follows from no. 1, Cor. 2 of Prop. 2, and the second from §6, no. 1, Prop. 1 (ii).

#### Theorem 2 {#lie-viii-s7-thm-2 .statement tag=014B}

(i) Let ( $_{\alpha})_{\alpha\in B}$ be the family of fundamental weights relative to B. Let $(T_{\alpha})_{\alpha\in B}$ be a family of indeterminates. The map $f \rightarrow f(([_{\alpha}])_{\alpha\in B})$ from $\mathbf{Z}[(T_{\alpha})_{\alpha\in B}]$ to $\mathscr{R}(\mathfrak{g})$ is an isomorphism of rings.

(ii) The homomorphism ch from $\mathscr{R}(\mathfrak{g})$ to $\mathbf{Z}[P]$ induces an isomorphism from the ring $\mathscr{R}(\mathfrak{g})$ to the ring $\mathbf{Z}[P]^W$.

(iii) Let E be a finite dimensional $\mathfrak{g}$-module. If ch $E =\sum_{\lambda\in P_{++}}m_{\lambda}$ch[$\lambda ]$, the isotypical component of E of highest weight $\lambda$ has length $m_{\lambda}$.

The family $([\lambda ])_{\lambda\in P_{++}}$ is a basis of the $\mathbf{Z}$-module $\mathscr{R}(\mathfrak{g})$, and the family (ch[$\lambda ])_{\lambda\in P_{++}}$ is a basis of the $\mathbf{Z}$-module $\mathbf{Z}[P]^W$ (Lemma 6, and Chap. VI, §3, no. 4, Prop. 3). This proves (ii) and (iii). Assertion (i) follows from (ii), Lemma 6 and Chap. VI, §3, no. 4, Th. 1.

#### Corollary {#lie-viii-s7-n7-cor-1 .statement tag=014C}

Let $E,E'$ be finite dimensional $\mathfrak{g}$-modules. Then E is isomorphic to $E'$ if and only if ch E = ch $E'$.

This follows from Th. 2 (ii) and the fact that $E,E'$ are semi-simple.

### Exercises {#lie-viii-s7-exercises}

All the $\mathfrak{g}$-modules considered (except those in Exerc. 14 and 15) are assumed to be finite dimensional.

See the [exercises for § 7](exercises/s7/).
