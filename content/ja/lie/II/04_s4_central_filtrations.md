---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 4
section_title: Central filtrations
lang: ja
source: lie-i-iii
book_pages: 142-149, 187-193
pdf_pages: 0160-0167, 0205-0211
extraction: ocr
subsections:
    - "no": 1
      title: REAL FILTRATIONS
      page: 142
      pdf_page: 160
    - "no": 2
      title: ORDER FUNCTION
      page: 143
      pdf_page: 161
    - "no": 3
      title: GRADED ALGEBRA ASSOCIATED WITH A FILTERED ALGEBRA
      page: 144
      pdf_page: 162
    - "no": 4
      title: CENTRAL FILTRATIONS ON A GROUP
      page: 145
      pdf_page: 163
    - "no": 5
      title: AN EXAMPLE OF A CENTRAL FILTRATION
      page: 147
      pdf_page: 165
    - "no": 6
      title: INTEGRAL CENTRAL FILTRATIONS
      page: 148
      pdf_page: 166
statements: 12
exercises: 18
content_sha256: b60d0f142fa3f69ffddf37a4240ef97de3c1bdae10cb77f4851f3a5e372ab640
translated_from: content/en/lie/II/04_s4_central_filtrations.md
translation_method: google
source_content_sha256: 6dd2b136d04753cfdf0792754a0655d7811d3c21519c55e6a5ca6b7546279e90
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: e1056e2c719d4412d8940ef993c2a87a1468068217a6942abc88e9728389c12b
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 4。中央濾過

### 1. 実際の濾過

#### 定義 1 {#lie-ii-s4-def-1 .statement tag=0A4H}

$G$を群とします。 $G$ の実際のフィルタリングは、$G$ の部分群のファミリー $(G_\alpha)_{\alpha \in \mathbf{R}}$ です。
$$
G_\alpha = \bigcap_{\beta < \alpha} G_\beta \quad \text{for all } \alpha \in \mathbf{R}.
$$

公式 (1) は $\beta < \alpha$ に対して $G_\alpha \subset G_\beta$ を意味するため、ファミリー $(G_\alpha)$ は *減少する* になります。濾過 $(G_\alpha)$ が $\bigcap_\alpha G_\alpha$ 簡約するから単位元の場合は *分離* と呼ばれ、 $G = \bigcup_\alpha G_\alpha$ の場合は *完全* と呼ばれます。

#### 注意 {#lie-ii-s4-n1-rem-1 .statement tag=0A4I}

$(G_n)_{n \in \mathbf{Z}}$ を $G$ の部分群の減少列とします。 *可換代数*、章 III, § 2, no. 1、定義の意味での減少する濾過です。 1. 区間 $]n-1, n]$ のすべての整数 $n$ とすべての $\alpha$ $\mathbf{R}$、$H_\alpha = G_n$、特に$H_n = G_n$と書きます。したがって、$G$ で実際の濾過 $(H_\alpha)_{\alpha \in \mathbf{R}}$ が得られるのは明らかです。このような濾過は、*積分濾過*と呼ばれます。したがって、*可換代数*、章 III, § 2 という意味での減少する濾過は、積分濾過と識別できます。

$A$ を代数とします。 $A$の加法群の実際の濾過$(A_\alpha)$は、$\mathbf{R}$の$\alpha, \beta$に対して$A_\alpha . A_\beta \subset A_{\alpha + \beta}$、$\alpha \in \mathbf{R}$に対して$K . A_\alpha \subset A_\alpha$であれば、代数構造と互換性があると呼ばれます。濾過が徹底的である場合、$(A_\alpha)$ は、代数構造と互換性のある、$A$ の位相未満の 0 の近傍の基本的な系です。 $B$ を単位代数とします。 $B$の加法群の実際の濾過$(B_\alpha)$は、代数構造および$1 \in B_0$と互換性がある場合、ユニット代数構造と互換性があると呼ばれます。

### 2. 位数写像

