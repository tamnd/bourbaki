---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VI
chapter_title: ROOT SYSTEMS
section: 3
section_title: Exponential invariants
lang: ja
source: lie-iv-vi
pdf_pages: 0207-0213, 0254-0254
extraction: ocr
subsections:
    - "no": 1
      title: GROUP ALGEBRA OF A FREE ABELIAN GROUP
      page: 0
      pdf_page: 207
    - "no": 2
      title: CASE OF THE GROUP OF WEIGHTS; MAXIMAL TERMS
      page: 0
      pdf_page: 208
    - "no": 3
      title: ANTI-INvariant ELEMENTS
      page: 0
      pdf_page: 209
    - "no": 4
      title: INVARIANT ELEMENTS
      page: 0
      pdf_page: 212
statements: 13
exercises: 2
content_sha256: ec772d2e41561e35fe219c3ef762b66dc12c1674e9b0b2faab5df4db9c143699
translated_from: content/en/lie/VI/03_s3_exponential_invariants.md
translation_method: google
source_content_sha256: b9746d131eb1272ab4f94dead490215a8154be0c1a153b0693388de4edd688ad
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: d6f79bbad1a661d03e4c8d959096505323bf777412d3e517954cc1ad02e09e63
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 3。指数不変量

この切断では、文字Aは単位元を伴う可換環を表し、0には減りません。

### 1. 群代数 (無料アーベル群)

P を有限階数 $l$ の自由な $\mathbf{Z}$ モジュールとする。 We denote by $A[P]$ the group algebra of the additive group of P over A (*Algebra*, Chap. III, § 2, no. 6). 任意の $p \in P$ については、$A[P]$ の $e^p$ 対応する元で表します。 この場合、$(e^p)_{p \in P}$ は A-加群 $A[P]$ の *基底* であり、任意の $p, p' \in P$ について、次のようになります。
$$
e^p e^{p'} = e^{p + p'}, \quad (e^p)^{-1} = e^{-p}, \quad e^0 = 1.
$$

#### 補題 1 {#lie-vi-s3-lem-1 .statement tag=0AXN}

*Assume that A is factorial* (*Commutative Algebra*, Chap. VII, § 3, no. 1, Def. 1).
(i) *The ring $A[P]$ is factorial.*
(ii) *If $u, v$ are non-proportional elements of P, the elements $1 - e^u, 1 - e^v$ of $A[P]$ are relatively prime.*

$(p_1, p_2, \ldots, p_l)$ を P の基底とし、$X_1, X_2, \ldots, X_l$ を不定とします。 $X_1^{n_1} X_2^{n_2} \ldots X_l^{n_l}$ ($n_1, n_2, \ldots, n_l \in \mathbf{Z}$) から $e^{n_1 p_1 + \cdots + n_l p_l}$ に至る$A[X_1, \ldots, X_l, X_1^{-1}, \ldots, X_l^{-1}]$ から $A[P]$ までの A 線形写像は、環の同型です。ここで、$A[X_1, \ldots, X_l]$ は階乗環 (*可換代数*、第 VII, § 3, no. 5)、$A[X_1, \ldots, X_l, X_1^{-1}, \ldots, X_l^{-1}]$ は $A[X_1, \ldots, X_l]$ の分数の環であるため、これも階乗です。

$P'$ (それぞれ $P''$) を P の元の集合とし、そのうちのいくつかは倍数属するから $\mathbf{Z}u + \mathbf{Z}v$ (それぞれ $\mathbf{Z}u$) です。このとき、群 $P/P'$ と $P'/P''$ はねじれがないため、$P'$ には $P''$ の補数が存在し、P には $P'$ の補数が存在します。その結果、$\mathbf{Z}$ 加群 P の基底 $(z_1, z_2, \ldots, z_l)$ が存在し、有理数整数 $j, m, n$ は $u = jz_1, v = mz_1 + nz_2, j > 0, n > 0$ になります。 $1 \leq i \leq l$ に $X_i = e^{z_i}$ を代入すると、$1 - e^u = 1 - X_1^j, 1 - e^v = 1 - X_1^m X_2^n$ になります。 K を A の体の分数の代数閉包とすると、$A[P]$ は環 $B = K[X_1, \ldots, X_l, X_1^{-1}, \ldots, X_l^{-1}]$ の部分環と識別できます。 単位元 $z$ の $j$ 番目の根では、$1 - zX_1$ が極値になります。
$$
K[X_1, \ldots, X_l];
$$
さらに、$1 - zX_1$ 含むによって生成される理想は、$X_i$ に単項式はありません。私たち結論するは、Bの理想$(1 - zX_1)B$が高さ1の素理想であると考えます。

