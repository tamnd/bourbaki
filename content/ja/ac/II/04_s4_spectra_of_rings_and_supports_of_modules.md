---
book: ac
book_title: Commutative Algebra
chapter: II
chapter_title: LOCALIZATION
section: 4
section_title: Spectra of rings and supports of modules
lang: ja
source: ac-i-vii
book_pages: 94-107, 140-146
pdf_pages: 0114-0127, 0160-0166
extraction: ocr
subsections:
    - "no": 1
      title: IRREDUCIBLE SPACES
      page: 94
      pdf_page: 114
    - "no": 2
      title: NOETHERIAN TOPOLOGICAL SPACES
      page: 97
      pdf_page: 117
    - "no": 3
      title: THE PRIME SPECTRUM OF A RING
      page: 98
      pdf_page: 118
    - "no": 4
      title: THE SUPPORT OF A MODULE
      page: 104
      pdf_page: 124
statements: 49
exercises: 28
content_sha256: 191176ecf5a5f7265d678d59e79f306b6f022512b27bfbd840c8c995504144f0
translated_from: content/en/ac/II/04_s4_spectra_of_rings_and_supports_of_modules.md
translation_method: google
source_content_sha256: aa56aa107c641a6f533bca5b5920334a1f4dfec7d2788424e0037a9fcb53cc7b
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: fe4b5d86023cf974f48f05b318291eea46f6237a1f5089dbc0264ede4406025c
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 4. 環のスペクトルと加群のサポート

### 1. 還元不可能空間

#### 定義 1 {#ac-ii-s4-def-1 .statement tag=0498}

位相幾何学的空間 $X$ は、$X$ の空でない開いた集合のすべての有限共通部分が空でない場合、既約と呼ばれます。

$X$ の開いた集合の空族を考慮すると、既約空間が空ではないことがわかります。トポロジカル空間 $X$ が既約であるためには、それが空でないこと、そして 2 つの空ではない開いた集合の $X$ のうち共通部分が常に空ではないこと (または、同じことになるが、2 つの閉じた集合のうち和集合が空でないこと) が必要かつ十分である。 $X$ は常に $X$ とは区別されます)。

#### 命題 1 {#ac-ii-s4-prop-1 .statement tag=0499}

$X$ を空ではないトポロジカル空間とします。次の条件は同等です。
(a) $X$ は既約です。
(b) $X$ の空ではないオープン集合はすべて $X$ に密集しています。
(c) $X$ の開いているすべての集合が接続されています。

定義により、$X$ で密な集合は、空ではないすべての開いた集合と一致する集合となるため、(a) と (b) は等価です。 $U_1$ と $U_2$ が互いに素空ではないオープン集合である場合、$U_1 \cup U_2$ は切断されたオープン集合であるため、(c) が (a) を意味するのは明らかです。最後に、(a) が (c) を意味することを示しましょう。 $U$ が切断されたオープン集合である場合、それは 2 つの互いに素空ではない集合 $U', U''$ のうち和集合であり、これらは $U$ でオープンであるため、$X$ でもオープンです。これは、次のことを意味します。 $X$ は還元不可能ではありません。

ハウスドルフ空間は、単一の点から構成される場合にのみ既約です。

$X$ の部分空間 $E$ が既約である場合、トポロジカル空間 $X$ の部分集合 $E$ は既約集合と呼ばれます。そのためには、$X$ に開いて $E$ と一致する集合 $U, V$ の対ごとに、$U \cap V$ も $E$ と一致するか、または (同じことになります) 対ごとに、 集合 $F, G$ は、$X$ と満たす $E \subset F \cup G$、$E \subset F$、$E \subset G$ は休業となります。 $n$の帰納法により、$(F_i)_{1 \leq i \leq n}$が$E \subset \bigcup_{i=1}^n F_i$となる$X$の閉じた集合の有限族である場合、$E \subset F_i$となる添字$i$が存在すると推測します。

#### 命題 2 {#ac-ii-s4-prop-2 .statement tag=049A}

トポロジー 空間 $X$ において、集合 $E$ が既約であるためには、その閉包 $\overline{E}$ が既約であることが必要かつ十分です。

$X$ のオープン集合が $E$ を満たすには、$\overline{E}$ を満たすことが必要かつ十分です。上記の注意から命題が続きます。

#### 命題 3 {#ac-ii-s4-prop-3 .statement tag=049B}

(i) *$X$ が既約空間である場合、$X$ の空でないすべての開いた部分集合は既約です。

(ii) *$(U_\alpha)_{\alpha \in A}$ を、添字 $(\alpha, \beta)$ のすべての対に対して $U_\alpha \cap U_\beta = \emptyset$ となるような、開いた集合のトポロジカル空間 $X$ からなるの空でないカバーとします。 集合 $U_\alpha$ が既約であれば、空間 $X$ は既約です。*

(i) $X$ が既約の場合、$U \subset X$ は空ではなく、$X$ で開いており、$V \subset U$ は空ではなく、$U$ で開いており、$V$ も$X$ で開いているため、$X$ では密で、*なおさら* では密です$U$。すると、$U$は既約です(命題 1)。

(ii) $X$ のすべての空でないオープン集合 $V$ について、すべての $\alpha \in A$ について $V \cap U_\alpha \neq \emptyset$ について、$V \cap U_\alpha$ が $U_\alpha$ で仮定だけ密であること、従って$V$ が密であることを示します。 $X$ そしてこれは、$X$ が既約であることを証明します (命題 1)。現在、$V \cap U_y \neq \emptyset$ となるような添字 $y$ が少なくとも 1 つ存在します。すべての $\alpha$ と $V \cap U_y$ に対する $U_\alpha \cap U_y \neq \emptyset$ は、$U_y$、$U_y \cap V \neq \emptyset$、*なおさら* $U_y \cap V \neq \emptyset$ に密集しており、(ii) の証明が完成します。

#### 命題 4 {#ac-ii-s4-prop-4 .statement tag=049C}

*$X$と$Y$を2つのトポロジー空間と$f$を$X$から$Y$までの連続写像とする。 $X$ の既約部分集合 $E$ ごとに、$f(E)$ は $Y$ の既約部分集合です。*

$U, V$が$f(E)$を満たす$Y$の2つのオープン集合である場合、$f^{-1}(U)$と$f^{-1}(V)$は$E$を満たす$X$のオープン集合です。その結果、$f^{-1}(U) \cap f^{-1}(V) = f^{-1}(U \cap V)$ は $E$ と一致します。これは、$U \cap V$ が $f(E)$ と一致し、命題が証明されることを意味します。

#### 定義 2 {#ac-ii-s4-def-2 .statement tag=049D}

*トポロジカル空間 $X$ のすべての最大既約部分集合は、$X$ の既約成分と呼ばれます。

