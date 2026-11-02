---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 13
section_title: p-radical extensions of height _ 1
lang: ja
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.98-A V.106, A V.170-A V.171
pdf_pages: 0212-0220, 0284-0285
extraction: ocr
subsections:
    - "no": 1
      title: $p$-free subsets and pbases
      page: 98
      pdf_page: 212
    - "no": 2
      title: Differentials and pbases
      page: 100
      pdf_page: 214
    - "no": 3
      title: The correspondence between subfields and Lie algebras of derivations
      page: 104
      pdf_page: 218
statements: 21
exercises: 6
content_sha256: c8dd377adf596a5b4cb0ed474dbbcd0a6cbe1bdf92f0914fa5d0ff11a93ea237
translated_from: content/en/alg/V/13_s13_p_radical_extensions_of_height_1.md
translation_method: google
source_content_sha256: d7c5aa125c07daf15aa12374780d959bd9cb9aac8300a2a5e8c9396f60d1751b
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: e99d5081359fd57ab6aa9ad2484ce50127ec4f6251f03357718780142ca2527d
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 13。 $p$-急激な身長の伸長$\leq 1$

この段落全体を通じて、$p$ は素数数を表します。考慮されたすべての体は特性 $p$ のものです。

### 1. $p$ フリー 部分集合および pbase

#### 定義 1 {#alg-v-s13-def-1 .statement tag=06QX}

Let $K$ be a field and $L$ a $p$-radical extension of height $\leq 1$ of $K$. $L$の元の家族$(x_i)_{i \in I}$は、$i \in I$と準同型すべてに対して$x_i \notin K$であれば、$K$以上$p$が無いと言われます（それぞれ、$K$以上$L$を基準として$p$）。 標準単射 $u_i : K(x_i) \to L$ から派生した $L$ への $\bigotimes_{i \in I} K(x_i)$ は単射 (それぞれ全単射) です。

$a$ が $L - K$ の元である場合、それは高さ 1 の $p$ 基数であるため、$K$ 上の最小多項式は $X^p - a^p$ ($V$, p. 24、提案 1) です。したがって、$\{1, a, \ldots, a^{p-1}\}$ は $K$ 上の $K(a)$ の基底です。 $(x_i)_{i \in I}$ を、有限台 $a = (\alpha_i)_{i \in I}$ のすべての家族のうち、$L - K$ の元と $\mathbf{N}^{(I)}$ からなるの $A$ 部分集合の家族とし、すべての $i \in I$ に対して $\alpha_i < p$ が得られるようにします。 Prop. 9 (III, p. 471) shows that the elements $\bigotimes_{i \in I} x_i^{\alpha_i}$ as $a$ runs over $A$ form a basis of the vector space $\bigotimes_{i \in I} K(x_i)$ over $K$. さらに、$\bigotimes_{i \in I} K(x_i)$ の $L$ への標準準同型は像 $K(x_i)_{i \in I}$ ($V$, p. 18, Cor. 1) となり、次の命題が得られます。

#### 命題 1 {#alg-v-s13-prop-1 .statement tag=06QY}

$K$ を体、$L$ を $K$ の高さ $\leq 1$ と $x = (x_i)_{i \in I}$ の $p$ 根拡張、つまり $L$ の元の族とする。すると、$A$の$a$に対して、積$x'' = \prod_{i \in I} x_i^{\alpha_i}$によって$K$上のベクトル空間$K(x_i)_{i \in I}$が生成されます。 $(x_i)_{i \in I}$ が $p$ から自由になるためには（それぞれ $p$ ベースで）、家族 $(x^a)_{a \in A}$ が $K$ 以降（それぞれ $K$ より $L$ の基底 ）自由であることが必要かつ十分です。

#### 系 {#alg-v-s13-n1-cor-1 .statement tag=06QZ}

— L' を 2 つの線形互いに素部分拡張 K' と L によって生成された体 K の拡大とします。 L が K 上の高さ $\leq 1$ の p ラジカルであると仮定します。 *そのとき* L' は K' 上の高さ $\leq 1$ の p-ラジカルです。さらに、L の元の族が K 上で p-free (それぞれ、K 上で $L$ の p 基底) であるためには、それが K' 上で p-free (それぞれ、K' 上で L' の p-基底) であることが必要かつ十分です。

