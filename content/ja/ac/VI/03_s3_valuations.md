---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 3
section_title: Valuations
lang: ja
source: ac-i-vii
book_pages: 385-393, 446-449
pdf_pages: 0403-0411, 0464-0467
extraction: ocr
subsections:
    - "no": 1
      title: VALUATIONS ON A RING
      page: 385
      pdf_page: 403
    - "no": 2
      title: VALUATIONS ON A FIELD
      page: 387
      pdf_page: 405
    - "no": 3
      title: TRANSLATIONS
      page: 389
      pdf_page: 407
    - "no": 4
      title: EXAMPLES OF VALUATIONS
      page: 389
      pdf_page: 407
    - "no": 5
      title: IDEALS OF A VALUATION RING
      page: 391
      pdf_page: 409
    - "no": 6
      title: DISCRETE VALUATIONS
      page: 392
      pdf_page: 410
statements: 15
exercises: 8
content_sha256: 60cc27798d7e2fe9127f966d239e7d5dabcaea0b648d76c2ec271db89268150a
translated_from: content/en/ac/VI/03_s3_valuations.md
translation_method: google
source_content_sha256: 53da8eeb6a8932911f9fa4e5bb93b698a2373f5f22e0893d102d4323fd2301f1
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: d3c8689a595548b7679e4ca460d7ff94c4adae72532f9a65ddbab247e1611baa
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 3. 評価

### 1. 環の評価

$\Gamma$ を加法的に書かれた完全順序可換群とします。この章の残りの部分では、$+\infty;$で示される$\Gamma$元に隣接して得られる群、集合について、これを集合を$\Gamma_\infty$で表し、次のように与えます。 $+\infty$ は最大の元で、他の語では、すべての $a \in \Gamma;$ に対して $a < +\infty$ になります (2) $\Gamma$ 上の法則誘導するが指定された群法則である可換モノイド構造式で定義されます

$$
(+\infty) + (+\infty) = +\infty, \quad a + (+\infty) = +\infty
$$

for all $\alpha \in \Gamma$; it is immediately verified that this law is associative and commutative and that the relation $\alpha_1 \leq \beta$ in $\Gamma_\infty$ implies $\alpha_1 + \gamma \leq \beta + \gamma$ for all $\gamma \in \Gamma_a$.

#### 定義 1 {#ac-vi-s3-def-1 .statement tag=04T2}

*$C$ を (必ずしも可換であるとは限らない) 環とし、$\Gamma$ を加法的に書かれた完全に順序付けられた可換群とします。 $\Gamma$ の値を含む $C$ の評価は、以下の条件を満たす任意の写像 $v : C \to \Gamma_\infty$ です:*

(VL_I) $v(xy) = v(x) + v(y)$ は $x \in C, y \in C$ です。
(VL_{II}) $v(x + y) \geq \inf(v(x), v(y))$ は $x \in C, y \in C$ です。
(VL_{III}) $v(1) = 0$ と $v(0) = +\infty$。

If $C$ has no divisor of zero other than 0, the unique mapping $v_0$ of $C$ to $\Gamma_\infty$ such that $v_0(x) = 0$ for $x \neq 0$ and $v_0(0) = +\infty$ is a valuation, called the *improper valuation* on $C$. If $z \in C$ is such that $z^n = 1$ for some integer $n \geq 1$, then, by (VL_I), $nv(z) = v(z^n) = 0$ and hence $v(z) = 0$ for *every* valuation $v$ on $C$, since $\Gamma$ is a totally ordered group. 特に $v(-1) = 0$、よって $v(-x) = v(x)$ はすべての $x \in C$ に対してです。 さらに、(VL_I) から、$C$ のすべての $x, y$ に対して $v(xy) = v(yx)$ が得られます。 $x$ が $C$ で反転可能な場合、$v(x^{-1}) = -v(x)$ になります。

#### 命題 1 {#ac-vi-s3-prop-1 .statement tag=04T3}

*$v$ を (必ずしも可換ではない) 環 $C$ の評価とします。 元 $x_i \in C$ ($1 \leq i \leq n$) の場合、*

$$
v \left( \sum_{i=1}^n x_i \right) \geq \inf_{1 \leq i \leq n} v(x_i)
$$

さらに、$v(x_k) = \inf_{1 \leq i \leq n} v(x_i)$ となる添字 $k$ が 1 つ存在する場合、(1) の両辺は等しい。特に、$v(x) \neq v(y)$ の場合は、$v(x + y) = \inf(v(x), v(y))$ になります。

