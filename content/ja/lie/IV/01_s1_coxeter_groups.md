---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IV
chapter_title: COXETER GROUPS AND TITS SYSTEMS
section: 1
section_title: Coxeter Groups
lang: ja
source: lie-iv-vi
pdf_pages: 0014-0028, 0044-0056
extraction: ocr
subsections:
    - "no": 1
      title: LENGTH AND REDUCED DECOMPOSITIONS
      page: 0
      pdf_page: 14
    - "no": 2
      title: DIHEDRAL GROUPS
      page: 0
      pdf_page: 15
    - "no": 3
      title: FIRST PROPERTIES OF COXETER GROUPS
      page: 0
      pdf_page: 17
    - "no": 4
      title: REDUCED DECOMPOSITIONS IN A COXETER GROUP
      page: 0
      pdf_page: 18
    - "no": 5
      title: THE EXCHANGE CONDITION
      page: 0
      pdf_page: 20
    - "no": 6
      title: CHARACTERISATION OF COXETER GROUPS
      page: 0
      pdf_page: 23
    - "no": 7
      title: FAMILIES OF PARTITIONS
      page: 0
      pdf_page: 23
    - "no": 8
      title: SUBGROUPS OF COXETER GROUPS
      page: 0
      pdf_page: 25
    - "no": 9
      title: COXETER MATRICES AND COXETER GRAPHS
      page: 0
      pdf_page: 26
statements: 30
exercises: 26
content_sha256: 61d3dc858406a17aae185e6b048609d9d99cd16e59e3235afb851581dc8b06cb
translated_from: content/en/lie/IV/01_s1_coxeter_groups.md
translation_method: google
source_content_sha256: aeca25119a4e3b1300664856f323c4070b977911903d6cf99cfb24051466f433
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: 2ceed707eea79c8c0d21d3b9684bfbd342da5d70131e75f142717d5deee8300b
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 1。コクセター 群

この切断では、W は単位元 1 で乗算的に書かれた群を表し、S は S = S^{-1} および 1 \notin S となる W の生成元の集合を表します。 W のすべての元は、S の有限列の元の積です。 no. 3 以降、S のすべての元は位数 2 であると仮定します。

### 1. 長さと削減された分解

#### 定義 1 {#lie-iv-s1-def-1 .statement tag=0ALN}

\in W にしましょう。 The length of w (with respect to S), denoted by l_S(w) or simply by l(w), is the smallest integer q \geq 0 such that w is the product of a sequence of q elements of S. (S に関して) w の縮小分解は、w = s_1 \cdots s_q および q = l(w) となるような、S の元の任意の数列 s = (s_1, \ldots, s_q) です。

したがって、1 は長さ 0 の一意元であり、S は長さ 1 の元で構成されます。

#### 命題 1 {#lie-iv-s1-prop-1 .statement tag=0ALO}

w と w' を W にします。 公式があります:

$$
l(ww') \leq l(w) + l(w'), \tag{1}
$$
$$
l(w^{-1}) = l(w), \tag{2}
$$
$$
|l(w) - l(w')| \leq l(w{w'}^{-1}). \tag{3}
$$

(s_1, \ldots, s_p) と (s'_1, \ldots, s'_q) をそれぞれ w と w' の分解だけ減らすとします。したがって、l(w) = p および l(w') = q となります。 ww' = s_1 \ldots s_p s'_1 \ldots s'_q なので、 l(ww') \leq p + q, 証明 (1) となります。 S = S^{-1} かつ w^{-1} = s_p^{-1} \ldots s_1^{-1} なので、l(w^{-1}) \leq p = l(w) となります。 置き換えること w by w^{-1} は、逆の不等式 l(w) \leq l(w^{-1})、証明 (2) を与えます。 (1) と (2) の置き換えること w by ww'^{-1} は関係を与えます

