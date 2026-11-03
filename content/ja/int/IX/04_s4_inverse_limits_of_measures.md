---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 4
section_title: Inverse limits of measures
lang: ja
source: int-vii-ix
book_pages: INT IX.49-INT IX.55, INT IX.112-INT IX.113
pdf_pages: 0231-0237, 0294-0295
extraction: ocr
subsections:
    - "no": 1
      title: Complements on compact spaces and inverse limits
      page: 50
      pdf_page: 232
    - "no": 2
      title: Inverse systems of measures
      page: 50
      pdf_page: 232
    - "no": 3
      title: The case of countable inverse systems
      page: 54
      pdf_page: 236
statements: 7
exercises: 2
content_sha256: 86734d6adff7fc69b7c8434141b9c3ef1beb1aa88a294039325e48501776504a
translated_from: content/en/int/IX/04_s4_inverse_limits_of_measures.md
translation_method: google
source_content_sha256: 5dd841f191bacbaf28441eec0f88259078f641775a797c2d66f85a7d4bd2a6c4
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: a616de626a11b0f336afb13fb70a25b7c3c31ba4d54d62baac45dd61c065a413
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 4。メジャーの逆極限

*この切断を通して、I は空でない集合を表し、$i \leq j$ で示される予約注文関係が装備されており、この関係に向けられています。 (GT、I, §4, No. 4) を思い出してください。I によってインデックス付けされたトポロジカル空間の逆系はファミリー $(T_i, p_{ij})$ です。ここで、$T_i$ はトポロジカル空間で、$p_{ij}$ は $T_j$ の連続写像です。 $i \leq j$の場合は$T_i$、$p_{ii}$は$T_i$の恒等写像、$i \leq j \leq k$の場合は$p_{ik} = p_{ij} \circ p_{jk}$です。 T を位相ベクトル空間および $(p_i)_{i \in I}$ を連続写像 $p_i : T \to T_i$ の族とする。 $i \leq j$ に対して $p_i = p_{ij} \circ p_j$ がある場合、家族 $(p_i)_{i \in I}$ は一貫していると言われ、T に個別の $x, y$ に対して $p_i(x) \neq p_i(y)$ のような $i \in I$ が存在する場合、分離していると言われます。 $T = \varprojlim T_i$ と $p_i$ が T の $T_i$ への標準写像であるとき、家族 $(p_i)_{i \in I}$ は一貫しており、分離しています。*

(3) スーリン空間では、すべてのボレル集合はスーリン集合です (GT、IX, §6, No. 3、提案 11)。
(4) より一般的には、$f : X \to Y$ がスースリン空間間の連続全単射である場合、$\mu \mapsto f(\mu)$ は、X 上の有界測度の集合から Y 上の有界測度の集合への全単射写像です (§ 2, No. 4、提案 9)。

### 1. コンパクト空間と逆数極限の補数

#### 命題 1 {#int-ix-s4-prop-1 .statement tag=09QM}

— X と Y を 2 つのトポロジー 空間とし、f を X の Y への連続写像とします。 $(K_\alpha)_{\alpha \in A}$ を、共通部分 K を持つ X のコンパクト部分集合の減少する有向族とする。 次に$f(K) = \bigcap_{\alpha \in A} f(K_\alpha)$。

というのは、y を $\bigcap_{\alpha \in A} f(K_\alpha)$ の点とします。 $\alpha \in A$、集合、$L_\alpha = K_\alpha \cap f^{-1}(y)$はコンパクト、空でないごとに。ファミリ $(L_\alpha)_{\alpha \in A}$ は下向きなので、その共通部分 L は空でないです。さて、$L = K \cap f^{-1}(y)$、よって $y \in f(K)$。したがって、包含 $f(K) \supset \bigcap_{\alpha \in A} f(K_\alpha)$ が証明されましたが、その逆の包含は明らかです。