命題 2 から、$X$ のすべての既約成分は $X$ で *閉じられます*。

#### 命題 5 {#ac-ii-s4-prop-5 .statement tag=049E}

*$X$をトポロジカル空間とします。 $X$ のすべての既約部分集合は、$X$ の既約成分に含まれており、$X$ はその既約成分の和集合です。

最初の主張を証明するには、Zorn の補題により、$X$ の既約部分集合の集合 3 が *帰納的*であることを証明すれば十分です。 $\mathscr{G}$ を包含によって完全に順序付けされた $\mathfrak{S}$ の部分集合とします。 集合 $F \in \mathscr{G}$ の和集合 $E$ が既約であることを示します。 $U, V$を、$E$を満たす$X$の2つの開いた集合とします。 $\mathscr{G}$ は完全に順序付けされているため、$U$ と $V$ との出会いである集合 $F \in \mathscr{G}$ が存在します。 $F$ は既約であるため、$U \cap V$ は $F$ を満たすため、$E$ も満たされます。これは、$E$ が既約であり、したがって 3 が帰納的であることを証明します。 2 番目の主張は、1 つの点の $X$ からなるのすべての部分集合が既約であるため、最初の主張が続きます。

#### 系 {#ac-ii-s4-n1-cor-1 .statement tag=049F}

*トポロジー 空間 $X$ のすべての接続された成分は、$X$ の既約成分の和集合です。

$X$ のすべての既約部分空間は命題 1 によって接続されているため、接続された $X$ の成分に含まれます。

$X$ の 2 つの別個の既約成分は、共通の (練習問題 11) に点が含まれる可能性があることに注意してください。

#### 命題 6 {#ac-ii-s4-prop-6 .statement tag=049G}

*$X$ をトポロジカル空間と $(P_i)_{1 \leq i \leq n}$ $X$ からなるおよび既約閉集合を覆うアジナイトとします。すると、$X$の既約成分は、$P_i$の集合の(包含に関して)極大元になります。

比較可能な 2 つの $P_i$ が存在しない場合に限定することもできます。 $E$ が $X$ の既約部分集合である場合、$E \subset \bigcup_{i=1}^n P_i$、したがって $E$ は閉じた集合 $P_i$ の 1 つに含まれます。これは、$P_i$ が $X$ の唯一の最大既約部分集合であることを証明します。

#### 系 {#ac-ii-s4-n1-cor-2 .statement tag=049H}

*$X$ をトポロジカルな空間と $E$ 部分空間とし、明確な既約成分 $Q_i$ ($1 \leq i \leq n$) のアジナイト数のみを持ちます。その場合、$X$ の閉包 $\overline{E}$ の既約成分は、$i \neq j$ の $Q_i$ ($1 \leq i \leq n$) と $\overline{Q}_i \# \overline{Q}_j$ の閉包 $\overline{Q}_i$ です。

$\overline{E}$ は、既約 (命題 2) である $\overline{Q}_i$ の和集合です。 $Q_i$ は $E$、$\overline{Q}_i \cap E = Q_i$ に閉まるため、 命題のおかげで、$Q_i \notin Q_j$ が $i \neq j$、$\overline{Q}_i \notin \overline{Q}_j$、よって系として 6.

#### 注意 {#ac-ii-s4-n1-rem-1 .statement tag=049I}

$X$ には、明確な既約成分 $X_i$ ($1 \leq i \leq n$) のアジナイト数のみがあるとします。次に、$U_+ = \mathbf{C}(\bigcup_{j \neq i} X_j)$は$X$に開いており、$X_i \notin \bigcup_{j \neq i} X_j$以降$X_i$は密です。したがって、$U_i$ ($1 \leq i \leq n$) は空ではなく、既約 (命題 2) である $X$ の開いた集合であり、ペアの互いに素とその和集合が $X$ に密集しています。

#### 命題 7 {#ac-ii-s4-prop-7 .statement tag=049J}

*$U$ をトポロジカル空間 $X$ の開部分集合とします。 写像 $V \mapsto \overline{V}$ ($X$ での閉包) は、集合の全単射 & $U$ の既約部分集合で、$U$ で集合に閉じられ、既約部分集合 & $X$で閉じられ、$U$と出会う$X$。 逆全単射は$Z \mapsto Z \cap U$です。特に、この全単射写像集合 & 既約成分 & $U$ を集合に、既約成分 & $X$ を$U$ と満たします*。

$V$が$U$で閉じて既約であれば、$\overline{V}$は既約（命題2）と$V = \overline{V} \cap U$です。逆に、$Z$ が既約で、$X$ で閉じて$U$ を満たす場合、$Z \cap U$ は$Z$ の空ではない開いた部分集合であるため、既約 (命題 3) であり、$Z$ では密であり、$Z$ が閉店、$Z = \overline{Z} \cap U$。これは命題を証明します。

### 2. ネーター トポロジカル空間

#### 定義 3 {#ac-ii-s4-def-3 .statement tag=049K}

トポロジカル空間 $X$ は、包含順に並べられた $X$ の閉じた部分集合の空でないすべての集合が最小の元を持つ場合、 ネーター と呼ばれます。

包含順に並べた、$X$ のオープン部分集合の空でないすべての集合に極大元がある、またはクローズド (オープン) 集合のすべての減少する (それぞれ増加する) 数列が静止している (集合) と言うのは、同じことになります。 理論、章 111、§ 6, no. 5、命題 6)。

#### 命題 8 {#ac-ii-s4-prop-8 .statement tag=049L}

(i) ネーター 空間のすべての部分空間はネーター です。
(ii) $(A_i)_{i \in I}$ をトポロジカル空間 $X$ の有限被覆とする。 $X$ の部分空間 $A_i$ がネーター である場合、$X$ はネーター です。

(i) Let $X$ be a Noetherian space, $A$ a subspace of $X$ and $(F_i)$ a decreasing sequence of subsets of $A$ which are closed in $A$; then $F_i = \overline{F_n} \cap A$ and the closures $\overline{F_n}$ of the $F_i$ in $X$ form a decreasing sequence of closed subsets of $X$. この数列が静止しているので、 数列 $(F_i)$ も静止しています。

(ii) $(G_n)_{n \geq 0}$ を $X$ のクローズド部分集合の減少列とします。 仮定までに、数列 $(G_n \cap A_i)_{n \geq 0}$ はそれぞれ静止しています。 $I$ が有限であるため、$n \geq n_0$、$G_n \cap A_i = G_{n_0} \cap A_i$、すべての $i \in I$ に対して、整数 $n_0$ が存在します。でも
$$
G_n = \bigcup_{i \in I} (G_n \cap A_i)
$$
したがって、数列 $(G_n)$ は静止しており、$X$ はネーター です。

#### 命題 9 {#ac-ii-s4-prop-9 .statement tag=049M}

