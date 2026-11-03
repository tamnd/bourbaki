---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 3
section_title: Tensor products
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 243-266, 395-396
pdf_pages: 0267-0290, 0419-0420
extraction: ocr
subsections:
    - "no": 1
      title: TENSOR PRODUCT OF TWO MODULES
      page: 243
      pdf_page: 267
    - "no": 2
      title: TENSOR PRODUCT OF TWO LINEAR MAPPINGS
      page: 245
      pdf_page: 269
    - "no": 3
      title: CHANGE OF RING
      page: 246
      pdf_page: 270
    - "no": 4
      title: OPERATORS ON A TENSOR PRODUCT; TENSOR PRODUCTS AS MULTIMODULES
      page: 247
      pdf_page: 271
    - "no": 5
      title: TENSOR PRODUCT OF TWO MODULES OVER A COMMUTATIVE RING
      page: 249
      pdf_page: 273
    - "no": 6
      title: PROPERTIES OF $E \otimes_A F$ RELATIVE TO EXACT SEQUENCES
      page: 251
      pdf_page: 275
    - "no": 7
      title: TENSOR PRODUCTS OF PRODUCTS AND DIRECT SUMS
      page: 254
      pdf_page: 278
    - "no": 8
      title: ASSOCIATIVITY OF THE TENSOR PRODUCT
      page: 258
      pdf_page: 282
    - "no": 9
      title: TENSOR PRODUCT OF FAMILIES OF MULTIMODULES
      page: 259
      pdf_page: 283
statements: 30
exercises: 4
content_sha256: bf396231b44f2aa2ece669ab00293f194360c136c16b17d0c22dc3e283d73700
translated_from: content/en/alg/II/03_s3_tensor_products.md
translation_method: google
source_content_sha256: 4cc4310afca7381c71a95e1a30d8b454ee7692d8209261c6a3c8ad67f1781a39
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: b3a9d2952fb363d687eb48d2aa9203141e72e59329224e9195e9c09e802daca8
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 3。 テンソル積

### 1. テンソル積/2 加群

$G_1, G_2$ を 2 つの $\mathbf{Z}$ モジュールとします。集合 $G = G_1 \times G_2$ の $\mathbf{Z}$ モジュールへのマッピング $u$ は、$u(x_1, x_2)$ が「$x_1$ および $x_2$ に関して加法的」である場合、双加法 (または $\mathbf{Z}$ 双線形) と呼ばれます。正確に言うと、これは、$G_1$の$x_1, y_1$、$G_2$の$x_2, y_2$、

$$
u(x_1 + y_1, x_2) = u(x_1, x_2) + u(y_1, x_2)
$$
$$
u(x_1, x_2 + y_2) = u(x_1, x_2) + u(x_1, y_2).
$$

これは特に、すべての $x_1 \in G_1, x_2 \in G_2$ に対して $u(0, x_2) = u(x_1, 0) = 0$ を意味することに注意してください。

A を環、E 右A-加群、F 左A-加群とします。普遍的な写像問題 (集合理論, IV, § 3, no. 1) を検討します。ここで、$\Sigma$ は $\mathbf{Z}$ モジュール構造の種です (射は、他の語では $\mathbf{Z}$ 線形写像であり、 加法群準同型)、および $\alpha$-マッピングは、$E \times F$ の写像 $f$ を $\mathbf{Z}$ モジュール G に変換します。これは、すべての $x \in E, y \in F$ に対して、$\mathbf{Z}$ 双線形であり、さらに満たすです。 $\lambda \in A$

$$(1)$$
$$
f(x \lambda, y) = f(x, \lambda y).
$$

この問題が解を認めることを示します。 このために、$E \times F$ の要素と $\mathbf{Z}$ (§ 1, no. 11) の係数との形式的な線形結合の $\mathbf{Z}$ 加群 $C = \mathbf{Z}^{(E \times F)}$ を検討します。その基礎は、$x \in E$ と $y \in F$ の順序ペア $(x, y)$ から構成されると考えることができます。 D を、次の型の 1 つの元によって生成された C のサブ $\mathbf{Z}$ モジュールとします。

$$(2)$$
$$
\begin{cases}
(x_1 + x_2, y) - (x_1, y) - (x_2, y) \\
(x, y_1 + y_2) - (x, y_1) - (x, y_2) \\
(x \lambda, y) - (x, \lambda y)
\end{cases}
$$

ここで、$x, x_1, x_2$ は $E$ に、$y, y_1, y_2$ は $F$ に、$\lambda$ は $A$ にあります。

#### 定義 1 {#alg-ii-s3-def-1 .statement tag=05OR}

*右側の A モジュール E と左側の A モジュール F* のテンソル積。$E \otimes_A F$ または $E \otimes_A F$ (または、混乱を恐れない場合は単に $E \otimes F$) で表されます。 * は $\mathbf{Z}$ モジュール* $C/D$ ($\mathbf{Z}$ モジュール C の商)タイプの 1 つの要素によって生成されたサブモジュール $D$ による、$E \times F$ の要素と $\mathbf{Z}$ の係数の形式的な線形結合の組み合わせ (2))。 ※$x \in E$と$y \in F$では、元の標準像$C = \mathbf{Z}^{(E \times F)}$の$(x, y)$である$E \otimes_A F$の元を$x \otimes y$で表し、$x$と$y$のテンソル積と呼びます。

$E \times F$ の $E \otimes_A F$ への写像 $(x, y) \mapsto x \otimes y$ は *正規* と呼ばれます。これは、条件 (1) を満たす $\mathbf{Z}$ 双線形写像です。

先ほど提起した普遍写像問題のテンソル積 $E \otimes_A F$ と上記の標準写像形解を示します。正確に言うと:

#### 命題 1 {#alg-ii-s3-prop-1 .statement tag=05OS}

(a) *$g$ を、$E \otimes_A F$ の $\mathbf{Z}$ モジュール $G$ への $\mathbf{Z}$ 線形マッピングとします。 $E \times F$ の $G$ への写像 $(x, y) \mapsto f(x, y) = g(x \otimes y)$ は $\mathbf{Z}$ 双線形であり、条件 (1) を満たします。*

(b) *逆に、$f$ を $E \times F$ の $\mathbf{Z}$ 加群 $G$ 満たす条件 (1) への $\mathbf{Z}$ 双線形写像とする。この場合、$x \in E, y \in F$ に対して $f(x, y) = g(x \otimes y)$ となるような、$E \otimes_A F$ の $G$ への $\mathbf{Z}$ 線形写像 $g$ が 1 つだけ存在します。

$\phi$ が $E \times F$ の $E \otimes_A F$ への標準写像を表す場合、$f = g \circ \phi$。 よって (a)。 (b) を示すために、定義 1 の記法で、$f$ 拡大するが $C$ の $\bar{f}$ から $G$ (§ 1, no. 11, 命題 17) への$\mathbf{Z}$ 線形マッピングに注目します。 関係 (1) により、型 (2) の 1 つの $C$ のすべての元に対して $\bar{f}$ は零となり、したがって $D$ になります。したがって、$C/D = E \otimes_A F$ から $G$ への $\mathbf{Z}$ 線形写像 $g$ が存在し、$\bar{f} = g \circ \psi$ になります。ここで、$\psi : C \to C/D$ は標準準同型 (§ 1, no. 8, *注意*) です。 $g$ の一意性は、形 $x \otimes y$ の元によって $E \otimes_A F$ が $\mathbf{Z}$ モジュールとして生成されるため、明らかになります。

命題 1 定義する $E \times F$ の $\mathbf{Z}$ 双線形写像 $f$ の $\mathbf{Z}$ モジュールの *標準同型* を $G$、満たす条件 (1) に、 $\mathbf{Z}$-モジュール$\mathrm{Hom}_{\mathbf{Z}}(E \otimes_A F, G)$。

$A = \mathbf{Z}$、条件 (1) は、*すべての* $\mathbf{Z}$-双線形写像 $f$ および $C$ の部分加群 $D$ について、(2) の最初の 2 つの型のうち元によってすでに生成されています。

ここで一般的なケースに戻り、$E'$ と $F'$ がそれぞれ $E$ と $F$ の基礎となる $\mathbf{Z}$ モジュールを表す場合、上記の注意と定義 1 は、$\mathbf{Z}$ モジュール $E \otimes_A F$ が次のとおりであることがすぐにわかります。 形 $(x \lambda) \otimes y - x \otimes (\lambda y)$ の元によって生成されたサブ $\mathbf{Z}$ モジュールによって、$\mathbf{Z}$ モジュール $E' \otimes_{\mathbf{Z}} F'$ の *商* と正規に識別されます。ここで、$x$ は $E$ を通過し、$y$ は通過します$F$ と $\lambda$ は $A$ を通過します。

#### 系 1 {#alg-ii-s3-prop-1-cor-1 .statement tag=05OT}

*$H$ を $\mathbf{Z}$ モジュール、$h : E \times F \to H$ を $\mathbf{Z}$ 双線形マッピング満たす条件 (1) とし、$H$ が $h(E \times F)$ によって生成されるようにします。 すべての $\mathbf{Z}$ モジュール $G$ および $E \times F$ から $G$ 満たす (1)* へのすべての $\mathbf{Z}$ 双線形写像 $f$ に対して、$f = g \circ h$ のような $\mathbf{Z}$ 線形写像 $g : H \to G$ が存在すると仮定します。 次に、$\phi$ が $E \times F$ の $E \otimes_A F$ への正準写像を表す場合、$h = \theta \circ \phi$ のような $E \otimes_A F$ の $H$ への同型写像 $\theta$ が 1 つだけ存在します。

仮定 $h(E \times F)$ 生成する $H$ は $g$ の一意性を意味します。したがって、系は、普遍的な写像問題 (集合理論、IV, § 3, no. 1) の解の一般的な一意性性質にすぎません。

#### 系 2 {#alg-ii-s3-prop-1-cor-2 .statement tag=05OU}

*$E^0$ (それぞれ $F^0$) *加群* $E$ (それぞれ $F$) *反対環* $A^0$ の上の左 (それぞれ右) 加群とみなします。 *その場合、* $\mathbf{Z}$* モジュール同型* $\sigma : E \otimes_A F \to F^0 \otimes_{A^0} E^0$ * $\sigma(x \otimes y) = y \otimes x$ * $x \in E$ * および* $y \in F$ (テンソル積の "可換性") が存在します。

$E^0$ と $F^0$ 上の $A^0$ モジュール構造の定義により、 $E \times F$ の $F^0 \otimes_{A^0} E^0$ への写像 $(x, y) \mapsto y \otimes x$ は $\mathbf{Z}$ 双線形であり、条件 (1) を満たします。 よって $\mathbf{Z}$ 線形写像 $\sigma$ の存在と一意性。同様に、$\mathbf{Z}$ 線形マッピング $\tau : F^0 \otimes_{A^0} E^0 \to E \otimes_A F$ は、$\tau(y \otimes x) = x \otimes y$ と明らかに $\sigma$ および $\tau$ が逆同型になるように定義されます。

#### 注意 {#alg-ii-s3-n1-rem-1 .statement tag=05OV}

非ゼロ加群のテンソル積は、零になる可能性があります。たとえば、2 つの $\mathbf{Z}$ モジュール $E = \mathbf{Z}/2\mathbf{Z}$ と $F = \mathbf{Z}/3\mathbf{Z}$、$2x = 0$ と $3y = 0$ をすべての $x \in E$ と $y \in F$ に対してとります。したがって、$E \otimes_{\mathbf{Z}} F$では、
$$
x \otimes y = 3(x \otimes y) - 2(x \otimes y) = x \otimes (3y) - (2x) \otimes y = 0
$$
すべての$x$ と $y$ (cf. no. 6、系 4 ～ 命題 6)。

### 2. テンソル積/2 線形写像

$A$ を環、$E, E'$ 2 つの右側 $A$ モジュール、$F, F'$ 2 つの左側 $A$ モジュール、および $u : E \to E'$ と $v : F \to F'$ 2 つの $A$ 線形マッピングとします。 写像であることは簡単に検証できます。
$$
(x, y) \mapsto u(x) \otimes v(y)
$$
$E \times F$ の $E' \oplus_A F'$ は $\mathbf{Z}$ 双線形であり、no. 1 の条件 (1) を満たします。したがって、no. 1 の命題 1 までに、次のような $\mathbf{Z}$ 線形写像 $w : E \otimes_A F \to E' \otimes_A F'$ が 1 つだけ存在します。
$$
w(x \otimes y) = u(x) \otimes v(y)
$$
$x \in E, y \in F$用。この写像は$u \otimes v$（混乱が生じない場合）で表され、線形写像$u$と$v$の*テンソル積*と呼ばれます。

