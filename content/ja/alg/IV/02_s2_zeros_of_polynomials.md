---
book: alg
book_title: Algebra
chapter: IV
chapter_title: POLYNOMIALS AND RATIONAL FRACTIONS
section: 2
section_title: Zeros of polynomials
lang: ja
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A IV.14-A IV.19, A IV.87-A IV.88
pdf_pages: 0023-0028, 0096-0097
extraction: ocr
subsections:
    - "no": 1
      title: Roots of a polynomial in one indeterminate. Multiplicity
      page: 14
      pdf_page: 23
    - "no": 2
      title: Differential criterion for the multiplicity of a root
      page: 17
      pdf_page: 26
    - "no": 3
      title: Polynomial functions on an infinite integral domain
      page: 17
      pdf_page: 26
statements: 20
exercises: 13
content_sha256: b197f5ffa7abcf138021fd721f2b08c71ed0580c7e6cadca360e73d676691d21
translated_from: content/en/alg/IV/02_s2_zeros_of_polynomials.md
translation_method: google
source_content_sha256: 581af5e1e6500b23403ced41ae2a03e6692f4156d4da25e5f960df6e8a7c1371
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 935083a5fa72de973dcecf237c804b7e49ec47d7217deb39f730f31ca469e1f6
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 2。多項式の零

### 1. 根は不定数の多項式です。 重複度

$g \in A[(X_i)_{i \in I}]$ と $E$ を単一結合$A$-代数とする。 $x = (x_i)_{i \in I}$ を、$E$ のペアごとに置換可能な元の族とする。 $g(x) = 0$ の場合、$x$ は $E^l$ の $g$ の零であるとします。 $f$ が単一不定多項式の場合、$E$ の $f$ の零は、$E$ の $f$ の根とも呼ばれます。

#### 命題 1 {#alg-iv-s2-prop-1 .statement tag=06AO}

— $f \in A[X]$ と $\alpha \in A$ としましょう。 $f$を$X - \alpha$で割った余りは$f(\alpha)$です。 $\alpha$が$f$の根になるには、$X - \alpha$が$A[X]$の$f$の因子になることが必要かつ十分です。

なぜなら、$u,\ v \in \mathbf{A}[X]$ が $f = (X - \alpha)\ u + v,\ \deg v < 1$ である場合、$v$ はスカラーであり、$f(a) = (a - a)\ u(\alpha) + v = v$ です。これは最初の主張を証明し、2 番目はそこから続きます。

#### 命題 2 {#alg-iv-s2-prop-2 .statement tag=06AP}

— *$f \in \mathbf{A}[X]$、$a \in \mathbf{A}$、$h$を整数 $\geq 0$とします。次の条件は同等*:
(i) $f$ は $(X - \alpha)^h$ で割り切れますが、$(X - \alpha)^{h-1}$ では割り切れません。
(ii) *$f = (X - \alpha)^h g$ と $g(a) \neq 0$ のような $g \in \mathbf{A}[X]$ が存在します。
(i) $\Rightarrow$ (ii) 提案 1 から直ちに続きます。
(ii) $\Rightarrow$ (i) : $g$ が根として $a$ を認めない場合、$f = (X - \alpha)^h g$ と仮定します。すると、$f$ は $(X - \alpha)^h$ で割り切れます。 $g_1 \in \mathbf{A}[X]$ が $f = (X - \alpha)^{h+1} g_1$ のように存在した場合、$(X - \alpha)^n$ は $\mathbf{A}[X]$ の零の因子ではないため (IV、p. 9、提案 7)、$g = (X - a)\ g_1$ となり、$g(\alpha) = 0$ が得られます。不条理です。

#### 命題 3 {#alg-iv-s2-prop-3 .statement tag=06AQ}

— *$f$を$\mathbf{A}[X]$と$a \in \mathbf{A}$の非ゼロ元とします。提案 2 の整数 $h \geq 0$ 満たす条件 (i) と (ii) は 1 つだけ存在します。
これは、iff が $(X - \alpha)^h$、次に $\deg f \geq h$ (IV、p. 9、提案 7) で割り切れるという事実を念頭に置くと、条件 (i) については明らかです。

#### 定義 1 {#alg-iv-s2-def-1 .statement tag=06AR}