#### 命題 2 {#int-ix-s4-prop-2 .statement tag=09QN}

— I によってインデックス付けされたトポロジカル空間の逆系 $(T_i, p_{ij})$、トポロジカル空間 T、および連続写像 $p_i : T \to T_i$ の一貫した分離族が与えられるとします。それから：

a) T のすべてのコンパクト部分集合 K に対して、1 つは $K = \bigcap_{i \in I} p_i^{-1}(p_i(K))$ を持ちます。

b) K と L を T の 2 つの互いに素コンパクト部分集合とする。 $p_j(K)$ と $p_j(L)$ が $j \geq i$ に対して互いに素となるような $i \in I$ が存在する。

a) x を $\bigcap_{i \in I} p_i^{-1}(p_i(K))$ の点とします。 K の点 y のすべての $i \in I$、集合 $K_i$ について、$p_i(y) = p_i(x)$ は K の空でないが閉じた部分集合になります。 $i \leq j$ には $K_i \supset K_j$ があり、K がコンパクトなので、集合したがって、$\bigcap_{i \in I} K_i$ は空でないになります。あなたを$\bigcap_{i \in I} K_i$中点としましょう。 $i \in I$、よって $y = x$ には、$y \in K$ と $p_i(y) = p_i(x)$ があります。最後に、$x \in K$、これは $K \supset \bigcap_{i \in I} p_i^{-1}(p_i(K))$ が含まれていることを証明します。逆の包含は明らかです。

b) $i \in I$、集合 $M_i = p_i^{-1}(p_i(K)) \cap L$ ごとに;これはコンパクト空間 L の閉じた部分集合で、$i \leq j$ に対して $M_i \supset M_j$ があり、a) により、

$$
\bigcap_{i \in I} M_i = K \cap L = \varnothing.
$$

従って、$M_i = \varnothing$ となるような添字 i が存在します。 $j \geq i$ の場合、$p_j^{-1}(p_j(K)) \cap L = M_j \subset M_i = \varnothing$、よって $p_j(K) \cap p_j(L) = \varnothing$ があります。

### 2. メジャーの逆系

#### 定義 1 {#int-ix-s4-def-1 .statement tag=09QO}

— $\mathscr{T} = (T_i, p_{ij})$ を、I でインデックス付けされたトポロジカル空間の逆数系とします。 $\mathscr{T}$ ファミリー $(\mu_i)_{i \in I}$ 上の測度の逆関数系 (または部分逆元系) を呼びます。ここで、$\mu_i$ は、すべての $i \in I$ に対する $T_i$ 上の有界測度であり、$\mu_i = p_{ij}(\mu_j)$ (それぞれ $\mu_i \geq p_{ij}(\mu_j)$) は、 $i \leq j$。

#### 命題 3 {#int-ix-s4-prop-3 .statement tag=09QP}

*$I$ によってインデックス付けされたトポロジカル空間 $\mathscr{T} = (T_i, p_{ij})$ の逆系、トポロジカル空間 $T$、連続写像 $p_i : T \to T_i$ ($i \in I$ の場合) の一貫した分離族、および$\mathscr{T}$ の小節のサブインバース系 $(\mu_i)_{i \in I}$。 $T$、集合* の各コンパクト部分集合 K

$$
J(K) = \inf_{i \in I} \mu_i^\bullet(p_i(K)).
$$

*その後、$T$ には有界メジャー $\pi$ が存在し、$T$ の各コンパクト部分集合 $K$ に対して $\pi^\bullet(K) = J(K)$ というような 1 つだけが存在します。すべての $i \in I$ に対して $\mu_i \geq p_i(\pi)$ があり、$\pi$ は $T$ 満たすこの条件の最大のです。*