$$
l(w) - l(w') \leq l(w{w'}^{-1}), \tag{4}
$$
$$
l(w{w'}^{-1}) = l(w'w^{-1}). \tag{5}
$$

(4)の$w$と$w'$を交換すると、(5)で$l(w') - l(w) \leq l(w{w'}^{-1})$、(3)で証明が得られます。

#### 系 {#lie-iv-s1-n1-cor-1 .statement tag=0ALP}

*$s = (s_1, \ldots, s_p)$と$s' = (s'_1, \ldots, s'_q)$を$S$の元の2つの数列とし、$w = s_1 \ldots s_p$と$w' = s'_1 \ldots s'_q$とします。 数列 $(s_1, \ldots, s_p, s'_1, \ldots, s'_q)$ が $ww'$ の分解を減じたものである場合、$s$ は $w$ の分解を減じたものであり、$s'$ は $w'$ の 1 つです。

仮定、$l(w) \leq p$、$l(w') \leq q$、$l(ww') = p + q$ まで。 (1) までに、$l(w) = p$ と $l(w') = q$ が必要なので、系になります。

#### 注意 {#lie-iv-s1-n1-rem-1 .statement tag=0ALQ}

公式 (1) と (2)、公式 $d(w, w') = l(w{w'}^{-1})$ 定義するを考慮すると、$W$ 上の距離は、右変換の下では不変です。

### 2. 上反角群

#### 定義 2 {#lie-iv-s1-def-2 .statement tag=0ALR}

*二面体群は 2 つの位数のうち 2 つの異なる元によって生成される群です。

#### 例 {#lie-iv-s1-n2-exa-1 .statement tag=0ALS}

$M$ を乗法群 $\{1, -1\}$ とし、$m$ を整数 $\geq 2$ (それぞれ $m = \infty$) とします。次に、$M$ は、$(-1).x = -x$ によって群 $\mathbf{Z}/m\mathbf{Z}$ (それぞれ $\mathbf{Z}$) に作用し、$\mathbf{Z}/m\mathbf{Z}$ によって$M$ の対応する半直接積 (それぞれ$M$ に作用) $\mathbf{Z}$) は $D_m$ で表されます。したがって、$D_m$ の元は、$\varepsilon = \pm 1$ と $x \in \mathbf{Z}/m\mathbf{Z}$ (それぞれ $x \in \mathbf{Z}$) を含む対 $(\varepsilon, x)$ です。 $D_m$の群法則は公式によって与えられます
$$
(\varepsilon, x).(\varepsilon', x') = (\varepsilon \varepsilon', \varepsilon' x + x').
$$
1 を法とする $m$ (それぞれ $\iota = 1$) と集合の $\iota$ 類で表します。
$$
\rho = (-1, 0), \quad \rho' = (-1, \iota), \quad \pi = (1, \iota).
$$
続いて$\rho^2 = {\rho'}^2 = 1$と$\pi = \rho \rho'$。 公式
$$
\pi^n = (1, n\iota), \quad \rho \pi^n = (-1, n\iota)
$$
$D_m$ が $\{\rho, \rho'\}$ によって生成された二面体群であることを示します。

#### 命題 2 {#lie-iv-s1-prop-2 .statement tag=0ALT}

*$S$ は 2 つの異なる元 $s$ と位数 2 の $s'$ で構成されていると仮定します。

(i) *$p = ss'$によって生成された$W$の部分群$P$は正常で、$W$は部分群$T = \{1, s\}$と$P$の半直接積です。さらに、$(W : P) = 2$.*

(ii) *$m$ を $p$ の位数 (有限または無限) とします。すると、$m \geq 2$と$W$は位数$2m$になります。 $D_m$ から $W$ には、$\varphi(\rho) = s$ と $\varphi(\rho') = s'$ などの固有の同型 $\varphi$ があります*。

(i) $sps^{-1} = sss's = s's = p^{-1}$ があるため、
$$
sp^n s^{-1} = p^{-n}
$$

整数 $n$ごとに。 $W$ は $\{ s, s' \}$ によって生成され、したがって $\{ s, p \}$ によって生成されるため、部分群 $P$ は正常です。したがって、$TP$ は $W$ の部分群であり、$TP$ 含む $s$ と $s' = sp$ なので、$W = TP = P \cup sP$ になります。したがって、(i) を証明するには、$W \neq P$ を示すだけで十分です。 $W = P$ の場合、群 $W$ は可換なので、$p^2 = s^2 {s'}^2 = 1$ となります。しかし、その場合、$W = P$ の唯一の元は 1 と $p$ となり、$W$ 含むには少なくとも 3 つの元、つまり 1、$s$、$s'$ が存在するという仮定と矛盾します。

(ii) $s \neq s'$ なので、$p \neq 1$ があり、したがって $m \geq 2$ になります。 $P$は位数$m$と$(W : P) = 2$の$W$の位数は$2m$です。 $m$ が有限 (または無限) の場合、$\mathbf{Z}/m\mathbf{Z}$ (それぞれ $\mathbf{Z}$) から $\pi$ から $p$ を経て $P$ までの同型 $\varphi'$ が存在します。 さらに、$-1$から$s$を経て$M = \{ 1, -1 \}$から$T$まで同型$\varphi''$が存在します。 群 $W$ は、$T$ と $P$ の半直接積です。 公式 (9) と $\rho \pi^n \rho^{-1} = \pi^{-n}$、$\varphi'$ と $\varphi''$ 誘導する同型 $\varphi$ を$D_m$ から $W$ まで考慮すると、$\varphi(\rho) = s$ と $\varphi(\pi) = p$、したがって $\varphi(\rho') = s'$ になります。 The uniqueness of $\varphi$ follows from the fact that $D_m$ is generated by $\{ \rho, \rho' \}$.

#### 注意 {#lie-iv-s1-n2-rem-1 .statement tag=0ALU}

2 つの異なる元 $s$ と位数 2 の $s'$ によって生成された位数 $2m$ の二面体群 $W$ を考えます。 $s_q$ (それぞれ $s'_q$) 数列で表します長さ $q$ のうち、奇数 (偶数) の項が $s$ に等しく、偶数 (奇数) の項が $s'$ に等しく、$w_q$ (それぞれ $w'_q$) を積とします。 数列 $s_q$ (それぞれ $s'_q$)。我々は持っています

$$
w_{2k} = (ss')^k, \quad w_{2k+1} = (ss')^k s,
$$
$$
w'_{2k} = (s's)^k = (ss')^{-k}, \quad w'_{2k+1} = (s's)^k s' = (ss')^{-k-1} s.
$$

$s = (s_1, \ldots, s_q)$ が $W$ の元 $w$ を減じた分解 ($\{ s, s' \}$ に関して) である場合、明らかに $1 \leq i \leq q-1$ に対して $s_i \neq s_{i+1}$ です。したがって、$s = s_q$ または $s = s'_q$ になります。

$m = \infty$ の場合、$n \in \mathbf{Z}$ の元 $(ss')^n$ と $(ss')^n s$ は別個です。 したがって、元 $w_q$ ($q \geq 0$) と $w'_q$ ($q > 0$) は別個であり、$s$ が $w_q$ (それぞれ $w'_q$) の分解を減じたものである場合、必然的に $s = s_q$ (それぞれ $s = s'_q$) になります。 このことから、$l(w_q) = l(w'_q) = q$ と、$W$ の元を縮小した分解の *集合は、$s_q$ と $s'_q$* で構成されることがわかります。 さらに、$W$ のすべての元には、固有の縮小された分解があります。

ここで、$m$ が *有限* であると仮定します。 $q \geq 2m$ の場合、$w_q = w_{q-2m}$ と $w'_q = w'_{q-2m}$ があります。 $m \leq q \leq 2m$ の場合、$w_q = w'_{2m-q}$、$w'_q = w_{2m-q}$ があります。したがって、$q > m$ の場合、$s_q$ も $s'_q$ も分解減らされません。したがって、$W$ の $2m$ 元は、$1 \leq q \leq m-1$ および $w_m = w'_m$ の場合、$2m$ 元 $w_0 = w'_0$、$w_q$、$w'_q$ のいずれかになります。したがって、これらの $2m$ 元は別個であり、上記のように $q \leq m$ の $l(w_q) = l(w'_q) = q$ と、$W$ の元の縮小分解の *集合は、$s_q$ と $s'_q$ で構成されることがわかります。 $0 \leq q \leq m$*。 $w_m$ を除く$W$ のすべての元には、固有の縮小された分解があります。 $w_m$には2つあります。

### 3. コクセターの最初の特性群

これから、S の元は位数 2 であると仮定することを思い出してください。

#### 定義 3 {#lie-iv-s1-def-3 .statement tag=0ALV}

(W, S) は、次の条件を満たす場合、Coxeter 系であると言われます。

(C) S の s, s' について、m(s, s') が有限であるように、m(s, s') を ss' の位数とし、I を対 (s, s') の集合とする。 生成する集合 S および関係 (ss')^{m(s,s')} = 1 (s, s') の I 形群 W のプレゼンテーション¹。

(W, S) がコクセター 系であるとき、言葉の乱用によって、W はコクセター 群であるとも言います。

#### 例 1 {#lie-iv-s1-n3-exa-1 .statement tag=0ALW}

m を整数 $\geq 2$ または $\infty$ とし、W を生成元 S = {s, s'} の集合と、m が有限のとき $m = \infty$、$s^2 = {s'}^2 = (ss')^m = 1$ のとき関係 $s^2 = {s'}^2 = 1$ で定義される群とします。一方、(7) で定義される D_m の二面角群 D_m (no. 2, 例) と元 $\rho$ および $\rho'$ を考えてみましょう。 m が有限のとき、$\rho^2 = (\rho')^2 = 1$ と $(\rho\rho')^m = 1$ なので、$f(s) = \rho$ と $f(s') = \rho'$ となるような W から D_m までの一意な準同型 f が存在します。 $\rho\rho'$ は位数 m であるため、ss' 自体は位数 m であることになります。したがって、(W, S) はコクセター 系、W は位数 $2m$ の二面体群、f は同型です (提案 2)。

構造の輸送により、すべての二面体群はコクセター 群であることがわかります。

#### 例 2 {#lie-iv-s1-n3-exa-2 .statement tag=0ALX}

$\mathfrak{S}_n$ を、$n \geq 2$ と対称な次数 n の群とします。 $s_i$ を i と $i+1$ の $1 \leq i < n$ への転置とし、S = {s_1, ..., s_{n-1}} とします。 $(\mathfrak{S}_n, S)$ が Coxeter 系であることを示すことができます (§ 2, no.4、例、および § 1、例題 4)。

#### 例 3 {#lie-iv-s1-n3-exa-3 .statement tag=0ALY}

有限 Coxeter 群、cf. の分類については、第 1 章を参照してください。 4、§ 4。

#### 注意 {#lie-iv-s1-n3-rem-1 .statement tag=0ALZ}

(W, S) が Coxeter 系であると仮定します。 W から群 {1, -1} まで、すべての $s \in S$ に対して $\varepsilon(s) = -1$ によって特徴付けられる準同型 $\varepsilon$ が存在します。 $\varepsilon(w)$ を w の署名と呼びます。それは$(-1)^{l(w)}$に等しいです。したがって、公式 $\varepsilon(ww') = \varepsilon(w)\varepsilon(w')$ は $l(ww') \equiv l(w) + l(w') \mod 2$ に変換されます。

¹ これは、(W, S) には次の普遍性があることを意味します。 I の (s, s') に対して $(f(s)f(s'))^{m(s,s')} = 1$ となるように、S から G までの群 G と写像 f が与えられると、f を拡張する W から G までの準同型 g が存在します。 S 生成する W であるため、この準同型は一意です。 この定義に相当する形は次のとおりです。 Let $\overline{W}$ be a group, f a homomorphism from $\overline{W}$ to W and h a map from S to $\overline{W}$ such that $f(h(s)) = s$ and $(h(s)h(s'))^{m(s,s')} = 1$ for (s, s') in S and such that the h(s) (for $s \in S$) generate $\overline{W}$. この場合、 f は単射です (したがって、$\overline{W}$ から W までの同型です)。

#### 命題 3 {#lie-iv-s1-prop-3 .statement tag=0AM0}

(W, S) が Coxeter 系であると仮定します。次に、次の条件が満たされる場合に限り、S の 2 つの元と s' は W で共役$^2$ になります。

(I) $s_1 = s, s_q = s'$ と $s_j s_{j+1}$ が $1 \leq j < q$ に対して有限奇数位数となるような S の元の有限列 $(s_1, \ldots, s_q)$ が存在します。

S の s と s' が、$p = ss'$ が有限位数 $2n + 1$ となるようなものとします。 (9) により、$sp^{-n} = p^n s$ したがって

$$
p^n sp^{-n} = p^n p^n s - p^{-1} s = s' ss = s',
$$

そして $s'$ は s に対して共役です。

S のすべての s について、$A_s$ を $s' \in S$ 満たす (I) の集合とします。 (I) の仮説では、上記により、$1 \leq j < q$ に対して元 $s_j$ と $s_{j+1}$ は共役となるため、$A_s$ のすべての元 $s'$ は s に対して共役となります。

$f$ を S から $M = \{1, -1\}$ までの写像とし、$A_s$ では 1、$S - A_s$ では -1 とします。 S の $s'$ と $s''$ を、$s's''$ が有限の位数 m になるようにします。次に、$s'$ と $s''$ が両方とも $A_s$ にある場合、または両方とも $S - A_s$ にある場合は、$f(s') f(s'') = 1$ になります。もう 1 つのケースでは、$f(s') f(s'') = -1$ ですが、m は偶数です。したがって、すべての場合において $(f(s') f(s''))^m = 1$ となります。 (W, S) は Coxeter 系なので、S に f を誘導する W から M までの準同型 g が存在します。$s'$ を s の共役とします。 s 属するから g の核なので、$s'$ も同様になり、したがって $f(s') = g(s') = 1$、そして最後に $s' \in A_s$ になります。 Q.E.D.

### 4. コクセター 群で分解を削減

(W, S) が Coxeter 系であると仮定します。 T を S の元の W の共役の集合とします。 For any finite sequence $s = (s_1, \ldots, s_q)$ of elements of S, denote by $\Phi(s)$ the sequence $(t_1, \ldots, t_q)$ of elements of T defined by

$$
t_j = (s_1 \ldots s_{j-1}) s_j (s_1 \ldots s_{j-1})^{-1} \quad \text{for } 1 \leq j \leq q.
$$

次に$t_1 = s_1$と$s_1 \ldots s_q = t_q t_{q-1} \ldots t_1$です。任意の元 $t \in T$ については、$1 \leq j \leq q$ と $t_j = t$ のように、整数 $j$ の $n(s, t)$ 数で表します。最後に、入れます

$$
R = \{1, -1\} \times T.
$$

#### 補題 1 {#lie-iv-s1-lem-1 .statement tag=0AM1}

(i) $w \in W$ と $t \in T$ とします。 数 $(-1)^{n(s, t)}$ は、$w = s_1 \ldots s_q$ となるような S の元のすべての数列 $s = (s_1, \ldots, s_q)$ に対して同じ値 $\eta(w, t)$ を持ちます。

(ii) $w \in W$ について、$U_w$ を R からそれ自体までの写像とします。

$$
U_w(\varepsilon, t) = (\varepsilon \cdot \eta(w^{-1}, t), wtw^{-1}) \quad (\varepsilon = \pm 1, t \in T).
$$

写像 $w \mapsto U_w$ は、W の準同型から R の置換の群です。

(2) 変換を互いに結合する W の内部自己同型が存在する場合、群 W の 2 つの元 (それぞれ 2 つの部分集合) は共役であると言われることを思い出してください。

$s \in S$、定義する写像 $U_s$ の場合、$R$ からそれ自体まで、
$$
U_s(\varepsilon, t) = (\varepsilon.(-1)^{\delta_{s,t}}, st s^{-1}) \quad (\varepsilon = \pm 1, t \in T),
$$
ここで、$\delta_{s,t}$ はクロネッカー記号です。 $U_s^2 = \mathrm{Id}_R$ は明らかであり、$U_s$ は $R$ の置換であることがわかります。

$s = (s_1, \ldots, s_q)$ を $S$ の元の数列とします。 $w = s_q \ldots s_1$と$U_s = U_{s_q} \ldots U_{s_1}$を入れます。 $q$の帰納法までに、
$$
U_s(\varepsilon, t) = (\varepsilon.(-1)^{n(s,t)}, wt w^{-1}).
$$
$q = 0, 1$ についてはこれが明らかです。 $q > 1$の場合は、$s' = (s_1, \ldots, s_{q-1})$を入れて、
$$
w' = s_{q-1} \ldots s_1.
$$
帰納法の仮定を使用すると、次のようになります。
$$
\begin{align*}
U_s(\varepsilon, t) &= U_{s_q}(U_{s_q}(\varepsilon.(-1)^{n(s',t)}, w't {w'}^{-1})) \\
&= (\varepsilon.(-1)^{n(s',t)+\delta_{s_q,w't {w'}^{-1}}}, wt w^{-1}).
\end{align*}
$$
しかし、$\Phi(s) = (\Phi(s'), {w'}^{-1} s_q w')$ と $n(s, t) = n(s', t) + \delta_{w', -1} s_q w', t$、証明公式 (14)。

さて、$p = ss'$ が有限の位数 $m$ を持つような$s, s' \in S$ とします。 Let $s = (s_1, \ldots, s_{2m})$ be the sequence of elements of $S$ defined by $s_j = s$ for $j$ odd and $s_j = s'$ for $j$ even. この場合、$s_{2m} \ldots s_1 = p^{-m} = 1$ と公式 (11) は次のことを意味します。
$$
t_j = p^{j-1} s \quad \text{for } 1 \leq j \leq 2m.
$$
$p$ は位数 $m$ であるため、元 $t_1, \ldots, t_m$ は区別され、$t_{j+m} = t_j$ は $1 \leq j \leq m$ となります。 したがって、すべての $t \in T$、整数 $n(s, t)$ は 0 または 2 に等しく、(14) は $U_s = \mathrm{Id}_R$ を示します。 その他語、$(U_s U_{s'})^m = \mathrm{Id}_R$。 したがって、Coxeter 系の定義により、$R$ の置換の $W$ から群まで準同型 $w \mapsto U_w$ が存在し、$U_s$ は (13) の右辺で与えられます。 次に、$w = s_q \ldots s_1$ と補題 1 が (14) からすぐに続くように、数列 $s = (s_1, \ldots, s_q)$ ごとに $U_w = U_s$ が続きます。

#### 補題 2 {#lie-iv-s1-lem-2 .statement tag=0AM2}

*$s = (s_1, \ldots, s_q)$、$\Phi(s) = (t_1, \ldots, t_q)$、$w = s_1 \ldots s_q$とします。 $T_w$ を $\eta(w, t) = -1$ となるような $T$ の元の集合とします。この場合、$t_i$ が異なる場合に限り、$s$ は $w$ の縮小分解となり、その場合は $T_w = \{ t_1, \ldots, t_q \}$ と $\mathrm{Card}(T_w) = l(w)$ になります。*

明らかに$T_w \subset \{ t_1, \ldots, t_q \}$。 $s$ を減らすと、$\mathrm{Card}(T_w) \leq l(w)$ になります。さらに、$t_i$ が別個である場合、$t$ が属するから $\{ t_1, \ldots, t_q \}$ に該当するかどうかに応じて、$n(s, t)$ は 1 または 0 に等しくなります。 $T_w = \{ t_1, \ldots, t_q \}$ と $q = \mathrm{Card}(T_w) \leq l(w)$ が続き、これは $s$ が減少することを意味します。最後に $t_i = t_j$ が $i < j$ になったとします。これにより、$u = s_{i+1} \ldots s_{j-1}$ を使用すると、$s_i = us_j u^{-1}$ が得られます。

$$
w = s_1 \ldots s_{i-1} s_{i+1} \ldots s_{j-1} s_{j+1} \ldots s_q.
$$

これは、$s$ が $w$ の縮小分解ではないことを示しています。

#### 補題 3 {#lie-iv-s1-lem-3 .statement tag=0AM3}

*$w \in W$ と $s \in S$ を $l(sw) \leq l(w)$ となるようにします。 $w = s_1 \ldots s_q$ を含む $S$ の元の数列 $s = (s_1, \ldots, s_q)$ に対して、 $1 \leq j \leq q$ および * となるような整数 $j$ が存在します。

$$
ss_1 \ldots s_{j-1} = s_1 \ldots s_{j-1} s_j.
$$

$p$ を $w$ と $w' = sw$ の長さとします。 no. 3、$l(w') \equiv l(w) + 1$ mod の *注意* によって。 2. 仮定 $l(w') \leq l(w)$ および関係

$$
|l(w) - l(w')| \leq l(w{w'}^{-1}) = l(s) = 1
$$

従って、$l(w') = p - 1$ につながります。 選ぶ削減された分解

$$
(s'_1, \ldots, s'_{p-1})
$$

$w'$ に$s = (s, s'_1, \ldots, s'_{p-1})$ と $\Phi(s') = (t'_1, \ldots, t'_p)$ を入れます。 $s'$ が $w$ の分解であり、$t'_1 = s$ であることは明らかです。 元 $t'_1, \ldots, t'_p$ は補題 2 によって区別され、$n(s', s) = 1$ になります。 $w$ は数列 $s$ の積であるため、$n(s, s) \equiv n(s', s)$ mod があります。 2 by 補題 1、つまり $n(s, s) \neq 0$ です。従って、$s$ は、数列 $\Phi(s)$ の元 $t_j$ の 1 つに等しいため、補題となります。

#### 注意 {#lie-iv-s1-n4-rem-1 .statement tag=0AM4}

補題 2 で定義された集合 $T_w$ は、形 $w''s{w''}^{-1}$ 対応するの元から$w = w''sw'$ と $l(w') + l(w'') + 1 = l(w)$ のようなトリプル $(w', w'', s) \in W \times W \times S$ で構成されます。

### 5. 交換条件

「交換条件」とは、$(W, S)$に関する以下の主張です。

**(E)** *$w \in W$ と $s \in S$ を $l(sw) \leq l(w)$ となるようにします。 $w$ の縮小された分解 $(s_1, \ldots, s_q)$ に対して、$1 \leq j \leq q$ および* となるような整数 $j$ が存在します。

$$
ss_1 \ldots s_{j-1} = s_1 \ldots s_{j-1} s_j.
$$

この数では、$(W, S)$が(E)を満たすと仮定します。 補題 3 までに、$(W, S)$ が Coxeter 系であれば、これは当てはまります。従って、この数の結果は Coxeter 系に当てはまります。

#### 命題 4 {#lie-iv-s1-prop-4 .statement tag=0AM5}

*$s \in S, w \in W$ と $s = (s_1, \ldots, s_q)$ を $w$ の縮小分解とします。その場合、次のいずれかが成立する必要があります:*

a) $l(sw) = l(w) + 1$ と $(s, s_1, \ldots, s_q)$ は、$sw$ の縮小分解です。

b) $l(sw) = l(w) - 1$ そして、$1 \leq j \leq q$、$(s_1, \ldots, s_{j-1}, s_{j+1}, \ldots, s_q)$ が $sw$ の縮小分解であり、$(s, s_1, \ldots, s_{j-1}, s_{j+1}, \ldots, s_q)$ が $w$ の縮小分解であるような整数 $j$ が存在します。

$w' = sw$を入れてください。 no. 1 の公式 (3) までに、
$$
|l(w) - l(w')| \leq l(s) = 1.
$$
次の 2 つのケースを区別します。

a) $l(w') > l(w)$。次に、$l(w') = q + 1$ と $w' = ss_1 \ldots s_q$ なので、
$$
(s, s_1, \ldots, s_q)
$$
$w'$ の削減された分解です。

b) $l(w') \leq l(w)$。 (E) により、$1 \leq j \leq q$ と (16) を満たすような整数 $j$ が存在します。次に $w = ss_1 \ldots s_{j-1} s_{j+1} \ldots s_q$ 以降
$$
w' = s_1 \ldots s_{j-1} s_{j+1} \ldots s_q.
$$
$q - 1 \leq l(w') \leq q$ なので、$l(w') = q - 1$ となり、$(s_1, \ldots, s_{j-1}, s_{j+1}, \ldots, s_q)$ は $w'$ の分解を減じたものになります。

#### 補題 4 {#lie-iv-s1-lem-4 .statement tag=0AM6}

$w \in W$ に長さ $q \geq 1$ を持たせ、D を $w$ の分解を減じた集合とし、F を D から集合 E までの写像とする。D の元 $s = (s_1, \ldots, s_q); s' = (s'_1, \ldots, s'_q)$ の場合、$F(s) = F(s')$ と仮定します。 満たす次の仮説のいずれか:

a) $s_1 = s'_1$ または $s_q = s'_q$。
b) S には、$j$ 奇数と $k$ 偶数に対して $s_j = s'_k = s$ と $s_k = s'_j = s'$ となる s と $s'$ が存在します。

この場合、F は一定になります。

A) $s, s' \in D$ として、$t = (s'_1, s_1, \ldots, s_{q-1})$ を置きます。 $F(s) \neq F(s')$ の場合、$t \in D$ と $F(t) \neq F(s)$ であることを示します。 確かに、$w = s'_1 \ldots s'_q$、したがって $s'_1 w = s'_2 \ldots s'_q$ は長さ $< q$ です。 提案 4 により、D に対して $1 \leq j \leq q$ および数列 $u = (s'_1, s_1, \ldots, s_{j-1}, s_{j+1}, \ldots, s_q)$ 属するとなるような整数 $j$ が存在します。 条件までに$F(u) = F(s')$があります a); $j \neq q$ の場合、同じ理由で $F(s) = F(u)$ があり、したがって仮定とは反対に $F(s) = F(s')$ になります。 したがって、$j = q$、したがって、$t = u \in D$、$F(t) = F(s') \neq F(s)$ となります。

B) s と $s'$ 属するを D にします。S の q 元の $0 \leq j \leq q + 1$ 定義する数列 $s_j$ を含む任意の整数 $j$ について、次のようになります。
$$
s_0 = (s'_1, \ldots, s'_q)
$$
$$
s_1 = (s_1, \ldots, s_q)
$$
$$
s_{q+1-k} = (s_1, s'_1, \ldots, s_1, s'_1, s_1, s_2, \ldots, s_k)
$$
$q - k$ 偶数と $0 \leq k \leq q$
$$
s_{q+1-k} = (s'_1, s_1, \ldots, s_1, s'_1, s_1, s_2, \ldots, s_k)
$$
$q - k$ 奇数と $0 \leq k \leq q$ の場合。

(H_j) 主張 「s_j \in D, s_{j+1} \in D \text{ and } F(s_j) \neq F(s_{j+1})」 で表します。 A) により、(H_j) \implies (H_{j+1}) は $0 \leq j < q$ に対して、(H_q) は条件 b) によって満たされません。従って、(H_0)は満たされません。 $s_0 = s'$ と $s_1 = s$ なので、$F(s) = F(s')$ になります。

#### 命題 5 {#lie-iv-s1-prop-5 .statement tag=0AM7}

*M をモノイド (単位元 1) および f 写像として S から M に変換します。S の s, s' \in について、m(s, s') を ss' の位数とし、次のようにします*

$$
a(s, s') = \begin{cases}
(f(s)f(s'))^l & \text{if } m(s, s') = 2l, l \text{ finite} \\
(f(s)f(s'))^lf(s) & \text{if } m(s, s') = 2l + 1, l \text{ finite} \\
1 & \text{if } m(s, s') = \infty.
\end{cases}
$$

* $s \neq s'$ が S にあるときに常に $a(s, s') = a(s', s)$ が存在すると、W から M までに次のような写像 g が存在します*
$$
g(w) = f(s_1) \ldots f(s_q)
$$
*すべての $w \in W$ と、w の削減された分解 $(s_1, \ldots, s_q)$ に対して。*

任意の $w \in W$ について、$D_w$ を w の分解と $D_w$ から M に減じた $F_w$ 写像の集合とします。
$$
F_w(s_1, \ldots, s_q) = f(s_1) \ldots f(s_q).
$$
w の長さ上の帰納法によって $F_w$ が定数であることを証明し、提案 5 を確立します。 ケース $l(w) = 0, 1$ は自明なので、$q \geq 2$ と主張が $l(w) < q$ を使用して元について証明されると仮定します。 w を長さ q と $s, s' \in D_w$ とする。 補題 4 により、その補題の a) と b) の場合に $F_w(s) = F_w(s')$ であることを証明すれば十分です。

a) 公式
$$
F_w(s_1, \ldots, s_q) = f(s_1)F_{w''}(s_2, \ldots, s_q) = F_{w'}(s_1, \ldots, s_{q-1})f(s_q)
$$
$w' = s_1 \ldots s_{q-1}$、$w'' = s_2 \ldots s_q$、帰納法の仮定は、$s_1 = s'_1$ または $s_q = s'_q$ の場合、$F_w(s) = F_w(s')$ であることを示します。

b) S の 2 つの元と s' が存在し、j が奇数、k が偶数に対して $s_j = s'_k = s$ と $s_k = s'_j = s'$ が存在すると仮定します。 $s \neq s'$の場合を扱うだけで十分です。 数列 s と s' は、s と s' によって生成される二面体群内の w の 2 つの異なる還元分解です。 no. 2 の *注意* により、ss の位数 m は必然的に有限となり、その注意の記法では、$s = s_m$ と $s' = s'_m$ になります。従って、$F_w(s) = a(s, s')$ と $F_w(s') = a(s', s)$ が続きます。
$$
F_w(s) = F_w(s').
$$

### 6. コクセターの特徴付け群

#### 定理 1 {#lie-iv-s1-thm-1 .statement tag=0AM8}

(W, S) は、no. 5 の交換条件 (E) を満たす場合に限り、Coxeter 系です。

Lemma 3 of no. 4 shows that any Coxeter system satisfies (E).

逆に、(E)が満たされるとする。 G を S から G までの群および f 写像とし、s および $s'$ 属するから S および $ss'$ が有限位数 m であるときはいつでも $(f(s)f(s'))^m = 1$ とします。提案 5 により、W から G までの写像 g が存在します。
$$
g(w) = f(s_1) \ldots f(s_q)
$$
$w = s_1 \ldots s_q$ が長さのときはいつでも q. (W, S) がコクセター 系であることを証明するには、g が公式の帰結である準同型であることを証明すれば十分です。
$$
g(sw) = f(s)g(w) \quad \text{for } s \in S, w \in W
$$
S 生成する W 以降。no. 5 の提案 4 により、2 つのケースのみが可能です。

a) $l(sw) = l(w) + 1$: $(s_1, \ldots, s_q)$ が $w$ の縮小分解である場合、$(s, s_1, \ldots, s_q)$ は $sw$ の縮小分解であるため、(21)。

b) $l(sw) = l(w) - 1$: $w' = sw$ を入れます。次に$w = sw'$と$l(sw') = l(w') + 1$。 a) により、$(f(s))^2 = 1$ から $g(w) = f(s)g(sw)$、したがって $f(s)g(w) = g(sw)$ になります。

### 7. 分割のご家族

(W, S) が Coxeter 系であると仮定します。任意の $s \in S$ について、$P_s$ を $l(sw) > l(w)$ となるような W の元 $w$ の集合とします。次のようなプロパティがあります。

(A) $\bigcap_{s \in S} P_s = \{1\}$。

確かに、$w \neq 1$ を W とし、$(s_1, \ldots, s_q)$ を $w$ の縮小分解とします。すると、$q \geq 1$と$(s_2, \ldots, s_q)$は$s_2w$の分解を減じたものなので、$l(w) = q$と$l(s_1w) = q - 1$になります。したがって、$w \notin P_{s_1}$です。

(B) *S の任意の s については、W の集合 $P_s$ および $sP_s$ 形分割*

$w \in W$と$s \in S$としましょう。 no. 5 の提案 4 により、2 つのケースを区別する必要があります。

a) $l(sw) = l(w) + 1$: 次に $w \in P_s$。
b) $l(sw) = l(w) - 1$: $w' = sw$ を入れて $w = sw'$;それから
$$
l(w') < l(sw')
$$
したがって$w' \in P_s$、つまり$w \in sP_s$です。

(C) *s, s' を S に、w を W にします。$w \in P_s$ と $ws' \in P_s$ の場合、$sw = ws'$。*

$q$を$w$の長さとします。 $w \in P_s$ からは、$l(sw) = q + 1$ になります。そして$ws' \in P_s$からは$l(sws') = l(ws') - 1 \leq q$になります。 $l(sws') = l(sw) \pm 1$ 以来、ついに$l(ws') = q + 1$ と $l(sws') = q$ ができました。

$(s_1, \ldots, s_q)$ を $w$ と $s_{q+1} = s'$ の縮小分解とします。この場合、$(s_1, \ldots, s_q, s_{q+1})$ は、長さ $q + 1$ の元 $ws'$ を減じた分解です。 条件の交換により、次のような整数 $j$ と $1 \leq j \leq q + 1$ が存在します。
$$
ss_1 \ldots s_{j-1} = s_1 \ldots s_j.
$$
(22)
$1 \leq j \leq q$ の場合、$sw = s_1 \ldots s_{j-1} s_{j+1} \ldots s_q$ は公式 $l(sw) = q + 1$ と矛盾します。したがって、$j = q + 1$ と公式 (22) は $sw = ws'$ と書くことができます。

逆に、次の結果が得られます。

#### 命題 6 {#lie-iv-s1-prop-6 .statement tag=0AM9}

*$(P_s)_{s \in S}$ ** $W$ *満たす* (C) * と次の条件* の部分集合の家族としましょう:

(A') $1 \in P_s$ *全員に* $s \in S$。
(B') *集合* $P_s$ *と* $sP_s$ *すべて* $s \in S$ で互いに素です。

*すると*、$(W, S)$ *はCoxeter 系であり、* $P_s$ *は元* $w$ *の* $W$ *そのような* $l(sw) > l(w)$。

$s \in S$と$w \in W$としましょう。次の 2 つの可能性があります。

a) $w \notin P_s$。 $(s_1, \ldots, s_q)$ を $w$ の縮小分解とします。
$$
w_j = s_1 \ldots s_j
$$
$1 \leq j \leq q$の場合。 $w_0 = 1$も入れてください。 (A')による$w_0 \in P_s$と$w = w_q$が$P_s$にないので、$w_{j-1} \in P_s$と$w_j = w_{j-1} s_j$が属するから$P_s$にならないように、$1 \leq j \leq q$を持つ整数$j$が存在します。 (C)により、
$$
sw_{j-1} = w_{j-1} s_j.
$$
したがって、私たちは公式を証明しました
$$
ss_1 \ldots s_{j-1} = s_1 \ldots s_{j-1} s_j
$$
これは、$sw = s_1 \ldots s_{j-1} s_{j+1} \ldots s_q$ と $l(sw) < l(w)$ を意味します。

b) $w \in P_s$: $w' = sw$ を入れて、(B') によって $w' \notin P_s$ になります。 a) により、$l(sw') < l(w')$、つまり $l(w) < l(sw)$ が得られます。

a) と b) を比較すると、$P_s$ は $l(sw) > l(w)$ となるような $w \in W$ で構成されていることがわかります。 a) で見たように、ここから交換条件が続き、したがって、$(W, S)$ は Coxeter 系 (no. 6 の Th. 1) です。

