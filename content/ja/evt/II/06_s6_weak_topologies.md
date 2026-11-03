---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 6
section_title: Weak topologies
lang: ja
source: evt-i-v
book_pages: TVS II.40-TVS II.53, TVS II.81-TVS II.86
pdf_pages: 0077-0090, 0118-0123
extraction: ocr
subsections:
    - "no": 1
      title: Dual vector spaces
      page: 40
      pdf_page: 77
    - "no": 2
      title: Weak topologies
      page: 42
      pdf_page: 79
    - "no": 3
      title: Polar sets and orthogonal subspaces
      page: 44
      pdf_page: 81
    - "no": 4
      title: Transposition of a continuous linear mapping
      page: 46
      pdf_page: 83
    - "no": 5
      title: Quotient spaces and subspaces of a weak space
      page: 48
      pdf_page: 85
    - "no": 6
      title: Products of weak topologies
      page: 50
      pdf_page: 87
    - "no": 7
      title: Weakly complete spaces
      page: 51
      pdf_page: 88
    - "no": 8
      title: Complete convex cones in weak spaces
      page: 52
      pdf_page: 89
statements: 41
exercises: 20
content_sha256: d8e8e86ece27da32f8291059f364c1280cdd40476ab715630417fa9608396d4d
translated_from: content/en/evt/II/06_s6_weak_topologies.md
translation_method: google
source_content_sha256: 99514709d3c5833b248b220057a632a5ff5dc72f7ecf8af9bb7a09eddc3274a1
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 1407a3e9bdaa1247e093b45efb70fc5ddaa43a817a429412957fb0b598d84775
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 6。弱いトポロジー

### 1. デュアルベクトル空間

$F$ と $G$ を 2 つの実数ベクトル空間とし、$(x, y) \mapsto B(x, y)$ を $F \times G$ 上の*双線形* 形とします。 双線形形式 $B$ *ベクトル空間* $F$ *および* $G$ *双対性*を置く、または F と G が (B に対して) 双対性であると言います。 $B(x, y) = 0$ の場合、$x \in F$ と $y \in G$ は (B によって定義される双対性について) 直交すると言うことを思い出してください。すべての $x \in M$ がすべての $y \in N$ (A, IX, § 1.2) に直交する場合、F の部分集合 M と G の部分集合 N は直交すると言います。

B によって定義される双対性が、次の条件を満たす場合、F (それぞれ G) で分離していると言います。

(D_I) *F のすべての $x \neq 0$ に対して、$B(x, y) \neq 0$ となるような $y \in G$ が存在します。* (それぞれ

(D_{II}) *G のすべての $y \neq 0$ に対して、$B(x, y) \neq 0$ となる $x \in F$ が存在します。)

B によって定義される双対性は、F と G の両方で分離している場合、分離していると言われます。そのためには、双線形形式 B が A、IX, § 1.1 の意味で分離していることが必要かつ十分です。より正確には、次の結果が得られます。

#### 命題 1 {#evt-ii-s6-prop-1 .statement tag=07H0}

*F、Gを$F \times G$上の2つの実数ベクトル空間とB双線形形式とする。しましょう*

$$
d_B : y \mapsto B(., y),
$$
$$
s_B : x \mapsto B(x, .)
$$

*F の双対 $F^*$ における G の線形写像と、G の双対 $G^*$ における F の線形写像は、それぞれ B* (A, IX, § 1.1) の右側と左側に関連付けられます。次に、$d_B$ (それぞれ $s_B$) が単射である場合に限り、B は F と G を G (それぞれ F) で分離する双対関係に置きます。*

F と G が B による分離双対に置かれるとき、多くの場合、$s_B$ (それぞれ $d_B$) によって $G^*$ (それぞれ $F^*$) の部分空間を伴う同一視する F (それぞれ G) になります。この識別がどのように行われるかを指定せずに、F (または G) を $G^*$ (それぞれ $F^*$) の部分空間とみなすとき、私たちは常に前述の識別を使用します。 双線形形式 B は、正規の双線形形式の制限から $F \times G$ と識別されます。

$$
(x^*, x) \mapsto \langle x, x^* \rangle \quad (\text{resp. } (x, x^*) \mapsto \langle x, x^* \rangle).
$$

#### 例 {#evt-ii-s6-n1-exa-1 .statement tag=07H1}

— 1) E をベクトル空間とし、E* をその双対とする。 $E \times E^*$ (A, II, § 2.3) 上の正規の双線形形式 $(x, x^*) \mapsto \langle x, x^* \rangle$ は、E と E* を分離双対に置きます: for (D_{II}) は、関係 $x^* \neq 0$ の定義のため真であり、もう一方ではわかっています一方、E のすべての $x \neq 0$ に対して、$\langle x, x^* \rangle \neq 0$ (A, II, § 7.5, th. 6) となる線型形式 $x^* \in E^*$ が存在し、これは (D_I) を証明します。 E と $E^{**}$ の部分空間の同一性は、標準写像 $c_E$ (*loc. cit.*) によってここで行われます。

E が *有限* 次元であるとき、正準双線形形式の制限から $E \times G$ によって双対性を分離している E* の * 唯一の* 部分空間 G は、空間 E* 自体です。なぜなら、E は正規的に $E^{**}$ (*loc. cit.*) と識別され、$G \neq E^*$ があれば、すべての $x^* \in G$ (A, II, § 7.5, th. 7) に対して $\langle a, x^* \rangle = 0$ となるように E に $a \neq 0$ が存在することになり、これは矛盾する仮定。

2) E が *無限* 次元ベクトル空間で、E' が E* のベクトル部分空間であるとき、標準双線形形式の制限から $E \times E'$ によって定義される E と E' の双対性は常に E' で分離します。 $E' \neq E^*$でもEで区切ることができます。最も重要なケースは、E がトポロジカルベクトル空間である場合に発生します。

#### 定義 1 {#evt-ii-s6-def-1 .statement tag=07H2}

— *位相的なベクトル空間 E の双対とは、E* の部分空間 E'、E 上の連続線型形式によって形成されるベクトル空間 E の双対を意味します。

E が *ハウスドルフの局所凸* 空間であるとき、E とその双対 E' の間の双対性は分離しています。これは、ハーン・バナッハ定理 (II, p. 24, cor. 1) から導き出され、E のすべての $x \neq 0$ に対して、次のような $x' \in E'$ が存在します。 $\langle x, x' \rangle \neq 0$。

#### 注意 {#evt-ii-s6-n1-rem-1 .statement tag=07H3}

— 1) E が *トポロジー* ベクトル空間である場合、*ベクトル空間* E の双対 $E^*$ は、混乱を避けるために E の *代数双対 * と呼ばれます。また、$E^*$ は、E に *最も細かい* 局所凸型位相 (II, p. 25, *例* 2) を与えることによって得られるトポロジカルベクトル空間の双対であることにも注意します。
2) トポロジカルベクトル空間の双対 E' 自体は位相、〜でない限りを持ちません。これは明示的に述べられています。
3) F と $G \subset F^*$ が正準双線形形式によって双対性を分離している場合、これは、$G \subset G_1$ などの $F^*$ のすべての部分空間 $G_1$ について、F と $G_1$ にも当てはまります。

### 2. 弱いトポロジー

#### 定義 2 {#evt-ii-s6-def-2 .statement tag=07H4}

