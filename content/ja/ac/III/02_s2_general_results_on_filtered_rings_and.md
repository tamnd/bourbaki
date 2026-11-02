---
book: ac
book_title: Commutative Algebra
chapter: III
chapter_title: GRADUATIONS. FILTRATIONS AND TOPOLOGIES
section: 2
section_title: General results on filtered rings and modules
lang: ja
source: ac-i-vii
book_pages: 162-195, 233-245
pdf_pages: 0182-0215, 0253-0265
extraction: ocr
subsections:
    - "no": 1
      title: FILTERED RINGS AND MODULES
      page: 162
      pdf_page: 182
    - "no": 2
      title: THE ORDER FUNCTION
      page: 165
      pdf_page: 185
    - "no": 3
      title: THE GRADED MODULE ASSOCIATED WITH A FILTERED MODULE
      page: 165
      pdf_page: 185
    - "no": 4
      title: HOMOMORPHISMS COMPATIBLE WITH FILTRATIONS
      page: 169
      pdf_page: 189
    - "no": 5
      title: THE TOPOLOGY DEFINED BY A FILTRATION
      page: 170
      pdf_page: 190
    - "no": 6
      title: COMPLETE FILTERED MODULES
      page: 173
      pdf_page: 193
    - "no": 7
      title: LINEAR COMPACTNESS PROPERTIES OF COMPLETE FILTERED MODULES
      page: 176
      pdf_page: 196
    - "no": 8
      title: THE LIFT OF HOMOMORPHISMS OF ASSOCIATED GRADED MODULES
      page: 177
      pdf_page: 197
    - "no": 9
      title: THE LIFT OF FAMILIES OF ELEMENTS OF AN ASSOCIATED GRADED MODULE
      page: 179
      pdf_page: 199
    - "no": 10
      title: 'APPLICATION: EXAMPLES OF NOETHERIAN RINGS'
      page: 183
      pdf_page: 203
    - "no": 11
      title: COMPLETE m-ADIC RINGS AND INVERSE LIMITS
      page: 185
      pdf_page: 205
    - "no": 12
      title: THE HAUSDORFF COMPLETION OF A FILTERED MODULE
      page: 187
      pdf_page: 207
    - "no": 13
      title: THE HAUSDORFF COMPLETION OF A SEMI-LOCAL RING
      page: 192
      pdf_page: 212
statements: 57
exercises: 31
content_sha256: c0451c3b8232ab04008adf589dbd19d740200ac80bbcc8738f5253f1b9116c0e
translated_from: content/en/ac/III/02_s2_general_results_on_filtered_rings_and.md
translation_method: google
source_content_sha256: 0a34905c17ca45e9431cd3c4d11e11fd5e18faa0d9245992a206dca25aae5226
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 21e243913c2d1d6f7108b4984749abe58a9070b3c6de740e81ee560d2607367b
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 2。フィルタリングされた環および加群の一般的な結果

### 1. 環と加群をフィルタリングしました

#### 定義 1 {#ac-iii-s2-def-1 .statement tag=04DH}

増加する (それぞれ減少する) 群 $G$ の部分群の数列 $(G_n)_{n \in \mathbf{Z}}$ は、$G$ での増加する (それぞれ減少する) の濾過と呼ばれます。
濾過を施した群を濾過済み群と呼びます。

$(G_n)_{n \in \mathbf{Z}}$ が群 $G$ での増加する (それぞれ減少する) の濾過であり、$G'_n = G_{-n}$ と書くと、明らかに $(G'_n)_{n \in \mathbf{Z}}$ は $G$ での減少する (それぞれ増加する) の濾過です。したがって、私たちは研究を減少する濾過に限定することができ、したがって今後濾過について話すときは減少する濾過を意味し、そうでない場合は〜でない限りを意味します。

群 $G$ の減少するろ過 $(G_n)_{n \in \mathbf{Z}}$ を考えると、明らかに $\bigcap_{n \in \mathbf{Z}} G_n$ と $\bigcup_{n \in \mathbf{Z}} G_n$ は $G$ の部分群です。 $\bigcup_{n \in \mathbf{Z}} G_n$ が単位元に還元される場合、濾過は分離済みと呼ばれ、$\bigcup_{n \in \mathbf{Z}} G_n = G$ の場合は完全と呼ばれます。

#### 定義 2 {#ac-iii-s2-def-2 .statement tag=04DI}

環 $A$ の場合、加法群 $A$ 上の濾過 $(A_n)_{n \in \mathbf{Z}}$ は、次の場合に $A$ の環構造と互換性があると呼ばれます。

(1)
$$
A_m A_n \subset A_{m+n} \quad \text{for} \quad m \in \mathbf{Z}, \quad n \in \mathbf{Z}
$$

(2)
$$
1 \in A_0.
$$
このろ過を行った環 $A$ は、ろ過された環と呼ばれます。

条件 (1) と (2) は、$A_n$ が $A$ と $A_n$ (左と右) $A_0$ モジュールの部分環であることを示しています。 集合 $B = \bigcup_{n \in \mathbf{Z}} A_n$ は、$A$ と集合 $n = \bigcap_{n \in \mathbf{Z}} A_n$ の部分環であり、$B$ の両面の理想です。 (1) により、すべての $k \in \mathbf{Z}$、$x \in A_{k-p}$、よって、$ax \in A$、$xa \in A$ が $x \in n$ と $a \in A_k$ の場合、したがって、$ax \in n$ と $xa \in n$ です。

重要な特定のケースは、$A_n = A$;次に、$n \leq 0$の$A_n = A$、そしてすべての$A_n$は$A$の両面の理想です。

#### 定義 3 {#ac-iii-s2-def-3 .statement tag=04DJ}

$A$ をフィルタリングされた環、$(A_n)_{n \in \mathbf{Z}}$ をそのフィルタリング、$E$ を $A$ モジュールとします。 $E$ 上のフィルタリング $(E_n)_{n \in \mathbf{Z}}$ は、次の場合、フィルタリングされた環 $A$ に対してその加群構造と互換性があると呼ばれます。
$$
A_m E_n \subset E_{m+n} \quad \text{for} \quad m \in \mathbf{Z}, \quad n \in \mathbf{Z}.
$$
このフィルターを備えた $A$ モジュール $E$ は、フィルター付き加群と呼ばれます。

$E_n$ はすべて $A_n$ モジュールです。 $B = \bigcup_{n \in \mathbf{Z}} A_n$ の場合、明らかに $\bigcup_{n \in \mathbf{Z}} E_n$ は $B$ モジュールであり、上記の $\bigcap_{n \in \mathbf{Z}} A_n$ と同じ議論により $\bigcap_{n \in \mathbf{Z}} E_n$ も同様です。 $A_n = A$の場合、$E_n$はすべて$E$の部分加群です。

例

(1) $A$ を型 $\mathbf{Z}$ の等級付けされた環とします。すべての $i \in \mathbf{Z}$ について、$A_{(i)}$ を $A$ の次数 $i$ の同種元の部分群とします。 $A_n = \sum_{i \geq n} A_{(i)}$ と書きましょう。次に、$(A_n)$ の$A$ の環構造と互換性のある、包括的で分離された減少する濾過が明らかです。この濾過は、目盛り $(A_{(i)})_{i \in \mathbf{Z}}$ に関連付けられていると言われ、濾過された環 $A$ は、与えられた等級環 $A$ に関連付けられていると言われています。

ここで、$E$ を型 $\mathbf{Z}$ の等級付けされた環 $A$ の等級付けされた加群とし、すべての $i \in \mathbf{Z}$ について、$E_{(i)}$ を同種の元の部分群とします。 次数 $i$/$E$。 $E_n = \sum_{i \geq n} E_{(i)}$ と書きましょう。次に、$(E_n)$ は徹底的で分離された減少する濾過であり、濾過された環 $A$ よりも $E$ の加群構造と互換性があります。この濾過は目盛 $(E_{(i)})_{i \in \mathbf{Z}}$ に関連付けられていると言われ、濾過された加群 $E$ は与えられた等級加群 $E$ に関連付けられていると言われています。

(2) $A$ をフィルタリングされた環、$(A_n)_{n \in \mathbf{Z}}$ をそのフィルタリング、$E$ を $A$ モジュールとします。 $E_n = A_n E$ と書きましょう。 (1) から次のことがわかります
$$
A_m E_n = A_m A_n E \subset A_{m+n} E = E_{m+n},
$$
そして(2)からその$E_0 = E$; $(E_n)$ は、$E$ の $A$ モジュール構造と互換性のある徹底的な濾過です。この濾過は、$A$ に与えられた濾過 $(A_n)$ から派生したと言われています。 $(A_n)$ が分離され、$E$ と $A_n$ が有限生成された $A$ モジュール (cf. 、練習問題 2; ただし、§ 3, no. 3、命題 5 および命題を参照) であっても、必ずしも分離されているわけではないことに注意してください。 no. 2、系 ～ 命題 4)

(3) $A$を環、$m$を$A$の両面理想とする。 Let us write $A_n = m^n$ for $n \geq 0$, $A_n = A$ for $n < 0$; it is immediate that $(A_n)$ is an exhaustive filtration on $A$, called the $m$-adic filtration. Let $E$ be an $A$-module; the filtration $(E_n)$ derived from the $m$-adic filtration on $A$ is called the $m$-adic filtration on $E$; in other words, $E_n = m^n E$ for $n \geq 0$ and $E_n = E$ for $n < 0$.

If $A$ is commutative and $B$ is an $A$-algebra, $n = mB$ is a two-sided ideal of $B$ and, for every $B$-module $F$, $n^k F = m^k F$ and hence the $n$-adic filtration on $F$ coincides with the $m$-adic filtration (if $F$ is considered as an $A$-module).

(4) $A$ がフィルタリングされた環であり、$(A_n)$ がそのフィルタリングである場合、左側の $A$ モジュール $A_n$ は、フィルタリング $(A_n)$ を備えたフィルタリングされた $A$ モジュールです。一方、明らかに $(A_n)$ は反対環 $A^0$ の環構造と互換性のある濾過であり、$A_n$ は濾過 $(A_n)$ を備えた濾過された (左) $A^0$ モジュールです。

(5) 環 $A$ 集合 $A_n$ では、$n > 0$ については $A_n = 0$、$n \leq 0$ 形については $A_n = A$ となるように、上の自明な目盛りに関連するいわゆる自明な濾過 (例 1) $A$; $A$ モジュール $E$ では、サブ $A$ モジュールのすべてのフィルタ $(E_n)$ からなるは、フィルタされた環 $A$ 上で $E$ の加群構造と互換性があります。その場合、$\mathbf{Z}$ に自明なフィルタリングが与えられた場合、フィルタリングされたすべての可換群 $G$ はフィルタリングされた $\mathbf{Z}$ 加群であると言えます。

$G$ をフィルター処理された群とし、$(G_n)_{n \in \mathbf{Z}}$ をそのフィルター処理とします。明らかに、$G$の部分群$H$ごとに、$(H \cap G_n)_{n \in \mathbf{Z}}$は$G$の濾過によって引き起こされると言われています。 $G$ にある場合、それは網羅的 (それぞれ分離) です。同様に、$H$ が $G$ の通常の部分群である場合、ファミリー $((H.G_n)/H)_{n \in \mathbf{Z}}$ は群 $G/H$ の濾過であり、$G$ の濾過の $H$ の下で商と呼ばれます。 $(G_n)$ であれば網羅的です。 $G'$ が他ので濾過され、 群と $(G'_n)_{n \in \mathbf{Z}}$ で濾過されたものである場合、$(G_n \times G'_n)$ は、$G$ と $G'$ での濾過の積と呼ばれる $G \times G'$ での濾過であり、これが網羅的です(それぞれ分離) $(G_n)$ と $(G'_n)$ の場合。

ここで、$A$ をフィルタリングされた環とし、$(A_n)$ をそのフィルタリングとします。 $A$ のすべての部分環 $B$ で、明らかに $A$ の濾過によって引き起こされる濾過は、$B$ の環構造と互換性があります。 $b$ が $A$ の両面理想である場合、$A$ の$A/b$ の商濾過は、この環の構造と互換性があります。
$$
(A_n + b)(A_m + b) \subset A_{n+m} + b.
$$
$A'$ が環で他のフィルタリングされている場合、$A \times A'$ の積フィルタリングは、この環の構造と互換性があります。

最後に、$E$ をフィルタリングされた $A$ モジュール、$(E_n)$ をそのフィルタリングとします。 $E$ の部分加群 $F$ ごとに、$E$ の濾過によって引き起こされる濾過は、$F$ の $A$ モジュール構造と互換性があり、商加群 $E/F$ では、$E$ の濾過の商と互換性があります。として、$A$ モジュール構造と互換性があります。
$$
A_n(F + E_m) \subset F + A_n E_m \subset F + E_{m+n}.
$$

E の濾過が A (例 2) の濾過から派生した場合、E/F の商濾過も同様ですが、一般に、濾過は *F (練習問題 1; ただし、no. 2、定理 2 を参照) に誘導されるわけではないことに注意してください。

E' が他のフィルタリング A-加群の場合、E × E' の積フィルタリングは、その A-加群構造と互換性があります。 E と E' の濾過が A (例 2) の濾過から派生した場合、その積の濾過も同様です。

### 2. 位数写像

A をフィルタリングされた環、E をフィルタリングされた A-加群、(E_n) を E のフィルタリングとします。すべての x ∈ E について、v(x) は、x ∈ E_n となるような整数 n ∈ Z 上の集合の R の *最小* 上界を表します。次に、次の同値が成り立ちます。

$$
\begin{cases}
v(x) = -\infty \Leftrightarrow x \notin \bigcup_{n \in \mathbf{Z}} E_n \\
v(x) = p \Leftrightarrow x \in E_p \text{ and } x \notin E_{p+1} \\
v(x) = +\infty \Leftrightarrow x \in \bigcap_{n \in \mathbf{Z}} E_n
\end{cases}
$$

写像 v : E → \overline{\mathbf{R}} は、フィルタリングされた加群 E の位数写像と呼ばれます。 v が既知であれば、E_n も既知です。なぜなら、E_n は、v(x) ≥ n である x ∈ E の集合であるからです。 E_n が E の加法的部分群であるという事実は、関係を意味します

$$
v(x - y) \geq \inf(v(x), v(y)).
$$

上記の定義は、特にフィルタリングされた A-加群 A に適用されます。 w を位数写像とします。 no. 1 の方程式 (3) から、a ∈ A および x ∈ E について、次のことがわかります。

$$
v(ax) \geq w(a) + v(x)
$$
右辺が定義されているときは常に。特に、a ∈ A および b ∈ A の場合、

$$
w(ab) \geq w(a) + w(b)
$$
右辺が定義されるたびに。

*位数写像* は、フィルタリングされた群 G 上でも同様に定義されますが、必ずしも可換である必要はありません。 対応する関係 ～ (5) が書き込まれます

$$
v(yx^{-1}) = v(xy^{-1}) \geq \inf(v(x), v(y)).
$$

### 3. フィルタリングされた加群に関連付けられたグレーディング加群

G を可換群 (加法的に書かれる) とし、(G_n) を G のフィルタリングとします。

$$
\begin{align*}
\operatorname{gr}_n(G) &= G_n / G_{n+1} \quad \text{for } n \in \mathbf{Z} \\
\operatorname{gr}(G) &= \bigoplus_{n \in \mathbf{Z}} \operatorname{gr}_n(G).
\end{align*}
$$

可換群 gr(G) は、型 $\mathbf{Z}$ の段階的群であり、フィルタリングされた群 G に関連付けられた *段階的群と呼ばれます。 gr(G) の次数 $n$ の同次元は、 $\mathrm{gr}_n(G)$。

ここで、A をフィルタリングされた環、(A_n) をそのフィルタリング、E をフィルタリングされた A-加群、(E_n) をそのフィルタリングとします。すべての$p \in \mathbf{Z}$、$q \in \mathbf{Z}$、写像

$$
\mathrm{gr}_p(A) \times \mathrm{gr}_q(E) \to \mathrm{gr}_{p+q}(E)
$$

は次のように定義されます: $a \in \mathrm{gr}_p(A)$、$\xi \in \mathrm{gr}_q(E)$、$a$ の 2 つの代表 $a, a'$ と $\xi$、$ax \in E_{p+q}$、$a'x' \in E_{p+q}$、および $ax \equiv a'x'$ (修正 $E_{p+q+1}$) の 2 つの代表 $x, x'$ が与えられた場合、