$G$ を単位元 $e$ で群とします。 $(G_\alpha)$ を $G$ での実際のフィルタリングとします。 $G$ のすべての $x$ について、$I_x$ は実数 $\alpha$ の集合を表し、$x \in G_\alpha$ となるようにします。 $\alpha \in I_x$ と $\beta < \alpha$ の場合、$\beta \in I_x$、したがって $I_x$ は区間になります (*一般位相*、章 IV, § 2, no. 4、命題 1)。 関係 (1) を使用すると、これが有限である場合、$I_x$ 含むが最小の上界であることがわかります。したがって、$I_x$ は形 $]-\infty, v(x)] \cap \mathbf{R}$ と $v(x) \in \overline{\mathbf{R}}$ です。 $v(x) = \sup \{ \alpha \mid x \in G_\alpha \}$ があります。

$G$ の $\overline{\mathbf{R}}$ への写像 $v$ は、実際の濾過 $(G_\alpha)$ に関連付けられた *位数写像* と呼ばれ、$v(x)$ は $x$ の *位数* と呼ばれます。この写像には次の特性があります。

(a) *$x \in G$ と $\alpha \in \mathbf{R}$ の場合、関係 $x \in G_\alpha$ と $v(x) \geq \alpha$ は同等です。*

(b) *$G$の$x, y$の場合*
$$
v(x^{-1}) = v(x), \qquad v(e) = +\infty.
$$
$$
v(xy) \geq \inf(v(x), v(y)).
$$

*さらに、$v(x) > v(y)$であれば、(3)で等式が得られます。

(c) *すべての$\alpha \in \mathbf{R}$について、$G_\alpha^+$は$v(x) > \alpha$となるように$x \in G$の集合を表すものとします。その場合、$G_\alpha^+ = \bigcup_{\beta > \alpha} G_\beta$、特に $G_\alpha^+$ は $G$ の部分群になります。*

逆に、$v$ を $G$ の写像として、$\overline{\mathbf{R}}$ 満たす関係 (2) (3) とします。すべての $\alpha \in \mathbf{R}$ について、$G_\alpha$ を $x \in G$ の集合とし、$v(x) \geq \alpha$ とします。次に、$(G_\alpha)_{\alpha \in \mathbf{R}}$ は $G$ の実際のフィルタリングであり、$v$ はこのフィルタリングに関連付けられた位数写像です。

濾過 $(G_\alpha)$ が統合されるためには、$v$ 写像 $G$ を $\mathbf{Z} \cup \{+\infty, -\infty\}$ に変換することが必要かつ十分です。それが網羅的である (それぞれ分離される) ためには、$-v^{-1}(-\infty) = \varnothing$ (それぞれ $-v^{-1}(+\infty) = \{\epsilon\}$) であることが必要かつ十分です。

$A$ を K-代数 (それぞれ単位 K-代数) とします。以上より、関係

$$
"x \in A_\alpha \Leftrightarrow v(x) \geq \alpha \quad \text{for } x \in A \text{ and } \alpha \in \mathbf{R}"
$$

徹底したリアルろ過の定義する集合の全単射 $(A_\alpha)_{\alpha \in \mathbf{R}}$ は代数 (それぞれ単体代数) と互換性あり $A$ の構造から写像の集合まで$v : A \to \overline{\mathbf{R}}$ は、以下の値 $-\infty$ および満たすの公理 (4) ～ (7) (それぞれ (4) ～ (8)) を採用しません。

(4) $$v(x + y) \geq \inf(v(x), v(y)) \quad (x, y \text{ in } A)$$
(5) $$v(-x) = v(x) \qquad (x \in A)$$
(6) $$v(\lambda x) \geq v(x) \qquad (\lambda \in K, x \in A)$$
(7) $$v(xy) \geq v(x) + v(y) \qquad (x, y \text{ in } A)$$
(8) $$v(1) \geq 0.$$

#### 注意 {#lie-ii-s4-n2-rem-1 .statement tag=0A4J}

$v(x)$ がどこでも $+\infty$ に等しいわけではない場合、条件 (7) と (8) は $v(1) = 0$ を意味します。

### 3. フィルタリングされた代数に関連付けられた採点代数

$G$ を、実濾過 $(G_\alpha)_{\alpha \in \mathbf{R}}$ を伴う *可換* 群とします。 前にのように書きます

