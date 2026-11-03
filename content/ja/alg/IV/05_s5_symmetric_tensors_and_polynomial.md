---
book: alg
book_title: Algebra
chapter: IV
chapter_title: POLYNOMIALS AND RATIONAL FRACTIONS
section: 5
section_title: Symmetric tensors and polynomial mappings
lang: ja
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A IV.41-A IV.61, A IV.91-A IV.98
pdf_pages: 0050-0070, 0100-0107
extraction: ocr
subsections:
    - "no": 1
      title: Relative traces
      page: 41
      pdf_page: 50
    - "no": 2
      title: Definition of symmetric tensors
      page: 42
      pdf_page: 51
    - "no": 3
      title: Product for symmetric tensors
      page: 43
      pdf_page: 52
    - "no": 4
      title: Divided powers
      page: 45
      pdf_page: 54
    - "no": 5
      title: Symmetric tensors over a free module
      page: 47
      pdf_page: 56
    - "no": 6
      title: The functor TS
      page: 48
      pdf_page: 57
    - "no": 7
      title: Coproduct for symmetric tensors
      page: 50
      pdf_page: 59
    - "no": 8
      title: Relations between TS(M) and S(M)
      page: 52
      pdf_page: 61
    - "no": 9
      title: Homogeneous polynomial mappings
      page: 54
      pdf_page: 63
    - "no": 10
      title: Polynomial mappings
      page: 57
      pdf_page: 66
    - "no": 11
      title: Relations between $\mathbf{S}(M^*)$, TS(M)*gr and Pol(M, A)
      page: 59
      pdf_page: 68
statements: 41
exercises: 16
errata:
    - says: For each $w \in \Omega$ let $u_\omega = \sum_{b \in \omega} b$
      read: For each $\omega \in \Omega$ let $u_\omega = \sum_{b \in \omega} b$
      why: Omega is B/H and its elements are orbits, written omega everywhere else in Lemma 1 on page 56, including in the subscript and under the sum of this very sentence. The quantifier alone is set roman.
    - says: put $\omega' = w - \{v_\omega\}$ and $B' = \bigcup_{\omega \in \Omega} w'$
      read: put $\omega' = \omega - \{v_\omega\}$ and $B' = \bigcup_{\omega \in \Omega} \omega'$
      why: The thing omega' is obtained from is the orbit omega, named round twice earlier in the same clause of (ii), and the union is over the omega' just defined. Page 56 sets both of these two as roman w.
    - says: we have $u_\omega \in U^H$ for all $w \in \Omega$
      read: we have $u_\omega \in U^H$ for all $\omega \in \Omega$
      why: The proof on page 56 sets the subscript of u round and the quantifier of the same letter roman, in one clause.
content_sha256: e91075266d65f24c5f2d5e1d491c12e48ed80e7b4b5bab588049b6ea7823331c
translated_from: content/en/alg/IV/05_s5_symmetric_tensors_and_polynomial.md
translation_method: google
source_content_sha256: 0718f77b4c960447aa7b0aaceb1e4b634413b342ee6a1fdee7d6efa83b9be82a
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: d173a2bfeb42986931efb483ab6155c24882919b19cc04e7639a23fe37abaf8b
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 5。対称テンソルおよび多項式写像

### 1. 相対トレース

H を群とし、M を左 A[H] モジュール $^{(1)}$ とします。すべての $h \in H$ $^{(2)}$ に対して $hm = m$ となるように、すべての $m \in M$ の $M^H$ 集合で表します。これは M のサブ A モジュールです。

G を H の部分群とすると、$M^G$ は M 含む $M^H$ のサブ A モジュールです。

$m \in M^G$、$h \in H$ が与えられ、$x = hG$ が h を法とする G の左剰余類である場合、$xm = hGm = \{hm\}$ が得られます。 記法元 $hm$ を乱用すると、M は xm と書かれます。 $h' \in H$ の場合、

(1)
$$
h'(xm) = (h'x) m .
$$

これから G が H において有限添字であると仮定します。

(2)
$$
\sum_{x \in H/G} xm \in M^H .
$$

というのは、$h' \in H$ が与えられると、(1) のおかげで、

$$
h' \left( \sum_{x \in H/G} xm \right) = \sum_{x \in H/G} (h'x) m = \sum_{y \in H/G} ym .
$$

(1) H (III, p. 446) の A[H] 群代数と表す。
(2) この記法を、集合(*集合理論*、II、p. 102)の積の研究で導入されたものと混同しないように注意する必要があります。

#### 定義 1 {#alg-iv-s5-def-1 .statement tag=06CT}

— G が H の有限インデックスである場合、次のように定義される $M^G$ から $M^H$ へのマッピングを $\mathrm{Tr}_{H/G}$ で表します。

$$
\mathrm{Tr}_{H/G} m = \sum_{x \in H/G} x m .
$$

この写像は、A-加群$M^G$の準同型がA-加群$M^H$になります。

#### 命題 1 {#alg-iv-s5-prop-1 .statement tag=06CU}

— (i) $m \in M^G$ と $h \in H$ とします。次に$hm \in M^{hGh^{-1}}$と

$$
\mathrm{Tr}_{H/hGh^{-1}}(hm) = \mathrm{Tr}_{H/G} m .
$$

(ii) F を G の有限添字の G の部分群とし、$m \in M^F$ とすると、

$$
\mathrm{Tr}_{H/G}(\mathrm{Tr}_{G/F} m) = \mathrm{Tr}_{H/F} m
$$

(iii) *$m \in M^H$ の場合は、$\mathrm{Tr}_{H/G} m = (H : G) \cdot m$。

(i) $h \in H$ とします。 $h' \in H$と$m \in M$には、$\varphi(h') = hh'h^{-1}$と$\psi(m) = hm$を入れましょう。 $\varphi(h') \psi(m) = \psi(h'm)$ があります。 構造の転送により、$m \in M^G$ であれば $hm \in M^{hGh^{-1}}$ であると推測され、

$$
\mathrm{Tr}_{H/hGh^{-1}}(hm) = \psi(\mathrm{Tr}_{H/G}(m)) .
$$

$\mathrm{Tr}_{H/G}(m) \in M^H$ なので、これは (i) を証明します。

(ii) $m \in M^F$ と $(g_\alpha)_\alpha \in_A$ を G mod F の左剰余類の代表の系と、H mod G の左剰余類の代表の $(h_\beta)_\beta \in_B$ 系とします。すると、$(h_\beta g_\alpha)_{(\beta,\alpha) \in B \times A}$ は H mod F の左剰余類の代表の系となります。

$$
\begin{align*}
\mathrm{Tr}_{H/G}(\mathrm{Tr}_{G/F} m) &= \sum_{\beta \in B} h_\beta \left( \sum_{\alpha \in A} g_\alpha m \right) \\
&= \sum_{(\beta,\alpha) \in B \times A} (h_\beta g_\alpha) m = \mathrm{Tr}_{H/F} m .
\end{align*}
$$

(iii) この主張は明らかです。

### 2. 対称テンソルの定義

M をA-加群とします。 (III, p. 501) は、$\mathfrak{S}_n$ が A-加群 $T^n(M)$ の左側で作用することを思い出します。

$$
\sigma(x_1 \otimes x_2 \otimes \ldots \otimes x_n) = x_{\sigma^{-1}(1)} \otimes x_{\sigma^{-1}(2)} \otimes \ldots \otimes x_{\sigma^{-1}(n)}
$$

$x_1, \ldots, x_n \in M$ と $\sigma \in \mathfrak{S}_n$ の場合。 元 $z \in T^n(M)$ は、すべての $\sigma \in \mathfrak{S}_n$ に対して $\sigma \cdot z = z$ が位数 n の対称テンソルと呼ばれます。それらは形 $\mathbf{TS}^n(M)$ で示される $T^n(M)$ のサブ A モジュールです。 $\mathbf{TS}^0(M) = A, \mathbf{TS}^1(M) = M$があります。入れましょう

TS(M) = $\bigoplus_{n=0}^{\infty} TS^n(M)$;これは、$\mathbf{T}(M)$ のグレードのサブ A モジュールです。 $z \in T^n(M)$ 元 $\sum_{\sigma \in S_n} \sigma . z$ 属するから $TS^n(M)$ ごとに;これを$s . z$で表し、$z$の対称化と呼びます。 写像 $s : z \mapsto s . z$ は、A-加群 $T^n(M)$ の準同型を A-加群 $TS^n(M)$ に変換します。 $z \in TS^n(M)$なら$s . z = n! \ z$。

### 3. 積対称の場合テンソル

$p, q \in \mathbf{N}$ と $S_{p|q}$ をすべての置換 $\sigma \in S_{p-q}$ のうち $S_{p+q}$ からなるの部分群とし、区間 $(1, p)$ と $\mathbf{N}$ の $(p+1, p+q)$ を安定させます。 $\sigma \in S_p$ と $\sigma' \in S_q$ の場合、$1 \leq n \leq p$ に $\sigma''(n) = \sigma(n)$ を、$1 \leq n \leq q$ に $\sigma''(p+n) = p + \sigma'(n)$ を代入することで、$S_{p|q}$ の定義する元 $\sigma''$ が得られます。 写像 $(\sigma, \sigma') \mapsto \sigma''$ は、$S_p \times S_q$ の $S_{p|q}$ 上の同型です。

$z \in TS^p(M)$、$z' \in TS^q(M)$ とすると、$T^{p+q}(M)$ の元 $z \otimes z'$ は $S_{p|q}$ の下で不変です。したがって、$TS^{p+q}(M)$ の定義する元 $\operatorname{Tr}_{S_{p+q}/S_{p|q}}(z \otimes z')$ が可能です。 $TS(M)$ に A-bilinear 乗法 $(y, y') \mapsto yy'$ を装備し、$p, q \in \mathbf{N}$、$z \in TS^p(M)$、$z' \in TS^q(M)$ については次のようになります。

$$
zz' = \operatorname{Tr}_{S_{p+q}/S_{p|q}}(z \otimes z')
$$

$y \in TS(M)$ と $y' \in TS(M)$ の場合、$yy'$ を $y$ と $y'$ の対称積と呼びます。家族$(TS^p(M))_p$、 は、型 $\mathbf{N}$の代数 $TS(M)$の卒業であり、$\mathbf{T}(M)$の単位元は$TS(M)$の単位元です。

$S_{p,q}$ を次のような $\sigma \in S_{p+q}$ の集合とします。

$$
\begin{align*}
&\sigma(1) < \sigma(2) < \ldots < \sigma(p) \\
&\sigma(p+1) < \sigma(p+2) < \ldots < \sigma(p+q).
\end{align*}
$$

$S_{p,q} \times S_{p|q}$ の $S_{p+q}$ への写像 $(\sigma, \tau) \mapsto \sigma \tau$ は全単射 (I, p. 60, 例 2);したがって、$z \in TS^p(M)$ と $z' \in TS^q(M)$ の場合、

$$
zz' = \sum_{\sigma \in S_{p,q}} \sigma(z \otimes z')
$$