— *上記の記法により、$a$ は $f$ に対して位数 $h$、または重複度 $h$ であると言えます。*
$h > 0$ の場合、$a$ は位数 $h$ または重複度 $h$ の根であるとも言えます。 位数 1 の根は単純根、位数 2 の根は二重根、... 位数 $> 1$ の根は倍数と言われます。

#### 注意 1 {#alg-iv-s2-n1-rem-1 .statement tag=06AS}

$f = 0$ の場合、$a \in \mathbf{A}$ と整数 $h \geq 0$ が何であれ、$a$ は $f$ に対して位数 $\geq h$ であると言うことに同意します。任意の $f \in \mathbf{A}[X]$ と $a \in \mathbf{A}$ について、$a$ が $f$ に対して位数 $\geq h$ を持つということは、$(X - \alpha)^h$ 割る $f$ を意味します。

#### 注意 2 {#alg-iv-s2-n1-rem-2 .statement tag=06AT}

$B$ を可換環含む $\mathbf{A}$ を部分環とします。 $f \in \mathbf{A}[X]$ をゼロ以外の$a \in \mathbf{A}$ とします。 $f$に対する$a$の位数は、$f$を$B[X]$の元とみなしても、$\mathbf{A}[X]$の元とみなしても、同じです。これは、提案 2 の条件 (ii) から明らかです。

#### 命題 4 {#alg-iv-s2-prop-4 .statement tag=06AU}

— *$f$ と $g$ を $\mathbf{A}[X]$ の非ゼロ元とします。 $a \in \mathbf{A}$、$f$と$g$に対する$a$の位数をそれぞれ$p$と$q$とします。*
(i) *$f + g$に対する$a$の位数は$\geq \inf(p, q)$です。 $p \neq q$* の場合、$\inf(p, q)$ に等しい。
(ii) *$fg$に対する$a$の位数は$\geq p + q$です。 $\mathbf{A}$ が整域* の場合、これは $p + q$ と等しくなります。

というのは、$f(X) = (X - \alpha)^p f_1(X)$、$g(X) = (X - \alpha)^q g_1(X)$ と $f_1(\alpha) \neq 0$、$g_1(a) \neq 0$ があるからです。たとえば、$p \leq q$; と仮定します。それなら私たちは持っています
$$
f(X) + g(X) = (X - \alpha)^p (f_1(X) + (X - \alpha)^{q-p} g_1(X)) .
$$

$p < q$ の場合、$a$ は $f_1(X) + (X - \alpha)^{q-p} g_1(X)$ の根ではありません。これは(i)を証明します。一方、$A$ が整域の場合、$f(X)g(X) = (X - \alpha)^{p+q} f_1(X)g_1(X)$ と $f_1(\alpha)g_1(\alpha) \neq 0$ が得られます。これは(ii)を証明します。

#### 命題 5 {#alg-iv-s2-prop-5 .statement tag=06AV}

※$A$が整域だとします。 Let $f$ be a non-zero element of $A[X]$, and $\alpha_1, \ldots, \alpha_p$ pairwise distinct roots of $f$ in $A$, of orders $k_1, \ldots, k_r$. 我々は持っています*

$$
f(X) = (X - \alpha_1)^{k_1}(X - \alpha_2)^{k_2} \ldots (X - \alpha_p)^{k_p} g(X)
$$

*ここで、$g \in A[X]$ と $\alpha_1, \ldots, \alpha_p$ は $g$ の根ではありません。*

$p$ で帰納法まで進み、命題は $p = 1$ で明らかです。 1. 次に、$f(X) = g_1(X)g_2(X)$ と仮定します。

$$
g_1(X) = (X - \alpha_1)^{k_1} \ldots (X - \alpha_{p-1})^{k_{p-1}}, \quad g_2(X) \in A[X].
$$

$A$ は整域であり、$\alpha_p$ は $\alpha_1, \ldots, \alpha_{p-1}$ とは異なるため、$\alpha_p$ は $g_1(X)$ の根ではないため、$\alpha_p$ は位数の根 $k_p$ になります。 $g_2(X)$ (提案 4、(ii))。したがって、$g_2(X)$ は $(X - \alpha_p)^{k_p}$ で割り切れます。