— *F と G を 2 つのベクトル空間とし、双線形形式 B によって双対性を持たせます。すべての線型形式 $B(., y): x \mapsto B(x, y)$ を連続にする F 上の最も粗い位相 (y は G 内で変化します) を、F と G の双対性によって定義される F 上の弱い位相と呼び、それを $\sigma(F, G)$ で表します。

同様に、G、交換すること F、および定義 1 の G で弱い位相 $\sigma(G, F)$ を定義するとします。この交換すること F と G の可能性は、この段落で続くすべての結果と定義に当てはまります。

混同の可能性がない限り、弱い位相 $\sigma(F, G)$ に関連する性質を表すために、形容詞「弱い」と副詞「弱い」を使用します。たとえば、「弱い収束」や「弱い連続写像」などについて説明します。

$G \subset F^*$ の場合、記法 $\sigma(F, G)$ は常に、標準双線形形式 $(x, x^*) \mapsto \langle x, x^* \rangle$ の双対性対応する ～ 制限 $F \times G$ によって定義される弱い位相を表します。

F と G に追加の仮説を立てない場合、曖昧さがない限り、$(x, y)$ で双線形形式 B の値 $B(x, y)$ に対して $\langle x, y \rangle$ と書くことがよくあります。この段落の残りの部分ではこの規約を採用します。

$\sigma(F, G)$ の弱い位相を運ぶベクトル空間 F は *弱い空間* と呼ばれます。

弱い位相 $\sigma(F, G)$ は *局所的に凸* (II、p. 26、提案 4) ;より正確には、$\mathbf{R}^G$ の F の線形写像 $\phi : x \mapsto (\langle x, y \rangle)_{y \in G}$ による $\mathbf{R}^G$ の *積* 位相の逆像です。 y が G (II, p. 5) で変化する場合、*準ノルム* $x \mapsto |\langle x, y \rangle|$ の集合によって定義されます。 G の点のすべての $\alpha > 0$ とすべての有限族 $(y_i)_{1 \leq i \leq n}$ について、$W(y_1, ..., y_n; \alpha)$ を $1 \leq i \leq n$ に対して $|\langle x, y_i \rangle| \leq \alpha$ となるように $x \in F$ の集合とします。これらの集合 ($\alpha, n$ および $y_i$ は任意) 形は、$\sigma(F, G)$ の * 0 の近傍の * 基本的な系です。 $W(y_1, ..., y_n; \alpha)$ 含むは、*有限*余次元の F の *ベクトル部分空間* であることに注意してください。これは、$1 \leq i \leq n$ に対する方程式 $\langle x, y_i \rangle = 0$ によって定義されます。

#### 命題 2 {#evt-ii-s6-prop-2 .statement tag=07H5}

— *弱い位相* $\sigma(F, G)$ *$F$ * と* $G$ * の間の双対性が * $F$ で分離している場合に限り、ハウスドルフです。

これは、II、p. 3、プロップの特殊なケースです。 2.

#### 命題 3 {#evt-ii-s6-prop-3 .statement tag=07H6}

— *$F$ *と* $G$ *を双対性における 2 つの実数ベクトル空間とします。 * $F$ のすべての線型形式、*それは $\sigma(F, G)$ にわたって連続し、* $x \mapsto \langle x, y \rangle$ * 一部の* $y \in G$ として書くことができます。 *元* $y \in G$ *二元性が* $G$ で分離しているときはユニークです。

なぜなら、$F$の線型形式$f$が$\sigma(F, G)$に対して連続であるということは、$F$、$|f(x)| \leq \sup_{1 \leq i \leq n} |\langle x, y_i \rangle|$のすべての$x$について、点$y_i \in G$($1 \leq i \leq n$)の有限集合が存在することを意味するからです。 (II、p. 6、提案5)。したがって、$n$ 関係 $\langle x, y_i \rangle = 0$ ($1 \leq i \leq n$) は $f(x) = 0$ を暗示し、したがって (A, II, § 7.5, cor. 1)、すべての $x \in F$ に対して $f(x) = \langle x, y \rangle$ となるような線形結合 $y = \sum_{i=1}^n \lambda_i y_i$ が存在します。 一意性は (D$_\text{II}$) から続きます。

言い換えれば、双対性が $G$ で分離し、$F$ がトポロジー $\sigma(F, G)$ を持つ場合、このトポロジーの $F$ の双対と正準的に $G$ を識別できます (II、p. 42、def. 1)。

#### 系 1 {#evt-ii-s6-prop-3-cor-1 .statement tag=07H7}

— *家族* $(a_i)$ *of 点 of* $F$ *は位相* $\sigma(F, G)$ の合計です *すべて* $y \neq 0$ *in* $G$、 *添字* $i$ *そのような* $\langle a_i, y \rangle \neq 0$が存在します。

プロップを使用するため。 3とI、p. 13、th。 1、性質は、$\sigma(F, G)$に対して超平面含むすべての$a_i$が閉じていないという事実を表します。したがって、系は cor から続きます。 II、p. 38 の 3 つ。

#### 系 2 {#evt-ii-s6-prop-3-cor-2 .statement tag=07H8}

— *ファミリー* $(a_i)$ *of 点 of* $F$ *は位相* $\sigma(F, G)$ に対してトポロジー的に独立しており、*場合に限り、すべての添字* $i$ に対して、 *元* $b_i \in G$ *が存在する* : $\langle a_i, b_i \rangle \neq 0$ *および* $\langle a_\kappa, b_i \rangle = 0$ *すべて* $\kappa \neq i$。

これは、すべての $i$ に対して、$\sigma(F, G)$ には閉じた超平面が存在し、含む添字 $\kappa \neq i$ を含むすべての $a_\kappa$ が存在しますが、含む $a_i$ には存在しません。

#### 系 3 {#evt-ii-s6-prop-3-cor-3 .statement tag=07H9}

— ** $G_1$ * と* $G_2$ * を、* $F^*$ の 2 つのベクトル部分空間とし、* $F$ * (正規の双線形形式の制限の場合)* と* します。 *その場合* $\sigma(F, G_2)$ *は $\sigma(F, G_1)$ よりもより細かいです *もし、そしてその場合に限り* $G_1 \subset G_2$。

条件で十分なのは明らかです。逆に、$\sigma(F, G_2)$ が $\sigma(F, G_1)$ よりもより細かいである場合、$\sigma(F, G_1)$ に対して連続するすべての線型形式は、$\sigma(F, G_2)$ に対しても連続であるため、プロパティにより $G_1 \subset G_2$ になります。 3.

#### 系 4 {#evt-ii-s6-prop-3-cor-4 .statement tag=07HA}

— *$G$ *を双対* $F^*$ のベクトル部分空間、*ベクトル空間* $F$ とします。 *その後* $F$ *と* $G$ *は分離双対性* (正準双線形形式の場合) *場合に限り* $G$ * $F^*$ * 位相* $\sigma(F^*, F)$ に密集しています。

これは cor から続きます。 1.

### 3. 極性集合および直交性部分空間

#### 定義 2 {#evt-ii-s6-def-2-bis .statement tag=07HB}

F と G を双対性において 2 (実数) ベクトル空間とします。 F のすべての集合 M について、すべての $x \in M$ について $\langle x, y \rangle \geq -1$ であるそれらの y ∈ G の M の極点を集合と呼びます。 (複合体ベクトル空間、cf. II、p. 64 の場合。)

