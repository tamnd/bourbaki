---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 7
section_title: Approximation theorem
lang: ja
source: ac-i-vii
book_pages: 412-416, 460-461
pdf_pages: 0430-0434, 0478-0479
extraction: ocr
subsections:
    - "no": 1
      title: THE INTERSECTION OF A FINITE NUMBER OF VALUATION RINGS
      page: 412
      pdf_page: 430
    - "no": 2
      title: INDEPENDENT VALUATIONS
      page: 413
      pdf_page: 431
    - "no": 3
      title: THE CASE OF ABSOLUTE VALUES
      page: 415
      pdf_page: 433
statements: 14
exercises: 3
content_sha256: 3139a521d9022af3ff301a5fa2c85b582dea641690945180cb1d31b739af954f
translated_from: content/en/ac/VI/07_s7_approximation_theorem.md
translation_method: google
source_content_sha256: b2cb895d1415aea075090da4a69834fe352e4f0135aedb112aadd7070f320371
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 6e11eaf2647d4c5074693cce729e529be710d5190b4b0a6c67a18d5fe8ce6a39
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 7. 近似値定理

### 1. 有限の評価額の共通部分数環

#### 命題 1 {#ac-vi-s7-prop-1 .statement tag=04VN}

$K$を体、$(\mathbf{A}_i)_{1 \leq i \leq n}$アジナイトファミリーの評価$K$と$B = \bigcap_{i=1}^n \mathbf{A}_i$の環とします。 $p_i = B \cap m(\mathbf{A}_i)$と書きます。すると、すべての $i$ に対して $A_i = B_{p_i}$ となり、$B$ のラクションのジルドは $K$ になります。

明らかに$B_{p_i} \subset A_i$。 逆が含まれていることを証明するには、次の補題が必要です。

#### 補題 1 {#ac-vi-s7-lem-1 .statement tag=04VO}

$v_i$ ($1 \leq i \leq n$) を jield $K$ と $x \in K^*$ の評価とします。次に、次の形式の多項式 $(X)$ が存在します。

$$
f(X) = 1 + n_1 X + \cdots + n_{k-1} X^{k-1} + X^k \quad (k \geq 2,\ n_j \in \mathbf{Z} \text{ for } 1 \leq j \leq k - 1)
$$

$f(x) \neq 0$ と元 $z = f(x)^{-1}$ は、$1 \leq i \leq n$ に対して次の特性を享受します。

$$
v_i(z) = 0 \qquad \text{if} \quad v_i(x) \geq 0 \\
v_i(z) + v_i(x) > 0 \qquad \text{if} \quad v_i(x) < 0.
$$

この補題をしばらく仮定して、それが $A_1 \subset B_{p_1}$ をどのように暗示するかを示します。 $x$ を $A_i$ の非ゼロ元とします。 補題を $x$ に適用し、評価額 $v_i$ を $\mathbf{A}_i$ に関連付けます。次に、すべての $i$ に対して $v_i(z) \geq 0$ と $v_i(zx) \geq 0$、したがって $z \in B$ と $zx \in B$ になります。 $v_1(x) \geq 0$、$v_1(z) = 0$、したがって $z \notin p_1$ となります。したがって$x = zx/z \in B_{p_1}$です。 $B$の分数の体次に、含む $A_1$となり、したがって$K$になります。

