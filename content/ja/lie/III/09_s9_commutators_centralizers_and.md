---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 9
section_title: Commutators, centralizers and normalizers in a Lie group
lang: ja
source: lie-i-iii
book_pages: 342-359, 397-409
pdf_pages: 0360-0377, 0415-0427
extraction: ocr
subsections:
    - "no": 1
      title: COMMUTATORS IN A TOPOLOGICAL GROUP
      page: 342
      pdf_page: 360
    - "no": 2
      title: COMMUTATORS IN A LIE GROUP
      page: 343
      pdf_page: 361
    - "no": 3
      title: CENTRALIZERS
      page: 346
      pdf_page: 364
    - "no": 4
      title: NORMALIZERS
      page: 347
      pdf_page: 365
    - "no": 5
      title: NILPOTENT LIE GROUPS
      page: 347
      pdf_page: 365
    - "no": 6
      title: SOLVABLE LIE GROUPS
      page: 352
      pdf_page: 370
    - "no": 7
      title: RADICAL OF A LIE GROUP
      page: 354
      pdf_page: 372
    - "no": 8
      title: SEMI-SIMPLE LIE GROUPS
      page: 355
      pdf_page: 373
statements: 54
exercises: 42
content_sha256: 47e5a05c6249119bb7f99e9368798d2bb019f36549f1fc4698eea070eba669b2
translated_from: content/en/lie/III/09_s9_commutators_centralizers_and.md
translation_method: google
source_content_sha256: 5160b395f31c39ef9f1ad5f95ebd21b2c6f9dc63a62483b154ec6113d26d8afa
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 53f622a8cfce1cec30fa2420fe65af4feed2e31be4a4cadf30d900eecd79937c
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 9。 交換子、リー群のセントラライザーとノーマライザー

この段落では、K は標数0 であると仮定します。

### 1. トポロジー 群の交換子

G を位相ベクトル群とします。式によれば、定義する群 $\overline{D^0G}, \overline{D^1G}, \overline{D^2G}, \ldots$ と $\overline{C^1G}, \overline{C^2G}, \overline{C^3G}, \ldots$

$$
\begin{aligned}
\overline{D^0G} &= G, & \overline{D^{i+1}G} &= (\overline{D^iG}, \overline{D^iG}) \\
\overline{C^1G} &= G, & \overline{C^{i+1}G} &= (G, \overline{C^iG}).
\end{aligned}
$$

#### 命題 1 {#lie-iii-s9-prop-1 .statement tag=0AII}

*G をトポロジカル群とし、A と B 部分群を G とします。すると* $(\overline{A}, \overline{B}) = (\overline{A}, \overline{B}), \overline{D^iA} = \overline{D^iA}, \overline{C^iA} = \overline{C^iA}$ となります。

$\phi$ を G への $G \times G$ の連続写像 $(x, y) \mapsto x^{-1}y^{-1}xy$ とします。すると、$\phi(A \times B) \subset (A, B)$、したがって $\phi(\overline{A} \times \overline{B}) \subset (\overline{A}, \overline{B})$、したがって

$$
(\overline{A}, \overline{B}) \subset (\overline{A}, \overline{B});
$$

反対の包含は明らかなので、$(\overline{A}, \overline{B}) = (\overline{A}, \overline{B})$。明らかに $\overline{D^0A} = \overline{D^0A}$; 等式 $\overline{D^iA} = \overline{D^iA}$ と仮定すると、次のようになります。

$$
\overline{D^{i+1}A} = (\overline{D^iA}, \overline{D^iA}) = (\overline{D^iA}, \overline{D^iA}) = (\overline{D^iA}, \overline{D^iA}) = \overline{D^{i+1}A}
$$

したがって、すべての $i$ に対して $\overline{D^iA} = \overline{D^iA}$ となります。 公式 $\overline{C^iA} = \overline{C^iA}$ の証明も同様です。

#### 系 1 {#lie-iii-s9-prop-1-cor-1 .statement tag=0AIJ}

*G がハウスドルフの場合、次の条件は同等です*:
(i) *G は可解* (それぞれ *ゼロポテント*);
(ii) $\overline{D^iG} = \{e\}$ (それぞれ $\overline{C^iG} = \{e\}$) *十分大きい* $i$ の場合。
$D^iG \subset \overline{D^iG}, C^iG \subset \overline{C^iG}$ したがって (ii) $\Rightarrow$ (i)。 $\{e\} = \{\overline{e}\}$ したがって (i) $\Rightarrow$ (ii) 命題 1.

#### 系 2 {#lie-iii-s9-prop-1-cor-2 .statement tag=0AIK}

*G を G のハウスドルフ トポロジカル群および A 部分群とします。A が解ける* (それぞれ *零能、可換*、*$\overline{A}$ *そう*であることが必要かつ十分です*)。

§ 9.2

これは命題 1 の直後に続きます。

#### 命題 2 {#lie-iii-s9-prop-2 .statement tag=0AIL}

G をトポロジー 群、G の A と B 部分群とします。A が接続されている場合、(A, B) は接続されます。

B の固定 y の場合、x ∈ A と (x, y) の集合 M_y が接続されます (写像 x ↦ (x, y) の A から G への変換は連続です)。 e ∈ M_y なので、y ∈ B を持つ M_y の和集合 R が接続されます。しかし、(A, B) は R によって生成された G の部分群、よって命題です。

### 2. リー群の交換子

#### 命題 3 {#lie-iii-s9-prop-3 .statement tag=0AIM}

G を有限次元リー群、G の H_1 と H_2 部分群とします。h_1、h_2、h をそれぞれ H_1 H_2 と (H_1, H_2) に対する e でのリー接線部分代数とします。次に、[h_1, h_2] ⊂ h となります。

a ∈ h_1、b ∈ h_2 とします。 K には 0 の開近傍 I が存在し、G には次のような I の解析写像 f_1、f_2 が存在します。

$$
f_1(0) = f_2(0) = e, \quad f_1(I) \subset H_1, \quad f_2(I) \subset H_2,
$$
$$
(T_0 f_1)1 = a, \quad (T_0 f_2)1 = b.
$$

私たちは書きます
$$
f(\lambda, \mu) = (f_1(\lambda), f_2(\mu)) \in (H_1, H_2) \quad \text{for } \lambda, \mu \text{ in I}.
$$

写像 e から 0 になるチャートを使用して、G の e のオープン近傍と K' のオープン部分集合を同一視する表します。 すると、L(G) が K' と同定されます。 § 5, no. 2, 命題 1 により、f(\lambda, \mu) を原点に関する積分系列として展開すると、
$$
f(\lambda, \mu) = \lambda \mu [a, b] + \sum_{i \geq 1, j \geq 1, i+j \geq 2} \lambda^i \mu^j a_{ij}
$$
ここで、a_{ij} ∈ K' (f(\lambda, \mu) の展開における \lambda^i と \mu^j の項は、f(\lambda, 0) = f(0, \mu) = 0 であるため、零になります)。 I の \mu を修正します。 \lambda を 0 に近づけると、次のことがわかります。
$$
\mu [a, b] + \sum_{j \geq 2} \mu^j a_{1j} \in h.
$$
これはすべての \mu ∈ I に当てはまるので、 [a, b] ∈ h になります。

#### 注意 {#lie-iii-s9-n2-rem-1 .statement tag=0AIN}

H_1 と H_2 が G の Lie 部分群でつながっているとしても、[h_1, h_2] によって生成される L(G) の Lie 部分代数は一般に h とは異なります。

#### 命題 4 {#lie-iii-s9-prop-4 .statement tag=0AIO}

G を有限次元の実数または複素数リー群とします。 A、B、C を [L(A), L(C)] ⊂ L(C) となるような G の整数部分群とします。
$$
[L(B), L(C)] \subset L(C).
$$
[L(A), L(B)] ⊂ L(C) の場合、(A, B) ⊂ C。 [L(A), L(B)] = L(C) の場合、(A, B) = C となります。

$[L(A), L(B)] \subset L(C)$ と仮定します。 和 $L(A) + L(B) + L(C)$ は $L(G)$ の嘘部分代数です。 $G$ とリー代数 $L(A) + L(B) + L(C)$ の積分部分群を考慮すると、問題は次の場合に帰着します。

$$
L(A) + L(B) + L(C) = L(G)
$$

と$G$が接続されています。すると$L(C)$は$L(G)$の理想となります。まず、$G$ が単純に接続されているとします。次に、$C$ は、$G$ (§ 6, no. 6、命題 14) の通常の嘘部分群です。 $\phi$ を $G$ から $G/C$ への標準的な射とします。それから

$$
[L(\phi)(L(A)), L(\phi)(L(B))] = \{0\}
$$

