---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 3
section_title: Actions
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 24-29, 129-132
pdf_pages: 0048-0053, 0153-0156
extraction: ocr
subsections:
    - "no": 1
      title: ACTIONS
      page: 24
      pdf_page: 48
    - "no": 2
      title: SUBSETS STABLE UNDER AN ACTION. INDUCED ACTION
      page: 26
      pdf_page: 50
    - "no": 3
      title: QUOTIENT ACTION
      page: 26
      pdf_page: 50
    - "no": 4
      title: DISTRIBUTIVITY
      page: 27
      pdf_page: 51
    - "no": 5
      title: DISTRIBUTIVITY OF ONE INTERNAL LAW WITH RESPECT TO ANOTHER
      page: 29
      pdf_page: 53
statements: 14
exercises: 10
content_sha256: e4026aed21f2f3485e2caa2ba6e1659256d5233c04cd4a791fad77ffa92d23cd
translated_from: content/en/alg/I/03_s3_actions.md
translation_method: google
source_content_sha256: 7e8fbe4c81b4a012c8fdf0810f23488766fe66b340393425e3d9b307319fe67d
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: a6c35c7949eb5882e0a095cf8d204ce8c03ac76bad1c3e90fed115a7cfd75d59
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 3。 作用

### 1. 作用

#### 定義 1 {#alg-i-s3-def-1 .statement tag=057T}

※$\Omega$とEを2つの集合とします。 E の写像の集合 $E^E$ への $\Omega$ の写像は、E では $\Omega$ の作用と呼ばれます。

$\alpha \mapsto f_\alpha$ を E の $\Omega$ の作用とします。 写像 $(\alpha, x) \mapsto f_\alpha(x)$ (それぞれ $(x, \alpha) \mapsto f_\alpha(x)$) は、左* (それぞれ *右*) の *法則と呼ばれます。 *E* 上の $\Omega$ の *作用 *E* 上の $\Omega$ の指定された作用に関連付けられています。 $\Omega \times E$ (それぞれ$E \times \Omega$) の写像 $g$ が E に与えられると、E には $\Omega$ の作用 $\alpha \mapsto f_\alpha$ が 1 つだけ存在し、関連する左 (または右) 作用の法則は $g$ になります。 (*集合理論*、II, § 5, no. 2、命題 3)。

この章では、略して「法則 of 作用」と言うことにします。

† または、E のときどき合成* の *外部法則で、$\Omega$ が集合として動作します。

「左作用の法則」の代わりに。 E の元 $f_\alpha(x)$ ($\alpha \in \Omega$ と $x \in E$ の場合) は、ときどきは、$\alpha$ の下の $x$ の *変換*、または $\alpha$ と $x$ の *合成* と呼ばれます。多くの場合、左 (または右) 乗法記法 $\alpha . x$ (または $x . \alpha$) で表され、ドットは省略される場合があります。 $\alpha$ と $x$ の合成は、$\alpha$ と $x$ (それぞれ $x$ と $\alpha$) の *積* と呼ばれます。指数関数記法 $x^\alpha$ も使用されます。以下の段落の議論では、一般に記法 $\alpha \perp x$ を使用します。 $\Omega$ の元は、*演算子* と呼ばれることがよくあります。

#### 例 {#alg-i-s3-n1-exa-1 .statement tag=057U}

(1) E を乗算的に書かれた結合マグマとする。 E の厳密に正の整数 $n$ 写像 $x \mapsto x^n$ と関連する写像は、E 上の $\mathbf{N}^*$ の作用です。E が群の場合、有理数整数 $a$ と関連する写像 E の E への写像 $x \mapsto x^a$ は、E の $\mathbf{Z}$ の作用です。

(2) E を法則を持つマグマとし、$\top$ で表す。 E の $x \in E$ 写像 $A \mapsto x \top A$ の集合の部分集合をそれ自体に関連付けた写像は、$\mathscr{P}(E)$ 上の E の作用です。

(3) E を集合とします。 $E^E$ の恒等写像は、E の $E^E$ の作用であり、*標準作用* と呼ばれます。 作用の対応する法則は、$E^E \times E$ の写像 $(f, x) \mapsto f(x)$ を E に変換します。

