---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: FREE LIE ALGEBRAS
section: 3
section_title: Enveloping algebra of the free Lie algebra
lang: ja
source: lie-i-iii
book_pages: 136-142, 186-187
pdf_pages: 0154-0160, 0204-0205
extraction: ocr
subsections:
    - "no": 1
      title: ENVELOPING ALGEBRA OF $L(X)$
      page: 136
      pdf_page: 154
    - "no": 2
      title: PROJECTOR OF $A^+(X)$ ONTO $L(X)$
      page: 138
      pdf_page: 156
    - "no": 3
      title: DIMENSION OF THE HOMOGENEOUS COMPONENTS OF L(X)
      page: 140
      pdf_page: 158
statements: 11
exercises: 4
content_sha256: 43b4e92e6d23a1e435a8f646aa66fe9b72db5b490dcb28462ffba22179915806
translated_from: content/en/lie/II/03_s3_enveloping_algebra_of_the_free_lie.md
translation_method: google
source_content_sha256: 1d39611cf30ae9228e327035d9d7254aba6ff04ead058f79653b16b5bbbadc54
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: 8667ee8e8aefabe845d19742eaf8966785c25e81918ec7802861f7e053f3e3de
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 3。無料のリー代数を代数で包みます

この段落では、$A(X) = A_K(X)$ は、環 $K$ (代数, 章 III, § 2, no. 7, 定義) に対する集合 $X$ の自由結合代数 Libas(X) を表します。 2)。 $X$ は、$A(X)$ の標準像と同一視されます。 $K$加群$A(X)$は$X$から導出された自由モノイド$Mo(X)$を基底として認めていることを思い出してください。 $A^+(X)$ は、空ではない語によって生成された $A(X)$ の部分加群を表します。

### 1. $L(X)$ の代数を包み込む

#### 定理 1 {#lie-ii-s3-thm-1 .statement tag=0A42}

*$X$ *を* $A(X)$ *(§ 2, no. 2, 命題 1)*に標準単射を拡張した一意のリー代数準同型を* $\alpha : L(X) \to A(X)$ * とします。 *$\sigma : L(X) \to U(L(X))$ を、$L(X)$ を包む代数の標準写像とし、$\beta : U(L(X)) \to A(X)$ を、$\beta \circ \sigma = \alpha$ (章 I, § 2, no. 1, 命題 1) となるような固有の単位代数準同型とします。 次に:
(a) $\alpha$ は単射であり、$\alpha(L(X))$ は $A(X)$ の直和因子部分加群です。
(b) $\beta$ は全単射です。

B を B の X の K-代数と $\phi$ 写像とする。 § 2, no. 2 の命題 1 までに、$\psi | X = \phi$ となるようなリー代数準同型 $\psi : L(X) \to B$ が存在します。 章 I, § 2, no. 1 の命題 1 によって、$\theta \circ \sigma = \psi$ となるような単位代数準同型 $\theta : U(L(X)) \to B$ が存在し、したがって $(\theta \circ \sigma) | X = \phi$ となるような単位が存在します。 $\sigma(X)$ 生成するが単位代数 $U(L(X))$ であるように、準同型 $\theta$ は独自の単位代数準同型満たす後者条件です。これは、順序付けられた対 $(U(L(X)), \sigma | X)$ が $A(X)$ と同じユニバーサル写像問題の解であることを示しています。 $\phi$ を X の標準単射として$A(X)$ に入れると、$\beta$ は同型であると推定され、(b) が証明されます。

最後に、$L(X)$ は自由K-加群 (§ 2, no. 11、系 ～ 定理 1) であるため、$\sigma$ は単射であり、$\sigma(L(X))$ は $U(L(X))$ の直和因子部分加群 (章 I, § 2, no. 7、系) 3から定理1）。 (b) により、(a) が証明されます。

#### 系 1 {#lie-ii-s3-thm-1-cor-1 .statement tag=0A43}

代数 $A(X)$ には、X の元が原始的になるように、$A(X)$ を双晶にする一意の余積が存在します。さらに、$\beta$は、大角$U(L(X))$の同型を、この大角構造で$A(X)$に重ねたものです。

これは、定理の主張 (b) と、X 生成するが単位代数 $A(X)$ であるという事実から続きます。

今後、$A(X)$ にはこの二桁構造が与えられ、$L(X)$ は$\alpha$ の下の像、つまりX によって生成された$A(X)$ の嘘部分代数と同一視されます。

#### 系 2 {#lie-ii-s3-thm-1-cor-2 .statement tag=0A44}

