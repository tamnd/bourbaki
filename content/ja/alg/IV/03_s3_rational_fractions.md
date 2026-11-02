---
book: alg
book_title: Algebra
chapter: IV
chapter_title: POLYNOMIALS AND RATIONAL FRACTIONS
section: 3
section_title: Rational fractions
lang: ja
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A IV.19-A IV.24, A IV.89-A IV.90
pdf_pages: 0028-0033, 0098-0099
extraction: ocr
subsections:
    - "no": 1
      title: Definition of rational fractions
      page: 19
      pdf_page: 28
    - "no": 2
      title: Degrees
      page: 20
      pdf_page: 29
    - "no": 3
      title: Substitutions
      page: 21
      pdf_page: 30
    - "no": 4
      title: Differentials and derivations
      page: 23
      pdf_page: 32
statements: 6
exercises: 7
content_sha256: 3ebff7bba1653480ec6aaefbbab9d54404f2b236265cdad97a4b81445ac5ae8c
translated_from: content/en/alg/IV/03_s3_rational_fractions.md
translation_method: google
source_content_sha256: adebb07e34c4e82901da99d345bb6f746140b39d50f239de82732119ccaa1a31
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 7068361892f0b20e988fad1011008b129b2d241bce07df63caf4ae3e0bd17a4d
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 3。 有理分数

### 1. 定義/有理分数

#### 定義 1 {#alg-iv-s3-def-1 .statement tag=06BL}

※Kを可換体とI集合とする。 整域 $K[(X_i)_{i \in I}]$ の分数 (I、p. 116) の体は、$K((X_i)_{i \in I})$ または $K(X_i)_{i \in I}$ で表されます。その元は、K の係数とともに不定数 $X_i$ で有理分数と呼ばれます。

$I = \{1, 2, \ldots, n\}$ の場合、$K((X_i)_{i \in I})$ の代わりに $K(X_1, X_2, \ldots, X_n)$ と書きます。

A を整域とし、K を分数の体とします。 環 $A[(X_i)_{i \in I}]$ は、$K[(X_i)_{i \in I}]$ の部分環と同一視される可能性があるため、$K((X_i)_{i \in I})$ の部分環とも同一視されます。それぞれの $f \in K[(X_i)_{i \in I}]$ に対して、$\alpha f \in A[(X_i)_{i \in I}]$ となる A の非ゼロ元 $\alpha$ が存在します。したがって、$K((X_i)_{i \in I})$ のすべての元は、$u, v \in A[(X_i)_{i \in I}], v \neq 0$ である $u/v$ と書くことができます。したがって、$K((X_i)_{i \in I})$ は、$A[(X_i)_{i \in I}]$ の分数の体と同一視される可能性があります。

ここで、K を可換体、I 集合、J ⊂ I とします。 B = K[(X_i)_{i ∈ J}] とすると、K[(X_i)_{i ∈ I}] = B[(X_i)_{i ∈ I - J}] となります。これまで述べてきたことから、K((X_i)_{i ∈ I}) は次のように識別できます。 K'((X_i)_{i ∈ I - J})、ここで K' = K((X_i)_{i ∈ J})。

### 2. 次数

K を可換体とします。 K((X_i)_{i ∈ I}) のすべての元 r に対して、v ≠ 0 および r = $\frac{u}{v}$ となる u、v ∈ K[(X_i)_{i ∈ I}] が存在します。 関係 $\frac{u}{v} = \frac{u_1}{v_1}$、ここで、v ≠ 0、v_1 ≠ 0 は uv_1 = vu_1 と同等です。 r ≠ 0 の場合、u ≠ 0 および u_1 ≠ 0 となるため、deg u + deg v_1 = deg v + deg u_1 (IV, p. 9)、または deg u − deg v = deg u_1 − deg v_1 となります。したがって、有理数整数 deg u − deg v は r にのみ依存します。これを次数、または r の合計次数と呼び、度 r で表します。 deg 0 = −∞ と書くことに同意します。 J ⊂ I の場合、添字 j ∈ J の X_j に関して同様に定義する次数ができます。 r が多項式の場合、これらの概念一致するは IV で定義されたものと一致し、 p. 2。

#### 命題 1 {#alg-iv-s3-prop-1 .statement tag=06BM}

— r、s を 2 有理分数とします。

(i) deg r ≠ deg s の場合、次のようになります。

$$
r + s \neq 0 \quad \text{and} \quad \deg(r + s) = \sup(\deg r, \deg s)
$$

deg r = deg s の場合、deg(r + s) ≤ deg r となります。

(ii) deg(rs) = deg r + deg s となります。

r と s がゼロ以外の場合については、極限自身で対処できます。

