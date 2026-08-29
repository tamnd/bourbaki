---
book: ts
book_title: Théories spectrales
chapter: IV
chapter_title: THÉORIE SPECTRALE HILBERTIENNE
section: 5
section_title: Opérateurs partiels normaux et théorème spectral
lang: en
source: ts-iii-v-fr
book_pages: TS IV.262-TS IV.311, TS IV.352-TS IV.372
pdf_pages: 0275-0324, 0365-0385
extraction: native
subsections:
    - "no": 1
      title: Bornification
      page: 262
      pdf_page: 275
    - "no": 2
      title: Opérateurs partiels normaux et théorème spectral
      page: 265
      pdf_page: 278
    - "no": 3
      title: Calcul fonctionnel universellement mesurable
      page: 270
      pdf_page: 283
    - "no": 4
      title: Projecteurs spectraux
      page: 277
      pdf_page: 290
    - "no": 5
      title: La formule de Helffer–Sjöstrand
      page: 280
      pdf_page: 293
    - "no": 6
      title: Topologies résolvantes et continuité du calcul fonctionnel
      page: 285
      pdf_page: 298
    - "no": 7
      title: Décomposition polaire
      page: 289
      pdf_page: 302
    - "no": 8
      title: Opérateurs auto-adjoints définis par une forme hermitienne partielle positive
      page: 291
      pdf_page: 304
    - "no": 9
      title: Principes variationnels pour le spectre des opérateurs positifs
      page: 296
      pdf_page: 309
    - "no": 10
      title: Perturbation compacte et spectre essentiel
      page: 303
      pdf_page: 316
    - "no": 11
      title: Perturbation
      page: 305
      pdf_page: 318
    - "no": 12
      title: Opérateurs à résolvante compacte
      page: 307
      pdf_page: 320
statements: 75
exercises: 43
content_sha256: 10dc37b619e64ee4a121601fe906832b609fb0f17e1d46252b2e1db1c97c4fb6
translated_from: content/fr/ts/IV/05_s5_operateurs_partiels_normaux_et_theoreme.md
source_lang: fr
translation_method: machine
source_content_sha256: f70f085776eb5d6d046d7d9ac871a7701df94e569116088cb03b244cfa02460d
translation_model: gpt-5.4, gpt-5-6-mini
translation_run: translate-en-mt-e6203a96
glossary_version: 34
glossary_terms_sha256: d789d61b366e0ff5947042a1efbf869a0cadf813742e44b7037e46c608da9763
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 5. NORMAL PARTIAL OPERATORS AND THE SPECTRAL THEOREM

### 1. Bornification

Let E be a complex Hilbert space. Let $s$ denote the unitary mapping $(x, y)\mapsto (-y, x)$ on $E\oplus E$. Let $u$ be a closed partial operator with dense domain on E. The partial operator $u^*u$ is self-adjoint and positive (Prop. 12 of IV, p. 241), hence $-1\notin$ Sp($u^*u$) (Prop. 17 of IV, p. 248). We set $W(u) = (1_E+u^*u)^{-1}=-R(u^*u,-1)$; this is a positive and injective endomorphism of E.

Let $p_1$ and $p_2$ denote the two canonical projections of $\Gamma_u$ into E. They are elements of $\mathscr{L}(\Gamma_u; E)$, and we have the equality of correspondences $p_2=u\circ p_1$. Let $(j,|p^*_1|)$ be the polar decomposition (Def. 4 of I, p. 140) of the endomorphism $p^*_1\in \mathscr{L}(E; \Gamma_u)$, so that $p^*_1=|p^*_1| \circ j$. The mapping $j$ is a partial isometry of E into $\Gamma_u$.

#### Definition 1 {#ts-iv-s5-def-1 .statement tag=0359}

The endomorphism $p_2\circ j$ of E is called the bornification of $u$; we denote this endomorphism by $b(u)$.

We have $\|b(u)\|\leqslant 1$.

#### Proposition 1 {#ts-iv-s5-prop-1 .statement tag=035A}

We have the formulas

$$
|p^*_1|= W(u)^{1/2} \tag{1}
$$

$$
b(u) =u\circ W(u)^{1/2}=u\circ  |p^*_1| \tag{2}
$$

$$
1_E-b(u)^*b(u) = W(u) \tag{3}
$$

$$
b(u)W(u) = W(u^*)b(u),b(u)W(u)^{1/2}= W(u^*)^{1/2}b(u) \tag{4}
$$

Let $x\in E$. Put $y= W(u)(x)\in$ dom($u^*u$). We have $y\in$ dom($u$) and $u(y)\in$ dom($u^*$). For every element $(y_1, u(y_1))$ of $\Gamma_u$, where $y_1\in$ dom($u$), we compute

$$
\langle (y, u(y))|(y_1, u(y_1))\rangle =\langle y|y_1\rangle +\langle u(y)|u(y_1)\rangle
$$

$$
=\langle y+u^*u(y)|y_1\rangle =\langle x|p_1(y_1, u(y_1))\rangle
$$

This means that $p^*_1(x) = (y, u(y))$, whence $p_1\circ p^*_1(x) =y= W(u)(x)$. Consequently, we have $p_1\circ p^*_1= W(u)$, hence $|p^*_1|= W(u)^{1/2}$, that is, formula (1). In particular, since Im($p_1$) $=$ Im($|p^*_1|$) by the Cor. to Prop. 11 of I, p. 140, it follows that dom($u$) $=$ Im($p_1$) $=$ Im(W($u$)$^{1/2}$). The partial operator $u\circ W(u)^{1/2}$ therefore has the space E as domain. The relation $p_1\circ j= (p^*_1)^*\circ j=|p^*_1|= W(u)^{1/2}$ (Prop. 11, a) of I, p. 140) then implies that

$$
b(u) =p_2\circ j=u\circ p_1\circ j=u\circ W(u)^{1/2}
$$

which is formula (2).

On has Ker($j$) $=$ Ker($|p^*_1|$) (prop. 10, b) of I, p. 139) and formula (1) therefore implies that the partial isometry $j: E\rightarrow \Gamma_u$ is injective, hence isometric, whence $j^*\circ j= 1_E$. Writing $j= (p_1\circ j, b(u))$, we find

$$
1_E=j^*\circ j= (p_1\circ j)^*(p_1\circ j) +b(u)^*b(u) = W(u) +b(u)^*b(u)
$$

whence formula (3).

Let $x\in$ dom($u$) and put $y= W(u)(x)$. We have $y\in$ dom($u$) and formula $y+u^*u(y) =x$ implies that $u^*u(y)\in$ dom($u$). We then have

$$
W(u^*)^{-1}(u(y)) = (1_E+uu^*)(u(y))
$$

$$
=u(y) +uu^*u(y) =u(y+u^*u(y)) =u(x)
$$

which means that the reduction of $u\circ W(u)$ to the domain of $u$ is equal to $W(u^*)\circ u$. Since the image of $|p^*_1|$ is equal to that of $p_1$ (cor. of prop. 11 of I, p. 140) and hence to the domain of $u$, it follows that

$$
u\circ W(u)\circ  |p^*_1|= W(u^*)\circ u\circ  |p^*_1|= W(u^*)\circ b(u)
$$

(formula (2)). Moreover, $|p^*_1|= W(u)^{1/2}$ commutes with $W(u)$, hence we obtain

$$
b(u)\circ W(u) =u\circ  |p^*_1| \circ W(u) =u\circ W(u)\circ  |p^*_1|= W(u^*)\circ b(u)
$$

This relation implies that $b(u)\circ f(W(u)) =f(W(u^*))\circ b(u)$ for every function $f\in \mathscr{C}(\mathbf{R}_+)$ (prop. 11 of I, p. 113), hence in particular that $b(u)\circ W(u)^{1/2}= W(u^*)^{1/2}\circ b(u)$. This proves formula (4) and concludes the proof.

#### Corollary {#ts-iv-s5-n1-cor-1 .statement tag=035B}

We have $b(u)^*=b(u^*)$.

Let $q_1$ and $q_2$ be the projections $\Gamma_{u^*}\rightarrow E$ and let $(k,|q_1^*|)$ be the polar decomposition of $q_1^*$, so that $b(u^*) =q_2\circ k$. For all $x$ and $y$ in E, we have $j(x)\in \Gamma_u$ and $k(y)\in \Gamma_{u^*}$, and since $\Gamma_u$ is orthogonal to $s(\Gamma_{u^*})$ by prop. 7 of IV, p. 236, it follows that

$$
0 =\langle j(x)|s(k(y))\rangle =\langle p_1\circ j(x)| -q_2\circ k(y)\rangle +\langle p_2\circ j(x)|q_1\circ k(y)\rangle
$$

Since $p_1\circ j=|p^*_1|$ and $q_1\circ k=|q^*_1|$ (prop. 11, b) of I, p. 140) we obtain

$$
\langle b(u)x| |q^*_1|y\rangle =\langle |p^*_1|x|b(u^*)y\rangle
$$

hence $|q^*_1|b(u) =b(u^*)^*|p^*_1|$. Using formulas (1) and (4), we conclude that $b(u)|p^*_1|=|q^*_1|b(u) =b(u^*)^*|p^*_1|$, and since the image of $|p^*_1|$ is the domain of $u$, which is dense in E, we deduce $b(u) =b(u^*)^*$.

We denote by Ω(E) the set of $v\in \mathscr{L}(E)$ such that $1_E-v^*v$ is positive and injective. For $v\in \Omega (E)$, the hermitian endomorphism $(1_E-v^*v)^{1/2}$ is injective, since its square is so, and we denote by $B(v)$ the partial operator $v\circ ((1_E-v^*v)^{1/2})^{-1}$.

Note that $1_E-v^*v$ is positive if and only if $\|v\|\leqslant 1$, since one has $\langle x|(1_E-v^*v)(x)\rangle =\|x\|^2- \|v(x)\|^2$ for every $x\in E$.

#### Lemma 1 {#ts-iv-s5-lem-1 .statement tag=035C}

The subset Ω(E) is self-adjoint in $\mathscr{L}(E)$.

Let $v\in \Omega (E)$. One has $\|v^*\|=\|v\|\leqslant 1$ therefore the endomorphism $1_E-vv^*$ is positive. It is injective: if $x\in$ Ker(1$_E-vv^*$), one has $vv^*(x) =x$, whence $v^*(v(v^*(x))) =v^*(x)$ then $v^*(x) = 0$, since $1_E-v^*v$ is injective, and finally $x=v(v^*(x)) = 0$. The lemma follows.

#### Proposition 2 {#ts-iv-s5-prop-2 .statement tag=035D}

The mapping $u\mapsto b(u)$ defines a bijection of the set of closed partial operators with dense domain on E onto the set Ω(E). The inverse bijection is given by $v\mapsto B(v)$.

The relation $1_E-b(u)^*b(u) = W(u)$ (formula (3)) implies that $b(u)$ belongs to Ω(E) since $W(u)$ is positive and injective. Since moreover $b(u) =u\circ W(u)^{1/2}$ (formula (2)), one obtains

$$
u=b(u)\circ (W(u)^{1/2})^{-1}=b(u)\circ ((1-b(u)^*b(u))^{1/2})^{-1}= B(b(u))
$$

Conversely, let $v\in \Omega (E)$. Put $w= (1_E-v^*v)^{1/2}$ and let $u= B(v) =v\circ w^{-1}$. The domain of $u$ is the image of $w$, which is dense in E since $w$ is hermitian and injective (EVT, V, p. 41, prop. 4 (i)). For every $x\in$ dom($u$), one has

$$
\|u(x)\|^2=\langle (v^*v)(w^{-1}(x))|w^{-1}(x)\rangle
$$

$$
=-\langle (1_E-v^*v)(w^{-1}(x))|w^{-1}(x)\rangle +\|w^{-1}(x)\|^2
$$

$$
=-\langle w(x)|w^{-1}(x)\rangle +\|w^{-1}(x)\|^2
$$

since $(1_E-v^*v)\circ w^{-1}$ is the restriction of $w$ to the domain of $w^{-1}$. Since $w$ is self-adjoint, one deduces that

$$
\|w^{-1}(x)\|^2=\|x\|^2+\|v\circ w^{-1}(x)\|^2=\|x\|^2+\|u(x)\|^2
$$

and the partial operator $B(v) =u=v\circ w^{-1}$ is therefore closed by Lemma 2 of IV, p. 231.

Finally let us prove that $b(B(v)) =v$. Since $u=v\circ w^{-1}$, one has $v=u\circ w$, and it is therefore enough to verify that $w= W(u)^{1/2}$ (formula (2)), or even that $1_E-v^*v= W(u)$.

The endomorphism $v^*$ belongs to Ω(E) by Lemma 1. Put $w'= (1_E-vv^*)^{1/2}$. It is a positive injective endomorphism of E, and one has $v\circ w=w'\circ v$ (prop. 11 of I, p. 113). The graph of $u$ is the set of elements of the form $(w(x), v(x))$ for $x\in E$. By prop. 7 of IV, p. 236, the graph of $u^*$ is $s(\Gamma_u)^{\circ}$. Since, for all $x$ and $y\in E$, one has

$$
\langle (w'(x), v^*(x))|(-v(y), w(y))\rangle =-\langle x|w'v(y)\rangle +\langle x|vw(y)\rangle = 0
$$

the graph of $u^*$ contains elements of the form $(w'(x), v^*(x))$ for $x\in E$, and one then has $u^*(w'(x)) =v^*(x)$. In particular, the domain of $u^*$ contains the image of $w'$.

Let $x\in E$ and put $y=w^2(x) = (1_E-v^*v)(x)$, so that $x=y+v^*v(x)$. One has $y\in$ dom($u$) and $u(y) =v(w^{-1}(y)) =v(w(x)) =w'(v(x))$. In particular, $u(y)\in$ Im($w$)$\subset$ dom($u^*$), and $u^*(u(y)) =v^*(v(x))$. Hence there follows $x=y+v^*v(x) =y+u^*u(y)$, whence $y= W(u)(x)$, that is to say

$$
(1_E-v^*v)(x) = W(u)(x)
$$

Thus it has been proved that $1_E-v^*v= W(u)$, as desired.

#### Corollary {#ts-iv-s5-n1-cor-2 .statement tag=035E}

The endomorphism $b(u)$ is hermitian if and only if $u$ is self-adjoint.

This results from the injectivity of the mapping $u\mapsto b(u)$ (prop. 2) and from the formula $b(u^*) =b(u)^*$ (cor. of prop. 1).

### 2. Normal partial operators and the spectral theorem

In this number, E is a complex Hilbert space.

#### Definition 2 {#ts-iv-s5-def-2 .statement tag=035F}

Let $u$ be a partial operator on E. One says that $u$ is normal if $u$ is closed with dense domain and if its bornification $b(u)$ is a normal endomorphism of E.

If $u\in \mathscr{L}$ (E), this definition agrees with EVT, V, p. 42, def. 4, by virtue of the formulas $1_E-b(u)^*b(u) = W(u) = (1_E+u^*u)^{-1}$ (prop. 1 of IV, p. 262) and $b(u^*) =b(u)^*$ (cor. of loc. cit.).

If $u$ is a self-adjoint partial operator on E, then $b(u)$ is hermitian (cor. of prop. 2 of IV, p. 264), therefore $u$ is normal.

Let D be the open unit disk in $\mathbf{C}$. We denote by $\beta$ the function from $\mathbf{C}$ into D defined by $\beta (z) =z/\surd\overline{1 + |z|^2}$. It is a homeomorphism, whose inverse satisfies $\beta^{-1}(z) =z/\surd\overline{1 - |z|^2}$ for $z\in D$.

Let $u\in \mathscr{L}(E)$. It follows from formulas (2) and (3) of proposition 1 of IV, p. 262 that $u=\beta^{-1}(b(u))$, and therefore

$$
b(u) =\beta (u) \tag{5}
$$

#### Lemma 2 {#ts-iv-s5-lem-2 .statement tag=035G}

Let X be a locally compact topological space and let $\mu$ be a positive measure on X.

a) Let $g$ be a $\mu$-measurable function on X. The multiplication operator $m_g$ on $L^2(X, \mu)$ is normal and $b(m_g) =m_{\beta\circ g}$;

b) Let $h: X\rightarrow D$ be a $\mu$-measurable function. The endomorphism $m_h$ belongs to $\Omega (L^2(X, \mu))$ and $B(m_h) =m_{\beta^{-1}\circ h}$.

The partial operator $m_g$ is closed with dense domain. Since $m^*_gm_g=$ $m_{\overline{g}}m_g=m_{|g|^2}$ (prop. 23 of IV, p. 253 and prop. 24 of IV, p. 255), one has

$$
W(m_g) =-R(m_{|g|^2},-1) =m_{(1+|g|^2)^{-1}}
$$

(prop. 22 of IV, p. 252). This implies

$$
b(m_g) =m_g\circ W(m_g)^{1/2}=m_g\circ m_{(1+|g|^2)^{-1/2}}=m_{\beta\circ g}
$$

by formula (2) of IV, p. 262, cor. of prop. 6 of IV, p. 187 and lemma 6 of IV, p. 254. Finally applying prop. 6 of IV, p. 187, one obtains assertion a).

Let us prove b). Since $1- |h(x)|^2>0$ for every $x\in X$, one has $m_h\in$ $\Omega (L^2(X, \mu))$ (cor. of Prop. 6 of IV, p. 187). Since the mapping $u\mapsto b(u)$ is injective (Prop. 2 of IV, p. 264) and the endomorphisms $b(B(m_h))$ and $b(m_{\beta^{-1}\circ h})$ are equal to $m_h$ by assertion a), it follows that $B(m_h) =m_{\beta^{-1}\circ h}$.

#### Theorem 1 (“Spectral Theorem”) {#ts-iv-s5-thm-1 .statement tag=035H}

Let $u$ be a normal partial operator on the Hilbert space E. There exist a locally compact topological space X, a positive measure $\mu$ on X, an isometric isomorphism $\theta$ of $L^2(X, \mu)$ onto E, and a continuous function $g$ on X, such that $u=\theta \circ m_g\circ \theta^{-1}$.

The endomorphism $b(u)$ of E is normal by definition. According to the spectral theorem for normal endomorphisms of E (Corollary 1 of IV, p. 193), there therefore exist a locally compact topological space $\widetilde{X}$, a positive measure $\mu$ on $\widetilde{X}$, an isometric isomorphism $\widetilde{\theta}$ of $L^2(\widetilde{X}, \mu)$ onto E, and a bounded continuous function $h$ on $\widetilde{X}$, such that $b(u)$ coincides with $\widetilde{\theta}\circ m_h\circ \widetilde{\theta}^{-1}$.

Let N be the closed subset of the $x\in \widetilde{X}$ such that $|h(x)|\geqslant 1$. Since the endomorphism $1-b(u)^*b(u) =\widetilde{\theta}\circ m_{1-|h|^2}\circ \widetilde{\theta}^{-1}$ is positive and injective, the set N is locally $\mu$-negligible (Lemma 7 of IV, p. 186 and cor. of Prop. 6 of IV, p. 187). Put then $X =\widetilde{X}-$ N. It is a locally compact space, and the restriction of functions to X induces an isometric isomorphism of $L^2(\widetilde{X}, \mu)$ onto $L^2(X, \mu|X)$ (Prop. 1 of IV, p. 179). The composition of $\widetilde{\theta}$ and of the restriction of functions to X therefore induces an isometric isomorphism $\theta$ of $L^2(X, \mu|X)$ onto E. As $b(u) =\theta \circ m_{h|X}\circ \theta^{-1}$, it follows that $u=\theta \circ m_{\beta^{-1}\circ(h|X)}\circ \theta^{-1}$ (Lemma 2). The theorem follows from this formula.

#### Lemma 3 {#ts-iv-s5-lem-3 .statement tag=035I}

Let $u$ be a normal partial operator on E. One has

Sp($b(u)$)$\cap D =\beta$(Sp($u$)).

One has $b(u) =u\circ W(u)^{1/2}$ (Prop. 1 of IV, p. 262). The endomorphism $W(u)^{1/2}$ is injective and its image is the domain of $u$ (formula (1) of IV, p. 262).