関係 (1) は、$n$ 上の帰納法による公理 (VL_{II}) から導き出されます。 $v(x_k) = \inf_{1 \leq i \leq n} v(x_i)$ となる 1 つの添字 $k$ が存在する場合、(1) で $y = \sum_{i \neq k} x_i$ と $z = \sum_{i=1}^n x_i$、$v(y) > v(x_k)$ と $v(z) \geq v(x_k)$ を書きます。 $v(z) > v(x_k)$, 関係 $x_k = z - y$ は $v(x_k) \geq \inf(v(z), v(y)) > v(x_k)$ になりますが、これは不合理です。 よって $v(z) = v(x_k)$、これは 2 番目の主張を証明します。

#### 系 {#ac-vi-s3-n1-cor-1 .statement tag=04T4}

*If a finite sequence of elements $(x_i)_{1 \leq i \leq n}$ of $C$ (for $n \geq 2$) is such that $\sum_{i=1}^n x_i = 0$, there exist at least two distinct indices $j, k$ such that*

$$
v(x_j) = v(x_k) = \inf_{1 \leq i \leq n} v(x_i).
$$

$v(x_k) = \inf_{1 \leq i \leq n} v(x_i)$、命題 1 のような添字 $k$ が 1 つだけある場合、関係 $n \geq 2$ および仮定とは反対に、すべての $i$ に対して $v(x_k) = v(0) = +\infty$、よって $v(x_i) = +\infty$ が示されます。 $k$。

注意
(1) $v : C \to \Gamma_\infty$ が環 $B$ から $C$ の $C$ と $u : B \to C$ 準同型の評価である場合、複合写像 $B \xrightarrow{u} C \xrightarrow{v} \Gamma_\infty$ の評価は明らかです$\Gamma$に値が入った$B$。

(2) Conditions (VL$_I$) and (VL$_II$) show immediately that the set $\bar{v}^{-1}(+\infty)$ is a two-sided ideal $\mathfrak{p}$ in $C$ distinct from $C$ by virtue of (VL$_III$); moreover, if $x, y$ are two elements of $C$ such that $v(xy) = +\infty$, it follows from (VL,) that necessarily $v(x) = +\infty$ or $v(y) = +\infty$; in other words, the quotient ring $C/\mathfrak{p}$ has no divisor of 0 other than 0; it is immediately verified that the mapping $\bar{v} : C/\mathfrak{p} \to \Gamma_\infty$ derived from $v$ by passing to the quotient is a valuation on $C/\mathfrak{p}$, the inverse image of $+\infty$ under this valuation reducing to 0.

### 2. 体の評価

#### 命題 2 {#ac-vi-s3-prop-2 .statement tag=04T5}

