---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Lie Algebras
section: 5
section_title: Solvable Lie algebras
lang: ja
source: lie-i-iii
book_pages: 43-50, 99-101
pdf_pages: 0061-0068, 0117-0119
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF SOLVABLE LIE ALGEBRAS
      page: 43
      pdf_page: 61
    - "no": 2
      title: RADICAL OF A LIE ALGEBRA
      page: 44
      pdf_page: 62
    - "no": 3
      title: NILPOTENT RADICAL OF A LIE ALGEBRA
      page: 44
      pdf_page: 62
    - "no": 4
      title: A CRITERION FOR SOLVABILITY
      page: 47
      pdf_page: 65
    - "no": 5
      title: FURTHER PROPERTIES OF THE RADICAL
      page: 48
      pdf_page: 66
    - "no": 6
      title: EXTENSION OF THE BASE FIELD
      page: 49
      pdf_page: 67
statements: 27
exercises: 17
content_sha256: ffe04ebd52df20ee3d7fecdd7b7a3badfe66a69ff5ae0aec72e7165122e1f70b
translated_from: content/en/lie/I/05_s5_solvable_lie_algebras.md
translation_method: google
source_content_sha256: 17ded9a5fe0c8a2a7818b8d120cc2777d7e553298aff0352151f7762860f3aac
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: 4d3487a649e105ee366c00bd195c75522822fc7c2daf48731c95053e836159ed
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 5。 可解リー代数

以降、$K$ は特性 0 の体を示し、すべてのリー代数は $K$ 上で有限次元であると仮定されることを思い出してください。

### 1. 定義/可解リー代数

#### 定義 1 {#lie-i-s5-def-1 .statement tag=09Y1}

*リー代数 $g$ は、その k 番目に導出された代数 $D^k g$ が十分大きい $k$ に対して零である場合、解決可能と呼ばれます。*

べき零リー代数は解けます。

#### 命題 1 {#lie-i-s5-prop-1 .statement tag=09Y2}

※可解リー代数の部分代数と商代数は解けます。解ける代数による解ける代数のすべての拡大は解けます。可解な代数のすべての有限積は可解です。*

$g$ を $g$ から $t$ に$g$、$t = g/h$、$\phi$ 標準写像をリー代数、$g'$ 部分代数、$h$ とします。 $g$ が解けるなら、一部の整数 $k$ に対して $D^k g = \{0\}$、したがって $D^k g' \subset D^k g = \{0\}$、$D^k t = \phi(D^k g) = \{0\}$、そして$g'$ と $t$ が解けます。 $h$ と $t$ が解ける場合、次のような整数 $s, t$ が存在します。

$$
D^s h = D^t t = \{0\};
$$

すると$D^t g \subset h$、したがって$D^{s+t} g = D^s(D^t g) \subset D^s h = \{0\}$と$g$は解けます。 最後の主張は、因子の数の帰納法による2番目から続きます。

#### 命題 2 {#lie-i-s5-prop-2 .statement tag=09Y3}

※$g$をリー代数とします。次の条件は同等です:*

(a) $g$ は解けます。
(b) *代数 $g_i/g_{i+1}$ が可換 ($i = 0, 1, \ldots, n-1$) となるような $g$ のイデアの減少列 $g = g_0 \supset g_1 \supset \cdots \supset g_n = \{0\}$ が存在します。*
(c) *$g'_{i+1}$ が $g'_i$ のイデアルであり、$g'_i/g'_{i+1}$ が可換 ($i = 0, 1, \ldots, p-1$) であるような、$g$ の部分代数の減少列 $g = g'_0 \supset g'_1 \supset \cdots \supset g'_p = \{0\}$ が存在します。*
(d) *$g''_{i+1}$ がコディメンション 1 ($i = 0, 1, \ldots, q-1$) の $g''_i$ の理想となるような $g$ の部分代数の減少列 $g = g''_0 \supset g''_1 \supset \cdots \supset g''_q = \{0\}$ が存在します。

