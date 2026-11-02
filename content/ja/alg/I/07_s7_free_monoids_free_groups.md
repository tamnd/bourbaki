---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 7
section_title: Free monoids, free groups
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 81-96, 159-171
pdf_pages: 0105-0120, 0183-0195
extraction: ocr
subsections:
    - "no": 1
      title: FREE MAGMAS
      page: 81
      pdf_page: 105
    - "no": 2
      title: FREE MONOIDS
      page: 82
      pdf_page: 106
    - "no": 3
      title: AMALGAMATED SUM OF MONOIDS
      page: 84
      pdf_page: 108
    - "no": 4
      title: APPLICATION TO FREE MONOIDS
      page: 88
      pdf_page: 112
    - "no": 5
      title: FREE GROUPS
      page: 89
      pdf_page: 113
    - "no": 6
      title: PRESENTATIONS OF A GROUP
      page: 90
      pdf_page: 114
    - "no": 7
      title: FREE COMMUTATIVE GROUPS AND MONOIDS
      page: 92
      pdf_page: 116
    - "no": 8
      title: EXPONENTIAL NOTATION
      page: 94
      pdf_page: 118
    - "no": 9
      title: RELATIONS BETWEEN THE VARIOUS FREE OBJECTS
      page: 95
      pdf_page: 119
statements: 17
exercises: 40
content_sha256: 1765e98b8f7ba62685cba2c96bc7ecfe2990f1933be138013e91e034c06b8343
translated_from: content/en/alg/I/07_s7_free_monoids_free_groups.md
translation_method: google
source_content_sha256: 97dfa3c35501eb8d7f97ddf5171fd22adaac2703346a99cfb362c9406ce8d816
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 25744d8bc9761af1685168acc8f33093cbb4c55d6685ac7b2032616b2c8592b5
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 7。無料のモノイド、無料群

この段落では、X は集合を表します。 Unless otherwise mentioned, the identity element of a monoid will be denoted by e.

### 1. 無料のマグマ

集合 $M_n(X)$ の数列は、整数 $n \geqslant 1$ 上の帰納法によって次のように定義されます。 $n \geqslant 2$、$M_n(X)$ に対して $M_1(X) = X$ を書くと、集合の集合和になります。 $M_p(X) \times M_{n-p}(X)$ は $1 \leqslant p \leqslant n-1$ です。 $(M_n(X))_{n \geqslant 1}$ 族の集合和は $M(X)$ で示されます。 集合 $M_n(X)$ のそれぞれは、$M(X)$ の標準像と同一視されます。 $M(X)$ の各元 $w$ には、$w \in M_n(X)$ のような固有の整数 $n$ が存在します。それは$w$の長さと呼ばれ、$l(w)$で表されます。 集合 X は、長さ 1 の $M(X)$ の元で構成されます。