$$
ax - a'x' = (a - a')x + a'(x - x')
$$

$a - a' \in A_{p+1}$ と $x - x' \in E_{q+1}$ したがって、主張は no. 1 の公式 (3) から続きます。したがって、 $\alpha\xi$ 類で表すことができます。

$$
E_{p+1}/E_{p+q+1} = \mathrm{gr}_{p+q}(E)
$$

任意の代表者 $a \in a$ および任意の代表者 $x \in \xi$ の積 $ax$。 写像 (9) が *Z 双線形* であるのは明らかです。線形性により、$\mathbf{Z}$-双線形写像を導き出します。

$$
\mathrm{gr}(A) \times \mathrm{gr}(E) \to \mathrm{gr}(E).
$$

この定義を最初にケース $E = A_0$ に適用すると、写像 (10) は $\mathrm{gr}(A)$ 上の合成の内部法則であり、これは *結合* であることがすぐに検証され、 $\mathrm{gr}_0(A)$ の標準像である単位元を持ちます。 Aの単位元;したがって、$\mathrm{gr}(A)$ 環構造の定義するとなり、卒業$(\mathrm{gr}_n(A))_{n \in \mathbf{Z}}$ は定義までにこの構造と互換性があります。このように定義された等級付けされた環 $\mathrm{gr}(A)$ (型 $\mathbf{Z}$) は、フィルタリングされた環 A に関連付けられた *等級付けされた環* と呼ばれます。 A が可換であれば、それは明らかに可換です。 $\mathrm{gr}_0(A)$は$\mathrm{gr}(A)$の部分環です。一方、写像 (10) は、$\mathrm{gr}(E)$ 上の$\mathrm{gr}(A)$ 加群外部法則であり、加群の公理が自明に満たされており、$\mathrm{gr}(E)$ の卒業$(\mathrm{gr}_n(E))_{n \in \mathbf{Z}}$ は明らかにこの加群構造と互換性があります。このように定義された段階的 $\mathrm{gr}(A)$ モジュール $\mathrm{gr}(E)$ (型 $\mathbf{Z}$) は、フィルター処理された A-加群 E に関連付けられた *段階的加群と呼ばれます。

*例*

#### 例 1 {#ac-iii-s2-n3-exa-1 .statement tag=04DK}

A を 0 の因子ではない A の可換環および $t$ 元とします。A に *(t)*-*アジック フィルトレーション* (no. 1, *例 3*) を与えましょう。次に、関連する等級付けされた環 $\mathrm{gr}(A)$ は、*多項式環* $(A/(t))[X]$ と標準的に同型です。 $\mathrm{gr}_n(A) = 0$ の場合、$n < 0$ の場合、定義環 $\mathrm{gr}_0(A)$ では、環 $A/(t)$ になります。ここで、$t$ 関係 $at^n \equiv 0$ (mod. $t^{n+1}$) の仮定が $a \equiv 0$ (mod. $t$) と同等であることに注目します。 $\tau$ が $\mathrm{gr}_1(A)$ の $t$ の標準像である場合、$\mathrm{gr}_n(A)$ のすべての元は $\alpha \in \mathrm{gr}_0(A)$ の形 $\alpha \tau^n$ に一意に書き込まれます。 よって私たちの主張。

#### 例 2 {#ac-iii-s2-n3-exa-2 .statement tag=04DL}

$K$ を正式な冪系列の可換環、$A$ 環とします

$$
K[[X_1,\ldots,X_r]]
$$

(*代数、章 IV, § 5*) と $m$ $A$ の理想。その元は定数項のない正式な冪系列です。 $A$ に $m$ 進数 *filtration* (no. 1, *例 3*) を与えましょう。 $M_1,\ldots,M_s$ が合計次数 $n-1$ の $X_1,\ldots,X_r$ の別個の単項式である場合、明らかに合計位数 $\omega(u)\geq n$ のすべての形式的冪系列 $u$

*(loc. cit.、no. 2)* は、$\displaystyle\sum_{k=1}^{s}u_kM_k$ と書かれる場合があります。ここで、$u_k$ 属するから $m$ です。 $m^n$ は、$\omega(u)\geq n$ となる形式的な冪系列 $u$ の集合であることが**わかります**。これは、$\omega$ が $m$ 進フィルタリングの *順序関数* であることを示しています。したがって、明らかに、すべての形式的な冪系列 $u\in m^n$ に対して、$u$ mod と合同である次数 $n$ という固有の *同次多項式* が $X_i$ に存在します。 $m^{n+1}$、つまり、次数の項の和、$u$の$n$。私たち結論するは、$\operatorname{gr}(A)$ が *多項式環* $K[X_1,\ldots,X_r]$ と標準的に同型であると考えます。

#### 例 3 {#ac-iii-s2-n3-exa-3 .statement tag=04DM}

More generally, let $A$ be a commutative ring, $b$ an ideal of $A$ and $A$ be given the $b$-adic filtration. $B=\operatorname{gr}_0(A)$, $F=\operatorname{gr}_1(A)=b/b^2$ と書くと、(*代数, 章 III*)、$B$ モジュール $F$ の恒等写像を *対称から準同型 $u$ に一意に拡張できることがわかります。 代数* $F$ の $S(F)$ から $B$-代数 $\operatorname{gr}(A)$ へ。 $\operatorname{gr}(A)$ の定義から、$u$ は等級付けされた代数* の *全射準同型であることがわかります。 $n\geq1$ の場合、$\operatorname{gr}_n(A)$ のすべての元は、形 $y=x_1x_2\cdots x_n$ の元の $b^{n+1}$ を加味して類の和になります。ここで、$x_i\in b$ $(1\leq i\leq n)$ です。 $\xi_i$ が $x_i$ mod の類の場合。 $b^2$、明らかに $y$ mod の類です。 $b^{n+1}$ は元 $u(\xi_1)\cdots u(\xi_n)$、よっては私たちの主張です。 特に、$B$-モジュール $F$ の生成元のすべての系は、$B$-代数 $\operatorname{gr}(A)$ の生成元の系です。

If now $E$ is an $A$-module and $E$ is given the $b$-adic filtration, it is seen similarly that the graded $\operatorname{gr}(A)$-module $\operatorname{gr}(E)$ is *generated* by $\operatorname{gr}_0(E)=E/bE$. To be precise, the restriction $\phi$ to $\operatorname{gr}(A)\times\operatorname{gr}_0(E)$ of the external law on the $\operatorname{gr}(A)$-module $\operatorname{gr}(E)$ is a $\mathbf{Z}$-bilinear mapping of $\operatorname{gr}(A)\times\operatorname{gr}_0(E)$ to $\operatorname{gr}(E)$; moreover $\operatorname{gr}(A)$ is a $(\operatorname{gr}_0(A),\operatorname{gr}_0(A))$-bimodule and $\operatorname{gr}_0(E)$ a $\operatorname{gr}_0(A)$-module; it is immediately verified that, for $a\in\operatorname{gr}(A)$, $\alpha_0\in\operatorname{gr}_0(A)$, $\xi\in\operatorname{gr}_0(E)$,

$$
\phi(a\alpha_0,\xi)=\phi(a,\alpha_0\xi)
$$

したがって $\phi$ 定義するは *全射* $\operatorname{gr}_1(A)$ 線形写像

(11)

$$
\gamma_E:\operatorname{gr}(A)\otimes_{\operatorname{gr}_0(A)}\operatorname{gr}_0(E)\longrightarrow\operatorname{gr}(E)
$$

これは *正規* と呼ばれます。

#### 例 4 {#ac-iii-s2-n3-exa-4 .statement tag=04DN}

\* $K$ を可換環、$\mathfrak g$ リー代数を $K$ および $U$ を、$\mathfrak g$ を囲む代数とします。 *増加する濾過* $(U_n)_{n\in\mathbf{Z}}$は、$n<0$の$U_n=\{0\}$をとり、$U$の元の$n\geq0$集合を$U_n$で表すことにより$U$で定義され、和と表現できます。 積最大 $n$ 元 $\mathfrak g$ の場合

U_0 = K および gr(U) は可換K-代数 (リー群およびリー代数、章 I, § 2, no. 6) です。 標準写像 g から gr_1(U) = U_1/U_0 は、K-加群 g から K-代数 gr(U) の対称代数 $S(g)$ の準同型 h に一意に拡張できます。 準同型 h は全射であり、K-加群 g が自由の場合、h は全単射です (上記、no. 7、定理 1)。

#### 例 5 {#ac-iii-s2-n3-exa-5 .statement tag=04DO}

A を型 $\mathbf{Z}$ の評価環とし、E を型 $\mathbf{Z}$ の評価 A-加群とします。 $A_{(i)}$ (それぞれ $E_{(i)}$) を A (それぞれ E) の次数 i の同種元の部分群とします。 A と E にその目盛り (no. 1、例 1) に関連付けられた濾過が与えられ、A' と E' がこのようにして得られた濾過された環と濾過された A-加群を表すものとします。次に、$A_{(n)}$ の写像元をその標準像に変換する Z 線形マッピング $A \to \mathrm{gr}(A')$ は明らかです。
$$
\mathrm{gr}_n(A) = \left( \bigoplus_{i \geq n} A_{(i)} \right) / \left( \bigoplus_{i \geq n+1} A_{(i)} \right)
$$
グレードは環同型です。正規グレードの A-加群同型 $E \to \mathrm{gr}(E')$ も同様に定義されます。

#### 命題 1 {#ac-iii-s2-prop-1 .statement tag=04DP}

A をフィルター処理された環、$(A_n)_{n \in \mathbf{Z}}$ のフィルター処理、および v の次数関数とします。 $\mathrm{gr}(A)$ が環で、零の因子がないとします。次に、注文された対の元 a、b の環 $B = \bigcup_{n \in \mathbf{Z}} A_n$、$v(ab) = v(a) + v(b)$ ごとに。

$n = \bigcap_{n \in \mathbf{Z}} A_n$ は環 B の両側イデアルであるため、$v(a)$ または $v(b)$ が $+\infty$ に等しい場合、公式が成り立ちます。 そうでない場合、$v(a) = r$ と $v(b) = s$ は整数になります。 MOD の類 $\alpha$。 b modのA、+、$\beta$。 A、+_1 は $\mathrm{gr}(A)$ の定義によって $\neq 0$、仮定 $\alpha \beta \neq 0$ によってよってとなるため、$ab \notin A_{r+s+1}$ は $ab \in A_{r+s}$ として、
$$
v(ab) = v(a) + v(b).
$$

#### 系 {#ac-iii-s2-n3-cor-1 .statement tag=04DQ}

A をフィルタリングされた環およびそのフィルタリング $(A_n)_{n \in \mathbf{Z}}$ とします。 集合 $B = \bigcup_{n \in \mathbf{Z}} A_n$、$n = \bigcap_{n \in \mathbf{Z}} A_n$ にしましょう。 環 $\mathrm{gr}(A)$ に零の因子がない場合、環 $B/n$ もありません。
aとbがnに対する所属ではなくBの元であれば、$v(a) \neq +\infty$と$v(b) \neq +\infty$、よって$v(ab) \neq +\infty$、したがって$ab \notin n$になります。

環 A は整域であり、$\mathrm{gr}(A)$ が整域 (練習問題 2) になることなく濾過 (A_n) が徹底的に分離される可能性があることに注意してください。

#### 注意 {#ac-iii-s2-n3-rem-1 .statement tag=04DR}

G を群とします。これは、すべての $n \in \mathbf{Z}$ に対して $G_{n+1}$ が G で正規となるようなフィルタ処理 $(G_n)_{n \in \mathbf{Z}}$ と必ずしも可換ではありません。もう一度$\mathrm{gr}_n(G) = G_n/G_{n+1}$にしましょう。 The restricted product of the family $(\mathrm{gr}_n(G))_{n \in \mathbf{Z}}$, that is the subgroup of the product $\prod_{n \in \mathbf{Z}} \mathrm{gr}_n(G)$ consisting of the elements $(\xi_n)$ all of whose components, except at most a finite number, are equal to the identity element, is also called the graded group associated with G and denoted by $\mathrm{gr}(G)$.

### 4. 準同型ろ過と互換性があります

G、G' を 2 つの可換群 (加法的に書く)、(G_n) G に対するフィルタリング、(G'_n) は G' に対するフィルタリングとします。 準同型 h : G → G' は、すべての n ∈ Z に対して h(G_n) ⊂ G'_n である場合、G および G' の濾過と互換性があると呼ばれます。合成準同型 G_n $\xrightarrow{h} G'_n \longrightarrow G'_n/G'_{n+1}$ は、G_{n+1} では零であるため、商を考慮すると定義するになります。 準同型 h_n : G_n/G_{n+1} → G'_n/G'_{n+1};したがって、一意の加法群準同型 gr(h) : gr(G) → gr(G') が存在し、すべての n ∈ Z に対して、gr(h) 一致する (h_n on gr_n(G) = G_n/G_{n+1}) となります。 gr(h) は、h に関連付けられた等級付けされた群準同型と呼ばれます。 G'' が 3 番目のフィルター処理された群であり、h' : G' → G'' 準同型で、フィルターと互換性がある場合、h' ∘ h は準同型で、フィルターと互換性があり、

(12)
$$
\operatorname{gr}(h' \circ h) = \operatorname{gr}(h') \circ \operatorname{gr}(h)
$$

#### 命題 2 {#ac-iii-s2-prop-2 .statement tag=04DS}

G を G のフィルタリングされた可換群および H 部分群とします。 H に誘導濾過と G/H 商濾過を与えるとします。 j : H → G が標準単射で、p : G → G/H 標準全射の場合、j と p は濾過と数列に適合します。

(13)
$$
0 \longrightarrow \operatorname{gr}(H) \xrightarrow{\operatorname{gr}(j)} \operatorname{gr}(G) \xrightarrow{\operatorname{gr}(p)} \operatorname{gr}(G/H) \longrightarrow 0
$$
正確です。

最初の主張は明らかです。 (G_n) が G のフィルタリングである場合、
$$
(H \cap G_n) \cap G_{n+1} = H \cap G_{n+1}
$$
したがって、 gr(j) は単射的です。しかも標準写像
$$
G_n \to (H + G_n)/H
$$
は全射なので、 (12) より gr(p) と gr(p) ∘ gr(j) = 0 も同様です。最後に、gr(p) の $\xi \in G_n/G_{n+1}$ 属するから核とします。この場合、 x ∈ H + G_{n+1} となるような x ∈ ξ が存在します。しかし G_{n+1} ⊂ G として、
$$
G_n \cap (H + G_{n+1}) = (H \cap G_n) + G_{n+1}
$$
したがって、x = y + z ここで、y ∈ H ∩ G、および z ∈ G, +_1;これは ξ が類 mod であることを証明します。 G、j(y) の +_1、その他の語では gr(j) の下の gr(H) の属するから像です。

フィルタリングされた可換群の完全系列 0 → G' \xrightarrow{u} G \xrightarrow{v} G'' → 0 の場合、u と v はフィルタリングと互換性があり、 数列 0 \longrightarrow \operatorname{gr}(G') \xrightarrow{\operatorname{gr}(u)} であることに注意してください。 \operatorname{gr}(G) \xrightarrow{\operatorname{gr}(v)} \operatorname{gr}(G'') \longrightarrow 0 は必ずしも正確ではありません (練習問題 4)。

ここで、A と B が 2 つのフィルタリングされた環と h: A → B 環準同型である場合、これはフィルタリングと互換性があり、等級付けされた群準同型 gr(h): gr(A) → gr(B) も環準同型であることがすぐに検証されます。特に、誘導濾過により A' が A の部分環である場合、gr(A') は gr(A) の等級付けされた部分環 (命題 2) と標準的に識別されます。 b が A の両側イデアルで、A/b に商フィルタリングが与えられる場合、gr(A/b) は商等級付けされた環 gr(A)/gr(b) (命題 2) で標準的に識別されます。

最後に、A をフィルタリングされた環、E、F 2 つのフィルタリングされた A-加群、および u : E → F 準同型がフィルタリングと互換性があるとします。 その場合、 gr(u) : gr(E) → gr(F) は gr(A) 線形写像であるため、段階的な gr(A) モジュールの次数 0 の同次準同型となるのは明らかです。 さらに、u' : E → F が他の A 準同型性がフィルタリングと互換性がある場合、u + u' も同様であり、

