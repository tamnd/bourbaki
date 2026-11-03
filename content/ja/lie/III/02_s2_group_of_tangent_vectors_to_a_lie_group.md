---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 2
section_title: Group of tangent vectors to a Lie group
lang: ja
source: lie-i-iii
book_pages: 233-238
pdf_pages: 0251-0256
extraction: ocr
subsections:
    - "no": 1
      title: TANGENT LAWS OF COMPOSITION
      page: 233
      pdf_page: 251
    - "no": 2
      title: GROUP OF TANGENT VECTORS TO A LIE GROUP
      page: 235
      pdf_page: 253
    - "no": 3
      title: CASE OF GROUP GERMS
      page: 237
      pdf_page: 255
statements: 10
exercises: 0
content_sha256: 0428c0fa5c45770f666ac38ab604fe0d451ec659dcea78eec6e4a61151189fae
translated_from: content/en/lie/III/02_s2_group_of_tangent_vectors_to_a_lie_group.md
translation_method: google
source_content_sha256: 9312e1a966f1c5bc60ded7611d1345461f06db492fc343d729b16bcbbd46a1c0
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: 1bdb78b112e2e48a785df31836f745f2d1213df76d1f29299409d2629c453cb4
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 2。 ベクトルからリー群までの接線群

### 1. 接線法則/合成

X と Y を類 C^r の多様体とします。 X \times Y は類 C^r の多様体であり、接線の写像 (T(pr_1), T(pr_2))、積であることがわかっています (微分可能および解析多様体、R、8.1.4)。 写像を正規の射影にすると、類の同型は、T(X \times Y) の T(X) \times T(Y) 上の C^{r-1} です。\footnote{r = 1 の場合、これは (T(pr_1), T(pr_2)) は、T(X) \times T(Y) 上の T(X \times Y) の準同型です。} この同型は、基底空間 X \times Y を含むベクトルバンドル構造と互換性があり、これを許可します。 同一視する T(X \times Y) と T(X) \times T(Y) です。 a ∈ X, b ∈ Y, u ∈ T_a(X), v ∈ T_b(Y) とします。上記の識別により、(u, v) を T_{(a, b)}(X × Y) の元とみなすことができます。それから

$$(u, v) = (u, 0) + (0, v)$$

そして (u, 0) (それぞれ (0, v)) は、X (それぞれ Y) のX × Y への浸漬 x ↦ (x, b) (それぞれ y ↦ (a, y)) の接線写像の下にある u (それぞれ v) の像です。正確にする必要がある場合は、次のように書きます。 T_a(x) の零元には 0_a。

Now let X, Y, Z be manifolds of class C^r and f a mapping of class C^r of X × Y into Z. 接線写像は、上記の同定を使用すると、T(X) × T(Y) の類 C^{r-1} の写像を T(Z) に変換したものになります。 u ∈ T_a(X) および v ∈ T_b(Y) の場合、

(1)
$$T(f)(u, v) = T(f)(u, 0_b) + T(f)(0_a, v),$$
(2)
$$T(f)(0_a, 0_b) = 0_{f(a, b)}.$$

一方、写像 y ↦ f(a, y) は、浸漬 y ↦ (a, y) と f の合成です。それは次のとおりです

(3) $T(f)(0, v)$ は、$y \mapsto f(a, y)$ への接線写像の下にある v の像です。

同様に

(4) $T(f)(u, 0)$ は、$x \mapsto f(x, b)$ への接線写像の下にある u の像です。

X × Y の Z への写像 f を (x, y) ↦ xy で表すと、u ∈ T(X), v ∈ T(Y) の元 T(f)(u, v) を表すために uv がよく使われます。

X を類 C^r の多様体とし、m: X × X → X 合成の類 C^r の X の法則とします。すると、T(m) は T(X) 上の類 C^{r-1} の法則 of 合成です。 mに接する合成の法則と呼ばれます。 X への T(X) の標準射影 p は、法則 m および T(m) と互換性があります。他の語では、

(5)
$$p \circ T(m) = m \circ (p \times p).$$

(2) から次のことがわかります。

(6)
$$T(m)(0_x, 0_y) = 0_{m(x, y)}$$

X のすべての x、y について;その他の語、零、切断、$x \mapsto 0_x$のT(X)は法則m、T(m)と互換性があります。

#### 命題 1 {#lie-iii-s2-prop-1 .statement tag=0A8Y}