#### 命題 2 {#alg-iv-s5-prop-2 .statement tag=06CV}

— (i) A-代数 $TS(M)$ は結合的、可換的、および単位的です。

(ii) $p_1, \ldots, p_n$ を整数 $> 0$ とし、$S_{p_1| \ldots |p_n}$ をすべての $\sigma \in S_{p_1+\cdots+p_n}$ の集合とし、次の $\mathbf{N}$ の区間を安定させます。

$$
(1, p_1), (p_1+1, p_1+p_2), \ldots, (p_1+\cdots+p_{n-1}+1, p_1+\cdots+p_n).
$$

$z_1 \in \mathbf{TS}^{p_1}(M) , \ldots , z_n \in \mathbf{TS}^{p_n}(M)$ にして、それでは

$$
z_1 z_2 \ldots z_n = \operatorname{Tr}_{\mathfrak{S}_{p_1 + \cdots + p_n}/\mathfrak{S}_{p_1}| \cdots | p_n} (z_1 \otimes z_2 \otimes \ldots \otimes z_n) .
$$

特に$x_1, \ldots, x_r \in M$の場合、$x_1 \ldots x_r = s(x_1 \otimes \ldots \otimes x_r)$があります。

$n = 1$ については、主張 (ii) がクリアです。 関係と仮定します。

$$
z_2 \ldots z_n = \operatorname{Tr}_{\mathfrak{S}_{p_2 + \cdots + p_n}/\mathfrak{S}_{p_2}| \cdots | p_n} (z_2 \otimes \ldots \otimes z_n)
$$

が証明されており、制限から$(1, p_1)$までが同一性であるすべての置換のうち、$\mathfrak{S}_{p_1 + \cdots + p_n}$からなるの部分群と同一視する$\mathfrak{S}_{p_2 + \cdots + p_n}$を考えましょう。それから

$$
\operatorname{Tr}_{\mathfrak{S}_{p_1}|p_2+\cdots+p_n/\mathfrak{S}_{p_1}|p_2| \cdots | p_n} (z_1 \otimes z_2 \otimes \ldots \otimes z_r) =
$$
$$
= z_1 \otimes \operatorname{Tr}_{\mathfrak{S}_{p_2+\cdots+p_n}/\mathfrak{S}_{p_2}| \cdots | p_n} (z_2 \otimes \ldots \otimes z_r) = z_1 \otimes (z_2 \ldots z_n) .
$$

したがって、

$$
z_1 z_2 \ldots z_r = z_1 (z_2 \ldots z_r) =
$$
$$
= \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2+\cdots+p_n}/\mathfrak{S}_{p_1}|p_2-\cdots+p_n} (z_1 \otimes (z_2 \ldots z_n))
$$
$$
= \operatorname{Tr}_{\mathfrak{S}_{p_1+\cdots+p_n}/\mathfrak{S}_{p_1}|p_2+\cdots+p_n} (\operatorname{Tr}_{\mathfrak{S}_{p_1}|p_2+\cdots+p_n/\mathfrak{S}_{p_1}|p_2| \cdots | p_n} (z_1 \otimes z_2 \otimes \ldots \otimes z_n))
$$
$$
= \operatorname{Tr}_{\mathfrak{S}_{p_1-\cdots+p_n}/\mathfrak{S}_{p_1}| \cdots | p_n} (z_1 \otimes z_2 \otimes \ldots \otimes z_n)
$$

IV、p. 42の提案1、(ii)による。したがって、(ii)が成立する。

特に、

$$
z_1 (z_2 z_3) = \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2+p_3}/\mathfrak{S}_{p_1}|p_2|p_3} (z_1 \otimes z_2 \otimes z_3) ,
$$

そして同じように私たちはそれを示します

$$
(z_1 z_2) z_3 = \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2+p_3}/\mathfrak{S}_{p_1}|p_2|p_3} (z_1 \otimes z_2 \otimes z_3) .
$$

したがって、代数 $\mathbf{TS}(M)$ は結合的です。

$o$ を $\mathfrak{S}_{p_1+p_2}$ の元とすると、次のようになります。

$$
\begin{align*}
\sigma(1) &= p_2 + 1, \; \sigma(2) = p_2 + 2, \; \ldots, \; \sigma(p_1) = p_2 + p_1 , \\
\sigma(p_1 + 1) &= 1, \; \sigma(p_1 + 2) = 2, \; \ldots, \; \sigma(p_1 + p_2) = p_2 .
\end{align*}
$$

それから

$$
z_2 z_1 = \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2}/\mathfrak{S}_{p_2}|p_1} (z_2 \otimes z_1)
$$
$$
= \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2}/\sigma \mathfrak{S}_{p_1}|p_2 \sigma^{-1}\sigma} (z_1 \otimes z_2)
$$
$$
= \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2}/\mathfrak{S}_{p_1}|p_2} (z_1 \otimes z_2) \quad \text{by Prop 1, (i)}
$$
$$
= z_1 z_2 .
$$

したがって、代数 $\mathbf{TS}(M)$ は可換です。

なお、$\mathbf{T}(M)$の$\mathbf{TS}(M)$の標準単射は、一般に代数準同型ではありません。さらに悪いことに、$\mathbf{TS}(M)$ は、$\mathbf{T}(M)$ の乗法では一般的に安定していません。

### 4. 分割冪

$x \in M$と$k \in \mathbf{N}$としましょう。 $x, \otimes x_2 \otimes \ldots \otimes x_k$ であることは明らかです。
$$
x_1 = x_2 = \cdots = x_k = x ,
$$
は$\mathbf{TS}^k(M)$の元です。

#### 定義 2 {#alg-iv-s5-def-2 .statement tag=06CW}

*場合* $x \in M$、*元* $x \otimes x \otimes \ldots \otimes x$ *of* $\mathbf{TS}^k(M)$ *は* $\gamma_k(x)$ で表されます。

#### 命題 3 {#alg-iv-s5-prop-3 .statement tag=06CX}