Let $\lambda \in \mathbf{C}$. The number $\lambda$ belongs to the resolvent set of $u$ if and only if $(u-\lambda 1_E)\circ W(u)^{1/2}$ is a bijective linear mapping of E into E (Remark 3 of IV, p. 245). Now, by formula (3) of IV, p. 262, one has

$$
(u-\lambda 1_E)\circ W(u)^{1/2}=b(u)-\lambda (1_E-b(u)^*b(u))^{1/2}=f_{\lambda}(b(u))
$$

where $f_{\lambda}$ is the continuous function defined on $\overline{D}$ by $z\mapsto z-\lambda (1- |z|^2)^{1/2}$. The endomorphism $f_{\lambda}(b(u))$ is bijective if and only if its spectrum does not contain 0. Since Sp($f_{\lambda}(b(u))$) $=f_{\lambda}$(Sp($b(u)$)) (Corollary 2 of Proposition 7 of I, p. 111), this is so if and only if 0 does not belong to the set $f_{\lambda}$(Sp($b(u)$)). Thus, $\lambda \in$ Sp($u$) if and only if there exists $z\in$ Sp($b(u)$)$\cap D$ such that

$$
z-\lambda (1- |z|^2)^{1/2}= 0
$$

This equality, if it is valid, implies that $z\in D$, and means that $\lambda =\beta^{-1}(z)$. It follows that Sp($u$) $=\beta^{-1}$(Sp($b(u)$)$\cap D$), as stated.

Let $u$ be a normal partial operator on E. Let $f\in \mathscr{K}$ (Sp($u$)). The mapping $z\mapsto f(\beta^{-1}(z))$ of Sp($b(u)$)$\cap D$ into $\mathbf{C}$ is continuous and has compact support; the unique mapping $f_{\beta}$ of Sp($b(u)$) into $\mathbf{C}$ which extends it by zero is therefore continuous.

#### Definition 3 {#ts-iv-s5-def-3 .statement tag=035J}

For every function $f\in \mathscr{K}$ (Sp($u$)), one defines the endomorphism $f(u)$ of E by $f(u) =f_{\beta}(b(u))$.

The mapping $f\mapsto f_{\beta}$ is a complex algebra morphism of $\mathscr{K}$ (Sp($u$)) into $\mathscr{C}$(Sp($b(u)$)), hence the mapping $f\mapsto f(u)$ is a complex algebra morphism of $\mathscr{K}$ (Sp($u$)) into $\mathscr{L}(E)$. One has $\overline{f}(u) =f(u)^*$ since $\overline{f}_{\beta}=\overline{f_{\beta}}$. If $f\geqslant 0$ then $f_{\beta}\geqslant 0$, hence $f(u)$ is a positive endomorphism of E.

#### Remark {#ts-iv-s5-n2-rem-3 .statement tag=035K}

Suppose that $u$ is a normal endomorphism of E, so that Sp($u$) is a compact subset of $\mathbf{C}$. Since the bounded transform $b(u)$ coincides with $\beta (u)$ (formula (5)), and Sp($b(u)$) $=\beta$(Sp($u$)) (Corollary 2 of Proposition 7 of I, p. 111), the spectrum of $b(u)$ is a compact subset of D. For every continuous function $f\in \mathscr{C}$ (Sp($u$)), the function $f_{\beta}$ coincides with the restriction of $f\circ \beta^{-1}$ to Sp($u$). Consequently, $f_{\beta}(\beta (u))$ coincides with the endomorphism $f(u)$ defined by the continuous functional calculus of $u$. The above definition is therefore compatible with that of the continuous functional calculus of the involutive algebra $\mathscr{L}(E)$.

Let $f\in \mathscr{K}$ (Sp($u$)). We have

$$
\|f(u)\|\leqslant \|f_{\beta}\|_{\infty}=\|f\|_{\infty}
$$

so that, for all $x$ and $y$ in E, one obtains the inequality $|\langle x|f(u)y\rangle |\leqslant \|x\| \|y\| \|f\|_{\infty}$. The mapping $f\mapsto  \langle x|f(u)y\rangle$ is therefore a bounded measure on Sp($u$), of total mass $\leqslant \|x\|\|y\|$ (INT, IV, p. 154, § 4, n$^o7$). If $x=y$, it is a positive measure, since $f(u)$ is positive when $f\geqslant 0$.

#### Definition 4 {#ts-iv-s5-def-4 .statement tag=035L}

Let $u$ be a normal partial operator on a complex Hilbert space E. Let $x$ and $y$ be in E. The bounded measure on Sp($u$) defined by $f\mapsto  \langle x|f(u)y\rangle$ for $f\in \mathscr{K}$ (Sp($u$)) is called the spectral measure of $(x, y)$ relative to $u$. When $x=y$, one says that it is the spectral measure of $x$ relative to $u$.

#### Remark 1 {#ts-iv-s5-n2-rem-1 .statement tag=035M}

When $u$ is continuous, this definition coincides with that of Definition 2 of IV, p. 190.

#### Remark 2 {#ts-iv-s5-n2-rem-2 .statement tag=035N}

Let $j$ be the canonical inclusion of Sp($u$) in $\mathbf{C}$. Since Sp($u$) is closed, the mapping $j$ is $\mu$-proper for every bounded measure $\mu$ on Sp($u$) (INT, V, p. 68, § 6, n$^o1$, Proposition 1). One will often identify the spectral measures of $u$ with the measures on $\mathbf{C}$ which are their images under $j($cf. INT, V, p. 84, § 7, n$^o2)$.

The mapping of $E\times E$ into the Banach space $\mathscr{M}^1$(Sp($u$)) which associates to $(x, y)$ the spectral measure of $(x, y)$ relative to $u$ is sesquilinear and continuous of norm $\leqslant 1$.

#### Lemma 4 {#ts-iv-s5-lem-4 .statement tag=035O}

Let X be a locally compact topological space, let $\mu$ be a positive measure on X, and let $g$ be a $\mu$-measurable function on X. Let $m_g$ be the operator of multiplication by $g$ on $L^2(X, \mu)$.

a) The mapping $f\mapsto f(m_g)$ of $\mathscr{K}$ (Sp($m_g$)) into $\mathscr{L}(L^2(X, \mu))$ is given by $f\mapsto m_{f\circ g}$;

b) For $f_1$ and $f_2$ in $\mathscr{L}^2(X, \mu)$ of classes $\widetilde{f}_1$ and $\widetilde{f}_2$ in $L^2(X, \mu)$, the spectral measure dede of the image measure $g(\frac{(}{f}\widetilde{f}_{11}f,_2\widetilde{f}\cdot^2\mu)$ )relative to. $m_g$ is the restriction to Sp($m_g$)

The partial operator $m_g$ is normal and $b(m_g) =m_{\beta\circ g}=m_{g(1+|g|^2)^{-1/2}}$ (lemma 2). Moreover $\beta (g(x))$ belongs to Sp($m_{\beta\circ g}$) for every $x$ outside a locally $\mu$-negligible set $Y\subset X$ (proposition 22 of IV, p. 252 and lemma 1 of IV, p. 181). Since $f_{\beta}(\beta (g(x))) =f(g(x))$ for every $x\in X$ - Y, it follows that $f(m_g) =m_{f\circ g}$ from definition 3 and the cor. of prop. 6 of IV, p. 187.

Let $f_1$ and $f_2$ be in $\mathscr{L}^2(X, \mu)$ of classes $\widetilde{f}_1$ and $\widetilde{f}_2$ in $L^2(X, \mu)$. Since the measure $\nu =f_1f_2\cdot \mu$ is bounded, the image measure $g(\nu )$ is defined (INT, V, p. 69, § 6, n$^o1$, rem. 1). Let $f\in \mathscr{K}$ (Sp($m_g$)). We have $f(m_g) =m_{f\circ g}$ by a), whence

$$
\langle \widetilde{f}_1|f(m_g)\widetilde{f}_2\rangle =\int_X\overline{f}_1(f\circ g)f_2d\mu=\int_X(f\circ g) (\overline{f}_1f_2d\mu) =\int_{\mathbf{C}}f d\nu
$$

(INT, V, p. 69, § 6, n$^o1$, formula (1)), which establishes assertion b).

#### Example {#ts-iv-s5-n2-exa-1 .statement tag=035P}

Let $n\in \mathbf{N}$. We endow $\mathbf{R}^n$ with Lebesgue measure, and we identify $\mathbf{R}^n$ and its dual group as in corollary 3 of II, p. 236. Let N denote the euclidean norm on $\mathbf{R}^n$ and $\mathscr{F}$ the Fourier transform on $\mathscr{S}(\mathbf{R}^n)$ and on $\mathscr{S}'(\mathbf{R}^n)$ (n$^o12$ of IV, p. 217).

Let $\Delta_{\mathscr{S}}$ be the partial operator on $L^2(\mathbf{R}^n)$ whose domain is the space $\mathscr{S}(\mathbf{R}^n)$ and such that

$$
\Delta_{\mathscr{S}}(\varphi ) =-\sum_{i=1}^n\partial_i^2\varphi
$$

for every $\varphi \in \mathscr{S}(\mathbf{R}^n)$. One then has $\mathscr{F}(\Delta_{\mathscr{S}}(\varphi )) = 4\pi^2N^2\mathscr{F}(\varphi )$ for every function $\varphi \in \mathscr{S}(\mathbf{R}^n)$ (remark 12 of IV, p. 220). Since the Fourier transform is an automorphism of $\mathscr{S}(\mathbf{R}^n)$ (prop. 18 of IV, p. 219), this means that the partial operator $u=\mathscr{F}\circ \Delta_{\mathscr{S}}\circ \mathscr{F}^{-1}$ is the restriction of the multiplication operator $m_{4\pi^2N^2}$ to the space $\mathscr{S}(\mathbf{R}^n)$. The partial operator $u$ is closable and symmetric; its closure is the positive self-adjoint partial operator $m_{4\pi^2N^2}$ (prop. 6 of IV, p. 232, applied to the space $\mathscr{D}(\mathbf{R}^n)\subset \mathscr{S}(\mathbf{R}^n)$ with the aid of prop. 4 of IV, p. 202). Consequently, the partial operator $\Delta_{\mathscr{S}}$ is essentially self-adjoint. Its closure is denoted by Δ; it is a positive self-adjoint operator, and it is the unique Laplacian on $\mathbf{R}^n($cf. example of No.$^o6$ of IV, p. 243 and cor. to prop. 26 of IV, p. 257).

According to prop. 21 of IV, p. 223, the Sobolev space $H^2(\mathbf{R}^n)$ is the set of $f\in L^2(\mathbf{R}^n)$ such that $(1 + N^2)\mathscr{F}(f)$ belongs to $L^2(\mathbf{R}^n)$, that is to say such that $\mathscr{F}(f)$ belongs to the domain of $m_{4\pi^2N^2}$. Since the Fourier transform is an isometric isomorphism of the space $L^2(\mathbf{R}^n)$ onto itself (th. 1 of II, p. 215), the domain of the Laplacian Δ is $H^2(\mathbf{R}^n)$. One has $\Delta  =\mathscr{F}^{-1}\circ m_{4\pi^2N^2}\circ \mathscr{F}$. In particular, the spectrum of Δ is equal to $\mathbf{R}_+$.

### 3. Universally measurable functional calculus

In this No. the Hilbert spaces considered are complex.

Let $u$ be a normal partial operator on a Hilbert space E. Denote by $\mu_{x,y}$ (resp. $\mu_y$) the spectral measure of $(x, y)\in E\times E$ (resp. of $y$) relative to $u$.

Let $y\in E$. The mapping $\mathscr{K}$ (Sp($u$))$\rightarrow E$ defined by $f\mapsto f(u)(y)$ satisfies

$$
\|f(u)(y)\|^2=\int|f|^2\mu_y=\|f\|^2_{\mathscr{L}^2(Sp(u),\mu_y)}
$$

Sp($u$)

There therefore exists a unique isometric linear mapping ev$_y$ of the space $L^2$(Sp($u$)$, \mu_y$) into E such that ev$_y(\widetilde{f}) =f(u)(y)$ if $\widetilde{f}$ is the class of a function $f\in \mathscr{K}$ (Sp($u$)).

Let $f$ be a universally measurable function defined on the spectrum of $u$. Denote by $D_f$ the set of elements $y\in E$ such that $f$ belongs to $\mathscr{L}^2$(Sp($u$)$, \mu_y$).

#### Proposition 3 {#ts-iv-s5-prop-3 .statement tag=035Q}

Let $f$ be a universally measurable function defined on the spectrum of $u$. The set $D_f$ is a dense vector subspace of E. The mapping $y\mapsto$ ev$_y(f)$ is a normal partial operator on E whose domain is $D_f$, and which is denoted by $f(u)$.

For every $x\in E$ and every $y\in D_f$, one has $f\in \mathscr{L}^1$(Sp($u$)$, \mu_{x,y}$) and

$$
\langle x|f(u)y\rangle =\int f \mu_{x,y} \tag{6}
$$

Sp($u$)

We shall prove the following more precise statement:

#### Proposition 4 {#ts-iv-s5-prop-4 .statement tag=035R}

Let $f$ be a universally measurable function on the spectrum of $u$.

a) The set $D_f$ is a dense vector subspace of E. The mapping $f(u) :y\mapsto$ ev$_y(f)$ of $D_f$ into E is linear and coincides with $1_E$ if $f= 1$;

b) Let $g\in \mathscr{L}_u$(Sp($u$)). For every $y\in D_f$ and every $x\in D_g$, one has $f g\in \mathscr{L}^1$(Sp($u$)$, \mu_{x,y}$), and

$$
\langle g(u)x|f(u)y\rangle =\int gf \mu_{x,y} \tag{7}
$$

Sp($u$)

c) Suppose that $E = L^2(X, \mu)$ where X is a locally compact topological space and $\mu$ a positive measure on X, and that $u=m_h$, where $h: X\rightarrow \mathbf{C}$ is $\mu$-measurable. One has $f(m_h) =m_{f\circ h}$.

According to Theorem 1 of IV, p. 266, one may suppose that one is in the situation of assertion c), that is to say that $E = L^2(X, \mu)$ and $u=m_h$, where X is a locally compact topological space, $\mu$ a positive measure on X and $h: X\rightarrow \mathbf{C}$ is $\mu$-measurable. We shall denote by $\widetilde{\varphi}$ the class in $L^2(X, \mu)$ of a function $\varphi \in \mathscr{L}^2(X, \mu)$.

Let S = Sp($m_h$). We denote by $\mu_{\widetilde{\varphi}_1,\widetilde{\varphi}_2}$ (resp. $\mu_{\widetilde{\varphi}}$) the spectral measure of $(\widetilde{\varphi}_1,\widetilde{\varphi}_2)$ (resp. of $\widetilde{\varphi}$) relative to $m_h$ for every $(\varphi_1, \varphi_2)\in \mathscr{L}^2(X, \mu)^2$ (resp. every $\varphi \in \mathscr{L}^2(X, \mu)$).

Let $\varphi \in \mathscr{L}^2(X, \mu)$. The spectral measure $\mu_{\widetilde{\varphi}}$ is equal to the image measure $h(|\varphi |^2\cdot \mu)$ on S (Lemma 4 of IV, p. 269). Since the function $f$ is $\mu_{\varphi}$-measurable, one has $\varphi \in D_f$ if and only if the integrals

$$
\int_S^*|f|^2d\mu_{\widetilde{\varphi}}=\int_S^*|f|^2h(|\varphi |^2d\mu) =\int_X^*|f\circ h|^2|\varphi |^2d\mu
$$

are finite (INT, V, p. 70, § 6, n$^o2$, prop. 2). This means that $D_f$ is the domain of the multiplication operator $m_{f\circ h}$, which is a dense subspace of E (prop. 5 of IV, p. 232).

The restriction of ev$_{\widetilde{\varphi}}$ to classes of functions $g\in \mathscr{K}(S)$ is the mapping which to a class $\widetilde{g}$ associates the element $g(m_h)(\widetilde{\varphi}) =m_{g\circ h}(\widetilde{\varphi})$ (lemma 4 of IV, p. 269). The mapping ev$_{\varphi}$ therefore coincides with the isometric mapping of $L^2(S, \mu_{\varphi})$ into $L^2(X, \mu)$ deduced by passing to quotients from the mapping $g\widetilde{\mapsto}(g\circ h)\cdot \varphi$ of $\mathscr{L}^2(S, \mu_{\widetilde{\varphi}})$ into $\mathscr{L}^2(X, \mu)$.

In particular, therefore, we have ev$_{\varphi}(f) =m_{f\circ h}(\widetilde{\varphi})$, so that the mapping $f(m_h)$ of $D_f$ into E coincides with the partial operator $m_{f\circ h}$. This proves assertion c); if $f= 1$, we find ev$_{\varphi}(1) =\widetilde{\varphi}$, which also concludes the proof of a).

Let us prove assertion b). Let $\varphi_1$ and $\varphi_2$ be functions such that $\widetilde{\varphi}_1\in D_f$ and $\widetilde{\varphi}_2\in D_g$. We then have (INT, V, loc. cit.)

$$
\int_S^*|f g| |\mu_{\widetilde{\varphi}_1,\widetilde{\varphi}_2}|=\int_X^*|(f\circ h)(g\circ h)\varphi_1\varphi_2|d\mu
$$

$$
\leqslant \|(f\circ h)\varphi_1\| \|(g\circ h)\varphi_2\|
$$

which is finite; hence $f g\in \mathscr{L}^1(S, \mu_{\widetilde{\varphi}_1,\widetilde{\varphi}_2})$. Moreover, we then have

$$
\langle g(m_h)(\widetilde{\varphi}_2)|f(m_h)(\widetilde{\varphi}_1)\rangle =\int_X\overline{(g\circ h) \varphi_2}(f\circ h)\varphi_1d\mu
$$

$$
=\int_Sgf d\mu_{\widetilde{\varphi}_1,\widetilde{\varphi}_2}
$$

which concludes the proof.

#### Definition 5 {#ts-iv-s5-def-5 .statement tag=035S}

The mapping $f\mapsto f(u)$ of $\mathscr{L}_u$(Sp($u$)) into the set of normal partial operators on E defined by prop. 3 of IV, p. 271 is called the universally measurable functional calculus mapping associated with $u$.

More generally, let T be a set and $g:$ Sp($u$)$\times T\rightarrow \mathbf{C}$ a mapping; let $t\in T$ be such that the function $g_t:z\mapsto g(z, t)$ is universally measurable on Sp($u$). We then write $g(u, t) =g_t(u)$.

Formula (7) implies in particular that (8) $\|f(u)(y)\|^2=\int|f|^2\mu_y$

Sp($u$)

for every $f\in \mathscr{L}_u$(Sp($u$)) and every $y\in D_f$. Taking $f= 1$, we deduce that $\mu_y$ is a positive measure of total mass $\|y\|^2$.

If $u$ is a normal partial operator on a Hilbert space E and $f\in \mathscr{K}$ (Sp($u$)), then $D_f= E$ and the partial operator $f(u)$ is then continuous, since

$$
\|f(u)y\|\leqslant \|f\|_{\infty}\|y\|
$$

for every $y\in E$ by (8). The endomorphism $f(u)$ coincides with that of Definition 3 of IV, p. 268.

#### Corollary 1 {#ts-iv-s5-def-5-cor-1 .statement tag=035T}

a) For every $f\in \mathscr{L}_u$(Sp($u$)), the partial operator $f(u)$ is normal and $f(u)^*=\overline{f}(u)$. Moreover, $f(u)$ is positive if $f\geqslant 0$, and self-adjoint if $f$ is real-valued;

b) Let $k\in \mathbf{N}$ and $f(z) =z^k$ for $z\in$ Sp($u$). Then $f(u) =u^k$;

c) Let $\lambda \in \mathbf{C}-$ Sp($u$) and $f(z) = (\lambda -z)^{-1}$ for $z\in$ Sp($u$). Then $f(u) = R(u, \lambda )$;

d) One has $\beta (u) =b(u)$;

e) Let $f\in \mathscr{L}_u$(Sp($u$)) and $g\in \mathscr{L}_u$(Sp($u$)) be such that $|g|\leqslant 1 +|f|$. The domain of $g(u)$ is a core for $f(u)$.