*X を類 C^r の多様体とし、X の類 C^r の合成の m 法則とします。 m が結合性 (または可換性) の場合、T(m) は結合性 (または可換性) です。*

m が結合の場合、$m \circ (m \times \mathrm{Id}_X) = m \circ (\mathrm{Id}_X \times m)$、よって

$$T(m) \circ (T(m) \times \mathrm{Id}_{T(X)}) = T(m) \circ (\mathrm{Id}_{T(X)} \times T(m))$$

したがって、$T(m)$ は結合します。 $s$ を $X \times X$ の写像 $(x, y) \mapsto (y, x)$ を $X \times X$ にします。 $m$ が可換である場合、$m \circ s = m$ となり、したがって

$$
T(m) \circ T(s) = T(m).
$$

ただし、$T(s)$ は $T(X) \times T(X)$ の写像 $(u, v) \mapsto (v, u)$ が $T(X) \times T(X)$ になります。したがって、$T(m)$ は可換です。

#### 命題 2 {#lie-iii-s2-prop-2 .statement tag=0A8Z}

*$X$ を類 $C^r$ の多様体、$m$ 法則の合成 、類 $C^r$ の $X$ および$e$ 単位元とします。 $m$。

(i) *The vector $0_e$ is an identity element for $T(m)$.
(ii) *$T_e(X)$ is stable under $T(m)$ and the law of composition induced on $T_e(X)$ by $T(m)$ is the vector space addition on $T_e(X)$.
(iii) *Let $U$ be an open subset of $X$ and $\alpha$ a mapping of class $C^r$ of $U$ into $X$ such that, for all $x \in U$, $\alpha(x)$ is the inverse of $x$ under $m$. 次に、すべての $u \in T(U)$ について、$T(\alpha)u$ は $T(m)$ の下の $u$ の逆数になります。

性質 (3) と (4) は、すべての $u \in T(X)$、よって (i) について $T(m)(0_e, u) = T(m)(u, 0_e) = u$ であることを示しています。 $T_e(X)$の$u, v$については、

$$
T(m)(u, v) = T(m)(u, 0_e) + T(m)(0_e, v) = u + v,
$$

よって (ii)。最後に、すべての $x \in U$ に対して関係 $m(x, \alpha(x)) = m(\alpha(x), x) = e$ が暗示されます。

$$
T(m)(u, T(\alpha)(u)) = T(m)(T(\alpha)u, u) = 0_e
$$

すべての $u \in T(U)$、よって (iii)。

#### 命題 3 {#lie-iii-s2-prop-3 .statement tag=0A90}

*Let $X_1, X_2, \ldots, X_p, Y$ be manifolds of class $C^r$, $i$ an integer of $\{1, p\}$, $m_i$ (resp. $n$) a law of composition of class $C^r$ on $X_i$ (resp. $Y$) and $u$ a mapping of class $C^r$ of $X_1 \times X_2 \times \cdots \times X_p$ into $Y$. $u$ が添字 $i$ の変数に対して分配的である場合、$T(u)$ は添字 $i$ の変数に対して分配的です。

証明は命題 1 と類似しています。

### 2. ベクトルからリー群までの接線群

#### 命題 4 {#lie-iii-s2-prop-4 .statement tag=0A91}

※$G$をリー群とします。すると、$T(G)$は、$G$の乗法に合成の法則が接するので、リー群になります。 $T(G)$の単位元はベクトル$0_e$です。

これは命題 1 と 2 から続きます。

#### 命題 5 {#lie-iii-s2-prop-5 .statement tag=0A92}

※$G$と$H$を$G$のリー群と$f$射を$H$にします。すると、$T(f)$ はリー群 $T(G)$ の射がリー群 $T(H)$ になります。