r = $\frac{u}{v}$, s = $\frac{w}{z}$ と書きましょう。ここで、u、v、w、z は非ゼロ多項式です。 rs = $\frac{uw}{vz}$ なので、

$$
\deg(rs) = \deg(uw) - \deg(vz) = \deg u - \deg v + \deg w - \deg z =
= \deg r + \deg s.
$$

一方、r + s = $\frac{uz + vw}{vz}$ となります。 deg r ≠ deg s、他の語 deg u + deg z ≠ deg w + deg v であるとします。その場合、uz + vw ≠ 0、そして

$$
\begin{align*}
\deg(r + s) &= \deg(uz + vw) - \deg(vz) \\
&= \sup(\deg(uz), \deg(vw)) - \deg(vz) \\
&= \sup(\deg(uz) - \deg(vz), \deg(wv) - \deg(vz)) \\
&= \sup(\deg r, \deg s).
\end{align*}
$$

deg r = deg s、つまり deg u + deg z = deg w + deg v であるとします。r + s ≠ 0 の場合、次のようになります。

$$
\begin{align*}
\deg(r + s) &= \deg(uz + vw) - \deg(vz) \\
&\leq \deg(uz) - \deg(vz) = \deg r
\end{align*}
$$

\* 写像 r ↦ −deg r は、体 K((X_i)_{i ∈ I}) の離散評価です。 \*

### 3. 交代

K を可換体、E を単位結合 K-代数、$x = (x_i)_{i \in I}$ を E のペアごとに置換可能な元の族とする。すべての非ゼロ $v \in B$ の $B = K[(X_i)_{i \in I}]$ と $S_x$ 集合を、$v(x)$ となるようにするは E で可逆です。$u \in B,\ v \in S_x$ と $f = \frac{u}{v} \in K((X_i)_{i \in I})$ としましょう。 元 $u(x)\ v(x)^{-1} = v(x)^{-1}u(x)$ は E で定義されます。さらに、$u_1,\ v_1$ が $f = \frac{u_1}{v_1}$ と $v_1 \in S_x$ のような 2 つの多項式である場合、$uv_1 = vu_1$、したがって $u(x)v_1(x) = v(x)u_1(x)$ などとなります。
$$
u(x)\ v(x)^{-1} = u_1(x)\ v_1(x)^{-1}.
$$

$f \in K((X_i)_{i \in I})$ にしましょう。 $f = \frac{u}{v}$ と $v \in S_x$ のような *少なくとも 1 つのカップル* $(u, v)$ が存在する場合、x は $f$ で *置換可能* であると言います。 元 $u(x)\ v(x)^{-1}$ は、$f$ と $x$ にのみ依存し、$f(x)$ または $f((x_i))$ または $f((x_i)_{i \in I})$ で表されます。

#### 命題 2 {#alg-iv-s3-prop-2 .statement tag=06BN}

*K を可換体、E を単位結合 K-代数、$x = (x_i)_{i \in I}$ を E のペアごとに置換可能な元の族とする。$f \in K((X_i)_{i \in I})$ の集合 $S_x^{-1}B$ で、x は $f$ の K-部分代数に置換可能$K((X_i)_{i \in I})$。 写像 $f \mapsto f(x)$ は、E への $S_x^{-1}B$ の単位準同型 $\varphi$ です。 像 $\varphi(S_x^{-1}B)$ は、すべての $yz^{-1}$ の集合であり、ここで y は、生成された E の単位部分代数 $K[x]_E$ を実行します。家族 x によって、z は $K[x]_E$ のすべての可逆元のうち集合を超えます。

$f_1 = \frac{u_1}{v_1},\ f_2 = \frac{u_2}{v_2}$ を $K((X_i)_{i \in I})$ の 2 つの元として、$v_1,\ v_2 \in S_x$ とします。 $f_1 + f_2 = \frac{u_1v_2 + u_2v_1}{v_1v_2},\ f_1f_2 = \frac{u_1u_2}{v_1v_2}$と$v_1,\ v_2 \in S_x$がございます。したがって、$S_x^{-1}B$ は $K((X_i)_{i \in I})$ の K-部分代数です。 命題の残りはクリアです。

#### 系 {#alg-iv-s3-n3-cor-1 .statement tag=06BO}

*Lを可換体、KをLの部分体、$x = (x_i)_{i \in I}$をLの元、M集合からなるを$x_i$、Uとします。すべての $f \in K((X_i)_{i \in I})$ の集合で、U の $f$ と $\varphi$ の準同型 $f \mapsto f(x)$ を L に置き換えることができます。したがって、$\varphi(U)$ は、$KUM$ によって生成された L の部分体です。

L' を、$KUM$ によって生成された L の部分体とします。私たちは持っています
$$
K \cup M \subset \varphi(U) \subset L'
$$
そして$\varphi(U)$はLの部分環です。ここで、提案 2 は、$\varphi(U)$ が L の部分体、よって $\varphi(U) = L'$ であることを意味します。