(i) *$x \in M$ の場合、* $x$ の *pth 冪、*計算式* $\mathbf{TS}(M)$、*は $p! \; \gamma_p(x)$ に等しい。
(ii) *Let* $x_1, \ldots, x_n \in M$; *その後*
$$
\gamma_p(x_1 + x_2 + \cdots + x_n) = \sum_{p_1 + p_2 + \cdots + p_n = p} \gamma_{p_1}(x_1) \; \gamma_{p_2}(x_2) \ldots \gamma_{p_n}(x_n) .
$$
(iii) *$x_1, \ldots, x_n \in M$ と *させて* $p_1, \ldots, p_n$ *整数* $\geqslant 0$ *そして* $p = p_1 + \ldots + p_n$ とします。 *$E$ *写像* の集合 $\varphi$ *の* $\{1, \ldots, p\}$ *に* $(1, \ldots, n)$ *そのような*
$$
\operatorname{Card} \varphi^{-1}(1) = p_1, \ldots, \operatorname{Card} \varphi^{-1}(n) = p_n .
$$
*それでは*
$$
\gamma_{p_1}(x_1) \; \gamma_{p_2}(x_2) \ldots \gamma_{p_n}(x_n) = \sum_{\varphi \in E} x_{\varphi(1)} \otimes x_{\varphi(2)} \otimes \ldots \otimes x_{\varphi(p)} .
$$
(iv) *$x \in M$ *そして* $q, r$ *整数* $\geqslant 0$ とします。 *それでは*
$$
\gamma_q(x) \; \gamma_r(x) = \frac{(q + r)!}{q! \; r!} \; \gamma_{q + r}(x) .
$$
(v) *Let* $x_1, \ldots, x, \in M$、*そしてfor* $H \subset (1, \ldots, n)$ *put* $x_H = \sum_{i \in H} x_i$、*then*
$$
(-1)^n x_1 x_2 \ldots x_n = \sum_{H \subset \{1, \ldots, n\}} (-1)^{\operatorname{Card} H} \gamma_n(x_H) .
$$

主張 (i) は提案 2 (ii) からすぐに続きます。

(ii) を証明しましょう。 n の帰納法により、$n = 2$ の場合を考慮するだけで十分であることがわかります。それでは、

$$
\gamma_p(x_1 + x_2) = (x_1 + x_2) \otimes (x_1 + x_2) \otimes ... \otimes (x_1 + x_2) \quad @\text{factors})
$$
$$
= \sum_{p_1 + p_2 = p} \sum_{\sigma \in S_{p_1, p_2}} \sigma(x_1 \otimes x_1 \otimes ... \otimes x_1 \otimes x_2 \otimes x_2 \otimes ... \otimes x_2)
$$
$$
= \sum_{p_1 + p_2 = p} \sum_{\sigma \in S_{p_1, p_2}} \sigma(\gamma_{p_1}(x_1) \otimes \gamma_{p_2}(x_2))
$$
$$
= \sum_{p_1 + p_2 = p} \gamma_{p_1}(x_1) \gamma_{p_2}(x_2).
$$

(iii) を証明するには、$S_{p_1, ..., p_n}$ を制限から区間である $(1, p_1 + ... + p_n)$ の置換の集合とします。
$$(1, p_1), (p_1 + 1, p_1 + p_2), ..., (p_1 + ... + p_{n-1} + 1, p_1 + ... + p_n)$$
増加するです。 I、p. 60、例 2 および提案 2 により、(ii)
$$
\gamma_{p_1}(x_1) \gamma_{p_2}(x_2) ... \gamma_{p_n}(x_n) = \sum_{\rho \in S_{p_1, p_2, ..., p_n}} \rho(x_1 \otimes x_1 \otimes ... \otimes x_1 \otimes x_2 \otimes x_2 \otimes ... \otimes x_2 \otimes ... \otimes x_n \otimes x_n \otimes ... \otimes x_n)
$$
($p_i$ 因子 $x_i$) そして、この和は次と等しくなります。
$$
\sum_{\varphi \in E} x_{\varphi(1)} \otimes x_{\varphi(2)} \otimes ... \otimes x_{\varphi(p)}.
$$

(iii) に$n = 2, x_1 = x_2 = x, p_1 = q$ と $p_2 = r$ を入れると、(iv) (I、前掲) が得られます。

最後に (v) は、元 $x_i$ の環 $\mathbf{T}(M)$ に適用される、I、p. 100 の提案 2、(ii) および提案 2 に続きます。

#### 注意 1 {#alg-iv-s5-n4-rem-1 .statement tag=06CY}

$(x_i)_{i \in I}$ を M の元の家族とします。それぞれの $\nu \in \mathbf{N}^{(I)}$ に対して、
$$
x_\nu = \prod_{i \in I} \gamma_{\nu_i}(x_i).
$$
$(\lambda_i) \in \mathbf{A}^{(1)}$ と $p \in \mathbf{N}$ の場合、提案 3 (ii) により、
$$
\gamma_p \left( \sum_{i \in I} \lambda_i x_i \right) = \sum_{\nu \in \mathbf{N}^{(I)}, |\nu| = p} \lambda^\nu x_\nu.
$$
(6)

#### 注意 2 {#alg-iv-s5-n4-rem-2 .statement tag=06CZ}

$\mathscr{M}$を$(1, p)$の写像の集合をIとします。 定義する写像 $\rho \mapsto \rho^*$ の $\mathscr{M}$ を $\mathbf{N}^{(I)}$ に代入します
$$
\rho^*(i) = \operatorname{Card} \rho^{-1}(i)
$$

$\mathscr{M}$ から満たす $\rho_1^* = \rho_2^*$ の 2 つの元 $\rho_1, \rho_2$ では、$\rho_2 = \rho_1 \circ \sigma$ (I, p. 95) となる$\sigma \in \mathfrak{S}_p$ が存在することが必要十分です。提案 3 (iii) により、$|\nu| = p$ については、次のようになります。

$$
x_\nu = \sum_{\rho \in \mathscr{M}, \rho^* = \nu} x_{\rho(1)} \otimes x_{\rho(2)} \otimes \ldots \otimes x_{\rho(p)}
$$

### 5. 自由加群に対して対称テンソル

#### 命題 4 {#alg-iv-s5-prop-4 .statement tag=06D0}

— $M$ を自由にし、$M$ の $(e_i)_{i \in I}$ 基底を自由にします。

(i) $\nu \in \mathbf{N}^{(I)}$ については $e_\nu = \prod_{i \in I} \gamma_{\nu_i}(e_i)$ とします。すると、$(e_\nu)_{\nu \in \mathbf{N}^{(I)}}$ は $A$ モジュール $TS(M)$ の基底になります。特に、代数 $\mathbf{TS}(M)$ は、$k \in N$ と $x \in M$ に対して、元 $\gamma_k(x)$ のファミリーによって生成されます。

(ii) 各 $p \in N$ について、$\mathbf{TS}^p(M)$ は $A$ モジュール $\mathbf{T}^p(M)$ の直因子です。

上の注意 2 の記法を使用しましょう。家族$(e_{\rho(1)} \otimes \ldots \otimes e_{\rho(p)})_{\rho \in \mathscr{M}}$は$\mathbf{T}^p(M)$の基底です。したがって、提案 4 は、公式 (7) と次の補題に続き、$H = \mathfrak{S}_p$ と $U = \mathbf{T}^p(M)$ に適用されます。

#### 補題 1 {#alg-iv-s5-lem-1 .statement tag=06D1}

$H$ を有限群とし、$U$ を左の $A[H]$ モジュールとします。 $A$ モジュール $U$ が $U$ の $H$ の演算で安定している基底 $B$ を持ち、$\Omega = B/H$ を置くとします。それぞれ $w \in \Omega$ に対して $u_\omega = \sum_{b \in \omega} b$ とします。それから

(i) $(u_\omega)_{\omega \in \Omega}$ は、$A$ モジュール $U^H$ の基底です。

(ii) それぞれの $\omega \in \Omega$ について、$v$ を $\omega$ の点とします。 $\omega' = w - \{v_\omega\}$と$B' = \bigcup_{\omega \in \Omega} w'$を置くと、$B'$は$U$の$U^H$に対する補足部分空間の基底になります。

