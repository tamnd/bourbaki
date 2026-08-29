---
book: ts
book_title: Théories spectrales
chapter: I
chapter_title: ALGÈBRES NORMÉES
section: 7
section_title: Spectre des endomorphismes des espaces de Banach
lang: en
source: ts-i-ii-fr
book_pages: TS I.127-TS I.142, TS I.187-TS I.191
pdf_pages: 0140-0155, 0200-0204
extraction: native
subsections:
    - "no": 1
      title: Spectre d’un endomorphisme
      page: 127
      pdf_page: 140
    - "no": 2
      title: Projecteurs spectraux
      page: 129
      pdf_page: 142
    - "no": 3
      title: Points isolés du spectre
      page: 131
      pdf_page: 144
    - "no": 4
      title: Spectre de la transposée d’un endomorphisme
      page: 131
      pdf_page: 144
    - "no": 5
      title: Cas des espaces hilbertiens
      page: 132
      pdf_page: 145
    - "no": 6
      title: Image numérique
      page: 135
      pdf_page: 148
    - "no": 7
      title: Éléments positifs
      page: 138
      pdf_page: 151
    - "no": 8
      title: Décomposition polaire
      page: 139
      pdf_page: 152
statements: 24
exercises: 16
content_sha256: c0d3782fe36d1716c0a232855572d590f23110c38326670940e28ab4d7ed8d02
translated_from: content/fr/ts/I/07_s7_spectre_des_endomorphismes_des_espaces.md
source_lang: fr
translation_method: machine
source_content_sha256: 90c5ebfb67550b16acbeedb79edf4eb2c5fa302fcbf9b60219e942491284aef8
translation_model: gpt-5.4, gpt-5-mini
translation_run: translate-en-mt-5ef61683
glossary_version: 34
glossary_terms_sha256: 9d3d72d2c3ca766ffb7d9f552c695d6a26b148a85ab357d3c94b6c919fa472f2
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 7. SPECTRUM OF ENDOMORPHISMS OF BANACH SPACES

Unless otherwise stated, the vector spaces considered in this paragraph are vector spaces over $\mathbf{C}$. We denote by $1_E$ the identity mapping of a vector space E. An endomorphism of a topological vector space E is a continuous linear mapping of E into E.

Let E be a topological vector space and let $u$ be an endomorphism of E. If F is a subspace of E stable under $u$, we shall say that the endomorphism of F deduced from $u$ by passing to subspaces is the endomorphism of F deduced from $u$. We denote it by $u|F$.

### 1. Spectrum of an endomorphism

#### Definition 1 {#ts-i-s7-def-1 .statement tag=02G0}

Let E be a topological vector space and let $u$ be an endomorphism of E. The spectrum of $u$, denoted by Sp($u$), is the spectrum of $u$ relative to the unital algebra $\mathscr{L}(E)$.

Let E be a topological vector space and let $u\in \mathscr{L}(E)$. The spectrum of $u$ is the set of complex numbers $\lambda$ such that $u-\lambda 1_E$ is not an automorphism of E. If E is metrisable complete, it is also the set of complex numbers $\lambda$ such that $u-\lambda 1_E$ is not bijective (EVT, I, p. 19, Corollary 1).

Every eigenvalue of $u$ belongs to the spectrum of $u$, but the converse is false in general.

In the remainder of this paragraph, we shall confine ourselves to studying the notion of spectrum in the case where E is a Banach space.

#### Lemma 1 {#ts-i-s7-lem-1 .statement tag=02G1}

Let E be a Banach space and let $u$ be an endomorphism of E. Let $(E_i)_{i\in I}$ be a finite family of closed subspaces of E, stable under $u$, such that $E =\bigoplus_{i\in I}E_i$. For each $i\in I$, let $u_i$ denote the endomorphism of $E_i$ deduced from $u$. Then Sp($u$) $=\bigcup_{i\in I}$ Sp($u_i$), and for every $f\in \mathscr{O}$(Sp($u$)), the endomorphism $f(u)$ stabilises the spaces $E_i$, and $f(u)$ coincides with $f(u_i)$ on $E_i$.

The endomorphism $u$ is an isomorphism if and only if $u_i$ is an isomorphism for every $i\in I$. Applying this property to $u-\lambda 1_E$, we deduce that Sp($u$) is the union of the sets Sp($u_i$) for $i\in I$.

Let $f\in \mathscr{O}$(Sp($u$)). The endomorphism $f(u)$ of E belongs to the bicommutant of $u$ in $\mathscr{L}(E)$ (Theorem 5 of I, p. 74), and therefore commutes with the projectors $p_i$. It therefore stabilizes the spaces $E_i$. Consider the continuous unital morphism $\varpi$ of the product algebra $\prod_{i\in I}\mathscr{L}(E_i)$ into $\mathscr{L}(E)$ defined by $(v_i)_{i\in I}\mapsto \bigoplus_iv_i$. It maps the family $(u_i)$ to $u$. Proposition 7 of I, p. 75 then implies that Sp($u$)$\subset \bigcup_{i\in I}$ Sp($u_i$) and

$$
f(u) =f(\varpi ((u_i)_{i\in I})) =\varpi ((f(u_i))_{i\in I}) =\bigoplus_{i\in I}f(u_i)
$$

which concludes the proof of the lemma.

#### Proposition 1 {#ts-i-s7-prop-1 .statement tag=02G2}

Let E be a complex Banach space and $u$ an endomorphism of E. Let $\lambda \in \mathbf{C}$ and $f\in \mathscr{O}$(Sp($u$)). We have

Ker($u-\lambda 1_E$)$\subset$ Ker($f(u)-f(\lambda )1_E$).

Let $x\in E$ be nonzero. The set A of the $v\in \mathscr{L}(E)$ such that $x$ is an eigenvector of $v$ is a unital subalgebra of $\mathscr{L}(E)$.

The algebra A is full: if $v\in A$ is invertible in $\mathscr{L}(E)$ and if $x$ is an eigenvector of $v$ for the eigenvalue $\lambda$, then $\lambda \not= 0$ and $v^{-1}(x) =\lambda^{-1}x$, which proves that $v^{-1}\in A$.