$f \in K((X_i)_{i \in I})$ と $(g_i)_{i \in I}$ を $K((Y_l)_{l \in L})$ の元の家族とする。 (g_i) が f に代入可能である場合、f((g_i)) は K((Y_l)_{l \in L}) の元です。特に、(X_i)_{i \in I} は f および f = f((X_i)_{i \in I}) に代入可能です。

#### 命題 3 {#alg-iv-s3-prop-3 .statement tag=06BP}

— E を K 上の代数とします。これは結合的、可換的、単位的で非ゼロです。 f \in K((X_i)_{i \in I}) とし、各 i \in I に対して g_i \in K((Y_l)_{l \in L}) とします。 E の元の族 y = (y_l)_{l \in L} が与えられた場合、y が各 g_i に代入可能であり、(g_i(y))_{i \in I} が f に代入可能であるとします。次に:
(i) (g_i)_{i \in I} は f に代入可能です。
(ii) K((Y_l)_{l \in L}) の h 元 f((g_i)) で表すと、y は h に代入可能であり、h(y) = f((g_i(y))) となります。

I を有限であるとみなしてもよいでしょう。 仮定により、それぞれの $i \in I$ に対して、$g_i$ を形 $p_i/q_i$ に入れることができます。ここで、$p_i, q_i \in K[(Y_l)_{l \in L}]$ と $q_i(y)$ は E で反転可能です。同様に、f は $u/v$ として書くことができます。ここで、$u, v \in K[(X_i)_{i \in I}]$ と$v((g_i(y)))$ は反転可能です。 $m = \sup(\deg u, \deg v)$ とし、$w = \prod_{i \in I} q_i \in K[(Y_l)_{l \in L}]$、$u_1 = u((g_i)) w^m$、$v_1 = v((g_i)) w^m$ とします。多項式 u は、$\sum_{i \in I} \nu_i \leq m$ となるような単項式 $\prod_{i \in I} X_i^{\nu_i}$ の K 線形結合です。 mの選択による$w^m \prod_{i \in I} g_i^{\nu_i} = w^m \left( \prod_{i \in I} p_i^{\nu_i} \right) \left( \prod_{i \in I} q_i^{\nu_i} \right)^{-1} \in K[(Y_l)_{l \in L}]$があります。したがって、$u_1 \in K[(Y_l)_{l \in L}]$、同様に$v_1 \in K[(Y_l)_{l \in L}]$となります。また、$v_1(y) = (w(y))^m v((g_i(y)))$は反転可能です。したがって、$v_1 \neq 0$、したがって、$E \neq 0$、したがって、$v((g_i)) \neq 0$。したがって、ファミリー $(g_i)$ は f に置き換え可能です。 $f((g_i)) = u_1/v_1$ があるため、y は $h = f((g_i))$ と $h(y) = u_1(y)/v_1(y) = u((g_i(y)))/v((g_i(y))) = f((g_i(y)))$ で置き換え可能です。

K を可換体、E を可換結合かつ単位 K-代数、f \in K((X_i)_{i \in I}) とします。 T_f を f に代入可能なすべての x = (x_i)_{i \in I} \in E^I の集合とします。 T_f から E への写像 x \mapsto f(x) は、f (および E) に関連付けられた有理数写像と呼ばれます。 ときどきは \tilde{f} で表します。 g \in K((X_i)_{i \in I}) の場合、T_f \cap T_g \部分集合 T_{f+g}、T_f \cap T_g \部分集合 T_{fg} が得られるため、f + g (それぞれ fg) に関連付けられた有理数写像は T_f \cap T_g で定義されます。この集合には \tilde{f} + \tilde{g} (それぞれ \tilde{f}\tilde{g}) と同じ値があります。 f(x) が可逆であるように、T'_f を T_f の x \の集合とします。 x \in T'_f の場合、x は 1/f に代入可能であり、1/f に関連付けられた有理数写像は x 値 f(x)^{-1} になります。

K が無限大可換体の場合、f \in K((X_i)_{i \in I})、g \in K((X_i)_{i \in I})、および \tilde{f}、\tilde{g} は、f、g (および K) に関連付けられた有理数写像です。 = \tilde{g}(x) すべての x \in T_f \cap T_g に対して f = g。 f = u/v および g = u_1/v_1 (u、v、u_1、v_1 が多項式) の場合、すべての x に対して u(x)v_1(x) = u_1(x)v(x) となり、v(x)v_1(x) \neq 0 となるため、uv_1 = u_1v (IV, p. 18, Th. 2)。したがって、 写像 f \mapsto \tilde{f} は単射法であり、多くの場合同一視する f および \tilde{f} となります。