ここで補題の証明に進みます。 $I$ を添字 $i$ の集合として、$v_i(x) \geq 0$ とします。すべての $i \in I$ について、$\bar{x}_i$ が $\kappa(\mathbf{A}_i)$ の $x$ の標準像を表すものとします。すべての $i \in I$ に対して、次のような多項式構成するを作成します。 $\kappa(\mathbf{A}_i)$ の $g(\bar{x}_i) = 0$ となるような形 (1) の多項式 $g(X)$ が存在する場合、そのような多項式であるとみなします。それ以外の場合は、$f_i = 1$ を使用します。次に、$f(X) = 1 + X^2 \prod_{i \in I} f_i(X)$と書きます。それは明らかに形 (1) の多項式です。 $i \in I$ の場合、$f(x) \in A_i$、さらに $(\bar{x}_i) \neq 0$ は構成になります。したがって、$f(x) \notin m(\mathbf{A}_i)$、$v_i(f(x)) = 0$、$v(z) = 0$ となります。 $i \notin I$ の場合、$v_i(x) < 0$、よって $v_i(f(x)) = kv_i(x)$ (§ 3, no. 1、命題 1)、および

$$
v_i(x) + v_i(z) = (1 - k)v_i(x) > 0
$$

($k \geq 2$以降)。 よって補題。

#### 命題 2 {#ac-vi-s7-prop-2 .statement tag=04VP}

命題 1 の仮説をもとに、$i \neq j$ に対して $\mathbf{A}_i \not\subset \mathbf{A}_j$ をさらに仮定します。その場合、$p_i$ は $B$ の個別の最大理想であり、$B$ のすべての最大理想は $p_i$ のいずれかに等しくなります。

$i \neq j$に対して$p_i \subset p_j$なら$\mathbf{A}_i = B_{p_i} \supset B_{p_j} = \mathbf{A}_j$。したがって、章 II, § 3, no. 5、系を命題 17 に適用するだけで十分です。

#### 系 1 {#ac-vi-s7-prop-2-cor-1 .statement tag=04VQ}

$i \neq j$ を $A_i \not\subset A_j$ とします。 元 $a_i \in A_i$ ($1 \leq i \leq n$) の各家族には、$1 \leq i \leq n$ に対して $x \equiv a_i \pmod{m(A_i)}$ となるような $x \in B$ が存在します。

$p_i$ は $B$、$A_i/m(A_i) = B_{p_i}/p_iB_{p_i} = B/p_i$ の最大の理想であるため、すべての $i$ に対して $a_i \in B$ であると想定できます。 系は、$B$ から $\prod_{i=1}^n (B/p_i)$ までの標準写像が全射であるという事実から続きます (章 11、§ 1, no. 2、命題 5)。

#### 系 2 {#ac-vi-s7-prop-2-cor-2 .statement tag=04VR}

$i \neq j$ を $A_i \not\subset A_j$ とします。 $i \neq j$に対して$v_i(x_i) = 0$と$v_j(x_i) > 0$となるような$K$の元$x_i$($1 \leq i \leq n$)が存在します。

添字 $i$ 系を適用するに対して、$a_i = 1$ と $a_j = 0$ が $j \neq i$ となるように、家族 $(a_i)$ に 1 を与えます。

#### 系 3 {#ac-vi-s7-prop-2-cor-3 .statement tag=04VS}

$K$ 含む $B$ 含むの各評価環は $A_i$ のいずれかです。

$A_i \not\subset A_j$ が $i \# j$ である場合にのみ注意を払うことができます。 $V$ を $K$ 含む $B$ の評価額環とします。私たちは書きます
$$
p = m(V) \cap B.
$$
$B$ 含む $p$、よっての最大理想 $p_i$ が存在します。
$$
A_i = B_{p_i} \subset B, \subset V.
$$

### 2. 独立した評価

#### 定義 1 {#ac-vi-s7-def-1 .statement tag=04VT}

$A$ と $A'$ を、同じ体 $K$ の 2 つの評価環とします。 $K$ が $A$ と $A'$ によって生成された環である場合、$A$ と $A'$ は独立していると呼ばれます。 $K$ の 2 つの評価は、その環が独立している場合は独立していると呼ばれ、そうでない場合は依存しています。

$K$ での不適切な評価は、$K$ でのすべての評価とは独立しています。 $K$ の高さ 1 の 2 つの評価が独立しているためには、それらが等価ではないことが必要かつ十分です (§ 4, no. 5、命題 6 (c))。