The algebra A is closed in $\mathscr{L}(E)$. In fact, if $(v_n)_{n\in\mathbf{N}}$ is a sequence in A such that $v_n$ converges to $v\in \mathscr{L}(E)$, the sequence $(\lambda_n)_{n\in\mathbf{N}}$ such that $v_n(x) =\lambda_nx$ is bounded, and therefore admits a subsequence converging to a complex number $\mu$, so that $v(x) =\mu x$.

Suppose that $x$ is an eigenvector of $u$ and that $u(x) =\lambda x$. The algebra A contains $u$, and therefore contains the closed full unital subalgebra B generated by $u$, which is commutative. The mapping $\chi : B\rightarrow \mathbf{C}$ which associates with $v$ the eigenvalue of $v$ relative to $x$ is a character of B such that $\chi (u) =\lambda$. For every $f\in \mathscr{O}$(Sp($u$)), we have $f(u)\in B$ and $\chi (f(u)) =f(\chi (u)) =f(\lambda )$ by Proposition 7 of I, p. 75, whence the proposition.

### 2. Spectral projectors

Soit E a Banach space. We denote by A the unital Banach algebra $\mathscr{L}(E)$ of the endomorphisms of E. Let $u\in A$.

Let H be a subset of Sp($u$) which is both open and closed in Sp($u$); let K denote its complement in Sp($u$).

The idempotent element associated with $u$ and H (No.$^o12$ of I, p. 81) is a continuous projector of E, called the spectral projector associated with $u$ and H; it is denoted by $e_H(u)$, or simply by $e_H$. Its image is called the spectral subspace of E associated with $u$ and H, and is denoted by $E_H(u)$, or simply by $E_H$. Its kernel is $E_K(u)$, and is also denoted by $\widetilde{E}_H(u)$, or simply by $\widetilde{E}_H$. The space E is the topological direct sum of the closed subspaces $E_H$ and $E_K$. For one to have $E_H= 0$, it is necessary and sufficient that one have $e_H= 0$, that is to say that the characteristic function $f_H$ of H on Sp($u$) be the zero function, that is to say that $H =\emptyset$.

Every endomorphism $v$ of E which commutes with $u$ also commutes with $e_H(u)$ (Theorem 5 of I, p. 74), hence stabilizes $E_H$ and $E_K$. In particular, the endomorphism $u$ leaves the subspaces $E_H$ and $E_K$ stable. The space $E_K$ is the only topological supplement of $E_H$ in E which is stable by $u$.

The unital algebra $A_H=e_HAe_H($loc. cit.) is the subalgebra of A formed by the endomorphisms of E which leave $E_H$ stable and which are zero on $E_K$. For every $v\in A_H$, we denote by $v|E_H$ the endomorphism of $E_H$ deduced from $v$. The mapping $v\mapsto v|E_H$ is an isomorphism of $A_H$ onto $\mathscr{L}(E_H)$. In particular, one has Sp($u|E_H$) $=$ Sp$_{A_H}(u|E_H) = H$ and Sp$_{A_K}(u|E_K) = K$ by the formula (18) of I, p. 82.

#### Proposition 2 {#ts-i-s7-prop-2 .statement tag=02G3}

Let E be a Banach space and $u$ an endomorphism of E. Let $E_1$ and $E_2$ be closed subspaces of E invariant under $u$ such that $E = E_1\oplus E_2$. Suppose that the endomorphisms $u_1$ and $u_2$ of $E_1$ and $E_2$ induced by $u$ have disjoint spectra $H_1=$ Sp($u_1$) and $H_2$ = Sp($u_2$). Then Sp($u$) $= H_1\cup H_2$ and $e_{H_1}(u)$ is the projector with image $E_1$ and kernel $E_2$. In particular, one has $E_{H_1}= E_1$ and $E_{H_2}= E_2$.

One has Sp($u$) $= H_1\cup H_2($I, p. 128, Lemma 1). Since the sets $H_1$ and $H_2$ are compact, they are open and closed in Sp($u$). For every holomorphic function $f$ in a neighbourhood of Sp($u$), the endomorphism $f(u)$ leaves $E_1$ and $E_2$ invariant and coincides in $E_1$ with $f(u_1)$ and in $E_2$ with $f(u_2)$ (loc. cit.). Take in particular for $f$ the germ of holomorphic function $f_{H_1}$ which is equal to 1 in a neighbourhood of $H_1$ and 0 in a neighbourhood of $H_2$ (cf. No. 12 of I, p. 81); then $f_{H_1}(u_1)$ is the identity mapping of $E_1$ since $f_{H_1}$ = 1 in a neighbourhood of $H_1=$ Sp($u_1$), and $f_{H_1}(u_2)$ is zero since $f_{H_1}= 0$ in a neighbourhood of $H_2$. Hence $e_{H_1}(u) =f_{H_1}(u)$ is the projector with image $E_1$ and kernel $E_2$, and therefore one has $E_1= E_{H_1}$ and $E_2= E_{H_2}$.

Let E be a Banach space and $u$ an endomorphism of E. Let $(H_i)_{i\in I}$ be a finite family of open and closed subsets of Sp($u$), pairwise disjoint, and let H be their union. Relations (15) and (16) of I, p. 81 imply the following assertions :

a) The family of projectors $(e_{H_i}(u))_{i\in I}$ is orthogonal (that is to say, $e_{H_i}(u)e_{H_j}(u) = 0$ for all $(i, j)$ in $I^2$ such that $i\not=j$, cf. A, II, p. 18, Def. 7) and its sum is $e_H(u)$;

b) The vector space $E_H$ is the topological direct sum of the family $(E_{H_i})_{i\in I}$;

c) For every $j\in I$, one has $E_{Sp(u)-H_j}= E_{Sp(u)-H}\oplus \bigoplus_{i\not=j}E_{H_i}$;

d) The vector space $E_{Sp(u)-H}$ is the intersection of the family $(E_{Sp(u)-H_i})_{i\in I}$.

When H = Sp($u$), the decomposition as topological direct sum $\bigoplus_{i\in I}E_{H_i}$ of E is called the spectral decomposition of E associated with $u$ and with the finite partition $(H_i)_{i\in I}$ of Sp($u$).