$G_1, G_2$ が $G_1 \subset G_2$ のような $F^*$ の 2 つの部分空間である場合、$G_1$ の M の極は、$G_2$ の M の極と $G_1$ の交点になります。

混乱の危険がない場合、F の部分集合 M の G の極性を表すために $M^\circ$ を使用します。同様に、G の集合の F の極性を定義する使用します。

明らかに、すべてのスカラー $\lambda \neq 0$ とすべての $M \subset F$ に対して、$(\lambda M)^\circ = \lambda^{-1} M^\circ$ が得られます。 関係 $M \subset N \subset F$ は $N^\circ \subset M^\circ$ を意味します。 N が M を吸収する場合、$M^\circ$ は $N^\circ$ を吸収します。すべての家族について、F の集合の $(M_\alpha)$ は、$\bigcup \alpha M_\alpha$ の極集合は、極集合 $M_\alpha^\circ$ の共通部分です。 $y \in M^\circ$ の場合、閉じた半空間は関係 $\langle x, y \rangle \geq -1$ 含む 0 と M によって定義されるため、$M_1$ が $M \cup \{0\}$ の凸包絡線である場合、$M_1^\circ = M^\circ$ であることがわかります。

明らかに$M \subset M^{\circ \circ}$。したがって、
$$
(M^{\circ \circ})^\circ \subset M^\circ \subset (M^\circ)^{\circ \circ} = (M^{\circ \circ})^\circ
$$
つまり、$M^{\circ \circ \circ} = M^\circ$ (cf. S、III, § 1.5、提案 2)。

M が F の対称部分集合である場合、$M^\circ$ は G の対称部分集合です。この場合、$M^\circ$ は $y \in G$ の集合であり、すべての $x \in M$ に対して $|\langle x, y \rangle| \leq 1$ になります。

#### 命題 4 {#evt-ii-s6-prop-4 .statement tag=07HC}

(i) F の任意の集合 M について、極集合 $M^\circ$ は含む 0 である凸集合であり、位相 $\sigma(G, F)$ では G で閉じられます。

(ii) M が頂点 0 の円錐である場合、$M^\circ$ は頂点 0 の円錐であり、すべての $x \in M$ に対して $\langle x, y \rangle \geq 0$ となるように、$y \in G$ の集合でもあります。

(iii) M が F のベクトル部分空間である場合、$M^\circ$ は G のベクトル部分空間であり、すべての $x \in M$ に対して $\langle x, y \rangle = 0$ となるように、$y \in G$ の集合でもあります。

(i) 線型形式 $y \mapsto \langle x, y \rangle$ は $\sigma(G, F)$ に対して連続であるため、定義からすぐに主張が​​得られ、超平面で決まる半空間が凸であることがわかります。

(ii) M が頂点 0 の円錐で、$x \in M, y \in M^\circ$ の場合、$\lambda x \in M$ として、すべての $\lambda > 0$ に対して、$\langle \lambda x, y \rangle \geq -1$、つまり $\lambda \langle x, y \rangle \geq -1$ が得られます。これはすべての$\lambda > 0$に当てはまるので、$\langle x, y \rangle \geq 0$となり、(ii)が証明されます。

(iii) 同様に、M が F のベクトル部分空間である場合、関係 $x \in M, y \in M^\circ$ は、今度は、すべての実数 $\lambda$ に対して $\lambda \langle x, y \rangle \geq -1$ を意味しますが、これは $\langle x, y \rangle = 0$ の場合にのみ可能です。

M が F のベクトル部分空間である場合、$M^\circ$ は G における M の直交であると言います。 $G \subset F^*$の場合、$M^\circ$はGの共通部分であり、Fの代数双対$F^*$においてMに直交する部分空間です(A、II, § 2.4、定義4)。

F のベクトル部分空間 M と G のベクトル部分空間 N について、$M \subset N^o$ (または同等に、$N \subset M^\circ$ の場合) の場合、M と N は直交すると言います。

#### 定理 1 (双極性障害定理) {#evt-ii-s6-thm-1 .statement tag=07HD}

F、G を双対性における 2 つの実数ベクトル空間とする。 F の部分集合 M ごとに、G の M の極集合 $M^\circ$ の F の極集合 $M^{\circ \circ}$ は、$M \cup \{0\}$ の閉じた凸包絡線 ($\sigma(F, G)$ の場合) です。

$M$ が凸であり、$0 \in M$ の場合だけを考慮する必要があることがわかりました。 $M$の位相$\sigma(F, G)$の閉包を$\overline{M}$で表すと、$\overline{M}$は$F$の凸集合になります。小道具。 II、p. 44の4は$M^{\circ\circ} \supseteq \overline{M}$を示しています。 一方、$a \in F$ が属するから $\overline{M}$ にならない場合、$F$ に閉じた超平面 $H$ が存在し、$a$ を $\overline{M}$ から厳密に分離します (II、p. 38、提案 4)。 $H$ は含む 0 ではないので、$H$ が方程式 $\langle x, y \rangle = -1$ (II, p. 43、提案 3) を持つような $y \in G$ が存在します。したがって、$x \in \overline{M}$ と $\langle a, y \rangle < -1$ はすべて $\langle x, y \rangle > -1$ となります。 これは、$y \in M^\circ$ と $a \notin M^{\circ\circ}$、そして関係 $M^{\circ\circ} = \overline{M}$ が続くことを意味します。

#### 系 1 {#evt-ii-s6-thm-1-cor-1 .statement tag=07HE}

*任意の家族* $(M_\alpha)$ *閉じた凸型集合 of* $F$ *(in 位相* $\sigma(F, G)$*)、それぞれの含む* 0、*極集合の共通部分* $M = \bigcap \limits_{\alpha} M_\alpha$ *は凸型閉じた包絡線* (*の* $\sigma(G, F)$) * 和集合の * $M_\alpha^\circ$。

なぜなら、$N$ がこの凸型の閉じたエンベロープである場合、

$$
N^\circ = \bigcap \limits_{\alpha} M_\alpha^{\circ\circ} = \bigcap \limits_{\alpha} M_\alpha = M
$$

よって $N = N^{\circ\circ} = M^\circ$。

コルの結論。 $M_\alpha$が凸でない場合は必ずしも1が成り立つわけではありません。

#### 系 2 {#evt-ii-s6-thm-1-cor-2 .statement tag=07HF}

*各ベクトル部分空間* $M$ *の* $F$、*部分空間* $M^{\circ\circ}$ *は、位相* $\sigma(F, G)$の* $M$ *の終結です。

#### 注意 {#evt-ii-s6-n3-rem-1 .statement tag=07HG}