$w$ と $w'$ を $M(X)$ に入れます。 $p = l(w)$ と $q = l(w')$ と書きます。 The image of $(w, w')$ under the canonical injection of $M_p(X) \times M_q(X)$ into the sum set $M_{p+q}(X)$ is called the composition of $w$ and $w'$ and is denoted by $ww'$ or $w.w'$. 次に、$l(w.w') = l(w) + l(w')$ と長さ $\geqslant 2$ の $M(X)$ のすべての元は、$M(X)$ の $w', w''$ を使用して形 $w'w''$ に一意に書き込むことができます。

合成 $(w, w') \mapsto w.w'$ の法則を加えた集合 $M(X)$ を、X (§ 1, no. 1、定義 1) に構築された自由マグマと呼びます。

#### 命題 1 {#alg-i-s7-prop-1 .statement tag=05FH}

M をマグマとします。 X のすべての写像 f を M に変換すると、独自の方法で $M(X)$ の射を M に拡張できます。

$n \geqslant$ の帰納法により、写像 $f_n : M_n(X) \to M$ は次のように定義されます。 f_1 = f とします。 n \geq 2 の場合、写像 f_n は、$p = 1, 2, \ldots, n-1$ の $f_n(w.w') = f_p(w).f_{n-p}(w')$ と $M_p(X) \times M_{n-p}(X)$ の $(w, w')$ によって定義されます。 $g$を$M(X)$の写像を$M$にすると、整数$n \geq 1$ごとに$M_n(X)$に誘導する$f_n$が加わります。明らかに、$g$は$M(X)$の一意な準同型を$M$、つまり拡大する$f$です。

$u$ を $X$ の写像から集合 $Y$ にします。 命題 1 までに、$X$ に $u$ を伴う一致するである $M(Y)$ に、$M(X)$ の準同型が 1 つだけ存在します。 $M(u)$と表記します。 $v$が$Y$の写像を集合$Z$に、準同型$M(v) \circ M(u)$を$M(X)$に$M(Z)$一致するとし、$X$に$v \circ u$を加えた場合、 よって

$$
M(v) \circ M(u) = M(v \circ u).
$$

#### 命題 2 {#alg-i-s7-prop-2 .statement tag=05FI}

※$u : X \to Y$を写像とします。 $u$ が単射（それぞれ全単射、全単射）の場合、$M(u)$ も同様です。*

$u$ が単射だと仮定します。 $X$ が空の場合、$M(X)$ も空であるため、$M(u)$ は単射です。 $X$ が空でない場合、$X$ に $Y$ の写像 $v$ が存在し、$v \circ u$ は $X$ の恒等写像 (*集合理論*, II, § 3, no. 8, 命題 8); 写像 $M(v) \circ M(u) = M(v \circ u)$ は $M(X)$ の恒等写像であるため、$M(u)$ は単射法です。

When $u$ is surjective, there exists a mapping $w$ of $Y$ into $X$ such that $u \circ w$ is the identity mapping of $Y$ (*Set Theory*, II, § 3, no. 8, Proposition 8). この場合、$M(u) \circ M(w) = M(u \circ w)$ は $M(Y)$ の恒等写像であるため、$M(u)$ は全射になります。

最後に、$u$ が全単射である場合、それは単射および全射であるため、$M(u)$ は同じ性質を持ちます。

$S$ を $X$ の部分集合とします。 命題までに、$S$ の 2 単射を $X$ に拡張し、$M(S)$ の同型を$M(X)$ のサブマグマ $M'(S)$ に拡張できます。この同型によってマグマ$M(S)$と$M'(S)$が識別されます。そして、$M(S)$は$S$によって生成された$M(X)$のサブマグマです。

$X$ を集合とし、$(u_\alpha, v_\alpha)_{\alpha \in I}$ を $M(X)$ の元の順序付けられた対の族とします。 $R$ を $M(X)$ の法則と互換性のある $M(X)$ の同値関係とし、$(u_\alpha, v_\alpha)$ (§ 1, no. 6) によって生成します。マグマ $M(X)/R$ は、$X$ と関係者* $(u_\alpha, v_\alpha)_{\alpha \in I}$ によって定義される*マグマと呼ばれます。 $h$ を $M(X)$ から $M(X)/R$ への正規の射とします。すると、$h(X)$によって$M(X)/R$が生成されます。

$N$ をマグマ、$(n_x)_{x \in X}$ を $N$ の元の族とします。 $k$ を $M(X)$ から $N$ までの射とし、すべての $x \in X$ に対して $k(x) = n_x$ (命題 1) とします。すべての $\alpha \in I$ に対して $k(u_\alpha) = k(v_\alpha)$ である場合、すべての $x \in X$ に対して $f(h(x)) = n_x$ となるような射 $f : M(X)/R \to N$ が 1 つだけ存在します (§ 1, no. 6、命題 9)。

### 2. 自由モノイド

$\mathbf{N}$ の区間 $[1, n]$ (おそらく空) によってインデックス付けされた $X$ の元の有限列 $w = (x_i)_{1 \leq i \leq n}$ は、$X$ に構築された *語* と呼ばれます。 整数 $n$ は、語 $w$ の *長さ* と呼ばれ、$l(w)$ で表されます。 長さ 0 の固有の語、つまり空の数列 $e$ があります。 $\mathbf{X}$ は、長さ 1 の語の集合と識別されます。

$w = (x_i)_{1 \leq i \leq m}$ と $w' = (x'_j)_{1 \leq j \leq n}$ を 2 つの語とします。 $w$ と $w'$ の合成は、語 $u = (y_k)_{1 \leq k \leq m+n}$ で定義されます

$$
y_k = \begin{cases}
x_k & \text{for } 1 \leq k \leq m \\
x'_{k-m} & \text{for } m+1 \leq k \leq m+n.
\end{cases}
$$

他の語、数列 $w''$は、数列 $w$の元を次に$w'$の元を書き込むことで得られます。 $w$ と $w'$ の合成は、一般に $ww'$ または $w.w'$ で表されます。 $w$と$w'$を並べるとときどきになると言われています。その後、構成 $l(w.w') = l(w) + l(w')$までに。

関係 $we = ew = w$ は、語 $w$ ごとに直ちに確立されます。 $w = (x_i)_{1 \leq i \leq m}$、$w' = (x'_j)_{1 \leq j \leq n}$、$w'' = (x''_k)_{1 \leq k \leq p}$ を 3 つの語とします。明らかに、語 $w(w'w'')$ と $(ww')w''$ はどちらも、次のように定義される語 $(y_l)_{1 \leq l \leq m+n+p}$ に等しいです。

$$
y_l = \begin{cases}
x_l & \text{if } 1 \leq l \leq m \\
x_{l-m} & \text{if } m+1 \leq l \leq m+n \\
x''_{l-m-n} & \text{if } m+n+1 \leq l \leq m+n+p.
\end{cases}
$$

上記は、合成 $(w, w') \mapsto w.w'$ の法則を用いて $\mathbf{X}$ に構築された語の集合が単位元 $e$ とのモノイドであることを示しています。それは $\mathrm{Mo}(\mathbf{X})$ で示され、$\mathbf{X}$ 上に構築された *自由モノイドと呼ばれます。 語の積の定義から、すべての語 $w = (x_i)_{1 \leq i \leq n}$ は積 $\prod_{i=1}^n x_i$ に等しいことがわかります。したがって、語は形 $x_1 \ldots x_n$ で書かれる可能性があります。

#### 命題 3 {#alg-i-s7-prop-3 .statement tag=05FJ}

*M をモノイドとする。 X のすべての写像 f を M 拡大するに、Mo(X) の準同型を M に一意に変換します。*

$g$を$\mathrm{Mo}(\mathbf{X})$の準同型を$M$に延長して$f$とします。 $w = (x_i)_{1 \leq i \leq n}$ が語の場合、モノイド $\mathrm{Mo}(\mathbf{X})$、よっての $w = \prod_{i=1}^n x_i$

$$
g(w) = \prod_{i=1}^n g(x_i) = \prod_{i=1}^n f(x_i)
$$

モノイド $M$ (§ 1, no. 2, 公式 (2)) で。これは$g$の一意性を証明します。

語 $w = (x_i)_{1 \leq i \leq n}$ ごとに $h(w) = \prod_{i=1}^n f(x_i)$ とします。 $\mathrm{Mo}(\mathbf{X})$ の積の結合性定理 (§ 1, no. 3, 定理 1) と定義は $h(ww') = h(w)h(w')$ を暗示します。慣例により、空の積 $h(e)$ は $M$ の単位元であり、$x \in \mathbf{X}$ の $h(x) = f(x)$ です。したがって、$h$ は、$\mathrm{Mo}(x)$ の準同型を $f$ に拡張した $M$ になります。

$u : \mathbf{X} \to \mathbf{Y}$を写像とします。 命題 3 までに、Mo(X) の Mo(Y) への準同型は 1 つだけ存在します。これは、X で u と一致するになります。それはMo(u)で表されます。 写像語 $(x_i)_{1 \leq i \leq n}$ から語 $(u(x_i))_{1 \leq i \leq n}$ です。マグマ (no. 1) の場合と同様に、方程式 Mo(v \circ u) = Mo(v) \circ Mo(u) が写像 $v : Y \to Z$ ごとに成立し、u がそうであれば Mo(u) が単射（それぞれ全単射、全単射）であることが示されます。 X の部分集合 S ごとに、Mo(S) は S によって生成された Mo(X) の部分モノイドと識別されます。

X を集合とし、$(u_\alpha, v_\alpha)_{\alpha \in I}$ を Mo(X) の元の順序付けられた対の族とします。 R を、Mo(X) の法則と互換性のある Mo(X) の同値関係とし、$(u_\alpha, v_\alpha)$ (§ 1, no. 6) によって生成します。モノイド Mo(X)/R は、X とリレーター* $(u_\alpha, v_\alpha)_{\alpha \in I}$ によって定義される *モノイドと呼ばれます。 h を Mo(X)/R に対する Mo(X) の正準射とします。すると h(X) によって Mo(X) が生成されます。

N をモノイド、$(n_x)_{x \in X}$ を N の元族とする。k を Mo(X) の射を N に置き換え、すべての $x \in X$ (命題 3) に対して $k(x) = n_x$ とする。すべての $\alpha \in I$ に対して $k(u_\alpha) = k(v_\alpha)$ の場合、すべての $x \in X$ (§ 1, no. 6、命題 9) に対して $f(h(x)) = n_x$ となるようなマグマ射 $f : Mo(X)/R \to N$ が 1 つだけ存在します。 k はユニタルであるため、f はモノイド射です。

### 3. モノイドの融合和

*$(M_i)_{i \in I}$ はモノイド族を表し、$e_i$ 単位元は $M_i$ を表します。モノイド A と準同型 $h_i : A \to M_i$ ($i \in I$ の場合)* の族が与えられています。

家族 $(M_i)_{i \in I}$ の集合 S 和には、$i \in I$ と $x \in M_i$ を含む、注文された対 $(i, x)$ が元あります。 $M_i$ の $i \in I$、$x, x'$ を含むすべてのトリプル $\alpha = (i, x, x')$ について、$u_\alpha = (i, xx')$ と $v_\alpha = (i, x).(i, x')$ を書き込みます。 $I \times I \times A$ のトリプル $\lambda = (i, j, a)$ ごとに、$p_\lambda = (i, h_i(a))$ と $q_\lambda = (j, h_j(a))$ を書き込みます。すべての $i \in I$ には、$\varepsilon_i = (i, e_i)$ と書きます。 S と関係子 $(u_\alpha, v_\alpha)$、$(p_\lambda, q_\lambda)$、$(\varepsilon_i, e)$ によって定義されるモノイド M は、族* $(M_i)_{i \in I}$ *A によって * 融合された *和と呼ばれます。$\phi$ が M 上の Mo(S) の標準準同型を表し、$\phi_i(x) = \phi(i, x)$ と書きます。 $(i, x) \in S$。 $\phi_i$ は $M_i$ の *標準写像* を M に変換したものであると言われています。すべての $a \in A$ に対して、元 $\phi(i, h_i(a))$ は i から独立しており、$h(a)$ で表されます。\footnote{I が空の場合、$M = \{e\}$ と$a \in A$ 全員に対して$h(a) = e$。}

生成元とリレーター (no. 2) によって定義されるモノイドの普遍性は、次の結果を意味します。

#### 命題 4 {#alg-i-s7-prop-4 .statement tag=05FK}

(a) *すべての $i \in I$ について、写像 $\phi_i$ は、$M_i$ の準同型を M に変換し、すべての $i \in I$ については $\phi_i \circ h_i = h$ です。さらに、M は $\bigcup_{i \in I} \phi_i(M_i)$ によって生成されます。*

(b) *$M'$ をモノイドとし、$f' : M_i \to M'$ ($i \in I$ の場合) 準同型を、$f_i \circ h_i$ が $i \in I$ から独立であるようにします。すべての $i \in I$ に対して $f_i = f \circ \phi_i$ となるような準同型 $f : M \to M'$ が 1 つだけ存在します。*

以下では、次のようにします仮定:

(A) *すべての $i \in I$ に対して、$A \times P_i$ の $M_i$ への写像 $(a, p) \mapsto h_i(a).p$ が全単射となるように、$M_i$ 含む $e_i$ の部分集合 $P_i$ が存在します。

これは、準同型 $h_i$ が単射であることを意味します。 $x \in M$ にしましょう。 有限列 $\sigma = (a; i_1, \ldots, i_n; p_1, \ldots, p_n)$ と $a \in A, i_\alpha \in I$ および $p_\alpha \in P_{i_\alpha}$ ($1 \leq \alpha \leq n$、満たす)

$$
x = h(a) \cdot \prod_{\alpha=1}^n \phi_{i_\alpha}(p_\alpha)
$$

は $x$ の分解と呼ばれます。 整数 $n \geq 0$ は、分解 $\sigma$ の長さと呼ばれ、$l(\sigma)$ で表されます。 数列 $(e)$ は、長さの分解 、$M$ の単位元の 0 です。 分解 $\sigma$ は、$1 \leq \alpha < n$ に対して $i_\alpha \neq i_{\alpha+1}$ が、$1 \leq \alpha \leq n$ に対して $p_\alpha \neq e_{i_\alpha}$ の場合、還元と呼ばれます。

#### 命題 5 {#alg-i-s7-prop-5 .statement tag=05FL}

仮定 (A) では、$M$ のすべての元 $x$ は、一意の縮小された分解 $\sigma$ を認めます。 $x$ のすべての分解 $\sigma' \neq \sigma$ は $l(\sigma') > l(\sigma)$ を満たします。