$T(f')$ が分析的であることはわかっています。一方、$m$ (それぞれ $n$) が $G$ (それぞれ $H$) の乗法を表すものとします。次に、$f \circ m = n \circ (f \times f)$、よって

$$
T(f) \circ T(m) = T(n) \circ (T(f) \times T(f)),
$$

これは$T(f)$が群準同型であるという事実を表します。

#### 系 {#lie-iii-s2-n2-cor-1 .statement tag=0A93}

※$G_1, \ldots, G_n$をリー群とします。 多様体 $T(G_1 \times \cdots \times G_n)$ の多様体 $T(G_1) \times \cdots \times T(G_n)$ への標準同型はリー群同型です。*

$\mathrm{pr}_i$ は $G_1 \times \cdots \times G_n$ の射から $G_i$ になり、したがって $T(\mathrm{pr}_i)$ は $T(G_1 \times \cdots \times G_n)$ の射から $T(G_i)$ になります。

#### 命題 6 {#lie-iii-s2-prop-6 .statement tag=0A94}

*$G$をリー群とします。*
  (i) *正規の射影 $p : T(G) \to G$ はリー群射です。*
  (ii) *$p$の核は$T_e(G)$です。 それは$T(G)$の嘘部分群です。 $T(G)$ の結果によって $T_e(G)$ に誘発されたリー群構造は、完全正規数空間 $T_e(G)$ のリー群構造です。*
  (iii) *零切断 $s$ は、リー群の同型 $G$ が、$T(G)$ の部分群 $s(G)$ (これを部分群同一視するとします) $G$).*
  (iv) *リー群 $T(G)$ は、$T_e(G)$ による $G$ の半直接積です。

主張 (i) は (5) から続きます。 主張 (ii) は、命題 2 (ii) を考慮すると明らかです。 主張 (iii) と (iv) は (6) と § 1、命題 8 から続きます。

$u \in T(G)$ と $g \in G$ としましょう。 (3)と(4)により、群$T(G)$で計算された積$ug, gu$は、$T(\delta(g^{-1}))$と$T(\gamma(g))$の下の$u$の像になります。 It follows from § 1, Corollary 2 to Proposition 17 that the mapping $(g, u) \mapsto gu$ of $G \times T_e(G)$ into $T(G)$ is an isomorphism of the trivial vector bundle $G \times T_e(G)$ with base space $G$ onto the vector bundle $T(G)$. 逆同型は、$T(G)$ の *左矮化* と呼ばれます。 写像 $(g, u) \mapsto ug$ を考慮すると、$T(G)$ の *正しい矮小化* も同様に定義されます。

#### 命題 7 {#lie-iii-s2-prop-7 .statement tag=0A95}

*$G$ をリー群、$M$ 多様体の類 $C^r$ と $f$ および $g$ 写像の類 $C^r$ の $M$ とします$G$なので、$fg$は類の写像、$M$の$C^r$が$G$になります。 $m \in M, x = f(m), y = g(m), u \in T_m(M)$ にしましょう。それから*

$$
(T fg)u = T(f)u.y + x.T(g)u.
$$

$m$ を $G$ の乗法とします。次に$fg = m \circ (f, g)$。今

$$
T(f, g)(u) = (T(f)u, T(g)u),
$$

したがって $T(fg)u = T(f)u.T(g)u$ です。次に、$f$ を $m$ に置き換えて (1) を適用するだけで十分です。

#### 系 {#lie-iii-s2-n2-cor-2 .statement tag=0A96}

*$n \in \mathbf{Z}$にしておきます。 $G$の$G$への$e$から写像$g \mapsto g^n$への接線写像は、$T_e(G)$の$x \mapsto nx$から$T_e(G)$への写像です。

