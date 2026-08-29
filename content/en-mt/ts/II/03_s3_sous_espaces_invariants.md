---
book: ts
book_title: Théories spectrales
chapter: II
chapter_title: GROUPES LOCALEMENT COMPACTS COMMUTATIFS
section: 3
section_title: Sous-espaces invariants
lang: en
source: ts-i-ii-fr
book_pages: TS II.250-TS II.261, TS II.308-TS II.318
pdf_pages: 0262-0273, 0320-0330
extraction: native
subsections:
    - "no": 1
      title: Le cas de l’espace hilbertien $L^2(G)$
      page: 251
      pdf_page: 263
    - "no": 2
      title: Idéaux fermés de $L^1(G)$
      page: 251
      pdf_page: 263
    - "no": 3
      title: Sous-espaces invariants faiblement fermés de $L^{\infty}(G)$
      page: 257
      pdf_page: 269
statements: 12
exercises: 19
content_sha256: e8711a1f911a52cd46969798526bf587664ce4bff24468093600ea5ec18b7674
translated_from: content/fr/ts/II/03_s3_sous_espaces_invariants.md
source_lang: fr
translation_method: machine
source_content_sha256: 53b9dd4c4ef649cd2bc5283995540b3c864a2e7f5144d3f97d442f0fa2bfffc2
translation_model: gpt-5.4, gpt-5-6-mini, gpt-5-mini
translation_run: translate-en-mt-bc38f5e9
glossary_version: 34
glossary_terms_sha256: 70dd9d5608118a51fea2ed3d745ade25be8ad69e96347d9b6b1f2ef3bbfbb1d0
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 3. INVARIANT SUBSPACES

The object of this No. is the study of certain subspaces invariant under translation in the spaces $L^1(G)$, $L^2(G)$ and $L^{\infty}(G)$.

### 1. The case of the Hilbert space $L^2(G)$

For every measurable subset M of $\widehat{G}$, we denote by $E_M$ the set of $f\in$ $L^2(G)$ such that the Fourier transform $\mathscr{F}_G(f)$ is zero almost everywhere on $\widehat{G}$. Let $\varphi_M$ be the characteristic function of M. The space $E_M$ is the kernel of the continuous linear mapping $f\mapsto \varphi_M\mathscr{F}_G(f)$ from $L^2(G)$ into $L^2(\widehat{G})$, and is therefore a closed subspace of $L^2(G)$.

#### Proposition 1 {#ts-ii-s3-prop-1 .statement tag=02N3}

a) Let M be a measurable subset of $\widehat{G}$. For every $x\in G$, the space $E_M$ is stable under the mapping $f\mapsto \varepsilon_x*f$;

b) Let M and N be measurable subsets of $\widehat{G}$. We have $E_M= E_N$ if and only if M and N are equal up to a locally negligible set;

c) Every subspace of $L^2(G)$ stable under the mappings $f\mapsto \varepsilon_x*f$ for every $x\in G$ is of the form $E_M$ for some measurable subset M of $\widehat{G}$.

This result will be proved later (cf. V, to appear).

### 2. Closed ideals of $L^1(G)$

The cotransform of Fourier on the Banach algebra $L^1(G)$ is identified with the Gelfand transform of $L^1(G)$ (II, p. 209). With this identification, recall that if I is an ideal of $L^1(G)$, we denote by V(I) the closed set in $\widehat{G}$ of characters $\chi \in \widehat{G}$ such that, for every function $f\in I$, the cotransform of Fourier of $f$ vanishes at $\chi ($cf. I, p. 30). For every subset M of $\widehat{G}$, we denote by Υ(M) the closed ideal of $f\in L^1(G)$ such that $\overline{\mathscr{F}}_G(f)$ vanishes on M (I, p. 30).

By prop. 2 of II, p. 219, the Banach algebra $L^1(G)$ is regular. By § 5 of I, p. 88, we therefore deduce the following properties of the transform and cotransform of Fourier:

1) If F is a closed subset of $\widehat{G}$ and K a compact subset of $\widehat{G}$ such that $F\cap K =\emptyset$, there exists a function $f\in L^1(G)$ such that $\mathscr{F}_G(f)$ is equal to 0 on F and to 1 on K (I, p. 88, prop. 1; for this fact and the following ones, one passes from the cotransform of Fourier to the transform of Fourier by means of formula (8) of II, p. 207).

2) Let M be a closed subset of $\widehat{G}$. The set of ideals I of $L^1(G)$ such that V(I) = M has as greatest element Υ(M) and as smallest element the set of $f\in L^1(G)$ whose cotransform of Fourier has compact support disjoint from M (I, p. 91, prop. 4).

3) Let I be an ideal of $L^1(G)$, and let $g:\widehat{G}\rightarrow \mathbf{C}$ be a continuous function. Suppose that, for every $\chi \in \widehat{G}$, there exists a function $f_{\chi}\in I$ such that $g$ is equal to $\mathscr{F}_G(f_{\chi})$ in a neighbourhood of $\chi$. Suppose moreover that there exists a function $f_{\infty}\in I$ such that $g$ is equal to $\mathscr{F}_G(f_{\infty})$ in the complement of a compact subset of $\widehat{G}$, this latter condition always being satisfied if G is discrete. Then there exists a function $f\in I$ such that $g=\mathscr{F}_G(f)$ (I, p. 91, cor. 2).

#### Lemma 1 {#ts-ii-s3-lem-1 .statement tag=02N4}

The space of functions of $L^1(G)$ whose Fourier transform has compact support is dense in $L^1(G)$.

Since $\mathscr{K}(\widehat{G})$ is dense in $L^2(\widehat{G})$ and the Fourier transform of $L^2(G)$ is an isometry onto $L^2(\widehat{G})$ (th. 1 of II, p. 215), the subspace V of $L^2(G)$ formed by the $f\in L^2(G)$ such that $\mathscr{F}_G(f)\in \mathscr{K}(\widehat{G})$ is dense in $L^2(G)$.

Let $g\in L^1(G)$. There exist $g_1, g_2\in L^2(G)$ such that $g=g_1g_2$ (one may for example take $g_1=|g|^{1/2}$, and $g_2(x) = 0$ if $g(x) = 0,g_2(x) =$ $g(x)/g_1(x)$ otherwise). It follows therefore from what precedes that $g$ is the limit of a sequence of functions of the form $h_1h_2$, where $h_1$ and $h_2$ belong to V. Now $\mathscr{F}_G(h_1h_2) =\mathscr{F}_G(h_1)*\mathscr{F}_G(h_2)$ (II, p. 223, prop. 14), and $\mathscr{F}_G(h_1)*$ $\mathscr{F}_G(h_2)$ belongs to $\mathscr{K}(G)$. The lemma follows.

#### Proposition 2 {#ts-ii-s3-prop-2 .statement tag=02N5}

Let I be a closed ideal of $L^1(G)$, and let $f\in L^1(G)$. If $\overline{\mathscr{F}}_G(f)$ vanishes on a neighbourhood of V(I), then $f$ belongs to I.

Let $\varepsilon  >0$. There exists a function $g\in L^1(G)$ such that $\|f-f*g\|_1<$ $\varepsilon$ (prop. 8 of II, p. 211 (iv)). Let $h\in L^1(G)$ be such that the support of $\overline{\mathscr{F}}_G(h)$ is compact and $\|f\|_1\|g-h\|_1< \varepsilon$ (lemma 1). We have

$$
\|f-f*h\|_1\leqslant \|f-f*g\|_1+\|f*(g-h)\|_1<2\varepsilon
$$

By the assumption on $f$, the function $\overline{\mathscr{F}}_G(f*h) =\overline{\mathscr{F}}_G(f)\overline{\mathscr{F}}_G(h)$ has compact support disjoint from V(I), which implies that $f*h\in I$ (remark 2 above). Since $\varepsilon$ is arbitrarily small, we have $f\in$ I = I.

#### Theorem 1 {#ts-ii-s3-thm-1 .statement tag=02N6}