— トポロジー $\sigma(G, F)$ の $G$ の 0 のすべての近傍には、$|\langle x_i, y \rangle| \leq 1$ ($1 \leq i \leq n$) の形式の有限数の不等式によって定義される近傍 $V$ が含まれます。ここで、$x_i$ は $F$ の任意の点です。 $A$ が $x_i$ の集合の *対称凸包絡線* である場合、 $V$ は $G$ の $A$ の *極性集合* $A^\circ$ です。 $F$ の有限対称集合の * $G$ の *極子 (またはその凸包絡線) は、$\sigma(G, F)$ の $G$ の 0 の基本的な近傍系を形成していると言えます。 双対性が $F$ で分離している場合、これらの凸型エンベロープは、$\sigma(F, G)$ (II、p. 14、提案 15 の cor. 1) および有限次元に対して *コンパクト* になります。 逆に、$F$ の有限次元* $C$ のすべての *コンパクトな凸集合 ($\sigma(F, G)$ 位相を含む) は、$F$ の *有限部分集合* の凸包絡線に含まれます。 というのは、$M$ を有限次元含む $C$ のベクトル部分空間とします。 $(e_i)_{1 \leq i \leq n}$ が $M$ の基底である場合、$C$ は閉平行面中心 0 に含まれており、基底 $e_i$ (GT, VI, § 1.3) のベクトル上に構築されていると仮定できます。今、この平行面は点 $\sum \limits_{i=1}^n \varepsilon_i e_i$ と $\varepsilon_i = \pm 1$ の凸包絡線である明らかです。

したがって、($\sigma(F, G)$ がハウスドルフの場合) * $F$ における有限次元、凸、コンパクトな集合の極 ($\sigma(F, G)$ または任意のハウスドルフの局所的に凸な位相より細かいについては、$F$ 上の $\sigma(F, G)$ よりも) と言えます。 形 $\sigma(G, F)$ の 0 の近傍の基本的な系。

#### 系 3 {#evt-ii-s6-thm-1-cor-3 .statement tag=07HH}

*$\mathscr{T}$ * を局所凸型空間* $E$ の位相とし、* $E'$ * その双対* (II、p. 42、def. 1) とします。

(i) E の *閉じた凸集合は、位相 $\mathscr{T}$ と弱い位相 $\sigma(E, E')$ で同じです。

(ii) *E の部分集合 M ごとに、$E'$ の M の極集合 $M^\circ$ の E の極集合 $M^{\circ\circ}$ は、位相 $\mathscr{T}$ の$M \cup \{0\}$ の凸閉包絡線です。

明らかに、(ii) は (i) と th から導かれます。 1. デュアル$E'$の定義から、II、p. 43、プロップに続きます。 3 位相 $\mathscr{T}$ の E の連続線型形式は、$\sigma(E, E')$ の連続線型形式と同じであることがわかります。したがって、E の閉じた半空間は、$\mathscr{T}$ と $\sigma(E, E')$ (II、p. 15、提案 17) で同じであり、主張 (i) は、II、p. 38、cor から続きます。 1.

### 4. 連続した線形写像の移調

この No. では、(F, G) と $(F_1, G_1)$ が双対性のある 2 つのベクトル空間であると仮定します。

#### 命題 5 {#evt-ii-s6-prop-5 .statement tag=07HI}

*あなたを$F_1$のFの線形写像とします。次のプロパティは同等です:*

a) *u は、弱いトポロジ $\sigma(F, G)$ および $\sigma(F_1, G_1)$ では連続です;*

b) *次のような写像 $v : G_1 \to G$ が存在します*

$$
\langle u(y), z_1 \rangle = \langle y, v(z_1) \rangle
$$

すべての $y \in F$ と $z \in G_1$ に対して。

*これらの性質が成り立つと、F と G の双対性が G で分離している場合、写像 v 満たす (1) は一意であり、v は線形です。*

u が弱いトポロジーに対して連続である場合、すべての $z_1 \in G_1$、線型形式 $y \mapsto \langle u(y), z_1 \rangle$ について、F 上の $\sigma(F, G)$ に対して連続であるため、(II, p. 43、提案 3) は $v(z_1) \in G$ を伴う $y \mapsto \langle y, v(z_1) \rangle$ として書くことができ、これは a) が b) を意味することを示しています。逆に、b) が true の場合、すべての $z_1 \in G_1$、線型形式について、

$$
y \mapsto \langle y, v(z_1) \rangle = \langle u(y), z_1 \rangle
$$

は $\sigma(F, G)$ に対して連続です。弱いトポロジの定義から、u は $\sigma(F, G)$ および $\sigma(F_1, G_1)$ に対して連続であることがわかります (I、p. 10、cor. 1)。 v の一意性は (D_{II}) から得られ、この一意性は v が線形であることを意味します。

#### 注意 {#evt-ii-s6-n4-rem-1 .statement tag=07HJ}

— F と G の双対性が G で分離し、$F_1$ と $G_1$ の双対性が $G_1$ で分離すると仮定します。 同一視する G と $G_1$ を、それぞれ $F^*$ と $F_1^*$ の部分空間とすると、条件 a) と b) は $^t u(G_1) \subset G$ と等価です。 v は、u (A、II, § 2.5) から $G_1$ の転置 $^t u$ の制限です。

単純に（混乱の可能性がない場合）、v は u の *転置* であると言い（一方では F と G の間、他方では $F_1$ と $G_1$ の間の双対性に対して）、それを表すために再び $^t u$ を使用します。

#### 系 {#evt-ii-s6-n4-cor-1 .statement tag=07HK}

*F と G の双対性が G で分離しているとします。u が $F_1$ の F の線形写像であり、$\sigma(F, G)$ と $\sigma(F_1, G_1)$ の間連続である場合、* 転置は $G$ の $G_1$ の線形写像であり、 $\sigma(G_1, F_1)$と$\sigma(G, F)$。さらに、$F_1$ と $G_1$ の二重性が $F_1$ で分離すると、${}^t({}^t u) = u$ になります。

$F$ と $F_1$ をプロップの $G$ と $G_1$ に交換するだけで十分です。 5.

#### 命題 6 {#evt-ii-s6-prop-6 .statement tag=07HL}

*$F$ と $G$ (それぞれ $F_1$ と $G_1$) の間の二重性が $G$ (それぞれ $F_1$) で分離すると仮定します。 $\sigma(F, G)$と$\sigma(F_1, G_1)$に連続する$F_1$の$F$の線形写像を$u$とします。 $A$ を $F$ では集合とし、$F_1$ では $A_1$ 集合とします。それから*：

(i) *$(u(A))^{\circ} = {}^t u^{-1}(A^{\circ})$があります*。

(ii) *${}^t u(A_1^{\circ}) \subset (u^{-1}(A_1))^{\circ}$ があります。さらに、$A$ が閉じていて、($\sigma(F_1, G_1)$ の場合) 凸であり、含むが原点である場合、${}^t u(A_1^{\circ}) = (u^{-1}(A_1))^{\circ}$ が得られます。*

$z_1 \in G_1$、関係 $z_1 \in (u(A))^{\circ}$ がすべての $y \in A$ についての $\langle u(y), z_1 \rangle \geq -1$ と等価であり、関係 ${}^t u(z_1) \in A^{\circ}$ がすべての $y \in A$ について$\langle y, {}^t u(z_1) \rangle \geq -1$ と同等であるとし、主張 (i) は (1) を使用して続きます。次の交換すること $u$ と ${}^t u$ と適用 (i) から $G_1$ の集合 $A_1^{\circ}$ が得られます

$$
({}^t u(A_1^{\circ}))^{\circ} = u^{-1}(A_1^{\circ \circ}) \supset u^{-1}(A_1)
$$

そこから極点を取ると

$$
({}^t u(A_1^{\circ}))^{\circ \circ} \subset (u^{-1}(A_1))^{\circ} .
$$

双極性障害定理 (II、p. 44、th. 1) によって ${}^t u(A_1^{\circ}) \subset ({}^t u(A_1^{\circ}))^{\circ \circ}$ が得られます。最後の主張は (2) から続き、双極性定理はそれ以降 $A_1^{\circ \circ} = A_1$ と ${}^t u(A_1^{\circ})$ が凸で、含むが原点です。