$$
G_\alpha^+ = \bigcup_{\beta > \alpha} G_\beta;
$$

明らかに $G_\alpha^+$ は $G_\alpha$ の部分群です。 $\operatorname{gr}_\alpha(G) = G_\alpha / G_\alpha^+$ と書きますと、

$$
\operatorname{gr}(G) = \bigoplus_{\alpha \in \mathbf{R}} \operatorname{gr}_\alpha(G).
$$

フィルタリングされた群* $G$ に関連付けられた * 等級付けされた群は群 $\operatorname{gr}(G)$ であり、その自然な段階は型 $\mathbf{R}$ です。

#### 注意 {#lie-ii-s4-n3-rem-1 .statement tag=0A4K}

濾過$(G_\alpha)$が積分の場合、$\operatorname{gr}_\alpha(G) = \{0\}$は非積分$\alpha$、整数$n$ごとに$\operatorname{gr}_n(G) = G_n / G_{n-1}$となります。関連するグレード群の定義は、したがって一致するは *可換代数*、章 III, § 2, no. 3 のグレードと本質的に同じになります。

$A$ を代数 (それぞれ単体代数) とし、$(A_\alpha)_{\alpha \in \mathbf{R}}$ を代数 (それぞれ単体代数) 構造 (no. 1) と互換性のある実際の濾過とします。それから

$$
A_\alpha \cdot A_\beta \subset A_{\alpha + \beta}, \qquad A_\alpha^+ \cdot A_\beta + A_\alpha \cdot A_\beta^+ \subset A_{\alpha + \beta}^+
$$

そして、商を双線形写像として、$A_\alpha \times A_\beta$ の双線形写像を $A$ 定義するの乗法の $A_{\alpha + \beta}$ 制限に変換します。

$$
\operatorname{gr}_\alpha(A) \times \operatorname{gr}_\beta(A) \to \operatorname{gr}_{\alpha + \beta}(A).
$$

gr(A) × gr(A) の双線形写像を gr(A) に導出し、それを型 $\mathbf{R}$ の段階的代数 (それぞれ単位段階的代数) にします。 A が結合 (可換、リー) 代数の場合、gr(A) も同様です。

### 4. 群の中央濾過

#### 定義 2 {#lie-ii-s4-def-2 .statement tag=0A4L}

G を群とします。 G 上の実際の濾過 $(G_\alpha)$ は、$G_\beta$ 属する ～ $G_{\alpha + \beta}$ の $G = \bigcup_{\alpha > 0} G_\alpha$ と交換子 $(x, y) = x^{-1}y^{-1}xy$ の元 x の $G_\alpha$ と元 y の場合、中央と呼ばれます。

位数写像 v の項では、上記の定義は関係に変換されます
$$
v(x) > 0, \quad v((x, y)) \geq v(x) + v(y) \quad \text{for all } x, y \text{ in } G.
$$
$v(x) \neq +\infty$ であれば $v((x, y)) > v(x)$ であると推測します。 $x^y = y^{-1}xy$ (cf. 代数, 章 I, § 6, no. 2) と書くと、$x^y = x.(x, y)$, よって
$$
v(x^y) = v(x).
$$
この関係は、Gの部分群$G_\alpha$がそれぞれ正常であることを表しています。 $G_\alpha$ 形は、G の群構造 (一般的な位相、章 III, § 1, no. 2、例) と互換性のある位相の e の近傍の基本系で、フィルターによって定義されると言われています。 $(G_\alpha)$。

