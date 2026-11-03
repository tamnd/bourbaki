---
book: int
book_title: Integration
chapter: VI
chapter_title: VECTORIAL INTEGRATION
section: 1
section_title: Integration of vector-valued functions
lang: ja
source: int-i-vi
pdf_pages: 0392-0409, 0447-0453
extraction: ocr
subsections:
    - "no": 1
      title: Scalarly essentially integrable functions
      page: 2
      pdf_page: 393
    - "no": 2
      title: Properties of the integral of a scalarly essentially integrable function
      page: 5
      pdf_page: 396
    - "no": 3
      title: Integrals of operators
      page: 7
      pdf_page: 398
    - "no": 4
      title: The property (GDF)
      page: 9
      pdf_page: 400
    - "no": 5
      title: Measurable mappings and scalarly measurable mappings
      page: 12
      pdf_page: 403
    - "no": 6
      title: 'Applications: I. Extension of a continuous function to a space of measures'
      page: 13
      pdf_page: 404
    - "no": 7
      title: 'Applications: II. Extension, to a space of measures, of a continuous function with values in a space of operators'
      page: 15
      pdf_page: 406
statements: 34
exercises: 27
content_sha256: f9944d7ae5e333dce8d1d7a6711bcaf792a1176b4253659c324cdc3f6a8fa47b
translated_from: content/en/int/VI/01_s1_integration_of_vector_valued_functions.md
translation_method: google
source_content_sha256: 9798f2a69885491f713db436a4833ff226e18b3becfed322106b65f6897d576a
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: cd6c68f8795adfbaf3f43711ce37603c0950a28cf8189841db08322c6c36cc92
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 1。ベクトル値写像の積分

この切断を通して、$\mu$ は T 上の正の測度を示し、F は $\mathbf{R}$ に対して局所的に凸なハウスドルフベクトル空間を示します。 F への T のすべての写像 f、および F の双対 $F'$ のすべての元 $z'$ について、T 上の数値写像 $z' \circ f$ を $\langle f, z' \rangle$ または $\langle z', f \rangle$ で表します。 すべての $z' \in F'$ に対して $\langle z', f \rangle$ に性質 $P$ がある場合、 f は *スカラー的に* 性質 $P$ を持つと言えます。 For example, we shall say that $f$ is *scalarly essentially $\mu$-integrable* if, for every $z' \in F'$, $\langle z', f \rangle$ is essentially $\mu$-integrable.\footnote{The special case $F = \mathscr{M}(X)$ ($X$ a locally compact space), equipped with the vague topology $\sigma(\mathscr{M}(X), \mathscr{K}(X))$, yields the concept of 'scalarly essentially $\mu$-integrable', for a mapping $f : T \to \mathscr{M}_+(X)$, defined in Ch. V, §3, No. 1.}

この定義、$F$の位相は、$F$の二重$F'$を媒介としてのみ介入することに注意してください。 写像 $f$ がスカラー的に性質 $P$ を持つ場合、$F$ の位相が、間の双対性と互換性のある局所的に凸なハウスドルフ位相に置き換えられると、再びスカラー的に性質 $P$ になります。 $F$と$F'$。

### 1. スカラー的に本質的に可積分関数

$f$ が本質的にスカラー的に $T$ の $F$ への $\mu$ 積分可能な写像である場合、写像 $z' \mapsto \int \langle f(t), z' \rangle d\mu(t)$ は $F'$ 上の線型形式、つまり代数双対の元です。 ${F'}^*$。

#### 定義 1 {#int-vi-s1-def-1 .statement tag=098E}

*1 は、$\mu$ に関する $f$ の積分* を呼び出し、* によって表されます* $\int f d\mu$ *または* $\int f(t) d\mu(t)$、* ${F'}^*$ の *元 *定義*
$$
\left\langle z', \int f d\mu \right\rangle = \int \langle z', f \rangle d\mu
$$
*全員に* $z' \in F'$。

$f$ がコンパクトなサポートで連続している場合、それはスカラー的に積分可能であり、Def. 1 一致するに、第 3 章で与えられた $f$ の積分の定義を加えます。 III, §3, No. 1。 一方、$F$ が Banach 空間であり、$f$ が本質的に可積分である場合 (Ch. V, §1, No. 3、デフォルト。 3) の場合、$f$ はスカラー的に本質的に積分可能であり、Def. 1 一致するに、章 V で与えられる $f$ の積分の定義を加えたもの (Ch. V, §1, No. 3 と Ch. IV, §4, No. 2、コル。 Thの1 1)。

#### 例 {#int-vi-s1-n1-exa-1 .statement tag=098F}

— $X$ を、$T$ の空間、$t \mapsto \lambda_t$ 写像を $X$ のメジャーの空間 $\mathscr{M}(X)$ に局所的に圧縮したものとします。家族 $t \mapsto \lambda_t$ が $\mu$ で十分であると言うということは、それが肯定的な尺度で構成されており、 写像 $t \mapsto \lambda_t$ がスカラー的に本質的に $\mu$ 可積分可能であり、 位相 $\sigma(\mathscr{M}(X), \mathscr{K}(X))$ について $\mu$ 可測であることを意味します。 章 5 の初版の「μ-adequate」の定義 (Ch. V、第 1 版、§3, No. 1、Def. 1)。前の章が翻訳である第 2 版では、 項 「μ-適切」 定義するより弱い (より一般的な) 概念 (Ch. V, §3, No. 1、定義 1)。より正確には、ポジティブな尺度のスカラー的に本質的に $\mu$ 可積分族 $t \mapsto \lambda_t$ は、章 V の初版の意味で $\mu$ が適切であり、それが第 2 版の意味で $\mu$ が適切であり、漠然とである場合に限ります。 $\mu$-測定可能、つまり、$\mu$-$\sigma(\mathscr{M}(X), \mathscr{K}(X))$ について測定可能 (Ch. V, §3, No. 1、提案 2 b))。 2 つの定義は、$X$ の位相が可算数の基底 (*同上*。提案 2 c)) を持つときは常に等しく、これは章 VI (§3) の場合に当てはまります。従って、章の残りの部分では、「μ-適切」の 2 つの解釈と第 42 章の初版への参照との間に区別はありません。 V は、第 2 版では最も近い同等のものに置き換えられました。}

$\mu$ に関する積分は、第 3 章で $\int \lambda_t\, d\mu(t)$ と示された尺度です。 V, §3, No. 1。

#### 注意 1 {#int-vi-s1-n1-rem-1 .statement tag=098G}

F が有限次元であれば、T から F へのスカラー的に本質的に積分可能なすべての写像は本質的に積分可能です (Ch. V, §1, No. 3)。しかし、一般的な場合、コンパクトな空間 T 上のスカラー的に無視できる写像は、$\mu$ 測定可能でさえない可能性があります (例 12)。

#### 注意 2 {#int-vi-s1-n1-rem-2 .statement tag=098H}