Let I be a closed ideal of $L^1(G)$ distinct from $L^1(G)$. There exists a character $\widehat{x}\in \widehat{G}$ such that $\mathscr{F}_G(f)(\widehat{x}) = 0$ for every $f\in I$.

Comme the algebra $L^1(G)$ is regular (prop. 2 of II, p. 219) and without radical (cor. of prop. 22 of I, p. 126), and since the set of functions whose Fourier cotransform has compact support is dense in $L^1(G)$ (lemma 1), cor. 1 of I, p. 92 shows that the ideal I is contained in a regular maximal ideal of $L^1(G)$, that is to say in the kernel of a character $\widehat{y}$ of $L^1(G)$ (th. 2 of I, p. 30); one can then take $\widehat{x}=\widehat{y}^{-1}($cf. formula (8) of II, p. 207).

Corollary 1 (Wiener Tauberian Theorem)

Let $f\in L^1(G)$. If the Fourier transform of $f$ does not vanish, the functions $f*\varepsilon_x:g\mapsto f(gx^{-1})$, where $x$ runs through G, form a total set in $L^1(G)$ (EVT, I, p. 12, def. 1).

Let V be the closed vector subspace of $L^1(G)$ generated by the $f*\varepsilon_x$. By INT, VIII, §4, cor. of prop. 20, the space V is a closed ideal of $L^1(G)$. By th. 1 we have $V = L^1(G)$.

#### Definition 1 {#ts-ii-s3-def-1 .statement tag=02N7}

Let $g$ be a complex function on G and let Φ be a filter on G. We say that $g$ is slowly oscillating following Φ if, for every $\varepsilon  >0$, there exists a set $M\in \Phi$ and a neighbourhood V of $e$ in G such that

$x\in M$ and $y\in V=\Rightarrow |g(xy)-g(x)|\leqslant \varepsilon$.

#### Corollary 2 {#ts-ii-s3-def-1-cor-2 .statement tag=02N8}

Let Φ be a filter on G invariant under translation. Let $f\in L^1(G)$ such that the Fourier transform of $f$ does not vanish and such that $\int_Gf(x)dx= 1$. Let $g\in L^{\infty}(G)$. Suppose that $f*g$ has a finite limit $\alpha$ following Φ.

a) For every function $h\in L^1(G)$ such that $\int_Gh(x)dx= 1$, the limit of $h*g$ following Φ is equal to $\alpha$;

b) Suppose in addition that $g$ is slowly oscillating following Φ. Then $g$ tends to $\alpha$ following Φ.

Replacing $g$ by $g-\alpha$, we reduce to the case where $\alpha = 0$. Let I be the set of functions $h\in L^1(G)$ such that $h*g$ tends to 0 following Φ. The set I is a vector subspace of $L^1(G)$ invariant under translation. It is a closed space. Indeed, let $h\in \overline{I}$. For every function $h_0\in L^1(G)$ and every $x\in G$, we have

$$
|(h*g)(x)|\leqslant |((h-h_0)*g)(x)|+|(h_0*g)(x)|
$$

$$
\leqslant \|h-h_0\|_1\|g\|_{\infty}+|(h_0*g)(x)|
$$

For every $\varepsilon  >0$, there exists $h_0\in I$ such that $\|h-h_0\|_1\|g\|_{\infty}< \varepsilon$. Let $M\in$ Φ such that $|(h_0*g)(x)|< \varepsilon$ for every $x\in M$. We then have $|(h*g)(x)|<2\varepsilon$ for every $x\in M$, hence $h*g$ converges to 0 following Φ. This shows that $h\in I$.

The space I is therefore a closed ideal of $L^1(G)$. We have $f\in I$ by assumption, hence $I = L^1(G)$ by th. 1 since the Fourier transform of $f$ does not vanish. This implies a).

Let us place ourselves under the hypotheses of b). Let $\varepsilon  >0$. Since $g$ is slowly oscillating according to Φ, there exists $M\in \Phi$ and a compact neighbourhood V of $e$ such that

$x\in M$ and $y\in V =\Rightarrow  |g(y^{-1}x)-g(x)|\leqslant \varepsilon$.

