---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 1
section_title: Essential upper integral
lang: ja
source: int-i-vi
book_pages: INT V.2-INT V.11
pdf_pages: 0257-0266, 0349-0350
extraction: ocr
subsections:
    - "no": 1
      title: Definition of the essential upper integral
      page: 2
      pdf_page: 257
    - "no": 2
      title: Moderated functions and measures
      page: 4
      pdf_page: 259
    - "no": 3
      title: Essentially integrable functions
      page: 7
      pdf_page: 262
    - "no": 4
      title: A property special to the essential upper integral
      page: 10
      pdf_page: 265
statements: 22
exercises: 6
content_sha256: f7f2d2a85ba6323296d8546486966840f8dc2b73dd0e466068dabd717ba00cc2
translated_from: content/en/int/V/01_s1_essential_upper_integral.md
translation_method: google
source_content_sha256: d19dbe1131a1bb0064d0db8332b6983acb2090fbcf25d4ea5abb63e1585fb1b0
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: e0bbc81d9552cc294e2d269beee7dc61da95a229619ca67ec657f2bb7ba0052e
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 1。必須の上部積分

### 1. 重要な上部積分の定義

#### 定義 1 {#int-v-s1-def-1 .statement tag=08ZO}

写像 $f \in \mathscr{F}_+(T)$ ごとに、$\mu$ に関する$f$ の本質的な上積分を呼び出し、数 $\mu^*(f \varphi_K)$ の集合の有限であるかどうかにかかわらず、$K$ が超過する上限を $\mu^\bullet(f)$ で示します。 集合 of compact 部分集合 of $T$. $T$ の部分集合 $A$ ごとに、集合 $\mu^\bullet(A) = \mu^\bullet(\varphi_A)$ が 1 つずつ追加されます。

記法 $\int^\bullet f d\mu$、$\int^\bullet f(t) d\mu(t)$、$\int^\bullet f \mu$ も使用されます。
$T$ の各コンパクト部分集合 $K$ に対して $f \varphi_K \leq f$ なので、1 つは

$$
\int^\bullet f d\mu \leq \int^* f d\mu .
$$

$\mu^\bullet(f) \neq \mu^*(f)$; ということが起こる可能性があります。なぜなら、条件 $\mu^*(f) = 0$ は $f$ が無視できることを意味し、条件 $\mu^\bullet(f) = 0$ は $f$ が局所的に無視できることを意味し (Ch. IV, §5, No. 2、提案 5)、無視できないが局所的に無視できる集合が存在する可能性がある (Ch. IV, §1、エクサー 5)。

$\mathscr{F}_+(T)$ の写像 $\mu^\bullet$ を $\overline{\mathbf{R}}$ 一致するに、$\mathscr{K}_+(T)$ に $\mu$ を加えます。したがって、2 つのメジャー $\mu_1$ と $\mu_2$ は、$\mu_1^\bullet = \mu_2^\bullet$ が等しくなります。

#### 命題 1 {#int-v-s1-prop-1 .statement tag=08ZP}

a) If $f$ and $g$ are two numerical functions $\geq 0$ that are equal locally almost everywhere, then $\mu^\bullet(f) = \mu^\bullet(g)$.
b) If $f$ and $g$ are two numerical functions $\geq 0$ such that $f \leq g$, then $\mu^\bullet(f) \leq \mu^\bullet(g)$.
c) If $f$ is a numerical function $\geq 0$, and $\alpha$ is a number $\geq 0$, then $\mu^\bullet(\alpha f) = \alpha \mu^\bullet(f)$.
d) If $f$ and $g$ are two numerical functions $\geq 0$, then $\mu^\bullet(f + g) \leq \mu^\bullet(f) + \mu^\bullet(g)$.
e) If $(f_n)_{n \in \mathbf{N}}$ is an increasing sequence of numerical functions $\geq 0$, and if $f = \lim_{n \to \infty} f_n$, then $\mu^\bullet(f) = \lim_{n \to \infty} \mu^\bullet(f_n)$.

性質 a)、b)、c)、d) は、上積分の対応する性質からすぐに推定できます。 a) 第 1 章の命題 6 から。 IV, §2, No. 3 と命題 5 章 IV, §5, No. 2; b)、c)、d) 命題 10、11、12 章より。 IV, §1, No. 3。 e) を確立するには、$T$ のコンパクト部分集合の $\mathfrak{K}$ 集合で表します。 定理 3章による IV, §1, No. 3、私たちは持っています

