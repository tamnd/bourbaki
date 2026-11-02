---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 6
section_title: Symmetric algebras
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 497-506, 632-633
pdf_pages: 0521-0530, 0656-0657
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF THE SYMMETRIC ALGEBRA OF A MODULE
      page: 497
      pdf_page: 521
    - "no": 2
      title: FUNCTORIAL PROPERTIES OF THE SYMMETRIC ALGEBRA
      page: 498
      pdf_page: 522
    - "no": 3
      title: n-th symmetric power of a module and symmetric multilinear mappings
      page: 500
      pdf_page: 524
    - "no": 4
      title: EXTENSION OF THE RING OF SCALARS
      page: 502
      pdf_page: 526
    - "no": 5
      title: DIRECT LIMIT OF SYMMETRIC ALGEBRAS
      page: 503
      pdf_page: 527
    - "no": 6
      title: SYMMETRIC ALGEBRA OF A DIRECT SUM. SYMMETRIC ALGEBRA OF A FREE MODULE. SYMMETRIC ALGEBRA OF A GRADED MODULE
      page: 503
      pdf_page: 527
statements: 17
exercises: 5
content_sha256: f532a26108dbcd76cb7dd611b52bdf8dd903ad73171f5776ada9b42e24e34d9f
translated_from: content/en/alg/III/06_s6_symmetric_algebras.md
translation_method: google
source_content_sha256: a716a1c3cf99e3d34241000d92ee39248d92a3c9503fa59066fb7f864e19044c
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 7decda09352000a203c5a57e6996335f2a67ece03d2f92dd17670d38f7934258
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 6。対称代数

### 1. 加群の対称的な代数の定義

#### 定義 1 {#alg-iii-s6-def-1 .statement tag=0626}

※Aを可換環、MをA-加群とします。 S(M)、Sym(M)、または S_A(M) で示される M の対称代数は、次によって生成される両側理想 $\mathfrak{J}'$ ($\mathfrak{J}'_M$ とも示される) により、テンソル代数 T(M) の A 上の商代数です。 T(M) の元 $xy - yx = x \otimes y - y \otimes x$、x と y は M を通過します。*

イデアル $\mathfrak{J}'$ は次数 2 の同次元によって生成されるため、段階的イデアル (II, § 11, no. 3、命題 2) です。 $\mathfrak{J}'_n = \mathfrak{J}' \cap T^n(M)$と書きます。 代数 S(M) は、$S^n(M) = T^n(M)/\mathfrak{J}'_n$ の卒業 (正規と呼ばれます) からなるによって等級付けされます。現在、$\mathfrak{J}'_0 = \mathfrak{J}'_1 = \{0\}$、したがって $S^0(M)$ は A と、$S^1(M)$ は $T^1(M) = M$ と正規に識別されます。これらの識別は常に以下で行い、$\phi'$ または $\phi'_M$ 標準単射 $M \to S(M)$ で表します。

#### 命題 1 {#alg-iii-s6-prop-1 .statement tag=0627}

*代数 S(M) は可換です。*

M の $x, y$ に対して定義 $\phi'(x)\phi'(y) = \phi'(y)\phi'(x)$ により、そして元 $\phi'(x)$ として、x は M、生成する S(M) を通過し、結論は § 1, no. 7 から得られます。

#### 命題 2 {#alg-iii-s6-prop-2 .statement tag=0628}

*E を A-代数および $f : M \to E$ A-線型写像とすると、*
$$(1)$$
$$ f(x)f(y) = f(y)f(x) \text{ for all } x, y \text{ in } M. $$
*$f = g \circ \phi'$ となる A-代数準同型 $g : S(M) \to E$ は 1 つだけ存在します。*