Let $\varphi$ be the characteristic function of V and $\mu=\int\varphi (x)dx$. For every $x\in G$, we have

$$
\frac{1}{\mu}(\varphi *g)(x) =\frac{1}{\mu}\int_Vg(y^{-1}x)dy=g(x) +\frac{1}{\mu}\int_V(g(y^{-1}x)-g(x))dy
$$

Thus for every $x\in M$, we have

$$
|\frac{1}{\mu}(\varphi *g)(x)-g(x)|\leqslant \varepsilon
$$

Since, by a), the limit of $\varphi *g$ according to Φ is zero, we have lim sup$_{\Phi}|g|\leqslant \varepsilon$. Since $\varepsilon$ is arbitrary, we conclude that the limit of $g$ according to Φ is zero, which proves b).

#### Lemma 2 {#ts-ii-s3-lem-2 .statement tag=02N9}

Let K be a compact subset of G. For every $\eta  >0$, there exists a function $j\in L^1(G)$ such that:

$$
\surd
$$

a) $\|j\|_1\leqslant$ 2 ;

b) the function $\mathscr{F}_G(j)$ is equal to 1 in a neighbourhood of the identity element of $\widehat{G}$;

c) for every $x\in K$, we have $\|j-j*\varepsilon_x\|_1\leqslant \eta$.

The set $U_1$ of the elements $\widehat{x}\in \widehat{G}$ such that

$$
|\langle \widehat{x}, x\rangle  -1|\leqslant \frac{\eta}{4}
$$

for every $x\in$ K is a neighbourhood of $e$ in $\widehat{G}$. Let U $\subset U_1$ be an open, symmetric, and integrable neighbourhood for the Haar measure $m=d\widehat{x}$ of $\widehat{G}$ dual to the measure $dx$. Let $V\subset U$ be a compact symmetric neighbourhood of $e$ such that $m(V)\geqslant \frac{1}{2}m(U)$. Let us denote by $\varphi_U$ (resp. $\varphi_V$) the characteristic function of U (resp. of V). Since $\varphi_U$ belongs to $L^2(G)$, there exists $u\in L^2(G)$ such that $\varphi_U=\mathscr{F}_G(u)$ (th. 1 of II, p. 215). Analogously, there exists a function $v\in L^2(G)$ such that $\varphi_V=\mathscr{F}_G(v)$. We now prove that the function $j=\frac{1}{m(V)}uv$ verifies the required properties. We have $j\in L^1(G)$.

a) By the Plancherel theorem and the condition $m(V)\geqslant \frac{1}{2}m(U)$, we have

$$
\|j\|_1\leqslant \frac{\|u\|_2\|v\|_2}{m(V)}=\frac{\|\mathscr{F}_G(u)\|_2\|\mathscr{F}_G(v)\|_2}{m(V)}=\surd\overline{mm(U)(V)m(V)}\leqslant \surd \overline{2}
$$

b) There exists a neighbourhood W of $e$ in $\widehat{G}$ such that WV $\subset U$ (TG, II, p. 31, prop. 4). For every $\widehat{x}\in W$, we have $\widehat{x}V\subset U$, and prop. 14 of II, p. 223 implies

$$
\mathscr{F}_G(j)(\widehat{x}) =\frac{1}{m(V)}(\mathscr{F}_G(u)*\mathscr{F}_G(v))(\widehat{x})
$$

$$
=\frac{1}{m(V)}\int_{\widehat{G}}\varphi_U(\widehat{y})\varphi_V(\widehat{y}^{-1}\widehat{x})dm(\widehat{y})
$$

$$
=\frac{m(U \cap\widehat{x}V^{-1})}{m(V)}=\frac{m(\widehat{x}V)}{m(V)}= 1
$$

since V is symmetric.

c) If $x\in K$, we have

$$
\|u-u*\varepsilon_x\|^2_2=\int_{\widehat{G}}|\mathscr{F}_G(u)(\widehat{x})(1- \langle x,\widehat{x}\rangle )||^2dm(\widehat{x})\leqslant m(U)(\frac{\eta}{4})^2
$$