まず、集合 $I$ の切断フィルタ $\mathfrak{F}$ に関して、$J(K)$ が $\mu_i^\bullet((p_i(K)))$ の極限であることを証明しましょう。このためには、(GT, IV, §5, No. 2, Th. 2) で次のことを示すだけで十分です。 $i \leq j$の場合は$\mu_i^\bullet(p_i(K)) \geq \mu_j^\bullet(p_j(K))$。今、設定 $\mu_{ij}' = p_{ij}(\mu_j)$、$\mu_{ij}' \leq \mu_i$ と $p_j(K) \subset \overline{p_{ij}}^{-1}(p_i(K))$、よってがあります

$$
\mu_j^\bullet(p_j(K)) \leq \mu_j^\bullet(\overline{p_{ij}}^{-1}(p_i(K))) = (\mu_{ij}')^\bullet(p_i(K)) \leq \mu_i^\bullet(p_i(K)).
$$

それでは、写像 $J$ の性質の研究に移りましょう。
1) $K \subset L$ のとき、$J(K) \leq J(L)$ であることは明らかです。
2) $K$ と $L$ を、$T$ の 2 つのコンパクトな部分集合とします。 $i \in I$ ごとに、$p_i(K \cup L) = p_i(K) \cup p_i(L)$、よってがあります。

$$
\mu_i^\bullet(p_i(K \cup L)) \leq \mu_i^\bullet(p_i(K)) + \mu_i^\bullet(p_i(L));
$$

フィルタ$\mathfrak{F}$に関して移行から極限を計算すると、$J(K \cup L) \leq J(K) + J(L)$が得られます。
3) コンパクト集合 $K$ と $L$ が互いに素であるとします。 No. 1 の提案 2 により、$j \geq i$ に対して $p_j(K) \cap p_j(L) = \varnothing$ となるような $i \in I$ が存在します。従って、$j \geq i$ については、

$$
\mu_j^\bullet(p_j(K \cup L)) = \mu_j^\bullet(p_j(K)) + \mu_j^\bullet(p_j(L)),
$$

フィルター $\mathfrak{F}$ に対して移行から極限によって $J(K \cup L) = J(K) + J(L)$。
4) $(K_\alpha)_{\alpha \in A}$ を、共通部分 $K$ を持つ$T$ のコンパクト部分集合の有向族減少するとします。 No. 1、$p_i(K) = \bigcap_{\alpha \in A} p_i(K_\alpha)$ の提案 1、したがってすべての $i \in I$ に対して $\mu_i^\bullet(p_i(K)) = \inf_{\alpha \in A} \mu_i^\bullet(p_i(K_\alpha))$ による (§ 1, No. 6、提案 5 の修正)。これから推測すると、
$$
J(K) = \inf_{i \in I} \mu_i^\bullet(p_i(K)) = \inf_{i \in I} \inf_{\alpha \in A} \mu_i^\bullet(p_i(K_\alpha))
= \inf_{\alpha \in A} \inf_{i \in I} \mu_i^\bullet(p_i(K_\alpha)) = \inf_{\alpha \in A} J(K_\alpha).
$$
5) 選ぶと $i \in I$ と集合 $c = \mu_i^\bullet(T_i)$ としましょう。この場合、$c$ は有限であり、$J(K) \leq \mu_i^\bullet(p_i(K)) \leq \mu_i^\bullet(T_i)$ なので、$T$ の各コンパクト集合 $K$ に対して $J(K) \leq c$ となります。

上記のプロパティにより、適用 Th が許可されます。 § 3, No. 1 の 1 つ。 結論する、$T$ のすべてのコンパクト部分集合 $K$ に対して $\pi^\bullet(K) = J(K)$ となるような、$T$ には 1 つだけの有界メジャー $\pi$ が存在します。 すべての $i \in I$ について、$p_i$ の下の $\pi$ の像である $T_i$ の小節を $\nu_i$ で表します。 $i \in I$、$A$ を $T_i$ のコンパクト部分集合、および $\overline{p_i^{-1}(A)}$ のコンパクト部分集合の $\mathscr{L}$ 集合とします。 § 1, No. 2 の注意 3 までに、$\pi^\bullet(\overline{p_i^{-1}(A)}) = \sup_{K \in \mathscr{L}} \pi^\bullet(K)$ になります。さらに、$K \in \mathscr{L}$、よって、$\nu_i^\bullet(A) = \sup_{K \in \mathscr{L}} J(K)$には$\nu_i^\bullet(A) = \pi^\bullet(\overline{p_i^{-1}(A)})$、$J(K) = \pi^\bullet(K)$が入ります。