$$
\lim_{n \to \infty} \mu^\bullet(f_n) = \sup_{n \in \mathbf{N}} \sup_{K \in \mathfrak{K}} \mu^*(f_n \varphi_K) = \sup_{K \in \mathfrak{K}} \sup_{n \in \mathbf{N}} \mu^*(f_n \varphi_K)
= \sup_{K \in \mathfrak{K}} \mu^*(f \varphi_K) = \mu^\bullet(f) .
$$

等式は関係 d) $f$ と $g$ が測定可能であれば、Cor により成り立ちます。 Thの4。 5、Ch. IV, §5, No. 6。より一般的には、次のような結果が得られます。

#### 命題 2 {#int-v-s1-prop-2 .statement tag=08ZQ}

*$f, g, h$を$\mathscr{F}_+$の3つの元とします。 $g$ と $h$ が測定可能であれば、*

$$
\int^\bullet f(g + h)\, d\mu = \int^\bullet fg\, d\mu + \int^\bullet fh\, d\mu.
$$

1 は、上部積分の類似の公式の証明にすぐに還元されます。 $f(g + h) = fg + fh$ 以降 (慣例として $0 \cdot (+\infty) = 0$)、

$$
\int^* f(g + h)\, d\mu \leq \int^* fg\, d\mu + \int^* fh\, d\mu;
$$

逆の不等式を確立することが残っています。 $u$ を、$u \geq f(g + h)$ となるような下位の半連続写像とします。 集合 $v = \frac{u}{g + h}$ は集合で $g + h > 0$、$v = +\infty$ は集合で $g + h = 0$ です。次に$v \geq f$と$u \geq v(g + h)$、よって

$$
\int^* v(g + h)\, d\mu \leq \int^* u\, d\mu
$$

その結果、$v$ は測定可能です (Ch. IV, §5, No. 6、Th. 5 の Cor. 4)。

$$
\int^* fg\, d\mu + \int^* fh\, d\mu \leq \int^* vg\, d\mu + \int^* vh\, d\mu \\
= \int^* v(g + h)\, d\mu \leq \int^* u\, d\mu,
$$

これは、$u$ は任意であるため、望ましい不等式を意味します。

#### 系 {#int-v-s1-n1-cor-1 .statement tag=08ZR}

*$f$ を測定可能な写像 $\geq 0$ の写像 $\geq 0$、$(g_n)$ 数列とします。それから$\int^\bullet f \left( \sum_n g_n \right) d\mu = \sum_n \left( \int^\bullet f g_n\, d\mu \right)$。

有限列の場合、これは提案 2 の明らか帰結であり、無限シーケンスの場合は、提案 1 の e) によってこれから推定できます。

#### 命題 3 {#int-v-s1-prop-3 .statement tag=08ZS}

*有限の数 $\alpha \geq 0$ および $\mathbf{T}$ の小節 $\mu, \nu$ のすべての対に対して、

$$
(\alpha \mu)^\bullet = \alpha \mu^\bullet \\
(\mu + \nu)^\bullet = \mu^\bullet + \nu^\bullet.
$$

さらに、関係 $\mu \leq \nu$ は $\mu^\bullet \leq \nu^\bullet$ を意味します。*

証明は、第 3 章の類似の主張からの明らかです。 IV (§1, No. 3、提案 15)。

#### 命題 4 {#int-v-s1-prop-4 .statement tag=08ZT}

— *すべての数値写像* $f \geqslant 0$ *これは、下位の半連続* $T$、$\mu^\bullet(f) = \mu^*(f)$ です。

というのは、$g$ を $\mathscr{K}_+(T)$ で写像とし、$g \leqslant f$ とします。 $K$ が $g$ の (コンパクトな) サポートである場合、$\mu(g) \leqslant \mu^*(f \varphi_K) \leqslant \mu^\bullet(f)$ です。上積分の定義により、$\mu^*(f) \leqslant \mu^\bullet(f)$、従って$\mu^*(f) = \mu^\bullet(f)$ (公式 (1)) となります。

### 2. モデレートされた写像と対策

#### 命題 5 {#int-v-s1-prop-5 .statement tag=08ZU}