$n \geqslant 0$ の場合、命題 7 から $n$ に帰納法が続きます。一方、$e$ から写像 $g \mapsto g^{-1}$ までの接線写像は、写像 $x \mapsto -x$ (no. 1, 命題 2）。

G を類 C^r のリー群, X 多様体と、X 上の G の左演算の類 C^r の (g, x) \mapsto gx 法則とします。 命題 1 について議論して、T(X) 上の T(G) の類 C^{r-1} の左演算の法則を導出します。これも (u, v) \mapsto uv で表します。 G (それぞれ X) を T(G) の零切断 (それぞれ T(X)) の像と識別すると、(6) により、T(X) 拡大するの T(G) の左演算の法則がわかります。 XのGの左法則演算。 すべての u \in T_g(G) と v \in T_x(X) について、(1) により、

$$
uv = gv + ux.
$$

g \in G および v \in T_x(X) の場合、gv は、(3) により、x での接線写像の下にある v の像を写像 y \mapsto gy X を X に変換します。この接線写像は、T_x(X)のT_{gx}(X)への同型です。特に、

$$
g(v + v') = gv + gv', \quad g(\lambda v) = \lambda(gv) \quad \text{for } v, v' \text{ in } T_x(X), \lambda \in K.
$$

x \in X と u \in T_g(G) の場合、ux は (4) g での接線写像の下にある u の像を写像 h \mapsto hx G から X に変換します。したがって、

$$
(u + u')x = ux + u'x, \quad (\lambda u)x = \lambda(ux) \quad \text{for } u, u' \text{ in } T_g(G), \lambda \in K.
$$

上記は、リー群が左 (または右) 変換によってそれ自体で動作する場合に適用できます。 T(G) 上の T(G) の演算の対応する法則は、リー群 T(G) の左 (右) 変換によって定義されます。したがって、式 (7)、(8)、および (9) は T(G) で有効です。

#### 命題 8 {#lie-iii-s2-prop-8 .statement tag=0A97}

G_1 と G_2 をリー群、X_i (i = 1, 2) 上の G_i の類 C^r の左演算の類 C^r の X_1 と X_2 多様体を f_i 法則とします。 \phi を G_1 から G_2 への射とし、\psi を X_1 から X_2 への \phi 射影とします。したがって、T(\psi) は、T(X_1) から T(X_2) への T(\phi) 射です。

f_2 \circ (\phi \times \psi) = \psi \circ f_1, よって

$$
T(f_2) \circ (T(\phi) \times T(\psi)) = T(\psi) \circ T(f_1).
$$

G を類 C^r のリー群, X 多様体と、X 上の G の左演算の類 C^r の (g, x) \mapsto gx 法則とします。 I を K 含む 0 の開部分集合とし、 \gamma: 類 C^r の I \to G 写像を \gamma(0) = e とします。させて

$$
a = T_0(\gamma)1 \in T_e(G).
$$

x \in X とします。 (4) を使用すると、ax は接線写像から \lambda \mapsto \gamma(\lambda)x までの接線ベクトル 1 から 0 での I までの像です。 したがって *ベクトル体* x \mapsto ax on X * はベクトル体は、写像* (\lambda, x) \mapsto \gamma(\lambda)x *微分可能および解析的という意味で、多様体*、R、8.4.5 によって定義されます。

### 3. 群細菌の場合

(G, e, \theta, m) をリー群胚芽、\Omega を m の定義の集合とします。次に、T(\Omega) は T(G) \time T(G) のオープン部分集合で識別され、T(m) は $T(\Omega)$ から $T(G)$ への解析写像です。 no. 2 と同様に、$(T(G), 0_e, T(\theta), T(m))$ がリー群細菌であることが確認できます。 $G$ と $T(G)$ の積は、乗算的に書かれることがよくあります。 $T(G)$ の $G$ に対する正規の射影は、リー群細菌の射です。 $T_e(m)$から$T_e(G)$の制限は、$T_e(G)$のベクトル空間加法です。 $T(G)$の零切断は、$T(G)$の嘘部分群細菌の上にリー群細菌$G$の同型が$G$と同一視するを掛けたものです。 $f$が$G$の射をリー群の細菌$H$にすると、$T(f): T(G) \to T(H)$はリー群の細菌の射になります。

$G \times T_e(G)$ の $T(G)$ への写像 $\phi: (g, u) \mapsto gu$ は、自明なベクトルバンドル $G \times T_e(G)$ の同型と基底空間 $G$ のベクトルバンドル $T(G)$ です。 for $\phi$ と $\phi^{-1}$ は解析的であり、ベクトルバンドル射であるため、*Differentiable and Analytic 多様体*、R、7.2.1 を適用するだけで十分です。 (no. 2 の証明も適応可能です。) 同型 $\phi^{-1}$ は、$T(G)$ の左の矮小化と呼ばれます。 写像 $(g, u) \mapsto ug$ の逆同型は右矮化と呼ばれます。

Let $X$ be a manifold of class $C^r$ and $\psi$ a law chunk of left operation of class $C^r$ of $G$ on $X$. Then $T(\psi)$ is a law chunk of left operation of class $C^{r-1}$ of $T(G)$ on $T(X)$ extending $\psi$. 式 (7)、(8)、(9) は、$gx$ が定義されている場合でも有効です。 $I$ が $K$ 含む 0 のオープン部分集合である場合、$\gamma: I \to G$ が類 $C^r$ の写像である場合、$\gamma(0) = e$ であり、$a = T_0(\gamma)1$ の場合、ベクトル体 $X$ で定義された $x \mapsto ax$ は、*微分可能かつ解析的多様体*、R、8.4.5 の意味で、写像 $(\lambda, x) \mapsto \gamma(\lambda)x$ によって定義されたベクトル体です。