${L'}^p \subset K \subset K'$と$L' = K'(L)$、よって${L'}^p = {K'}^p({L'}^p) \subset K'$があります。他の語では、L' は K' の高さ $\leq 1$ の p ラジカルの拡張です。 系の残りの主張は、提案 1 と、V、p. 14、提案 5 からすぐに続きます。

#### 注意 {#alg-v-s13-n1-rem-1 .statement tag=06R0}

K を体、L を K の高さ $\leq 1$ の p ラジカル拡張とし、$(x_i)_i$、L の元の族とする。 A を多項式代数 $K[(X_i)_{i \in I}]$ とし、多項式 $X_i^p - x_i^p$ と $\varphi : A \to L$ K-代数準同型によって生成される A のイデアルを、各 $i \in I$ に対して $\varphi(X_i) = x_i$ となるようにします。ファミリ $(x_i)_i$ は、$\varphi$ の核が a に等しい場合に限り、p-free です。 $K[(X_i)]/a$ は代数 $\bigotimes_{i \in I} K[X_i]/(X_i^p - x_i^p)$ と識別される場合があります。

L を、体 K の高さ $\leq 1$ の p ラジカル拡張とします。 $L$ の部分集合 S は、それ自体に対する S の恒等写像によって定義される族が p フリー (または p 基底) である場合、p フリー (または p 基底) であると言われます。 $L$ の元の族 $(x_i)_i$ が p-free (それぞれ p 基底) であるためには、写像 $i \mapsto x_i$ が p-free 部分集合 (それぞれ p 基底) で I の全単射であることが必要かつ十分です。 Lの。提案 1 により、p-free 集合のすべての部分集合は p-free です。逆に、S が L の部分集合で、そのすべての有限部分集合が p-free である場合、S は p-free です。最後に、K 上の L の p 基底は、$L = K(B)$ となる p-free 部分集合 B です。

#### 命題 2 {#alg-v-s13-prop-2 .statement tag=06R1}

— K を体、$L$ を K の高さ $\leq 1$ と L の S 部分集合の p ラジカル拡張とします。 S が p-free であるためには、S の部分集合 $T \neq S$ ごとに $K(T) \neq K(S)$ であることが必要かつ十分です。

まず、S が p-free であると仮定し、$T \neq S$ を S の部分集合とします。0 と $p-1$ の間の整数の有限台 $a = (\alpha_s)_{s \in S}$ を持つ族の A 集合で表します。 $A'$ を、$S - T$ のすべての について $a_s = 0$ となるように、家族 $a = (\alpha_s)_{s \in S}$ のからなるの部分集合とします。 $a \in A$には$u_a = \prod_{s \in S} s^{\alpha_s}$も入れます。すると (V, p. 98、提案 1) ファミリー $(u_a)_{a \in A'}$ は K 上の $K(S)$ の基底であり、サブファミリー $(u_a)_{a \in A'}$ は K 上の $K(T)$ の基底です。 $A' \neq A$ 以来、次のようになります。 $K(T) \neq K(S)$。

ここで、S が p-free ではないと仮定します。次に、S の元 $x_1, ..., x_n$ の整数 $n \geq 1$ と数列が存在し、$(x_1, ..., x_{n-1})$ は p-free ですが、$(x_1, ..., x_n)$ は p-free ではありません。 $[K(x_1, ..., x_{n-1}):K] = p^{n-1}$と$[K(x_1, ..., x_n):K] < p^n$がございます。 $[K(x_1, ..., x_n):K]$ は $[K(x_1, ..., x_{n-1}):K]$ の倍数であるため、次のようになります。

$$
[K(x_1, ..., x_n):K] = [K(x_1, ..., x_{n-1}):K].
$$

よって $x_n \in K(x_1, ..., x_{n-1})$。これは$K(S - \{x_n\}) = K(S)$を示しています。

#### 命題 3 {#alg-v-s13-prop-3 .statement tag=06R2}

— K を体、L を K と S の高さ $\leq 1$ の p ラジカル拡張とし、T を L の 2 つ部分集合とします。次の条件は同等です。
a) 部分集合 S は K 上で p-free であり、T は K(S) 上で p-free です。
b) $S \cap T = \varnothing$ *および* S U T は K 上で p-free です。
T が K(S) 上で p-free の場合、$T \cap K(S) = \varnothing$ となおさら $S \cap T = \varnothing$ が得られます。したがって、S と T 互いに素を仮定することができます。 A をすべての家族 $a = (a_x)_{x \in S \cup T}$ の $N^{(S \cup T)}$ からなるのうち部分集合とし、すべての $x \in S \cup T$ を $a_x < p$ とし、$N^{(S)}$ と $A''$ を定義する部分集合 $A'$ とします。 $N^{(T)}$も同様です。自然な方法で、同一視する $N^{(S \cup T)}$ を $N^{(S)} \times N^{(T)}$ とすると、A は $A' \times A''$ と識別されます。 $a \in A$ には $u_a = \prod_{x \in S \cup T} x^{\alpha_x}$ を、同様に定義する $u'_\beta$ と $u''_\gamma$ を $\beta \in A'$ と $\gamma \in A''$ に入れます。 $A = A' \times A''$の$a = (\beta, \gamma)$に対して$u_a = u'_\beta u''_\gamma$がございます。さらに、$(u'_\beta)_{\beta \in A'}$ 生成するベクトル K 空間 K(S) (V, p. 94、提案 1)。 S U T が K 上で p-free であるためには、族 $(u'_\beta u''_\gamma)_{\beta \in A', \gamma \in A''}$ が K 上で自由であることが必要かつ十分です (V, p. 98、提案 1)。家族 $(u'_\beta)_{\beta \in A'}$ が K 上で自由であり、家族 $(u''_\gamma)_{\gamma \in A''}$ が K(S) 上で自由であると仮定することも同じになります (II、p. 222)。ここで、a) と b) の同値は、提案 1 (V, p. 98) から導き出されます。