In view of the spectral theorem (th. 1 of IV, p. 266), this follows from the preceding proposition combined, respectively, with:

a) lemma 2, a) of IV, p. 266, prop. 23 of IV, p. 253, and its corollary;

b) prop. 24, b) of IV, p. 255;

c) prop. 22, b) of IV, p. 252;

d) lemma 2, a) of IV, p. 266;

e) prop. 6, b) of IV, p. 232.

#### Remark {#ts-iv-s5-n3-rem-1 .statement tag=035U}

For $f=$ Id$_{Sp(u)}$, one has $f(u) =u$ (assertion b) for $k= 1$). The domain of $u$ therefore coincides with the set of $x\in E$ such that the identity function of Sp($u$) belongs to $\mathscr{L}^2$(Sp($u$)$, \mu_x$); in particular it contains the elements $x\in E$ such that the measure $\mu_x$ has compact support.

The following corollary generalizes the corollary to prop. 16 of IV, p. 247 and prop. 17 of IV, p. 248.

#### Corollary 2 {#ts-iv-s5-def-5-cor-2 .statement tag=035V}

Let $u$ be a normal partial operator on the Hilbert space E. It is supposed that E is nonzero.

a) The spectrum of $u$ is nonempty;

b) For every $\lambda \in \mathbf{C}-$ Sp($u$), the norm of the resolvent $R(u, \lambda )$ is equal to $1/\delta$, where $\delta  >0$ is the distance in $\mathbf{C}$ from $\lambda$ to the spectrum of $u$.

c) For every $\varepsilon  >$ 0, the $\varepsilon$-pseudospectrum PSp$_{\varepsilon}(u)$ is the set of $\lambda \in \mathbf{C}$ at distance $< \varepsilon$ from Sp($u$).

Suppose that the spectrum of $u$ is empty. Then $u$ is injective, and the endomorphism $u^{-1}=-R(u,0)$ is normal (cor. 1, c) and a)). We have Sp($u^{-1}$)$\subset  \{0\}$ (prop. 15, a)), hence Sp($u^{-1}$) $=\{0\}($I, p. 26, cor. 1). Since $u^{-1}$ is normal, this implies that $u^{-1}= 0 ($I, p. 110, example 1), which is a contradiction since E is not zero.

To prove b), one may suppose that $u$ is the multiplication operator $m_g$ on $L^2(X, \mu)$, where $g$ is a continuous function on a locally compact topological space X endowed with a positive measure $\mu$ (th. 1 of IV, p. 266). Let $\lambda \in \mathbf{C}-$ Sp($u$) and let $\delta  >0$ be the distance from $\lambda$ to the spectrum of $u$. To prove that $\|R(u, \lambda )\|=\delta^{-1}$, one is reduced to the case $\lambda = 0$ by replacing $u$ by $u-\lambda 1_E$. The real number $\delta$ is then the distance from 0 to the spectrum of $m_g$. Since the latter coincides with the $\mu$-essential image of $g$, the result is a consequence of lemma 3 of IV, p. 182.

Finally, assertion c) follows from b) and from the definition of PSp$_{\varepsilon}(u)$ (IV, p. 250, def. 9).

#### Corollary 3 {#ts-iv-s5-def-5-cor-3 .statement tag=035W}

Let $u$ be a partial normal operator on a Hilbert space E. Let $f\in \mathscr{L}_u$(Sp($u$)). For all $x$ and $y$ in E, the spectral measure of $(x, y)$ relative to $f(u)$ is the image measure $f(\mu)$, where $\mu$ is the spectral measure of $(x, y)$ relative to $u$.

In view of the spectral theorem (th. 1 of IV, p. 266), one may suppose that $u$ is the multiplication operator $m_g$ on $L^2(X, \mu)$, where X is a locally compact topological space, $\mu$ a positive measure on X and $g\in \mathscr{C}(X)$. Let $f_1$ and $f_2$ be in $\mathscr{L}^2(X, \mu)$, with classes $\widetilde{f}_1$ and $\widetilde{f}_2$ in $L^2(X, \mu)$. Since $f(m_g) =m_{f\circ g}$ (prop. 4, c)), the spectral measure of $(\widetilde{f}_1,\widetilde{f}_2)$ relative to $f(m_g)$ is the image measure $(f\circ g)(\overline{f}_1f_2\cdot \mu)$ (lemma 4, b) of IV, p. 269). This measure is equal to the image measure $f(g(f_1f_2\cdot \mu))$ (INT, V, p. 72, § 6, n$^o4$, prop. 4, a)), whence the assertion (lemma 4, b) of IV, p. 269).

#### Corollary 4 {#ts-iv-s5-def-5-cor-4 .statement tag=035X}

Let $g\in \mathscr{L}_u$(Sp($f(u)$)). We have $g(f(u)) = (g\circ f)(u)$.

We have $g\circ f\in \mathscr{L}_u$(Sp($u$)) (lemma 5 of IV, p. 184). For all $x$ and $y$ in E, let us denote by $\mu'_{x,y}$ the spectral measure of $(x, y)$ relative to $f(u)$. By the preceding corollary and INT, V, p. 71, § 6, No. 2, th. 1, we have $g\in \mathscr{L}^2$(Sp($f(u)$)$, \mu'_{x,y}$) if and only if $g\circ f\in \mathscr{L}^2$(Sp($u$)$, \mu_{x,y}$), so that the domain of $g(f(u))$ is equal to the domain of $(g\circ f)(u)$. For all $x\in E$ and $y\in$ dom($g(f(u))$), we then have the formula

$$
\langle x|g(f(u))y\rangle =\int g \mu'_{x,y}
$$

Sp($f(u)$)

$=\int g f(\mu_{x,y}) =\langle x|(g\circ f)y\rangle$

Sp($f(u)$)

(loc. cit.), whence $g(f(u)) = (g\circ f)(u)$.

#### Proposition 5 {#ts-iv-s5-prop-5 .statement tag=035Y}

Let $u$ be a normal partial operator on a Hilbert space E.

a) If $f\in \mathscr{L}_u^{\infty}$(Sp($u$)), then $f(u)\in \mathscr{L}(E)$;

b) If $f\in \mathscr{L}_u^{\infty}$(Sp($u$)) and $g\in \mathscr{L}_u$(Sp($u$)), then $f(u)\circ g(u)\subset (f g)(u)$;

c) The mapping $f\mapsto f(u)$ of $\mathscr{L}_u^{\infty}$(Sp($u$)) into $\mathscr{L}(E)$ is a continuous unital morphism of involutive algebras. In particular, we have $\|f(u)\|\leqslant \|f\|_{\infty}$ for $f\in \mathscr{L}_u^{\infty}$(Sp($u$));

d) If $u\in \mathscr{L}(E)$, then for every $f\in \mathscr{L}_u^{\infty}$(Sp($u$)), the endomorphism $f(u)$ belongs to the bicommutant of $u$ in $\mathscr{L}(E)$.

Let $f\in \mathscr{L}_u^{\infty}$(Sp($u$)). We have $D_f= E$ and $f(u)$ is a continuous endomorphism of E by formula (8), p. 272, whence assertion a).

Let $g\in \mathscr{L}_u$(Sp($u$)). Let $y\in D_g$. We have $y\in D_{f g}$ and, for every $x\in E$, there follows $\langle \overline{f}(u)x|g(u)y\rangle =\langle x|(f g)(u)y\rangle$ by formula (7), p. 271, whence $f(u)(g(u)y) = (f g)(u)(y)$, which proves b).

From a) and b), the mapping $f\mapsto f(u)$ of $\mathscr{L}_u^{\infty}$(Sp($u$)) into $\mathscr{L}(E)$ is a unital morphism of involutive algebras; consequently, it is a continuous morphism of norm $\leqslant 1$(I, p. 104, prop. 2), whence assertion c).

Suppose that $u$ is an endomorphism of E. Let $v\in \mathscr{L}(E)$ be permutable with $u$. Then one has $v\circ f(u) =f(u)\circ v$ for $f\in \mathscr{C}$ (Sp($u$)) by the properties of the continuous functional calculus (I, p. 110, remark). Let $x$ and $y$ be in E. The formulas

$$
\langle x|(v\circ f(u))y\rangle =\langle x|(f(u)\circ v)y\rangle \tag{9}
$$

valid for every function $f\in \mathscr{C}$ (Sp($u$)), mean that the spectral measures of $(v^*(x), y)$ and of $(x, v(y))$ relative to $u$ are equal. By formula (6), p. 271, this equality implies that formula (9) is valid for every $f\in \mathscr{L}_u^{\infty}$(Sp($u$)). Hence $v\circ f(u) =f(u)\circ v$.

#### Corollary {#ts-iv-s5-n3-cor-1 .statement tag=035Z}

Let $f$ and $g$ be in $\mathscr{L}_u$(Sp($u$)) and let $(x, y)\in D_f\times D_g$. The spectral measure of $(f(u)x, g(u)y)$ relative to $u$ is the measure $f g\cdot \mu_{x,y}$, where $\mu_{x,y}$ is the spectral measure of $(x, y)$ relative to $u$.

Let $\nu$ denote the spectral measure of $(f(u)x, g(u)y)$ relative to $u$. For every function $\varphi \in \mathscr{K}$ (Sp($u$)), one has

$$
\int\varphi  \nu =\langle f(u)x|\varphi (u)(g(u)y)\rangle
$$

Sp($u$)

$=\langle f(u)x|(\varphi g)(u)y\rangle =\int f \varphi g \mu_{x,y}$,

Sp($u$)

(prop. 5, b)), whence $\nu =f g\cdot \mu_{x,y}$.

#### Proposition 6 {#ts-iv-s5-prop-6 .statement tag=0360}

Let $u$ be a normal partial operator on a Hilbert space E. Let $(f_n)_{n\in\mathbf{N}}$ be a sequence in $\mathscr{L}_u$(Sp($u$)) which converges simply to $f\in \mathscr{L}_u$(Sp($u$)) and such that there exists $g\in \mathscr{L}_u$(Sp($u$)) satisfying $|f_n|\leqslant g$ for all $n\in \mathbf{N}$. Then dom($g(u)$)$\subset$ dom($f_n(u)$) for all $n\in \mathbf{N}$ and dom($g(u)$)$\subset$ dom($f(u)$). Moreover, for every element $y$ of the domain of $g(u)$, one has

$f(u)(y) =$ lim$_{n\rightarrow+\infty}f_n(u)(y)$.

In particular, if $f_n\in \mathscr{L}_u^{\infty}$(Sp($u$)) for all $n\in \mathbf{N}$ and if the functions $f_n$ are uniformly bounded, then $f_n(u)$ converges to $f(u)$ in the space $\mathscr{L}(E)$ endowed with the topology of simple convergence.

Let us denote by $\mu_{x,y}$ (resp. $\mu_x$) the spectral measure of $(x, y)$ (resp. of $x$) relative to $u$.

Let $y\in$ dom($g(u)$), so that $g\in \mathscr{L}^2$(Sp($u$)$, \mu_y$). The condition $|f_n|\leqslant g$ implies that $f_n\in \mathscr{L}^2$(Sp($u$)$, \mu_y$), hence $y\in$ dom($f_n(u)$).

Since $(f_n)$ converges simply to $f$ and $|f_n|\leqslant g$, one has $f\in \mathscr{L}^2$(Sp($u$)$, \mu_y$) by Lebesgue's theorem (INT, IV, p. 137, § 3, n$^o7$, th. 6), hence $y\in$ dom($f(u)$). Moreover, the sequence $(f_n)$ converges to $f$ in $\mathscr{L}^2$(Sp($u$)$, \mu_y$), hence the norm of $f_n(u)y$ converges to the norm of $f(u)y$.

Let $x\in E$. The functions $f$ and $g$, as well as the functions $f_n$ for every $n\in \mathbf{N}$, belong to $\mathscr{L}^1$(Sp($u$)$, \mu_{x,y}$) (prop. 3). By Lebesgue's theorem (INT, IV, loc. cit.), the sequence $(f_n)$ converges to $f$ in $\mathscr{L}^1$(Sp($u$)$, \mu_{x,y}$), whence

$$
\langle x|f_n(u)y\rangle =\int f_n\mu_{x,y}\rightarrow \int f \mu_{x,y}=\langle x|f(u)y\rangle
$$

Sp($u$) Sp($u$)

It follows that $f_n(u)(y)$ converges to $f(u)(y)$ (EVT, V, p. 17, prop. 10).

#### Proposition 7 {#ts-iv-s5-prop-7 .statement tag=0361}

Let X be a locally compact topological space and $\nu$ a measure on X. Let $g:\mathbf{C}\times X\rightarrow \mathbf{C}$ be a continuous function with compact support. For $z\in \mathbf{C}$, put

$$
h(z) =\int_Xg(z, x)d\nu (x)
$$

a) The mapping $h$ of $\mathbf{C}$ into $\mathbf{C}$ is continuous and bounded;

b) The mapping of X into $\mathscr{L}(E)$ defined by $x\mapsto g(u, x)$ is $\nu$-integrable and one has

$$
h(u) =\int_Xg(u, x)d\nu (x)
$$

The function $h$ is bounded because $g$ is continuous with compact support, and it is continuous by INT, IV, p. 144, § 4, n$^o3$, cor. 1. Since $g$ is continuous and with compact support, the mapping $x\mapsto g(u, x)$ is continuous from X into $\mathscr{L}(E)$ (TG, X, p. 28, th. 3 and prop. 5, c)). This mapping has compact support, hence is bounded and integrable on X with respect to $\nu$. Let us write

$$
v=\int_Xg(u, x)d\nu (x)\in \mathscr{L}(E)
$$

Let $y$ and $z$ be elements of E and $\mu$ the spectral measure of $(y, z)$ relative to $u$. One has

$$
\langle y|v(z)\rangle =\int\langle y|g(u, x)z\rangle d\nu (x) =\int(\int g(\lambda , x)d\mu(\lambda ))d\nu (x)
$$

X X Sp($u$)

(formula (6), p. 271). Since $g\in \mathscr{K}(\mathbf{C}\times X)$, it follows that

$$
\langle y|v(z)\rangle =\int_{Sp(u)}(\int_Xg(\lambda , x)d\nu (x))d\mu(\lambda ) =\langle y|h(u)z\rangle
$$

by INT, III, p. 84, § 4, n$^o1$, th. 2 and formula (6), p. 271. This proves that $v=h(u)$, as required.

### 4. Spectral projectors

Let $u$ be a partial normal operator on a complex Hilbert space E. Let A be a universally measurable subset of Sp($u$) and $\varphi_A$ its characteristic function. Since $\varphi_A$ is bounded and satisfies $\varphi^2_A=\varphi_A$, the endomorphism $\varphi_A(u)$ of E is an orthogonal projector of E. It is called the spectral projector of $u$ defined by A. We denote it by $p_A=\varphi_A(u)$. One has $p_{\emptyset}= 0$ and $p_{Sp(u)}= 1_E$.

Let A be a universally measurable subset of $\mathbf{C}$. The spectral projector of $u$ defined by A is the spectral projector $p_{Sp(u)\cap A}$. It is also denoted simply by $p_A$. For every function $f\in \mathscr{L}_u$(Sp($u$)), every $x\in E$ and every $y\in$ dom($f(u)$), one has the formula

$$
\langle p_A(x)|f(u)y\rangle =\int f d\mu \tag{10}
$$

Sp($u$)$\cap A$

where $\mu$ is the spectral measure of $(x, y)$ relative to $u$ (formula (7), p. 271).

Let A and B be universally measurable subsets of Sp($u$). Since $\varphi_A\varphi_B=\varphi_{A\cap B}$, one has $p_A\circ p_B=p_{A\cap B}$ (prop. 5 of IV, p. 275, c)). In particular, if A and B are disjoint, the images of $p_A$ and of $p_B$ are orthogonal.

#### Proposition 8 {#ts-iv-s5-prop-8 .statement tag=0362}

Let $(A_i)_{i\in I}$ be a denumerable family of pairwise disjoint universally measurable subsets of Sp($u$), and let $p_i$ be the spectral projector of $u$ defined by $A_i$. The union A of the sets $A_i$ is a universally measurable subset of Sp($u$), and the series $\sum_ip_i$ converges to $p_A$ in $\mathscr{L}(E)$ endowed with the topology of simple convergence.

The set A is universally measurable by INT, IV, p. 177, § 5, n$^o4$, cor. 2. The series $\sum_i\varphi_{A_i}$ converges simply to $\varphi_A$ and its partial sums are bounded by 1. The assertion therefore results from prop. 6 of IV, p. 276.

#### Proposition 9 {#ts-iv-s5-prop-9 .statement tag=0363}

Let A be a closed subset of Sp($u$). Let $\varphi_A$ be the characteristic function of A and $p_A=\varphi_A(u)$ the spectral projector of $u$ defined by A. Let us denote by $E_A$ the image of $p_A$. It is a closed subspace of E.

a) The subspace $E_A$ is the space of the $x\in E$ such that the support of the spectral measure of $x$ relative to $u$ is contained in A;

b) If A is bounded in $\mathbf{C}$, then $E_A$ is contained in the domain of $u$;

c) For every $x$ belonging to the domain of $u$, one has $p_A(x)\in$ dom($u$) and $u(p_A(x))\in E_A$, in particular $u(x)\in E_A$ if $x\in$ dom($u$)$\cap E_A$.

For $x$ in E, one denotes by $\mu_x$ the spectral measure of $x$ relative to $u$.

Let us prove a). Let $x$ be an element of $E_A$. Let $z\in \mathbf{C}-$ A and U a relatively compact open neighbourhood of $z$ which does not meet A. For every function $f\in \mathscr{K}(\mathbf{C})$ with support contained in U, one has

$$
\int f \mu_x=\langle x|f(u)x\rangle =\langle p_A(x)|f(u)x\rangle =\int f \mu_x= 0
$$

Sp($u$) Sp($u$)$\cap A$ according to formula (10). This means that $z$ does not belong to the support of $\mu_x$. Consequently, the support of $\mu_x$ is contained in A.

Conversely, let $x\in E$ be such that the support of $\mu_x$ is contained in A. We have

$$
\langle x|p_A(x)\rangle =\int\mu_x=\int\mu_x=\langle x|x\rangle
$$

Sp($u$)$\cap A$ Sp($u$)

(loc. cit.) therefore $\|p_A(x)-x\|^2=\|p_A(x)\|^2- \|x\|^2\leqslant 0$ and consequently $p_A(x) =x$, that is to say $x\in E_A$.

Assertion b) follows from a) and from the remark in IV, p. 273.

Let us prove c). The domain of $u$ is the set of $x\in E$ such that the identity function of Sp($u$) belongs to $\mathscr{L}^2$(Sp($u$)$, \mu_x$) $($loc. cit.). Since $\mu_{p_A(x)}=\varphi_A\cdot \mu_x$ for $x\in E$ (cor. of Prop. 5 of IV, p. 275), one has $p_A(x)\in$ dom($u$) if $x\in$ dom($u$).

Let $x\in$ dom($u$) and $y=p_A(x)$; one has $y\in$ dom($u$)$\cap E_A$ according to c). The spectral measure of $u(y)$ relative to $u$ is $|$Id$_{Sp(u)}|^2\cdot \mu_y($loc. cit.). Since $\mu_y$ has support in A, the same is true of $\mu_{u(y)}$, hence $u(y)\in E_A$ according to a).

#### Corollary {#ts-iv-s5-n4-cor-1 .statement tag=0364}

Let $\lambda \in$ Sp($u$). The image of $p_{\{\lambda\}}$ is the proper subspace of $u$ relative to $\lambda$.

Let $x\in$ dom($u$). Let $\mu$ (resp. $\nu$ ) denote the spectral measure of the element $x$ relative to $u$ (resp. the spectral measure of $(x, u(x))$ relative to $u$). One has $\nu =$ Id$_{Sp(u)}\cdot \mu$ (Corollary to Proposition 5 of IV, p. 275). If $u(x) =\lambda x$, one also has $\nu =\lambda \mu$, whence the equality Id$_{Sp(u)}\cdot \mu=\lambda \mu$. This implies that the support of $\mu$ is contained in $\{\lambda \}($cf. INT, V, p. 46, § 5, n$^o3$, Corollary 2) and therefore $x$ belongs to the image of $p_{\{\lambda\}}$ (Proposition 9, a)).

