---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 17
section_title: Regular extensions
lang: ja
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.180-A V.181
pdf_pages: 0251-0259, 0294-0295
extraction: ocr
subsections:
    - "no": 1
      title: Complements on the relative separable algebraic closure
      page: 137
      pdf_page: 251
    - "no": 2
      title: The tensor product of extensions
      page: 139
      pdf_page: 253
    - "no": 3
      title: Regular algebras
      page: 140
      pdf_page: 254
    - "no": 4
      title: Regular extensions
      page: 141
      pdf_page: 255
    - "no": 5
      title: Characterization of regular extensions
      page: 142
      pdf_page: 256
    - "no": 6
      title: Application to composite extensions
      page: 143
      pdf_page: 257
statements: 20
exercises: 5
content_sha256: ff07a856392ef34b2b07e97b5c668ce949c1e949cc2ebcea5101407887412ef1
translated_from: content/en/alg/V/17_s17_regular_extensions.md
translation_method: google
source_content_sha256: c3f351f5e813a393d1fb207cf121c6dd2bc4e8303d881b9cf4b097b0c621cb53
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: c7831e02af8036b24b388c5bc19ddfd3a5803e970337d559607d95a690052e13
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 17。レギュラー 拡大

### 1. 相対可分性代数閉包の補数

#### 定理 1 (ザリスキー) {#alg-v-s17-thm-1 .statement tag=06VP}

— *K を K の体、L 拡大、$K_1$ L (V、p. 44) の K の相対分離可能代数閉包、$K_2$ K の相対代数閉包とするL (V、p. 19) および $(X_i)_{i \in I}$ は不確定要素のファミリーです。この場合、$K_1(X_i)_{i \in I}$ は、$L(X_i)_{i \in I}$ の $K(X_i)_{i \in I}$ の相対可分代数閉包であり、$K_2(X_i)_{i \in I}$ は、$L(X_i)_{i \in I}$ の $K(X_i)_{i \in I}$ の相対可分代数閉包です。

A) E が体で、E の F 拡大体であり、F のすべての元が E 属するから E までの可分代数であると仮定します。 $u$ を $F(X)$ の元とします。これは、$E(X)$ に関して可分な代数的です。 $u$ 属するから $E(X)$ までを示します。 $F(X)$ には、$u = P/Q$ となる 2 つの互いに素な多項式 P と Q が存在し、Q をモニックとみなすことができます。 S を、P と Q の係数の F からなるの*有限* 部分集合、$F_0 = E(S)$ とし、A を $F_0$ から $F_0$ への E 微分とします。 $D$ を$F_0(X)$ の導分とし、$F_0$ および写像 $X$ から $0$ の$A$ と一致します (V、p. 128、提案 3)。

$u \in F_0(X)$ は $E(X)$ 上で可分代数であり、$D$ は $E(X)$ 上の零であるため、$D(u) = 0$ (V, p.129、提案 4)、よって $D(P) . Q = P . D(Q)$ が得られます。 $P$ と $Q$ は互いに素なので、 $Q$ 割る $D(Q)$ (IV, p. 13, Cor. 4) を結論するとします。現在、$Q$ は形で書かれる可能性があります
$$
Q(X) = X^n + a_1 X^{n-1} + \ldots + a_{n-1} X + a_n
$$
$F_0$ に $a_1, \ldots, a_n$ が入っています。 $D(x) = 0$ 以来、私たちはこうして
$$
D(Q) = \Delta(a_1) X^{n-1} + \cdots + \Delta(a_{n-1}) X + \Delta(a_n)
$$
よって $\deg D(Q) < \deg Q$。 $Q$ 割る $D(Q)$ なので、これは $D(Q) = 0$ の場合にのみ可能です。でも、$D(P) . Q = P . D(Q)$だから$D(P) = 0$。ここで (1) と、$P$ に対する同様の公式は、$A$ が $P$ の係数と $Q$、よって $A = 0$ の集合 $S$ を全滅させることを示しています。 $F_0 = E(S)$。 V、p. 135、Cor. 2、したがって、$E$ の有限生成された拡大 $F_0$ は分離可能な代数です。 $E$ と $F$ の仮説により、$F_0 = E$ が得られ、最終的には $u \in E(X)$ になります。