(可換代数、第 VII, § 1, no. 6)、従って、$1 - zX_1$ は B の極値です。従って、B の $1 - X_1^j$ の極値因子は、形 $1 - zX_1$ です。さて、B の因子割る $1 - X_1^m X_2^n$ はどれも (準同型 $f$ については、B から B まで、$i \geq 2$ の $f(X_1) = z^{-1}, f(X_i) = X_i$ は満たされません)

$$
f(1 - zX_1) = 0 \quad \text{and} \quad f(1 - X_1^m X_2^n) = 1 - z^{-m} X_2^n \neq 0).
$$

従って、$1 - X_1^j$ と $1 - X_1^m X_2^n$ は B で相対的に素です。その結果、$A[P]$ の$1 - X_1^j$ と $1 - X_1^m X_2^n$ の共通の因子は B で反転可能であるため、形の元による乗法までは可逆です。 $X_1^{k_1} X_2^{k_2} \ldots X_l^{k_l}$、A の元 $a$ に等しい。他の語, $a$ 割る 1 は A において、従って A において可逆です。 従って、最終的に、$1 - X_1^j$ と $1 - X_1^m X_2^n$ は $A[P]$ において互いに素です。

### 2. 重みの群の場合。最大項

前の数の記法を保持し、Rを実数ベクトル空間Vの約根系とします。この切断の残りでは、R (§ 1, no. 9) の重みの P 群をとります。 群 $W = W(R)$ は P に作用するため、代数 $A[P]$ にも作用します。 $w \in W$と$p \in P$には$w(e^p) = e^{w(p)}$があります。

C を R のチャンバー (§ 1, no. 5) とし、$B = (\alpha_i)_{1 \leq i \leq l}$ を R の対応する基底とします。 C によって定義される位数構造を含む V (従って P) を提供します。 $p, p' \in P, p \geq p'$の場合、$p - p'$が$\alpha_i$の線形結合で正の係数である場合に限ります。

#### 定義 1 {#lie-vi-s3-def-1 .statement tag=0AXO}

$x = \sum_{p \in P} x_p e^p$を$A[P]$の元とします。 $x_p \neq 0$ が x のサポートと呼ばれるような $p \in P$ の集合 S は x のサポートと呼ばれ、S の極大元の集合 X は x の最大サポートと呼ばれます。 項 $x_p e^p$ と $p \in X$ は、x の最大値項と呼ばれます。

#### 補題 2 {#lie-vi-s3-lem-2 .statement tag=0AXP}

$x \in A[P]$ と $(x_p e^p)_{p \in X}$ を x の最大値項の族とする。 $q \in P$ と $y \in A[P]$ を、$e^q$ が y の一意の最大値項となるようにします。すると、$xy$ の最大項の族は $(x_p e^{p+q})_{p \in X}$ になります。

$x = \sum_p x_p e^p, y = \sum_r y_r e^r$と$xy = \sum_t z_t e^t$を入れます。次に、$y_r \neq 0$ と $z_t = \sum_{p+r=t} x_p y_r$ など、すべての $r \in P$ に対して $r \leq q$ になります。

$t = p + q = p' + r$ と $p \in X$ および $x_{p'} y_r \neq 0$ の場合、$r \leq q$、従って $p' \geq p$、その結果 $p' = p$ となります。従って、$z_{p+q} = x_p y_q = x_p \neq 0$。これは、$X + q$が積$xy$のサポートに含まれていることを示しています。

一方、$t = p' + r$と$x_{p'} y_r \neq 0$の場合、$p' \leq p$となるような$p \in X$が存在し、$t \leq p + q$が得られます。従って、$xy$ の最大のサポートは $X + q$ に含まれます。 $X + q$ の 2 つの元は比較できないため、$X + q$ は正確に $xy$ の最大サポートであることがわかり、上で$p \in X$ の $z_{p+q} = x_p$ が確認され、補題の証明が完成します。

#### 注意 {#lie-vi-s3-n2-rem-1 .statement tag=0AXQ}

$x \neq 0$ は、$x$ の最大サポートが空ではないことを意味するため、補題 2 は、$y$ が形 $e^q$ の一意の最大値項を認めるときは常に、$x \neq 0$ が $xy \neq 0$ を意味することを示します。

### 3. 反不変式元

前の数の記法を保持します。 元 $w \in W$ の $\varepsilon(w)$ 行列式で表します。したがって、
$$
\varepsilon(w) = (-1)^{l(w)},
$$
長さ $l(w)$ は、反射のファミリー $s_{\alpha_i}$ と相対的に取られます。