#### 系 {#alg-v-s13-n1-cor-2 .statement tag=06R3}

— L を K の高さ $\leq 1$ の p ラジカル拡張とし、M を L の部分拡張とします。この場合、L は M 上の高さ $\leq 1$ の p ラジカルであり、M は K 上の高さ $\leq 1$ の p ラジカルです。 さらに、B が K 上の M の p 基底であり、C が M 上の L の p 基底である場合、$B \cap C = \varnothing$ および $B \cup C$ はK に対する L の p ベース。

Kを体とします。族 $(x_i)_{i \in I}$ は、$K^p$ 上の K の p 基底である場合、K の (絶対) p 基底であると言われます。すべての整数 $n \geq 1$ を、すべての $i \in I$ に対して $\alpha_i < p^n$ となるように、すべての $a = (\alpha_i)_{i \in I}$ の $N^{(I)}$ からなるの $\Lambda(n)$ 部分集合で表します。

#### 命題 4 {#alg-v-s13-prop-4 .statement tag=06R4}

— $x = (x_i)_{i \in I}$ を K の p 基底とします。すべての整数 $n \geq 1$ に対して、族 $(x^u)_{u \in \Lambda(n)}$ は $K^{p^n}$ 上の K の基底です。

$n = 1$ 主張簡約するの場合、提案 1 (V、p. 98) に。 集合 $\Lambda(n)$ は、形 $a = \beta + p^{n-1}\gamma$ の $N^{(I)}$ の元と $\beta \in \Lambda(n-1)$ と $\gamma \in \Lambda(1)$ で構成されます。そんな分解はユニークで、$x^\alpha = x^\beta (x^\gamma)^{p^{n-1}}$もございます。さらに、族 $(x_i^{p^{n-1}})_{i \in I}$ は明らかに $K^{p^n}$ に対する $K^{p^{n-1}}$ の p 基底であるため、族 $(x^\gamma)^{p^{n-1}}$ は $K^{p^n}$ に対する $K^{p^{n-1}}$ の基底です。したがって、II、p. 222、提案 25 を使用して、帰納法によって結論が得られます。

### 2. 差分と pbase

K を (特性 p の) 体および K 上の V ベクトル空間とします。 (III, p. 552) V への K の導分は、V 満たすへの K の写像 D であることを思い出します。 関係
$$
\begin{align*}
D(x + y) &= D(x) + D(y) \\
D(xy) &= xD(y) + yD(x)
\end{align*}
$$

$x,\ y \in K$の場合。すべての $x \neq 0$ とすべての $n \in \mathbf{Z}$ (III、p. 557、および 558) に対して、$D(1) = 0$ と $D(x^n) = nx^{n-1}D(x)$ が続きます。 $K$ は特性 $p$ であるため、すべての $x \in K$ が成立します。

$$
D(x^p) = 0 .
$$

さらに (III、p. 558)、$x,\ y \in K,\ y \neq 0$ については、

$$
D(x/y) = (yD(x) - xD(y))/y^2
$$

