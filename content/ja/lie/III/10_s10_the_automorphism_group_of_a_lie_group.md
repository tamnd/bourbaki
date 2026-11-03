---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 10
section_title: The automorphism group of a Lie group
lang: ja
source: lie-i-iii
book_pages: 359-368
pdf_pages: 0377-0386, 0427-0427
extraction: ocr
subsections:
    - "no": 1
      title: INFINITESIMAL AUTOMORPHISMS
      page: 359
      pdf_page: 377
    - "no": 2
      title: THE AUTOMORPHISM GROUP OF A LIE GROUP (REAL OR COMPLEX CASE)
      page: 362
      pdf_page: 380
    - "no": 3
      title: THE AUTOMORPHISM GROUP OF A LIE GROUP (ULTRAMETRIC CASE)
      page: 367
      pdf_page: 385
statements: 13
exercises: 4
content_sha256: d597013b0547ab643b52a83e96722b64d5191f5d27c1bd14a9a8e3baf5ff1c82
translated_from: content/en/lie/III/10_s10_the_automorphism_group_of_a_lie_group.md
translation_method: google
source_content_sha256: f9d7400def142eff7395a68ad471a8fd0e9e5f47e8dd9c61b495ed3c4a325f89
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: 61477138f641ee8400fe637ddf51baee21bbff46408d440abbe17d4f15c5da59
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 10。 リー群中自己同型群

この段落では、K は標数0 であると仮定します。

### 1. 無限小自己同型

#### 補題 1 {#lie-iii-s10-lem-1 .statement tag=0AL6}

G を G 上のリー群と $\alpha$ ベクトル体とします。すべての $g \in G$ について、
$$
\beta(g) = \alpha(g)g^{-1} \in L(G).
$$
次の条件は同等です。
(i) $\alpha$ は群 G の準同型を群 T(G) に変換します。
(ii) G のすべての $g, g'$、$\alpha(gg') = \alpha(g)g' + g\alpha(g')$ について。
(iii) G のすべての $g, g'$、$\beta(gg_1) = \beta(g) + (\mathrm{Ad}\,g)\beta(g')$。