f の積分は、スカラー的に局所的に $\mu$ が無視できる F への T の写像の空間を法とする f の類にのみ依存することは明らかです。スカラー的に局所的に無視できる写像 g は、必ずしもほぼどこでも零であるわけではないことに注意してください (Exer. 12)。ただし、これは実際に、位相 $\sigma(F', F)$ に対して密な F' 数列 $(\mathbf{z}'_n)$ が存在する場合に当てはまります。つまり、$H_n$ が点 $t \in T$ の局所的に無視できる集合であり、$\langle g(t), \mathbf{z}'_n \rangle \neq 0$、和集合である場合です。 $H_n$ の H は局所的に無視でき、すべての $t \notin H$ について、すべての n、よって $g(t) = 0$ に対して $\langle g(t), \mathbf{z}'_n \rangle = 0$ が存在します。

u をハウスドルフ局所凸空間 G への F の連続線形写像とする。その転置 $^t u$ は $G'$ から $F'$ への線形写像であり、(代数) 転置 $^t(^t u)$ は u を拡張する ${F'}^*$ から ${G'}^*$ への線形写像であり、これを再び u で表します。 この規約により、次のようになります。

#### 命題 1 {#int-vi-s1-prop-1 .statement tag=098I}

— *f がスカラー的に本質的に $\mu$ 積分可能である T の F への写像である場合、写像 $u \circ f$ はスカラー的に本質的に $\mu$ 積分可能であり、*
$$
\int (u \circ f)\, d\mu = u \left( \int f\, d\mu \right).
$$
$\mathbf{z}' \in G'$、$\langle \mathbf{z}', u \circ f \rangle = \langle ^t u(\mathbf{z}'), f \rangle$、よってごとに最初の主張。 2 番目は公式から続きます
$$
\left\langle \mathbf{z}', \int (u \circ f)\, d\mu \right\rangle = \int \langle \mathbf{z}', u \circ f \rangle\, d\mu = \left\langle ^t u(\mathbf{z}'), \int f\, d\mu \right\rangle = \left\langle \mathbf{z}', u \left( \int f\, d\mu \right) \right\rangle.
$$

特に、f が本質的にスカラー的に $\mu$ 積分可能である場合、F の位相がより粗い位相に置き換えられても、 f は本質的にスカラー的に $\mu$ 積分可能のままです。

#### 命題 2 {#int-vi-s1-prop-2 .statement tag=098J}

— *f を、T から F への本質的にスカラー的に $\mu$ 積分可能な写像とする。 $\mu$ 可測で有界であるすべての数値写像 $g \geqslant 0$ について、T から F への写像 $t \mapsto g(t)f(t)$ (gf または fg で示す) は本質的にスカラー的に$\mu$-積分可能、f は本質的にスカラー的に $(g \cdot \mu)$-積分可能、および*
$$
\int f\, d(g \cdot \mu) = \int fg\, d\mu.
$$

これは、すべての $\mathbf{z}' \in F'$ に対する公式 $\langle \mathbf{z}', gf \rangle = g \langle \mathbf{z}', f \rangle$ の明らか帰結と、本質的にすべての $\mu$ 可積分スカラー 写像 $h$ の公式 $\int h d(g \cdot \mu) = \int hg d\mu$ です (Ch. V, §5, No. 3、Th. 1)。

本質的に可積分な数値写像についての非常に多くの命題は、 語の語を、スカラー的に本質的に可積分なベクトル値写像についての命題に転置することができます。 より重要なことの中で、写像が稠密度によって定義される測度に関して本質的に可積分であることについて、条件に注意を促します。 V, §5, No. 3、木。 1)、または小節の像に関して (Ch. V, §6, No. 2、木。 1）、または誘発された措置に関して（Ch. V, §7, No. 1、木。 1)、または要約可能な一連の積極的な措置の和に関して。 V, §2, No. 2、小道具。 1 と 3 および Cor.提案 1 の 3)。 これらの転置は読者に委ねられています。

ただし、「二重積分」で主張対応するから定理を得るには (Ch. V, §3, No. 3、木。 1 と §8, No. 4、Th。 1 (Lebesgue–Fubini 定理))、仮説を強化する必要があります (cf. Exer. 1)。 適用に前に引用した定理を写像 $\langle \mathbf{z}', f \rangle$ のそれぞれに適用すると、$\mathbf{z}' \in F'$ となり、次の命題が得られます。

#### 命題 3 {#int-vi-s1-prop-3 .statement tag=098K}

— $X$ を局所的にコンパクトな空間、$t \mapsto \lambda_t$ を $X$ の積極的な措置の $\mu$-適切$^3$ ファミリー (Ch. V, §3, No. 1、Def. 1) とし、$\nu = \int \lambda_t d\mu(t)$ とします。 $f$ を $X$ の写像から $F$ にします。 $1^\circ$ $f$ がスカラー的に $\nu$ 積分可能であると仮定します。 $2^\circ$ には、局所的に無視できる $\mu$ 集合 $N \subset T$ が存在し、$t \notin N$ ごとに、$f$ はスカラー的に $\lambda_t$ 積分可能であり、$\int f d\lambda_t \in F$ になります。次に、$t \notin N$ に対して定義された写像 $t \mapsto \int f d\lambda_t$ は、本質的にスカラー的に $\mu$ 積分可能であり、$^4$

$$
\int f(x) d\nu(x) = \int d\mu(t) \int f(x) d\lambda_t(x) .
$$

#### 命題 4 {#int-vi-s1-prop-4 .statement tag=098L}