#### 系 1 {#evt-ii-s6-prop-6-cor-1 .statement tag=07HM}

※支柱記法付き。 6、関係 $u(A) \subset A_1$ は ${}^t u(A_1^{\circ}) \subset A^{\circ}$ を意味します。さらに $A_1$ が凸で閉じており ($\sigma(F_1, G_1)$ の場合)、および含むが原点である場合、これら 2 つの関係は同等です。*

実際、関係 $u(A) \subset A_1$ は $A \subset u^{-1}(A_1)$ と同等であるため、

$$
{}^t u(A_1^{\circ}) \subset {}^t u(A_1^{\circ}) \subset (u^{-1}(A_1))^{\circ} \subset A^{\circ}
$$

逆に、関係 ${}^t u(A_1^{\circ}) \subset A^{\circ}$ は暗黙的に意味します

$$
A^{\circ \circ} \subset ({}^t u(A_1^{\circ}))^{\circ} = u^{-1}(A_1^{\circ \circ})
$$

(2)から。 $A_1 = A_1^{\circ \circ}$ の場合、$A \subset u^{-1}(A_1)$ であると推測されます。

#### 系 2 {#evt-ii-s6-prop-6-cor-2 .statement tag=07HN}

※$u$を$\sigma(F, G)$と$\sigma(F_1, G_1)$に続く$F_1$の$F$の線形写像とします。それから*

(3)

$$
\operatorname{Ker}({}^t u) = (\operatorname{Im}(u))^{\circ} ,
$$

(4)

$$
\overline{\operatorname{Im}({}^t u)} = (\operatorname{Ker}(u))^{\circ} .
$$

*$F$ と $G$ の間、および $F_1$ と $G_1$ の間の双対性が分離していると仮定します。その場合、${}^t u$が単射である場合に限り、$u(F)$は$F_1$($\sigma(F_1, G_1)$の場合)で密になります。*

プロップを適用します。弱いトポロジ $\sigma(G, F)$ と $\sigma(F_1, G_1)$ がハウスドルフであるという事実を利用して、$A = F$ と $A_1 = \{0\}$ で 6 を計算します。 最後の主張は (4)、交換すること $u$ および $^t u$ の結果です。

### 5. 弱い空間の商空間と部分空間

$F, G$ を双対性における 2 つの実数ベクトル空間とします。 $M$ を $F$ のベクトル部分空間とし、$G$ の直交$M^\circ$ の部分空間 $N$ を考えます。 $y_1, y_2$ が合同 mod である $G$ の 2 つの点である場合。 $x \in M$すべてに対して$N$、次に$\langle x, y_1 \rangle = \langle x, y_2 \rangle$。それぞれ類 $\dot{y}$ mod。 $N$、$y$が$\dot{y}$で$\langle x, \dot{y} \rangle$ずつ変化するとき、$\langle x, y \rangle$の共通の値を表します。明らかに$(x, \dot{y}) \mapsto \langle x, \dot{y} \rangle$は$M \times (G/N)$の双線形形式です。

#### 命題 7 {#evt-ii-s6-prop-7 .statement tag=07HO}

— *$M$を$F$のベクトル部分空間と$G$の$N$ベクトル部分空間とし、$F$と$G$は双対性の2つのベクトル空間です。 $M$ と $N$ が直交しているとします (これは、という、$N \subset M^\circ$、または $M \subset N^\circ$ に相当します)。 ベクトル空間 $M$ と $G/N$ は、双線形形式* $(x, \dot{y}) \mapsto \langle x, \dot{y} \rangle$ によって二重性になります。

(i) *位相 $\sigma(M, G/N)$ は、この双対性が $\sigma(F, G)$ によって引き起こされるためです (特に $\sigma(F, G) = \sigma(F, G/F^\circ)$ があります)。

(ii) *この双対性の位相 $\sigma(G/N, M)$ は、$\sigma(G, F)$ の商位相より$N$ 粗い。これらのトポロジは、$M + G^\circ = N^\circ$ の場合にのみ同一です。

(i) $G/N$ のすべての元は類 mod です。 $N$/元/$G$; $z_i (1 \leq i \leq n)$ が $G$ の元で、$\dot{z}_i (1 \leq i \leq n)$ が $G/N$ の $z_i$ の類である場合、 $1 \leq i \leq n$ の $|\langle y, \dot{z}_i \rangle| \leq \alpha$ が $y \in M$ の集合になります。 $x \in F$ のうち集合のうち $M$ は、$1 \leq i \leq n$ に対して $|\langle x, z_i \rangle| \leq \alpha$ になります。結論は、弱者位相の 0 の近傍の定義から得られます。