(3) からすぐに、$(u, v) \mapsto u \otimes v$ は *canonical* と呼ばれる $\mathbf{Z}\text{-bilinear}$ 写像であることがわかります。
$$
\operatorname{Hom}_A(E, E') \times \operatorname{Hom}_A(F, F') \to \operatorname{Hom}_{\mathbf{Z}}(E \otimes_A F, E' \otimes_A F').
$$

これは、正準と呼ばれる no. 1 $\mathbf{Z}$ 線形写像の命題 1 によって対応します。

(4) $$
\operatorname{Hom}_A(E, E') \otimes_{\mathbf{Z}} \operatorname{Hom}_A(F, F') \to \operatorname{Hom}_{\mathbf{Z}}(E \otimes_A F, E' \otimes_A F')
$$
これは、テンソル積線形写像 $u \otimes v : E \otimes_A F \to E' \otimes_A F'$ のすべての元 $u \otimes v$ に関連付けられます。 標準写像 (4) *必ずしも単射でも全射でもない*ことに注意してください。したがって、記法 $u \otimes v$ は混乱を招く可能性があり、文脈上、それがテンソル積の元を表すのか、線形写像を表すのかを示す必要があります。

さらに、$E''$ を右の $A$ モジュール、$F''$ を左の $A$ モジュール、および $u' : E' \to E''$、$v' : F' \to F''$ $A$ の線形マッピングとします。 (3) から次のことがわかります。
(5)
$$
(u' \circ u) \otimes (v' \circ v) = (u' \otimes v') \circ (u \otimes v).
$$

### 3. 環中変更

#### 命題 2 {#alg-ii-s3-prop-2 .statement tag=05OW}

*$A, B$ を 2 つの環、$\rho : B \to A$ 環準同型、および $E$ (それぞれ $F$) の右 (それぞれ左) $A$ モジュールとします。その場合、唯一の $\mathbf{Z}$-線形マッピング* が存在します。
(6)
$$
\phi : \rho_*(E) \otimes_B \rho_*(F) \to E \otimes_A F
$$
*すべての $x \in E$ と $y \in F$ について、元の $\phi$ $\rho_*(E) \otimes_B \rho_*(F)$ の $x \otimes y$ の下の像は、$E \otimes_A F$ の元 $x \otimes y$ になります。この $\mathbf{Z}$ 線形写像は全射法です。*

$\rho_*(E) \times \rho_*(F)$ の $E \otimes_A F$ へのマッピング $(x, y) \mapsto x \otimes y$ を検討します。それは$\mathbf{Z}$-双線形であり、すべての$\beta \in B$について、定義により$(x \rho(\beta)) \otimes y = x \otimes (\rho(\beta)y)$であるため、no. 1の条件(1)が成り立ち、そこから$\phi$の存在と一意性が決まります(no. 1、命題1)。 後者の主張は、 元 $x \otimes y$ 生成するの $\mathbf{Z}$ モジュール $E \otimes_A F$ から導き出されます。

写像 (6) は *正規* と呼ばれます。

#### 系 {#alg-ii-s3-n3-cor-1 .statement tag=05OX}

*$\mathfrak{J}$ を、$\mathfrak{J}$ が $E$ の消滅子と $F$ の消滅子に含まれるように、$E$ (それぞれ $F$) が正規の左 (それぞれ右) を持つように、$A$ の両側理想とする。 $(A/\mathfrak{J})$ モジュール構造* ($§ 1$、no. 12)。 *それでは標準準同型* (6)
$$
\phi : E \otimes_A F \to E \otimes_{A/\mathfrak{J}} F
$$
*対応する ～ 標準準同型 $\rho : A \to A/\mathfrak{J}$ が正体です。*

すべての $\bar{\alpha} \in A/\mathfrak{J}$、すべての $x \in E$、およびすべての $y \in F$、$x \bar{\alpha} = x \alpha$ (それぞれ $\bar{\alpha} y = \alpha y$) について、$\rho(\alpha) = \bar{\alpha}$ などのすべての $\alpha$ について。 $C = \mathbf{Z}^{(E \times F)}$ の場合、元 $(x \alpha, y) - (x, \alpha y)$ によって生成された $C$ の部分加群は、元 $(x \bar{\alpha}, y) - (x, \bar{\alpha} y)$ によって生成された部分加群と等しくなります。