— $T$ と $T'$ を 2 つの局所的にコンパクトな空間、$\mu$ (それぞれ $\mu'$) を $T$ (それぞれ $T'$) での正の測度、$\nu = \mu \otimes \mu'$ 積を $X = T \times T'$ での測度とする。 $f$を$X$の写像を$F$にします。 次のように仮定します。 $1^\circ$ $f$ はスカラー的に $\nu$ 積分可能です。 $2^\circ$、すべての $t \notin N$ について、マッピング $t' \mapsto f(t, t')$ がスカラー的に $\mu'$ 積分可能、および $\int f(t, t') d\mu'(t') \in F$ となるような、局所的な $\mu$ 無視可能な集合 $N \subset T$ が存在します。 次に、$t \notin N$ に対して定義された写像 $t \mapsto \int f(t, t') d\mu'(t')$ は、本質的にスカラー的に $\mu$ 積分可能であり、$^4$

$$
\iint f(t, t') d\mu(t) d\mu'(t') = \int d\mu(t) \int f(t, t') d\mu'(t') .
$$

$^3$族はスカラー的に本質的に $\mu$-可積分であると仮定するだけで十分であり、したがって命題は「$\mu$-十分」の 2 つの解釈のいずれにも当てはまります。
$^4$等式は ${F'}^*$ の元として。

### 2. 本質的にスカラーの積分の性質可積分関数

#### 命題 5 {#int-vi-s1-prop-5 .statement tag=098M}

— $\mu$を、$T$、$S$、$\mu$を運ぶ$\mu$可測集合の有界正の測度とする（Ch. V, §5, No. 7、デフォルト。 4)、$f$ は、$F$ の値とスカラー的に $\mu$ 積分可能 (*) 写像です。 位相 $\sigma(F', F')$ を備えた空間 $F'$* の $f(S)$ の閉じた凸包絡線を $D$ とします。 次に$\int f\, d\mu \in \mu(T)D$。

$D$ は閉じた半空間含む $f(S)$ (TVS、II, §5, No. 3、提案 4 の Cor. 1) の共通部分であるため、すべての $t \in S$ ($z' \in F', a \in \mathbf{R}$) について関係 $\langle f(t), z' \rangle \leq a$ が意味することを証明すれば十分です。 $\langle z', \int f\, d\mu \rangle \leq a \cdot \mu(T)$;しかし、$\int f\, d\mu = \int_S f\, d\mu$ 以降、これは第 6 章から続きます。 IV, §4, No. 2、コル。 Thの1 1.

#### 系 {#int-vi-s1-n2-cor-1 .statement tag=098N}

— $\mu$ を $T$ 、$S$ を $\mu$ を運ぶ $\mu$ 可測集合、および $f$ を $T$ から $F$ へ、スカラー的に $\mu$ 可測で、$f(S)$ となるような写像とする。は、$F$ の弱くコンパクトな凸サブセット $A$ に含まれています。 この場合、$f$ はスカラー的に $\mu$ 積分可能であり、$\int f\, d\mu \in \mu(T)A \subset F$ です。

すべての $z' \in F'$ に対して、$\langle z', f \rangle$ は $\mu$ 可測であり、$S$ で境界があるため、可積分可能です。これは、$f$ がスカラー的に可積分であることを証明します。また、$A$は$F_\sigma$でコンパクトなので$F'$*で閉じられ、$F'$*の$f(S)$の閉じた凸包絡線は$A$、よって系に含まれます。

#### 命題 6 {#int-vi-s1-prop-6 .statement tag=098O}

— $f$ を、$F$ の値をもつスカラー的に本質的に $\mu$ 積分可能な関数、つまり $\int f\, d\mu \in F$ とする。 $F$ の各下位半連続半ノルム $q$ について、

$$
q\left( \int f\, d\mu \right) \leq \int^\bullet (q \circ f)\, d\mu .
$$

$D$ を $z \in F$ の集合とし、$q(z) \leq 1$ とします。 $D$ は閉じており、凸であり、含む $0$ であるため、$D = D^{oo}$ (TVS、II, §6, No. 3、Th. 1 の Cor. 3)。従って、$z' \in D^\circ$ ごとに $|\langle z', \int f\, d\mu \rangle| \leq \int^\bullet (q \circ f)\, d\mu$ があることを証明すれば十分です。しかし、これは、$t \in T$ごとに$|\langle z', f(t) \rangle| \leq q(f(t))$という事実からすぐに得られます。

数値写像 $q \circ f$ は $\mu$ 測定可能である必要はないことに注意してください (例 12)。

#### 命題 7 {#int-vi-s1-prop-7 .statement tag=098P}

— $f$ を、$T$ から $F$ へのマッピングとし、スカラー的に本質的に $\mu$ 積分可能であり、すべてのコンパクトなサブセットに $T$、$f(K)$ の $K$ が含まれるようにします。

(*) *有界* 正測度 $\mu$ の場合、$\mu$ 可積分関数と本質的に $\mu$ 可積分関数の概念は同じであることを思い出してください (提案 9 の V, §1, No. 3 項)。

5 上部本質積分の元の記法は $\overline{\int^*}$ ですが、第 2 章の第 2 版では $\int^\bullet$ に変更されました。 V。

F の弱くコンパクトでバランスの取れた凸型の部分集合で、次に $\int f d\mu$ 属するが F の双双 $F''$ に。

T のすべてのコンパクト部分集合 K に対して、

$$
\int f \varphi_K d\mu = \int (f \varphi_K) d(\varphi_K \cdot \mu);
$$

コル。提案 5 の は、有界メジャー $\varphi_K \cdot \mu$ および写像 $f \varphi_K$ に適用でき、結果として $\int f \varphi_K d\mu \in F$ になります。 従って、すべての $z' \in F'$ に対して、$\langle z', f \rangle$ は本質的に $\mu$ 可積分です (Ch. V, §1, No. 3、提案 10)

$$
\int \langle z', f \rangle d\mu = \lim_K \int \langle z', f \rangle \varphi_K d\mu,
$$

Tのコンパクト部分集合の増加する有向集合に対して極限がとられています。この集合に関して、位相$\sigma({F'}^*, F')$に対して$\int f \varphi_K d\mu$が$\int f d\mu$に収束する結論するです。今、

$$
\left| \left\langle z', \int f \varphi_K d\mu \right\rangle \right| = \left| \int \langle z', f \rangle \varphi_K d\mu \right| \leq \int |\langle z', f \rangle| d\mu,
$$

これは、元 $\int f \varphi_K d\mu$ の集合が $F_\sigma$ の *有界* 部分集合であること、従って F の部分集合であることを証明します (TVS、IV, §1, No. 1、提案 1)。従って、命題 7 は、次の補題の帰結です。

#### 補題 1 {#int-vi-s1-lem-1 .statement tag=098Q}

*F のすべての有界部分集合の ${F'}^*$ (位相 $\sigma({F'}^*, F')$ の場合) の閉包は、双対 $F''$ に含まれます。

なぜなら、F の有界部分集合は、F の強い双対 $F'$ の 0 の近傍の極点 ($F''$ 内) に含まれているため、$\sigma(F'', F')$ の $F''$ では比較的コンパクトです (TVS、III, §3, No. 5、提案 7 および No. 4、提案 4 の Cor. 2)。 $\sigma(F'', F')$は$\sigma({F'}^*, F')$によって導かれるので、補題が証明されます。

#### 系 {#int-vi-s1-n2-cor-2 .statement tag=098R}

*F が半再帰的であると仮定し、f をスカラー的に本質的に $\mu$ 積分可能な T の F への写像とし、T の圧縮部分集合 K ごとに $f(K)$ が有界であるとします。次に、$\int f d\mu$ 属するを F に*します。

なぜなら、F のすべての有界部分集合は比較的弱くコンパクト (TVS、IV, §2, No. 2、Th. 1)、および $F = F''$ だからです。

#### 命題 8 {#int-vi-s1-prop-8 .statement tag=098S}

*$\mu$をT、S a $\mu$可測集合がTの$\mu$、f a $\mu$可測写像をFに運び、$f(S)$がFの完全で有界でバランスの取れた凸面部分集合Bに含まれるようにする。 f はスカラー的に $\mu$ 積分可能であり、 $\int f d\mu \in \mu(T)B \subset F$.*

Sは$\mu$可積分であるため、各$K_n$に対するfの制限が連続となるように、$\mu$-無視できる集合Nとコンパクト部分集合の数列$(K_n)$によって形成されるSの分割が存在します（Ch. IV, §4, No. 6、コリント 4 および §5, No. 1、定義 1)。従って、$f(K_n)$ は、$F$ のコンパクトな部分集合です。 $f(K_n)$ の閉じたバランスの取れた凸包絡線 $B_n$ は、事前コンパクト (TVS、II, §4, No. 1、提案 3) であり、$F$ の完全な部分集合 $B$ に含まれるため、コンパクトであり、*なおさら* は弱くコンパクトです。その結果、(提案 5 の修正) $f \varphi_{K_n}$ はスカラー的に $\mu$ 積分可能であり、

$$
z_n = \int f \varphi_{K_n} d\mu \in \mu(K_n)B_n \subset \mu(K_n)B .
$$

$F$ 上のすべての連続半ノルム $p$ について、次のことがわかります。

$$
p(z_n) \leq \mu(K_n) \cdot \sup_{x \in B} p(x) ;
$$

$B$ は有界であり、一般的な項 $\mu(K_n)$ を持つ系列は収束し、和 $\mu(T)$ を持つため、一般的な項 $s_n = z_1 + z_2 + \cdots + z_n$ を持つ数列は完全なコーシー 数列であることがわかります。 部分集合 $\mu(T)B$/$F$。 従って、この数列は $\mu(T)B$ の元 $s$ に収束します。 $T - S$ で $f(t) = 0$ と仮定できるので、ルベーグの定理を写像 $\langle z', f \rangle$ ($z' \in F'$) に適用すると、$s = \int f d\mu$ が証明されます。

### 3. 演算子の積分

$G$ と $H$ を $\mathbf{R}$ 上の 2 つのハウスドルフ局所凸空間とし、$F$ が *点ごとの* 収束のトポロジーを備えた $G$ から $H$ への連続線形写像の空間 $\mathscr{L}(G; H)$ であると仮定します。 $F$ 上のすべての連続線形形式は、積空間 $H^G$ (TVS、II, §4, No. 1、提案 2) 上の連続線形形式に拡張でき、従って $u \mapsto \sum_{i=1}^n \langle u(a_i), b'_i \rangle$ と書くことができます。ここで、$a_i$ (それぞれ $b'_i$) は $G$ (それぞれ双対 $H'$ の要素) です。 $H$)。 $T$ の $F$ への写像 $U$ がスカラー的に本質的に $\mu$ 可積分であると言うことは、すべての $a \in G$ とすべての $b \in H'$ について、数値関数 $t \mapsto \langle U(t) \cdot a, b' \rangle$ が本質的に $\mu$ 可積分であることを意味します。

#### 命題 9 {#int-vi-s1-prop-9 .statement tag=098T}

*$U$ を、スカラー的に本質的に $T$ を $F = \mathscr{L}_s(G; H)$ に積分可能な $\mu$ 写像とします。 位数その$\int U d\mu \in F$において、以下の2つ条件が満たされていれば必要十分です。

a) *$x \in G$、$\int (U(t) \cdot x) d\mu(t) \in H$ごとに。*

b) *$H'$ の各等連続部分集合 $B'$ について、線型形式 $u_{y'} : x \mapsto \int \langle U(t) \cdot x, y' \rangle d\mu(t)$ の集合 ($y'$ が $B'$ に重なる) は等連続です。*

条件 a)とb)は必須です。なぜなら、すべての $x \in G$, 写像 $\tilde{x} : V \mapsto V \cdot x$ の $\mathscr{L}_s(G; H)$ から $H$ への変換は線形であるため、(No. 1,

提案 1) $\widetilde{\mathbf{x}} \circ U : t \mapsto U(t) \cdot \mathbf{x}$ は本質的にスカラー的に $\mu$ 可積分可能であり、

$$
(1) \quad S \cdot \mathbf{x} = \int (U(t) \cdot \mathbf{x})\, d\mu(t),
$$