#### 定理 1 (評価額の概算定理) {#ac-vi-s7-thm-1 .statement tag=04VU}

$v_i$ ($1 \leq i \leq n$) を、$v_i$ の対と $\Gamma_i$ 位数群で独立した体 $K$ の評価とします。 $a_i \in K$ と $\alpha_i \in \Gamma_i$ ($1 \leq i \leq n$) とします。すると、すべての $i$ に対して $v_i(x - a_i) \geq \alpha_i$ となるような $x \in K$ が存在します。

$v_i$ が不適切な場合、$a_i = 0$ と関係 $v_i(x - a_i) \geq a_i$ はすべての $x \in K$ に当てはまります。したがって、$v_i$ は不適切ではないと考えてよいでしょう。

$A_i$ を $v_i$、$B = \bigcap_{i=1}^n A_i$、$p_i = m(A_i) \cap B$ の環とします。 no. 1 の命題 1 までに、$a_i$ は $a_i = b_i/s$ ($b_i \in B, s \in B - \{0\}$) と書き込まれる可能性があります。 $x = y/s$ と $\alpha_i' = \alpha_i + v_i(s)$ と書くと、$v_i(y - 6_i) \geq \alpha_i'$ になります。これは、すべての $i$ に対して $a_i \in B$ と仮定できることを示しています。すべての $i$ に対して $\alpha_i > 0$ と仮定することもできます。 $v_i$ を $z \in \mathbf{K}$ の集合として、$v_i(z) \geq a$ を$q_i = v_i \cap B$ と書きます。 $x \in B, v_i(x - a_i) \geq \alpha_i$ は $x \equiv a_i (\mathfrak{q}_i)$ と同等です。したがって、標準準同型 $B \to \prod_{i=1}^n (B/q_i)$ は全射であること、つまり $i \neq j$ (章 11, § 1, no. 2, 命題 5) に対する $q_i + q_j = B$ であることを示す必要があります。 B の最大理想は $\mathfrak{p}_i$ (命題 2) であるため、これは $i \neq j$ に対して $q_i \notin \mathfrak{p}_j$ であることを示すだけで十分です。

$q_i \subset \mathfrak{p}_j$と$i \neq j$が存在する$i, j$が存在するとします。すぐに、$q_i$ の根基が B の *素* イデアル $p$ であることが分かります。次に $p \subset \mathfrak{p}_j$、そして $\alpha_i > 0$ から $p \subset \mathfrak{p}_i$ 、したがって $q_i \subset \mathfrak{p}_i$ です。したがって、$A_1 = B_s \subset B_p$ (no. 1, 命題 1) および同様に $A_1 \subset B_r$ となります。さて、$v_i \neq (0)$ と $v_i = B_{\mathfrak{p}_i} q_i$ (章 11、§ 2, no. 4、命題 10)、$q_i \neq (0)$、よって $p \neq (0)$、$B_r \neq K$ となります。この$A_1$と$A_1$が独立した矛盾する仮定です。

$p$ が素数であることはまだわかりません。これは、次の補題から導き出されます。

#### 補題 2 {#ac-vi-s7-lem-2 .statement tag=04VV}

*A を評価環とし、b を A とは異なる A のイデアルとします。その場合、b の根基 c は素イデアルです。*

$xy \in c$ だとします。そして、$(xy)^n \in b$となるような$n \geq 1$が存在します。 $v$ を A に関連付けられた評価額とします。たとえば、$v(x) \geq v(y)$ の場合、

$$
v(x^{2n}) \geq v(x^n y^n),
$$

よって $x^{2n} \in b$ と $x \in c$

#### 系 1 {#ac-vi-s7-lem-2-cor-1 .statement tag=04VW}

*元 $\gamma_i \in \Gamma_i$ ($1 \leq i \leq n$) の各家族には、$v_i(x) = \gamma_i$ ($1 \leq i \leq n$) となるような $x \in K$ が存在します。