B) ここで、$E$ が拡大体 $F$ で比較的代数的に閉じており、$E$ の特性指数を $p$ で表すとします。 $u$ を $E(X)$ の代数である $F(X)$ の元とします。 $v = u^{p^f}$ が $E(X)$ 上で可分代数となるような整数 $f \geq 0$ が存在します (V, p. 44、提案 13)。 A) したがって、$v \in E(X)$ となります。 $F[X]$ と $Q$ モニックには相対的に素な多項式 $P$ と $Q$ を持つ形 $P/Q$ に$u$ の一意の表現が存在します。 $E[X]$ と $Q_1$ モニックでは、$P_1$ と $Q_1$ が互いに素であり、同様の分解 $v = P_1/Q_1$ があります。したがって、$P_1/Q_1 = P^{p^f}/Q^{p^f}$;多項式 $P^{p^f}$ と $Q^{p^f}$ は、$P_1$ や $Q_1$ のように、$F[X]$ (IV, p. 13、Cor. 6) において相対的に素であり、$Q^{p^f}$ はモニックです。 $P^{p^f} = P_1 \in E[X]$と$Q^{p^f} = Q_1 \in E[X]$が続きます。したがって、$P$ と $Q$ の係数は、$E$ に対して $p$ 基であり、したがって、$E$ は$F$ で比較的代数的に閉じているため、属するから $E$ になります。したがって、$P \in E[X]$、$Q \in E[X]$、そして最後に $u \in E(X)$ になります。これは、$E(X)$ が $F(X)$ で比較的代数的に閉じていることを証明します。

C) 定理 1 の記法を使用します。 $K_1$ は、$K$ の分離可能な代数拡大であるため、$K(X_i)_{i \in I}$ の拡大 $K_1(X_i)_{i \in I}$ は代数的で分離可能です (V、p. 39、提案 6)。 さらに、$L$ のすべての元は代数的であり、$K$、属するから$K$ まで分離可能です (V、p. 44、提案 13、a))。 $J$ を $I$ の有限部分集合とします。 $J$ の基数上の明らか帰納法により、A) から $L(X_i)_{i \in I}$ のすべての元が代数的であり、$K(X_i)_{i \in I}$、属するから $K_1(X_i)_{i \in J}$ まで分離可能であると推定されます。 最後に、$u$ を $L(X_i)_{i \in I}$ の元とし、代数的で $K(X_i)_{i \in I}$ で分離可能とします。 $u$ 属するから $L(X_i)_{i \in I}$ となるような $I$ の有限部分集合 $J$ が存在し、$K(X_i)_{i \in J}$ に関しては代数的で分離可能です。言われたことによると、$u$ 属するから $K_1(X_i)_{i \in J}$、そしてなおさらから $K_1(X_i)_{i \in I}$ です。

したがって、A) から、$K_1(X_i)_{i \in I}$ は $L(X_i)_{i \in I}$ における $K(X_i)_{i \in I}$ の相対的な分離閉包であると推定されました。同様に、B) から、$K_2(X_i)_{i \in I}$ は $L(X_i)_{i \in I}$ の $K(X_i)_{i \in I}$ の相対代数閉包であることがわかります。

### 2. 拡大中テンソル積

#### 命題 1 {#alg-v-s17-prop-1 .statement tag=06VQ}

— $\Omega$ を体 $K$ の拡大とし、$L, M$ を $\Omega$ の 2 つの部分拡張とし、代数的に $K$ 上の互いに素とします。 $L$ の $K$ の相対可分代数閉包が $K$^1 に等しいとします。 $\varphi$ を、$x \in L, y \in M$ に対する $L \otimes_K M$ から $\Omega$ 写像 $x \otimes y$ への $xy$ への $K$-代数準同型性とし、$p$ を核とする$\varphi$。すると、$p$ は $L \otimes_K M$ の冪零元の集合であり、これは $L \otimes_K M$ の主理想である最小のです。