(a) $\Rightarrow$ (b): $g$ の派生理想の数列を考慮すれば十分です。
(b) $\Rightarrow$ (c): これは明らかです。
(c) $\Rightarrow$ (d): 条件 (c) が成立すると仮定します。 $g'_i$ 含む $g'_{i+1}$ のすべてのベクトル部分空間は、直ちに $g'_i$、よっての理想になります (d)。
(d) $\Rightarrow$ (a): これは、可溶な代数によって可溶な代数の拡大が可溶であるという事実からすぐに得られます。

† 読者は、$K$ の特性に関する仮定が nos では使用されていないことに注意するでしょう。この段落の 1 と 2。

例/可解リー代数

I。 $g$ を $K$ と $g$ の $(e_1, e_2)$ 基底上の 2 次元ベクトル空間とします。 $g$ 上には、$[e_1, e_2] = e_2$ となるような交代的双線形乗法 $(x, y) \mapsto [x, y]$ が 1 つだけ存在します。 したがって、$g$ が可解リー代数構造となることは簡単に検証できます。 ここで、$h$ を $K$ 上の次元 2 の非可換リー代数とします。 $h$ が $g$ と同型であることを示します。 $(f_1, f_2)$ を $h$ の基底とします。 元 $[f_1, f_2]$ はゼロではない (そうでない場合、$h$ は可換である) ので、生成するは 1 次元の部分空間 $t$ の $h$ です。 次に$[h, h] = t$。 $(e'_1, e'_2)$ を $h$ の基底として、$e'_2 \in t$ とします。 次に、$[e'_1, e'_2] = \lambda e'_2$ と $\lambda \neq 0$ を組み合わせます。 置き換えること $e'_1$ $\lambda^{-1} e_1$ により、$\lambda = 1$、よってが私たちの主張であると想定できます。

II。 § 1の式(5)は$\mathscr{D}t(n, K) = n(n, K)$を証明します。 $n(n, K)$ は零能であり、したがって可解であるため、$t(n, K)$ は可解です。したがって、$st(n, K)$は解けます。特に、$st(2, K)$ は、例 I の代数と同型です。

### 2. リー代数中根基

$a, b$ を、リー代数 $g$ の 2 つの解決可能な理想とする。 代数 $(a + b)/b$ は $a/(a \cap b)$ と同型であるため解け、$(a + b)/b$ の $b$ による拡大である $a + b$ も解けます (命題 1)。したがって、$g$ 含むの最大の可溶イデアルは $g$ のすべての可溶イデアル、したがって $g$ には最大のの可溶イデアルが存在します。これにより、次の定義が可能になります。

#### 定義 2 {#lie-i-s5-def-2 .statement tag=09Y4}

* リー代数の根基は、その最大のの解決可能な理想です。*

#### 命題 3 {#lie-i-s5-prop-3 .statement tag=09Y5}

* リー代数 $g$ の根基 $r$ は、$g/r$ が根基 $\{0\}$ となるような $g$ の最小のの理想です。

$a$ を $g$ から $g/a$ への $g$ と $\phi$ 標準写像の理想とします。 $g/a$の根基が零であれば、$g/a$の解ける理想である$\phi(r)$は零です。したがって$r \subset a$です。

一方、根基 $r'$ の $g/r$ の逆像 $\phi^{-1}(r')$ は、命題 1 で解ける$g$ のイデアルなので、$r$ に等しくなります。したがって$r' = \{0\}$。

#### 命題 4 {#lie-i-s5-prop-4 .statement tag=09Y6}

※$g_1, \ldots, g_n$をリー代数とします。 The radical $r$ of the product of the $g_i$ is the product of the radicals $r_i$ of the $g_i$.*

$r_i$ の積 $r'$ は解けるイデアル (命題 1) なので、$r' \subset r$ です。 $g_i$ の $r$ の標準像は、$g_i$ の解決可能な理想であるため、$r_i$ に含まれます。したがって$r \subset r'$です。

### 3. 無能根基/リー代数

#### 定義 3 {#lie-i-s5-def-3 .statement tag=09Y7}

※$g$をリー代数とします。 $g$ の零能根基は、$g$ の有限次元単純表現の核の共通部分です。

#### 注意 {#lie-i-s5-n3-rem-1 .statement tag=09Y8}

(1) $s$ を $g$ のゼロポテント根基とします。 $g$のベクトル部分空間のすべての減少列が静止しているため、核が共通部分$s$を持つ$g$の有限次元単純表現の有限数が存在します。