命題 2 の仮説と記法を使用して、$E'$ を右 $B$ 加群、$F'$ を左 $B$ 加群とし、2 つの *半線形* 写像 $u : E' \to E$、v:F' \to F を考慮します。 準同型 $\rho : B \to A$; $u$ (それぞれ $v$) は $B$ の線形マッピング $E' \to \rho_*(E)$ (それぞれ $F' \to \rho_*(F')$)、 よっては $w(x' \otimes y') = u(x') \otimes v(y')$ となる $\mathbf{Z}$ の線形マッピング $w : E' \otimes_B F' \to \rho_*(E) \otimes_B \rho_*(F)$ と考えることができます。 $x' \in E',\ y' \in F'$; 標準写像 (6) とこの写像を合成すると、$x' \in E',\ y' \in F'$ に対して $w'(x' \otimes y') = u(x') \otimes v(y')$ となるような $\mathbf{Z}$ 線形写像 $w' : E' \otimes_B F' \to E \otimes_A F$ が得られます。これは写像で、混乱が生じなければ通常は $u \otimes v$ で表されます。明らかに $(u, v) \mapsto u \otimes v$ は $\mathbf{Z}$ 双線形写像です

$$
\operatorname{Hom}_B(E', \rho_*(E)) \times \operatorname{Hom}_B(F', \rho_*(F)) \to \operatorname{Hom}_\mathbf{Z}(E' \otimes_B F', E \otimes_A F).
$$

さらに、$C$ が 3 番目の環、$\sigma : C \to B$ 準同型、$E''$ が右側の $C$ モジュール、$F''$ が左側の $C$ モジュールである場合、$u' : E'' \to E'$ および $v' : F'' \to F'$ の半線形マッピングとなります。 $\sigma$ を基準にすると、

$$
(u \circ u') \otimes (v \circ v') = (u \otimes v) \circ (u' \otimes v').
$$

### 4. テンソル積のオペレーター。 テンソル積マルチモジュールとして

no. 1 の仮説と記法を使用すると、$A$ モジュール $E$ (それぞれ $F$) のすべての自己準同型 $u$ (それぞれ $v$) に対して、$u \otimes 1_F$ (それぞれ $1_E \otimes v$) は次のようになります。 $\mathbf{Z}$ モジュール $E \otimes_A F$ の自己準同型; (5) (no. 2) から、写像 $u \mapsto u \otimes 1_F$ (それぞれ $v \mapsto 1_E \otimes v$) は *環準同型* であることがわかります。

$$
\operatorname{End}_A(E) \to \operatorname{End}_\mathbf{Z}(E \otimes_A F)
$$

(それぞれ $\operatorname{End}_A(F) \to \operatorname{End}_\mathbf{Z}(E \otimes_A F)$);さらに、

$$
(u \otimes 1_F) \circ (1_E \otimes v) = (1_E \otimes v) \circ (u \otimes 1_F) = u \otimes v
$$

したがって、(§ 1, no. 14) $E \otimes_A F$ は、環 $\operatorname{End}_A(E)$ および $\operatorname{End}_A(F)$ に関して正規 *left 両側加群* 構造を持ちます。

したがって、$E$ に $((B'_i); A, (C'_j))$ マルチモジュール構造が与えられ、$F$ に $(A, (B''_h); (C''_{k_c}))$ マルチモジュール構造 (§ 1, no. 14) が与えられたとします。 環準同型 $B'_i \to \operatorname{End}_A(E)$、$C'_j{}^0 \to \operatorname{End}_A(E)$ はペアごとに置換可能な像で与えられ、環準同型 $B''_h \to \operatorname{End}_A(F)$、$C''_{k_c}{}^0 \to \operatorname{End}_A(F)$ はペアごとに置換可能な像で与えられると言うのと同じことになります。これらの準同型を、上で定義した標準準同型 $\operatorname{End}_A(E) \to \operatorname{End}_\mathbf{Z}(E \otimes_A F)$ および $\operatorname{End}_A(F) \to \operatorname{End}_\mathbf{Z}(E \otimes_A F)$ とそれぞれ合成すると、（(7) を考慮して） 環準同型となることがわかります。

$$
\begin{align*}
B'_i &\to \operatorname{End}_\mathbf{Z}(E \otimes_A F), & C'_j{}^0 &\to \operatorname{End}_\mathbf{Z}(E \otimes_A F) \\
B''_h &\to \operatorname{End}_\mathbf{Z}(E \otimes_A F), & C''_{k_c}{}^0 &\to \operatorname{End}_\mathbf{Z}(E \otimes_A F)
\end{align*}
$$

*ペアワイズ置換可能* 像で定義されます。他の語では、$E \otimes_A F$ に $((B'_i), (B''_h); (C'_j), (C''_{k_c}))$ マルチモジュール構造が定義されています。このマルチモジュールは、* の *テンソル積* ($A$ に対して) とも呼ばれます。

((B'_i); A, (C'_j))-マルチモジュール E と (A, (B''_h); (C''_k))-マルチモジュール F。このマルチモジュールは、no. 1 で検討したものと類似したユニバーサル写像問題の解です。正確に言うと:

#### 命題 3 {#alg-ii-s3-prop-3 .statement tag=05OY}

G を ((B'_i), (B''_h); (C'_j), (C''_k)) マルチモジュールとします。

(a) g をマルチモジュール E $\otimes_A$ F から G への線形写像とします。 E $\times$ F から G への写像 $f : (x, y) \mapsto g(x \otimes y)$ は $\mathbf{Z}$ 双線形であり、no. 1 と条件の関係 (1) を満たします。

$$
\begin{cases}
f(\mu'_i x, y) = \mu'_i f(x, y), & f(x v'_j, y) = f(x, y) v'_j \\
f(x, \mu''_h y) = \mu''_h f(x, y), & f(x, y v''_k) = f(x, y) v''_k
\end{cases}
$$

すべての $x \in E, y \in F, \mu'_i \in B'_i, v'_j \in C'_j, \mu''_h \in B''_h, v''_k \in C''_k, i, j, h, k$ は任意です。

(b) 逆に、f を E $\times$ F から G 満たす条件 (1) (no. 1) および (8) への $\mathbf{Z}$ 双線形写像とする。次に、$x \in E, y \in F$ に対して $f(x, y) = g(x \otimes y)$ となるように、マルチモジュール G にマルチモジュール E $\otimes_A$ F の線形写像 g が 1 つだけ存在します。

主張 (a) は、E $\otimes_A$ F 上のマルチモジュール構造の定義の直後に続きます。たとえば、$(x \otimes y)v'_j = (xv'_j) \otimes y$ です。 (b) を証明するには、まず、no. 1 の命題 1 が $x \in E, y \in F$ に対して $g(x \otimes y) = f(x, y)$ となるような $\mathbf{Z}$ 線形写像 g の存在と一意性を与えることに注意します。必要なのは、マルチモジュール構造に対して g が線形であることを確認することだけです。 元 $x \otimes y$ 生成する $\mathbf{Z}$ モジュール E $\otimes_A$ F として、関係 $g(\mu'(x \otimes y)) = \mu'_i g(x \otimes y)$ とその類似物を検証するだけで十分です。しかし、これは公式 $g(x \otimes y) = f(x, y)$ と関係 (8) の直後に続きます。

#### スコリウム {#alg-ii-s3-n4-sch-1 .statement tag=05OZ}

E $\otimes_A$ F の元は、一般に形 $\sum_i (x_i \otimes y_i)$ でいくつかの方法で記述できます。ここで、$x_i \in E$ と $y_i \in F$;しかし、マルチモジュール E $\otimes_A$ F の定義する線形写像 g をマルチモジュール G に変換するには、$\sum_i (x_i \otimes y_i) = \sum_j (x'_j \otimes y'_j)$ であれば $\sum_i g(x_i \otimes y_i) = \sum_j g(x'_j \otimes y'_j)$ であることを検証する必要はありません。 $x \in E$ と $y \in F$ に対して $g(x \otimes y)$ を与え、$(x, y) \mapsto g(x \otimes y)$ が $\mathbf{Z}$ 双線形であり、条件 (1) (no. 1) と (8) を満たすことを検証するだけで十分です。

E' を ((B'_i), A, (C'_j)) マルチモジュール、F' を (A, (B''_h); (C''_k)) マルチモジュール、およびマルチモジュールの $u : E \to E', v : F \to F'$ 線形写像とします。 定義 (no. 2) の直後、$u \otimes v$ はマルチモジュール E $\otimes_A$ F の線形写像であり、マルチモジュール E' $\otimes_A$ F' になります。

E は常に右A-加群を表すため、$_sA_d$ は環 A を (A, A)-bimodule (§ 1, no. 14, 例 1) とみなします。上記により、テンソル積 E $\otimes_A (_sA_d)$ は、$x \in E, \lambda \in A, \mu \in A$ に対して $(x \otimes \lambda)\mu = x \otimes (\lambda \mu)$ となるような正規の右A-加群構造を持ちます。 E $\times (_sA_d)$ の E への写像 $(x, \lambda) \mapsto x \lambda$ は $\mathbf{Z}$ 双線形であり、条件 (1) (no. 1) と (8) を満たします (後者では、$B'_i, C'_j$ と $B''_h$ が欠落しており、家族 $(C''_k)$ 簡約するから $A$);したがって (命題 3)、$x \in E, \lambda \in A$ に対して $g(x \otimes \lambda) = x\lambda$ となるような、$E \otimes_A (sA_d)$ から $E$ への$A$ 線形写像 $g$ (正規と呼ばれます) が存在します。

#### 命題 4 {#alg-ii-s3-prop-4 .statement tag=05P0}

*$E$ が右 $A$ 加群の場合、$E$ の $E \otimes_A (sA_d)$ への写像 $h : x \mapsto x \otimes 1$ は右 $A$ 加群同型であり、その逆同型 $g$ は $x \in E, \lambda \in A$ に対して $g(x \otimes \lambda) = x\lambda$ となる。

$g$ が標準写像の場合、$g \circ h$ は恒等写像 $1_E$ および $h \circ g$ 一致するで、$E \otimes_A (sA_d)$ の恒等写像が形 $x \otimes y$ の元になります。 生成する後者の$\mathbf{Z}$ モジュール。したがって結論です。

通常、$E \otimes_A (sA_d)$ の代わりに $E \otimes_A A$ と書き、上記の標準同型を使って $E$ を使って同一視する $E \otimes_A A$ と書くことがよくあります。 $E$ がその右側の $A$ モジュール構造と互換性のある (左または右の) $B$ モジュール構造も持っている場合、$g$ と $h$ は $E$ と $E \otimes_A A$ の $B$ モジュール構造の同型であることに注意してください。したがってマルチノード加群同型)。

ここで、$F$ を左側の $A$ モジュールとしましょう。 $(sA_d) \otimes_A F$ ($A \otimes_A F$ とも表される) は、正規の左 $A$ モジュール構造を持ち、命題 4 標準同型は、$A \otimes_A F$ から $F$ 写像 $\lambda \otimes x$ から $\lambda x$ に定義され、その逆同型は$x \mapsto 1 \otimes x$です。

特に、写像 $\lambda \otimes \mu$ から $\lambda \mu$ に$sA_d$ 上に$(A, A)$ バイモジュール$(sA_d) \otimes_A (sA_d)$ の標準同型が存在します。

### 5. テンソル積/2 加群可換環

$C$ を *可換* 環とします。すべての $C$ モジュール $E$、$E$ の加群構造は *それ自体と互換性* (§ 1, no. 14) があります。 $E$ と $F$ が 2 つの $C$ モジュールである場合、no. 4 を考慮すると、テンソル積 $E \otimes_C F$ 上に、それぞれ $\gamma(x \otimes y) = (\gamma x) \otimes y$ と $\gamma(x \otimes y) = x \otimes (\gamma y)$ となる *2 つの $C$ モジュール構造を定義できます。しかし、no. 1 の定義 1 によれば、この場合は $(\gamma x) \otimes y = x \otimes (\gamma y)$ なので、これら 2 つの構造は *同じ* です。 今後、$E \otimes_C F$ を $C$-*加群* として話すときは、このように定義された構造を意味し、そうでない場合は 〜でない限りを意味します。 標準同型。

$$
\sigma : F \otimes_C E \to E \otimes_C F
$$

(no. 1、系 2 ～ 命題 1) は、$C$ モジュール同型になります。

この定義から、$(a_\lambda)_{\lambda \in L}$ (それぞれ $(b_\mu)_{\mu \in M}$) が $C$ モジュール $E$ (それぞれ $F$) の *生成する系* である場合、$(a_\lambda \otimes b_\mu)$ は *生成するであることがわかります。 $C$ モジュール $E \otimes_C F$ の系*;特に、$E$ と $F$ が *有限生成* $C$ モジュールである場合、$E \otimes_C F$ も同様です。

For every $C$-module $G$, the $\mathbf{Z}$-bilinear mappings $f$ of $E \times F$ into $G$ for which

$$
f(\gamma x, y) = f(x, \gamma y) = \gamma f(x, y) \quad \text{for } x \in E, y \in F, \gamma \in C
$$

それらは、C-双線形と呼ばれ、形は、$\mathscr{L}_2(E, F; G)$で示されるC-モジュールと呼ばれます。 命題 3 (no. 4) 定義する正規の C モジュール同型 (cf. § 1, no. 14、注意 1)。

$$
\mathscr{L}_2(E, F; G) \to \mathrm{Hom}_C(E \otimes_C F, G).
$$

E'、F' を 2 つの C モジュールと 2 つの $u : E \to E'$、$v : F \to F'$ の C 線形マッピングとします。 (no. 4) $u \otimes v$ は、$E \otimes_C F$ から $E' \otimes_C F'$ への C 線形写像です。さらに、$(u, v) \mapsto u \otimes v$ が $\mathrm{Hom}_C(E, E') \times \mathrm{Hom}_C(F, F')$ から $\mathrm{Hom}_C(E \otimes_C F, E' \otimes_C F')$ への C 双線形写像であるのは明らかです。したがって、これに対して正規の対応するが存在し、正規と呼ばれる C 線形マッピングが存在します。

$$
\mathrm{Hom}_C(E, E') \otimes_C \mathrm{Hom}_C(F, F') \to \mathrm{Hom}_C(E \otimes_C F, E' \otimes_C F')
$$

テンソル積のすべての元 $u \otimes v$ に関連付けられます

$$
\mathrm{Hom}_C(E, E') \otimes_C \mathrm{Hom}_C(F, F')
$$

線形写像 $u \otimes v$。 標準写像 (11) *必ずしも単射でも全射でもない* (§ 4, 練習問題 2) ことに注意してください。

#### 注意 {#alg-ii-s3-n5-rem-1 .statement tag=05P1}

(1) A、B を 2 つ可換環、$\rho : B \to A$ 環準同型、E と F を 2 つ A-加群とします。すると、no. 3 の標準写像 (6) は B-線型写像になります

$$
\rho_*(E) \otimes \rho_*(F) \to \rho_*(E \otimes_A F).
$$

(2) このNo.で述べられていること。は次の場合に一般化できます: E を C の右A-加群、F 左A-加群、C 可換環および $\rho : C \to A$ 準同型を A に変換し、$\rho(C)$ が A の中心に含まれるようにします (cf. III, § 1, no. 3)。 次に、$\rho$ の C モジュール $\rho_*(E)$ と $\rho_*(F)$ および仮定は、これらの C モジュール構造がそれぞれ E および F (§ 1, no. 14) の A-加群構造と互換性があることを意味すると考えます。 The tensor product $E \otimes_A F$ is thus (by virtue of no. 4) given two C-module structures such that $\gamma(x \otimes y) = (x \rho(\gamma)) \otimes y$ and

$$
\gamma(x \otimes y) = x \otimes (\rho(\gamma)y)
$$

それぞれ $\gamma \in C$、$x \in E$、$y \in F$、定義 1 (no. 1) は、これら 2 つの構造が同一であることも示します。 E' (または F') が右 (または左) A-加群であり、$u : E \to E'$、$v : F \to F'$ が 2 つの A-線型写像である場合、$u \otimes v : E \otimes_A F \to E' \otimes_A F'$ は、定義したばかりの C モジュール構造に対して C 線形です。 写像 $(u, v) \mapsto u \otimes v$:

$$
\mathrm{Hom}_A(E, E') \times \mathrm{Hom}_A(F, F') \to \mathrm{Hom}_C(E \otimes_A F, E' \otimes_A F')
$$

は § 1, no. 14、*注意* 1)、よってで定義された C-双線形 ($\mathrm{Hom}_A(E, E')$ および $\mathrm{Hom}_A(F, F')$ の C モジュール構造の場合)、*正準* と呼ばれる *C-線形* 写像も導出します。

(13) $\operatorname{Hom}_A(E, E') \otimes_C \operatorname{Hom}_A(F, F') \to \operatorname{Hom}_C(E \otimes_A F, E' \otimes_A F')$。

(3) A を整域とし、K を分数の体とします。 E と F が 2 つのベクトル K スペースである場合、標準写像

$$
(E_{[A]}) \otimes_A (F_{[A]}) \to E \otimes_K F
$$

(no. 3 と § 1, no. 13) は *全客観* です。 $f$ が $E \times F$ のベクトル K 空間 G への *A 双線形* 写像である場合、$f$ も *K 双線形* であることを証明するだけで十分です (no. 4)。さて、Aの$\alpha \neq 0$すべてです。

$$
\alpha f(\alpha^{-1}x, y) = f(x, y) = \alpha f(x, \alpha^{-1}y)
$$
よって
$$
f(\alpha^{-1}x, y) = f(x, \alpha^{-1}y) = \alpha^{-1}f(x, y)
$$
G はベクトル K 空間であるため。

### 6. 完全系列に対する$E \otimes_A F$の特性

#### 命題 5 {#alg-ii-s3-prop-5 .statement tag=05P2}

*E、E'、E''を*右*、A-*加群*、Fを*左*、A-*加群*とします

(14)

$$
E' \xrightarrow{u} E \xrightarrow{v} E'' \to 0
$$

*完全系列/線形写像.* *書き込み* $\bar{u} = u \otimes 1_F, \bar{v} = v \otimes 1_F,$ *数列*

(15)

$$
E' \otimes_A F \xrightarrow{\bar{u}} E \otimes_A F \xrightarrow{\bar{v}} E'' \otimes_A F \to 0
$$

*of* $\mathbf{Z}$-*準同型* *は正確です*。

