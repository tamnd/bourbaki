---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 10
section_title: Derivations
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 550-574, 645-646
pdf_pages: 0574-0598, 0669-0670
extraction: ocr
subsections:
    - "no": 1
      title: COMMUTATION FACTORS
      page: 550
      pdf_page: 574
    - "no": 2
      title: GENERAL DEFINITION OF DERIVATIONS
      page: 551
      pdf_page: 575
    - "no": 3
      title: EXAMPLES OF DERIVATIONS
      page: 553
      pdf_page: 577
    - "no": 4
      title: COMPOSITION OF DERIVATIONS
      page: 554
      pdf_page: 578
    - "no": 5
      title: DERIVATIONS OF AN ALGEBRA A INTO AN A-MODULE
      page: 557
      pdf_page: 581
    - "no": 6
      title: DERIVATIONS OF AN ALGEBRA
      page: 559
      pdf_page: 583
    - "no": 7
      title: Functorial Properties
      page: 560
      pdf_page: 584
    - "no": 8
      title: RELATIONS BETWEEN DERIVATIONS AND ALGEBRA HOMOMORPHISMS
      page: 561
      pdf_page: 585
    - "no": 9
      title: EXTENSION OF DERIVATIONS
      page: 562
      pdf_page: 586
    - "no": 10
      title: UNIVERSAL PROBLEM FOR DERIVATIONS; NON-COMMUTATIVE CASE
      page: 567
      pdf_page: 591
    - "no": 11
      title: UNIVERSAL PROBLEM FOR DERIVATIONS; COMMUTATIVE CASE
      page: 568
      pdf_page: 592
    - "no": 12
      title: FUNCTIORIAL PROPERTIES OF K-DIFFERENTIALS
      page: 570
      pdf_page: 594
statements: 41
exercises: 5
content_sha256: bf9252eea7e1bbcd236d0216e67b4a71af8572cdbfa9215fd63f015817e39d10
translated_from: content/en/alg/III/10_s10_derivations.md
translation_method: google
source_content_sha256: aaeacce850abcb26b3dc2f0a2b6232e064f49c1f74a413c96833e391ff1f75f3
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 3bac597a9f82e75832c2f9c3f74fb9cc1e1dcad0e8f3b002ffb80f66a8cc6299
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 10。 導分

この段落および 〜でない限りで別途言及されている場合、考慮される代数は結合的であるとは想定されておらず、必ずしも単位元を所有しているとも想定されていません。 Kは可換環を表します。

### 1. 交換因子

この段落で特定せずに目盛りについて話す場合は、常に型 $\Delta$ の目盛りを意味します。ここで、$\Delta$ は加法的に書かれた可換群です。この段落では、$\mathbf{Z}$の値を含む$\Delta$上の交換因子を、$\Delta$上の交換因子（§ 4, no. 7、定義6）と呼びます。したがって、$\Delta$ 上の交換因子は、$\Delta \times \Delta$ の写像 $\varepsilon : (\alpha, \beta) \mapsto \varepsilon_{\alpha \beta} = \varepsilon(\alpha, \beta)$ から乗法群 $\{-1, 1\}$ に識別され、$\Delta$ の $\alpha, \alpha', \beta, \beta'$ については、

$$
\begin{cases}
\varepsilon(\alpha + \alpha', \beta) = \varepsilon(\alpha, \beta)\varepsilon(\alpha', \beta) \\
\varepsilon(\alpha, \beta + \beta') = \varepsilon(\alpha, \beta)\varepsilon(\alpha, \beta') \\
\varepsilon(\beta, \alpha) = \varepsilon(\alpha, \beta).
\end{cases}
$$

(1)

したがって、$\varepsilon(2\alpha, \beta) = \varepsilon(\alpha, 2\beta) = 1$ となります。

$\Delta = \mathbf{Z}$ の場合、すべての交換因子 $\varepsilon$ は $\varepsilon(1, 1)$ を与えることで決定されます。したがって、そのような因子は *2 つ* だけあり、最初のものは次のように定義されます。

(2)
$$
\varepsilon(p, q) = 1 \quad \text{for } p, q \text{ in } \mathbf{Z}
$$
そして2番目は
(3)
$$
\varepsilon(p, q) = (-1)^{pq} \quad \text{for } p, q \text{ in } \mathbf{Z}.
$$

### 2. 一般定義/導分

