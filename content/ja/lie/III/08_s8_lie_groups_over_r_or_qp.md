---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 8
section_title: Lie groups over R or Qp
lang: ja
source: lie-i-iii
book_pages: 337-342, 395-397
pdf_pages: 0355-0360, 0413-0415
extraction: ocr
subsections:
    - "no": 1
      title: CONTINUOUS MORPHISMS
      page: 337
      pdf_page: 355
    - "no": 2
      title: CLOSED SUBGROUPS
      page: 340
      pdf_page: 358
statements: 9
exercises: 7
content_sha256: 486e13b2c64d043980f9aca5ea9806eabdf2d963bf31747990bdf38f798f15c3
translated_from: content/en/lie/III/08_s8_lie_groups_over_r_or_qp.md
translation_method: google
source_content_sha256: 9a8748db60c9fd84976b7413bf30ec32e2a4b17c04a06e968ec301e544a51660
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: ac7c185de54e587a61f9404e8cdb10ba6b4de8e3f0390c6f1568ce54a8d24b91
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 8。 リー群 $\mathbf{R}$ と $\mathbf{Q}_p$ を超えました

### 1. 連続射

#### 定理 1 {#lie-iii-s8-thm-1 .statement tag=0AI2}

*G と H を、$\mathbf{R}$ または $\mathbf{Q}_p$ を超える 2 つのリー群細菌とする。 f を G から H への連続射とします。その場合、f は解析的です。*

$L(G)$ と $L(H)$ ノルムにそれらのトポロジ定義するが与えられ、すべての $x, y$ に対して $\| [x, y] \| \leq \|x\| \|y\|$ が得られます。 $L(G)$ の中心 0 のオープンボール V と、V で定義された G の指数関数写像 $\phi$ が存在します。 (1) $\phi(V)$ は、G の $e$ のオープン近傍です。 (2) $\phi$ は、解析的多様体 V の同型を解析的多様体 $\phi(V)$ に加えたものです。 (3) $x \in V$ および $nx \in V$ などのすべての $n \in \mathbf{Z}$ に対して $\phi(nx) = \phi(x)^n$。同様に W を定義する、H を $\psi$ とします。必要に応じて V を縮小すると、$f(\phi(V)) \subset \psi(W)$ と仮定できます。すると、$g = \psi^{-1} \circ f \circ \phi$はVの写像がWに連続します。

私たちはそれを示します
$$
(x \in V, \lambda \in \mathbf{Q} \text{ and } \lambda x \in V) \Rightarrow g(\lambda x) = \lambda g(x).
$$
$\lambda \neq 0$と考えられます。 $\mathbf{Z} - \{0\}$に$r, q$を$\lambda = \frac{r}{q}$とします。 $y = \frac{r}{q} x$ にしましょう。

$K = \mathbf{R}$の場合は、$z = \frac{x}{q} = \frac{y}{r} \in V$と書きます。その後、$x = qz, y = rz$、よって
$$
g(x) = \psi^{-1}(f(\phi(qz))) = \psi^{-1}(f(\phi(z)^q)) = \psi^{-1}(f(\phi(z))^q).
$$
$\psi^{-1}(f(\phi(z))^q) = q \psi^{-1}(f(\phi(z))) = qg(z)$ を示します。 $u \in \psi(W)$ が $u^q \in \psi(W)$ となる場合、$\psi^{-1}(u^q) = q \psi^{-1}(u)$ であることを確認するだけで十分です。しかし、$u = \psi(v)$、$u^q = \psi(v^q)$ の場合、$v^1/q \in W$、$(\psi(v^1/q))^q = u^q$、したがって $\psi(v^1/q) = u = \psi(v)$、したがって $v^1 = qv$ になります。

同様に、$g(y) = rg(z)$、よって (1)。

$K = \mathbf{Q}_p$ の場合、再度 $z = rx = qy \in V$、よって $g(z) = rg(x) = qg(y)$、よってと書きます (1)。