$$
\operatorname{gr}(u + u') = \operatorname{gr}(u) + \operatorname{gr}(u').
$$

注意

(1) 濾過と互換性のある明らかに濾過された環準同型 (それぞれ濾過された環 A を超える濾過された加群の準同型) は、濾過された環構造 (それぞれ濾過された A-加群構造) の射として解釈できます。 (集合理論、章 IV, § 2, no. 1)。

(2) E と F を、フィルタリングされた環 A 上の 2 つの加群とし、A のフィルタリング (A_n) から派生したフィルタリング (no. 1, 例 2) を持つものとします。したがって、すべての A-線型写像 u : E → F は濾過と互換性があります。

$$
u(A_nE) = A_nu(E) \subset A_nF.
$$

(3) フィルタリングと互換性のあるフィルタリングされた A-加群準同型 u : E → F は、零にならずに満たす gr(u) = 0 になる可能性があることに注意してください。これは、たとえば (n) 進フィルタリングを使用した加法群 $\mathbf{Z}$ の自己準同型 x ↦ nx に当てはまります (任意の整数 n > 1 の場合)。 E から F までの 2 つの準同型 u、v に対する関係 gr(u) = gr(v) は、濾過と互換性があるため、必ずしも u = u を意味するものではありません。

(4) この番号の冒頭の定義拡大するはすぐに 2 つの群 G、G' になります。これらは必ずしも可換ではなく、部分群 $G_n, G'_n$ によってフィルタリングされ、$G_{n+1}$ (それぞれ $G'_{n+1}$) が G (それぞれ $G'_n$) で正常となるようにします。 命題 2 も G に関する同じ仮説で有効であり、H が G で不変であると仮定すると、証明は記法を除いて変化しません。

### 5. 位相フィルターによって定義される

G を、G の通常の部分群の族 $(G_n)_{n \in \mathbf{Z}}$ によってフィルタリングされた群とします。G には、群構造と互換性のある固有の位相が存在し、G_n は G の近傍の単位元 e の基本的な系を構成します (一般位相、 章 III, § 1, no. 2、例);それは、フィルタリング (G_n) によって定義される G 上で位相と呼ばれます。フィルタリングされた群に関してトポロジカル概念を使用する場合、特に指定のない限り、フィルタリングによって定義された位相を伴う 〜でない限りを意味します。 G_n は G の部分群であり、開いているものと閉じているものがあることに注意してください (一般位相、章 III, § 2, no. 1、系 ～ 命題 4)。

各 G は G で正規であるため、G 一致するの左右の均一性の取り巻き。 G はハウスドルフ完了群 $\hat{G}$ (一般位相、章 III, § 3, no. 4、定理 1 および no. 1、命題 2) を認めると推測します。

G のすべての部分集合 M について、G の M の閉包は次と等しくなります。

$$
\bigcap_{n \in \mathbf{Z}} (M . G_n) = \bigcap_{n \in \mathbf{Z}} (G_n . M)
$$

(一般位相、章 III, § 3, no. 1、公式 (1));特に $\bigcap_{n \in \mathbf{Z}} G$ は $\{e\}$ の終結です。したがって、G 上の位相がハウスドルフであるためには、濾過 (G_n) が分離されることが必要かつ十分であることがわかります。 G 上の位相が離散的であるためには、$G_+ = \{e\}$ となるような $n \in \mathbf{Z}$ が存在することが必要かつ十分です (この場合、$m \geq n$ に対して $G_m = \{e\}$)。この場合、フィルタ (G_n) は離散と呼ばれます。

G に関連付けられたハウスドルフ群は $H = G / \left( \bigcap_{n \in \mathbf{Z}} G_n \right)$ であるため、関連付けられた等級付けされた群 gr(G) および gr(H) (H に商フィルタリングが与えられた場合) が標準的に識別されます。

G' を他のフィルタリング群および $u : G \to G'$ 準同型フィルタリングと互換性のあるものにしないでください。 G と G' のトポロジの定義は、$u$ が連続であることをすぐに示します (*)。 H が G の部分群 (それぞれ正常部分群) である場合、G 上のものによって H に誘発される位相 (それぞれ G の H に対して商位相) は、G 上のフィルタによって誘発される濾過によって定義される H (それぞれ G/H) 上の位相です。 G の商位相)。 G および G' の積位相は、G および G' の濾過の積によって定義される位相です。