Let $f$ be an element of $\mathscr{O}$(Sp($u$)). The spectrum of the endomorphism $f(u)$ of E is the image under $f$ of the spectrum of $u($I, p. 75, Prop. 8). Let L be a subset open and closed in Sp($f(u)$). The set H of elements $\lambda \in$ Sp($u$) such that $f(\lambda )$ belongs to L is open and closed in Sp($u$), and one has $e_L(f(u)) =e_H(u)$ since $f_L\circ f=f_H$ in $\mathscr{O}$(Sp($u$)) (loc. cit.).

### 3. Isolated points of the spectrum

Let E be a Banach space and let $u$ be an endomorphism of E. Let $\lambda \in \mathbf{C}$ be an isolated point of Sp($u$). One then puts $E_{\lambda}(u) = E_{\{\lambda\}}(u)$ and $e_{\lambda}(u)$ for the spectral projector with image $E_{\lambda}(u)$ associated with $u$ and with $\{\lambda \}$.

One also puts $\widetilde{E}_{\lambda}(u) = E_{Sp(u)-\{\lambda\}}(u)$. The spectrum of the endomorphism of $\widetilde{E}_{\lambda}(u)$ induced by $u$ is Sp($u$)$-\{\lambda \}$; in particular, $u-\lambda 1_E$ induces an automorphism of $\widetilde{E}_{\lambda}(u)$.

The space $E_{\lambda}(u)$ is not zero. The spectrum of the endomorphism of $E_{\lambda}(u)$ induced by $u$ is reduced to $\lambda$, therefore $u-\lambda 1_E$ induces a quasi-nilpotent endomorphism of $E_{\lambda}(u)$. The endomorphism $u-\lambda 1_E$ induces an automorphism of $\widetilde{E}_{\lambda}(u)$, therefore Ker($u-\lambda 1_E$)$^n\subset E_{\lambda}(u)$ for every $n\in \mathbf{N}$. In particular, one has Ker($u-\lambda 1_E$)$\subset E_{\lambda}(u)$.

For $\lambda$ to be a pole of order $p >0$ of the resolvent of $u$, it is necessary and sufficient that $(u-\lambda 1_E)^{p-1}e_{\lambda}(u)\not= 0$ and $(u-\lambda 1_E)^pe_{\lambda}(u) = 0$ (corollary of proposition 17 of I, p. 83). In this case, we have $E_{\lambda}(u) =$ Ker(($u-\lambda 1_E$)$^p$) and $\widetilde{E}_{\lambda}(u) =$ Im(($u-\lambda 1_E$)$^p$), since $(u-\lambda 1_E)^p$ induces an automorphism of $\widetilde{E}_{\lambda}(u)$. We have also

$(u-\lambda 1_E)^{p-1}e_{\lambda}(u) =$ lim$_{z\rightarrow\lambda}(z-\lambda 1_E)^pR(u, z)$

by proposition 17 of I, p. 83.

It should be noted that in general $E_{\lambda}(u)$ is not the union of the family (Ker(($u-\lambda 1_E$)$^n$))$_{n\in\mathbf{N}}$, nor even the closure of this union; in particular, an isolated point of Sp($u$) is not necessarily an eigenvalue of $u($I, p. 187, exerc. 1). Analogously, there may exist eigenvalues of $u$ which are not isolated points of Sp($u$) (I, p. 188, exerc. 2).

### 4. Spectrum of the transpose of an endomorphism

#### Proposition 3 {#ts-i-s7-prop-3 .statement tag=02G4}

Let E be a Banach space and let $E'$ be its dual. Let $u$ be an endomorphism of E.

a) We have Sp($u$) $=$ Sp($^tu$) ;

b) For every $f\in \mathscr{O}$(Sp($u$)), we have $f(^tu) =^tf(u)$ ;

c) We have $e_H(^tu) =^te_H(u)$ for every subset H of Sp($u$) which is open and closed.

For an endomorphism of E to be an automorphism, it is necessary and sufficient that its transpose be an automorphism of $E'$ (EVT, IV, p. 30, cor. 5), whence assertion a).

The mapping $v\mapsto^tv$ is a continuous unital homomorphism of the Banach algebra $\mathscr{L}(E)$ into the opposite Banach algebra of $\mathscr{L}(E')$ (EVT, IV, p. 7, prop. 8). Since the algebra $\mathscr{O}$(Sp($^tu$)) is commutative, the mapping $f\mapsto^tf(u)$ is a continuous unital homomorphism of the algebra $\mathscr{O}$(Sp($^tu$)) into the algebra $\mathscr{L}(E')$. This homomorphism maps the germ of the identity mapping of $\mathbf{C}$ to $^tu$, and therefore coincides with the homomorphism $f\mapsto f(^tu)$ (th. 5 of I, p. 74). This proves b).

Assertion c) results from b), applied to the function $f_H$ equal to 1 in a neighbourhood of H and to 0 in a neighbourhood of its complement in Sp($u$).

#### Remark {#ts-i-s7-n4-rem-1 .statement tag=02G5}

Let H be a subset open and closed in Sp($u$), whose associated spectral decomposition is $E = E_H(u)\oplus \widetilde{E}_H(u)$. It follows from assertion c) that if one identifies $E'$ with $E_H(u)'\oplus \widetilde{E}_H(u)'$, then we have $E'_H(^tu) = E_H(u)'$ and $\widetilde{E}'_H(^tu) =\widetilde{E}_H(u)'$.

### 5. Case of Hilbert spaces

In this No., Hilbert spaces over $K =\mathbf{R}$ or $\mathbf{C}$ are considered. We denote by $\langle x_1|x_2\rangle$ the scalar product of two vectors $x_1$ and $x_2$ in a Hilbert space E.

If E is a complex Hilbert space, the Banach algebra $\mathscr{L}(E)$ endowed with the involution $u\mapsto u^*$ is a star algebra (Example 1 of I, p. 102). In particular, if $u\in \mathscr{L}(E)$, one has $\varrho (u^*) =\varrho (u)$ and Sp($u^*$) $=$ Sp($u$).

Let $u\in \mathscr{L}(E)$ be a normal endomorphism and let $\lambda \in \mathbf{C}$. The proper subspace of $u$ relative to $\lambda$ coincides with the proper subspace of the adjoint $u^*$ relative to $\lambda$ (EVT, V, p. 43, cor. of prop. 8). However, these spaces do not in general coincide if $u$ is not normal (exercise 3 of I, p. 188).