上の式より、$D$の核は、$K$含む$K^p$の部分体$E$となります。 $M$ を $K$ の部分体とします。 $M$-線形であれば、$D$ は $M$-導出であると言います。 (2)により、$D$～$M$の制限を零と仮定することと同じになります。

(III, p. 570) は、$K$ の$M$ 微分と、$K$ から $\Omega_M(K)$ への正規の $M$-導出$d = d_{K/M}$ の加群 $\Omega_M(K)$ を定義しました。 $d_{K/M}$ 生成するベクトル $K$-スペース $\Omega_M(K)$ の像。 For a mapping $D$ of $K$ into $V$ to be an $M$-derivation it is necessary and sufficient that there should exist a $K$-linear mapping $u : \Omega_M(K) \to V$ such that $D = u \circ d_{K/M}$; this mapping $u$ is uniquely determined.

#### 命題 5 {#alg-v-s13-prop-5 .statement tag=06R5}

*$K$ を元 $x$ によって生成された $K$ の体と $L$ 拡大とし、$x \notin K,\ x^p \in K$ とします。 Let $V$ be a vector space over $L$ and $A$ a derivation of $K$ into $V$ such that $\Delta(x^p) = 0$. 次に、$L$ を $V$ に拡張し、$A$ を延長する$D(x) = 0$ などの一意の導分 $D$ が存在します。

$V$、p. 24 より、提案 1、$\{1,\ x,\ \ldots,\ x^{p-1}\}$ は、$K$ に対する $L$ の基底です。 $L$ のすべての元 $u = a_0 + a_1x + \ldots + a_{p-1}x^{p-1}$ ($K$ には $a_0,\ \ldots,\ a_{p-1}$ が含まれます) に $D(u) = A(a_0) + x\Delta(a_1) + \ldots + x^{p-1}\Delta(a_{p-1})$ を置きます。 $D$ 拡大する $A$ が (1) を満たすことは明らかです。したがって、関係を確立するだけで十分です

$$
D(uv) = u \cdot D(v) + v \cdot D(u)
$$

$u$ が形 $ax^i$ と $v$ の形 $bx^j$ で、$K,\ 0 \leq i < p$ と $0 \leq j < p$ に $a,\ b$ がある場合。

$i + j < p$ のとき、$uv = x^{i+j}ab$、よって $D(uv) = x^{i+j}\Delta(ab)$ になります。それ以外の場合は、$0 \leq i + j - p < p$ があるので、$abx^p \in K$ で $uv = x^{i+j-p}(abx^p)$ になりますが、$A(x^p) = 0$ なので、$A(abx^p) = x^pA(ab)$、よってが再び $D(uv) = x^{i+j}\Delta(ab)$ になります。したがって、すべての場合において、

$$
\begin{align*}
D(uv) &= x^{i+j}\Delta(ab) = x^i x^j (a \cdot A(b) + b \cdot \Delta(a)) \\
&= (ax^i)x^j \cdot \Delta(b) + (bx^j)x^i \cdot \Delta(a) = u \cdot D(v) + v \cdot D(u) .
\end{align*}
$$

#### 系 1 {#alg-v-s13-prop-5-cor-1 .statement tag=06R6}

*Let $K$ be a field, $L$ a $p$-radical extension of height $\leq 1$ of $K$ and $V$ a vector space over $L$. $K$ の導分 $A$ から $V$ までは、$L^p$ 拡大するから導分の $L$ で $V$ に消えます。

Zorn の補題 (E、III、p. 20) により、$A$ から導分 $D_0 : L_0 \to V$ までの最大拡大が存在します。ここで、$L_0$ は $L$ 含むの部分体です$K$。 $x \in L$ にしましょう。 $x^p \in L_0$と$A(x^p) = 0$、よって$D_0(x^p) = 0$があります。提案 5 により、

D_0 拡大する ～ 導分は L_0(x) で定義されます。 D_0 の最大値指標により、L_0(x) = L, よって x ∈ L_0 となります。 x は任意なので、L_0 = L である結論するとなります。

#### 系 2 {#alg-v-s13-prop-5-cor-2 .statement tag=06R7}

— L を体 K の高さ ≤ l の p 根拡張とし、E を L の部分拡張とする。 U を E の元の差分によって生成された Ω_K(L) の部分空間とします。すると、E は、U に対する差分属するを持つ L の元で構成されます。特に、すべての x ∈ について d_{L/K}x ≠ 0 になります。 L − K.