### 8. コクセターの部分群群

この数では、$(W, S)$がコクセター系であると仮定します。 $S$ の部分集合 $X$ については、$X$ によって生成された $W$ の $W_X$ 部分群で表します。

#### 命題 7 {#lie-iv-s1-prop-7 .statement tag=0AMA}

※$w$を$W$に入れます。 $S$ の部分集合 $S_w$ は、$w$ の分解 $(s_1, \ldots, s_q)$ を減じたものに対して $\{s_1, \ldots, s_q\} = S_w$ となるように存在します。*

$M$ で $S$ の部分集合のモノイドからなるを合成法則 $(A, B) \mapsto A \cup B$ で表します。 $M$の単位元は$\varnothing$です。 $s \in S$に$f(s) = \{s\}$を入れます。 no. 5の提案5を$M$と$f$に適用します。 $m(s, s')$ が有限である場合、$S$ の $s, s'$ に対して $a(s, s') = \{s, s'\}$ が存在するため、$W$ から $M$ まで写像 $g : w \mapsto S_w$ が存在し、$g(w) = f(s_1) \cup \cdots \cup f(s_q)$、つまり任意の$S_w = \{s_1, \ldots, s_q\}$ が存在します。 $w \in W$ および $w$ のうち減らされた分解 $(s_1, \ldots, s_q)$。

#### 系 1 {#lie-iv-s1-prop-7-cor-1 .statement tag=0AMB}

*$S$の部分集合 $X$、$W$の部分群 $W_X$は、$S_w \subset X$となるように、$W$の元$w$で構成されます。

$S$ に $s_1, \ldots, s_q$ がある $w = s_1 \ldots s_q$ の場合、$w^{-1} = s_q \ldots s_1$;したがって

$$
S_{w^{-1}} = S_w.
$$

no. 5 の提案 4 は、$s \in S$ と $w' \in W$ が $S_{sw'} \subset \{s\} \cup S_{w'}$ であることを示しており、これは公式を意味します

$$
S_{ww'} \subset S_w \cup S_{w'}
$$

$w$ の長さに帰納法によって。 (23) と (24) により、$w \in W$ の集合 $U$ は、$S_w \subset X$ が $W$ の部分群になります。 $X \subset U \subset W_X$ があるため、$U = W_X$ になります。

#### 系 2 {#lie-iv-s1-prop-7-cor-2 .statement tag=0AMC}

※$S$の部分集合$X$の場合、$W_X \cap S = X$がございます。

これはコルからの続きです。 $S$ の $s$ には 1 と公式 $S_s = \{s\}$ が入ります。

#### 系 3 {#lie-iv-s1-prop-7-cor-3 .statement tag=0AMD}

*集合 $S$ は、$W$ の最小生成する集合です。

$X \subset S$ 生成する $W$ の場合、Cor により $W = W_X$、したがって $X = S \cap W_X = S$ になります。 2.*

#### 系 4 {#lie-iv-s1-prop-7-cor-4 .statement tag=0AME}

*$S$の任意の部分集合$X$と$W_X$の任意の$w$について、$W_X$の生成する集合$X$に関して$w$の長さは$l_S(w)$に等しい。

$(s_1, \ldots, s_q)$ を $w$ の分解を $W$ の元として考慮したものとします。 $1 \leq j \leq q$ (Cor. 1) には $w = s_1 \ldots s_q$ と $s_j \in X$ があります。さらに、$w$ できないは、$q' < q$ の積 $X \subset S$ の元から $q = l_S(w)$ の定義になります。*

#### 定理 2 {#lie-iv-s1-thm-2 .statement tag=0AMF}

(i) *$S$ の任意の部分集合 $X$ について、対 $(W_X, X)$ はコクセター 系です。*

(ii) $(X_i)_{i \in I}$ を $S$ の部分集合の家族とする。 $X = \bigcap_{i \in I} X_i$の場合は、$W_X = \bigcap_{i \in I} W_{X_i}$。

(iii) $X$ と $X'$ を $S$ の 2 つの部分集合とします。次に、$X \subset X'$ (それぞれ $X = X'$) の場合に限り、$W_X \subset W_{X'}$ (それぞれ $W_X = W_{X'}$) になります。

$X$ のすべての元は、位数 2 および $X$ 生成する $W_X$ です。 $x \in X$ と $w \in W_X$ を $l_X(xw) \leq l_X(w) = q$ にします。コル著提案 7 の 4、
$$
l_S(xw) \leq l_S(w) = q.
$$
$x_1, \ldots, x_q$ を $X$ の元とし、$w = x_1 \ldots x_q$ とします。 $(W, S)$ は交換条件 (no. 6 の 1 番目) を満たすので、$1 \leq j \leq q$ と $xx_1 \ldots x_{j-1} = x_1 \ldots x_{j-1} x_j$ となる整数 $j$ が存在します。したがって、$(W_X, X)$ は交換条件を満たし、したがって Coxeter 系 (no. 6 の Th. 1) です。これは(i)を証明します。

主張 (ii) と (iii) は Cor の直後に続きます。提案 7 の 1。

### 9. コクセター 行列とコクセター グラフ

#### 定義 4 {#lie-iv-s1-def-4 .statement tag=0AMG}

$I$ を集合とします。 型 $I$ の Coxeter 行列は対称平方行列 $M = (m_{ij})_{i,j \in I}$ であり、そのエントリは整数または $+\infty$ 満たす関係
$$
m_{ii} = 1 \quad \text{for all } i \in I; \tag{25}
$$
$$
m_{ij} \geq 2 \quad \text{for } i, j \in I \text{ with } i \neq j. \tag{26}
$$

型 $I$ の Coxeter グラフは、(言葉の乱用により) 集合の頂点として $I$ を持ち、このグラフの辺の集合から写像 $f$ を持つグラフ $\Gamma^3$ の対からなるです。 $+\infty$ の集合からなると整数 $\geq 3$ の集合。 $\Gamma$ は、Coxeter グラフ $(\Gamma, f)$ の基礎となるグラフと呼ばれます。

Coxeter グラフ $(\Gamma, f)$ は、次のように型 $I$ の Coxeter 行列 $M$ に関連付けられます。

グラフ $\Gamma$ には、$I$ の集合と集合対 $\{i, j\}$ の元 $I$ の$m_{ij} \geq 3$ と写像の辺の集合があります。 $f$ は、$M$ のエッジ $\{i, j\}$ 対応する元 $m_{ij}$ に関連付けられます。

It is clear that this gives rise to a bijection between the set of Coxeter matrices of type $I$ and the set of Coxeter graphs of type $I$.

読者が私たちの議論を理解しやすくするために、私たちは多くの場合、型 $I$ の Coxeter グラフをその基礎となるグラフを表すために使用される図式で表し、各エッジ $\{i, j\}$ 数 $f(\{i, j\})$ の横または上に書き込みます。通常、これらの数が 3 に等しい場合は省略されます。

3 定義およびここで使用されるグラフのプロパティについては、付録を参照してください。

If (W, S) is a Coxeter system, the matrix $M = (m(s, s'))_{s, s' \in S}$, where $m(s, s')$ is the order of $ss'$, is a Coxeter matrix of type S which is called the Coxeter matrix of (W, S): indeed, $m(s, s) = 1$ since $s^2 = 1$ for all $s \in S$, and $m(s, s') = m(s', s) \geqslant 2$ if $s \neq s'$ since $ss' = (s's)^{-1}$ is then $\neq 1$. M に関連付けられた Coxeter グラフ $(\Gamma, f)$ を (W, S) の Coxeter グラフと呼びます。 $\Gamma$ の 2 つの頂点 $s$ と $s'$ は、$s$ と $s'$ が交換しない場合にのみ *結合* されることに注意してください。 たとえば、位数 $2m$ の二面体群のコクセター 行列は $\begin{pmatrix} 1 & m \\ m & 1 \end{pmatrix}$ で、そのコクセター グラフは次のように表されます。

$$
\circ \overset{m}{\text{---}} \circ
$$

$m \geqslant 3$ (または

$$
\circ \text{---} \circ
$$

$m = 3$の場合)そして、

$$
\circ \qquad \circ
$$

$m = 2$のとき。 \* 対称群 $\mathfrak{S}_n$ の Coxeter グラフは次のように表されます。

$$
\circ \text{---} \circ \text{---} \circ \cdots \circ \text{---} \circ
$$

($n - 1$ 頂点。) \*

後で (第 V, § 4 章) で、逆に、どの Coxeter 行列も Coxeter 系の行列であることを示します。

コクセター 系 (W, S) は、そのコクセター グラフの基礎となるグラフが *接続* (付録, no. 2) で *空ではない*場合、*既約*であると言われます。同様に、S は空ではなく、S' のすべての元が S'' のすべての元と交換するような、S の 2 つの異なる部分集合 S' および S'' への S の分割は存在しません。より一般的には、$(\Gamma_i)_{i \in I}$ を$\Gamma$ (付録、no. 2) の接続された成分のファミリーとし、$S_i$ を$\Gamma_i$ の頂点の集合とします。 $W_i = W_{S_i}$ を、$S_i$ (cf. no. 8) によって生成された W の部分群とします。そして、$(W_i, S_i)$ は、(W, S) の *既約成分* と呼ばれる既約 Coxeter 系 (no. 8, Th. 2) です。さらに、群 W は、$i \in I$ に対する部分群 $W_i$ の *制限付き直接積*[^1] です。実際、これは次のより一般的な命題から導き出されます。

#### 命題 8 {#lie-iv-s1-prop-8 .statement tag=0AMH}

$(S_i)_{i \in I}$ を $S$ の分割とし、$i \neq j$ の場合、$S_i$ のすべての元が $S_j$ のすべての元と交換するようにします。すべての $i \in I$ について、$W_i$ を $S_i$ によって生成された部分群とします。次に、$W$ は、家族 $(W_i)_{i \in I}$ の制限された直接の積です。

$j \neq i$ の $W_j$ の和集合によって生成されたすべての $i \in I$ 部分群 $W'_i$ も $S'_i = \bigcup_{j \neq i} S_j$ によって生成されることは明らかです。したがって、
$$
W_i \cap W'_i = W_\varnothing = \{1\}
$$
Th 著no. 8の2。 $W$は$W_i$の和集合から生成されるので、命題が証明されます。

### 練習問題 {#lie-iv-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。

[^1]: A group G is the *restricted direct product* of a family $(G_i)_{i \in I}$ of subgroups if, for any finite subset J of I, the subgroup $G_J$ of G generated by the $G_i$ for $i \in J$ is the direct product of the $G_i$ for $i \in J$ and if G is the union of the $G_J$. 同様に、$G_i$ のすべての元は、$i \neq j$ については $G_j$ のすべての元と交換でき、G のすべての元は、有限個を除くすべての$g_i \in G_i$ および $g_i = 1$ と積 $\prod_{i \in I} g_i$ として一意に書くことができます。 添字 $i$。 この最後の条件は、$G_i$の和集合によってGが生成され、$i \notin J$のような$i \in I$とIのすべての有限部分集合Jに対して$G_i \cap G_J = \{1\}$が生成されるというと同等です。