これら表現のうち直和は半単純であり、 核があります。したがって、g の有限次元半単純表現の核の集合には、最小の元、つまり s が存在します。

(2) § 4, no. 3 の命題 4 (c) により、s は g の有限次元表現の零位理想の最大のの共通部分にもなります。特に、s は g の最大のの虚数イデアルに含まれているため、g の虚数イデアルになります。

(3) $\mathscr{D}g$ の零である g のすべての線型形式 $\lambda$ は、g の単純な表現 (空間 K 付き)、よって $\lambda(s) = \{0\}$ です。 $s \subset \mathscr{D}g$ ということになります。一方、s は注意 2 により g の根基 r に含まれます。$s = r \cap \mathscr{D}g$ であることを証明します。

#### 補題 1 {#lie-i-s5-lem-1 .statement tag=09Y9}

Let V be a finite-dimensional vector space over K, g a subalgebra of gl(V) such that V is a simple g-module and a a commutative ideal of g. 次に$a \cap \mathscr{D}g = \{0\}$。 S を 1 と a によって生成される $\mathscr{L}(V)$ の部分代数とします。

b が、すべての $b \in b$ とすべての $s \in S$ に対して $\operatorname{Tr} bs = 0$ であるような、a に含まれる g のイデアルである場合、特に、S の定義により、すべての整数 $n > 0$ に対して $\operatorname{Tr}(b^n) = 0$ となり、したがって b はゼロポテント (代数, 章) VII, § 5, no. 5、系 4 ～ 命題 13); b の元はすべて nilpotent であるため、$b = \{0\}$ (§ 4, no. 3、補題 2) です。まずこれを g の理想 $[g, a]$ に適用します。 $x \in g, a \in a, s \in S$ の場合、$as = sa$ 以降は $\operatorname{Tr}[x, a]s = \operatorname{Tr}(xas - axs) = \operatorname{Tr} x(as - sa) = 0$ になります。したがって$[g, a] = \{0\}$です。したがって、g の元は a のものと可換であり、したがって S のものとも可換です。 $x, y$ 属するが g および $s \in S$ である場合、

$$
\operatorname{Tr}[x, y]s = \operatorname{Tr}(xys - yxs) = \operatorname{Tr} x(ys - sy) = 0
$$

$ys = sy$以来;次に、b を理想的な $\mathscr{D}g \cap a$ とすると、$\mathscr{D}g \cap a = \{0\}$ となります。

#### 定理 1 {#lie-i-s5-thm-1 .statement tag=09YA}

g をリー代数、r を根基、そして s をゼロポテント根基とします。次に$s = \mathscr{D}g \cap r$。

$s \subset \mathscr{D}g \cap r$ ということはすでにわかっています。したがって、$\rho$ が g の有限次元単純表現である場合、$\rho(\mathscr{D}g \cap r) = \{0\}$ であることを示せば十分です。 k を最小の整数 $\geq 0$ とし、$\rho(\mathscr{D}^{k+1}r) = \{0\}$ とします。 $g' = \rho(g)$、$a' = \rho(D^k r)$と書きます。 $\mathscr{D}^k r$ は g のイデアル、$a'$ は $g'$ のイデアルです。このイデアルは $\rho(\mathscr{D}^{k+1}r) = \{0\}$ 以降可換です。 V が $\rho$、$g' \subset \operatorname{gl}(V)$ の空間である場合、V は単純な $g'$ モジュールです。それから$\rho(\mathscr{D}g \cap \mathscr{D}^k r) \subset \mathscr{D}g' \cap a' = \{0\}$。 $k > 0$なら、kの定義とは逆に、$\mathscr{D}^k r \subset \mathscr{D}g$と$\rho(\mathscr{D}^k r) = \{0\}$です。したがって、$k = 0$、つまり

$$
\rho(\mathscr{D}g \cap r) = \{0\}.
$$

#### 系 1 {#lie-i-s5-thm-1-cor-1 .statement tag=09YB}

g を可解リー代数とします。 gの無力根基は$\mathscr{D}g$です。 $\rho$ が g の有限次元単純表現である場合、$\rho(g)$ は可換であり、1 と $\rho(g)$ によって生成される結合代数 L は K 上の有限次数の体です。