x を、E に対する所属ではなく、L の元とします。そのとき、{1, x, ..., x^{p^{l-1}}} は、E 上の E(x) の基底です。A を、0 ≤ i < の場合、Δ(x^i) = ix' となるような E(x) の L への E 線形写像とします。 p. A が E(x) から L への E 微分、特に K 微分であることをすぐに検証します。コル著提案 1 から提案 5 まで、A を拡張する L への L の K 導出 D が存在します。Ω_K(L) の普遍性により、このベクトル L 空間上に D = u ∘ となる線型形式 u が存在します。 d_{L/K}。 D(x) = x および D|E = 0 です。したがって、u(d_{L/K}x) ≠ 0 および u|U = 0、よって d_{L/K}x ∉ U となります。

最後の主張は E = K の特殊なケースです。すると U = 0 になります。

#### 定理 1 {#alg-v-s13-thm-1 .statement tag=06R8}

— L を、体 K および (a_i)_{i ∈ I} の高さ ≤ l の p 根拡張とし、L の元の族とします。

a) (x_i)_{i ∈ I} が K 上で p-free であるためには、族 (dx_i)_{i ∈ I} がベクトル L-空間 Ω_K(L) で自由であることが必要かつ十分です。

b) For (x_i)_{i ∈ I} to generate L over K it is necessary and sufficient that the family (dx_i)_{i ∈ I} should generate the vector L-space Ω_K(L).

c) (x_i)_{i ∈ I} が K 上の L の p 基底であるためには、族 (dx_i)_{i ∈ I} がベクトル L 空間 Ω_K(L) の基底であることが必要かつ十分です。

まず、体 K((x_i)_{i ∈ ∈ I}) の元の微分 dx は線形結合であり、微分 dx_i, i ∈ I の L には係数が含まれることに注意してください。族 (x_i)_{i ∈ I} が p-free であるためには、すべての i ∈ I に対して x_i ∉ K(x_j)_{j ∈ I - {i}} であることが必要かつ十分です (V, p. 99、提案 2)。コル著提案 5 の 2 これは、dx_i が、I の j ≠ i に対する dx_j の線形結合ではないことを意味します。 主張 a) はこれから続きます。ここで b) はコルからすぐに続きます。 2 から提案 5 まで、および c) は a) と b) から導かれます。

次の系は Cor を作成します。提案 5 の 1 はより具体的です:

#### 系 {#alg-v-s13-n2-cor-1 .statement tag=06R9}

— (x_i)_{i ∈ I} を K 上の L の p 基底とします。 V を L 上のベクトル空間とします。K の導分を V に変換し、L^p と (u_i)_{i で消滅します。 ∈ I} V の元の家族。次に、V には拡大する A と写像 x_i がすべての i ∈ I に対して u_i となる、L の一意の導分 D が存在します。

コル著提案 5 の 1 では、A を拡張した V に L の導分 D_0 が存在します。 A を拡張した V の L の導分は、正確に形の写像 D = D_0 + u ∘ d_{L/K} です。 u は、Ω_K(L) の V への L 線形写像です。 線形写像 u が条件 u(dx_i) = u_i − D_0(x_i) を満たす場合に限り、D(x_i) = u_i になります。 dx_i 族は Ω_K(L) の基底なので、この決定する u は一意に系が続きます。

L を K の高さ $\leq 1$ の p 基拡張とし、$(x_i)_{i \in I}$ を K 上の L の p 基底とします。 Thさんへ。 1 $i \in I$ ごとに、$D_i(x_j) = \delta_{ij}$ (クロネッカー記号) によって特徴付けられる L から L への K 導出$D_i$ が存在します。 $D_i$ は、$x_i$ に関して * 部分的な導分と呼ばれるときどきです。 $I$ が *有限* の場合、族 $(D_i)_{i \in I}$ は、L から L への K 導出の L からなる上のベクトル空間の基底です。

Th. 1 により、p 塩基の研究をベクトル空間の基底の研究に減らすことができます。たとえば、次の結果が得られます。

#### 定理 2 {#alg-v-s13-thm-2 .statement tag=06RA}

— *Lを、体K*の高さ$\leq 1$のpラジカル拡張とします。
  *a)* *K 上に L の p 基底が存在します。より正確には、S が K 上で L の p-free 部分集合と、$S \subset T$ および $L = K(T)$ のような L の T 部分集合である場合、次のような K 上で L の p 基底 B が存在します。 $S \subset B \subset T$.*
  *b)* *K 上の L の 2 つの p 塩基は同じ基数を持ちます。*
  *c)* *$[L:K]$が有限であるためには、L以上のベクトル空間$\Omega_K(L)$がL以上の有限次元であることが必要かつ十分であり、その場合*