必要に応じて、置き換えること $\Omega$ by 代数閉包で、$\Omega$ が代数的に閉じていると仮定することができます。 $B$ を、$K$ に対する $M$ の超越基底とし、$N$ を、$\Omega$ および$N_r$ (それぞれ$N_s$) 集合における $K(B)$ の相対代数閉包とします。 $K(B)$ 上で分離可能な (それぞれ p-ラジカル) $N$ の元。 $M$ は $K(B)$ に対して代数的であるため、$N$ は $\Omega$ における $M$ の相対値代数閉包であることに注意してください。

$$
\begin{array}{ccccccccc}
L & \longrightarrow & L(B) & \longrightarrow & L(B \cup N_s) \\
\uparrow & & \uparrow & & \uparrow \\
K & \longrightarrow & K(B) & \longrightarrow & N_s \\
& & \downarrow & & \downarrow \\
& & M & \longrightarrow & N \\
\uparrow & & \downarrow & & \downarrow \\
N_r & \longrightarrow & N & \longrightarrow & \Omega
\end{array}
$$

図1

次の準同型の連鎖を定義する見てみましょう。

$$
L \otimes_K M \xrightarrow{\alpha} L \otimes_K N \xrightarrow{\beta} (L \otimes_K K(B)) \otimes_{K(B)} N \xrightarrow{\gamma} L(B) \otimes_{K(B)} N
$$
$$
\rightarrow L(B) \otimes_{K(B)} N_s \otimes_{K(B)} N_r \xrightarrow{\varepsilon} L(B \cup N_s) \otimes_{K(B)} N_r \xrightarrow{\zeta} \Omega .
$$

$\alpha = \mathrm{Id}_L \otimes u$ があり、$u$ は $M$ の標準単射を $N$ に変換したものであるため、$\alpha$ は単射法です。 写像 $\beta$ は、$x \in L$ に対して写像 $x \otimes y$ から $(x \otimes 1) \otimes y$ (II、p. 278、提案 2) である可換群の同型であり、 $y \in N$。 $\gamma = v \otimes \mathrm{Id}_N$があります。ここで、$v$は、$x \in L$と$y \in K(B)$について、$L \otimes_K K(B)$の$L(B)$への写像$x \otimes y$から$xy$への$K$-代数準同型です。 $L$ と $M$ は代数的に $K$ に対して互いに素であるため、提案 14 (V, p. 114) は、$L$ と $K(B)$ が $K$ に対して線形に互いに素であることを示しています。 other 語、$v$ は単射なので、$y$ は単射です。 $N$ は $K(B)$ の準ガロア拡張であるため、$N$ 写像への $N_s \otimes_{K(B)} N_r$ の $K(B)$-代数同型写像 $w$ が存在します (V, p. 76, 提案 13)。 $x \otimes y$へ

1 この仮定は、$L$が$K$の主要な拡大であるというによって表されるときどきです。

xy は $x \in \mathbf{N}$ と $y \in \mathbf{N}_r$ を表します。 *同型* $\mathrm{Id}_{L(B)} \otimes w \ ^1$ を 6 で表します。 Thさんより1 (V, p. 137) と K の拡大 L 上の仮定、$L(B)$ のすべての元は代数的で、$K(B)$ 属するから $K(B)$ にわたって分離可能です。特に、$L(B) \cap N_s = K(B)$ があります。 $N_r$ は $K(B)$ のガロア拡大なので、Th. 5 (V, p. 71) は、$x \in L(B)$ に対して $L(B U N_r)$ 写像 $x \otimes y$ から $xy$ への $L(B) \otimes_{K(B)} N_s$ の $K(B)$-代数同型写像 $w'$ が存在することを示しています。 $y \in N_r$; *同型* $w' \otimes \mathrm{Id}_{N_r}$ を $\varepsilon$ で表します。最後に、$\zeta$は、$x \in L(B U N_r)$と$y \in N_r$に対して、K-代数準同型写像$x \otimes y$から$xy$となります。