こちら$r = g$、よって $s = \mathscr{D}g$。したがって、$\varphi(\mathscr{D}g) = \{0\}$ は、$g' = \rho(g)$ が可換であることを示します。 $L$ のすべての元 $\neq 0$ は、シュールの補題によって反転できます。したがって、$L$は体です。

#### 系 2 (嘘定理) {#lie-i-s5-thm-1-cor-2 .statement tag=09YC}

*$g$を可解リー代数とします。 $K$ が代数的に閉じていると仮定します。 $M$ を $K$ 上の有限次元の $g$ モジュールとし、$(M_i)_{0 \leq i \leq r}$ を $M$ の Jordan-Hölder 系列とします。次に、$M_{i-1}/M_i$ は、$1 \leq i \leq r$ に対して $K$ 1 上で次元であり、すべての $x \in g$、$x_{M_{i-1}/M_i} = \lambda_i(x) \cdot 1$ で、$\lambda_i$ は $g$ の線型形式であり、零です。 $\mathscr{D}g$。特に、$K$ 上の有限次元のすべての単純な $g$ モジュールは、実際には次元 1 です。*

$\rho_i$ を $M_{i-1}/M_i$ の $g$ の表現とします。 1 と $\rho_i(g)$ によって生成される結合代数 $L_i$ は体であり、$K$ の有限拡大であるため、$K$ に等しくなります。そして、$M_{i-1}/M_i$ は単純な $L_i$ モジュール、よって $\dim M_{i-1}/M_i = 1$ です。 系の残りは明らかです。

#### 注意 {#lie-i-s5-n3-rem-2 .statement tag=09YD}

(1) $(M_i)_{0 \leq i \leq r}$ が $M$ の他の Jordan-Hölder 系列に置き換えられる場合、数列 $(\lambda_1, \ldots, \lambda_r)$ は形 $(\lambda_{\pi(1)}, \ldots, \lambda_{\pi(r)})$ の数列に置き換えられます。ここで、$\pi$ は、置換です$\{1, \ldots, r\}$、ヨルダン・ヘルダー定理より以下の通り。

(2) $(e_1, \ldots, e_r)$ を $M$ の基底とし、$e_i \in M_{i-1}, e_i \notin M_i$ ($1 \leq i \leq r$) とします。 If $x \in g$ the endomorphism of $M$ corresponding to $x$ is represented with respect to this basis by a triangular matrix whose diagonal coefficients are

$$
\lambda_1(x), \ldots, \lambda_r(x).
$$

#### 系 3 {#lie-i-s5-thm-1-cor-3 .statement tag=09YE}

*$K$ が代数的に閉じていると仮定します。 If $g$ is an $r$-dimensional solvable Lie algebra, every ideal of $g$ is a term of a decreasing sequence of ideals of dimensions $r, r-1, \ldots, 0$.*

Every ideal is part of a Jordan-Hölder series of $g$, considered as the space of the adjoint representation (*Algebra*, Chapter I, § 6, no. 14, Corollary to Theorem 8); then it suffices to apply Corollary 2.

#### 系 4 {#lie-i-s5-thm-1-cor-4 .statement tag=09YF}

※$K = \mathbf{R}$とします。 $g$を可解リー代数とします。 $g$ のすべての単純な表現は次元 $\leq 2$ になります。 $g$ のすべての理想は、減少列の項 $(g_i)_{0 \leq i \leq m}$ のような理想であり、$g_0 = g, g_m = \{0\}, \dim g_{i-1}/g_i \leq 2$ ($1 \leq i \leq m$) です。

これは、系 2 および系 3 と同様の方法で、$\mathbf{R}$ のすべての代数拡大が次数 $\leq 2$ であるという事実を使用して証明されます。

#### 系 5 {#lie-i-s5-thm-1-cor-5 .statement tag=09YG}

*リー代数 $g$ が解けるには、$\mathscr{D}g$ が零であることが必要かつ十分です。*

条件は系 1 によって必要です。$g/\mathscr{D}g$ は可換なので十分です。

#### 系 6 {#lie-i-s5-thm-1-cor-6 .statement tag=09YH}

*$\varphi$をリー代数$g$の有限次元表現とします。 * r を g の根基とします。 $\rho(x)$ がゼロポテンシー 属するから最大のの理想ゼロポテンシー $\rho$ の $n$ となるようなすべての元 $x \in r$。