Conversely, suppose that $x$ belongs to the image $E_{\lambda}$ of $p_{\{\lambda\}}$. Then $x$ belongs to dom($u$) and $u(x)$ also belongs to $E_{\lambda}($loc. cit., b)). Since $\varphi_{\{\lambda\}}\cdot$ (Id$_{Sp(u)}-\lambda$ ) $= 0$, one has the relation $p_{\{\lambda\}}\circ (u-\lambda 1_E)\subset 0$ (Proposition 5 of IV, p. 275, c)), whence $0 =p_{\{\lambda\}}(u(x))-\lambda p_{\{\lambda\}}(x) =u(x)-\lambda x$.

#### Proposition 10 {#ts-iv-s5-prop-10 .statement tag=0365}

Let $\lambda \in \mathbf{C}$. One has $\lambda \in$ Sp($u$) if and only if, for every open neighbourhood V of $\lambda$ in $\mathbf{C}$, the spectral projector $p_V$ of $u$ relative to V is nonzero.

If $\lambda  \notin$ Sp($u$), then there exists an open neighbourhood V of $\lambda$ in $\mathbf{C}$ which does not meet Sp($u$), and then $p_V=p_{\emptyset}= 0$.

Conversely, suppose that there exists an open neighbourhood V of $\lambda$ in $\mathbf{C}$ such that $p_V= 0$. Let $c >0$ be such that the disc with center $\lambda$ and radius $c$ is contained in V.

Let $x\in$ dom($u$) and let $\mu_x$ be the spectral measure of $x$ relative to $u$. Since $\mu_x(V) =\langle x|p_V(x)\rangle = 0$, one computes

$$
\int_{\mathbf{C}}|z-\lambda |^2d\mu_x(z) =\int_{\mathbf{C}-V}|z-\lambda |^2d\mu_x(z)
$$

$$
\geqslant c^2\int_{\mathbf{C}-V}d\mu_x(z) =c^2\int_{\mathbf{C}}d\mu_x(z) =c^2\|x\|^2
$$

But, on the other hand, one has

$$
\|u(x)-\lambda x\|^2=\int_{\mathbf{C}}|z-\lambda |^2d\mu_x(z) =\|u^*(x)-\lambda x\|^2
$$

(formula (8), p. 272), whence $\|u(x)-\lambda x\|\geqslant c\|x\|$ and $\|u^*(x)-\lambda x\|\geqslant c\|x\|$. It follows that $\lambda$ belongs to the resolvent set of $u$ (Lemma 5 of IV, p. 248). This concludes the proof.

#### Corollary {#ts-iv-s5-n4-cor-2 .statement tag=0366}

Let A be an open set in $\mathbf{C}$ and $n\in \mathbf{N}$. If A contains $n$ elements of Sp($u$), then the dimension of the image of the spectral projector $p_A$ of $u$ relative to A is at least equal to $n$.

Let $\lambda_1, . . .,\lambda_n$ be distinct elements of the spectrum of $u$ belonging to A. There exists a family $(V_i)_{1\leqslant i\leqslant n}$ of pairwise disjoint open sets of $\mathbf{C}$ such that $\lambda_i\in V_i$ for $1\leqslant i\leqslant n$. Let B be the union of the sets $V_i$. The image of $p_A$ contains the image of the spectral projector $p_B$; moreover $p_B$ is the sum of the projectors $p_{V_i}$, and since the image of $p_{V_i}$ is orthogonal to the image of $p_{V_j}$ for all $i\not =j$, the result follows from Prop. 10.

### 5. The Helffer–Sjöstrand formula

In this No., E denotes a complex Hilbert space. We shall obtain a formula for certain cases of the functional calculus of a self-adjoint partial operator which is expressed directly in terms of the resolvent of the operator in question.

We endow $\mathbf{R}$ (resp. $\mathbf{C}$) with Lebesgue measure, denoted by $\mu$, and we identify the group $\mathbf{R}$ and its dual group by the mapping $(x, y)\mapsto$ exp(2$i\pi xy$) $($cf. Corollary 3 of II, p. 236).

For every function $f$ defined and differentiable on an open set U of $\mathbf{R}^2$, identified with $\mathbf{C}$, with real coordinates $x$ and $y$, we put

$$
\frac{\partial f}{\partial z}=\frac{1}{2}(\frac{\partial f}{\partial x}+i\frac{\partial f}{\partial y})
$$

(cf. VAR, R2, 8.8.10, p. 24).

#### Lemma 5 {#ts-iv-s5-lem-5 .statement tag=0367}

Let $f\in \mathscr{D}(\mathbf{R})$. There exists a function $\widetilde{f}$ in $\mathscr{D}(\mathbf{C})$ which coincides with $f$ on $\mathbf{R}$ and satisfies

$$
\frac{\partial\widetilde{f}}{\partial z}(x,0) = 0 \tag{11}
$$

for every $x\in \mathbf{R}$. One then has

$$
\frac{\partial\widetilde{f}}{\partial y}(x,0) =if'(x) \tag{12}
$$

for every $x\in \mathbf{R}$, and there exists a real number $C\geqslant 0$ such that

$$
|\frac{\partial\widetilde{f}}{\partial z}(x, y)|\leqslant C|y| \tag{13}
$$

for every $(x, y)\in \mathbf{R}^2$.

There exists $\varphi \in \mathscr{D}(\mathbf{R})$ whose support is contained in $[-2,2]$ and which is equal to 1 on $[-1,1]$ (Lemma 1 of IV, p. 196). Put

$$
\widetilde{f}(x, y) =(f(x) +iyf'(x))\varphi (y)
$$

for $(x, y)\in \mathbf{R}^2$. One has $\widetilde{f}\in \mathscr{D}(\mathbf{C})$ and $\widetilde{f}$ coincides with $f$ on $\mathbf{R}$. Moreover, for every $(x, y)\in \mathbf{R}^2$, one gets

$$
\frac{\partial\widetilde{f}}{\partial z}(x, y) =\frac{1}{2}((if(x)-yf'(x))\varphi '(y) +iyf''(x)\varphi (y))
$$

Since the function $\varphi$ is equal to 1 in a neighbourhood of 0, one has $\varphi '(0) = 0$, hence (11).

Let $\widetilde{f}$ be in $\mathscr{D}(\mathbf{C})$ satisfying (11). Formula (12) follows from this, and estimate (13) is obtained with the aid of the mean value theorem (FVR, I, p. 23, th. 2).

One says that $\widetilde{f}$ is an almost analytic extension of $f$.

#### Lemma 6 {#ts-iv-s5-lem-6 .statement tag=0368}

Let $\varepsilon  >0$. The function $\sigma_{\varepsilon}$ defined on $\mathbf{R}$ by

$$
\sigma_{\varepsilon}(x) =\frac{2i\varepsilon x}{x^2 + \varepsilon^2}
$$

belongs to $L^2(\mathbf{R})$. Its Fourier transform is the class in $L^2(\mathbf{R})$ of the function $\eta_{\varepsilon}$ which vanishes at 0 and satisfies

$$
\eta_{\varepsilon}(y) =\frac{2\pi \varepsilon y}{|y|}e^{-2\pi \varepsilon|y|}
$$

for every $y\not = 0$.

One has $\sigma_{\varepsilon}\in L^2(\mathbf{R})$ by prop. 3 of IV, p. 199, and the class of the function $\eta_{\varepsilon}$ belongs to $L^2(\mathbf{R})\cap L^1(\mathbf{R})$. For every $x\in \mathbf{R}$, one has

$$
\overline{\mathscr{F}}(\eta_{\varepsilon})(x) = 2\pi \varepsilon \int_{\mathbf{R}_+}e^{2\pi(ix-\varepsilon)y}dy-2\pi \varepsilon \int_{\mathbf{R}_-}e^{2\pi(ix+\varepsilon)y}dy
$$

$$
=\frac{\varepsilon}{\varepsilon-ix}-\frac{\varepsilon}{\varepsilon + ix}=\frac{2i\varepsilon x}{x^2 + \varepsilon^2}
$$

whence $\overline{\mathscr{F}}(\eta_{\varepsilon}) =\sigma_{\varepsilon}$. The result then follows from the fourier inversion formula in $L^2(\mathbf{R})$ (corollary of theorem 2 of II, p. 220).

#### Lemma 7 {#ts-iv-s5-lem-7 .statement tag=0369}

Let $f\in \mathscr{D}(\mathbf{R})$ and let $\widetilde{f}\in \mathscr{D}(\mathbf{C})$ be an almost analytic extension of $f$. For $\varepsilon  >0$, define $f_{\varepsilon}$ on $\mathbf{R}$ by

$$
f_{\varepsilon}(x) =-\frac{1}{2i\pi}\int_{\mathbf{R}}(\frac{\widetilde{f}(y + i\varepsilon)}{y-x + i\varepsilon}-\frac{\widetilde{f}(y-i\varepsilon)}{y-x-i\varepsilon})dy
$$

Then $f_{\varepsilon}$ is continuous and bounded, and $f_{\varepsilon}$ converges to $f$ in $\mathscr{C}_b(\mathbf{R})$ when $\varepsilon$ tends to 0.

The continuity of $f_{\varepsilon}$ is a consequence of INT, IV, p. 144, § 4, n$^o3$, cor. 1, since $\widetilde{f}$ has compact support. Moreover, if $r$ is such that the support of $\widetilde{f}$ is contained in $[-r, r]\times \mathbf{R}$, one has

$$
|f_{\varepsilon}(x)|\leqslant 2\|\widetilde{f}\|_{\infty}\int_{-r}^r\frac{1}{\surd(x-y)^2 + \varepsilon^2}dy\leqslant \frac{4r}{\varepsilon}\|\widetilde{f}\|_{\infty}
$$

therefore $f_{\varepsilon}$ is bounded.

The Taylor expansion to order 1 (FVR, I, p. 30, prop. 3) and formula (13) prove that there exist $M\geqslant 0$ and a function $\varrho_1$ on $\mathbf{R}^2$ such that

$\widetilde{f}(y+i\gamma ) =f(y) +i\gamma f'(y) +\gamma^2\varrho_1(y;\gamma )$, and $|\varrho_1(y;\gamma )|\leqslant M$,

for every $y\in \mathbf{R}$ and $\gamma \in \mathbf{R}$. Since the mapping $y\mapsto \widetilde{f}(y+i\gamma )$ has support contained in $[-r, r]$ for every $\gamma \in \mathbf{R}$, the mapping $y\mapsto \varrho_1(y;\gamma )$ has support contained in $[-r, r]$, for every $\gamma \in \mathbf{R}$.

Let $g_{\varepsilon}$ be the function defined on $\mathbf{R}^2$ by

$$
g_{\varepsilon}(x, y) =\frac{\widetilde{f}(y + i\varepsilon)}{y-x + i\varepsilon}-\frac{\widetilde{f}(y-i\varepsilon)}{y-x-i\varepsilon}
$$

For every $(x, y)\in \mathbf{R}^2$ and $\varepsilon  >0$, one obtains

$$
g_{\varepsilon}(x, y) =-\frac{2i\varepsilon}{(x-y)^2 + \varepsilon^2}f(y) +\frac{2i\varepsilon(y-x)}{(x-y)^2 + \varepsilon^2}f'(y)
$$

$$
+\varepsilon^2(\frac{\varrho_1(y; \varepsilon)}{y-x + i\varepsilon}-\frac{\varrho_1(y;-\varepsilon)}{y-x-i\varepsilon})
$$

Let $x\in \mathbf{R}$ and $\varepsilon  >0$. We have

$$
|\varepsilon^2\int_{\mathbf{R}}(\frac{\varrho_1(y;\varepsilon)}{y-x + i\varepsilon}-\frac{\varrho_1(y;-\varepsilon)}{y-x-i\varepsilon})dy|\leqslant 2M\varepsilon^2\int_{-r}^r\frac{dy}{\surd(x-y)^2 + \varepsilon^2}
$$

$$
\leqslant 4Mr\varepsilon
$$

Consequently, for every $x\in \mathbf{R}$, there follows

$$
f_{\varepsilon}(x) =-\frac{1}{2i\pi}\int_{\mathbf{R}}g_{\varepsilon}(x, y)dy= (f*\delta_{\varepsilon})(x)-\frac{1}{2i\pi}(f'*\sigma_{\varepsilon})(x) +k_{\varepsilon}(x)
$$

where $\delta_{\varepsilon}$ and $\sigma_{\varepsilon}$ are the functions on $\mathbf{R}$ defined by

$$
\delta_{\varepsilon}(x) =\frac{1}{\pi}\frac{\varepsilon}{x^2 + \varepsilon^2},\sigma_{\varepsilon}(x) =\frac{2i\varepsilon x}{x^2 + \varepsilon^2}
$$

and $\|k_{\varepsilon}\|_{\infty}\leqslant 2Mr\varepsilon$.

The function $\mathscr{F}(f')\in \mathscr{S}(\mathbf{R})$ is integrable (Prop. 18 of IV, p. 219 and Prop. 13 of IV, p. 213). By Lemma 6, there follows

$$
\int_{\mathbf{R}}|\mathscr{F}(f')(y)\mathscr{F}(\sigma_{\varepsilon})(y)|dy= 2\pi \varepsilon \int_{\mathbf{R}}|\mathscr{F}(f')(y)|e^{-2\pi \varepsilon|y|}dy
$$

$$
\leqslant 2\pi \varepsilon \int_{\mathbf{R}}|\mathscr{F}(f')(y)|dy
$$

therefore $\mathscr{F}(f')\mathscr{F}(\sigma_{\varepsilon})$ converges to 0 in $L^1(\mathbf{R})$ when $\varepsilon$ tends to 0. Since $f'$ and $\sigma_{\varepsilon}$ belong to $L^2(\mathbf{R})$, Prop. 14 of II, p. 223 implies that $f'*\sigma_{\varepsilon}=\overline{\mathscr{F}}(\mathscr{F}(f')\mathscr{F}(\sigma_{\varepsilon}))$ converges to 0 in $\mathscr{C}_b(\mathbf{R})$.

For every $\varepsilon  >0$, the positive measure $\delta_{\varepsilon}\cdot dx$ on $\mathbf{R}$ has total mass 1 (cf. FVR, III, p. 7). The set of measures $\delta_{\varepsilon}\cdot dx$ for $\varepsilon  >0$ and the filter induced on this set by the filter of neighbourhoods of 0 in $\mathbf{R}_+^*$ satisfy the hypotheses of Lemma 4 of INT, VIII, p. 137, § 2, n$^o7$. The measures $\delta_{\varepsilon}\cdot dx$ therefore converge in $\mathscr{M}^1(\mathbf{R})$ to the point measure $\varepsilon_0$ when $\varepsilon$ tends to 0. There follows $f*\delta_{\varepsilon}\rightarrow f$ in $\mathscr{C}_b(\mathbf{R})$ (INT, VIII, p. 163, § 4, n$^o4$). The lemma is proved.

Let $\mu$ denote the Lebesgue measure on $\mathbf{C}$.

#### Theorem 2 (Helffer–Sjöstrand) {#ts-iv-s5-thm-2 .statement tag=036A}

Let $u$ be a self-adjoint partial operator on E. Let $f\in \mathscr{D}(\mathbf{R})$ and $\widetilde{f}\in \mathscr{D}(\mathbf{C})$ be an almost-analytic extension of $f$. Let $h$ be the mapping from $\mathbf{C}$ into $\mathscr{L}(E)$ defined by

$$
h(\lambda ) =\frac{\partial\widetilde{f}}{\partial z}(\lambda )R(u, \lambda )
$$

if $\lambda \in \mathbf{C}-\mathbf{R}$ and $h(\lambda ) = 0$ if $\lambda \in \mathbf{R}$. Then $h$ is $\mu$-integrable on $\mathbf{C}$ and

$$
f(u) =-\frac{1}{\pi}\int_{\mathbf{C}}h(\lambda )d\mu(\lambda )
$$

The mapping $h$ is measurable and its support is compact. Since $u$ is self-adjoint, one has $\|R(u, \lambda )\|\leqslant |\mathscr{I}(\lambda )|^{-1}$ for every $\lambda \in \mathbf{C}-\mathbf{R}$ (Prop. 17 of IV, p. 248). The mapping $h$ is therefore bounded by formula (13), and consequently it is integrable over $\mathbf{C}$.

Let $\varepsilon \in \mathbf{R}^*_+$. Denote by $F^+_{\varepsilon}$ (resp. $F^-_{\varepsilon}$) the closed set in $\mathbf{C}$ of the $\lambda \in \mathbf{C}$ such that $\mathscr{I}(\lambda )\geqslant \varepsilon$ (resp. $\mathscr{I}(\lambda )\leqslant -\varepsilon$ ). One has

$\int_{\mathbf{C}}h(\lambda )d\mu(\lambda ) =$ lim$_{\varepsilon\rightarrow 0}(\int_{F^+_{\varepsilon}}h(\lambda )d\mu(\lambda ) +\int_{F^-_{\varepsilon}}h(\lambda )d\mu(\lambda ))$.

Let $r >0$ be such that the support of $h$ is contained in $C = [-r, r]^2$. Let us denote by $R_{\varepsilon}^+$ the box $[-2r,2r]\times [\varepsilon ,2r]$ in $\mathbf{C}$. It is a locally polyhedral subset of $\mathbf{C}$ (VAR, R2, 11.3, p. 48). It satisfies the following conditions:

(i) One has $R^+_{\varepsilon}\subset 2C\cap F^+_{\varepsilon}$;

(ii) The set $R^+_{\varepsilon}$ contains the intersection of $F^+_{\varepsilon}$ and the support of $h$;

(iii) The regular boundary $\partial R^+_{\varepsilon}$ (VAR, R2, 11.3.2, p. 49) contains the segment $S_{\varepsilon}= [-r, r] +i\varepsilon \subset \mathbf{C}$;

(iv) One has $h(\lambda ) = 0$ if $\lambda \in \partial R_{\varepsilon}^+-S_{\varepsilon}$.

Let $d\lambda$ (resp. $d\lambda$ ) denote the differential 1-form on $\mathbf{C}$ which is the differential of the identity mapping of $\mathbf{C}$ (resp. of complex conjugation). Let $g$ denote the function on $\mathbf{C}-\mathbf{R}$ with values in $\mathscr{L}(E)$ such that $g(\lambda ) =\widetilde{f}(\lambda )R(u, \lambda )$ for $\lambda \in \mathbf{C}-\mathbf{R}$. Put $\omega =g d\lambda$; it is a differential 1-form on $\mathbf{C}-\mathbf{R}$, with compact support and with values in $\mathscr{L}(E)$. Since the resolvent of $u$ is holomorphic (Prop. 14 of IV, p. 246), one has

$$
d\omega =(\frac{\partial\widetilde{f}}{\partial z}(\lambda )R(u, \lambda ) +\widetilde{f}(\lambda )\frac{\partial}{\partial z}R(u, \lambda ))d\lambda \wedge d\lambda =-h(\lambda )d\lambda \wedge d\lambda
$$

The vector measure associated with $d\omega$ (VAR, R2, 10.4.3, p. 43) is the measure with density $-2ih$ with respect to Lebesgue measure. Applying Stokes's formula to the locally polyhedral set $R_{\varepsilon}^+$ and to the differential form $\omega$ (VAR, R2, 11.3.4, p. 49), one therefore obtains

$$
\frac{i}{2}\int_{R^+_{\varepsilon}}d\omega =\frac{i}{2}\int_{\partial R^+_{\varepsilon}}\omega =\frac{i}{2}\int_{S_{\varepsilon}}\omega =\frac{i}{2}\int_{-r}^r\widetilde{f}(y+i\varepsilon )R(u, y+i\varepsilon )dy
$$

whence

$$
\int_{F^+_{\varepsilon}}h(\lambda )d\mu(\lambda ) =-\frac{i}{2}\int_{\mathbf{R}}\widetilde{f}(y+i\varepsilon )R(u, y+i\varepsilon )dy
$$

Reasoning analogously for $F^-_{\varepsilon}$, one obtains

$$
\int_{F^-_{\varepsilon}}h(\lambda )d\mu(\lambda ) =-\frac{i}{2}\int_{\mathbf{R}}\widetilde{f}(y-i\varepsilon )R(u, y-i\varepsilon )dy
$$

and one concludes that the integral of $h$ over $\mathbf{C}$ is the limit as $\varepsilon \rightarrow 0$ of

$$
v_{\varepsilon}=\frac{i}{2}\int_{\mathbf{R}}(\widetilde{f}(y+i\varepsilon )R(u, y+i\varepsilon )-\widetilde{f}(y-i\varepsilon )R(u, y-i\varepsilon ))dy
$$

By Prop. 7, one has $v_{\varepsilon}=\pi f_{\varepsilon}(u)$, where $f_{\varepsilon}$ is the function defined on $\mathbf{R}$ by

$$
f_{\varepsilon}(x) =-\frac{1}{2i\pi}\int_{\mathbf{R}}(\frac{\widetilde{f}(y + i\varepsilon)}{y-x + i\varepsilon}-\frac{\widetilde{f}(y-i\varepsilon)}{y-x-i\varepsilon})dy
$$

As $f_{\varepsilon}\rightarrow f$ when $\varepsilon \rightarrow 0$ in $\mathscr{C}_b(\mathbf{R})$ (Lemma 7), the endomorphism $v_{\varepsilon}=\pi f_{\varepsilon}(u)$ converges to $\pi f(u)$ in $\mathscr{L}(E)$ (Prop. 5 of IV, p. 275). The theorem is proved.

### 6. Resolvent Topologies and Continuity of the Functional Calculus

In this No., E denotes a complex Hilbert space. Recall that $\mathscr{A}(E)$ denotes the set of self-adjoint partial operators on E. We are going to extend to $\mathscr{A}(E)$ the continuity properties of No. 8 of IV, p. 194.

#### Definition 6 {#ts-iv-s5-def-6 .statement tag=036B}

Let $\mathscr{T}$ be a locally convex topology on $\mathscr{L}(E)$. The $\mathscr{T}$ -resolvent topology on $\mathscr{A}(E)$ is the least fine topology such that the mappings $u\mapsto R(u, \lambda )$ of $\mathscr{A}(E)$ into $\mathscr{L}(E)$ endowed with the topology $\mathscr{T}$ are continuous for every $\lambda \in \mathbf{C}-\mathbf{R}$.

#### Proposition 11 {#ts-iv-s5-prop-11 .statement tag=036C}

Let $\mathscr{T}$ be a locally convex topology on $\mathscr{L}(E)$ which is less fine than the Banach-space topology of $\mathscr{L}(E)$.

a) Let $f\in \mathscr{C}_0(\mathbf{R})$. For every sequence $(u_n)_{n\in\mathbf{N}}$ in $\mathscr{A}(E)$ which converges to $u$ for the $\mathscr{T}$ -resolvent topology, the sequence $(f(u_n))_{n\in\mathbf{N}}$ converges to $f(u)$ in the space $\mathscr{L}(E)$ endowed with the topology $\mathscr{T}$;

b) Suppose that every $u\in \mathscr{A}(E)$ admits a countable fundamental system of neighbourhoods for the $\mathscr{T}$ -resolvent topology. The mapping of $\mathscr{C}_0(\mathbf{R})\times \mathscr{A}(E)$ into the space $\mathscr{L}(E)$ endowed with the topology $\mathscr{T}$ defined by $(f, u)\mapsto f(u)$ is continuous.

Let us prove a). The topology $\mathscr{T}$ on $\mathscr{L}(E)$ is the supremum of the topologies defined by the seminorms continuous for the topology $\mathscr{T}$ (EVT, II, p. 26, Cor. and following remark). It is therefore enough to prove that for every seminorm $p$ on $\mathscr{L}(E)$ which is continuous for the topology $\mathscr{T}$, the sequence $p(f(u_n)-f(u))$ converges to 0 (TG, I, p. 51, Prop. 10).

Let $p$ be such a seminorm. Let $\mathscr{L}(E)_p$ denote the separated completed Banach space of the space $\mathscr{L}(E)$ endowed with the seminorm $p$, and let $\varpi$ denote the canonical mapping of $\mathscr{L}(E)$ into $\mathscr{L}(E)_p$; it is continuous, and one has $p(u) =\|\varpi (u)\|_p$ for every $u\in \mathscr{L}$ (E), where the norm is that of the space $\mathscr{L}(E)_p$.

Since $\mathscr{T}$ is less fine than the Banach-space topology of $\mathscr{L}$ (E), there exists $c\geqslant 0$ such that $p(u)\leqslant c\|u\|$ for every $u\in \mathscr{L}(E)$.

Suppose first that $f\in \mathscr{D}(\mathbf{R})$. Let $\widetilde{f}$ be an almost analytic extension of $f$. Let us denote by $\mu$ the Lebesgue measure on $\mathbf{C}$. By the Helffer–Sjöstrand formula (Theorem 2 of IV, p. 284), we have

$$
\varpi (f(u_n)) =-\frac{1}{\pi}\int_{\mathbf{C}}\frac{\partial\widetilde{f}}{\partial z}(\lambda )\varpi (R(u_n, \lambda ))d\mu(\lambda ) \tag{14}
$$

for every $n\in \mathbf{N}$.

Let $\lambda \in \mathbf{C}-\mathbf{R}$. By assumption, the sequence of resolvents $R(u_n, \lambda )$ converges to $R(u, \lambda )$ in $\mathscr{L}(E)$ endowed with the topology $\mathscr{T}$, hence the sequence $(\varpi (R(u_n, \lambda )))_n$ converges to $\varpi (R(u, \lambda ))$ in the Banach space $\mathscr{L}(E)_p$.

For every $n\in \mathbf{N}$, we have

$$
\|\frac{\partial\widetilde{f}}{\partial z}(\lambda )R(u_n, \lambda )\|\leqslant |\frac{1}{\mathscr{I} (\lambda)}\frac{\partial\widetilde{f}}{\partial z}(\lambda )|
$$

(Proposition 17 of IV, p. 248), hence

$$
\|\frac{\partial\widetilde{f}}{\partial z}(\lambda )\varpi (R(u_n, \lambda ))\|_p\leqslant c|\frac{1}{\mathscr{I} (\lambda)}\frac{\partial\widetilde{f}}{\partial z}(\lambda )|
$$

Estimate (13) of IV, p. 281 shows that the right-hand side of this inequality is a bounded function for $\lambda \in \mathbf{C}-\mathbf{R}$; it is integrable on $\mathbf{C}$ since $\widetilde{f}$ has compact support. It follows from Lebesgue's theorem (INT, IV, p. 137, § 3, n$^o7$, Theorem 6) and from the Helffer–Sjöstrand formula applied to $f$ that $\varpi (f(u_n))$ converges to $\varpi (f(u))$, hence $p(f(u_n)-f(u))$ tends to 0.

Suppose now that $f\in \mathscr{C}_0(\mathbf{R})$. Let $\varepsilon  >0$. There exists a function $f_{\varepsilon}$ in $\mathscr{D}(\mathbf{R})$ such that $\|f_{\varepsilon}-f\|_{\infty}\leqslant \varepsilon ($cf. Proposition 4, a) of IV, p. 202 and INT, III, p. 45, § 1, n$^o2$, Proposition 3). By Proposition 5, c) of IV, p. 275, we then have $\|f(u)-f_{\varepsilon}(u)\|\leqslant \varepsilon$ and $\|f(u_n)-f_{\varepsilon}(u_n)\|\leqslant \varepsilon$ for every $n\in \mathbf{N}$. Consequently, we obtain