(A) 削減された分解の一意性:

$\Sigma$ は、数列 $\sigma = (a; i_1, \ldots, i_n; p_1, \ldots, p_n)$ の集合を、$1 \leq \alpha \leq n$ に対して $n \geq 0$、$a \in A, i_\alpha \in I$、$p_\alpha \in P_{i_\alpha} - \{e_{i_\alpha}\}$ を表し、$1 \leq \alpha < n$ に対して$i_\alpha \neq i_{\alpha+1}$ を表すものとします。 $\Phi$ は、次のように定義される $\Sigma$ の写像を $M$ に表すものとします。

$$
\Phi(a; i_1, \ldots, i_n; p_1, \ldots, p_n) = h(a) \cdot \prod_{\alpha=1}^n \phi_{i_\alpha}(p_\alpha).
$$

$x \in M$ の縮小された分解は、$\Sigma$ の元 $\sigma$ となり、$\Phi(\sigma) = x$ になります。

For all $i \in I$, let $\Sigma_i$ be the subset of $\Sigma$ consisting of the sequences $(e; i_1, \ldots, i_n; p_1, \ldots, p_n)$ with $i \neq i_1$ when $n > 0$. させて

$$
\sigma = (e; i_1, \ldots, i_n; p_1, \ldots, p_n)
$$

$M_i$ の $\Sigma_i$ と $\xi$ にあります。 $\xi = h_i(a) \cdot p$ を $a \in A$ と $p \in P_i$ にします、そして

$$
\Psi_i(\xi, \sigma) = \begin{cases}
(a; i_1, \ldots, i_n; p_1, \ldots, p_n) & \text{if } p = e_i \\
(a; i, i_1, \ldots, i_n; p, p_1, \ldots, p_n) & \text{if } p \neq e_i.
\end{cases}
$$

$\Psi_i$が$\Sigma$に$M_i \times \Sigma_i$の全単射が加わった明らかです。

$i \in I$ と $x \in M_i$ としましょう。 $\Psi_i$ は全単射であるため、$\Sigma$ の写像 $f_{i,x}$ はそれ自体に次のように定義されます。

$$
f_{i,x}(\Psi_i(\xi, \sigma)) = \Psi_i(x\xi, \sigma) \quad (\xi \in M_i, \sigma \in \Sigma_i).
$$

さらに、$a \in A, f_a$ は、次のように定義される $\Sigma$ の写像を意味します。

$$
f_a(a'; i_1, \ldots, i_n; p_1, \ldots, p_n) = (aa'; i_1, \ldots, i_n; p_1, \ldots, p_n).
$$

Clearly $f_{i,e_i}$ is the identity mapping of $\Sigma$ and $f_{i,xx'} = f_{i,x} \circ f_{i,x'}$ for $x, x'$ in $M_i$ and $f_{i,h_i(a)} = f_a$ for $a \in A$ and $i \in I$.

Then Proposition 4 may be applied to the case where $M'$ is the monoid of mappings of $\Sigma$ into itself with law of composition $(f,f') \mapsto f \circ f'$ and where f_i is the homomorphism $x \mapsto f_{i,x}$ of $M_i$ into $M'$; then there exists a homomorphism $f$ of $M$ into $M'$ such that $f_{i,x} = f(\phi_i(x))$ for $i \in I$ and $x \in M_i$. しましょう
$$
\sigma = (a; i_1, \ldots, i_n; p_1, \ldots, p_n)
$$
$\Sigma$にいます。 式 (5) から (7) は、$n$ 関係に対する帰納法によって暗示されます。
$$
\begin{align*}
\sigma &= (f_a \circ f_{i_1, p_1} \circ \cdots \circ f_{i_n, p_n})(e) \\
&= f(h(a)\phi_{i_1}(p_1) \ldots \phi_{i_n}(p_n))(e),
\end{align*}
$$
それは$\sigma = f(\Phi(\sigma))(e)$です。 これは、$\Phi$ が単射であることを証明します。

(B) *分解*の存在:

$D$ を分解を認める $M$ の元の集合とします。次に、$e \in D$ と $M$ は $\bigcup_{i \in I} \phi_i(M_i)$ によって生成され、したがって $h(A) \cup \bigcup_{i \in I} \phi_i(P_i)$ によって生成されます。次に、すべての $i \in I$ に対して $D.\phi_i(P_i) \subset D$ です。 $D = M$ を証明するには、関係 $D.h(A) \subset D$ を証明すれば十分です。これは、次のより正確な補題から導き出されます。

#### 補題 1 {#alg-i-s7-lem-1 .statement tag=05FM}