By virtue of no. 2, formula (5), $\bar{v} \circ \bar{u} = (v \circ u) \otimes 1_F = 0$; the image $H = \bar{u}(E' \otimes F)$ is contained in the kernel $L = \operatorname{Ker}(\bar{v})$; by passing to the quotient, we therefore derive from $\bar{v}$ a $\mathbf{Z}$-linear mapping $f$ of the cokernel $M = (E \otimes F)/H$ of $\bar{u}$ into $E'' \otimes F$; it must be proved that $f$ is *bijective* and it will hence suffice to define a $\mathbf{Z}$-linear mapping $g : E'' \otimes F \to M$ such that $g \circ f$ and $f \circ g$ are the identity mappings.

$x'' \in E''$、$y \in F$ としましょう。 仮定までに、$v(x) = x''$となるような$x \in E$が存在します。 $x_1, x_2$ が E の 2 つの元で、$v(x_1) = v(x_2) = x''$ と $\phi : E \otimes F \to M$ が標準写像である場合、$\phi(x_1 \otimes y) = \phi(x_2 \otimes y)$ であることを示します。 $v(x) = 0$ の場合、$\phi(x \otimes y) = 0$ であることを証明すれば十分です。これは、$x = u(x')$ と $x' \in E'$、よって $x \otimes y = u(x') \otimes y = \bar{u}(x' \otimes y) \in H$ という事実から続きます。 $(x'', y)$ が、$v(x) = x''$ のように、すべての $x \in E$ の$\phi(x \otimes y)$ の一意の値にマッピングされる場合、$E'' \times F$ の写像が M に定義されます。この写像は $\mathbf{Z}$ 双線形であり、$x \in E$ に対する $v(x \lambda) = x'' \lambda$ と $(x \lambda) \otimes y = x \otimes (\lambda y)$ から、条件 (1) (no. 1) を満たします。したがって、$y \in F, x \in E$ と $x'' = v(x)$ に対して $g(x'' \otimes y) = \phi(x \otimes y)$ となるような、$E'' \otimes F$ の M への$\mathbf{Z}$ 線形マッピング $g$ が存在します。この定義は、 $f \circ g$ 一致すると恒等写像の元をさらに証明します。

形 $x'' \otimes y$ の $E'' \otimes F$ したがって、$f \circ g$ は $E'' \otimes F$ の恒等写像です。一方、$x \in E$と$y \in F$では、定義により$f(\phi(x \otimes y)) = v(x) \otimes y$、したがって$g(f(\phi(x \otimes y))) = \phi(x \otimes y)$となり、形$\phi(x \otimes y)$生成するMの元として、$g \circ f$はMの恒等写像になります。

#### 系 {#alg-ii-s3-n6-cor-1 .statement tag=05P3}

*F、F'、F'' を左A-加群、E 右A-加群とし、*
$$
\begin{array}{ccccc}
F' & \xrightarrow{s} & F & \xrightarrow{t} & F'' \longrightarrow 0
\end{array}
$$
*(16)*
*線形写像の完全系列。 \bar{s} = l_E \otimes s、\bar{t} = l_E \otimes t、\mathbf{Z}-準同型写像の数列* を書く
$$
\begin{array}{cccccc}
E \otimes_A F' & \xrightarrow{\bar{s}} & E \otimes_A F & \xrightarrow{\bar{t}} & E \otimes_A F'' & \longrightarrow 0
\end{array}
$$
*(17)*
*正確です。*

E (それぞれ F) が左 (それぞれ右) A^0 モジュールとみなされる場合、F \otimes_{A^0} E は E \otimes_A F と識別され、F' \otimes_{A^0} E と F'' \otimes_{A^0} E (no. 1, 系 2 から命題 1) にも同様の識別があります。 命題 5 の直後に系が続きます。

#### 注意 {#alg-ii-s3-n6-rem-1 .statement tag=05P4}

一般に、E' が右A-加群 E の部分加群で、 j : E' \to E 標準単射, 標準写像であることに注意してください。
$$
j \otimes 1_F : E' \otimes F \to E \otimes F
$$
*必ずしも単射であるとは限りません* 他の語では、完全系列について
$$
\begin{array}{ccccccc}
0 & \longrightarrow & E' & \xrightarrow{u} & E & \xrightarrow{v} & E'' \longrightarrow 0
\end{array}
$$
*(18)*
一般にできないは数列と結論づけられます
$$
\begin{array}{ccccccc}
0 & \longrightarrow & E' \otimes F & \xrightarrow{u} & E \otimes F & \xrightarrow{v} & E'' \otimes F \longrightarrow 0
\end{array}
$$
*(19)*
*正確です。*

たとえば、A = \mathbf{Z}、E = \mathbf{Z}、E' = 2\mathbf{Z}、F = \mathbf{Z}/2\mathbf{Z} とします。 E' は E と同型であるため、E' \otimes F は E \otimes F と同型であり、それ自体は F (no. 4, 命題 4) と同型です。ただし、すべての x' = 2x \in E' (x \in E) とすべての y \in F については、2y = 0 であるため、j(x') \otimes y = (2x) \otimes y = x \otimes (2y) = 0 となり、E \otimes F 簡約するの E' \otimes F の標準像は 0 になります。

他の語では、部分加群 E' of E と元 x \in E' について、元 x \otimes y 「E' \otimes F' で計算」と元 x \otimes y 「E \otimes F で計算」（他の語では、 元 j(x) \otimes y)。

後で、フラット加群, 加群 F という名前で、数列 (19) がすべての完全系列 (18) (*可換代数*, I, § 2) と正確になるように学習します。

#### 命題 6 {#alg-ii-s3-prop-6 .statement tag=05P5}

*2 つの完全系列 (14) と (16) が与えられると、準同型 v \otimes t : E \otimes_A F \to E'' \otimes_A F'' は全射であり、その核は次と等しい*
$$
\operatorname{Im}(u \otimes 1_F) + \operatorname{Im}(l_E \otimes s)
$$

したがって、$v \otimes t = (v \otimes 1_{F''}) \circ (1_E \otimes t)$ (no. 2, 公式 (5)) と $v \otimes t$ は、命題 5 とその系により、2 つの全射準同型の合成になります。 一方、$z \in E \otimes F$ が $v \otimes t$ の核にあるためには、 $(1_E \otimes t)(z)$ 属するから $v \otimes 1_{F''}$ の核、つまり (15) から像のおかげで必要十分です。

$$
u \otimes 1_{F''}: E' \otimes F'' \to E \otimes F''.
$$

しかし、準同型 $t: F \to F''$ が全射であるように、

$$
1_{E'} \otimes t: E' \otimes F \to E' \otimes F''
$$

系から命題 5 まで、したがって $z$ 簡約するの条件により、次のような $a \in E' \otimes F$ が存在します。

$$
(l_E \otimes t)(z) = (u \otimes t)(a).
$$

$b = z - (u \otimes 1_F)(a)$ にしましょう。次に、$(l_E \otimes t)(b) = 0$、(17) により、$l_E \otimes s$ の $b$ 属するから像となり、命題が証明されます。

その他語:

#### 系 1 {#alg-ii-s3-prop-6-cor-1 .statement tag=05P6}

*$E'$を右側の$A$モジュール$E$のサブモジュール、$F'$を左側の$A$モジュールのサブモジュール$F$、$\operatorname{Im}(E' \otimes_A F)$、$\operatorname{Im}(E \otimes_A F')$を$E \otimes_A F$のサブ$\mathbf{Z}$モジュールとします。それぞれの画像正規マッピング $E' \otimes_A F \to E \otimes_A F$ の、

$$
E \otimes_A F' \to E \otimes_A F.
$$

次に、標準的 $\mathbf{Z}$-モジュール同型* があります。

$$(20)\quad \pi : (E/E') \otimes_A (F/F') \to (E \otimes_A F)/(\operatorname{Im}(E' \otimes_A F) + \operatorname{Im}(E \otimes_A F'))$$

*$\xi \in E/E'$、$\eta \in F$、$\pi(\xi \otimes \eta)$ は、元 $x \otimes y \in E \otimes_A F$ のうちの類となり、$x \in \xi$ と $y \in \eta$ になります。

$E$ が $((B'_i); A, (C'_j))$ マルチモジュール、$F$ が $(A, (B''_h); (C''_k))$ マルチモジュール、および $E$ と $F$ の $E'$ と $F'$ *サブマルチモジュール* の場合、同型 (20) は同型であることに注意してください。 $((B'_i), (B''_h); (C'_j), (C''_k))$-マルチモジュール構造の両側 (no. 3)。

#### 系 2 {#alg-ii-s3-prop-6-cor-2 .statement tag=05P7}

*$a$を$A$の右側の理想、$F$を左側の$A$モジュール、$aF$を形$\lambda x$の元によって生成された$F$のサブ$\mathbf{Z}$モジュールとします。ここで、$\lambda \in a$と$x \in F$。次に、標準的 $\mathbf{Z}$ モジュール同型* があります。

$$(21)\quad \pi : (A/a) \otimes_A F \to F/aF$$

*すべての $\bar{\lambda} \in A/a$ とすべての $x \in F$ に対して、$\pi(\bar{\lambda} \otimes x)$ は類 mod となります。 $\lambda x$の$aF$、$\lambda \in \bar{\lambda}$。

特に、$A = \mathbf{Z}$ については、すべての整数 $n$ およびすべての $\mathbf{Z}$ モジュール $F$ について、$(\mathbf{Z}/n\mathbf{Z}) \otimes_{\mathbf{Z}} F$ は商 $\mathbf{Z}$ モジュール $F/nF$ と正規に識別されることがわかります。

#### 系 3 {#alg-ii-s3-prop-6-cor-3 .statement tag=05P8}

$A$を可換環、$a$を$A$と$E$、$F$の2つの$A$モジュールの理想とし、$a$が$F$の消滅子に含まれるようにします。この場合、$(A/a)$ モジュール $E \otimes_A F$ と $(E/aE) \otimes_{A/a} F$ は標準的に同型です。

$F$ と $E \otimes_A F$ は $a$ によって消滅するため、標準的な $(A/a)$ モジュール構造 ($§ 1$、no. 12) があり、$E' = aE$ と書くと、$\operatorname{Im}(E' \otimes_A F) = 0$ になります。次に、$E \otimes_A F$ の標準同型 (20) が $(E/aE) \otimes_A F$ 上にあり、後者自体は $(E/aE) \otimes_{A/a} F$ (no. 3、系から命題 2) と同一です。

#### 系 4 {#alg-ii-s3-prop-6-cor-4 .statement tag=05P9}

$a, b$ を可換環 $C$ の 2 つの理想とする。 $C$ モジュール $(C/a) \otimes_C (C/b)$ は、正規的に $C(a + b)$ と同型です。

### 7. 積と直和のテンソル積

$(E_\lambda)_{\lambda \in L}$ を右側の $A$ モジュールのファミリー、$(F_\mu)_{\mu \in M}$ を左側の $A$ モジュールのファミリーとし、積加群 $C = \prod_{\lambda \in L} E_\lambda, D = \prod_{\mu \in M} F_\mu$ を考えます。 写像 $C \times D$ の $((x_\lambda), (y_\mu)) \mapsto (x_\lambda \otimes y_\mu)$ を積 $\mathbf{Z}$ モジュールに
$$
\prod_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_A F_\mu)
$$
は$\mathbf{Z}$-双線形であり、明らかに条件 (1) (no. 1) を満たします。したがって、正規と呼ばれる (no. 1, 命題 1) $\mathbf{Z}$ 線形マッピングが存在します。
$$
f : \left( \prod_{\lambda \in L} E_\lambda \right) \otimes_A \left( \prod_{\mu \in M} F_\mu \right) \to \prod_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_A F_\mu)
$$
$f((x_\lambda) \otimes (y_\mu)) = (x_\lambda \otimes y_\mu)$ のようになります。

$C = R^L, D = S^M, R$ (それぞれ $S$) が右 (または左) $A$ モジュールである場合、標準写像 (22) はすべてのテンソル積 $u \otimes v$ に関連付けられます。ここで、$u$ は $L$ の写像から $R$ になり、 $v$ $M$ の写像を $S$ に、写像 $(\lambda, \mu) \mapsto u(\lambda) \otimes v(\mu)$ を $L \times M$ から $R \otimes_A S$ に。この場合でも、標準写像 (22) は一般に単射でも全射でもない (練習問題 3; cf. 系 3 ～ 命題 7)。

$E_\lambda$ が $((B'_i); A, (C'_j))$ マルチモジュール、$F_\mu$ $(A, (B''_h); (C''_{k_c}))$ マルチモジュールの場合、準同型 (22) は両側の $((B'_i), (B''_h); (C'_j), (C''_{k_c}))$ マルチモジュール構造に対しても準同型になります。

ここで、部分加群 $E = \bigoplus_{\lambda \in L} E_\lambda$ (それぞれ $\bigoplus_{\mu \in M} F_\mu$) または $C$ (それぞれ $D$) を考えてみましょう。 標準単射 $E \to C, F \to D$ 定義するは、標準的に $\mathbf{Z}$ 線形写像 $E \otimes_A F \to C \otimes_A D$ を写像 (22) と合成すると、$E \otimes_A F$ から $\prod_{\lambda, \mu} (E_\lambda \otimes_A F_\mu)$ への $\mathbf{Z}$ 線形写像 $g$ が得られます。
$$
g((x_\lambda) \otimes (y_\mu)) = (x_\lambda \otimes y_\mu);
$$

さらに、ファミリー $(x_\lambda)$ と $(y_\mu)$ には有限台があるため、$(x_\lambda \otimes y_\mu)$ もあり、したがって最終的に $g$ は標準準同型になります

$$
g : \left( \bigoplus_{\lambda \in L} E_\lambda \right) \otimes_A \left( \bigoplus_{\mu \in M} F_\mu \right) \to \bigoplus_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_A F_\mu),
$$

これは、(22) と同じ条件の下にあるマルチモジュール準同型です。

#### 命題 7 {#alg-ii-s3-prop-7 .statement tag=05PA}