(4) $(\Omega_i)_{i \in I}$ を集合の家族とします。 すべての $i \in I$ について、$f_i : \Omega_i \to E^E$ を E の $\Omega_i$ の作用とします。 $\Omega$ を $\Omega_i$ の和とします (*集合理論*, II, § 4, no. 8)。 $\Omega$ の $E^E$ へのマッピング $f$ は、$f_i$ を拡張し、E での $\Omega$ のアクションです。 これにより、作用の家族の研究を 1 人の作用の研究に簡約するすることができます。

(5) $\perp$ で示される法則を持つ E に対する $\Omega$ のアクション、$\Omega$ の部分集合 $\Xi$ および E の部分集合 X が与えられると、$\Xi \perp X$ は $\alpha \in \Xi$ および $x \in X$ と$\alpha \perp x$ の集合を表します。 $\Xi$ が 1 つの要素 $\alpha$ で構成される場合、通常は $\{\alpha\} \perp X$ の代わりに $\alpha \perp X$ と書きます。 $\alpha \in \Omega$ 写像 $X \mapsto \alpha \perp X$ に関連する写像は、$\mathscr{P}(E)$ 上の $\Omega$ の作用であり、これは、与えられた作用から拡大から部分集合の集合によって *派生* されると言われています。

(6) $\alpha \mapsto f_\alpha$ を E の $\Omega$ の作用とする。 g を $\Omega$ の $\Omega'$ の写像とする。すると、写像 $\beta \mapsto f_{g(\beta)}$ は E の $\Omega'$ の作用になります。

(7) $f : E \times E \to E$ を集合 E 上の合成の法則とします。 $x$ による元 $x \in E$ の左 (または右) 変換に関連する写像 $\gamma : x \mapsto \gamma_x$ (それぞれ $\delta : x \mapsto \delta_x$) (§ 2, no. 2) は、それ自体上の E の作用です。それは、与えられた法則から *派生* した、E の *左* (それぞれ *右*) *作用* と呼ばれます。 $f$ が可換なとき、これら 2 つは作用一致するになります。

$\gamma$ に関連付けられている左 (または右) 作用の法則は $f$ (それぞれ $f$ の反対側の法則) です。 $\delta$ に関連付けられた右 (または左) 作用の法則は $f$ (それぞれ法則から $f$ の反対側) です。

$\Omega, E, F$ を E の $\Omega$ の集合、$\alpha \mapsto f_\alpha$ 作用、および F の $\Omega$ の $\alpha \mapsto g_\alpha$ 作用とします。E の $\Omega$-*射を F* に、または E の *写像を F に変換すると、 $\Omega$* の作用は、E の写像 $h$ を F にすると次のようになります。

$$
g_\alpha(h(x)) = h(f_\alpha(x))
$$

すべての $\alpha \in \Omega$ と $x \in E$ に対して。 2 つの $\Omega$ 射のうち合成は $\Omega$ 射です。

$\Omega, \Xi, E, F$ をセット、$\alpha \mapsto f_\alpha$ を $E$ の $\Omega$ のアクション、$\beta \mapsto g_\beta$ を $F$ の $\Xi$ のアクション、および $\phi$ を $\Omega$ から $\Omega'$ にマッピングするとします。 $E$ の $F$ への $\phi$ 射は、$E$ の $F$ への写像 $h$ です。
$$
g_{\phi(\alpha)}(h(x)) = h(f_\alpha(x))
$$
$\alpha \in \Omega$ と $x \in E$ のすべてに。

### 2. 部分集合は作用の下で安定しています。誘導作用

#### 定義 2 {#alg-i-s3-def-2 .statement tag=057V}

*集合 $E$ の部分集合 $A$ は、すべての $\alpha \in \Omega$ に対して $f_\alpha(A) \subset A$ の場合、$E$ の $\Omega$ の作用 $\alpha \mapsto f_\alpha$ で安定と呼ばれます。 元 $E$ の $x$ は、$f_\alpha(x) = x$ の場合、$\Omega$ の元 $\alpha$ の下では不変と呼ばれます。*

特定のアクションの下での $E$ の安定サブセットの集合は安定です。 したがって、$E$ の特定の部分集合 $X$ には、$E$ 含むの最小の安定した部分集合が存在します。それは $X$ によって *生成*されると言われています。 元 $(f_{\alpha_1} \circ f_{\alpha_2} \circ \cdots \circ f_{\alpha_n})(x)$ で構成され、$i$ はすべて $x \in X, n \geq 0, \alpha_i \in \Omega$ になります。

#### 注意 {#alg-i-s3-n2-rem-1 .statement tag=057W}