since $U\subset U_1$, and analogously $\|v-v*\varepsilon_x\|^2_2\leqslant m(V)(\frac{\eta}{4})^2$. Hence

$$
\|j-j*\varepsilon_x\|_1=\frac{1}{m(V)}\|u(v-v*\varepsilon_x) + (v*\varepsilon_x)(u-u*\varepsilon_x)\|_1
$$

$$
\leqslant \frac{\eta}{4m(V)}(\|u\|_2\surd m(V) +\|v\|_2\surd\overline{m(U)})
$$

$$
=\eta \surd\overline{m2m(U)(V)m(V)}< \eta
$$

#### Proposition 3 {#ts-ii-s3-prop-3 .statement tag=02NA}

The algebra $L^1(G)$ satisfies the Ditkin condition (I, p. 92, def. 2).

Let $\chi$ be a character of $L^1(G)$. Distinguish two cases according as $\chi$ is zero or nonzero. If $\chi$ is zero, it must be verified that for every function $f\in L^1(G)$, there exists a sequence $(f_n)_{n\geqslant 1}$ in $L^1(G)$ such that $\mathscr{F}(f_n)$ vanishes outside a compact subset of $\widehat{G}$ and such that $f_n*f$ tends to $f$ in $L^1(G)$. The existence of such a sequence follows from Lemma 1 above and Proposition 8 of II, p. 211.

Suppose now that $\chi$ is nonzero, hence $\chi \in \mathsf{X}(L^1(G)) =\widehat{G}$ (Proposition 1 of II, p. 202). Let $f\in L^1(G)$ be such that $\mathscr{G}_{L^1(G)}(f)(\chi ) =$ $\overline{\mathscr{F}}(f)(\chi ) = 0$. It is a question of proving the existence of a sequence $(f_n)_{n\geqslant 1}$ in $L^1(G)$ such that $f*f_n$ converges to $f$ in $L^1(G)$ and such that $\overline{\mathscr{F}}(f_n)$ vanishes in a neighbourhood of $\chi$. We may suppose that $\|f\|_1= 1$. By translation in $\widehat{G}$, we reduce to the case where $\chi =e$.

Let $K_n$ be a compact subset of G such that

$$
\int_{G-K_n}|f(x)|dx\leqslant \frac{1}{n}
$$

Let $u_n\in L^1(G)$ be a function $\geqslant 0$ such that $\|u_n\|_1= 1$ and

$$
\|f-f*u_n\|_1\leqslant \frac{1}{n}
$$

(cf. Proposition 8 of II, p. 211, (iii)). According to Lemma$\surd$ 2, there exists a function $j_n$ in $L^1(G)$ such that $\|j_n\|_1\leqslant \overline{2}$, whose Fourier cotransform is equal to 1 in a neighbourhood of $e$, and moreover such that $\|j_n-j_n*\varepsilon_x\|_1\leqslant n^{-1}$ for every $x\in K_n$. Put

$$
f_n=u_n-j_n*u_n
$$

We shall prove that the sequence $(f_n)_{n\geqslant 1}$ has the required properties. First of all, we have

$$
\mathscr{F}(f_n) =\mathscr{F}(u_n)-\mathscr{F}(j_n)\mathscr{F}(u_n) = (1-\mathscr{F}(j_n))\mathscr{F}(u_n)
$$

hence the Fourier transform of $f_n$ vanishes in a neighbourhood of $\chi =e$. On the other hand,

1

$$
\|f*f_n-f\|_1\leqslant \|f*u_n-f\|_1+\|f*j_n\|_1\|u_n\|_1\leqslant +\|f*j_n\|_1
$$

$$
n
$$

Now, for almost every $y\in G$, we have

$$
(f*j_n)(y) =\int_Gf(x)j_n(x^{-1}y)dx=\int_Gf(x)(j_n(x^{-1}y)-j_n(y))dx
$$

since, by assumption, we have $\mathscr{F}(f)(e) =\int_Gf(x)dx= 0$. Hence

$$
\|f*j_n\|_1\leqslant \int_G|f(x)| \|j_n*\varepsilon_x-j_n\|_1dx
$$