$$
f(X) = (X - \alpha_1)^{k_1} \ldots (X - \alpha_p)^{k_p} g(X)
$$

どこで$g(X) \in A[X]$。明らかに、$\alpha_1, \ldots, \alpha_p$ は $g$ の根ではありません。

#### 定理 1 {#alg-iv-s2-thm-1 .statement tag=06AW}

※$A$を整域とします。ゼロ以外の元 $f$ の $A[X]$、次数 $n$ が与えられると、$A$ のすべての根のうち位数の和は $\leq n$ になります。

これは提案 5 の直後の結果です。

#### 系 {#alg-iv-s2-n1-cor-1 .statement tag=06AX}

※$A$が整域であると仮定し、次数$\leq n$の$f, g \in A[X]$とします。 $1 \leq i \leq n + 1$ に対して $f(x_i) = g(x_i)$ となるような、元 $x_1, \ldots, x_{n+1}$ と $A$ のペアごとに異なる $n + 1$ が存在する場合、$f = g$ になります。*

Thを適用すれば十分です。 1 ～ $f - g$。

#### 命題 6 (ラグランジュ補間公式) {#alg-iv-s2-prop-6 .statement tag=06AY}

— *$K$を可換体、$\alpha_1, \alpha_2, \ldots, a,$を$K$の元、および$\beta_1, \beta_2, \ldots, \beta_n$を$K$の元とします。 $i = 1, 2, \ldots, n$ には*を入れます

$$
f_i(X) = \prod_{j \in U(i)} (X - \alpha_j)/(\alpha_i - \alpha_j),
$$

*ここで、$U(i)$ は整数 $j$ の集合であり、$j \neq i$ と $1 \leq j \leq n$ になります。すると、$\beta_1 f_1 + \ldots + \beta_n f_n$ は $K[X]$ の一意元 $f$ となり、$1 \leq i \leq n$ に対して $\deg f < n$ と $f(\alpha_i) = \beta_i$ が成り立ちます。

一意性オフはコルから続きます。 Thさんへ。 1. $f = \beta_1 f_1 + \ldots + \beta_n f_n$ とすると、$f_i$ には次数 $n - 1$ があるため、$\deg f < n$ が得られます。一方、$j \neq i$ と $f_i(\alpha_i) = 1$ では $f_i(\alpha_j) = 0$ なので、$1 \leq i \leq n$ では $f(\alpha_i) = \beta_i$ になります。

#### 系 {#alg-iv-s2-n1-cor-2 .statement tag=06AZ}

— $\mathbf{A}$ が整域であると仮定します。 次数 $< n$ の $f \in \mathbf{A}[X]$ を、$K$ を $\mathbf{A}$ の部分環 、つまり体とします。 If there exist $n$ distinct elements $\alpha_1, \ldots, a_n$ of $\mathbf{A}$ such that $\alpha_i \in K$ and $f(\alpha_i) \in K$ for $i = 1, \ldots, n$, then $f \in K[X]$.

### 2. 根の重複度の差異基準

#### 命題 7 {#alg-iv-s2-prop-7 .statement tag=06B0}

— $f \in \mathbf{A}[X]$ と $a \in \mathbf{A}$ を根オフにします。 $a$ を単純な根オフにするためには、$a$ が $f$ の導関数 $Df$ の根であってはいけないことが必要かつ十分です。

仮定までに$f = (X - a)\ g$、ここで$g \in \mathbf{A}[X]$になります。 $a$ が $f$ の単純な根であるためには、$g(\alpha) \neq 0$ であることが必要かつ十分です。現在、$Df = g + (X - \alpha)\ Dg$、よって $(Df)(\alpha) = g(\alpha)$ がいます。

より一般的には:

#### 命題 8 {#alg-iv-s2-prop-8 .statement tag=06B1}

— $f \in \mathbf{A}[X]$ と $a \in \mathbf{A}$ とし、$a$ が $f$ に対して位数 $k \geq 1$ を持つと仮定します。その場合、$a$ は $Df$ に対して位数 $\geq k - 1$ になります。 $k . 1$が$\mathbf{A}$でキャンセル可能な場合、$a$は$Df$に対して位数$k - 1$になります。