トポロジー 空間 $X$ がネーター であるためには、$X$ 内のすべての開いた集合が準コンパクトであることが必要かつ十分です。

条件が必要であることを示すには、命題 8 によって、すべてのネーター 空間 $X$ が準コンパクトであることを証明すれば十分です。 $(U_i)_{i \in I}$ を $X$ のオープンカバーとします。 集合 $U_i$ の有限和集合の集合は空ではないため、極大元 $V = \bigcup_{i \in H} U_i$ を許容します。ここで、$H$ は $I$ の有限部分集合です。 定義までに、すべての $i \in I$ に対して $V \cup U_i = V$、したがって $V = X$ になります。

逆に、$X$ のすべてのオープン集合が準コンパクトであると仮定し、$(U_i)$ を $X$ のオープン部分集合の増加する数列とします。 $U_i$ の和集合 $V$ はオープンなので準コンパクトです。 $(U_i)$ は $V$ の開いたカバーであるため、$V$ のカバーである $(U_i)$ の有限サブファミリーがあり、したがって一部の添字 $n$ については $V = U_n$ となり、数列 $(U_i)$ が静止していることが証明されます。

#### 補題 1 (「ネーター 帰納法の原理」) {#ac-ii-s4-lem-1 .statement tag=049N}

*E を、空でないすべての部分集合が最小の元を許容する順序付き集合とします。 F を次の性質を持つ E の部分集合とします。 $a \in E$ が関係 $x < a$ が $x \in F$ を暗黙的に示すような場合、$a \in F$ になります。次に、$F = E$.*

$F \neq E$ と仮定します。その場合、$CF$ は最小の元 $b$ になります。 定義により、すべての $x < b$ に対して $x \in F$ となり、これは $b \in F$ を意味し、これは矛盾です。

#### 命題 10 {#ac-ii-s4-prop-10 .statement tag=049O}

*Xがネーター空間の場合、Xの既約成分の集合（およびXの結合成分のなおさら集合）は、有限。*

X が既約閉部分集合 (no. **1**, 命題 6) の有限和集合であることを証明すれば十分です。 E を包含順に並べた X の閉部分集合の集合とし、F を既約閉の有限和集合の集合として、ネーター 帰納法の原理を適用できることを示しましょう。 部分集合。 Y を、Y 属するのすべての閉じた部分集合 $\neq Y$ が F になるように、X の閉じた部分集合とします。Y が既約であれば、定義により $Y \in F$ が得られます。それ以外の場合、Y は Y とは異なる 2 つの閉じた部分集合 $Y_1,\ Y_2$ の和集合です。すると、F の定義によって仮定、よって $Y \in F$ によって $Y_1 \in F$ と $Y_2 \in F$ になります。

特に、*ハウスドルフ* ネーター 空間は必然的に *有限* であることがわかります。

### 3. 環の素スペクトル

A を A の素イデアルの環と X 集合とします。A のすべての部分集合 M について、含む M の素イデアルの $V(M)$ 集合で表します。明らかに、$a$ が M によって生成された A の理想である場合、$V(M) = V(a)$。 M が単一の元 f で構成されている場合、$V(\{f\})$ の代わりに $V(f)$ と書くと、$V(f) = V(Af)$ になります。 写像 $M \mapsto V(M)$ は、A および X への包含に関して *減少する* です。さらに、次の式が成り立ちます。

(1)
$$
V(0) = X, \quad V(1) = O;
$$

(2)
$$
V\left(\bigcup_{i \in I} M_i\right) = V\left(\sum_{i \in I} M_i\right) = \bigcap_{i \in I} V(M_i)
$$
すべての家族に対して、A の $(M_i)_{i \in I}$ の部分集合 。

(3)
$$
V(a \cap a') = V(aa') = V(a) \cup V(a')
$$
A の理想 $a,\ a'$ のすべての対に対して。 式 (1) と (2) は明らかです。一方、公式 (3) は、A の主イデアル $p$ からイデアル $a$ または $a'$ の 1 つである含むに対して、それが含む $aa'$ または含む $a \cap a'$ であることが必要かつ十分であることを意味します。そうすると、§ 1, no. 1の帰結、命題 1になります。 2 番目の公式 (1) には次の逆があります。$a$ が $V(a) = \varnothing$ となるような $A$ の理想である場合、$a = A$ になります。これは、$A$ 含む $a$ の最大理想が存在しないためです。 最後に、$a$ が $A$ の理想であり、$r(a)$ がその *根基* ($§ 2$、no. 6、定義 4) である場合、

$$
V(a) = V(r(a))
$$

$§ 2$、no. 6、系 1 から命題 13 まで。

Formulae (1) to (3) show that the subsets $V(M)$ of $X$ satisfy the *closed set* axioms of a topology (*General Topology*, Chapter I, $§ 1$, no. 4).

#### 定義 4 {#ac-ii-s4-def-4 .statement tag=049P}

※$A$を環とします。 $A$ の素イデアルの集合 $X$ は、閉じた集合が集合 $V(M)$ である位相で、$M$ が $\mathfrak{P}(A)$ を通るものであり、$A$ の素数スペクトルと呼ばれ、次のように表されます。 $\mathrm{Spec}(A)$。このように定義された位相は、$X$ 上のスペクトルまたはザリスキー 位相と呼ばれます。

明らかに、関係 $\mathrm{Spec}(A) = \varnothing$ は $A = \{0\}$ と同等です。

$X$ を環 $A$ の素スペクトルとします。すべての $f \in A$ について、$A$ * 含む* $f$ ではなく、$X_f$ 集合で表しましょう。したがって、$X_f = X - V(f)$ と $X_f$ は *オープン* 集合になります。 (2) により、$X$ のすべての閉じた部分集合は、形 $V(f)$ の閉じた集合の共通部分であるため、$X$、形はスペクトル位相の *基底* になります。 $X$。さらに、定義からすぐに次のようになります。

$$
X_0 = O,\quad X_1 = X,
$$

より一般的には、$A$ の可逆元 $f$ ごとに $X_{f^{-1}} = X$ です。

$$
X_{g^{-1}} = X, nX, \quad \text{for all } f, g \text{ in } A.
$$

$X$ のすべての部分集合 $Y$ について、$A$ の主要な理想の属するから $Y$ の$\mathfrak{J}(Y)$ 共通部分で表します。明らかに、$\mathfrak{J}(Y)$ は $A$ の理想であり、$X$ と $A$ に含めることに関して、写像 $Y \mapsto \mathfrak{J}(Y)$ は *減少する* です。明らかに関係

$$
\mathfrak{J}(\varnothing) = A
$$
$$
\mathfrak{J}\left( \bigcup_{\lambda \in L} Y_\lambda \right) = \bigcap_{\lambda \in L} \mathfrak{J}(Y_\lambda)
$$

すべての家族に、$(Y_\lambda)_{\lambda \in L}$、部分集合、$X$ が適用されます。さらに:

#### 命題 11 {#ac-ii-s4-prop-11 .statement tag=049Q}

※$A$を環、$a$を$A$、$Y$を$X = \mathrm{Spec}(A)$の部分集合とします。
(i) $V(a)$ は $X$ で閉じられ、$\mathfrak{J}(Y)$ はその根基に等しい $A$ の理想です。
(ii) $\mathfrak{J}(V(a))$ *は* $a$ *および* $V(\mathfrak{J}(Y))$ *の根基です* $Y$ *の* $X$.*

(iii) 写像 3 と V 定義する減少する全単射のうち、A の理想のX と集合の閉じた部分集合の集合の間の一方が他方の反転です。これらは根基に等しい。

主張 (i) と (ii) の最初の主張は、定義と § 2, no. 6 から続き、系 1 から命題 13 になります。閉じた集合 V(M) (一部の M ⊂ A) の場合含む Y の場合、すべての素数イデアル p ∈ Y に対して M ⊂ p となり、よって M ⊂ J(Y) となり、結果として V(M) ⊃ V(J(Y)) となります。 Y ⊂ V(J(Y)), V(J(Y)) は X 含む Y の最小のが閉じた集合となり、(ii) の証明が完成します。最後に、(ii) から、a がその根基に等しい素イデアルである場合、J(V(a)) = a であり、Y が X で閉じている場合、V(J(Y)) = Y になります。これは(iii)を証明します。

命題 11 から、M が A のいずれかの部分集合で、Y が X のいずれかの部分集合である場合、V(M) = V(J(V(M))) および J(Y) = J(V(J(Y)))。

#### 系 1 {#ac-ii-s4-prop-11-cor-1 .statement tag=049R}

X の閉じた部分集合のすべての族 (Y_λ)_{λ ∈ L} について、J(∩_{λ ∈ L} Y_λ) は理想 J(Y_λ) の和の根基です。

命題 11 (iii) から、J(∩_{λ ∈ L} Y_λ) は、その根基および含むのすべての J(Y_λ) に等しい最小の理想であることがわかります。この理想は含む ∑_{λ ∈ L} J(Y_λ) となり、従って ∑_{λ ∈ L} J(Y_λ) の根基 (§ 2, no. 6, 系 2 から命題) 13)、よって系。