すべての $u_\omega$ ($\omega \in \Omega$ の場合) および $B'$ の集合の和集合は、$U$ の基底です。したがって、$U' = \sum_{\omega \in \Omega} Au$ と $U'' = \sum_{b \in B'} Ab$ の場合、$U = U' \oplus U''$ になります。一方、すべての $w \in \Omega$ に対して $u_\omega \in U^H$ があるため、$U' \subset U^H$ となります。最後に、$(\alpha_b)_{b \in B}$を$A$と有限台の元の家族とし、$x = \sum_{b \in B} \alpha_b b$とします。 $x \in U^H$ の場合、すべての $b \in B$ とすべての $h \in H$ に対して $\alpha_{hb} = \alpha_b^H$、したがって $x \in U'$ となり、$U' = u^H$ が続きます。

#### 命題 5 {#alg-iv-s5-prop-5 .statement tag=06D2}

— $M$ を自由な $A$ モジュール、$k$ 整数 $\geq 0$、$P$ を $\gamma_k(M)$ によって生成された $\mathbf{TS}^k(M)$ のサブ$A$ モジュールとします。 $A$ が無限大の整域であると仮定します。そして、それぞれの $z \in \mathbf{TS}^k(M)$ に対して、$az \in P$ となるような $a \in A - \{0\}$ が存在します。

$K$ を $A$ の分数の体とします。 ベクトル K 空間 $V = \mathbf{TS}^k(M) \otimes_A K$ のサブ A モジュールを使用して同一視する $\mathbf{TS}^k(M)$ (提案 4、および II、p. 314)。 このベクトル K 空間は $\gamma_k(M)$ によって生成されること、つまり、V 満たす $f(\gamma_k(M)) = 0$ 上のすべての K 線形形式 $f$ は零であることを示さなければなりません。 提案 4 のように、$(e_i)_{i \in I}$ を M の基底とし、定義するを e とします。 $(\alpha_i) \in A^{(I)}$ については、(6) を考慮すると、

$$
0 = f \left( \gamma_k \left( \sum_{i \in I} \alpha_i e_I \right) \right) = \sum_{\nu \in N^{(I)}, |\nu| = k} \alpha^\nu f(e_\nu).
$$

コル著IV、p. 18 の 2 では、すべての $\nu \in N^{(I)}$、よって $f = 0$ に対して $f(e_\nu) = 0$ となります。

### 6. ファンクター TS

M, N を A-加群とし、M の u 準同型を N にします。 $T(u)(TS(M)) \subset TS(N)$ であることは明らかです。 TS(M)をT(u)から得られるTS(N)に写像をTS(u)と表記します。これが等級付けされた代数の単体準同型であることは簡単に検証され、すべての $x \in M$ と各整数 $p \geq 0$ に対して TS(u) $(\gamma_p(x)) = \gamma_p(u(x))$ が得られます。 $v : N \to P$ が A-加群の準同型である場合、次のようになります。

$$
TS(v \circ u) = TS(v) \circ TS(u).
$$

TS(u) の定義により、図式

$$
\begin{array}{cccc}
M & \longrightarrow & TS(M) \longrightarrow T(M) \\
u \downarrow & & \downarrow TS(u) & \downarrow T(u) \\
N & \longrightarrow & TS(N) \longrightarrow T(N)
\end{array}
$$

は可換であり、水平矢印は標準単射を示します。

M が N の直因子で、i : M \to N が標準単射の場合、TS(i) は TS(M) の直因子 R 上の TS(M) の単射準同型であり、これにより通常同一視する TS(M) と R が成り立ちます。これはテンソル代数について証明されます(III、p. 487)。

M が部分加群の家族 $(M_\lambda)_{\lambda \in L}$ の直和であるとします。 標準単射 $TS(M_\lambda) \to TS(M)$ 定義する正規と呼ばれる、等級付けされた代数の単位準同型 h:

$$
\bigotimes_{\lambda \in L} TS(M_\lambda) \to TS(M)
$$

$\lambda_1, \lambda_2, \ldots, \lambda_n$ を L のペアごとに異なる元とし、$x_1 \in M_{\lambda_1}, \ldots, x_n \in M_{\lambda_n}$ とします。 IV、p. 45 の提案 3、(ii) により、次のようになります。

$$
h \left( \sum_{p_1 + \cdots + p_n = p} \gamma_{p_1}(x_1) \otimes \cdots \otimes \gamma_{p_n}(x_n) \right) = \gamma_p(x_1 + \cdots + x_n).
$$

$N$ を、部分加群のファミリー $(N_\lambda)_\lambda$ の直和である $A$ モジュールとします。 $\lambda \in L$ ごとに、$u_\lambda$ を $M_\lambda$ の準同型から $N_\lambda$ にします。 $u$ を $M$ の準同型を $u_\lambda$ で定義される $N$ にするとします。それから図式

$$
\begin{array}{ccc}
\otimes \mathbf{TS}(M_\lambda) & \xrightarrow{h} & \mathbf{TS}(M) \\
\downarrow & & \downarrow \mathbf{TS}(u) \\
\otimes \mathbf{TS}(u_\lambda) & & \\
\downarrow & & \\
\otimes \mathbf{TS}(N_\lambda) & \xrightarrow{h'} & \mathbf{TS}(N)
\end{array}
$$

通勤時間、$h$ と $h'$ は標準準同型です。なぜなら、$z \in TS(M_\lambda)$ で、$i_\lambda$ (それぞれ $j_\lambda$) が $M_\lambda$ の標準単射を $M$ (それぞれ $N$ を $N$ に) を表す場合、次のようになります。

$$
\mathbf{TS}(u)(h(z)) = \mathbf{TS}(u) \circ \mathbf{TS}(i_\lambda)(z) = \mathbf{TS}(u \circ i_\lambda)(z) =
$$
$$
= \mathbf{TS}(j_\lambda \circ u_\lambda)(z) = \mathbf{TS}(j_\lambda) \circ \mathbf{TS}(u_\lambda)(z) = h'(\mathbf{TS}(u_\lambda)(z)) .
$$

#### 命題 6 {#alg-iv-s5-prop-6 .statement tag=06D3}

— *$M$ を、部分加群のファミリー $(M_\lambda)_\lambda$ の直和である $A$ モジュールとします。それぞれの $M_\lambda$ が自由加群である場合、$\otimes_{\lambda \in L} \mathbf{TS}(M_\lambda)$ の $\mathbf{TS}(M)$ への標準準同型は同型です。*

$(e_{i,\lambda})_{i, I_\lambda}$を$M_\lambda$の基底とします。 $\nu \in \mathbf{N}^{(I_\lambda)}$には$e_{\nu,\lambda} = \prod_{i \in I_\lambda} \gamma_{\nu(i)}(e_{i,\lambda})$を入れます。 $TS(M_\lambda)$ (IV、p. 47、提案 4 (i)) および $e_{0,\lambda}$ の $\nu \in \mathbf{N}^{(I_\lambda)}$ 形基底の $e_{\nu,\lambda}$ は、$\mathbf{TS}(M_\lambda)$ の単位要素です。したがって元

$$
\otimes_{\lambda \in L} e_{\nu_{\lambda,\lambda}}
$$

ここで、$\nu_\lambda \in \mathbf{N}^{(I_\lambda)}$ と $\nu_\lambda = 0$ は、添字の有限数、$\otimes_A TS(M_\lambda)$ の形基底を除きます。 命題の標準準同型の下の元(9)の像は$\prod_{\lambda \in L} e_{\nu_{\lambda,\lambda}}$です。家族 $(e_{i,\lambda})_{i, I_\lambda}$ の $(e_i)_i$、互いに素和集合で表すと、上記の元は正確に $\prod_{i \in I} \gamma_{\nu(i)}(e_i)$ で、$\nu \in \mathbf{N}^{(I)}$ なので、$\mathbf{TS}(M)$ の基底を構成します。これは命題を証明します。

提案 6 の条件では、逆同型 $\mathbf{TS}(M) \to \otimes_{\lambda} \mathbf{TS}(M_\lambda)$ は *正規* とも呼ばれます。多くの場合、$\mathbf{TS}(M)$ はこの同型によって $\otimes_{\lambda} TS(M_\lambda)$ と同一視されます。 $z \in TS(M_\lambda)$と$z' \in \mathbf{TS}(M_{\mu})$が$\lambda \neq \mu$である場合、$z \otimes z'$によって示される$\mathbf{TS}(M)$の元は、$\mathbf{T}(M)$の$z$と$z'$のテンソル積ではなく、対称であることに注意する必要があります。 $z$と$z'$の積。

#### 命題 7 {#alg-iv-s5-prop-7 .statement tag=06D4}

*$M$を$A$モジュールとし、$M \oplus M$の$u$写像$(x, y) \mapsto x + y$を$M$と$f$を複合写像にします*

$$
\mathbf{TS}(M) \otimes \mathbf{TS}(M) \xrightarrow{h} \mathbf{TS}(M \oplus M) \xrightarrow{\mathbf{TS}(u)} \mathbf{TS}(M)
$$

*ここで、$h$は標準準同型です。 $z, z' \in \mathbf{TS}(M)$ の場合は、$f(z \otimes z') = zz'$。*

$i$ を $M$ の写像 $x \mapsto (x, 0)$ を $M \oplus M$ とします。 $u \circ i = \mathrm{Id}_M$ があるため、$\mathbf{TS}(u) \circ \mathbf{TS}(i) = \mathrm{Id}_{\mathbf{TS}(M)}$ になります。したがって

$$
f(z \otimes 1) = \mathbf{TS}(u)(h(z \otimes 1)) = \mathbf{TS}(u)(\mathbf{TS}(i)(z)) = z .
$$

$f(1 \otimes z') = z'$、よって $f(z \otimes z') = f(z \otimes 1) f(1 \otimes z') = zz'$も同様です。

### 7. 余積対称の場合テンソル

$M$ を *自由な* $A$ モジュールとし、$\Delta_M = A$ を $M$ の対角線準同型 $x \mapsto (x, x)$ を $M \oplus M$ にするとします。 $c_M = c$ を準同型で構成される段階的 $A$-代数の単位準同型とします。

$$
\mathbf{TS}(M) \xrightarrow{\mathbf{TS}(\Delta)} \mathbf{TS}(M \oplus M) \xrightarrow{\sigma} \mathbf{TS}(M) \otimes \mathbf{TS}(M)
$$

ここで、$\sigma$は標準同型です。 $c$ を装備し、$\mathbf{TS}(M)$ はグレード$A$-cogebra です。

すべての $x \in M$ とそれぞれの整数 $p \geq 0$ について、$\mathbf{TS}(A)(\gamma_p(x)) = \gamma_p((x, x))$ が得られるため、(8) により、

$$
c(\gamma_p(x)) = \sum_{r+s=p} \gamma_r(x) \otimes \gamma_s(x).
$$

特に

$$
c(x) = x \otimes 1 + 1 \otimes x .
$$

$(x_i)_{i \in I}$ を $M$ の元の家族とし、$\nu \in \mathbf{N}^{(I)}$ に $x_\nu = \prod_{i \in I} \gamma_{\nu_i}(x_i)$ を置きます。

それから

$$
c(x_\nu) = \sum_{\rho + \sigma = \nu} x_\rho \otimes x_\sigma .
$$

$c$ は代数準同型であるため、これは *(10)* から導き出されます。

#### 命題 8 {#alg-iv-s5-prop-8 .statement tag=06D5}

— M を自由A-加群とすると、その代数と余代数構造により、TS (M) は段階的可換および共可換双数になります。 余単位は A-線型写像 $\varepsilon : TS(M) \to TS^0(M) = A$ で、$TS^p(M)$ の $p > 0$ の零が$\varepsilon(1) = 1$ になります。

私たちは、A-代数 $TS(M)$ が結合的、可換的、および単体であることを知っています。一方、余積は、グレード代数の構成準同型によるものです。ここで、余代数 $TS(M)$ が共結合的かつ共可換であるという事実は、公式 (10) から簡単に計算できます。 $TS(M)$ の A への写像 $\varepsilon$ は、$\varepsilon(l) = l$ のように等級付けされた代数の準同型です。最後に、$p > 0$、$\varepsilon(\gamma_0(x)) = l$ の場合、$x \in M$ ごとに $\varepsilon(\gamma_p(x)) = 0$ が得られます。心に留めておけば (lo)、これは $(F \otimes 1) \circ c = (l \otimes E) \circ c = \mathrm{Id}_{TS(M)}$ であることを示しています。したがって、$E$ は $TS(M)$ の余単位です。

#### 命題 9 {#alg-iv-s5-prop-9 .statement tag=06D6}

— M と N を自由A-加群とし、 u を M から N への A 準同型とする。その場合、$\mathbf{TS}(u)$ はビジェブラ準同型です。

$\Delta_N \circ u = (u,u) \circ \Delta_M$ があるため、図式

$$
\begin{array}{ccccccccc}
\mathbf{TS}(M) & \xrightarrow{\mathbf{TS}(\Delta_M)} & \mathbf{TS}(M \oplus M) & \xrightarrow{\sigma} & \mathbf{TS}(M) \otimes \mathbf{TS}(M) \\
\downarrow \mathbf{TS}(u) & & \downarrow \mathbf{TS}(u,u) & & \downarrow \mathbf{TS}(u) \otimes \mathbf{TS}(u) \\
\mathbf{TS}(N) & \xrightarrow{\mathbf{TS}(\Delta_N)} & \mathbf{TS}(N \oplus N) & \xrightarrow{\tau} & \mathbf{TS}(N) \otimes \mathbf{TS}(N),
\end{array}
$$

ここで、$\sigma$ と $\tau$ は標準同型であり、可換です (IV, p. 49)。したがって、$c_N \circ \mathbf{TS}(u) = (\mathbf{TS}(u) \otimes \mathbf{TS}(u)) \circ c_M$。

#### 命題 10 {#alg-iv-s5-prop-10 .statement tag=06D7}

— M を自由A-加群とすると、大角 $\mathbf{TS}(M)$ の原始元 (III, p. 602) は M の元です。

$(e_i)_{i \in I}$ を M の基底とし、$\nu \in \mathbf{N}^{(I)}$ に $e_\nu = \prod_{i \in I} \gamma_{\nu_i}(e_i)$ を代入します。 $z = \sum_{\nu \in \mathbf{N}^{(I)}} \lambda_\nu e_\nu$ を $\mathbf{TS}(M)$ の元とすると、(12) によって次のようになります。

$$
c(z) = \sum_\nu \lambda_\nu \sum_{\rho, \sigma \in \mathbf{N}^{(I)}, \rho + \sigma = \nu} e_\rho \otimes e_\sigma = \sum_{\rho, \sigma} \lambda_{\rho + \sigma} e_\rho \otimes e_\sigma
$$

したがって

$$
c(z) - 1 \otimes z - z \otimes 1 = \sum_{\rho \neq 0, \sigma \neq 0} \lambda_{\rho + \sigma} e_\rho \otimes e_\sigma - \lambda_0 e_0 \otimes e_0
$$

それで

zプリミティブ $\Leftrightarrow \lambda_{\rho + \sigma} = 0$ $\rho \neq 0$、$\sigma \neq 0$、$\lambda_0 = 0$のとき
$|\nu| \neq 1$のとき$\Leftrightarrow \lambda_\nu = 0$
$\Leftrightarrow z \in M$。

### 8. TS(M)とS(M)の間の関係

TS(M) の M の標準単射拡大するを、独自の方法で T(M) の代数準同型を TS(M) に変換します (III、p. 485、提案 1)。 IV、p. 43 の提案 2、(ii) より、この準同型は対称化の演算子です。 代数 TS(M) は可換であるため、図式となるような代数 S(M) から代数 TS(M) への正規と呼ばれる、唯一の代数準同型 $\varphi_M$ が存在します (III, p. 497)

$$
\begin{array}{ccc}
T(M) & \xrightarrow{\rho} & S(M) \\
& & \searrow s \\
& & TS(M)
\end{array}
$$

ここで、$\rho$ は T(M) から S(M) への標準準同型を表し、可換です。 $p \in \mathbf{N}$全員に対して$\varphi_M(S^p(M)) \subset TS^p(M)$がございます。

一方、TS(M) の標準単射 i を T(M) に合成し、T(M) の標準準同型 $\rho$ を S(M) に合成すると、標準と呼ばれる等級付けされた A-加群の準同型 $\psi_M$ が得られます。 図式

$$
\begin{array}{ccc}
TS(M) & \xrightarrow{\psi_M} & S(M) \\
& & \downarrow \rho \\
& & T(M)
\end{array}
$$

可換です。

$u : M \to N$ が A-加群の準同型である場合、図式

$$
\begin{array}{ccccccccc}
S(M) & \xrightarrow{\varphi_M} & TS(M) & \xrightarrow{\psi_M} & S(M) \\
| & & | & & | \\
S(N) & \xrightarrow{\varphi_N} & TS(N) & \xrightarrow{\psi_N} & S(N)
\end{array}
$$

容易に検証できるように、 は可換です。

M が加群 $M_\lambda$ の直和である場合、図式 (14)

$$
\begin{array}{ccc}
\otimes S(M_\lambda) & \xrightarrow{\otimes \varphi_{M_\lambda}} & \otimes TS(M_\lambda) \\
\downarrow f & & \downarrow g \\
S(M) & \xrightarrow{\varphi_M} & TS(M),
\end{array}
$$

ここで、$f$ と $g$ は標準準同型であり、可換です。 $g \circ \otimes \varphi_{M_\lambda}$ と $\varphi_M \circ f$ は代数準同型で、$\lambda$ ごとに $M_\lambda$ では一致するになります。

#### 命題 11 {#alg-iv-s5-prop-11 .statement tag=06D8}

— *$M$が無料の場合、$\varphi_M$は重賞ビジェブラの射です。*

図式 (13) と (14) の可換性を使用すると、可換式の図式が得られます。

$$
\begin{array}{ccccccccc}
S(M) & \xrightarrow{S(\Delta)} & S(M \oplus M) & \xrightarrow{h} & S(M) \otimes S(M) \\
\downarrow \varphi_M & & \downarrow \varphi_{M \oplus M} & & \downarrow \varphi_M \otimes \varphi_M \\
TS(M) & \xrightarrow{TS(\Delta)} & TS(M \oplus M) & \xrightarrow{k} & TS(M) \otimes TS(M),
\end{array}
$$

ここで、$\Delta$ は対角線準同型であり、$h, k$ は標準準同型です。 命題はこれに続きます。

#### 命題 12 {#alg-iv-s5-prop-12 .statement tag=06D9}

— (i) *$u \in S^n(M)$の場合は、$\psi_M(\varphi_M(u)) = n!u$。*

(ii) *$v \in TS^n(M)$ の場合は、$\varphi_M(\psi_M(v)) = n!v$。*

$x_1, \ldots, x_n \in M$ と $u$ を $S(M)$ で計算される積 $x_1 \ldots x_n$ とします。すると、$\varphi_M(u)$は$TS(M)$で計算された積$x_1 \ldots x_n$、つまり

$$
\sum_{\sigma \in \mathfrak{S}_n} x_{\sigma(1)} \otimes \ldots \otimes x_{\sigma(n)}.
$$

したがって、$\psi_M(\varphi_M(u))$ は $S(M)$ で計算された $\sum_{\sigma \in \mathfrak{S}_n} x_{\sigma(1)} \ldots x_{\sigma(n)}$ に等しい、つまり

$$
n! x_1 \ldots x_n = n!u.
$$

$v = \sum_{i=1}^p x_1^i \otimes x_2^i \otimes \ldots \otimes x_n^i$ を $TS^n(M)$ の元とします。ここで、$x_j^i$ 属するから $M$ です。その場合、$\psi_M(v)$ は、$S(M)$、よってで計算された $\sum_{i=1}^p x_1^i x_2^i \ldots x_n^i$ と等しくなります。

$$
\varphi_M(\psi_M(v)) = \sum_{i=1}^p s(x_1^i \otimes x_2^i \otimes \ldots \otimes x_n^i) = s(v) = n!v.
$$

#### 系 1 {#alg-iv-s5-prop-12-cor-1 .statement tag=06DA}

— *$\mathbf{A}$ が $\mathbf{Q}$ 代数である場合、$S(M)$ の $TS(M)$ への標準準同型は代数同型です。さらに$M$がフリーなら重賞ビジェブラの同型です*。

#### 系 2 {#alg-iv-s5-prop-12-cor-2 .statement tag=06DB}

— *$A$が$\mathbf{Q}$-代数である場合、$TS(M)$の$M$の元のn番目の冪によって加群$TS^n(M)$が生成されます。
これはコルからの続きです。 1 と $S(M)$* (III、p. 498) の対応する性質。

### 9. 同次多項式写像

#### 命題 13 {#alg-iv-s5-prop-13 .statement tag=06DC}

— *$M$と$N$を$A$モジュール、$q$整数$\geqslant 0$、$M$の$f$写像を$N$にします。 $M$ が無料であると仮定すると、次の条件は同等です。
(i) すべての $x \in M$ に対して $f(x) = g(x, x, \ldots, x)$ となるような、$M^q$ の $N$ への $q$ 線形写像 $g$ が存在します。
(ii) すべての $x \in M$ に対して $f(x) = h(\gamma_q(x))$ となるような、$TS^q(M)$ から $N$ への線形写像 $h$ が存在します。
(iii) 次のような $M$ の基底 $(e_i)_{i \in I}$ と $N$ の要素の族 $(u_\nu)_{\nu \in N^{(I)}, |\nu| = q}$ が存在します。
$$
f\left( \sum_{i \in I} \lambda_i e_i \right) = \sum_{\nu \in N^{(I)}, |\nu| = q} \lambda^\nu u_\nu
$$
$(\lambda_i) \in A^{(I)}$の皆さんへ。
(iv) $M$ の各基底 $(e_i)_{i \in I}$ に対して、次のような $N$ の要素の族 $(u_\nu)_{\nu \in N^{(I)}, |\nu| = q}$ が存在します。
$$
f\left( \sum_{i \in I} \lambda_i e_i \right) = \sum_{\nu \in N^{(I)}, |\nu| = q} \lambda^\nu u_\nu
$$
$(\lambda_i) \in A^{(I)}$の皆さんへ。
(i) $\Rightarrow$ (ii): $g$ が (i) を満たすとすると、任意の $x, \ldots, x, \in M$ に対して $g(x_1, x_2, \ldots, x_q) = g'(x_1 \otimes x_2 \otimes \ldots \otimes x)$ となる、$T^q(M)$ から $N$ への線形写像 $g'$ が存在します。 それから
$$
f(x) = g(x, x, \ldots, x) = g'(x \otimes x \otimes \ldots \otimes x) = g'(\gamma_q(x));
$$
そして、$h = g'|TS^q(M)$ を書くと、条件 (ii) が成り立つことがわかります。
(ii) $\Rightarrow$ (i) と (iv): (ii) の $h$ 満たす条件とします。 提案 4、(ii) (IV、p. 47) により、$T^q(M)$ の $N$ に $h = g'|TS^q(M)$ となる線形写像 $g'$ が存在します。 $g$ を、$g'$ に関連付けられた $M$ から $N$ への $q$ 線形写像とすると、任意の $x \in M$ について次のようになります。
$$
f(x) = h(\gamma_q(x)) = g'(x \otimes x \otimes \ldots \otimes x) = g(x, x, \ldots, x),
$$

よって (i)。一方、$(e_i)_{i \in I}$ が M の基底である場合、公式 (6) (IV, p. 46) により、

$$
f \left( \sum_i \lambda_i e_i \right) = h \left( \gamma_q \left( \sum_i \lambda_i e_i \right) \right) = h \left( \sum_{|\nu|=q} \lambda^\nu e_\nu \right)
$$

$e_\nu = \prod_{i \in I} \gamma_{\nu_i}(e_i)$ を書くとき;したがって、私たちは

$$
f \left( \sum_i \lambda_i e_i \right) = \sum_{|\nu|=q} \lambda^\nu h(e_\nu).
$$

(iv) $\Rightarrow$ (iii) は明らかです。
(iii) $\Rightarrow$ (ii) : (iii) の $(e_i), (u_\nu)$ 満たす条件が与えられた場合、$e_\nu = \prod_{i \in I} \gamma_{\nu_i}(e_i)$ を書き、$(e_\nu)_{|\nu|=q}$ が $\mathrm{TS}^q(M)$ の基底であることを思い出してください。 h を $h(e_\nu) = u_\nu$ で定義される N に $\mathrm{TS}^q(M)$ の準同型とします。 M の各 $x = \sum_i \lambda_i e_i$ について、次のようになります。

$$
f(x) = f \left( \sum_i \lambda_i e_i \right) = \sum_{|\nu|=q} \lambda^\nu u_\nu = h \left( \sum_{|\nu|=q} \lambda^\nu e_\nu \right) = h(\gamma_q(x))
$$

#### 定義 3 {#alg-iv-s5-def-3 .statement tag=06DD}

— M と N を A-加群 、q 整数 $\geq 0$ とします。 M が *free* であると仮定し、$\mathrm{Pol}_A^q(M, N)$ または単に M の写像の $\mathrm{Pol}^q(M, N)$ 集合を提案 13 の N 満たす条件に表すとします。 $\mathrm{Pol}^q(M, N)$の元は、Mの次数qの同次多項式写像をNに呼び出します。

提案 13 (i) 定義する準同型の A-加群 :

$$
\mathscr{L}_q(M, ..., M; N) \to \mathrm{Pol}^q(M, N).
$$

提案 13 (ii) 定義する準同型/A-加群

$$
\mathrm{Hom}_A(\mathbf{TS}^q(M), N) \to \mathrm{Pol}^q(M, N).
$$

これらの準同型は正規と呼ばれます。彼らは客観的です。

#### 例 1 {#alg-iv-s5-n9-exa-1 .statement tag=06DE}

M の N への次数 1 の同次多項式マッピングは、M から N への A 線形マッピングです。

#### 例 2 {#alg-iv-s5-n9-exa-2 .statement tag=06DF}

$(N_i)_{i \in I}$ を M の A-加群、$f_i$ 写像を $N_i, i \in I$ に、$f : M \to \prod_{i \in I} N_i$ 写像を成分 $f_i$ とする家族とします。 f が次数 q の同次多項式写像であるためには、各 $f_i$ が次数 q の同次多項式写像であることが必要かつ十分です。

#### 例 3 {#alg-iv-s5-n9-exa-3 .statement tag=06DG}

$(M_j)_{j \in J}$ を自由A-加群の有限族とし、$u : \prod_{j \in J} M_j \to N$ を多重線形写像とします。この場合、u は次数 $\mathrm{Card}(J)$ の多項式になります。

#### 例 4 {#alg-iv-s5-n9-exa-4 .statement tag=06DH}

$(X_i)_{i \in I}$ を不定数の族、$N$ を $A$ 加群、$u \in N[(X_i)_{i \in I}]$ を次数 $q$ の同次多項式とします。 $A^{(I)}$ の $N$ へのマッピング $(x_i)_{i \in I} \mapsto u((x_i)_{i \in I})$ は、次数 $q$ の同次多項式マッピングです: これは、提案 13 の条件 (iii) によってすぐにわかります。 $I$ が有限である場合、次数 $q$ の $A^{(I)} = A'$ から $N$ へのすべての同次多項式写像は、その形のものになります。

#### 例 5 {#alg-iv-s5-n9-exa-5 .statement tag=06DI}

$A^{(N)}$ の $A$ へのマッピング $(x_i)_{i \in N} \mapsto x_0^2 + x_1^2 + \ldots + x_n^2 + \ldots$ は、次数 2 の同次多項式マッピングです。 $A = 2/22$ の場合、線形写像 $(x_i)_{i \in I} \mapsto x_0 + x_1 + \ldots + x_n + \ldots$ で一致する

#### 例 6 {#alg-iv-s5-n9-exa-6 .statement tag=06DJ}

$f \in \mathrm{Pol}_A^q(M, N)$、$B$ を $B$ の可換環、$\rho$ 準同型として、$M$ と $N$ から派生した $B$ モジュールを $A$ と $M'$ と $N'$ にします。 $\rho$の。 $M'$ が無料であると仮定します。次に $f \in \mathrm{Pol}_B^q(M', N')$: これは提案 13 の条件 (i) からすぐに続きます。

#### 命題 14 {#alg-iv-s5-prop-14 .statement tag=06DK}

— $M, N, P$ を $A$ モジュール、$q$ と $r$ 整数 $\geqslant 0$ とし、$M$ と $N$ が空いていると仮定します。 $f \in \mathrm{Pol}^q(M, N)$、$f' \in \mathrm{Pol}^r(N, P)$の場合は、$f' \circ f \in \mathrm{Pol}^{qr}(M, P)$。

$M^q$ から $N$ への $q$ 線形写像 $g$ と、$N^r$ から $P$ への $r$ 線形写像 $g'$ が存在します。

$$
\begin{aligned}
f(x) &= g(x, x, \ldots, x) & \text{for all } x \in M, \\
f'(y) &= g'(y, y, \ldots, y) & \text{for all } y \in N.
\end{aligned}
$$

したがって、$x \in M$ ごとに、

$$
f'(f(x)) = g'(f(x), f(x), \ldots, f(x)) = g'(g(x, x, \ldots, x), \ldots, g(x, x, \ldots, x))
$$

$M^{qr}$ の $P$ への写像 $(x_1, \ldots, x_{qr}) \mapsto g'(g(x_1, \ldots, x_q), \ldots, g(x_{q(r-1)+1}, \ldots, x_{qr}))$ は $qr$ 線形です。

#### 命題 15 {#alg-iv-s5-prop-15 .statement tag=06DL}

— $M$ を自由な $A$ モジュール、$N$ を $A$ モジュール、$q$ 整数 $\geqslant 0$ とします。 写像 $y \mapsto q!y$ は $N$ の自己同型であると仮定します。 $f \in \mathrm{Pol}^q(M, N)$ とすると、すべての $x \in M$ に対して $f(x) = h(x, x, \ldots, x)$ となるような、$M^q$ の $M$ への対称 $q$ 線形写像 $h$ が 1 つだけ存在します。 $x_1, \ldots, x_q \in M$ については、

$$
h(x_1, x_2, \ldots, x_q) = \frac{(-1)^q}{q!} \sum_{H \subset \{1, 2, \ldots, q\}} (-1)^{\mathrm{Card}\ H} f\left( \sum_{i \in H} x_i \right).
$$

a) すべての $x \in M$ に対して $f(x) = g(x, x, \ldots, x)$ となるような、$M^q$ の $N$ への$q$ 線形写像 $g$ が存在します。 $M$ から $N$ への定義する $q$ 線形写像 $h$ を考えてみましょう。

$$
h(x_1, x_2, \ldots, x_q) = \frac{1}{q!} \sum_{\sigma \in S_q} g(x_{\sigma(1)}, x_{\sigma(2)}, \ldots, x_{\sigma(q)}).
$$

すると、$h$ は対称であり、すべての $x \in M$ に対して $f(x) = h(x, x, \ldots, x)$ になります。

b) $h$ を、f(x) = g(x, x, ..., x) となる $M^q$ から $N$ への対称 $q$ 線形写像とする。 l を T^q(M) の線形写像を N に変換し、任意の x_1, ..., x_q \in M に対して h(x_1, ..., x_q) = l(x_1 \otimes ... \otimes x_q) とします。