$$
=\int|f(x)| \|j_n*\varepsilon_x-j_n\|_1dx
$$

$$
+\int^{K_n}|f(x)| \|j_n*\varepsilon_x-j_n\|_1dx
$$

$G-K_n$

$1\int\int$ 5 $\leqslant |f(x)|dx+ 4|f(x)|dx\leqslant$.

$n_{K_n}G-K_{_n}n$

Finally, $\|f*f_n-f\|_1\leqslant 6n^{-1}$ and therefore $f*f_n$ converges in $f$ in $L^1(G)$, as desired.

Applying prop. 5, we obtain the following result:

#### Theorem 2 {#ts-ii-s3-thm-2 .statement tag=02NB}

Let I be a closed ideal of $L^1(G)$ such that the boundary of V(I) contains no nonempty perfect set. Then I is the set of functions $f\in L^1(G)$ such that $\mathscr{F}(f)$ vanishes on V(I).

For an arbitrary closed ideal of $L^1(G)$, the conclusion of th. 2 is in general false (cf. exer. 12 of II, p. 314). More precisely, one can now prove that, if G is noncompact, there exists a closed ideal of $L^1(G)$ which is not self-adjoint (see for example W. Rudin, Fourier analysis on groups, Interscience tracts in pure and applied mathematics, theorem 7.7.1.)

#### Corollary {#ts-ii-s3-n2-cor-1 .statement tag=02NC}

If a closed ideal I of $L^1(G)$ is contained in a single regular maximal ideal, then I itself is regular maximal.

### 3. Weakly closed invariant subspaces of $L^{\infty}(G)$

In this number, we identify $L^{\infty}(G)$ with the dual of $L^1(G)$, and equip it with the weak topology $\sigma (L^{\infty}(G),L^1(G))$. We denote by $(f, g)\mapsto  \langle f, g\rangle$ the bilinear mapping defining this duality for $f\in L^1(G)$ and $g\in L^{\infty}(G)$.

The mapping $W\mapsto W^{\circ}$ is a bijection of the set of weakly closed vector subspaces of $L^{\infty}(G)$ onto the set of closed vector subspaces of $L^1(G)$ (EVT, II, p. 55, prop. 10).

On the other hand, if $f\in L^1(G)$ and $x\in G$, the endomorphism $g\mapsto f*g$ (resp. $g\mapsto \varepsilon_x*g$) of the Banach space $L^1(G)$ has for transpose the endomorphism $h\mapsto \check{f}*h$ (resp. $h\mapsto \varepsilon_{x^{-1}}*h$) of the Banach space $L^{\infty}(G)$ (INT, VIII, §4, n$^o3$, example 6). For a closed vector subspace of $L^1(G)$ to be an ideal of $L^1(G)$, it is necessary and sufficient that it be invariant under the translations of G. Therefore, for a weakly closed vector subspace of $L^{\infty}(G)$ to be stable under convolution with the elements of $L^1(G)$, it is necessary and sufficient that it be invariant under the translations of G.

Let W be a weakly closed vector subspace of $L^{\infty}(G)$. Suppose that W (and therefore also $W^{\circ}$) is invariant under the translations of G. Let $f\in$ $L^1(G)$. For every $g\in L^{\infty}(G)$, we have $(\check{f}*g)(x) =\langle \varepsilon_x*f, g\rangle =\langle f, \varepsilon_{x^{-1}}*g\rangle$. Therefore, for $f$ to belong to $W^{\circ}$, it is necessary and sufficient that $\check{f}*g= 0$ for every $g\in W$.

If W is a weakly closed vector subspace of $L^{\infty}(G)$ invariant under translation, we shall denote by A(W) the set of characters $\chi \in \widehat{G}$ which belong to W. It is a closed subset of $\widehat{G}$. If F is a closed subset of $\widehat{G}$, we shall denote by Y(F) the weakly closed vector subspace of $L^{\infty}(G)$ generated by the elements of F; since every translation of G transforms each character into a function proportional to this character, the space Y(F) is invariant under translation.