したがって、$\phi(A)$ と $\phi(B)$ はハウスドルフ公式で通勤します。したがって、$(A, B) \subset C$。一般的な場合、$G'$ を $G$ の普遍的なカバーとし、$A', B', C'$ を $L(A') = L(A), L(B') = L(B), L(C') = L(C)$ となるような $G'$ の積分部分群とします。すると、$(A', B') \subset C'$と$A, B, C$は$G$、よって$(A, B) \subset C$の$A', B', C'$の標準像になります。一方、$(A, B)$ は、$G$ (§ 6, no. 2、系 ～ 命題 4) の積分部分群の基礎となる集合とそのリー代数含む $[L(A), L(B)]$ (命題3)。もし

$$
[L(A), L(B)] = L(C),
$$

次に$(A, B) \supset C$、よって $(A, B) = C$。

#### 系 {#lie-iii-s9-n2-cor-1 .statement tag=0AIP}

*G を、リー代数 g と接続された有限次元実数または複素数リー群とします。 部分群 $D^iG$ (それぞれ $C^iG$) は、 部分群とリー代数 $D^i\mathfrak{g}$ (それぞれ $C^i\mathfrak{g}$) と一体です。 G を単純に接続すると、Lie 部分群になります。

最初の主張は、$i$ の帰納法による命題 4 に続きます。 2 番目は最初と § 6, no. 6、命題 14 に続きます。

#### 命題 5 {#lie-iii-s9-prop-5 .statement tag=0AIQ}

*G を有限次元の実数または複素数リー群、A を G の積分部分群とすると、$DA = DA$ となります。特に、A は $\overline{A}$ の通常の部分群であり、$\overline{A}/A$ は可換です。*

$a = L(A)$ にしましょう。 $G_1$ を $g \in G$ の集合とすると、次のようになります。

$$(\mathrm{Ad}\, g)x \equiv x \pmod{\mathscr{D}a} \quad \text{for all } x \in a.$$

すると、$G_1$は$G$のクローズド部分群になります。 $y \in a$ の場合、$\exp y \in G_1$、§ 6, no. 4 により、系 3 (ii) から命題 10 になります。したがって、$G_1$ 含む $A$、したがって $\overline{A}$ となります。したがって、$g \in \overline{A}$ の場合、$L(\mathrm{Int}\, g)$ は $a$ を安定させ、したがって $\mathrm{Int}\, g$ は $A$ を安定させます。より正確には、$L(\mathrm{Int}\, g)$ 定義するは $a/\mathscr{D}a$ の同一性自己同型、したがって $\mathrm{Int}\, g$ 定義するは $A/DA$ の同一性自己同型です。これは、$(\overline{A}, A) \subset DA$ であることを証明します。 $G$ の実リー群構造では、$\overline{A}$ は嘘部分群 (§ 8, no. 2, 定理 2) です。 $b$をそのリー代数とします。 $G_2$ を $g \in G$ の集合とすると、次のようになります。

$$(\mathrm{Ad}\, g)x \equiv x \pmod{\mathscr{D}a} \quad \text{for all } x \in b.$$

上記により、$G_2 \supseteq A$、したがって$G_2 \supseteq \overline{A}$となります。したがって、$g \in \overline{A}$ では、Int $g$ は DA を安定にし、定義するは $\overline{A}/DA$ の恒等式自己同型を残します。したがって$DA \supseteq D\overline{A}$です。

#### 命題 6 {#lie-iii-s9-prop-6 .statement tag=0AIR}

*K が超計量であると仮定します。 G を有限次元リー群とします。 A、B、Cを、$[L(A), L(C)] \subset L(C)$、$[L(B), L(C)] \subset L(C)$となるようなGのLie部分群とする。 $[L(A), L(B)] \subset L(C)$ の場合、$(A', B') \subset C$ となるような A、B の開いた部分群 A'、B' が存在します。 $[L(A), L(B)] \subset L(C)$ の場合、$(A', B') = C'$ となるような A、B、C のうち、開いている部分群 A'、B'、C' が存在します。*

$[L(A), L(B)] \subset L(C)$ だとします。 命題 4 の証明のように、$L(C)$ が $L(G)$ の理想である場合には、問題簡約するとなります。そして、オープン部分群による置き換えることGにより、GでCが正常な場合($§ 7$,no. 1,命題2)に簡約するとなります。 $\phi$ を $G/C$ に対する G の正規の射とします。それから
$$
[L(\phi)(L(A)), L(\phi)(L(B))] = \{0\}.
$$
ハウスドルフ公式のそばには、$\phi(A')$ と $\phi(B')$ が通勤する、よって $(A', B') \subset C$ のように、A、B の開いた部分群 A'、B' が存在します。さらに次のように仮定します
$$
[L(A), L(B)] = L(C).
$$
命題 3 までに、ライ部分代数は $e$ 含む $L(C)$ で $(A', B')$ に接します。したがって、$(A', B')$ 含むは、リー代数 $L(C)$ を伴う G の嘘部分群の胚芽です。したがって、$(A', B')$はCのオープン部分群です。

#### 系 {#lie-iii-s9-n2-cor-2 .statement tag=0AIS}

*K が超計量であると仮定します。 G をリー代数 g を持つ有限次元リー群とします。 G の開いた部分群 $G_0$ が存在し、すべての $i$ に対して、$D^iG_0$ (それぞれ $C^iG_0$) は、リー代数 $\mathscr{D}^ig$ (それぞれ $\mathscr{C}^ig$) と G の嘘部分群になります。

(a) 命題 3 を帰納的に適用し、G のすべてのオープン部分群 $G_1$ とすべての $i$、$D^iG_1$ 含むに対して、リー代数 $\mathscr{D}^ig$ と G の部分群ジャームを嘘をつく。

(b) $G'$ を G のオープン部分群とし、$i \leq n$ に対して、$D^iG'$ はリー代数 $\mathscr{D}^ig$ を伴う G の嘘部分群とします。 命題 6までに、$D^nG'$のオープン部分群 $H_1, H_2$が存在し、$(H_1, H_2)$はリー代数 $\mathscr{D}^{n+1}g$との嘘部分群になります。 $G''$ を、$D^nG'' \subset H_1 \cap H_2$ に対して十分小さい $G'$ の開いた部分群とします。続いて$D^{n+1}G'' \subset (H_1, H_2)$。 関係
$$
D^0G'' \subset D^0G', D^1G'' \subset D^1G', \ldots, D^nG'' \subset D^nG', D^{n+1}G'' \subset (H_1, H_2)
$$
(a) を使用して、$D^iG''$ は、$i \leq n + 1$ に対して、リー代数 $\mathscr{D}^ig$ を伴う G の嘘部分群であることを証明します。

(c) $\mathscr{D}^pg = \mathscr{D}^{p+1}g = \cdots$ となるような整数 $p$ が存在します。上記により、$D^iG_0$ が $i \leq p$ に対して、リー代数 $\mathscr{D}^ig$ と G の嘘部分群となるような G の開いた部分群 $G_0$ が存在します。しかし、(a) により、$i > p$ の $D^pG_0 \supset D^iG_0$ 以来、$i > p$ にも同じ主張が当てはまります。

(d) $C^i$ についても同様の議論である。

### 3. 集中化者

群の 2 つの元 $x, y$ が、$(x, y) = e$、$(\mathrm{Int}\, x)y = y$、または $(\mathrm{Int}\, y)x = x$ の場合、置換可能と呼ばれることを思い出してください。そして、リー代数の 2 つの元 $a, b$ が、$[a, b] = 0$、$(\mathrm{ad}\, a).b = 0$、または $(\mathrm{ad}\, b).a = 0$ の場合、置換可能と呼ばれます。 $G$ をリー群、$x \in G$、$a \in \mathbf{L}(G)$ とします。 $x$ と $a$ は、$(\mathrm{Ad}\, x).a = a$ の場合、つまり $\mathbf{T}(G)$ の $xa = ax$ の場合、置換可能と呼ばれます。

$G$をリー群、$g$をそのリー代数、$A$を$G$の部分集合、$a$を$g$の部分集合とします。 $Z_G(A)$ (それぞれ $Z_G(a)$) は、$A$ (それぞれ $a$) のすべての元と置換可能な $G$ の元の集合を表すものとします。 $G$の閉店部分群です。 $\mathfrak{z}_g(A)$ (それぞれ $\mathfrak{z}_g(a)$) は、$A$ (それぞれ $a$) のすべての元と置換可能な $g$ の元の集合を表すものとします。 $g$の閉じた嘘部分代数です。

#### 命題 7 {#lie-iii-s9-prop-7 .statement tag=0AIT}

*$G$を有限次元のリー群、$g$をそのリー代数、$a$を$g$の有限次元部分集合とします。すると、$Z_G(a)$ は $G$ とリー代数 $\mathfrak{z}_g(a)$ の嘘部分群です。

これは、§ 3、命題 44、系 2 から命題 39 まで続きます。

#### 命題 8 {#lie-iii-s9-prop-8 .statement tag=0AIU}

*$G$を有限次元の実数または複素数リー群、$g$をそのリー代数、$A$を$G$の部分集合とする。すると、$Z_G(A)$ は、$G$ とリー代数 $\mathfrak{z}_g(A)$ の嘘部分群になります。

$A$ が 1 つの点 $a$ で構成されているとします。すると、$Z_G(A)$は$\mathrm{Int}\, a$の固定点の集合になります。したがって、$Z_G(A)$は$G$の嘘部分群であり、$\mathbf{L}(Z_G(A))$は$\mathrm{Ad}\, a$の固定点の集合、つまり$\mathfrak{z}_g(A)$(§ 3, no. 8, 系 1から命題 29）。一般的なケースは、§ 6, no. 2、系 3 ～ 命題 1 によって続きます。

#### 命題 9 {#lie-iii-s9-prop-9 .statement tag=0AIV}

*$G$を有限次元の実数または複素数リー群、$g$をそのリー代数、$A$を$G$と$a = \mathbf{L}(A)$の積分部分群とする。次に、$Z_G(A) = Z_G(a)$、$\mathfrak{z}_g(A) = \mathfrak{z}_g(a)$、$Z_G(A)$ は、$G$ とリー代数 $\mathfrak{z}_g(a)$ の嘘部分群です。

$x \in G$ にしましょう。それから
$$
x \in Z_G(A) \iff A \subset Z_G(\{x\}) \\
\iff a \subset \mathbf{L}(Z_G(\{x\})) \quad (\text{§ 6, Corollary 2 to Proposition 3}) \\
\iff a \subset \mathfrak{z}_g(\{x\}) \quad (\text{Proposition 8}) \\
\iff x \in Z_G(a)
$$
したがって $Z_G(A) = Z_G(a)$ です。 $u \in g$ にしましょう。それから
$$
u \in \mathfrak{z}_g(A) \iff A \subset Z_G(\{u\}) \\
\iff a \subset \mathbf{L}(Z_G(\{u\})) \quad (\text{§ 6, Corollary 2 to Proposition 3}) \\
\iff a \subset \mathfrak{z}_g(\{u\}) \quad (\text{Proposition 7}) \\
\iff u \in \mathfrak{z}_g(a)
$$
したがって $\mathfrak{z}_g(A) = \mathfrak{z}_g(a)$ です。 最後の主張は、命題 7 または命題 8 から続きます。

### 4. ノーマライザー

Gをリー群、$g$をそのリー代数、AをGの部分集合、$g$の$a$部分集合とします。この切断では、$N_G(A)$は$g \in G$の集合を表し、$gAg^{-1} = A$となります。 Aが閉じていれば閉じているGの部分群です。 $n_g(a)$ は、$[x, a] \subset a$ (cf. 章 I, § 1, no. 4) のように、$x \in g$ の集合を表します。 $a$が休みの場合は$g$の部分代数です。 $N_g(a)$ は、$gag^{-1} = a$ のように、$g \in G$ の集合を表します。

#### 命題 10 {#lie-iii-s9-prop-10 .statement tag=0AIW}

*G を有限次元のリー群、g をそのリー代数、g のベクトル部分空間とします。次に、$N_G(a)$ は、リー代数 $n_g(a)$ を含む G の嘘部分群です。* これは、§ 3、命題 44、系 1 から命題 39 に続きます。

#### 命題 11 {#lie-iii-s9-prop-11 .statement tag=0AIX}

*G を有限次元の実数または複素数リー群、g をそのリー代数、A を G と $a = L(A)$ の積分部分群とします。次に、$N_G(A) = N_G(a)$ と $N_G(A)$ は、リー代数 $n_g(a)$ を伴う G 含む $\overline{A}$ の嘘部分群です。* 等式 $N_G(A) = N_G(a)$ は、§ 6, no. 2、系 2 から続きます。 命題 3. 命題 10 までに、$N_G(A)$ は、リー代数 $n_g(a)$ を持つ G の嘘部分群になります。したがって、$N_G(A)$は閉まっています。 $N_G(A) \supset A$、$N_G(A) \supset \overline{A}$ として。

#### 系 {#lie-iii-s9-n4-cor-1 .statement tag=0AIY}

* $a = n_g(a)$ の場合、A は G の嘘部分群であり、$N_G(A)$ の同一性成分です。* この同一性成分は、リー代数 $n_g(a)$ (命題 11) を持つ嘘部分群であり、したがって、§ 6, no. 2, 定理 2 (i) により A に等しくなります。

### 5. 無能リー群

#### 命題 12 {#lie-iii-s9-prop-12 .statement tag=0AIZ}

*G を有限次元リー群とします。 $L(G)$ がゼロポテントであるためには、G がゼロゼロポテント部分群を持っていることが必要かつ十分です。* G がゼロポテントオープン部分群 $G_0$ を持っているとします。 命題 4 と 6、no. 2、$C^iL(G_0) = \{0\}$ の結果から、十分大きい $i$ になります。したがって、$L(G_0) = L(G)$ は無能です。

$L(G)$ が零であると仮定します。 $K = \mathbf{R}$ または $\mathbf{C}$ の場合、G の同一性成分 $G_0$ は、系 ～ 命題 4、no. 2、および $G_0$ によってゼロポテントになります。K が超計量の場合、系 ～ 命題 6, no. 2 は、$C^iG_1 \cap V = \{e\}$ となる G の e の開いた部分群 $G_1$、整数 $i > 0$ および近傍 V が存在することを証明します。次に、$G_0$ が $G_1$、$C^iG_0 \subset V$ の十分に小さい部分群である場合、$C^iG_0 = \{e\}$ と $G_0$ はゼロポテントです。

$g$をべき零リー代数とします。 ハウスドルフ系列 $H(X, Y)$ 対応するから $g$ には、非ゼロ項の有限数しかなく、(章 II, § 6, no. 5, *注意 3*) の法則がわかっています。 合成 $(x, y) \mapsto H(x, y)$ 定義する群構造 $g$。 さらに、$g$ が完全で正規であると仮定します。 明らかに、法則 H は連続多項式 (*微分可能かつ解析的多様体*、R、付録) です。 したがって、$g$ は、法則 H とともに、リー群 G となり、$g$ に *関連付けられている* と言われます。 § 4, no. 2、補題 2 と 3、$L(G) = g$ によって。 $g$ の $\phi$ から $G$ への恒等マッピングは、すべての $x \in g, \lambda \in K, \lambda' \in K$ に対して $\phi(\lambda x)\phi(\lambda'x) = \phi((\lambda + \lambda')x)$ となるような $G$ の指数マッピングです。 トポロジー 補充を認める $g$ のすべての嘘部分代数 $\mathfrak{h}$ は、$G$ と $L(H) = \mathfrak{h}$ の嘘部分群 $H$ です。

#### 命題 13 {#lie-iii-s9-prop-13 .statement tag=0AJ0}

* $G$ を、$\mathbf{R}$ または $\mathbf{C}$ に対する有限次元の単純接続されたゼロポテントリー群とします。

(i) $\exp_G$ は、$L(G)$ から $G$ に関連付けられているリー群の同型です。

(ii) *$G$ のすべての積分部分群は、$G$ の単純接続された嘘部分群です。*

$g = L(G)$ を無能 (命題 12) とします。 同じリー代数を持つ$\mathbf{R}$または$\mathbf{C}$を介して単純に接続された2つのリー群は同型であるため($§ 6$, no. 3, 定理 3 (ii))、$G$が群と関連付けられている場合、命題を証明するだけで十分です。 $g$。 次に、(i) と (ii) は、言われたことから続きます前に命題。

#### 命題 14 {#lie-iii-s9-prop-14 .statement tag=0AJ1}

*$G$ を、$\mathbf{R}$ または $\mathbf{C}$ 上で接続された有限次元のリー群とします。

(i) *$G$ が零能である場合、$\exp_G$ はエタールかつ全射です。*

(ii) *$K = \mathbf{C}$ と $\exp_G$ がエタールの場合、$G$ は零能です。*

$G'$ を $G$ の普遍的なカバー 空間とします。 $\phi$ を $G'$ から $G$ への正規の射とします。次に、$\exp_G = \phi \circ \exp_{G'}$ ($§ 6$、no. 4、命題 10) となり、したがって (i) は命題 13 (i) から続きます。

$K = \mathbf{C}$ と $\exp$ がエタールの場合、すべての $x \in L(G)$ と $x$ には、固有値所属 ～ $2i\pi(\mathbf{Z} - \{0\})$ ($§ 6$、no. 4、系 ～ 命題) はありません。 12)。 適用これを $\lambda x$ にすると、$\lambda$ は $\mathbf{C}$ まで変化します。その結果、$\mathrm{ad}\, x$ のすべての固有値は零となり、したがって $\mathrm{ad}\, x$ はゼロポテントになります。したがって、$L(G)$ は無能 (章 I、$§ 4$、系 1 ～ 定理 1) であり、したがって $G$ は無能 (命題 12) です。

#### 命題 15 {#lie-iii-s9-prop-15 .statement tag=0AJ2}

*$G$ を、$\mathbf{R}$ または $\mathbf{C}$ 上の有限次元連結冪能リー群とし、$A$ を $G$ の整数部分群とします。次に、$Z_G(A)$ は、$G$ とリー代数 $\mathfrak{z}_G(L(A))$ が接続された嘘部分群です。

no. 3 の命題 9 までに、$Z_G(A)$ が接続されていることを証明するのに十分です。 $g \in Z_G(A)$ にしましょう。 $g = \exp x$ (命題 14) となるような $x \in L(G)$ が存在します。次に、$\mathrm{Ad}\, g|L(A) = 1$ (no. 3、命題 9)、したがってすべての $n \in \mathbf{Z}$ に対して$\mathrm{Ad}\, g^n|L(A) = 1$、したがってすべての $n \in \mathbf{Z}$ に対して$\exp(\mathrm{ad}\, nx)|L(A) = 1$ となります。 写像として

$$
\lambda \mapsto \exp(\mathrm{ad}\, \lambda x)|L(A)
$$

$K$ の $\mathscr{L}(L(A), L(G))$ への変換は多項式で、すべての $\lambda \in K$ に対して $\exp(\mathrm{ad}\, \lambda x)|L(A) = 1$、つまりすべての $\lambda \in K$ に対して $\exp(\lambda x) \in Z_G(A)$ になります。

#### 命題 16 {#lie-iii-s9-prop-16 .statement tag=0AJ3}

*$G$ を $\mathbf{R}$ または $\mathbf{C}$ 上の有限次元の冪能リー群とし、$A$ を $G$ とは異なる $G$ の積分部分群とする。したがって、$N_G(A)$ は、$A$ とは異なる、$G$ の接続された嘘部分群です。

$N_G(A) \neq A$ (代数、章 I, § 6、系 1 ～ 命題 8)。 no. 4 の命題 11 までに、$N_G(A)$ が接続されていることを証明するだけで済みます。 $g \in N_G(A)$ にしましょう。 $g = \exp x$ (命題 14) となるような $x \in L(G)$ が存在します。 $E$ を $u \in \mathscr{L}(L(G))$ の $\mathscr{L}(L(G))$ からなるのベクトル部分空間とし、$u(L(A)) \subset L(A)$ とします。次に、$\mathrm{Ad}\, g^n \in E$、したがってすべての $n \in \mathbf{Z}$ に対して $\exp(\mathrm{ad}\, nx) \in E$ となります。したがって、すべての $\lambda \in K$ に対して $\exp(\mathrm{ad}\, \lambda x) \in E$、つまりすべての $\lambda \in K$ に対して $\exp(\lambda x) \in N_G(A)$ となります。

#### 命題 17 {#lie-iii-s9-prop-17 .statement tag=0AJ4}

*$g$を、$0 \leq i < n$に対して$g_0 = g, g_n = \{0\}$と$[g, g_i] \subset g_{i+1}$が成り立つような、$g$の理想の$K$と$(g_0, g_1, \ldots, g_n)$減少列上の有限次元べき零リー代数とする。 $a_1, a_2, \ldots, a_p$ を $g$ のベクトル部分空間とし、それぞれの $g_i$ を $a_j$ と合わせた共通部分の直和とします。 $g$ に合成 $H$ のハウスドルフ法則を与えましょう。 $\phi$ を写像* とします

$$
(x_1, x_2, \ldots, x_p) \mapsto x_1 \mathbf{H} x_2 \mathbf{H} \cdots \mathbf{H} x_p
$$

$a_1 \times a_2 \times \cdots \times a_p$ から $g$ に。

(i) $\phi$ は $g$ 上の $a_1 \times a_2 \times \cdots \times a_p$ の全単射です。
(ii) $\phi$ と $\phi^{-1}$ は多項式写像です。
(iii) $(a_1 \times a_2 \times \cdots \times a_p)^2$ の $a_1 \times a_2 \times \cdots \times a_p$ への写像 $(x, y) \mapsto \phi^{-1}(\phi(x) \cdot \phi(y)^{-1})$ は多項式です。

命題は $\dim g = 0$ にとって明らかです。 次元 $< \dim g$ に対して $\dim g > 0$ と命題が確立されたとします。 $g_{n-1} \neq \{0\}$ と $g_{n-1}$ は、$g$ の非ゼロの中心イデアルであると想定できます。 $h = g_{n-1} \cap a_j \neq \{0\}$ となるような添字 $j$ が存在します。 $g' = g/h$、$\theta$ を、$g$ の$g'$、$g'_i = \theta(g_i)$、$a'_i = \theta(a_i)$ に対する正規の射とします。すると、$(g'_0, g'_1, \ldots, g'_n)$ は $g'$ の理想の減少列であり、$g'_0 = g', g'_n = \{0\}$ は、

$$
[g', g'_i] \subset g'_{i+1}
$$

$0 \leq i < n$ の場合、各 $g'_i$ は $a'_j$ を含むその共通部分の直和です。 $\phi'$ を写像とします

$$
(x'_1, x'_2, \ldots, x'_p) \mapsto x'_1 \mathbf{H} x'_2 \mathbf{H} \cdots \mathbf{H} x'_p
$$

$a'_1 \times a'_2 \times \cdots \times a'_p$ を $g'$ に。 帰納法の仮定により、$\phi'$ は全単射、$\phi', {\phi'}^{-1}$ は多項式写像になります。

$x \in g$ にしましょう。私たちは書きます

(1)
$$
{\phi'}^{-1}(\theta(x)) = (x'_1(x), x'_2(x), \ldots, x'_p(x)).
$$
それから
(2)
$$
\theta(x) = x'_1(x) \mathbf{H} x'_2(x) \mathbf{H} \cdots \mathbf{H} x'_p(x).
$$
$h_1$を$g$の$h$、$a_k$の和を$k \neq j$と$a_j$の$h$の補充を補うベクトル部分空間とします。 $h_1$ 上には $\theta \circ \eta = \mathrm{Id}_{g'}$ となる $g'$ の全単射 $\eta$ が存在します。 $x \in g$ については、次のように書きます。
(3)
$$
\zeta(x) = \eta(x'_1(x)) \mathbf{H} \eta(x'_2(x)) \mathbf{H} \cdots \mathbf{H} \eta(x'_p(x)) \in g.
$$
(4)
$$
y(x) = \zeta(x)^{-1} \mathbf{H} x = (-\zeta(x)) \cdot x.
$$

(2) と (3) により、$\theta(\zeta(x)) = \theta(x)$、したがって $y(x) \in \mathfrak{h}$ になります。最後に書きます
$$
(5) \quad \psi(x) = (\eta(x_1'(x)), \ldots, \eta(x_p'(x)) + y(x), \ldots, \eta(x_p'(x))) \in a_1 \times \cdots \times a_p.
$$
$y(x)$は$\mathfrak{g}$の中心となるため、
$$
\begin{align*}
\phi(\psi(x)) &= \eta(x_1'(x)) \mathbin{\mathbf{H}} \cdots \mathbin{\mathbf{H}} \eta(x_p'(x)) \mathbin{\mathbf{H}} \cdots \mathbin{\mathbf{H}} \eta(x_p'(x)) \mathbin{\mathbf{H}} y(x) \\
&= \zeta(x) \mathbin{\mathbf{H}} y(x) & \text{by (3)} \\
&= x & \text{by (4).}
\end{align*}
$$
したがって$\phi \circ \psi = \mathrm{Id}_g$です。次に、$(x_1, x_2, \ldots, x_p) \in a_1 \times a_2 \times \cdots \times a_p$ を$x = \phi(x_1, x_2, \ldots, x_p) = x_1 \mathbin{\mathbf{H}} x_2 \mathbin{\mathbf{H}} \cdots \mathbin{\mathbf{H}} x_p$ と書きます。それから
$$
\theta(x) = \theta(x_1) \mathbin{\mathbf{H}} \theta(x_2) \mathbin{\mathbf{H}} \cdots \mathbin{\mathbf{H}} \theta(x_p),
$$
したがって、$1 \leq i \leq p$の場合は$x_i'(x) = \theta(x_i)$、したがって
$$
\begin{align*}
\zeta(x) &= x_1 \mathbin{\mathbf{H}} x_2 \mathbin{\mathbf{H}} \cdots \mathbin{\mathbf{H}} (\eta \theta(x_j)) \mathbin{\mathbf{H}} \cdots \mathbin{\mathbf{H}} x_p \\
y(x) &= x_j - \eta \theta(x_j).
\end{align*}
$$
次に(5)までに
$$
\psi(x) = (x_1, \ldots, \eta \theta(x_j) + x_j - \eta \theta(x_j), \ldots, x_p) = (x_1, x_2, \ldots, x_p).
$$
したがって$\psi \circ \phi = \mathrm{Id}_{a_1 \times \ldots \times a_p}$です。これは(i)を証明します。ハウスドルフ法則が多項式であるため、$\phi$ も多項式です。 帰納法の仮定により、${\phi'}^{-1}$ は多項式になります。 公式 (1)、写像 $x_j'$ は多項式であるため、$\zeta$ は多項式 (公式 (3))、$y$ は多項式 (公式 (4))、$\psi$ は多項式です(公式(5))。これは(ii)を証明します。 主張 (iii) は、(i) と (ii) およびハウスドルフ法則が多項式であるという事実から導き出されます。

ゼロポテントリー群の **例。** $G$ を $\mathbf{GL}(n, K)$ の厳密な下三角部分群とします。それは$\mathbf{GL}(n, K)$の嘘部分群であり、$L(G) \subset \mathfrak{gl}(n, K)$は対角零（§ 3, no. 10、命題36）を持つ下三角行列のリー代数です。 章 II, § 4, no. 6 までに、*注意*、$G$ は無能です。今後、$K = \mathbf{R}$ または $\mathbf{C}$ と仮定します。 $G$は$K^{n(n-1)/2}$と同相なので、$G$は単純に接続されます。 $L(G)$ から $G$ への指数写像は、ちょうど写像です
$$
u \mapsto \exp u = \sum_{k \geq 0} \frac{u^k}{k!} = \sum_{k=0}^{n-1} \frac{u^k}{k!}
$$
(§ 6, no. 4、*例*)。 命題 13 までに、指数関数は多様体 $L(G)$ の同型から多様体 $G$ になります。 命題 17 の § 6, no. 9 は逆全単射 $\log$ になります。 $K^n$ ノルムを与えます。 *スペクトル理論*によると、章 I, § 4, no. 9、$g \in G$ と $\|g - 1\| < 1$、
$$
\log g = \sum_{k \geq 1} \frac{(-1)^{k-1}}{k} (g - 1)^k
$$

つまり
$$
\log g = \sum_{k=1}^{n-1} \frac{(-1)^{k-1}}{k} (g-1)^k.
$$
しかし、(6) の 2 つの辺は、$g \in G$ に対する $g$ の解析的な写像であるため、すべての $g \in G$ について等しいです。

#### 命題 18 {#lie-iii-s9-prop-18 .statement tag=0AJ5}

※kを可換体とします。 V 有限次元のベクトル空間 > 0 は k および $\mathbf{GL}(V)$ の G 部分群を超え、その元は単能性です*。
  (i) *G 内のすべての g に対して gv = v となるような、V の非ゼロ元 v が存在します。*
  (ii) *G のすべての g \ について、B に関する g の行列が下三角であり、そのすべての対角線元が 1 に等しいような V の基底 B が存在します。*
  (iii) *群 G は無能です。*
    (a) まず、k が代数的に閉じており、G の恒等式表現が単純であると仮定します。 a、b を G とする。 それから
    $$
    \operatorname{Tr}(a(b-1)) = \operatorname{Tr}(ab-1) - \operatorname{Tr}(a-1) = 0 - 0 = 0
    $$
    $ab - 1$ と $a - 1$ は無能です。 G によって生成された $\mathscr{L}(V)$ のベクトル部分空間は $\mathscr{L}(V)$ (*代数*、章 VIII, § 4、系 1 ～ 命題 2)、すべての $u \in \mathscr{L}(V)$ に対して $\operatorname{Tr}(u(b-1)) = 0$ であるため、 $b = 1$。 従って、$G = \{1\}$。
    (b) ここで一般的なケースに移ります。 $\bar{k}$ を k の代数閉包、$\bar{V} = V \otimes_k \bar{k}$ と $a \in G$ の $a \otimes 1$ の $\bar{G} \subset \mathbf{GL}(\bar{V})$ 集合とします。 W (それぞれ $W'$) を、G (それぞれ $\bar{G}$) のもとで不変な V (それぞれ $\bar{V}$) の要素の集合とする。 次に、$W = \bigcap_{g \in G} \operatorname{Ker}(g-1)$と$W' = \bigcap_{g \in G} \operatorname{Ker}(g-1) \otimes 1$に対して$W' = W \otimes_k \bar{k}$。 $V_1$ が、$\bar{G}$ の下で安定している $\bar{V}$ の非ゼロベクトル部分空間の集合内の最小要素を表す場合、証明の部分 (a) により $V_1 \subset W'$ となります。従って $W \neq \{0\}$ となり、(i) が証明されます。
    (c) $\dim V$ の帰納により、(i) から、$V_n = V$ と G から標準的に導出された$V_i/V_{i-1}$ の自己同型群は、すべての $i$ について $\{1\}$ に減少するような、G のもとで安定なV のベクトル部分空間の増加系列 $(V_1, V_2, \ldots, V_n)$ が存在することがわかります（ $r \leq 0$の場合は$V_r = \{0\}$）。 これは、最初に (ii) を意味し、その結果として (iii) (章 II, § 4, no. 6, *注意*) を意味します。

#### 系 1 {#lie-iii-s9-prop-18-cor-1 .statement tag=0AJ6}

*G を有限次元の接続された実数または複素数リー群とします。 G が nilpotent であるためには、Ad G のすべての元が nilpotent であることが必要かつ十分です。*

Ad G のすべての元が単能性である場合、Ad G はゼロ能性 (命題 18) であるため、Ad G の中心の拡大である G はゼロ能性です。 G が無能である場合、$L(G)$ は無能であるため、$\operatorname{ad} x$ はすべての $x \in L(G)$ に対して無能であり、したがって $\operatorname{Ad}(\exp x) = \exp \operatorname{ad} x$ は単能性です。しかし、G のすべての元は、一部の $x \in L(G)$ (命題 14) では、形 $\exp x$ になります。

#### 系 2 {#lie-iii-s9-prop-18-cor-2 .statement tag=0AJ7}

*単能性要素で構成される $\mathbf{GL}(n, K)$ のすべての解析部分群は、単純に接続されたリー部分群です。*

これは、命題 13 (ii) および 18 (ii) と、下側の厳密な三角形群が単純に接続されているという事実から導き出されます。

### 6. 解決可能リー群

#### 命題 19 {#lie-iii-s9-prop-19 .statement tag=0AJ8}

*$G$を有限次元のリー群とします。 $L(G)$ が解決可能であるためには、$G$ が解決可能なオープン部分群を持っていることが必要かつ十分です。*

証明は、no. 5 の命題 12 に類似しています。

#### 命題 20 {#lie-iii-s9-prop-20 .statement tag=0AJ9}

*$G$ を、$\mathbf{R}$ または $\mathbf{C}$ および $g = L(G)$ 上の有限次元 $n$ の単純に接続された可解なリー群とします。 $(g_n, g_{n-1}, \ldots, g_0)$ を次元 $n, n-1, \ldots, 0$ の $g$ の部分代数の数列とし、$g_{i-1}$ が $i = n, n-1, \ldots, 1.\dagger$ に対する $g_i$ の理想となるようにします。 $G_i$ を $G$ の積分部分群とします。 対応するから$g_i$まで。 $x_i$ を所属 ～ $g_{i-1}$ ではなく、$g_i$ のベクトルとします。 $\phi_i$ を写像* とします

$$
(\lambda_1, \lambda_2, \ldots, \lambda_i) \mapsto (\exp \lambda_1 x_1)(\exp \lambda_2 x_2) \cdots (\exp \lambda_i x_i)
$$

*$K^i$ を $G$ に。すると、$\phi_n$ は分析多様体の同型であり、すべての $i$ については $\phi_i(K^i) = G_i$ になります。

$n = 0$ 命題の場合は明らかです。 $n$の帰納法までに議論します。 $H$ を $L(H) = Kx_n$ となるような $G$ の積分部分群とします。 § 6, no. 6、系 1 から命題 14、$H$ と $G_{n-1}$ は単純に接続されています $G$ の部分群を嘘にし、リー群と同様に、$G$ は半直接積です$H$までに$G_{n-1}$まで。したがって、$\lambda \mapsto \exp(\lambda x_n)$ は、$K$ の同型から $H$ になり、帰納法の仮定写像になります。

$$
(\lambda_1, \lambda_2, \ldots, \lambda_{n-1}) \mapsto (\exp \lambda_1 x_1)(\exp \lambda_2 x_2) \cdots (\exp \lambda_{n-1} x_{n-1})
$$

は、分析的多様体 $K^{n-1}$ の分析的多様体 $G_{n-1}$ の同型で、$i = 1, 2, \ldots, n-1$ に対して写像 $K^i \times \{0\}$ から $G_i$ になります。したがって命題です。

#### 命題 21 {#lie-iii-s9-prop-21 .statement tag=0AJA}

*$G$ を、$\mathbf{R}$ または $\mathbf{C}$ 上の単純に接続された有限次元の可解なリー群と、$M$ を $G$ の積分部分群とします。すると、$M$は$G$の嘘部分群であり、単純に接続されています*。

命題 20 の記法 $n, g, g_i, x_i, \phi$ を引き続き使用しますが、$x_i$ に次の補足的な条件を課します。$i_p > i_{p-1} > \cdots > i_1$ を整数 $i$ として、$L(M) \cap g_i \neq L(M) \cap g_{i-1}$ とします。それから私たちは取る

$$
x_{i_k} \in L(M) \cap g_{i_k}
$$

\dagger このような数列は、章 I, § 5、命題 2 によって存在します。

$k = 1, 2, \ldots, p$の場合。 $n$ の帰納法により、$(x_{i_p}, x_{i_{p-1}}, \ldots, x_{i_1})$ が $L(M)$ の基底であることが簡単にわかります。 $N$ を、$L(N)$ の $L(M)$ への同型写像 $h$ が存在するような単純結合リー群とする。 しましょう
$$
y_p = h^{-1}(x_{i_p}), \ldots, y_1 = h^{-1}(x_{i_1}).
$$
命題 20、写像までに
$$
(\lambda_1, \lambda_2, \ldots, \lambda_p) \mapsto (\exp \lambda_1 y_1)(\exp \lambda_2 y_2) \cdots (\exp \lambda_p y_p)
$$
多様体 $K^p$ の多様体 $N$ の同型です。 $h = L(\tau)$ と $\tau(N) = M$ となるような $N$ から $G$ へのリー群射$\tau$ が存在します (§ 6, no. 2、命題 1 の系 1)。 したがって、$M$ は形の $G$ の元の集合です
$$
\tau((\exp \lambda_1 y_1) \cdots (\exp \lambda_p y_p)) = \exp(\lambda_1 L(\tau)y_1) \cdots \exp(\lambda_p L(\tau)y_p)
= \exp(\lambda_1 x_{i_1}) \cdots \exp(\lambda_p x_{i_p}).
$$
したがって、$M = \phi(T)$ ここで、$T$ は $K^n$ のベクトル部分空間です。

#### 命題 22 {#lie-iii-s9-prop-22 .statement tag=0AJB}

※$K = \mathbf{R}$または$\mathbf{C}$とします。 $V$ を有限次元ベクトル空間とし、$G$ を $\mathbf{GL}(V)$ の結合された可解な部分群とします。 $G$ の恒等式表現が単純であると仮定します。*
(i) *$K = \mathbf{R}$ の場合、$\dim V \leq 2$ と $G$ は可換です。*
(ii) *$K = \mathbf{C}$の場合は、$\dim V = 1$。*
(i) $K = \mathbf{R}$ と仮定します。この場合、$\mathbf{GL}(V)$ の$G$ の閉包 $H$ は、$\mathbf{GL}(V)$ の解ける連結嘘部分群 (no. 1, 系 2 から命題 1) です。したがって、$L(H)$ は解けます (命題 19)。 $L(G)$ の正体表現は単純です (§ 6, no. 5、系 2 ～ 命題 13)。したがって、$\dim V \leq 2$ と $L(G)$ は可換です (章 I, § 5、系 1 と 4 から定理 1)。したがって、$G$ は可換です。
(ii) $K = \mathbf{C}$ と仮定します。 $W$ を、$G$ で安定している $V$ の非ゼロ実数ベクトル部分空間のうちの最小値元とします。 $W$ によって生成された$V$ の複素数ベクトル部分空間は、$G$ の恒等式表現が単純であるため、$V$ に等しくなります。 (i) により、$G|W$ は可換です。したがって、$G$ は可換です。したがって、$G$ のすべての元はホモテティー (*代数*、章 VIII, § 4、系 1 ～ 命題 2)、つまり $\dim V = 1$ になります。

#### 系 {#lie-iii-s9-n6-cor-1 .statement tag=0AJC}

*$V$ を有限次元 $> 0$ の複素数ベクトル空間と、$G$ を $\mathbf{GL}(V)$ の連結された可解な部分群とします。*
(i) *すべての $g \in G$ に対して $gv \in Cv$ となるような、$V$ の非ゼロ元 $v$ が存在します。
(ii) *すべての $g \in G$ について、$B$ に関して $g$ の行列が下三角となるような $V$ の基底 $B$ が存在します。
$V_1$ を、$G$ で安定している $V$ の非ゼロベクトル部分空間のうちの最小値元とします。 命題 22 (ii)、$\dim V_1 = 1$ までに。 これは(i)を証明します。 $\dim V$ での帰納により、$i < n$ と $V_n = V$ に対して $\dim V_{i+1}/V_i = 1$ となるような、$G$ の下で安定する$V$ のベクトル部分空間の増加シーケンス $(V_1, V_2, \ldots, V_n)$ が存在することになります。したがって (ii)。

### 7. リー群中根基

#### 命題 23 {#lie-iii-s9-prop-23 .statement tag=0AJD}

*$G$ を有限次元の実数または複素数リー群、$r$ 根基の $L(G)$* (章 I, § 5、定義 2) * および $n$ 最大のの冪能理想とする$L(G)$* (章 I, § 4, no. 4)。 *$R$ (それぞれ $N$) を、$G$ とリー代数 $r$ (それぞれ $n$) の積分部分群とします。この場合、$R$ (それぞれ $N$) は、$G$ の解ける (それぞれゼロポテントな) 嘘部分群であり、$G$ のすべての連続自己同型の下で不変です。 *$G$ の法線部分群に接続されたすべての可解 (それぞれゼロポテント) は、$R$ (それぞれ $N$) に含まれます。

群 $R$ は解けます ($§ 6$、命題 19)。 $K = R$ だとします。 $G'$ を、$G$ の接続された可解法線部分群とします。このとき、$\overline{G'}$ は、$G$ ($§ 8$, no. 2, 定理 2) の接続された可解 (no. 1, 系 2 ～ 命題 1) の通常の嘘部分群です。したがって、$L(\overline{G'})$ は、$L(G)$、よって、$L(\overline{G'}) \subset r$、$\overline{G'} \subset R$ の解決可能な理想です。特に、$\overline{R} \subset R$、したがって$R$は閉じており、したがって$G$の嘘部分群になります。 $K = C$ と仮定します。 $H$ を、$G$ の基礎となる本当の嘘部分群とします。 $r'$ が $L(H)$ の根基である場合、$ir'$ は $L(H)$、よって $r' = ir'$ の解ける理想です。したがって、$r \subset r' \subset r$ となり、上記により、$R$ は $H$ で閉じられ、したがって $G$ で閉じられます。したがって、$R$は$G$の嘘部分群です。 $G$ の接続されたすべての解決可能な法線部分群は、$H$ の接続された可解決法線部分群であるため、$R$ に含まれます。したがって、$K = C$ と $K = R$ について、$R$ は $G$ の最大のが接続された可解正規法線部分群であることを証明しました。したがって、$R$ は、$G$ のすべての連続する自己同型の下で不変です。 $N$ の証明は完全に類似しています。

#### 定義 1 {#lie-iii-s9-def-1 .statement tag=0AJE}

*$G$を有限次元の実数または複素数リー群とします。 $G$ の根基は、$G$ の最大のが解ける法線部分群に接続されています。*

#### 注意 {#lie-iii-s9-n7-rem-1 .statement tag=0AJF}

$G$がつながっていても、$G$の根基に含まれない$G$の解ける法線部分群が存在する可能性があります。

#### 命題 24 {#lie-iii-s9-prop-24 .statement tag=0AJG}

※$K = R$または$C$とします。 $G_1, G_2$ を 2 つの有限次元接続リー群、$R_1$ と $R_2$ の根号、および $G_1$ から $G_2$ への全射射を $\phi$ とします。 次に、$\phi(R_1) = R_2$.*

$§ 3$、no. 8、命題 28、$L(\phi)$ は全射です。したがって、$L(\phi)(L(R_1)) = L(R_2)$ (章 I、$§ 6$、系 3 から命題 2) となります。 $i$を$R_1$の標準単射を$G_1$にします。すると、$\phi \circ i$の像は$R_2$($§ 6$、no. 2、系1から命題1)になります。

#### 命題 25 {#lie-iii-s9-prop-25 .statement tag=0AJH}

※$K = R$または$C$とします。 $G_1, G_2$ を、リー群と $R_1$ と $R_2$ の根基を有限次元で接続するとします。 $G_1 \times G_2$ の根基は $R_1 \times R_2$ です。*

これは、章 I、$§ 5$、命題 4 と続きます。

### 8. 半単純リー 群

#### 命題 26 {#lie-iii-s9-prop-26 .statement tag=0AJI}

G を有限次元の接続された実数または複素数リー群とします。次の条件は同等です。
(i) $L(G)$ は半単純です。
(ii) G の根基は $\{e\}$ です。
(iii) G のすべての通常の可換積分部分群は $\{e\}$ に等しい。
条件 (ii) は、$L(G)$ の根基が $\{0\}$ であることを意味し、したがって (i) $\Leftrightarrow$ (ii) (章 I, § 6, 定理 1) となります。 (i)と(iii)の同値は、§ 6, no. 6、命題14から続きます。

#### 定義 2 {#lie-iii-s9-def-2 .statement tag=0AJJ}

接続された実数または複素数リー群は、有限次元であり、命題 26 の条件を満たす場合、半単純と呼ばれます。

#### 注意 1 {#lie-iii-s9-n8-rem-1 .statement tag=0AJK}

G を有限次元の接続された実数または複素数リー群とします。 G が半単純でない場合、G は、$G' \neq \{e\}$ のように、すべての連続自己同型の下で不変である可換接続リー 部分群 $G'$ を持ちます。 n を最大の $L(G)$ の零理想理想とするからです。 $n \neq \{0\}$ と対応する解析的部分群 N は嘘部分群であり、G (no. 7, 命題 23) のすべての連続自己同型の下で不変です。 N の中心 $G'$ は望ましい特性を持っています。

#### 命題 27 {#lie-iii-s9-prop-27 .statement tag=0AJL}

G を有限次元の接続された実数または複素数リー群とします。次の条件は同等です。
(i) $L(G)$ は単純です。
(ii) G の正規積分部分群は $\{e\}$ と G だけであり、さらに G は可換ではありません。
これは、§ 6, no. 6、命題 14 に続きます。

#### 定義 3 {#lie-iii-s9-def-3 .statement tag=0AJM}

接続された実数または複素数リー群は、有限次元であり、命題 27 の条件を満たす場合、ほぼ単純であると呼ばれます。

#### 命題 28 {#lie-iii-s9-prop-28 .statement tag=0AJN}

G を単純接続された実数または複素数リー群とします。次の条件は同等です。
(i) G は半単純;
(ii) G は、ほぼ単純な群の有限数の積と同型です。
G がほぼ単純なリー群の有限積である場合、$L(G)$ は単純なリー代数の有限積であるため、半単純になります。 G が半単純の場合、$L(G)$ は単純なリー代数 $L_1, \ldots, L_n$ の積と同型です。 $G_i$ をリー群とリー代数 $L_i$ を単純に接続したものとします。したがって、これはほぼ単純です。この場合、G と $G_1 \times \cdots \times G_n$ は単純に接続されており、同型リー代数を持ち、したがって同型です。

#### 補題 1 {#lie-iii-s9-lem-1 .statement tag=0AJO}

G を接続されたトポロジー 群、Z をその中心、$Z'$ を Z の離散部分群とします。すると、$G/Z'$ の中心は $Z/Z'$ です。
y を G の元とし、その類モジュロ $Z'$ が中心元であるとします。

G/Z」。 $\phi$ を G の写像 $g \mapsto gyg^{-1}y^{-1}$ として G にすると、$\phi(G)$ が接続されて $Z'$ に含まれ、したがって $\phi(G) = \phi(\{e\}) = \{e\}$ になります。したがって$y \in Z$。

#### 命題 29 {#lie-iii-s9-prop-29 .statement tag=0AJP}

*G を実数または複素数リー群に接続した半単純とします。*
(i) $G = (G, G)$。
(ii) *中心 G の Z は離散的です。*
(iii) $G/Z$ の *中心は $\{e\}$* です。
主張 (i) は、系から命題 4、no. 2 および章 I, § 6、定理 1 に続きます。
主張 (ii) は、§ 6, no. 4、系 4 から命題 10 および章 I, § 6, no. 1、*注意 2* に続きます。
主張 (iii) は (ii) と補題 1 から続きます。

#### 命題 30 {#lie-iii-s9-prop-30 .statement tag=0AJQ}

(i) *$\mathfrak{g}$ を半単純実数または複素数リー代数とします。このとき、Int $\mathfrak{g}$ は Aut $\mathfrak{g}$.* の恒等式成分です。
(ii) *G を実数または複素数リー群に接続した半単純とします。 G の随伴群は Aut $L(G)$ の恒等体成分です。 中心簡約するから単位元です*。
$\mathfrak{g}$ のすべての導分は内部 (章 I, § 6、系 3 ～ 命題 1) であるため、$L(\mathrm{Int}\,\mathfrak{g}) = L(\mathrm{Aut}\,\mathfrak{g})$ となり、(i) が証明されます。 (ii) の最初の主張は (i) から続きます。 2 番目は、命題 29 (iii) と § 6, no. 4、系 4 (ii) から命題 10 に続きます。

#### 注意 2 {#lie-iii-s9-n8-rem-2 .statement tag=0AJR}

$\mathfrak{g}$ を複素半単純リー代数とし、$\mathfrak{g}_0$ をその基礎となる実数リー代数とします。次に、Aut$(\mathfrak{g})$ は Aut$(\mathfrak{g}_0)$ で Int$(\mathfrak{g}_0) \subset \mathrm{Aut}(\mathfrak{g})$ に対してオープンです。

#### 命題 31 {#lie-iii-s9-prop-31 .statement tag=0AJS}

*G を単純に接続された有限次元の実数または複素数リー群とし、R をその根基とします。 G がリー群として S と R の半直接積であるような、G の半単純単純結合リー部分群 S が存在します。 S' が G の半単純整数部分群である場合、$L(G)$ の冪能根基に次のような x が存在します*
$$
(\mathrm{Ad}\exp x)(S') \subset S.
$$
これは、§ 6, no. 6、系 1 から命題 14、章 I, § 6、定理 5、系 1 と続きます。

#### 補題 2 {#lie-iii-s9-lem-2 .statement tag=0AJT}

*G を群 (それぞれトポロジカル群)、G' を G の通常の部分群、V 有限次元ベクトル空間可換体 k (それぞれ、K について)、$\rho$ 線型表現 (それぞれ連続線型表現) とします。 V と $\rho' = \rho|_{G'}$ の G の。*
(i) *$\rho$が半単純の場合、$\rho'$は半単純です。*
(ii) *$\rho'$ が半単純で、$G/G'$ (または $G/\overline{G}'$) のすべての有限次元線形 k 表現 (または連続線形 K 表現) が半単純である場合、$\rho$ は半単純です。
$\rho$ が半単純であるとします。 $\rho'$ が半単純であることを証明します。 $\rho$ が単純な場合を考えれば十分です。 $V'$ を V の最小非ゼロサブ G' 加群とする。すべての $g \in G$、$\rho(G')\rho(g)V' = \rho(g)\rho(G')V' = \rho(g)V'$ について、他の語 $\rho(g)V'$ は $\rho(G')$ で安定しています。 $V''$ が $\rho(g)V'$ のサブ $G'$ モジュールである場合、$\rho(g)^{-1}V''$ は $V'$ のサブ $G'$ モジュールであるため、$V''$ は $\{0\}$ または $\rho(g)V'$ と等しくなります。

したがって、すべての $g \in G$ に対して、$\rho(g)V'$ は単純な $G'$ モジュールです。しかし、$\sum_{g \in G} \rho(g)V'$ は、$V$、よって $V = \sum_{g \in G} \rho(g)V'$ の非ゼロのサブ$G$ 加群です。したがって、$\rho'$ は半単純です。

$\rho'$ が半単純であるとします。 $W$ を $V$ の非ゼロのサブ$G$ 加群とする。 $\rho'$ は半単純であるため、$\rho'(G)$ と交換する $W$ 上に $V$ のプロジェクター $f_0$ が存在します。 $E$ を $f \in \mathscr{L}(V, V)$ の集合とし、これは $\rho(G')$ と可換であり、写像 $V$ は $W$ に、制限から $W$ はホモテティー となります。 $f \in E$ の場合、ホモテティー $f|W$ の比率を $\alpha(f)$ とします。 次に、$f_0 \in E$ と $\alpha(f_0) = 1$ です。 明らかに、$\alpha$ は $E$ の線型形式です。 $E$の超平面である$F = \mathrm{Ker}\, \alpha$とします。 $f \in E$ と $g \in G$ については、$\sigma(g)f = \rho(g) \circ f \circ \rho(g)^{-1}$ と書きます。次に、$\sigma(g)f$ 写像 $V$ を $W$ に変換し、制限から $W$ は$\alpha(f')$ の比ホモテティー になります。 $g' \in G'$ の場合、
$$
\begin{align*}
\sigma(g)f \circ \rho(g') &= \rho(g) \circ f \circ \rho(g)^{-1} \circ \rho(g') \\
&= \rho(g) \circ f \circ \rho(g^{-1}g'g) \circ \rho(g^{-1}) \\
&= \rho(g) \circ \rho(g^{-1}g'g) \circ f \circ \rho(g^{-1}) \\
&= \rho(g') \circ \rho(g) \circ f \circ \rho(g^{-1}) \\
&= \rho(g') \circ \sigma(g)f.
\end{align*}
$$
したがって$\sigma(g)f \in E$です。 したがって、$\sigma$ は、$E$ 上の $G$ の線形 $k$ 表現 (それぞれ連続線形 $K$ 表現) であり、$F$ は安定しています。 次に、トポロジーの場合、$g \in G'$ に対して $\sigma(g) = \mathrm{Id}_E$ が、したがって $g \in \overline{G'}$ に対してもなります。 $G/G'$ (それぞれ $G/\overline{G'}$) のすべての有限次元 $k$ 線形表現 (それぞれ連続 $K$ 線形表現) が半単純であると仮定します。 次に、$G$ で安定している $F$ の $E$ 補充が存在します。 他の語には、$G$のもとで不変である$\alpha(f) = 1$となるような$f \in E$が存在します。 すると、$f$ は $V$ の射影子から $W$ へ、$g \in G$、$\rho(g) \circ f \circ \rho(g^{-1}) = f$ では、$f$ は $\rho(G)$ と交換します。 したがって、$\rho$ は半単純です。

#### 定理 1 {#lie-iii-s9-thm-1 .statement tag=0AJU}

*$G$ を有限次元の実数または複素数リー群、$G_0$ をその恒等式成分、$R$ をその根基および $L(G)$ の $r$ 根基とします。 $G/G_0$ が有限であると仮定します。 $\rho$ を $G$ の有限次元解析線型表現とします。次の条件は同等です:*
(i) $\rho$ は半単純です。
(ii) $\rho|G_0$ は半単純です。
(iii) $\rho|R$ は半単純です。
(iv) $L(\rho)$ は半単純です。
(v) $L(\rho)|r$ は半単純です。
(i) $\Leftrightarrow$ (ii) 補題 2 および統合、章 VII, § 3、命題 1。
(ii) $\Leftrightarrow$ (iv) および (iii) $\Leftrightarrow$ (v) § 6, no. 5、系 2 ～ 命題 13 による。
(iv) $\Leftrightarrow$ (v) by 章 I, § 6、定理 ４．

#### 系 1 {#lie-iii-s9-thm-1-cor-1 .statement tag=0AJV}

*$\rho, \rho_1, \rho_2$ を有限次元半単純解析線形表現とする

リー群

$G$ と $n$ 整数 $\geq 0$ の送信。すると$\rho_1 \otimes \rho_2, T^n \rho, S^n \rho, \wedge^n \rho$(付録)は半単純になります。

$\rho_1 \otimes \rho_2$ の半単純性は、定理 1 および章 I, § 6、系 1 から定理 4 に続きます。 $T^n \rho, S^n \rho, \wedge^n \rho$ の半単純性は、$\rho_1 \otimes \rho_2$ の半単純性から続きます。

$k$ が標数 0 の可換体、$\Gamma$ 群および $\rho_1$ および $\rho_2$ 有限次元半単純 $\Gamma$ の線形表現 $k$ である場合、 $\rho_1 \otimes \rho_2$は半単純です。

#### 系 2 {#lie-iii-s9-thm-1-cor-2 .statement tag=0AJW}

*$\rho$を、ベクトル空間$V$、$S$の$V$と$S^G$の対称代数における$G$の有限次元半単純解析線型表現とします。 部分代数の $S$ からなるの元は $(S\rho)(G)$ の下では不変です。この場合、$S^G$ は有限生成された代数です。*

これは、定理 1、章 I, § 6、定理 6 (a) および *可換代数*、章 V, § 1、定理 2 から続きます。

#### 系 3 {#lie-iii-s9-thm-1-cor-3 .statement tag=0AJX}

*$G$ を実数または複素数リー群とし、$G_0$ をその恒等式成分とします。 $G_0$ が半単純で、$G/G_0$ が有限であると仮定します。したがって、$G$ のすべての有限次元解析線型表現は半単純になります。*

#### 命題 32 {#lie-iii-s9-prop-32 .statement tag=0AJY}

*$G$を有限次元接続された実リー群とします。 $L(G)$ が還元的であると仮定します。次の条件は同等です。

(i) $G/\overline{D^1}G$ はコンパクトです。
(ii) (それぞれ (ii')) 複素数 (実数) ベクトル空間上の $G$ のすべての有限次元解析線型表現は半単純です。

(i) $\Rightarrow$ (ii'): $G/\overline{D^1}G$ がコンパクトであると仮定します。このとき、有限次元実数ベクトル空間上の $G/\overline{D^1}G$ のすべての連続線型表現は、 半単純 (*積分*, 章 VII, § 3, 命題 1) になります。 $\rho$ を実数ベクトル空間上の $G$ の有限次元解析線型表現とします。この場合、$\rho|D^1G$ は解析的であり、$D^1G$ は半単純 (章 I, § 6, 命題 5) であるため、$\rho|D^1G$ は半単純 (系 3 ～ 定理) となります。 1)。したがって、$\rho$ は半単純 (補題 2) です。

(i) $\Rightarrow$ (ii') も同様に見ることができます。

(i) $\Rightarrow$ (ii): $G/\overline{D^1}G$ はコンパクトではないため、形 $\mathbf{R}^p \times \mathbf{T}^q$ の群と $p > 0$ ($§ 6$、no. 4、命題 11 (ii)) が同型であるとします。次に、$\mathbf{R}$ に対する$G/\overline{D^1}G$ の全射射が存在し、したがって$\mathbf{R}$ に対する$G$ の全射射が存在します。 写像

$$
g \mapsto \sigma(g) = \begin{pmatrix} 1 & 0 \\ \rho(g) & 1 \end{pmatrix}
$$

$\sigma(G)$ で安定している $\mathbf{R}^2$ の 1 次元ベクトル部分空間は $\mathbf{R}(0, 1)$ であるため、$\mathbf{R}^2$ 上の $G$ の解析線型表現は半単純ではありません。

(ii) $\Rightarrow$ (i) も同様に見ることができます。

#### 命題 33 {#lie-iii-s9-prop-33 .statement tag=0AJZ}

G を連結成分の数が有限である有限次元複素リー群、$\varphi$ を G の有限次元解析線形表現、$G'$ を実リー群 G の整数部分群とし、$L(G')$ が $\mathbf{C}$ 上で $L(G)$ を生成するものとします。 すると、$\varphi$ が半単純になるためには、$\varphi|G'$ が半単純になることが必要十分です。

$\varphi' = \varphi|G'$ にしましょう。 $\varphi$ (それぞれ $\varphi'$) が半単純であるためには、$L(\varphi)$ (それぞれ $L(\varphi')$) が半単純 (定理 1) であることが必要かつ十分です。 Vを$\varphi$の空間とします。 V のベクトル部分空間が $L(\varphi)(L(G))$ で安定するためには、$L(\varphi')(L(G'))$ で安定することが必要かつ十分です。したがって命題です。

### 練習問題 {#lie-iii-s9-exercises}

[§ 9 に対して練習問題](exercises/s9/)を参照してください。