この番号の残りの部分では、G は群を示し、中央濾過は $(G_\alpha)$ です。すべての $\alpha \in \mathbf{R}$ に対して、私たちは G の定義する部分群 $G_\alpha^+$ によって
$$
G_\alpha^+ = \bigcup_{\beta > \alpha} G_\beta.
$$
特に$\alpha \leq 0$の$G_\alpha^+ = G_\alpha = G$。 A と B が G の 2 つの部分群である場合、(A, B) は $a \in A$ と $b \in B$ を含む交換子 $(a, b)$ によって生成される G の部分群を表すことを思い出してください。これで記法の式が得られます
$$
(G_\alpha, G_\beta) \subset G_{\alpha + \beta}
$$
$$
(G_\alpha^+, G_\beta^+) \subset G_{\alpha + \beta}^+
$$
$$
(G, G_\alpha) \subset G_\alpha^+.
$$
(14) により、$G_\alpha^+$ はすべての $\alpha \in \mathbf{R}$ に対して $G_\alpha$ の通常の部分群であり、剰余群 $\mathrm{gr}_\alpha(G) = G_\alpha / G_\alpha^+$ は可換です。 $\mathrm{gr}(G) = \bigoplus_{\alpha \in \mathbf{R}} \mathrm{gr}_\alpha(G)$と書き、この群に型$\mathbf{R}$の卒業を与え、$\mathrm{gr}_\alpha(G)$は次数$\alpha$の元から構成されます。次に、$\alpha \leq 0$の場合は$\mathrm{gr}_\alpha(G) = \{0\}$です。

#### 命題 1 {#lie-ii-s4-prop-1 .statement tag=0A4M}

(i) $\alpha, \beta$ を $\mathbf{R}$ に入れます。二重添加剤写像が存在します
$$
\phi_{\alpha \beta} : \mathrm{gr}_\alpha(G) \times \mathrm{gr}_\beta(G) \to \mathrm{gr}_{\alpha + \beta}(G)
$$

写像 $(xG_\alpha^+, yG_\beta^+)$ を $(x, y)G_{\alpha+\beta}^+$ に重ねます。

(ii) $\phi$ を、$\mathrm{gr}(G) \times \mathrm{gr}(G)$ から $\mathrm{gr}(G)$ への二重加法写像とします。その $\mathrm{gr}_\alpha(G) \times \mathrm{gr}_\beta(G)$ に対する制限は、順序付けられた対 $(\alpha, \beta)$ ごとに $\phi_{\alpha\beta}$ になります。 写像 $\phi$ は $\mathrm{gr}(G)$ に嘘 $\mathbf{Z}$-代数構造を与えます。

(i) アイデンティティを思い出す