$E$ を法則を持つマグマとし、$\tau$ で表します。 $E$ のサブセット $A$ は、それ自体に対する $E$ の左のアクションの下では安定ですが、それ自体に対する $E$ の右のアクションの下では必ずしも安定するとは限りません。 $E$ のサブセット $A$ は、それ自体に対する $E$ の左 (右) アクションの下で安定ですが、$E$ の法則の下では安定ですが、その逆は一般に当てはまりません。 より正確には、$A$ は、$A \tau A \subset A$ の場合およびその場合に限り、$E$ の法則の下で安定しますが、$A$ は、$E \tau A \subset A$ (それぞれ $A \tau E \subset A$) の場合に限り、$E$ 上の左 (または右) 作用の下で安定します。

#### 例 {#alg-i-s3-n2-exa-1 .statement tag=057X}

マグマ$E$を乗法で集合$\mathbf{N}$とします。 集合 $\{1\}$ は、$\mathbf{N}$ の内部法則の下で安定していますが、$\{1\}$ によって生成された$\mathbf{N}$ 自体の作用の下で安定している部分集合は、$\mathbf{N}$ の全体です。

#### 定義 3 {#alg-i-s3-def-3 .statement tag=057Y}

*$\alpha \mapsto f_\alpha$を$E$の$\Omega$の作用、$A$を$E$の安定した部分集合とします。 $f_\alpha$から$A$の元$\alpha \in \Omega$制限（$A$の写像とみなされる）に関連する写像は、$A$の$\Omega$の作用です与えられた作用.* によって誘発されると言われています。

### 3. 商作用

#### 定義 4 {#alg-i-s3-def-4 .statement tag=057Z}

*$\alpha \mapsto f_\alpha$を集合$E$の集合$\Omega$の作用とします。 $E$ 上の同値関係 $R$ は、$E$ のすべての元 $x$ と $y$ について、$x \equiv y \pmod{R}$ とすべての $\alpha \in \Omega, f_\alpha(x) \equiv f_\alpha(y) \pmod{R}$ が一致する場合、指定された作用と互換性があると言われます。 移行によって商まで$f_\alpha$から派生した$E/R$の元$\alpha \in \Omega$写像と関連付けられた写像は、$E/R$上の$\Omega$の作用と呼ばれます。 $E$ の $\Omega$ の作用のうち商。*

$E$ をマグマ、$R$ 同値関係を $E$ とします。 $R$ は、左 (それぞれ *右*) と互換性がある場合、$E$ の法則と *左* (または *右*) *互換*であると言われます。

右) E の作用は、E の法則から派生します。R が E の法則と互換性があるためには、E の法則と左右に互換性があることが必要かつ十分です。

§ 1, no. 6の命題6、7、8の類似点である主張と証明は読者に任せます。

### 4. 分配性

#### 定義 5 {#alg-i-s3-def-5 .statement tag=0580}

$E_1, \ldots, E_n$とFを集合とし、$E_1 \times \cdots \times E_n$の写像をFにします。$i \in \{1, n\}$とします。 $E_i$ と F に構造のマグマが与えられたとします。部分写像の場合、u は添字変数 i に対して分配的であると言われます。

$$
x_i \mapsto u(a_1, \ldots, a_{i-1}, x_i, a_{i+1}, \ldots, a_n)
$$

$E_j$ と $j \neq i$ のすべての固定 $a_j$ に対して、$E_i$ の準同型が F になります。

$\top$ が $E_i$ と F 上の内部法則を表す場合、u の分配性は次の方程式で与えられます。