仮定までに、$f = (X - a)^k g$と$g(a) \neq 0$のような$g \in \mathbf{A}[X]$が存在します。したがって、$Df = k(X - \alpha)^{k-1}g + (X - \alpha)^k Dg = (X - \alpha)^{k-1}(kg + (X - \alpha)\ Dg)$ は、命題の最初の部分を確立します。 $X = \alpha$の$kg + (X - \alpha)\ Dg$の値は$kg(a)$で、$k . 1$が$\mathbf{A}$でキャンセル可能な場合、これはゼロ以外になります。これは命題の 2 番目の部分を証明します。

$k$ を整数 $> 0$ として、$\mathbf{A}$ に $k . 1 = 0$ が入るようにします。 $f(X) = X^k$の場合、$0$は位数の根、$f$の$k$、および$Df$の任意の高い位数の根です。

#### 系 {#alg-iv-s2-n2-cor-1 .statement tag=06B2}

— $f \in \mathbf{A}[X]$、$a \in \mathbf{A}$、$p$ 整数 $\geq 0$ を、さらに $\mathbf{A}$ で $p! . 1$ がキャンセル可能であると仮定します。次に、$a$ が位数の根 $f$ の $p$ であるためには、$a$ が $D^pf$ の根ではなく、$f, Df, ..., D^{p-1}f$ の根であることが必要かつ十分です。

これは、$p$ の帰納法による提案 8 に続きます。

### 3. 無限大の多項式関数整域

#### 命題 9 {#alg-iv-s2-prop-9 .statement tag=06B3}

— $A$ が整域であると仮定します。 $I$ を集合、$(\mathbf{H}_i)_{i \in I}$ を $\mathbf{A}$ と $H = \prod_{i \in I} \mathbf{H}_i \subset A'$ の無限の部分集合の族とします。 $\mathbf{A}[(X_i)_{i \in I}]$ の非ゼロ元、およびすべての $x \in H$ のうち $H_f$ 集合で、$f(x) \neq 0$ となる場合、$H$ と $H_f$ は等価です。

a) まず、$I$ が有限であると仮定し、$n = \mathrm{Card}\ I$ を置きます。 命題は $n = 0$ に対してクリアです。 $n$の帰納法までにそれを証明します。 選ぶ元 $I$ の $i_0$ に $J = I - \{i_0\}$、$B = \mathbf{A}[(X_i)_{i \in J}]$ を入れます。 $f \neq 0$ なので、$g_0, \ldots, g_m \in B$ と $g_m \neq 0$ を、$f = \sum_{k=0}^m g_k X_{i_0}^k$ と書くことができます。すべての $x \in \prod_{i \in s} H_i$ の帰納法の仮定集合 K により、$g_m(x) \neq 0$ は $\prod_{i \in J} H_i$ と等価になります。 $x \in K$ の多項式の場合
$$
h(X_{i_0}) = \sum_{k=0}^m g_k(x) X_{i_0}^k \in A[X_{i_0}]
$$
はゼロではありません。 Thさんより1 (IV, p. 16) $a \in H_{i_0}$ の集合により、$h(\alpha) \neq 0$ は $H_{i_0}$ よってと等価になります
$$
\operatorname{Card} H \geq \operatorname{Card} H_f \geq (\operatorname{Card} K) \cdot (\operatorname{Card} H_{i_0}) = \operatorname{Card} H,
$$
それで$\operatorname{Card} H = \operatorname{Card} H_f$。

b) 一般的なケースでは、I のうち有限部分集合 $I'$ があり、$f \in A[(X_i)_{i \in I'}]$ となります。 $H'_f$ をすべての $x \in \prod_{i \in I'} H_i$ の集合として、$f(x) \neq 0$ とします。それから
$$
H_f = H'_f \times \left( \prod_{i \in I - I'} H_i \right),
$$
そして、証明の最初の部分を $H'_f$ に適用するだけで十分です。

#### 系 1 {#alg-iv-s2-prop-9-cor-1 .statement tag=06B4}

— *提案 9 の仮定と記法を維持します。l が空でない場合、$H_f$ は無限です。

#### 系 2 {#alg-iv-s2-prop-9-cor-2 .statement tag=06B5}