$$
(-1)^q q! h(x_1, ..., x_q) = (-1)^q \sum_{\sigma \in S_q} h(x_{\sigma(1)}, ..., x_{\sigma(q)}) =
= (-1)^q l(s(x_1 \otimes ... \otimes x_q)) = \sum_{H \subset \{1, ..., q\}} (-1)^{\text{Card } H} l \left( \gamma_q \left( \sum_{i \in H} x_i \right) \right)
$$

提案 3、(v) (IV、p. 45) による。今

$$
l \left( \gamma_q \left( \sum_{i \in H} x_i \right) \right) = h \left( \sum_{i \in H} x_i, ..., \sum_{i \in H} x_i \right) = f \left( \sum_{i \in H} x_i \right)
$$

これは h の公式 (16) と一意性を証明します。

#### 命題 16 {#alg-iv-s5-prop-16 .statement tag=06DM}

— *Hom ($\mathbf{TS}^q(M)$, N) の M を自由A-加群、N A-加群、q 正の整数、u 標準準同型を$\mathbf{Pol}^Y(M, N)$ とする。

(i) *A が無限大整域で、N がねじれのない場合、u は同型です。*

(ii) *N の写像 $y \mapsto q!y$ が単射であれば、u は同型です。*

命題の 2 つの場合では、u が単射であること、つまり、$\gamma_q(M)$ 上の零である N への $\mathbf{TS}^q(M)$ のすべての線形写像 f が消滅することを証明する必要があります。