V を $\rho$ の空間とします。 $(V_i)_{0 \leq i \leq r}$ を V の r 加群構造のジョルダン・ヘルダー 系列とし、$\rho_i$ を空間 $V_i / V_{i-1}$ ($1 \leq i \leq r$) を持つ r の表現とします。 $\rho(x)$ が無能であれば、$\rho_i(x)$ も無能です。 $\rho_i(x)$ によって生成されるすべての $i$ 代数は、体、$\rho_i(x) = 0$ です。逆に、$i$がすべて$\rho_i(x) = 0$なら、$\rho(x) = 0$。これは、$\rho(x)$ が零能であるような $x \in r$ の集合 $a$ が r の理想であることを示しています。一方、$[g, a] \subset \mathscr{D}g \cap r \subset n \cap r \subset a$、したがって$a$ は g のイデアルです。これは$a \subset n$であることを証明します。

#### 系 7 {#lie-i-s5-thm-1-cor-7 .statement tag=09YI}

gをリー代数、rを根基とします。次の 4 つの集合は同一です。 (a) 最大の g の零理想体。 (b) 最大の r の零イデアル。 (c) $\mathrm{ad}_g x$ がゼロになるような $x \in r$ の集合。 (d) $\mathrm{ad}_r x$ がゼロになるような $x \in r$ の集合。

これらの集合を$a, b, c, d$と表すことにします。 内包物$a \subset b \subset d \subset c$はクリアです。 $c \subset a$ by 系 6 を g の随伴項表現に適用します。

### 4. 解決可能性の基準

#### 補題 2 {#lie-i-s5-lem-2 .statement tag=09YJ}