(1) $$
u(a_1, \ldots, a_{i-1}, x_i \top x'_i, a_{i+1}, a_n) \\
= u(a_1, \ldots, a_{i-1}, x_i, a_{i+1}, \ldots, a_n) \top u(a_1, \ldots, a_{i-1}, x'_i, a_{i+1}, \ldots, a_n)
$$

$i = 1, 2, \ldots, n, a_1 \in E_1, \ldots, a_{i-1} \in E_{i-1}, x_i \in E_i, x'_i \in E_i, a_{i+1} \in E_{i+1}, \ldots, a_n \in E_n$の場合。

#### 例 {#alg-i-s3-n4-exa-1 .statement tag=0581}

E を乗算的に書かれたモノイド (それぞれ群) とします。 E への $\mathbf{N} \times E$ (それぞれ $\mathbf{Z} \times E$) の写像 $(n, x) \mapsto x^n$ は、方程式 $x^{m+n} = x^m x^n$ (加法は $\mathbf{N}$ の法則として) によって最初の変数に関して分配されます。 E が可換である場合、この写像は方程式 $(xy)^n = x^n y^n$ により 2 番目の変数に関して分配的です。

#### 命題 1 {#alg-i-s3-prop-1 .statement tag=0582}

$E_1, E_2, \ldots, E_n$ と F を加法的に書かれた可換モノイドとし、u を $E_1 \times \cdots \times E_n$ の写像を F にするとします。これはすべての変数に関して分配的です。 $i = 1, 2, \ldots, n$ について、$L_i$ を空でない有限集合とし、$(x_{i,\lambda})_{\lambda \in L_i}$ を $E_i$ の元の族とします。 $y_i = \sum_{\lambda \in L_i} x_{i,\lambda}$を$i = 1, 2, \ldots, n$にしましょう。それから

(2) $$
u(y_1, \ldots, y_n) = \sum_\alpha u(x_1, \alpha_1, \ldots, x_n, \alpha_n)
$$

和は、数列 $\alpha = (\alpha_1, \ldots, \alpha_n)$ 所属から $L_1 \times \cdots \times L_n$ まですべて引き継がれます。

§ 1, no. 2の公式(2)から続く$n = 1$の場合をnについて帰納法で議論します。同じ参考文献より

(3) $$
u(y_1, \ldots, y_{n-1}, y_n) = \sum_{\alpha_n \in L_n} u(y_1, \ldots, y_{n-1}, x_n, \alpha_n)
$$

$y_n = \sum_{\alpha_n \in L_n} x_{n,\alpha_n}$と写像の$E_n$の$z \mapsto u(y_1, \ldots, y_{n-1}, z)$を$F$に入れるとマグマ準同型になります。 $E_1 \times \cdots \times E_{n-1}$ から $F$ までの分配写像 $(z_1, \ldots, z_{n-1}) \mapsto u(z_1, \ldots, z_{n-1}, x_n, \alpha_n)$ に帰納法の仮定が適用されることで、

(4)
$$
u(y_1, \ldots, y_{n-1}, x_n, \alpha_n) = \sum_{\alpha_1, \ldots, \alpha_{n-1}} u(x_1, \alpha_1, \ldots, x_{n-1}, \alpha_{n-1}, x_n, \alpha_n),
$$
和が数列 $(\alpha_1, \ldots, \alpha_{n-1})$ 所属から $M = L_1 \times \cdots \times L_{n-1}$ に引き継がれます。現在$L_1 \times \cdots \times L_n = M \times L_n$;書く
$$
t_{\alpha_1, \ldots, \alpha_n} = u(x_1, \alpha_1, \ldots, x_n, \alpha_n),
$$
私たちは持っています
(5)
$$
\sum_{\alpha_1, \ldots, \alpha_n} t_{\alpha_1, \ldots, \alpha_n} = \sum_{\alpha_n} \left( \sum_{\alpha_1, \ldots, \alpha_{n-1}} t_{\alpha_1, \ldots, \alpha_{n-1}, \alpha_n} \right)
$$
§ 1, no. 5の公式 (7) 作。 (2) は (3)、(4)、(5) の直後に続きます。

#### 注意 {#alg-i-s3-n4-rem-1 .statement tag=0583}

$i = 1, 2, \ldots, n$ と $a_j \in E_j$ ($j \neq i$) に対して $u(a_1, \ldots, a_{i-1}, 0, a_{i+1}, \ldots, a_n) = 0$ の場合、公式 (2) は有限台の家族 $(x_i, \lambda)_{\lambda \in L_i}$ に当てはまります。

定義 5 の特殊なケースは、$u$ がマグマ $E$ 上の集合 $\Omega$ の作用に関連付けられた作用の法則である場合です。 $u$ が 2 番目の変数に関して分配的である場合、マグマ $E$ 上の $\Omega$ の作用も分配的であると言われます。その他語:

#### 定義 6 {#alg-i-s3-def-6 .statement tag=0584}

*作用* $\alpha \mapsto f_\alpha$ *集合* $\Omega$ *マグマ上* $E$ *すべて* $\alpha \in \Omega$, *写像* $f_\alpha$ *マグマの自己準同型であれば分配的であると言われています* $E$。

$\top$がマグマ$E$の法則と、$E$上の$\Omega$の作用に関連付けられた作用の法則を$\perp$とすると、後者の分配性は次のように表されます。 公式
(6)
$$
\alpha \perp (x \top y) = (\alpha \perp x) \top (\alpha \perp y) \quad \text{(for } \alpha \in \Omega \text{ and } x, y \in E\text{)}.
$$

言葉の乱用により、法則 $\perp$ は法則 $\top$ に対して分配的（または正しい分配的）であるとも言われます。

§ 1, no. 2 の公式 (2) は、注文されたすべての数列 $(x_\lambda)_{\lambda \in L}$ の $E$ の元とすべての $\alpha \in \Omega$ について、
(7)
$$
\alpha \perp \left( \bigwedge_{\lambda \in L} x_\lambda \right) = \bigwedge_{\lambda \in L} (\alpha \perp x_\lambda).
$$

作用 $\alpha \mapsto f_\alpha$ が分散的で、$E$ の同値関係 $R$ が、$E$ の合成および作用 $\alpha \mapsto f_\alpha$、商作用の法則と互換性がある場合$E/R$ は分配的です。

$E$ 上の法則を乗法的に記述する場合、この乗法に関して分配的である作用の法則に対して指数関数記法 $x^\alpha$ を使用することが多く、そのため、分配性は恒等式 $(xy)^\alpha = x^\alpha y^\alpha$ で表されます。 E 上の法則が加法的に書かれている場合、この加法に関して分配的である作用の法則に対して左 (または右) 乗法記法 $\alpha . x$ (または $x . \alpha$) を使用することが多く、その分配性は恒等式によって表現されます。

$$
\alpha(x + y) = \alpha x + \alpha y \quad (\text{resp. } (x + y)\alpha = x\alpha + y\alpha).
$$

また、$\Omega$ が $\overline{T}$ で示される内部法則を持ち、作用の法則が最初の変数に関して分配的である場合を考慮することもできます。これは、次のことを意味します。

(8)
$$
(\alpha \overline{T} \beta) \perp x = (\alpha \perp x) T (\beta \perp x)
$$
$\alpha, \beta \in \Omega$ と $x \in E$ のすべてに。次に、§ 1, no. 2 の公式 (2) までに

(9)
$$
\left( \overline{T}_{\lambda \in L} \alpha_{\lambda} \right) \perp x = \overline{T}_{\lambda \in L} (\alpha_{\lambda} \perp x)
$$
注文した数列 $(\alpha_{\lambda})_{\lambda \in L}$、元、$\Omega$、およびすべての $x \in E$ に対して。

### 5. 他のに対する 1 つの内部法則の分配性

#### 定義 7 {#alg-i-s3-def-7 .statement tag=0585}

$T$ と $\perp$ を集合 E 上の 2 つの内部法則とします。 法則 $\perp$ は、法則 $T$ に関して分配的であると言われます。

(10)
$$
x \perp (y T z) = (x \perp y) T (x \perp z)
$$
(11)
$$
(x T y) \perp z = (x \perp z) T (y \perp z)
$$
E のすべての $x, y, z$ について。

法則 $\perp$ が可換である場合、(10) と (11) は等価であることに注意してください。一般に、法則の 1 つは加算的に記述され、もう 1 つは乗算的に記述されます。 乗法が加法に関して分配的である場合、次のようになります。

(12)
$$
x . (y + z) = x . y + x . z
$$
(13)
$$
(x + y) . z = x . z + y . z
$$

#### 例 {#alg-i-s3-n5-exa-1 .statement tag=0586}

(1) 集合 E の部分集合の集合 $\mathscr{P}(E)$ では、内部法則 $\cap$ と $\cup$ はそれぞれ、それ自身と他方に対して分配的です。 これは、形の公式から導き出されます。

$$
A \cap (B \cup C) = (A \cap B) \cup (A \cap C)
$$
$$
A \cup (B \cap C) = (A \cup B) \cap (A \cup C).
$$

(2) $\mathbf{Z}$ (より一般的には、任意の完全に順序付けされた集合) では、法則 sup と inf はそれぞれ、他方およびそれ自体に関して分配的です。

(3) $\mathbf{Z}$ (*そしてより一般的には任意の環*) では、乗法は加法に関して分配的です。

(4) $\mathbf{N}$ 加法と乗法は、法則 sup と inf に関して分配的です。

### 練習問題 {#alg-i-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