$\mathbf{Q}$ は $K$ 内で密であるため、(1) は次のことを意味します。
$$
(x \in V, \lambda \in K \text{ and } \lambda x \in V) \Rightarrow g(\lambda x) = \lambda g(x).
$$
$x \in L(G)$ と $\lambda, \lambda'$ を $K^*$ の元とし、$\lambda x \in V, \lambda' x \in V$ とします。それから
$$
g(\lambda' x) = g\left( \frac{\lambda'}{\lambda} \lambda x \right) = \frac{\lambda'}{\lambda} g(\lambda x)
$$
(2) により、したがって $\frac{1}{\lambda} g(\lambda x) = \frac{1}{\lambda'} g(\lambda' x)$ になります。したがって、$g$ から $L(G)$ までの拡大 $h$ は、$\lambda x \in V$ となるように、すべての $\lambda$ に対して $h(x) = \frac{1}{\lambda} g(\lambda x)$ を書くことで定義されます。明らかに$h$ は連続しています。私たちはそれを示します
$$
(x \in L(G) \text{ and } \lambda \in K) \Rightarrow h(\lambda x) = \lambda h(x).
$$
$\lambda' \in K^*$ を $\lambda' x \in V$ と $\lambda' \lambda x \in V$ となるようにします。それから
$$
h(\lambda x) = \frac{1}{\lambda'} g(\lambda' \lambda x) = \frac{1}{\lambda'} \lambda g(\lambda' x) = \lambda \frac{1}{\lambda'} g(\lambda' x) = \lambda h(x).
$$
$x, y$ を $L(G)$ に入れます。その後、§ 4, no. 3 の命題 4 までに、
$$
\begin{align*}
h(x) + h(y) &= \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} \psi^{-1}(\psi(\lambda h(x)) \psi(\lambda h(y))) \\
&= \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} \psi^{-1}(\psi(h(\lambda x)) \psi(h(\lambda y))).
\end{align*}
$$
$|\lambda|$ が十分に小さい場合、$\lambda x \in V$ および $\lambda y \in V$ であるため、上記の式は次と等しくなります。
$$
\begin{align*}
&\lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} \psi^{-1}(f(\phi(\lambda x)) f(\phi(\lambda y))) \\
&= \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} (\psi^{-1} \circ f)(\phi(\lambda x) \phi(\lambda y)) \\
&= \lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} g(\phi^{-1}(\phi(\lambda x) \phi(\lambda y))) \\
&= \lim_{\lambda \in K^*, \lambda \to 0} h(\lambda^{-1} \phi^{-1}(\phi(\lambda x) \phi(\lambda y))) \\
&= h(\lim_{\lambda \in K^*, \lambda \to 0} \lambda^{-1} \phi^{-1}(\phi(\lambda x) \phi(\lambda y))) \\
&= h(x + y).
\end{align*}
$$
したがって、$h$ は連続かつ線形であり、したがって $g = h|V$ は解析的であり、したがって $f$ は $\phi(V)$ で解析的であり、したがって $f$ は解析的です (§ 1, no. 10)。

#### 系 1 {#lie-iii-s8-thm-1-cor-1 .statement tag=0AI3}

$G$ をトポロジー 群とします。 $G$ には、$G$ 上のトポロジカル群構造と互換性のある $\mathbf{R}$ (それぞれ $\mathbf{Q}_p$) 上に最大 1 つの解析多様体構造が存在します。

これは定理 1 の直後に続きます。

#### 定義 1 {#lie-iii-s8-def-1 .statement tag=0AI4}

*トポロジカル群 G は、その位相と互換性のある実数 (または p 進数) リー群構造が G 上に存在する場合、実数 (または p 進数) リー群と呼ばれます。*

したがって、その構造は一意であり、そのような群の *次元* について話すことができます。 G と H がそのような 2 つ群である場合、G から H への連続するすべての射は解析的です。

#### 系 2 {#lie-iii-s8-def-1-cor-2 .statement tag=0AI5}

*G を位相幾何学的群および V を e の開近傍とする。 V に、それを実数 (p 進数) リー群ジャームにする解析多様体構造があるとします。このとき、G は実数 (p 進数) リー群です。*

$g \in G$ にしましょう。 $V' \cup gV'g^{-1} \subset V$ となるような G には $e$ の開いた近傍 $V'$ が存在します。 $V'$ の $V$ への写像 $v \mapsto gv g^{-1}$ は連続的であり、したがってリー群細菌 $V'$ のリー群細菌 $V$ への分析的な射です。その場合、§ 1, no. 9 の命題を適用する 18 で十分です。

#### 注意 {#lie-iii-s8-n1-rem-1 .statement tag=0AI6}