$K \in \mathscr{L}$ には、$p_i(K) \subset A$、よって $J(K) \leq \mu_i^\bullet(p_i(K)) \leq \mu_i^\bullet(A)$、そして最後に $\nu_i^\bullet(A) \leq \mu_i^\bullet(A)$ があります。 $A$ は $T_i$ の任意のコンパクト集合なので、$\nu_i \leq \mu_i$ を結論するとします。 命題の最後の主張は明らかです。

Q.E.D.

#### 定理 1 (プロホロフ) {#int-ix-s4-thm-1 .statement tag=09QQ}

— *$\mathscr{T} = (T_i, p_{ij})$ を、$I$ によってインデックス付けされたトポロジカル空間の逆系、$T$ トポロジカル空間、および $(p_i)_{i \in I}$ を連続する写像 $p_i : T \to T_i$ の一貫した分離族とします。最後に、$(\mu_i)_{i \in I}$を$\mathscr{T}$のメジャーの逆数系とします。

すべての $i \in I$ に対して $p_i(\mu) = \mu_i$ となるような、$T$ に制限された尺度 $\mu$ が存在するには、次の条件が満たされることが必要かつ十分です。

(P) *すべての $\varepsilon > 0$ に対して、すべての $i \in I$ に対して $\mu_i^\bullet(T_i - p_i(K)) \leq \varepsilon$ となるような $T$ のコンパクトな部分集合 $K$ が存在します。

この場合、メジャー $\mu$ は一意に決定され、*
$$
\mu^\bullet(K) = \inf_i \mu_i^\bullet(p_i(K))
$$
*$T$* の各コンパクト集合 $K$ に対して。

まずは$\mu$の一意性を証明しましょう。 $\mu$ を、すべての $i \in I$ に対して $p_i(\mu) = \mu_i$ となるような、$T$ の制限された尺度とします。 $K$ を $T$ の圧縮部分集合とします。 No. 1の提案2によると、集合 $K$は、減少するの共通部分、*クローズド*の$(\overline{p_i^{-1}(p_i(K))})_{i \in I}$、$T$の部分集合です。コルによって。 § 1, No. 6 の提案 5 の、したがって、次のようになります。
$$
\mu^\bullet(K) = \inf_{i \in I} \mu^\bullet(\overline{p_i^{-1}(p_i(K))}) = \inf_{i \in I} \mu_i^\bullet(p_i(K)),
$$

これにより、公式 (2) が成立します。コンパクト集合の集合上の一致するが等しい 2 つのメジャー (§ 1, No. 2、提案 2 の補正) であるため、$\mu$ は一意であることになります。

提案 3 により、$T$ のすべてのコンパクト部分集合 $K$ に対して $\pi^\bullet(K) = \inf_{i \in I} \mu_i^\bullet(p_i(K))$ となるような、$T$ に制限された尺度 $\pi$ が存在します。 公式 (2) により、すべての $i \in I$ に対する $p_i(\mu) = \mu_i$ が関係と等価となるような、$T$ 上の有界メジャー $\mu$ が存在します。