$$
p(f(u_n)-f(u))\leqslant 2c\varepsilon +p(f_{\varepsilon}(u_n)-f_{\varepsilon}(u))
$$

for every $n\in \mathbf{N}$. Since $f_{\varepsilon}\in \mathscr{D}(\mathbf{R})$, the sequence $(p(f_{\varepsilon}(u_n)-f_{\varepsilon}(u)))_{n\in\mathbf{N}}$ converges to 0 by the preceding case, and therefore $p(f(u_n)-f(u))$ converges to 0. This completes the proof of a).

Let us prove assertion b). Under the assumption concerning $\mathscr{T}$, it follows from TG, IX, p. 17, Proposition 10 and the following remark, and from assertion a), that the mapping $u\mapsto f(u)$ from $\mathscr{A}(E)$ into $\mathscr{L}(E)$ is continuous when $f\in \mathscr{C}_0(\mathbf{R})$. Since the mappings $f\mapsto f(u)$ from $\mathscr{C}_0(\mathbf{R})$ into $\mathscr{L}(E)$ are continuous of norm $\leqslant 1$ for every $u\in \mathscr{A}(E)$ (Proposition 5, c) of IV, p. 275), assertion b) follows from TG, X, p. 13, Corollary 3.

#### Example 1 {#ts-iv-s5-n6-exa-1 .statement tag=036D}

Let $\mathfrak{S}$ be a set of bounded parts of E. The $\mathfrak{S}$-topology on $\mathscr{L}(E)$ (EVT, III, p. 13) is a locally convex topology less fine than the Banach-space topology of $\mathscr{L}(E)$.

#### Example 2 {#ts-iv-s5-n6-exa-2 .statement tag=036E}

Let $\mathscr{T}_b$ be the Banach-space topology of $\mathscr{L}(E)$. For the $\mathscr{T}_b$-resolvent topology, every $u\in \mathscr{A}(E)$ admits a countable fundamental system of neighbourhoods.

In fact, it is enough to prove that for every $\lambda \in$ **C-R** and every $\varepsilon  >0$, there exist $\lambda '\in \mathbf{Q}+i\mathbf{Q}^*$ and an integer $n\geqslant 1$ such that every partial operator $v\in \mathscr{A}(E)$ satisfying $\|R(v, \lambda ')-R(u, \lambda ')\|<1/n$ also satisfies the condition $\|R(v, \lambda )-R(u, \lambda )\|< \varepsilon$; writing

$$
\|R(v, \lambda )-R(u, \lambda )\|\leqslant \|R(v, \lambda )-R(v, \lambda ')\|
$$

$$
+\|R(v, \lambda ')-R(u, \lambda ')\|+\|R(u, \lambda ')-R(u, \lambda )\|
$$

this property follows from formula (8) of IV, p. 245, from the estimates of proposition 17 of IV, p. 248, and from the fact that $\mathbf{Q}+i\mathbf{Q}^*$ is everywhere dense in $\mathbf{C}-\mathbf{R}$.

The conclusion of the proposition is not valid in general if $\mathscr{C}_0(\mathbf{R})$ is replaced by $\mathscr{C}_b(\mathbf{R})$ (exercise 29 of IV, p. 366, e)). Nevertheless, one has the following result.

#### Corollary {#ts-iv-s5-n6-cor-1 .statement tag=036F}

Let $\mathscr{T}_s$ be the topology of simple convergence on $\mathscr{L}(E)$. Let $f\in \mathscr{C}_b(\mathbf{R})$. For every sequence $(u_n)_{n\in\mathbf{N}}$ in $\mathscr{A}(E)$ which converges to $u$ for the $\mathscr{T}_s$-resolvent topology, the sequence $(f(u_n))_{n\in\mathbf{N}}$ converges to $f(u)$ in $\mathscr{L}(E)$ endowed with the topology $\mathscr{T}_s$.

Let $(u_n)$ be a sequence in $\mathscr{A}(E)$ which converges to $u$ for the $\mathscr{T}_s$-resolvent topology. Let $x\in E$ and let $\varepsilon  >0$.

For every integer $N\in \mathbf{N}$, let $\varphi_N\in \mathscr{K}(\mathbf{R})$ be a function with support contained in $[-(N + 1),N + 1]$ such that $0\leqslant \varphi_N\leqslant 1$ and $\varphi_N(t) = 1$ for every $t\in [-N,N]$. The functions $\varphi_N$ converge simply to 1 as N tends to infinity, and satisfy $|\varphi_N|\leqslant 1$, hence prop. 6 of IV, p. 276 implies that there exists $N\in \mathbf{N}$ such that $\|\varphi_N(u)x-x\|\leqslant \varepsilon$. Put $f_N=f \varphi_N$.

For every $n\in \mathbf{N}$, one has

$$
\|f(u_n)x-f(u)x\|\leqslant \|f(u_n)x-f_N(u_n)x\|+ \tag{15}
$$

$$
\|f_N(u_n)x-f_N(u)x\|+\|f_N(u)x-f(u)x\|
$$

For every $v\in \mathscr{A}$ (E), one has

$$
\|f(v)x-f_N(v)x\|=\|(f(1-\varphi_N))(v)x\|
$$

$$
\leqslant \|f(v)\| \|x-\varphi_N(v)x\|\leqslant \|f\|_{\infty}\|x-\varphi_N(v)x\|
$$

(prop. 5, c) of IV, p. 275). Since $\varphi_N\in \mathscr{C}_0(\mathbf{R})$, assertion a) of prop. 11 applied to the $\mathscr{T}_s$-resolvent topology implies that $\varphi_N(u_n)x$ converges to $\varphi_N(u)x$ when $n\rightarrow +\infty$. Consequently, for every sufficiently large $n$, one has

$$
\|x-\varphi_N(u_n)x\|\leqslant \|x-\varphi_N(u)x\|+\varepsilon \|x\|\leqslant (1 +\|x\|)\varepsilon
$$

Inequality (15) then becomes

$$
\|f(u_n)x-f(u)x\|\leqslant \|f\|_{\infty}(2 +\|x\|)\varepsilon +\|f_N(u_n)x-f_N(u)x\|
$$

for every sufficiently large $n$. The proof is concluded by means of assertion a) of loc. cit., applied to the function $f_N\in \mathscr{C}_0(\mathbf{R})$ and to the $\mathscr{T}_s$-resolvent topology.

### 7. Polar decomposition

#### Lemma 8 {#ts-iv-s5-lem-8 .statement tag=036G}

Let E be a separated topological vector space. Let $(E_1,\|\cdot \|_1)$ and $(E_2,\|\cdot \|_2)$ be dense subspaces of E endowed with Hilbert space structures such that the canonical injections of $E_1$ and $E_2$ into E are continuous. Let F be a subspace of $E_1\cap E_2$, dense in $E_1$ and $E_2$ for these Hilbert space structures. If $\|x\|_1=\|x\|_2$ for every $x\in F$, then $E_1= E_2$ and $\|\cdot \|_1=\|\cdot \|_2$.

Let $x\in E_1$. There exists a sequence $(x_n)_{n\in\mathbf{N}}$ in F such that $x_n$ converges to $x$ in the Hilbert space $E_1$. Since $\|x_n-x_m\|_2=\|x_n-x_m\|_1$ for all integers $n$ and $m$, the sequence $(x_n)$ is a Cauchy sequence in $E_2$. Let $y$ be its limit. We have $\|y\|_2=$ lim$\|x_n\|_2=\|x\|_1$. Since the canonical injections of $E_1$ and $E_2$ into E are continuous, we have $x_n\rightarrow x$ in E and analogously $x_n\rightarrow y$ in E. Thus it follows that $x=y$ and $\|x\|_1=\|x\|_2$; in particular, $E_1\subset E_2$. We conclude by symmetry.

Let E be a complex Hilbert space. Let $u$ be a self-adjoint positive partial operator on E. For every $\alpha \in \mathbf{R}_+$, we set $u^{\alpha}=f(u)$, where $f$ is the continuous mapping $x\mapsto x^{\alpha}$ of $\mathbf{R}_+$ into $\mathbf{R}$. This is a self-adjoint positive partial operator (Cor. 1, a) of IV, p. 273). When $u\in \mathscr{L}$ (E), this notation is compatible with the notation relative to the involutive algebra $\mathscr{L}(E) ($cf. Prop. 16 of I, p. 118). If $\alpha$ is a positive integer, the partial operator $u^{\alpha}$ coincides with the partial operator defined by the composition $u\circ  \cdots  \circ u$ (Cor. 1, b) of IV, p. 273).

Let $\beta \in \mathbf{R}_+$. We have $u^{\alpha \beta}= (u^{\alpha})^{\beta}$ (Cor. 4 of IV, p. 274). In particular, if $\alpha  >0$, then the partial operator $u^{1/\alpha}$ is the unique self-adjoint positive partial operator $v$ on E such that $v^{\alpha}=u$.

Suppose that $0\leqslant \alpha \leqslant \beta$. Then dom($u^{\beta}$)$\subset$ dom($u^{\alpha}$) $:$ in fact, for every real number $x\geqslant 0$, one has $x^{\alpha}\leqslant 1 +x^{\beta}$, and the result then follows from the definition of the domain of $u^{\alpha}($cf. Prop. 3 of IV, p. 271).

Let $u$ be a closed operator with dense domain from E into a complex Hilbert space F. The partial operator $u^*u$ is self-adjoint and positive (Prop. 12 of IV, p. 241). We write $|u|= (u^*u)^{1/2}$.

#### Proposition 12 {#ts-iv-s5-prop-12 .statement tag=036H}

Let $u$ be a closed operator with dense domain from E into a complex Hilbert space F.

a) The domain of the positive self-adjoint partial operator $|u|$ coincides with the domain of $u$;

b) There exists a unique partially isometric linear mapping $j$ of E into F such that $u=j|u|$ and Ker($j$) $=$ Ker($u$);

c) Let $u_1$ be a positive self-adjoint operator on E and $j_1$ a partially isometric linear mapping of E into F such that $u=j_1u_1$ and Ker($j_1$) $=$ Ker($u_1$). Then $u_1=|u|$ and $j_1=j$.

The domain of $u^*u$ is contained in dom($u$) and in dom($|u|$). It is dense in the Hilbert spaces $E_u($loc. cit.) and $E_{|u|}$ (Cor. 1, e) of IV, p. 273) and, for every $x\in$ dom($u^*u$), one has

$$
\|x\|^2_u=\|x\|^2+\langle u(x)|u(x)\rangle =\|x\|^2+\langle x|(u^*u)(x)\rangle \tag{16}
$$

$$
=\|x\|^2+\langle |u|(x)| |u|(x)\rangle =\|x\|^2_{|u|}
$$

Consequently, the Hilbert spaces $E_u$ and $E_{|u|}$ are equal (Lemma 8), hence dom($u$) $=$ dom($|u|$) and $\|u(x)\|$ = $\||u|(x)\|$ for every $x\in$ dom($u$).

Formula (16) implies that Ker($u$) $=$ Ker($|u|$) and that there exists a unique isometric linear mapping $v$ of Im($|u|$) onto Im($u$) satisfying $v(|u|(x)) =u(x)$ for every $x\in$ dom($|u|$). Since $|u|$ is self-adjoint, one has Im($|u|$)$^{\circ}=$ Ker($|u|$) (Prop. 7, c) of IV, p. 236). There therefore exists a unique partial isometry $j$ of E into F which extends $v$ and vanishes on Ker($|u|$) $=$ Ker($u$). Since E = Ker($u$)$\oplus$ Im($|u|$), this mapping is the unique partially isometric mapping such that $u=j|u|$ and Ker($j$) $=$ Ker($u$).

Let us prove c). We have $u_1j_1^*j_1u_1\subset (j_1u_1)^*j_1u_1=u^*u$. The linear mapping $j_1^*j_1$ is the orthogonal projector with kernel Ker($j_1$) $=$ Ker($u_1$) (TVS, V, p. 41, Prop. 5 (ii)) and hence with image Ker($u_1$)$^{\circ}=$ Im($u_1$) (Prop. 7, c) of IV, p. 236). Consequently, $u^2_1\subset u^*u$, whence $u^2_1=u^*u$ since these two operators are self-adjoint. Thus, it follows that $u_1= (u^*u)^{1/2}$, and the assertion of uniqueness in b) finally proves that $j_1=j$.

#### Definition 7 {#ts-iv-s5-def-7 .statement tag=036I}

Let $u$ be a closed operator with dense domain from E into a complex Hilbert space F. The pair $(j,|u|)$ determined by Prop. 12 is called the polar decomposition of $u$.

Suppose that $u\in \mathscr{L}(E; F)$. Its polar decomposition in the sense of this definition coincides with that of Definition 4 of I, p. 140.

### 8. Self-Adjoint Operators Defined by a Positive Partial Hermitian Form