どこで$S = \int U\, d\mu \in \mathscr{L}_s(G; H)$。これは a) を証明します。また、(1) と書くこともあります。

$$
(2) \quad \langle S \cdot \mathbf{x}, \mathbf{y}' \rangle = \int \langle U(t) \cdot \mathbf{x}, \mathbf{y}' \rangle\, d\mu(t) = \langle \mathbf{x}, u_{\mathbf{y}'} \rangle,
$$

その他語 ${}^t S \cdot \mathbf{y}' = u_{\mathbf{y}'}$ で。 $S$ は連続なので、${}^t S$ 変換 $H'$ の各等連続部分集合を $G'$、よっての等連続部分集合に変換します。 b)。

逆に、a) と b) が検証されたとします。 a) により、公式 (1) 定義する線形写像 $S$ の $G$ を $H$ に変換し、すべての $\mathbf{y}' \in H'$ について、この写像は (2) (No. 1、提案 1) を満たします。しかしその後、条件 (b) は、$S$ が連続であると述べています (TVS、II, §6, No. 4、提案 5 と 6、および III, §3, No. 5、提案 7)、したがって $S \in \mathscr{L}_s(G; H)$ です。最後に、公式 (2) により、$S = \int U\, d\mu$ が証明されます。

#### 系 {#int-vi-s1-n3-cor-1 .statement tag=098U}

— *条件提案 9 の b) は、次の 2 つの場合のそれぞれで満たされます*:

$1^\circ$ *メジャー $\mu$ は有界であり、$S$ がそのサポートである場合、$U(S)$ は $\mathscr{L}(G; H)$* の等連続部分集合です。

提案 9 の $2^\circ$ *条件 a) が満たされ、空間 $G$ がバレル化され、$T$ の各コンパクト部分集合 $K$ について、$U(K)$ は$\mathscr{L}_s(G; H)$* の有界部分集合になります。

まず$1^\circ$のケースに身を置いてみましょう。 $S = T$ (Ch. V, §7, No. 1、Th. 1) の場合に限定できます。次に、$H'$ の各等連続部分集合 $B'$ に対して、すべての $\mathbf{y}' \in B'$ とすべての $t \in T$ に対して ${}^t U(t) \cdot \mathbf{y}' \in A'$ となるような、等連続で、凸状で、バランスが取れた弱く閉じた部分集合 $A' \subset G'$ が存在します (TVS、II, §6, No. 4、提案6)。 $U$ はスカラー的に $\mu$ 積分可能であるため、$\sigma(G', G)$ を備えた$G$ のデュアル $G'$ に $T$ の写像 $t \mapsto {}^t U(t) \cdot \mathbf{y}'$ はスカラー的に $\mu$ 積分可能であり、次のように書くことができます。

$$
u_{\mathbf{y}'} = \int ({}^t U(t) \cdot \mathbf{y}')\, d\mu(t).
$$

$A'$ は $\sigma(G', G)$ に対して凸でコンパクトなので、Cor. No. 2 の提案 5 は、$\mathbf{y}' \in B'$ ごとに $u_{\mathbf{y}'} \in \mu(T)A'$ であることを示しており、これは私たちの主張を証明します。

ここで$2^\circ$のケースに身を置いてみましょう。すべての $\mathbf{y}' \in H'$ およびすべてのコンパクト部分集合 $K$ の $T$、集合

$$
u_{K, \mathbf{y}'} = \int \varphi_K(t) ({}^t U(t) \cdot \mathbf{y}')\, d\mu(t),
$$

$G$ の代数双対 $G^*$ の元。 $G$ はバレル化されているため、$\mathscr{L}_s(G; H)$ のすべての境界付き部分集合は等連続です (TVS、III, §4, No. 2、Th. 1)。引数の最初の部分は、写像 $\varphi_K U$ と制限されたメジャー $\varphi_K \cdot \mu$ に適用され、$u_{K, y'} \in G'$ を示します。さらに、位相 $\sigma(G^*, G)$ については、$T$ のコンパクト部分集合の増加する有向集合に関して、$u_{y'} = \lim_{K} = u_{K, y'}$、極限が取られます (Ch. V, §1, No. 3、提案 10)。提案 9 の条件 b) を検証するには、提案 9 により、(1) で定義された $G$ の $H$ への線形写像 $S$ が連続であることを証明するだけで十分です。さらに、$G$ はバレル化されているため、$G$ と $H$ が弱められたトポロジーを備えている場合、$S$ が連続であることを証明するだけで十分です (TVS、IV, §1, No. 3、提案 7)。最後に、(2) により、$y' \in H'$ ごとに $u_{y'} \in G'$ が表示されることになります。 $u_{y'}$ は、$u_{K, y'}$ の集合 $M'$ の$\sigma(G^*, G)$ に対して閉包内にあるため、$K$ は $T$ のコンパクト部分集合の集合を超えますので、次のことを証明すれば十分です。 $M'$ は等連続です (TVS、III, §3, No. 4、提案 4)。そして、$G$ はバレル化されているため、すべての $x \in G$ について、$\langle x, u_{K, y'} \rangle$ の集合が制限されていると言えることになります (TVS、III, §4, No. 2、Th. 1)。しかし、これは関係から一気に続きます。

$$
|\langle x, u_{K, y'} \rangle| = \left| \int \varphi_K(t) \langle U(t) \cdot x, y' \rangle d\mu(t) \right| \leq \int |\langle U(t) \cdot x, y' \rangle| d\mu(t).
$$

#### 命題 10 {#int-vi-s1-prop-10 .statement tag=098V}

— *$U$を$T$の写像を$F = \mathscr{L}_s(G; H)$にします。次の 3 つのケースのそれぞれで、$U$ は本質的にスカラー的に $\mu$ 積分可能であり、$\int U d\mu \in \mathscr{L}_s(G; H)$ です。

a) $H$ は準完全で、$\mu$ は有界であり、$S$ がそのサポートである場合、$U$ は$\mu$ 可測であり、$U(S)$ は等連続です。

b) $H$ は半再帰的であり、$\mu$ は有界であり、$S$ がそのサポートである場合、$U$ はスカラー的に $\mu$ 可測であり、$U(S)$ は等連続です。

c) $H$ は半再帰、$G$ はバレル、$U$ はスカラー的に本質的に $\mu$ 積分可能で、$T$ のすべてのコンパクト部分集合 $K$ について、$U(K)$ は有界です。

$U$ がスカラー的に本質的に可積分であるという事実は、3 つのケースすべてで明らかです。提案 9 とその系により、各ケースにおいて提案 9 の条件 a) を検証するだけで十分です。 さて、この条件は、最初のケースの No. 2 の提案 8 と Cor.他の 2 つのケースでは、No. 2 の提案 7 の。

### 4. 性質 (GDF)

この番号では、次の性質 (「可算閉グラフ」 性質と呼ばれます) を持つ局所凸空間 $F$ を検討します。

⁶ *Graphe dénombrablement fermé*、よってのイニシャル (GDF)。

(GDF) *u が F の線形写像から Banach 空間 B で、積空間 F × B において、u のグラフ Γ のすべての収束数列の点のすべての極限が再び属するから Γ になる場合、u は連続です。*

すべてのフレシェ空間には性質 (GDF) (TVS、I, §3, No. 3、Th. 1 の Cor. 5) があります。 付録では、空間の他の例が性質 (GDF) を持っていることがわかります。

#### 命題 11 {#int-vi-s1-prop-11 .statement tag=098W}

*各ハウスドルフの局所凸型空間 F と性質 (GDF) はバレル化されています。*

V を F のバレル、q をゲージ、F の準ノルムとします。 H を、この単一の半ノルムによって定義される位相を備えた空間 F に関連付けられたハウスドルフ空間とします。 H の完成 $\widehat{H}$ は Banach 空間です。 $\pi$ を F の標準写像を $\widehat{H}$ にします。 $\pi$ が *連続* であることを示します (F の元の位相の場合)。これにより、命題が確立されます。なぜなら、$\widehat{H}$ の単位元ボールの$\pi$ の下にあるV、逆像が F の 0 の近傍になるからです。 $\pi$ の連続性を確立するには、(GDF) のおかげで、次のグラフが示されるだけで十分です。 $\pi$は$F \times \widehat{H}$で*休業中*です。他の語では、$\mathscr{F}$ が F のフィルターで、$x \in F$ に収束し、その像 $\pi(\mathscr{F})$ が $y \in \widehat{H}$ に収束し、次に $y = \pi(x)$ に収束することを確認する必要があります。さて、$F'$のVの極点$V^\circ$の各元$x'$は、$\widehat{H}$（再び$x'$と示されています）とこれらの集合の連続する線型形式に一方向でのみ拡張できます。 形は $\widehat{H}$ の双対の単位元ボールです。したがって、$x' \in V^\circ$ ごとに $\langle y, x' \rangle = \langle \pi(x), x' \rangle$ を示すだけで十分です。しかし、これは関係から続きます