これまで述べられてきたことは、$\eta = \varepsilon \delta \gamma \beta \alpha$ が $L \otimes_K M$ から $L(B U N_r) \otimes_{K(B), N_r}$ への単射K-代数準同型であることを示しています。さらに、M のすべての元は、$a_i \in \mathbf{N}$ の場合は形 $\sum_{i=1}^n a_i b_i$、$1 \leq i \leq n$ の場合は $b_i \in \mathbf{N}_r$ になります。したがって、$\varphi = \zeta \eta$ が得られます。

$\varphi$ の核 $p$ は $L \otimes_K M$ の主要なイデアルであるため、提案 2 (V、p. 118) により、$L \otimes_K M$ 属するから $p$ までのすべての冪零元が決まります。逆に、$a$ を $p$ の元とします。 $1 \leq i \leq s$には$\eta(a) = \sum_{r=1}^s b_i \otimes c_i$と$b_i \in L(B U N_r)$と$c_i \in N_r$を入れます。 $N_r$ は $K(B)$ の p ラジカル拡張であるため、$1 \leq i \leq s$ に対して $c_i^{p^f}$ 属するから $K(B)$ となるような整数 $f \geq 0$ が存在します ($p$ は K の特性指数です)。しかし、私たちは持っています

$$
\eta(a^{p^f}) = \sum_{i=1}^s b_i^{p^f} \otimes c_i^{p^f} = \left( \sum_{i=1}^s b_i^{p^f} c_i^{p^f} \right) \otimes 1 - \zeta \eta(a)^{p^f} \otimes 1 = 0
$$

$\eta$ は単射なので、最終的には $a^{p^f} = 0$ になります。したがって、$p$ は、$L \otimes_K M$ のすべての冪零元のうちの集合であることが示されました。これで、提案 2 (V, p. 118) による $L \otimes_K M$ 含む $p$ のすべての素イデアルが得られます。

#### 系 {#alg-v-s17-n2-cor-1 .statement tag=06VR}

*LとMを体Kの2つの拡大とする。LにおけるKの相対可分代数閉包がKに等しいと仮定する。そのとき、$L \otimes_K M$の冪零元の集合pが素イデアルである。さらに、L または M が K 上で分離可能である場合、$L \otimes_K M$ は整域です。*

L と M は、K (V, p. 116, Th. 5) の拡大 $\Omega$ の代数的互いに素部分拡張であると仮定できます。この場合、提案 1 (V, p. 139) により、p は素イデアルになります。さらに、L または M が K 上で分離可能である場合、$L \otimes_K M$ は、環を分離拡大の定義で減じたものになります (V、p. 119、定義 1)。 p が素数なので、$p = 0$ と $L \otimes_K M$ は整域になります。

### 3. レギュラー 代数

#### 定義 1 {#alg-v-s17-def-1 .statement tag=06VS}

※Kを体とします。 K の拡大 L ごとに $L \otimes_K A$ が整域である場合、K を超える代数は正規であると言われます。*

通常の代数は特に整域であるため、可換です。

#### 命題 2 {#alg-v-s17-prop-2 .statement tag=06VT}

— $A$ と $B$ を体 $K$ 上の 2 つの代数とします。 $A$ が整域で、$B$ が通常の場合、$A \otimes_K B$ は整域です。

$L$ を $A$ の分数の体とします。 $B$ は正則 $K$-代数なので、$L \otimes_K B$ は整域、したがって $L \otimes_K B$ の部分環と同型であるため、$A \otimes_K B$ も同様です。

#### 命題 3 {#alg-v-s17-prop-3 .statement tag=06VU}