$K$ を (必ずしも可換ではない) 体とし、$v$ を $\Gamma$ の値による $K$ の評価とします。 Then:
(i) For $x \neq 0$, $v(x) \neq +\infty$.
(ii) The set $A$ of $x \in K$ such that $v(x) \geq O$ is a subring of $K$.
(iii) For all $a \geq O$ in $\Gamma$, the set $V$, (resp. $V'_a$) of $x \in A$ such that $v(x) > a$ (resp. $v(x) \geq a$) is a two-sided ideal of $A$ and every (left or right) ideal $\neq (O)$ of $A$ contains $m$ of the $V'_a$.
(iv) The set $m(A)$ of $x \in A$ such that $v(x) > O$ is the greatest ideal $\#A$ in $A$; $U(A) = A - m(A)$ is the set of invertible elements of $A$ and $\kappa(A) := A/m(A)$ is a (not necessarily commutative) field.
(v) For all $x \in K - A$, $x^{-1} \in m(A)$.

主張 (i) は、$\bar{v}^{-1}(+\infty)$ が $K$ に等しくない $K$ の理想であるという事実から導き出されます。 $A$ が環であり、$V$ および $V'_a$ の両面理想であるという事実の検証は、公理 (VL$_I$)、(VL$_II$)、および (VL$_III$) のおかげで自明です。 $a$ が $A$ と $x \neq 0$ 属するから $A$ までの (たとえば左の) 理想である場合、$v(y) \geq v(x)$ となるすべての $y \in A$ は $y = zx$ と書くことができます。ここで、$z = yx^{-1}$ であるため、$v(z) = v(y) - v(x) \geq O$ となり、したがって$z \in A$;他の語の左理想 $Ax$ 含むでは $a > v(x)$ の $V'_a$ です。 集合 $U(A) = A - m(A)$ は $x \in K$ の集合で、$v(x) = 0$ になります。 $x \in U(A)$ の場合、
$$
v(x^{-1}) = -v(x) = 0,
$$
よって $x^{-1} \in U(A)$;逆に、$y \in A$ が $A$ で可逆であれば、$v(y) \geq 0$、$v(y^{-1}) \geq 0$、$v(y) + v(y^{-1}) = 0$、よって、$v(y) = 0$、$y \in U(A)$ になります。これは (iv) を証明し、(v) は定義からすぐに続きます。

$A$ (それぞれ $m(A)$、$\kappa(A)$) は、$K$ での評価 $v$ の環 (それぞれ理想、剰余体) と呼ばれます。

明らかに、U(A) は準同型 $v : K^* \to \Gamma$ の核および乗法群 $K^*$ の $v$ の下の像 $v(K^*)$ は加法群 $\Gamma$ の部分群です。 $v$ の位数群または値群は、$K^*/U(A)$ と同型です。 $x \in K$、元 $\Gamma_\infty$ の $v(x)$ は評価額と呼ばれるときどき 、$v$ の $x$ の位数です。 $K$ の 2 つの評価 $v, v'$ が同じ環を持っている場合、それらは同等と呼ばれます。

#### 命題 3 {#ac-vi-s3-prop-3 .statement tag=04T6}

* (必ずしも可換ではない) 体 $K$ に対する 2 つの評価 $v, v'$ が同等であるためには、順序付けられた群 $v'(K^*)$ に順序付けられた群 $v(K^*)$ の同型 $\lambda$ が存在することが必要かつ十分です。それ $v' = A \circ v$.*

Suppose $v$ and $v'$ are equivalent; by hypothesis, the ring $A$ of the valuation $v$ being the same as that of $v'$, $v$ and $v'$ (restricted to $K^*$) factor into homomorphisms $K^* \to K^*/U(A) \xrightarrow{\mu} v(K^*)$, $K^* \to K^*/U(A) \xrightarrow{\nu} v'(K^*)$, where $\mu$ and $\nu$ are isomorphisms; moreover, the set of positive elements of $v(K^*)$ (resp. $v'(K^*)$) is the image under $\mu$ (resp. $\nu$) of the set of classes mod. $U(A)$ of elements $\neq 0$ of $m(A)$; we conclude that $A = v \circ \mu^{-1}$ solves the problem, the converse being obvious.

ここで、$K$ が可換体であると仮定します。その場合、$K$、環、$A$ の評価$v$ のすべての評価$v$ は、§ 1, no. 2、定義 2 の意味での $K$ の評価環になります (これは用語を正当化します)。これは、命題 2 (c) および § 1 no. 2、定理 1 (c) の直後に続きます。 *Conversely*, recall that for every integral domain $B$ whose field of fractions is $K$ the relation of divisibility $x|y$ (equivalent to $y \in Bx$) makes $K^*$ into a preordered group, whose *associated ordered group* $\Gamma_B$ is the quotient $K^*/U(B)$ of $K^*$ by the group $U(B)$ of invertible elements of $B$, the positive elements of this group being those of $B^*/U(B)$ (where $B^* = B - \{0\}$); the mapping $x \mapsto Bx$ defines, by passing to the quotient, an isomorphism of the ordered group $K^*/U(B)$ onto the group (ordered by the relation $\supset$) of non-zero principal fractional ideals of $K$ (*Algebra*, Chapter VI, § 1, no. 5). 分数 $K$ の体を伴う環 $A$ と、群 $\Gamma_A = K^*/U(A)$ が *完全に順序付けられている* は、正確に K* の *評価環 (§ 1, no. 2, 定理 1 (d)) です。 $v_A$ が $\Gamma_A$ に対する $K^*$ の標準準同型を表す場合、$v_A$ ($v_A(0) = +\infty$ で拡張) が環が $A$ である$K$ での評価 (*正規* と呼ばれる) であるのは明らかです。 $v_A$に相当するすべての評価は$v = \sigma \circ v_A$と書くことができます。ここで、$\sigma$は$\Gamma_A$の同型を群の部分群に加え、$v$はその値（命題3）をとります。 $\sigma \circ v_A$ は、$v$ の *正準因数分解* と呼ばれます。

#### 命題 4 {#ac-vi-s3-prop-4 .statement tag=04T7}

*$C$を整域、$K$を分数の体、$C^* = C - \{0\}$、$v : C \to \Gamma_\infty$を$C$での評価とします。次に、$K$ には固有の評価 $w$ が存在します。これは、拡大する $v$ と $w(K^*)$ は、$v(C^*)$ によって生成された $\Gamma$ の部分群です。

*代数*、章 I, § 2, no. 7 の定理 2 により、$K^*$ から $\Gamma$ まで一意な準同型 $w$ が存在し、拡大する $v|C^*$ と $w(K^*)$ が生成されます。 $v(C^*)$。 $w$ が公理 (VL$_{\text{II}}$) を満たすことを証明する必要があります。次に、$x' \in K^*, y \in K^*$ を $x + y \in K^*$ となるようにします。 $ax \in \mathbf{C}^*$ と $ay \in \mathbf{C}^*$、よって $a(x + y) \in \mathbf{C}^*$ のような $a \in \mathbf{C}^*$ が存在します。 $w$から$\mathbf{C}^*$の制限は(VL$_{\text{II}}$)を満たすので、

$$
w(a(x + y)) \geq \inf(w(ax), w(ay)).
$$

両辺から $w(a)$ を消去すると、次のようになります。

$$
w(x + y) \geq \inf(w(x), w(y)).
$$

### 3. 翻訳

$K$ を (可換) 体、$f$ を $K$ の場所、$v$ を $K$ の評価、$A$ を $K$ の評価環とします。 $A$が$f$の環、および$v$の環である場合、$A, f$と$v$は*関連付けられている*と言えます。 no. 1 と § 2, no. 3 により、3 つのオブジェクト $A$、$f$、$v$ がそれぞれ、次に他の 2 つが決定する (場所と評価に関する限り、同値まで) になります。特に次の同値があります。

$$
\begin{array}{lllll}
x \in A & \Leftrightarrow & f(x) \neq \infty \\
x \in m(A) & \Leftrightarrow & f(x) = 0 \\
x \in A - m(A) = U(A) & \Leftrightarrow & f(x) \neq 0 \quad \text{and} \quad f(x) \neq \infty \Leftrightarrow v(x) = 0 \\
x \in K - A & \Leftrightarrow & f(x) = \infty & \Leftrightarrow & v(x) < 0
\end{array}
$$

評価環、場所、または評価に関するすべての結果は、他の 2 つの結果概念に変換できます。したがって、命題 4 of § 2, no. 4 は次のようになります。

#### 命題 5 {#ac-vi-s3-prop-5 .statement tag=04T8}

*$K$を体、$v$を$K$と$K$の$K'$拡大の評価とします。 $K'$ には $v'$ という評価が存在します。その制限から $K$ は $v$ に相当します。*

$\Gamma_v$ と $\Gamma_{v'}$ を $v$ と $v'$ の位数群とします。 Since the restriction of $v'$ to $K$ is equivalent to $v$, there exists an isomorphism $A$ of $\Gamma_v$ onto a subgroup of $\Gamma_{v'}$, such that $v' = A \circ v$ on $K$. $\Gamma_v$ を $\lambda$ によって $\lambda(\Gamma_v)$ と同一視すると、 $v'$ 拡大する $v$ であることがわかります。

$\Gamma_{v'}$ は一般に $\lambda(\Gamma_v)$ とは *区別* され、$v'$ の同値類は必ずしも一意ではないことに注意してください。これについては§ 8で*戻ります*。

§ 1, no. 3 の定理 3 (または § 2, no. 5 の命題 6) を翻訳すると、次のようになります。

#### 命題 6 {#ac-vi-s3-prop-6 .statement tag=04T9}

*$K$を体、$K$の$A$部分環、$K$の$x$元とします。 $x$が$A$に対して整数であるためには、$A$ではプラスである$K$のすべての評価が$x$ではプラスであることが必要かつ十分です。*

これ以降、上記と同様の翻訳を実行する手間は通常、読者に任せることにします。

### 4. 評価額の例

§ 1, no. 4 で与えられた評価環の例について、以下の *例 1 ～ 4* を提供してください。

#### 例 (1) {#ac-vi-s3-n4-exa-1 .statement tag=04TA}

F* のすべての元は根単位元であるため、有限体 F のすべての評価は不適切です。

#### 例 (2) {#ac-vi-s3-n4-exa-2 .statement tag=04TB}

K が体 K' の部分体である場合、K' の評価額の K に対する制限は、K の評価額です。

#### 例 (3) {#ac-vi-s3-n4-exa-3 .statement tag=04TC}

k を体とし、K = k((T)) とします。 写像 v 写像のすべての非ゼロ形式冪系列から位数 (代数, 章 IV, § 5, no. 7) は、位数群が Z であり、環がk[[T]]。関連する場所は標準準同型 f: k[[T]] → k を設定 f(u) = ∞ if u ∉ k[[T]] によって k((T)) に拡張します。

#### 例 (4) {#ac-vi-s3-n4-exa-4 .statement tag=04TD}

A を主イデアル整域、K を分数の体、p を A の極値元とします。 x ∈ K* の場合、v_p(x) は x の分解における p の指数を極値元 (代数, 章 VII, § 1, no. 3, 定理 2) として表します。 v_p は、位数群が Z、環が A_{A_p} である評価であることがすぐにわかります。 したがって、§ 1, no. 4 の命題 3 によって、同値まで、不適切ではなく A に対してプラスである K のすべての評価が得られます。 A = Z として、Q の p 進評価を回復します (一般位相、章 IX, § 3, no. 2)。これらの評価は、同値までは、不適切ではない Q の唯一の評価です (§ 1, no. 4、系 1 ～ 命題 3)。 A = k[X]、ここでkは体、制限からkが不適切であるk(X)の不適切でない評価は次のとおりです(同値まで): 一方では、Pが以下の既約モニック多項式の集合を実行する評価v_P k[X] 一方、評価 v は次のように定義されます。

$$
v(P/Q) = \deg(Q) - \deg(P)
$$

P ∈ k[X] および Q ∈ k[X] (§ 1, no. 4、系 2 ～ 命題 3) の場合。これらすべての評価は明らかに Z が位数群であり、それらの剰余体は k (代数, 章 V, § 3, no. 1) の単次代数拡大です。

#### 例 (5) {#ac-vi-s3-n4-exa-5 .statement tag=04TE}

C[X, Y] から C((T)) までの写像 P(X, Y) ↦ P(T, e^T) は単射 (実数変数の写像、章 IV, §2、命題 9) であるため、次のようにすることができます。 C(X, Y)の同型からC((T))の部分体まで拡張されました。 The restriction to this subfield of the valuation on C((T)) defined in Example 3 defines a valuation on C(X, Y) which is improper on C, whose order group is Z and whose residue field is C.

no. 2 の命題 4 により、位数群および剰余体が与えられる評価構成するが可能になります。

#### 例 (6) {#ac-vi-s3-n4-exa-6 .statement tag=04TF}

Γ を完全順序付け群および k 体とします。 Γ_+ を k 上の Γ の正の元と Γ_+ の C 代数のモノイドとします。 定義までに、C は k 上で基底 (x_\alpha)_{\alpha \in \Gamma_-} を持ち、その乗法表は x_\alpha x_\beta = x_{\alpha + \beta} になります。 $x = \sum a_\alpha x_\alpha$ が C の非ゼロ元である場合、$v(x) = \inf_{a_\alpha \neq 0} (a)$ と $v(0) = +\infty$ を書き込みます。 $C$ から $\Gamma_\infty$ の写像 $v$ が no. 1 の条件 (VL_I) および (VL_{II}) を満たし、$C$ が整域であることがすぐに検証されます。 $K$ を、$C$ の分数の体と、拡大する $v$ (命題 4、no. 2) である$K$ の評価額を$w$ とします。 $\Gamma$ のすべての元は 2 つの正の元の差であるため、$w$ は $\Gamma$ を位数群として認めます。 $A$を$w$と$m$の環をその最大の理想とする。 $A$ が $m$ と $k$ ($k \cdot 1$ と同一視される) の直和であることを示し、$w$ の剰余体が $k$ と同型であることを証明します。明らかに$m \cap k = (0)$。一方、$a > 0$の$x_a$によって生成される$C$の理想を$p$で表すと、$K$の評価0のすべての元$x$は形$(a + y)/(b + z)$に書き込むことができます。 $a \in k^*, b \in k^*, y \in p$ と $z \in p$;それから

$$
x = ab^{-1} + (by - az)b^{-1}(b + z)^{-1}
$$

よって $w(x - ab^{-1}) > 0$ と $x \equiv ab^{-1} \pmod{m}$;これは主張を示しています。

$\Gamma = \mathbf{Z} \times \mathbf{Z}$ の場合、$K = k(X, Y)$ と上記の構成は、$k$ では不適切な $k(X, Y)$ の評価を提供します。その位数群は $\mathbf{Z} \times \mathbf{Z}$、剰余体は $k$ です。これらの評価は、$\mathbf{Z} \times \mathbf{Z}$ で選択された位数構造に依存します。たとえば、$\mathbf{Z} \times \mathbf{Z}$ には辞書編集的な順序を指定できます。あるいは実際、無理数数 $a$ の場合、$\mathbf{Z} \times \mathbf{Z}$ は準同型 $(m, n) \mapsto m + n\alpha$ ($a$ は無理数であるため単射法である準同型) の下で $\mathbf{R}$ の部分群と同一視され、以下によって誘発される順序付けが与えられる可能性があります。 $\mathbf{R}$のこと。

no. 2の命題4を使用したその他の構成の評価については、§ 10で説明します。

### 5. バリュエーションの理想環

#### 定義 2 {#ac-vi-s3-def-2 .statement tag=04TG}

*G を順序付けた集合とします。 関係 $x \in M$ と $y \geq x$ が $y \in M$ を暗示する場合、G の部分集合はメジャーと呼ばれます。*

$K$ を体、$v$ を $K$、$v$ の $A$ 環、および $v$ の $G$ 位数群の評価とします。すべてのメジャー 部分集合 $M \subset G$ について、$a(M)$ を $x \in K$ の集合とし、$v(x) \in M \cup \{+\infty\}$ とします。明らかに、$a(M)$ は $K$ のサブ A モジュールです。

#### 命題 7 {#ac-vi-s3-prop-7 .statement tag=04TH}

*写像 $M \mapsto a(M)$ は、$G$ のメジャー 部分集合の集合の増加する全単射を $K$ のサブ A モジュールの集合に配置します。

$b$ を $K$ のサブ A モジュールとします。 $x \in b - (0)$ の $v(x)$ の集合は、$G$ のメジャー 部分集合 $M(b)$ です。 命題次の方程式が証明されると 7 が表示されます。

(2) $G$ のメジャー 部分集合 $N$ ごとに $M(a(N)) = N$。
(3) $K$ のすべてのサブ A モジュール $b$ に対して $a(M(b)) = b$。

公式 (2) は簡単です。すべての $m \in N$ に対して、$v(x) = m$ となるような $x \in K$ が存在するからです。それから明らかに $b \subset a(M(b))$;逆に、$x \in a(M(b))$ として、$x \neq 0$ と仮定します。

次に $v(x) \in M(b)$ となり、したがって $v(x) = v(y)$ となる $y \in b$ が存在します。 よって $x = uy$ ここで $v(u) = 0$ は、$x \in A$ $y \subset b$ を証明し、証明を完成させます。

#### 系 {#ac-vi-s3-n5-cor-1 .statement tag=04TI}

$G_+$を$G$の正の元の集合とします。 写像 $M \mapsto a(M)$ は、$G_+$ のメジャー 部分集合の集合の全単射を、$A$ の理想の集合に重ねたものです。

$A = a(G_+)$ と同様に、$a(M) \subset A$ は $M \subset G_+$ と同等です。

たとえば、最大理想値 $m(A)$ は $a(S)$ に等しく、ここで $S$ は $G$ の厳密に正の元の集合を示します。

### 6. 個別の評価

#### 定義 3 {#ac-vi-s3-def-3 .statement tag=04TJ}

$K$ を (必ずしも可換ではない) 体、$v$ を $K$ および $\Gamma$ 位数群の $v$ の評価とします。 $\mathbf{Z}$ 上に順序付けられた群 $\Gamma$ の (必然的に一意な) 同型が存在する場合、$v$ は離散的と呼ばれます。この同型の下で、$\gamma$を$\Gamma$対応するから$1$の元とします。 $v(u) = \gamma$ が $v$ の均一化器と呼ばれるように、$K$ のすべての元 $u$ です。離散評価は、位数群が $\mathbf{Z}$ の場合、標準と呼ばれます。

たとえば、主イデアル * または階乗領域の極値元 $p$ によって定義される評価 $v_p$ は、均一化要素として $p$ を認める標準化された離散評価です。特に、$k$ が体である場合、$k[[T]]$ は$k((T))$ の離散評価の環となり、$T$ を均一化要因として認めます。 $S$ を、$S$ 上の有理型写像の次元 1、$K$ 体、および $S$ の $z_0$ 点の接続された複素解析多様体とします。 $z_0$ で正則である $\in K$ をオフにした集合は、離散評価 $v$ の環です。 写像 $f \in K$ が $v$ に対して均一化されるためには、$z_0$ で零が正則であり、$S$ に$z_0$ の近傍 $V$ が存在することが必要かつ十分です。 制限から $V$ は、$V$ の準同型から $\mathbf{C}$ の原点の近傍になります。この例と他の類似物が語 「ユニフォームライザー」の起源です。*

#### 命題 8 {#ac-vi-s3-prop-8 .statement tag=04TK}

$K$ を (必ずしも可換ではない) 体、$v$ を $K$、$A$ 環の $v$、および $u$ を $v$ の均一化とする。 $A$ のゼロ以外の理想は両面的であり、形 $Au^n$ ($n \geq 0$) の理想です。

$v$ が標準であるため、$v(u) = 1$ であると仮定できます。すべての $x \in K^*$ に対して、$(v(x) = n = v(u^n)$ となるような整数 $n \in \mathbf{Z}$ が存在するため、次のように書くことができます。

$$
x = zu^n = u^n z',
$$

ここで、$z, z'$ は環 $A$ の 2 つの可逆元です。 よって命題。

#### 命題 9 {#ac-vi-s3-prop-9 .statement tag=04TL}

$A$ を、分数の体とは異なるローカルな整域とします。次の条件は同等です。
(a) $A$ は個別評価の環です。
(b) $A$ は主イデアル整域です。
(c) 理想は$m(A)$が主で、$\bigcap_{n=1}^{\infty} m(A)^n = (0)$が理想です。

(d) $A$ は *ネーター 環* であり、$m(A)$ は *プリンシパル* です。
(e) $A$ は *ネーター の評価環* です。

命題 8 は、(a) が (b)、(d)、および (e) を意味することを示します。 $A$ が主イデアル整域の場合、$A$ はローカル (*代数*、章 VII, § 1, no. 3、定理 2) であるため、$m(A) = Au$ と $A$ のゼロ以外のすべての理想は形 $Au^n$ になります。したがって $\bigcap_{n=1}^\infty m(A)^n = 0$;これは、(b) が (c) を意味することを示しています。 一方、(d) は (c) (章 III, § 3, no. 2、系 ～ 命題 5) を意味します。 § 1, no. 4 の命題 2 により、(c) は (a) を意味します。 したがって、条件 (a)、(b)、(c)、(d) は同等であり、(e) を意味します。 最後に、(e) が成り立つと仮定し、(b) が成り立つことを示しましょう。次の補題を証明すれば十分です。

#### 補題 1 {#ac-vi-s3-lem-1 .statement tag=04TM}

※$A$を評価環とします。有限生成されたねじれのない $A$ モジュールはすべて無料です。有限に生成されたすべての理想 $\mathfrak{a}$ または $A$ が主です。ねじれのないすべての $A$ モジュールは平らです。*

$E$ を有限生成されたねじれのない $A$ モジュールとし、$x_1, \ldots, x_n$ を数で最小となる$E$ の生成元とします。それらが線形独立であることを示します。 $\sum_{i=1}^n a_i x_i = 0$ ($a_i \in A$) が $x_i$ の間の自明ではない関係である場合、$A$ の主な理想の集合は包含によって完全に順序付けられるため、$a_i$ の 1 つ、たとえば $a_1$ と割るの他のすべてが含まれます。 (§ 1, no. 2, 定理 1); 関係は自明ではないため、$a_1 \neq 0$ となります。 $E$ にはねじれがないため、$a_1$ によって割るが得られます。これは、$a_1 = 1$ と仮定することになります。しかし、$x_1$ は$n$ の最小指標とは反対に、$x_2, \ldots, x_n$ の線形結合になります。したがって、$E$ は無料です。

特に、$A$ の有限生成されたすべての理想 $\mathfrak{a}$ が主であり、系の生成元の $\mathfrak{a}$ のすべての元は、そのうちの 1 つである倍数です。 章 I, § 2, no. 4 の命題 3 は、ねじれのないすべての $A$ モジュールが平坦であることを示しています。

### 練習問題 {#ac-vi-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