$$
\langle y, x' \rangle = \lim_{\mathscr{F}} \langle \pi(z), x' \rangle = \lim_{\mathscr{F}} \langle z, x' \rangle = \langle x, x' \rangle = \langle \pi(x), x' \rangle .
$$

#### 定理 1 {#int-vi-s1-thm-1 .statement tag=098X}

(Gelfand–Dunford)—*F を、性質 (GDF)、$F'_s$ の弱い双対を持つ局所的に凸なハウスドルフ空間とします。スカラー的に本質的に $\mu$ 積分可能である $F'_s$ への T のすべての写像 f について、$\int f d\mu$ 属するから $F'$ への積分です。*

$F'_s$ の双対が F (TVS、II, §6, No. 2、提案 3) であることを思い出してください。したがって、すべての $z \in F$ に対して、数値写像 $\langle z, f \rangle$ は本質的に $\mu$ 可積分です。 $L^1(\mu)$ の類を $\theta(z)$ とします。 $\int f d\mu \in F'$ を示すには、線型形式 $z \mapsto \langle z, \int f d\mu \rangle$ が F 上で連続であることを証明する必要があります。実際、次のより強力な結果を証明します。

#### 補題 2 {#int-vi-s1-lem-2 .statement tag=098Y}

*f を T の $F'_s$ への写像とし、$z \in F$ ごとに数値写像 $\langle z, f \rangle$ 属するから $\overline{\mathscr{L}}^p(\mu)$ ($1 \leq p \leq +\infty$) とします。 $L^p(\mu)$のこの写像の類を$\theta(z)$とします。次に、$z \mapsto \theta(z)$ は、F の線形写像が $L^p(\mu)$ に連続したものになります。

(GDF) 特性により、$(\theta(z_n))$ が $u \in L^p(\mu)$ に収束するような、$z$ に収束する F の要素のすべてのシーケンス $(z_n)$ に対して、$u = \theta(z)$ が存在することを示すだけで十分です。 ここで、サブシーケンスによって置き換えること必要に応じて数列 $(z_n)$ を使用すると、写像 $\langle z_n, f \rangle$ の数列がほぼどこでも局所的に写像 $h \in \overline{\mathscr{L}}^p(\mu)$ に収束し、$L^p(\mu)$ では類 $u$ が生じると仮定できます。 (Ch. IV, §3, No. 4、木。 3およびCh. V, §1, No. 3)。 仮定までに、すべての $t \in T$ 数列 $(\langle z_n, f(t) \rangle)$ が $\langle z, f(t) \rangle$ に収束するため、ほぼどこでも局所的に $h(t) = \langle z, f(t) \rangle$ があり、その結果、$u = \theta(z)$ になります。

#### 系 1 {#int-vi-s1-lem-2-cor-1 .statement tag=098Z}

*$G_i$ ($1 \leq i \leq n$) を性質 (GDF) を持つ局所凸ハウスドルフ $n$ 空間とし、$F$ を点単位収束の位相を備えた $\prod_{i=1}^n G_i$ 上で個別に連続する多重線形形式の空間とします。 $T$ の $F$ へのすべての写像 $f$ は、本質的にスカラー的に $\mu$ 積分可能であり、$\int f d\mu \in F$ になります。*

空間 $F$ はテンソル積 $\bigotimes_{i=1}^n G_i$ と双対関係にあり、$F$ への点収束の位相は他ならぬ位相 $\sigma(F, \bigotimes_{i=1}^n G_i)$ です。 従って、代数双対 ${F'}^*$ は、$\prod_{i=1}^n G_i$ 上のすべての多重線形形式の空間です。 $z = (z_1, \ldots, z_n)$ を $\prod_{i=1}^n G_i$ の要素とします。すべての多重線形形式 $u \in {F'}^*$ について、マッピング $x \mapsto u(z_1, \ldots, z_{i-1}, x, z_{i+1}, \ldots, z_n)$ は $G_i$ 上の線形形式であり、これを $\lambda_i(z)(u)$ で表します。従って、トポロジー $\sigma({F'}^*, \bigotimes_{i=1}^n G_i)$ と $\sigma(G_i^*, G_i)$ に対して連続する、${F'}^*$ の線形写像 $\lambda_i(z)$ から $G_i$ の代数双対 $G_i^*$ への写像が得られます。 $u \in F$ ということは、添字 $i$ と $z \in \prod_{i=1}^n G_i$ ごとに $\lambda_i(z)(u) \in G_i'$ があることを意味します。 さて、No. 1の提案1により、$F$の写像$\lambda_i(z)$は、位相$\sigma(G_i', G_i)$を備えた$T$の$G_i'$へのスカラー的に本質的に$\mu$積分可能な写像であり、そして
$$
\int (\lambda_i(z) \circ f) d\mu = \lambda_i(z) \left( \int f d\mu \right).
$$
Thさんより1、$1 \leq i \leq n$の$\int (\lambda_i(z) \circ f) d\mu \in G_i'$、従って$\int f d\mu \in F$。

#### 系 2 {#int-vi-s1-lem-2-cor-2 .statement tag=0990}

*$G$ を性質 (GDF) を持つ局所凸ハウスドルフ空間とし、$H$ を半反射型空間とし、その強い双対 $H_b'$ は性質 (GDF) (cf. App., No. 2,提案 3)。 $F$ を空間 $\mathscr{L}_s(G; H)$ とします。 $T$ のすべての写像 $U$ を $F$ に変換するもので、本質的にスカラー的に $\mu$ 積分可能であり、$\int U d\mu$ 属するから $F$ までの積分です。

$G$ はバレル化されているため (提案 11)、$\mathscr{L}(G; H) = \mathscr{L}(G_\sigma; H_\sigma)$ (TVS、IV, §1, No. 3、提案 7)。さらに、2 つの空間は同じ双対 $G \otimes H'$ を持っているため、置き換える $F = \mathscr{L}_s(G; H)$ を空間 $\mathscr{L}_s(G_\sigma; H_\sigma)$ で行うことができます (TVS、II, §6, No. 2、提案 3、および上記 No. 3 の最初の段落)。 $u \in \mathscr{L}(G; H) = \mathscr{L}(G_\sigma; H_\sigma)$ ごとに 1 つの集合 $\tilde{u}(x, y') = \langle u(x, y') \rangle$ ($x \in G$ の場合、 y' \in H' ) の場合、線形写像 $u \mapsto \tilde{u}$ は、個別に連続する双線形形式の空間 $F_1$ に対する F の全単射です。 $G_\sigma \times H'_s$、ここで$H'_s$は、弱い位相$\sigma(H', H)$（App.、No. 1）を装備したデュアル$H'$を表します。さらに、この写像は、点ごとの収束 (*loc. cit.*) の位相を備えた $\mathscr{L}_s(G_\sigma; H_\sigma)$ の $F_1$ への同型です。しかし、仮定によりHは$H'_b$の双対であるため、$F_1$は$G \times H'_b$に別途連続した双線形形式の空間でもあります。コル。従って、2 は Cor から導き出されます。 1.

Cor に注意してください。 2 は、G が *Banach 空間* であり、H が *再帰的 Banach 空間* である場合に特に当てはまります。

### 5. 測定可能写像およびスカラー測定可能写像

局所的にハウスドルフに凸な空間 F への T の写像 f がスカラー的に $\mu$ 可測である場合、一般に f が $\mu$ 可測であるということにはなりません (Exer. 12)。それにもかかわらず:

#### 命題 12 {#int-vi-s1-prop-12 .statement tag=0991}