— *A が無限大整域であるか、A が無限大体上で代数であると仮定します。すべての $f \in A[(X_i)_{i \in I}]$ について、$\tilde{f}: A^I \to A$ を f (IV, p. 4) によって定義される多項式関数とします。したがって、写像 $f \mapsto \tilde{f}$ は単射法です。*

A が無限大整域の場合、提案 9 からすぐに系が得られます。A が無限大体 k 上で代数であるとします。 $f = \sum_{\nu \in \mathbf{N}^{(I)}} \alpha_\nu X^\nu$ を $A[(X_i)_{i \in I}]$ の非ゼロ元とします。その場合、$\alpha_{\nu_0} \neq 0$ となるような $\nu_0 \in \mathbf{N}^{(I)}$ と、$\varphi(\alpha_{\nu_0}) \neq 0$ となるような A 上の k 線形形式 $\varphi$ が存在します。 $g = \sum_{\nu \in \mathbf{N}^{(I)}} \varphi(a_\nu) X^\nu \in k[(X_i)_{i \in I}]$ しましょう。 $g \neq 0$ があるため、$g(x) \neq 0$ のような $x \in k^I$ が存在します。次に$\varphi(f(x)) = g(x) \neq 0$、そして$f(x) \neq 0$です。

A が無限大整域である場合、または A が無限大体を超える代数である場合、通常は同一視すると $\tilde{f}$ が一致します。

A が有限であると仮定し、$f(X) = \prod_{a \in A} (X - a)$、次に $f \neq 0$ ですが、$\tilde{f} = 0$ とします。その他の例については、IV、p. 88、練習問題 7 および 8 を参照してください。

#### 定理 2 (代数恒等式の拡大の原理) {#alg-iv-s2-thm-2 .statement tag=06B6}

— *A が無限大の整域であるとします。 $g_1, \ldots, g_m, f$ を $A[(X_i)_{i \in I}]$ の元とし、次の仮説を仮定します:*

a) $g_1 \neq 0, \ldots, g_m \neq 0$;
b) *すべて* $x \in \mathbf{A}^1$ *そのような* $g_1(x) \neq 0, \ldots, g_m(x) \neq 0$、*私たちは* $f(x) = 0$。 *それでは* $f = 0$。

$f \neq 0$ の場合、$fg_1 \ldots g_m \neq 0$ (IV, p. 9, 提案 8) があるため、$f(x)g_1(x) \ldots g_m(x) \neq 0$ (IV, p. 18, Cor. 2) のような $x \in \mathbf{A}^1$ が存在し、これは矛盾する仮定。

#### スコリウム {#alg-iv-s2-n3-sch-1 .statement tag=06B7}

— A を整域と $f \in A[(X_i)_{i \in I}]$ とします。 Th. 2 は、$f = 0$ の証明の便利な手段を提供します。無限の整域 E 含む A を部分環と考えるだけで十分です。すべての $(x_i) \in E^I$ (または、指定された非ゼロ多項式の有限数が消失しない $(x_i) \in E^I$ についても) について $f((x_i)) = 0$ を示すことができれば、$f = 0$ になります。 A 自体が無限ではない場合、たとえば E を環 $A[X]$ またはその分数の体とすることができます。

関係 $f = 0$ を証明したら、すべての $(y_i) \in F^I$ に対して $f((y_i)) = 0$ であると明確に推論できます。ここで、F は任意の単位結合および可換 A-代数です。特に、F は有限または非整数の場合があります。

In other words, the proof of the identity $f((x_i)) = 0$ when the $x_i$ run over an infinite integral domain containing A as subring (with the possible restriction that $g_k((x_i)) \neq 0$ for $1 \leq k \leq m$, where the $g_k$ are non-zero polynomials) implies the same identity when the $x_i$ run over any unital associative and commutative A-algebra.

特に$f \in Z[(X_i)_{i \in I}]$ にしましょう。 $x_i$ が $\mathbf{Z}$ を通過したときに $f((x_i)) = 0$ ($1 \leq k \leq m$ に対して $g_k((x_i)) \neq 0$ が制限になる可能性があり、$g_k$ はゼロではない $\mathbf{Z}[(X_i)]$ の元です)、$x_i$ が任意の元を通過したときに同じ同一性が得られます。 可換環。

### 練習問題 {#alg-iv-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