In this No., E denotes a complex Hilbert space.

#### Definition 8 {#ts-iv-s5-def-8 .statement tag=036J}

Let D be a vector subspace of E. A partial Hermitian form on E with domain D is a correspondence $q= (\Gamma ,E\times E,\mathbf{C})$ whose domain of definition is $D\times D$, whose graph Γ is functional, and such that the mapping from $D\times D$ into $\mathbf{C}$ defined by Γ is a Hermitian form. We write dom($q$) $= D$.

We say that $q$ is a positive partial form if the Hermitian form which it defines is positive.

Let $u$ be a self-adjoint partial operator on E. For every elements $x$ and $y$ of E, we denote by $\mu_{x,y}$ (resp. $\mu_x$) the spectral measure of $(x, y)$ (resp. of $x$) relative to $u$.

Let $(j,|u|)$ be the polar decomposition of $u$ (Def. 7 of IV, p. 290). Let us denote by $D'$ the domain of $|u|^{1/2}$. By definition, this is the space of the $x\in E$ such that the function $z\mapsto  |z|$ is integrable on Sp($u$) with respect to the measure $\mu_x$. It contains dom($u$).

Let $(x, y)\in D'\times D'$. The identity function on Sp($u$) is integrable with respect to the measure $\mu_{x,y}$ (Prop. 4, b) of IV, p. 271); we put

$$
q_u(x, y) =\int t d\mu_{x,y}(t)
$$

Sp($u$)

If $y\in$ dom($u$), we have $q_u(x, y) =\langle x|u(y)\rangle$ by formula (6) of IV, p. 271. The mapping $q_u$ is a Hermitian form on $D'$. It defines a partial Hermitian form on E, said to be associated with $u$. If the operator $u$ is positive, then the form $q_u$ is a positive partial Hermitian form.

#### Definition 9 {#ts-iv-s5-def-9 .statement tag=036K}

Let $q$ be a positive partial Hermitian form on E. We denote by $E_q$ the separated prehilbertian space dom($q$) endowed with the scalar product

$$
(x|y)_q=\langle x|y\rangle +q(x, y)
$$

We denote by $\|x\|_q$ the norm of $x\in E_q$. We say that the form $q$ is closed if $E_q$ is a Hilbert space.

#### Proposition 13 {#ts-iv-s5-prop-13 .statement tag=036L}

Let $u$ be a positive self-adjoint partial operator on E. Let $q_u$ be the associated positive partial form.

a) The domain of $q_u$ is the domain of $u^{1/2}$, and for all $x$ and $y$ in dom($u^{1/2}$), one has $q_u(x, y) =\langle u^{1/2}(x)|u^{1/2}(y)\rangle$;

b) The positive partial form $q_u$ is closed. The domain of $u$ is a core for $q_u$.

Since $u$ is positive, one has $|u|=u$. The domain dom($|u|^{1/2}$) of $q_u$ therefore coincides with dom($u^{1/2}$), and one has

$$
q_u(x, y) =\int t d\mu_{x,y}(t) =\int t^{1/2}\cdot t^{1/2}d\mu_{x,y}(t)
$$

Sp($u$) Sp($u$)

$$
=\langle u^{1/2}(x)|u^{1/2}(y)\rangle
$$

for $x$ and $y$ in dom($q_u$) (prop. 4, b) of IV, p. 271). This proves assertion a).

Moreover, the prehilbertian space $E_{q_u}$ then coincides with the prehilbertian space $E_{u^{1/2}}$ associated with $u^{1/2}$ (def. 4 of IV, p. 230). Since $u^{1/2}$ is a closed partial operator, this space is a Hilbert space (prop. 4 of IV, p. 230) and dom($u$) is dense in $E_{u^{1/2}}$ by assertion e) of cor. 1 of IV, p. 273.

Let $q$ be a partial hermitian form on E with domain D dense in E. For $y\in D$, let us denote by $\lambda_y$ the linear form $x\mapsto q(y, x)$ on D. We denote by $\widetilde{D}$ the set of $y\in D$ such that the linear form $\lambda_y$ is continuous on D.

Let $y\in \widetilde{D}$. Since D is dense in E, there exists a unique continuous linear form on E which extends $\lambda_y$. We denote it again by $\lambda_y$. There exists a unique element $u(y)$ in E such that $\lambda_y(x) =\langle u(y)|x\rangle$ for every $x\in E$ (EVT, V, p. 15, th. 3). The mapping $y\mapsto u(y)$ is linear from $\widetilde{D}$ into E; the partial operator $u$ on E with domain $\widetilde{D}$ is called the partial operator representing $q$. One therefore has

$$
q(x, y) =\langle x|u(y)\rangle
$$

for $y\in$ dom($u$) and $x\in D$.

#### Remark {#ts-iv-s5-n8-rem-1 .statement tag=036M}

Let $q$ be a closed positive partial form and $q'$ a continuous positive Hermitian form on E. The positive Hermitian form defined on dom($q$) by $(x, y)\mapsto q(x, y) +q'(x, y)$ is a closed positive partial Hermitian form with the same domain as $q$. It is denoted by $q+q'$.

By EVT, V, p. 16, Cor. 2, there exists a unique linear mapping $u'\in \mathscr{L}(E)$ such that $q'(x, y) =\langle x|u'(y)\rangle$ for every $(x, y)\in E\times E$. The endomorphism $u'$ is positive and the partial operator representing the closed positive partial Hermitian form $q+q'$ is $u+u'$.

#### Proposition 14 {#ts-iv-s5-prop-14 .statement tag=036N}

Let $q$ be a closed positive partial form with dense domain on E and $u$ the partial operator representing $q$.

a) The domain of $u$ is dense in the Hilbert space $E_q$;

b) The partial operator $u$ is self-adjoint and positive.

Since $q$ is closed, the prehilbertian space $E_q$ of Definition 9 is a Hilbert space.

Let us prove that the partial operator $u+ 1_E$ with domain dom($u$) is bijective. Since

$$
\langle x|(u+ 1_E)(x)\rangle =q(x, x) +\|x\|^2\geqslant \|x\|^2
$$

for every $x\in$ dom($u$), this partial operator is injective.

Let $y\in E$. The linear form on $E_q$ defined by $x\mapsto  \langle y|x\rangle$ is continuous since $\|x\|\leqslant \|x\|_q$. There therefore exists $y'\in E_q$ such that

$$
\langle y|x\rangle = (y'|x)_q=\langle y'|x\rangle +q(y', x)
$$

for every $x\in E_q$ (EVT, V, p. 15, Theorem 3). By definition, this means that $y'$ belongs to the domain of the partial operator $\widetilde{u}$ representing the partial form $(x, y)\mapsto (x|y)_q$ with domain dom($q$), and that $\widetilde{u}(y') =y$. Since $\widetilde{u}=u+ 1_E$ by the above remark, it follows that the partial operator $u+ 1_E$ is also surjective, hence bijective.

Let us prove that the domain of $u$ is dense in $E_q$. Let $y\in E_q$ be orthogonal to dom($u$) in $E_q$. There exists $y'\in$ dom($u$) such that $u(y')+y'=y$. We then have

$$
0 = (y|y')_q=\langle y|y'\rangle +q(y, y') =\langle y|y'+u(y')\rangle =\|y\|^2
$$

therefore $y= 0$. Assertion a) is therefore proved.

Since dom($q$) is dense in E and $\|x\|\leqslant \|x\|_q$ for every $x\in$ dom($q$), assertion a) implies that dom($u$) is dense in E. Since the form $q$ is Hermitian (resp. positive), for all $x$ and $y$ in dom($u$), we have

$$
\langle y|u(x)\rangle =q(y, x) =q(x, y) =\overline{\langle x|u(y)\rangle}=\langle u(y)|x\rangle
$$

(resp. $\langle x|u(x)\rangle =q(x, x)\geqslant 0$), so that $u$ is symmetric (resp. positive). Finally, the partial operator $u+ 1_E$ is self-adjoint by the corollary to proposition 10 of IV, p. 240, and the same is true of $u$.

#### Theorem 3 {#ts-iv-s5-thm-3 .statement tag=036O}

The mapping which associates with a positive self-adjoint operator $u$ on E the positive partial form $q_u$ is a bijection between the set of positive self-adjoint partial operators on E and the set of closed positive partial forms with dense domain on E. The inverse bijection associates with a positive partial form $q$ the partial operator representing $q$.

By prop. 13, b) and 14, b), the mappings described in the statement are well-defined. Let us prove that they are inverse bijections of one another.

Let $u$ be a positive self-adjoint partial operator on E and $q$ the positive partial form associated with $u$. Let $v$ denote the positive self-adjoint operator representing $q$. Let $y\in$ dom($u$)$\subset$ dom($u^{1/2}$) $=$ dom($q$). For every $x\in$ dom($q$) $=$ dom($u^{1/2}$), we have

$$
q(y, x) =\langle u^{1/2}(y)|u^{1/2}(x)\rangle =\langle u(y)|x\rangle
$$

hence $y$ belongs to the domain of $v$ and satisfies $v(y) =u(y)$. The partial operator $v$ is therefore an extension of $u$; since $u$ and $v$ are self-adjoint, they are equal.

Conversely, let $q$ be a closed positive partial form with dense domain and $u$ the positive self-adjoint partial operator representing $q$. We have dom($u$)$\subset$ dom($u^{1/2}$). For $x$ and $y$ in dom($u$), we have

$$
q_u(x, y) =\langle u^{1/2}(x)|u^{1/2}(y)\rangle =\langle x|u(y)\rangle =q(x, y)
$$

by prop. 13, a). Thus, the Hilbert spaces $E_q$ and $E_{q_u}$ both contain dom($u$) as a dense subspace (prop. 14, a) and prop. 13, b), respectively) and $\|x\|_q=\|x\|_{q_u}$ for every $x\in$ dom($u$). It follows that $E_q= E_{q_u}$ and that $q=q_u$ (lemma 8).

#### Corollary {#ts-iv-s5-n8-cor-1 .statement tag=036P}

Let $q$ be a closed positive partial form on E and $u$ the positive self-adjoint operator representing $q$. The domain of $q$ is equal to the domain of $(1_E+u)^{1/2}$, and we have

$$
\|x\|_q=\|(1_E+u)^{1/2}x\|
$$

for every $x\in$ dom($q$).

The domain of $q$ is equal to the domain of $u^{1/2}$ (Prop. 13, a)), which coincides with that of $(1_E+u)^{1/2}($cf. Prop. 3 of IV, p. 271). For every $x\in$ dom($u$)$\subset$ dom($u^{1/2}$), one has

$$
\|(1_E+u)^{1/2}x\|^2=\langle x|(1_E+u)(x)\rangle =\|x\|^2+\langle x|u(x)\rangle =\|x\|^2_q
$$

Since the domain of $u$ is dense in the Hilbert space $E_q$ (Prop. 14, a)), this formula extends by continuity to every $x\in$ dom($u^{1/2}$).

#### Example {#ts-iv-s5-n8-exa-1 .statement tag=036Q}

Let $u$ be a positive partial operator on E which is not necessarily closed. One defines a positive partial form $q$ with domain dom($u$) by

$$
q(x, y) =\langle x|u(y)\rangle
$$

for $x$ and $y$ in dom($u$). Let $E_q$ be the separated pre-Hilbert space of Definition 9 of IV, p. 292. Let $\widetilde{E}_q$ be the Hilbert space completion of $E_q$, whose scalar product is again denoted by $(x, y)\mapsto (x|y)_q$. Since the canonical injection $\iota$ of $E_q$ into E is continuous, it admits a unique continuous extension, denoted by $\widetilde{\iota}$, from $\widetilde{E}_q$ into E. The Hermitian form $q$ is continuous on $E_q$, and therefore is also extended to a unique continuous positive Hermitian form $\widetilde{q}$ on $\widetilde{E}_q$.

Let us prove that the linear mapping $\widetilde{\iota}$ is injective. Let $x\in$ Ker($\widetilde{\iota}$). Consider a sequence $(x_n)_{n\in\mathbf{N}}$ in $E_q$ which converges to $x$ in $\widetilde{E}_q$. Then one has

lim$_{n\rightarrow+\infty}\iota (x_n) =\widetilde{\iota}(x) = 0$,

hence the sequence $(x_n)_{n\in\mathbf{N}}$ converges to 0 in E. Let $y\in E_q$. Since $\widetilde{q}$ is continuous on $\widetilde{E}_q$, it follows that

$(x|y)_q=$ lim$_{n\rightarrow+\infty}(x_n|y)_q=$ lim$_{n\rightarrow+\infty}(\langle x_n|y\rangle +q(x_n, y))$

= lim$_{n\rightarrow+\infty}(\langle x_n|y\rangle +\langle x_n|u(y)\rangle )= 0$.

Since the space $E_q$ is dense in $\widetilde{E}_q$, it follows that $x= 0$, as desired.

Identifying $\widetilde{E}_q$ with its image under $\widetilde{\iota}$ in E, one interprets $\widetilde{q}$ as a closed positive partial form with dense domain extending $q$. The positive self-adjoint operator associated with $\widetilde{q}$ is a self-adjoint extension of $u$. It is called the Friedrichs extension of $u$.

#### Remark {#ts-iv-s5-n8-rem-2 .statement tag=036R}

Let $c\in \mathbf{R}_+$. Let $q$ be a closed partial hermitian form with dense domain such that $q(x, x)\geqslant -c\|x\|^2$ for every $x$ belonging to the domain of $q$. This means that the closed partial hermitian form with domain dom($q$) defined by $\widetilde{q}(x, y) =q(x, y) +c\langle x|y\rangle$ is a positive partial form. By Theorem 3, such forms therefore correspond to the self-adjoint partial operators $u$ on E such that $u+c1_E$ is positive, that is to say such that $u$ is bounded below (Def. 7 of IV, p. 237) by $-c$.

Conversely, let $u$ be a symmetric partial operator on E such that

$$
\langle x|u(x)\rangle \geqslant -c\|x\|^2 \tag{17}
$$

for every $x\in$ dom($u$). Then $v=u+c1_E$ is a positive partial operator on E. The Friedrichs extension of $u$ is defined to be the self-adjoint operator $\widetilde{v}-c1_E$, where $\widetilde{v}$ is the Friedrichs extension of $v$; it is a self-adjoint extension of $u$, which does not depend on the choice of the real number $c$ satisfying (17).

### 9. Variational Principles for the Spectrum of Positive Operators

In this No., E is a nonzero complex Hilbert space.

#### Proposition 15 {#ts-iv-s5-prop-15 .statement tag=036S}

Let $u$ be a self-adjoint partial operator on E. Suppose that $u$ is bounded below by $c\in \mathbf{R}$ (Def. 7 of IV, p. 237). Then