*F が分離可能で計化可能な局所的に凸な空間である場合、T から F へのすべてのスカラー的に $\mu$ 可測写像 f は $\mu$ 可測です。

なぜなら、F は Banach 空間の可算積 $\prod_n E_n$ の部分空間と見なすことができ (TVS、II, §1, No. 3、提案 3)、$\mathrm{pr}_n(F)$ は $E_n$ 内で密であり、したがって分離可能であると仮定できます。すべての n について、写像 $\mathrm{pr}_n \circ f$ はスカラー的に $\mu$ 測定可能であるため、$\mu$ 測定可能 (提案 10 のIV, §5, No. 5、Cor. 2)、その結果、 f は $\mu$ 測定可能です (Ch. IV, §5, No. 3、Th 1)。

#### 命題 13 {#int-vi-s1-prop-13 .statement tag=0992}

*F を局所凸空間とします。これは、分離可能、計化可能な局所凸空間 $F_n$ の数列の直接極限であり、F は $F_n$ の和集合です。 $F'$ を F の双対とし、位相 $\sigma(F', F)$ を装備します。すると、T の $F'$ へのスカラー的に $\mu$ 可測の写像 f はすべて $\mu$ 可測になります。*

まず、F が計量可能かつ分離可能であると仮定し、D を F の可算密集集合とします。 $(V_n)$ を F の平衡、凸、開いた近傍 0 の減少する基本数列とします。極集合 $V_n^\circ$ は等連続であり、それらの和集合はすべて $F'$ です。 $T_n = f(V_n^\circ)$ にしましょう。 数列 $(T_n)$ は増加すると $T = \bigcup T_n$ です。それぞれの $T_n$ が $\mu$-*測定可能* であることを示しましょう。確かに、$D \cap V_n^n$は$V_n$に密集しています。 $y \in D \cap V_n$ ごとに、$S_y$ を $t \in T$ の集合とし、$|\langle y, f(t) \rangle| \leq 1$ とします。 仮定は、$S_y$ のそれぞれが可測であることを意味し、$T_n$ は、$S_y$ ($y \in D \cap V_n$) の可算族の共通部分であることを意味します。そうなると、T のすべてのコンパクト部分集合 K とすべての $\varepsilon > 0$ に対して、$\mu(K - (K \cap T_n)) \leq \frac{\varepsilon}{4}$ となるような整数 n が存在し、その後 $\mu((K \cap T_n) - K_1) \leq \frac{\varepsilon}{4}$ となるような $K \cap T_n$ のコンパクト部分集合 $K_1$ が存在します。最後に、$\mu(K_1 - K_2) \leq \frac{\varepsilon}{2}$ と、写像 $\langle y, f \rangle$ ($y \in D$) のすべての制限から $K_2$ が連続するような、$K_1$ のコンパクト部分集合 $K_2$ が存在します (Ch. IV, §5, No. 1,提案 2)。 集合 $f(K_2) \subset f(T_n) \subset V_n^\circ$ は等連続であるため、$f(K_2)$ 上の $\sigma(F', F)$ によって誘導される位相は、$D$ (GT, X, §2, No. 4, Th. 1) での点収束の位相と同一です。従って、$f$ から $K_2$ の制限は連続し、最初のケースではよってが主張になります。

一般的なケースに移りましょう。 $z'$ が $F$ で連続する線型形式である場合、その制限 $z'_n$ から $F_n$ は連続します。 $F = \bigcup_n F_n$ 以降、$F$ の双対 $F'$ は、積 $\prod_n F'_n$ および $\operatorname{pr}_n z' = z'_n$ の線形部分空間で (代数的に) 識別される可能性があります。さらに、$F$ のそれぞれの有限部分集合は $F_n$ の 1 つに含まれているため、位相 $\sigma(F', F)$ はトポロジー $\sigma(F'_n, F_n)$ の積位相によって引き起こされる位相に他なりません。そうなると、$t \in T$ごとに$\operatorname{pr}_n(f(t))$は$f(t)$から$F_n$の制限となるため、$f$がスカラー的に$\mu$測定可能である場合、$\operatorname{pr}_n \circ f$はスカラー的に$\mu$測定可能です。 証明の最初の部分は、$\operatorname{pr}_n \circ f$ がすべての $n$ に対して $\mu$ 測定可能であることを示しており、従って、$f$ も同様です (Ch. IV, §5, No. 3、Th. 1)。

### 6. Applications: I. 写像から空間までの連続した措置の拡大

$T$ を局所コンパクト空間、$F$ を準完全、ハウスドルフ局所凸空間、$f$ を $T$ から $F$ への連続写像とする。 $\mu$ が $T$ のポジティブな尺度であり、コンパクトサポート $S$ がある場合、$f(S)$ はコンパクトです。 $f(S)$ の閉じた凸包絡線はコンパクト (TVS、III, §1, No. 6) であるため、$f$ はスカラー的に $\mu$ 積分可能であり、$\int f \, d\mu \in F$ (No. 2、提案 5 の補正)。 $\lambda$ がコンパクトなサポートを備えた実際のメジャーである場合、$\lambda^+$ と $\lambda^-$ はコンパクトなサポートを備えたポジティブなメジャーです。 設定 $\int f \, d\lambda = \int f \, d\lambda^+ - \int f \, d\lambda^-$、(関係 $(\lambda + \mu)^+ + \lambda^- + \mu^- = \lambda^+ + \mu^+ + (\lambda + \mu)^-$ を使用して) $\lambda \mapsto \int f \, d\lambda$ が、コンパクトなサポートを持つ $T$ のメジャーの空間 $\mathscr{C}'(T)$ の線形写像であり、局所的に凸な空間であることがすぐに検証されます。 $F$。

ここで、$\mathscr{C}(T)$ にコンパクトな収束の位相が装備されている場合 (この文では常に仮定します)、空間 $\mathscr{C}'(T)$ は、$T$ (よっての記法) 上の連続数値写像の双対空間 $\mathscr{C}(T)$ と識別される可能性があることを観察しましょう。いいえ、そして次の1つで）：なぜなら、それは一方では知られています（Ch. IV, §4, No. 8、提案14) $\mathscr{C}(T)$の連続線型形式まで拡張できる$T$の措置がコンパクトサポート付きの措置であり、逆に$\mathscr{C}(T)$の連続線型形式の制限から$\mathscr{K}(T)$が措置となる（位相以降） $\mathscr{K}(T)$ は、$\mathscr{C}(T)$ の位相によって引き起こされるものよりもより細かいです)。

#### 命題 14 {#int-vi-s1-prop-14 .statement tag=0993}

*T を局所コンパクト空間、F を準完全、ハウスドルフ局所凸空間、f を T から F への連続写像とする。 コンパクトなサポートを備えた T 上のメジャーの空間 $\mathscr{C}'(T)$ が、$\mathscr{C}(T)$ のコンパクトなサブセットにおける一様収束のトポロジーを備えている場合、マッピング $\lambda \mapsto \int f d\lambda$ は、$t \in T$ ごとに $\tilde{f}(\varepsilon_t) = f(t)$ となるような、F への $\mathscr{C}'(T)$ の固有の連続線形マッピング $\tilde{f}$ です。

拡大の一意性を確立するには、点が$\mathscr{C}'(T)$の$\varepsilon_t$形の合計集合を測定することを確認するだけで十分です。 $\mathscr{C}'(T)$ の双対は $\mathscr{C}(T)$ (TVS, IV, §1, No. 1, Th. 1) であるため、すべてのメジャー $\varepsilon_t$ に直交するすべての写像 $g \in \mathscr{C}(T)$ が定義 (TVS, IV, §1, No. 2,提案 2)。