Let $\lambda$ and $\mu$ be complex numbers such that $\lambda \not=\mu$. Let $x$ be a proper vector of $u$ relative to $\lambda$ and let $y$ be a proper vector of $u$ relative to $\mu$. Then $u^*(x) =\lambda x$, hence

$$
\mu\langle x|y\rangle =\langle x|u(y)\rangle =\langle u^*(x)|y\rangle =\langle \lambda x|y\rangle =\lambda \langle x|y\rangle
$$

It follows that $\langle x|y\rangle = 0$; the proper subspaces of $u$ are pairwise orthogonal. Moreover, for every $\lambda \in \mathbf{C}$, the proper subspace of $u$ relative to $\lambda$ coincides with the primary subspace of $u$ relative to $\lambda$, that is to say (LIE, VII, §1, n$^o1$) the union for $k\in \mathbf{N}$ of the kernels of $(u-\lambda 1_E)^k$ (EVT, V, p. 43, cor. of prop. 8).

#### Lemma 2 {#ts-i-s7-lem-2 .statement tag=02G6}

Let E be a complex Hilbert space and let $u$ be a normal endomorphism of E. Let $(E_i)_{i\in I}$ be a finite family of closed subspaces of E, stable under $u$ and pairwise orthogonal, such that $E =\bigoplus_{i\in I}E_i$. For every $i\in I$, let $u_i$ denote the endomorphism of $E_i$ induced by $u$. One has Sp($u$) $=\bigcup_{i\in I}$ Sp($u_i$), and for every $f\in \mathscr{C}$(Sp($u$)), the endomorphism $f(u)$ stabilises the spaces $E_i$, and $f(u)$ coincides with $f(u_i)$ on $E_i$.

The proof follows that of lemma 1 of I, p. 128, using the remark of 6 of I, p. 110 and prop. 8 of I, p. 112.

#### Proposition 4 {#ts-i-s7-prop-4 .statement tag=02G7}

Let E be a complex Hilbert space and let $u$ be a normal endomorphism of E. For every function $f\in \mathscr{C}$ (Sp($u$)) and every $\lambda \in \mathbf{C}$, one has

Ker($u-\lambda 1_E$)$\subset$ Ker($f(u)-f(\lambda )1_E$).

The proof is analogous to that of proposition 1 of I, p. 128; let us take up its arguments again. The algebra A introduced in loc. cit. is here a unital involutive subalgebra of $\mathscr{L}(E)$ (EVT, V, p. 43, cor.). It therefore contains the unital involutive subalgebra B generated by $u$, which is commutative. The mapping $\chi : B\rightarrow \mathbf{C}$ which, to $v$, assigns the eigenvalue of $v$ relative to $x$ is a character of B such that $\chi (u) =\lambda$. For every $f\in \mathscr{C}$ (Sp($u$))), one has $f(u)\in B$ and $\chi (f(u)) =f(\chi (u)) =f(\lambda )$ by prop. 8 of I, p. 112, whence the assertion.

#### Lemma 3 {#ts-i-s7-lem-3 .statement tag=02G8}

Let E be a Hilbert space and $p\in \mathscr{L}(E)$ a projector. The following assertions are equivalent:

(i) The projector $p$ is an orthogonal projector, that is to say Ker($p$) $=$ Im($p$)$^{\circ}$ (EVT, V, p. 13);

(ii) The projector $p$ is hermitian;

(iii) The projector $p$ is normal;

(iv) One has Ker($p$)$\subset$ Ker($p^*$) ;

(v) One has Im($p$)$\subset$ Im($p^*$) ;

(vi) The projector $p$ is positive;

(vii) One has $\|p\|\leqslant 1$.

Let us first recall that Ker($p^*$) $=$ Im($p$)$^{\circ}$ and Ker($p$) $=$ Im($p^*$)$^{\circ}$ (EVT, V, p. 41, prop. 4). Moreover, the image of $p$ (resp. $p^*$) is closed, since it coincides with the kernel of $1-p$ (resp. $1-p^*$). Therefore one has

(1) Im($p$) $=$ Ker($p^*$)$^{\circ}$, Im($p^*$) $=$ Ker($p$)$^{\circ}$.

(i) $=\Rightarrow$ (ii)$:p^*$ is a projector with kernel Im($p$)$^{\circ}=$ Ker($p$) and whose image is Im($p^*$)$^{\circ}=$ Ker($p$) $=$ Im($p$)$^{\circ}$; hence $p^*=p$.

(ii) $=\Rightarrow$ (iii) since every hermitian endomorphism is normal.

(iii) $=\Rightarrow$ (iv) : since $p$ is normal, one has $\|p(x)\|^2=\|p^*(x)\|^2$ for all $x$ in E (EVT, V, p. 43, Prop. 7), whence the required inclusion.

(iv) $=\Rightarrow$ (v) follows from equalities (1) above.

(v) $=\Rightarrow$ (vi) : for all $x\in E$, one has $p(x)\in$ Im($p^*$), and consequently $\langle p(x)|x\rangle =\langle p^*(p(x))|x\rangle =\|p(x)\|^2\geqslant 0$.

(vi) $=\Rightarrow$ (vii) : let $x\in E$ and $y=x-p(x)\in$ Ker($p$). For all $t\in \mathbf{R}$, one has by hypothesis

$$
\langle x+ty|p(x)\rangle =\langle x+ty|p(x+ty)\rangle \geqslant 0
$$

which is possible only if $\langle y|p(x)\rangle = 0$. But then

$$
\|p(x)\|^2=\langle x|p(x)\rangle \leqslant \|x\|\|p(x)\|
$$

and therefore $\|p\|\leqslant 1$.

(vii) $=\Rightarrow$ (i) : let $y\in$ Im($p$) ; denote by $z$ the orthogonal projection of $y$ onto Ker($p$)$^{\circ}$ and put $x=y-z\in$ Ker($p$). One has $p(z) =p(y) =y$, hence $\|y\|\leqslant \|z\|$ by hypothesis. But, since $x$ and $z$ are orthogonal, one has $\|y\|^2=\|x\|^2+\|z\|^2$, whence $\|x\|= 0$, that is to say $y=z$. Thus, Im($p$)$\subset$ Ker($p$)$^{\circ}$. Since moreover $\|p^*\|=\|p\|\leqslant 1$, one has analogously Im($p^*$)$\subset$ Ker($p^*$)$^{\circ}$, which yields the converse inclusion by (1).