$$
[L : K] = p^{[\Omega_K(L) : L]}
$$

主張 *a)* と *b)* は明らか (II, p. 292) です。 $[L : K]$ が有限である場合、*a)* により、$K$ 上の $L$ の有限 p 基底 $(x_1, ..., x_n)$ が存在します。次に、$K$以上の$L$の$1 \leq i \leq n$形基底と、$\Omega_K(L)$以上の微分$dx_1, ..., dx_n$形基底の$0 \leq \alpha_i < p$を含む単項式$x_1^{\alpha_1} ... x_n^{\alpha_n}$ $L$。したがって、$[L : K] = p^n$ と $[\Omega_K(L) : L] = n$ ができます。逆に、$\Omega_K(L)$ が $L$ 上で有限次元である場合、K 上で L の有限 p 基底が存在し (V, p. 102, Th. 1)、$[L : K]$ は有限です。

#### 系 {#alg-v-s13-n2-cor-2 .statement tag=06RB}

— *各 $x \in L - K$ に対して、K 含む X 上に L の p 基底が存在します。*

$\{x\}$ は $K$ を超える $L$ の p-free 部分集合であるため、Th を適用するだけで十分です。 2、*a)*。

K を K の体と $L$ 拡大とします。 $D$ がベクトル L 空間内の値による L の K 導出である場合、すべての $x \in L$ に対して $D(x^p) = 0$ が得られます。したがって、$D$ は $K(L^p)$ から導出されます。 $\Omega_K(L) = \Omega_{K(L^p)}(L)$ ということになります。 $L$ は $K(L^p)$ の高さ $\leq 1$ の p ラジカル拡張であるため、上記の結果を適用できます。たとえば、Th から。 1、*c)* 次のことを推定します: $(x_i)_{i \in I}$ を $L$ の元の族とする。 $(dx_i)_{i \in I}$ がベクトル L-空間 $\Omega_K(L)$ の基底であるためには、$(x_i)_{i \in I}$ が $K(L^p)$ に対する L の p 基底であることが必要かつ十分です。同様に、Cor.提案 5 の 2 は次のことを意味します。

#### 命題 6 {#alg-v-s13-prop-6 .statement tag=06RC}

— *K を (特性 p の) 体および K の L 拡大とします。*
  *a)* *$x \in L$; しましょう。差分 $d_{L/K}x$ は、x 属するから $K(L^p)$ の場合にのみ消滅します。*
  *b)* $\Omega_K(L) = 0$ $L = K(L^p)$ の場合に限り、*
  *c)* *L が K 上の有限高さの p ラジカルであると仮定します。 $L = K$ の場合に限り、$\Omega_K(L) = 0$。*

### 3. 導分の部分体とリー代数の間の対応

E 体で、E のすべての導分を g 集合でそれ自体に表します。 g は E 上でベクトル空間であり、演算は次のように定義されることを思い出してください。