#### 定義 2 {#lie-vi-s3-def-2 .statement tag=0AXR}

*元* $x \in A[P]$ *は* $W$ *if* の下で反不変であると言われます
$$
w(x) = (-1)^{l(w)}.x
$$
*全員に* $w \in W$。

$A[P]$ 形の反不変式元と $A[P]$ の $A$ サブモジュール。 $x \in A[P]$ については、
$$
J(x) = \sum_{w \in W} \varepsilon(w).w(x).
$$
(1)

$x \in A[P]$ と $w \in W$ については、
$$
w(J(x)) = \sum_{v \in W} \varepsilon(v).wv(x) = \varepsilon(w) \sum_{v \in W} \varepsilon(v).v(x) = \varepsilon(w).J(x)
$$
$J(x)$ は反不変です。一方、$q = \mathrm{Card}(W)$としましょう。 $A[P]$ の反不変式元 $x$ については、$J(x) = q.x$ が得られます。その結果、$q$ が $A$ で可逆である場合、写像 $q^{-1}J$ は反不変式元の $A[P]$ から部分加群への *射影* になります。

$\overline{\omega}_1, \ldots, \overline{\omega}_l$ をチャンバー $C$ の基本となる重み対応するとします。 $P \cap \overline{C}$ (それぞれ $P \cap C$) の要素は、$1 \leq i \leq l$ (§ 1, no. 10) の $n_i \geq 0$ (それぞれ $n_i > 0$) を含む形式 $n_1 \overline{\omega}_1 + \cdots + n_l \overline{\omega}_l$ の重みです。 一方、
$$
\rho = \overline{\omega}_1 + \cdots + \overline{\omega}_l
$$
は正の根 (*loc. cit.*) の半分和なので、$P \cap C$ の元は形 $\rho + p$ の重みと $p \in P \cap \overline{C}$ です。 最後に、$p \in P \cap C$ の場合、すべての $w \neq 1$ (§ 1, no. 6、提案 18 への修正) に対して $w(p) < p$ となり、$e^p$ は$J(e^p)$ の一意の最大値項になります。

#### 命題 1 {#lie-vi-s3-prop-1 .statement tag=0AXS}

*2 が * $A$ に零因子ではない場合、* 元* $J(e^p)$ *for* $p \in P \cap C$ *形基底の加群の反不変式元の * $A[P]$。

$w \in W$ と $p \in P \cap C$ の重み $w(p)$ はペアごとに区別されます。したがって、$p \in P \cap C$ の $J(e^p)$ は線形独立です。

一方、$x = \sum_p x_p e^p$ を $A[P]$ の反不変式元とします。壁に対して $p_0$ 属するの場合、反射 $s \in W$ の下では不変であり、
$$
x = \sum_p x_p e^p = -s(x) = -\sum_p x_p e^{s(p)}.
$$
したがって、$2x_{p_0} = 0$ なので、$x_{p_0} = 0$ になります。どの壁にも属するを持たないすべての元は、形 $w(p)$ と $w \in W$ および $p \in P \cap C$ で一意に書き込むことができるため、次のようになります。
$$
x = \sum_{p \in P \cap C} \sum_{w \in W} x_{w(p)} e^{w(p)}. \tag{2}
$$
$w(x) = \sum_p x_p e^{w(p)} = \varepsilon(w) \sum_p x_p e^p$、$x_{w(p)} = \varepsilon(w)x_p$ なので、(2) から次のように推測されます。
$$
x = \sum_{p \in P \cap C} x_p J(e^p),
$$
これで証明は完了です。

ここで、次のように定義された代数 $A[\frac{1}{2}P]$ の元 $d$ を考えてみましょう。
$$
d = \prod_{\alpha \in R, \alpha > 0} (e^{\alpha/2} - e^{-\alpha/2}) \\
= e^{\rho} \cdot \prod_{\alpha \in R, \alpha > 0} (1 - e^{-\alpha}) \\
= e^{-\rho} \cdot \prod_{\alpha \in R, \alpha > 0} (e^{\alpha} - 1).
$$
$\rho \in P$、$d \in A[P]$以来。

#### 命題 2 {#lie-vi-s3-prop-2 .statement tag=0AXT}

(i) * (3) で定義される要素 d は、A[P] の反不変要素です。その固有の最大項* (no. 2、定義1) *は* $e^{\rho}$ *および* $d = J(e^{\rho})$です。
(ii) *任意の* $p \in P$ について、*要素* $J(e^p)$ *は* $d$ *で一意に割り切れます*、そして商* $J(e^p)/d$ *は* $A[P]$ *$W$の下で不変です*。
(iii) *2 が * $A$ のゼロ除数ではない場合、*乗算* $d$ *は * $A[P]$ *不変条件下* $W$ *の反不変要素のセット* $A[P]$ の要素の集合からの全単射です。