$\lambda \mapsto \int f d\lambda$ が連続であることを示しましょう。 V を F の 0 の閉じたバランスの取れた凸近傍とします。 関係 $\lambda \in L^\circ$ と $z' \in V^\circ$ が $|\langle \int f d\lambda, z' \rangle| \leq 1$ を、または再び $|\int \langle f, z' \rangle d\lambda| \leq 1$ を暗示するような、$\mathscr{C}(T)$ の比較的コンパクトな部分集合 L が存在することを証明すれば十分です。この目的のために、$z'$ が $V^\circ$ を超えるため、数値写像 $\langle f, z' \rangle$ の集合 L が $\mathscr{C}(T)$ で比較的コンパクトであることを示します。 $V^\circ$ は $\sigma(F', F)$ に限定されているため、$t \in T$ が固定され、$V^\circ$ を超える $z'$ に対する数 $|\langle f(t), z' \rangle|$ の上限は有限です。したがって、アスコリの定理 (GT、X, §2, No. 5、Th. 2 の Cor. 2) のおかげで、$\langle f, z' \rangle$ ($z' \in V^\circ$) の集合が *等連続* であることを示すだけで十分です。しかし、すべての $t_0 \in T$ とすべての $\delta > 0$ に対して、すべての $t \in W$ に対して $f(t) - f(t_0) \in \delta V$ となるような T の $t_0$ の近傍 W が仮定までに存在します。すべての $t \in W$ とすべての $z' \in V^\circ$ に対して $|\langle f(t), z' \rangle - \langle f(t_0), z' \rangle| \leq \delta$ となり、証明が完成します。

#### 注意 {#int-vi-s1-n6-rem-1 .statement tag=0994}

— 1) 写像 $t \mapsto \varepsilon_t$ は、T の空間 $\mathscr{C}'(T)$ への *同相同型* です。なぜなら、L が $\mathscr{C}(T)$ と $t_0 \in T$ のコンパクト部分集合である場合、すべての $t \in W$ とすべての写像に対して $|g(t) - g(t_0)| \leq 1$ となるような $t_0$ の近傍 W が存在します (GT、X, §2, No. 5、Th. 2 の Cor. 3)。 $g \in L$、したがって、$t \in W$ の$\varepsilon_t - \varepsilon_{t_0} \in L^\circ$ は、$t \mapsto \varepsilon_t$ の連続性を証明します (cf. Ch. IV, §4, No. 8、提案 15); 加法で、逆行列写像が曖昧な位相に対してすでに連続であることがわかります (Ch. III, §1, No. 9、提案 13)、したがって、$\mathscr{C}(T)$ のコンパクトな部分集合における一様収束の位相に対して *なおさら* となります。 次に、$t \mapsto \varepsilon_t$を介して$\mathscr{C}'(T)$の像でTを識別すると、$\lambda \mapsto \int f d\lambda$は*線型*写像に対するfの一意の*連続拡大*であると言えます。

2) $\lambda \mapsto \int f d\lambda$ の連続性の証明では、F が準完全であるという事実を使用していないことに注意してください。したがって、提案 14 の結論は、この仮定がなくても、加法で、コンパクトなサポートを備えたすべての肯定的な手段 $\mu$ に対して $\int f d\mu \in F$ であることがわかっている限り、依然として有効です。

ここで、$f(T)$ が F の *有界* 部分集合であると仮定します。すると、T 上のすべての *有界* 正の測度 $\mu$ について、f はスカラー的に $\mu$ 積分可能であり、 $\int f d\mu \in F$

(No. 2、提案8)。 $\lambda$ が $T$ 上の任意の有界実測度である場合、$\lambda^+$ と $\lambda^-$ は有界であり、上記のように定義された $\lambda \mapsto \int f\, d\lambda$ は、$T$ 上の *有界* 測度の空間 $\mathscr{M}^1(T)$ の *線型* 写像であることがすぐにわかります。局所的に凸の空間 $F$、それは明らかに拡大する写像 $\lambda \mapsto \int f\, d\lambda$ の $\mathscr{C}'(T)$ が $F$ になります。

#### 命題 15 {#int-vi-s1-prop-15 .statement tag=0995}

*$T$を局所的にコンパクトな空間、$F$を準完全なハウスドルフの局所的に凸な空間、$f$を$f(T)$が有界となるような$T$の$F$への連続写像とする。 $\mathscr{M}^1(T)$ にバナッハ空間位相が装備されている場合、$\mathscr{M}^1(T)$ から $F$ への線形写像 $\lambda \mapsto \int f\, d\lambda$ が連続します。

$F$ の 0 の閉じたバランスのとれた凸近傍 $V$ ごとに、$f(T) \subset \rho V$ となるような $\rho > 0$ が存在します。したがって、$f(T)$ の閉じた平衡型の凸包絡線 $B$ は $\rho V$ に含まれ、仮定までに完成します。 $\| \lambda \| \leq 1/\rho$ の場合、No. 2、提案 8、および関係 $\| \lambda \| = \lambda^+(T) + \lambda^-(T)$ から、$\int f\, d\lambda \in B/\rho \subset V$ になります。

### 7. アプリケーション: II。演算子の空間で値と連続する写像の小節の拡大から空間まで

$G$ をハウスドルフ局所凸空間、$H$ ハウスドルフおよび準完全局所凸空間とし、連続線形写像の $F$ 空間 $\mathscr{L}(G; H)$ で表す$G$を$H$に、*コンパクトコンバージェンス*の位相を搭載。 空間 $F$ は必ずしも準完全ではなく、$t \mapsto U(t)$ が $T$ から $F$ への継続的な写像であり、$\mu$ がコンパクトなサポートを備えた $T$ に対する正の尺度である場合、必ずしも$\int U\, d\mu \in F$ を持つとは限りません (Exer. 27）。ただし、$T$ のすべてのコンパクト部分集合 $K$ について、$U(K)$ が *等連続* である場合、$F$ の平衡凸包絡線も等連続 (TVS、III, §3, No. 4) であり、$H$ が準完全であるため、この平衡型の閉包は凸型エンベロープは、$F$ の完全な部分集合になります (TVS、III, §3, No. 8、提案 11)。その場合、確かに $\int U\, d\mu \in F$ (No. 2、提案 8) が得られます。

$U$ に課せられた補足条件は、別の方法で表現される場合もあります。

#### 補題 3 {#int-vi-s1-lem-3 .statement tag=0996}

*$G, H$を、局所的にコンパクトな空間$T$を$\mathscr{L}(G; H)$に局所的に凸にした2つの空間、$U$写像とする。次の条件は同等です。
a) $T \times G$ から $H$ への写像 $(t, x) \mapsto U(t) \cdot x$ は連続です。
b) $T$ のすべてのコンパクト部分集合 $K$ について、$U(K)$ は等連続であり、すべての $x \in D$、写像 $t \mapsto U(t) \cdot x$ が連続するような合計集合 $D \subset G$ が存在します。 $T$.*

また、$U$がこれら条件を満たす場合、$U$は$T$をコンパクトコンバージェンス位相を備えた$\mathscr{L}(G; H)$に連続写像となります。

a) が b) を意味することを確認するには、$H$ の 0 の近傍 $V$ とすべての $t \in K$ について、仮定までに $T$ の $t$ の近傍 $L_t$ と $G$ の 0 の近傍 $W_t$ が存在することを観察します。 関係 $t' \in L_t$ と $x \in W_t$ は $U(t') \cdot x \in V$ を暗示します。 $K$ を近傍 $L_{t_i}$ の有限数でカバーし、位数の $W = \bigcap_i W_{t_i}$ を$t \in K$ と $x \in W$ のたびに$U(t) \cdot x \in V$ とするだけで十分であり、$U(K)$ の等連続性を証明します。

逆に、b) が検証されたとします。 $T$ のすべてのコンパクト部分集合 $K$ について、写像 $(t, x) \mapsto U(t) \cdot x$ が $K \times G$ で連続であることを示すだけで十分です。 $M = U(K)$ にしましょう。 $M$ は等連続であるため、$M$ では、$G$ の点ごとの収束の位相は、$D$ の点ごとの収束の位相 (GT、X, §2, No. 4、Th. 1) と同一になります。したがって、仮定 b) は、$\mathscr{L}(G; H)$ に点単位収束の位相が装備されている場合、$t \mapsto U(t)$ は $K$ から $\mathscr{L}(G; H)$ への連続的な写像であることを意味します。一方、$(A, x) \mapsto A \cdot x$ は、$M$ に点収束の位相が装備されている場合 (GT、X, §2, No. 1、提案 1 の Cor. 4)、$M \times G$ から $H$ への連続的な写像です。 写像 $(t, x) \mapsto U(t) \cdot x$ は $(t, x) \mapsto (U(t), x) \mapsto U(t) \cdot x$ として因数分解できるため、結論するは連続であることがわかります。