(ii) $p : G \to G/N$ を標準全射とします。 *商位相* $\mathscr{T}$ *of* $\sigma(G, F)$ *by* $N$ *が $\sigma(G/N, N^\circ)$ と同一であることを示します。 $z \in G, y \in N^\circ$ には $\langle y, p(z) \rangle = \langle y, z \rangle$ があるため、$\sigma(G/N, N^\circ)$ の 0 のすべての近傍は形 $p(V)$ になります。ここで、$V$ は $\sigma(G, F)$ の 0 の近傍が関係で飽和します。 $z - z' \in N$ なので、$\mathscr{T}$ は $\sigma(G/N, N^\circ)$ よりもより細かいになります。 逆に、$U = W(y_1, ..., y_n; \alpha)$ を $\sigma(G, F)$ の $G$ の 0 の近傍とし、$1 \leq i \leq n$ と $\alpha > 0$ の場合は $y_i \in F$ とします。 $1 \leq i \leq n$ には元 $t_i \in N^\circ$ が存在し、$U' = W(t_1, ..., t_n; \alpha)$ を置くと $p(U') \subset p(U)$ となることがわかります。これは、$\sigma(G/N, N^\circ)$ が $\mathscr{T}$ よりもより細かいであるため、実際には $\mathscr{T}$ と同一であることがわかります。 ここで、$L$ を $N^\circ$ と $y_i$ によって生成された $F$ のベクトル部分空間とし、$L$ の $N^\circ$ の補数部分空間を$P$ で示します。それは有限次元、例えば$m$です。 $(x_j)_{1 \leq j \leq m}$ を $P$ の基底とします。線形形式 $x \mapsto \langle x_j, z \rangle$ の $N$ に対する制約は線形独​​立です。そうでない場合、すべての $z \in N$、つまり $x \in N^\circ$ に対して $\langle x, z \rangle = 0$ となるような $P$ に $x \neq 0$ が存在し、$P$ の定義と矛盾します。 したがって、すべての $z' \in G$ に対して、すべての $j$ に対して $\langle x_j, z' \rangle = \langle x_j, s \rangle$ となるような $s \in N$ が存在すると結論付けます。 $z' = z + s$ の場合、すべての $x \in P$ に対して $\langle x, z \rangle = 0$ が得られます。 したがって、$t_i \in N^\circ$ と $w_i \in P$ に $y_i = t_i + w_i$ を入れます。 $1 \leq i \leq n$には$\langle y_i, z \rangle = \langle t_i, z \rangle = \langle t_i, z' \rangle$があります。したがって、すべての $z' \in U'$ に対して、$z' - z \in N$ となるような $z \in U$ が存在します。つまり、$p(U') \subset p(U)$ があります。

M が N° の任意の部分空間である場合に戻ると、明らかに $\sigma(G/N, M) = \sigma(G/N, M + G^\circ)$ であることに注意してください。さらにプロップから。 II、p. 43 の 3 を見ると、$y \in N^\circ$ が線型形式 $\dot{z} \mapsto \langle y, \dot{z} \rangle$ が $\sigma(G/N, M)$ に対して連続であるような場合、必然的に $y \in M + G^\circ$ になることがわかります。 結論する、商位相 $\mathscr{T}$ が $\sigma(G/N, M)$ に等しくなるためには、条件 $M + G^\circ = N^\circ$ が必要かつ十分であると考えます。

#### 注意 {#evt-ii-s6-n5-rem-1 .statement tag=07HP}

— M と G/N 間の双対性 (M と N は 2 つの直交部分空間) は、$M \cap G^\circ = \{0\}$ の場合に限り、M で分離します。 $N = M^\circ$ の場合に限り、G/N で分離されます。

#### 系 1 {#evt-ii-s6-prop-7-cor-1 .statement tag=07HQ}

— F と G の双対性が F で分離しているとします。F 位相 $\sigma(G/M^\circ, M)$ のベクトル部分空間 M は、M が閉じている場合に限り、$\sigma(G, F)$ の $M^\circ$ の商位相と同一です。 位相 $\sigma(F, G)$。

これはプロップから続きます。 7 $N = M^\circ$ を置き、$M^{\circ \circ}$ が $\sigma(F, G)$ の M の閉包であることを思い出してください (II, p. 45、cor. 2)。

#### 系 2 {#evt-ii-s6-prop-7-cor-2 .statement tag=07HR}

— M が有限次元 n で双対性が F で分離している場合、$M^\circ$ は G で共次元 n です。M が $\sigma(F, G)$ で閉じていて有限余次元 n で双対性が G で分離している場合、$M^\circ$ は次元 n です。

なぜなら、$G/M^0$ は M との二元性を分離しているからです。 M が次元 n の場合、同じことが $G/M^\circ$ (II, p. 41, 例 1) にも当てはまります。 M が閉じている場合、$F/M = F/M^{\circ \circ}$ は $M^\circ$ と分離双対関係にあります。 F/M が次元 n の場合、$M^\circ$ (II、p. 41、例 1) についても同じです。

#### 系 3 {#evt-ii-s6-prop-7-cor-3 .statement tag=07HS}

— (F, G)、(F_1, G_1) を分離双対性の 2 つの空間の対とし、u を F_1 の F の線形写像とし、$\sigma(F, G)$ と $\sigma(F_1, G_1)$ にわたって連続します。この場合、Im($^t u$) が $\sigma(G, F)$ の G の閉じた部分空間である場合に限り、u は F_1 の F の厳密な射です。

$N = \operatorname{Im}(^t u) \subset G$ にしましょう。 F では $N^0 = \operatorname{Ker}(u)$ (II, p. 47, 公式 (3)) であることがわかります。 $p : F \to F/N^\circ$ を標準写像とすると、u は次のように因数分解されます。

$$
u : F \xrightarrow{p} F/N^\circ \xrightarrow{w} F_1,
$$

ここで、w は単射です。 空間 $F/N^\circ$ と N は分離双対関係にあり、II、p. 48 の公式 (1) により、すべての $\dot{y} \in F/N^\circ$ と $z_1 \in G_1$ に対して $\langle w(\dot{y}), z_1 \rangle = \langle \dot{y}, ^t u(z_1) \rangle$ が得られます。この関係は、wが$F/N^\circ$の同型で、$\sigma(F/N^\circ, N)$の位相を運び、$\sigma(F_1, G_1)$によって位相が誘発された$u(F)$であることを示しています。したがって、結論は cor から得られます。 1 と定義は厳密な射です。

#### 系 4 {#evt-ii-s6-prop-7-cor-4 .statement tag=07HT}

— (F, G)、(F_1, G_1) を分離双対性の 2 つの対とし、u を $\sigma(F, G)$ と $\sigma(F_1, G_1)$ に連続する F_1 における F の線形写像とします。そして、$^t u$ が $^t u(G_1)$ 上の $G_1$ の同型 (位相 $\sigma(G_1, F_1)$ を含む) であり、$\sigma(G, F)$ によって誘導された位相である場合に限り、u は全射的です。

なぜなら、$u(F) = F_1$ がというと同等だと言うことは、$u(F)$ が閉じていて、$\sigma(F_1, G_1)$ に対して $F_1$ ではどこも密集しているからです。コル。 4 は cor から続きます。 3 は $^t u$ と II、p. 47、cor に適用されます。 2.

#### 注意 {#evt-ii-s6-n5-rem-2 .statement tag=07HU}

— 1) 双対性を分離する際に、$(F_1, G_1), (F_2, G_2), (F_3, G_3)$ を 3 つの対と空間とし、2 つの線形写像のうち数列を考慮します。

$$
F_1 \xrightarrow{u} F_2 \xrightarrow{v} F_3
$$

弱いトポロジー 対応するに対してそれぞれ $G_1, G_2, G_3$ と連続しています。転置された写像の数列を考慮します

$$
G_3 \xrightarrow{^tv} G_2 \xrightarrow{^tu} G_1 .
$$

$^t(v \circ u) = ^t u \circ ^t v$、したがって、関係 $v \circ u = 0$ が $^t u \circ ^t v = 0$ と同等であることは明らかです。 数列 (5) は、以下の 3 つの条件が満たされる場合にのみ正確です。

a) $^t u \circ ^t v = 0$;
b) $\operatorname{Im}(^t v)$ は $\operatorname{Ker}(^t u)$ で密です。
c) $^t u$ は、$G_1$ の $G_2$ の厳密な射です。

これは実質的に cor に続きます。 II、p. 49の3と、II、p. 47の式(3)と(4)。

2) $u$ が $F_1$ の $F$ の厳密な射である場合、$^t u$ は必然的に $G$ の $G_1$ の厳密な射であると考えてはなりません。他の語 $u$ は、$u(F)$ が $\sigma(F_1, G_1)$ の $F_1$ で閉じられることなく、厳密な射になる可能性があります。これは、例で示されます。ここで、$F$ は、$F_1$ と $G = G_1 / F^\circ$ の非クローズ部分空間であり、$u$ は標準単射です。同様に、数列 (5) が正確であるという事実は、(6) が正確であることを必ずしも意味しませんが、数列 (5) が正確で、$v$ が厳密な射である場合、注意 1 と II により、数列 (6) は正確です。 p. 49、コル。 3.

### 6. 弱いトポロジの積

#### 命題 8 {#evt-ii-s6-prop-8 .statement tag=07HV}

— $(F_i, G_i)_{i \in I}$ を二元性における空間の対の家族とする。 $F = \prod_{i \in I} F_i$ を $F_i$ の積空間とし、$G = \bigoplus_{i \in I} G_i$ を $G_i$ の直和とします。すべての $x = (x_i) \in F$ とすべての $y = (y_i) \in G$ について、$\langle x, y \rangle = \sum_{i \in I} \langle x_i, y_i \rangle$ (ゼロ以外の項が有限個だけある和) と書くと、位相 $\sigma(F, G)$ (双線形形式 $(x, y) \mapsto \langle x, y \rangle$ に対して) は次のようになります。トポロジー $\sigma(F_i, G_i)$ の積。