(1) $\mathbf{R}$ (それぞれ $\mathbf{Q}_p$) が $\mathbf{C}$ (練習問題 1) に置き換えられると、定理 1 とその帰結は真ではなくなります。

(2) G を位相ベクトル群とする。次の条件は同等であることが示されます†: (a) G は有限次元の実リー群です。 (b) G は局所的にコンパクトであり、$\{e\}$ とは異なる部分群の $e$ 含むの近傍が存在します。 (c) 空間 $\mathbf{R}^n$ のオープンボールと同型の $e$ のオープン近傍が存在します。 (それほど難しくない結果の場合は、cf. 練習問題 6 です。)

#### 命題 1 {#lie-iii-s8-prop-1 .statement tag=0AI7}

*G, G' を位相的群とし、f を G から G' への連続射とする。次の 3 つのケースのいずれかが当てはまると仮定します。
(a) G は実リー群で、G' は p 進数リー群です。
(b) G は p 進数リー群で、G' は実リー群です。
(c) G は p 進数リー群で、G' は $p \neq p'$ を持つ $p'$-進数リー群です。
この場合、f は局所的に定数になります。*

ケース(a)。 $G_0$ を G の同一性成分とします。すると、$f(G_0)$ は $G'$ の接続された部分群であるため、$f(G_0) = \{e\}$ と $G_0$ は G で開いています。

ケース(b)。 $V'$ を $G'$ の $e$ の近傍とし、$G'$ のすべての部分群が $V'$ 簡約する ～ $\{e\}$ (§ 4, no. 2、系 1 ～ 定理) に含まれるようにします。 2)。 $f(V) \subset V'$ となるような G には $e$ の近傍 V が存在します。次に、$G_1 \subset V$ (§ 7, no. 1, 命題 1) となる G の開いた部分群 $G_1$ が存在します。それから$f(G_1) = \{e\}$。