A が無限大整域であり、N はねじれがないと仮定します。すべての $z \in \mathbf{TS}^q(M)$ に対して、$az$ が y, (M) の元の A 線形結合であるような $a \in A - \{0\}$ が存在します (*IV*, p. 47、提案 5)。したがって、$af(z) = f(az) = 0$、そして$f(z) = 0$です。

次に、 N の写像 $y \mapsto q!y$ が単射であると仮定すると、 *IV*, p. 45 、提案 3 (v) により、 f は s 上で消滅します。て^q(M)。したがって、$z \in \mathbf{TS}^q(M)$ の場合、$q!f(z) = f(sz) = 0$ があり、したがって $f(z) = 0$ になります。

#### 系 {#alg-iv-s5-n9-cor-1 .statement tag=06DN}

— *M を M の自由A-加群、N A-加群、q 正の整数、$h \in \mathbf{Pol}^q(M, N)$、および $(e_i)_i$、基底とします。提案 16 の 2 つのケースでは、次のような N の元の固有の族 $(u,$、$\mathbf{N}^{(I)}, |\cdot|$、 、が存在します。 $h \left( \sum_{i \in I} \lambda_i e_i \right) = \sum_{|\nu| = q} \lambda^\nu u_\nu$ 全員$(\lambda_i) \in \mathbf{A}^{(1)}$*

### 10. 多項式写像

#### 定義 4 {#alg-iv-s5-def-4 .statement tag=06DO}

— *M と N を A-加群とし、M が自由であると仮定します。 写像(M, N) を、M を N に変換したすべての写像の A-加群とします。 写像(M, N) の部分加群 $\sum_{q > 0} \mathbf{Pol}_A^q(M, N)$ は、$\mathbf{Pol}_A(M, N)$ または単に $\mathbf{Pol}(M, N)$ で表されます。その元は M から N への多項式写像と呼ばれます。*

$(e_i)_{i \in I}$ を M の基底とし、$l$ が有限であると仮定します。提案 13 による (IV, p. 54) 写像 $f$ の M から N は、N に係数をもつ不定数 $X_i$ に多項式 F が存在する場合に限り、多項式になります。

$$
f \left( \sum_{i \in I} x_i e_i \right) = F(x)
$$

$A^{(I)}$ のすべての家族 $x = (x_i)_{i \in I}$ に。この性質は M に選択された基底とは独立しており、« 多項式写像 » という用語が正当化されます。

#### 命題 17 {#alg-iv-s5-prop-17 .statement tag=06DP}

— *M を自由A-加群とし、B を結合的、可換的、単位的 A-代数とします。この場合、$\mathrm{Pol}_A(M, B)$ は代数 $\mathrm{Map}(M, B)$ の部分 B 代数です。

これはDefから続きます。 4 および提案 13、(iv) (IV、p. 54)。

#### 命題 18 {#alg-iv-s5-prop-18 .statement tag=06DQ}

— *M、N、P を A-加群とし、M と N が自由であると仮定します。 $f \in \mathrm{Pol}(M, N)$、$g \in \mathrm{Pol}(N, P)$ の場合は、$g \circ f \in \mathrm{Pol}(M, P)$。

$g \in \mathrm{Pol}^q(N, P)$ のような整数 q が存在する場合、すぐに簡約するを行うことができます。その場合、すべての $y \in N$ に対して $g(y) = h(y, y, \ldots, y)$ となるような、$N^q$ の P への q 線形写像 $h$ が存在します。 $f$ を同次多項式写像の和として書くと、写像は証明に減ります。

$$
x \mapsto h(f_1(x), f_2(x), \ldots, f_q(x))
$$

M を P に変換します。ここで、$f_i \in \mathrm{Pol}^{q_i}(M, N)$ は多項式です。 $i = 1, \ldots, q$ については、すべての $x \in M$ に対して $f_i(x) = l_i(x, x, \ldots, x)$ となるような、N への $M^{q_i}$ の $q_i$ 線形マッピング $l_i$ が存在します。したがって、

$$
h(f_1(x), f_2(x), \ldots, f_q(x)) = h(l_1(x, \ldots, x), \ldots, l_q(x, \ldots, x)),
$$

そこから私たちの主張が続きます。

#### 補題 2 {#alg-iv-s5-lem-2 .statement tag=06DR}

— *N を A-加群、n 整数 $\geq 0$ とし、*

$$
f = m_0 + m_1 X + \cdots + m_n X^n \in N[X].
$$

*$f(\alpha_0) = \cdots = f(\alpha_r) = 0$ となるような $\alpha_0, \alpha_1, \ldots, \alpha_r \in A$ が存在し、N の比 $\alpha_i - \alpha_j$ の $i \neq j$ ホモテティー が単射となるような $f = 0$ が存在すると仮定します。*

(この補題は、IV、p. 16 の Cor. を一般化します。)

補題は明らかに $n = 0$ に当てはまります。 $n$の帰納法までに証明しましょう。我々は持っています

$$
f(X) = f(X) - f(\alpha_0) = \sum_{i=1}^n m_i (X^i - \alpha_0^i) = (X - \alpha_0) g(X)
$$

ここで g は形 $m_0' + m_1' X + \ldots + m_{n-1}' X^{n-1}$ の N[X] の元です。 補題の仮説は、$g(\alpha_1) = \cdots = g(\alpha_r) = 0$、したがって帰納法の仮定によって $g = 0$、したがって $f = 0$ を意味します。

#### 命題 19 {#alg-iv-s5-prop-19 .statement tag=06DS}

— *M を自由A-加群、N A-加群、G を A の無限加法部分群とし、G の非零元によって定義される N の相同性が単射であると仮定します。この場合、Pol(M, N) は Pol$^q$(M, N) の直和となります。*

$f_0, f_1, \ldots, f_n$ が $f_i \in \mathrm{Pol}^i(M, N)$ となるようにし、関係 $f_0 + \ldots + f_n = 0$ があると仮定します。 $x \in M$ とすれば、すべての $\lambda \in G$ は次のようになります。
$$
0 = \sum_{i=0}^n f_i(\lambda x) = \sum_{i=0}^n \lambda^i f_i(x).
$$
補題 2 を多項式 $\sum_{i=0}^n f_i(x) X^i$ に適用すると、次のようになります。
$$
f_0(x) = \cdots = f_n(x) = 0
$$

#### 系 {#alg-iv-s5-n10-cor-1 .statement tag=06DT}

— *A が無限大整域であると仮定します。 M を自由A-加群、N をねじりのない A モジュールとします。*

(i) *$\mathrm{Pol}(M, N) = \bigoplus_{q \geq 0} \mathrm{Pol}^q(M, N)$ があり、各 $\mathrm{Pol}^q(M, N)$ は正規的に $\mathrm{Hom}(\mathbf{T S}^q(M), N)$ で識別される可能性があります。*

(ii) *M の $f \in \mathrm{Pol}(M, N)$ と $(e_i)_i$、基底を仮定します。すべての $(\lambda_i) \in A^{(I)}$ に対して $f \left( \sum_{i \in I} \lambda_i e_i \right) = \sum_{\nu \in N^{(I)}} \lambda^\nu u_\nu$ となるような、N の元の $(u_\nu)_{\nu \in N^{(I)}}$ が 1 つだけ存在します。*

主張 (i) 提案 16 および 19 に従う、および (ii) (i) および Cor.提案16の。

### 11. $\mathbf{S}(M^*)$、TS(M)*gr と Pol(M, A) の間の関係

M を自由A-加群とすると、TS(M) (III, p. 580) の級数コジェブラッド構造から導出された、可換、結合、単元級数 $^1$ 代数の構造を級数双対 TS(M)*gr に装備します。 III、p. 497 までに、グレード付けされた A-代数のうち一意な準同型が存在します。
$$
\theta : \mathbf{S}(M^*) \to \mathbf{TS}(M)^{*gr}
$$
M* の次数 1 恒等写像に誘導します。

$^1$ TS(M) の次数 – k の準同型を A に格付けしたものは、ここでは TS(M)*gr (II, p. 377) の次数 k の元と見なされます。

#### 命題 20 {#alg-iv-s5-prop-20 .statement tag=06DU}

— *A-加群 M が自由で有限に生成される場合、$0$ は等級付けされた代数の同型です。*

$(e_i)_{i \in I}$ を $M$ の基底および $M^*$ の $(e_i^*)_{i \in I}$ 双対基底とします。 $\nu \in \mathbf{N}^I$の場合は

$$
e_\nu = \prod_{i \in I} \gamma_{\nu_i}(e_i) \in \mathbf{TS}(M)
$$

提案 4 (*IV*, p. 47) により、ファミリー $(e_\nu)_\nu,_{\mathbf{N}^I}$ は $TS(M)$ の基底です。 $(e_\nu^*)$ を $\mathbf{TS}(M)^{*gr}$ と $(e_\nu)$ の双対である基底とします。 III、p. 505、Th に照らして。 1 任意の $\nu \in \mathbf{N}^I$ について、

$$
e_\nu^* = \prod_{i \in I} (e_i^*)^{\nu_i},
$$

または、$\rho, \sigma \in \mathbf{N}^I$ には $e_\rho^* \cdot e_\sigma^* = e_{\rho + \sigma}^*$ があるとも言えます。しかし、この最後の主張は *IV*、p. 50、公式 (12) から続きます。

#### 注意 1 {#alg-iv-s5-n11-rem-1 .statement tag=06DV}

— 同様に、$M$ が有限生成された自由な $A$ モジュールである場合、III、p. 593 で定義される等級付けされた代数 $S(M)^{*gr}$ は $TS(M^*)$ で識別できることがわかります。

#### 命題 21 {#alg-iv-s5-prop-21 .statement tag=06DW}

— *標準準同型/A-加群* (*IV*、p. 55)

$$
u : \mathbf{TS}(M)^{*gr} \to \mathrm{Pol}_A(M, A)
$$

*は代数準同型です*

$a \in \mathbf{TS}^q(M)^*, b \in TS^r(M)^*, x \in M$ にしましょう。我々は持っています

$$
u(ab)(x) = \langle ab, \gamma_{q+r}(x) \rangle = \langle a \otimes b, c(\gamma_{q+r}(x)) \rangle =
= \langle a \otimes b, \gamma_q(x) \otimes \gamma_r(x) \rangle = \langle a, \gamma_q(x) \rangle \langle b, \gamma_r(x) \rangle = u(a)(x) \cdot u(b)(x),
$$

よって結果。

#### 注意 {#alg-iv-s5-n11-rem-2 .statement tag=06DX}

— 2) 合成準同型 $A, = u \circ 0 : S(M^*) \to \mathrm{Pol}_A(M, A)$ は、代数の固有の単位準同型であり、