すべての $i$ に対して $A_i \neq K$ であると仮定できます。次に、すべての $i$ に対して、$v_i(a_i) = \gamma_i$ のような $a_i \in K$ と、$\gamma_i < a_r$ のような $a_r \in \Gamma_r$ が存在します。これら元 $a_i$ に対して、定理を適用する 1: $v_i(x - a_i) > v_i(a_i)$ となるような $x \in K$ が存在します。 よって、$x = a_i + (x - a_i)$、$v_i(x) = v_i(a_i) = \gamma_i$ ($§ 3$、no. 1、命題 1)。

#### 系 2 {#ac-vi-s7-lem-2-cor-2 .statement tag=04VX}

*$\mathscr{T}_i$ を $K$ で $v_i$ によって定義された位相とします。 $K^n$ に $\mathscr{T}_i$ の位相積を与えましょう。 $v_i$が不正でなければ、$K^n$の対角線は$K^n$に密集しています。

#### 命題 3 {#ac-vi-s7-prop-3 .statement tag=04VY}

*$v$ と $v'$ を、同じ体 $K$ に対する 2 つの不適切でない評価とします。 $v$ と $v'$ から定義するまでは、$K$ 上の同じ位相に依存していることが必要十分です。

$v$ と $v'$ で定義されたトポロジ $\mathscr{T}_v$ と $\mathscr{T}_{v'}$ が同一であると仮定します。 $\mathscr{T}_v$ はハウスドルフであるため、$K^2$ の対角は閉じており、したがって $v$ と $v'$ は従属関係にあります (系 2 から定理 1)。

逆に、$v$ と $v'$ が依存しているとします。 Then their rings $A$ and $A'$ are contained in the same ring $A''$ distinct from $K$ and $A''$ is the ring of a valuation $v''$ ($§ 4$, no. 1, Proposition 1). 位相 $\mathscr{T}_{v''}$ が $\mathscr{T}_v$ と同一であることを示すだけで十分です。 $\Gamma$ と $\Gamma''$ を $v$ と $v''$ の位数群とします。 $\Gamma''$ 上に $\Gamma$ の増加する準同型 $\lambda$ が存在し、$v'' = A \circ v$ ($§ 4$, no. 3) になります。 $a'' \in I?''$ の場合は $a \in \lambda^{-1}(a'')$ にします。 条件 $v(x) \geq \alpha$ は $v''(x) \geq a''$ を意味します。 $\beta \in \Gamma$ と $\beta'' = \lambda(\beta)$ としましょう。 条件 $v(x) \leq \beta$ は $v''(x) \leq \beta''$ を意味し、したがって条件 $v''(x) > \beta''$ は $v(x) > \beta$ を意味します。 $v$ と $v''$ は不正ではないので、問題の不等式定義するは、$\mathscr{T}_v$ と $\mathscr{T}_{v''}$ の 0 の近傍の基本的な系です。 したがって、$\mathscr{T}_v = \mathscr{T}_{v''}$ となり、証明が完成します。

注意
(1) 命題 3 は、関係 「$v$ と $v'$ が依存している」が同値関係であることを示しています。
(2) 高さ 1 の評価と超計的絶対値値 (§ 6, no. 2) の間の関係を考慮すると、高さ 1 の評価の場合、等価絶対値値の特徴付け (一般位相、章) から命題 3 も続きます。 IX, § 3, no. 2、命題 5)。

#### 命題 4 {#ac-vi-s7-prop-4 .statement tag=04VZ}

*$v_1, \ldots, v_n$ ($n \geq 2$) を、同じ体 $K$ に対するペアごとの従属評価とします。 次に、$v_1, \ldots, v_n$ 生成する部分環 $\delta \ K$ のうち環 $A_1, \ldots, A_n$ は、$K$ とは異なります。*