*標準写像 (23) は全単射です。*

これを証明するには、$g \circ h$ と $h \circ g$ が恒等写像となるように、直和 $G = \bigoplus_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_A F_\mu)$ の $\mathbf{Z}$ 線形写像 $h$ を $E \otimes_A F$ に定義する行うだけで十分です。 しかし、$G$ から $E \otimes_A F$ への $\mathbf{Z}$ 線形写像を定義するには、$\mathbf{Z}$ 線形写像を定義するだけで十分です (§ 1, no. 6、命題 6)。

$$
h_{\lambda \mu} : E_\lambda \otimes_A F_\mu \to E \otimes_A F
$$

注文されたすべての対 $(\lambda, \mu)$ に対して、$h_{\lambda \mu} = i_\lambda \otimes j_\mu$ を取得します。ここで、$i_\lambda : E_\lambda \to E$ と $j_\mu : F_\mu \to F$ は標準単射です。 次に、$h \circ g$ は、$\mathbf{Z}$ モジュール $E \otimes_A F$ を生成する形式 $\left( \sum_\lambda x_\lambda \right) \otimes \left( \sum_\mu y_\mu \right)$ の要素の識別マッピングと明らかに一致します。同様に、$g \circ h$ は、$\mathbf{Z}$ モジュール $G$ を生成する形式 $\sum_{\lambda, \mu} (x_\lambda \otimes y_\mu)$ の要素の恒等マッピングと一致します。なぜなら、各順序ペア $(\lambda, \mu)$ の積が

$$
x_\lambda \otimes y_\mu \quad (x_\lambda \in E_\lambda, y_\mu \in F_\mu)
$$

生成する $\mathbf{Z}$ モジュール $E_\lambda \otimes_A F_\mu$。 よって命題。

$u_\lambda : E_\lambda \to E'_\lambda$、$v_\mu : F_\mu \to F'_\mu$ を $A$ 準同型射とします。明らかに図式

$$
\begin{array}{ccc}
\left( \bigoplus_\lambda E_\lambda \right) \otimes_A \left( \bigoplus_\mu F_\mu \right) & \longrightarrow & \bigoplus_{\lambda, \mu} (E_\lambda \otimes_A (F_\mu)) \\
(\bigoplus u_\lambda) \otimes (\bigoplus v_\mu) \downarrow & & \downarrow (\bigoplus (u_\lambda \otimes v_\mu)) \\
\left( \bigoplus_\lambda E'_\lambda \right) \otimes_A \left( \bigoplus_\mu F'_\mu \right) & \longrightarrow & \bigoplus_{\lambda, \mu} (E'_\lambda \otimes_A F'_\mu)
\end{array}
$$

可換です。

#### 系 1 {#alg-ii-s3-prop-7-cor-1 .statement tag=05PB}

*左の $A$ モジュール $F$ が基底 $(b_\mu)_{\mu \in M}$ を認める場合、$E \otimes_A F$ のすべての元は形 $\sum_\mu (x_\mu \otimes b_\mu)$ で一意に書くことができます。ここで、$x_\mu \in E$ とそのファミリー $(x_\mu)$ は、 有限台。 $\mathbf{Z}$ モジュール $E \otimes_A F$ は、$\mathbf{Z}$ モジュールと見なされる $E^{(M)}$ と同型です。*

基底 $(b_\mu)$ 定義する $F$ の同型を$\bigoplus_{\mu \in M} Ab_\mu$、よってに加えると、命題 7 のおかげで同型 $E \otimes_A F \to \bigoplus_{\mu \in M} (E \otimes_A Ab_\mu)$ があります。 ξ ↦ ξb_μ は Ab_μ 上の A_s の同型であるため、x ↦ x ⊗ b_μ は、no. 4 の命題 4、よって系により、E ⊗_A (Ab_μ) 上の E の同型です。

E が ((B'_i); A, (C'_j))-マルチモジュールの場合、標準同型 E ⊗_A F → E^{(M)} は ((B'_i); (C'_j))-マルチモジュール同型です。

特に、E も基底 (a_λ)_{λ ∈ L} を認める場合、すべての z ∈ E ⊗_A F は形 $\sum_{\lambda, \mu} (a_\lambda \xi_{\lambda\mu}) \otimes b_\mu$ で唯一一方向に記述できます。ここで、ξ_{λμ} 属するは A (および形有限台の家族)。 写像 $z \mapsto (\xi_{\lambda\mu})_{(\lambda, \mu) \in L \times M}$ は、\mathbf{Z} モジュール構造の A^{(L × M)} 上の E ⊗_A F の同型です (さらに、A の中心上の加群構造も)。より具体的には:

#### 系 2 {#alg-ii-s3-prop-7-cor-2 .statement tag=05PC}

*E と F が 2 つの自由加群可換環 C で、(a_λ) (それぞれ (b_μ)) が C モジュール E (それぞれ F) の基底である場合、(a_λ ⊗ b_μ) はモジュールの基底になります。 C-モジュール E ⊗_C F.*

言葉の乱用により、基底 (a_λ ⊗ b_μ) は、ときどきが基底 (a_λ) と (b_μ) の *テンソル積* と呼ばれます。

*注意 (1)*。 E を自由右A-加群、F を自由左A-加群、E の (a_λ)_{λ ∈ L} 基底および F の (b_μ)_{μ ∈ M} 基底とする。すべての元 z ∈ E ⊗_A Fは、y_λ ∈ F である $\sum_\lambda a_\lambda \otimes y_\lambda$ として一意に書くことができ、また、x_μ ∈ E である $\sum_\mu x_\mu \otimes b_\mu$ としても一意に書くことができます。 $y_\lambda = \sum_\mu \eta_{\lambda\mu} b_\mu$、$x_\mu = \sum_\lambda a_\lambda \xi_{\lambda\mu}$ (ξ_{λμ} と η_{λμ} 属するを A に書くと、$\xi_{\lambda\mu} = \eta_{\lambda\mu}$)すべて (λ, μ)、for

$$
\sum_\lambda \left( a_\lambda \otimes \left( \sum_\mu \eta_{\lambda\mu} b_\mu \right) \right) = \sum_{\lambda, \mu} ((a_\lambda \eta_{\lambda\mu}) \otimes b_\mu) = \sum_\mu \left( \left( \sum_\lambda a_\lambda \eta_{\lambda\mu} \right) \otimes b_\mu \right).
$$

#### 系 3 {#alg-ii-s3-prop-7-cor-3 .statement tag=05PD}

* (E_λ)_{λ ∈ L} を右A-加群の族とし、F を自由 (それぞれ有限に生成された自由) 左A-加群とします。それから標準写像 (22)

$$
\left( \prod_{\lambda \in L} E_\lambda \right) \otimes_A F \to \prod_{\lambda \in L} (E_\lambda \otimes_A F)
$$

は単射（それぞれ全単射）です。

(b_μ) が F の基底である場合、$\left( \prod_{\lambda \in L} E_\lambda \right) \otimes_A F$ のすべての元は $z = \sum_\mu ((x_\lambda^{(\mu)}) \otimes b_\mu)$ (系 1) として一意に書くことができます。その標準像が零であるということは、すべての λ ∈ L に対して $\sum_\mu (x_\lambda^{(\mu)} \otimes b_\mu) = 0$、したがってすべての λ ∈ L とすべての μ (系 1) に対して $x_\lambda^{(\mu)} = 0$、したがって $z = 0$ であることを意味します。

F が有限基底を認めるとき、標準写像が全単射であることを示すと、命題 7 によって次の場合に直ちに還元されます。

F = A_s;しかし、その後、両側は $\prod_{\lambda \in L} E_\lambda$ (no. 4, 命題 4) で標準的に識別され、 後でこれらの識別標準写像 (22) が識別になります。

#### 系 4 {#alg-ii-s3-prop-7-cor-4 .statement tag=05PE}

*A を環とし、零の因子を持たず、E を自由な右A-加群、F を自由な左A-加群とします。この場合、E $\otimes_A$ F の関係 x $\otimes$ y = 0 は、x = 0 または y = 0 を意味します。*