inf(Sp($u$)) $=$ inf$_{x\in dom(u)-\{0\}}\frac{\langle x|u(x)\rangle}{\|x\|^2}\in [c,+\infty [$.

Let $m$ be the right-hand side of the equality to be proved. Let $x\in E$ and let $\mu_x$ be the spectral measure of $x$ relative to $u$. We have

$$
\langle x|u(x)\rangle =\int t d\mu_x(t)
$$

Sp($u$)

$\geqslant$ inf(Sp($u$))$\int_{Sp(u)}d\mu_x(t) =$ inf(Sp($u$))$\|x\|^2$,

(formula (6), p. 271), hence inf(Sp($u$))$\leqslant m$. Conversely, the partial operator $u-m$ is positive, hence inf(Sp($u$))$-m=$ inf(Sp($u-m\cdot 1_E$))$\geqslant 0$ (Prop. 17 of IV, p. 248).

Prop. 9 of I, p. 139 corresponds to the particular case of this proposition when $u$ is a hermitian element of $\mathscr{L}$ (E), in which case it is necessarily bounded below. In this case, one also has

sup(Sp($u$)) $=$ sup$_{x\in dom(u)-\{0\}}\frac{\langle x|u(x)\rangle}{\|x\|^2}$

(loc. cit.); if $u$ does not belong to $\mathscr{L}$ (E), then this least upper bound is $+\infty$.

#### Definition 10 {#ts-iv-s5-def-10 .statement tag=036T}

Let $u$ be a normal partial operator on E. A complex number $\lambda \in$ Sp($u$) belongs to the discrete spectrum of $u$ if $\lambda$ is isolated in Sp($u$) and if $\lambda$ is an eigenvalue of finite multiplicity.

We denote by Sp$_s(u)$ the discrete spectrum of $u$. Its complement in Sp($u$) is called the essential spectrum of $u$ and denoted by Sp$_e(u)$.

The essential spectrum of a normal partial operator $u$ on E is closed in $\mathbf{C}$, since Sp($u$) is closed in $\mathbf{C}$ and the complement of the essential spectrum is open in Sp($u$). The discrete spectrum of $u$ is not necessarily closed in $\mathbf{C}$ (exercise 36 of IV, p. 369).

#### Lemma 9 {#ts-iv-s5-lem-9 .statement tag=036U}

Let E be a complex Hilbert space and $u$ a normal partial operator on E. Let $\lambda \in$ Sp($u$). Then $\lambda \in$ Sp$_s(u)$ if and only if there exists an open neighbourhood V of $\lambda$ in $\mathbf{C}$ such that the spectral projector $p_V$ of $u$ defined by V is of finite rank.

Let $\lambda \in$ Sp$_s(u)$. There exists an open neighbourhood V of $\lambda$ in $\mathbf{C}$ such that Sp($u$)$\cap V =\{\lambda \}$; then the spectral projector $p_V=p_{\{\lambda\}}$ is of finite rank (Cor. to Prop. 9 of IV, p. 278).

Conversely, suppose that there exists an open neighbourhood V of $\lambda$ such that the spectral projector $p_V$ is of finite rank $n\in \mathbf{N}$. By Cor. to Prop. 10 of IV, p. 279, the intersection $V\cap$ Sp($u$) contains at most $n$ elements, therefore $\lambda$ is isolated in Sp($u$). Hence it is an eigenvalue of $u$ of spectral multiplicity at most $n$ by Cor. to Prop. 9 of IV, p. 278.

In the remainder of this No., we assume that E is infinite-dimensional; the analogues of the results below when E is finite-dimensional are deduced from No.$^o4$ of IV, p. 153.

Let $u$ be a self-adjoint operator bounded below on E. Let $c$ be a lower bound of $u$; the spectrum of $u$ is contained in $[c,+\infty [$ (Prop. 15). Suppose that the essential spectrum of $u$ is not empty. We then denote by $\varrho_e$ the greatest lower bound of the essential spectrum of $u$, so that $\varrho_e\geqslant c$ and $\varrho_e$ is an element of the spectrum of $u$. We put Sp$_h(u) =$ Sp($u$)$\cap [\varrho_e,+\infty [$; this is a closed subset of Sp($u$), hence also of $\mathbf{C}$, such that inf(Sp$_h(u)$) $=\varrho_e$; it is called the upper part of the spectrum of $u$. If the essential spectrum of $u$ is empty, we put Sp$_h(u) =\emptyset$ and $\varrho_e= +\infty$.

The intersection Sp$_b(u) =$ Sp($u$)$\cap [0, \varrho_e[$ is contained in the discrete spectrum of $u$, and its elements are therefore isolated eigenvalues of finite multiplicity; it is said to be the lower part of the spectrum of $u$. Let $E_b$ be the closed subspace of E generated by the eigenspaces corresponding to the eigenvalues $\lambda \in$ Sp$_b(u)$. By the Cor. to Prop. 9 of IV, p. 278 and Prop. 8 of IV, p. 278, the space $E_b$ is the image of the spectral projector $p_{Sp_b(u)}$ defined by Sp$_b(u)$. Since Sp($u$) is the disjoint union of Sp$_b(u)$ and Sp$_h(u)$, the orthogonal complement $E_h$ of $E_b$ is the image of the spectral projector $p_{Sp_h(u)}$ defined by Sp$_h(u)$. If Sp$_b(u)$ is finite, then the space $E_b$ is of finite dimension; the space $E_h$ is then nonzero, since E is assumed to be infinite-dimensional.

#### Lemma 10 {#ts-iv-s5-lem-10 .statement tag=036V}

We have

$$
\langle x|u(x)\rangle \geqslant \varrho_e\|x\|^2 \tag{18}
$$

for every $x\in E_h\cap$ dom($u$).

If $x\in E_h\cap$ dom($u$), then the support of the spectral measure $\mu_x$ of $x$ relative to $u$ is contained in the interval $[\varrho_e,+\infty [$ (Prop. 9, a) of IV, p. 278), hence

$$
\langle x|u(x)\rangle =\int_{\mathbf{R}}td\mu_x(t)\geqslant \varrho_e\|x\|^2
$$

#### Lemma 11 {#ts-iv-s5-lem-11 .statement tag=036W}

Suppose that $E_b$ is finite-dimensional. Then, for every real number $\varepsilon  >$ 0, the image of the spectral projector of $u$ defined by $[\varrho_e, \varrho_e+\varepsilon ]$ is infinite-dimensional.

If $E_b$ is finite-dimensional, then the essential spectrum of $u$ is nonempty, hence $\varrho_e$ is finite and belongs to Sp$_e(u)$. Moreover, the lower spectrum Sp$_b(u)$ is finite, hence there exists $\delta  >0$ such that $[\varrho_e-\delta , \varrho_e+\delta ]\cap$ Sp($u$)$\subset [\varrho_e, \varrho_e+\delta ]$. The assertion then results from Lemma 9.

#### Proposition 16 {#ts-iv-s5-prop-16 .statement tag=036X}

The set Sp$_b(u)\subset [c, \varrho_e[$ is countable, discrete and closed in $[0, \varrho_e[$. It is the set of values of a strictly increasing sequence $(\nu_k)_{0\leqslant k<Card(Sp_b(u))}$ of positive real numbers; if Sp$_b(u)$ is infinite, then the sequence $(\nu_k)$ converges to $\varrho_e$.

Let us set T = Sp$_b(u)\cap [0, \varrho_e[$. It is a closed and discrete subset of $[c, \varrho_e[$ by definition. For every integer $i\geqslant 1$, the set Sp$_b(u)\cap [c, \varrho_e-1/i]$ is compact and discrete, hence finite. Since T is the union of these sets for $i\geqslant 1$, the set T is countable.

This concludes the proof if Sp$_b(u)$ is finite. If Sp$_b(u)$ is infinite, one concludes by applying Lemma 2 of III, p. 90 to the image S of T by the mapping $\lambda \mapsto \varrho_e-\lambda$.

For every integer $k$ such that $0\leqslant k <$ Card(Sp$_b(u)$), let $n_k\geqslant 1$ denote the multiplicity of the eigenvalue $\nu_k$ of $u$. Let us set $\mathbf{N}=\mathbf{N}\cup  \{+\infty \} \subset \mathbf{R}$. Let $M\in \overline{\mathbf{N}}$ be the sum of the multiplicities $n_k$. It is the Hilbert dimension of $E_b$, if one agrees to say that a space of infinite Hilbert dimension is of dimension $+\infty  \in \overline{\mathbf{N}}$.

For every integer $n$ such that $0\leqslant n <M$, one defines $\lambda_n(u) =\nu_k$, where $k\geqslant 0$ is the unique integer such that

$$
n_0+\cdots +n_{k-1}\leqslant n < n_0+\cdots +n_k
$$

If $n\in \mathbf{N}$ satisfies $n\geqslant M$, one sets $\lambda_n(u) =\varrho_e$. This case can occur only if Sp$_b(u)$ is finite, in which case $\varrho_e$ is finite, since it is assumed that E is of infinite dimension.

By construction, the sequence $(\lambda_n(u))_{n\in\mathbf{N}}$ is increasing and, for every element $\lambda$ of Sp$_b(u)$, the number of integers $n$ such that $\lambda_n(u) =\lambda$ is equal to the multiplicity of $\lambda$ as an eigenvalue of $u$. The sequence $(\lambda_n(u))_{n\in\mathbf{N}}$ tends to $+\infty$ if and only if the essential spectrum of $u$ is empty.

For every $n\in \mathbf{N}$, let $\mathscr{F}_n$ (resp. $\mathscr{F}_n^u$) denote the set of vector subspaces $F\subset E$ of dimension $n$ (resp. the set of vector subspaces $F\subset$ dom($u$) of dimension $n$).

Let $n\in \mathbf{N}$ be such that $n <M$ and let $F\in \mathscr{F}_n^u$. One says that F is adapted to $u$ if F admits an orthonormal basis $(f_i)_{0\leqslant i\leqslant n-1}$ such that $u(f_i) =\lambda_i(u)f_i$ for $0\leqslant i\leqslant n-1$.

Let $F\in \mathscr{F}_n^u$ be adapted to $u$. The space F is contained in $E_b$; it is generated by eigenvectors of $u$ for eigenvalues $\lambda \leqslant \lambda_{n-1}(u)$, and it contains the eigenspaces corresponding to the eigenvalues $\lambda  < \lambda_{n-1}(u)$. Moreover, for every universally measurable subset A of Sp($u$), the space F is stable under the spectral projector $p_A$ defined by A (prop. 9, c) of IV, p. 278).

#### Lemma 12 {#ts-iv-s5-lem-12 .statement tag=036Y}

Let $F\in \mathscr{F}_n^u$ be a subspace adapted to $u$. Every eigenvector of $u$ belonging to the space $F^{\circ}\cap E_b$ has an eigenvalue $\geqslant \lambda_n(u)$.

Let $\ell$ be such that $\lambda_{n-1}(u) =\nu_{\ell}$. Let $x\in F^{\circ}\cap E_b$ be an eigenvector of $u$ for an eigenvalue $\lambda$, and let $k <$ Card(Sp$_b(u)$) be such that $\lambda =\nu_k$.

The condition $k < \ell$ is impossible, for $\nu_k< \nu_{\ell}$, and the space F would then contain the eigensubspace for the eigenvalue $\nu_k$, contradicting the fact that $x$ is orthogonal to F. If $k=\ell$, then $x$ is an eigenvector for the eigenvalue $\lambda_{n-1}(u)$; since $x\in F^{\circ}$, the multiplicity $n_k$ is strictly greater than the number of integers $i < n$ such that $\lambda_i(u) =\nu_k$, which implies that $\lambda_n(u) =\lambda_{n-1}(u)$. Finally, if $k > \ell$, one has $\lambda =\nu_k> \nu_{\ell}=\lambda_{n-1}(u)$, hence $\lambda \geqslant \lambda_n(u)$.

For every subspace F of E, let

$\widetilde{r}_F(u) =$ inf$_{x\in dom(u)\cap F^{\circ}}\frac{\langle x|u(x)\rangle}{\|x\|^2}$,

$x\not =0$

$\widetilde{R}_F(u) =$ sup $\frac{\langle x|u(x)\rangle}{2}$.

$$
_{x\in dom(u)\cap F}\|x\|
$$

$x\not =0$

#### Proposition 17 {#ts-iv-s5-prop-17 .statement tag=036Z}

a) For every integer $n\in \mathbf{N}$, one has

$\lambda_n(u) =$ sup$_{F\in\mathscr{F}_n}\widetilde{r}_F(u) =$ inf$_{F\in\mathscr{F}_{n+1}^u}\widetilde{R}_F(u)$;

b) For every integer $n <M$ and for every subspace $F\in \mathscr{F}_n^u$ adapted to $u$, one has $\lambda_n(u) =\widetilde{r}_F(u)$;

c) For every integer $n <M$ and for every subspace $F\in \mathscr{F}_{n+1}^u$ adapted to $u$, one has $\lambda_n(u) =\widetilde{R}_F(u)$.

There exists an orthonormal basis $(e_n)_{0\leqslant n<M}$ of the space $E_b$ such that $e_n\in$ dom($u$) and $u(e_n) =\lambda_n(u)e_n$ for every $n$ such that $0\leqslant n <M$. For every $x\in E_b\cap$ dom($u$), one therefore has

$$
\langle x|u(x)\rangle =\sum_{0\leqslant n<M}\lambda_n(u)|\langle e_n|x\rangle |^2
$$

For every integer $n$ such that $1\leqslant n <M + 1$, let $F_n$ be the subspace of dimension $n$ of $E_b$ generated by $(e_0, . . . , e_{n-1})$. One has $F_n\subset$ dom($u$) and $F_n$ is adapted to $u$.

Let $n\in \mathbf{N}$ and $F\in \mathscr{F}_n$. Let us prove that $\widetilde{r}_F(u)\leqslant \lambda_n(u)$ and, consequently, that

(19) Fsup$_{\in\mathscr{F}_n}\widetilde{r}_F(u)\leqslant \lambda_n(u)$.

If $0\leqslant n <M$, in particular if M is infinite, then the restriction to $F_{n+1}$ of the orthogonal projection of E onto F is not injective, hence there exists $x\not = 0$ in $F_{n+1}$ orthogonal to F. Since

$$
\langle x|u(x)\rangle =\sum_{0\leqslant i\leqslant n}\lambda_i(u)|\langle e_i|x\rangle |^2=\lambda_n(u)|\langle e_n|x\rangle |^2\leqslant \lambda_n(u)\|x\|^2
$$

one has $\widetilde{r}_F(u)\leqslant \lambda_n(u)$.

If $M\in \mathbf{N}$ and $n\geqslant M$, then for every real number $\varepsilon  >0$, there exists $x$ of norm 1 in dom($u$) which is orthogonal to F and whose spectral measure $\mu_x$ has support contained in $[\varrho_e, \varrho_e+\varepsilon ]$ (Lemma 11 and Prop. 9, a) of IV, p. 278), whence

$$
\widetilde{r}_F(u)\leqslant \langle x|u(x)\rangle =\int_{Sp(u)}t d\mu_x(t)\leqslant \varrho_e+\varepsilon =\lambda_n(u) +\varepsilon
$$

by definition. Since $\varepsilon  >0$ is arbitrary, one therefore has $\widetilde{r}_F(u)\leqslant \lambda_n(u)$. Inequality (19) is therefore established.

Let $n\in \mathbf{N}$ and $F\in \mathscr{F}_{n+1}^u$. Let us prove that $\widetilde{R}_F(u)\geqslant \lambda_n(u)$ and, consequently, that

(20) Finf$_{\in\mathscr{F}_{n+1}^u}\widetilde{R}_F(u)\geqslant \lambda_n(u)$.

If $0\leqslant n <M$, observe that the restriction to F of the orthogonal projector onto $F_n$ is not injective, hence that there exists a vector $x\not = 0$ in F orthogonal to $F_n$. Put $x_b=p_{Sp_b(u)}(x)$ and $x_h=p_{Sp_h(u)}(x)$. We therefore have $x=x_b+x_h$. The elements $x_b$ and $x_h$ belong to the domain of $u$ (Prop. 9, c) of IV, p. 278) and are orthogonal to $F_n$. We have the lower bound

$$
\langle x_b|u(x_b)\rangle =\sum_{i\geqslant n}\lambda_i(u)|\langle e_i|x_b\rangle |^2\geqslant \lambda_n(u)\|x_b\|^2
$$

and $\langle x_h|u(x_h)\rangle \geqslant \varrho_e\|x_h\|^2$ (formula (18)), whence

$$
\langle x|u(x)\rangle =\langle x_b|u(x_b)\rangle +\langle x_h|u(x_h)\rangle
$$

$$
\geqslant \lambda_n(u)\|x_b\|^2+\varrho_e\|x_h\|^2\geqslant \lambda_n(u)\|x\|^2
$$

If M is finite and $n\geqslant M$, there exists $x\not = 0$ in F orthogonal to $E_b$, hence $x\in E_h$, and

$$
\langle x|u(x)\rangle \geqslant \varrho_e\|x\|^2=\lambda_n(u)\|x\|^2
$$

by (18). Inequality (20) is therefore proved.

We shall now prove assertions b) and c), which imply that inequalities (19) and (20) are equalities when $n <M$.

Let us prove assertion b). Let $F\in \mathscr{F}_n^u$ be a space adapted to $u$. We have the Hilbert direct sum

$F^{\circ}= E_h\oplus \bigoplus_{\lambda\in Sp_b(u)}$ Ker($u-\lambda \cdot 1_E$)$\oplus (F^{\circ}\cap$ Ker($u-\lambda_{n-1}(u)\cdot 1_E$)).

$\lambda >\lambda_{n-1}(u)$

Let $x\in F^{\circ}-\{0\}$. Write $x=x_h+y+z$, where $x_h\in E_h$ and $y$ (resp. $z$) belongs to the second (resp. third) space of the above decomposition. Using again (18) and the fact that every eigenvalue $\lambda  > \lambda_{n-1}(u)$ of $u$ is $\geqslant \lambda_n(u)$, we obtain

$$
\langle x|u(x)\rangle =\langle x_h|u(x_h)\rangle +\langle y|u(y)\rangle +\langle z|u(z)\rangle
$$

$$
\geqslant \varrho_e\|x_h\|^2+\lambda_n(u)\|y\|^2+\lambda_{n-1}(u)\|z\|^2
$$

If $z\not = 0$, then by Lemma 12, we have $\lambda_n(u) =\lambda_{n-1}(u)$. It follows therefore that $\langle x|u(x)\rangle \geqslant \lambda_n(u)\|x\|^2$, whence $\widetilde{r}_F(u)\geqslant \lambda_n(u)$. Combined with (19), this implies assertion b).

Let us prove assertion c). Let $F\in \mathscr{F}_{n+1}^u$ be a subspace adapted to $u$. Let $(f_i)_{0\leqslant i\leqslant n}$ be an orthonormal basis of F such that $u(f_i) =\lambda_i(u)f_i$ for $0\leqslant i\leqslant n$. For every $x\in F$, we have

$$
\langle x|u(x)\rangle =\sum_{0\leqslant i\leqslant n}\lambda_i(u)|\langle f_i|x\rangle |^2\leqslant \lambda_n(u)\|x\|^2
$$

with equality if $x=f_n$, hence $\widetilde{R}_F(u) =\lambda_n(u)$.

Let us prove finally that (19) and (20) are equalities when $n\geqslant M$. In this case, M is finite, hence $E_b$ is contained in the domain of $u$; moreover, we have $\lambda_n(u) =\varrho_e$ by definition.

There exists $F\in \mathscr{F}_n$ containing $E_b$. Any element $x\not = 0$ of dom($u$) orthogonal to F is therefore orthogonal to $E_b$, and satisfies

$$
\frac{\langle x|u(x)\rangle}{2}\geqslant \varrho_e
$$

$$
\|x\|
$$

(formula (18)), hence $\widetilde{r}_F(u)\geqslant \varrho_e=\lambda_n(u)$, and consequently

sup$_{F\in\mathscr{F}_n}\widetilde{r}_F(u)\geqslant \lambda_n(u)$.

Let $\varepsilon  >0$. Since $E_b$ is finite-dimensional, it follows from lemma 11 that there exists an orthonormal family $(x_i)_{i\in I}$ of elements of E such that the subspace F generated by $E_b$ and $(x_i)_{i\in I}$ is of dimension $n+ 1$ and is contained in dom($u$), and such that $\langle x_i|u(x_i)\rangle \leqslant \varrho_e+\varepsilon$ for all $i\in I$. One then has $\widetilde{R}_F(u)\leqslant \varrho_e+\varepsilon$. Since $\varepsilon  >0$ is arbitrary, one concludes that

inf$_{F\in\mathscr{F}_{n+1}^u}\widetilde{R}_F(u)\leqslant \varrho_e=\lambda_n(u)$.

The proposition is proved.

### 10. Compact Perturbation and Essential Spectrum

In this number, E is an infinite-dimensional complex Hilbert space.

#### Lemma 13 {#ts-iv-s5-lem-13 .statement tag=0370}

Let I be an orthonormal family in E. The family I converges weakly to 0 with respect to the filter of complements of finite subsets of I.

Let $x\in E$. By Bessel's inequality (EVT, V, p. 21, prop. 4) and TG, IV, p. 37, th. 1, the family $(|\langle e_i|x\rangle |^2)_{i\in I}$ is summable, hence $\langle e_i|x\rangle$ tends to 0 with respect to the filter of complements of finite subsets of I (TG, III, p. 38, prop. 1).

#### Proposition 18 {#ts-iv-s5-prop-18 .statement tag=0371}

Let $u$ be a self-adjoint partial operator on E and $\lambda$ a real number. Then $\lambda \in$ Sp$_e(u)$ if and only if there exists an orthonormal sequence $(x_n)_{n\in\mathbf{N}}$ in E such that $u(x_n)-\lambda x_n$ tends to 0 in E.

Suppose first that $\lambda \in$ Sp$_e(u)$. If the spectral projector of $u$ relative to $\{\lambda \}$ is of infinite rank, any orthonormal sequence $(x_n)$ in its image answers the question (cf. cor. to prop. 9 of IV, p. 278). We shall suppose in the sequel that this is not the case.

For each $k\in \mathbf{N}$, let $J_k$ be the set of $t\in [\lambda -1, \lambda + 1]$ such that

$$
\frac{1}{k + 2}<|t-\lambda |\leqslant \frac{1}{k + 1}
$$

The sets $J_k$ are pairwise disjoint. Moreover, for every integer $K\in \mathbf{N}$, the sets $(J_k)_{k\geqslant K}$ form a partition of the set

$$
I_K= [\lambda -1/(K + 1), \lambda + 1/(K + 1)]-\{0\}
$$

Since the spectral projector of $u$ relative to $I_K\cup  \{0\}$ is of infinite rank (lemma 9 of IV, p. 297) and that relative to $\{\lambda \}$ is supposed to be of finite rank, one deduces from prop. 8 of IV, p. 278 that there exists a strictly increasing sequence $(k_n)_{n\in\mathbf{N}}$ in $\mathbf{N}$ such that the spectral projector $p_n$ of $u$ relative to $J_{k_n}$ is nonzero. Let $x_n$ be a vector of norm 1 in the image of $p_n$. The sequence $(x_n)$ is orthonormal, since the image of $p_n$ is orthogonal to that of $p_m$ for all $n\not =m$ in $\mathbf{N}$.

Let $n\in \mathbf{N}$. Let $\mu_n$ denote the spectral measure of $x_n$ relative to $u$; its support is contained in $J_{k_n}$ (prop. 9 of IV, p. 278). It follows that

$$
\|u(x_n)-\lambda x_n\|^2=\int|t-\lambda |^2d\mu_n(t)\leqslant 1_2
$$

$$
_{\mathbf{C}}k_n
$$

therefore the sequence $(x_n)_{n\in\mathbf{N}}$ has the required property.

Conversely, suppose that there exists an orthonormal sequence $(x_n)_{n\in\mathbf{N}}$ in E such that $u(x_n)-\lambda x_n\rightarrow$ 0. Let $\mu_n$ denote the spectral measure of $x_n$ relative to $u$.

Let $\varepsilon  >0$. Let $p_{\varepsilon}$ denote the spectral projector of $u$ relative to the open interval $I_{\varepsilon}= ]\lambda -\varepsilon , \lambda +\varepsilon [$. For every $n\in \mathbf{N}$, we have

$$
1 =\|x_n\|^2=\mu_n(I_{\varepsilon}) +\mu_n(\mathbf{R}-I_{\varepsilon})
$$

$$
\leqslant \mu_n(I_{\varepsilon}) +1_2\int|t-\lambda |^2d\mu_n(t)
$$

$$
\varepsilon_{\mathbf{R}-I_{\varepsilon}}
$$

$$
=\|p_{\varepsilon}(x_n)\|^2+\frac{1}{\varepsilon^2}\|u(x_n)-\lambda x_n\|^2
$$

The assumption on the sequence $(x_n)$ therefore implies that the norm of $p_{\varepsilon}(x_n)$ cannot tend to 0. Since the orthonormal sequence $(x_n)$ converges weakly to 0 in E (Lemma 13), the projector $p_{\varepsilon}$ cannot be compact (Cor. of Prop. 6 of III, p. 6) and is consequently of infinite rank. Since this holds for every $\varepsilon  >0$, Lemma 9 of IV, p. 297 allows us to conclude that $\lambda \in$ Sp$_e(u)$.

The following theorem is the analogue for self-adjoint partial operators of Theorem 3 of III, p. 93.

#### Theorem 4 {#ts-iv-s5-thm-4 .statement tag=0372}

Let $u$ be a self-adjoint partial operator on E. The essential spectrum of $u$ is the intersection of the sets Sp($u+v$), where $v$ runs through the set of compact hermitian endomorphisms of E.

The partial operator $u+v$ is self-adjoint for every hermitian endomorphism $v$ of E, since $(u+v)^*=u^*+v^*($cf. IV, p. 236).

Let us prove that if $v$ is compact, then Sp$_e(u)\subset$ Sp$_e(u+v)$. Let $\lambda \in$ Sp$_e(u)$, and let $(x_n)_{n\in\mathbf{N}}$ be an orthonormal sequence in E such that $u(x_n)-\lambda x_n$ converges to 0 (Prop. 18). The sequence $(x_n)$ converges weakly to 0 in E (Lemma 13), and since the endomorphism $v$ is compact, the sequence $(v(x_n))_{n\in\mathbf{N}}$ converges to 0 in E (Cor. of Prop. 6 of III, p. 6). Consequently the sequence $(u+v)(x_n)-\lambda x_n$ converges to 0 in E, and Prop. 18 implies that $\lambda \in$ Sp$_e(u+v)$.

The essential spectrum of $u$ is therefore contained in the intersection of the sets Sp($u+v$) for hermitian $v\in \mathscr{L}^c(E)$.

Conversely, let $\lambda \in$ Sp$_s(u)$. Let $E_{\lambda}$ be the proper subspace of $u$ relative to $\lambda$, and $p_{\lambda}$ the orthoprojector with image $E_{\lambda}$; it is the spectral projector of $u$ relative to $\{\lambda \}$ (Cor. of Prop. 9 of IV, p. 278). By definition of the sensitive spectrum, the projector $p_{\lambda}$ is of finite rank, hence compact. Put $w=u+p_{\lambda}$; it is a self-adjoint partial operator. To conclude the proof, let us verify that $\lambda$ belongs to the resolvent set of $w$.

We have $E_{\lambda}\subset$ dom($u$), and the spaces $E_{\lambda}$ and dom($u$)$\cap E^{\circ}_{\lambda}$ are invariant under $u$ (Prop. 9 of IV, p. 278).

Let $x\in$ dom($u$). Write $x=p_{\lambda}(x)+y$, where $y\in$ dom($u$)$\cap E^{\circ}_{\lambda}$. From the above, we have

$$
\|w(x)-\lambda x\|^2=\|p_{\lambda}(x)\|^2+\|w(y)-\lambda y\|^2 \tag{21}
$$

Let V be an open neighbourhood of $\lambda$ not meeting the spectrum of $u$, and let $c >0$ be such that the disk with center $\lambda$ and radius $c$ is contained in V. Let $\mu_y$ be the spectral measure of $y$ relative to $u$. Since $y$ is orthogonal to $E_{\lambda}$, the support of $\mu_y$ does not meet V (loc. cit.). We then have

$$
\|w(y)-\lambda y\|^2=\|u(y)-\lambda y\|^2=\int_{\mathbf{C}}|t-\lambda |^2d\mu_y(t)\geqslant c^2\|y\|^2 \tag{22}
$$

It follows from (21) and (22) that $\|w(x)-\lambda x\|^2\geqslant$ inf($c^2,1$)$\|x\|^2$; since $w$ is self-adjoint and $\lambda \in \mathbf{R}$, the conclusion then follows from Lemma 5 of IV, p. 248.

#### Corollary {#ts-iv-s5-n10-cor-1 .statement tag=0373}

Let $u$ be a self-adjoint partial operator on E and $v$ a compact hermitian endomorphism of E. Then Sp$_e(u+v) =$ Sp$_e(u)$.

This follows immediately from the theorem.

### 11. Perturbation

In this No., E is a complex Hilbert space.

If $u$ is a self-adjoint partial operator on E and $v\in \mathscr{L}(E)$ is a hermitian endomorphism, then $u+v$ is self-adjoint (cf. IV, p. 236). This is not so in general when $v$ is a symmetric partial operator (Exercise 9 of IV, p. 347). We shall nevertheless obtain positive results of this type in this No.

#### Definition 11 {#ts-iv-s5-def-11 .statement tag=0374}

Let $u$ be a partial operator on E. A partial operator $v$ on E is said to be bounded relatively to $u$ if dom($u$)$\subset$ dom($v$) and if $v$ defines, by passage to the subspace, a continuous linear mapping of $E_u$ into E.

Let $u$ be a partial operator on E. Let $v$ be a partial operator bounded relatively to $u$. There exists a real number $m$ such that

$$
\|v(x)\|\leqslant m(\|x\|+\|u(x)\|)
$$

for all $x\in$ dom($u$). The greatest lower bound of the real numbers $a\geqslant 0$ such that there exists a real number $b$ such that

$$
\|v(x)\|\leqslant a\|u(x)\|+b\|x\|
$$

is called the relative norm of $v$ with respect to $u$, and is denoted by $\|v\|_u$,

for every $x\in$ dom($u$). The relative norm of $v$ is therefore less than or equal to the norm of the restriction of $v$ to the space $E_u$.

#### Remark {#ts-iv-s5-n11-rem-1 .statement tag=0375}

Let $u$ be a partial operator on E. Every endomorphism $v\in \mathscr{L}(E)$ is bounded relatively to $u$ and its relative norm is zero, since $\|v(x)\|\leqslant \|v\| \|x\|$ for every $x\in$ dom($u$), which makes it possible to take $a= 0$ in the above inequality.

#### Theorem 5 (Kato-Rellich) {#ts-iv-s5-thm-5 .statement tag=0376}

Let $u$ be a self-adjoint partial operator on E and $v$ a symmetric partial operator bounded relatively to $u$. If the relative norm $\|v\|_u$ is $<1$, then the partial operator $u+v$ with domain dom($u$) is self-adjoint.

Since $\|v\|_u<1$, there exist by definition positive real numbers $a$ and $b$ such that $a <1$ and $\|v(x)\|\leqslant a\|u(x)\|+b\|x\|$ for every $x\in$ dom($u$).

Let $t\in \mathbf{R}^*$. Put $w_t=v\circ R(u, it)$. We have dom($w_t$) $= E$ since the image of $R(u, it)$ is contained in the domain of $u$, which is contained in the domain of $v$ by hypothesis. Let $x\in$ dom($u$). Since $u$ is self-adjoint, we have

$$
\|(it-u)x\|^2=\|itx\|^2+\|u(x)\|^2-it\langle x|u(x)\rangle +it\langle u(x)|x\rangle
$$

$$
=|t|^2\|x\|^2+\|u(x)\|^2
$$

whence the inequalities $\|u(x)\|\leqslant \|(it-u)x\|$ and $\|x\|\leqslant |t|^{-1}\|(it-u)x\|$. But then we get

$$
\|v(x)\|\leqslant (a+b|t|^{-1})\|(it-u)x\|
$$

In particular, put $x= R(u, it)y$ for $y\in E$; we obtain

$$
\|w_t(y)\|\leqslant (a+b|t|^{-1})\|y\|
$$

It follows that $w_t\in \mathscr{L}(E)$ and that $\|w_t\|\leqslant a+|t|^{-1}b$.

Since $a <$ 1, there exists $t\in \mathbf{R}^*_+$ such that $a+b|t|^{-1}<1$. Then $\|w_t\|<1$ and $\|w_{-t}\|<1$; the endomorphisms $1_E-w_t$ and $1_E-w_{-t}$ of E are therefore invertible (Prop. 2 of I, p. 22). Since we have the formula $(1_E-w_t)\circ (it-u) =it-(u+v)$, this implies that $u+v-it$ is surjective; analogously, the partial operator $u+v+it$ is surjective. It follows that $u+v$ is self-adjoint (Prop. 11 of IV, p. 240).

### 12. Operators with compact resolvent

In this number, E denotes an infinite-dimensional complex Hilbert space.

#### Proposition 19 {#ts-iv-s5-prop-19 .statement tag=0377}

Let $u$ be a self-adjoint partial operator on E. The following conditions are equivalent :

(i) There exists an orthonormal basis $B = (e_j)_{j\in J}$ of E such that $u$ is diagonal in the basis B and the absolute value of the family of eigenvalues of $u$ tends to infinity along the filter of complements of finite subsets of J;

(ii) For every $\lambda$ belonging to the resolvent set of $u$, the resolvent $R(u, \lambda )$ is compact;

(iii) There exists a complex number $\lambda$ belonging to the resolvent set of $u$ such that the resolvent $R(u, \lambda )$ is compact;

(iv) The spectrum of $u$ coincides with the point spectrum of $u$.

Suppose that (i) is satisfied, and let $(\lambda_j)_{j\in J}$ be the family of eigenvalues of $u$. Let $\mu$ be the counting measure on J. The spectrum of $u$ is the $\mu$-essential image of the family $(\lambda_j)$ (Prop. 22 of IV, p. 252); it is the set of values of this family. For every $\lambda  \notin$ Sp($u$), the resolvent $R(u, \lambda )$ is diagonal in the basis B and the family of its eigenvalues is $((\lambda -\lambda_j)^{-1})_{j\in J}($loc. cit.). Since this family converges to 0, the endomorphism $R(u, \lambda )$ is compact (Prop. 2, (iii) of IV, p. 148). This proves that (i) implies (ii).

Since the resolvent set of $u$ is nonempty (cf. Prop. 17 of IV, p. 248), properties (ii) and (iii) are equivalent by formula (8) of IV, p. 245 and Proposition 3 of III, p. 5.

Since $R(u, \lambda )$ is normal for $\lambda  \notin$ Sp($u$) (Prop. 16 of IV, p. 247), condition (iii) implies (iv) by Prop. 15 of IV, p. 247 and Prop. 5 of III, p. 90.

Let us prove finally that (iv) implies (i). Let $\mathscr{O}$ be the set of orthonormal subsets of E consisting of eigenvectors for $u$. The set $\mathscr{O}$, ordered by inclusion, is of finite character (E, III, p. 34, Def. 2) since O belongs to $\mathscr{O}$ if and only if the sets consisting of at most two elements of O belong to $\mathscr{O}$. By E, III, p. 35, Th. 1, there exists a maximal element O of $\mathscr{O}$. Denote by F the closed subspace of E generated by O. For $e\in O$, there exists a unique $\lambda (e)\in \mathbf{R}$ such that $u(e) =\lambda (e)e$ (Prop. 17 of IV, p. 248).

The set of values of the mapping $\lambda$ of O into $\mathbf{R}$ coincides with the spectrum of $u$. In fact, on the one hand this set is contained in the spectrum of $u$ and on the other hand, if there exists $\lambda_0\in$ Sp($u$) which is not a value of $\lambda$, then $\lambda_0$ is an eigenvalue of $u$ by hypothesis. There exists a vector $e\in$ dom($u$) of norm 1 such that $u(e) =\lambda_0e$ and $e \notin O$; the subset $O\cup  \{e\}$ is orthonormal (since eigenspaces of $u$ relative to distinct eigenvalues are orthogonal by assertion b) of the corollary to Prop. 17 of IV, p. 248); it belongs to $\mathscr{O}$, contradicting the maximality of O.

Suppose that $F\not = E$. Then $F^{\circ}$ is nonzero. The endomorphism $R(u, i)$ of E is normal (prop. 16 of IV, p. 247). It leaves stable the subspace $F^{\circ}$ of E (lemma 4 of I, p. 135). Let $v$ be the endomorphism of $F^{\circ}$ deduced from $R(u, i)$ by passing to subspaces. It is a continuous and normal endomorphism of $F^{\circ}($loc. cit.) whose spectrum is contained in that of $R(u, i)$. Since $F^{\circ}$ is nonzero, the spectrum of $v$ is nonempty (cor. 1 of I, p. 26). Moreover, the spectrum of $v$ is not reduced to 0, since the normal endomorphism $v$ is nonzero (example 1 of I, p. 110). Let $s\in$ Sp($v$)$-\{0\}$. Since $s$ belongs to the spectrum of $R(u, i)$, there exists $e\in O$ such that $s= (i-\lambda (e))^{-1}$, and $s$ is an eigenvalue of $R(u, i)$ (prop. 15, a) of IV, p. 247). Since $s$ is nonzero, it is an isolated point of Sp(R($u, i$)) by assumption, hence also of Sp($v$). Thus, $s$ is an eigenvalue of $v$ (prop. 5, c) of I, p. 134). Let $e\in F^{\circ}$ be an eigenvector of norm 1 of $v$; it is also an eigenvector of $u$ (prop. 15, b) of IV, p. 247), and the set $O\cup  \{e\}$ contradicts the fact that O is maximal in $\mathscr{O}$. Hence F = E.

The family of elements of O is therefore an orthonormal basis of E formed of eigenvectors of $u$. The spectrum of $u$ is closed in $\mathbf{R}$, and the point spectrum is discrete; since these sets coincide, the set of elements $\lambda \in$ Sp($u$) such that $|\lambda |\leqslant R$ is compact, hence finite, for every $R>0$. Thus the family of absolute values of the eigenvalues of $u$ tends to infinity along the filter of complements of finite subsets of O. Therefore (iv) implies (i).

#### Definition 12 {#ts-iv-s5-def-12 .statement tag=0378}

Let $u$ be a self-adjoint partial operator on E. One says that $u$ has compact resolvent if the equivalent conditions of prop. 19 are satisfied.

#### Proposition 20 {#ts-iv-s5-prop-20 .statement tag=0379}

Let $u$ be a self-adjoint partial operator on E. Then $u$ has compact resolvent if and only if the canonical injection $j$ of the Hilbert space $E_u$ into E is compact.

Suppose that $u$ has compact resolvent. There exists $\lambda  \notin$ Sp($u$) such that $R(u, \lambda )$ is compact (prop. 19, (iii)). Let B be the unit ball of the Hilbert space $E_u$. Since $u$ is a continuous linear mapping of $E_u$ into E, the subset $B'= (\lambda 1_E-u)(B)$ of E is bounded. Since $R(u, \lambda )$ is compact, the subset $B = R(u, \lambda )(B')$ is relatively compact in E (remark 1 of III, p. 2). This proves that $j$ is compact.

Conversely, suppose that the linear mapping $j$ is compact. The complex number $i$ belong to the resolvent set of $u$ (Proposition 17 of IV, p. 248). We have $u\circ R(u, i) =-1_E+iR(u, i)$. Let B be the unit ball of E. For every $x\in B$, we have

$$
\|u\circ R(u, i)(x)\|=\|-x+iR(u, i)(x)\|\leqslant 1 +\|R(u, i)\|
$$

and consequently

$$
\|R(u, i)x\|^2_u=\|R(u, i)x\|^2+\|u\circ R(u, i)x\|^2
$$

$$
\leqslant \|R(u, i)\|^2+ (1 +\|R(u, i)\|)^2
$$

The image C of B under $R(u, i)$ is therefore bounded in $E_u$; since $j$ is compact by hypothesis, the set $C =j(C)$ is relatively compact in E (III, loc. cit.). Consequently, the resolvent $R(u, i)$ is compact and $u$ has compact resolvent (Proposition 19, (iii)).

#### Corollary {#ts-iv-s5-n12-cor-1 .statement tag=037A}

Let $q$ be a closed positive partial form on E and $u$ the positive self-adjoint operator representing $q$. The following conditions are equivalent:

(i) The partial operator $u$ has compact resolvent;

(ii) The positive endomorphism $\surd\overline{(1_E + u)^{-1}}= (1_E+u)^{-1/2}$ of E is compact;

(iii) The canonical injection $j$ of the Hilbert space $E_q$ (Definition 9 of IV, p. 292) into E is compact.

Since $u$ is positive, the real number $-1$ belong to the resolvent set of $u$ (Proposition 17 of IV, p. 248), hence the positive endomorphism $v=\surd\overline{(1_E + u)^{-1}}$ is defined, and we have $v= (1_E+u)^{-1/2}$ by the functional calculus.

The endomorphism $v$ is compact if and only if $v^2= (1_E+u)^{-1}$ is compact (Proposition 6 of III, p. 91), that is to say if and only if $u$ has compact resolvent (Proposition 19, (iii)). This proves that conditions (i) and (ii) are equivalent.

Suppose that the endomorphism $v$ is compact. Let B be the unit ball of the Hilbert space $E_q$. Since $(1_E+u)^{1/2}$ is a continuous linear mapping from $E_q$ into E (Corollary of Theorem 3 of IV, p. 294), the subset $B'= (1_E+u)^{1/2}(B)$ of E is bounded, hence the subset $j(B) = B =v(B')$ is relatively compact in E (Remark 1 of III, p. 2). This proves that $j$ is compact. Thus (ii) implies (iii).