$$
M^* = \mathrm{Pol}^1(M, A)
$$

$\mathrm{Pol}(M, A)$で。 $M$ が有限生成自由であり、$A$ が無限の整域である場合、$\lambda_M$ は全単射です (提案 20 および提案 19 の補正)。 特に、$A$ が無限整域の場合、$A[X_1, \ldots, X_n]$ の $\mathrm{Pol}(A^n, A)$ (*IV*, p. 4) への正準準同型写像 $f \mapsto \tilde{f}$ は同型写像です。

3) 余積 $c_S : S(M^*) \to S(M^* \times M^*)$ (III、p. 575、例 6) を考えてみましょう。任意の $v \in S(M^*)$、$x, y \in M$ について、多項式写像 $\lambda_{M \times M}(c_S(v)) : M \times M \to A$ 写像 $(x, y)$ ～ $A, (v)(x + y)$。このように定義された $S(M^*)$ から $\mathrm{Map}(M \times M, A)$ への 2 つの代数準同型は、関係のおかげで $M^*$ に一致します。

$$
(v \otimes 1 + 1 \otimes v)(x, y) = v(x + y) \quad (v \in M^*)
$$

### 練習問題 {#alg-iv-s5-exercises}

[§ 5 に対して練習問題](exercises/s5/)を参照してください。