可換環 $K$、型 $\Delta : A, A', A'', B, B', B''$ の 6 つの等級付けされた $K$ モジュール、および 3 つの $K$ 線形マッピングを考慮します。
$$
\mu : A \times A' \to A'', \qquad \lambda_1 : B \times A' \to B'', \qquad \lambda_2 : A \times B' \to B''
$$
対応する $K$ 線形マッピングのようなもの
$$
A \otimes_K A' \to A'', \qquad B \otimes_K A' \to B'', \qquad A \otimes_K B' \to B''
$$
*グレードは次数* 0です。 $a \in A, a' \in A'$ の像 $\mu(a, a')$ は、単純に $a.a'$ または $aa'$ で表され、他の 2 つの双線形マッピングでも同様です。 したがって、$a.a'$ の *次数* は、$a$ と $a'$ の次数の *和* です。

#### 定義 1 {#alg-iii-s10-def-1 .statement tag=0667}

*Given the above and a commutation factor $\varepsilon$ on $\Delta \times \Delta$, an $\varepsilon$-derivation (or $(K, \varepsilon)$-derivation) of degree $\delta \in \Delta$ of $(A, A', A'')$ into $(B, B', B'')$ is a triple of graded $K$-linear mappings of degree $\delta$:*
$$
d : A \to B, \qquad d' : A' \to B', \qquad d'' : A'' \to B''
$$
*such that, for every homogeneous element $a \in A$ and every element $a' \in A'$*
(4)
$$
d''(a.a') = (da).a' + \varepsilon_{\delta, \deg(a)}a.(d'a').
$$

$a$ と $a'$ が $A$ と $A'$ のそれぞれの生成する系を通過するとき、関係 (4) を検証するには線形性により明らかに十分です。

多くの場合、3 つの写像 $d, d', d''$ を同じ文字 $d$ で表すと便利です (これは、次数 $\delta$ の段階的な $K$ 線形マッピングを $d$ で均等に表すことで正当化できます)

$$
(a, a', a'') \mapsto (da, d'a', d''a'')
$$

$A \oplus A' \oplus A''$ を $B \oplus B' \oplus B''$ に変換します)。 関係 (4) はより簡単に書くことができます
$$
d(a.a') = (da).a' + \varepsilon_{\delta,\deg(a)} a.(da').
$$
*与えられた* 次数形の $(B, B', B'')$ への $(A, A', A'')$ の $\varepsilon$ 導出、段階的線形写像の K-加群のサブ K モジュール
$$
\operatorname{Hom}_{\mathbf{K}}(A \oplus A' \oplus A'', B \oplus B' \oplus B'').
$$
$\Delta$ のすべての $\alpha, \beta$ に対して $\varepsilon(\alpha, \beta) = 1$ の場合、$\varepsilon$ 導出ではなく、単純に *導分* (または *K 導出*) と言います。 導分形のサブ K モジュール
$$
\operatorname{Hom}_{\mathbf{K}}(A \oplus A' \oplus A'', B \oplus B' \oplus B'').
$$
$\Delta = \mathbf{Z}$ と $\varepsilon(p.q) = (-1)^{pq}$ の場合、*偶数* 次数のすべての $\varepsilon$ 導出は導分です。 *奇数* 次数のすべての $\varepsilon$ 導出は、*反導出* (または *K-反導出*) と呼ばれることがよくあります。したがって、反導出$d$ は満たされます。
$$
d(a.a') = (da).a' + (-1)^{\deg(a)} a.(da')
$$
*均質* 元 $a \in A$ の場合。

#### 注意 {#alg-iii-s10-n2-rem-1 .statement tag=0668}

(1) *導分* の概念は、これらの加群に自明な等級を与えることに同意することで、等級のない加群に対して定義できます。

(2) 与えられた次数 $\delta$ の $\varepsilon$ 導出のみを考慮する場合、 交換因子 $\varepsilon$ は次のように処理できます。 双線形写像 $\lambda_2 : A \times B' \to B''$ は、双線形写像 $\lambda'_2 : A \times B' \to B''$ によって置き換えることによって変更され、 *均質* $A$ およびすべての $b' \in B'$ の $a$、
$$
\lambda'_2(a, b') = \varepsilon_{\delta, \deg(a)} \lambda_2(a, b').
$$
この場合、$d$ は、双線形マッピング $\mu, \lambda_1, \lambda'_2$ に対して導分になります。

上記の一般的な $\varepsilon$ 導出の一般的な定義は、特に 2 つの場合に使用されます。

*ケース (I)*: $A = B, A' = B', A'' = B''$ と 3 つの双線形マッピング $\mu, \lambda_1, \lambda_2$ は *同じ* 写像に等しい。

*ケース (II)*: $A = A' = A'', B = B' = B''$、つまり ($\mu$ の場合) $A$ は *等級付けされた代数* と 2 つの K 双線形マッピングです。
$$
\lambda_1 : B \times A \to B, \quad \lambda_2 : A \times B \to B
$$
対応する K-線型写像 $B \otimes_K A \to B, A \otimes_K B \to B$ は次数 0 に等級付けされます。 $A$ の次数 $\delta$ から $B$ への $\varepsilon$ 導関数は、次に等級付けされた K-線型写像 $d : A \to B$ になります。 次数 $\delta$、$A$ のすべての同種 $x$ とすべての $y \in A$ に対して、関係が得られます。
$$
d(xy) = (dx)y + \varepsilon_{\delta, \deg(a)} x(dy).
$$

特にケース (II) で、A が単位結合 K-代数であり、$\lambda_1$ と $\lambda_2$ が (A, A) 双モジュール (§ 4, no. 3, 定義 3) の外部法則である場合を考えてみましょう。これは、A と B が 2 つのユニット結合 K-代数であり、次数付き K-代数 $\rho : A \to B$ のユニット準同型が与えられ、2 つの外部法則によって定義される B 上で (A, A) バイモジュール構造が考慮される場合に特に当てはまります。

$$
\lambda_1 : (b, a) \mapsto b \rho(a), \qquad \lambda_2 : (a, b) \mapsto \rho(a)b
$$

$a \in A, b \in B$の場合。

ケース (I) と (II) では、共通のに次のケースがあります。採点された K-代数 A を考慮し、$B = A$、写像 (7) は両方とも A で乗法であるとします。 次に、等級付けされた代数 A の $\varepsilon$ 導出 (または (K, $\varepsilon$) 導出) について話します。これは、A のすべての同種 $x$ に対する次数 $\delta$、満たす (8) の、A の等級付けされた K-線型写像です。 $y \in A$。 特に、A が (結合) $\mathbf{Z}$-代数とみなされる等級付けされた環である場合、環 A の $\varepsilon$-導出について話します。

A を単位可換結合 K-代数および B A-加群とします。 A の B への導分について話すとき、常に、その A-加群構造から派生した B 上の A ビモジュール構造を意味することが理解されます。それから公式

$$
d(xy) = x(dy) + y(dx) \quad \text{for} \quad x \in A, y \in A
$$

は、このような導分 $d : A \to B$ に当てはまります。

### 3. 導分中例

#### 例 1 {#alg-iii-s10-n3-exa-1 .statement tag=0669}

A を $\mathbf{R}$ の $\mathbf{R}$ への微分可能な写像の $\mathbf{R}$-代数とし、$x_0$ を $\mathbf{R}$ の点とする。 $\mathbf{R}$ は、外部法則 $(f, a) \mapsto f(x_0)a$ とともに A-加群と考えることができます。次に、(実数変数の写像、I, § 1, no. 3) より、写像 $f \mapsto Df(x_0)$ は導分になります。

$$
(D(fg))(x_0) = (Df(x_0))g(x_0) + f(x_0)(Dg(x_0)).*
$$

#### 例 2 {#alg-iii-s10-n3-exa-2 .statement tag=066A}

X を類 $C^\infty$ の微分可能な多様体とし、A を X 上の微分形の段階付き$\mathbf{R}$-代数とする。 X の外微分 $d\omega$ 上のすべての微分形 $\omega$ に関連する写像は、次数 +1 (微分可能および解析的多様体、R、§ 8) の逆導出です。*

#### 例 3 {#alg-iii-s10-n3-exa-3 .statement tag=066B}

A を連想 K-代数とします。すべての $a \in A$、写像 $x \mapsto ax - xa$ は、代数 A (cf. no. 6) の導分です。

#### 例 4 {#alg-iii-s10-n3-exa-4 .statement tag=066C}

M を K-加群とし、A を通常の目盛 (§ 7, no. 1) を持つ外装代数 $\bigwedge(M^*)$ とします。 *すべての $x \in M$ について、右内部積 $i(x)$ は次数 $-1$ の A の逆導出であることが § 11, no. 9 でわかります。

#### 例 5 {#alg-iii-s10-n3-exa-5 .statement tag=066D}

Returning to the general situation of Definition 1 of no. 2, let $\overline{K}$ be another commutative ring and $\rho : K \to \overline{K}$ a ring homomorphism; let $\overline{A}, \overline{A}', \overline{A}'', \overline{B}, \overline{B}', \overline{B}''$ denote the graded $\overline{K}$-modules obtained respectively from $A, A', A'', B, B', B''$ by extending the ring of scalars to $\overline{K}$ (II, § 11, no. 5); we derive from $\mu, \lambda_1$ and $\lambda_2$ $\overline{K}$-bilinear mappings
$$
\bar{\mu} : \overline{A} \times \overline{A}' \to \overline{A}'', \quad \bar{\lambda}_1 : \overline{B} \times \overline{A}' \to \overline{B}'', \quad \bar{\lambda}_2 : \overline{A} \times \overline{B}' \to \overline{B}''
$$
by considering the tensor products by $l_{\overline{K}}$ of the corresponding $K$-linear mappings to $\mu, \lambda_1$ and $\lambda_2$ (II, § 5, no. 1). Then, if $d$ is an $\varepsilon$-derivation of degree $\delta$ of $(A, A', A'')$ into $(B, B', B'')$, the mapping $\bar{d} = d \otimes l_{\overline{K}}$ of $\overline{A} \oplus \overline{A}' \oplus \overline{A}''$ into $\overline{B} \oplus \overline{B}' \oplus \overline{B}''$ is an $\varepsilon$-derivation of degree $\delta$ of $(\overline{A}, \overline{A}', \overline{A}'')$ into $(\overline{B}, \overline{B}', \overline{B}'')$.

#### 例 6 {#alg-iii-s10-n3-exa-6 .statement tag=066E}

$A$ を型 $\mathbf{Z}$ の段階的 $K$-代数とする。 次数 0、$d : A \to A$ の段階的線形 $K$ マッピングは、$x_n \in A_n (n \in \mathbf{Z})$、$d(x_n) = nx_n$ を取得することによって定義されます。この写像は、$x_p \in A_p, x_q \in A_q$ の場合、$A$ の導分です。
$$
d(x_p x_q) = (p + q)x_p x_q = d(x_p)x_q + x_p d(x_q).
$$

### 4. 導分中合成

このNo.で推測します。 no. 2 のケース (I) が成り立ちます。つまり、$A, A', A''$ は、型 $\Delta$ の 3 つの等級付けされた $K$ モジュールであり、等級付けされたモデルへの $K$ 双線形写像 $\mu : A \times A' \to A''$ 対応するが与えられます。 次数 0、$A \otimes_K A' \to A''$ の$K$ 線形マッピング。 $f(A) \subset A, f(A') \subset A'$ と $f(A'') \subset A''$ 形のような $A \oplus A' \oplus A''$ の等級付けされた自己準同型 $f$ は、等級付けされた連想代数 $\mathrm{Endgr}_K(A \oplus A' \oplus A'')$ (§ 3, no. 1、例) の等級付けされた部分代数 2)。特に、$(A, A', A'')$ の 2 つの $\varepsilon$ 派生は構成できますが、2 つの $\varepsilon$ 派生のうち合成が $\varepsilon$ 派生であると考えるべきではありません。

型 $\Delta$ のすべての等級付けされた代数 $B$ では、公式によって 2 つの同種元 $u, v$ の$\varepsilon$ 括弧 (または、$\varepsilon = 1$ の場合は単に括弧) が定義されます (10)
$$
[u, v]_\varepsilon = uv - \varepsilon_{\deg u, \deg v} vu \text{ (denoted simply by } [u, v] \text{ if } \varepsilon = 1).
$$
この写像を線形性で拡張すると、$B \times B$から$B$への$K$双線形写像$(u, v) \mapsto [u, v]_\varepsilon$が得られます。次に、$B$ の同次$u$ と $v$ について、
$$
[v, u]_\varepsilon = -\varepsilon_{\deg u, \deg v}[u, v]_\varepsilon.
$$
適用この定義から段階的代数 $\mathrm{Endgr}_K(A \oplus A' \oplus A'')$ へ、2 つの段階的自己準同型の$\varepsilon$ 括弧が定義されます。

#### 命題 1 {#alg-iii-s10-prop-1 .statement tag=066F}

*$d_1, d_2$ を、それぞれの次数 $\delta_1, \delta_2$ の $(A, A', A'')$ の 2 つの $\varepsilon$ 派生とします。次に、$\varepsilon$-括弧*
$$
[d_1, d_2]_\varepsilon = d_1 \circ d_2 - \varepsilon_{\delta_1, \delta_2} d_2 \circ d_1
$$
* は次数 $\delta_1 + \delta_2$ の $\varepsilon$ 派生です。さらに、$d$ が次数 $\delta$ の $(A, A', A'')$ の $\varepsilon$ 導関数であり、$\varepsilon_{\delta, \delta} = -1$ である場合、$d^2 = d \circ d$ は導分です。*

$x \in A$ が次数 $\xi$ と同次であると仮定します。 $y \in A'$ 全員にとって、
$$
d_1(d_2(xy)) = ((d_1 d_2)(x))y + \varepsilon_{\delta_1, \delta_2 + \xi}(d_2 x)(d_1 y)
+ \varepsilon_{\delta_2, \xi}(d_1 x)(d_2 y) + \varepsilon_{\delta_1 + \delta_2, \xi} x((d_1 d_2)(y))
$$
no. 1の式(1)を考慮します。 $d_1$ と $d_2$ の役割を交換すると、(1) (no. 1) を使用して再度簡略化した後でが得られます。
$$
(d_1 d_2)(xy) - \varepsilon_{\delta_1, \delta_2}(d_2 d_1)(xy) = ((d_1 d_2)(x))y - \varepsilon_{\delta_1, \delta_2}((d_2 d_1)(x))y
+ \varepsilon_{\delta_1 + \delta_2, \xi} x((d_1 d_2)(y))
- \varepsilon_{\delta_1, \delta_2} \varepsilon_{\delta_1 + \delta_2, \xi} x((d_2 d_1)(y))
$$
つまり、$d = [d_1, d_2]_\varepsilon$ と $\delta = \delta_1 + \delta_2$ を書くと、
$$
d(xy) = (dx)y + \varepsilon_{\delta, \xi} x(dy)
$$
これは、$d$ が $\varepsilon$ から派生したものであることを証明します。

一方、(11) で $d_1 = d_2 = d$、$\delta_1 = \delta_2 = \delta$、$\varepsilon_{\delta, \delta} = -1$ とすると、それ以降 (1) により $\varepsilon_{\delta, \delta + \xi} = -\varepsilon_{\delta, \xi}$ が得られます。
$$
d^2(xy) = (d^2 x)y + \varepsilon_{2\delta, \xi} x(d^2 y)
$$
そして、$\varepsilon_{2\delta, \xi} = 1$ として、$d^2$ は導分であることがわかります。

#### 系 {#alg-iii-s10-n4-cor-1 .statement tag=066G}

※$\Delta = \mathbf{Z}$とします。次に:*
(i) 逆導出の *平方は導分です。*
(ii) *2 つの導分のかっこは導分です。*
(iii) *逆導出の括弧と次数の導分は逆導出です。*
(iv) *$d_1$ と $d_2$ が逆導出である場合、$d_1 d_2 + d_2 d_1$ は導分です。

この番号の始まりの仮説の下で、$(A, A', A'')$ の *ペアごとに置換可能な導分* の有限列 $D = (d_i)_{1 \leq i \leq n}$ を考えてみましょう。 代数 $K[X_1, \ldots, X_n]$ のすべての多項式 $P(X_1, \ldots, X_n)$ について、$\mathrm{Endgr}_K(A \oplus A' \oplus A'')$ の元 $P(d_1, \ldots, d_n)$ が定義されます (§ 2, no. 9)。 記法の省略形は $P(D)$ です。

#### 命題 2 {#alg-iii-s10-prop-2 .statement tag=066H}

*上記の仮説と記法を使用して、2n の不定数 $T_1, \ldots, T_n, T'_1, \ldots, T'_n$ を考慮し、すべての多項式 $F \in K[X_1, \ldots, X_n]$ に対して $F(T) = F(T_1, \ldots, T_n), F(T') = F(T'_1, \ldots, T'_n)$ を書き込み、*
$$
F(T + T') = F(T_1 + T'_1, \ldots, T_n + T'_n).
$$
*次のように仮定します*
$$
P(T + T') = \sum_i Q_i(T) R_i(T')
$$
*ここで、$Q_i$ と $R_i$ 属するから $K[X_1, \ldots, X_n]$ までです。次に、すべての $x \in A$ と $y \in A'$ について、*
$$
P(D)(xy) = \sum_i (Q_i(D)x)(R_i(D)y).
$$

他の不定数 $n$ $T_1'', \ldots, T_n''$ を導入し、多項式代数 $K[T_1, \ldots, T_n, T_1', \ldots, T_n', T_1'', \ldots, T_n''] = B$ を検討します。一方、$A \times A'$の双線形写像の$K$加群$M$を$A''$に考慮します。 $B$ モジュール構造は、$K$-双線形写像 $f \in M$ および $1 \leq i \leq n$ ごとに、次のように書くことによって $M$ に定義されます。

$$
\begin{cases}
(T_i f)(a, a') = f(d_i a, a') \\
(T_i' f)(a, a') = f(a, d_i a') \\
(T_i'' f)(a, a') = d_i(f(a, a'))
\end{cases}
$$

$d_i$ は 1 つの他ので置換可能であるため、すべての多項式 $F \in K[X_1, \ldots, X_n]$、$(F(T)f)(a, a') = f(F(D)a, a')$ について、

$$
(F(T')f)(a, a') = f(a, F(D)a')
$$

そして$(F(T'')f) = F(D)(f(a, a'))$。したがって、(12) を証明するには、次のことを示せば十分です。

$$
(P(T'') - \sum_i Q_i(T)R_i(T')).\mu = 0
$$

または、$B$ モジュール $M$ の $(P(T'') - P(T + T')).\mu = 0$。 Now, the hypothesis that the $d_i$ are derivations can also be expressed by saying that, for $1 \leq i \leq n$,

$$
(T_i'' - T_i - T_i').\mu = 0
$$

$B$ モジュール $M$ 内。多項式を逐次考えることで

$P(T_1'', T_2'', \ldots, T_n'') - P(T_1 + T_1', T_2'', \ldots, T_n'')$
$P(T_1 + T_1', T_2'', \ldots, T_n'') - P(T_1 + T_1', T_2 + T_2', \ldots, T_n'')$
$\ldots$
$P(T_1 + T_1', \ldots, T_{n-1} + T_{n-1}', T_n'') - P(T_1 + T_1', \ldots, T_{n-1} + T_{n-1}', T_n + T_n')$

差分$P(T'') - P(T + T')$は形に書き込むことができることがわかります。

$$
\sum_{i=1}^n (T_i'' - T_i - T_i') G_i(T, T', T'')
$$

ここで、$G_i$ は $B$ の元です。したがって、関係 (14) は、関係 (15) の明らか帰結です。

#### 系 (ライプニッツの公式) {#alg-iii-s10-n4-cor-2 .statement tag=066I}

*$d_i$ ($1 \leq i \leq n$) を他の 1 つで置換可能な $(A, A', A'')$ の $n$ 導分とします。 $\alpha = (\alpha_1, \ldots, \alpha_n) \in \mathbf{N}^n$ 全員について、私たちは書きます*

$$
d^\alpha = d_1^{\alpha_1} d_2^{\alpha_2} \ldots d_n^{\alpha_n}.
$$

次に、$x \in \mathbf{A}$ と $y \in \mathbf{A}'$ については、

$$
d^\alpha(xy) = \sum_{\beta + \gamma = \alpha} ((\beta, \gamma)) d^\beta(x)d^\gamma(y)
$$

と書いたところ（章の冒頭で紹介した記法）

$$
((\beta, \gamma)) = (\beta + \gamma)!/(\beta! \gamma!).
$$

これは、多項式公式 (I, § 8, no. 2) の直後に続きます。

$$
(T + T')^\alpha = \sum_{\beta + \gamma = \alpha} ((\beta, \gamma)) T^\beta {T'}^\gamma
$$

と命題 2.

### 5.  代数の導分を A-加群に

このNo.で推測します。 no. 2 の場合 (II) が成り立ちます。次に、グレード付けされた K-代数 A とグレード付けされた K-加群 E があり、さらに 2 つの次数 0 の K-線型写像があります。

$$
E \otimes_K A \to E, \quad A \otimes_K E \to E
$$

で示される

$$
x \otimes a \mapsto x.a \quad \text{and} \quad a \otimes x \mapsto a.x \quad \text{for } a \in A \text{ and } x \in E.
$$

#### 命題 3 {#alg-iii-s10-prop-3 .statement tag=066J}

$d : A \to E$ を次数 $\delta$ の $\varepsilon$ 導関数とします。この場合、$\mathrm{Ker}(d)$ は A のグレード部分代数です。 Aが単位元を認めれば、属するから$\mathrm{Ker}(d)$になります。

明らかに、$\mathrm{Ker}(d)$ は A の段階的なサブ K モジュールです。さらに、no. 2 の関係 (8) は、$x$ と $y$ が 2 つの同種元所属から $\mathrm{Ker}(d)$ である場合、$d(xy) = 0$、したがって $xy \in \mathrm{Ker}(d)$ であることを示しています。最後に、A が単位元 1 (次数 0、cf. § 3, no. 1) を認める場合、no. 2 の関係 (8) ($x$ と $y$ を 1 に置き換えると、$d(1) = d(1) + d(1)$ になります) $d(1) = 0$。

#### 系 {#alg-iii-s10-n5-cor-1 .statement tag=066K}

$d_1$ と $d_2$ を、同じ次数 $\delta$ の A から E までの 2 つの $\varepsilon$ 派生とします。 $d_1$ と $d_2$ が生成する系の代数 A の各元で同じ値を取る場合、$d_1 = d_2$ になります。

$d_1 - d_2$ は次数 $\delta$ の $\varepsilon$ 導関数であるため、$\mathrm{Ker}(d_1 - d_2)$ は A の部分代数であり、A の含む生成する系であるため、A と等しくなります。

#### 命題 4 {#alg-iii-s10-prop-4 .statement tag=066L}

$d : A \to E$ を次数 $\delta$ の $\varepsilon$ 導関数とします。 A が単位元 1 を持ち、$x$ を A の逆数 $x^{-1}$ を持つ A の同次元とします。

$$
d(x^{-1}) = -\varepsilon_{\delta, \deg(x)} x^{-1}((dx)x^{-1}) = -\varepsilon_{\delta, \deg(x)} (x^{-1}(dx))x^{-1}.
$$

$d(xx^{-1}) = d(1) = 0$ (命題 3)、よってがあります
$$
(dx)x^{-1} + \varepsilon_{\delta, \deg(x)} x(d(x^{-1})) = 0
$$
これは (19) の最初の公式を証明します。一方、$x^{-1}$ は、no. 1 の式 (1) より、次数 $-\deg(x)$ と$\varepsilon_{\delta, \deg(x)} = \varepsilon_{\delta, -\deg(x)}$ が同次です。 $d(x^{-1}x) = 0$と書くと、(19)の2番目の公式も同様に得られます。

#### 命題 5 {#alg-iii-s10-prop-5 .statement tag=066M}

*$\mathbf{A}$ が整域で、$\mathbf{L}$ が分数の体であるとします。 $\mathbf{A}$ のすべての導分から $\mathbf{L}$ 上のベクトル空間 $\mathbf{E}$ ($\mathbf{A}$ モジュールとみなされる) は、$\mathbf{L}$ の $\mathbf{E}$ の導分に一意に拡張できます。

$d$ を $\mathbf{A}$ の導分を $\mathbf{E}$ に、$\bar{d}$ 導分を $\mathbf{L}$ から $\mathbf{E}$ に延長して $d$ とします。次に、$u \in \mathbf{A}, v \in \mathbf{A}, v \neq 0$ については、(19) のおかげで、必然的に、
$$
\bar{d}(u/v) = v^{-1}du - uv^{-2}dv
$$
これは、$\bar{d}$ の一意性を証明します。逆に、$\bar{d}$ は公式 (20) によって定義できることを示します。 (20) の右辺の $u/v = u'/v'$ 値が、$u$ が $u'$ に、$v$ が $v'$ に置き換えられたときに、変更にならないことを最初に検証する必要があります。さて、$uv' = vu'$、したがって$v'(du) + u(dv') = v(du') + u'(dv)$、そして$uv'v^{-1} = u'$と$u'{v'}^{-1}v = u$なので、$v'(du - uv^{-1}dv) = v(du' - u'{v'}^{-1}dv')$です。したがって、写像 $\bar{d}: \mathbf{L} \to \mathbf{E}$ は拡大する $d$ と定義されています。 $\mathbf{K}$-線形であり、導分であることがすぐに検証されます。

#### 命題 6 {#alg-iii-s10-prop-6 .statement tag=066N}

*$\mathbf{A}$ が段階化された $\mathbf{K}$-代数の単位結合であり、$\mathbf{E}$ が段階化された $(\mathbf{A}, \mathbf{A})$-双モジュールであると仮定します。 $d : \mathbf{A} \to \mathbf{E}$ が次数 $\delta$ の $\varepsilon$ 導関数である場合、$\mathbf{A}$ の同次元の各有限列 $(x_i)_{1 \leq i \leq n}$ について、それぞれの次数 $\xi_i$ ($1 \leq i \leq n$)、
$$
d(x_1 x_2 \ldots x_n) = \sum_{i=1}^n \varepsilon_{\delta, \xi_1 + \cdots + \xi_{i-1}} x_1 \cdots x_{i-1} (dx_i) x_{i+1} \cdots x_n.
$$
公式 (21) は $n = 0$ に対して自明であり、(4) (no. 2) を考慮して、$n$ 上の帰納法によって証明されます。

#### 系 {#alg-iii-s10-n5-cor-2 .statement tag=066O}

*$\mathbf{A}$ が単位可換結合代数であり、$\mathbf{E}$ が $\mathbf{A}$ 加群であると仮定します。 $d : \mathbf{A} \to \mathbf{E}$ が導分の場合、整数 $n \geq 0$ ごとに、
$$
d(x^n) = nx^{n-1}(dx) \quad \text{for all } x \in \mathbf{A}.
$$
$\mathbf{A}$ に自明な卒業を与え、すべての $x_i$ が $x$ に等しいとして (21) を適用するだけで十分です。

次数 $\delta$ の $\varepsilon$ 導出 $d : \mathbf{A} \to \mathbf{E}$ の一般的なケースに戻ります。 $Z_\delta$ を $a \in \mathbf{A}$ の集合とすると、次数 $\alpha$ の同次成分 $a$ の $a_\alpha$ について、$\mathbf{E}$ のすべての同次 $x$ について、
$$
xa_\alpha = \varepsilon_{\alpha, \deg(x)} a_\alpha x.
$$

$A$ が代数に等級付けされた単位結合であり、$E$ が等級付けされた $(A, A)$ バイモジュールである場合、この定義からすぐに、$Z_\varepsilon$ は $A$ 含むの *等級付けされた部分代数* になります。 単位元。

#### 命題 7 {#alg-iii-s10-prop-7 .statement tag=066P}

*$A$ が代数に等級付けされた単位結合であり、$E$ が等級付けされた $(A, A)$ バイモジュールであると仮定します。 $d : A \to E$ を次数 $\delta$ の $\varepsilon$ 微分とし、$a$ を次数 $\alpha$ の $Z_\varepsilon$ の同次元とします。したがって、写像 $x \mapsto a(dx)$ は、次数 $\delta + \alpha$ の $\varepsilon$ 導関数です。*

$d'(x) = a(dx)$と書きます。 $A$ と $y \in A$ の次数 $\xi$ の同次の $x$ について、(23) と (1) (no. 1) により、

$$
d'(xy) = a((dx)y) + \varepsilon_{\delta, \xi} a(x(dy)) = (a(dx))y + \varepsilon_{\delta+\alpha, \xi}(xa)(dy)
= (d'x)y + \varepsilon_{\delta+\alpha, \xi} x(d'y).
$$

命題 7 は、$A$ から $E$ への $\varepsilon$ 導出の K-加群は、型 $\Delta$ の *等級付き $Z_\varepsilon$* 加群であると述べています。

### 6. 導分/代数

$A$ を等級付けされた K-代数とします。すべての*同種* 元 $a \in A$ について、$\mathrm{ad}_\varepsilon(a)$ とするか、混乱が生じない場合は単純に $\mathrm{ad}(a)$ として、$A$ の K-線型写像を $A$ と表します。

$$
x \mapsto [a, x]_\varepsilon
$$
(no. 4, 公式 (10)) これは *次数* $\deg a$ の評価です。

#### 命題 8 {#alg-iii-s10-prop-8 .statement tag=066Q}

*$A$ を採点済みの K-代数とします。*

(i) *すべての $\varepsilon$*-派生 $d : A \to A$ および $A$ のすべての同次元 $a$ について、

$$(24)$$
$$
[d, \mathrm{ad}_\varepsilon(a)]_\varepsilon = \mathrm{ad}_\varepsilon(da).
$$

(ii) *代数 $A$ が結合的である場合、$\mathrm{ad}_\varepsilon(a)$ は次数 $\deg(a)$ の $A$ の $\varepsilon$* 導出です。

(i) $d$ が次数 $\delta$ であると仮定し、$\alpha = \deg a$ として、$f = [d, \mathrm{ad}_\varepsilon(a)]_\varepsilon$ と書きます。 次数 $\xi$ のすべての同次元 $x \in A$ について、(1) (no. 1) により、

$$
f(x) = d(ax - \varepsilon(\alpha, \xi) xa) - \varepsilon_{\delta, \alpha}(a(dx)) - \varepsilon_{\alpha, \delta+\xi}(dx)a \\
= (da)x + \varepsilon_{\delta, \alpha} a(dx) - \varepsilon_{\alpha, \xi}(dx)a - \varepsilon_{\delta+\alpha, \xi} x(da) \\
- \varepsilon_{\delta, \alpha} a(dx) + \varepsilon_{\alpha, \xi}(dx)a \\
= (da)x - \varepsilon_{\delta+\alpha, \xi} x(da) = [da, x]_\varepsilon.
$$

(ii) 次数 $\xi$ の同次のすべての $x$ と、$A$ の次数 $\eta$ の同次のすべての $y$ について、

$$
\mathrm{ad}_\varepsilon(a)(xy) = a(xy) - \varepsilon_{\alpha, \xi+\eta}(xy)a \\
= (ax - \varepsilon_{\alpha, \xi} xa)y + \varepsilon_{\alpha, \xi} x(ay - \varepsilon_{\alpha, \eta} ya) \\
= \mathrm{ad}_\varepsilon(a)(x).y + \varepsilon_{\alpha, \xi} x.\mathrm{ad}_\varepsilon(a)(y)
$$
(1) と $A$ の結合性を考慮します。

$A$ が結合する場合、$\mathrm{ad}_\varepsilon(a)$ は、$a$ によって定義される $A$ の *内部 $\varepsilon$ 派生* と呼ばれます。

#### 系 {#alg-iii-s10-n6-cor-1 .statement tag=066R}

*$A$ を連想グレードの代数とします。 2 つの同種の元、$a, b$ の $A$、* の場合
$$
[\mathrm{ad}_\varepsilon(a), \mathrm{ad}_\varepsilon(b)]_\varepsilon = \mathrm{ad}_\varepsilon([a, b]_\varepsilon).
$$
(25)

(24) で $\mathrm{ad}_\varepsilon(a)$ によって置き換える $d$ と $\mathrm{ad}_\varepsilon(b)$ によって $\mathrm{ad}_\varepsilon(a)$ が得られれば十分です。

$\deg a = \alpha, \deg b = \beta$ の場合、公式 (25) は、次数 $\gamma$ の同次元 $c \in A$ ごとに、次の関係と等価です。
$$
\varepsilon_{\alpha, \gamma}[a, [b, c]_\varepsilon]_\varepsilon + \varepsilon_{\beta, \alpha}[b, [c, a]_\varepsilon]_\varepsilon + \varepsilon_{\gamma, \beta}[c, [a, b]_\varepsilon]_\varepsilon = 0
$$
*ヤコビアイデンティティ*と呼ばれます。

### 7. 機能特性

*この番号では、すべての代数は結合および単体であると想定され、すべての代数準同型は単体であると想定されます。

#### 命題 9 {#alg-iii-s10-prop-9 .statement tag=066S}

*$A, B$ を 2 つの段階的な $K$-代数、$E$ 1 つの $(A, A)$-双モジュール、および $F$ を段階的な $(B, B)$-二モジュールとします。 $\rho : A \to B$ を等級付き代数準同型とし、$\theta : E \to F$ を次数 0 の $A$ バイモジュール ($\rho$ を基準とした) の等級付き $A$ 準同型写像とします。

*(i)* *すべての $\varepsilon$-派生 $d' : B \to F$ に対して、$d' \circ \rho : A \to \rho^*(F)$ は同じ次数の $\varepsilon$-派生です。*
*(ii)* *すべての $\varepsilon$-派生 $d : A \to E$ に対して、$\theta \circ d : A \to \rho^*(F)$ は同じ次数の $\varepsilon$-派生です。*

関係のすぐ後に 2 つの主張が続きます
$$
d'(\rho(xy)) = d'(\rho(x)\rho(y)) = d'(\rho(x))\rho(y) + \varepsilon_{\delta', \xi}\rho(x)d'(\rho(y))
$$
$$
\theta(d(xy)) = \theta((dx)y + \varepsilon_{\delta, \xi}x(dy)) = \theta(dx)\rho(y) + \varepsilon_{\delta, \xi}\rho(x)\theta(dy)
$$
$x \in A$ の同種の次数 $\xi$ と $y \in A$、$\delta$ と $\delta'$ は、$d$ と $d'$ のそれぞれの次数を示します。

#### 系 {#alg-iii-s10-n7-cor-1 .statement tag=066T}

※$S$を代数$A$の生成する系とします。 $d' \circ \rho = \theta \circ d$の位数では、すべての$x \in S$に対して$d'(\rho(x)) = \theta(d(x))$があれば必要十分です。*

これは、命題 9 と no. 5、系 ～ 命題 3 の明らか帰結です。

命題 9 の条件では、$B$ が ($\rho$ によって) $(A, A)$ バイモジュール構造 (II, § 1, no. 14, *例 1*) を持っていることがわかります。

#### 命題 10 {#alg-iii-s10-prop-10 .statement tag=066U}

*命題 9 の条件では、$\varepsilon$ 導出$d' : B \to F$ が、$B$ と $\rho^*(F)$ の左 (それぞれ右) $A$ モジュール構造に対して $A$ 線形であるためには、次のことが必要かつ十分です。 $d'$ は $B$ の部分代数 $\rho(A)$ に零になります。*

左A-加群構造に対して証明を実行します。 $a \in A, b \in B$の場合、
$$
d'(\rho(a)b) = d'(\rho(a))b + \rho(a)d'b
$$
したがって、$d' \circ \rho = 0$ の場合、$d'$ は B および $\rho^*(F)$ の左A-加群構造に対して線形です。逆に、そうだとしたら特に
$$
d'(\rho(a)) = d'(\rho(a).1) = \rho(a)d'(1) = 0
$$
(no. 5、命題 3)。

特に、$D_K(B, F)$ は B の導分の K-加群を F (no. 2) に表すものとします。これらの導分は A-linear であり、他の語は $\rho(A)$ の零、形 $D_K(B, F)$ のサブ K モジュールであり、$D_{A,\rho}(B, F)$ または単に $D_A(B, F)$ で示されます (明らかに$D_K(B, F) = D_{K,\phi}(B, F)$、ここで、$\phi : K \to B$ は、B) の K-代数構造を定義する準同型です。

ここで、A、B、C を 3 つの等級付け K-代数、$\rho : A \to B, \sigma : B \to C$ 2 つの等級付け代数準同型、G を等級付けされた (C、C) バイモジュールとします。 $D_A(B, G)$、$D_B(C, G)$、$D_A(C, G)$ がそれぞれK-加群、$D_{A,\rho}(B, \sigma_*(G))$、$D_{B,\sigma}(C, G)$、$D_{A,\sigma \circ \rho}(C, G)$ を表す場合、$\sigma(\rho(A)) \subset \sigma(B)$ 以降、$D_B(C, G)$ は明らかに$D_A(C, G)$ のサブ K モジュールです。

#### 命題 11 {#alg-iii-s10-prop-11 .statement tag=066V}

*上記の条件の下に、K 準同型射の完全系列があります*
$$
0 \to D_B(C, G) \xrightarrow{u} D_A(C, G) \xrightarrow{v} D_A(B, G)
$$
*ここで、u は標準単射 、v は準同型 $d \mapsto d \circ \sigma$* (命題 9) です。

The kernel of v is the set of derivations $d : C \to G$ such that $d(\sigma(b)) = 0$ for all $b \in B$, which is precisely the image of u.

### 8. 導分と代数準同型の間の関係

この番号でもう一度仮定します。 no. 2 の *Case (II)* が成り立ち、等級付けされた K-代数 A は結合すると想定されません。 元 $\delta \in \Delta$ が与えられた場合、次のような等級付けされた K-加群 E($\delta$) (II, § 11, no. 2) を考慮します。
$$
(E(\delta))_\mu = E_{\mu+\delta}
$$
$\mu \in \Delta$ 全員のために。私たちは、同種の元 $a \in A$ と任意の元 $a' \in A, x, x'$ に対して、K-加群 $A \oplus E(\delta)$ で * 採点 K-代数* 構造を設定で定義するとしました。 $E(\delta)$
$$
(a, x)(a', x') = (aa', x.a' + \varepsilon_{\delta, \deg(a)} a.x');
$$
この乗法定義するの採点環構造が明らかであるという事実の検証。

射影 $p : (a, x) \mapsto a$ は、代数 $A \oplus E(\delta)$ の拡張と呼ばれ、グレード化された代数準同型です。 次数 0 のうち K-線型写像 $g : A \to A \oplus E(\delta)$ は、合成となる

$$
A \xrightarrow{g} A \oplus E(\delta) \xrightarrow{p} A
$$

アイデンティティ $1_A$ は形 $x \mapsto (x, f(x))$ の写像であり、$f : A \to E$ は次数 $\delta$ のグレード付けされた K-線型写像です。

#### 命題 12 {#alg-iii-s10-prop-12 .statement tag=066W}

*次数 $\delta$ の等級付けされた K-線型写像 $f : A \to E$ が $\varepsilon$ 派生となるためには、A の写像 $x \mapsto (x, f(x))$ から $A \oplus E(\delta)$ が等級付けされた K-代数準同型であることが必要かつ十分です。

$x$ が $A$ と $y \in A$ で均一であるという事実を利用する

$$
(xy, f(xy)) = (x, f(x)).(y, f(y)),
$$

(28) を考慮して、同等の関係を取得します。

$$
f(xy) = f(x).y + \varepsilon_{\delta, \deg(x)} x.f(y),
$$

よって命題。

#### 命題 13 {#alg-iii-s10-prop-13 .statement tag=066X}

*代数 $A \oplus E(\delta)$ が結合的かつ単一であるためには、$A$ が結合的かつ単一であること、および $E$ 上の写像 $(a, x) \mapsto a.x$ および $(a, x) \mapsto x.a$ 定義するが $(A, A)$ バイモジュール構造であることが必要かつ十分です。 $A \oplus E(\delta)$ の単位元は $(1, 0)$ になります。*

元 $(u, m) \in A \oplus E(\delta)$ がこの代数の単位元として書かれている場合、$u$ は $A$ の単位元でなければならないことがすぐにわかります。 $(u, m).(0, x) = (0, x).(u, m) = (0, x)$と書くと、$x \in E$に対して$u.x = x.u = x$が得られ、$(u, m).(u, 0) = (u, 0).(u, m) = (u, 0)$と書くと、$m = 0$が得られます。 $A \oplus E(\delta)$ のときに $A$ が結合的であるという事実は、拡張が全射準同型であるという事実からわかります。 The condition $(x.a').a'' = x.(a'.a'')$ is then equivalent to $((0, x)(a', 0))(a'', 0) = (0, x)((a', 0)(a'', 0))$ and similarly the condition $a.(a'.x) = (a.a').x$ is equivalent to

$$
(a, 0)((a', 0)(0, x)) = ((a, 0)(a', 0))(0, x);
$$

最後に条件 $a.(x.a') = (a.x).a'$ は以下と同等です

$$
(a, 0)((0, x)(a', 0)) = ((a, 0)(0, x))(a', 0).
$$

### 9. 導分中拡大

#### 命題 14 {#alg-iii-s10-prop-14 .statement tag=066Y}

*$A$を可換環、$M$を$A$モジュール、$B$を$A$代数$T(M)$（それぞれ$S(M)$、それぞれ$\Lambda(M)$）、$E$をaとします。 $(B, B)$-バイモジュール。 $d_0 : A \to E$ を環 $\mathbf{A}$ の導分として $\mathbf{A}$ モジュール $\mathbf{E}$ と $d_1 : M \to \mathbf{E}$ 加法群準同型に入れると、すべての $a \in \mathbf{A}$ とすべての $x \in M$ について、

$$
(29) \quad d_1(ax) = ad_1(x) + d_0(a) \cdot x,
$$

さらに、$B = S(M)$のとき、

$$
(30) \quad x \cdot d_1(y) + d_1(x) \cdot y = y \cdot d_1(x) + d_1(y) \cdot x
$$

$M$ のすべての $x, y$、そして $B = \bigwedge(M)$ のとき、

$$
(31) \quad x \cdot d_1(x) + d_1(x) \cdot x = 0
$$

$x \in M$の皆さんへ。次に、$(B, B)$-双モジュール $\mathbf{E}$ には、$d|_{\mathbf{A}} = d_0$ と $d|_{M} = d_1$ のように、$B$ ($\mathbf{Z}$-代数とみなされる) の導分 $d$ が 1 つだけ存在します。

以下で定義される$\mathbf{Z}$加群$B \oplus \mathbf{E}$の結合$\mathbf{Z}$-代数構造を取り上げます。

$$
(b, t)(b', t') = (bb', bt' + tb')
$$

これは、$(1, 0)$ を単位元 (no. 8、命題 13) とします。 標準単射 $t \mapsto (0, t)$ では、$\mathbf{E}$ は $\mathbf{E}^2 = \{0\}$ となるような $B \oplus \mathbf{E}$ の両側の理想と同一視されます。 一方、$h_0(a) = (a, d_0(a))$ によって定義される写像 $h_0 : B \oplus \mathbf{E}$ は、環準同型 (no. 8, 命題 12) です。この写像の下で、$B \oplus \mathbf{E}$は$\mathbf{A}$-代数になります。 さらに、すべての $x \in M$ について、$h_1(x) = (x, d_1(x))$ と書くと、$h_0$ の定義と (29) から $h_1(ax) = h_0(a)h_1(x)$ が得られます。他の語 $h_1$ は、$M$ から $B \oplus \mathbf{E}$ への $\mathbf{A}$ 線形マッピングです。 Then there exists one and only one $\mathbf{A}$-algebra homomorphism, $h : B \to B \oplus \mathbf{E}$ such that $h|_M = h_1$ (and necessarily $h|_{\mathbf{A}} = h_0$): for, if $B = T(M)$, this follows from $§ 5$, no. 1, Proposition 1; if $B = S(M)$, condition (30) shows that $h(x)h(y) = h(y)h(x)$ for all $x, y$ in $M$ and the conclusion follows from $§ 6$, no. 1, Proposition 2; finally if $B = \bigwedge(M)$, condition (31) shows that $(h(x))^2 = 0$ for all $x \in M$, since $x \wedge x = 0$ and the conclusion follows from $§ 7$, no. 1, Proposition 1. The homomorphism $h$ is such that the composition $p \circ h : B \to B$ with the augmentation $\rho : B \oplus \mathbf{E} \to B$ is the identity $l_B$, for $p \circ h$ and $l_B$ coincide by definition for the elements of $\mathbf{A}$ and those of $M$ and the set of these elements is a generating system of $B$. We can therefore write $h(b) = (b, d(b))$ for all $b \in B$ and the mapping $b \mapsto d(b)$ of $B$ into $\mathbf{E}$ is a derivation with the required properties, by virtue of Proposition 12 of no. 8.

#### 系 {#alg-iii-s10-n9-cor-1 .statement tag=066Z}

*Let $M$ be a graded $K$-module of type $\Delta$; the $K$-algebras $T(M)$, $S(M)$ and $\bigwedge(M)$ are given the corresponding graduations of type $\Delta' = \Delta \times \mathbf{Z}$ ($§ 5$, no. 5, Proposition 7, $§ 6$, no. 6, Proposition 10 and $§ 7$, no. 7, Proposition 11). 一方、$M$ には型 $\Delta'$ の目盛りが与えられ、すべての $\alpha \in \Delta$ に対して $M_{\alpha, 1} = M_{\alpha}$ が、$\alpha \in \Delta$ と $n \neq 1$ に対して $M_{\alpha, n} = \{0\}$ が与えられます。 $\varepsilon'$ を $\Delta'$ よりも交換因子とします。*

(i) E を型 $\Delta'$ の段階的 (左および右) $\mathbf{T}(M)$ バイモジュールとする。すべての $\delta \in \Delta$ とすべての整数 $n \in \mathbf{Z}$、次数 $\delta_1' = (\delta, n)$ のすべての等級付けされた K-線型写像 $f : M \to E$ は、次数 $\delta'$ の $\varepsilon'$ 派生 $d : \mathbf{T}(M) \to E$ に一意に拡張できます。

(ii) E を型 $\Delta'$ の段階的 $S(M)$ モジュールとする。 次数 $\delta'$ の段階化された K-線型写像 $f : M \to E$ が次数 $\delta'$ の $\varepsilon'$-導出 $d : S(M) \to E$ に拡張可能であるためには、均質な順序付けられたすべての対 $(x, y)$ が必要かつ十分です。 Mの元、

$$
x . f(y) + \varepsilon_{\delta', (\deg(y), 1)} y . f(x) = y . f(x) + \varepsilon_{\delta', (\deg(x), 1)} x . f(y).
$$

$\varepsilon'$-導出 d は一意になります。

(iii) E を型 $\Delta'$ の段階的 (左および右) $\Lambda(M)$ バイモジュールとする。 次数 $\delta'$ の段階的な K-線型写像 $f : M \to E$ を $\varepsilon'$ 派生に拡張できるようにする

$$
d : \Lambda(M) \to E
$$

次数 $\delta'$ の場合、M のすべての同次元 x に対して、次のことが必要かつ十分です。

$$
x . f(x) + \varepsilon_{\delta', (\deg(x), 1)} f(x) . x = 0.
$$

$\varepsilon'$-導出 d は一意になります。

Remark 2 of no. 2 is applied with one of the external B-module laws on E (with B equal to $\mathbf{T}(M)$, $S(M)$ or $\Lambda(M)$) modified; the external law thus modified is still, by (1) (no. 1), a B-module law and the B-module law thus obtained on E is still compatible with the other B-module structure. その場合、$A = K$ と $d_0 = 0$ を使用すると、命題を適用する 14 で十分です。

例 (1)。 命題 14 の適用では、$d_0 = 0$ 条件 (29) が単に $d_1$ が A 線形であることを意味することに注意してください。特に $E = B$ と、B 上の環構造から導出された (B, B) バイモジュール構造を考慮すると、$d_1$ が M の自己準同型の合成と標準単射 $M \to B$ であるとみなされるとき、条件 (30) と (31) は自動的に満たされます。 (30) については、$S(M)$ が可換であるため、これは明らかであり、(31) については、x と $s(x)$ が $\Lambda(M)$ の次数 1 であるという事実からわかります。したがって、M のすべての自己準同型 s は、次数 0 である $\mathbf{T}(M)$ (それぞれ $S(M)$、それぞれ $\Lambda(M)$) の導分 $D_s$ に一意に拡張できることがわかります。さらに、2 つの自己準同型 s、M の t については、

$$
[D_s, D_t] = D_{[s, t]}
$$

両辺は $\mathbf{T}(M)$ の導分 (それぞれ $S(M)$、それぞれ $\Lambda(M)$) であり、M の $[s, t]$ に等しい。

$D_s$ の式は、no. 5 の公式 (21) を使用して得られます。これにより、それぞれ、$M$ の $x_1, x_2, \ldots, x_n$ に対して、

$$
\begin{cases}
D_s(x_1 \otimes x_2 \otimes \cdots \otimes x_n) \\
\phantom{D_s(x_1 \otimes x_2 \otimes \cdots \otimes x_n)} = \sum_{i=1}^n x_1 \otimes \cdots \otimes x_{i-1} \otimes s(x_i) \otimes x_{i+1} \otimes \cdots \otimes x_n \\
D_s(x_1 x_2 \ldots x_n) = \sum_{i=1}^n x_1 \ldots x_{i-1} s(x_i) x_{i+1} \ldots x_n \\
D_s(x_1 \wedge x_2 \wedge \cdots \wedge x_n) \\
\phantom{D_s(x_1 \wedge x_2 \wedge \cdots \wedge x_n)} = \sum_{i=1}^n x_1 \wedge \cdots \wedge x_{i-1} \wedge s(x_i) \wedge x_{i+1} \wedge \cdots \wedge x_n.
\end{cases}
$$

代数 $\Lambda(M)$ の場合、$D_s$ は次のように解釈されます。

#### 命題 15 {#alg-iii-s10-prop-15 .statement tag=0670}

*$M$ が有限階数 $n$ の空き $K$ モジュールである場合、$M$ の $s$ ごとの自己準同型に対して、導分 $D_s$ の制限 ～ $\Lambda^n(M)$ ホモテティー は比率 $\operatorname{Tr}(s)$ です。*

$(e_j)_{1 \leq j \leq n}$を$M$の基底とし、$e = e_1 \wedge e_2 \wedge \cdots \wedge e_n$と書きます。もし
$$
s(e_j) = \sum_{k=1}^n \alpha_{jk} e_k,
$$
(36) の 3 番目の公式は次のようになります。
$$
D_s(e) = \sum_{i=1}^n e_1 \wedge \cdots \wedge e_{i-1} \wedge s(e_i) \wedge e_{i+1} \wedge \cdots \wedge e_n = \left( \sum_{j=1}^n \alpha_{jj} \right) e.
$$

*例 (2).* 系から命題 14、部分 (iii) では、$\Delta = \{0\}$ とし、$\Lambda(M)$ の卒業は通常の型 $\mathbf{Z}$ の卒業となります。一方、$\varepsilon(p, q) = (-1)^{pq}$ を取ります。次に、$M$ 上のすべての線型形式 $x^* \in M^*$ について、$x \mapsto \langle x, x^* \rangle$ は、$M$ の次数 $-1$ を $\Lambda(M)$ 満たす関係に段階的にマッピングした$K$ 線形マッピングです。 (34);その場合、$\Lambda(M)$、次数 $-1$ の *反派生* $i(x^*)$ が存在し、そのようなものになります (no. 5 の公式 (21) により)
$$
i(x^*)(x_1 \wedge \cdots \wedge x_n)
= \sum_{i=1}^n (-1)^{i-1} \langle x_i, x^* \rangle x_1 \wedge \cdots \wedge x_{i-1} \wedge x_{i+1} \wedge \cdots \wedge x_n
$$
これは、§ 11, no. 9、公式 (68) で定義される内部積の特殊なケースです。

#### 命題 16 {#alg-iii-s10-prop-16 .statement tag=0671}

*Let $A$ be a commutative $K$-algebra, $M_i$ ($1 \leq i \leq n$) and $P$ $A$-modules and $H$ the $A$-module of $A$-multilinear mappings of $M_1 \times M_2 \times \cdots \times M_n$* into P. Suppose that there is given a K-derivation $d_0 : A \to A$ of the algebra A, for each i, a K-linear mapping $d_i : M_i \to M_i$ and a K-linear mapping $D : P \to P$, so that, for $1 \leq i \leq n$, $(d_0, d_i, d_i)$ is a K-derivation of $(A, M_i, M_i)$ into itself and $(d_0, D, D)$ is a K-derivation of $(A, P, P)$ into itself. 次に、$(d_0, D', D')$ がそれ自体への $(A, H, H)$ の K 微分であるような K-線型写像 $D' : H \to H$ が存在し、

(37) $D(f(x_1, \ldots, x_n))$

$$
= (D'f)(x_1, \ldots, x_n) + \sum_{i=1}^n f(x_1, \ldots, x_{i-1}, d_ix_i, x_{i+1}, \ldots, x_n)
$$

$1 \leq i \leq n$ と $f \in H$ のすべての $x_i \in M_i$。

$f \in H$ について、(37) で定義された P への $M_1 \times M_2 \times \cdots \times M_n$ の写像 $D'f$ が A 多重線形であることを示します。 $a \in A$の場合、

$$
(D'f)(ax_1, x_2, \ldots, x_n) = D(af(x_1, \ldots, x_n)) - f(d_1(ax_1), x_2, \ldots, x_n)
$$
$$
-a \sum_{i=2}^n f(x_1, \ldots, x_{i-1}, d_ix_i, x_{i+1}, \ldots, x_n)
$$

そして仮定までに

$$
D(af(x_1, \ldots, x_n)) = (d_0a)f(x_1, \ldots, x_n) + aD(f(x_1, \ldots, x_n))
$$

と $d_1(ax_1) = (d_0a)x_1 + a.d_1x_1$ は次のようになります。

$$
(D'f)(ax_1, x_2, \ldots, x_n) = a.(D'f)(x_1, \ldots, x_n)
$$

それぞれの $x_i$ の線形性も同様に証明されます。一方で、

$$
(D'(af))(x_1, \ldots, x_n) = D(af(x_1, \ldots, x_n))
$$
$$
- \sum_{i=1}^n af(x_1, \ldots, x_{i-1}, d_ix_i, x_{i+1}, \ldots, x_n)
$$
$$
= (d_0a)f(x_1, \ldots, x_n)) + aD(f(x_1, \ldots, x_n))
$$
$$
- \sum_{i=1}^n af(x_1, \ldots, x_{i-1}, d_ix_i, x_{i+1}, \ldots, x_n)
$$
$$
= (d_0a)f(x_1, \ldots, x_n) + a(D'f)(x_1, \ldots, x_n)
$$

その他語

$$
D'(af) = (d_0a)f + a(D'f)
$$

これにより命題が確立されます。

#### 例 {#alg-iii-s10-n9-exa-1 .statement tag=0672}

(3) 適用命題 16 を $n = 1$、$M_1 = M$、$P = A$、次に M の双対である $H = M^*$ に適用すると、$(A, M, M)$ の K 導出$(d_0, d, d')$ に対して、次の K 導出$(d_0, d^*, d^*)$ が導出されることがわかります。 $(A, M^*, M^*)$そのような

(38) $d_0\langle m, m^*\rangle = \langle dm, m^*\rangle + \langle m, d^*m^*\rangle$

$m \in M$ と $m^* \in M^*$ の場合。 $M \oplus M^*$ の K-線型写像は、$M$ の $d$ と $M^*$ の $d^*$ に等しく、条件 (29) を満たすので、$A$-代数の $K$ 導出$D$ が存在します。 $T(M \oplus M^*)$、$A$の簡約するから$d_0$、$M$の$d$、$M^*$の$d^*$です。 $D$ の制限 $d_J^I$ から $T(M \oplus M^*)$ ($§ 5$, no. 6) のサブ$A$ 加群 $T_J^I(M)$ への$T_J^I(M)$ の $K$ 準同型写像は次のとおりです。 $(d_0, d_J^I, d_J^I)$ は、$(A, T_J^I(M), T_J^I(M))$ の $K$ 派生です。さらに、$i \in I, j \in J$ について、$I' = I - \{i\}, J' = J - \{j\}$ と書くと、縮約 $c_j^i$ ($§ 5$, no. 6) についてはすぐに検証されます。

$$
c_j^i(d_J^I(z)) = d_{J'}^{I'}(c_j^i(z)) \quad \text{for all } z \in T_J^I(M).
$$

(4) $M_i$ ($1 \leq i \leq 3$) を 3 つの $A$ モジュールとし、それぞれの $i$ について、$(d_0, d_i, d_i)$ が $(A, M_i, M_i)$ の導分であると仮定します。 適用命題 $(A, H_{ij}, H_{ij})$ の $n = 1$、導分 $(d_0, d_{ij}, d_{ij})$ に対しては 16 が再度適用されます。ここで、$H_{ij} = \operatorname{Hom}_A(M_i, M_j)$ は、順序付けられた対 $(i, j)$ ごとに導出されます。この記法では、$u \in \operatorname{Hom}_A(M_1, M_2)$と$v \in \operatorname{Hom}_A(M_2, M_3)$は、

$$
d_{13}(v \circ u) = (d_{23}v) \circ u + v \circ (d_{12}u)
$$
定義からすぐに確認できるように。

### 10. 導分用ユニバーサル問題;非可換の場合

残りの $§ 10$ を通じて、すべての代数は結合的かつ単体であると想定され、すべての代数準同型は単体であると想定されます。

$A$ を $K$ 代数としましょう。 テンソル積 $A \otimes_K A$ は標準的に $(A, A)$ バイモジュール構造を持ち、その下に

$$
x . (u \otimes v) . y = (xu) \otimes (vy)
$$
$A$ のすべての $x, y, u, v$ ($§ 4$、no. 3、例 2)。 $A$ の $m : A \otimes_K A \to A$ 対応するから乗法への $K$ 線形マッピング (したがって $m(x \otimes y) = xy$ など) は、$(A, A)$ バイモジュール準同型です。したがって、核 $I$ は $A \otimes_K A$ の部分両側加群です。

#### 補題 1 {#alg-iii-s10-lem-1 .statement tag=0673}

*写像 $\delta_A : x \mapsto x \otimes 1 - 1 \otimes x$ は $A$ から $I$ への $K$ 導出であり、$\delta_A$ の像によって、左の $A$ 加群として $I$ が生成されます。

最初の主張は、次の事実から導き出されます。

$$
(xy) \otimes 1 - 1 \otimes (xy) = (x \otimes 1 - 1 \otimes x) . y + x . (y \otimes 1 - 1 \otimes y)
$$
(40)による。一方、元 $\sum_i x_i \otimes y_i$ ($A$ の $x_i, y_i$ の場合) 属するから $I$ の場合、定義 $\sum_i x_i y_i = 0$ により、したがって

$$
\sum_i (x_i \otimes y_i) = \sum_i x_i (1 \otimes y_i - y_i \otimes 1)
$$
(40) により、補題の証明が完了します。

#### 命題 17 {#alg-iii-s10-prop-17 .statement tag=0674}

*導分* $\delta_A$ *次の普遍性* があります: すべての $(A, A)$-bimodule $E$ およびすべての $K$-導出 $d : A \to E$ に対して、次のような 1 つだけの $(A, A)$-bimodule 準同型 $f : I \to E$ が存在します。 $d = f \circ \delta_A$。

注意まず​​、すべての $(A, A)$-bimodule 準同型 $f : I \to E$ について、$f \circ \delta_A$ は導分 (no. 7, 命題 9) です。逆に、$d : A \to E$ を K 導出とします。次に、$d = f \circ \delta_A$、$f$ が、$\delta_A$ の定義に対する条件によって *一意に決定される * ような $(A, A)$ バイモジュール準同型 $f : I \to E$ が存在する場合、次のことが証明されることを最初に証明します。

$$
f(x \otimes 1 - 1 \otimes x) = dx
$$

そして私たちの主張は、$\delta_A$ の像がすでに生成する I として左A-加群 (補題 1) であるという事実から導き出されます。

$$
f\left( \sum_i x_i \otimes y_i \right) = \sum_i x_i \cdot f(1 \otimes y_i - y_i \otimes 1) = -\sum_i x_i \cdot dy_i.
$$

逆に、$A \times A$ から $E$ への写像 $(x, y) \mapsto -x \cdot dy$ は $K$ 双線形であるため、$g(x \otimes y) = -x \cdot dy$ となるような $K$ 線形写像 $g : A \otimes_K A \to E$ が 1 つだけ存在します。 $g$ から $I$ の制限 $f$ が左側と右A-加群構造に対して A 線形であることを検証するだけで十分です。最初の主張は $(xx') \cdot dy = x \cdot (x' \cdot dy)$ 以来明らかです。 2 番目を証明するには、$\sum_i x_i \otimes y_i \in I$ と $x \in A$ の場合、

$$
\sum_i x_i \cdot d(y_i x) = \sum_i x_i \cdot dy_i \cdot x + \sum_i (x_i y_i) \cdot dx
$$

しかし、$\sum_i x_i y_i = 0$ by $I$ の定義なので、これで証明が完了します。

したがって、*標準* $K$-モジュール *同型* $f \mapsto f \circ \delta_A$ を定義しました。

$$
\operatorname{Hom}_{(A, A)}(I, E) \to D_K(A, E)
$$

左側は、$A$ の $(A, A)$ バイモジュール準同型の $E$ への $K$ モジュールです。

### 11. 導分用ユニバーサル問題;可換格

ここで、$A$ が *可換* $K$-代数であり、$E$ が $A$-*加群* であると仮定します。 $E$ は、その 2 つの外部法則が指定された $A$ モジュール法則と同一である $(A, A)$ バイモジュールと考えることができます。一方、$A \otimes_K A$ の $(A, A)$ バイモジュール構造は、$A \otimes_K A$ の *可換環* 構造から生じる $(A \otimes_K A)$ モジュール構造と同一です。なぜなら、この場合、$A$ の $x, y, u, v$ については、

$$
x \cdot (u \otimes v) \cdot y = (xu) \otimes (vy) = (xu) \otimes (yv) = (x \otimes y)(u \otimes v).
$$

したがって、$m$ の核 $\mathfrak{J}$ は、この場合、環 $A \otimes_K A$ の *理想* であり、$m : A \otimes_K A \to A$ が全射であるため、$(A \otimes_K A)/\mathfrak{J}$ は $A$ と同型です。また、$E$ が $m$ (他の語では $(A \otimes_K A)$ モジュール $m_*(E)$) によって $(A \otimes_K A)$ モジュールとみなされる場合、$(A, A)$-*両側加群* 準同型 $\mathfrak{J} \to E$ は次のように識別されます。 $(A \otimes_K A)$-*加群* 準同型 $\mathfrak{J} \to E$ (§ 4, no. 3)、他の語には正規の $K$ モジュール同型があります。

$$
\operatorname{Hom}_{(A, A)}(\mathfrak{J}, E) \to \operatorname{Hom}_{A \otimes_K A}(\mathfrak{J}, E).
$$

一方、$\mathfrak{J}E = \{0\}$ は、元 $1 \otimes x - x \otimes 1$ 生成する $\mathfrak{J}$ を $(A \otimes_K A)$ モジュールとして (no. 10、補題 1)、すべての $z \in E$ に対して、

$$
(1 \otimes x - x \otimes 1)z = 0
$$

$E$ の $(A \otimes_K A)$ モジュール構造の定義により。 $\mathfrak{J}$ は $(A \otimes_K A)$ モジュール $E$ の消滅子に含まれており、$E$ の $((A \otimes_K A)/\mathfrak{J})$ モジュール構造は定義によって、$E$ で与えられた最初の $A$ モジュール構造にすぎないため、 標準同型中

$$
\mathfrak{J} \otimes_K ((A \otimes_K A)/\mathfrak{J})
$$

$\mathfrak{J}/\mathfrak{J}^2$ (§ 4, no. 1、系 1 ～ 命題 1)、標準的 $K$ モジュール同型に

$$
\operatorname{Hom}_{A \otimes_K A}(\mathfrak{J}, E) \to \operatorname{Hom}_A(\mathfrak{J}/\mathfrak{J}^2, E).
$$

no. 10 の命題 17 を考慮すると、次の命題が証明されたことがわかります。

#### 命題 18 {#alg-iii-s10-prop-18 .statement tag=0675}

*$A$ を可換 $K$-代数、$\mathfrak{J}$ を全射法標準準同型 $m : A \otimes_K A \to A$ のイデアル核とすると、$A$ は $(A \otimes_K A)/\mathfrak{J}$ と同型であり、$\mathfrak{J}/\mathfrak{J}^2$ は標準的に$A$モジュール構造。 $d_{A/K} : A \to I/I^2$ を、$x \otimes 1 - 1 \otimes x$ モジュロ $\mathfrak{J}^2$ のすべての $x \in A$ 類に関連する $K$ 線形マッピングとします。 写像 $d_{A/K}$ は $K$ 導出であり、すべての $A$ モジュール $E$ とすべての $K$ 導出 $D : A \to E$ に対して、次のような $A$ 線形写像 $g : \mathfrak{J}/\mathfrak{J}^2 \to E$ が 1 つだけ存在します。 $D = g \circ d_{A/K}$.*

#### 例 {#alg-iii-s10-n11-exa-1 .statement tag=0676}

M を K-加群とします。 no. 9 の命題 14 から、すべての S(M) モジュール E について、写像 D ↦ D | が得られます。 M 定義する Hom_K(M, E) 上の D_K(S(M), E) の S(M) モジュール同型;一方、E は S(M) モジュールであるため、Hom_K(M, E) は正規同型です。

$$
\operatorname{Hom}_{S(M)}(M \otimes_K S(M), E),
$$

M から E へのすべての K 準同型性は形 $x \mapsto h(x \otimes 1)$ で一意に表現可能です。

$$
h \in \operatorname{Hom}_{S(M)}(M \otimes_K S(M), E)
$$

(II, § 5, no. 1)。 D_0 を、M に対する制限が標準準同型 $x \mapsto x \otimes 1$ である K 導出$S(M) \to M \otimes_K S(M)$ とします。したがって、すべての K 導出 D : S(M) → E は、次のように $h \circ D_0$ として一意に書くことができます。

$$
h \in \operatorname{Hom}_{S(M)}(M \otimes_K S(M), E).
$$

ユニバーサル写像問題の解の一意性により、固有の S(M) モジュール同型が存在することがわかります。

$$
\omega : M \otimes_K S(M) \to \Omega_K(S(M))
$$

$D_0 \circ \omega = d_{S(M)/K}$;他の語、すべての$x \in M$、$\omega(x \otimes 1) = dx$。

特に、*M が基底* $(e_\lambda)_{\lambda \in L}$ を持つ自由K-加群の場合、$\Omega_K(S(M))$ * は差動の基底集合* $de_\lambda$ を持つフリー S(M) モジュールです。特に、S(M) が多項式代数 $K[X_1, \ldots, X_n]$ (§ 6, no. 6) で識別される $L = \{1, n\}$ の場合を考えてみましょう。すべての多項式 $P \in K[X_1, \ldots, X_n]$ について、一意に書くことができます

$$
dP = \sum_{i=1}^n D_i P . dX_i
$$

$D_i P \in K[X_1, \ldots, X_n]$ と、上記のおかげで、写像 $P \mapsto D_i P$ は、基底 $(dX_i)$ に対する $\Omega_K(S(M))$ 上の座標形への $K[X_1, \ldots, X_n]$ 対応するの *K 導出* です。また、$D_i P$ の代わりに $\frac{\partial P}{\partial X_i}$ とも書きます。これは、$X_i$ に関する P の *偏導関数* と呼ばれます。

### 12. K微分の機能的特性

#### 命題 19 {#alg-iii-s10-prop-19 .statement tag=0677}

*しましょう*

$$
\begin{array}{ccc}
K & \xrightarrow{\rho} & K' \\
\downarrow \eta & & \downarrow \eta' \\
A & \xrightarrow{u} & A'
\end{array}
$$

*可換図式の可換環準同型*、$\eta$ (それぞれ $\eta'$) *作成*

A (それぞれ $A'$) を $K$-代数 (それぞれ $K'$-代数) に変換します。可換図式をレンダリングする $A$ 線形マッピング $v : \Omega_K(A) \to \Omega_{K'}(A')$ が 1 つだけ存在します。

$$
\begin{array}{ccc}
A & \xrightarrow{u} & A' \\
d_{A/K} \downarrow & & d_{A'/K'} \downarrow \\
\Omega_K(A) & \xrightarrow{v} & \Omega_{K'}(A')
\end{array}
$$

$d_{A'/K'} \circ u$ は、$A$ モジュール $\Omega_{K'}(A')$ の値を使用した $A$ の $K$ 導出です。 $v$の存在と一意性は、no. 11の命題18から続きます。

命題 19 の写像 $v$ は $\Omega(u)$ で表されます。 可換環準同型の可換図式がある場合

$$
\begin{array}{cccccc}
K & \xrightarrow{\sigma} & K' & \xrightarrow{\sigma'} & K'' \\
\eta \downarrow & & \eta' \downarrow & & \eta'' \downarrow \\
A & \xrightarrow{u} & A' & \xrightarrow{u'} & A''
\end{array}
$$

命題 19 の一意性性質からすぐに続きます。

$$
\Omega(u' \circ u) = \Omega(u') \circ \Omega(u).
$$

$\Omega_{K'}(A')$ は $A'$ モジュールであるため、$\Omega(u)$ から正規に $A'$ 線形マッピングを導出します。

$$(41)$$
$$
\Omega_0(u) : \Omega_K(A) \otimes_A A' \to \Omega_{K'}(A')
$$

$\Omega(u)$ は $\Omega_0(u)$ と標準準同型 $i_A : \Omega_K(A) \to \Omega_K(A) \otimes_A A'$ の合成です。すべての $A'$ モジュール $E'$ には、可換図式があります。

$$
\begin{array}{ccc}
\operatorname{Hom}_{A'}(\Omega_{K'}(A'), E') & \xrightarrow{\operatorname{Hom}(\Omega_0(u), 1_{E'})} & \operatorname{Hom}_{A'}(\Omega_K(A) \otimes_A A', E') \\
\phi_{A'} \downarrow & & \phi_A \circ r_A \downarrow \\
D_{K'}(A', E') & \xrightarrow{C(u)} & D_K(A, E)
\end{array}
$$

ここで、$C(u)$ は写像 $D \mapsto D \circ u$ (no. 7、命題 9)、$r_A$ は標準同型

$$
\operatorname{Hom}(i_A, 1_{E'}) : \operatorname{Hom}_{A'}(\Omega_K(A) \otimes_A A', E') \to \operatorname{Hom}_A(\Omega_K(A), E');
$$

これは、同型 $\phi_A$ と $\phi_{A'}$ の命題 19 と定義の直後に続きます。

#### 命題 20 {#alg-iii-s10-prop-20 .statement tag=0678}

*$A' = A \otimes_K K'$、$\eta': K' \to A'$と$u: A \to A'$標準準同型があるとします。次に、$A'$-線形マッピング*

$$
\Omega_0(u): \Omega_K(A) \otimes_A A' \to \Omega_{K'}(A')
$$

*は同型です*

図式 (42) では垂直矢印が全単射であるという事実により、簡約するから証明では、図式 (42) のすべての $A'$ モジュール $E'$, 準同型 $C(u): D \mapsto D \circ u$ が全単射 (II, § 2, no. 1, 定理 1）。ここで、$\mathrm{Hom}(u, 1_{E'}): \mathrm{Hom}_{K'}(A \otimes_K K', E') \to \mathrm{Hom}_K(A, E')$ は同型 (II, § 5, no. 1, 命題 1) であり、$C(u)$ はその制限から $D_{K'}(A', E')$ であるため単射です。さらに、$f: A' \to E'$ が次のような$K'$ 線形写像である場合、

$$
f \circ u: A \to E'
$$

は $K$ 導出であり、$f$ が $K'$ 線形であるという事実と、$A$ の $x, y$ に対する $f((x \otimes 1)(y \otimes 1)) = (y \otimes 1)f(x \otimes 1) + (x \otimes 1)f(y \otimes 1)$、$f$ が $K'$-*導分*、元であるという事実からすぐに続きます。 $K'$モジュール$A'$の生成する系を形成する$x \in A$の$x \otimes 1$。これで、$C(u)$ が全単射であることが証明で完了します。

ここからは、$\rho: K \to K'$ が $K$ の *恒等写像* である場合に注目します。したがって、すべての $K$-代数準同型性 $u: A \to B$ は $B$-線形写像に写像されます。

$$
\Omega_0(u): \Omega_K(A) \otimes_K B \to \Omega_K(B).
$$

一方、$B$ は $u$ による $A$-代数であるため、$A$-*微分* $\Omega_A(B)$ の $B$ 加群を考えることができます。正規の導分 $d_{B/A}: B \to \Omega_A(B)$ は *なおさら* $K$ 導出であるため、一意に因数分解されます。

$$
B \xrightarrow{d_{B/K}} \Omega_K(B) \xrightarrow{\Omega_u} \Omega_A(B)
$$

ここで、$\Omega_u$ は $B$ 線形マッピング (no. 11、命題 18) です。すべての $B$ モジュール $E$ には、可換図式があります。

$$
\begin{array}{ccc}
\mathrm{Hom}_B(\Omega_A(B), E) & \xrightarrow{\mathrm{Hom}(\Omega_u, 1_E)} & \mathrm{Hom}_B(\Omega_K(B), E) \\
\downarrow \phi_{A,B} & & \downarrow \phi_{K,B} \\
D_A(B, E) & \xrightarrow{j_u} & D_K(B, E)
\end{array}
$$

ここで、$j_u$ は標準単射 (no. 7) です。これは、no. 11 の命題 18 の直後に続きます。

#### 命題 21 {#alg-iii-s10-prop-21 .statement tag=0679}

*$B$ 線形マッピングのうち数列*

$$
\Omega_K(A) \otimes_A B \xrightarrow{\Omega_0(u)} \Omega_K(B) \xrightarrow{\Omega_u} \Omega_A(B) \to 0
$$

*正確です。*

簡約するは、B-加群 E ごとに、数列であることを確認します。

$$
0 \to \operatorname{Hom}_B(\Omega_A(B), E) \xrightarrow{\operatorname{Hom}(\Omega_u, 1_E)} \operatorname{Hom}_B(\Omega_K(B), E) \xrightarrow{\operatorname{Hom}(\Omega_0(u), 1_E)} \operatorname{Hom}_B(\Omega_K(A) \otimes_A B, E)
$$

正確です (II, § 2, no. 1, 定理 1)。しかし、可換式図式 (42) と (44) では垂直矢印が同型であるという事実により、数列を示すだけで十分です。

$$
0 \longrightarrow D_A(B, E) \xrightarrow{j_u} D_K(B, E) \xrightarrow{C(u)} D_K(A, E)
$$

は正確です。これは、no. 7 の命題 11 にすぎません。

ここで、K-代数準同型 $u : A \to B$ が全射である場合を考えます。 $\mathfrak{J}$ がその核である場合、B は $A/\mathfrak{J}$ と同型です。正準導分 $d = d_{A/K}$ と合成 A-線型写像の制限 $d|_{\mathfrak{J}} : \mathfrak{J} \to \Omega_K(A)$ を考慮します。

$$
d' : \mathfrak{J} \xrightarrow{d|_{\mathfrak{J}}} \Omega_K(A) \xrightarrow{i_A} \Omega_K(A) \otimes_A B.
$$

次に、$d'(\mathfrak{J}^2) = 0$、以降、$\mathfrak{J}$の$x, y$については、

$$
d'(xy) = d(xy) \otimes 1 = (x.dy + y.dx) \otimes 1 = dy \otimes u(x) + dx \otimes u(y) = 0
$$

$u(x) = u(y) = 0$から。したがって、$d'$ から移行によって商、A-線型写像が導出されます。

$$
\bar{d} : \mathfrak{J}/\mathfrak{J}^2 \to \Omega_K(A) \otimes_A B
$$

そして、$\mathfrak{J}$ が A-加群 $\mathfrak{J}/\mathfrak{J}^2$ を全滅させると、$\bar{d}$ は B-線型写像になります。

#### 命題 22 {#alg-iii-s10-prop-22 .statement tag=067A}

※可換K-代数 A、$B = A/\mathfrak{J}$、$u : A \to B$ 標準準同型の理想を$\mathfrak{J}$ とします。 数列/B-線型写像*

$$
\mathfrak{J}/\mathfrak{J}^2 \xrightarrow{\bar{d}} \Omega_K(A) \otimes_A B \xrightarrow{\Omega_0(u)} \Omega_K(B) \to 0
$$

* は正確です。*

$\Omega_K(A) \otimes_A B$ は $\Omega_K(A)/\mathfrak{J}\Omega_K(A)$ と同一視されており、この商加群では $\bar{d}$ の像が $d(\mathfrak{J})$ の像であることに注意してください。したがって、$\operatorname{Im}(\bar{d})$ による $\Omega_K(A) \otimes_A B$ の商は、商 $\Omega_K(A)/N$ で識別されます。ここで、N は、$\mathfrak{J}\Omega_K(A)$ と $d(\mathfrak{J})$ によって生成されたサブ A モジュールです。さらに、複合写像

$$
A \xrightarrow{d_{A/K}} \Omega_K(A) \longrightarrow \Omega_K(A)/N
$$

は K 微分 (no. 7, 命題 9) であり、N の定義による $\mathfrak{J}$ の零であるため、移行から商のとき、定義するは K 微分です。 $D_0 : B \to \Omega_K(A)/N$。

普遍的な写像問題の解の一意性を考慮すると、簡約するから証明まで、すべての B-加群 E およびすべての K 導出 D: B → E に対して、固有の B-線型写像 g が存在します。 Ω_K(A)/N → E であり、D = g ∘ D_0 となります。しかし、合成写像 D ∘ u: A → E は K 微分 (no. 7, 命題 9) であるため、f ∘ d_{A/K} = D ∘ u となる A-線型写像 f: Ω_K(A) → E が 1 つだけ存在します。この関係は、f が d(Σ) 上で零であることをすでに示しています。 E が B-加群であるため、ΣE = {0} と同様に、ΣΩ_K(A) では f は零です。したがって、f は N で零、定義する、移行から商、B-線型写像のとき、 g: Ω_K(A)/N → E となり、g ∘ D_0 = D となります。 g の一意性は f の一意性から続きます。

u: A → B が単射準同型であっても、Ω_0(u): Ω_K(A) ⊗_A B → Ω_K(B) が単射法 (練習問題 5) であると考えてはなりません。ただし、次の命題があります。

#### 命題 23 {#alg-iii-s10-prop-23 .statement tag=067B}

A を整数 K-代数、B を分数の体、u: A → B 標準単射とします。すると、Ω_0(u): Ω_K(A) ⊗_A B → Ω_K(B) は同型となります。

図式 (42) で垂直矢印が全単射であるという事実を使用すると、簡約するから証明は、B 上のすべてのベクトル空間 E について、写像 C(u): D_K(B, E) → D_K(A, E) が全単射になります。しかし、これは、A から E へのすべての K 導出は、B から E への K 導出に一意に拡張できるという事実から帰結します (no. 5, 命題 5)。

### 練習問題 {#alg-iii-s10-exercises}

[§ 10 に対して練習問題](exercises/s10/)を参照してください。