$1 \leq i \leq l$ の場合、反射 $s_i = s_{\alpha_i}$ は、$\alpha_i$ と $s_i(\alpha_i) = -\alpha_i$ 以外の正の根の安定した集合を残すことがわかります (§ 1, no. 6、提案 17 の Cor. 1)。したがって、
$$
s_i(d) = (e^{-\alpha_i/2} - e^{\alpha_i/2}) \prod_{\alpha \in R, \alpha > 0, \alpha \neq \alpha_i} (e^{\alpha/2} - e^{-\alpha/2}) \\
= -d = \varepsilon(s_i).d.
$$
$s_i$ 生成する $W$ なので、(i) の最初の主張が証明されます。 (i) の 2 番目の主張は、(3) と補題 2 の直後に続き、1 が $\alpha \in R, \alpha > 0$ に対する $1 - e^{-\alpha}$ の一意の最大値項であることに注意してください。

ここで$A = \mathbf{Z}$と仮定します。提案 1 により、

$$
d = \prod_{p \in P \cap C} c_p J(e^p) \quad \text{with} \quad c_p \in \mathbf{Z}.
$$

一方で、明らかになっているのは、

$$
d = e^\rho + \sum_{q < \rho} c'_q e^q.
$$

$p \neq \rho$で$p \in P \cap C$なら、$d$の$e^p$の$p > \rho$と係数は(5)により零になります。したがって、$c_p = 0$。さらに、(4)と(5)の$e^\rho$の係数を比較すると、$c_\rho = 1$、したがって$d = J(e^\rho)$であることがわかります。

引き続き $A = \mathbf{Z}$ と仮定します。 $p \in P, \alpha \in \mathbf{R}$ と $M$ を、部分群 $\{1, s_\alpha\}$ に関する$W$ の右剰余類の代表の系とします。それから、

$$
J(e^p) = \sum_{w \in M} \varepsilon(w) e^{w(p)} + \sum_{w \in M} \varepsilon(s_\alpha w) e^{s_\alpha w(p)}.
$$

現在 $s_\alpha w(p) = w(p) - \langle \alpha^*, w(p) \rangle \alpha = w(p) + n_w \alpha$ は $n_w \in \mathbf{Z}$ です。したがって、

$$
J(e^p) = \sum_{w \in M} \varepsilon(w) e^{w(p)} (1 - e^{n_w \alpha}).
$$

$n_w \geq 0$ の場合、$1 - e^{n_w \alpha}$ は $1 - e^\alpha$ で割り切れることは明らかであり、これは $1 - e^{n_w \alpha} = -e^{n_w \alpha}(1 - e^{-n_w \alpha})$ 以降の $n_w < 0$ の場合にも当てはまります。したがって、$J(e^p)$は$\mathbf{Z}[P]$の$1 - e^\alpha$で割り切れます。

補題 1 により、$\mathbf{Z}[P]$ は階乗、$\alpha \in \mathbf{R}$ と $\alpha > 0$ の元 $1 - e^\alpha$ は互いに素です。したがって、$J(e^p)$ は $\mathbf{Z}[P]$ で積 $\prod_{\alpha > 0} (1 - e^\alpha)$ で割り切れ、したがって $d = e^{-\rho} \prod_{\alpha > 0} (1 - e^\alpha)$ でも割り切れます。

一般的なケースに戻ると、$\mathbf{Z}$ から $A$ までのスカラーの拡大により、上記から $d = J(e^\rho)$ と、すべての元 $J(e^p)$ は $d$ で割り切れると推定されます。 $e^\rho$ は $d$ の一意の最大値項であるため、no. 2 の注意は、$J(e^p) = dy$ となる一意元 $y \in A[P]$ が存在することを示し、直ちに$y$ は$W$ の下で不変であることがわかり、したがって次のようになります$d$ と $J(e^p)$ は反不変です。これにより、(i) と (ii) が証明されます。

最後に、2 が $A$ の零因子ではない場合、no. 2 の注意と提案 1 は (iii) を意味します。

#### 注意 1 {#lie-vi-s3-n3-rem-1 .statement tag=0AXU}

2 が $A$ の零因子ではない場合、$d$ が $e^\rho$ を最大値項とする $A[P]$ の一意の反不変式元であることを確認するのは簡単です。

#### 注意 2 {#lie-vi-s3-n3-rem-2 .statement tag=0AXV}