— $K$ を体とします。
a) 正則$K$-代数のすべての部分代数それ自体が正則です。
b) 2 つの正則 $K$-代数のテンソル積は再び正則です。
c) $A$ を $K$-代数、$K$ の $K'$ 拡大とする。 $A$ が正則であるためには、スカラーの拡大により $A$ から導出される $K'$-代数 $A_{(K')}$ が正則であることが必要かつ十分です。

a) (それぞれ c)) の証明は、提案 3、V、p. 119、後で置き換えることの部分 a) (それぞれ d)) の環を « 整域だけ削減したものと同一です。 » と « 分離可能な代数 » と « 通常の代数 »。 b)を証明しましょう。

$A$ と $B$ を 2 つの通常の $K$-代数とする。 $L$を$K$の拡大とします。 $A$が正則なので、環 $L \otimes_K A$は整域になります。提案 2 により、$B$ が正則であるため、環 $(L \otimes_K A) \otimes_K B$ は整域になります。最後に、環 $L \otimes_K (A \otimes_K B)$ は $(L \otimes_K A) \otimes_K B$ と同型なので、整域になります。これは、$A \otimes_K B$ が通常の $K$-代数であることを示しています。

### 4. レギュラー 拡大

#### 定義 2 {#alg-v-s17-def-2 .statement tag=06VV}

— 体の拡大が $K$-代数 として正則であれば、 $K$ は正則であると言われます。

#### 命題 4 {#alg-v-s17-prop-4 .statement tag=06VW}

— $A$ を体 $K$ 上の代数として、整域とし、$E$ を分数の体とします。 $L$ を $K$ の拡大とします。 環 $L \otimes_K A$ が整域の場合、$L \otimes_K E$ にも同じことが当てはまります。

$L \otimes_K A$ が整域の場合、分数 $F$ の体に埋め込まれる可能性があります。 $x \in L$ に $u(x) = x \otimes 1$ を書き、$E$ の $F$ への $K$ 準同型写像、つまり $A$ の拡大する単射準同型 $y \mapsto 1 \otimes y$ が $F$ になることを $v$ で表します。提案 6 (V、p. 14) によると、$F$ の部分体 $u(L)$ と $v(E)$ は、$K$ に対して直線的に互いに素です。したがって、$L \otimes_K E$ の $F$ (V, p. 12) への準同型 $u * v$ は単射法です。これは、$L \otimes_K E$ が整域であることを示しています。

#### 系 {#alg-v-s17-n4-cor-1 .statement tag=06VX}

— $A$ が正規の $K$-代数であるためには、その分数の体が $K$ の正規の拡大であることが必要かつ十分です。

条件は、提案 4 によって必要であり、提案 3、a) によって十分です。

#### 命題 5 {#alg-v-s17-prop-5 .statement tag=06VY}

— 体 $K$ のすべての純粋な拡大は規則的です。

前述の系によって、すべての多項式代数 $A = K[X_i]_i$ が正則 $K$-代数であることを証明するのに十分です。 $L$ を $K$ の拡大とします。 環 $L \otimes_K A$ は $L[X_i]_{i \in I}$ (III, p. 449, 注意 2) と同型なので、整域 (IV, p. 9、提案 8)。

#### 命題 6 {#alg-v-s17-prop-6 .statement tag=06VZ}

— L を体 K の拡大とします。L が正規であれば、L のすべての部分拡張は正規です。逆に、L の有限に生成されたすべての部分拡張が正規である場合、L は正規です。

最初の主張は、提案 3、a) から続きます。

M を K の拡大とし、$\mathscr{U}$ を L の有限生成されたすべての部分拡張の集合とします。各 E $\in \mathscr{U}$、環 $M \otimes_K E$ は、$M \otimes_K L$ の部分環と識別される可能性があり、したがって、和集合が $M \otimes_K L$ である$M \otimes_K L$ の部分環の増加するの有向ファミリーが得られます。 2 番目の主張がすぐに続きます。