#### Proposition 5 {#ts-i-s7-prop-5 .statement tag=02G9}

Let E be a complex Hilbert space and $u$ a normal endomorphism of E.

a) For every open and closed subset H of the spectrum of $u$, the spectral projector $e_H(u)$ is an orthogonal projector whose kernel is the image of the spectral projector $e_{Sp(u)-H}(u)$ ;

b) If $H_1$ and $H_2$ are disjoint open and closed subsets of the spectrum of $u$, then the spectral subspaces $E_{H_1}$ and $E_{H_2}$ are orthogonal ;

c) If $\lambda \in \mathbf{C}$ is an isolated point of the spectrum of $u$, then $\lambda$ is an eigenvalue of $u$ and the image of the spectral projector $e_{\lambda}(u)$ is the eigenspace of $u$ relative to $\lambda$.

Let us prove a). Since the holomorphic functional calculus is compatible with the continuous functional calculus (I, p. 111, cor. 1), we have $e_H(u) =\varphi_H(u)$, where $\varphi_H\in \mathscr{C}$ (Sp($u$)) is the characteristic function of H. This implies $e_H(u)^*=\overline{\varphi}_H(u) =\varphi_H(u) =e_H(u)$, hence $e_H(u)$ is an orthogonal projector (lemma 3, (ii)). Its kernel is the image of the projector $1-e_H(u) =e_{Sp(u)-H}(u)$.

Let us prove b). The characteristic functions $\varphi_{H_1}$ and $\varphi_{H_2}$ of $H_1$ and $H_2$ in Sp($u$) are continuous and their product is zero, which implies $e_{H_1}(u)\circ e_{H_2}(u) =e_{H_2}(u)\circ e_{H_1}(u) = 0$. The inclusions $E_{H_2}(u)\subset E_{H_1}(u)^{\circ}$ and $E_{H_1}(u)\subset E_{H_2}(u)^{\circ}$ follow.

Finally, let us prove assertion c). The characteristic function $\varphi_{\lambda}$ of $\{\lambda \}$ is continuous and non-zero on Sp($u$) ; it satisfies $(z-\lambda )\varphi_{\lambda}(z) = 0$ for every $z\in$ Sp($u$). Hence we have $(u-\lambda 1_E)\varphi_{\lambda}(u) = 0$. The image of $\varphi_{\lambda}(u)$, which is non-zero, is therefore contained in the proper subspace of $u$ relative to $\lambda$. Since we have $e_{\lambda}(u) =\varphi_{\lambda}(u)$ and the image of $e_{\lambda}(u)$ contains the proper subspace of $u$ relative to $\lambda$, the assertion follows.

#### Lemma 4 {#ts-i-s7-lem-4 .statement tag=02GA}

Let E be a Hilbert space and let $u$ be a normal endomorphism of E. Let F be a closed subspace of E containing a total set of proper vectors of $u$. Then $F^{\circ}$ is stable under $u$ and the endomorphism $\widetilde{u}$ of $F^{\circ}$ deduced from $u$ is normal.

Since $u$ is normal, every proper vector of $u$ is also a proper vector of $u^*$ (EVT, V, p. 43, cor.). The assumption therefore implies that F is stable under $u$ and under $u^*$. By EVT, V, p. 41, prop. 4 (ii), we therefore have $u(F^{\circ})\subset F^{\circ}$ and $u^*(F^{\circ})\subset F^{\circ}$. It follows that the adjoint of $\widetilde{u}$ is the endomorphism of $F^{\circ}$ deduced from $u^*$. Since $u$ is normal, the endomorphism $\widetilde{u}$ is normal.

### 6. Numerical image

#### Definition 2 {#ts-i-s7-def-2 .statement tag=02GB}

Let E be a complex Hilbert space and let $u$ be an endomorphism of E. The **numerical image** of $u$ is the set of complex numbers of the form $\langle x|u(x)\rangle$, where $x$ ranges over the unit sphere of E. We denote by $\iota (u)$ the numerical image of $u$.

The numerical image of $u^*$ is the image of $\iota (u)$ under complex conjugation. For any complex numbers $\lambda$ and $\mu$, the numerical image of $\lambda u+\mu1_E$ is equal to $\lambda \iota (u) +\mu$.

#### Proposition 6 {#ts-i-s7-prop-6 .statement tag=02GC}

Let E be a complex Hilbert space and let $u$ be an endomorphism of E.

a) The set of eigenvalues of $u$ is contained in $\iota (u)$;

b) The spectrum of $u$ is contained in the closure of $\iota (u)$ in $\mathbf{C}$.

Let $\lambda$ be an eigenvalue of $u$ and let $x\in E$ be a nonzero vector such that $u(x) =\lambda x$. Replacing $x$ by $x/\|x\|$ if necessary, one may suppose that $\|x\|= 1$. Then $\langle x|u(x)\rangle =\lambda$, hence $\lambda \in \iota (u)$.

Let us prove b). Considering $u-\lambda 1_E$, we are reduced to proving that if 0 belongs to the spectrum of $u$, then 0 is adherent to $\iota (u)$.

Suppose first that there exists a real number $c >$ 0 such that $\|u(x)\|\geqslant c$ for every $x$ of norm 1 in E. Then the endomorphism $u$ is injective and closed (Lemma 8 of I, p. 107). Since it is not invertible by hypothesis, it is not surjective. Consequently, the orthogonal complement of the kernel of $u^*$ is not equal to E (EVT, V, p. 41, Prop. 4), which proves that the kernel of $u^*$ is not reduced to 0. Thus 0 belongs to $\iota (u^*)$, hence to $\iota (u)$.

If the preceding assumption is not valid, then for every integer $n\geqslant 1$, there exists a vector $x_n$ of norm 1 in E such that $\|u(x_n)\|\leqslant 1/n$. We then have $|\langle x_n|u(x_n)\rangle |\leqslant 1/n$, which implies that 0 belongs to the closure of $\iota (u)$.