Let W be a weakly closed subspace of $L^{\infty}(G)$ invariant under the translations of G. According to the bipolar theorem (EVT, II, p. 48, th. 1), a character $\chi$ belongs to W if and only if it belongs to $(W^{\circ})^{\circ}$; this last space is the set of functions $g\in L^{\infty}(G)$ such that $\langle f, g\rangle = 0$ for $f\in W^{\circ}$. We have $\langle f, \chi \rangle =\overline{\mathscr{F}}(f)(\chi )$, and therefore

$$
A(W) = V(W^{\circ})
$$

Similarly, a function $f\in L^1(G)$ belong to $Y(F)^{\circ}$ if and only if $\langle f, \chi \rangle = 0$ for every $\chi \in F$, which is equivalent to $\overline{\mathscr{F}}(f)(\chi ) = 0$ for $\chi \in F$, that is, to $f\in \Upsilon (F)$. Hence (loc. cit.) we have

$$
Y(F) = \Upsilon (F)^{\circ}
$$

The relations V(Υ(F)) = F (I, p. 13 and I, p. 30) and $\Upsilon (V(I))\supset I$, combined with the bipolar theorem (TVS, II, p. 48, th. 1), then yield

$$
A(Y(F)) = F,Y(A(W))\subset W
$$

#### Proposition 4 {#ts-ii-s3-prop-4 .statement tag=02ND}

Let W be a weakly closed vector subspace of $L^{\infty}(G)$, invariant under translation and nonzero. Then W contains at least one character of G.

We have seen that $A(W) = V(W^{\circ})$. Since $W\not= 0$, we have $W^{\circ}\not= L^1(G)$, and then $V(W^{\circ})$ is nonempty by th. 1 of II, p. 252.

#### Proposition 5 {#ts-ii-s3-prop-5 .statement tag=02NE}

Let W be a weakly closed vector subspace of $L^{\infty}(G)$ invariant under translation.

a) For every neighbourhood U of A(W) in $\widehat{G}$, every function of W is the weak limit of linear combinations of characters belonging to U;

b) If the boundary of A(W) contains no nonempty perfect set, every function of W is the weak limit of linear combinations of characters belonging to W.

To prove a), it is enough by the bipolar theorem to show that if $f$ is a function of $L^1(G)$ orthogonal to the elements of U, then $f$ is orthogonal to W. Now the Fourier cotransform $\overline{\mathscr{F}}(f)$ then vanishes on the neighbourhood U of $A(W) = V(W^{\circ})$, so that prop. 2 of II, p. 252 shows indeed that $f\in W^{\circ}$. Assertion b) is established similarly, using th. 2 of II, p. 257 instead of prop. 2 of II, p. 252.

# Exercises

In all the exercises of Chapter II, the dual of $\mathbf{R}^n$ (resp. of $(\mathbf{R}/\mathbf{Z})^n$, of $\mathbf{Z}^n$) is identified with $\mathbf{R}^n$ (resp. with $\mathbf{Z}^n$, with $(\mathbf{R}/\mathbf{Z})^n$) according to corollary 3 of II, p. 236. For $x$ and $y$ in $\mathbf{R}^n$, we write $x\cdot y=\sum_ix_iy_i$. We write $\mathbf{T}=\mathbf{R}/\mathbf{Z}$, and endow $\mathbf{T}$ with its real Lie group structure (LIE, III, p. 105, prop. 11). The Fourier transform of a function $f$ will often be denoted by $\widehat{f}$.

For every nonzero real number $t$, we write s($t$) $=t/|t|$, and we put s(0) = 0 (sign function).

If E is a topological vector space and $(x_h)_{h\in\mathbf{Z}}$ a family of elements of E, the series with general term $x_h$ is said to converge symmetrically in E to $x\in E$ if the sequence $(s_n)_{n\geqslant 1}$ defined by

$$
s_n=\sum_{-n\leqslant h\leqslant n}x_h
$$

converges to $x$ in E.

A probability measure on a locally compact topological space X is a positive measure of total mass 1. The set of probability measures on X is denoted by $\mathscr{P}(X)$.

Unless otherwise stated, G denotes a locally compact commutative topological group.

## EXERCISES {#ts-ii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