#### 命題 7 {#alg-v-s17-prop-7 .statement tag=06W0}

— L を体 K および M の拡大と L-代数 (たとえば、 L の拡大) とします。 L が K 上で正則であり、M が正則 L-代数である場合、M は K-代数として正則です。

E を K の拡大とします。 L は K よりも正規なので、$E \otimes_K L$ は整域です。提案 2 (V, p. 141) により、環 $(E \otimes_K L) \otimes_L M$ は整域となり、これと同型の環 $E \otimes_K M$ にも同じことが当てはまります (II. p. 278、提案 2)。したがって、結果は次のとおりです。

#### 命題 8 {#alg-v-s17-prop-8 .statement tag=06W1}

— L と M を体 K の 2 つの拡大とします。

a) M が K に対して正則である場合、整域 $L \otimes_K M$ の分数の体は L の正則拡大です。

b) L と M が K の正規の拡大である場合、同じことが $L \otimes_K M$ の分数の体にも当てはまります。

主張 a) は提案 3、c) (V、p. 141) および Cor. V、p. 141; 主張 b) は、提案 3、b) (V、p. 141) および Cor. V、p. 141の。

### 5. 通常の拡大の特徴付け

#### 命題 9 {#alg-v-s17-prop-9 .statement tag=06W2}

— K を K の体、$\overline{K}$ 代数閉包、および K の L 拡大とします。すると、次の条件は等価です。

a) L は K 上で分離可能であり、K は L において比較的代数的に閉じています。

b) L は K の通常の拡大です。

c) 環 $\overline{K} \otimes_K L$ は整域です。

d) $\overline{L}$ を L の代数閉包とします。次に、L は、$\overline{L}$ における K の相対的な代数閉包から K 上で線形に互いに素になります。

さらに、これら条件が成り立つとき、$\overline{K} \otimes_K L$は体となります。

a) $\Rightarrow$ b): M を K の拡大とします。a) の仮説の下では、V、p. 140、Cor より、環 $M \otimes_K L$ は整域です。

b) $\Rightarrow$ c): これは定義から導き出されます。 2.

c) $\Rightarrow$ d): d) の記法を使用して、$\overline{L}$ の K の相対値代数閉包を使用して同一視できる $\overline{K}$ (V、p. 22、例 2)。 環 $A = \overline{K} \otimes_K L$ が整域であるとします。 E を K 上の有限次数の K の部分拡張とする。 部分環

A の E $\otimes_K$ L は整域であるため、L 上の有限次数の代数です。コルによって。 V、p. 10の体です。 $\bar{K}$は上記型の拡大Eの和集合増加する有向集合なので、Aは体になります（V、p. 11、提案3）。 したがって、A の $\bar{L}$ へのマッピング $x \otimes y$ から $xy$ ($x \in \bar{K}$ と $y \in L$ の場合) への正準準同型性は単射的であるため、L と $\bar{K}$ は K に関して線形素です。

$d) \Rightarrow a)$: d) の仮説の下では、$L \cap \bar{K} = K$ があるため、K はL で比較的代数的に閉じています。さらに、p が K の特性指数である場合、体 $L$ は $K^{p^{-\infty}}$ から $K$ にわたって線形に互いに素であるため、L は K 上で分離可能です (V、p. 123、Cor. 1)。

#### 系 1 {#alg-v-s17-prop-9-cor-1 .statement tag=06W3}

— A が体 K よりも代数であるとします。A が通常の K-代数であるためには、環 $\bar{K} \otimes_K A$ が整域であることが必要かつ十分です。

記載されている条件は明らかに必要です。 逆に、$\bar{K} \otimes_K A$を整域として、Aの分数のE体で表します。 提案 4 により (V, p. 141) 環 $\bar{K} \otimes_K E$ は整域であるため、提案 9 により E は K の正規の拡大です。 V、p. 141、Cor. によると、A は K-代数として正規であると結論する。