ケース(c)。 § 7、定理 4、および系から命題 8 までには、$G'$ に $e$ の近傍 $V'$ が存在し、すべての $x' \in V' - \{e\}$、${x'}^{p^n}$ には傾向がありません。

† たとえば、D. Montgomery と L を参照してください。 Zippin、*位相変換群*、純粋および応用数学におけるインターサイエンス トラクト、no. 1、インターサイエンス出版社、ニューヨーク、1955 年 (特に、169 および 184 ページ)。

$n$ が $+\infty$ になる傾向があるため、$e$ になります。 $G$ には $f(V) \subset V'$ となる $e$ の近傍 $V$ が存在します。 § 7、定理 4、および命題 9 までに、$G_1 \subset V$ となるような$G$ のオープン部分群 $G_1$ が存在し、すべての$x \in G_1$ について、$x^{p^n}$ は次のように $e$ になる傾向があります。 $n$は$+\infty$になる傾向があります。それから$f(G_1) = \{e\}$。

### 2. 閉店部分群

#### 定理 2 {#lie-iii-s8-thm-2 .statement tag=0AI8}

*$G$ を $\mathbf{R}$ または $\mathbf{Q}_p$ 上の有限次元リー群とします。 $G$ のすべての閉じた部分群は、$G$ の嘘部分群です。 より一般的には、$U$ を、$G$ の $e$ の対称オープン近傍と、$H$ $U$ の空でないクローズ部分空間とし、条件 $x \in H$、$y \in H$、$xy^{-1} \in U$ が意味するようにします。 $xy^{-1} \in H$。 したがって、$H$ は $G$ の嘘部分群の細菌です。

$\mathfrak{h}$ を、$e$ (§ 4, no. 5, 定義 2) で $H$ に接する嘘部分代数とします。 リー代数 $\mathfrak{h}$ と$H$ に含まれる$G$ の嘘部分群細菌$H_0$ が存在します。 $G$のそれによって誘発された位相により、$H$に$H_0$が開いていることを証明します。これにより、$H$ が $G$ の解析部分多様体であることが証明され、定理が確立されます。

$L(G)$には$\mathfrak{h}$を補足するベクトル部分空間$\mathfrak{k}$、$\mathfrak{h}$と$\mathfrak{k}$にはそれぞれ零の対称オープン近傍$V_1, V_2$、そして写像$\phi$の指数関数が存在します。 $G$ は $V_1 + V_2$ で定義され、次のプロパティを持っています。

(a) 写像 $(a_1, a_2) \mapsto \phi(a_1)\phi(a_2)$ は、$G$ のオープン部分集合 $V$ に対する $V_1 \times V_2$ の解析同型です。
(b) $\phi(V_1) \subset H_0$;
(c) $V^2 \subset U$。

$H \cap (\phi(V_1)\phi(V'_2)) = \phi(V_1)$ となるような、$V_2$ に 0 の開いた近傍 $V'_2$ が存在することを証明します (これにより証明が達成されます)。

主張が false であると仮定します。次に、$V_1$ の数列 $(x_n)$ と $V_2 - \{0\}$ の数列 $(y_n)$ が 0 になる傾向があり、すべての $n$ で $\phi(x_n)\phi(y_n) \in H$ が得られます。次に(c)で$\phi(y_n) \in H$。

$K = \mathbf{Q}_p$ の場合、$V_2$ は $\mathfrak{k}$ の加法部分群であり、すべての $a \in V_2$ とすべての $p \in \mathbf{Z}$ に対して $\phi(pa) = \phi(a)^p$ であると想定できます。 次に、すべての $\lambda \in \mathbf{Z}$ に対して $\phi(\lambda y_1) \in H$ となり、すべての $\lambda \in \mathbf{Z}_p$ に対して連続性が生じます。 The mapping $f : \lambda \mapsto \phi(\lambda y_1)$ of $\mathbf{Z}_p$ into $G$ is analytic and takes its values in $H$ and $(T_0f)(1) = y_1$. したがって$y_1 \in \mathfrak{h}$となり、これは不合理です。 したがって、$\mathbf{Q}_p$の場合には定理が成立します。

$K = \mathbf{R}$ の場合、$V_2$ が接続され、$y_n$ 属するから $\frac{1}{2}V_2 - \{0\}$ が接続されていると想定できます。 必要に応じて $(y_n)$ の部分列を取得することで、$\lambda_n^{-1}y_n$ が $V_2 - \{0\}$ の元 $y$ になる傾向があるようなゼロ以外のスカラーの数列 $(\lambda_n)$ を見つけることができます。 数列 $(\lambda_n)$ は 0 になる傾向があります。 $\lambda \in \mathbf{R}$ を $\lambda y \in \frac{1}{2}V_2$ となるようにします。 $\exp(\lambda y) \in H$ であることを証明します。 すべての $n$ に対して $\lambda \lambda_n^{-1}y_n \in \frac{1}{2}V_2$ であると想定できます。 $k_n \in \mathbf{Z}$ を、$|\lambda - k_n \lambda_n|$ が 0 になる傾向があるとします。 $n$ 十分大きい、$(\lambda - k_n \lambda_n)\lambda_n^{-1}y_n \in \frac{1}{2}V_2$、したがって $k_n y_n \in \frac{1}{2}V_2$ の場合。 したがって、$h$ 整数および $0 \leq |h| \leq |k_n|$ は $\exp(h y_n) \in H$ になります ($|h|$ の帰納法に見られるように)。 それから
$$
\exp(\lambda y) = \lim_{n \to \infty} \exp(\lambda \lambda_n^{-1}y_n) = \lim_{n \to \infty} (\exp((\lambda - k_n \lambda_n)\lambda_n^{-1}y_n) \exp(k_n y_n))
= \lim_{n \to \infty} \exp k_n y_n \in H.
$$

したがって、写像 $f : \lambda \mapsto \exp \lambda y$、$\lambda y \in \frac{1}{4}V_2$ は、$H$ と $(T_0f)(1) = y$ でその値をとります。したがって$y \in \mathfrak{h}$となり、これは不合理です。したがって、$\mathbf{R}$の場合には定理が成立します。

$G$ が有限次元 (練習問題 12) であると想定されていない場合、定理 2 は真ではなくなります。

#### 系 1 {#lie-iii-s8-thm-2-cor-1 .statement tag=0AI9}

*$G'$を局所的にコンパクトな群、$G$を$\mathbf{R}$(それぞれ$\mathbf{Q}_p$)上の有限次元リー群、$f$を$G'$から$G$への連続射とする。 $f$ の核が離散である場合、$G'$ は有限次元の実数 (それぞれ $p$ 進数) リー群です。*

$G'$ には $e$ のコンパクト近傍 $V$ が存在し、$f|V$ は $G$ のコンパクト部分空間に対する $V$ の同写写像となります。 $U$ が $G$ の $e$ の十分に小さいオープン近傍である場合、定理 2 の仮説は $H = f(V) \cap U$ で満たされます。 したがって、$H$ は $G$ の嘘部分群の細菌です。 $W$ を $f|V$ の下の $H$ の逆像とします。 すると、$W$は$G'$の$e$の近傍になります。 $W$ に、$H$ から $(f|W)^{-1}$ によって転送された解析多様体構造を与えます。 For all $z \in G'$, the mapping $x \mapsto f(z)x f(z)^{-1}$ of $G$ into $G$ is analytic; hence there exists an open neighbourhood $W'$ of $e$ in $W$ such that the mapping $x' \mapsto zx'z^{-1}$ of $W'$ into $W$ is analytic. By Proposition 18 of § 1, no. 9, there exists on $G'$ a Lie group structure which induces on a sufficiently small open neighbourhood of $e$ the same analytic structure as $W$ and hence the same topology as the initial topology on $G'$.

#### 系 2 {#lie-iii-s8-thm-2-cor-2 .statement tag=0AIA}

*Let $G$ be a finite-dimensional Lie group over $K$, $H$ a subgroup of $G$, $V$ an open neighbourhood of $e$ in $G$ and $(M_i)_{i \in I}$ a family of analytic manifolds over $K$; for all $i \in I$, let $f_i$ be a $K$-analytic mapping of $V$ into $M_i$ such that*

$$
H \cap V = \{ x \in V \mid f_i(x) = f_i(e) \text{ for all } i \in I \}.
$$

(i) *$K = \mathbf{C}$ の場合、$H$ は $G$ の嘘部分群です。*
(ii) *$K$ が $\mathbf{Q}_p$ の有限拡大で、$I$ が有限である場合、$H$ は $G$ の嘘部分群です。

(i) $K = \mathbf{C}$ と仮定します。 $G$を実リー群とみなします。すると、$H$ は、$G$ (定理 2) の本当の嘘部分群になります。 $a \in L(H)$ にしましょう。 $\mathbf{C}$ の $0$ の接続されたオープン近傍 $W$ が存在し、すべての $\lambda \in W$ に対して $\exp \lambda a \in V$ になります。 $i \in I$ にしましょう。 $\lambda \in \mathbf{R} \cap W$なら$f_i(\exp \lambda a) = f_i(e)$。したがって、解析継続により $\lambda \in W$ であれば $f_i(\exp \lambda a) = f_i(e)$ となります。したがって、$\lambda \in W$ に対しては $\exp \lambda a \in H$、したがってすべての $\mu \in \mathbf{C}$ に対しては $\mu a \in L(H)$ となります。したがって、$H$ は複素数リー群 $G$ (§ 4, no. 2, 命題 2) の嘘部分群です。

(ii) $K$ が $\mathbf{Q}_p$ の有限拡大であると仮定します。 $G$は$\mathbf{Q}_p$よりもリー群と考えます。これは有限次元であり、定理 2 は、$H$ が $G$ の $p$ 進嘘部分群であることを意味します。 $I$ は有限であるため、$\prod_{i \in I} M_i$ は多様体であり、家族 $(f_i)$ 簡約するから単一の写像 $f$ であると仮定できます。 $a \in L(G)$ にしましょう。 $\phi$ を $G$ の指数写像とします。次に、$\lambda \in \mathbf{Q}_p$ と $|\lambda|$ の場合、$f(\phi(\lambda a)) = f(e)$ は十分に小さいです。 $f$ は K 解析であるため、$\lambda \in K$ と $|\lambda|$ に対して $f(\phi(\lambda a)) = f(e)$ は十分に小さいということになります。したがって、$\lambda \in K$ および $|\lambda|$ に対して $\phi(\lambda a) \in H$ は十分に小さいため、すべての $\mu \in K$ に対して $\mu a \in L(H)$ となります。 (i)と同様に証明が完成します。

仮定を省略すると、I は有限であるという系 2 (ii) は真ではなくなります。

### 練習問題 {#lie-iii-s8-exercises}

[§ 8 に対して練習問題](exercises/s8/)を参照してください。