#### 系 2 {#ac-ii-s4-prop-11-cor-2 .statement tag=049S}

r(a) が A のイデアル a の根基を表すものとします。 a と b が A の 2 つのイデアルである場合、関係 V(a) ⊂ V(b) は b ⊂ r(a) および r(b) ⊂ r(a) と同等です。

関係 b ⊂ r(a) と r(b) ⊂ r(a) が等価であるのは明らかであり、V(a) = V(r(a)) であるため、系は命題 11 の直後に続きます (iii)。

#### 系 3 {#ac-ii-s4-prop-11-cor-3 .statement tag=049T}

(f_λ)_{λ ∈ L} を A の元の族とする。 元 g ∈ A から満たす X_g ⊂ ∪_{λ ∈ L} X_{f_λ} に対して、次が存在することが必要十分である。 整数 n > 0 であるため、g^n 属するは f_λ によって生成される理想値になります。

関係 X_g ⊂ ∪_{λ ∈ L} X_{f_λ} は V(g) ⊃ ∩_{λ ∈ L} V(f_λ) と同等であり、系を適用する 2 に十分です。

系 4、A の 2 つの元 f, g から満たす X_f = X_g に対して、f^m ∈ Ag と g^n ∈ Af となる 2 つの整数 m > 0, n > 0 が存在すれば必要十分です。

#### 系 5 {#ac-ii-s4-prop-11-cor-5 .statement tag=049U}

$f \in A$ から満たす $X_f = \varnothing$ については、$f$ がゼロ能であることが必要かつ十分です。

これは系 4 の直後に続きます。

#### 系 6 {#ac-ii-s4-prop-11-cor-6 .statement tag=049V}

点 $p \in X = \mathrm{Spec}(A)$ の集合からなるの終結は、主要理想値含む $p$ の集合 $V(p)$ です。 集合 $\{p\}$ が $X$ で閉じられるためには (または、言葉の乱用で言うかもしれませんが、$p$ が $X$ の閉点になるために)、 $p$ が最大であることが必要かつ十分です。

#### 系 7 {#ac-ii-s4-prop-11-cor-7 .statement tag=049W}

$A$ がネーター 環の場合、$X = \mathrm{Spec}(A)$ はネーター 空間となります。

#### 命題 12 {#ac-ii-s4-prop-12 .statement tag=049X}

すべての $f \in A$ について、$X = \mathrm{Spec}(A)$ の開いた集合 $X_f$ は準コンパクトです。特に、空間 $X$ は準コンパクトです。

位相の $X_g$ 形基底のように、$(g_\lambda)_{\lambda \in L}$ が $X_f \subset \bigcup_{\lambda \in L} X_{g_\lambda}$ となるような $A$ の元の族である場合、次のような有限部分族 $(g_{\lambda_i})_{i \in I}$ が存在することを証明するのに十分です。 $X_f = \bigcup_{i \in I} X_{g_{\lambda_i}}$。しかし、関係 $X_f = \bigcup_{\lambda \in L} X_{g_\lambda}$ は、整数 $n > 0$ と、そのサブファミリーによって生成された理想 (系 3 から命題 11) に対して "f" 属するとなるような有限サブファミリー $(g_{\lambda_i})_{i \in I}$ が存在することを意味します。 よって命題。

#### 命題 13 {#ac-ii-s4-prop-13 .statement tag=049Y}