というのは、$F$ に位相 $\mathscr{T}$ が与えられたとします。 位数では、すべての $y \in G$、線型形式 $x \mapsto \langle x, y \rangle$ が $\mathscr{T}$ に対して連続である必要があり、$\langle x, y \rangle$ の定義までに、写像 $x \mapsto \langle \operatorname{pr}_i x, y_i \rangle$ のそれぞれが連続であることが必要かつ十分です。 $\mathscr{T}$、$I$ および $G_i$ の $y_i$ では、$i$ は任意です。しかし、これは、$F_i$ の $F$ の写像 $\operatorname{pr}_i$ が、$\mathscr{T}$ と $\sigma(F_i, G_i)$ (I、p. 10、cor. 1) に対して連続であることを意味します。これでデモンストレーションは完了です。

#### 注意 {#evt-ii-s6-n6-rem-1 .statement tag=07HW}

— $F$ と $G$ の間の二重性は $F$ (それぞれ $G$ ) で分離し、すべての $i \in I$ についてその場合に限り、$F_i$ と $G_i$ の間の二重性は $F_i$ (それぞれ $G_i$ ) で分離します。 $F$ と $G$ の双対性が $F$ (それぞれ $G$) で分離している場合、$F$ (それぞれ $G$) では、1 つの $G_i$ (それぞれ $F_i$) に直交する部分空間が正準的に識別されます。 $G$ の部分空間 (それぞれ $F$) は、$F_\kappa$ の積の部分空間で、$\kappa \neq i$ ($G_\kappa$ の直和は $\kappa \neq i$ となる) です。

#### 系 1 {#evt-ii-s6-prop-8-cor-1 .statement tag=07HX}

— 二元性を分離する場合、F と G を 2 ベクトル空間とします。 空間 F ($\sigma(F, G)$ 付き) が 2 つの部分空間 M, N の直接位相和である場合、空間 G ($\sigma(G, F)$ 付き) は、それぞれ M と N に直交する部分空間 $M^\circ, N^\circ$ の直接位相位相和です。

$p : F \to M, q : F \to N$ を F の射影子対応する ～ 分解を M と N の直和にするとします。これらの条件写像 $(p, q) : F \to M \times N$ はトポロジカル同型です。 $M_1 = G/M^\circ, N_1 = G/N^\circ$ の場合、M と N のトポロジー (F のトポロジーによって誘導される) は、それぞれ $\sigma(M, M_1)$、$\sigma(N, N_1)$ と同一です (II、p. 48、提案 7)。 写像 $^t(p, q) : M_1 \times N_1 \to G$ は、$M_1, N_1$ と G にトポロジー $\sigma(M_1, M)$、$\sigma(N_1, N)$、$\sigma(G, F)$ をプロパティによって与えると、トポロジー 同型になります。 8. この写像 $M_1$ (それぞれ $N_1$) は、G の像として部分空間 $N^\circ$ (それぞれ $M^\circ$)、および位相 $\sigma(M_1, M)$ (それぞれ $\sigma(N_1, N)$) を持ちます。 $N^\circ$ (それぞれ $M^\circ$) に $\sigma(G, F)$ によって像位相が誘発され、そこから系が続きます。

#### 系 2 {#evt-ii-s6-prop-8-cor-2 .statement tag=07HY}

— $(e_i)_{i \in J}$ を双対 $F^*$ を持つベクトル空間 F の基底とし、$u : \mathbf{R}^{(I)} \to F$ をこの基底によって定義される (代数的) 同型とします。次に、転置された写像 $^t u : F^* \to \mathbf{R}^I$ は、$F^*$ が位相 $\sigma(F^*, F)$ と $\mathbf{R}^I$ 積位相を運ぶとき、トポロジカル同型になります。

(A, II, § 2.6, prop. 10) $^t u$ は全単射であり、$x^* \in F^*$ についてすべての $i \in I$ に $\langle e_i, x^* \rangle = \xi_i^*$ を代入すると、像 $^t u(x^*)$ はベクトル $(\xi_i^*)$ であることがわかります。 $\mathbf{R}^I$ なので、F のすべての $x = \sum_i \xi_i e_i$ に対して、$\langle x, x^* \rangle = \sum_i \xi_i \xi_i^*$ が得られます。 系はこの公式とプロップから続きます。 8.

### 7. 弱い完成度空間

#### 命題 9 {#evt-ii-s6-prop-9 .statement tag=07HZ}

— 双対性を分離する場合、F、G を 2 つのベクトル空間とします。 $\hat{F}$ が位相 $\sigma(F, G)$ に対する空間 F の完成であり、$G^*$ が位相 $\sigma(G^*, G)$ である標準単射 $j : F \to G^*$ を考慮すると、j の連続拡大 $\hat{j} : \hat{F} \to G^*$ は次のようになります。トポロジー ベクトル空間の同型。

なぜなら、$\sigma(G^*, G)$ を備えた$G^*$ はハウスドルフであり、完全であることがわかります (II, p. 51, cor. 2)。 $G^*$ のベクトル部分空間を持つ j によって F を識別すると、$\sigma(G^*, G)$ によって F に誘導されるトポロジーは $\sigma(F, G)$ であり、F はトポロジー $\sigma(G^*, G)$ (II, p. 43, cor. 4) の $G^*$ で密になります。そこから命題が導き出されます。

したがって、弱い位相に対して完全なベクトル空間は、$\sigma(G^*, G)$ を備えた任意のベクトル空間 G の双対 $G^*$ です。 後で II、p. 51、cor。 2、それらは実直線の積 $\mathbf{R}^I$ と (トポロジー的に) 同型です。言語を簡略化するために、これらを積行と呼びます (これら空間の本質的な特徴については、II、p. 85、演習 13 および II、p. 81、演習 1 を参照してください)。

$G^*$ では、$\sigma(G^*, G)$ 位相がハウスドルフの弱いトポロジの中で最小であることに注目します。なぜなら、$\sigma(G^*, G)$ より粗い弱い位相は必然的に形 $\sigma(G^*, H)$ となるからです。ここで、$H \subset G$ (II, p. 43, cor. 3)。しかし、$H \neq G$ の場合、null ではなく、$H$ (A, II, § 7.3, prop. 8) に直交する線型形式 $x^* \in G^*$ が存在するため、$\sigma(G^*, H)$ はハウスドルフではありません。

この発言から、$F, G$ が 2 つのベクトル空間である場合、トポロジー $\sigma(G^*, G)$ と $\sigma(F^*, F)$ に対して連続である *線形全単射* $u : G^* \to F^*$ は必然的に *双連続* であると推測します。

#### 命題 10 {#evt-ii-s6-prop-10 .statement tag=07I0}

*$G$ を実数のベクトル空間とし、$F = G^*$ を位相 $\sigma(G^*, G)$ との双対とします。*

(i) *マッピング $V \mapsto V^\circ$ は、$F$ の閉じたベクトル部分空間のセット上の $G$ のベクトル部分空間のセットの全単射です。

(ii) *$F$ のすべての閉じたベクトル部分空間は、行の積であり、トポロジカルな補数を持ちます。*