最後に、補題の最後の主張は、$M$ においてコンパクト収束の位相がポイントワイズ収束 (GT, X, §2, No. 4, Th. 1) のそれと同一であるという事実から導き出されます。

したがって、$U$ が補題 3 の条件を満たすと仮定します。次に ($H$ が準完全である場合) No. 6、$\mathscr{C}'(T)$ の線形写像 $\lambda \mapsto \int U d\lambda$ を $F = \mathscr{L}(G; H)$ に変換するように、1 つの定義するを追加します。私たちは集合 $U(\lambda) = \int U d\lambda$です。

#### 命題 16 {#int-vi-s1-prop-16 .statement tag=0997}

— $G, H$ を 2 つのハウスドルフ局所凸空間とし、$H$ を準完全であると仮定します。 $U$ を $T$ から $\mathscr{L}(G; H)$ への写像とし、$(t, x) \mapsto U(t) \cdot x$ が $T \times G$ から $H$ への連続する写像とします。次に、$\mathscr{C}'(T) \times G$ の $H$ への双線形写像 $(\lambda, x) \mapsto U(\lambda) \cdot x$ は、$\mathscr{C}'(T)$ の等連続部分集合および$G$ のコンパクト部分集合と比べて非連続です (これは、線形写像 $\lambda \mapsto U(\lambda)$ が意味します) $\mathscr{C}'(T)$ から $F$ は連続です)。

$\mathscr{C}'(T)$の写像としての$\lambda \mapsto U(t)$の$F$への連続性は、No. 6の提案14に続く補題3と注意2から続きます。従って、$H$ の 0 の閉じたバランスのとれた凸近傍 $V$ と、$\mathscr{C}'(T)$ の等連続部分集合 $N$ ごとに、$G$ に 0 の近傍 $W$ が存在し、関係 $x \in W, \lambda \in N$ が意味することを証明する必要があります。それは$U(\lambda) \cdot x \in V$です。 $N = S^\circ$ ($S$ は $\mathscr{C}(T)$ の 0 の近傍です) と仮定できます。その結果、$S$ は写像 $g \in \mathscr{C}(T)$ の集合であると仮定できます。つまり、コンパクト部分集合上の $|g(t)| \leq 1$ です。 $T$の$K$。それを示せば十分です

|⟨U(λ)・x,x′⟩| x ∈ W、x′ ∈ V°、および λ ∈ S° の場合は ≤ 1。さて、U(K) は等連続であるため、 関係 t ∈ K, x ∈ W は U(t) · x ∈ V を意味するような 0 の近傍 W が G に存在します。したがって、関係 x ∈ W, x′ ∈ V° は、S に対して写像 t ↦ ⟨U(t) · x, x′⟩ 属するを意味するため、 |⟨U(t) · x, x′⟩| = |∫⟨U(t) · x, x′⟩ dλ(t)| ≤ 1 x 定義 S°。

ここで、U が T から F への連続写像であり、さらに U(T) が等連続であると仮定しましょう。 次に、上記と同じ推論は、(H が準完全であるため) T 上のすべての有界正の測度 μ に対して、 ∫ U dμ ∈ F であることを示します。 従って、上記のように、定義する、M^1(T) の線形写像 λ ↦ ∫ U dλ = U(λ) を F に変換し、拡大する C'(T) の類似の写像を F に変換することができます。 さらに、H の 0 の閉じた平衡した凸近傍 V ごとに、G の 0 の近傍 W が仮定までに存在し、すべての x ∈ W およびすべての t ∈ T について U(t) · x ∈ V を持ち、結果として (V が弱く閉じているため) ∫ (U(t) · x)dλ(t) ∈ ||λ|| · V (No. 2、提案 5)。 その他語:

#### 命題 17 {#int-vi-s1-prop-17 .statement tag=0998}

— G、H を 2 つのハウスドルフ局所凸空間とし、H を準完全であると仮定します。 U を T の L(G; H) (t, x) ↦ U(t) · x が T × G 上で連続であり、U(T) が等連続であるような式。 次に、M^1(T) に Banach 空間位相が装備されている場合、M^1(T) × G の H への双線形写像 (λ, x) ↦ U(λ) · x は連続です (これは特に、M^1(T) の線形写像 λ ↦ U(λ) が L(G; H) は L(G; H) には、有界収束の位相が装備されています。

#### 命題 18 {#int-vi-s1-prop-18 .statement tag=0999}

— G_1、G_2、H_1、H_2 を 4 つの局所凸ハウスドルフ空間とし、H_1 と H_2 を準完全であると仮定します。 A : G_1 → G_2 と B : H_1 → H_2 が 2 つ連続する線形写像とする。 U_1 : T → L(G_1; H_1)、U_2 : T → L(G_2; H_2) を提案 16 (それぞれ提案 17) の 2 つの写像満たす条件とし、すべての t ∈ T に対して B ◦ U_1(t) と仮定します。 = U_2(t) ¡

実際、すべての x ∈ G_1 について、(No. 1、提案 1) が得られます。

$$
(B \circ U_1(\lambda)) \cdot x = \int \left( (B \circ U_1(t)) \cdot x \right) d\lambda(t)
$$
$$
= \int \left( (U_2(t) \circ A) \cdot x \right) d\lambda(t) = U_2(\lambda) \cdot (A \cdot x).
$$

#### 注意 1 {#int-vi-s1-n7-rem-1 .statement tag=099A}

G と H が Banach 空間であり、U が T の写像である L(G; H) であるとします。 (t, x) ↦ U(t) · x は T × G 上で連続です。 これは、有限写像 t ↦ \|U(t)\| が意味することに注意してください。は、T のすべてのコンパクト部分集合と T 上の下部半連続で境界があり、$x$ が G のボール $|x| \leq 1$ の上を走るとき、連続写像 $t \mapsto |U(t) \cdot x|$ の上部エンベロープになります。 集合 $h(t) = \| U(t) \|$。次に、$h$ が $\mu$ 可積分となるような T 上のすべての正の測度 $\mu$ に対して、再び $\int U d\mu \in \mathscr{L}(G; H)$ が得られます。なぜなら、メジャー $\nu = h \cdot \mu$ は仮定によって制限されるからです。したがって、$\nu$-無視できる集合 N とコンパクトな部分集合の数列 $(K_n)$ によって形成される T の分割が存在します。この番号の冒頭で行われた議論は、$\varphi_{K_n} \cdot \mu$ の措置に適用され、次のことを示しています。

$$
A_n = \int \varphi_{K_n} U \, d\mu \in F = \mathscr{L}(G; H),
$$

そしてさらに (No. 2、提案 6)、$\| A_n \| \leq \int \varphi_{K_n} \| U \| \, d\mu \leq \nu(K_n)$。したがって、系列と一般的な項 $A_n$ はバナッハ空間 $\mathscr{L}(G; H)$ に絶対収束し、その和が $\int U \, d\mu$ であり、その $\| \int U \, d\mu \| \leq \int \| U \| \, d\mu$ であるのは明らかです。

#### 注意 2 {#int-vi-s1-n7-rem-2 .statement tag=099B}

$G = H$ が準完全で、$U$ が提案 16 の仮説を満たすと仮定します。M を、弱い位相 $\sigma(\mathscr{C}'(T), \mathscr{C}(T))$ に対して、空間 $\mathscr{C}'(T)$ の密な部分集合とし、X を閉線形とします。 $\lambda \in M$ ごとに $U(\lambda)(X) \subset X$ となるような H の部分空間。次に、すべての $t \in T$ についても $U(t)(X) \subset X$ です。実際、X に直交するすべての $x \in X$ とすべての $x' \in H'$ について、すべての $\lambda \in M$ について仮定 $\langle U(\lambda) \cdot x, x' \rangle = 0$ により、$\int \langle U(t) \cdot x, x' \rangle \, d\mu(t) = 0$ と書くことができます。したがって、M に直交する連続写像 $t \mapsto \langle U(t) \cdot x, x' \rangle$ は 0 となり、すべての $x' \in X^\circ$ に対して $\langle U(t) \cdot x, x' \rangle = 0$、すべての $t \in T$ と $x \in X$ に対してよって $U(t) \cdot x \in X$ が得られ、これは私たちの主張を証明します。

### 練習問題 {#int-vi-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