$n = 2$ 命題 4 の場合、定義 1 から続きます。これが $n - 1$ の評価にも当てはまると仮定します。すると、K と含む $A_1, \ldots, A_{n-1}$ とは異なる K の部分環 A が存在します。 部分環 B $\neq K$ 含む $A_{n-1}$ と $A_n$ も存在します。 A と B 含む $A_{n-1}$ として、包含に関して比較可能です (§ 4, no. 1、系から命題 1)。したがって、これら 2 つの大きい方は、含むすべての $A_i$ になります。

### 3. 絶対値の場合

#### 定理 2 (絶対値値の近似値定理) {#ac-vi-s7-thm-2 .statement tag=04W0}

*$f_i$ ($1 \leq i \leq n$) を同じ体 $K$ 上で絶対的な値とします。これは不適切ではなく、同等なものは 2 つありません。 $a_i \ (1 \leq i \leq n)$ を $K$ と $\varepsilon$ 実数 $> 0$ の元とします。そして、すべての $i$ に対して $f_i(x - a_i) \leq \varepsilon$ となるような $x \in K$ が存在します。*

$K_i$ が $f_i$ によって定義される位相を含む体 K を表すものとします。証明される結果は以下と同等です: 積 $P = K_1 \times \cdots \times K_n$ では、対角線 D の閉包 $\overline{D}$ は P に等しいです。これは $n = 1$ では明らかです。この点が$k < n$に対するk絶対値値の場合に成立したとする。

まず、K の $2 \leq h \leq n$、元 $x_h$ に対して、$3 \leq i \leq h$ に対して $f_1(x_h) < 1, f_2(x_h) > 1$ および $f_i(x_h) \neq 1$ が存在することを示します。 $h$の帰納法までに議論します。 $h = 2$ の場合、これは、$f_1$ と $f_2$ が等価ではないという事実から生じます。したがって、$x_{h-1}$の存在が示され、$x_h$の存在が証明されたと仮定します。 $f_h(x_{h-1}) \neq 1$の場合、$x_h = x_{h-1}$を取る可能性があります。 $f_h(x_{h-1}) = 1$ の場合、$f_h(z) \neq 1$ と $x_h = z(x_{h-1})^s$ が s 十分大きいについて問題を解くように選ぶ $z \in K^*$ を計算します。これで$x_h$の存在が証明されました。

整数 $q$ は無限大になる傾向があり、$f_1(x_n^q)$ は 0 になる傾向があり、$f_2(x_n^q)$ は $+\infty$ になる傾向があり、$f_i(x_n^q)$ は 0 または $i \geq 3$ の場合は $+\infty$ になる傾向があります。 $y_q = x_n^q(1 + x_n^q)^{-1}$ を書いています。
$$
1 - y_q = (1 + x_n^q)^{-1};
$$
したがって、数列 $(y_q)$ は、$K_1$ では 0、$K_2$ では 1、$i \geq 3$ では $K_i$ で 0 または 1 になる傾向があります。したがって、$K_i$ の番号付けを変更すると、$\overline{D}$ 含む点 $(e_1, \ldots, e_n)$ のような整数 $r$ ($1 \leq r < n$) が存在すると仮定できます。ここで、$e_i = 1$ は $1 \leq i \leq r$ であり、 $r + 1 \leq i \leq n$の$e_i = 0$。さて、$\overline{D}$ は P のベクトルサブ K 空間です。 したがって、$\overline{D}$ 含むの対角線 D' と D''
$$
P' = K_1 \times \cdots \times K_r,
$$
そして$P'' = K_{r+1} \times \cdots \times K_n$。 帰納法の仮定、$P' = \overline{D}'$、$P'' = \overline{D}''$までに。したがって$\overline{D} = P$です。

### 練習問題 {#ac-vi-s7-exercises}

[§ 7 に対して練習問題](exercises/s7/)を参照してください。