#### 系 2 {#alg-v-s17-prop-9-cor-2 .statement tag=06W4}

— K を代数閉体とします。 整域であるすべての K-代数は通常の K-代数です。特に、K のすべての拡大は規則的です。

これはコルからの続きです。 1.

#### 系 3 {#alg-v-s17-prop-9-cor-3 .statement tag=06W5}

— K を代数閉体とします。 A と B が 2 つの K-代数で、整域である場合、$A \otimes_K B$ についても同じことが当てはまります。

コル著2、A と B は正規の K-代数であり、提案 2 (V, p. 141) を適用するだけで十分です。

### 6. 複合材料への応用拡大

#### 命題 10 {#alg-v-s17-prop-10 .statement tag=06W6}

— L と M を、体 K の 2 つの拡大と、L と M (V、p. 12) の合成拡大である$(E, u, v)$ とします。 環 $L \otimes_K M$ が整域であり、E の部分拡張 $u(L)$ と $v(M)$ が K 上で代数的に互いに素であるとします。その場合、$u(L)$ と $v(M)$ は K 上で線形に互いに素になります。

$w = u * v$ (V, p. 12) を置き、整域 $L \otimes_K M$ の分数の F 体と同一視する L (それぞれ M) を、写像によって F の部分体で表します。 $x \mapsto x \otimes 1$ (それぞれ $y \mapsto 1 \otimes y$);この場合、w から L (または M) の制限は u (または v) になります。 B を K に対する M の超越基底とします (V, p. 109, Th. 1)。

仮定により、$u(L)$ と $v(M)$ は代数的に K 上で互いに素になります。したがって (V, p. 114, 提案 14)、$u(L)$ と $v(K(B))$ は K 上で線形互いに素です。 したがって、L 上の u および v ou K(B) と一致する K 準同型性 $u': L(B) \to E$ が存在します。 構成 L により、M は F の K に対して直線的に互いに素になります。提案 8 (V, p. 15) による F の部分体 $L(B)$ と $M$ は $K(B)$ に対して線形互いに素です。したがって、$L(B)$ では $u'$ と一致し、$M$ では $v$ と一致する K 準同型性 $w' : M[L(B)] \to E$ が存在することになります。しかし、体 $F$ は $M \cup L(B)$ によって生成され、$M$ は $K(B)$ に対して代数的です。したがって、$M[L(B)] = F$ (V、p. 18、コリント 2) になります。したがって、$w'$ は $F$ から $E$ への K-同型写像であり、その $L$ (それぞれ $M$) に対する制限は $u$ (それぞれ $v$) であるという結論する 。これは、$u(L)$ と $v(M)$ が $K$ に対して直線的に互いに素であることを示しています。

#### 系 1 {#alg-v-s17-prop-10-cor-1 .statement tag=06W7}

*$\Omega$ を体 $K$ の拡大とし、$L$ を $K$ の正規の $\Omega$ のサブエクステンションとします。 $L$ から $K$ までの代数的に互いに素である $\Omega$ のすべての部分拡張 $M$ は、線形互いに素です。*

環 $L \otimes_K M$ は、通常の拡大の定義による整域であり、提案 10 を適用するだけで十分です。

#### 系 2 {#alg-v-s17-prop-10-cor-2 .statement tag=06W8}

*$\Omega$ を体 $K$ と $L, M$ $\Omega$ の 2 つのサブエクステンションの拡大とします。 $L$ が $K$ 上で分離可能であり、$M$ の $K$ の相対値分離閉包が $K$ に等しいとします。 $L$ と $M$ が代数的に $K$ に対して互いに素である場合、それらは線形的に $K$ に対して互いに素になります。*

提案 10 によれば、環 $L \otimes_K M$ は整域 (V, p. 140, Cor.) であることに留意するだけで十分です。

練習問題

### 練習問題 {#alg-v-s17-exercises}

[§ 17 に対して練習問題](exercises/s17/)を参照してください。