(P') $i \in I$全員に対して$p_i(\pi) = \mu_i$。

$i \leq j$ の場合、$\mu_i = p_{ij}(\mu_j)$、よって $\mu_i^\bullet(T_i) = \mu_j^\bullet(T_j)$ があります。 $I$ が指示されているため、すべての $i \in I$ に対して $\mu_i^\bullet(T_i) = c$ となるような有限の数 $c \geq 0$ が存在します。提案 3 によれば、測度 $\mu_i - p_i(\pi)$ は正であるため、その総質量が零である場合、つまり $\mu_i(T_i) = p_i(\pi)^\bullet(T_i)$ の場合に限り、零となります。 $p_i(\pi)^\bullet(T_i) = \pi^\bullet(T)$ なので、条件 (P') は $\pi^\bullet(T) = c$、つまり (§ 1, No. 2, 注意 3) から性質と等価です。

(P'') $\sup_{K \in \mathscr{K}} \pi^\bullet(K) = c$、ここで $\mathscr{K}$ は $T$ のコンパクト部分集合の集合です。

さて、$K \in \mathscr{K}$ については、

$$
\pi^\bullet(K) = \inf_{i \in I} \mu_i^\bullet(p_i(K)) = c - \sup_{i \in I} \mu_i^\bullet(T_i - p_i(K))
$$

そしてこの公式は、(P) と (P'') の同値を直ちに暗示します。

Q.E.D.

$(T_i, p_{ij})$ をトポロジー 空間の逆数系とします。 集合 $T = \lim_{\leftarrow} T_i$ を$T$ の $p_i$ 標準写像で$T_i$ に表します。一般化した定義第2章III, § 4, No. 5、$T$ 上の有界メジャー $\mu$ は、すべての $i \in I$ に対して $\mu_i = p_i(\mu)$ である場合、*メジャーの逆数系* $(\mu_i)_{i \in I}$ の *逆数極限であると言えます。 Th. 1 は、メジャーの逆数極限が存在するかどうかの基準を提供します。 空間 $T_i$ が *コンパクト* で、 写像 $p_{ij}$ 全射である場合、 $T$ はコンパクトで、 $i \in I$ ごとに $p_i(T) = T_i$ になります。したがって、条件 (P) は満たされ、この場合、第 99 章の提案 8、(iv) が回収されます。 III, § 4, No. 5。

#### 注意 {#int-ix-s4-n2-rem-1 .statement tag=09QR}

— $(\mu_i)_{i \in I}$ を、空間 $\mathscr{T} = (T_i, p_{ij})$ の逆数系のメジャーの逆数系とします。トポロジー 空間 $T'$ と連続写像 $p'_i : T' \to T_i$ が与えられたと仮定します。家族 $(p'_i)_{i \in I}$ は一貫しているが、必ずしも分離しているわけではないと仮定します。 *プロホロフの条件 (P) が家族* $(p'_i)_{i \in I}$ によって満足される場合、 *尺度が存在します* $\mu'$ (*必ずしも一意ではない*) *上* $T'$ *そのような* $p'_i(\mu') = \mu_i$ *すべてに対して* $i \in I$。

集合 $T = \lim_{\leftarrow} T_i$ と $p' = (p'_i)_{i \in I}$ の場合、$T$ の $p_i$ 標準写像を$T_i$ に表します。プロホロフの条件は、$T$ と $p_i$ によって満たされます。なぜなら、$p_i(p'(K')) = p'_i(K')$ と $p'(K')$ は、$T'$ のすべてのコンパクト部分集合 $K'$ に対して $T$ でコンパクトだからです。 Thさんより1、すべての $i \in I$ に対して $p_i(\mu) = \mu_i$ となるような、$T$ に制限された尺度 $\mu$ が存在します。 $K'$ を $T'$ のコンパクト集合とします。それから$\mu^\bullet(p'(K')) = \inf_{i \in I} \mu_i^\bullet(p'_i(K'))$、よって
$$
\mu^\bullet(T - p'(K')) = \sup_{i \in I} \mu_i^\bullet(T_i - p_i'(K')).
$$
$\varepsilon > 0$ にしましょう。プロホロフの条件 (P) は $p_i'$ によって満たされるため、$\mu^\bullet(T - p'(K')) \leq \varepsilon$ となるような $T'$ のコンパクトな部分集合 $K'$ を見つけることができます。次に、§2, No. 4 の提案 8 は、すべての $i \in I$ に対して $\mu = p'(\mu')$、よって $\mu_i = p_i(\mu) = p_i(p'(\mu')) = p_i'(\mu')$ を使用して、$T'$ に制限された尺度 $\mu'$ の存在を確立します。

### 3. 可算逆数系の場合

#### 定理 2 {#int-ix-s4-thm-2 .statement tag=09QS}

— *有向事前注文集合 I に可算余終点部分集合があると仮定します。 $\mathscr{T} = (T_i, p_{ij})$ をトポロジー 空間、$T = \lim_{\leftarrow} T_i$、$p_i$ 標準写像の $T$ から $T_i$ への逆数系とします。次に、$\mathscr{T}$ の小節のすべての逆系 $(\mu_i)_{i \in I}$ は、逆極限を認めます。*

まず、$I = \mathbf{N}$ と集合 $q_n = p_{n,n+1}$ の場合を扱います。 $\varepsilon > 0$ にしましょう。 定義するは、次のように、コンパクト集合 $L_n \subset T_n$ の再帰的数列です。 $L_0$ は、$\mu_0^\bullet(T_0 - L_0) \leq \varepsilon/2$ となるような $T_0$ のコンパクト部分集合であり、$n \geq 0$ については、コンパクト集合 $L_{n+1}$ が含まれます。 $\overline{q_n^{-1}(L_n)}$ と満足
$$
\mu_{n+1}^\bullet(\overline{q_n^{-1}(L_n)} - L_{n+1}) \leq \varepsilon/2^{n+2}.
$$
この構成は、§1, No. 2 の *注意 3* によって可能です。私たちは持っています
$$
\begin{align*}
\mu_{n+1}^\bullet(T_{n+1} - L_{n+1}) &= \mu_{n+1}^\bullet(T_{n+1} - \overline{q_n^{-1}(L_n)}) + \mu_{n+1}^\bullet(\overline{q_n^{-1}(L_n)} - L_{n+1}) \\
&\leq \mu_{n+1}^\bullet(T_{n+1} - \overline{q_n^{-1}(L_n)}) + \varepsilon/2^{n+2} \\
&= \mu_n^\bullet(T_n - L_n) + \varepsilon/2^{n+2}
\end{align*}
$$
$\mu_n = q_n(\mu_{n+1})$だから。 $p$の帰納法までに、次のように推測されます。
$$
\mu_p^\bullet(T_p - L_p) \leq \varepsilon(1 - 1/2^{p+1}) \leq \varepsilon.
$$
$T$は$\prod_{n \in \mathbf{N}} T_n$の閉じた部分空間と積空間$\prod_{n \in \mathbf{N}} L_n$がコンパクトなので、$T$の部分集合$L = T \cap \prod_{n \in \mathbf{N}} L_n = \bigcap_{n \in \mathbf{N}} \overline{p_n^{-1}(L_n)}$はコンパクトです。 $n \in \mathbf{N}$ にしましょう。 $p_n(L) = \bigcap_{m \geq n} p_{nm}(L_m)$ (GT、I, §9, No. 6、Prop. 8) と $m' \geq m \geq n$、よっての $p_{nm}(L_m) \supset p_{nm'}(L_{m'})$ があります。
$$
\mu_n^\bullet(T_n - p_n(L)) = \lim_{m \to \infty} \mu_n^\bullet(T_n - p_{nm}(L_m)).
$$

ただし、$m \geq n$ の場合、メジャー $\mu_n$ は、$p_{nm}$、よっての下の $\mu_m$ の像です。

$$
\mu_n^\bullet(T_n - p_{nm}(L_m)) = \mu_m^\bullet(T_m - \overline{p}_{nm}(p_{nm}(L_m))) \leq \mu_m^\bullet(T_m - L_m) \leq \varepsilon;
$$

$m$に対して移行から極限を行うと、$\mu_n^\bullet(T_n - p_n(L)) \leq \varepsilon$が得られます。他の語では、プロホロフの条件 (P) が満たされ、すべての $n \in \mathbf{N}$ に対して $\mu_n = p_n(\mu)$ となるような、$T$ に制限された尺度 $\mu$ が存在します (No. 2, Th. 1)。

一般的なケースに移りましょう。$I$ 増加する cofinal 数列 $(i_n)_{n \in \mathbf{N}}$ が存在します。 写像 $t \mapsto (p_{i_n}(t))_{n \in \mathbf{N}}$ は、系 $(T_{i_n}, p_{i_n i_m})$ (GT, I, §4, No. 4) の逆行列極限への $T$ の準同型写像です。したがって、証明の最初の部分までに、すべての $n \in \mathbf{N}$ に対して $\mu_{i_n} = p_{i_n}(\mu)$ となるような、$T$ 上の制限された尺度 $\mu$ が存在します。 $i \in I$ にしましょう。 $n \in \mathbf{N}$ には $i \leq i_n$、よってが存在します

$$
p_i(\mu) = p_{i i_n}(p_{i_n}(\mu)) = p_{i i_n}(\mu_{i_n}) = \mu_i.
$$

Q.E.D.

定理 2 は次の状況でよく使用されます: $D$ を可算集合とし、$(X_t)_{t \in D}$ をトポロジー 空間の族とする。 $\mathfrak{F}$ を包含順に並べた $D$ の有限部分集合の集合とします。 $\mathfrak{F}$、集合 $X_J = \prod_{t \in J} X_t$の$J$、および$J \subset J'$の場合、$p_{JJ'}$を部分積$X_J$に対する$X_{J'}$の標準射影とします。また、集合 $X = \prod_{t \in D} X_t$ は、$X$ の標準的な射影を部分的な積 $X_J$ に$p_J$ で表します。簡単に (cf. S, III, §7, No. 2, 注意 3) 族 $(p_J)_{J \in \mathfrak{F}}$ 定義するが $X$ の $\lim_{\leftarrow} X_J$ への同型写像であることを示します。メジャーの逆系は、$J \subset J'$ に対して $\mu_J = p_{JJ'}(\mu_{J'})$ となるような、$X_J$ 上の有界メジャー $\mu_J$ のファミリーになります。 $D$ の有限部分集合 $J$ ごとに $\mu_J = p_J(\mu)$ となるような、$X$ には $\mu$ という制限されたメジャーが 1 つだけ存在します (*コルモゴロフの定理*)。 1 つのときどきは、$\mu$ は $\prod_{t \in D} X_t$ のメジャーで *マージン* $\mu_J$ があると述べています。

特に、$t \in D$ ごとに、総質量 1 の $X_t$ のメジャー $\nu_t$ が与えられたとします。 $D$ の有限部分集合 $J$ ごとに集合 $\mu_J = \bigotimes_{t \in J} \nu_t$ が与えられるとします。 $J \subset J'$を$D$の2つの有限部分集合とし、$K = J' - J$とします。 $X_{J'}$ を $X_J \times X_K$ と同一視すると、$\mu_{J'} = \mu_J \otimes \mu_K$ があり、$\mu_K$ の尺度の総質量は 1 であるため、$X_J$ 上の$\mu_J \otimes \mu_K$ の射影は$\mu_J$ に等しくなります。マージン $\mu_J$ を認める $X$ のメジャーは $\bigotimes_{t \in D} \nu_t$ で示され、ファミリー* $(\nu_t)_{t \in D}$ の *積と呼ばれます。 空間 $X_t$ がコンパクトになると、Ch の構成が回復します。 III, §4, No. 6。

### 練習問題 {#int-ix-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