Proposition 7 (Hausdorff-Toeplitz Theorem)

Let E be a complex Hilbert space and let $u\in \mathscr{L}(E)$. The numerical range $\iota (u)$ is a convex subset of $\mathbf{C}$.

We shall need two lemmas to prove this proposition.

#### Lemma 5 {#ts-i-s7-lem-5 .statement tag=02GD}

Let E be a complex Hilbert space of dimension 2. Let us make the real vector space $\mathscr{L}(E)_h$ of Hermitian endomorphisms of E into a prehilbertian normed space by means of the norm $u\mapsto$ Tr($u^*u$)$^{1/2}$. The set of

$$
\surd
$$

orthogonal projectors of rank 1 of E is the sphere S of radius $1/$ 2 centred at $\frac{1}{2}1_E$ in the affine subspace of dimension 3 of endomorphisms of trace 1 in $\mathscr{L}(E)_h$.

Let F be the real affine subspace of $\mathscr{L}(E)_h$ formed by the elements of trace 1. The orthogonal projectors of rank 1 of E belong to F (Lemma 3, (ii)).

Let $u\in F$. We have $\|u-\frac{1}{2}1_E\|^2=$ Tr($u^2-u+\frac{1}{4}$) $=$ Tr($u^2$)$-\frac{1}{2}$. Consequently, $u\in S$ if and only if Tr($u^2$) $= 1$. Since 2 det($u$) $=$ Tr($u$)$^2-$ Tr($u^2$) $= 1-$ Tr($u^2$), this condition is equivalent to det($u$) $= 0$. By the Hamilton–Cayley theorem (A, III, p. 107, prop. 20), we therefore have $u\in S$ if and only if $u^2-u= 0$, which means that $u$ is a hermitian projector of rank 1 (loc. cit.), whence the result.

#### Lemma 6 {#ts-i-s7-lem-6 .statement tag=02GE}

Let E be a normed real vector space, let F be a real vector space, and let $u: E\rightarrow F$ be a non-injective affine mapping. Let B be a ball in E and S the corresponding sphere. Then $u(S) =$ $u(B)$, and in particular, $u(S)$ is convex.

We reduce to the case where $u$ is linear and where B is the unit ball of E. We have $u(S)\subset u(B)$. Conversely, let $x\in B$ and let $y$ be a nonzero element of Ker($u$). The image of the continuous mapping $t\mapsto  \|x+ty\|$ of $\mathbf{R}$ into $\mathbf{R}_+$ is an unbounded interval containing the real number $\|x\|\leqslant 1$. There therefore exists $t\in \mathbf{R}$ such that $\|x+ty\|= 1$. Then $x+ty\in S$ and $u(x+ty) =u(x)$, hence $u(x)\in u(S)$.

Let us prove prop. 7. Let $x$ and $y$ be elements of the unit sphere of E; let us prove that the segment with endpoints $\langle x|u(x)\rangle$ and $\langle y|u(y)\rangle$ is contained in the numerical image of $u$.

Let F be the subspace of E generated by $x$ and $y$. If dim(F) = 1, we have $\langle x|u(x)\rangle =\langle y|u(y)\rangle$, whence the assertion. Otherwise, dim(F) = 2; let $p$ then be the orthogonal projector of E with image F, and let us denote by $u_F$ the endomorphism of F given by $x\mapsto p(u(x))$. Since $p$ is hermitian (lemma 3 of I, p. 133), we have $\langle z|u_F(z)\rangle =\langle z|u(z)\rangle$ for every $z\in F$, so that $\iota (u_F)\subset \iota (u)$. We may therefore suppose that E = F.

For every element $z$ of E, let $v_z$ be the hermitian endomorphism of E defined by $t\mapsto  \langle z|t\rangle z$; one has $\langle z|u(z)\rangle =$ Tr($u\circ v_z$). When $z$ runs through the unit sphere of E$,v_z$ ranges over the set of orthoprojectors of rank 1 of E, which is a sphere S in the real affine subspace V of $\mathscr{L}(E)$ formed by the hermitian endomorphisms of E of trace 1 (lemma 5). The numerical image of E is therefore the set of Tr($u\circ v$), for $v\in S$. The mapping $v\mapsto$ Tr($u\circ v$) of V into $\mathbf{C}$ is linear. Since dim$_{\mathbf{R}}(V) = 3>$ dim$_{\mathbf{R}}(\mathbf{C})$, it is not injective; it therefore follows from lemma 6 that $\iota (u)$ is convex.

### 7. Positive Elements

Let E be a complex Hilbert space. Let $u$ be an endomorphism of E. Recall (EVT, V, p. 45, def. 6) that $u$ is said to be positive if one has $\langle x|u(x)\rangle \geqslant 0$ for every $x\in E$. The endomorphism $u$ is then hermitian (loc. cit.). Moreover, if F is a complex Hilbert space and if $v\in$ $\mathscr{L}(F; E)$, then the endomorphism $v^*uv$ of F is positive (EVT, V, p. 45, prop. 12).

#### Proposition 8 {#ts-i-s7-prop-8 .statement tag=02GF}

Let E be a complex Hilbert space. Let $u$ be an endomorphism of E. The following conditions are equivalent:

(i) The endomorphism $u$ is positive;

(ii) The numerical image of $u$ is contained in $\mathbf{R}_+$;

(iii) The endomorphism $u$ is a positive element of the involutive algebra $\mathscr{L}(E)$ ;

(iv) There exists a hermitian element $v$ of $\mathscr{L}(E)$ such that $u=v^2$;

(v) There exists a continuous linear mapping $v$ of E into a complex Hilbert space F such that $u=v^*v$.

By EVT, V, p. 45, def. $6,u$ is positive if and only if it is hermitian and if $\langle x|u(x)\rangle \geqslant 0$ for every $x\in E$. The implication (i) $=\Rightarrow$ (ii) therefore follows from the definition of the numerical image.

(ii) $=\Rightarrow$ (iii) : the assumption implies that $u$ is hermitian (EVT, V, p. 45, and remark, p. 2) and its spectrum is contained in $\mathbf{R}_+$ (prop. 6) ; hence $u$ is a positive element of the involutive algebra $\mathscr{L}(E)$.

(iii) $=\Rightarrow$ (iv) : this is a particular case of prop. 16 of I, p. 118.