$$(D + D')(x) = D(x) + D'(x), \quad (aD)(x) = a \cdot D(x)$$

$g$の$D, D'$と$E$の$a, x$。また、$D$と$D'$がEの導分をEにすると、$[D, D'] = DD' - D'D$(III、p. 554)も同様です。最後に、ライプニッツの公式 (III, p. 556) は次のようになります。

$$D^p(xy) = x \cdot D^p(y) + \sum_{j=1}^{p-1} \binom{p}{j} D^j(x) D^{p-j}(y) + D^p(x) \cdot y$$

($x, y$ で $E$); $1 \leq j \leq p-1$ の二項係数 $\binom{p}{j}$ は $p$ ($V$, p. 4, 補題 1) で割り切れるので、$D^p$ は E の導分を E に変換したものであることがわかります。すぐに関係が見つかります ( $a, a' \in E$)

$$[aD, a'D'] = aa' \cdot [D, D'] + (aD(a')) \cdot D' - (a'D'(a)) \cdot D.$$

特に、$g \times g$ から $g$ への写像 $(D, D') \mapsto [D, D']$ は $E^p$ 線形です。

$E^p \subset K$ と $[E : K]$ が有限であるように、$\mathscr{C}$ 集合の部分体 $K$ の $E$ で表します。それぞれの $K \in \mathscr{C}$ を、E の K 導出の $g(K)$ 集合で表します。 Further, we denote by $\mathscr{L}$ the set of vector subspaces $l$ of $g$ of finite dimension over E and such that $[D, D'] \in h$ and $D^p \in h$ for any $D, D'$ in $h$; for each $h \in \mathscr{L}$ we denote by $I(h)$ the set of $x \in E$ such that $D(x) = 0$ for all $D \in h$.

#### 定理 3 (ジェイコブソン) {#alg-v-s13-thm-3 .statement tag=06RD}

— *写像 $K \mapsto g(K)$ と $l \mapsto I(h)$ は、それぞれ $\mathscr{C}$ の $\mathscr{L}$ と $\mathscr{L}$ の $\mathscr{C}$ の全単射であり、相互に反転しています。 $K \in \mathscr{C}$ と $h \in \mathscr{L}$ 対応するがお互いに一致する場合、$[E : K] = p^{[h : E]}$*。

証明には、いくつかの予備的な補題が必要です。

#### 補題 1 {#alg-v-s13-lem-1 .statement tag=06RE}

— *Lを体、Vベクトル空間をL、そしてVの自己準同型を$u^p = u$とする。それぞれの $i \in \mathbf{F}_p$ について、$V_i$ を $u - i$ の核とします。それでは*

$$\mathbf{V} = \bigoplus_{i \in \mathbf{F}_p} V_i.$$

それぞれの $i \in \mathbf{F}_p$ を $P_i(X)$ で多項式 $- \prod_{j \neq i} (X - j)$ で表します。我々は持っています

$$(X - i) P_i(X) = X - X^p$$

公式 (2) ($V$, p. 94) 作。引用された公式 (2) を導き出すと、次のことがわかります。

$$\sum_{i \in \mathbf{F}_p} P_i(X) = 1$$

式(8)と(9)は、$V$写像$V$の自己準同型$P_i(u)$を$V_i$に、$\sum_{i \in \mathbf{F}_p} P_i(u) = 1$、よって$V = \sum_{i \in \mathbf{F}_p} V_i$を示しています。 和が直接であることを示すことはまだ残っています。それぞれの $i \in \mathbf{F}_p$ に対して $v_i \in V_i$ を設定します。 $P_i(u)$ がすべての $j \neq i$ に対して $v_j$ を全滅させることは明らかであり、$a = -\prod_{n \in \mathbf{F}_p^*} n \neq 0$ で $P(u)v_i = av_i$ が得られます。したがって、関係 $\sum_{i \in \mathbf{F}_p} v_i = 0$ はすべての $i \in \mathbf{F}_p$ に対して $v_i = 0$ を意味し、したがって和は直接的です。

#### 補題 2 {#alg-v-s13-lem-2 .statement tag=06RF}

*D を $D^p = D$ となる E の導分とし、K を D の核とする。E に $D(x) = x$ となる非ゼロの x が存在すると仮定します。すると、K は E 含む $E^p$ の部分体となり、$[E : K] = p$ となります。*

K が E 含む $E^p$ の部分体であることは明らかです。 $i \in \mathbf{F}_p$ を $D - i$ の $K_i$ 核で表します。 $K_0 = K$ と補題 1 は $E = \bigoplus_{i \in \mathbf{F}_p} K_i$ を示しています。 $i \in \mathbf{F}_p$ と $u$ を $K_i$ にします。私たちは持っています
$$
D(xu) = D(x) \cdot u + x \cdot D(u) = xu + x(iu) = (i + 1)xu
$$
よって $xu \in K_{i+1}$。 x はゼロではないので、x による乗法は、すべての $i \in \mathbf{F}_p$ に対して写像 $K_i$ を$K_{i+1}$ 上に置くベクトル K 空間 E の自己同型です。 $[K_0 : K] = 1$ なので、$i \in \mathbf{F}_p$ よって $[E : K] = p$ はすべて $[K_i : K] = 1$ になります。

#### 補題 3 {#alg-v-s13-lem-3 .statement tag=06RG}

*$\mathfrak{h} \in \mathscr{L}$ を E 上の次元とします。すると、$I(\mathfrak{h})$ 属するから $\mathscr{C}$ となり、$[E : I(\mathfrak{h})] = p^s$ が得られます。

$I(\mathfrak{h})$ が $E$ 含む $E^p$ の部分体であることは明らかです。それぞれの $x \in E$ について、$f_x$ を I 上の E 線形形式 $D \mapsto D(x)$ とします)。これら線型形式の kcrncls の共通部分は 0 に等しいため、それら生成するベクトル空間は $\mathfrak{h}$ (II、p. 301、Th. 7) と二重になります。したがって、この双対の線型形式 $f_{x_1}, \ldots, f_{x_s}$ 形基底のように、$E$ には $x_1, \ldots, x_s$ が存在します。 $(\Delta_1, \ldots, \Delta_s)$ を、$\Delta_i(x_j) = f_{x_j}(\Delta_i) = \delta_{ij}$ によって特徴付けられる $\mathfrak{h}$ の基底とします。 $D_i = x_i \Delta_i$ を置くと、$(D_1, \ldots, D_s)$ は E 上の I の基底となり、$D_i(x_j) = x_i \delta_{ij}$ が得られます。 導分 $D_i^p - D_i$ と $[D_i, D_j]$ を $i, j = 1, \ldots, s$ 属するから I に）、$x_1, \ldots, x_s$ を殲滅します。したがって、私たちは
$$
D_i^p = D_i , \quad [D_i, D_j] = 0
$$
0 から s の範囲の i について、$K_i$ 共通部分の核の導分 $D_j$ の $1 \leq j \leq i$ を表します。すると、$K_i$ は E の部分体となり、次のようになります。
$$
E = K_0 \supset K_1 \supset \ldots \supset K_{s-1} \supset K_s = I(\mathfrak{h}) .
$$
i を 0 から $s-1$ の間とします。この場合、$D_{i+1}$ は $D_1, \ldots, D_i$ と交換するため、$K_i$ は $D_{i+1}$ の下で安定します。さらに$D_{i+1}^p = D_{i+1}$、$D_{i+1}(x_{i+1}) = x_{i+1} \neq 0$、$x_{i+1} \in K_i$もあります。したがって、補題 1 は、$[K_i : K_{i+1}] = p$、よって、最終的には $[E : K] = [K_0 : K_s] = p^s$ であることを意味します。

定理の証明まで来ました。 I) $\in \mathscr{L}$ を E 上の次元とし、$K = I(\mathfrak{h})$ を置きます。次に、$[E : K] = p^s$ by 補題 3、よって $[\Omega_K(E) : E] = s$ by

Th. 2、c) (V、p. 103)。微分写像の加群の普遍性により、$u \mapsto u \circ d_{E/K}$は$\Omega_K(E)$と$g(K)$の双対の同型となり、したがって$[g(K):E] = s$になります。これで$[\mathfrak{h}:E] = s$と$\mathfrak{h} \subset g(K)$、よって$\mathfrak{h} = g(K)$、つまり$\mathfrak{h} = g(I(\mathfrak{h}))$ができました。

逆に、体 $K \in \mathscr{C}$ ごとに、$g(K)$ 属するから $\mathscr{L}$ であることは明らかです (V、p. 103、Th. 2、c))。 *$x$ 属するから $I(g(K))$ の場合、$\Omega_K(E)$、よって $d_{E/K}x = 0$ の各線型形式 $u$ に対して $u(d_{E/K}x) = 0$ があり、最終的に Cor によって $x \in K$ になります。提案 5 の 2 (V、p. 102)。したがって、$K = I(g(K))$ となります。

#### 注意 {#alg-v-s13-n3-rem-1 .statement tag=06RH}

— 1) 相互に逆全単射 $K \mapsto g(K)$ と $\mathfrak{h} \mapsto I(\mathfrak{h})$ は包含反転です。したがって、$\mathfrak{h} \mapsto I(\mathfrak{h})$ は、$\mathscr{C}$ の反対の順序集合上の順序集合 $\mathscr{L}$ の同型です。したがって、$\mathfrak{h} \cap \mathfrak{h}'$は$\mathfrak{h}$と$\mathfrak{h}'$の両方に含まれる$\mathscr{L}$の最大の元であるため、$\mathscr{L}$の$\mathfrak{h}, \mathfrak{h}'$に対して関係$I(\mathfrak{h} \cap \mathfrak{h}') = E^p(I(\mathfrak{h}), I(\mathfrak{h}'))$が得られます。

2) 写像 $D \mapsto D^p$ の下で安定している $g$ の有限次元のすべての部分空間は、括弧演算の下でも安定していることがわかります。

### 練習問題 {#alg-v-s13-exercises}

[§ 13 に対して練習問題](exercises/s13/)を参照してください。