$A, A'$ を、$A$ から $A'$ までの 2 つの環、$X = \mathrm{Spec}(A), X' = \mathrm{Spec}(A')$、$h$ 準同型とします。 $X'$から$X$までの写像$^a h : p' \mapsto \overline{h}(p')$は連続です。

$M \subset A$ の場合、集合 $(^a h)^{-1}(V(M))$ は $A'$ の素イデア $p'$ の集合であり、$M \subset \overline{h}(p')$ は $h(M) \subset p'$ と等価です。この集合は $V(h(M))$ に等しいため、閉じられます。

準同型 $h$ に関連付けられた $^a h$ 写像を呼び出します。

#### 注意 {#ac-ii-s4-n3-rem-1 .statement tag=049Z}

$h$ が全射で、$a$ がその核である場合、スペクトル位相の定義から、$^a h$ は、スペクトル位相の閉じた部分空間 $V(a)$ に対する $X'$ の同型写像であることがわかります。 $X$; $A'$ の主理想 $p'$ から含む $A'$ の理想 $b'$ に対しては、$\overline{h}(p')$ 含む $\overline{h}(b')$ であることが必要かつ十分です。まず、$b'$ を素数とすることで、$^a h$ が単射法であることがわかります。さらに、$A'$の$b'$、$V(b')$の$^a h$の下の像は$V(\overline{h}(b'))$、よっての主張、形$\overline{h}(b')$の理想はすべて、 $A$ と含む $a$。

#### 系 {#ac-ii-s4-n3-cor-1 .statement tag=04A0}

$S$ を $A$、$A' = S^{-1}A$、$h$ 標準準同型 $i_A^S$ の乗算部分集合とします。この場合、$^a h$ は、$S$ を満たさない$A$ の素イデアルの $X = \mathrm{Spec}(A)$ からなるの部分空間に対する $X' = \mathrm{Spec}(A')$ の同型写像です。

$f' = f/s$ とします。ここで、$f \in A, s \in S$; $s/1$ は $A'$ で反転可能であるため、$X'_{f'} = X'_{f/1}$ になります。 $^a h$ は単射法であり、すべての $p' \in X'$、関係 $f/1 \in p'$、$f \in h^{-1}(p') = ^a h(p')$ が等価であること、したがって条件 $p' \in X'_{f/1}$ と $^a h(p') \in X_f$ が等価であることはすでにわかっています。これは、$X$ (それぞれ $X$) の位相の $X, (resp.\ X'_{f'})$ 形基底以来、$^a h(X'_{f'})$ が $X_f \cap ^a h(X')$、よって最初の主張に等しいことを示しています。 2 番目の主張は、 、 no. 5、 命題 11 (ii) から続きます。

#### 命題 14 {#ac-ii-s4-prop-14 .statement tag=04A1}

※$A$を環とします。 For a subset $Y$ of $X = \mathrm{Spec}(A)$ to be irreducible, it is necessary and sufficient that the ideal $\mathfrak{J}(Y)$ be prime.*

$p = \mathfrak{J}(Y)$ と書くと、元 $f \in A$ に対して、関係 $f \in p$ は $Y \subset V(f)$ と同等であることがわかります。 $Y$ が既約であり、$f, g$ が $fg \in p$ となるように $A$ の元であるとします。それから
$$
Y \subset V(fg) = V(f) \cup V(g);
$$
$Y$ は既約であり、$V(f)$ と $V(g)$ が閉じているため、$Y \subset V(f)$ または $Y \subset V(g)$ であるため、$f \in p$ または $g \in p$ となり、$p$ が素数であることが証明されます。

ここで、$p$ が素数であると仮定します。次に、$\overline{Y} = V(p)$ (命題 11 (ii))、そして、$p$ が素数であるため、$p = \mathfrak{J}(\{p\})$、よって $\overline{Y} = V(\mathfrak{J}(\{p\})) = \{p\}$ (命題 11 (ii)) となります。単一の点の集合からなるが既約であるように、$Y$ も既約です (no. 1、命題 2)。

#### 系 1 {#ac-ii-s4-prop-14-cor-1 .statement tag=04A2}

* 環 $A$ が $X = \mathrm{Spec}(A)$ が既約であるためには、$A$ の商がそのニルラジカル $\mathfrak{N}$ によって整域になることが必要かつ十分です。

命題 11 (i) により、$\mathfrak{J}(X)$ は理想$(0)$ の根基、つまり $\mathfrak{N}$ になります。

#### 系 2 {#ac-ii-s4-prop-14-cor-2 .statement tag=04A3}

*写像 $p \mapsto V(p)$ は、$X = \mathrm{Spec}(A)$ の全単射を既約閉の集合上に$X$ の部分集合を重ねたものです。特に、$X$の閉じた部分集合$Y$の既約成分は集合$V(p)$であり、ここで$p$は、最少の元の集合の集合を貫いています。 $A$ どれが含む $\mathfrak{J}(Y)$.*

$A$ のすべての素イデアル $p$ に対して $\mathfrak{J}(V(p)) = p$ が、$X$ のすべての閉じた部分集合 $Y$ に対して $Y = V(\mathfrak{J}(Y))$ として、最初の主張は命題 14 から続きます。一方、$Y \supset V(p)$ については、次のことが必要十分です。
$$
p = \mathfrak{J}(V(p)) \supset \mathfrak{J}(Y)
$$
(命題 11)、よって 2 番目の主張。

#### 系 3 {#ac-ii-s4-prop-14-cor-3 .statement tag=04A4}

*ネーター 環 $A$ の最小素イデアルの集合は有限です。*

$X = \mathrm{Spec}(A)$ には、既約成分 (系 7 から命題 11 および no. 2、命題 10) の有限の数のみがあり、系は上記の系 2 から続きます。

#### 命題 15 {#ac-ii-s4-prop-15 .statement tag=04A5}

Let $A$ be a ring, $I$ a finite set and $E$ the set of orthogonal families $(e_i)_{i \in I}$ of idempotents $e_i \neq 0$ of $A$ such that $\sum_{i \in I} e_i = 1$. すべての $(e_i)_{i \in I} \in E$ に対して、私たちは集合 $\overline{\omega}((e_i)_{i \in I}) = (\mathrm{V}(A(1 - e_i)))_{i \in I}$、$\sigma((e_i)_{i \in I}) = (Ae_i)_{i \in I}$ です。 次に、$\overline{\omega}$ は $E$ の全単射から集合 $P$ の分割 $(U_i)_{i \in I}$ の $X = \mathrm{Spec}(A)$ がオープンの集合になり、$\sigma$ は $E$ の全単射になります。 集合 $S$ 家族 $(a_i)_{i \in I}$ 理想 $\neq 0$ $A$ で、$A$ は $a_i$ の直和になります。

$(e_i)_{i \in I}$ を $E$ と集合 $Y_i = \mathrm{V}(A(1 - e_i))$ の元とします。 $i \neq j$の場合、$1 = 1 - e_i + e_i(1 - e_j) \in A(1 - e_i) + A(1 - e_j)$、よって $Y_i \cap Y_j = \varnothing$（式(1)、(2)）。一方で、

$$
\bigcup_{i \in I} Y_i = \mathrm{V}\left( \prod_{i \in I} A(1 - e_i) \right)
$$

(公式(3));

仮定 $\prod_{i \in I} (1 - e_i) = 1 - \sum_{i \in I} e_i = 0$、よって $\bigcup_{i \in I} Y_i = X$ (公式 (I)) による。 $Y_i$が定休日のため、よって$\overline{\omega}(E) \subset P$も営業しております。また、明らかに $A = \sum_{i \in I} Ae_i$; $0 = \sum_{i \in I} a_i e_i$ の場合、$a_i \in A$ の場合、すべての $i$ に対して $e_i$、$O = a_i e_i^2 = a_i e_i$ を掛けることで得られます。これは$\sigma(E) \subset S$であることを証明します。

#### 補題 2 {#ac-ii-s4-lem-2 .statement tag=04A6}

** $e, f$ * が * $A$ の 2 つの冪等である場合*、 $Ae$ * と* $Af$ * が同じ根基* を持つ場合、 $e = f$ になります。

$e = e^m \in Af$ と $f = f^n \in Ae$ のような仮定整数 $m \geq 0, n \geq 0$ が存在します。 $x, y$ を $e = xf, f = ye$ となるように $A$ の元とします。次に$ef = x^2 = x = e$、同様に$ef = ye^2 = ye = f$、よって $e = f$。

補題 2 と系 2 ～ 命題 11 は、写像 $\overline{\omega}$ と $\sigma$ が*単射*であることを示しています。

$\sigma$ が全射であることを示しましょう。 $(a_i)_{i \in I}$ が $S$ の元である場合、$1 = \sum_{i \in I} e_i$ となる元 $e_i \in a_i$ があります。 $i \neq j$の場合、$e_i e_j \in a_i \cap a_j = \{0\}$、よって

$$
e_i = \sum_{j \in I} e_i e_j = e_i^2;
$$

最後に、$Ae_i \subset a_i$、すべての $i \in I$ と $\sum_{i \in I} Ae_i = A$、よって $Ae_i = a_i$ です。

$\overline{\omega}$ が全射であることを証明することはまだ残っています。 $(U_i)_{i \in I}$ を $P$ と集合 $Z_i = \bigcup_{j \neq i} U_j$ の元とします。 $U_i$と$Z_i$が閉じているため、$U_i = \mathrm{V}(a_i), Z_i = \mathrm{V}(b_i)$のような$A$の理想$a_i, b_i$が存在します。ここで、さらに $a_i \cap b_i = 0$ と仮定することが可能であることを示します。現在 $U_i \cap Z_i = \varnothing$、よって $a_i + b_i = A$; $a_i, b_i \in a_i, b_i$ を $a_i + b_i = 1$ となるようにします。次に、$X = U_i \cup Z_i = \mathrm{V}(a_i b_i)$ (公式 (3));したがって、$a_i b_i$ のすべての元は無能です (系 2 ～ 命題 11)。 $p$ を整数として、$a_i^p b_i^p = 0$ とします。それから$U_i \subset \mathrm{V}(Aa_i) = \mathrm{V}(Aa_i^p)$、

$$
Z_i \subset \mathrm{V}(Ab_i) = \mathrm{V}(Ab_i^p)
$$

そして $V(Aa_i) \cap V(Ab_i) = V(Aa_i + Ab_i) = \varnothing$、したがって $U_i = V(Aa_i^p)$ と $Z_i = V(Ab_i^p)$ により、主張置き換えること $a_i$ $Aa_i^p$ および $b_i$ $Ab_i^p$ が確立されます。このように選択された理想 $a_i$ と $b_i$ は、$\sigma$ が全単射であるという事実から、$1 = e_i + f_i, e_i f_i = 0, a_i = Af_i, b_i = Ae_i$ のような 2 つの冪等 $f_i \in a_i, e_i \in b_i$ が存在することがわかります。 $i \neq j$ の場合、$X = Z, \cup Z_j = V(Ae_i e_j)$ となり、$e_i e_j$ はべき等であるため、補題 2 は $e_i e_j = 0$ であることを示します。最後に、$e = \sum_{i \in I} e_i$ はべき等であり、すべての $i \in I$、よって $V(Ae) \subset Z$、すべての $i$ に対して $e_i \in Ae$ です。それは次のとおりです

$$
V(Ae) = \varnothing = V(A.1)
$$

補題 2 は $e = 1$ も示します。

#### 系 1 {#ac-ii-s4-lem-2-cor-1 .statement tag=04A7}

$A$ を環、$r$ を $A$ および $h : A \to A/r$ 標準準同型のゼロ理想とする。 $\sum_{i \in I} e'_i = 1$ となる$A/r$ の冪等の有限直交族 $(e'_i)_{i \in I}$ ごとに、すべての $i \in I$ に対して $\sum_{i \in I} e_i = 1$ と $h(e_i) = e'_i$ となる $A$ の冪等の有限直交族 $(e_i)_{i \in I}$ が存在します。

$A' = A/r$と書きます。私たちは次のことを知っています (命題 13 に続く注意)

$$
ah : \operatorname{Spec}(A') \to \operatorname{Spec}(A)
$$

は同型写像であり、$A$ 含む $r$ by 仮定のすべての素イデアルです。 命題 15 は、$A$ に $\sum_{i \in I} e_i = 1$ のような冪等の有限直交族 $(e_i)_{i \in I}$ が存在し、$V(A'(1 - e'_i))$ の $ah$ の下の像が $V(A(1 - e_i))$ であることを示しています。しかし明らかに $V(A(1 - e_i))$ は $ah$ の下の像でもあります

$$
V(A'(1 - h(e'_i)));
$$

$1 - e'_i$ と $1 - h(e_i)$ はべき等であるため、補題 2 は $e'_i = h(e_i)$、よって系を示します。

#### 系 2 {#ac-ii-s4-lem-2-cor-2 .statement tag=04A8}

環 $A$ の素スペクトル $X = \operatorname{Spec}(A)$ が接続されるためには、$A$ 含むが $0$ と $1$ 以外に冪等がないことが必要かつ十分です。

$X$が繋がっていないということは、$\varnothing$や$X$とは別個の開いた閉じた$X$集合が存在することを意味します。

### 4. 加群のサポート

#### 定義 5 {#ac-ii-s4-def-5 .statement tag=04A9}

$A$ を環 、$M$ を $A$ モジュールとします。 $M_p \neq 0$ が $M$ のサポートと呼ばれ、$\operatorname{Supp}(M)$ で示されるような、$A$ の主な理想の $p$ の集合 。

$A$ のすべての最大イデアルは素数であるため、直ちに § 3, no. 3、系 2 から定理 1 が続き、$A$ モジュール $M$ が $0$ に等しいためには、$\operatorname{Supp}(M) = \varnothing$ であることが必要かつ十分です。

#### 例 {#ac-ii-s4-n4-exa-1 .statement tag=04AA}

$a$ を $A$ の理想とします。 no. 3 の記法では、
$$
V(a) = \operatorname{Supp}(A/a).
$$
$p$ が $a \notin p$ となるような $A$ の素数である場合、$(A/a)_p = 0$ (§ 3, no. 1, 注意 3)。一方、$a \subset p$ の場合、$aA_p$ は $A$ の最大イデアル $pA_p$ に含まれており、$(A/a)_p$ は $A_p/aA_p$ と同型であるため、非ゼロ (§ 3, no. 1, 命題 3) になります。 よって私たちの主張。
特に$\operatorname{Supp}(A) = \operatorname{Spec}(A)$。

#### 命題 16 {#ac-ii-s4-prop-16 .statement tag=04AB}

$A$ を環とし、$M$ を $A$ モジュールとします。
(i) *$N$ が $M$ の部分加群である場合、*
$$
\operatorname{Supp}(M) = \operatorname{Supp}(N) \cup \operatorname{Supp}(M/N).
$$
(ii) *$M$ が部分加群の家族 $(N_i)_{i \in I}$ の和である場合、*
$$
\operatorname{Supp}(M) = \bigcup_{i \in I} \operatorname{Supp}(N_i).
$$
(i) 完全系列 $0 \to N \to M \to M/N \to 0$ から、$A$ の各素イデアル $p$ に対して、完全系列を導き出します。
$$
0 \to N_p \to M_p \to (M/N)_p \to 0
$$
(§ 2, no. 4、定理 1)。 $M$ が 0 に減少するには、$N_p$ と $(M/N)_p$ がゼロになることが必要かつ十分です。他の語, 関係 $p \notin \operatorname{Supp}(M)$ は「p $\notin \operatorname{Supp}(N)$ と $p \notin \operatorname{Supp}(M/N)$」に相当し、(i) を証明します。
(ii) $A$、$M$ の各素イデアル $p$ は、部分加群 $(N_i)_p$ (§ 2, no. 4) の族の和です。 $M, \neq 0$ ということは、$(N_i)_p \neq 0$、よってのような $i \in I$ が存在することを意味します (ii)。

#### 系 {#ac-ii-s4-n4-cor-1 .statement tag=04AC}

*$A$を環、$M$を$A$モジュール、$(m_i)_{i \in I}$を$M$の生成元の系、$a$、$m_i$の消滅子とします。それから*
$$
\operatorname{Supp}(M) = \bigcup_{i \in I} V(a_i).
$$
$\operatorname{Supp}(M) = \bigcup_{i \in I} \operatorname{Supp}(Am_i)$ by 命題 16 (ii)。一方、$Am_i$ は $A$ 加群 $A/a_i$ と同型であり、次のことがわかります。
$$
\operatorname{Supp}(A/a_i) = V(a_i)
$$
(上記例)。

#### 命題 17 {#ac-ii-s4-prop-17 .statement tag=04AD}

*$A$ を環、$M$ を $A$ モジュール、$a$ を消滅子とします。 $M$ が有限生成される場合、* $\operatorname{Supp}(M) = V(a)$ * および* $\operatorname{Supp}(M)$ * したがって、* $\operatorname{Spec}(A)$ に閉じられます。
$(m_i)_{1 \leq i \leq n}$ を $M$ の生成元の系とし、$a$ を $m_i$ の消滅子とします。 $a = \bigcap_{i=1}^n a_i$ なので、$V(a) = \bigcup_{i=1}^n V(a_i)$ (no. 3、方程式 (3)) となり、系から命題 16 に続き、命題になります。

#### 系 1 {#ac-ii-s4-prop-17-cor-1 .statement tag=04AE}

$A$ を環、$M$ を有限生成された $A$ モジュール、および $A$ の $a$ 元とします。 $M$ のサポートのすべての基本理想に対する $a$ から属するについては、$M$ のホモテティー が比 $a$ でゼロになることが必要かつ十分です。

It follows from Proposition 17 that the intersection of the prime ideals belonging to $\operatorname{Supp}(M)$ is the radical of the annihilator $a$ of $M$ (no. 3, Proposition 11 (ii)). この根基に対して $a$ 属するは、冪 $a^k \in a$ が存在し、したがって $a^k M = 0$ が存在するというというと同等です。

#### 系 2 {#ac-ii-s4-prop-17-cor-2 .statement tag=04AF}

$A$ をネーター 環、$M$ を有限生成された $A$ 加群、$a$ を $A$ の理想とする。 $\operatorname{Supp}(M) \subset V(a)$ の場合、$a^k M = 0$ となるような整数 $k$ が存在することが必要十分です。

$b$ が $M$ の消滅子である場合、関係 $\operatorname{Supp}(M) \subset V(a)$ は命題 17 による $V(b) \subset V(a)$ に相当し、したがって $a \subset r(b)$ に相当します。ここで、$r(b)$ は $b$ の根基です。 (no. 3、系 2 ～ 命題 11)。 $A$ はネーター なので、この条件は、$a^k \subset b$ (§ 2, no. 6, 命題 15) のように整数 $k > 0$ が存在することにも相当します。

#### 命題 18 {#ac-ii-s4-prop-18 .statement tag=04AG}

$M, M'$ を 2 有限生成加群環 $A$ とします。それから

$$
\operatorname{Supp}(M \otimes_A M') = \operatorname{Supp}(M) \cap \operatorname{Supp}(M').
$$

$p$ が $A$ の素イデアルである場合、関係 $(M \otimes_A M')_p \neq 0$ と "$M_p \neq 0$ と $M'_p \neq 0$" が同等であることを証明する必要があります。 $A_p$ 加群 $M, \otimes_{A_p} M'_p$ と $(M \otimes_A M')_p$ は同型 (§ 2, no. 7、命題 18) であるため、主張は次の補題から続きます。

#### 補題 3 {#ac-ii-s4-lem-3 .statement tag=04AH}

$B$ を局所環、$E$ および $E'$ の 2 つの有限生成された $B$ モジュールとします。 $E \neq 0$ と $E' \neq 0$ の場合は、$E \otimes_B E' \neq 0$ です。

$k$ を $B$ の剰余体とします。 § 3, no. 2、命題 4、$k \otimes_B E \neq 0$、$k \otimes_B E' \neq 0$ のおかげで。それから私たちはそれを推測します

$$
(k \otimes_B E) \otimes_k (k \otimes_B E') \neq 0
$$

(代数、章 II, § 3, no. 7)。しかし、テンソル積は結合的であるため (上記引用、§ 3, no. 8)、このテンソル積は次と同型です。

$$
E \otimes_B ((k \otimes_k k) \otimes_B E') = E \otimes_B (k \otimes_B E')
$$

したがって、$k \otimes_B (E \otimes_B E')$、よって補題になります。

#### 系 {#ac-ii-s4-n4-cor-2 .statement tag=04AI}

$M$ を有限生成された $A$ モジュール、$n$ をその消滅子とします。 $A$、$\operatorname{Supp}(M/aM) = V(a) \cap V(n) = V(a + n)$ のすべての理想 $a$ に対して。

$M/aM = M \otimes_A (A/a)$と$A/a$は有限に生成されます。

#### 命題 19 {#ac-ii-s4-prop-19 .statement tag=04AJ}

$A, B$ を 2 つの環、$\phi : A \to B$ 準同型とします。
$$
^{a}\phi : \operatorname{Spec}(B) \to \operatorname{Spec}(A)
$$
$\phi$ (命題 13) に関連付けられた連続する写像。 $A$ モジュール $M$ ごとに、
$$
\operatorname{Supp}(M_{(B)}) \subset ^{a}\phi(\operatorname{Supp}(M)) ; \text{if also } M \text{ is finitely generated, then}
$$
$$
\operatorname{Supp}(M_{(B)}) = ^{a}\phi^{-1}(\operatorname{Supp}(M)).
$$
$q$を$B$と$p = \phi^{-1}(q)$の主要な理想とします。 $q$ 属するから $\operatorname{Supp}(M_{(B)})$ とします。次に、$M_{(B)} \otimes_B B_q = (M \otimes_A B) \otimes_B B_q = M \otimes_A B_q = (M \otimes_A A_p) \otimes_A B_q$、準同型 $A \to B \to B_q$ 因子から $A \to A_p \to B_q$ (§ 2, no. 1、命題 2)。したがって、仮定 $M_{(B)} \otimes_B B_q \neq 0$ は、$M \otimes_A A_q \neq 0$、よっての最初の主張を意味します。 準同型 $\phi_q : A_p \to B_q$ はローカルであるため、2 番目の主張は次の補題から続きます。

#### 補題 4 {#ac-ii-s4-lem-4 .statement tag=04AK}

$A, B$ を 2 つの局所環、$p : A \to B$ をローカル準同型、$E$ を有限生成された $A$ モジュールとします。 $E \neq 0$ の場合は、$E_{(B)} \neq 0$。

$m$ を $A$ と $k = A/m$ 剰余体の最大理想とする。 仮定は $B \otimes_A k = B/mB \neq 0$ を意味します。 テンソル積は結合的であるため、$(E \otimes_A B) \otimes_A k$ は $E \otimes_A (B \otimes_A k)$ と同型であり、したがって $E \otimes_A (k \otimes_k (B \otimes_A k))$ にも、最後に $(E \otimes_A k) \otimes_k (B \otimes_A k)$ にも同型です。 § 3, no. 2、命題 4、$E \otimes_A k \neq 0$ により、したがって $(E \otimes_A B) \otimes_A k \neq 0$ (代数、章 II, § 3, no. 7) およびなおさら $E \otimes_A B \neq 0$。

#### 命題 20 {#ac-ii-s4-prop-20 .statement tag=04AL}

$A$を環、$M$を有限生成された$A$加群とする。すべての素イデアル $p \in \operatorname{Supp}(M)$ に対して、ゼロ以外の $A$ 準同型性 $w : M \to A/p$ が存在します。

$p \in \operatorname{Supp}(M)$ にしましょう。 $M$は有限生成され、$M_p \neq 0$は、
$$
M_p/pM_p = M_p \otimes_A (A_p/pA_p) \neq 0
$$
(§ 3, no. 2、命題 4)。 $K = A_p/pA_p$ を整域の $A/p$ の分数の体とします。 $M_p/pM_p$ は $K$ を超えるベクトル空間であり、0 に減らないため、非ゼロの線型形式 $u : M_p/pM_p \to K$ が存在します。 $(x_i)_1 <_n^*$ が $M$ の生成元の系、$x_i$ の $\bar{x}_i$ 像である場合、$(A/p)$ モジュール $M_p/pM_p$ には、元 $\alpha \neq 0$ が存在します。 $A/p$ は、$1 \leq i \leq n$ に対して $\alpha u(\bar{x}_i)$ 属するから $A/p$ になります。したがって、$v = \alpha u$ は、$M_p/pM_p$ から $A/p$ までの非ゼロの $(A/p)$ 線形マッピングです。 合成
$$
w : M \longrightarrow M, \longrightarrow M_p/pM_p \overset{v}{\longrightarrow} A/p
$$
したがって、 は必須の準同型です。

### 練習問題 {#ac-ii-s4-exercises}

(b) $n = \dim(M)$ とします。 次元 1 の M の直因子 (それぞれ $n - 1$) は *lines* (それぞれ超平面) と呼ばれます。 M の超平面 H が存在し、そのすべての元が $u$ の下で不変である場合、同一性と異なる自己同型 $u \in \mathbf{GL}(M)$ は *transvection* と呼ばれます。次に $u(x) = x + a\phi(x)$、ここで $\phi$ は M 上の線型形式で、$H = \mathrm{Ker}(\phi)$ と $a \in H$ になります。 逆を取得します。 A が可換である場合、行列式 1 のすべての自己同型 $u \in \mathbf{GL}(M)$ がトランスベクションの積であることを示します (M の任意の基底に関して、$u$ の行列において、すべての列含むが、 A の少なくとも 1 つの可逆元と形 $I + E_{ij} \ (i \neq j)$ の行列はトランスベクションの行列です)。

(c) $1 - u$ の核が M の直因子にならないように、自己同型 $u \in \mathbf{GL}(M)$ の例を与えます (A を形式的な冪系列の局所環 $K[[X]]$ とします) 1 つは体 K と $M = A$ で不確定です)。

(d) Give an example of direct factors N, P of M (necessarily free) such that $N + P$ and $N \cap P$ are not direct factors of M. (Take $A = K[X]/(X^2)$, where K is a field and $M = A^2$.)

¶ 15. A を (可換) 環および M A-加群とします。

(a) M の部分加群 M' が純粋 (章 I, § 2, 練習問題 24) であるためには、A のすべての最大理想 $m$ に対して、$M'_m$ が $M_m$ の純粋な部分加群であることが必要かつ十分です (次の定理 1 を使用します)。 no. 3）。

(b) A が局所環で、最大理想値 $m$ と M が有限生成自由A-加群であると仮定します。 有限生成された M の部分加群 M' が純粋であるためには、それが M の直因子であることが必要かつ十分です。 (no. 2 の系 1 から命題 5、簡約するから証明を使用すると、$M' \subset mM$ の場合、$M'$ のみが可能です$M' = 0$ の場合、M の純粋な部分加群になります。)

16. $(A_\lambda, f_{\mu\lambda})$ を局所環の直接系とし、$f_{\mu\lambda}$ がローカルの準同型となるようにします。 $m_\lambda$を$A_\lambda$と$K_\lambda = A_\lambda/m_\lambda$の最大の理想とする。すると、$A = \varprojlim A_\lambda$ は局所環で、その最大理想は $m = \varprojlim m_\lambda$ で、剰余体は $\bar{K} = \varprojlim K_\lambda$ です。さらに、$\lambda < \mu$に対して$m_\mu = A_\mu m_\lambda$なら、$m = Am$、すべて$\lambda$です。

94

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