※$1 \leq \alpha \leq n$の$I$には$i_1, \ldots, i_n$、$P_{i_\alpha}$には$p_\alpha$を入れます。すべての $a \in A$ に対して、$p'_\alpha \in P_{i_\alpha}$ を含む $a' \in A$ と数列 $(p'_\alpha)_{1 \leq \alpha \leq n}$ が存在します*
$$
\phi_{i_1}(p_1) \ldots \phi_{i_n}(p_n)h(a) = h(a')\phi_{i_1}(p'_1) \ldots \phi_{i_n}(p'_n).
$$
$h(a) = \phi_{i_n}(h_{i_n}(a))$ そして、$a_n \in A$ と $p'_n \in P_{i_n}$ が存在します
$$
p_n \cdot h_{i_n}(a) = h_{i_n}(a_n) \cdot p'_n.
$$
したがって、$\phi_{i_n}(p_n)h(a) = h(a_n)\phi_{i_n}(p'_n)$、よってとなります。
$$
\phi_{i_1}(p_1) \ldots \phi_{i_{n-1}}(p_{n-1})\phi_{i_n}(p_n)h(a) = \phi_{i_1}(p_1) \ldots \phi_{i_{n-1}}(p_{n-1})h(a_n)\phi_{i_n}(p'_n);
$$
補題は、これから$n$の帰納法までに続きます。

(C) *証明* 終了:

$x \in M$ を、$n$ を $x$ の分解のうち長さの最小値とします。 長さ $n$ の $x$ のすべての分解 $\sigma$ が減少することを証明します。これにより、$x$ の縮小された分解の存在が確立されます。縮小された分解の一意性は、$x$ の分解 $\sigma' \neq \sigma$ ごとに $l(\sigma') > l(\sigma)$ を意味します。

$n = 0$ の場合は自明なので、$n > 0$ と仮定します。しましょう
$$
\sigma = (a; i_1, \ldots, i_n; p_1, \ldots, p_n)
$$
分解/$x$/長さ$n$になります。 $1 \leq \alpha \leq n$と$p_\alpha = e_{i_\alpha}$を含む整数$\alpha$が存在した場合、数列
$$
(a; i_1, \ldots, i_{\alpha-1}, i_{\alpha+1}, \ldots, i_n; p_1, \ldots, p_{\alpha-1}, p_{\alpha+1}, \ldots, p_n)
$$

長さ $n - 1$ の $x$ のうち分解になりますが、これは除外されます。 $1 \leq \alpha < n$ と $i_{\alpha} = i_{\alpha + 1}$ を含む整数 $\alpha$ が存在すると仮定します。
$$
p_{\alpha} p_{\alpha + 1} = h_{i_{\alpha}}(a') \cdot p'_{\alpha}
$$
$a' \in \mathbf{A}$ と $p'_{\alpha} \in P_{i_{\alpha}}$ で。 補題 1 によって元 $a'' \in \mathbf{A}$ が存在します、
$$
p'_{1} \in P_{i_{1}}, \ldots, p'_{\alpha - 1} \in P_{i_{\alpha - 1}}
$$
そのような
$$
\phi_{i_{1}}(p_{1}) \cdots \phi_{i_{\alpha - 1}}(p_{\alpha - 1}) h(a') = h(a'') \phi_{i_{1}}(p'_{1}) \cdots \phi_{i_{\alpha - 1}}(p'_{\alpha - 1})
$$
そして数列
$$
(aa''; i_{1}, \ldots, i_{\alpha - 1}, i_{\alpha}, i_{\alpha + 2}, \ldots, i_{n}; p'_{1}, \ldots, p'_{\alpha - 1}, p'_{\alpha}, p_{\alpha + 2}, \ldots, p_{n})
$$
は長さ $n - 1$ の $x$ の分解であり、矛盾しています。

したがって、$\sigma$ が減少することが証明されました。

#### 系 {#alg-i-s7-n3-cor-1 .statement tag=05FN}

※仮定 (A) 準同型 $\phi_{i}$ と $h$ は単射法です。 $i \neq j$ の場合、$I$、$\phi_{i}(M_{i}) \cap \phi_{j}(M_{j}) = h(\mathbf{A})$。*

まず、$h$ は単射法です。$h(a) = h(a')$ の場合、$(a)$ と $(a')$ は、$M$、よって $a = a'$ の同じ元を 2 つ縮小した分解です。 $i \in I$ にしましょう。次に$h(\mathbf{A}) = \phi_{i}(h_{i}(\mathbf{A})) \subset \phi_{i}(M_{i})$; 分解の削減の一意性は、
$$
h(\mathbf{A}) \cap \phi_{i}(M_{i} - h_{i}(\mathbf{A})) = \varnothing,
$$
よって $\phi_{i}(M_{i} - h_{i}(\mathbf{A})) = \phi_{i}(M_{i}) - h(\mathbf{A})$。

準同型 $\phi_{i}$ と関係の単射性
$$
\phi_{i}(M_{i}) \cap \phi_{j}(M_{j}) \subset h(\mathbf{A})
$$
$i \neq j$ については、次の事実の帰結になります: $I$ の $i, j$、$M_{i} - h_{i}(\mathbf{A})$ の $x$、$M_{j} - h_{j}(\mathbf{A})$ の $y$ については、関係 $\phi_{i}(x) = \phi_{j}(y)$ は $i = j$ を暗示します。 $x = y$。 $x = h_{i}(a) \cdot p$と$y = h_{j}(b) \cdot q$を$\mathbf{A}$の$a, b$、$P_{i} - \{e_{i}\}$の$p$、$P_{j} - \{e_{j}\}$の$y$とします。すると、$\phi_{i}(x) = h(a)\phi_{i}(p)$と$\phi_{j}(y) = h(b)\phi_{j}(q)$、したがって、$(a; i; p)$と$(b; j; q)$は、同じ$M$の元を2つ減じた分解になります。したがって、$i = j, a = b$ と $p = q$、よって $x = h_{i}(a)p = h_{j}(b)q = y$ が続きます。

仮定 (A) が満たされると、$M$ の部分モノイドを$\phi_{i}$ によって同一視するの各モノイド$M_{i}$ とします。同様に、$M$の部分モノイドを$h$までに同一視する$\mathbf{A}$とします。次に、$\bigcup_{i \in I} M_{i}$と$M_{i} \cap M_{j} = \mathbf{A}$により$i \neq j$に対して$M$が生成されます。

$M$ のすべての元は、$1 \leq \alpha < n$ に対して $a \in \mathbf{A}, p_{1} \in P_{i_{1}} - \{e\}, \ldots, p_{n} \in P_{i_{n}} - \{e\}$ と $i_{\alpha} \neq i_{\alpha + 1}$ を使用して、形 $a \prod_{\alpha = 1}^{n} p_{\alpha}$ で一意に記述することができます。最後に、$M'$ がモノイドで、$(f_{i}: M_{i} \to M')$ ($i \in I$ の場合) 制限から $\mathbf{A}$ が$\mathbf{A}$ から $M'$ への準同型と同じ準同型の族である場合、存在するのは 1 つだけです。 準同型 $f: M \to M'$ は、すべての $i \in I$ に対して $M_{i}$ に $f_{i}$ を誘導します。

仮定 (A) は 2 つの重要なケースで満たされます。

(a) $A = \{e\}$。この場合、モノイド族 $(M_i)_{i \in I}$ があり、$M$ はこの族の *モノイド和* と呼ばれます。各 $M_i$ は $M$ の部分モノイドで識別され、$M$ は $\bigcup_{i \in I} M_i$ によって生成されます。さらに、$i \neq j$に対して$M_i \cap M_j = \{e\}$。 $M$ のすべての元は、形 $x_1 \ldots x_n$ で一意に記述できます。
$$
x_1 \in M_{i_1} - \{e\}, \ldots, x_n \in M_{i_n} - \{e\}
$$
$1 \leq \alpha \leq n$の場合は$i_\alpha \neq i_{\alpha+1}$。最後に、準同型 $(f_i : M_i \to M')$ の各家族には、一意な準同型 $f : M \to M'$ が存在し、その制限から $M_i$ までの$i \in I$ はすべて $f_i$ になります。

(b) 部分群と同じ群 $A$ として群 $(G_i)_{i \in I}$ 含むの族があり、$h_i$ は $A$ の単射から $G_i$ になります。 $A$ によって結合された族 $(G_i)_{i \in I}$ の和は *群* $G$ になります。モノイド $G$ は $\bigcup_{i \in I} \phi_i(G_i)$ によって生成され、$\bigcup_{i \in I} \phi_i(G_i)$ のすべての元は逆を認めます$G$ (cf. § 2, no. 3、系 1 ～ 命題 4); $I = \{1, 2\}$の場合は$*_A G_i$または$G_1 *_A G_2$で表されます。 $A$が単位元で構成される場合、$G$は群の家族*$(G_i)_{i \in I}$の*自由な積であるとも言われ、$* G_i$（$I = \{1, 2\}$の場合は$G_1 * G_2$）で表されます。

### 4. 自由モノイドへの応用

#### 補題 2 {#alg-i-s7-lem-2 .statement tag=05FO}

*$M$ をすべての $x \in X$ に対して $M_x = \mathbf{N}$ によって定義されるファミリー $(M_x)_{x \in X}$ のモノイド和とし、$\phi_x$ は $M_x$ の標準準同型を$M$ に表すものとします。 写像 $x \mapsto \phi_x(1)$ の $X$ を $M$ 拡大するから同型 $h$ の $\mathrm{Mo}(X)$ を $M$ に。

$h$ を $\mathrm{Mo}(X)$ の準同型を $h(x) = \phi_x(1)$ で特徴付けられる $M$ にします。 整数 $n \geq 0$、$\phi_x(n) = \phi_x(1)^n = h(x)^n$ ごとに、$M$ は $\bigcup_{x \in X} \phi_x(\mathbf{N})$ によって生成されるため、$h(X)$ によっても生成されます。 したがって、$h$ は *全射* です。 さらに、$X$ のすべての $x$ について、写像 $n \mapsto x^n$ は $\mathbf{N} = M_x$ の $\mathrm{Mo}(X)$ の準同型です。したがって、$x \in X$ と $n \in \mathbf{N}$ に対して $h'(\phi_x(n)) = x^n$ となるように、$M$ の $\mathrm{Mo}(X)$ に (no. 3, 命題 4) 準同型 $h'$ が存在します。特に、$x \in X$ に対する $h'(h(x)) = x$ であるため、$h' \circ h$ は $\mathrm{Mo}(X)$ の同一性準同型です。 したがって、$h$ は *単射* です。 したがって、$h$ は全単射であることが証明されました。

#### 命題 6 {#alg-i-s7-prop-6 .statement tag=05FP}

*$w$を$\mathrm{Mo}(X)$の元とします。
(a) $X$ および整数 $m(\alpha) > 0$ のうち、整数 $n \geq 0$、元 $x_\alpha$ が存在します（

† $G_1 * G_2$ は、*集合理論*、IV, § 2, no. 4 という意味での $G_1$ と $G_2$ の「積」ではないことに注意してください（また、「カテゴリの理論」という意味でも、この理論、$G_1 * G_2$ は$G_1$と$G_2$の「和」）。

$1 \leq \alpha \leq n$ は、$1 \leq \alpha < n$ と $w = \prod_{\alpha=1}^n x_\alpha^{m(\alpha)}$ に対して $x_\alpha \neq x_{\alpha+1}$ になります。 数列 $(x_\alpha, m(\alpha))_{1 \leq \alpha \leq n}$ はこれら条件によって一意に決まります。

(b) $p$ を正の整数、$X$ で $x'_\beta$、$1 \leq \beta \leq p$ に対して$\mathbf{N}$ で $m'(\beta)$ を$w = \prod_{\beta=1}^p {x'}^{m'(\beta)}$ とする。次に$p \geq n$。 $p = n$なら$x'_\beta = x_\beta$、$1 \leq \beta \leq p$なら$m'(\beta) = m(\beta)$。

補題 2 の記法では、$x \in X$ と $n \in \mathbf{N}$ は $h^{-1}(\phi_x(n)) = x^n$ です。 命題 6 は、no. 3、命題 5 から続きます。

### 5. 無料群

すべての$x \in X$を$G_x = \mathbf{Z}$とします。ファミリ $(G_x)_{x \in X}$ のフリー 積は、* $X$ 上に構築された * フリー 群と呼ばれ、$F(X)$ で示されます。 $\phi_x$ は $G_x = \mathbf{Z}$ の標準準同型を $F(X)$ に表すものとします。 no. 3、系から命題 5、写像 $x \mapsto \phi_x(1)$ $X$ から $F(X)$ までは単射です。この写像の下の $F(X)$ に像を加えて同一視する $X$ とします。次に、$X$ 生成する $F(X)$ と $e \notin X$ です。

適用 no. 3、命題 5、次の結果が得られます。

#### 命題 7 {#alg-i-s7-prop-7 .statement tag=05FQ}

*g を無料の群* $F(X)$ の元とします。 *整数* $n \geq 0$ *および数列* $(x_\alpha, m(\alpha))_{1 \leq \alpha \leq n}$ *関係* $x_\alpha \in X$、$x_\alpha \neq x_{\alpha+1}$ *for* $1 \leq \alpha < n$、$m(\alpha) \in \mathbf{Z}$、$m(\alpha) \neq 0$ *for* $1 \leq \alpha \leq n$、 *そして* $g = \prod_{\alpha=1}^n x_\alpha^{m(\alpha)}$。

無料の群 $F(X)$ では、次の普遍性をお楽しみいただけます。

#### 命題 8 {#alg-i-s7-prop-8 .statement tag=05FR}

*G を群および f 写像 of* $X$ *into G とする。 拡大する f* となる準同型* $\bar{f}$ *of* $F(X)$ *into G が 1 つだけ存在します。

$\bar{f}$ の一意性は、群 $F(X)$ が $X$ によって生成されるという事実から帰結します。 $X$ のすべての $x$ について、$f_x$ を $\mathbf{Z}$ の準同型 $n \mapsto f(x)^n$ から $G$ にします。 By no. 3, Proposition 4, there exists a homomorphism $\bar{f}$ of $F(X)$ into $G$ such that $\bar{f}(x^n) = f_x(n)$ for $x \in X$ and $n \in \mathbf{Z}$; in particular, $\bar{f}(x) = f_x(1) = f(x)$ for all $x \in X$ and hence $\bar{f}$ extends $f$.

$u : X \to Y$を写像とします。 命題 8 までに、$F(X)$ の準同型が $F(Y)$ に 1 つだけ存在し、$X$ に $u$ が付いた一致するになります。それは$F(u)$で示されます。マグマの場合と同様 (no. 1) 公式

$$
F(v \circ u) = F(v) \circ F(u)
$$

は写像 $v : Y \to Z$ ごとに成立し、$u$ がそうである場合、$F(u)$ は単射（それぞれ全単射、全単射）であることが示されます。 $X$ の部分集合 $S$ ごとに、$F(S)$ は $S$ によって生成された $F(X)$ の部分群と識別されます。

Iを集合とします。場合によっては、I の同一視する $i$ を、フリーの群 $F(I)$ の標準像 $\phi_i(1)$ としないことが重要です。後者は$T_i$ (場合によっては$T'_i, X_i, \ldots$) で表され、添字 $i$ の *不定* と呼ばれます。フリーの群 $F(I)$ は、$I = \{1, 2, \ldots, n\}$ の場合は $F((T_i)_{i \in I})$ または $F(T_1, \ldots, T_n)$ で表されます。

$G$ を群とし、$t = (t_i)_{i \in I}$ を $G$ の元の家族とします。 命題 8 までに、すべての $i \in I$ に対して $f_t(T_i) = t_i$ を特徴とする $F((T_i)_{i \in I})$ の $G$ に準同型 $f_t$ が存在します。 The image of an element $w$ of $F((T_i)_{i \in I})$ under $f_t$ will be denoted by $w(t)$ or $w(t_1, \ldots, t_n)$ if $I = \{1, 2, \ldots, n\}$; $w(t)$ is said to result from the *substitution* $T_i \mapsto t_i$ in $w$. 特に、$G = F((T_i)_{i \in I})$ と $(t_i) = (T_i) = T, f_T$ が $G$、よって $w(T) = w$ の同一性準同型である場合、 $I = \{1, 2, \ldots, n\}$ の場合は、次に $w(T_1, \ldots, T_n) = w$ です。

$G$と$G'$を、$G$の2つの群、$u$準同型を$G$の元の$G'$と$t = (t_1, \ldots, t_n)$有限列とします。 $t' = (u(t_1), \ldots, u(t_n))$ にしましょう。 $F(T_1, \ldots, T_n)$ の準同型 $u \circ f_t$ を $G'$ 写像 $T_i$ から $u(t_i)$ にすると、$1 \leq i \leq n$ となり、$f_{t'}$ に等しくなります。 $F(T_1, \ldots, T_n)$ の $w$ の場合、

$$
u(w(t_1, \ldots, t_n)) = w(u(t_1), \ldots, u(t_n)).
$$

$F(T_1, \ldots, T_n)$ に $w$ を与え、フリーの群 $F(T'_1, \ldots, T'_m)$ に元 $v_1, \ldots, v_n$ を与えます。 $F(T'_1, \ldots, T'_m)$ の $T_i \mapsto v_i$ 定義する元 $w' = w(v_1, \ldots, v_n)$ の置換。 $G$ を $G$ の群、$t_1, \ldots, t_m$ 元、および $F(T'_1, \ldots, T'_m)$ の $u$ 準同型を、$1 \leq j \leq m$ の $u(T'_j) = t_j$ で特徴付けられる $G$ とします。次に$u(v_i) = v_i(t_1, \ldots, t_m)$と$u(w') = w(t_1, \ldots, t_m)$。 公式 (8) はつまり、

$$
w'(t_1, \ldots, t_m) = w(v_1(t_1, \ldots, t_m), \ldots, v_n(t_1, \ldots, t_m)).
$$

これにより、「機能的な記法」 $w(t_1, \ldots, t_n)$ が正当化されます。読者は、拡大する式 (8) と (9) から任意のインデックス付け集合の場合に任せられます。

### 6. 群のプレゼンテーション

$G$ を群とし、$t = (t_i)_{i \in I}$ を $G$ の元の家族とします。 $f_t$を自由な群$F(I)$の一意な準同型を$G$とし、写像$i$を$t_i$にします。 $f_t$の像は、$G$の元$t_i$によって生成された部分群です。 $f_t$の核の元は、家族$t$の*関係者*と呼ばれます。 $f_t$ が全射（単射、全単射）の場合、$t$ は *生成する* (それぞれ *free*、*basic*) と呼ばれます。

$G$を群とします。 $G$ の *プレゼンテーション* は、生成するファミリー $\mathbf{t} = (t_i)_{i \in I}$ の順序付けられた対 $(\mathbf{t}, \mathbf{r})$ からなると、$f_t$ の核 $N_t$ が元によって生成されるようなリレーターのファミリー $\mathbf{r} = (r_j)_{j \in J}$ です。 $g \in F(I)$と$j \in J$の場合は$gr_jg^{-1}$。 $N_t$は$j \in J$の$r_j$によって生成された$F(I)$の通常の部分群である（他の語、最小のは$F(I)$含むの通常の部分群である）と言うのと同じことになります。 元 $r_j$ ($j \in J$)、cf. § 4, no. 4)。言葉の乱用により、生成元 $t_i$ と関係 $r_j(\mathbf{t}) = e$ は、群 $G$ の *プレゼンテーション* を構成するといわれています。

I を集合とし、$r = (r_j)_{j \in J}$ を自由な群 $F(I)$ の元の族とします。 $N(r)$を、$j \in J$の$r_j$によって生成された$F(I)$の通常の部分群とします。 $F(I, r) = F(I)/N(r)$ と $\tau_i$ が $N(r)$ を法とする $i$ の類を表すものとします。 $\tau = (\tau_i)_{i \in I}$ とともに注文された対 $(\tau, r)$ は、群 $F(I, r)$ のプレゼンテーションです。 $G$ が群で、$(t, r)$ が $t = (t_i)_{i \in I}$ を伴う $G$ の表現である場合、$F(I, r)$ から $G$ 上に$u(\tau_i) = t_i$ となる固有の同型 $u$ が存在します。 $i \in I$。 群 $F(I, r)$ は、生成元 $\tau_i$ とその関係者 $r_j$ によって定義されていると言われたり、言葉の乱用によって *生成元 $\tau_i$ と関係* $r_j(\tau) = e$ によって定義されていると言われています。 $I = \{1, n\}$と$J = \{1, m\}$のとき、$F(I, r)$はプレゼンテーションによって定義されると言われています

$$
\langle \tau_1, \ldots, \tau_n; r_1, \ldots, r_m \rangle.
$$

$r_j = u_j^{-1} v_j$ と $u_j$ および $v_j$ が $F(I)$ の場合、このプレゼンテーションは同じ記号で表されます。

$$
\langle \tau_1, \ldots, \tau_n; u_1 = v_1, \ldots, u_m = v_m \rangle.
$$

#### 例 {#alg-i-s7-n6-exa-1 .statement tag=05FS}

(1) プレゼンテーション$\langle \tau; \tau^q = e \rangle$ で定義された群は、位数 $q$ の循環です。

(2) プレゼンテーション $\langle x, y; xy = yx \rangle$ で定義された群は $\mathbf{Z} \times \mathbf{Z}$ と同型です。

#### 命題 9 {#alg-i-s7-prop-9 .statement tag=05FT}

*$G$を群、$t = (t_i)_{i \in I}$生成するを$G$の家族、$r = (r_j)_{j \in J}$を$t$の親戚の家族とする。次の条件は同等です:*

(a) *注文した対* $(t, r)$ *は $G$ のプレゼンテーションです。

(b) *$G'$ *を群とし、* $t' = (t'_i)_{i \in I}$ *元の* $G'$の家族とする。 *もし* $r_j(t') = e$ *すべてに* $j \in J$、*存在する* 準同型* $u$ *の* $G$ *に* $G'$ *そのような* $u(t_i) = t'_i$ *すべてに* $i \in I$。

(c) *$\overline{G}$ *を群とし、* $\bar{t} = (\bar{t}_i)_{i \in I}$ *生成するの家族* $\overline{G}$ *そのような* $r_j(\bar{t}) = e$ *すべてについて* $j \in J$ とします。 *Every homomorphism of* $\overline{G}$ *into* $G$ *which maps* $\bar{t}_i$ *to* $t_i$ *for all* $i \in I$ *is an isomorphism*.

Let $f$ denote the homomorphism of $F(I)$ into $G$ which maps $i$ to $t_i$ for all $i \in I$ and $N$ the kernel of $f$.

(a) $\Rightarrow$ (b): $(t, r)$ が $G$ のプレゼンテーションであると仮定し、$t' = (t'_i)_{i \in I}$ を群 $G'$ の元とすべての $j \in J$ に対する $r_j(t') = e$ の族とする。 $f'$ を $F(I)$ の準同型から、すべての $i \in I$ について $f'(i) = t'_i$ によって特徴付けられる $G'$ とします。 すべての $j \in J$ については仮定 $f'(r_j) = e$ によって、また、$N$ は $j \in J$ と $g \in F(I), f'(N) = \{e\}$ については元 $gr_jg^{-1}$ によって生成されます。 準同型 $f \colon F(I) \to G$ は核 $N$ と全射なので、 $f' = u \circ f$ となるような準同型 $u \colon G \to G'$ が存在します。 次に$u(t_i) = u(f(i)) = f'(i) = t'_i$。

(b) $\Rightarrow$ (c): 条件 (b) が成り立つとします。 $t = (t_i)_{i \in I}$ を、すべての $j \in J$ に対して $r_j(t) = e$ となるように、群 $G$ の生成するファミリーとし、$v$ を、すべての $i \in I$ に対して $v(\bar{t}_i) = t_i$ となるように、$\overline{G}$ の $G$ である準同型とします。家族 $(t_i)_{i \in I}$ 生成する $G$ として、準同型 $v$ は*全射*です。 性質 (b) までに、すべての $i \in I$ に対して $u(t_i) = \bar{t}_i$ となるような準同型 $u \colon G \to \overline{G}$ が存在します。すると、すべての $i \in I$ に対して $u(v(\bar{t}_i)) = \bar{t}_i$ となり、したがって $u \circ v$ は $\overline{G}$ 上の恒等となり、$v$ が単射であることが証明されます。したがって、$v$ は同型であり、条件 (c) が成り立ちます。

(c) $\Rightarrow$ (a): 条件 (c) が成り立つとします。 $t'_i$ を $F(I, r)$ と $t' = (t'_i)_{i \in I}$ の $i$ の標準像とします。 then $r_j(t') = e$ for all $j \in J$. As $r_j(t) = e$ for all $j \in J$, there exists one and only one homomorphism $v$ of $F(I, r)$ into $G$ such that $v(t_i) = t_i$ for all $i \in I$. By (c), $v$ is an isomorphism of $F(I, r)$ onto $G$ which transforms the presentation $(t', r)$ of $F(I, r)$ into a presentation $(t, r)$ of $G$.

### 7. 自由可換群とモノイド

$X$ のすべての写像を $\mathbf{Z}$ に変換する集合 $\mathbf{Z}^X$ は、$(\alpha + \beta)(x) = \alpha(x) + \beta(x)$ ($\alpha, \beta \in \mathbf{Z}^X, x \in X$) で定義される法則の下で可換群です。 $\mathbf{Z}^X$ の元は、マルチインデックスと呼ばれるときどきです。 0で示される単位元は、値0を持つ定数写像です。$\alpha \in \mathbf{Z}^X$、$x \in X$の集合$S_\alpha$の場合、$\alpha(x) \neq 0$は$\alpha$のサポートと呼ばれます。次に、$\mathbf{Z}^X$の$\alpha, \beta$に対して$S_0 = \varnothing$と$S_{\alpha+\beta} \subset S_\alpha \cup S_\beta$。したがって、写像 $\alpha : X \to \mathbf{Z}$の有限台の集合 $\mathbf{Z}^{(X)}$は、$X$で構築された自由可換群と呼ばれる$\mathbf{Z}^X$の部分群です。

すべての $x \in X$ について、$\delta_x$ は次のように定義される $\mathbf{Z}^{(X)}$ の元を表すものとします。

$$
\delta_x(y) = \begin{cases}
1 & \text{if } y = x \\
0 & \text{if } y \neq x.
\end{cases}
$$

また、$\alpha$の$\alpha \in \mathbf{Z}^{(X)}$、整数、$|\alpha|$、長さは公式で定義されます。

$$
|\alpha| = \sum_{x \in X} \alpha(x).
$$

次の関係が直ちに確立されます。

$$
\alpha = \sum_{x \in X} \alpha(x) \cdot \delta_x
$$
$$
|\delta_x| = 1, \quad |0| = 0
$$
$$
|\alpha + \beta| = |\alpha| + |\beta|
$$

$\mathbf{Z}^{(X)}$の$\alpha, \beta$と$X$の$x$。

位数関係 $\alpha \leq \beta$ は、すべての $x \in X$ に対して $\alpha(x) \leq \beta(x)$ によって $\mathbf{Z}^{(X)}$ で定義されます。 関係 $\alpha \leq \beta$ と $\alpha' \leq \beta'$ は、$\alpha + \alpha' \leq \beta + \beta'$、$|\alpha| \leq |\beta|$、$-\alpha \geq -\beta$ を暗示します。さらに、関係 $\alpha \leq \beta$ は $\beta - \alpha \geq 0$ と同等です。 $\mathbf{Z}^{(X)}$ の元 $\alpha \geq 0$ の集合は $\mathbf{N}^{(X)}$ で示されます。それは、$X$の写像の集合から有限台の$\mathbf{N}$になり、$\mathbf{Z}^{(X)}$の部分モノイドは、$X$で構築された自由可換モノイドと呼ばれます。 長さ 1 の元は、$\mathbf{N}^{(X)} - \{0\}$ の最小の元であり、$\delta_x$ ($x \in X$) の集合を構成します。

モノイド$\mathbf{N}^{(X)}$と群$\mathbf{Z}^{(X)}$は、次の普遍性を楽しんでいます。

#### 命題 10 {#alg-i-s7-prop-10 .statement tag=05FU}

*M を可換モノイド (それぞれ群) とし、X の f 写像を M にします。M には、すべての $x \in X$ に対して $g(\delta_x) = f(x)$ となるような $\mathbf{N}^{(X)}$ (それぞれ $\mathbf{Z}^{(X)}$) の準同型が 1 つだけ存在します。 *M が加法的に書かれている場合、* $\mathbf{N}^{(X)}$ のすべての $\alpha$ (それぞれ $\mathbf{Z}^{(X)}$) に対して $g(\alpha) = \sum_{x \in X} \alpha(x) \cdot f(x)$ になります。

$g$ を $\mathbf{N}^{(X)}$ (それぞれ $\mathbf{Z}^{(X)}$) の準同型を M にすると、すべての $x \in X$ に対して $g(\delta_x) = f(x)$ になります。 $\mathbf{N}^{(X)}$ (それぞれ $\mathbf{Z}^{(X)}$) のすべての $\alpha$ について、(12) から次のようになります。
$$
g(\alpha) = \sum_{x \in X} \alpha(x) \cdot g(\delta_x) = \sum_{x \in X} \alpha(x) \cdot f(x),
$$
$g$ のよって一意性。

$\mathbf{N}^{(X)}$ (それぞれ $\mathbf{Z}^{(X)}$) のすべての $\alpha$ については、$g(\alpha) = \sum_{x \in X} \alpha(x) \cdot f(x)$ と書きます。それから明らかに $g(0) = 0$; $\mathbf{N}^{(X)}$ の $\alpha, \beta$ (それぞれ $\mathbf{Z}^{(X)}$)、
$$
\begin{align*}
g(\alpha + \beta) &= \sum_{x \in X} (\alpha(x) + \beta(x)) \cdot f(x) \\
&= \sum_{x \in X} [\alpha(x) \cdot f(x) + \beta(x) \cdot f(x)] \\
&= \sum_{x \in X} \alpha(x) \cdot f(x) + \sum_{x \in X} \beta(x) \cdot f(x) \\
&= g(\alpha) + g(\beta)
\end{align*}
$$
したがって、$g$ は、$\mathbf{N}^{(X)}$ (それぞれ $\mathbf{Z}^{(X)}$) の準同型を M に変換します。また、$X$ の $y$ については、
$$
g(\delta_y) = \sum_{x \in X} \delta_y(x) \cdot f(x);
$$
現在は $x \neq y$ と $\delta_y(y) \cdot f(y) = f(y)$、よって $g(\delta_y) = f(y)$ に対して $\delta_y(x) \cdot f(x) = 0$ です。

$u : X \to Y$を写像とします。 命題 10 までに、$\mathbf{Z}^{(X)}$ の準同型が 1 つだけ存在し、$\mathbf{Z}^{(Y)}$ になり、すべての $x \in X$ に対して写像 $\delta_x$ から $\delta_{u(x)}$ になります。それは$\mathbf{Z}^{(u)}$で示されます。 写像 $\alpha \in \mathbf{Z}^{(X)}$ から元 $\beta \in \mathbf{Z}^{(Y)}$ が次のように定義されていることがすぐにわかります。
$$
\beta(y) = \sum_{x \in u^{-1}(y)} \alpha(x).
$$
マグマ (no. 1) の場合と同様に、写像 $v : Y \to Z$ ごとに公式 $\mathbf{Z}^{(v \circ u)} = \mathbf{Z}^{(v)} \circ \mathbf{Z}^{(y)}$ が確立されます。 $u$ が単射である場合、$\mathbf{Z}^{(u)}$ は単射（それぞれ全単射、全単射）であることも示されています。

S を X の部分集合とします。私が X への S の単射である場合、写像 $f = \mathbf{Z}^{(i)}$ は、$s \in S$ に対して元 $\delta_s$ によって生成された $\mathbf{Z}^{(X)}$ の部分群 H への $\mathbf{Z}^{(S)}$ の同型です。 (15)により、
$$
(f(\alpha))(x) = \begin{cases}
\alpha(x) & \text{if } x \in S \\
0 & \text{if } x \in X - S
\end{cases}
$$

したがって、$H$ は、$S$ に含まれるサポートの $\mathbf{Z}^{(X)}$ の元の集合です。今後、$\mathbf{Z}^{(S)}$ は $f$ によって $H$ と識別されます。

公式 (15) は、$\mathbf{Z}^{(u)}$ の制限から $\mathbf{N}^{(X)}$ 誘導する準同型 $\mathbf{N}^{(X)}$ の $\mathbf{N}^{(u)}$ が $\mathbf{N}^{(Y)}$ になることを示しています。その後、写像 $v : Y \to Z$ ごとに $\mathbf{N}^{(v \circ u)} = \mathbf{N}^{(v)} \circ \mathbf{N}^{(u)}$ が加算されます。さらに、$u$ がそうである場合、$\mathbf{N}^{(u)}$ は単射詞 (それぞれ全単射、全単射) です。 $S$ が $X$ の部分集合である場合、

$$
\mathbf{N}^{(S)} = \mathbf{Z}^{(S)} \cap \mathbf{N}^{(X)}.
$$

#### 注意 {#alg-i-s7-n7-rem-1 .statement tag=05FV}

$M$ を厳密に正の整数の乗法モノイドとし、$\mathfrak{P}$ を素数数 (§ 4, no. 10, 定義 15) の集合とします。 命題 10 までに、数 $p$ ごとに $u(\delta_p) = p$ で特徴付けられる $\mathbf{N}^{(\mathfrak{P})}$ の $M$ に準同型 $u$ が存在します。 次に、$\mathbf{N}^{(\mathfrak{P})}$ の $\alpha$ と § 4, no. 10 の定理 7 の $u(\alpha) = \prod_{p \in \mathfrak{P}} p^{\alpha(p)}$ は、$u$ が $H$ 上の $\mathbf{N}^{(\mathfrak{P})}$ の同型であることを示します。

### 8. 指数関数記法

$M$ を乗算的に書かれたモノイド、$u = (u_x)_{x \in X}$ を対で通勤する $M$ の元の家族とします。 Let $\alpha$ be in $\mathbf{N}^{(X)}$; the elements $u_x^{\alpha(x)}$ and $u_y^{\alpha(y)}$ of $M$ commute for $x, y$ in $X$ and there exists a finite subset $S$ of $X$ such that $u_x^{\alpha(x)} = 1$ for $x$ in $X - S$. したがって、次のように書くことができます。

$$
u^\alpha = \prod_{x \in X} u_x^{\alpha(x)}.
$$

$M'$ を、家族 $(u_x)_{x \in X}$ によって生成された $M$ の部分モノイドとします。これは可換です (§ 1, no. 5、系 2 から命題 4)。 There thus exists (no. 7, Proposition 10) a unique homomorphism $f$ of $\mathbf{N}^{(X)}$ into $M'$ such that $f(\delta_x) = u_x$ for all $x \in X$ and $f(\alpha) = u^\alpha$ for all $\alpha$ in $\mathbf{N}^{(X)}$. 次の式を導き出します

$$
u^{\alpha + \beta} = u^\alpha . u^\beta
$$
$$
u^0 = 1
$$
$$
u^{\delta_x} = u_x
$$

$\mathbf{N}^{(X)}$の$\alpha, \beta$と$X$の$x$。

$v = (v_x)_{x \in X}$ を $M$ の元の他の家族とします。 $X$ の $x, y$ に $v_x v_y = v_y v_x$ と $u_x v_y = v_y u_x$ があるとします。 次に、すべての $x \in X$ に対して $u_x \in L$ と $v_x \in L$ となるような $M$ の可換部分モノイド $L$ (§ 1, no. 5、系 2 から命題 4) が存在します。 The mapping $\alpha \mapsto u^\alpha . v^\alpha$ of $\mathbf{N}^{(X)}$ into $L$ is then a homomorphism (§ 1, no. 5, Proposition 5) mapping $\delta_x$ to $u_x . v_x$. したがって、公式となります。

$$
u^\alpha . v^\alpha = (u . v)^\alpha,
$$

ここで、$u . v$ はファミリー $(u_x . v_x)_{x \in X}$ です。

M が可換の場合、M の元のすべての族 $u$ に対して $u^\alpha$ が定義でき、制限がなくても式 (15) ～ (20) が成り立ちます。

### 9. さまざまなフリーオブジェクトの間の関係

自由モノイド Mo(X) はマグマであるため、no. 1 の命題 1 は、制限 ～ X が正体となる準同型 $\lambda : M(X) \to Mo(X)$ の存在を示します。同様に、自由群 F(X) は、X 拡大するから準同型 $\mu : Mo(X) \to F(X)$ (no. 2, 命題 3) のモノイド恒等写像です。 no. 4、命題 6 および no. 5、命題 7 までは、$\mu$ は単射法です。同様に、no. 7の命題 10とno. 5の命題 8は、すべての$x \in X$に対して$\nu(x) = \delta_x$と$\pi(x) = \delta_x$によって特徴付けられる準同型$\nu : Mo(X) \to N^{(X)}$と$\pi : F(X) \to Z^{(X)}$の存在を示しています。 $i$が$N^{(X)}$の単射を$Z^{(X)}$にすると、Mo(X)の2つの準同型$i \circ \nu$と$\pi \circ \mu$がXの$Z^{(X)}$一致するになり、 よって $i \circ \nu = \pi \circ \mu$。この状況は、次の可換図式で要約できます。

$$
\begin{array}{ccc}
M(X) & \xrightarrow{\lambda} & Mo(X) \\
& & \downarrow \mu \\
& & F(X) \xrightarrow{\pi} Z^{(X)}
\end{array}
$$

準同型 $\lambda, \mu, \nu$ と $\pi$ は正規と呼ばれます。

w を M(X) にします。 $l(w)$ の帰納法によって、語 $\lambda(w)$ の長さが w の長さと等しいことがすぐに示されます。さらに

$$
\nu(x_1 \ldots x_n) = \sum_{i=1}^n \delta_{x_i}
$$
X、よって $|\nu(x_1 \ldots x_n)| = n$ の $x_1, \ldots, x_n$ は (13) と (14) によって計算されます。その他語では、

$$
|\nu(u)| = l(u) \quad (u \in Mo(X)).
$$

#### 命題 11 {#alg-i-s7-prop-11 .statement tag=05FW}

*The canonical homomorphism $\nu$ of Mo(X) into $N^{(X)}$ is surjective.* Let $w = x_1 \ldots x_n$ and $w' = x'_1 \ldots x'_m$ be two elements of Mo(X); in order that $\nu(w) = \nu(w')$, it is necessary and sufficient that $m = n$ and that there exist a permutation $\sigma \in S_n$ with $x'_i = x_{\sigma(i)}$ for $1 \leq i \leq n$.

$\nu$ の像は、$N^{(X)}$ 含む元 $\delta_x$ ($x \in X$ の場合) の部分モノイド I です。 公式 (12) (no. 7) は、$I = N^{(X)}$ が $(\delta_x)_{x \in X}$ ファミリーによって$N^{(X)}$ が生成されることを示しています。したがって、$\nu$ は全射法です。

$1 \leq i \leq n$ に対して $m = n$ と $x'_i = x_{\sigma(i)}$ の場合、

$$
\nu(w') = \sum_{i=1}^n \delta_{x'_i} = \sum_{i=1}^n \delta_{x_{\sigma(i)}} = \sum_{i=1}^n \delta_{x_i} = \nu(w)
$$

公式 (21) および可換性定理 (§ 1, no. 5、定理 2) による。

逆に、$v(w)$ と $v(w')$ が $\mathbf{N}^{(X)}$ の同じ元 $\alpha$ に等しいと仮定します。 公式 (22)、$n = |\alpha| = m$ 作。 すべての $x \in X$ について、$I_x$ (それぞれ $I'_x$) を整数 $i$ の集合とし、$1 \leq i \leq n$ と $x_i = x$ (それぞれ $x'_i = x$) とします。 したがって、$(I_x)_{x \in X}$ と $(I'_x)_{x \in X}$ は、区間の分割、$\mathbf{N}$ の $[1, n]$ です。さらに、公式
$$
\alpha = \sum_{i=1}^n \delta_{x_i}
$$
$\alpha(x)$ が $I_x$ の基数であることを示します。同様に公式
$$
\alpha = \sum_{i=1}^n \delta_{x'_i}
$$
$\alpha(x)$ が $I'_x$ の基数であることを示します。 したがって、すべての $x \in X$ に対して $\sigma(I'_x) = I_x$、つまり $i = 1, \ldots, n$ に対して $x'_i = x_{\sigma(i)}$ となるような $[1, n]$ の置換 $\sigma$ が存在します。

#### 注意 {#alg-i-s7-n9-rem-1 .statement tag=05FX}

$S$ を $X$ の部分集合とします。 $M(S)$ は $M(X)$ のサブマグマ、$Mo(S)$ は $Mo(X)$ の部分モノイド、$N^{(S)}$ は $N^{(X)}$ の部分モノイドと識別されたことを思い出してください。それから
$$
M(S) = \lambda^{-1}(Mo(S)).
$$
明らかに$\lambda(M(S)) \subset Mo(S)$。 $w \in \lambda^{-1}(Mo(S))$ にしましょう。 $l(w)$の帰納法までに$w \in M(S)$であることがわかります。 $l(w) = 1$なら一目瞭然。 $l(w) > 1$の場合、$w_1, w_2 \in M(X)$、$l(w_1) < l(w)$、$l(w_2) < l(w)$で$w = w_1 w_2$と書くこともあります。次に$\lambda(w_1) \lambda(w_2) \in Mo(S)$、したがって$\lambda(w_1) \in Mo(S)$と$\lambda(w_2) \in Mo(S)$、よって$w_1 \in M(S)$と$w_2 \in M(S)$、帰納法の仮定、そして最後に$w \in M(S)$です。

また、
$$
Mo(S) = v^{-1}(N^{(S)}).
$$
これは公式 (21) の直後に続きます。

さらに、$N^{(S)}$ は、$S$ にサポートが含まれている $N^{(X)}$ の元の集合です。 $(S_i)_{i \in I}$ が共通部分 $S$ の $X$ の部分集合の族である場合、$N^{(S)} = \bigcap_{i \in I} N^{(S_i)}$ と式 (23) と (24) は次のことを意味します。
$$
M(S) = \bigcap_{i \in I} M(S_i), \quad Mo(S) = \bigcap_{i \in I} Mo(S_i).
$$

### 練習問題 {#alg-i-s7-exercises}

[§ 7 に対して練習問題](exercises/s7/)を参照してください。