他の語では、$(S(M), \phi')$ は * 普遍写像問題* (*集合理論*, IV, § 3, no. 1) の解であり、$\Sigma$ は A-代数の種です。 構造、$\alpha$-マッピングは、A-加群 M から A-代数満たすの線形写像です (1)。

g の一意性は、$\phi'(M) = M$ 生成する S(M) という事実から導き出されます。 g の存在を証明するには、§ 5, No. 1, 命題 1 により、$f = g_1 \circ \phi;$ となるような A-代数準同型 $g_1 : T(M) \to E$ が存在することに注意してください。

証明する必要があるのは、$g_1$ が理想的な $\mathfrak{J}'$ 上で零であるということだけです。その場合、$p : T(M) \to S(M) = T(M)/\mathfrak{J}'$ が標準準同型である場合、$g : S(M) \to E$ が代数準同型である $g_1 = g \circ p$ と書くことができ、結論は次の事実から得られます。 $p \circ \phi = \phi'$。さて、$g_1$の核は、(1)と関係$g_1 \circ \phi = f$のおかげで、$M$の$x, y$に対して含む元$x \otimes y - y \otimes x$となる両面理想です。これで証明は完了です。

#### 注意 {#alg-iii-s6-n1-rem-1 .statement tag=0629}

(1) $E$ が型 $\mathbf{Z}$ の段階化された $A$-代数であり、目盛が $(E_n)$ であると仮定します。また、線形写像 $f$ (満たす (1) と仮定) は次のようであると仮定します。
(2)
$$
f(M) \subset E_1.
$$
次に、関係 $g(x_1 x_2 \ldots x_p) = f(x_1) f(x_2) \ldots f(x_p)$ と $x_i \in M$ は、すべての $p \geq 0$ に対して $g(S^p(M)) \subset E_p$ であることを示し、したがって $g$ は等級付けされた代数準同型です。

(2) $S(M)$ のすべての元は、形 $x_1 x_2 \ldots x_n$ の積の和であり、$x_i$ 属するから $M$ です。 $S(M)$ で取得されたそのような積と、$T(M)$ で取得された類似の積を混同しないように注意する必要があります。

(3) $n!.1$ が $A$ で反転可能な場合、$A$ モジュール $S^n(M)$ は形 $x^n$ の元によって生成されます。ここで、$x \in M$;これは、上記の注意と I, § 8, no. 2、命題 2 から続きます。

### 2. 対称代数の関数的性質

#### 命題 3 {#alg-iii-s6-prop-3 .statement tag=062A}

*$A$ を可換環、$M$、$N$ の 2 つの $A$ モジュールと $u : M \to N$ の $A$ 線形マッピングとします。 図式* となるような $A$-代数準同型性 $u' : S(M) \to S(N)$ が 1 つだけ存在します。

$$
\begin{array}{ccc}
M & \xrightarrow{u} & N \\
\downarrow \phi'_M & & \downarrow \phi'_N \\
S(M) & \xrightarrow{u'} & S(N)
\end{array}
$$

*は可換です。さらに、$u'$ はグレード代数準同型です。*

$u'$ の存在と一意性は、可換代数 $S(N)$ と $f = \phi'_N \circ u : M \to S(N)$ に適用される no. 1、命題 2 から続きます。として
$$
f(M) \subset S^1(N) = N,
$$
$u'$ が等級付けされた代数準同型であるという事実は、no. 1, *注意* 1 から導き出されます。

命題 3 の準同型 $u'$ は、以降、$S(u)$ で示されます。 $P$ が $A$ モジュール、$v : N \to P$ が $A$ 線形マッピングの場合、
$$
S(v \circ u) = S(v) \circ S(u)
$$

for $S(v) \circ S(u)$ は代数準同型で図式を可換にレンダリングします

$$
\begin{array}{ccc}
M & \xrightarrow{v \circ u} & P \\
\downarrow \phi'_M & & \downarrow \phi'_P \\
S(M) & \xrightarrow{S(v) \circ S(u)} & S(P)
\end{array}
$$

$S(M)$ 含む $M = S^1(M)$ として、$S(u)$ はときどきであり、$u$ から $S(M)$ の *標準拡大* と呼ばれます。 制限 $S^n(u): S^n(M) \to S^n(N)$ は次のとおりです
$$
S^n(u)(x_1 x_2 \ldots x_n) = u(x_1) u(x_2) \ldots u(x_n)
$$
ここで、$S(u)$ は代数準同型と $S^1(u) = u$ なので、$x_i \in M$ です。 制限 $S^0(u)$ から $A$ は恒等写像です。 $S^n(u)$は、$T^n(u): T^n(M) \to T^n(N)$から移行から商までに取得できることに注意してください。

#### 命題 4 {#alg-iii-s6-prop-4 .statement tag=062B}

*$u: M \to N$ が全射的 $A$ 線形写像である場合、準同型 $S(u): S(M) \to S(N)$ は全射的であり、その核は $u$ の核 $P \subset M \subset S(M)$ によって生成される $S(M)$ のイデアルです。

$v = T(u): T(M) \to T(N)$と書きます。私たちは (§ 5, no. 2, 命題 3) $v$ が全射であることを知っており、したがって定義から $v(\mathfrak{J}'_M) = \mathfrak{J}'_N$ が導かれます。 $\mathfrak{R}$ が $v$ の核であれば、$v^{-1}(\mathfrak{J}'_N) = \mathfrak{R} + \mathfrak{J}'_M$ です。 $S(u): T(M)/\mathfrak{J}'_M \to T(N)/\mathfrak{J}'_N$は$v$から移行から商まで導かれるので、核が$\mathfrak{R}' = (\mathfrak{R} + \mathfrak{J}'_M)/\mathfrak{J}'_M$である全射準同型になります。 $\mathfrak{R}$ は $u$ (§ 5, no. 2) の核 $P$ によって生成されるため、$\mathfrak{R}'$ も生成されます。

$u: M \to N$ が*単射詞* 線形写像である場合、$S(u)$ が単射詞写像 (練習問題 1) であるとは限りません。ただし、$u$ が単射で、$u(M)$ が $N$ の *直因子* であり、$S(u)$ の像 ($S(M)$ と同型) が $S(N)$ の *直因子* である場合は当てはまります。 証明は、$S$ による $T(u)$ (§ 5, no. 2) 置き換えること $T$ に対する類似の主張と同じです。

#### 命題 5 {#alg-iii-s6-prop-5 .statement tag=062C}

*$N$ と $P$ を $A$ モジュール $M$ の 2 つの部分加群とし、それらの和 $N + P$ が $M$ の直因子であり、共通部分 $N \cap P$ が$N$と$P$の直因子。次に、準同型 $S(N) \to S(M)$、$S(P) \to S(M)$、および*
$$
S(N \cap P) \to S(M),
$$
*標準的な拡大の標準単射は単射です。 $S(N)$、$S(P)$、$S(N \cap P)$ が、準同型によって $S(M)$ の部分代数と識別される場合、*
$$
S(N \cap P) = S(N) \cap S(P).
$$
(4)

証明簡約するから § 5, no. 2、命題 4 置き換えること $T$ が $S$ まで続きます。 命題 5 の仮説は、$A$ が体であるとき、$M$ の *任意の* 部分加群 $N, P$ に対して常に当てはまります。

#### 系 {#alg-iii-s6-n2-cor-1 .statement tag=062D}

*K を K 上の可換体および M ベクトル空間とします。すべての元 $z \in S(M)$ に対して、$z \in S(N)$ および N が有限次元となるような M のうち最小のベクトル空間 N が存在します。

証明は、§ 5, no. 2、系から命題 4 置き換えること T の全体を通して S から派生します。

N は、z に *関連付けられた* M のベクトル部分空間と呼ばれます。

### 3. 加群の n 番目の対称冪および対称多重線形マッピング

X, Y を 2 つの集合と $n$ 整数 $\geqslant 1$ とします。 A *symmetric mapping* of $X^n$ into Y is any mapping $f : X^n \to Y$ such that, for every permutation $\sigma \in \mathscr{S}_n$ and every element $(x_i) \in X^n$,

$$
f(x_{\sigma(1)}, x_{\sigma(2)}, \ldots, x_{\sigma(n)}) = f(x_1, x_2, \ldots, x_n).
$$

連続する 2 つの整数生成する群 $\mathscr{S}_n$ (I, § 5, no. 7) を交換する転置として、$\sigma$ がそのような転置である場合、条件 (5) が成り立つだけで十分です。

Y が可換環 A 上の *加群* である場合、明らかに、Y への $X^n$ の対称写像の集合は、Y への $X^n$ のすべての写像の A-加群 $Y^{X^n}$ の *部分加群* です。

#### 命題 6 {#alg-iii-s6-prop-6 .statement tag=062E}

※Aを可換環、MとNを2 A-加群とします。すべての A-線型写像 $g : S^n(M) \to N$ ($n \geqslant 1$) が n 線形マッピング* に関連付けられている場合、

$$
(x_1, x_2, \ldots, x_n) \mapsto g(x_1 x_2 \ldots x_n)
$$

*(右側の積は代数 $S(M)$ に取り込まれます)、$M^n$ を N に変換した対称 n 線形写像の A-加群に対する A-加群 $\operatorname{Hom}_A(S^n(M), N)$ の全単射A-線型写像が得られます。

II, § 3, no. 9 を思い出してください。$M^n$ から N への *すべての * n 線形写像の A-加群 $\operatorname{Hom}_A(T^n(M), N)$ から A-加群 $\mathscr{L}_n(M, \ldots, M; N)$ への正規の全単射が、すべての A-線型写像 $f : T^n(M) \to N$ の n 線形写像と関連付けることによって得られます。

$$
\tilde{f} : (x_1, x_2, \ldots, x_n) \mapsto f(x_1 \otimes x_2 \otimes \cdots \otimes x_n).
$$

一方、A-線型写像 $g : S^n(M) \to N$ は、$g$ 写像 $f = g \circ p_n$ と関連付けることにより、$f$ が零 *on* $\mathfrak{J}'_n$ となるように、A-線型写像 $f : T^n(M) \to N$ と 1 対 1 の対応になります。

$$
p_n : T^n(M) \to S^n(M) = T^n(M)/\mathfrak{J}'_n
$$

は標準準同型 (II, § 2, no. 1、定理 1) です。しかし、$\mathfrak{J}'_n$ は形の元の線形結合であるため、

$$
(u_1 \otimes u_2 \otimes \cdots \otimes u_p) \otimes (x \otimes y - y \otimes x) \otimes (v_1 \otimes \cdots \otimes v_{n-p-2})
$$

n 番目の対称冪

(x, y, u_i, v_j in M)、写像 f が形 g \circ p_n であると言うことは、対応する n 線形写像 $\bar{f}$ が関係を満たすことを意味します。

$$
\bar{f}(u_1, \ldots, u_p, x, y, v_1, \ldots, v_{n-p-2}) = \bar{f}(u_1, \ldots, u_p, y, x, v_1, \ldots, v_{n-p-2});
$$

他の語では、上で見てきたことから、これは $\bar{f}$ が *対称* であることを意味します。 よって命題という事実を考慮して、

$$
p_n(x_1 \otimes x_2 \otimes \cdots \otimes x_n) = x_1 x_2 \ldots x_n
$$

$x_i \in M$ を使用します。

A-加群 $S^n(M)$ は M の *n 番目の対称冪* と呼ばれます。すべての A-加群準同型 $u : M \to N$、写像 $S^n(u) : S^n(M) \to S^n(N)$ について、$S^n(M)$ 上の $S(u)$ との一致するは *n 番目の対称と呼ばれます冪 of u*.

#### 注意 {#alg-iii-s6-n3-rem-1 .statement tag=062F}

$\sigma$ を $\mathfrak{S}_n$ の置換とします。 写像として

$$
(x_1, x_2, \ldots, x_n) \mapsto x_{\sigma^{-1}(1)} \otimes x_{\sigma^{-1}(2)} \otimes \cdots \otimes x_{\sigma^{-1}(n)}
$$

$M^n$ から $T^n(M)$ への変換は A-多重線形であり、次のように一意に書くことができます。

$$
(x_1, \ldots, x_n) \mapsto u_\sigma(x_1 \otimes x_2 \otimes \cdots \otimes x_n),
$$

ここで、$u_\sigma$ は A-加群 $T^n(M)$ の *自己準同型* であり、$z \mapsto \sigma . z$ とも表されます。明らかに、$\sigma$ が $\mathfrak{S}_n$ の単位元である場合、$u_\sigma$ が同一性です。一方、$y_i = x_{\sigma^{-1}(i)}$ と書くと、置換 $\tau \in \mathfrak{S}_n, y_{\tau^{-1}(i)} = x_{\sigma^{-1}(\tau^{-1}(i))}$ ごとに $\tau . (\sigma . z) = (\tau \sigma) . z$ が得られます。他の語、A-加群 $T^n(M)$は演算$(\sigma, z) \mapsto \sigma . z$(I, § 5, no. 1)の下の左$\mathfrak{S}_n$-*集合*です。 *すべて* $\sigma \in \mathfrak{S}_n$ の $\sigma . z = z$ が (反変) *対称テンソル of 位数 n* と呼ばれるような、$T^n(M)$ の元。それらは $T^n(M)$ のサブ A モジュール $S'_n(M)$ 形です。

すべての $z \in T^n(M)$ について、$s . z = \sum_{\sigma \in \mathfrak{S}_n} \sigma . z$ と書き、$s . z$ をテンソル $z$ の *対称化* と呼びます。明らかに、$s . z$ は対称なテンソルであるため、$z \mapsto s . z$ は $T^n(M)$ の自己準同型であり、像 $S''_n(M)$ は $S'_n(M)$ に含まれます。一般的には、$S''_n(M) \neq S'_n(M)$ (練習問題 5) です。 $z$ が対称テンソルの場合、$s . z = n! z$。 *n の場合は、次のようになります!は A* で可逆であり、自己準同型 $z \mapsto (n!)^{-1} s . z$ は $T^n(M)$ (II, § 1, no. 8) の *射影子* であり、その像は $S'_n(M) = S''_n(M)$ です。さらに、この射影子の*核*はちょうど$\mathfrak{J}'_n$です。なぜなら、明らかに、すべての $\sigma \in \mathfrak{S}_n$ と $\mathfrak{J}'_n$ に対する $\sigma(\mathfrak{J}'_n) \subset \mathfrak{J}'_n$ は、テンソル $z - \rho . z$ によって生成された定義によって生成されます。ここで、$\rho$ は、$\{1, n\}$ の 2 つの連続する数を交換する転置です。また、$\sigma, \tau$ が $\mathfrak{S}_n$ の 2 つの置換である場合、$z - (\sigma \tau) . z = z - \sigma . z + \sigma . (z - \tau . z)$、よってになります ($\mathfrak{S}_n$ のすべての置換は 2 つの連続する数を交換する転置の積であるため) $z - \sigma . z \in \mathfrak{J}'_n$ はすべて$z \in T^n(M)$と$\sigma \in \mathfrak{S}_n$。したがって、(常に n! が A で可逆であると仮定すると)、次のことがわかります。

$$
z - (n!)^{-1} s . z = \sum_{\sigma \in \mathfrak{S}_n} (n!)^{-1} (z - \sigma . z) \in \mathfrak{J}'_n
$$

すべての $z \in T^n(M)$ が私たちの主張を証明します。

When $n!$ is invertible in $A$, the submodules $S'_n(M)$ and $\mathfrak{g}'_n$ of $T^n(M)$ are therefore supplementary and the restriction to $S'_n(M)$ of the canonical homomorphism $T^n(M) \to S^n(M) = T^n(M)/\mathfrak{g}'_n$ is an $A$-module isomorphism, which allows us in the case envisaged to identify symmetric tensors of order $n$ with the elements of the $n$-th symmetric power of $M$. Note however that this identification is not compatible with multiplication, the product (in $T(M)$) of two symmetric tensors not being symmetric in general and not therefore having as image in $S(M)$ the product of the images of the symmetric tensors considered.

### 4. スカラーの環の拡大

$A, A'$ を 2 つの可換環、$\rho : A \to A'$ 環準同型、$M$ $A$ 加群、$M'$ $A'$ 加群、$f : M \to M'$ を $A$ 準同型射とします ( $\rho$) の $M$ を $M'$ にします。合成写像 $M \xrightarrow{f} M' \xrightarrow{\phi_{M'}} S_{A'}(M')$ は、$M$ から可換代数 $\rho_*(S_A(M'))$ への $A$ 線形マッピングです。その場合、no. 1、命題が存在します。 2) 代数 $f' : S_A(M) \to S_{A'}(M')$ を可換にレンダリングする唯一の $A$-準同型性図式

$$
\begin{array}{ccc}
M & \xrightarrow{f} & M' \\
\downarrow \phi_M' & & \downarrow \phi_{M'}' \\
S_A(M) & \xrightarrow{f'} & S_{A'}(M')
\end{array}
$$

$\sigma : A' \to A''$ が他の環準同型である場合、$M''$ は $A''$ 加群、$g : M' \to M''$ は $A'$ 準同型性 ($\sigma$ に対して)、$g' : S_{A'}(M') \to S_{A''}(M'')$ であることがすぐにわかります。 対応する $A'$-代数の準同型、その後、代数の合成 $A$-準同型

$$
S_A(M) \xrightarrow{f'} S_{A'}(M') \xrightarrow{g'} S_{A''}(M'')
$$

対応するを合成 $A$-準同型性 $g \circ f : M \to M''$ ($\sigma \circ \rho$ に対して)。

#### 命題 7 {#alg-iii-s6-prop-7 .statement tag=062G}

$A, B$ を 2 つの可換環、$\rho : A \to B$ 環準同型、および $M$ を $A$ モジュールとします。正規版拡大

$$
\psi : S_B(B \otimes_A M) \to B \otimes_A S_A(M)
$$

$B$-線形写像 $l_B \otimes \phi_M' : B \otimes_A M \to B \otimes_A S_A(M)$ は段階化された $B$-代数同型写像です。

証明は、§ 5, no. 3、命題 5 置き換えること $T$ から $S$ 、$\phi_M$ から $\phi_M'$ から導出されます。

### 5. 対称代数の直接極限

$(A_\alpha, \phi_{\beta\alpha})$ を、$A_\alpha$ モジュール、$A = \lim \rightarrow A_\alpha$、$M = \lim \rightarrow M_\alpha$ の可換環、$(M_\alpha, f_{\beta\alpha})$ 直接系の有向直接系とします。 $\alpha \leq \beta$ については、$A_\alpha$-準同型 $f_{\beta\alpha}: M_\alpha \to M_\beta$ と $A_\alpha$-代数準同型 (no. 4, 公式 (8)) $f'_{\beta\alpha}: S_{A_\alpha}(M_\alpha) \to S_{A_\beta}(M_\beta)$ から正規に導出され、(9) (no. 4) から次のようになります。 $(S_{A_\alpha}(M_\alpha), f'_{\beta\alpha})$ は、$A_\alpha$-代数*の *直接系です。一方、$f_\alpha: M_\alpha \to M$ は標準的な $A$ 準同型写像です。 (no. 4, 公式 (8)) $A_\alpha$-代数準同型性を導き出します

$$
f'_\alpha: S_{A_\alpha}(M) \to S_A(M)
$$

また、(9) から、$f'_\alpha$ は $A_\alpha$ 準同型の直接系を構成することがわかります。

#### 命題 8 {#alg-iii-s6-prop-8 .statement tag=062H}

*$A$-準同型* $f' = \lim \rightarrow f'_\alpha : \lim \rightarrow S_{A_\alpha}(M_\alpha) \to S_A(M)$ *等級付けされた代数同型.*

証明は、$S$ による $T$ および $\phi'$ による $\phi$ を通じて、可換代数の直接の極限が可換であるという事実を考慮すると、§ 5, no. 5、命題 6 置き換えることと同じです。

### 6. 直和の対称的な代数。 自由加群の対称的な代数。対称的な代数と段階的な加群

$A$ を $A$ モジュールのファミリーの可換環、$M = \bigoplus_{\lambda \in L} M_\lambda$ 直和、および $j_\lambda: M_\lambda \to M$ 標準単射とします。 代数 $S(j_\lambda): S(M_\lambda) \to S(M)$ の $A$ 準同型性を導き出します。 $S(M)$ は可換なので、§ 4, no. 5 の命題 8 は準同型 $S(j_\lambda)$ に適用でき、したがって一意な代数準同型が存在します。

$$
g: \bigotimes_{\lambda \in L} S(M_\lambda) \to S(M)
$$
($g_M$ によっても示されます) すべての $\lambda \in L$ に対して $S(j_\lambda) = g \circ f_\lambda$ となるように、ここで

$$
f_\lambda: S(M_\lambda) \to \bigotimes_{\lambda \in L} S(M_\lambda)
$$

は標準準同型を表します。

#### 命題 9 {#alg-iii-s6-prop-9 .statement tag=062I}

*標準準同型* $g$ *(公式 (10))* * は、グレード代数同型* (cf. § 4, no. 8、*注意 1*) です。

$g$ が全単射であることを証明するには、定義する代数準同型

$$
h: S(M) \to \bigotimes_{\lambda \in L} S(M_\lambda)
$$

$g \circ h$ と $h \circ g$ は、それぞれ $S(M)$ と $\bigotimes_{\lambda \in L} S(M_\lambda)$ の恒等写像になります。それぞれの $\lambda \in L$ について、$u_\lambda$ を合成線形写像とします。
$$
M_\lambda \xrightarrow{\phi'_M} S(M_\lambda) \xrightarrow{f_\lambda} \bigotimes_{\lambda \in L} S(M_\lambda).
$$
すべての $\lambda \in L$ に対して $u \circ j_\lambda = u_\lambda$ となるような $A$ 線形写像 $u : M \to \bigotimes_{\lambda \in L} S(M_\lambda)$ が 1 つだけ存在します。 $S(M_\lambda)$ が可換であるため、そのテンソル積 (§ 4, no. 5) も可換であるため、 (no. 1, 命題 2) $h \circ \phi'_M = u$ のような一意な代数準同型 $h : S(M) \to \bigotimes_{\lambda \in L} S(M_\lambda)$ が存在します。一方、$u(M)$ は、等級付けされた代数 $\bigotimes_{\lambda \in L} S(M_\lambda)$ の次数 1 の元の部分加群に含まれるのは明らかであるため、$h$ は等級付けされた代数準同型です。 $x_\lambda \in M_\lambda$の場合、
$$
h(g(u_\lambda(x_\lambda))) = h(g(f_\lambda(\phi'_M(x_\lambda)))) = h(S(j_\lambda)(\phi'_M(x_\lambda))) = h(\phi'_M(j_\lambda(x_\lambda))) = u_\lambda(x_\lambda);
$$
$u_\lambda(x_\lambda)$ 生成する代数 $\bigotimes_{\lambda \in L} S(M_\lambda)$ (§ 4, no. 5、命題 8) のように、$h \circ g$ は確かに恒等写像です。同様に、
$$
g(h(\phi'_M(j_\lambda(x_\lambda)))) = g(u_\lambda(x_\lambda)) = g(f_\lambda(\phi'_M(x_\lambda))) = S(j_\lambda)(\phi'_M(x_\lambda)) = \phi'_M(j_\lambda(x_\lambda))
$$
そして、元 $\phi'_M(j_\lambda(x_\lambda))$ 生成する代数 $S(M)$ のように、$g \circ h$ は確かに恒等写像です。

注意 (1) $N = \bigoplus_{\lambda \in L} N_\lambda$ を、$L$ をインデックス集合とする$A$ モジュールの他のファミリの直和とし、すべての$\lambda \in L$ について、$v_\lambda : M_\lambda \to N_\lambda$ を$A$ 線形マッピングとします。 よってには、$A$ 線形マッピング $v = \bigoplus_\lambda v_\lambda : M \to N$ (II, § 1, no. 6、命題 6) があります。それから図式
$$
\begin{array}{ccc}
\bigotimes_{\lambda \in L} S(M_\lambda) & \xrightarrow{g_M} & S(M) \\
\downarrow & & \downarrow S(v) \\
\bigoplus_{\lambda \in L} S(v_\lambda) & \xrightarrow{g_N} & S(N)
\end{array}
$$
は、定義 (§ 4, no. 5, 系から命題 8) まで可換です。

同型 $g$ によって $S^n(M)$ が識別される $\bigotimes_{\lambda \in L} S(M_\lambda)$ のサブモジュール $A$ をより正確に記述することができます。 For every finite subset $J$ of $L$, we write $E_J = \bigotimes_{\lambda \in J} S(M_\lambda)$, so that $\bigotimes_{\lambda \in L} S(M_\lambda) = \varprojlim E_J$ relative to the directed set $\mathscr{F}(L)$ of finite subsets of $L$, by definition (§ 4, no. 5). For every family $\nu = (n_\lambda) \in \mathbf{N}^{(L)}$ (thus having *finite* support) such that $\sum_{\lambda \in L} n_\lambda = n$ and every finite subset $J$ of $L$ containing the support of the family $\nu$, we write

$$
S^{J,\nu}(M) = \bigotimes_{\lambda \in J} S^{n_\lambda}(M_\lambda)
$$

したがって、$E_J$ の次数 $n$ の元のうち部分加群 $E_{J,n}$ は、$J$ に含まれるすべての家族 $\nu$ に対する$S^{J,\nu}(M)$ の *直和* となり、$\sum_{\lambda \in L} n_\lambda = n$ となる(§ 4, no. 7、命題 10、§ 4, no. 8)。 慣例として、支援が $J$ に含まれない家族 $\nu$ には $S^{J,\nu}(M) = \{0\}$ と書きます。次に、$E_{J,n}$ は、*すべて* の *直和* と $S^{J,\nu}(M)$ と呼ぶこともできます。ここで、$\nu$ は、$\sum_{\lambda \in L} n_\lambda = n$ のように、*すべて* ファミリ $\nu = (n_\lambda)_{\lambda \in L}$ の集合 $H_n$ を通過します。 $S^0(M_\lambda)$ は $A$ と同一視されるため、明らかに、$L$ の 2 つの有限部分集合 $J \subset J'$ と、$J$、標準写像 $S^{J,\nu}(M) \to S^{J',\nu}(M)$ (標準写像の制限) に含まれるサポートの家族 $\nu$ も同様です。 $E_J \to E_J$ から $S^{J,\nu}(M)$) は *全単射*です。 $\nu \in H_n$ 全員に対して、次のように書くと、

$$
S^\nu(M) = \varprojlim S^{J,\nu}(M)
$$

II, § 6, no. 2、命題 5 を考慮すると、次のことがわかります。

#### 系 {#alg-iii-s6-n6-cor-1 .statement tag=062J}

*The A-module* $S^n(M)$ *is the image under isomorphism* (10) *of the submodule of* $\bigotimes_{\lambda \in L} S(M_\lambda)$ *the direct sum of the submodules* $S^\nu(M)$ *for all the families* $\nu = (n_\lambda) \in \mathbf{N}^{(L)}$ *such that* $\sum_{\lambda \in L} n_\lambda = n$; *if* $J$ *は* $\nu$、$S^\nu(M)$ *は標準的に* $\bigotimes_{\lambda \in J} S^{n_\lambda}(M_\lambda)$と同型です。

一般に、$S^\nu(M)$、$\bigotimes_{\lambda \in J} S^{n_\lambda}(M_\lambda)$、および$S^n(M)$ の像が識別されます。

#### 定理 1 {#alg-iii-s6-thm-1 .statement tag=062K}

*$A$ *を可換環とし、* $M$ *自由* $A$-*加群を基底* $(e_\lambda)_{\lambda \in L}$ とします。 *有限台の写像* $\alpha : L \to \mathbf{N}$ * ごとに、次のように書きます*

$$
e^\alpha = \prod_{\lambda \in L} e_\lambda^{\alpha(\lambda)}
$$

(*可換代数* $S(M)$の*積)。 *その後* $\alpha$ * が集合* $\mathbf{N}^{(L)}$ * の写像から * $L$ * $\mathbf{N}$ に * 有限台の* $e^\alpha$ * 形基底を通過すると$A$-*加群* $S(M)$。

$M$ は $M_\lambda = Ae_\lambda$ の直和であるため、$L$ が単一の元に還元され、次に命題を適用する 9 になるとき、定理を証明するのに十分です。 しかし、$M = Ae$ (*e* は自由な元) の場合、 $M$ のすべての $x, y$ に対して $x \otimes y - y \otimes x = 0$。したがって、イデアル $\mathfrak{g}'$ は零、よって $T(Ae) = S(Ae)$、定理となり、§ 5, no. 5、定理 1 から続きます。

基底 (14) の乗法表は次のように与えられます。

(15)
$$
e^\alpha e^\beta = e^{\alpha + \beta}
$$
ここで、$\alpha + \beta$ は $L$ の写像 $\lambda \mapsto \alpha(\lambda) + \beta(\lambda)$ を $\mathbf{N}$ に変換します。他の語では、$S(M)$ の基底 $(e^\alpha)$ は、乗法法則 (15) とともに、$L$ から導出される自由可換モノイド $N^{(L)}$ と正準的に同型です。 (§ 2, no. 9)、自由加群 $M$ の基底の対称代数 $S(M)$ (そのインデックス集合は $L$) は、多項式代数と正準的に同型であることがわかります。 $A[(X_\lambda)_{\lambda \in L}]$、標準同型は、写像 $e_\lambda$ から $X_\lambda$ によって取得されます。特に (§ 2, no. 7, 命題 7)、$L$ の各写像 $f : L \to E$ を可換 $A$-代数 $E$ に入れると、そのような $A$-代数準同型性 $\tilde{f} : S(M) \to E$ が 1 つだけ存在します。それは$\tilde{f}(e_\lambda) = f(\lambda)$です。

注意 (2)。上記の結果は、II, § 1, no. 11、系 3 ～ 命題 17 を考慮すると、多項式代数と対称代数の普遍的性質の帰結としても同様に得られます。

#### 系 {#alg-iii-s6-n6-cor-2 .statement tag=062L}

*$M$ が射影 $A$ モジュールの場合、$S(M)$ は射影 $A$ モジュールです。*

証明は§ 5, no. 5、系～定理1、置き換えること$T$by$S$と同じです。

#### 命題 10 {#alg-iii-s6-prop-10 .statement tag=062M}

*$\Delta$ を可換モノイド、$M$ を型 $\Delta$ および $(M_\alpha)_{\alpha \in \Delta}$ の段階的な $A$ 加群とする。 注文されたすべての対 $(\alpha, n) \in \Delta \times \mathbf{N}$ について、$S^{\alpha, n}(M)$ を $S^n(M)$ の部分加群部分加群 $\bigotimes_{\lambda \in J} S^{n_\lambda}(M_{\alpha_\lambda})$ の直和とします。ここで、$(n_\lambda)_{\lambda \in L}$ は整数 $\geq 0$ の家族の集合を通過します。 $\sum_{\lambda \in L} n_\lambda = n$、$J$ がそのサポートであり、それぞれの $(n_\lambda), (\alpha_\lambda)_{\lambda \in J}$ が $\sum_{\lambda \in J} \alpha_\lambda = \alpha$ のように $\Delta^J$ の家族の集合を通過します。 この場合、$(S^{\alpha, n}(M))_{(\alpha, n) \in \Delta \times \mathbf{N}}$ は、$S(M)$ の代数構造と互換性のある型 $\Delta \times \mathbf{N}$ の唯一の目盛りであり、$M = S^1(M)$ の誘導するは指定された目盛りです*。

$S(M)$ が $S^{\alpha, n}(M)$ の直和であるという事実は、系から命題 9 に続きます。 証明の残りは、§ 5, no. 5、命題 7の証明の終わりと同じです。

より具体的には、$\Delta = \mathbf{Z}$ と仮定し、$S(M)$ に上記で定義した型 $\mathbf{Z} \times \mathbf{N}$ (したがって型 $\mathbf{Z} \times \mathbf{Z}$) の合計卒業量 (型 $\mathbf{Z}$) (II, § 11, no. 1) 対応するを与えるとします。したがって、この目盛りの下での次数 $n \in \mathbf{Z}$ の同種の元は、$q + m = n$ に対する $S^{q, m}(M)$ の直和のものです。 $f$ を、等級付けされた $A$ 加群 $M$ の *次数* 0 の *同次* 線形写像を、型 $\mathbf{Z}$ の *可換* 等級付けされた $A$-代数 $F$ にします。次に、$M$ の均質な $x_i$ に対する公式 $g(x_1 x_2 \ldots x_n) = f(x_1) f(x_2) \ldots f(x_n)$ から以下のように、$f = g \circ \phi_M'$ が型* $\mathbf{Z}$ の等級付けされた代数の *準同型となるような代数準同型 $g : S(M) \to F$ です。 $f$の仮定と型の$\mathbf{Z}$の卒業の定義から$S(M)$です。

### 練習問題 {#alg-iii-s6-exercises}

[§ 6 に対して練習問題](exercises/s6/)を参照してください。