双極性定理 (II、p. 45、cor. 2) によると、$V \mapsto V^\circ$ は全単射の集合のベクトル部分空間 $V$ の $G$ で、*クローズド* 集合の$\sigma(G, G^*)$はベクトル部分空間の$F$が休業となります。しかし、定義までに、$G$の*すべての*線型形式は$\sigma(G, G^*)$にわたって連続であるため、$G$のすべてのベクトル部分空間は閉じており、方程式$\langle y, y_\lambda^* \rangle = 0$($y_\lambda^* \in G^*$)の系によって定義されます。これは(i)を証明します。

ここで、$W$ を $F$ の閉じた部分空間とします。すると、$G$ に $V = W^\circ$ が入った $W = V^\circ$ ができます。 $V'$ を $G$ の $V$ の補数とします。 $F = G^*$ は正規的に $V^* \oplus {V'}^*$ と識別でき、${V'}^*$ は $V^\circ = W$ と識別できることがわかっています (A、II, § 2.6、提案 10 と一致)。さらに (II、p. 50、提案 8) 位相 $\sigma(G^*, G)$ は、トポロジー $\sigma(V^*, V)$ および $\sigma({V'}^*, V')$ の積と識別できます。これは主張 (ii) を証明します。

けれども、位相 $\sigma(G, G^*)$ では、$G$ のすべてのベクトル部分空間が閉じています。$G$ が無限大の次元である場合、位相 $\sigma(G, G^*)$ は最も細かい局所凸ではないことに注意してください。 $G$ の位相、$\sigma(G, G^*)$ 含むベクトル部分空間の無限次元の 0 のすべての近傍 : ただし、これは $G$ (II、 p. 43、cor. 3）。

### 8. 弱い完全な凸錐体空間

#### 補題 1 {#evt-ii-s6-lem-1 .statement tag=07I1}

*$E$ をハウスドルフ弱空間とし、$C$ を$E$ の頂点 0 を持つ適切な円錐とし、$E$ の均一な構造を完全なものとします。 $E$ のすべての連続線型形式は、$C$ で正となる $E$ の 2 つの連続線型形式の差になります。*

$E'$ を $E$ の双対、$F$ を $E'$ の代数双対とし、位相 $\sigma(F, E')$ とします。 $H = C^\circ - C^\circ$ を、$E$ では連続で、$C$ では正である線型形式の差によって形成される $E'$ のベクトル部分空間とします (II、p. 44、提案 4)。 $F$ における $H$ への直交が $\{0\}$ (II, p. 41, *例* 1) であることを示せば十分です。次に、$a \in F$ を $H$ に直交させます。 $a$ は $C^\circ$ に直交しているため、$F$ の $C$ の双極に対して属するでなければなりません。しかし、$E$ は $F$ の部分空間として識別可能であり、$C$ が完了し、$F$ で閉じられるため、$a \in C$ (II, p. 44, th. 1) が得られます。同様に、$a$ は $-C^\circ$ に直交するため、$a \in -C$ となります。 $C$が正しいので、$a = 0$になります。

#### 命題 11 {#evt-ii-s6-prop-11 .statement tag=07I2}

*$E$ をハウスドルフ弱空間とし、$C$ を $E$ の頂点 0 であり、$E$ の均一な構造で完全な凸円錐とします。

次に、集合 I と、積空間 $\mathbf{R}^I$ に次の特性を持つ E の連続線形写像 u が存在します。

a) u は、それぞれ E と $\mathbf{R}^I$ の制服構造に対して、$u(C)$ の C の同型です。

b) $u(C) \subset \mathbf{R}_+^I$ があります。

さらに、E の均一性によって C に誘導された均一性構造が計量可能である場合、$I = \mathbf{N}$ を取ることができます。

$(f_i)_{i \in I}$ を、$C \times C$ 定義する上の形 $(x, y) \mapsto |f_i(x - y)|$ の有限和が C の均一構造となるような E の連続線型形式の族とする。 (構造が計量可能である場合、$I = \mathbf{N}$ を取得できます。) 補題 1 により、$f_i$ のそれぞれが C で正であるとさらに仮定できます。あなたを$\mathbf{R}^I$のEの線形写像$x \mapsto (f_i(x))_{i \in I}$とします。 u が連続していることと、$u(C) \subset \mathbf{R}_+^I$ であることは明らかです。 制限 $u|C$ は、$u(C)$ の C から全射である一様連続写像です。さらに、C の $x, y$ がすべての $i \in I$ に対して $f_i(x) = f_i(y)$ となる場合、C の均一構造はハウスドルフであるため、$x = y$ になります。したがって、$u|C$ は全単射です。最後に、W が C の制服構造の側近である場合、I と数 $\varepsilon > 0$ の有限集合 J が存在し、$i \in J$ に対する関係 $|f_i(x) - f_i(y)| \leq \varepsilon$ が意味します。 $(x, y) \in W$;したがって、$u|C$ は、考慮されている制服構造の $u(C)$ の C の同型です。

#### 系 1 {#evt-ii-s6-prop-11-cor-1 .statement tag=07I3}

— E をハウスドルフ弱空間とし、C を E の頂点 0 の固有の凸円錐とし、E のそれによって誘導される一様構造に対して完全なものとします。すると、C の $C \times C$ の写像 $(x, y) \mapsto x + y$ が固有になります。

プロップのせいで。 11 では、$E = \mathbf{R}^I$ と $C = \mathbf{R}_+^I$ と仮定できます (GT、I, § 10.1、cor. 1 および 4)。しかし、その後、Cの$C \times C$の写像$(x, y) \mapsto x + y$は$((\xi_i), (\eta_i)) \mapsto (\xi_i + \eta_i)$と書かれ、$\mathbf{R}_+$の$\mathbf{R}_+ \times \mathbf{R}_+$の連続写像$f : (\xi, \eta) \mapsto \xi + \eta$が適切であるという証明に制限できます。 (GT, I, § 10.1, cor.3), さて、すべての $\zeta \in \mathbf{R}_+$ について、$f(\zeta)$ は対 $(\xi, \zeta - \xi)$ の集合であり、$0 \leq \xi \leq \zeta$ であるため、区間の f により逆像となることがわかります。 $[0, \zeta]$は$(\xi, \eta) \in \mathbf{R}_+ \times \mathbf{R}_+$の集合を$\xi + \eta \leq \zeta$としてコンパクトにしました。結論は適用 (GT、I, § 10.3、提案 7) に従います。

#### 系 2 {#evt-ii-s6-prop-11-cor-2 .statement tag=07I4}

— E をハウスドルフ弱空間とし、E の頂点 0 を持つ適切な凸円錐 C とし、これは E の均一構造に対して完全です。

(i) E のすべての点 a に対して、共通部分 $C \cap (a - C)$ はコンパクトです。

(ii) A, B を C で 2 つ閉じた集合とする。すると、$A + B$はCでクローズされた集合になります。

(i) $x + y = a$ が cor からコンパクトになるような $(x, y) \in C \times C$ の集合 1 と GT から、I, § 10.2、th。 1、b)。さて、この集合は、$x \in C \cap (a - C)$に対する$(x, a - x)$の集合でもあり、これは(i)を証明します。

(ii) A と B が C で閉じられる場合、$A \times B$ は $C \times C$ で閉じられるため、$A + B$ は C 後でで閉じられます。 1 と GT、I, § 10.1、プロップ。 1.

### 練習問題 {#evt-ii-s6-exercises}

[§ 6 に対して練習問題](exercises/s6/)を参照してください。