G 上の v を位数写像 (no. 2) とします。G 上の仮定は、G のすべての x、y について $v(xy x^{-1}) = v(y)$、したがって $v(xy^{-1}) = v(yx^{-1}) = v(x^{-1}y) = v(y^{-1}x)$ であることを意味します。$\rho$ を実数として、$0 < \rho < 1$ とします (たとえば

(*) この章では、一般位相、章 III, § 2, no. 8 でいわゆる「連続表現」と呼ばれるものの意味で、語「連続準同型」を使用します。 語 「準同型」は、一般的な位相、章 III, § 2, no. 8、定義 1 の意味で使用されることはありません。この概念では、混乱を避けるために、位数では常に項 「厳密な射」を使用します。

$\rho = 1/e$ とし、G のすべての $x, y$ を $d(x, y) = \rho^{v(xy^{-1})}$ とします。すると、no. 2 の $d(x, x) = 0, d(x, y) = d(y, x)$ と不等式 (5') は次のようになります。

$$
(15) \quad d(x, y) \leq \sup(d(x, z), d(y, z))
$$

G のすべての $x, y, z$ は三角形不等式を意味します

$$
d(x, y) \leq d(x, z) + d(y, z).
$$

したがって、$d$ は左と右の変換の下で不変である G の *擬似計量* であり、G_n は $d(e, x) < \rho^n$ となるような $x \in G$ の集合です。 $d$ によって定義された均一構造は、トポロジカル群 G 上の均一構造になります。 G がハウスドルフの場合、G は *0 次元* 計量可能トポロジカル空間 (*一般位相*, 章 IX, § 6, no. 4) です。 $d$ は、フィルタリング (G_n) も網羅的である場合の G 上の *距離* です。

トポロジカル環 A が与えられた場合、*左トポロジカル A-加群* は A-加群 E であり、その加法群構造と互換性のある位相であり、$A \times E$ から E までの写像 $(a, x) \mapsto ax$ は連続であることを思い出してください (*一般位相*、 章 III, § 6, no. 6）。

#### 命題 3 {#ac-iii-s2-prop-3 .statement tag=04DT}

*A をフィルタリングされた環、(A_n) のフィルタリング、B 部分環 $\bigcup_{n \in \mathbf{Z}} A_n$ の A、E をフィルタリングされた B-加群、(E_n) のフィルタリング、F を E のサブ B モジュール $\bigcup_{n \in \mathbf{Z}} E_n$ とします。次に、写像 $(a, x) \mapsto ax$ が $B \times F$ からF は連続です。*

$a, \in B, x_0 \in F$ にしましょう。 仮定整数 $r, s$ によって、$a_0 \in A_r$ と $x_0 \in E_s$ が存在します。 関係

$$
ax - a_0x_0 = (a - a_0)x_0 + a_0(x - x_0) + (a - a_0)(x - x_0)
$$

$a - a_0 \in A_i$ と $x - x_0 \in E_j$、$ax - a_0x_0$ 属するの場合、

$$
E_{i+s} + E_{j+r} + E_{i+j}.
$$

次に、整数 $n$、$ax - a_0x_0 \in E_n$、$i \geq n - s, j \geq n - r$ と $i + j \geq n$ が与えられた場合、$i$ と $j$ が十分大きいである限り、これが続きます。

#### 系 {#ac-iii-s2-n5-cor-1 .statement tag=04DU}

*環 B はトポロジカル環であり、B-加群 F はトポロジカル B-加群です。*

最初の主張は、適用命題 3 から $F = B$ によって取得されます。

特に、フィルタリングが*徹底的*であるフィルタリングされた環 A はトポロジカル環であることがわかります。そうであれば、濾過が*徹底的*である濾過されたすべての A-加群はトポロジカル A-加群になります。

#### 命題 4 {#ac-iii-s2-prop-4 .statement tag=04DV}

*A を網羅的濾過 (A_n) で濾過した可換環とし、A の理想を p とします。環 $\operatorname{gr}(A)$ の理想 $\operatorname{gr}(p) = \bigoplus_{n \in \mathbf{Z}} (p \cap A_n)/(p \cap A_{n+1})$ が素数であるとします。このとき、A における p の閉包は主イデアルです。*

gr(A/p) は gr(A)/gr(p) (no. 4, 命題 2) と同型であるため、整域であることがわかっています。私たちは結論する、$A / \bigcap_{n \in \mathbf{Z}} (p + A_n)$ は整域 (no. 3、系から命題 1) です。その場合、$p$ の終結 $\bigcap_{n \in \mathbf{Z}} (p + A_n)$ が最も理想的です。

Let $A$ be a ring and $m$ a two-sided ideal of $A$; the topology defined on $A$ by the $m$-adic filtration (no. 1, Example 3) is called the *m-adic topology*; as the *m*-adic filtration is exhaustive, $A$ is a topological ring with this topology (Corollary to Proposition 3). 同様に、すべての $A$ モジュール $E$ について、$m$ 進フィルタリングによって定義された位相は、$E$ の *m 進数位相* と呼ばれます。 $E$ は、この位相の下のトポロジカル $A$ モジュールです。

$m'$ を $A$ の両面理想である他のとします。 $A$ の $m'$ 進数位相が $m$ 進数位相よりも *より細かい* であるためには、 ${m'}^n \subset m$ となるような整数 $n > 0$ が存在することが必要かつ十分です。 条件は必要であり、それが満たされる場合、すべての $h > 0$ に対して ${m'}^{hn} \subset m^h$ となるため、条件で十分です。 If $A$ is a *commutative Noetherian ring*, it amounts to the same to say that $V(m) \subset V(m')$ in the prime spectrum of $A$ (Chapter II, § 4, no. 3, Corollary 2 to Proposition 11 and § 2, no. 6, Proposition 15).

### 6. フィルタリングが完了しました加群

#### 命題 5 {#ac-iii-s2-prop-5 .statement tag=04DW}

*$G$ をフィルター処理された群とし、そのフィルター $(G_n)$ は $G$ の不変式部分群で構成されます。次の条件は同等です:*

(a) $G$ は完全なトポロジー 群です。

(b) *関連ハウスドルフ群* $G' = G / (\bigcap_{n \in \mathbf{Z}} G_n)$ *完備*。

(c) *$G$ のすべての Cauchy 数列は収束します*。

* $G$ が可換で加法的に記述された場合、これらの条件は以下と同等です:*

(d) *各族* $L$の有限部分集合の補数のフィルタ$\mathscr{F}$に関して0に収束する$G'$の元の$(x_\lambda)_{\lambda \in L}$は$G'$*で加算可能です。

$G$ のフィルターがコーシー フィルター (または収束フィルター) であるためには、標準写像 $G \to G'$ の下の像がコーシー (それぞれ収束) フィルター (*一般位相*、章 II, § 3, no. 1、命題) であることが必要かつ十分です。 4); よってまず​​は (a) と (b) の同値です。一方、$G'$ は計化可能であるため、*General 位相* の命題 9、章 IX, § 2, no. 6 から (b) と (c) の同値が続きます。

ここで、$G$ が可換であると仮定します。 $G'$ が完全であると仮定し、$(x_\lambda)_{\lambda \in L}$ を $\mathscr{F}$ に関して 0 に収束する $G'$ の元の族とする。 For every neighbourhood $V'$ of 0 in $G$ which is a subgroup of $G'$, there exists a finite subset $J$ of $L$ such that the condition $\lambda \in L - J$ implies $x_\lambda \in V'$; then $\sum_{\lambda \in H} x_\lambda \in V'$ for every finite subset $H$ of $L$ not meeting $J$, which shows that the family $(x_\lambda)_{\lambda \in L}$ is summable (*General Topology*, Chapter III, § 5, no. 2, Theorem 1).

逆に、条件 (d) が成り立ち、$(x_n)$ を $G'$ 上のコーシー 数列とします。ファミリ $(x_{n+1} - x_n)$ は加算可能であり、特に一般的な項 $x_{n+1} - x_n$ を持つ系列は収束するため、数列 $(x_n)$ は収束します。

$G$ を、濾過された群とし、その濾過 $(G_r)$ は、$G$ の通常の部分群で構成されます。 剰余群 $G/G_n$ は *個別* であり、したがって完全です。なぜなら、$G_r$ は $G$ で開いているからです。 $f_n$ を標準写像 $G \to G/G_n$ とし、$m \leq n$ について $f_{mn}$ を標準写像 $G/G_n \to G/G_m$ とします。 $(G/G_n, f_{mn})$ は、離散群の逆系で、$\mathbf{Z}$ がインデックス集合 (*一般的な位相*、章 III, § 7, no. 3) として使用されます。 Let $\tilde{G}$ be the topological group the inverse limit of this inverse system and for all $n$ let $g_n : \tilde{G} \to G/G_n$ be the canonical mapping; let $f : G \to \tilde{G}$ be the inverse limit of the inverse system of mappings $(f_n)$ such that $f_n = g_n \circ f$ for all $n$; finally, let $j$ be the canonical mapping of $G$ to its Hausdorff completion $\hat{G}$; as the $G/G_n$ are complete, there exists a unique topological group isomorphism $i : \hat{G} \to \tilde{G}$ such that $f = i \circ j$ (*loc. cit.*, Corollary 1 to Proposition 2); we shall call it the *canonical* isomorphism of $\hat{G}$ onto $\tilde{G}$.

$H$ を他の濾過された群とし、その濾過 $(H_r)$ は通常の $H$ の部分群で構成され、$u : G \to H$ を濾過 (no. 4) と互換性のある準同型とします。 Set $\tilde{H} = \lim H/H_n$; for all $n$, $u$ defines by taking quotients a homomorphism $u_n : G/G_n \to H/H_n$ and the $u_n$ obviously form an inverse system of mappings; set $\tilde{u} = \lim u_n$. さらに、$\hat{H}$ を、$u$ から移行によってハウスドルフ完全化 (*一般位相*、章 II, § 3, no. 7、命題 15) に導出された $H$ および $ti : \hat{G} \to H$ 準同型のハウスドルフ完全化とします。 定義からすぐに、標準同型によって $\hat{G}$ が $\tilde{G}$ と同一視され、$\hat{H}$ が $\tilde{H}$ と同一視される場合、$ti$ は $\tilde{u}$ と同一視されます。 特に、結論するは、すべての $n$ に対して、$u_n$ が同型である場合、$ti$ はトポロジー 群の同型であると考えます。

*群と環* を完全にフィルタリングしたもののうちの例

#### 例 1 {#ac-iii-s2-n6-exa-1 .statement tag=04DX}

$G$ を完全にフィルタリングされた群とします。誘導濾過を伴う $G$ のすべての *closed* 部分群が完了します (*一般位相*、章 II, § 3, no. 4、命題 8)。 商を含む $G$ のすべての剰余群で濾過が完了します (*一般位相*、章 IX, § 3, no. 1、*注意* 1)。

#### 例 2 {#ac-iii-s2-n6-exa-2 .statement tag=04DY}

$A$ をフィルタリングされた可換環とし、そのフィルタリングを $(a_n)_{n \in \mathbf{Z}}$ で表します。 $A'$ を正式な冪系列 $A[[X_1, \ldots, X_s]]$ の環とします。すべての $e = (e_1, \ldots, e_s) \in \mathbf{N}^s$ について、$|e| = \sum_{i=1}^s e_i$、$X^e = \prod_{i=1}^s X_i^{e_i}$ と書き、すべての元 $P \in A'$ を一意に$P = \sum_{e \in \mathbf{N}^s} \alpha_{e,P} X^e$ $\alpha_{e,P} \in A$ に書き込むことができます。すべての $n \in \mathbf{Z}$ について、$a'_n$ が $P \in A'$ の集合を表し、すべての $e \in \mathbf{N}^s$ が $\alpha_{e,P} \in a_{n-|e|}$ になるようにします。 $a'_n$ が $A'$ の *理想* であることを示します。明らかに、$a'_n$ は $A'$ の添加物部分群です。一方、$P \in a'_n$ と $Q \in A'$ の場合は、すべて $e \in \mathbf{N}^s$、$\alpha_{e,PQ} = \sum_{e'+e''=e} \alpha_{e',Q}\alpha_{e'',P}$ になります。 関係 $e' + e'' = e$ は $|e''| \leq |e|$、$PQ \in a'_n$ を意味します。さらに、$Q \in a'_m$ の場合、$e' + e'' = e$ については、$\alpha_{e',Q}\alpha_{e'',P} \in a_{m-|e'|}a_{n-|e''|} \subset a_{m+n-|e|}$ となり、$(a'_n)_{n \in \mathbf{Z}}$ が$A'$ の環構造と互換性のある *フィルタリング* であることが証明されます (明らかに $1 \in a'_0$ の場合)。将来、$A'$ を濾過された環として話す場合、別の言い方をすれば、濾過 (ああ) を伴う 〜でない限りを意味することになります。明らかに、$\bigcap_{n \in \mathbf{Z}} a'_n$ は正式な冪系列の集合であり、そのすべての係数属するから $\bigcap_{n \in \mathbf{Z}} a_n$ です。 $A$ がハウスドルフであれば、$A'$ もハウスドルフです。 $a_0 = A$なら、$a'_0 = A'$。

#### 命題 6 {#ac-iii-s2-prop-6 .statement tag=04DZ}

※上記記法において、$a_0 = A$とし、写像$P \mapsto (\alpha_{e,P})_{e \in \mathbf{N}^s}$を$h$とします。次に、$h$ は、加法トポロジカル群 $A^{\mathbf{N}^s}$ 上の加法トポロジー 群 $A$ の同型です。 多項式環 $A[X_1, \ldots, X_s]$ は $A'$ に密集しています。 $A$ が完了すると、$A'$ も完了します。*

明らかに $h$ は全単射です。 $V_n = h(a'_n)$ は $(a_e) \in A^{\mathbf{N}^s}$ の集合であり、すべての $e \in \mathbf{N}^s$ に対して $a_e \in a_{n-|e|}$ となり、$|e| \leq n$ になります。これらの元 $e$ は数で有限であるため、$V_n$ は $A^{\mathbf{N}^s}$ の 0 の近傍です。 逆に、$V$ が $A^{\mathbf{N}^s}$ の 0 の近傍である場合、$\mathbf{N}^s$ の有限部分集合 $E$ と整数 $v$ があり、すべての $e \in E$ に対して条件 $a_e \in a_v$ が暗黙的に表されます。 $(a_e) \in V$; $n$ が $e \in E$ の整数 $v + |e|$ の最大のである場合、$h(a'_n) \subset V$ となり、命題 6 の最初の主張が証明されます。

さらに、$n$と$E$を上記のように定義すると、すべての$P \in A'$に対して$h(P - \sum_{e \in E} \alpha_{e,P}X^e) \in V$となり、$A'$では$A[X_1, \ldots, X_s]$が密であることがわかります。 最後の主張は最初から続き、空間が完了したものの積が完了したという事実です。

Let $m$ be an ideal of $A$ and suppose that $(a_i)$ is the $m$-adic filtration; then, if $n$ is the ideal of $A'$ generated by $m$ and the $X_i$ ($1 \leq i \leq s$), the filtration $(a_i)$ is the $n$-adic filtration. 明らかに、すべての $k \geq 0$ に対して、$n^k$ は、$|e| \leq k$、よって $n^k \subset a \&$ のように、すべての $e \in \mathbf{N}^s$ に対して $a \in m^{k-|e|}$ となるように、元 $aX^e$ によって生成されます。 逆に$a'_k \subset n^k$を証明してみましょう。 すべての $P \in a'_k$、$P = P' + P''$、ここで $P' = \sum_{|e| < k} \alpha_{e,P}X^e$、$P'' = \sum_{|e| \geq k} \alpha_{e,P}X^e$。 明らかに、$P'' = \sum_{|e|=k} X^e Q_e$ と書くことが可能です。ここで、$Q_e$ は、$A'$、よって $P'' \in n^k$ の元です。一方、$e \in \mathbf{N}^s$、よって $P' \in n^k$ はすべて明らかに $\alpha_{e,P}X^e \in n^k$ です。 次に$n^k = a'_k$。

#### 系 {#ac-iii-s2-n6-cor-1 .statement tag=04E0}

*$A$を可換環とすると、

$$
A' = A[[X_1, \ldots, X_s]]
$$

*$s$ の正式な冪系列の環は、定数項を持たずに、正式な冪系列の$A'$ からなるの理想を $A$ と $n$ 上で不定とします。 環 $A'$ はハウスドルフであり、n 進数位相と完全* であり、多項式環 $A[X_1, \ldots, X_s]$ は $A'$ のどこでも密集しています。

今述べたことを$m = \{0\}$のケースに適用すれば十分です。

### 7. 完全にフィルタリングされた加群の線形コンパクトネス特性

E が A-加群の場合、E のアフィン部分集合 (またはアフィン線形多様体) は、空の部分集合 F または形 $a + M$ です。ここで、$a \in E$ および M は、F の方向 (代数, と呼ばれる) E の部分加群です。 章 II, § 9、番号 1 および 3)。

#### 命題 7 {#ac-iii-s2-prop-7 .statement tag=04E1}

A をフィルタリングされた環、E をフィルタリングされた A-加群および $(E_n)$ のフィルタリングとします。 $E_0 = E$、$E_n$ は E の部分加群、A-加群 $E/E_n$ はアルティン、そして最後にトポロジカル群 E はハウスドルフで完全であると仮定します。このとき、E の空でない閉アフィン部分集合の減少列の共通部分は空ではありません。

no. 6 で、E はハウスドルフで完全なので、$\tilde{E} = \lim_{\leftarrow} E/E_n$ と同一視されることが分かりました。 $(W_p)$ を E の空でない閉じたアフィン部分集合の減少列とし、すべての $n \geq 0$ について、$W_{p,n}$ を $E/E_n$ の $W_p$ の標準像とします。すべての $p$ とすべての $n$ に対して $x_n \in W_{p,n}$ となるように構成する数列 $x = (x_n) \in \tilde{E}$ を実行します。したがって、すべての $p$ とすべての $n$ に対して $x \in W_p + E_n$ が得られ、$W_p$ が閉じているため、すべての $p$ (no. 5) に対して $x \in W_p$ となり、命題が証明されます。

$E/E_0 = 0$として、$x_0 = 0$とします。 $x_i$ が $0 \leq i \leq n - 1$ に対して定義されており、$W'_{p,n}$ が $E/E_{n-1}$ の標準像が $x_{n-1}$ である $W_{p,n}$ の元の集合であるとします。 $x_{n-1} \in W_{p,n-1}$ と $W_{p,n-1}$ は $W_{p,n}$ の標準像であるため、$W'_{p,n}$ は空ではなく、明らかに $E/E_n$ のアフィン部分集合です。また、数列 $(W'_{p,n})_{p \in \mathbf{N}}$ は減少するです。 $E/E_n$ がアルティンであるため、この数列は静止しています (そうでないと、$W'_{p,n}$ の方向である $E/E_n$ の部分加群の数列が真に減少するになります。これは不合理です)。したがって、$x_n$ を $\bigcap_{p \in \mathbf{N}} W'_{p,n}$ の元にするだけで十分であり、$(x_n)$ の構成は、帰納法によって実行できます。

#### 命題 8 {#ac-iii-s2-prop-8 .statement tag=04E2}

A と E 満たすが命題の仮説であるとします。 7. $(F_p)$ を、$\bigcap F_p = 0$ となるような E の閉じた部分加群の減少列とします。次に、E の 0 のすべての近傍 V に対して、$F_p \subset V$ となるような $p$ が存在します (他の語、フィルター $(F_p)$ の基底は 0 に収束します)。

V は $E_n$ の 1 つであると想定できます。この場合、$E/V$ はアルティンになります。 $F'_p = (F_p + V)/V$ と書きましょう。 $E/V$ の部分加群の $F'_p$ 形減少列のように、すべての $p > j$ に対して $F'_p = F'_j$ となる整数 $j$ が存在します。 $F'_j = \{0\}$ が表示され、証明が完了します。 $x \in F'_j$ と W を F の元の集合とし、$E/V$ の像は $x$ ($p \geq j$) です。 j の定義による W は、E の空ではない閉じたアフィン部分集合であり、明らかに $W_{p+1} \subset W$ です。

次に、命題 7 から、すべての W, に対して元 y 所属が存在することがわかります。 Wとして、$\subset F,$と$\bigcap_{p \in \mathbf{N}} F_p = \{0\}, y = 0$。 E/V では x は y の標準像であるため、$x = 0$ (cf. 練習問題 15 ～ 21)。

### 8. 関連グレード加群の準同型中挙上

#### 定理 1 {#ac-iii-s2-thm-1 .statement tag=04E3}

X、Y を 2 つのフィルター 群とし、そのフィルター $(X_n), (Y_n)$ は通常の部分群で構成されます。 $u : X \to Y$ を濾過と互換性のある準同型にします。

(i) 濾過 $(X_n)$ が徹底的であると仮定します。 $\mathrm{gr}(u)$ が単射であるためには、すべての $n \in \mathbf{Z}$ に対して $\bar{u}^{-1}(Y_n) = X_n$ であることが必要かつ十分です。

(ii) 次の仮説のいずれかが成立すると仮定します。(α) X は完全であり、Y Hausdorff です。 (β) Y は離散的です。次に、$\mathrm{gr}(u)$ が全射的であるためには、すべての $n \in \mathbf{Z}$ に対して $Y_n = u(X_n)$ であることが必要かつ十分です。

(i) 写像 $\mathrm{gr}_n(u)$ が単射であると言うことは、次のことを意味します。
$$
X_n \cap \bar{u}^{-1}(Y_{n+1}) \subset X_{n+1}.
$$
$(Y_{n+1}) = X_{n+1}$ の場合は明らかにこれに当てはまります。逆に、もし
$$
X_n \cap \bar{u}^{-1}(Y_{n+1}) \subset X_{n+1}
$$
すべての $n$ について、$k$ の帰納法によって、すべての $n \in \mathbf{Z}$ とすべての $k \geq 0$ について $X_{n-k} \cap \bar{u}^{-1}(Y_{n+1}) \subset X_{n+1}$ が推定されます。濾過 $(X_n)$ が徹底的であるため、すべての $n$ に対して、$X_n$ は $X_{n-k}$ ($k \geq 0$) の和集合であるため、すべての $n$ に対して $\bar{u}^{-1}(Y_{n+1}) \subset X_{n+1}$、したがって $X_{n+1} \subset \bar{u}^{-1}(Y_{n+1})$ となり、完了することがわかります。 証明。

(ii) 写像 $\mathrm{gr}_n(u)$ が全射であると言うことは、次のことを意味します。
$$
Y_n = u(X_n)Y_{n+1}.
$$
すべての $n \in \mathbf{Z}$ に対して $Y_n = u(X_n)Y_{n+1}$ の場合、これは明らかに当てはまります。 $n$ を $Y_n$ の整数と $y$ 元とします。すべての $k \geq 0$ に対して $x_k \in X_n$、$x_{k+1} \equiv x_k \pmod{X_{n+k}}$、および $u(x_k) \equiv y \pmod{Y_{n+k}}$ となるように、$X_n$ の元の定義する数列 $(x_k)_{k \geq 0}$ を計算します。 X の単位元に等しい $x_0$ を取得すると、確かに $u(x_0) \equiv y \pmod{Y_n}$ が得られます。 $x_k \in X_n$ が $u(x_k) \equiv y \pmod{Y_{n+k}}$ になるように構築されたとします。それから$(u(x_k))^{-1}y \in Y_{n+k}$; 仮定は、$u(t) \equiv (u(x_k))^{-1}y \pmod{Y_{n+k+1}}$、したがって $u(x_k t) \equiv y \pmod{Y_{n+k+1}}$ となるような $t \in X_{n+k}$ が存在することを意味します。 帰納法を実行するには、$x_{k+1} = x_k t$を取るだけで十分です。したがって、Y が離散であれば、$Y_{n+k} = \{e'\}$ (Y の単位元)、よって $u(x_k) = y$ という$k \geq 0$ が存在するので、この場合、すべての $n$ に対して $u(X_n) = Y$ であることが証明されます。ここで、X が完了し、Y Hausdorff が完成したとします。 $h \geq k \geq 0$ に対する $x_h^{-1} x_k \in X_{n+k}$ と同様に、$(x_k)$ は $X_n$ のコーシー 数列です。として

X_n は X で閉じられているため完全です。この数列には X_n に少なくとも 1 つの極限 x があります。 u の連続性により、u(x) は Y 内の数列 (u(x_k)) の一意の極限であり、Y はハウスドルフです。しかし、関係 u(x_k) \equiv y (\text{mod. } Y_{n+k+1}) は、y がこの数列, よって $u(x) = y$ の極限であることを示し、$u(X_n) = Y_n$ であることも証明されています。

#### 系 1 {#ac-iii-s2-thm-1-cor-1 .statement tag=04E4}

*X がハウスドルフであり、その濾過が徹底的であると仮定します。次に、gr(u) が単射であれば、u は単射です。*

e、e'をそれぞれXの単位元、Yとする。それから
$$
\bar{u}^{-1}(e') \subset \bigcap_n \bar{u}^{-1}(Y_n) = \bigcap_n X_n = \{e\}
$$
仮定、よって系による。

#### 系 2 {#ac-iii-s2-thm-1-cor-2 .statement tag=04E5}

*次のいずれかの仮説が成り立つと仮定します。*
$(\alpha)$ *X は完了し、Y はハウスドルフであり、その濾過は徹底的です。*
$(\beta)$ *Y は離散的であり、その濾過は徹底的です。*
*そして、gr(u) が全射であれば、u は全射です。*

この場合は$Y = \bigcup_n Y_n = \bigcup_n u(X_n) \subset u(X)$です。

#### 系 3 {#ac-iii-s2-thm-1-cor-3 .statement tag=04E6}

*X と Y がハウスドルフであり、X と Y の濾過が網羅され、X が完了したと仮定します。次に、gr(u) が全単射であれば、u は全単射になります。*

A を局所環、m をその最大理想、M を A-加群とします。 A と M に *m-adic* フィルタリングが与えられ、gr(A) と gr(M) が等級付けされた環と A と M に関連付けられた等級付けされた gr(A) モジュールであるとします。 標準写像 (11) が常に *全射的*であることを確認しました (no. 3, 例 3)。 M の次の性質を考慮します。
*(GR)* *標準写像*
$$
\gamma_M : \operatorname{gr}(A) \otimes_{\operatorname{gr}_0(A)} \operatorname{gr}_0(M) \to \operatorname{gr}(M)
$$
*は全単射*です。

#### 命題 9 {#ac-iii-s2-prop-9 .statement tag=04E7}

*A を局所環、m をその最大イデアル、M、N を 2 つ A-加群とし、u : N \to M を A 準同型とする。 M と N に m 進フィルタリングが与えられ、次のように仮定します。 (1) M は性質 (GR) を満たす。 (2) \operatorname{gr}_0(u) : \operatorname{gr}_0(N) \to \operatorname{gr}_0(M) は単射法です。この場合、 \operatorname{gr}(u) : \operatorname{gr}(N) \to \operatorname{gr}(M) は単射法であり、N と P = \operatorname{Coker}(u) 満たす性質 (GR) と整数 $n > 0$ ごとに $m^n N = \bar{u}^{-1}(m^n M)$ となります。*

図式であることがすぐに確認されます。
$$
\begin{array}{ccc}
\operatorname{gr}(A) \otimes_{\operatorname{gr}_0(A)} \operatorname{gr}_0(N) & \xrightarrow{1 \otimes \operatorname{gr}_0(u)} & \operatorname{gr}(A) \otimes_{\operatorname{gr}_0(A)} \operatorname{gr}_0(M) \\
\downarrow \gamma_N & & \downarrow \gamma_M \\
\operatorname{gr}(N) & \xrightarrow{\operatorname{gr}(u)} & \operatorname{gr}(M)
\end{array}
$$

可換です。 $\mathrm{gr}_0(A) = A/m$ は体であるため、仮定は $1 \otimes \mathrm{gr}_0(u)$ が単射であることを意味します。 仮定 $\gamma_M$ は単射法であるため、$\gamma_M \circ (1 \otimes \mathrm{gr}_0(u))$ も単射法です。これは、まず、$\gamma_N$ が単単射であるため全単射であり、したがって $\mathrm{gr}(u)$ が単射であることを意味します。 公式 $\tilde{u}^1(m^nM) = m^nN$ は、定理 1 (i) の帰結になります。

また、$N' = u(N)$と書いて、$j : N' \to M$を標準単射とします。 $p : M \to P = M/N'$ が標準準同型の場合、可換式では図式

$$
\begin{array}{ccccccccc}
\mathrm{gr}(A) \otimes \mathrm{gr}_0(N') & \xrightarrow{1 \otimes \mathrm{gr}_0(j)} & \mathrm{gr}(A) \otimes \mathrm{gr}_0(M) & \xrightarrow{1 \otimes \mathrm{gr}_0(p)} & \mathrm{gr}(A) \otimes \mathrm{gr}_0(P) & \to & 0 \\
\downarrow \gamma_{N'} & & \downarrow \gamma_M & & \downarrow \gamma_P & & \\
\mathrm{gr}(N') & \xrightarrow{\mathrm{gr}(j)} & \mathrm{gr}(M) & \xrightarrow{\mathrm{gr}(p)} & \mathrm{gr}(P) & \to & 0
\end{array}
$$

下の行は正確 (no. 4, 命題 2) であり、no. 4 の命題 2 と $\mathrm{gr}_0(A)$ が体であるという事実により、上の行も同様です。さらに、$\mathrm{gr}(j)$ は単射 (no. 4, 命題 2) であるため、$\mathrm{gr}_0(j)$ は単射です。 $j$ に適用される議論の最初の部分は、$\gamma_{N'}$ が全単射であることを示しています。 $\gamma_M$ も仮定によって全単射であるため、結論するは $\gamma_P$ が全単射であると考えられます (章 I, § 1, no. 4、系 2 から命題 2)。

#### 系 {#ac-iii-s2-n8-cor-1 .statement tag=04E8}

命題 9 の仮説の下で、$N$ が $m$ 進濾過を備えたハウスドルフであると仮定すると、$u$ は単射的になります。

これは、$\mathrm{gr}(u)$ が単射法 (系 1 から定理 1) であるという事実からわかります。

\* 注意。 命題 9 の仮説が成立し、さらに次の条件のいずれかが成立すると仮定します。
(1) $m$ は無能です。
(2) $A$ はネーター で、$P$ は理想的にはハウスドルフ (cf. § 5, no. 1) です。
その場合、$P$ はフラットな $A$ モジュールです。これは、$A/m$ が体であるため、$\gamma_P$ が全単射であり、§ 5, no. 2, 定理 1 (iv) であるという事実から続きます。 \*

### 9. 関連するグレード加群の元の家族の挙上

$A$ をフィルタリングされた可換環、$(A_n)_{n \in \mathbf{Z}}$ そのフィルタリング、および $A$ の $C$ 部分環を$C \cap A_1 = \{0\}$ とする。 標準写像 $A_0 \to A_0/A_1 = \mathrm{gr}_0(A)$ の制限から $C$ は単射法なので、 $\mathrm{gr}_0(A)$ の部分加群で同一視する $C$ が可能になります。これは、同様の場合に通常行うことです。 $A_1 \neq A$ で、$K$ が $A$ のいずれかの部分体である場合、$K \cap A_1$ は含む 1 ではなく $K$ の理想であるため、$K \cap A_1 = (0)$ になります。その場合、$K$ は $\mathrm{gr}_0(A)$ の部分体と同一視される可能性があります。

#### 命題 10 {#ac-iii-s2-prop-10 .statement tag=04E9}

Let $A$ be a filtered commutative ring and $(A_n)$ its filtration; suppose that there exists a subring $C$ of $A_0$ such that $C \cap A_n = \{0\}$ and $C$ is identified with a subring of $\mathrm{gr}_0(A)$. $(x_i)_{1 \leq i \leq q}$ を $A$ の元の有限族とする。 $1 \leq i \leq q$ に対して $x_i \in A_n$ を仮定し、$\xi_i$ を $1 \leq i \leq q$ に対して $\mathrm{gr}_{n_i}(A)$ の $x_i$ の類とします。

(i) $\mathrm{gr}(A)$ の元の族 $(\xi_i)$ が $C$ に対して代数的に自由である場合、族 $(x_i)$ は $C$ に対して代数的に自由です。

(ii) $A$ のフィルタリングが網羅的かつ離散的で、$(\xi_i)$ が $C$-代数 $\mathrm{gr}(A)$ の生成元の系である場合、$(x_i)$ は $C$-代数の生成元の系です。 $A$。

$A'$ を $\mathbf{C}$ 上の多項式代数 $\mathbf{C}[X_1, \ldots, X_q]$ とします。 $A'$ に型 $\mathbf{Z}$ の目盛 $(A'_n)$ を与えます。ここで、$A_n$ は、$\sum_{i=1}^q n_i s(i) = n$ となるような単項式 $X_1^{s(1)} \ldots X_q^{s(q)}$ の $\mathbf{C}$ 線形結合の集合です。 $\mathbf{C}$-代数 $A'$ から $\mathbf{C}$-代数 $A$ まで、$u$ を準同型 $f \mapsto f(x_1, \ldots, x_q)$ とします。すべての $n \in \mathbf{Z}$ に対して定義、$u(A'_n) \subset A_n$ が含まれるため、$u$ は、そのグレードの環構造、cf. no. 1 に関連付けられたフィルタリングされた環構造が与えられているため、$(A')$ と互換性があります。 例 1)。そうすると、(i)の仮定は、

$$
\mathrm{gr}(u): A' = \mathrm{gr}(A') \to \mathrm{gr}(A)
$$

は単射です。 $A'$ の濾過は網羅的で分離されているため、no. 8 の系 1 から定理 1 が適用でき、$u$ は単射的であり、これは (i) の結論を証明します。同様に、(\&) 上の仮定 (ii) は、$\mathrm{gr}(u)$ が全射であることを意味します。 $A$ は離散的であり、その濾過は網羅的であるため、no. 8 の系 2 ～ 定理 1 は適用でき、$u$ は全射的であり、(ii) の結論を証明します。

#### 命題 11 {#ac-iii-s2-prop-11 .statement tag=04EA}

$A$ を、$C \cap A_n = 0$ と $(x_i)_{1 \leq i \leq q}$ が $x_i \in A_{n_i}$ となるような $A$ の元の有限族であるように、$A_0$ の可換環、$C$ 部分環を完全なハウスドルフフィルタリングしたものとします。 $1 \leq i \leq q$の場合は$n_i > 0$。 $\xi_i$ を $1 \leq i \leq q$ の $\mathrm{gr}_{n_i}(A)$ の $x_i$ の類とします。

(i) 形式冪系列 $A'' = \mathbf{C}[[X_1, \ldots, X_q]]$ から $A$ の代数から $1 \leq i \leq q$ に対して $v(X_i) = x_i$ となるような固有の $C$ 準同型写像 $v$ が存在します。

(ii) 族 $(\xi_i)$ が $C$ 上で代数的に自由である場合、 準同型 $v$ は単射的です。

(iii) $A$ のフィルタリングが網羅的であり、族 $(\xi_i)$ が $C$-代数 $\mathrm{gr}(A)$ の生成元の系である場合、準同型 $v$ は全射的です。

すべての $i$ に対して $n_i \geq 1$、すべての単項式 $X_1^{s(1)} \ldots X_q^{s(q)}$ に対して $\sum_{i=1}^q n_i s(i) \geq \sum_{i=1}^q s(i)$、そして逆に、$r$ が $n_i$ の最大のである場合、$\sum_{i=1}^q n_i s(i) \leq r \cdot \sum_{i=1}^q s(i)$ となります。 $A''_n$ が、非ゼロ項 $a_s X_1^{s(1)} \ldots X_q^{s(q)}$ 満たす $\sum_{i=1}^q n_i s(i) \geq n$ の公式冪系列の集合を表す場合、no. 6、系から命題 6 は次のようになります。 $A''$ はハウスドルフであり、徹底した濾過が完了しています $(A''_n)$ と

$$
A' = \mathbf{C}[X_1, \ldots, X_q]
$$

is dense in $A''$; moreover the homomorphism $u$ defined in the proof of Proposition 10 is continuous on $A'$ and can be extended uniquely to a continuous homomorphism $v : A \to A$, since $A$ is Hausdorff and complete (General Topology, Chapter III, § 3, no. 3, Proposition 5), which proves (i); also, $\mathrm{gr}(A'') = \mathrm{gr}(A')$ and $\mathrm{gr}(v) = \mathrm{gr}(u)$; (ii) and (iii) then follow respectively from Corollaries 1 and 2 to Theorem 1 of no. 8 in view of the hypotheses on $A$.

命題の(ii)(それぞれ(iii))の結論は、というによって表されるときどきであり、家族$(x_i)$は$C$(それぞれ$A$の生成元の正式な系)に対して形式的に自由であるということである。

#### 命題 12 {#ac-iii-s2-prop-12 .statement tag=04EB}

$A$ をフィルタリングされた環、$E$ をフィルタリングされた $A$ モジュール、$(A_n)$ と $(E_n)$ を $A$ と $E$ でのそれぞれのフィルタリングとします。 $A$が完了し、濾過$(E_n)$が徹底的に行われて分離されたとします。 $(x_i)_{i \in I}$ を $E$ の元の有限族とし、$i \in I$ について、$n(i)$ を $x_i \in E_{n(i)}$ となるような整数とします。最後に、$\xi_i$ を $\mathrm{gr}_{n(i)}(E)$ の $x_i$ の類とします。次に、$(\xi_i)$ が $\mathrm{gr}(A)$ モジュール $\mathrm{gr}(E)$ の生成元の系である場合、$(x_i)$ は $A$ モジュール $E$ の生成元の系です。

$A$ モジュール $L = A'$ で、$L_0$ が集合 $(a_i)$ を表し、すべての $i \in I$ に対して $a_i \in A_{n - n(i)}$ となるようにします。 $p$ と $q$ が最小で、$n(i)$ の最大のである場合、$L$ で定義 $(L_n)$ が定義される $A^I_{n-q} \supset L_0 \supset A^I_{n-p}$ と位相は、積位相と同じです。したがって、$L$ は完全にフィルタリングされた $A$ モジュールです。 $L$ は自由であるため、$u((a_i)) = \sum_{i \in I} a_i x_i$ となるような $A$ 線形マッピング $u : L \to E$ が存在し、明らかにフィルタリングと互換性があります。私たち証明しなければならないは $u$ が全射法であり、このためには、系 2 から定理 1、no. 8 によって、次のことを示すだけで十分です。

$$
\mathrm{gr}(u) : \mathrm{gr}(L) \to \mathrm{gr}(E)
$$

は全射的、またはすべての $x \in E_n$ に対して、すべての $i \in I$ と $x \equiv \sum_{i \in I} a_i x_i \pmod{E_{n+1}}$ に対して $a_i \in A_{n-n(i)}$ となるような族 $(a_i)$ が存在するとも言えます。 $\xi$ を $\mathrm{gr}_n(E)$ の $x$ の類とします。 $\xi_i$ 生成すると $\mathrm{gr}(A)$ モジュール $\mathrm{gr}(E)$ なので、 $\xi = \sum_{i \in I} \alpha_i \xi_i$ となるような $\alpha_i \in \mathrm{gr}(A)$ が存在し、必要に応じて置き換えることによって $\alpha_i \in \mathrm{gr}_{n-n(i)}(A)$ が同次の成分によって $\alpha_i$ になると仮定することができます。 次数 $n - n(i)$。この場合、$\alpha_i$ は元 $a_i \in A_{n-n(i)}$ の像であり、家族 $(a_i)$ には必要な性質が含まれます。

#### 系 1 {#ac-iii-s2-prop-12-cor-1 .statement tag=04EC}

$A$ を完全にフィルタリングされた環とし、$E$ をフィルタリングされた $A$ モジュールとし、そのフィルタリングは徹底的で分離されています。 $\mathrm{gr}(E)$ が有限生成 (それぞれネーター) $\mathrm{gr}(A)$ モジュールである場合、 $E$ は有限生成 (それぞれネーター) $A$ モジュールです。

$\mathrm{gr}(E)$ が有限生成される場合、同種生成元の有限系が存在し、命題 12 は $E$ が有限生成されることを示します。ここで、$\mathrm{gr}(E)$ がネーター で、$F$ が $E$ の部分加群であるとします。 $E$ の濾過によって $F$ に引き起こされる濾過は網羅的で分離され、$\mathrm{gr}(F)$ は gr(E) のサブ gr(A) モジュール (no. 4, 命題 2) で識別されるため、仮定によって有限的に生成されます。私たちは結論する、Fは有限生成A-加群であるため、Eはネーターです。

#### 系 2 {#ac-iii-s2-prop-12-cor-2 .statement tag=04ED}

A を、濾過が徹底的である完全なハウスドルフ濾過された環とします。 gr(A) が左ネーター環の場合、A も同様です。

E = A で系を適用する 1 とすれば十分です。

#### 系 3 {#ac-iii-s2-prop-12-cor-3 .statement tag=04EE}

Aを完全にフィルタリングされた環、(A_n)そのフィルタリング、EをハウスドルフフィルタリングされたA-加群、(E_n)そのフィルタリング、およびFをEの有限生成された部分加群とします。 A_∞ = A、E_0 = E と仮定します。

(i) すべての k ≥ 0 について、E_k = E_{k+1} + A_k F の場合、F = E。
(ii) さらに、E の濾過が A の濾過から導出されると仮定すると (no. 1, 例 2)、関係 E = E_1 + F は F = E を意味します。

ξ_i (1 ≤ i ≤ n) を類 mod とします。 F の生成元の有限系の E_1。 It follows from the given hypothesis that for all k ≥ 0 every element of gr_k(E) can be expressed in the form $\sum_{i=1}^n \alpha_i \xi_i$ where $\alpha_i \in \mathrm{gr}(A)$; the $\xi_i$ therefore generate the gr(A)-module gr(E), which proves (i) by virtue of Proposition 12. E の濾過が A の濾過から導出される場合、関係 E = E_1 + F は次のことを意味します。

$$
E_k = A_k E = A_k E_1 + A_k F = A_k A_1 E + A_k F \subset A_{k+1} E + A_k F \\
= E_{k+1} + A_k F \subset E_k,
$$

よって (ii)。

#### 命題 13 {#ac-iii-s2-prop-13 .statement tag=04EF}

A を環とします。A と E A-加群のヤコブソン根基に含まれる A の両面イデアルです。 A と E に m 進フィルタリング (no. 1, 例 3) が与えられるとします。次の条件のいずれかが成立すると仮定します。
(a) E は有限生成A-加群、A はハウスドルフです。
(b) m は無能です。

E が自由A-加群であるためには、E/mE がフリー (A/m) モジュールであること、および E 満たす性質 (GR) (no. 8) であることが必要かつ十分です。

If E is a free A-module and $(e_\lambda)$ a basis of E, $m^k E$ is the direct sum of the submodules $m^k e_\lambda$ of E for all $k > 0$ (Algebra, Chapter II, § 3, no. 7, Remark); then $m^k E / m^{k+1} E$ is identified with the direct sum of the $m^k e_\lambda / m^{k+1} e_\lambda$ (Algebra, Chapter 11, § 1, no. 6, Proposition 7). まず ($k = 0$ について) 標準写像以降、(A/m) モジュール $E / mE$ の $E / mE = (A / m) \otimes_A E$ 形基底の $e_\lambda$ の類 $1 \otimes e_\lambda$ を推定します。

$$
(m^k / m^{k+1}) \otimes_A (E / mE) \to m^k E / m^{k+1} E
$$

すべての $k \geq 0$ に対して全単射です。したがって、$\gamma_E$ は全単射です。この証明の部分では、条件 (a) も条件 (b) も使用していないことに注意してください。

逆に、主張の条件が成立し、$(x_i)_{i \in I}$ を E の元の族とし、その類 mod を仮定します。 $(A/m)$ モジュール $E/mE$ の $mE$ 形基底。 L を自由A-加群 $A_s^{(I)}$、$(f_i)_{i \in I}$ を標準基底、$u : L \to E$ A-線型写像として、すべての $i \in I$ に対して $u(f_i) = x_i$ とします。仮説はすでに $u$ が全射であることを暗示しています (章 II, § 3, no. 2、系 1 から命題 4) が、$u$ が単射であることを証明することはまだ残っています。ここで、仮説 (a) と (b) はそれぞれ、A がハウスドルフであることを意味しており、したがって、$m^kL = (m^k)^{(I)}$ (代数, 章 II, § 3, no. 7, 注意) と $\operatorname{gr}(L)$ が次のように識別されるため、m 進フィルタリングでも L になります。 証明の最初の部分から $\operatorname{gr}(A) \otimes_{A/m} (L/mL)$。 準同型 $u$ はフィルタと互換性があり、$v$ が $\operatorname{gr}(L)$ の全単射である $\operatorname{gr}(u) = \gamma_E \circ v$ を書き込むことができます。
$$
\operatorname{gr}(A) \otimes_{A/m} (E/mE)
$$
写像類オフ、モード。 $1 \otimes \bar{x}_i$ に mM を加えます。ここで、$\bar{x}_i$ は $x_i$ mod の類です。 $mE$。次に、仮定は、$\operatorname{gr}(u)$ が単射であることを暗示し、系 1 から定理 1、no. 8 の助けを借りて結論が続きます。

### 10.  アプリケーション: ネーター 環の例

#### 補題 1 {#ac-iii-s2-lem-1 .statement tag=04EG}

A を、型 $\mathbf{Z}$ の等級付けされた環とし、その等級 $(A_n)$ が、すべての $n < 0$ について $A_n = 0$ またはすべての $n > 0$ について $A_n = 0$ となるようにします。 M を型 $\mathbf{Z}$ の A-加群と評価します。 M がネーター A-加群であるためには、M のすべての等級付けされた部分加群が有限に生成されることが必要かつ十分です。

$n \mapsto -n$ は群 $\mathbf{Z}$ の自己同型であるため、すべての $n > 0$ について $A_n = 0$ の場合に注意を限定することができます。 A' と M' は、それぞれの目盛り (no. 1、例 1) に関連付けられた濾過を備えた環 A と加群 M を示し、これらは網羅的で分離されています。 A の仮定は、A' が離散的であり、したがって完全であることを意味します。 E が M のサブ A モジュールである場合、E に誘導濾過を与えることによって得られる濾波された A' モジュール E' はハウスドルフであり、その濾過は網羅的です。さらに、$\operatorname{gr}(E')$ は $M = \operatorname{gr}(M')$ の段階的なサブ A モジュールで識別されるため、仮定によって有限に生成されます。結論は、no. 9 の系 1 から命題 12 に続きます。

#### 定理 2 {#ac-iii-s2-thm-2 .statement tag=04EH}

A を型 $\mathbf{N}$ の環に評価し、M を型 $\mathbf{N}$ の A-加群と、それぞれの卒業$(A_n)$ と $(M_n)$ に評価するとします。すべての $n > 0$ に対して $A_n = A_0 a^n$ と $M_n = a^n M_0$ が存在する元 $a \in A_0$ が存在するとします。次に、M がネーター $A_0$-モジュールである場合、M はネーター A-加群です。

補題 1 により、M のすべての段階的な部分加群 N が有限に生成されることを証明するのに十分です。すべての $r \geq 0$ について、$N_r = N \cap M_r$ とし、L_r を $a^r m \in N_r$ となるような $m \in M_0$ の集合とします。として
$$
a^r A_0 \subset A_r = A_0 a^r, \quad a^r A_0 L_r \subset A_0 a^r L_r \subset A_0 N_r \subset N_r
$$

したがって、L は M, のサブ A,-モジュールです。さらに、

$$
aN_r \subset N \cap aM_r = N \cap M_{r+1} = N_{r+1}
$$

したがって、数列 $(L_r)_{r \geq 0}$ は増加するです。 仮定は、$r \geq n$ に対して $L_r = L_n$ となるような整数 $n \geq 0$ が存在することを意味します。 それぞれの $r \leq n$ について、$(m_{r,s})_{1 \leq s \leq k_r}$ を A、モジュール $L_r$ の生成元の系とします。 $1 \leq s \leq k_r$, $0 \leq r \leq n$ 形系 of 生成元 of A-加群 N に対して元 $a^r m_{r,s}$ であることを示します。 $L_r$ の定義により、すべての $r$ に対して $M_r = a^r M_0$、すべての $r$ に対して $N_r = a^r L_r$ として。 次に、$r \leq n$ については、

$$
N_r = a^r L_r = \sum_{s=1}^{k_r} a^r A_0 m_{r,s} \subset \sum_{s=1}^{k_r} A_0 a^r m_{rs},
$$

そして、$r > n$については、

$$
N_r = a^r L_n = \sum_{s=1}^{k_n} a^r A_0 m_{n,s} \subset \sum_{s=1}^{k_n} A_0 a^r m_{n,s} \subset \sum_{s=1}^{k_n} A_0 a^{r-n} \cdot (a^n m_{n,s})
$$

これで証明 (cf. 練習問題 10) が完了します。

#### 系 1 (ヒルベルトの定理) {#ac-iii-s2-thm-2-cor-1 .statement tag=04EI}

*すべての可換ネーター 環 C、多項式環 C[X] はネーター* (cf. 練習問題 10) です。

#### 系 2 {#ac-iii-s2-thm-2-cor-2 .statement tag=04EJ}

*すべての可換ネーター 環 C およびすべての整数 $n > 0$ について、多項式環 C[X_1, ..., X_n] はネーター です。*

これは、系 1 から $n$ の帰納法に続きます。

#### 系 3 {#ac-iii-s2-thm-2-cor-3 .statement tag=04EK}

*C が可換ネーター 環である場合、有限生成された可換 C-代数はすべてネーター 環です。*

このような代数は、多項式代数 C[X_1, ..., X_n] (§ 1, no. 1) の商と同型です。

#### 系 4 {#ac-iii-s2-thm-2-cor-4 .statement tag=04EL}

*A を型 $\mathbf{N}$ の等級付けされた可換環とし、$(A_n)$ をその卒業とします。 A がネーター であるためには、$A_n$ がネーター であり、A が論理的に生成された A,-代数であることが必要かつ十分です。

条件は系 3 までに十分です。逆に、A がネーター であると仮定します。 A の理想である $m = \sum_{n \geq 1} A_n$ が有限に生成されます。この場合、A は有限生成された A,-代数 (§ 1, no. 2, 系から命題 1) です。一方、$A/m$と同型の$A_n$は、ネーター 環です。

#### 系 5 {#ac-iii-s2-thm-2-cor-5 .statement tag=04EM}

*A を可換環とし、$A/m$ がネーター、$m/m^2$ が論理的に生成された $(A/m)$ モジュール、A がハウスドルフであり、m 進数位相で完了するような A のイデアルとする。すると、gr(A) と A はネーター となります。*

gr(A) は $m/m^2$ (no. 3, 例 3) によって生成された $(A/m)$ モジュールであるため、環 gr(A) は系 3 によるネーター です。これから、A 自体はネーター (no. 9, 系 2 ～ 命題 12)。

#### 系 6 {#ac-iii-s2-thm-2-cor-6 .statement tag=04EN}

すべての可換ネーター 環 C およびすべての整数 n > 0 について、形式冪系列 $\mathbf{C}[[X_1, \ldots, X_n]]$ の環はネーター です。

これは、系 5 と no. 6、系から命題 6 に続きます。m が、定数項を持たない形式冪系列の $A = \mathbf{C}[[X_1, \ldots, X_n]]$ からなるのイデアルである場合、$A/m$ は以下と同型です。 C と $m/m^2$ を C モジュール $\mathbf{C}"$ に接続します。

注意

(1) 系 2、3、6 は、C が可換体の場合に特に当てはまります。

\* (2) g を可換ネーター 環 C 上のリー代数とし、g が有限生成された C 加群であると仮定します。 g を包囲する代数 U に、no. 3、例 4 で定義される増加するろ過 $(U_n)$ を与えます。対応する位相では、U は離散的であり、したがってハウスドルフ完全です。関連する段階的環 gr(U) は有限生成された C-代数であり、対称代数 $\mathscr{S}(g)$ の商であるため、 gr(U) はネーター 環 (系 3) であり、U は左であり、 右ネーター 環 (no. 9、系 2 ～ 命題 12)。 \*

### 11. 完全な m-ADIC 環および逆数極限

no. 6 で、A が可換環で、A がハウスドルフで m 進数位相で完成するような A のイデアルである場合、トポロジカル環 $A$ は、離散環 $A_i = A/m^{i+1} \ (i \in \mathbf{N})$ の逆行列極限と正準的に同一視されることがわかりました。 標準写像へ

$$
h_{ij}: A/m^{j+1} \to A/m^{i+1} \quad (i \leq j);
$$

$h_{ij}$ は全射法であり、$n_{ij}$ がその核である場合、

$$
n_{ij} = m^{i+1}/m^{j+1} = (m/m^{j+1})^{i+1} =
$$

特に$(n_{0j})^{j+1} = 0$。逆に:

#### 命題 14 {#ac-iii-s2-prop-14 .statement tag=04EO}

$(A_i, h_{ij})$ を離散可換環の逆数系とし、インデックス付け集合を $\mathbf{N}$ とし、$(M_i, u_{ij})$ を環の逆数系に対する加群の逆数系とします。 $(A_i, h_{ij})$。 $n_j$ は $h_{0j}: A \to A$ の核と、集合 $A = \lim A_i$、$M = \lim M_i$ を表すものとします。次のように仮定します。

(a) すべての $i \in \mathbf{N}$ について、$h_{ii}$ は A 上の恒等写像であり、$i \leq j$ については、$h_{ij}$ と $u_{ij}$ は全射です。
(b) $i \leq j$、$h_{ij}$、$u_{ij}$ の核は、それぞれ$n_j^{i+1}$、$n_j^{i+1} M_j$ です。

次に:
(i) $A$ は完全なハウスドルフ位相環、$M$ は完全なハウスドルフ位相 A-加群、標準写像 $h_i : A \to A_i$、$u_i : M \to M_i$ は全射です。
(ii) $M_0$ が有限生成された A,-加群である場合、$M$ は有限生成A-加群です。

正確に言うと、$u_0(S)$ 生成する M となるような M のすべての有限部分集合 S は、M の生成元の系になります。

(i) の主張は、一般位相、章 II, § 3, no. 5、系から命題 10 および系 1 から定理 1 に続きます。

すべての $i \in \mathbf{N}$ について、$m_{i+1} = \mathrm{Ker}(h_i), N_{i+1} = \mathrm{Ker}(u_i)$ と書きましょう。それから

$$
m_{i+1} = \lim_{k \geq 0} h_{i,t+k}^{-1}(0) = \lim_{\leftarrow} n_{i+1}^{t+k}
$$

そして$N_{i+1} = \lim_{\leftarrow} n_{i+k}^{t+1} M_{i+k}$; $h_{i+k}$ と $u_{i+k}$ は全射なので、

$$
h_{i+k}(m_{i+1}) = n_{i+k}^{t+1}, \quad u_{i+k}(N_{i+1}) = n_{i+k}^{t+1} M_{i+k}.
$$

$i \geq 1$ と $j \geq 1$ に対して $m_i N_j \subset N_{i+j}$、つまり証明と $u_{i+j-1}(m_i N_j) = 0$ が一致することを示しましょう。今

$$
u_{i+j-1}(m_i N_j) = h_{i+j-1}(m_i) u_{i+j-1}(N_j)
$$

すべての $k \geq 0$、$n_k^{k+1}$ ($h_{kk}$ の核) は 0 に等しいため、$n_{i+j-1}^{t'}(n_{i+j-1}^{t'} M_{i+j-1}) = 0$ に等しい。同様に、$m_i m_j \subset m_{i+j}$ もわかります。 $i \leq 0$ について、集合 $m_i = A$ と $N_i = M$ の場合、$(m_i)_{i \in \mathbf{Z}}$ は A の濾過であり、$(N_i)_{i \in \mathbf{Z}}$ は A の濾過と互換性のある M の濾過です。 A と M のトポロジは明らかに、これらのフィルタリングによって定義されたものです。そうであれば、S によって生成される M の $h_1(a) = n_1$ と $M'$ 部分加群が成り立つような A のイデアルを $a$ とします。私たちはそれを証明するつもりです

$$
N_i = a^i M' + N_{i+1} \quad \text{for } i \geq 0.
$$

$a_i = h_i(a), M'_i = u_i(M')$ と書きましょう。それを示せば十分です

$$
u_i(N_i) = a_i^i M'_i.
$$

これは、$N_0 = M$ と $M'_0 = M$ が仮定までに $i = 0$ の場合に当てはまります。 $i \geq 1$の場合、(16)により$u_i(N_i) = n_i^i M_i$になります。 $h_{1i}$ は全射法で、$h_{0i} = h_{01} \circ h_{1i}$、$h_{1i}$ 写像核 $n_i$ の $h_i$、核 $n_1$ の $h_1$、および $n_i = h_{1i}(n_1)$ です。それから

$$
h_{1i}(a_i) = h_1(a) = n_1 = h_{1i}(n_i)
$$

そして、$h_{1i}$ の核は $n_i^2$、$n_i \subset a_i + n_i^2$、$a_i \subset n_i$ であるため、よって $n_i = a_i + n_i^2$ となります。さらに$u_{0i}(M'_i) = u_0(M') = M, = u_{0i}(M_i)$、そして$\mathrm{Ker}(u_{0i}) = n_i M_i$、$M_i = M'_i + n_i M_i$。 よって

$$
n_i^i M_i = (a_i + n_i^2)^i (M'_i + n_i M_i).
$$

さて、$a_i^k n_i^{i+1-k} \subset n_i^{i+1} = 0$ は $0 \leq k \leq i$ になります。その場合、確実に $u_i(N_i) = n_i M_i = a_i^i M'_i$ となり、(17) が証明されます。

さらに、$m_1 = h_1(n_1)$、よって、$a \subset m_1$、したがって $a^i \subset m_1^i \subset m_i$、よって

$N_i \subset m_i M' + N_{i+1}$;一方、明らかに $m_i M \subset N_i$ なので、すべての $i \geq 0$ に対して $N_i = m_i M' + N_{i+1}$ です。次に、no. 9 の系 3 から命題 12 に$M' = M$ が続き、証明が完成します。

#### 系 1 {#ac-iii-s2-prop-14-cor-1 .statement tag=04EP}

*記法と命題 14 の仮説では、$M_0$ が有限生成された $A$ 加群であり、$A$ の理想的な $n_1$ が有限生成されると仮定します。 $m_1$ を $h_1$ の核とします。 $A$ と $M$ のトポロジは、それぞれこの環とこの加群の $m_1$ 進トポロジになります。正確に言うと、$h_i$ と $u_i$ のすべての $i \geq 0$、核は、それぞれ $m_1^{i+1}$ と $m_1^{i+1} M$ です。さらに、$m_1 / m_1^2$ は有限生成された $A$ モジュールです。*

命題 14 の証明のうち記法を保存します。ここでの仮説により、イデアル $a$ が有限に生成されると仮定できます。 $i \geq 0$ を任意の整数とします。すべての$j \geq 0$、by (17)、$N_{i+j} = a^j(a^i M) + N_{i+j+1} \subset m_j(a^i M) + N_{i+j+1}$;逆に、$m_j(a^i M) \subset m_j m_i M \subset m_{i+j} M \subset N_{i+j}$、よって

$$
N_{i+j} = m_j(a^i M) + N_{i+j+1}.
$$

$a$ と $M$ は有限生成される $A$ モジュールであるため、$a^i M$ も同様です。 適用系 3 ～ 命題 no. 9 ～ 加群の 12 $N_i$ $N_{ij} = N_i$ で定義された濾過$(N_{ij})_{j \in \mathbf{Z}}$、$j < 0$ の場合、$N_{ij} = N_{i+j}$ の場合$j \geq 0$、$N_i = a^i M$、よって $N_i \subset m_1^i M$ が得られます。でも、$m_1^i M \subset m_i M \subset N_i$、よって $N_i = m_1^i M$も。 適用これを、$M = A$、$u_{ij} = h_{ij}$の場合に、$m_i = m_1^i$を求めます。さらに、(17)より$m_1 = a + m_1^2$となり、系の最後の主張が証明されます。

#### 系 2 {#ac-iii-s2-prop-14-cor-2 .statement tag=04EQ}

*系 1 の仮説の下では、$A$ がネーター であるためには、$A$ がそうであることが必要かつ十分です。*

条件は、$A$ が $A$ の商と同型であるため必要です。 no. 10、系 5 ～ 定理 2 のおかげで十分です。

### 12. フィルタリングされた加群のハウスドルフ完成

$G$ をフィルター処理された群とし、そのフィルター $(G_n)$ は $G$ の通常の部分群で構成されます。トポロジカル群 $G$ の *ハウスドルフ完全* $\hat{G}$ は、*離散* 群 $G/G_n$, 標準準同型の逆関数極限 $\lim \leftarrow G/G_n$ と正準的に同一視されることをすでに思い出しました (no. 6)。 $i : G \to \hat{G}$ には、$G$ ($\hat{G}$ のどこでも密集している) と関連付けられたハウスドルフ像群と、$G$ の$\{0\}$ の閉鎖$\bigcap G_n$ を持つ核があります。 $G$の部分群$G_n$のハウスドルフ完了$\hat{G}_n$は、$\hat{G}$の$i(G_n)$の終結と識別されます（*一般位相*、章II, § 3, no. 9、系1から命題 18)、$G$ 以降、$\hat{G}$ は休業となります。

$$
G, = i^{-1}(\hat{G}_n) = i^{-1}(\hat{G}_n \cap i(G)).
$$

さらに、$\hat{G}_n$ 形は、$\hat{G}$ の 0 の近傍の基本的な系 (*一般位相*、章 111、§ 3, no. 4、命題 7) であるため、ノーマルオープン部分群です。 $\hat{G}$ (一般位相、章 111、§ 2, no. 3、命題 8); $\hat{G}$ の位相は濾過 $(\hat{G}_n)$ によって定義され、常に定義によって分離されます。 $\hat{G}$は$i(G)$が密で$\hat{G}_n$は空いているので、

$$
\hat{G} = i(G) \cdot \hat{G}_n
$$

そして同様に

$$
= i(G_{n-1}) \cdot \hat{G}_n.
$$

(18) と (19) から、$(G_n)$ が存在する場合にのみ、濾過 $(\hat{G}_n)$ が網羅的であると推測します。

2 番目の同型定理 (代数、章 I, § 6, no. 13、定理 6 (d)) と式 (18)、(19)、(20) は、標準準同型を示します。

$$
G_{n-1}/G_n \to \hat{G}_{n-1}/\hat{G}_n, \quad G/G_n \to \hat{G}/\hat{G}_n,
$$

は全単射なので標準準同型も同様です

$$
\operatorname{gr}(G) \to \operatorname{gr}(\hat{G}).
$$

ここで、$A$ をフィルタリングされた環、$E$ をフィルタリングされた $A$ モジュール、$(A_n)$ と $(E_n)$ をそれぞれ $A$ と $E$ のフィルタリングとします。これらのフィルタリングは網羅的であるため、対応するトポロジでは、$A$ はトポロジカル環であり、$E$ はトポロジカル $A$ モジュール (no. 5、命題 3) であると仮定します。次に、(一般位相、章 111、§6、番号 5 および 6) $\hat{A}$ をトポロジカル環として、$\hat{E}$ をトポロジカル $\hat{A}$ モジュールとして定義しました。 $i : A \to \hat{A}$が標準準同型なら、$A$の乗法の連続性により、$i(A_m)i(A_n) \subset i(A_{m+n})$、よって、

$$
\hat{A}_m \hat{A}_n \subset \hat{A}_{m+n}
$$

$A_n$ は $\hat{A}$ の $i(A_n)$ の終結であるため。同様に次のように示すことができます

$$
\hat{A}_m \hat{E}_n \subset \hat{E}_{m+n};
$$

その他語:

#### 命題 15 {#ac-iii-s2-prop-15 .statement tag=04ER}

$A$ をフィルタリングされた環および $E$ をフィルタリングされた $A$ モジュールとし、$A$ および $E$ のそれぞれのフィルタリング $(A_n), (E_n)$ が網羅的であるとします。次に、$(\hat{A}_n)$ は、$\hat{A}$ の環構造と互換性のある濾過であり、$(\hat{E}_n)$ は、濾過された環 $\hat{A}$ を超えて、$\hat{E}$ の加群構造と互換性のある濾過です。さらに、これらのフィルタリングは網羅的であり、それぞれ $\hat{A}$ と $\hat{E}$ のトポロジーが定義するです。最後に、グレード付き $\mathbf{Z}$ モジュールの標準写像 $\operatorname{gr}(A) \to \operatorname{gr}(\hat{A})$ と $\operatorname{gr}(E) \to \operatorname{gr}(\hat{E})$ は、それぞれグレード付き環同型とグレード付き $\operatorname{gr}(A)$ モジュール同型です。

以下では、各ユニフォーム空間 $X$ について、$j_X$ は、$X$ からそのハウスドルフ完成 $\hat{X}$ および $X_0 = j_X(X)$ までの標準写像を表し、ハウスドルフである $\hat{X}$ のユニフォーム部分空間を示します。 空間は $X$ に関連付けられています。 $X$ の位相は、$X_0$ の$j_X$ の下の逆像であることを思い出してください (一般位相、

章 II, § 3, no. 7、命題 12）。また、すべての一様連続写像 $f : X \to Y$ に対して、$\hat{f}$ は $\hat{X}$ から $\hat{Y}$ までの一様連続写像を表し、$\hat{f} \circ j_X = j_Y \circ f$ (上記参照、命題 15) であることも思い出してください。 $X$ が $Y$ および $\mathscr{E}$ 標準単射のユニフォーム部分空間である場合、$\hat{X}$ は $\hat{Y}$ のユニフォーム部分空間と識別され、$\hat{f}$ は $X$ の標準単射となります。 $\hat{Y}$ (同上、no. 9. 系 1 ～ 命題 18)。

#### 補題 2 {#ac-iii-s2-lem-2 .statement tag=04ES}

*$X \xrightarrow{f} Y \xrightarrow{g} Z$ をトポロジカル群 (代数, 章 II, § 1, no. 4, 注意) の厳密な射の完全系列とします。 $X, Y, Z$ がハウスドルフ完成群を認め、単位元 $\mathscr{E} X, Y, Z$ が近傍の可算基底系を認めるとします。したがって、$\hat{X} \xrightarrow{\hat{f}} \hat{Y} \xrightarrow{\hat{g}} \hat{Z}$ は厳密な射の完全系列です。*

$N_1, N_g$ をそれぞれの核オフと $g$ とします。書きましょう

$$
f = f_3 \circ f_2 \circ f_1
$$

ここで、$f_1$ は標準写像 $X \to X/N_f$、$f_2$ は $X/N_f$ の $N$ 上の同型、$f_3$ は標準単射 $N \to Y$ です。 $f_2$ は $(X/N_f)^*$ の $\hat{N}_g$ への同型であることはすでに知っていますし、$f_1$ は $N$ から $\hat{Y}$ への単射厳密な射であることを思い出しました。 $\hat{f}_1$ が全射厳密射であることを示せば、$\hat{f}$ は厳密射 (一般位相, 章 III, § 2, no. 8, 注意 2) であることがわかります。 $g_1$ を標準写像 $Y \to Y/N_g$ とします。 $\hat{g}_1$ が核 $\hat{N}_g$ の全射厳密射であることを示すと、上記のように $\hat{g}$ が厳密射であり、数列 $\hat{X} \xrightarrow{\hat{f}} \hat{Y} \xrightarrow{\hat{g}} \hat{Z}$ が正確であることがわかります。したがって、問題を証明に縮約しました。つまり、$Y = X/N$ ($N$ は $X$ の正規の部分群) で、$f : X \to Y$ が標準写像である場合、$\hat{f}$ は *全射厳密な射です。 核* $\hat{N}$。

$f_0 : X_0 \to Y_0$ を $X_0$ に $f$ を加えた一致するを写像とします。 $j_X$ (それぞれ $j_Y$) は $X$ から $X$ への全射厳密射 (それぞれ $Y$ から $Y_0$) であるため、 $f_0$ は全射厳密射 (一般位相、 章 III, § 2, no. 8、注意 3）。 $X_0$ と $Y_0$ が計量可能になりました (一般位相、章 IX, § 3, no. 1、命題 1)。次に、一般位相、章 IX, § 3, no. 1、系 1 から命題 4 および補題 1 から、$\hat{f}_0 = \hat{f}$ は全射厳密射であり、閉包核 $\hat{N}_0'$ を持つことがわかります。 *in* 核 $N_0'$ $f_0$ の $X$。 そうすれば、$\hat{N}_0' = \hat{N}$ を証明できれば十分です。 今は $N_0'$ 明らかに含む $N_0 = j_X(N)$; $N_0'$ が $N_0$ *in* $X$ の閉包 $\overline{N}_0$ に含まれていることを示すだけで十分です。 今、

$$
u = j_X^{-1}(X_0 - \overline{N}_0) = X - j_X^{-1}(\overline{N}_0)
$$

$X$ でオープンの集合ですが、$N$ と一致しません。 $f$ は全射厳密射であるため、$V = f(U)$ は $Y$ の含む単位元 $e'$ ではなく、$Y$ のオープン集合であるため、$e'$ の閉包を満たしていません。その場合、$j_Y(V)$ は $Y_0$ の含む単位元になりません。しかし、$j_Y(V) = f_0(X_0 - \overline{N}_0)$ なので $N'_0 \subset \overline{N}_0$ となり、補題 2 の証明が完成します。

#### 命題 16 {#ac-iii-s2-prop-16 .statement tag=04ET}

*$A$をフィルタリングされた環、($A,$)そのフィルタリング、$E$を$A$モジュール、($E_n$)$A$からなるのフィルタリングから派生した$E$のフィルタリングとします。 $E_n = A_n E$。濾過 ($A,$) が徹底的で、加群 $E$ が有限に生成されるとします。 $i : E \to \hat{E}$ が標準写像の場合、すべての $n \in \mathbf{Z}$ について、*
$$
8_n = \hat{A}_n \hat{E} = \hat{A}_n i(E) \quad \text{and} \quad \hat{E} = \hat{A}.i(E).
$$
*特に $\hat{E}$ は有限生成された $\hat{A}$ モジュールです。*

方程式 $A_n E = E_n$ は、$A$ モジュール $8, \hat{A}_n \hat{E} \subset 8$ 上の外部法則の連続性により、明らかに $\hat{A}_n \hat{E} \supset \hat{A}_n i(E)$ を意味します。 仮定までに全射準同型 $u : L \to E$ が存在します。ここで、$L = A_s^I$、$I$ は有限の集合です。 $L$ に積の濾過を与え、$L_n = A_n^I$ のからなるを$L$ 積位相で定義するにします。次に、$\hat{L} = \hat{A}_s^I$ と $\hat{L}_n = \hat{A}_n^I$ (*一般位相*、章 II, § 3, no. 9、系 2 ～ 命題 18)。 $j : L \to \hat{L}$ を $L$ の標準写像と $(e_i)_{i \in I}$ 標準基底とします。 元 $\sum_{i \in I} a_{ij}(e_i)$ (すべての $i \in I$ に対して $a_i \in \hat{A}$) から属するから $\hat{L}_n$ まで、すべての $i$ に対して $a_i \in \hat{A}_n$ であることが必要かつ十分です。それから$\hat{L}_n = \hat{A}_n . j(L)$。そうなると、定義 $u(\hat{L}_n) = A_n E = E_n$ により、$u$ は $L$ から $E$ への *厳密な射* になります (*一般位相*、章 III, § 2, no. 8、命題 24)。 補題 2 は、$\hat{u} : \hat{L} \to \hat{E}$ が *全射厳密射* であることを示します。 $\hat{L}_n$ はオープン部分群オフであるため、$\hat{u}(\hat{L}_n)$ は $\hat{E}$ のオープン (したがってクローズ) 部分群です。しかし、$\hat{u}(\hat{L}_n) = \hat{A}_n \hat{u}(j(L)) = \hat{A}_n i(E)$、そして$i(E_n) \subset A_n i(E) \subset \hat{A}_n i(E)$、最後に$\hat{E}_n \subset \hat{A}_n i(E) \subset \hat{A}_n \hat{E} \subset \hat{E}_n$、したがって$\hat{E}_n = \hat{A}_n \hat{E} = \hat{A}_n i(E)$になります。 設定 $n = 0$ により、(25) の 2 番目の公式が得られます。

#### 系 1 {#ac-iii-s2-prop-16-cor-1 .statement tag=04EU}

*命題 16 の条件では、$A$ が完了すると、$E$ も完了します。*

標準写像 $A \to \hat{A}$ は全射法 (no. 6, 命題 5) なので、(25) によって $\hat{E} = i(E)$ となり、結論は no. 6 の命題 5 になります。

#### 系 2 {#ac-iii-s2-prop-16-cor-2 .statement tag=04EV}

*$A$を可換環、$m$を$A$の有限生成イデアル、$\hat{A}$を$m$進数位相に関する$A$のハウスドルフ完成とします。次に、$\hat{A}$ 上のすべての整数 $n > 0$ と位相の $\hat{m}^n = (\hat{m})^n = m^n . \hat{A}$ は、$\hat{m}$ 進数の位相です。*

$A$ の有限生成された理想である $A_n = m^n$ を書いてみましょう。 公式 $m^p A_n = m^{n+p}$ は、$A$ モジュールの $m$ 進数位相を使用した $m$ 進数位相一致するによって、 $A$ で位相が誘導されたことを示しています。 $A_n$ (no. 1、*例 3*)。

命題により 16 が $E = A_n$、$\hat{A}_n = \hat{A}.A_n$ に他の語 $\hat{m}^n = m^n . \hat{A}$ に適用されます。特に$m = m . \hat{A}$、よって
$$
(\hat{m})^n = m^n . \hat{A} = \hat{A}.A_n
$$
(cf. 練習問題 12)。

濾過済みのハウスドルフ完成品の例環

(1) $A$ を型 $\mathbf{N}$ の等級付けされた環とし、$(A_n)_{n \geq 0}$ をその卒業とします。分離され徹底的な関連ろ過を与えてください (no. 1, 例 1)。 加法群 $A$ は正規的に $B = \prod_{n \in \mathbf{N}} A_n$ の部分群と同一視されます。 $B$ に離散トポロジーの位相積が与えられた場合、$A$ で誘導された位相は、$A$ でのフィルタリングによって定義される位相になります。また、$B$ は完全なトポロジー 群であり、$A$ は $B$ に密集しています (一般位相、章 III, §2, no. 9、命題 25)。次に、加法的なトポロジカル群 $B$ は、ハウスドルフ加法群 $A$ の完成 $\hat{A}$ と識別され、命題 15 から、それが一意の環構造を持ち、トポロジカル環の完成となることがわかります。 $A$。この環の定義する乗法に対して、$A'_n = \sum_{i > n} A_i$ と書くと、両面イデアル $A'_n$ の $B$ の閉包は $x = (x_i) \in B$ の集合 $B$ となり、$x_i = 0$ が成り立つことに注意してください。 $i \leq n$。次に、$x = (x_i), y = (y_i)$を$B$の2つの元と$z = (z_i)$の積とします。次に、すべての $n > 0$、$x \equiv x'_n$ (mod. $B_n$)、$y \equiv y'_n$ (mod. $B_n$) について、$x'_n = (x_i)_{0 \leq i \leq n}$、$y'_n = (y_i)_{0 \leq i \leq n}$、よって $z \equiv x'_n y'_n$ (mod. $B_n$) となります。しかし、$x'_n$ と $y'_n$ 属するから $A$ なので、すべての $n \in \mathbf{N}$ について、

$$
z_n = \sum_{j=0}^n x_j y_{n-j}.
$$

特に、no. 6 の系から命題 6 を再度取得します。 $C$ が可換環の場合、多項式環 $C[X_1, \ldots, X_r]$ の完了は、通常の目盛り (合計次数による) に関連付けられた濾過を伴って正規に識別されます。正式な冪系列 $C[[X_1, \ldots, X_r]]$ (cf. 代数、章 IV, §5, no. 10) の環。

*(2) $K$ を評価済みの完全な可換体とします。 $K$ にわたる $r$ 変数における収束系列の環の完了は、形式的冪系列 $K[[X_1, \ldots, X_r]]$ の環と標準的に識別されます。 \*

(3) $a$ を主イデアル整域の非ゼロの非反転要素とする。 $A$ の (a) 進数位相は、$a$ 進数位相とも呼ばれます。それは、ハウスドルフです。理想 $(a^n)$ 簡約するの共通部分を 0 (代数、章 VII, §1, no. 3) にします。この位相に対する$A$の完成は必ずしも整域（cf.no. 13、注意3）ではないことに注意してください。関連する等級付けされた環 $\mathrm{gr}(A) = \mathrm{gr}(\hat{A})$ は、正準的に $(A/a)[X]$ (no. 3, 例 1) と同型です。 $A = \mathbf{Z}$ の場合、n 進数位相 ($n > 1$) に関する $\mathbf{Z}$ の完成は $\mathbf{Z}_n$ で示され、その元は $n$ 進数整数と呼ばれます。

$\mathbf{Z}/n^k \mathbf{Z}$ のすべての元は、形 $\sum_{i=0}^{k-1} a_i n^i$ の一意の代表を認めます。ここで、すべての $i$ に対して $0 \leq a_i \leq n - 1$ です。さらに、$\mathbf{Z}/n^{k-1} \mathbf{Z}$の標準像は$\sum_{i=0}^{k-2} a_i n^i$の類です。 These remarks and the fact that $Z$, is canonically identified with the inverse limit $\lim_{\leftarrow} \mathbf{Z}/n^k \mathbf{Z}$ show immediately that every element of $Z$, can be written uniquely in the form $\sum_{i=0}^{\infty} a_i n^i$ where $0 \leq a_i < n$ and conversely that such a series is convergent in $\mathbf{Z}$.

### 13. ハウスドルフによるセミローカルリングの完成

#### 命題 17 {#ac-iii-s2-prop-17 .statement tag=04EW}

$A$ を可換環とし、$(m_{\lambda})_{\lambda \in L}$ を $A$ とは異なる $A$ の理想群とし、$m_{\lambda}$ と $m_{\mu}$ が $\lambda \neq \mu$ に対して相対的に素であるとします。 すべての家族について、整数 $\geq 0$、有限台、集合 $a_s = \bigcap_{\lambda \in L} m_{\lambda}^{s(\lambda)}$ の $s = (s(\lambda))_{\lambda \in L}$ ($s(\lambda) \neq 0$、cf. などの $\lambda$ の $m_{\lambda}^{s(\lambda)}$ の積に等しい) 章 11、§ 1, no. 2、命題 3 および 5)。 $a_s$ 形位相 $\mathscr{T}$ に対する 0 の近傍の基本系は、$A$ の環構造と互換性があります。この位相に関する$A$のハウスドルフ完成を$\hat{A}$とします。 一方、すべての $\lambda \in L$ について、$A_{\lambda}$ を $m_{\lambda}$ 進数位相を持つ環 $A$ とし、$\hat{A}_{\lambda}$ をそのハウスドルフ完成とします。 $u : A \to \prod_{\lambda \in L} A_{\lambda}$ が対角線準同型を表す場合、$u$ は連続で、対応する準同型 $\hat{u} :$

$$
\hat{A} \to \left( \prod_{\lambda \in L} A_{\lambda} \right)^{\hat{}} = \prod_{\lambda \in L} \hat{A}_{\lambda}
$$

(一般的な位相、章 III, § 6, no. 5 および章 II, § 3, no. 9、系 2 ～ 命題 18) はトポロジカル環同型です。

最初の主張は、一般位相、章 III, § 6, no. 3、例 3 から続きます。 集合 $B = \prod_{\lambda \in L} A_{\lambda}$ にしましょう。 $A$ の位相は、各 $m_{\lambda}$ 進トポロジよりもより細かいであるため、写像 $\mathrm{pr}_{\lambda} \circ u$ は連続であり、したがって $u$ も連続です。 また、$u(a_s)$ は、$B$ の対角$A$ の共通部分と、$B$ の開いた集合 $\bigcap_{\lambda \in L} \mathrm{pr}_{\lambda}^{-1}(m_{\lambda}^{s(\lambda)})$ です。したがって、$u$ は、加法群 $A$ から $B$ と像 $A$ の厳密な射であることがわかります。 現在、$\Delta$ は $B$ に密集しています。 For let $b = (a_{\lambda})_{\lambda \in L}$ be an element of $B$; every neighbourhood of $b$ in $B$ contains a set of the form $b + V$, where $V = \bigcap_{\lambda \in L} \mathrm{pr}_{\lambda}^{-1}(m_{\lambda}^{s(\lambda)})$ for a family $s = (s(\lambda))_{\lambda \in L}$ with finite support of integers $\geq 0$. $m_{\lambda}^{s(\lambda)}$ は対 (章 II, § 1, no. 2, 命題 3) で相対的に素であるため、すべての $\lambda$ (前述、命題 5) に対して $x \equiv a_{\lambda} \pmod{m_{\lambda}^{s(\lambda)}}$ となるような $x \in A$ が存在し、したがって $(b + V) \cap A \neq \varnothing$ が存在します。 群 $B/\Delta$ のハウスドルフ完成は $\{0\}$ になります。 適用補題 2 no. 12 から完全系列 $0 \to A \xrightarrow{u} B, A \xrightarrow{u} B \to B/\Delta$ まで、$\hat{u}$ は $\hat{B}$ 上の $\hat{A}$ の同型であることがわかります。

#### 系 {#ac-iii-s2-n13-cor-1 .statement tag=04EX}

$A$ を主イデアル整域とし、$P$ を $A$ の極値元 (代数、章 VII, § 1, no. 3) の代表系とします。 $A$の位相は、$\mathbf{A}$の$\neq 0$形の基本的な系の$\mathbf{A}$の環構造と互換性のある0の近傍がハウスドルフであり、$\mathbf{A}$の完成であるこの位相は、$x$ から $P$ まで実行される $x$ 進トポロジーに関して、$\mathbf{A}$ の完成形の積と正規同型です。

$\pi \in P$ が最大かつ個別であり、したがって比較的素である主イデア $(x)$ は、$x$ 進トポロジーがハウスドルフであることをすでに見ました (no. 12, 例 3)。したがって、位相も命題 17 の主張で定義されます。 より細かいは、それぞれの $x$ 進トポロジよりも優れています。

If the Corollary to Proposition 17 is applied when $\mathbf{A} = \mathbf{Z}$, we denote by $\hat{\mathbf{Z}}$ the completion of $\mathbf{Z}$ with respect to the topology for which all the ideals $\neq 0$ of $\mathbf{Z}$ form a fundamental system of neighbourhoods of 0, the ring isomorphic to the product $\prod_{p \in P} \mathbf{Z}_p$ of the rings of $p$-adic integers (P being the set of prime numbers).

注意

(1) 明らかに、命題 17 の条件では、位相 $\mathscr{T}$ が、$\mathbf{A}$ の $m_\lambda$ 進トポロジーの最小の上界です。

(2) $\prod_{\lambda \in L} \hat{A}_\lambda$ のすべての閉理想 $a$ は、その射影 $a_\lambda = \mathrm{pr}_\lambda(a)$ の積と同一であり、これらは $A_\lambda$ の閉理想です。 $\hat{A}_\lambda$ は、$\prod_{\lambda} \hat{A}_\lambda$ の閉じた理想 $A'_\lambda$ と $a \cap A'_\lambda$ の$a_\lambda$ (代数、章 I, §8, no. 10、命題 6) と標準的に同一視され、$a_\lambda$ の和は密集しています。 積 $\prod_\lambda a_\lambda$ (一般位相、章 III, §2, no. 9、命題 25) 後者は$\prod_\lambda \hat{A}_\lambda$、よって主張は休業となります。

#### 命題 18 {#ac-iii-s2-prop-18 .statement tag=04EY}

Let $\mathbf{A}$ be a commutative ring, $(m_i)_{1 \leq i \leq q}$ a finite family of distinct maximal ideals of $\mathbf{A}$, t the product ideal $m_1 m_2 \ldots m_q = m_1 \cap m_2 \cap \ldots \cap m_q$ and $S$ the multiplicative subset $\bigcap_{i=1}^q (\mathbf{A} - m_i)$. $\mathbf{A}$ に $r$ 進数位相、環 $B = S^{-1} \mathbf{A}$ $rB$ 進数位相、および局所環 $A_n$ のそれぞれ $(m_i A_{m_i})$ 進数位相を与えます。 $u : \mathbf{A} \to B$、$v_i : B \to A_{m_i}$ を標準準同型 (章 II, §2, no.1、系 2 ～ 命題 2) および $v$ 準同型 $(v_i) : B \to \prod_{i=1}^q A_n$ とします。 準同型 $u$ と $v$ は連続であり、対応する準同型 $\hat{u} : \hat{\mathbf{A}} \to$ と $\hat{v} : \hat{B} \to \prod_{n} (A_n)^*$ は位相的環同型です。

$1 \leq i \leq q$ の$m_i \cap S = \varnothing$、したがって、$B$ の理想的な $m'_i = m_i B$ は最大 (章 II, §2, no. 5、命題 11) であり、
$$
rB = m'_1 \cap m'_2 \cap \cdots \cap m'_q
$$

(章 II, § 2, no. 4);最後に、$B_{m'_i} = A_i$、標準同型 (章 11、§ 2, no. 5、命題 11) までです。 $\bar{u}^1(rB) = r$と$\bar{v}_i^1(m_iA_{m_i}) \supset rB$のように、$u$と$v$は連続です。それなら、次のことを証明すれば十分です。

$$
w = v \circ u : A \to \prod_{i=1}^4 A_{m_i},
$$

$\hat{w}$ は $\prod_{i=1}^q \hat{A}_{m_i}$ 上の $\hat{A}$ の同型であり、この結果を $B$ に適用すると、$m'_i$ は $\hat{v}$ が同型であるため、$\hat{u}$ であることがわかります。 $c$ の $m_i$ 含む冪の冪のすべての積、したがって $r$ 進の位相は、$m_i$ 進のトポロジの最小の上界であることに注意してください。さらに、$A_i$ が $m_i$ 進数の位相と $\phi : A \to \prod_{i=1}^q A$ で環 $A$ を表す場合、対角写像、$\hat{\phi} : \hat{A} \to \prod_{i=1}^4 \hat{A}_i$ は同型 (命題 17) です。 すると、すべては証明となり、$u_i : A_i \to A_{m_i}$ が標準写像であれば、$\hat{u}_i : \hat{A}_i \to \hat{A}_{m_i}$ は同型になります。 さて、すべての$n$、写像

$$
u_{i,n} : A/m_i^n \to A_{m_i}/m_i^n A_{m_i}
$$

$u_i$ から商を取り出すと、同型 (章 II, §3, no. 3, 命題 9) になります。私たちの主張は、$\hat{A}_i$ (それぞれ $\hat{A}_{m_i}$) が離散環 $A/m_i^n$ (それぞれ $A_{m_i}/m_i^n A_{m_i}$) (cf. no. 6) の逆数極限であるという事実から導き出されます。

注意 (3)。 整域 $A$ は、そのハウスドルフ補完 $\hat{A}$ が零の非ゼロの約数を許容するようなものになり得ることがわかります。

#### 命題 19 {#ac-iii-s2-prop-19 .statement tag=04EZ}

$A$を可換環、$m$を$A$の最大理想とします。 $m$進数位相に関する$A$のハウスドルフ完成$\hat{A}$は局所環で、その最大理想値は$m$です。

$a = \bigcap_{k \geq 1} m^k$、$\hat{A}$ が $A$ に関連付けられたハウスドルフ環 $A/a$ の完成であり、$m/a$ が $A/a$ で最大であるため、$A$ が $m$ 進数に関してハウスドルフであると仮定できます。 位相。 $A/m$ と $\hat{A}/\hat{m}$ は同型環 (no. 12, 公式 (21)) であるため、$m$ は $\hat{A}$ で最大になります。 $\hat{A}$ の位相は濾過 $(m^n)^*$ (no. 12) によって定義されるため、命題は次の補題の帰結になります。

#### 補題 3 {#ac-iii-s2-lem-3 .statement tag=04F0}

$A$ を完全なハウスドルフ トポロジー 環とします。そこには、0 の近傍の基本系 $\mathscr{G}$、$A$ の加法部分群からなるが存在します。
(i) $\lim_{n \to m} x^n = 0$、$1 - x$ が $A$ で反転可能であり、その逆数が $\sum_{n=0}^\infty x^n$ に等しいようなすべての $x \in A$ について。
(ii) $a$ を、すべての $x \in a$ に対して $\lim_{n \to \infty} x^n = 0$ となるような $A$ の両側理想とする。 $\mathbf{A}$ の元 y が可逆であるためには、その類 mod. が必要かつ十分です。 a は $\mathbf{A}/a$ で反転可能です。特に a は、$\mathbf{A}$ のヤコブソン根基に含まれています。

(i) として

$$
(1 - x)(1 + x + \cdots + x^n) = (1 + x + \cdots + x^n)(1 - x) = 1 - x^{n+1},
$$

それはすべて、系列と一般的な項 $x^n$ が $\mathbf{A}$ に収束するという証明になります。現在、仮定までに、$\mathbf{A}$の0のすべての近傍$V \in \mathfrak{S}$に対して、すべての$n \geq p$に対して$x^n \in V$となるような整数$p > 0$が存在します。私たち結論する

$$
x^p + x^{p+1} + \ldots + x^q \in V
$$

すべての $q \geq p$ と私たちの主張はコーシーの基準 (*一般位相*、章 III, § 5, no. 2、定理 1) に従います。

(ii) $yy' \equiv 1$ (mod. a) と $y'y \equiv 1$ (mod. a) となるような $y' \in \mathbf{A}$ が存在すると仮定します。 a の仮定は、(i) によって、$yy'$ と $y'y$ が $\mathbf{A}$ で反転可能であるため、$y$ が $\mathbf{A}$ で反転可能であることを意味します。 In particular, every $x \in a$ is such that $1 - x$ is invertible in $\mathbf{A}$ and, as a is a two-sided ideal of $\mathbf{A}$, it is contained in the Jacobson radical of $\mathbf{A}$ (*Algebra*, Chapter VIII, § 6, no. 3, Theorem 1).

この補題を確立したら、それをトポロジー 環 $\hat{\mathbf{A}}$ と理想 $\hat{\mathfrak{m}}$ に適用するだけで十分です。すべての $x \in \hat{\mathfrak{m}}$、$x^n \in (\hat{\mathfrak{m}})^n \subset (\mathfrak{m}^n)^{\wedge}$、数列 $(x^n)$ は 0 になる傾向があるためです。

$\mathbf{A} = \mathbf{Z}$ を取ると、$\mathbf{Z}$ のすべての最大イデアルは形 $p\mathbf{Z}$ になります。ここで、$p$ は素数です。 $p$進数数$\mathbf{Z}_p$の環は局所環で、その$p\mathbf{Z}_p$は最大イデアル(系2から命題16)であり、その剰余体は$\mathbf{Z}/p\mathbf{Z} = \mathbf{F}_p$と同型です、そして、 $p\mathbf{Z}_{(p)}$ 進数位相を持つ $\mathbf{Z}_{(p)}$ は、$\mathbf{Z}$、含む $\mathbf{Z}$ のトポロジー 部分環と識別されます。

#### 系 {#ac-iii-s2-n13-cor-2 .statement tag=04F1}

$\mathbf{A}$ を準局所リング (章 II, § 3, no. 5)、$m_i$ をその明確な最大理想 $(1 \leq i \leq q)$ とします。

$$
r = m_1 \cap m_2 \cap \cdots \cap m_q
$$

ジェイコブソン根基です。 r 進数位相に関する $\mathbf{A}$ のハウスドルフ完全化 $\hat{\mathbf{A}}$ は準局所環であり、正準的に積 $\prod_{i=1}^q \hat{\mathbf{A}}_{m_i}$ と同型です。ここで、$\hat{\mathbf{A}}_{m_i}$ は局所環 $\mathbf{A}_{m_i}$ のハウスドルフ完全化環です。 $(m_i \mathbf{A}_{m_i})$進数の位相を尊重します。

### 練習問題 {#ac-iii-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