条件 (i) は、G のすべての $g, g'$ について、群 T(G) に次の式があることを意味します。
$$
\beta(g)g\beta(g')g' = \beta(gg')gg'
$$
または
$$
\beta(g)((\mathrm{Ad}\,g)\beta(g'))gg' = \beta(gg')gg'.
$$
しかし、T(G) の $\beta(g)$ と $(\mathrm{Ad}\,g)\beta(g')$ の積は、$L(G)$ (§ 2, no. 1, 命題 2) の $\beta(g)$ と $(\mathrm{Ad}\,g)\beta(g')$ の和にすぎません。したがって、(i) $\Leftrightarrow$ (iii)。一方、条件 (ii) は、$\beta(gg')gg' = \beta(g)gg' + g\beta(g')g'$、または
$$
\beta(gg') = \beta(g) + (\mathrm{Ad}\,g)\beta(g')
$$
したがって (ii) $\Leftrightarrow$ (iii)。

#### 定義 1 {#lie-iii-s10-def-1 .statement tag=0AL7}

G をリー群とします。 G の微小自己同型は、補題 1 の G 満たす条件上の任意の解析ベクトル体です。

#### 補題 2 {#lie-iii-s10-lem-2 .statement tag=0AL8}

$K'$ を K、A の$K'$-多様体、B および C $K$-多様体、および $f$ を $A \times B$ の $K'$-解析的写像とする非離散閉部分体とします。 C。仮に、全員にとって、

リー群

$a \in A$、*写像* $b \mapsto f(a, b)$ *of* B *into* C *は* K-*分析*です。 *そして、すべて* $t \in TA$、*写像* $u \mapsto (Tf)(t, u)$ *の* TB *を* TC *はK-*分析*です。

$t \in TA$を固定して$g(u) = (Tf)(t, u)$と書きます。明らかに $g$ は K' 分析的です。 *微分可能および解析的多様体*、R、5.14.6 により、接線写像から $g$ が K 線形であることを証明するだけで十分です。 A、B、C は完全ノルマブル空間 E、F、G 上で 0 の近傍が K'、K、K 上で開いており、$t$ は 0 で A に接していると仮定できます。同一視する TA、TB、TC、$A \times E, B \times F, C \times G$ と$t$ と E の元。次に、すべての $(x, y) \in TB = B \times F$ です。

$$
g(x, y) = (f(0, x), (D_1f)(0, x)(t) + (D_2f)(0, x)(y)).
$$

私たちは同一視する $T(B \times F)$ と $(B \times F) \times (F \times F)$ 、$T(C \times G)$ と $(C \times G) \times (G \times G)$ です。それでは、皆さんに

$$
((x, y), (h, k)) \in T(B \times F) = (B \times F) \times (F \times F),
$$

$(Tg)((x, y), (h, k)) = ((a, b), (c, d))$、ここで

$$
\begin{align*}
a &= f(0, x), \\
b &= (D_1f)(0, x)(t) + (D_2f)(0, x)(y), \quad c = (D_2f)(0, x)(h), \\
d &= (D_2D_1f)(0, x)(t, h) + (D_2D_2f)(0, x)(y, h) + (D_2f)(0, x)(k).
\end{align*}
$$

$(x, y) \in B \times F$ を修正します。 $F \times F$ から $G \times G$ への写像 $(h, k) \mapsto (c, d)$ が K 線形であることを証明する必要があります。 B の写像 $x \mapsto f(0, x)$ を C に変換すると、K 解析であるため、写像

$$
(h, k) \mapsto (D_2f)(0, x)(h), \quad (h, k) \mapsto (D_2D_2f)(0, x)(y, h),
$$
$$(h, k) \mapsto (D_2f)(0, x)(k)$$

は K 線形です。一方、

$$
(D_2D_1f)(0, x)(t, h) = \lim_{\lambda \in K', \lambda \to 0} \lambda^{-1}((D_2f)(\lambda t, x)(h) - (D_2f)(0, x)(h))
$$

そして、固定 $\lambda$ の場合、写像 $x \mapsto f(\lambda t, x)$ は K 解析であるため、写像 $h \mapsto (D_2f)(\lambda t, x)(h)$ は K 線形です。

#### 命題 1 {#lie-iii-s10-prop-1 .statement tag=0AL9}

*K' *を非離散閉部分体 of* K, G *リー群 over* K, V *多様体 over* K' *and* $(v, g) \mapsto vg$ *a* K'-*analytic 写像 of* V $\times$ G *into* G. *すべて* $v \in V$、*写像* $g \mapsto vg$ *of* G *into* G *は自己同型 of* G であるとします。 *$\varepsilon$ *be 元 of* V *そのような* $\varepsilon g = g$ *すべて* $g \in G$ * と * $a \in T_\varepsilon(V)$。 *するとベクトル体* $g \mapsto ag$ *on* G *は * G の無限小自己同型です。

$v \in V,\ g_1 \in G,\ g_2 \in G,\ v(g_1g_2) = (vg_1)(vg_2)$の場合。したがって、$u_1 \in TG,\ u_2 \in TG,\ a(u_1u_2) = (au_1)(au_2)$ (§ 2, no. 1, 命題 3) の場合です。特に、TG への G の写像 $g \mapsto ag$ は群準同型です。一方、この写像は補題 2 によって解析されます。

#### 命題 2 {#lie-iii-s10-prop-2 .statement tag=0ALA}

*G を *実数または複素数リー群および * $\alpha$ *G の無限小値自己同型とします。次の特性を持つ G 上の K の解析的演算 $(\lambda, g) \mapsto \phi_\lambda(g)$ の法則が存在します。
(1) D が無限小演算の関連する法則である場合、$D(1) = \alpha$。
(2) $\lambda \in K$、$\phi_\lambda \in \mathrm{Aut}\, G$ 全員。
(a) すべての $\mu > 0$ について、$K_\mu$ を K の中心 0 および半径 $\mu$ の開球とします。すべての $g \in G$ について、$\mathscr{F}_g$ を球で定義された解析積分曲線 $f$ の $\alpha$ の集合とします。 $K_\mu$ などの $f(0) = g$。 Differentiable and Analytic 多様体、R、9.1.3 および 9.1.5 によると、$\mathscr{F}_g$ は空ではなく、定義のドメインの共通部分上の $\mathscr{F}_g$ 一致するの 2 つの元です。 $\mu(g)$ を数 $\mu$ の最小の上界とし、$K_\mu$ で定義された $\mathscr{F}_g$ の元が存在するようにします。 $K_{\mu(g)}$ で定義された $\mathscr{F}_g$ の一意元が存在します。それを$f_g$で表します。
(b) $g_1, g_2$ を G、$f_1 \in \mathscr{F}_{g_1}, f_2 \in \mathscr{F}_{g_2}$ とし、$f_1$ と $f_2$ を同じボール $K_\mu$ 上に定義します。次に、$f_1 f_2 : K_\mu \to G$ が分析的で、$(f_1 f_2)(0) = g_1 g_2$ です。一方、$\lambda \in K_\mu$ 全員にとって、

$$
(T_\lambda(f_1 f_2))1 = (T_\lambda f_1)1 \cdot f_2(\lambda) + f_1(\lambda) \cdot (T_\lambda f_2)1 \quad (\S\ 2,\ \text{Proposition 7})
$$
$$
= \alpha(f_1(\lambda)) f_2(\lambda) + f_1(\lambda) \alpha(f_2(\lambda))
$$
$$
= \alpha((f_1 f_2)(\lambda)) \tag{\text{Lemma 1}}
$$

したがって $f_1 f_2 \in \mathscr{F}_{g_1 g_2}$ です。これは、$\mu(g_1 g_2) \geq \inf_{g \in V} (\mu(g_1), \mu(g_2))$ であることを証明します。
(c) 微分可能かつ解析的多様体、R、9.1.4 および 9.1.5 により、$\sigma = \inf_{g \in V} \mu(g) > 0$ となる G の e の近傍 V が存在します。 $h \in G$ と C を接続された成分とします。 $h' \in C$、$\mu(h') \geq \inf(\sigma, \mu(h)) > 0$ はすべて (b) によります。一方、写像 $f_{h'}$ では、$h' \in C$ はC で値を取ります。 Differentiable and Analytic によると、多様体、R、9.1.4 と 9.1.5、C の $\mu = +\infty$、最後に G の $\mu = +\infty$ です。次に、すべての $g \in G$ とすべての $\lambda \in K$ を $f_g(\lambda) = \phi_\lambda(g)$ とします。微分可能かつ解析的多様体、R、9.1.4 および 9.1.5 により、写像 $(\lambda, g) \mapsto \phi_\lambda(g)$ は G 上の K の解析的演算の法則です。明らかに、D が無限小演算の関連する法則である場合、 $D(1) = \alpha$。 (b)により、

$$
\phi_\lambda(g_1 g_2) = \phi_\lambda(g_1) \phi_\lambda(g_2)
$$

すべての$\lambda \in K, g_1 \in G, g_1 \in G$に。

#### 命題 3 {#lie-iii-s10-prop-3 .statement tag=0ALB}

K が超計量であると仮定します。 G をコンパクト・リー群および $\alpha$ を G の無限小自己同型とします。 There exist an open subgroup I of K and a law of analytic operation $(\lambda, g) \mapsto \phi_\lambda(g)$ of I on G with the following properties:
(1) if D is the associated law of infinitesimal operation, then $D(1) = \alpha$;
(2) for all $\lambda \in I, \phi_\lambda \in \mathrm{Aut}\, G$.
As G is compact, there exist an open subgroup I' of K and a law of analytic operation $(\lambda, g) \mapsto \phi_\lambda(g)$ of I' on G with property (1) of the proposition (§ 4, no. 7, Corollary 2 to Theorem 6). $\lambda \in I'$ と $g \in G$ を $\phi_\lambda(g) = f_g(\lambda)$ と書きます。 次に、$G$と$\lambda \in I'$の$g_1, g_2$については、

$$
(T_\lambda(f_{g_1}f_{g_2}))1 = (T_\lambda f_{g_1})1 \cdot f_{g_2}(\lambda) + f_{g_1}(\lambda) \cdot (T_\lambda f_{g_2})1 \\
= \alpha(f_{g_1}(\lambda)) f_{g_2}(\lambda) + f_{g_1}(\lambda) \alpha(f_{g_2}(\lambda)) \\
= \alpha(f_{g_1}(\lambda) f_{g_2}(\lambda))
$$

そして$(f_{g_1}f_{g_2})(0) = g_1 g_2 = f_{g_1g_2}(0)$。したがって、$(g_1', g_2', \lambda)$ に対して $f_{g_1'g_2'}(\lambda) = f_{g_1'}(\lambda) f_{g_2'}(\lambda)$

$(g_1, g_2, 0)$ の近傍 (微分可能および解析多様体、R、9.1.8)。 $G$ はコンパクトなので、すべての $g_1 \in G, g_2 \in G, \lambda \in I$ に対して $f_{g_1g_2}(\lambda) = f_{g_1}(\lambda) f_{g_2}(\lambda)$ となるように、$I'$ の開いた部分群 $I$ が存在します。他には語、$\lambda \in I$には$\phi_\lambda \in \mathrm{Aut}\, G$が入ります。

#### 補題 3 {#lie-iii-s10-lem-3 .statement tag=0ALC}

$G$と$G'$を$G$のリー群と$\phi$準同型を$\mathrm{Aut}(G')$にします。 Let $f(g, g') = (\phi(g))(g')$ for $g \in G, g' \in G'$.次の条件について考えてみましょう。
(i) $f$ is analytic;
(ii) $f$ は $(e_G, e_{G'})$ の近傍で解析的です。
(iii) すべての $g' \in G'$、写像 $g \mapsto f(g, g')$ は分析的です。
次に、(i) $\Leftrightarrow$ ((ii) と (iii)) です。 $G$ が接続されている場合、(i) $\Leftrightarrow$ (ii)。
明らかに (i) は (ii) と (iii) を意味します。 $g_0 \in G, g_0' \in G'$ にしましょう。 For all $g \in G, g' \in G'$,

$$
f(gg_0, g'g_0') = (\phi(g)\phi(g_0))(g'g_0') = \phi(g)(\phi(g_0)g').\phi(g)(\phi(g_0)g_0').
$$

これは、含意 ((ii) と (iii)) $\Rightarrow$ (i) を証明します。最後に、$G'$ が接続されている場合、$e_{G'}$ の近傍ごとに $G'$ が生成されるため、(ii) $\Rightarrow$ (iii) が生成されます。

### 2. 自己同型群/リー群 (実際のケースまたは複雑なケース)

この番号では$K = \mathbf{R}$または$\mathbf{C}$とします。

#### 補題 4 {#lie-iii-s10-lem-4 .statement tag=0ALD}

$H$ を有限次元単純接続リー群とします。
(i) すべての $u \in \mathrm{Aut}\, L(H)$ について、$\theta(u)$ を $L(\theta(u)) = u$ となるような $H$ の一意の自己同型とします。 次に、$(\mathrm{Aut}\, L(H)) \times H$ の $H$ への写像 $(u, g) \mapsto \theta(u)g$ は分析的です。
(ii) $N$ を、$v(N) = N$ となるような、$H$ の嘘部分群と $v \in \mathrm{Aut}\, H$ の$\mathrm{Aut}(H, N)$ 集合とする。 すると、$0^{-1}(\mathrm{Aut}(H, N))$は$\mathrm{Aut}\, L(H)$の嘘部分群になります。
(iii) $N$ が離散かつ正規であるため、$G = H/N$ のリー代数が $L(H)$ と同一視されるとします。 すべての $w \in \mathrm{Aut}\, G$ について、$\eta(w)$ を $L(\eta(w)) = L(w)$ となるような $H$ の一意の自己同型とします。 すると、写像 $\eta$ は、群 $\mathrm{Aut}\, G$ の同型が群 $\mathrm{Aut}(H, N)$ になります。
(i) を証明するには、no. 1 の補題 3 によって、写像 $(u, g) \mapsto \theta(u)g$ が $(\mathrm{Id}_{L(H)}, e)$ の近傍で解析的であることを検証するだけで十分です。 $L(H)$ には 0 の開いた近傍 B が存在し、$\psi = \exp_H|B$ は H の e の開いた近傍に対する B の解析的同型になります。 Aut $L(H)$ には $\mathrm{Id}_{L(H)}$ のオープン近傍 U が存在し、$U(B') \subset B$ のように $L(H)$ には 0 のオープン近傍 $B'$ が存在します。 Then the mapping $(u, g) \mapsto \theta(u)g$ of $U \times \psi(B')$ into H is composed of the following mappings:

$U \times \psi(B')$ の写像 $(u, g) \mapsto (u, \psi^{-1}(g))$ を $U \times B'$ に。
写像 $(u, x) \mapsto u(x)$ の $U \times B'$ を $B$ に。
写像 $y \mapsto \psi(y)$ の $B$ を $G$ にします。

したがって、この写像は分析的です。

$p$ を同次空間 $H/N$ への H の標準写像とします。すると、$\theta^{-1}(\mathrm{Aut}(H, N))$ は $u \in \mathrm{Aut}\ L(H)$ の集合となり、次のようになります。
$$
p(\theta(u)g) = p(e), \quad p(\theta(u^{-1})g) = p(e)
$$
すべての$g \in N$に。 § 8, no. 2、定理 2、系 2 から定理 2 により、これは (ii) を証明します。

N が離散的で正規であると仮定します。 $w \in \mathrm{Aut}\ G$ にしましょう。それから
$$
L(p \circ \eta(w)) = L(\eta(w)) = L(w) = L(w \circ p)
$$
したがって $p \circ \eta(w) = w \circ p$、したがって $\eta(w) \in \mathrm{Aut}(H, N)$ です。明らかに、$\mathrm{Aut}\ G$ の $\mathrm{Aut}(H, N)$ への写像 $\eta$ は単射準同型です。 $p : H \to G$ は水没であるため、この準同型は全射法です。

G を G の局所的にコンパクトな群および $\Gamma$ 自己同型群とします。 位相 $\mathscr{T}_\beta$ が $\Gamma$ (一般位相、章 X, § 3, no. 5) で定義されていることを思い出してください。 これは、$\Gamma$ の $C_c(G; G)$ への写像 $v \mapsto v$ と $v \mapsto v^{-1}$ (コンパクトな収束位相による G への連続写像の空間) が連続する最も粗い位相です。 位相 $\mathscr{T}_\beta$ は、$\Gamma$ の群構造と互換性があります (上記参照)。 G のすべてのコンパクト部分集合 L と G の $e_G$ のすべての近傍 U について、$N(L, U)$ を $\phi \in \Gamma$ の集合とし、すべての $g \in L$ について $\phi(g) \in gU$ と $\phi^{-1}(g) \in gU$ を定義します。次に、$N(L, U)$ 形 $e_\Gamma$ の近傍の基本的な系です。 G がコンパクト部分集合 C によって生成される場合、位相 $\mathscr{T}_\beta$ も最も粗い位相であり、$\Gamma$ から $C_u(C; G)$ までの写像 $v \mapsto v|C$ と $v \mapsto v^{-1}|C$ が連続します (各コンパクト部分集合について) G は十分大きい n の $(C \cup C^{-1})^n$ に含まれます）。 K が局所的にコンパクトで、V が K 上の有限次元ベクトル空間である場合、$\mathbf{GL}(V)$ 上の位相 $\mathscr{T}_\beta$ は通常の位相です。

#### 定理 1 {#lie-iii-s10-thm-1 .statement tag=0ALE}

G を有限次元リー群とし、その恒等式成分を $G_0$ とします。 G が $G_0$ と元の有限数によって生成されるとします。

(i) $\mathrm{Aut}\ G$ 1 つだけのアナリティクス多様体構造満たすには、次の条件が存在します。
(AUT) $\mathrm{Aut}\ G$ へのすべての解析的多様体 M と M のすべての写像 f について、G への $M \times G$ の写像 $(m, g) \mapsto f(m)g$ が解析的である場合に限り、f は解析的です。

主張の残りの部分で Aut G がこれ構造を持っているとします。
(ii) Aut G は有限次元リー群です。
(iii) Aut G の射 $\phi : u \mapsto L(u)$ から Aut L(G) への変換は解析的です。
(iv) G が接続されている場合、$\phi$ は Aut L(G) のライ部分群上のリー群 Aut G の同型です。 G が単純に接続されている場合、この Lie 部分群は Aut L(G) と等しくなります。
(v) $a$ を G の微小自己同型の集合とする。 すると、$a$ は、ベクトル体のリー代数と、(Aut G) $\times$ G の写像 $(u, g) \mapsto u(g)$ に関連付けられた微小演算の法則です。 G へのL(Aut G) の同型です。 $a$へ。
(vi) リー群 Aut G の位相は位相 $\mathscr{T}_\beta$ です。
(a) (i) で検討した分析構造の一意性は明らかです。
(b) G が接続されているとします。 Let H be the universal covering space of G, $p$ the canonical morphism of H onto G and N = Ker $p$. 記法 $\theta$, $\eta$ と補題 4 の Aut(H, N) を紹介します。 私たちは、Aut L(G) の輸送リー群構造を $\theta$ によって Aut H にします。 すると、Aut H は有限次元リー群になり、Aut(H, N) は Aut H の Lie 部分群 (補題 4 (ii)) になります。 $\eta^{-1}$ によって Aut(H, N) を輸送リー群構造から Aut G に変換します。 すると、Aut G は有限次元のリー群になります。 定理の性質 (ii)、(iii)、(iv) が満たされ、(Aut G) $\times$ G から G への写像 $(u, g) \mapsto u(g)$ は解析的です (補題 4 (i))。 M を Aut G への M の多様体、$f$ 写像、および G への M $\times$ G の $\phi$ 写像 $(m, g) \mapsto f(m)g$ とする。 明らかに、$f$ が分析的であれば、$\phi$ も分析的です。 $\phi$ が分析的であると仮定します。 次に、T$\phi$: TM $\times$ TG $\to$ TG は分析的です。したがって、制限から M $\times$ L(G) へ、つまり M $\times$ L(G) から L(G) への写像 $(m, x) \mapsto L(f(m))x$ は解析的です。 L(G) は有限次元であるため、M の写像 $m \mapsto L(f(m))$ を Aut L(G) に変換することは解析的であり、したがって $f$ は解析的であることになります。 したがって、(i) が成り立ちます。

L(G) にノルムを与えます。 すべての $\lambda > 0$ について、B_\lambda を L(G) の中心 0 および半径 $\lambda$ の開球とする。 選ぶ $\lambda > 0$ は、$\psi = \exp_G|_{B_\lambda}$ が G の開部分多様体 $\psi(B_\lambda)$ 上の解析的多様体 B_\lambda の同型となるのに十分小さいです。 $\Phi$ を Aut G のフィルターとします。 Aut G で $\Phi$ が $\mathrm{Id}_G$ に収束するには、Aut L(G) で $L(\Phi)$ が $\mathrm{Id}_{L(G)}$ に収束することが必要かつ十分であり、したがって、$L(\Phi)|_{B_{\lambda/2}}$ と $L(\Phi)^{-1}|_{B_{\lambda/2}}$ は一様に $\mathrm{Id}_{B_{\lambda/2}}$ に収束します。 この条件は、$\Phi|\psi(B_{\lambda/2})$ と $\Phi^{-1}|\psi(B_{\lambda/2})$ が一様に $\mathrm{Id}_{\psi(B_{\lambda/2})}$ に収束することを意味します。 逆に、$\Phi|\psi(B_{\lambda/2})$ が$\mathrm{Id}_{\psi(B_{\lambda/2})}$ に一様に収束するとします。 $u \in M$ であれば $u(\psi(B_{\lambda/2})) \subset \psi(B_{2\lambda/3})$ となるような M $\in \Phi$ が存在します。この場合、L(u)(B_{\lambda/2}) は、L(G) の接続された部分集合であり、$\exp_G$ の下の像は $\psi(B_{2\lambda/3})$ に含まれるため、L(u)(B_{\lambda/2}) は満たされません。 $B_\lambda - B_{2\lambda/3}$ したがって、 L(u)(B_{\lambda/2}) $\subset$ B_\lambda;その場合、仮定 $\Phi|\psi(B_{\lambda/2})$ が $\mathrm{Id}_{\psi(B_{\lambda/2})}$ に一様に収束するということは、$L(\Phi)|_{B_{\lambda/2}}$ が $\mathrm{Id}_{B_{\lambda/2}}$ に一様に収束することを意味します。 すると次のようになります。

$$
(\Phi \text{ converges to } \mathrm{Id}_G \text{ in Aut } G) \iff (\Phi \text{ converges to } \mathrm{Id}_G \text{ under } \mathscr{T}_\beta).
$$

これは (vi) を証明します。

D を、G 上の Aut(G) の左演算の法則に関連付けられた無限小演算の法則とします。 no. 1、$D(L(\text{Aut } G)) = a$ の命題 1 と 2 によって。 したがって、a に対して a はベクトル体のリー代数であり、D は a に対して $L(\text{Aut } G)$ の射です。 $x_1$ と $x_2$ を $L(\text{Aut } G)$ の元とし、$D(x_1) = D(x_2)$ とします。 すると、G 上の演算 $(\lambda, g) \mapsto (\exp \lambda x_1)g$ の法則と K の $(\lambda, g) \mapsto (\exp \lambda x_2)g$ は、無限小演算の同じ関連する法則を持ちます。したがって、$|\lambda|$ が十分に小さい場合、e ($§ 4$、no. 7、定理 6)、よって $\exp \lambda x_1 = \exp \lambda x_2$ の近傍上の$\exp \lambda x_1$ と $\exp \lambda x_2$ 一致するです。 したがって、$x_1 = x_2$ であるため、D は a 上の $L(\text{Aut } G)$ の同型になります。

したがって、定理は G 接続について完全に証明されました。

(c) 一般的なケースに移ります。 仮定により、G は $G_0$ と元 $x_1, x_2, \ldots, x_n$ の有限数によって生成されます。 $u \in \text{Aut } G$ ごとに $G_0$ が安定します。 $\text{Aut}_1 G$ を $u \in \text{Aut } G$ の集合とし、移行から商で、$G/G_0$ の同一性自己同型を与えます。 これは通常の $\text{Aut } G$ の部分群です。 By part (b) of the proof, $\text{Aut } G_0$ has a canonical Lie group structure and the mapping $(g_1, g_2, \ldots, g_n, u) \mapsto (ug_1, ug_2, \ldots, ug_n)$ of $G_0^n \times \text{Aut } G_0$ into $G_0^n$ is analytic. P を $\text{Aut } G_0$ の $G_0^n$ の対応する半直積とします。それは有限次元のリー群 ($§ 1$、no. 4、命題 7) です。

If $w \in \text{Aut}_1 G$, we write
$$
w_0 = w|G_0 \in \text{Aut } G_0 \\
w_i = x_i^{-1}w(x_i) \in G_0 \quad (1 \leq i \leq n) \\
\zeta(w) = ((w_1, \ldots, w_n), w_0) \in P.
$$
For all $w, w'$ in $\text{Aut}_1 G$,
$$
\begin{align*}
\zeta(w)\zeta(w') &= ((w_1, \ldots, w_n)(w_0(w'_1), \ldots, w_0(w'_n)), w_0w'_0) \\
&= ((w_1w_0(w'_1), \ldots, w_nw_0(w'_n)), w_0w'_0) \\
&= ((x^{-1}w(x_1)w(x_1^{-1}w'(x_1)), \ldots, x_n^{-1}w(x_n)w(x_n^{-1}w'(x_n))), w_0w'_0) \\
&= (((ww')_1, \ldots, (ww')_n), (ww')_0) \\
&= \zeta(ww')
\end{align*}
$$
and hence $\zeta$ is a homomorphism of $\text{Aut}_1 G$ into P. This homomorphism is obviously injective.

$\zeta(\text{Aut}_1 G)$ が P で閉じていることを示します。$\Phi$ を、$\zeta(\Phi)$ が P の点 $((w_1, \ldots, w_n), w_0)$ に収束するように、$\text{Aut}_1 G$ のフィルターとします。次に、$\Phi$ は G の写像 v から G に点的に収束します。明らかに、v は の自己準同型です。 群 G. さらに、v は各剰余類 $G_0$ を法として安定し、$v|G_0 = w_0$ を残します。 $v \in \text{Aut}_1 G$ということになります。 $\zeta(v) = ((w_1, \ldots, w_n), w_0)$ として、$\zeta(\text{Aut}_1 G)$ が P で閉じていることを示しました。

(d) 証明の部分 (d) では、$K = \mathbf{R}$ と仮定します。 $§ 8$、no. 2、定理 2、$\zeta(\text{Aut}_1 G)$ は P の嘘部分群です。私たちは $\zeta^{-1}$ によって $\zeta(\text{Aut}_1 G)$ から $\text{Aut}_1 G$ に輸送実リー群構造を行います。したがって、$\text{Aut}_1 G$ は有限次元のリー群になります。

M を Aut_1G への M の解析的多様体, f 写像と M × G の G への φ 写像 (m, g) ↦ f(m)g とします。次の同値があります。

f分析的
⇔ 写像 m: ↦ (f(m))_i、0 ≤ i ≤ n は解析的です
⇔ {M の写像 m ↦ f(m)x_i を G に、1 ≤ i ≤ n の場合、解析的です
そして
写像 (m, g) ↦ M × G_0 を G に変換する f(m)g は解析的です
⇔ φ は解析的です。

w ∈ Aut_1G の場合、L(w) = L(w_0) であるため、Aut_1G の射 w ↦ L(w) から Aut L(G) への変換は解析的です。 We see as in (b) that the law of infinitesimal operation associated with the law of operation of Aut_1G on G is an isomorphism of L(Aut_1G) onto a.

C を G_0 生成する G_0 の圧縮部分集合とします。フィルタ Φ が Aut_1G で $\mathrm{Id}_G$ に収束するには、Φ|(C ∪ {x_1} ∪ ... ∪ {x_n}) と Φ^{-1}|(C ∪ {x_1} ∪ ... ∪ {x_n}) が均一に収束することが必要かつ十分です。

Id_a|(C ∪ {x_1} ∪ ... ∪ {x_n})。

したがって、Aut_1G の位相は位相 $\mathscr{T}_\beta$ です。

明らかに、Aut_1G は位相 $\mathscr{T}_\beta$ の Aut G でオープンしています。この位相と互換性のある Aut G リー群構造が存在し、上記で構築された Aut_1G 構造を誘導します (§ 8, no. 1、系 2 ～ 定理 1)。 リー群 Aut G が定理の特性を持つという事実は、Aut_1G の対応する特性から導き出されます。

(e) 証明の部分 (e) では、K = C と仮定します。 (c) と § 8, no. 2 の定理 2 により、Aut_1G 実リー群構造上には、P の実 Lie 部分群上で ζ が Aut_1G の同型となるようなものが存在します。

The law of operation (w, g) ↦ wg of (Aut_1G) × G on G is real analytic. D を無限小演算に関連付けられた法則とします。 no. 1の命題 1と2により、D(L(Aut_1G)) = a。

すべての α ∈ a について、α_0 が α から G_0 までの制限を表すものとします。それは、L(Aut G_0) の元を持つ証明の部分 (b) により、同一視するとなる G_0 の無限小自己同型です。 1 ≤ i ≤ n の場合、次のように書きます。

$$ \alpha_i = x_i^{-1} \alpha(x_i) \in L(G) = L(G_0). $$

最後に$f(\alpha) = ((\alpha_1, ..., \alpha_n), \alpha_0) \in L(P)$と書きます。この場合、 f は a の L(P) への C 線形写像になります。

一方、明らかに$L(\zeta) = f \circ D$。 したがって、$L(\zeta)(L(Aut_1G)) = f(a)$ は L(P) の複素数ベクトル部分空間です。 § 4, no. 2の命題 2により、$\zeta(Aut_1G)$はPの複素Lie部分群であり、(d)と全く同じように進めることができます。$\zeta(Aut_1G)$上の複素リー群構造を$\zeta^{-1}$によってAut_1Gに輸送すると、(d)のように次のことがわかります。 Aut_1G は、定理の特性 (i)、(ii)、(iii)、(v)、および (vi) に類似した特性を持っています。

明らかに、Aut₁G は位相 $\mathscr{T}_\beta$ の Aut G で開いています。 $w \in \mathrm{Aut}\ G$ にしましょう。 $\sigma$ を Aut₁G の自己同型 $v \mapsto wvw^{-1}$ とします。これは実解析的 ($§ 8$、no. 1、定理 1)、$L(\sigma)$ は $L(\mathrm{Aut}_1 G)$ の $\mathbf{R}$ 自己同型であり、

$$
D \circ L(\mathrm{Aut}_1 G) \circ D^{-1}
$$

は $a$ の $\mathbf{R}$ 自己同型です。 この自己同型は、$w$から構造の輸送によって導出された$a$の自己同型でもあります。 $w$ は K 解析であるため、$L(\sigma)$ は K 線形であることがわかります。 したがって、$\sigma$ は K 解析です ($§ 3$、no. 8、命題 32)。 $§ 1$、no. 9、命題 18 までに、$\mathrm{Aut}_1 G$ が Aut G の開いた嘘部分群であるような、Aut G 上に唯一の Lie K 群構造が存在します。 この構造が定理の特性を持つという事実は、$\mathrm{Aut}_1 G$ の対応するの特性から導き出されます。

#### 系 1 {#lie-iii-s10-thm-1-cor-1 .statement tag=0ALF}

*G を有限次元実リー群とし、$G_0$ その恒等式成分とする。 G が $G_0$ と元の有限数によって生成されるとします。この場合、Aut G は位相 $\mathscr{T}_\beta$ を持ち、有限次元実リー群になります。*

#### 系 2 {#lie-iii-s10-thm-1-cor-2 .statement tag=0ALG}

*G を実数または複素数リー群に接続した半単純とします。 群 Int G は Aut G の正体成分*

写像 $u \mapsto L(u)$ は、Aut $L(G)$ (定理 1) の Lie 部分群に対する Aut G の同型です。この同型の下にある Int G の像は Ad G です。しかし、Ad G は Aut $L(G)$ ($§ 9$, no. 8, 命題 30 (ii)) の同一性成分です。

### 3. 自己同型群/リー群 (ウルトラメトリックケース)

#### 定理 2 {#lie-iii-s10-thm-2 .statement tag=0ALH}

*K が超計量かつ局所的にコンパクトで、G がコンパクト・リー群、主張の場合、定理 1 の (i)、(ii)、(iii)、(v)、(vi) が真になります。*
(a) (i) で検討した分析構造の一意性は明らかです。
(b) G が正規化可能なリー代数 L によって定義されるリー群であると仮定します。次に、G は L のオープン ボールとクローズ ボールです。 $w \in \mathrm{Aut}\ G$ にしましょう。次に、$L(w)$ 一致すると $w$ を 0 の近傍に入れます。$x \in G$ とします。 $p$を剰余体の特徴とします。次に、$n$ が $+\infty$ になる傾向があるように、$p^n x$ は 0 になる傾向があります。したがって、$w(p^n x) = L(w)(p^n x)$ となるような $n$ が存在します。したがって

$$
p^n w(x) = w(x)^{p^n} = w(x^{p^n}) = w(p^n x)
= L(w)(p^n x) = p^n L(w)(x)
$$

よって $w(x) = L(w)(x)$。したがって、$w = L(w)|G$。

$\Gamma$ を $\gamma \in \mathrm{Aut}\ L(G)$ の集合として、$\gamma(G) = G$ とします。 G は $L(G)$ でオープンかつコンパクトであるため、$\Gamma$ は $\mathrm{Aut}\ L(G)$ のオープン部分群です。以上により、Aut G は $\Gamma$、よってと同定され、Aut G にはリー群構造が存在し、定理 1 の性質 (i)、(ii)、(iii)、(vi) が明らかです。 性質 (v) は、no. 1 の命題 1 と 3 から続きます。

(c) 一般的なケースに移ります。 § 7, no. 1, 命題 1 により、(b) で考慮した型である G の開コンパクト部分群 G_0 が存在します。 次に、G は G_0 と元 x_1, x_2, ..., x_n の有限数によって生成されます。 Aut_1G を u ∈ Aut G の集合とし、1 ≤ i ≤ n の場合、u(G_0) = G_0 および u(x_iG_0) = x_iG_0 とします。 定理 1、部分 (c) の証明のように、G_0^n による Aut G_0 の半直接積 P と Aut_1G の単射準同型 ζ を P に変換し、像が P で閉じられているように定義するを作ります。

(d)、(e): 引数は、定理 1 の証明の部分 (d)、(e) とまったく同じです。R は Q_p に置き換えられ、命題 2 の代わりに命題 3 が使用されます。

#### 注意 {#lie-iii-s10-n3-rem-1 .statement tag=0ALI}

K = Q_p で、リー群 G が圧縮部分集合 (cf. 練習問題 2) によって生成される場合、定理 1 の主張 (i)、(ii)、(iii)、(vi) は依然として真ですが、(v) (練習問題 3) は真ではありません。

### 練習問題 {#lie-iii-s10-exercises}

[§ 10 に対して練習問題](exercises/s10/)を参照してください。