— *$A$ *$T$ の部分集合とします。 *次のプロパティは同等です*:
a) *集合* $A$ * は、* $\mu$* 積分可能なオープン集合* の数列の和集合に含まれます。
b) *集合* $A$ * は* $\mu$* 積分可能集合* の数列の和集合に含まれます。
c) *集合* $A$ *は、コンパクト集合の数列の和集合と* $\mu$*-無視できる集合*に含まれます。

プロパティ a) と c) のそれぞれが b) を意味することは明らかです。逆に、b) は、有限の外部測度のすべての集合が積分可能な開いた集合 (Ch. IV, §1, No. 4、提案 19) に含まれるため、a) を意味し、b) は、すべての可積分集合がコンパクトの数列の和集合であるため、c) を意味します。 集合と無視できる程度の集合 (Ch. IV, §4, No. 6、Th. 4 の Cor. 2)。

#### 定義 2 {#int-v-s1-def-2 .statement tag=08ZV}

— * $T$ * の *部分集合は、命題 5* に相当する条件を満たす場合、* $\mu$* が緩和されていると言われます。 *写像は $T$ に定義されており、 *ベクトル空間または $\overline{\mathbf{R}}$ に値が含まれており、* $\mu$* 緩和された* の補数で零である場合、 * $\mu$* 緩和されていると言われます* 部分集合/* $T$。 *測定* $\mu$ *は* $T$ *が* $\mu$*-緩和された集合*の場合、緩和されたと言われます。

$\mu$ が緩和措置である場合、$T$ のすべての写像は $\mu$ 緩和され、$T$ のすべての部分集合は $\mu$ 緩和されます。

#### 注意 {#int-v-s1-n2-rem-1 .statement tag=08ZW}

— 1) $\theta$ が $T$ の複雑な尺度である場合、$f$ が $|\theta|$ で緩和されている場合 (それぞれ $|\theta|$ が緩和されている場合)、写像 $f$ は $\theta$ で緩和されている (それぞれ $\theta$ が緩和されている) と言えます。
2) すべての制限された措置は緩和されます。 $T$ がコンパクト集合の可算和集合である場合、$T$ のすべての小節は緩和されます。
3) $(f_n)$ を、$\overline{\mathbf{R}}$ に値を加えた$\mu$ の写像の数列とします。それぞれの $n$ について、$U_n$ を、有限の外側メジャーの開集合の可算和集合である開集合とし、$f_n$ は $U_n$ の外側の零になります。 写像 $s = \sum_{n \in \mathbf{N}} |f_n|$ は $\bigcup_{n \in \mathbf{N}} U_n$ の外側の零です。したがって、これは $\mu$ で緩和されており、同じことが $|f| \leq s$ などのすべての写像 $f$ にも当てはまります。これは、特に写像 $\liminf_{n \to \infty} f_n$、$\limsup_{n \to \infty} f_n$、および $\sum_{n \in \mathbf{N}} f_n$ (和が定義されている場合) に当てはまります。

4) 写像は、ほぼどこでも、緩和された写像と同等です。

#### 命題 6 {#int-v-s1-prop-6 .statement tag=08ZX}

— *$f$ を、$T$ で定義された正の数値写像とし、$\mu$ 測定可能で $\mu$ 緩和されます。次に、和が $f$ に等しい、$\mathscr{F}_+(T)$ の元の数列 $(h_n)_{n \in \mathbf{N}}$ が存在し、次の特性を持ちます:*

1) *写像 $h_0$ は $\mu$ は無視できます。*
2) *すべての $n \geq 1$ に対して、$h_n$ が $K_n$ の外側に零であり、$h_n$ から $K_n$ の制限が有限連続であるようなコンパクト集合 $K_n$ が存在します。

$f$ が正の可測値写像の数列 $(f_n)$ の和であり、それぞれ主張に性質があるとします。 $f$ にもそれがあることは明らかです。 集合
$$
f_n = \inf(f, n+1) - \inf(f, n)
$$
$n \in \mathbf{N}$ごとに; $f$ は数列 $(f_n)$ の和に等しいため、$f$ が緩和され *制限されている* と仮定して命題を確立するだけで十分です。次に、$t \in T$ の $A$ 集合を$f(t) > 0$ のように表します。 $A$ は可測かつ緩和されているため、$A = \bigcup_n A_n$ となるようなペアの互いに素可積分集合の数列 $(A_n)$ が存在します。 写像 $f \varphi_{A_n}$ では、証明主張に減額されます。他の語では、$f$ が有界であり、零が可積分集合 $I$ の外側にあると仮定できます。しかし、$I$は無視できる集合$N$の和集合と互いに素コンパクトな集合の数列$(L_n)$です（Ch.IV, §4, No. 6、Th.4のCor.2）。したがって、$f$ が有界であり、零がコンパクト集合 $L$ の外側にある場合を扱うことになります。

$\mathscr{K}$ を、$f|K$ が連続となるようにコンパクトな部分集合 $K$ の $T$ の集合とします。 $\mathscr{K}$ は $\mu$ 密であるため (Ch. IV, §5, No. 10、提案 15)、$L$ は無視できるペアワイズの集合 $N$ および数列 $(K_n)_{n \geq 1}$ の和集合です。 互いに素元/$\mathscr{K}$ (Ch. IV, §5, No. 8、Def. 6)。 $n \geq 1$ の場合は写像 $h_0 = f \varphi_N$、$h_n = f \varphi_{K_n}$ 次に、主張の満たす条件。

次の命題により、本質的な上部積分の学習に加えて、上部積分の学習も簡約する可能になります。

#### 命題 7 {#int-v-s1-prop-7 .statement tag=08ZY}

— *$f$を$\mathscr{F}_+(T)$の元とします。*
1) *写像 $f$ が $\mu$ で管理されていない場合、$\mu^*(f) = +\infty$。*
2) *写像 $f$ が $\mu$ で管理されている場合、$\mu^*(f) = \mu^*(f)$。*
3) *$\mu^*(f) < +\infty$ の場合、$T$ のコンパクトな部分集合の数列の$\mu$ が緩和された部分集合 $A$、和集合が存在し、局所的にほぼどこでも$f = f \varphi_A$ になります。

最初の主張は、第 1 章の補題 1 の直後に続きます。 IV, §5, No. 6。 2 番目を確立するには、f が A の外側で零になるように緩和された部分集合を $A$ で表します。 A は、無視できるほど小さい集合 $A_0$ の和集合と、コンパクトな集合の数列 $(A_n)_{n \geq 1}$ であり、これは増加するであると想定できます。 写像 $f$ は、ほぼどこでも写像 $f \varphi_{A_n}$ ($n \geq 1$) の上部エンベロープに等しいため、(Ch. IV, §1, No. 3、Th. 3 および §2, No. 3、提案 6)

$$
\mu^*(f) = \lim_{n \to \infty} \mu^*(f \varphi_{A_n}) \leq \mu^\bullet(f),
$$

公式のおかげでよって等式 $\mu^*(f) = \mu^\bullet(f)$ (1)。最後に、$\mu^\bullet(f) < +\infty$; と仮定します。次のようなコンパクト集合の増加する数列 $(A_n)$ が存在します。

$$
\mu^\bullet(f) = \sup_n \mu^*(f \varphi_{A_n}).
$$

集合 $A = \bigcup_n A_n$; 2 番目のメンバーは $\mu^*(f \varphi_A)$ (Ch. IV, §1, No. 3、Th. 3)、つまり $\mu^\bullet(f \varphi_A)$ (上記の提案 1 または 2 による) に等しい。 $\mu^\bullet(f) = \mu^\bullet(f \varphi_A) + \mu^\bullet(f \varphi_{\mathbf{C}_A})$ (提案 2) なので、$\mu^\bullet(f \varphi_{\mathbf{C}_A}) = 0$ があり、そこから 3) が続きます。

#### 系 1 {#int-v-s1-prop-7-cor-1 .statement tag=08ZZ}

*f が無視できるためには、それが局所的に無視でき、緩和されることが必要かつ十分です。*

#### 系 2 {#int-v-s1-prop-7-cor-2 .statement tag=0900}

*$\mu$ が緩和された尺度である場合 (特に、$\mu$ が制限されている場合、または T が無限で可算である場合)、$\mu^* = \mu^\bullet$.*

#### 命題 8 {#int-v-s1-prop-8 .statement tag=0901}

a) *H を写像 $\geq 0$ の集合とし、下部半連続、関係 $\leq$ に向けます。それから*

$$
\mu^\bullet \left( \sup_{h \in H} h \right) = \sup_{h \in H} \mu^\bullet(h).
$$

b) *H を写像 $\geq 0$ の集合、上部半連続、関係 $\geq$ に向けたものとする。 H 写像 $h_0$ に $\mu^\bullet(h_0) < +\infty$ が存在する場合、*

$$
\mu^\bullet \left( \inf_{h \in H} h \right) = \inf_{h \in H} \mu^\bullet(h).
$$

主張 a) は、提案 4 を考慮すると、第 4 章の定理 1 の繰り返しです。 IV, §1, No. 1。 b) を確立するには、集合 $\eta = \inf_{h \in H} h$、$a$ を数 $> 0$ とします。次のようなコンパクトな集合 K が存在します (Ch. IV, §4, No. 4、提案 5 の Cor. 1):

$$
\mu^\bullet(h_0) - a \leq \mu^*(h_0 \varphi_K) = \mu(h_0 \varphi_K) \leq \mu^\bullet(h_0).
$$

写像 $h\varphi_K$、$h$ が$H$、形集合の上半連続写像を通過し、含む可積分関数である関係 $\geqslant$ に向けられます。したがって (Ch. IV, §4, No. 4、提案 5 の Cor. 2):

$$
\mu^*(\eta\varphi_K) = \inf_{h \in H} \mu^*(h\varphi_K).
$$

しかし (Ch. IV, §4, No. 4、提案 5 の Cor. 1) 写像 $h \in H$ ごとに $\mu^\bullet(h_0\varphi_{C_K}) \leqslant a$、よって $\mu^\bullet(h\varphi_{C_K}) \leqslant a$ となり、$h \leqslant h_0$ となります。したがって、最後に次のようになります。

$$
\mu^\bullet(\eta) \geqslant \mu^*(\eta\varphi_K) = \inf_{h \in H} \mu^*(h\varphi_K) \geqslant \inf_{h \in H} \mu^\bullet(h) - a.
$$

不等式 $\mu^\bullet(\eta) \leqslant \inf_{h \in H} \mu^\bullet(h)$ は自明であり、$a$ は任意であるため、命題が成立します。

### 3. 基本的に可積分関数

$F$ を本物のバナッハ空間とします。 空間 $\mathscr{F}_F^p$ (Ch. IV, §3, No. 3) および $\mathscr{L}_F^p$ (Ch. IV, §3, No. 4、Def. 2) の元が $\mu$ で調整された写像 (Ch. IV, §5, No. 6、補題) であることを思い出してください。 1); $\mathscr{N}_F$ はまだ $T$ のごくわずかな写像の空間を $F$ に表すため、局所的に無視できる $T$ の写像のうち空間 $\mathscr{N}_F^\infty$ を $F$ に導入します。

#### 補題 {#int-v-s1-n3-lem-1 .statement tag=0902}

*$g$ と $g'$ を 2 つの $\mu$ で調整された写像とし、$F$ に値を加えます。 $g$ と $g'$ がほぼどこでも局所的に同じ写像 $f$ と等しい場合、$g = g'$ はほぼどこでも*。

なぜなら、$D$ を $t \in T$ の集合とし、$g(t) \neq g'(t)$ とするためです。 $D$ は局所的には無視でき、緩和されているため、無視できます (提案 7 の訂正 1)。

$f$に等しい写像$g \in \mathscr{F}_F^p$が存在するように、写像の集合$T$の$f$を$F$に$\overline{\mathscr{F}}_F^p(T, \mu)$（または単に$\overline{\mathscr{F}}_F^p(\mu)$、$\overline{\mathscr{F}}_F^p$）で表します。ほぼどこでもローカルに。 数 $N_p(g)$ は補題による$f$ のみに依存するので、$\overline{N}_p(f) = N_p(g)$ と書きます。 写像 $\overline{N}_p$ は明らかに $\overline{\mathscr{F}}_F^p$ の準ノルムであり、$\overline{\mathscr{F}}_F^p$ には $\overline{N}_p$ によって定義される位相が装備されていると常に仮定します。この位相の 0 の終点は空間 $\mathscr{N}_F^\infty$ です。 関係 $\overline{\mathscr{F}}_F^p = \mathscr{F}_F^p + \mathscr{N}_F^\infty$、$\mathscr{N}_F^\infty \cap \mathscr{F}_F^p = \mathscr{N}_F$ (補題) は、標準化された空間 $\overline{\mathscr{F}}_F^p / \mathscr{N}_F^\infty$ が完全な $\mathscr{F}_F^p / \mathscr{N}_F$ と正規的に同一視される可能性があることを示しています (Ch. IV, §3, No. 3、提案 5)。したがって、$\overline{\mathscr{F}}_F^p$自体が完了しています。

同様に、$\overline{\mathscr{F}}_F^p$ の $\overline{\mathscr{L}}_F^p(T, \mu)$ (または $\overline{\mathscr{L}}_F^p(\mu)$、または $\overline{\mathscr{L}}_F^p$) 部分空間 $\mathscr{L}_F^p + \mathscr{N}_F^\infty$ で表します。 $\overline{\mathscr{L}}_F^p$ を、*測定可能な* 写像によって構成される $\overline{\mathscr{F}}_F^p$ の部分空間として特徴付けることもできます (Ch. IV, §5, No. 6、Th. 5)。

正規化された空間 $\overline{\mathscr{L}}_F^p / \mathscr{N}_F^\infty$ は、標準的に $L_F^p$ と識別される場合があります。これで$\overline{\mathscr{L}}_F^p$は完了です。その元は *p 番目の冪本質的には可積分関数* と呼ばれ、この用語は次の命題によって正当化されます。

#### 命題 9 {#int-v-s1-prop-9 .statement tag=0903}

*T の写像 f から F への属するから $\overline{\mathscr{F}}_F^p$ (それぞれ $\overline{\mathscr{L}}_F^p$ へ) について、必要かつ十分である場合* (それぞれ * f が測定可能であること、および*)

$$
\mu^\bullet(|f|^p) < +\infty .
$$

*その場合、* $\overline{N}_p(f) = (\mu^\bullet(|f|^p))^{1/p}$ になります。

私たちは、$\overline{\mathscr{F}}_F^p$に関して、明らかに極限自分自身を主張にするかもしれません。 f 属するから $\overline{\mathscr{F}}_F^p$ の場合、 g を写像所属から $\mathscr{F}_F^p$ とし、局所的にほぼどこでも f に等しくなります。 $|f|^p = |g|^p$ ほぼどこにでもローカルに存在するため、

$$
\mu^\bullet(|f|^p) = \mu^\bullet(|g|^p) = \mu^*(|g|^p) < +\infty
$$

(提案 1、a) および提案 7)、一方、$\overline{N}_p$ の定義により、

$$
\overline{N}_p(f) = N_p(g) = (\mu^*(|g|^p))^{1/p} .
$$

逆に、$\mu^\bullet(|f|^p) < +\infty$; と仮定します。その場合、 f が T − A のほぼどこでも局所的に零となるような、緩和された集合 A が存在します (提案 7)。 写像 $f \varphi_A$ は、局所的にほぼどこでも f に等しく、$N_p(f \varphi_A) = \overline{N}_p(f) < +\infty$ となるため、属するから $\mathscr{F}_F^p$、および $f \in \overline{\mathscr{F}}_F^p$ となります。

#### 系 {#int-v-s1-n3-cor-1 .statement tag=0904}

*f を属するから $\mathscr{L}_F^p$ にするには、f 属するから $\overline{\mathscr{L}}_F^p$ と節制することが必要十分です。*

#### 定義 3 {#int-v-s1-def-3 .statement tag=0905}

*$\overline{\mathscr{L}}_F^1$の元は、Fの値で本質的に$\mu$可積分関数と呼ばれます。$L_F^1$の写像$\tilde{f} \mapsto \mu(f)$を$\overline{\mathscr{L}}_F^1$の標準写像と$L_F^1$でFに合成すると、連続関数が得られます。 $\overline{\mathscr{L}}_F^1$の線形写像をFに、拡大するの写像$f \mapsto \int f d\mu$をFに$\mathscr{L}_F^1$をFにします。1は、この写像の$f \in \overline{\mathscr{L}}_F^1$の$\int f d\mu$または$\mu(f)$値を示します。 元は、$\mu$ に関する f の積分と呼ばれます*。

ほぼどこでも局所的に等しい 2 つの本質的に等しい 2 つの可積分関数は、同じ積分を持ちます。有限で本質的に可積分であるすべての写像 $f \geq 0$ に対して、$\int^\bullet f d\mu = \int f d\mu$。 A が集合で、その特性写像が本質的に可積分である場合、A は *本質的に $\mu$ 可積分である集合* であると言われます。 $\int \varphi_A d\mu$ は $\mu(A)$ とも表され、再び A の *メジャー* と呼ばれます。

If a function $f$, with values in $F$, is defined locally almost everywhere in $T$, we again say that $f$ is *essentially integrable* if it is equal, locally almost everywhere, to a function $f_1$ that is everywhere defined and integrable; we then set
$$
\int f\, d\mu = \int f_1\, d\mu,
$$
and this definition is independent of the integrable function $f_1$ everywhere defined and equal locally almost everywhere to $f$ (Lemma). 1 つの定義するも同様に、ほぼどこでも局所的に定義され有限である $\overline{\mathbf{R}}$ の値を持つ写像に対する本質的な可積分関数の概念です。

読者は、第 3 章の結果を本質的に可積分関数まで拡張することに何の困難もありません。 可積分関数のIV, §4、置き換えることの「ほぼどこでも」、主張では「地元のほぼどこでも」。たとえば、不等式に注目してください。
$$
\left| \int f\, d\mu \right| \leq \int |f|\, d\mu,
$$
Banach 空間の値を含む基本的にすべての可積分関数 $f$ に有効です。

#### 命題 10 {#int-v-s1-prop-10 .statement tag=0906}

*$\mathfrak{K}$を、$T$のコンパクト部分集合の$\mu$密集合とします。*
a) *$f$ が数値写像 $\geq 0$ の場合、*
$$
\mu^\bullet(f) = \sup_{K \in \mathfrak{K}} \mu^*(f \varphi_K).
$$
b) *$f$ が本質的に可積分関数で、バナッハ空間 $F$ に値が含まれる場合、*
$$
\int f\, d\mu = \lim_{\mathfrak{K}} \int f \varphi_K\, d\mu,
$$
*極限は、有向 ($\subset$) 集合 $\mathfrak{K}$ に関して取られています。*

a) を確立するには、$T$ のすべてのコンパクト部分集合 $L$ について、
$$
\int^* f \varphi_L\, d\mu = \sup_K \int^* f \varphi_K\, d\mu,
$$
ここで、$K$ は、$L$ 所属から $\mathfrak{K}$ の部分集合の集合を上回ります。 $L$ は無視できる集合の和集合および増加する数列 $(K_n)$ $\mathfrak{K}$ の元であるため (Ch. IV, §5, No. 8、提案 12)、これは、上部積分における定理から極限に続きます (Ch. IV, §1, No. 3、木。 3)。

ここで、$f$ 属するから $\mathscr{L}_F^1$ だとします。 $\varepsilon$ を数 $> 0$ とし、$K$ を $\mathfrak{K}$ の元とします。
$$
\int |f| \varphi_K\, d\mu \geq \int |f|\, d\mu - \varepsilon
$$

(そのような K は a) によって存在します)。次に、すべてのコンパクト集合 H 含む K に対して、

$$
\left| \int f \, d\mu - \int f \varphi_H \, d\mu \right| \leq \int |f| \varphi_{\mathbf{C}_H} \, d\mu \leq \int |f| \varphi_{\mathbf{C}_K} \, d\mu \leq \varepsilon .
$$

拡大から複雑な Banach 空間と対策。 F を複素バナッハ空間とします。 記法の乱用により、F の基礎となる本物のバナハ空間も F で表されます。バナハ空間 $\overline{\mathscr{L}}_F^p(T, \mu)$ には、自然な複合バナハ空間構造が装備される可能性があり、これの実数と複素数構造のどちらを使用しているかを具体的にする必要があります。 空間。この章では、反対の明示的な言及がなければ、常に実際の構造であることが理解されます。

$\theta$ を複素測度としましょう。私たちは集合 $\overline{\mathscr{L}}_F^p(T, \theta) = \overline{\mathscr{L}}_F^p(T, |\theta|)$; F が複素バナッハ空間の場合、上記と同じ注意を作ることができます。特に、F に値を含む写像 f は、$|\theta|$ に対して本質的に可積分である場合、$\theta$ に対して本質的に可積分であると呼ばれます。提案 10 の主張 b)、その後拡大するを同時に複雑な措置に適用します。

### 4. 性質重要な上部積分に特別な

次の結果は続編で頻繁に使用されます。 主張では、通常の上積分による 1 つのできない置き換えるの必須上積分です (例 4 を参照)。

#### 命題 11 {#int-v-s1-prop-11 .statement tag=0907}

— $(\lambda_\alpha)_{\alpha \in A}$ を、関係 $\leq$ に向けられ、$\mathscr{M}(T)$ に最高値 $\lambda$ を持つ、T 上のポジティブ測度の族とします。次に、すべての数値写像 $f \geq 0$ について、

$$
\lambda^\bullet(f) = \sup_{\alpha \in A} \lambda_\alpha^\bullet(f).
$$

$f$ 属するから $\mathscr{K}(T)$ のとき、これは $\mathscr{M}(T)$ の有向集合の最高値の関係簡約するから定義になります（II, §2, No. 2、補題章）。次に、ある写像 $g \in \mathscr{K}_+$ に対して $f \leq g$ があるとします (他の語では、$f$ は有界であり、コンパクト集合 K の外側に零があります)。 $\alpha$ を $\lambda_\alpha(g) \geq \lambda(g) - \varepsilon$ となるように添字とします。ここで、$\varepsilon$ は数 $> 0$ です。メジャー $\nu = \lambda - \lambda_\alpha$ が正であるため、$\nu^*(f) \leq \nu(g) \leq \varepsilon$ または $\lambda_\alpha^*(f) \geq \lambda^*(f) - \varepsilon$ になります (Ch. IV, §1, No. 3、提案 15)。 ($\varepsilon$ は任意であるため) (5) の 2 番目のメンバーは最初の $\geq$ になります。逆の不等式は明白なので、考慮中の特別な場合には (5) が確立されます。次に、$f$ は K の外側にある零ですが必ずしも有界ではなく、整数 $n$ ごとに集合 $f_n = \inf(f, n)$ であるとします。それから

$$
\lambda^\bullet(f) = \sup_{n \in \mathbf{N}} \lambda^\bullet(f_n) = \sup_{n \in \mathbf{N}} \sup_{\alpha \in A} \lambda_\alpha^\bullet(f_n) = \sup_{\alpha \in A} \sup_{n \in \mathbf{N}} \lambda_\alpha^\bullet(f_n) = \sup_{\alpha \in A} \lambda_\alpha^\bullet(f).
$$

最後に、$f$ で制限が作成されず、$T$ のコンパクト部分集合の $\mathscr{K}$ 集合によって示されます。
$$
\lambda^\bullet(f) = \sup_{K \in \mathscr{K}} \lambda^\bullet(f \varphi_K) = \sup_{K \in \mathscr{K}} \sup_{\alpha \in A} \lambda_\alpha^\bullet(f \varphi_K)
$$
$$
= \sup_{\alpha \in A} \sup_{K \in \mathscr{K}} \lambda_\alpha^\bullet(f \varphi_K) = \sup_{\alpha \in A} \lambda_\alpha^\bullet(f).
$$

#### 系 1 {#int-v-s1-prop-11-cor-1 .statement tag=0908}

*T の部分集合 N が局所的に $\lambda$-無視できるためには、N がすべての $\alpha \in A$ について局所的に $\lambda_\alpha$-無視できることが必要かつ十分です。

#### 系 2 {#int-v-s1-prop-11-cor-2 .statement tag=0909}

*トポロジカル空間 G への T の写像 g が $\lambda$ 可測であるためには、すべての $\alpha \in A$ について $\lambda_\alpha$ 可測であることが必要かつ十分です。

$\alpha$ ごとに $\lambda_\alpha \leq \lambda$ があるため、条件は明らかに必要です (Ch. IV, §1, No. 3、提案 15)。 逆に、$g$ がすべての $\alpha$ に対して $\lambda_\alpha$ 可測であると仮定し、$g|K$ が連続となるような T のコンパクト部分集合 K の $\mathscr{K}$ 集合で表し、L を $L \cap K$ が次のようなコンパクト集合とします。 $\lambda$ - $K \in \mathscr{K}$ ごとに無視できます。 集合 $\mathscr{K}$ は $\lambda_\alpha$ 密であるため、L はすべての $\alpha$ について $\lambda_\alpha$ が無視できます (Ch. IV, §5, No. 8、提案 12)、したがって、$\lambda$ は無視できます (Cor. 1)。 したがって、$\mathscr{K}$ は $\lambda$ 密であり、$g$ は $\lambda$ 測定可能であるということになります (Ch. IV, §5, No. 10、提案 15)。

### 練習問題 {#int-v-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