$(a_\lambda)$ を E の基底、F の $(b_\mu)$ 基底、そして $x = \sum_\lambda a_\lambda \xi_\lambda, y = \sum_\mu \eta_\mu b_\mu$ とします。この場合、$x \otimes y = \sum_{\lambda, \mu} ((a_\lambda \xi_\lambda \eta_\mu) \otimes b_\mu$ および関係 $x \otimes y = 0$ は、添字 $(\lambda, \mu)$ (系 1) のすべての注文された対に対して $\xi_\lambda \eta_\mu = 0$ を意味します。したがって、$x \neq 0$、つまり少なくとも 1 つの $\lambda$ について $\xi_\lambda \neq 0$ の場合、すべての $\mu$、よって $y = 0$ について $\eta_\mu = 0$ ということになります。

#### 系 5 {#alg-ii-s3-prop-7-cor-5 .statement tag=05PF}

*E を右A-加群、F 左A-加群、E の M 部分加群、F の N 部分加群とします。M が E の直因子と F の N 直因子である場合、標準準同型 $M \otimes_A N \to E \otimes_A F$ は単射であり、この準同型の下にある $M \otimes_A N$ の像は、$\mathbf{Z}$ モジュール $E \otimes_A F$ の直因子です。

これは命題 7 の直後に続きます。

E が $((B'_i); A, (C'_j))$ マルチモジュール、F が $(A, (B''_h); (C''_k))$ マルチモジュール、M と N が直因子の場合、$M \otimes N$ は $((B'_i), (B''_h); (C'_j), (C''_k))$ マルチモジュール $E \otimes F$ の直因子であることに注意してください。

#### 系 6 {#alg-ii-s3-prop-7-cor-6 .statement tag=05PG}

*P を射影左A-加群とし、E、F を 2 つ右A-加群とします。 単射準同型 $u : E \to F$、準同型*ごとに
$$
u \otimes 1_P : E \otimes_A P \to F \otimes_A P
$$
*は単射です。*

$L = P \oplus Q$ が自由 (§ 2, no. 2、命題 4) であり、$u \otimes 1_L$ が識別される (命題 7) というような左A-加群 Q が存在します。
$$(u \otimes 1_P) \oplus (u \otimes 1_Q);$$
したがって、P が *free* (§ 1, no. 6, 系 1 ～ 命題 7) のとき、系を証明するだけで十分です。 no. 4、命題の直後に続く$P = A_s$の場合に対する同じ議論簡約する問題。

#### 系 7 {#alg-ii-s3-prop-7-cor-7 .statement tag=05PH}

※Cを可換環とします。 E と F が 2 つの射影 C 加群の場合、$E \otimes_C F$ は射影 C 加群です。*

これは、系 5 と、2 つの空き C モジュールのうちのテンソル積が空き C モジュール (系 2) であるという事実からすぐに続きます。

#### 注意 2 {#alg-ii-s3-n7-rem-2 .statement tag=05PI}

命題 7 の仮説の下で、$E'_\lambda$ を $E_\lambda$ の部分加群、$F_\mu$ の $F'_\mu$ 部分加群とし、$E' = \bigoplus_{\lambda \in L} E'_\lambda$、$F' = \bigoplus_{\mu \in M} F'_\mu$ とします。 Im$(E' \otimes_A F')$ (それぞれ Im(E'_λ ⊗_A F'_μ)) が、標準写像の下での E ⊗_A F (それぞれ E_λ ⊗_A F_μ) における E' ⊗_A F' (それぞれ E'_λ ⊗_A F'_μ) の像を表すものとします。次に、同型 (23) はサブ$\mathbf{Z}$ モジュールを識別します

$$
\operatorname{Im}(E' \otimes_A F') \quad \text{and} \quad \bigoplus_{(\lambda, \mu) \in I \times M} \operatorname{Im}(E'_\lambda \otimes_A F'_\mu);
$$

これは図式の可換性の直後に続きます

$$
\begin{array}{ccc}
\left( \bigoplus_\lambda E'_\lambda \right) \otimes_A \left( \bigoplus_\mu F'_\mu \right) & \longrightarrow & \left( \bigoplus_\lambda E_\lambda \right) \otimes_A \left( \bigoplus_\mu F_\mu \right) \\
\downarrow & & \downarrow \\
\bigoplus_{\lambda, \mu} (E'_\lambda \otimes_A F'_\mu) & \longrightarrow & \bigoplus_{\lambda, \mu} (E_\lambda \otimes_A F_\mu)
\end{array}
$$

ここで、垂直矢印は標準同型です。

### 8. テンソル積の結合性

#### 命題 8 {#alg-ii-s3-prop-8 .statement tag=05PJ}

*A、B を 2 つの環、E 右A-加群、F を (A, B) バイモジュール、G 左B-加群とします。この場合、E ⊗_A F は右B-加群、F ⊗_B G 左A-加群となり、唯一の $\mathbf{Z}$ 線形写像* が存在します。

$$
\phi : (E \otimes_A F) \otimes_B G \to E \otimes_A (F \otimes_B G)
$$

*そのような* $\phi((x \otimes y) \otimes z) = x \otimes (y \otimes z)$ *$x \in E,\ y \in F,\ z \in G;$ に対して* さらに、 *この $\mathbf{Z}$ 線形写像は全単射* (テンソル積の「結合性」) です。

E ⊗_A F の右B-加群構造と F ⊗_B G の左A-加群構造は、no. 4 で定義されています。 $\phi$ の一意性は、元 $(x \otimes y) \otimes z$ 生成するの $\mathbf{Z}$ モジュール $(E \otimes_A F) \otimes_B G$ であるため、明らかです。 $\phi$ の存在を示すために、すべての $z \in G,\ h_z : y \mapsto y \otimes z$ が左A-加群 F の A-線型写像から左A-加群 F ⊗_BG になることに注意します。 $g_z = 1_E \otimes h_z$ と書きます。したがって、これは E ⊗_A F の E への $\mathbf{Z}$ 線形写像です。 ⊗_A (F ⊗_B G) を考え、写像 $(t, z) \mapsto g_z(t)$ を $(E \otimes_A F \times G$ から $E \otimes_A (F \otimes_B G)$ まで考えます。 $z \in G,\ z' \in G$に対する$h_{z + z'} = h_z + h_{z'}$のように、上の写像が$\mathbf{Z}$双線形であることは明らかです。さらに、すべての $\mu \in B,\ g_{\mu z}(t) = g_z(t \mu)$ について次のことを示します。 $x \in E$ と $y \in F$ の $t = x \otimes y$ に対してこれを行うだけで十分であることは明らかです。今そして

$$
g_{\mu z}(x \otimes y) = x \otimes (y \otimes \mu z)
$$
$$
g_z((x \otimes y)\mu) = g_z(x \otimes y\mu) = x \otimes (y\mu \otimes z).
$$

命題 1 (no. 1) は、$\mathbf{Z}$ 線形写像の存在を証明します。

$$
\phi : (E \otimes_A F) \otimes_B G \to E \otimes_A (F \otimes_B G)
$$

$\phi(t \otimes z) = g_z(t)$ なので、$\phi((x \otimes y) \otimes z) = x \otimes (y \otimes z)$ となります。同様に、$\mathbf{Z}$-線形マッピング

$$
\psi : E \otimes_A (F \otimes_B G) \to (E \otimes_A F) \otimes_B G
$$

$\psi(x \otimes (y \otimes z)) = (x \otimes y) \otimes z$ と明らかに $\psi \circ \phi$ と $\phi \circ \psi$ は、それぞれ $(E \otimes_A F) \otimes_B G$ と $E \otimes_A (F \otimes_B G)$ の恒等写像であるように定義されます。これらの生成する系では簡約するから恒等写像であるためです。 $\mathbf{Z}$-モジュール。

$E$ が $((C'_i); A, (D'_j))$ マルチモジュール、$F$ が $(A, (C''_h); B, (D''_k))$ マルチモジュール、$G$ が $(B, (C'''_l); (D'''_m))$ マルチモジュールである場合、命題 8 で定義された標準同型が $((C'_i), (C''_h), (C'''_l); (D'_j), (D''_k), (D'''_m))$ マルチモジュールであることは明らかです。 同型。特に、$C$ が *可換* の環と $E, F, G$ 3 つの $C$ モジュールの場合、標準的 $C$ モジュール同型が存在します。

$$
(E \otimes_C F) \otimes_C G \to E \otimes_C (F \otimes_C G).
$$

以下では、特定の条件の下で、テンソル積の定義がマルチモジュールのファミリーに一般化できることを見ていきます。特に、命題 8 の仮説の下では、$\mathbf{Z}$ モジュール $E \otimes_A F \otimes_B G$ が得られます。これは、各モジュールと正規同型です。 $\mathbf{Z}$-モジュール $(E \otimes_A F) \otimes_B G$ および $E \otimes_A (F \otimes_B G)$ であり、後者はこれで識別されます。

### 9. マルチモジュールのファミリーのテンソル積

$(G_\lambda)_{\lambda \in L}$ を $\mathbf{Z}$ モジュールのファミリーとします。 写像 $u$ の集合 $G = \prod_{\lambda \in L} G_\lambda$ を $\mathbf{Z}$ モジュールに変換することは、$(x_\lambda) \mapsto u((x_\lambda))$ が各変数 $x_\lambda$ に関して加算的である場合、*多重加算* (または $\mathbf{Z}$-*多重線形*) であると言われます。正確に言うと、これは、すべての $\mu \in L$ とすべての元 $(a_\lambda) \in \prod_{\lambda \neq \mu} G_\lambda$ について、$G$ を $G_\mu \times \prod_{\lambda \neq \mu} G_\lambda$ と正規に識別することを意味します。

$$
u(x_\mu + y_\mu, (a_\lambda)) = u(x_\mu, (a_\lambda)) + u(y_\mu, (a_\lambda)) \quad \text{for } x_\mu, y_\mu \text{ in } G_\mu.
$$

これは、特に、$x_\lambda$ の 1 つが零の場合、$u((x_\lambda)) = 0$ であることを意味します。

また、*普遍的な写像問題* も考慮します。ここで、$\Sigma$ は $\mathbf{Z}$ モジュール構造の種であり、$\alpha$ マッピングは $G$ の $\mathbf{Z}$ モジュールへの多重加法写像です。 解は、$G$ の元の正式な線形結合の$\mathbf{Z}$ モジュール $C = \mathbf{Z}^{(G)}$ と、$\mathbf{Z}$ の係数およびサブ$\mathbf{Z}$ モジュール $D$ を考慮することによって得られます。 $C$ は元の形によって生成されました

$$
(x_\mu + y_\mu, (z_\lambda)_{\lambda \neq \mu}) - (x_\mu, (z_\lambda)_{\lambda \neq \mu}) - (y_\mu, (z_\lambda)_{\lambda \neq \mu})
$$

ここで、$\mu \in L, x_\mu \in G_\mu, y_\mu \in G_\mu$ と $z_\lambda \in G_\lambda$ ($\lambda \neq \mu$) は任意です。 商 $\mathbf{Z}$ モジュール $C/D$ は、$\mathbf{Z}$-*加群* のファミリー* $(G_\lambda)_{\lambda \in L}$ の *テンソル積 ($\mathbf{Z}$ 以上) と呼ばれ、$\bigotimes_{\lambda \in L} G_\lambda$ で示されます。 $G$ の元 $(x_\lambda)_{\lambda \in L}$ ごとに、$C$ の標準基底の元について、$\bigotimes_{\lambda \in L} x_\lambda$ は、C/D のこの元の標準像を表します。上記の定義から、Gの$\bigotimes_{\lambda \in L} G_\lambda$への写像$\phi : (x_\lambda) \mapsto \bigotimes_{\lambda \in L} x_\lambda$は$\mathbf{Z}$多重線形であり、Gの$\mathbf{Z}$モジュールHへの$\mathbf{Z}$多重線形写像$f$には、ただ1つだけ存在することがわかります。 $f = g \circ \phi$ となるような $\mathbf{Z}$-線形マッピング $g : \bigotimes_{\lambda \in L} G_\lambda \to H$;したがって、順序付けられた対 $\left( \bigotimes_{\lambda \in L} G_\lambda, \phi \right)$ は、問題の普遍的な写像問題を解決します。

$(G'_\lambda)_{\lambda \in L}$ を $\mathbf{Z}$ モジュールの他のファミリーとし、すべての $\lambda \in L$ について、$v_\lambda : G_\lambda \to G'_\lambda$ を $\mathbf{Z}$ 線形マッピング (可換群の他の語準同型では) とします。 次にマッピング
$$
(x_\lambda) \mapsto \bigotimes_{\lambda \in L} v_\lambda(x_\lambda)
$$
G の $\bigotimes_{\lambda \in L} G'_\lambda$ への変換は $\mathbf{Z}$ 多線形であるため、$\bigotimes_{\lambda \in L} v_\lambda$ で示される $\bigotimes_{\lambda \in L} G_\lambda$ から $\bigotimes_{\lambda \in L} G'_\lambda$ への $\mathbf{Z}$ 線形写像が標準的に定義されます。
$$
\left( \bigotimes_{\lambda \in L} v_\lambda \right) \left( \bigotimes_{\lambda \in L} x_\lambda \right) = \bigotimes_{\lambda \in L} v_\lambda(x_\lambda).
$$
特に、一部の $\mu \in L$ について、$G_\mu$ の準同型性 $\theta$ を考慮します。 $\lambda \neq \mu$ に対して $v_\mu = \theta$ と $v_\lambda = 1_{G_\lambda}$ が $\bigotimes_{\lambda \in L} v_\lambda$ に等しい $\bigotimes_{\lambda \in L} G_\lambda$ の準同型性を $\tilde{\theta}$ で表します。

次に、集合 $\Omega$、写像が与えられたとします。
$$
c : \omega \mapsto (\rho(\omega), \sigma(\omega))
$$
$\Omega$ を $L \times L$ に、そしてすべての $\omega \in \Omega$、自己準同型 $p_\omega$ の $G_{\rho(\omega)}$ と自己準同型 $q_\omega$ $G_{\sigma(\omega)}$。彼らには対応する、$P = \bigotimes_{\lambda \in L} G_\lambda$の自己準同型$\tilde{p}_\omega$と$\tilde{q}_\omega$がいます。 R を、$\omega$ が $\Omega$ を通過するときに、自己準同型* $\tilde{p}_\omega - \tilde{q}_\omega$ の像の和集合によって生成される P のサブ$\mathbf{Z}$ 加群とする。 商 $\mathbf{Z}$ モジュール $P/R$ は、ファミリー* $(G_\lambda)_{\lambda \in L}$ の *テンソル積と呼ばれ、*c、p、q に関連しており、$\bigotimes_{(c, p, q)} G_\lambda$ で示されます。上で定義した写像 $\phi : G \to \bigotimes_{\lambda \in L} G_\lambda$ と標準準同型 $P \to P/R$ を合成すると、$\mathbf{Z}$ 多重線形写像 $\phi_{(c, p, q)} : G \to \bigotimes_{(c, p, q)} G_\lambda$ が得られ、$\phi_{(c, p, q)}((x_\lambda)) = \bigotimes_{(c, p, q)} x_\lambda$ または単に $\bigotimes_{(c)} x_\lambda$ と書きます。 $\bigotimes_{(c, p, q)} x_\lambda$ と $\phi_{(c, p, q)}$ の順序付けられた対からなるは、次の *ユニバーサル写像問題* を解決します: $\bar{p}_\omega$ (それぞれ $\bar{q}_\omega$) は写像を表します
$$
(x_{\rho(\omega)}, (x_\lambda)_{\lambda \neq \rho(\omega)}) \mapsto (p_\omega(x_{\rho(\omega)}), (x_\lambda)_{\lambda \neq \rho(\omega)})
$$
(それぞれ $(x_{\sigma(\omega)}, (x_\lambda)_{\lambda \neq \sigma(\omega)}) \mapsto (q_\omega(x_{\sigma(\omega)}), (x_\lambda)_{\lambda \neq \sigma(\omega)})$)
G を自分自身に取り込みます。次に、$\Sigma$ は $\mathbf{Z}$ モジュール構造の種とみなされ、α マッピングは $G$ の $\mathbf{Z}$ 多重線形写像 $u$ を満たす条件である $\mathbf{Z}$ モジュールにマッピングします。

$$(26)$$
$$
u \circ \bar{p}_\omega = u \circ \bar{q}_\omega
$$

すべての$\omega \in \Omega$に。 証明は上記の定義から明らかです。

この構成は、特に no. 1 で説明した $E \otimes_A F$ を復元します。この場合、$L = \{1, 2\}$、$G_1 = E$、$G_2 = F$、$\Omega = A$ をとります。さらに、すべての $\omega \in A$ について、$\rho(\omega) = 1$、$\sigma(\omega) = 2$、$\omega$ は、$\mathbf{Z}$ モジュール $E$ の自己準同型 $x \mapsto x\omega$ と、$q_\omega$ 自己準同型 $y \mapsto \omega y$ が必要です。 $\mathbf{Z}$-モジュール$F$。

$(G'_\lambda)_{\lambda \in L}$ を $\mathbf{Z}$ モジュールの 2 番目のファミリーとします。 写像 $c$ を同じに保ち、$G'_{\rho(\omega)}$ の $\omega \in \Omega$、自己準同型 $p'_\omega$、および $G'_{\sigma(\omega)}$ の自己準同型 $q'_\omega$ がすべて与えられたとします。すべての $\lambda \in L$ について、$v_\lambda : G_\lambda \to G'_\lambda$ を、すべての $\omega \in \Omega$ について、次のような $\mathbf{Z}$ 線形マッピングとします。

$$(27)$$
$$
v_{\rho(\omega)} \circ p_\omega = p'_\omega \circ v_{\rho(\omega)} \quad \text{and} \quad v_{\sigma(\omega)} \circ q_\omega = q'_\omega \circ v_{\sigma(\omega)}
$$

(言い換えると、すべての $\lambda \in L$ に対して、$v_\lambda$ は、$\xi$ と $\eta$ を使用して、$p_\xi$ と $q_\eta$ (それぞれ $p'_\xi$ と $q'_\eta$) で定義された $G_\lambda$ (それぞれ $G'_\lambda$) の作用法則の射です。 $\rho(\xi) = \lambda$ と $\sigma(\eta) = \lambda$)。 それから写像
$$
u : (x_\lambda) \mapsto \bigotimes_{(c, p', q')} v_\lambda(x_\lambda)
$$
$G$ から $\bigotimes_{(c, p', q')} G'_\lambda$ への変換は $\mathbf{Z}$ 多線形であり、 条件 (26) を満たすため、 定義するは $\bigotimes_{(c, p, q)} G_\lambda$ から $\bigotimes_{(c, p', q')} G'_\lambda$ への $\mathbf{Z}$ 線形写像となり、混乱が生じない場合は単に $\bigotimes_{(c)} v_\lambda$ で表すことにします。

ここで、このように定義された一般テンソル積に対して「結合性」 性質を与えます。 $(L_i)_{1 \leq i \leq n}$ を $L$ の有限分割とします。すべての添字 $i$ について、$\Omega_i$ は、$\rho(\omega) \in L_i$ と $\sigma(\omega) \in L_i$ のように、$\Omega$ の部分集合からなる元を表します。明らかに、$\Omega_i$ はペアで互いに素です。私たちは集合$\Omega' = \Omega - \left( \bigcup_i \Omega_i \right)$です。それぞれの添字 $i$ について、$c^{(i)}$ は $\Omega_i$ から $L_i \times L_i$ への写像 $\omega \mapsto (\rho(\omega), \sigma(\omega))$ を表します。 $\omega \in \Omega_i$ の場合、$p_\omega$ と $q_\omega$ の代わりに $p^{(i)}_\omega$ と $q^{(i)}_\omega$ と書きます。次に、それぞれの $i$ に「部分」テンソル積があります。
$$
F_i = \bigotimes_{(c^{(i)}, p^{(i)}, q^{(i)})} G_\lambda.
$$

さらに次の「順列性」仮定を作ります。

(P) *$\omega \in \Omega'$、$p_\omega$ (それぞれ $q_\omega$) は、$\xi \notin \Omega'$、$\eta \notin \Omega'$、$\rho(\omega) = \rho(\xi) = \sigma(\eta)$ のように、$G_{\rho(\omega)}$ (それぞれ $G_{\sigma(\omega)}$) の自己準同型 $p_\xi$ および $q_\eta$ と並べ替えられます。 (それぞれ $\sigma(\omega) = \rho(\xi) = \sigma(\eta)$).*

それぞれの $\omega \in \Omega'$ について、$i$ を $\rho(\omega) \in L_i$ となるような添字とします。次に、$v_{\rho(\omega)} = p_\omega$ と $v_\lambda = 1_{G_\lambda}$ が $\lambda \neq \rho(\omega)$ となる家族 $(v_\lambda)_{\lambda \in L_i}$ を考えます。 仮定 (P) は、家族 $(v_\lambda)$ が条件 (27) を満たすことを意味します (ここで、$p'$ と $p$ は $p^{(i)}$、$q'$、$q$ は $q^{(i)}$、$\omega$ に置き換える必要があります) 元 $\xi$ が $\Omega_i$ を通過するまで）。したがって、自己準同型 $\bigotimes_{(c^{(i)})} v_\lambda = r_\omega$ は、$\mathbf{Z}$ モジュール $F_i$ から導出されます。同様に、自己準同型 $s_\omega$ は、$q_\omega$ で始まる $\mathbf{Z}$ モジュール $F_j$ で定義され、$j$ は $\sigma(\omega) \in L_j$ となるように添字になります。最後に$d(\omega) = (i, j)$をさせます。次に、*テンソル積* $\bigotimes_{(d, r, s)} F_i$ と対応する標準写像を定義するとします。

$$
\phi_{(d, r, s)} : \prod_{i=1}^n F_i \to \bigotimes_{(d, r, s)} F_i.
$$

一方、$i$、標準写像については、

$$
\psi_i = \phi_{(c^{(i)}, p^{(i)}, q^{(i)})} : \prod_{\lambda \in L_i} G_\lambda \to F_i;
$$

集合の積の結合性を使用して、 $G$ から $\bigotimes_{(d, r, s)} F_i$ への $\mathbf{Z}$ 多重線形写像 $\psi = \phi_{(d, r, s)} \circ (\psi_i)$ が導出されます。 *順序付けられた対* $\left( \bigotimes_{(d, r, s)} F_i, \psi \right)$ * は、* $\left( \bigotimes_{(c, p, q)} G_\lambda, \phi_{(c, p, q)} \right)$ と同じユニバーサル問題の解であることを示し、よっては * 固有の* $\mathbf{Z}$ モジュール *同型* の存在に従うことになります。

$$
\theta : \bigotimes_{(c, p, q)} G_\lambda \to \bigotimes_{(d, r, s)} F_i
$$

$\psi = \theta \circ \phi_{(c, p, q)}$ (*集合理論*, IV, § 3, no. 1) のようになります。

$n$ の帰納法までに、証明は $n = 2$ のケースに還元されます。簡単にするために、$\bigotimes_{(d, r, s)} F_i$ と $\bigotimes_{(d, r, s)} y_i$ の代わりに $F_1 \otimes_{(d)} F_2$ と $y_1 \otimes_{(d)} y_2$ と書きます。 $G$ から $F_1 \otimes_{(d)} F_2$ までの写像を検討してください

$$
h : (x_\lambda) \to \left( \bigotimes_{(c^{(1)})} x_\lambda \right) \otimes_{(d)} \left( \bigotimes_{(c^{(2)})} x_\lambda \right).
$$

それは明らかに $\mathbf{Z}$-多重線形です。すべての $\omega \in \Omega$ について条件 (26) を満たすことがわかります。 $\omega \in \Omega_1$ または $\omega \in \Omega_2$ の場合、これは明らかです。それ以外の場合、アイデアを修正するために位数で、$\rho(\omega) \in L_1$ と $\sigma(\omega) \in L_2$、$h \circ \bar{p}_\omega$ の値と $(x_\lambda)$ の $h \circ \bar{q}_\omega$ がそれぞれ次のとおりであるとします。

$$
\left( r_\omega \left( \bigotimes_{(c^{(1)})} x_\lambda \right) \right) \otimes_{(d)} \left( \bigotimes_{(c^{(2)})} x_\lambda \right) \quad \text{and} \quad \left( \bigotimes_{(c^{(1)})} x_\lambda \right) \otimes_{(d)} \left( s_\omega \left( \bigotimes_{(c^{(2)})} x_\lambda \right) \right)
$$

これらは、$F_1 \otimes_{(d)} F_2$ の定義によっても等しくなります。

そうであれば、$u$ を、条件 (26) を満たす、$G$ の $\mathbf{Z}$ モジュール $H$ への $\mathbf{Z}$ 多線形写像とする。 $u = v \circ h$ となるような $\mathbf{Z}$ 線形写像 $v : F_1 \otimes_{(d)} F_2 \to H$ を定義し、それが私たちの主張を証明します (no. 1、命題 1 の系 1 の議論を繰り返します)。 すべての $z_2 = (x_\lambda)_{\lambda \in L_2}$ について、$\prod_{\lambda \in L_1} G_\lambda$ の「部分」線形写像を $H$ とみなします。

$$
u(., z_2): (x_\lambda)_{\lambda \in L_1} \mapsto u((x_\lambda)_{\lambda \in L_1}, z_2) = u((x_\lambda)_{\lambda \in L}).
$$

明らかに、それは $\mathbf{Z}$ 多重線形であり、$\omega \in \Omega_1$ に対して条件 (26) を満たします。したがって、定義により、$F_1$ から $H$ への $\mathbf{Z}$ 線形写像 $y_1 \mapsto w_1(y_1, x_2)$ が存在します。

$$
w_1\left( \bigotimes_{(c^{(1)})} x_\lambda, z_2 \right) = u((x_\lambda)_{\lambda \in L_1}, z_2)
$$

次に写像を検討します

$$
u_2: (x_\lambda)_{\lambda \in L_2} \mapsto w_1(., (x_\lambda)_{\lambda \in L_2})
$$

$\prod_{\lambda \in L_2} G_\lambda$ を $\mathrm{Hom}_\mathbf{Z}(F_1, H)$ に。これは明らかに $\mathbf{Z}$ 多重線形であり、$u$ と関係 (28) および (29) 上の仮定のおかげで、形 $\bigotimes_{(c^{(1)})} x_\lambda$ の元が考慮され、$\omega \in \Omega_2$ に対する条件 (26) を満たします。 生成する $\mathbf{Z}$ モジュール $F_1$。したがって、$\mathbf{Z}$ 線形マッピングが存在します。

$$
w_2: F_2 \to \mathrm{Hom}_\mathbf{Z}(F_1, H)
$$

そのような

$$
w_2\left( \bigotimes_{(c^{(2)})} x_\lambda \right) = u_2((x_\lambda)_{\lambda \in L_2})
$$

またはまた

$$
\left( w_2\left( \bigotimes_{(c^{(2)})} x_\lambda \right) \right)\left( \bigotimes_{(c^{(1)})} x_\lambda \right) = u((x_\lambda)_{\lambda \in L}).
$$

ここで、$y_1 \in F_1, y_2 \in F_2$、$H$ の元を検討します。

$$
w(y_1, y_2) = (w_2(y_2))(y_1).
$$

明らかに、$w$ は $F_1 \times F_2$ から $H$ への $\mathbf{Z}$ 双線形写像です。さらに、すべての $\omega \in \Omega'$ について、(アイデアを修正するために、$\rho(\omega) \in L_1$ と $\sigma(\omega) \in L_2$ と仮定します) ことを示します。

$$
w(r_\omega(y_1), y_2) = w(y_1, s_\omega(y_2)).
$$

$y_1$ (それぞれ $y_2$) が $\bigotimes_{(c^{(1)})} x_\lambda$ (それぞれ $\bigotimes_{(c^{(2)})} x_\lambda$) の形式である場合、これらの要素が $\mathbf{Z}$ モジュール $F_1$ (それぞれ $F_2$) を生成するため、この関係を検証するだけで十分です。 ただし、定義, $r_\omega\left( \bigotimes_{(c^{(1)})} x_\lambda \right) = \bigotimes_{(c^{(1)})} x'_\lambda$ で、L₁ の λ ≠ ρ(ω) の場合、$x'_{\rho(\omega)} = p_\omega(x_{\rho(\omega)})$ と $x'_\lambda = x_\lambda$ です。同様に $s_\omega\left( \bigotimes_{(c^{(2)})} x_\lambda \right) = \bigotimes_{(c^{(2)})} x''_\lambda$、L₂ の λ ≠ σ(ω) の場合、$x''_{\sigma(\omega)} = q_\omega(x'_{\sigma(\omega)})$ と $x''_\lambda = x_\lambda$。 (30) と (31) を使用すると、(26) から関係 (32) が得られます。 したがって、$v(y_1 \otimes y_2) = w(y_1, y_2)$ となるような F₁ ⊗ F₂ の H への$\mathbf{Z}$ 線形写像 v が存在し、(30) と (31) から $v \circ h = u$ が得られます。

上記で定義された一般的なテンソル積の最も重要な特殊ケースは次のとおりです。 環のファミリー $(A_i)_{1 \leq i \leq n-1}$ とファミリー $(E_i)_{1 \leq i \leq n}$ から始めます。ここで、$E_1$ は右側の $A_1$ モジュール、$E_n$ は左側の $A_{n-1}$ 加群です。 $2 \leq i \leq n-1$、$E_i$ は $(A_{i-1}, A_i)$ バイモジュールです。次に、上記の定義は次のように適用されます。 L は集合 $[1, n]$、$G_i = E_i$、Ω は $A_i$ ($1 \leq i \leq n-1$) の集合和です。 $\omega \in A_i$ ($1 \leq i \leq n-1$) の場合、$\rho(\omega) = i$、$\sigma(\omega) = i + 1$、$p_\omega$ は、$Z$ モジュール $E_i$ および $q_\omega$ 自己準同型の自己準同型 $x \mapsto x\omega$ となります。 $Z$ モジュール $E_{i+1}$ の $y \mapsto \omega y$; 対応するテンソル積は次のように表されます。

$$
E_1 \otimes_{A_1} E_2 \otimes_{A_2} E_3 \otimes \cdots \otimes_{A_{n-2}} E_{n-1} \otimes_{A_{n-1}} E_n
$$

(記法ここで、$A_i$ は時々抑制される場合があります) およびこのテンソル積の $\bigotimes_{(c, p, q)} x_i$ と元は、$1 \leq i \leq n$ に対して $x_i \in E_i$ となるような家族 $(x_i)$ に対して、混乱が生じなければ $x_1 \otimes x_2 \otimes \cdots \otimes x_n$ と書くことができます。類似の記法が $Z$ 線形マッピング $\bigotimes_{(c)} v_i$ に使用されます。 $2 \leq i \leq n-1$ の $E_i$ は両側加群であるため、$[1, n]$ のすべての分割に対して仮定 (P) が成り立ちます。 $n = 3$ のとき、no. 8 でほのめかされた $Z$ 加群 $E \otimes_A F \otimes_B G$ を定義し、命題 8 (no. 8) を回収しました。

それぞれの $E_i$ がマルチモジュールの場合 ($2 \leq i \leq n-1$、$A_{i-1}$ については、環の 1 つが左側で動作し、$A_i$ 環の 1 つが右側で動作し、$i = 1$ と $i = n$ については条件が類似) の場合、次のようになります。 no. 4では、$E_i$($1 \leq i \leq n$)で動作する$A_i$を除くすべての環に関して、$E_1 \otimes_{A_1} E_2 \otimes \cdots \otimes_{A_{n-1}} E_n$でマルチモジュール構造が定義されています。

特に、C を可換環、$(E_i)_{1 \leq i \leq n}$ を C モジュールのファミリーとします。与えられた構造と $E_i$ に、与えられた構造と同一の 2 つの C モジュール構造を $E_1$ と $E_n$ に与えることにより、$2 \leq i \leq n-1$ に与えられた構造と同一の 3 つの C モジュール構造を与え、テンソル積上で定義するを実現します。

$$
E_1 \otimes_C E_2 \otimes_C E_3 \otimes \cdots \otimes_C E_{n-1} \otimes_C E_n
$$

$n$ C モジュール構造は 1 つの他のと互換性があり、すべての $\gamma \in C$ と $(x_i) \in \prod_{i=1}^n E_i$ については定義によって作成されているため、実際には同一です。

$$
(\gamma x_1) \otimes x_2 \otimes \cdots \otimes x_n \\
= x_1 \otimes (\gamma x_2) \otimes \cdots \otimes x_n = \cdots = x_1 \otimes x_2 \otimes \cdots \otimes (\gamma x_n).
$$

テンソル積 (34) を C モジュールとして話すときは、特に言及しない限り、常にこの構造、〜でない限りを意味し、混乱が生じない限り、テンソル積 (34) も $\bigotimes_{1 \leq i \leq n} E_i$ で表されます。すべての C モジュール G に対して、$\prod_{i=1}^n E_i$ の G への $\mathbf{Z}$ 多線形写像は、すべての添字 i に対して、満たす関係

$$
f(x_1, \ldots, x_{i-1}, \gamma x_i, x_{i+1}, \ldots, x_n) = \gamma f(x_1, \ldots, x_n)
$$

$\gamma \in \mathbf{C}$ と $(x_i) \in \prod_i E_i$ は、C-多重線形と呼ばれ、形は、$\mathscr{L}_n(E_1, \ldots, E_n; G)$ で示される C-モジュールと呼ばれます。 テンソル積 (34) の普遍性により、定義する正規の C モジュール同型が可能になります。

$$
\mathscr{L}_n(E_1, \ldots, E_n; G) \to \operatorname{Hom}_\mathbf{C}(E_1 \otimes_\mathbf{C} E_2 \otimes \cdots \otimes_\mathbf{C} E_n, G)
$$

これは、すべての C 多線形マッピング f と C 線形マッピング g を次のように関連付けます。

$$
f(x_1, \ldots, x_n) = g(x_1 \otimes x_2 \otimes \cdots \otimes x_n).
$$

$E_1 \times \cdots \times E_n$ から $\mathbf{C}$ への C 多重線形写像は、$n$ 線形形式とも呼ばれます。

$(F_i)_{1 \leq i \leq n}$ を C モジュールの他のファミリとします。 n 個の C 線形写像 $u_i : E_i \to F_i, u_1 \otimes u_2 \otimes \cdots \otimes u_n$ ($\bigotimes_{1 \leq i \leq n} u_i$ とも表される) のすべての系は、次の C 線形写像です。

$$
E_1 \otimes_\mathbf{C} E_2 \otimes \cdots \otimes_\mathbf{C} E_n \text{ into } F_1 \otimes_\mathbf{C} F_2 \otimes \cdots \otimes_\mathbf{C} F_n.
$$

さらに、$(u_1, \ldots, u_n) \mapsto u_1 \otimes u_2 \otimes \cdots \otimes u_n$ は、$\prod_i \operatorname{Hom}_\mathbf{C}(E_i, F_i)$ の C 多重線形写像です。

$$
\operatorname{Hom}_\mathbf{C}(E_1 \otimes_\mathbf{C} E \otimes \cdots \otimes_\mathbf{C} E_n, F_1 \otimes_\mathbf{C} F_2 \otimes \cdots \otimes_\mathbf{C} F_n).
$$

したがって、後者の写像に対して正準的に対応するがあり、正準と呼ばれる C 線形マッピングが存在します。

$$
\operatorname{Hom}_\mathbf{C}(E_1, F_1) \otimes_\mathbf{C} \operatorname{Hom}_\mathbf{C}(E_2, F_2) \otimes \cdots \otimes_\mathbf{C} \operatorname{Hom}_\mathbf{C}(E_n, F_n)
$$
$$
\to \operatorname{Hom}_\mathbf{C}(E_1 \otimes_\mathbf{C} E_2 \otimes \cdots \otimes_\mathbf{C} E_n, F_1 \otimes_\mathbf{C} F_2 \otimes \cdots \otimes_\mathbf{C} F_n)
$$

no. 5 で定義されたものを $n = 2$ に一般化します。

前に見た一般結合性性質は、ここで次のように特殊化できます。 分割 $(J_k)_{1 \leq k \leq m}$ of 区間 $\{1, n\}$ of $\mathbf{N}$ の場合、$k$、$F_k$ をそれぞれテンソル積 $E_{i_1} \otimes_\mathbf{C} E_{i_2} \otimes \cdots \otimes_\mathbf{C} E_{i_r}$ とします。ここで、$(i_1, \ldots, i_r)$ は真に増加する数列/元/$J_k$。次に、標準的な C モジュール同型 (「結合性同型」と呼ばれます) があります。

$$
F_1 \otimes_C F_2 \otimes \cdots \otimes_C F_m \to E_1 \otimes_C E_2 \otimes \cdots \otimes_C E_n
$$

上記では、記法、写像テンソル積

$$
y_1 \otimes y_2 \otimes \cdots \otimes y_m, \quad \text{where } y_k = x_{i_1} \otimes x_{i_2} \otimes \cdots \otimes x_{i_r},
$$

テンソル積 $x_1 \otimes x_2 \otimes \cdots \otimes x_n$ (すべての $i$ を$x_i \in E_i$) にします。

特に、$\pi$ が $\{1, n\}$ の置換である場合、$1 \leq k \leq n$ に対して $J_k = \{\pi(k)\}$ を書くと、正規 ("可換性") 同型が得られます。

$$
E_{\pi(1)} \otimes_C E_{\pi(2)} \otimes \cdots \otimes_C E_{\pi(n)} \to E_1 \otimes_C E_2 \otimes \cdots \otimes_C E_n
$$

写像 $x_{\pi(1)} \otimes x_{\pi(2)} \otimes \cdots \otimes x_{\pi(n)}$ から $x_1 \otimes x_2 \otimes \cdots \otimes x_n$ まで。多くの場合、これらの標準同型の下で、さまざまなテンソル積を対応するから 1 つの他のに同一視するします。

$1 \leq i \leq n$ については、$E_i$ が基底 $(b^{(i)}_{\lambda_i})_{\lambda_i \in L_i}$ を認めるとします。 $n$ の帰納法により、no. 7、系 2 から命題 7 から、$(\lambda_1, \ldots, \lambda_n)$ が $\prod_{1 \leq i \leq n} L_i$ を通る家族 $(b^{(1)}_{\lambda_1} \otimes b^{(2)}_{\lambda_2} \otimes \cdots \otimes b^{(n)}_{\lambda_n})$ は、$\bigoplus_{1 \leq i \leq n} E_i$、ときどきの基底であることがわかります。問題の基底 $(b^{(1)}_{\lambda_1})$ の *テンソル積* と呼ばれます。

#### 注意 {#alg-ii-s3-n9-rem-1 .statement tag=05PK}

(1) 可換環に対する加群の場合に関する上記の注意は、テンソル積 $E_1 \otimes_{A_1} E_2 \otimes \cdots \otimes_{A_{n-1}} E_n$ がある場合、no. 5, *注意* 2 のように一般化されます。ここで、環 $A_i$ は必ずしも可換ではありません。 $i$ には、同じ *可換* 環 $C$ の準同型 $\rho_i : C \to A$ があり、次のようになります: (1) $\rho_i(C)$ は $A_i$ の *中心* に含まれます。 (2) $2 \leq i \leq n - 1$ の場合、準同型 $\rho_{i-1}$ と $\rho_i$ *一致する* を使用して取得された $E_i$ の $C$ モジュール構造。次に、(13) (no. 5) と同様に、$E_1 \otimes_{A_1} E_2 \otimes \cdots \otimes_{A_{n-1}} E_n$ と標準写像で $C$-*加群* 構造が得られますが、これについては読者に説明してもらいます。

(2) $A, B$ を 2 つの環、$E$ を右 $A$ モジュール、$E'$ を左 $A$ モジュール、$F$ を右 $B$ モジュール、$F'$ を左とします。 $B$-モジュール。 $(E \otimes_A E') \times (F \otimes_B F')$ の $\mathbf{Z}\text{-bilinear}$ 写像は $\mathbf{Z}\text{-module}$ $G$ になり、$E \times E' \times F \times F'$ の $\mathbf{Z}\text{-multilinear}$ 写像 $f$ は $G$ と *1 対 1 の対応* になります。 満たす条件

$$
\begin{cases}
f(x \lambda, x', y, y') = f(x, \lambda x', y, y') \\
f(x, x', y \mu, y') = f(x, x', y, \mu y')
\end{cases}
$$

$\lambda \in A, \mu \in B, x \in E, x' \in E', y \in F, y' \in F'$の場合。この番号に記載されている一般的な構成これの簡約する証明は、形のテンソル積の結合性性質から続く、$(E \otimes_A E') \otimes_{\mathbf{Z}} (F \otimes_B F')$ と $E \otimes_A E' \otimes_{\mathbf{Z}} F \otimes_B F'$ の間の正規の $\mathbf{Z}\text{-module}$ 同型を定義します (33)。

### 練習問題 {#alg-ii-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