The linear mapping $\widetilde{v}:x\mapsto (1_E+u)^{-1/2}(x)$ from E into $E_q$ is well-defined and isometric (Corollary of Theorem 3 of IV, p. 294). Since $v=j\circ \widetilde{v}$, condition (iii) implies (ii) (Proposition 3 of III, p. 5).

#### Example {#ts-iv-s5-n12-exa-1 .statement tag=037B}

Let $n\in \mathbf{N}$. Let U be an open set in $\mathbf{R}^n$. Endow U with Lebesgue measure, denoted by $\mu$. Let Δ be the scalar differential operator $-\sum^n_{i=1}\partial_i^2$ on U. The partial operator $\Delta_-$ with domain $\mathscr{D}(U)$ defined by $\varphi \mapsto \Delta (\varphi )$ is closable (Proposition 13 of IV, p. 242) and symmetric (IV, p. 243). It is positive, since for every $\varphi \in \mathscr{D}$(U), we have

$$
\langle \varphi |\Delta_-(\varphi )\rangle =\int_U\overline{\varphi}\Delta (\varphi )d\mu=-\sum_{i=1}^n\int_U\varphi  \partial_i^2\varphi  d\mu
$$

$$
=\sum_{i=1}^n\int_U\partial_i\varphi  \partial_i\varphi  d\mu=\int_U\sum_{i=1}^n|\partial_i\varphi |^2d\mu\geqslant 0
$$

We denote by $\Delta_D$ the Friedrichs extension of the positive symmetric partial operator $\Delta_-($IV, p. 295, Example); it is a Laplacian on U, called the Dirichlet Laplacian on U.

Let $q$ be the positive partial form associated with $\Delta_D$. The domain of $q$ is the Hilbert space completion of $\mathscr{D}(U)$ for the positive Hermitian form defined by

$$
(\varphi_1, \varphi_2)\mapsto \int_U\overline{\varphi}_1\varphi_2+\sum_{i=1}^n\int_U\overline{\partial_i\varphi_1}\partial_i\varphi_2
$$

for every $(\varphi_1, \varphi_2)\in \mathscr{D}(U)\times \mathscr{D}(U)$. In other words, the domain of $q$ is the Sobolev space $H^1_0(U)$ (No.$^o14$ of IV, p. 221).

*Suppose that U is bounded. The canonical injection of $H^1_0(U)$ into $L^2(U)$ is compact; the Dirichlet Laplacian on U is therefore an operator with compact resolvent (Corollary of Proposition 20). Since the Hilbert space $H^1_0(U)$ is of countable type (Proposition 20 of IV, p. 222), and since the image of $\Delta_D$ is of infinite dimension, there exists an increasing sequence $(\lambda_n)_{n\geqslant 0}$ of real numbers tending to $+\infty$ and an orthonormal basis $(f_n)_{n\in\mathbf{N}}$ of $L^2$(U), whose elements belong to the domain of $\Delta_D$, such that $\Delta_D(f_n) =\lambda_nf_n$ for every $n\in \mathbf{N}$. One can prove ("Weyl's law") that as T tends to $+\infty$, one has

$$
\sum_{n\in\mathbf{N}}1\sim \frac{c_n}{(2\pi)^n}mT^{n/2}
$$

$\lambda_n\leqslant T$

where $c_n=\pi^{n/2}/\Gamma (1 +n/2)$ is the volume of the unit ball in $\mathbf{R}^n$ (INT, V, p. 101, § 8, n$^o7$) and $m >0$ is the Lebesgue measure of U.*

## EXERCISES {#ts-iv-s5-exercises}

Unless otherwise stated, the Hilbert spaces below are supposed complex.

See the [exercises for § 5](exercises/s5/).