$x$ を有限次元ベクトル空間 V の自己準同型とし、s (それぞれ n) をその半単純 (それぞれ無能) 成分 (cf. 代数, 章 VIII, § 9, no. 4, 定義 4）。 $\mathrm{ad}\, x, \mathrm{ad}\, s, \mathrm{ad}\, n$ を、$\mathfrak{gl}(V)$ の随伴表現における $x, s, n$ のそれぞれの像とします。このとき、$\mathrm{ad}\, s$ (それぞれ$\mathrm{ad}\, n$) は、$\mathrm{ad}\, x$ の半単純 (それぞれゼロポテント) 成分であり、K に係数があり、定数項がない$\mathrm{ad}\, x$ の多項式に等しくなります。

$\mathrm{ad}\, x = \mathrm{ad}\, s + \mathrm{ad}\, n, [\mathrm{ad}\, s, \mathrm{ad}\, n] = 0$ と $\mathrm{ad}\, n$ は無能であることがわかっています ($§ 4$、補題 1)。 $\mathrm{ad}\, s$ は半単純であることがわかります。 K が代数的に閉じている場合 (cf. 代数, 章 VIII, § 9, no. 2, 命題 3) にこれを行うだけで十分です。次に、$(e_i)_{1 \leq i \leq n}$ を V の基底とし、$s(e_i) = \lambda_i e_i$ ($\lambda_i \in K$) とします。 $(E_{ij})$を$M_n(K) = \mathfrak{gl}(V)$の標準基底とします。 $§ 1$の式(5)より、

$$
(\mathrm{ad}\, s)\cdot E_{ij} = (\lambda_i - \lambda_j)E_{ij}
$$

したがって、$\mathrm{ad}\, s$ は半単純です。 The last assertion of the lemma follows from Algebra, Chapter VIII, § 9, no. 4, Proposition 8.

#### 補題 3 {#lie-i-s5-lem-3 .statement tag=09YK}

Mを有限次元ベクトル空間、AとBを$\mathfrak{gl}(M)$の2つベクトル部分空間として$B \subset A$、Tを$t \in \mathfrak{gl}(M)$の集合として$[t, A] \subset B$とします。 $z \in T$ がすべての $u \in T$ に対して $\mathrm{Tr}(zu) = 0$ となるような場合、$z$ は零能です。

K が代数的に閉じている場合にこれを証明すれば十分であり、今後はこれを仮定します。 s と n を z の半単純と冪能成分とし、$(e_i)$ を $s(e_i) = \lambda_i e_i$ ($\lambda_i \in K$) となる M の基底とします。 $V \subset K$ を $\lambda_i$ によって生成された $\mathbf{Q}$ 上のベクトル空間とします。 $V = \{0\}$ を証明する必要があります。 f を V 上の $\mathbf{Q}$ 線形形式とし、t を次のような M の自己準同型とします。

$te_i = f(\lambda_i)e_i$。 $(E_{ij})$ が $E_{ij}e_k = \delta_{jk}e_i$ によって定義される $\mathfrak{gl}(M)$ の標準基底である場合、
$$
\begin{align*}
(\mathrm{ad}\ s)E_{ij} &= (\lambda_i - \lambda_j)E_{ij} \\
(\mathrm{ad}\ t)E_{ij} &= (f(\lambda_i) - f(\lambda_j))E_{ij}.
\end{align*}
$$

定数項がなく、K に係数があり、すべての i と j について $P(\lambda_i - \lambda_j) = f(\lambda_i) - f(\lambda_j)$ となる多項式 P が存在します ($\lambda_i - \lambda_j = \lambda_h - \lambda_k$ の場合は $f(\lambda_i) - f(\lambda_j) = f(\lambda_h) - f(\lambda_k)$、$\lambda_i - \lambda_j = 0$ の場合は $f(\lambda_i) - f(\lambda_j) = 0$)。次に$\mathrm{ad}\ t = P(\mathrm{ad}\ s)$。一方、$\mathrm{ad}\ s$は$\mathrm{ad}\ z$に定数項を持たない多項式です。現在、$(\mathrm{ad}\ z)(A) \subset B$、よって、また$(\mathrm{ad}\ t)(A) \subset B$です。 仮定 $0 = \mathrm{Tr}(zt) = \sum \lambda_i f(\lambda_i)$、よって $0 = f(\mathrm{Tr}(zt)) = \sum f(\lambda_i)^2$までに。 $f(\lambda_i)$ は有理数、$f = 0$ なので、証明が完成します。

#### 定理 2 (カルタンの基準) {#lie-i-s5-thm-2 .statement tag=09YL}

*g をリー代数、M 有限次元ベクトル空間、M 上の g の ρ 表現、ρ に関連付けられた g 上の β 双線形形式とする。この場合、ρ(g) は、$\mathscr{D}$g が β に関して g に直交する場合に限り、解くことができます。*

それは明らかに、g が $\mathfrak{gl}(M)$ の嘘部分代数で、ρ が恒等写像である場合に還元できます。 g が可解であれば、$\mathscr{D}$ g は g (定理 1) の恒等式表現の零イデアルの最大のに含まれるため、β に関して g と直交します (§ 4, 命題 4 (d))。 $\mathscr{D}$g が β に関して g に直交するとします。 g が可解であることを証明します。 T を $[t, g] \subset \mathscr{D}g$ となるような $t \in \mathfrak{gl}(M)$ の集合とします。 $t \in T$ と x、y 属するから g の場合、$[t, x] \in \mathscr{D}g$ となり、したがって
$$
\mathrm{Tr}(t[x, y]) = \beta([t, x], y) = 0
$$
すべての $u \in \mathscr{D}g$ に対して、線形性 $\mathrm{Tr}(tu) = 0$ によりよって 。また、明らかに$\mathscr{D}g \subset T$。したがって、(補題 3) $\mathscr{D}$g のすべての元はゼロ能です。したがって、$\mathscr{D}$g はゼロポテント (§ 4、系 3 ～ 定理 1) であり、したがって g は可解です (no. 3、系 5 ～ 定理 1)。

### 5. 根基のその他の特性

#### 命題 5 {#lie-i-s5-prop-5 .statement tag=09YM}

*g をリー代数、r を根基とします。*
(a) *ρ が g の有限次元表現で、β が関連する双線形形式である場合、r と $\mathscr{D}$g は β に関して直交します。*
(b) *r は、殺人形に関する $\mathscr{D}$g の直交です。*
x、y を g、$z \in r$ とする。次に $[y, z] \in \mathscr{D}g \cap r$ 以降
$$
\beta([x, y], z) = \beta(x, [y, z]) = 0
$$
(定理1)。したがって、(a)。
r' を Killing 形に対する $\mathscr{D}$g の直交とします。以上より含む r となる g (§ 3, no. 6, 命題 7 (a)) の理想です。一方、g の随伴表現の下にある r' の像 s は可解 (定理 2) であるため、r' は s の中心拡大として可解です。したがって、r' ⊂ r となります。

#### 系 1 {#lie-i-s5-prop-5-cor-1 .statement tag=09YN}

g をリー代数とします。この場合、$\mathscr{D}g$ が Killing 形に関して g に直交する場合に限り、g は解けます。

これは、命題 5 (b) の明らか帰結です。

#### 系 2 {#lie-i-s5-prop-5-cor-2 .statement tag=09YO}

リー代数 g の根基 r は特性理想です。

$\mathscr{D}g$ は特徴的な理想であり、Killing 形は完全に不変です (§ 3, no. 6、命題 10)。したがって、殺人形に対する$\mathscr{D}g$ の直交は、特徴的なイデアルです (§ 3, no. 6, 命題 7 (b))。

#### 系 3 {#lie-i-s5-prop-5-cor-3 .statement tag=09YP}

g をリー代数、r を根基、a を g のイデアルとします。この場合、a の根基は $r \cap a$ に等しくなります。

r ∩ a は a の可解なイデアルであるため、a の根基 r' に含まれます。逆に、r' は g のイデアル (系 2 および § 1, no. 4, 命題 2) であるため、r' ⊂ r となります。

系 2 は次のようにより正確にすることができます。

#### 命題 6 {#lie-i-s5-prop-6 .statement tag=09YQ}

g をリー代数、r を根基、n を最大のの零理想理想とする。 g 写像 r の導分ごとを n に変換します。

D を g の導分とします。 g' = g + Kx_0 をリー代数とします。ここで、g は、すべての x ∈ g (§ 1, no. 8, 例 1) に対して Dx = [x_0, x] となる余次元 1 のイデアルです。 系 3 ～ 命題 5 により、r は g' の根基 r' に含まれます。この場合、D(r) = [x_0, r] ⊂ [g', g'] ∩ r' = s' となります。すべての x ∈ s' に対して、ad_{g'} x は零能です (定理 1)。したがって、すべての x ∈ s' ∩ g に対して、ad_g x は零能です。したがって、D(r) は g の冪能イデアル s' ∩ g に含まれます。

#### 系 {#lie-i-s5-n5-cor-1 .statement tag=09YR}

最大のリー代数の無能イデアは特徴的なイデアです。

#### 注意 {#lie-i-s5-n5-rem-1 .statement tag=09YS}

上記の結果の一部を要約すると、r、n、s、t がそれぞれ、g の根基、g の尐能イデアル最大の、g の冪能根基、および Killing 形に関する g の直交を表す場合、次のようになります。

$$
r \supset t \supset n \supset s.
$$

包含 r ⊃ t は命題 5 (b) から導かれます。包含 t ⊃ n は § 4, no. 4, 命題 6 (b) から続きます。 no. 3 の注意 2 で n ⊃ s が含まれることが指摘されています。

### 6. 基礎体中拡大

g を K の嘘 K-代数および K_1 拡大とします。明らかに g_{(K_1)} は、$\mathscr{D}^n(g_{(K_1)}) = (\mathscr{D}^n g)_{(K_1)}$ 以来 g が解ける場合にのみ解けます。

r を g の根基とします。すると、$r_{(K_1)}$ * は $g_{(K_1)}$ の根基です。 $\beta$ を g の殺害形とします。 r は $\beta$ (命題 5 (b)) に対する $\mathscr{D}g$ の直交であるため、$r_{(K_1)}$ は、$\beta$ から拡大によって K から $K_1$ まで導かれる形に対する $(\mathscr{D}g)_{(K_1)} = \mathscr{D}(g_{(K_1)})$ の直交です。 $g_{(K_1)}$中形(§ 3, no. 8)を殺害。次に、主張は、命題 5 (b) をさらに適用したものになります。

### 練習問題 {#lie-i-s5-exercises}

§ 5 の規則は、特に記載されていない限り、引き続き有効です 〜でない限り。

[§ 5 に対して練習問題](exercises/s5/)を参照してください。