no. 2 の補題 2 は、商 $J(e^p)/d$ ($p \in P \cap C$ の場合) の一意の最大値項が $e^{p-\rho}$ であることを示しています。

### 4. 不変式元

$A[P]^W$ を、$W$ の下で不変である $A[P]$ のからなる 、元の部分代数とします。 $p \in P$ について、$W$ の下での $p$ の軌道を $W.p$ で表し、$S(e^p) = \sum_{q \in W.p} e^q$ を $e^p$ の $W$ 変換の合計とします。これは $W$ 不変要素です。

$p \in P \cap \overline{C}$ の場合、すべての $w \in W$ ($\S$ 1、no. 6、提案 18) に対して $w(p) \leq p$ となり、$e^p$ は $S(e^p)$ の一意の最大値項になります。

$x = \sum_p x_p e^p \in A[P]^W$ にしましょう。次に、すべての $p \in P$ とすべての $w \in W$ に対して $x_{w(p)} = x_p$ を返します。

一方、$P$ の $W$ のすべての軌道は、ちょうど 1 つの点 ($\S$ 1、no. 5、Th. 2) で $P \cap \overline{C}$ と一致します。したがって、

$$
x = \sum_{P \cap \overline{C}} x_p S(e^p).
$$

私たちは次のように推測します。

#### 補題 3 {#lie-vi-s3-lem-3 .statement tag=0AXW}

*$S(e^p)$ は、$A$ モジュール $A[P]^W$ の $p \in P \cap \overline{C}$ 形基底です。*

$$
e_{i_0} = x_{i_0} - \sum_{j < i_0} a_{i_0 j} e_j,
$$
そこから (b) が続きます。したがって、$J' \in \mathfrak{S}$、矛盾です。したがって、$J = I$ と補題が証明されます。

補題 4 を $I = P \cap \overline{C}$ に適用します。 $q \in I$ を、$I_q$ を $p \in I$ の集合として、$p \leq q$ とします。 $p \in I_q$、関係の場合
$$
q - p \geq 0,\quad p \in \overline{C},\quad q \in \overline{C}
$$
それを暗示します
$$
(q - p|p) \geq 0 \quad \text{and} \quad (q - p|q) \geq 0,
$$
そしてそれゆえに
$$
(p|p) \leq (p|q) \leq (q|q).
$$
したがって、集合 $I_q$ は *有界* です。 $I$ は離散であるため、$I_q$ は *有限* となり、$I$ が条件 (MIN) を満たすことは明らかです。一方、$p \in I$ の皆様にとっては、
$$
x_p = e^p + \sum_{q < p} c_{pq} e^q
$$
したがって(6)によります。
$$
x_p = S(e^p) + \sum_{q < p, q \in I} c_{pq} S(e^q).
$$
命題は、補題 3 と 4 の後に続きます。

#### 定理 1 {#lie-vi-s3-thm-1 .statement tag=0AXX}

*$\overline{\omega}_1, \ldots, \overline{\omega}_l$をチャンバー$C$に対する基本重み対応するとし、$1 \leq i \leq l$について、$x_i$を$A[P]^W$の元とし、$e^{\overline{\omega}_i}$をその固有の最大値項とします。しましょう*
$$
\varphi : \Lambda[X_1, \ldots, X_l] \to A[P]^W
$$
*$X_i$から$x_i$にかかる多項式代数$\Lambda[X_1, \ldots, X_l]$から$A[P]^W$の準同型になります。すると、写像 $\varphi$ は同型となります。*

補題 2 は、単項式 $X_1^{n_1} \ldots X_l^{n_l}$ の $\varphi$ の下の像が、一意の最大値項 $e^{n_1 \overline{\omega}_1 + \cdots + n_l \overline{\omega}_l}$ を持つ元であることを意味します。 $P \cap \overline{C}$ のすべての元は形 $n_1 \overline{\omega}_1 + \cdots + n_l \overline{\omega}_l$ で一意に記述できるため、提案 3 は、単項式 $X_1^{n_1} \ldots X_l^{n_l}$ の $\varphi$ の下の像が $A[P]^W$ の基底であることを示しています。 定理。

#### 例 1 {#lie-vi-s3-n4-exa-1 .statement tag=0AXY}

$x_i = S(e^{\overline{\omega}_i})$ が可能です。

#### 例 2 {#lie-vi-s3-n4-exa-2 .statement tag=0AXZ}

no. 3 の *注意* 2 までに、$x_i = J(e^{\rho + \overline{\omega}_i})/d$ を取ることができます (no. 3 に記法が入ります)。

### 練習問題 {#lie-vi-s3-exercises}

記法と仮定は No. の番号です。 2、3、4。

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