$$(xx', y) = (x, y)x'(x', y)$$

$G$ の $x, x', y$ (*代数*、章 I, § 6, no. 2、公式 (4 ビス))。

$x \in G_\alpha$ と $y \in G_\beta$ の場合、$G_{\alpha+\beta}$ の元 $(x, y)$ の $G_{\alpha+\beta}^+$ を法とする類は $f(x, y)$ で表されます。 $G_{\alpha+\beta}$の$a$と$G$、$a^{-1}.ax' = (a, x') \in G_{\alpha+\beta}^+$の$x'$の場合。特に、$f(x, y)$ は、$(x, y)x'$ の $G_{\alpha+\beta}^+$ を法とする類に等しくなります。したがって、公式 (15) は次のことを意味します。

$$f(xx', y) = f(x, y)f(x', y).$$

現在 $(y, x) = (x, y)^{-1}$、よって

$$f(y, x) = f(x, y)^{-1}.$$

(16) と (17) から推測します。

$$f(x, yy') = f(x, y)f(x, y').$$

商写像 $\phi_{\alpha\beta} : \mathrm{gr}_\alpha(G) \times \mathrm{gr}_\beta(G) \to \mathrm{gr}_{\alpha+\beta}(G)$ を取得して、 写像 $f : G_\alpha \times G_\beta \to \mathrm{gr}_{\alpha+\beta}(G)$ 定義するであることを証明する必要があります。 (16) と (18) により、(13') から導かれる、$x \in G_\alpha^+$ または $y \in G_\beta^+$ であれば $f(x, y) = 0$ であることを証明するのに十分です。

(ii) $(x, x) = e$ として、(17) から $\phi$ は交代的 $\mathbf{Z}$-双線形写像であることがわかります。したがって、$u \in \mathrm{gr}_\alpha(G)$、$v \in \mathrm{gr}_\beta(G)$、$w \in \mathrm{gr}_\gamma(G)$ について、次のことを証明する必要があります。

$$\phi(u, \phi(v, w)) + \phi(v, \phi(w, u)) + \phi(w, \phi(u, v)) = 0.$$

$x \in G_\alpha, y \in G_\beta$ と $z \in G_\gamma$ をそれぞれ $u, v$ と $w$ を表す元とします。 $x^y$ と $x$ は $G_\alpha^+$ を法として合同である $G_\alpha$ の 2 つの元であり、したがって $x^y$ は $G_\alpha$ における $u$ の代表であることがわかります。 $(y, z)$ は $G_{\beta+\gamma}$ の $\phi(v, w)$ の代表であるため、$(x^y, (y, z))$ は $G_{\alpha+\beta+\gamma}$ の $\phi(u, \phi(v, w))$ の代表であることがわかります。循環置換により、$(y^z, (z, x))$と$(z^x, (x, y))$がそれぞれ$G_{\alpha+\beta+\gamma}$の$\phi(v, \phi(w, u))$と$\phi(w, \phi(u, v))$を表していることが分かります。 関係 (19) は、次の恒等式の帰結になります (*代数*、章 I, § 6, no. 2、公式 (15))。

$$(x^y, (y, z)).(y^z, (z, x)).(z^x, (x, y)) = e.$$

命題 1 で定義された $\mathbf{Z}$ 上のリー代数 $\mathrm{gr}(G)$ は、フィルタリングされた群* $G$ に関連付けられた * 等級付けされたリー代数と呼ばれます。

### 5. 中央濾過の例

$A$ を、$A_0 = A$ となるような単位代数濾過 $(A_\alpha)$ を伴う単位結合代数とします。その場合、$A_\alpha$ は、すべての $\alpha \in \mathbf{R}$ に対する $A$ の両面の理想となります。 $A^*$ が $A$ の可逆元の乗法群を表すものとします。すべての $\alpha > 0$ について、$\Gamma_\alpha$ が $x - 1 \in A_\alpha$ となるような $x \in A^*$ の集合を表すものとします。 $\beta \leq 0$を$\Gamma = \bigcup_{\alpha > 0} \Gamma_\alpha$と$\Gamma_\beta = \Gamma$と書きます。

#### 命題 2 {#lie-ii-s4-prop-2 .statement tag=0A4N}

*集合 $\Gamma$ は $A^*$ の部分群であり、$(\Gamma_\alpha)$ は $\Gamma$ の中央濾過です。*

構成による$\Gamma = \bigcup_{\alpha > 0} \Gamma_\alpha$と関係 $\Gamma_\alpha = \bigcap_{\beta < \alpha} \Gamma_\beta$は$A_\alpha = \bigcap_{\beta < \alpha} A_\beta$から続きます。

$\Gamma_\alpha$ は $A^*$ の部分群であることがわかります。現在 $1 \in \Gamma_\alpha$; $x, y$ を $\Gamma_\alpha$、よって $x - 1 \in A_\alpha, y - 1 \in A_\alpha$ に入れます。 $A_\alpha$ は $A$ の両面イデアルであるため、公式は
$$
(21) \quad xy - 1 = (x - 1)(y - 1) + (x - 1) + (y - 1),
$$
$$
(22) \quad x^{-1} - 1 = -x^{-1}(x - 1),
$$
$xy - 1 \in A_\alpha$ と $x^{-1} - 1 \in A_\alpha$、よって $xy \in \Gamma_\alpha$ と $x^{-1} \in \Gamma_\alpha$ を暗示します。

$\Gamma = \bigcup_{\alpha > 0} \Gamma_\alpha$ として、これは $A^*$ の部分群です。

最後に$\alpha > 0, \beta > 0, x \in \Gamma_\alpha$と$y \in \Gamma_\beta$をさせます。 $x - 1 = \xi$と$y - 1 = \eta$としましょう。それから
$$
(23) \quad (x, y) - 1 = x^{-1}y^{-1}(\xi \eta - \eta \xi);
$$
仮定、$\xi \in A_\alpha$、$\eta \in A_\beta$、よって $\xi \eta - \eta \xi \in A_{\alpha + \beta}$ による。 $A_{\alpha + \beta}$ は、$A$、$(x, y) - 1 \in A_{\alpha + \beta}$、よって $(x, y) \in \Gamma_{\alpha + \beta}$ の両面の理想です。

#### 注意 {#lie-ii-s4-n5-rem-1 .statement tag=0A4O}

$\alpha \geq 0, \beta \geq 0$ と $x \in \Gamma_\alpha, y \in \Gamma_\beta$ としましょう。式(21)、(22)、(23)より、
$$
(24) \quad x^{-1} - 1 \equiv -(x - 1) \pmod{A_{2\alpha}}
$$
$$
(25) \quad xy - 1 \equiv (x - 1) + (y - 1) \pmod{A_{\alpha + \beta}}
$$
$$
(26) \quad (x, y) - 1 \equiv [(x - 1), (y - 1)] \pmod{A_{\alpha + \beta + \inf(\alpha, \beta)}}.
$$

たとえば (26) を証明します。 $x - 1 = \xi$ と $y - 1 = \eta$ の場合、(23) は次のようになります。
$$
(x, y) - 1 - [\xi, \eta] = ((x^{-1} - 1) + (y^{-1} - 1) + (x^{-1} - 1)(y^{-1} - 1))[\xi, \eta].
$$
ここで、$[\xi, \eta] \in A_{\alpha + \beta}$、$(x^{-1} - 1) \in A_\alpha$、$(y^{-1} - 1) \in A_\beta$、よってにより (26) が得られます。

$G$ を群と $\rho : G \to \Gamma$ 準同型とします。すべての実数 $\alpha$ については、$G_\alpha = \rho^{-1}(\Gamma_\alpha)$ と書きます。 $(\Gamma_\alpha)$が$\Gamma$の中央濾過であるため、$(G_\alpha)$が$G$の中央濾過であることは明らかになります。

#### 命題 3 {#lie-ii-s4-prop-3 .statement tag=0A4P}

(i) *すべての $\alpha \in \mathbf{R}$ に対して、元 $a \in G_\alpha$ の $G_\alpha^+$ を法とする写像類から $\rho(a) - 1$ の $A_\alpha^+$ を法とする類である一意な群準同型 $g_\alpha : \mathrm{gr}_\alpha(G) \to \mathrm{gr}_\alpha(A)$ が存在します。

(ii) g を gr(G) の群準同型として gr(A) に変換します。その制限から gr_\alpha(G) はすべての \alpha について g_\alpha になります。 写像 g はリー \mathbf{Z}-代数の単射準同型です。

(i) \alpha > 0 とします。仮定により、G_\alpha のすべての a について、\rho(a) - 1 \in A_\alpha; p_\alpha(a) が \rho(a) - 1 を法とする A_\alpha^+ の類を表すものとします。 A_{2\alpha} \部分集合 A_\alpha^+ であるため、関係 (25) は p_\alpha(ab) = p_\alpha(a) + p_\alpha(b) を意味します。次に、 \rho(a) - 1 \in A_\alpha^+ の場合に限り、 \in G_\alpha^+ になります。したがって、G_\alpha^+ は、G_\alpha の gr_\alpha(A) への準同型 p_\alpha の核です。 移行から商では、p_\alpha から定義する単射準同型 gr_\alpha(G) の g_\alpha を gr_\alpha(A) に変換します。

\alpha \leq 0 の場合、gr_\alpha(G) = \{0\} であり、唯一の選択は g_\alpha = 0 です。

(ii) g_\alpha はすべての実数 \alpha に対して単射であるため、g は単射です。 g がリー代数準同型であることを示します。 \alpha \leq 0 に対して gr_\alpha(G) = \{0\} であるため、公式を確立するだけで十分です。

$$
p_{\alpha+\beta}((a, b)) = [p_\alpha(a), p_\beta(b)]
$$

\alpha > 0、\beta > 0、\rightarrow \in G_\alpha および b \in G_\beta の場合、(26) から続きます。

### 6. 一体型中央濾過装置

(no. 1, 注意) を思い出してください。群 G 上の濾過 (G_\alpha) は、すべての整数 n と \{n-1, n\} 内のすべての \alpha \ について G_\alpha = G_n である場合、積分と呼ばれます。 群 G に積分中央濾過が与えられることは、G 満たす条件の部分群の数列 (G_n)_{n \geq 1} が与えられることと同等です。

(i) \quad G_1 = G
(ii) \quad G_n \supset G_{n+1} \quad \text{for all } n \geq 1
$m \geq 1$ と $n \geq 1$ の場合は $(iii) \quad (G_m, G_n) \subset G_{m+n}$。

すべての整数 n \geq 1 に対して、G_n は G の正規の部分群であり、 商 gr_n(G) = G_n/G_{n+1} は可換です。 商, 写像 (x, y) \mapsto (x, y) = x^{-1}y^{-1}xy の G_m \times G_n を G_{m+n} にすると、 gr(G) = \bigoplus_{n \geq 1} gr_n(G) で定義するをグレーディングリー代数にすることができます。 型 \mathbf{N} の環 \mathbf{Z} の構造。

(代数, 章 I, § 6, no. 3, 定義 5) 群 G の下中央系列が次のように定義されていることを思い出してください。

$$
C^1G = G, \quad C^{n+1} = (G, C^nG) \quad \text{for } n \geq 1.
$$

対応する濾過はGの下部中央濾過と呼ばれます。

#### 命題 4 {#lie-ii-s4-prop-4 .statement tag=0A4Q}

(i) G の下部中央系列は、G 上の統合された中央濾過です。

(ii) (G_n)_{n \in \mathbf{N}^*} が G 上の積分中心濾過である場合、すべての n \in \mathbf{N}^* に対して C^nG \部分集合 G_n となります。

主張 (i) は代数, 章 I, § 6, no. 3, 公式 (7) で証明されました。

n について帰納法によって (ii) を証明します。 C^1G = G = G_1; n > 1の場合、

$$
C^nG = (G, C^{n-1}G) \subset (G, G_{n-1}) \subset G_n.
$$

#### 命題 5 {#lie-ii-s4-prop-5 .statement tag=0A4R}

G を群とし、gr(G) を G の下部中央濾過に関連する段階的リー $\mathbf{Z}$ 代数とする。すると、gr(G) は $\mathrm{gr}_1(G) = G/(G, G)$ によって生成されます。

L を、$\mathrm{gr}_1(G)$ によって生成された gr(G) の嘘部分代数とします。 $L \supset \mathrm{gr}_n(G)$ by 帰納法 n について、主張は $n = 1$ にとって自明であることを示します。 $n > 1$ と $L \supset \mathrm{gr}_{n-1}(G)$ と仮定します。 gr(G) のリー代数法則の $C^nG = (G, C^{n-1}G)$、構成はすぐに次のことを示しています。

$$
\mathrm{gr}_n(G) = [\mathrm{gr}_1(G), \mathrm{gr}_{n-1}(G)] \subset L.
$$

上の証明は、リー代数 gr(G) (§ 2, no. 7) の下中央系列が次の式で与えられることを示しています。

$$
\mathscr{C}^n(\mathrm{gr}(G)) = \sum_{m \geq n} \mathrm{gr}_m(G).
$$

#### 注意 {#lie-ii-s4-n6-rem-1 .statement tag=0A4S}

k を n 行、n 列と元を持つ下三角行列の k を環、n 整数 $> 0$、A 集合とします。 $p \geq 0$の場合、$A_p$を$(x_{ij}) \in A$の集合とし、$i - j < p$に対して$x_{ij} = 0$とします。続いて$A_0 = A$と$A_pA_q \subset A_{p+q}$。 $\Gamma_p = 1 + A_p$ にしましょう。この場合、$\Gamma_1$ は、k 上の位数 n の厳密な下三角群と呼ばれる、$\mathbf{GL}(n, k)$ の部分群です。 no. 5の命題 2により、$(\Gamma_p)$は$\Gamma_1$の積分濾過となります。 $\Gamma_n = \{1\}$ であるため、群 $\Gamma_1$ は無能であることがわかります (代数、章 I, § 6, no. 3、定義 6)。

### 練習問題 {#lie-ii-s4-exercises}

次の練習問題では、文字 G は群を表します。

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