$K$ が特性 0 の体である場合、$L(X)$ は $A(X)$ の原始関数元のリー代数です。

これは、§ 1, no. 5 の系 1 と系から命題 9 に続きます。

#### 注意 {#lie-ii-s3-n1-rem-1 .statement tag=0A45}

(1) $K'$ を可換環含む K とします。$A(X)$、$L(X)$、$L_{K'}(X)$ が $A_{K'}(X)$ の部分集合と同一視される場合、定理 1 関係の部分 (a) から推定します。

$$
L(X) = L_{K'}(X) \cap A(X).
$$

(2) 環 K の加法群にねじれがないと仮定する場合のみ、系 2 ～ 定理 1 は有効です。まず、$K = \mathbf{Z}$ と仮定します。 $A(X)$ のすべてのプリミティブ元は、$A_q(X)$ のプリミティブ元であるため、$L_q(X) \cap A(X) = L(X)$ (系 2 および公式 (1)) に含まれます。一般的なケースでは、K は $\mathbf{Z}$ でフラットであり、§ 1, no. 2 の注意 2 と § 2, no. 5 の命題 3 を適用します。

(3) $\Delta$ を可換モノイドとし、$X$ の $\phi_0$ 写像を関連するモノイドの $\Delta$ と $\phi : Mo(X) \to \Delta$ 準同型にします。 $A(X)$ に *代数*、章 III, § 3, no. 1、*例* 3 で定義された目盛り $(A^\delta(X))_{\delta \in \Delta}$ と、§ 2, no. 6 で定義された目盛り $(L^\delta(X))_{\delta \in \Delta}$ が $L(X)$ に与えられた場合、$\delta \in \Delta$ については、次のようになります。 $L^\delta(X) \subset L(X) \cap A^\delta(X)$。 $L$ は $\delta \in \Delta$ の $L^\delta(X)$ の和であり、$\delta \in \Delta$ の $L(X) \cap A^\delta(X)$ の和は直接であることを意味します。

$$
L^\delta(X) = L(X) \cap A^\delta(X).
$$

(4) $A$ を単位結合代数とし、$t = (t_i)_{i \in I}$ を $A$ の元の族とする。 図式があります

$$
\begin{array}{ccc}
L(I) & \xrightarrow{f_t} & A \\
i \downarrow & & \downarrow g_t \\
A(I)
\end{array}
$$

ここで、$i$ は標準単射、$f_t$ は $t$ で定義されるリー代数準同型、$g_t$ は $i \in I$ に対して $g_t(i) = t_i$ となるような単位代数準同型です。 図式は、$I$ 上で $g_t \circ i$ および $f_t$ 一致するに対して可換です。 $P \in L(I)$、元 $P((t_i)_{i \in I})$ が § 2, no. 4、一致するで定義され、元 $P((t_i)_{i \in I})$ が *代数*、章 III, § 2, no. 8、*例* 2 で定義されている場合、ということになります。

### 2. $A^+(X)$ の射影子から $L(X)$

$\pi$ を $A^+(X)$ の線形写像を $L(X)$ にすると、次のように定義されます。

$$
\pi(x_1 \ldots x_n) = (\operatorname{ad}(x_1) \circ \cdots \circ \operatorname{ad}(x_{n-1}))(x_n)
$$

$X$の$n > 0, x_1, \ldots, x_n$用。

#### 命題 1 {#lie-ii-s3-prop-1 .statement tag=0A46}

(a) *$\pi$から$L(X)$の制限$\pi_0$は、$L(X)$の導分です。*
(b) *すべての整数 $n \geq 1$ と $L^n(X)$、$\pi(u) = n.u$ のすべての $u$ について。*

(a) $E$ を加群 $L(X)$ の自己準同型環と $A(X)$ の $\theta$ 準同型を $E$ にし、すべての $x \in X$ について$\theta(x) = \operatorname{ad} x$ とする。 $\theta$から$L(X)$の制限は$L(X)$のリー代数準同型から$E$になり、$X$の一致すると$L(X)$、よっての随伴表現です

$$
\theta(u).v = [u, v] \quad \text{for } u, v \text{ in } L(X).
$$

$a$ を $A(X)$ に、$b$ を $A^+(X)$ にします。それから

$$
\pi(a.b) = \theta(a).\pi(b).
$$

$X$ の $p \geq 0, q \geq 1$ と $x_1, \ldots, x_{p+q}$ のケース $a = x_1 \ldots x_p, \ b = x_{p+1} \ldots x_{p+q}$ を考慮するだけで十分です。しかし、その後、$x \in X$の$\theta(x) = \operatorname{ad} x$から、(3)の直後に(5)が続きます。

$u$ と $v$ を $L(X)$ に入れます。 (4) と (5) により、

$$
\pi_0([u, v]) = \pi(uv - vu) = \theta(u) \cdot \pi(v) - \theta(v) \cdot \pi(u)
= [u, \pi(v)] - [v, \pi(u)] = [u, \pi_0(v)] + [\pi_0(u), v],
$$

したがって、$\pi_0$ は $L(X)$ の導分です。

(b) $\pi_1$ を加群 $L(X)$ の自己準同型と$L^n(X)$ の一致すると乗法整数 $n \geq 1$ とします。 公式 $[L^n(X), L^m(X)] \subset L^{n+m}(X)$ は、$\pi_1$ が導分 (*代数*, 章 III, § 10, no. 3, *例* 6) であることを示します。 $L(X)$ の導分 $\pi_1 - \pi_0$ は、$X$ の零であり、$X$ 生成する $L(X)$、$\pi_0 = \pi_1$、よってと同様です (b)。

#### 系 {#lie-ii-s3-n2-cor-1 .statement tag=0A47}

*K が Q 代数であると仮定します。 P をそれ自体に次のような $A^+(X)$ の線形写像とします*

$$
P(x_1 \ldots x_n) = \frac{1}{n} (\operatorname{ad} x_1 \circ \cdots \circ \operatorname{ad} x_{n-1})(x_n)
$$

*Xの$n \geq 1$と$x_1, \ldots, x_n$用。すると、P は $A^+(X)$ の射影子から $L(X)$ になります。*

$L(X)$にはPの像が含まれています。さらに、$L^n(X)$、$P(u) = \frac{1}{n} \pi(u)$、よって $P(u) = u$ のすべての $n \geq 1$ とすべての $u$ について、命題 1 によって計算されます。

$$
L(X) = \sum_{n \geq 1} L^n(X),
$$

$L(X)$ に対する P の制限が同一性であることがわかります。

#### 注意 {#lie-ii-s3-n2-rem-1 .statement tag=0A48}

Suppose that K is a field of characteristic zero and let Q be the projector of $A(X) = U(L(X))$ onto $L(X)$ associated with the canonical graduation of $U(L(X))$, cf. § 1, no. 5. *$\alpha \in \mathbf{N}^{(X)}$、$Q(A^\alpha(X)) \subset L^\alpha(X)$の場合。* Q の像と核が型 $\mathbf{N}^{(X)}$ の段階で $A(X)$ の部分加群に評価されることを確認するだけで十分です。 これは、$L(X)$ に等しい像について明らかです。 一方、$n$ を整数 $\geq 1$ とします。 The vector subspace of $A(X)$ generated by the $y^n$, where $y \in L(X)$, is equal to the vector subspace of $A(X)$ generated by the $\sum_{\sigma \in S_n} y_{\sigma(1)} y_{\sigma(2)} \cdots y_{\sigma(n)}$, where $y_1, y_2, \ldots, y_n$ are homogeneous elements of $L(X)$; then this subspace is a graded submodule of $A(X)$.

(カード(X) $\geq 2$、射影子 P および Q が $A^+(X)$ で一致する* にならないことに注意してください。たとえば、$x, y$ が $x \neq y$ の X にあり、次のように書きます。

$$
z = x[x, y] + [x, y]x = x^2y - yx^2.
$$

次に、$Q(z) = 0$ と $P(z) = \frac{1}{3}[x, [x, y]] \neq 0$、cf. § 2, no. 10、*例* と no. 11、*定理* 1)。

### 3. L(X)の均質な成分の次元

X を集合、$\alpha$ 元の $\mathbf{N}^{(X)}$ および d 整数 > 0 とします。$\alpha = d\beta$ となるような $\beta \in \mathbf{N}^{(X)}$ が存在する場合、$d|\alpha$ と書きます。一意の元 $\beta$ は、$\alpha/d$ で表されます。

#### 補題 1 {#lie-ii-s3-lem-1 .statement tag=0A49}

n を整数 > 0、$T_1, \ldots, T_n$ を不定、および $\mathbf{Z}$ の $u_1, \ldots, u_n$ 元とします。 $(c(\alpha))_{\alpha \in \mathbf{N}^n - \{0\}}$ を次のような $\mathbf{Z}$ の元の家族とします。

$$
1 - \sum_{i=1}^n u_i T_i = \prod_{\alpha \neq 0} (1 - T^\alpha)^{c(\alpha)}.
$$

$\alpha \in \mathbf{N}^n - \{0\}$の皆様、

$$
c(\alpha) = \frac{1}{|\alpha|} \sum_{d|\alpha} \mu(d) \frac{(|\alpha|/d)!}{(\alpha/d)!} u^{\alpha/d}
$$

ここで、$\mu$ はメビウス写像 (付録) です。

公式 (7) は、両辺の対数 (代数、章 IV, § 6, no. 9) を取ると次と等価です。

$$
\log \left( 1 - \sum_{i=1}^n u_i T_i \right) = \sum_{\alpha \neq 0} c(\alpha) \log (1 - T^\alpha).
$$

今

$$
-\log \left( 1 - \sum_{i=1}^n u_i T_i \right) = \sum_{j \geq 1} \frac{1}{j} \left( \sum_{i=1}^n u_i T_i \right)^j
$$
$$
= \sum_{j \geq 1} \frac{1}{j} \sum_{|\beta|=j} \frac{|\beta|!}{\beta!} u^\beta T^\beta
$$
$$
= \sum_{|\beta|>0} \frac{1}{|\beta|} \frac{|\beta|!}{\beta!} u^\beta T^\beta.
$$

一方で

$$
-\sum_{\alpha \neq 0} c(\alpha) \log (1 - T^\alpha) = \sum_{|\alpha|>0, k \geq 1} \frac{1}{k} c(\alpha) T^{k\alpha}
$$
$$
= \sum_{|\beta|>0, k|\beta} \frac{1}{k} c\left( \frac{\beta}{k} \right) T^\beta.
$$

したがって、(7) は次と同等です。

$$
\sum_{k|\beta} \left| \frac{\beta}{k} \right| c\left( \frac{\beta}{k} \right) = \frac{|\beta|!}{\beta!} u^\beta \quad \text{for all } \beta \in \mathbf{N}^n - \{0\}.
$$

$\Lambda$ を $(\lambda_1, \lambda_2, \ldots, \lambda_n) \in \mathbf{N}^n - \{0\}$ の集合とし、g.c.d. $\lambda_1, \lambda_2, \ldots, \lambda_n$ は 1 に等しい。 $\mathbf{N}^n - \{0\}$ のすべての元は、形 $m\lambda$ で一意に書き込むことができます。ここで、$m$ は、整数 $\geqslant 1$ および $\lambda \in \Lambda$ です。 条件 (12) は以下と同等です

$$
\sum_{k|m} \left| \frac{m\lambda}{k} \right| c\left( \frac{m\lambda}{k} \right) = \frac{(m|\lambda|)!}{(m\lambda)!} u^{m\lambda} \quad \text{for all } \lambda \in \Lambda \text{ and all } m \geqslant 1.
$$

メビウス反転公式 (付録) により、条件 (13) は次と等価です。

$$
|m\lambda| c(m\lambda) = \sum_{d|m} \mu(d) \frac{\left| \frac{m\lambda}{d} \right|!}{\left( \frac{m\lambda}{d} \right)!} u^{\frac{m\lambda}{d}}
$$

すべての $\lambda \in \Lambda$ とすべての $m \geqslant 1$ に対して。

#### 定理 2 {#lie-ii-s3-thm-2 .statement tag=0A4A}

*$X$を有限の集合と$n = \mathrm{Card}(X)$とします。*

(a) *すべての整数 $r \geqslant 1$ について、$K$ モジュール $L^r(X)$ には階数* がありません

$$
c(r) = \frac{1}{r} \sum_{d|r} \mu(d) n^{r/d},
$$

*ここで、$\mu$はメビウス写像です。*

(b) *すべての $\alpha \in \mathbf{N}^X - \{0\}$ について、$K$ モジュール $L^\alpha(X)$ (§ 2, no. 6) には階数* が含まれていません

$$
c(\alpha) = \frac{1}{|\alpha|} \sum_{d|\alpha} \mu(d) \frac{(|\alpha|/d)!}{(\alpha/d)!}.
$$

$r \in \mathbf{N}$ である加群 $L^r(X)$ と $\alpha \in \mathbf{N}^X$ である $L^\alpha(X)$ が無料であることはすでにわかっています (§ 2, no. 11、系から定理 1)。 $Mo(X)$ の標準準同型 $\phi$ を $\mathbf{N}^X$ (*代数*、章 III, § 3, no. 1、*例 3*) に定義する$A(X)$ の多階調 $(A^\alpha(X))_{\alpha \in \mathbf{N}^X}$ を考えます。次に、$A^\alpha(X) \cap L(X) = L^\alpha(X)$ by *注意 3* no. 1。 $\alpha \in \mathbf{N}^X$ の場合、$K$ モジュール $A^\alpha(X)$ は、$X$ の各文字 $x$ が $\alpha(x)$ 回出現する語の基底集合として認めます。 $d(\alpha)$ をこれら語の数、つまり $A^\alpha(X)$ の階数とします。正式な冪系列を 2 つの異なる方法で計算するとします。

$$
P((T_x)_{x \in X}) \in \mathbf{Z}[[((T_x)_{x \in X})]]
$$

によって定義される

$$
P(T) = \sum_{\alpha \in \mathbf{N}^X} d(\alpha) T^\alpha.
$$

(1) 私たちは、

$$
P(T) = \sum_{m \in Mo(X)} T^{\phi(m)} = \sum_{r=0}^\infty \sum_{x_1, \ldots, x_r} T_{x_1} \cdots T_{x_r} = \sum_{r=0}^\infty \left( \sum_{x \in X} T_x \right)^r
$$

よって

$$
P(T) = \left( 1 - \sum_{x \in X} T_x \right)^{-1}.
$$

(2) すべての $\alpha \in \mathbf{N}^X - \{0\}$ について、$(e_{\alpha,j})_{1 \leq j \leq c(\alpha)}$ を $L^\alpha(X)$ の基底とし、対 $(\alpha, j)$ の集合 $I$ を与えると、$\alpha \in \mathbf{N}^X - \{0\}$ と $1 \leq j \leq c(\alpha)$ の合計順序が決まります。 no. 1 の定理 1 およびポアンカレ・バーコフ・ヴィットによる定理 (章 I, § 2, no. 7、系 3 ～ 定理 1)、元
$$
y_m = \prod_{(\alpha, j) \in I} (e_{\alpha, j})^{m(\alpha, j)},
$$
ここで、添字 $m$ は、$A(X)$ の $\mathbf{N}^{(I)}$、形基底を通過します。それぞれの $y_m$ は多次数 $\sum_{(\alpha, j) \in I} m(\alpha, j) \alpha$ です。 $u(m)$ がこの多度を表すものとします。したがって、
$$
P(T) = \sum_{m \in \mathbf{N}^{(I)}} T^{u(m)} = \sum_{m \in \mathbf{N}^{(I)}} \prod_{(\alpha, j) \in I} T^{m(\alpha, j)\alpha}
= \prod_{(\alpha, j) \in I} \sum_{r=0}^\infty T^{r\alpha} = \prod_{(\alpha, j) \in I} (1 - T^\alpha)^{-1},
$$
ついによって
$$
P(T) = \prod_{\alpha \in \mathbf{N}^X - \{0\}} (1 - T^\alpha)^{-c(\alpha)}.
$$
(18) と (19) を比較すると、次のようになります。
$$
1 - \sum_{x \in X} T_x = \prod_{\alpha \in \mathbf{N}^X - \{0\}} (1 - T^\alpha)^{c(\alpha)}.
$$
補題 1 では (b) が得られます。

ここで、公式 (20) の $x \in X$ の $T_x$ を同じ不定数 $U$ に置き換えると、次のようになります。
$$
1 - nU = \prod_{\alpha \in \mathbf{N}^X - \{0\}} (1 - U^{|\alpha|})^{c(\alpha)} = \prod_{r > 0} (1 - U^r)^{c(r)}.
$$
適用補題 1 再び、(a) を推定します。

#### 例 {#lie-ii-s3-n3-exa-1 .statement tag=0A4B}

私たちは持っています
$$
\begin{align*}
c(1) &= n, & c(2) &= \frac{1}{2}(n^2 - n), & c(3) &= \frac{1}{3}(n^3 - n), \\
c(4) &= \frac{1}{4}(n^4 - n^2), & c(5) &= \frac{1}{5}(n^5 - n), & c(6) &= \frac{1}{6}(n^6 - n^3 - n^2 + n).
\end{align*}
$$

#### 注意 {#lie-ii-s3-n3-rem-1 .statement tag=0A4C}

$X$ を集合とし、$\alpha \in \mathbf{N}^{(X)}$ とします。無料の $K$ モジュール $L^\alpha(X)$ の階数も、公式 (16) によって与えられます。これは、§ 2, no. 6 の定理 2 (b) と命題 4 の直後に続きます。

### 練習問題 {#lie-ii-s3-exercises}

文字$X$は集合を表します。

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