\* $K[(X_i)_{i \in I}]$ (Comm. Alg.、VII, § 3, No. 2 p. 502、および Th. 2 p. 506 の Cor.) の階乗性を使用すると、次のことが簡単にわかります。すべての $f \in K((X_i)_{i \in I})$ に対して、次のような $u, v \in K[(X_i)_{i \in I}]$ が存在します。
    1) $f = u/v$;
    2) $x \in K^I$ が $f$ で代替可能であるためには、$v(x) \neq 0.$ が必要かつ十分です

### 4. ディファレンシャルと導分

$K$を可換体とします。 III、p. 558、提案 5 により、$K[(X_i)_{i \in I}]$ 拡大するのすべての導分 $D$ が、$K((X_i)_{i \in I})$ の導分 $\bar{D}$ にユニークな方法で追加されます。 $D, D'$が$K[(X_i)_{i \in I}]$の導分で置換可能な場合、括弧$[D, D'] = DD' - D'D$は零であるため、$K((X_i)_{i \in I})$の導分を$[D, D']$に拡張した$[\bar{D}, \bar{D}']$は零になります。他の語、$D$、$D'$ は置換可能です。特に、$K((X_i)_{i \in I})$ の導分 $D_i$ (IV、p. 6) 拡大するから導分は、再び $D_i$ で示され、ペアごとに置換可能です。 $f \in K((X_i)_{i \in I}), D_i f$ が $D_{x_i} f$ または $\frac{\partial f}{\partial x_i}$ または $f'_{x_i}$ とも書かれる場合。不定の $X$ が 1 つだけある場合は、記法 $Df, \frac{df}{dX}, f'$ が使用されます。

$B = K[(X_i)_{i \in I}], C = K((X_i)_{i \in I})$ にしましょう。 III、p. 574、提案 23、標準写像による

$$
\Omega_K(B) \otimes_B C \to \Omega_K(C)
$$

はベクトル $C$ スペースの同型です。 III、p. 570 を念頭に置くと、ベクトル $C$-空間 $\Omega_K(C)$ が $X_i$ の差分の族 $(dX_i)_{i \in I}$ を基底として認めることがわかります。 $\partial_i$ を、基底を基準とした $\Omega_K(C)$ 上の添字 $i$ の座標形とします。 Then the mapping $u \mapsto (\partial_i, du)$ of $C$ into itself is a derivation of $C$ which maps $X_i$ to 1 and $X_j$ to 0 for $j \neq i$, and so is equal to $D_i$; in other words, we have

$$
du = \sum_{i \in I} (D_i u) dX_i
$$

$u \in C$ごとに。 $I$ が有限である場合、$(D_i)_{i \in I}$ はベクトルの基底 $C$ の $C$ の導分の空間です。

#### 命題 4 {#alg-iv-s3-prop-4 .statement tag=06BQ}

— *$E$ を結合的、可換的、単位的な $K$-代数、$x = (x_i)_{i, I}$ を $E$ と $f \in K((X_i)_{i, I})$ の元の族とする。 $f$と$y = f(x)$で$x$が置換可能であるとします。
(i) 写像 $K[(X_i)_{i, I}]$ をそれ自体に組み込む $K((X_i)_{i, I})$ のすべての導分 $A$ について、$Af$ に $x$ が代入可能です。
(ii) $E$ の導分 $D$ を $E$ モジュールに入れると、

$$
Dy = \sum_{i \in I} (D_i f)(x) \cdot Dx_i .
$$

$f = \frac{u}{v}$ を E で反転可能な $u, v \in K[(X_i)_{i \in I}]$ と $v(x)$ とします。A をそれ自体の $K((X_i)_{i \in I})$ 写像 $K[(X_i)_{i \in I}]$ の導分とします。私たちは持っています
$$
\Delta f = \frac{(\Delta u)\ v - u(\Delta v)}{v^2}
$$
$v^2(x)$ は可逆であるため、x は $Af$ に代入可能です。 2番目に$r = u(x)$、$s = v(x)$を入れます。 $y = s^{-1}r$ があるので、E の導分 D を E モジュールに入れるごとに、
$$
\begin{align*}
Dy &= s^{-2}(s(Dr) - r(Ds)) \\
&= s^{-2}\left( s \sum_{i \in I} (D_iu)(x) \cdot Dx_i - r \sum_{i \in I} (D_iv)(x) \cdot Dx_i \right)
\end{align*}
$$
IV、p. 6の提案4による。したがって、$Dy = \sum_{i \in I} w_i \cdot Dx_i$は
$$
w_i = v(x)^{-2}(v(x)(D_iu)(x) - u(x)(D_iv)(x)) = (D_if)(x).
$$

### 練習問題 {#alg-iv-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