(iv) $=\Rightarrow$ (v) is immediate.

(v) $=\Rightarrow$ (i) : let F be a complex Hilbert space and let $v\in \mathscr{L}(E; F)$ be such that $u=v^*v$. Let $x\in E$. One has $\langle x|u(x)\rangle =\langle x|(v^*v)(x)\rangle =\|v(x)\|^2$, which proves that $u$ is positive.

Recall (EVT, V, p. 45, remark 1) that, for every hermitian element $u$ of $\mathscr{L}(E)$, one sets

$m(u) =$ inf$_{\|xx\in\|=1E}\langle x|u(x)\rangle =$ inf $\iota (u) =$ inf$_{x\in E-\{0\}}\frac{\langle x|u(x)\rangle}{\|x\|^2}$,

$M(u) =$ sup$_{x\in E}\langle x|u(x)\rangle =$ sup $\iota (u) =$ sup$_{x\in E-\{0\}}\frac{\langle x|u(x)\rangle}{\|x\|^2}$.

$\|x\|=1$

If $E =\{0\}$, one has $M(u) =-\infty ,m(u) = +\infty$ and $\iota (u) =\emptyset$.

Suppose $E$ nonzero; one then has $m(u)\leqslant M(u)$ and the numerical image of $u$ is an interval with endpoints $m(u)$ and $M(u)$. By Prop. 6, Sp($u$) is contained in the interval $[m(u),M(u)]$. More precisely:

#### Proposition 9 {#ts-i-s7-prop-9 .statement tag=02GG}

Let $E$ be a complex Hilbert space and let $u$ be a hermitian element of $\mathscr{L}(E)$.

a) One has $m(u) =$ inf Sp($u$) and $M(u) =$ sup Sp($u$) ;

b) If $E$ is nonzero, one has $\|u\|=$ sup($|m(u)|,|M(u)|$).

Let $\lambda \in \mathbf{R}$. In order that $\lambda$ be a lower bound of the spectrum of $u$, it is necessary and sufficient that $u-\lambda \geqslant 0$. This is equivalent (Prop. 8, (ii)) to the condition $\langle x|u(x)\rangle \geqslant \lambda \|x\|^2$ for every $x\in E$, that is, to $m(u)\geqslant \lambda$. This proves that $m(u)$ is the greatest lower bound of Sp($u$). Similarly, one verifies that $M(u)$ is the least upper bound of Sp($u$).

Since $u$ is normal, one has $\varrho (u) =\|u\|$ (Cor. 1 of I, p. 108). Since $E\not=\{0\}$, the spectrum of $u$ is not empty (Cor. 1 of I, p. 26) and $\varrho (u)$ is the radius of the smallest disk with center 0 which contains Sp($u$) (Theorem 1 of I, p. 24), hence b) follows from a).

### 8. Polar Decomposition

In this number, complex Hilbert spaces are considered.

Let $E_1$ and $E_2$ be Hilbert spaces and let $u\in \mathscr{L}(E_1; E_2)$. The endomorphism $u^*u$ of $E_1$ is positive (Prop. 8), hence one can form the positive element $(u^*u)^{1/2}$ of $\mathscr{L}(E_1)$.

#### Definition 3 {#ts-i-s7-def-3 .statement tag=02GH}

One says that $(u^*u)^{1/2}$ is the absolute value of $u$, and it is denoted by $|u|$.

In the case where $E_1= E_2$, this definition coincides with that given in Remark 9 of I, p. 119.

For an element $u$ of $\mathscr{L}(E_1; E_2)$, let us recall (EVT, V, p. 41, Def. 2) that the initial subspace of $u$ is the closed subspace Ker($u$)$^{\circ}$ of $E_1$ and the final subspace of $u$ is the closed subspace Im($u$) of $E_2$.

#### Proposition 10 {#ts-i-s7-prop-10 .statement tag=02GI}

Let $E_1$ and $E_2$ be complex Hilbert spaces and let $u\in \mathscr{L}(E_1; E_2)$.

a) The initial subspace and the final subspace of $|u|$ are both equal to the initial subspace of $u$ and one has $\||u|\|=\|u\|$;

b) There exists a unique partially isometric mapping $j$ of $E_1$ into $E_2$ such that Ker($j$) $=$ Ker($u$) and $u=j|u|$;

c) The initial (resp. final) subspace of $j$ is equal to that of $u$;

d) Let $u_1$ be a positive element of $\mathscr{L}(E_1)$ and $j_1$ a partially isometric element of $\mathscr{L}(E_1; E_2)$ such that $u=j_1u_1$ and Ker($j_1$) $=$ Ker($u_1$). Then $u_1=|u|$ and $j_1=j$.

For every $x\in E_1$, one has

$$
\|u(x)\|^2=\langle x|(u^*u)(x)\rangle =\langle x||u|^2(x)\rangle =\||u|(x)\|^2 \tag{2}
$$

This proves that Ker($u$) $=$ Ker($|u|$) and $\||u|\|=\|u\|$. Since $|u|$ is hermitian, the closure of the image of $|u|$ is the orthogonal complement of its kernel (EVT, V, p. 41, prop. 4), that is to say the initial space of $u$, whence a).

Formula (2) implies that there exists an isometric mapping $v$ of Im($|u|$) onto Im($u$) such that $v(|u|(x)) =u(x)$ for every $x\in E_1$. Let $j$ be the unique element of $\mathscr{L}(E_1; E_2)$ which extends $v$ and vanishes on Im($|u|$)$^{\circ}=$ Ker($|u|$) $=$ Ker($u$). Then $j$ has the properties of b). The uniqueness of $j$ follows from the decomposition E = Ker($u$)$\oplus$ Im($|u|$).

The initial subspace of $j$ is Ker($j$)$^{\circ}=$ Ker($u$)$^{\circ}$, the initial space of $u$. Its final subspace is $j$(Ker($u$)$^{\circ}$) $=j$(Im($|u|$)) $=$ Im($u$), the final subspace of $u$. This proves c).

Let now $u_1$ and $j_1$ be as in d). We have $u^*u=u_1j_1^*j_1u_1$. The mapping $j_1^*j_1$ is the orthogonal projector with kernel Ker($j_1$) $=$ Ker($u_1$) (EVT, V, p. 41, prop. 5 (ii)) and hence with image Im($u_1$). Therefore $u^*u=u^2_1$ and hence $u_1= (u^*u)^{1/2}=|u|($I, p. 118, prop. 16). The uniqueness assertion of b) finally implies that $j_1=j$.

#### Definition 4 {#ts-i-s7-def-4 .statement tag=02GJ}

Let $E_1$ and $E_2$ be complex Hilbert spaces and $u\in \mathscr{L}(E_1; E_2)$. The pair $(j,|u|)$, where $j$ is the unique partially isometric mapping of $E_1$ into $E_2$ such that $u=j|u|$ and Ker($j$) $=$ Ker($u$), is called the polar decomposition of $u$.

#### Proposition 11 {#ts-i-s7-prop-11 .statement tag=02GK}

Let $E_1$ and $E_2$ be complex Hilbert spaces and $u\in \mathscr{L}(E_1; E_2)$. Let $(j,|u|)$ be the polar decomposition of $u$.

a) We have $|u|=j^*u=u^*j$;

b) We have $|u^*|=ju^*=uj^*$;

c) The polar decomposition of $u^*$ is $(j^*,|u^*|)$.

Let us put I = Ker($u$)$^{\circ}$ and F = Im($u$) for the initial subspace and the final subspace of $u$; moreover, we have I = Ker($|u|$)$^{\circ}=$ Im($|u|$) (prop. 10, a)). The mapping $j^*j$ is the orthogonal projector of $E_1$ onto I (loc. cit. and EVT, V, p. 41, prop. 5 (ii)). Therefore $j^*u=j^*j|u|=|u|$, then $u^*j= (j^*u)^*=|u|^*=|u|$, whence a).

Similarly, one calculates $u^*$ = $|u|j^*= (j^*j|u|)j^*$ = $j^*(j|u|j^*)$. The endomorphism $j|u|j^*$ of $E_2$ is positive. The linear mapping $j^*$ is partially isometric, with initial space F and final space I (EVT, V, p. 41, Prop. 5), and the linear mappings of I into F (resp. of F into I) deduced from $j$ and $j^*$ by passage to the subspaces are isomorphisms inverse to one another (loc. cit.). Hence Ker($j|u|j^*$) $=$ Ker($|u|j^*$) $=$ Ker($j^*$), since the image of $j^*$ is contained in Ker($u$)$^{\circ}=$ Ker($|u|$)$^{\circ}$. According to Prop. 10, d), the pair $(j^*, j|u|j^*)$ is the polar decomposition of $u^*$. This proves c), and assertion b) is then deduced from assertion a) applied to $u^*$.

#### Corollary {#ts-i-s7-n8-cor-1 .statement tag=02GL}

Let $E_1$ and $E_2$ be complex Hilbert spaces and let $u\in \mathscr{L}(E_1; E_2)$. Then Im($u$) $=$ Im($|u^*|$).

Let $(j,|u|)$ be the polar decomposition of $u$. One has $|u^*|=j|u|j^*=uj^*$ by the preceding proposition. By EVT, V, p. 41, Prop. 5, the mapping $j^*$ is partially isometric. Its final space is Ker($j$)$^{\circ}=$ Ker($u$)$^{\circ}$ (Prop. 10, c)). The assertion follows.

#### Proposition 12 {#ts-i-s7-prop-12 .statement tag=02GM}

Let $E_1$ and $E_2$ be complex Hilbert spaces and $u\in \mathscr{L}(E_1; E_2)$. Let $(j,|u|)$ be the polar decomposition of $u$. For $u$ to be bijective, it is necessary and sufficient that $|u|$ be invertible in $\mathscr{L}(E_1)$ and that $j$ be an isomorphism of $E_1$ onto $E_2$.

The condition is sufficient. Conversely, if $u$ is bijective, then $u^*u$ is invertible in $\mathscr{L}(E_1)$, and $|u|= (u^*u)^{1/2}$ is also invertible since its spectrum is contained in $\mathbf{R}_+^*$. Moreover, Ker($j$) $=$ Ker($u$) $=\{0\}$ and Im($j$) $=$ Im($u$) $= F$, whence $j$ maps $E_1$ isometrically onto $E_2$.

#### Proposition 13 {#ts-i-s7-prop-13 .statement tag=02GN}

Let E be a complex Hilbert space and $u$ an endomorphism of E. The following conditions are equivalent:

(i) The endomorphism $u$ is normal;

(ii) There exists a unitary element $v$ of $\mathscr{L}(E)$, permutable with $|u|$, such that $u=v|u|$.

Let $(j,|u|)$ be the polar decomposition of $u$. Suppose that $u$ is normal. Then $|u^*|= (uu^*)^{1/2}= (u^*u)^{1/2}=|u|$. Prop. 11 then implies $|u|j=|u^*|j=ju^*j=j|u|$. Moreover, $j$ leaves stable the supplementary orthogonal subspaces Ker($|u|$) $=$ Ker($j$) and Im($|u|$) $=$ Im($j$) (prop. 10). Let $v$ be the element of $\mathscr{L}(E)$ which coincides with $j$ on Ker($u$)$^{\circ}$ and with the identity mapping on Ker($u$). Since $j$ induces an isometry of Ker($u$)$^{\circ}$ onto Im($u$) $=$ Ker($u^*$)$^{\circ}=$ Ker($u$)$^{\circ}$ (since $u$ is normal), the endomorphism $v$ is unitary; moreover, it is permutable with $|u|$, since $j|u|=|u|j$, and one has $u=v|u|$.

Conversely, let $v$ be a unitary element of $\mathscr{L}(E)$, permutable with $|u|$, such that $u=v|u|$. One has $uu^*=v|u|^2v^*=|u|^2vv^*=|u|^2=u^*u$, therefore $u$ is normal.

Let E be a complex Hilbert space and $u\in \mathscr{L}(E)$. Let $(j,|u|)$ be the polar decomposition of $u$. It may happen that $j$ commutes with $|u|$ without $u$ being normal (Exercise 11 of I, p. 189).

## EXERCISES {#ts-i-s7-exercises}

In the exercises below, all Banach spaces are over $\mathbf{C}$.

See the [exercises for § 7](exercises/s7/).
