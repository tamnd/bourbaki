---
book: ac
book_title: Commutative Algebra
chapter: III
chapter_title: GRADUATIONS. FILTRATIONS AND TOPOLOGIES
section: 4
section_title: Lifting in complete rings
lang: ja
source: ac-i-vii
book_pages: 209-226, 255-258
pdf_pages: 0229-0246, 0275-0278
extraction: ocr
subsections:
    - "no": 1
      title: STRONGLY RELATIVELY PRIME POLYNOMIALS
      page: 209
      pdf_page: 229
    - "no": 2
      title: RESTRICTED FORMAL POWER SERIES
      page: 212
      pdf_page: 232
    - "no": 3
      title: HENSEL'S LEMMA
      page: 215
      pdf_page: 235
    - "no": 4
      title: COMPOSITION OF SYSTEMS OF FORMAL POWER SERIES
      page: 218
      pdf_page: 238
    - "no": 5
      title: SYSTEMS OF EQUATIONS IN COMPLETE RINGS
      page: 220
      pdf_page: 240
    - "no": 6
      title: APPLICATION TO DECOMPOSITIONS OF RINGS
      page: 225
      pdf_page: 245
statements: 23
exercises: 8
content_sha256: 10c7e335800619c1624d2626d32316386bffd421eb1e6c78ccfb356891c60701
translated_from: content/en/ac/III/04_s4_lifting_in_complete_rings.md
translation_method: google
source_content_sha256: e207aa232d5bd052ada28a852533dc7566c32021e210764a8b52a3fbf49d5170
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: d0e2635d55a547a48599ed9906cda4f116d18db2bd3a646a26da85d04767c9be
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 4. 吊り上げ完了環

### 1. 強相対素多項式

$R$ を可換環とします。 $R$ の 2 つの元 $x, y$ は、主イデアル $Rx$ と $Ry$ が相対的に素である場合、*強い相対素* と呼ばれ、他の語 (章 II, § 1, no. 2) が $R x + R y = R$ の場合、*強い相対素*と呼ばれます。 $ax + by = 1$ となるような $R$ の 2 つの元 $a, b$ が存在すると言うのと同じことになります。

#### 補題 1 (「ユークリッドの補題」) {#ac-iii-s4-lem-1 .statement tag=04HS}

*$x, y$を、$R$の2つの強く相対的に素な元とする。 $z \in R$ が $x$ 割る $yz$ である場合、$x$ 割る $z$。*

$1 = ax + by$なら$z = x(az) + (yz)b$。

$x$ と $y$ が $R$ において強く相対的に素である場合、
$$
R_{xy} = (Rx) \cap (Ry)
$$
(章 II, § 1, no. 2, 命題 5); $R$ が整域の場合、2 つの強く互いに素な元は、その積 (*代数*, 章 VI, § 1, no. 8) と等しい *lcm* を持ち、したがって、*代数*, 章という意味で *相対的に素* になります。 VI, § 1, no. 12。逆に、$R$ が主イデアル整域である場合、ベズーの恒等式 (*代数*, 章 VII, § 1, no. 2, 定理 1) からわかるように、2 つの互いに素な元も強く相対素です。

多項式環の場合、次の結果が得られます。

#### 命題 1 {#ac-iii-s4-prop-1 .statement tag=04HT}

*$\mathbf{A}$ を可換環、$P$ および $P'$ を $\mathbf{A}[X]$ の 2 つの強く相対的に素な多項式とします。 $P$ がモニックであり、次数 $s$ であると仮定します。すると、$\mathbf{A}[X]$ のすべての多項式 $T$ は、形* で一意に記述できます。
$$
T = PQ + P'Q'
$$
*ここで、$Q \in \mathbf{A}[X]$、$Q' \in \mathbf{A}[X]$、$\deg(Q') < s$。
さらに $\deg(T) \leq t$ と $\deg(P') \leq t - s$ なら、$\deg(Q) \leq t - s$*。

$P$ はモニックであるため、$\mathbf{A}[X]$ のすべての多項式 $R \neq 0$ に対して $PR \neq 0$、この場合は $\deg(PR) = s + \deg(R)$ になります。

$T$ を $\mathbf{A}[X]$ の任意の多項式とします。 $P$ と $P'$ によって生成される理想は $\mathbf{A}[X]$ の全体であるため、次のような多項式 $Q_1$ と $Q'$ が存在します。
$$
T = PQ_1 + P'_1Q'_1;
$$
$P$ は次数 $s$ のモニックであるため、ユークリッド除算 (*代数*, 章 IV, § 1, no. 5) は、$\deg(Q') < s$ に対して $Q'_1 = PQ'' + Q'$ となる 2 つの多項式 $Q', Q''$ が存在することを示します。それから私たちはそれを推測します
$$
T = PQ_1 + P'(PQ'' + Q') = PQ + P'Q'
$$
$Q = Q_1 + P'Q''$ です。 公式 (1) の一意性を示すには、関係を証明すれば十分です
$$
0 = PQ + P'Q', \quad \deg(Q') < s
$$
$Q = Q' = 0$を暗示します。ここで、(2) が成り立つ場合、$P$ 割る $-PQ = P'Q'$、そして $P$ と

P' は強く相対的に素であり、P 割る Q' 補題 1 です。 Q' ≠ 0 の場合、Q' = PS, よってとなる多項式 S ≠ 0 が存在します。

$$
\deg(Q') = s + \deg(S) \geq s,
$$

それは矛盾です。最初の注意により、Q' = 0、よって PQ = 0、そして最終的に Q = 0 であることが結論するわかります。

最後に、$\deg(T) \leq t$ と $\deg(P') \leq t - s$ を仮定します。 形 (1) の多項式 T を使用すると、

$$
\deg(P'Q') \leq \deg(P') + \deg(Q') < s + \deg(P') \leq t
$$

したがって

$$
s + \deg(Q) = \deg(PQ) = \deg(T - P'Q') \leq t
$$

よって $\deg(Q) \leq t - s$。

#### 例 {#ac-iii-s4-n1-exa-1 .statement tag=04HU}

多項式 $P \in \mathbf{A}[X]$ が $X - a$ (ここで $a \in \mathbf{A}$) に対して強相対素であるためには、$P(a)$ が $\mathbf{A}$ で *反転可能* であることが必要かつ十分です。なぜなら、P と $X - a$ が強い相対素数である場合、命題 1 から、$c \in \mathbf{A}$ と、$cP + (X - a)Q = 1$、よって $cP(a) = 1$、および $P(a)$ が可逆であるような多項式 $Q \in \mathbf{A}[X]$ が存在することがわかります。逆にユークリッド除算すると

$$
P = (X - a)R + P(a)
$$

そして、$b \in \mathbf{A}$ が $P(a) = b^{-1}$ の場合、$1 = bP - b(X - a)R$ と推定されます。これは、P と $X - a$ が強く相対的に素であることを示しています。

$\mathbf{A}$ と $\mathbf{B}$ を 2 つの可換環と $f : \mathbf{A} \to \mathbf{B}$ 環準同型とします。 $P = \sum_{i \geq 0} a_i X^i$ が $\mathbf{A}[[X]]$ の正式な冪系列である場合、$\bar{f}(P)$ は $\mathbf{B}[[X]]$ の正式な冪系列 $\sum_{i \geq 0} f(a_i) X^i$ を表します。 P が多項式の場合、$\bar{f}(P)$ も多項式であり、さらに P がモニックである場合、$\bar{f}(P)$ は P と同じ次数のモニックです。 最後に、$P \mapsto \bar{f}(P)$ は明らかに $\mathbf{A}[[X]]$ から $\mathbf{B}[[X]]$ の準同型であり、これは拡大する $f$ と写像 X から X まで。 *記法は、この段落の残りの部分では常にこの意味で使用されます。*

#### 命題 2 {#ac-iii-s4-prop-2 .statement tag=04HV}

*$\mathbf{A}$と$\mathbf{B}$を、$\mathbf{A}$から$\mathbf{B}$までの2つの可換環、$f$準同型、および$\mathbf{A}[X]$の2つの多項式$P, P'$とします。 $\mathbf{A}[X]$ で $P$ と $P'$ が強い相対素数である場合、$\mathbf{B}[X]$ では $\bar{f}(P)$ と $\bar{f}(P')$ が強い相対素数です。 逆は、全射である場合、その核が $\mathbf{A}$ のヤコブソン根基に含まれる場合、および $P$ が単音である場合に真です。*

P と P' が強く相対的に素であると仮定します。この場合、$\mathbf{A}[X]$ には$PQ + P'Q' = 1$ となる多項式 Q、Q' が存在します。私たちはそれを推測します

$$
\bar{f}(P)\bar{f}(Q) + \bar{f}(P')\bar{f}(Q') = 1,
$$

よって最初の主張。 2 番目を表示するには、a を $f$ の核とします。

$E = A[X]$ と $F$ を、$P$ と $P'$ によって生成された $E$ の理想とします。 $f$ は全射、$\bar{f}(P)$ モニックであるため、命題 1 は、すべての多項式 $T \in A[X]$ に対して、$A[X]$ に 2 つの多項式 $Q, Q'$ が存在することを示します。
$$
\bar{f}(T) = \bar{f}(P) \bar{f}(Q) + \bar{f}(P') \bar{f}(Q'),
$$
よって関係 $E = F + aE$。さて、$E/F$ は、すべての多項式が合同 mod であるため、有限生成された $A$ 加群です。 $P$ は次数 $< \deg(P)$ の多項式に変換され、$P$ はモニックです。 $E/F = a(E/F)$と$a$は$A$のヤコブソン根基に含まれているため、中山の補題は$E/F = 0$（代数、章、VIII, § 6, no. 3、系2から命題 6 )、これは、$P$ と $P'$ が強く相対的に素であることを意味します。

### 2. 限定されたフォーマル冪系列

#### 定義 1 {#ac-iii-s4-def-1 .statement tag=04HW}

可換トポロジー 環 $A$ は、理想 $\mathfrak{o} \subset A$ の近傍 $\mathfrak{o}$ からなるの基本系 $\mathscr{B}$ が存在する場合、線形トポロジー化されていると言われます (そしてその位相は線形であると言われます)。

このような環では、理想 $3 \in \mathscr{B}$ が開いていて閉じていることに注意してください (一般位相、章 111、§ 2, no. 1、系から命題 4 )。すべての $3 \in \mathscr{B}$ に対して、商トポロジカル環 $A/\mathfrak{J}$ は離散的になります。 $8 \in \mathscr{B}$、$8' \in \mathscr{B}$、$\mathfrak{J}' \subset 8$ については、させてください
$$
h_{\mathfrak{J}\mathfrak{J}'} : A/\mathfrak{J}' \to A/\mathfrak{J}
$$
標準写像になります。私たちは (一般位相、章 III, § 7, no. 3)、$(A/\mathfrak{J}, h_{\mathfrak{J}\mathfrak{J}'})$ が離散環 ($\supset$ によって順序付けされ、方向付けされたインデックス付け集合 $\mathscr{B}$ に対して) の逆系であることを知っています。 極限は、完全なハウスドルフ線形トポロジー化された環 $\tilde{A}$ です。さらに (前述の命題 2 )、厳密な射 $i : A \to \tilde{A}$ が定義されており、その核は $A$ の $\{0\}$ の閉包であり、像は $\tilde{A}$ のどこでも密であるため、$\tilde{A}$ は次のようになります。ハウスドルフによる$A$の完成と標準的に識別されます。

#### 定義 2 {#ac-iii-s4-def-2 .statement tag=04HX}

可換位相環 $A$ が与えられると、形式的冪系列
$$
T = \sum_{(n_i)} c_{n_1 n_2 \ldots n_p} X_1^{n_1} X_2^{n_2} \ldots X_p^{n_p}
$$
環 $A[[X_1, \ldots, X_p]]$ は、$A$ の 0 のすべての近傍 $V$ に対して、所属 ～ $V$ ではなく、係数 $c_{n_1 n_2 \ldots n_p}$ の有限の数しか存在しない場合、制限付きと呼ばれます。 語、ファミリー $(c_{n_1 n_2 \ldots n_p})$ は、$\mathbf{N}^p$ の有限部分集合の補数のフィルターに関して、$A$ で 0 になる傾向があります。

$A$ が線形トポロジー化されている場合、$A[[X_1, \ldots, X_p]]$ の $A[[X_1, \ldots, X_p]]$ 形部分環の制限された形式冪系列は、$A\{X_1, \ldots, X_p\}$ で示されます。
$$
T = \sum_{(n_i)} c_{n_1 \ldots n_p} X_1^{n_1} \ldots X_p^{n_p}, \quad T' = \sum_{(n_i)} c'_{n_1 \ldots n_p} X_1^{n_1} \ldots X_p^{n_p}
$$
$A$ の理想である $A$ に 0 の 2 つの制限された正式な冪系列と $\mathfrak{J}$ 近傍がある場合、それぞれに $c_{n_1 \ldots n_p} \in \mathfrak{z}$ と $c'_{n_1 \ldots n_p} \in \mathfrak{g}$ が成り立つような整数 $m$ が存在します。 系 $(n_1, \ldots, n_p)$ は、少なくとも 1 つの添字 $k$ に対して $n_k \geq m$ となる。今、もし

$$
T'' = TT' = \sum_{(n_i)} c''_{n_1 \ldots n_p} X_1^{n_1} \ldots X_p^{n_p},
$$

次に、すべての系 $(r_k), (s_k)$ に対して $c''_{n_1 \ldots n_p} = \sum c_{r_1 \ldots r_p} c'_{s_1 \ldots s_p}$ となり、$1 \leq k \leq p$ に対して $r_k + s_k = n_k$ となります。 結論する $n_k \geq 2m$ の場合、$r_k \geq m$ または $s_k \geq m$ となり、したがって、$\mathfrak{z}$ が理想であるため、$k$ が少なくとも 1 つ$n_k \geq 2m$ である限り、$c''_{n_1 \ldots n_p} \in \mathfrak{g}$ となり、主張が確立されます。さらに、定義と近傍 $\mathfrak{z} \in \mathscr{B}$ が $\mathbf{A}$ の加法部分群であるという事実からすぐにわかるように、制限された形式冪系列のすべての導関数 $\partial T / \partial X_i$ ($1 \leq i \leq p$) は制限されます。

$\mathbf{A}$ が離散であれば、制限形式冪系列の環は、単なる多項式環 $\mathbf{A}[X_1, \ldots, X_n]$ です。

$\mathbf{A}$ が線形トポロジー化されていると常に仮定し、$\mathscr{B}$ を $\mathbf{A}$ の理想の $\mathbf{A}$ からなるの 0 の近傍の基本系とします。すべての $\mathfrak{g} \in \mathscr{B}$ について、$p_\mathfrak{g}: \mathbf{A} \to \mathbf{A}/\mathfrak{g}$ を標準準同型とします。 定義までに、制限付きフォーマル冪系列 $T \in \mathbf{A}\{X_1, \ldots, X_n\}$ ごとに、

$$
\bar{p}_\mathfrak{g}(T) \in (\mathbf{A}/\mathfrak{g})[X_1, \ldots, X_p].
$$

明らかに

$$
((\mathbf{A}/\mathfrak{g})[X_1, \ldots, X_p], \bar{h}_{\mathfrak{g}\mathfrak{g}'})
$$

環の逆系 (有向インデックス集合 $\mathscr{B}$ に対して)、$(\bar{p}_\mathfrak{g})$ は準同型 $\mathbf{A}\{X_1, \ldots, X_n\} \to (\mathbf{A}/\mathfrak{g})[X_1, \ldots, X_p]$ の逆系です。すべての多項式は制限形式冪系列であるため、$\bar{p}_\mathfrak{g}$ は全射です。その核 $N_\mathfrak{g}$ は、係数属するから $\mathfrak{g}$ までの制限された正式な冪系列の $\mathbf{A}\{X_1, \ldots, X_n\}$ からなるの理想です。 $\mathbf{A}\{X_1, \ldots, X_n\}$ に (線型) 位相を与え、その $N_\mathfrak{g}$ ($\mathfrak{g} \in \mathscr{B}$ の場合) 形は 0 の近傍 (位相は明らかに $\mathbf{A}$ のそれにのみ依存します) の基本的な系とします。次に、将軍位相、章 III, § 7, no. 3、命題 2 から次のようになります。

$$
\pi = \lim_{\leftarrow} \bar{p}_\mathfrak{g}: \mathbf{A}\{X_1, \ldots, X_n\} \to \lim_{\rightarrow} (\mathbf{A}/\mathfrak{g})[X_1, \ldots, X_p]
$$

は厳密な射であり、その核は $\mathbf{A}\{X_1, \ldots, X_n\}$ の $\{0\}$ の閉包であり、その像は密です

$$
\mathbf{A}' = \lim_{\rightarrow} (\mathbf{A}/\mathfrak{g})[X_1, \ldots, X_n].
$$

#### 命題 3 {#ac-iii-s4-prop-3 .statement tag=04HY}

*線形トポロジ化された可換環 $\mathbf{A}$ がハウスドルフで完全な場合、 標準準同型 $\pi$ はトポロジカル環同型です。*

すべての $(n_1, \ldots, n) \in \mathbf{N}^p$ とすべての $3 \in \mathscr{B}$ について、$\phi_{n_1 \ldots n_p}^3$ を写像 $(A/\mathfrak{J})[X_1, \ldots, X_p] \to A/\mathfrak{J}$ とします。これは、この多項式の $X_1^{n_1} \ldots X_p^{n_p}$ の係数にすべての多項式を写像足したものです。明らかに、$\phi_{n_1 \ldots n_p}^3$ 形は、$(A/\mathfrak{J})$ モジュール準同型の逆系 (順序付けされた集合 $\mathscr{B}$ に対して) であり、$A$ は、以下によって正規に $\lim_{\leftarrow} (A/\mathfrak{J})$ と識別されます。 仮定、$\phi_{n_1 \ldots n_p} = \lim_{\leftarrow} \phi_{n_1 \ldots n_p}^3$ は、$A'$ から $A$ までの連続した $A$ 準同型写像です。 $A'$ のすべての元 $S = (S_\mathfrak{J})_{\mathfrak{J} \in \mathscr{B}}$ について、形式的な冪系列 $T = \sum_{(n_i)} \phi_{n_1 \ldots n_p}(S) X_1^{n_1} \ldots X_p^{n_p}$ が制限され、$\pi(T) = S$ を満たすことがわかります。すべての $3 \in \mathscr{B}$ とすべての $\mathfrak{J}' \in \mathscr{B}$ について、$\mathfrak{J}' \subset \mathfrak{J}$、関係 $\phi_{n_1 \ldots n_p}^{\mathfrak{J}'}(S_{\mathfrak{J}'}) = 0$ が意味するもの
$$
\phi_{n_1 \ldots n_p}^{\mathfrak{J}'}(S_{\mathfrak{J}'}) \in \mathfrak{J}/\mathfrak{J}'
$$
$S_{\mathfrak{J}}$ は多項式であるため、数で有限である $(n_1, \ldots, n_p)$ を除く $\phi_{n_1 \ldots n_p}(S) \in \mathfrak{J}$ は、最初の主張を証明する $\phi_{n_1 \ldots n_p}^{\mathfrak{J}}(S_{\mathfrak{J}}) \neq 0$ であることがわかります。 2 番目は定義から続きます。 $A$ はハウスドルフであるため、$\mathbf{N}_\mathfrak{J}$ 簡約するの共通部分は 0 になり、したがって $\pi$ は *全単射* となり、$\pi$ は厳密な射であるため、証明が完成します。

#### 命題 4 {#ac-iii-s4-prop-4 .statement tag=04HZ}

*$A, B$ を 2 つの線形トポロジ化された可換環、$B$ をハウスドルフで完全なもの、$u : A \to B$ を連続的な準同型とします。すべての家族 $b = (b_i)_{1 \leq i \leq p}$ of 元 of $B$ には、固有の連続する準同型* が存在します。
$$
\tilde{u} : A\{X_1, \ldots, X_p\} \to B
$$
*すべての $a \in A$ に対して $\tilde{u}(a) = u(a)$ が、$1 \leq i \leq p$ に対して $\tilde{u}(X_i) = b_i$ となるようにします。*

$a \in A$ に対して $v(a) = u(a)$ が、$1 \leq i \leq p$ に対して $v(X_i) = b_i$ となるような一意な準同型 $v : A[X_1, \ldots, X_p] \to B$ が存在します。さらに、$\mathfrak{J}$ が理想である $B$ の 0 の近傍である場合、$\overline{u}^{-1}(\mathfrak{J}) = 3$ は 0 の近傍である $A$ の理想であり、すべての多項式 $P \in \mathbf{N}_\mathfrak{J}$ について、明らかに $v(P) \in \mathfrak{J}$ であるため、$v$ は次のようになります。継続的な。 $A\{X_1, \ldots, X_p\}$には$A[X_1, \ldots, X_p]$が密集しているので、$\tilde{u}$の存在と一意性は、*一般位相*、章111、§ 3, no. 3、命題5と拡大の同一性の原則に従う。

$A = B$ と $u$ が恒等写像である特殊なケースでは、すべての限定形式冪系列 $f \in A\{X_1, \ldots, X_p\}$ の $\tilde{u}(f)$ の値に $f(b_1, \ldots, b_p)$ または $f(b)$ を書きます。

*注意*

#### 注意 1 {#ac-iii-s4-n2-rem-1 .statement tag=04I0}

命題 4 は、ハウスドルフで完全であると仮定される環 $A$ のすべての*閉じた* イデアル $a$ について、$1 \leq i \leq p$ に対する関係 $b_i \in a$ は、すべての制限形式冪に対して $f(b_1, \ldots, b_p) \in a$ を意味することを証明します。 系列 $f \in A\{X_1, \ldots, X_p\}$。

#### 注意 2 {#ac-iii-s4-n2-rem-2 .statement tag=04I1}

$A$ が線形トポロジー化されていると仮定します。 $r$ を 1 $\leq r \leq p$ となるように整数とし、環 $A\{X_1, \ldots, X_r\}$ に上で定義した位相を与えます。次に、トポロジー 環 $A\{X_1, \ldots, X_r\}$ は、制限形式冪系列の環と同一視されます。

$$
(A\{X_1, \ldots, X_r\})\{X_{r+1}, \ldots, X_p\}
$$

定義からすぐに以下の通り。

#### 注意 3 {#ac-iii-s4-n2-rem-3 .statement tag=04I2}

*注意 2* の記法で、さらに $A$ がハウスドルフで完全であると仮定し、すべての制限形式冪系列 $f \in A\{X_1, \ldots, X_r\}$ を形に記述してみましょう

$$
f = \sum_{(n_i)} c_{n_{r+1} \ldots n_p}(X_1, \ldots, X_r) X_{r+1}^{n_{r+1}} \ldots X_p^{n_p}
$$

ここで、$c_{n_{r+1} \ldots n_p}$ は正式な冪系列に限定されます。 系 $x = (x_1, \ldots, x_r)$ の元の $A$ ごとに、

$$
b_{n_{r+1} \ldots n_p} = c_{n_{r+1} \ldots n_p}(x_1, \ldots, x_p).
$$

*注意 1* からすぐに、$\sum_{(n_i)} b_{n_{r+1} \ldots n_p} X_{r+1}^{n_{r+1}} \ldots X_p^{n_p}$ は、$f(x_1, \ldots, x_r, X_{r+1}, \ldots, X_p)$ で示される *制限された*正式な冪系列であることがわかります。これは、$f$ の $1 \leq i \leq r$ を $X_i$ の $x_i$ に *置き換えることで得られると言われています。

### 3. ヘンゼルズ補題

トポロジカル環 $A$ では、$O$ が数列 $(x^n)_{n \geq 0}$ の極限である場合、元 $x$ は *トポロジー的にゼロポテント * と呼ばれます。 If $A$ is a *linearly topologized* commutative ring, to say that $x$ is topologically nilpotent means that for every open ideal $\mathfrak{J}$ of $A$ the canonical image of $x$ in $A/\mathfrak{J}$ is a *nilpotent* element of that ring. $\mathfrak{r}_g$ が $A/\mathfrak{J}$ の nil-radical である場合、明らかに $(\mathfrak{r}_g)$ は部分集合の逆系であり、$A$ のトポロジカル冪零元の集合 $t$ は、以下の $\mathfrak{r} = \lim \mathfrak{r}_g$ の逆像です。 標準準同型 $A \to \lim A/\mathfrak{J}$;したがって、それは $A$ の *閉じた理想* です。 $A$ も *Hausdorff* で *complete* である場合、この理想は $A$ のヤコブソン根基に含まれており、元 $x \in A$ が可逆であるためには、その類 mod. $t$ は、$A/t$ (§ 2, no. 13、補題 3) で反転可能です。

$A$ が環で、$m$ が $A$ の両側イデアルである場合、$m$ の元は *m 進数* 位相に関してトポロジー的に零であることに注意してください。

**定理 1 (ヘンゼル)**。 $A$ を完全なハウスドルフ線形トポロジ化された可換環とします。 $m$ を $A$ の閉じた理想とし、その元はトポロジー的にゼロポテンツです。 $B = A/m$ を商トポロジカル環および $\varphi : A \to B$ 標準写像とします。 $R$ を $A\{X\}$ の制限形式冪系列、 $\overline{P}$ $B[X]$ のモニック多項式、 $\overline{Q}$ を $B\{X\}$ の制限形式冪系列とします。 $\overline{\varphi}(R) = \overline{P} \cdot \overline{Q}$、$\overline{P}$、$\overline{Q}$ が $B\{X\}$ において強い相対素数であると仮定します。次に、首一多項式 $P \in A[X]$ の一意の順序付け対 $(P, Q)$ からなると、次のような制限された形式冪系列 $Q \in A\{X\}$ が存在します。
(4)
$$
R = P.Q, \quad \bar{\varphi}(P) = P, \quad \bar{\varphi}(Q) = \overline{Q}.
$$
さらに、$P$ と $Q$ は $A\{X\}$ において強く相対素であり、$R$ が多項式である場合、$Q$ も同様です。

証明は4つのステップに分かれています。最初の 3 つでは、$A$ が離散であると仮定します。その場合、$R$ と $\overline{Q}$ は多項式です。

(I) $m^2 = 0$
Let $S, T$ be two polynomials of $A[X]$ such that $S$ is monic and $\bar{\varphi}(S) = \overline{P}$, $\bar{\varphi}(T) = \overline{Q}$; Proposition 2 of no. 1 shows that $S$ and $T$ are strongly relatively prime; hence (no. 1, Proposition 1) there exists a unique ordered pair of polynomials $(S', T')$ of $A[X]$ such that
(5)
$$
R - ST = ST' + TS' \quad \text{and} \quad \deg(S') < \deg(S) = \deg(\overline{P}).
$$
The polynomials $P = S + TS'$, $Q = T + T'$ are then solutions to the problem; then in fact
(6)
$$
\overline{P} \cdot \bar{\varphi}(T') + \overline{Q} \cdot \bar{\varphi}(S') = \bar{\varphi}(ST' + TS') = \bar{\varphi}(R - ST) = 0.
$$
As $\overline{P}$ is monic, $\overline{P}$ and $\overline{Q}$ strongly relatively prime and
$$
\deg(\bar{\varphi}(S')) < \deg(\overline{P}),
$$
Proposition 1 of no. 1 shows that $\bar{\varphi}(S') = \bar{\varphi}(T') = 0$, in other words the coefficients of $S'$ and $T'$ belong to $m$ and the relation $m^2 = 0$ gives
$$
PQ = ST + ST' + TS' = R,
$$
which satisfies relation (4). Since $\bar{\varphi}(P) = \overline{P}$ and $\bar{\varphi}(Q) = \overline{Q}$, $P$ and $Q$ are strongly relatively prime (no. 1, Proposition 2); finally, if $P_1$ and $Q_1$ are two other polynomials in $A[X]$ satisfying (4) and such that $P_1$ is monic, then necessarily, setting $S'_1 = P_1 - S, \ T'_1 = Q_1 - T, \ \deg(S'_1) < \deg(S)$ and $R - ST = ST'_1 + TS'_1$ since $S'_1$ and $T'_1$ have their coefficients in $m$; but Proposition 1 then proves that $S' = S'_1$ and $T' = T'_1$, which proves the uniqueness of the ordered pair $(P, Q)$.

(2) $m$ は無能です
$n$ を $m^n = 0$ となるように最小の整数とし、$n = 2$ に対して定理が示されているので、$n > 2$ について帰納法によって議論してみましょう。 Let $A = A/m^{n-1}$, $m' = m/m^{n-1}$; as ${m'}^{n-1} = 0$, there exists a unique ordered pair $(P', Q')$ of polynomials in $A'[X]$ such that $P'$ is monic, $R' = P'Q'$, $\psi(P') = \overline{P}$ and $\psi(Q') = \overline{Q}$, where $\psi$ denotes the canonical homomorphism $A' \to A'/m' = B$, $\theta$ the canonical homomorphism $A \to A'$ and $R' = \tilde{\theta}(R)$. On the other hand, as $(m^{n-1})^2 = 0$, there exists a unique ordered pair $(P, Q)$ of polynomials in $A[X]$ such that $P$ is monic and $R = PQ$, $\bar{\theta}(P) = \overline{P}$, $\bar{\theta}(Q) = \overline{Q}$; as $\phi = \psi \circ \theta$, this shows the existence and uniqueness of $P$ and $Q$ satisfying (4); moreover $P'$ and $Q'$ are strongly relatively prime by the induction hypothesis and hence so are $P$ and $Q$.

(3) **離散的**

この場合、$m$ は必ずしも nilpotent ではありませんが、常に仮定による *nilideal* であることに注意してください。 $P_0$、$Q_0$ を、$\bar{\varphi}(P_0) = \overline{P}$、$\bar{\varphi}(Q_0) = \overline{Q}$、$P_0$ がモニックとなる 2 つの$A[X]$ の多項式とする。 $R - P_0 Q_0$の係数によって生成される$A$の理想$n$を考えてみましょう。それは有限に生成され、$m$ に含まれるため、*無能* (章 11、§ 2, no. 6、命題 15) であり、定義までに、$\psi : A \to A/n$ が標準写像の場合、$\bar{\psi}(R) = \bar{\psi}(P_0) \bar{\psi}(Q_0)$ になります。 さらに、$\bar{\psi}(P_0)$ と $\bar{\psi}(Q_0)$ は、$\overline{P}$ と $\overline{Q}$ の仮定と、no. 1 の 2 を標準準同型 $A/n \to A/m$ に適用する命題から、強い相対素数です。 したがって、ケース (2) により、$P$ がモニックであり、関係 (4) が成り立つような、$A[X]$ の多項式の順序付けられた対 $(P, Q)$ が存在します。 $\overline{P}$ と $\overline{Q}$ が強い相対素であるという事実は、$m$ が $A$ のヤコブソン根基に含まれているため、no. 1、命題 2 のおかげで、$P$ と $Q$ が$A[X]$ で強く相対素であることを意味します。 Suppose finally that $P_1$, $Q_1$ are two polynomials in $A[X]$ satisfying (4) and such that $P_1$ is monic and let $n_1$ be the finitely generated ideal of $A$ generated by the coefficients of $P - P_1$ and the coefficientsof $Q - Q_1$; as $n_1$ is contained in $m$, it is nilpotent and, if $\psi_1 : A \to A/n_1$ is the canonical mapping, $\bar{\psi}_1(P) = \bar{\psi}_1(P_1)$ and
$$
\bar{\psi}_1(Q) = \bar{\psi}_1(Q_1);
$$
the uniqueness property for case (2) therefore implies $P = P_1,\ Q = Q_1$.

(4) **一般的な場合**

$\mathscr{B}$ を、$A$ の理想の $A$ からなるの 0 の近傍の基本的な系とします。 すべての $\mathfrak{s} \in \mathscr{B}$ について、$f_{\mathfrak{s}}$ を標準写像 $A \to A/\mathfrak{s}$、$\phi_{\mathfrak{s}}$ 標準写像とします
$$
A/\mathfrak{s} \mapsto (A/\mathfrak{s})/((m + \mathfrak{s})/\mathfrak{s}) = A/(m + \mathfrak{s}),
$$
$g_{\mathfrak{s}}$ 標準写像 $B = A/m \to A(m + \mathfrak{s})$ そして $R_{\mathfrak{s}} = f_{\mathfrak{s}}(R)$、$P_{\mathfrak{s}} = g_{\mathfrak{s}}(\overline{P})$、$\overline{Q}_{\mathfrak{s}} = g_{\mathfrak{s}}(\overline{Q})$ と書きます。 それぞれの環 $A/\mathfrak{s}$ は離散であるため、ケース (3) をそれに適用することができ、$P_{\mathfrak{s}}$ がモニックであり、$R_{\mathfrak{s}} = P_{\mathfrak{s}} Q_{\mathfrak{s}}$、$\bar{\varphi}_{\mathfrak{s}}(P_{\mathfrak{s}}) = \overline{P}_{\mathfrak{s}}$、$\bar{\varphi}_{\mathfrak{s}}(Q_{\mathfrak{s}}) = \overline{Q}_{\mathfrak{s}}$ であるような、$(A/\mathfrak{s})[X]$ に固有の順序付けられた多項式対 $(P_{\mathfrak{s}}, Q_{\mathfrak{s}})$ が存在することがわかります。 この対の順序の一意性は、$\mathfrak{s}' \subset \mathfrak{s}$、$\mathfrak{s}' \in \mathscr{B}$、$f_{\mathfrak{s}'\mathfrak{s}} : A/\mathfrak{s}' \to A/\mathfrak{s}$ が標準写像の場合、$P_{\mathfrak{s}} = f_{\mathfrak{s}'\mathfrak{s}}(P_{\mathfrak{s}'})$、$Q_{\mathfrak{s}} = f_{\mathfrak{s}'\mathfrak{s}}(Q_{\mathfrak{s}'})$ であることを意味します。 次に、$A[X]$ と $\lim(A/\mathfrak{s})[X]$ (no. 2、命題 3) の正規同一化から、すべての $s \in \mathscr{B}$ に対して $R = PQ$ と $\bar{f}_s(P) = P_s, \bar{f}_s(Q) = Q_s$ が存在するような $P \in A\{X\}$ と $Q \in A\{X\}$ が存在することがわかります。 さらに、
$$
\bar{g}_s(\overline{P} - \overline{\varphi}(P)) = 0, \quad \bar{g}_s(\overline{Q} - \overline{\varphi}(Q)) = 0
$$
すべての $s \in \mathscr{B}$ について、つまり、$\overline{P} - \overline{\varphi}(P)$ および $\overline{Q} - \overline{\varphi}(Q)$ のすべての $\mathfrak{J} \in \mathscr{B}$ 係数について、すべての属するから $(m + \mathfrak{J})/m$ についてです。 しかし、$m$ は $A$、$\bigcap_s (m + s) = m$、よって $\overline{P} = \overline{\varphi}(P), \overline{Q} = \overline{\varphi}(Q)$、$P$、$Q$ で閉じられているため、確実に満たす (4) になります。さらに、$P_s$ はモニックであり、同じ次数であるため、制限形式冪系列 $P$ はモニック多項式です。 $(P', Q')$ が他の順序対満たす (4) で、$P'$ がモニック多項式である場合、$R_s = \bar{f}_s(P') \bar{f}_s(Q'), \bar{\varphi}_s(\bar{f}_s(P')) = \overline{P}_s$ と $\bar{\varphi}_s(\bar{f}_s(Q')) = \overline{Q}_s$ および (3) の場合の一意性により、すべての $s \in \mathscr{B}$ について $\bar{f}_s(P') = P_s, \bar{f}_s(Q') = Q_s$ が得られます。これは、$P = P'$ と $Q = Q'$ を意味します。 Let us show finally that $P$ and $Q$ are strongly relatively prime; by virtue of case (3) and Proposition 1 of no. 1, for all $s \in \mathscr{B}$, there exists a unique ordered pair $(S_s, T_s)$ of polynomials in $(A/\mathfrak{J})[X]$ such that
$$
1 = P_s S_s + Q_s T_s \quad \text{and} \quad \deg(T_s) < \deg(P_s) = \deg(\overline{P}).
$$
The uniqueness of this ordered pair shows immediately that, for $3' \in \mathscr{B}$, $\mathfrak{J}' \subset \mathfrak{J}, S_{3'} = \bar{f}_{33'}(S_{3}), T_{3'} = \bar{f}_{33'}(T_{3});$ taking account of no. 2, Proposition 3, we conclude that there exist two restricted formal power series $S, T$ of $A\{X\}$ such that $S_s = \bar{f}_s(S), T_s = \bar{f}_s(T)$ and $1 = PS + QT$.

$R$ が多項式である場合、$Q$ も多項式であることを検証する必要があります。ここで、$Q_s$ は構成による多項式であり、$P_s$ がモニックであるため、関係 $R_s = P_s Q_s$ が意味します
$$
\deg(Q_s) \leq \deg(R_s) \leq \deg(R)
$$
すべての$s \in \mathscr{B}$; よって $Q$ の定義によって必要な結果がすぐに得られます。

### 4. 合成の系の正式な冪系列

$A$ を可換環とします。 系と言いましょう
$$
\mathbf{f} = (f_1, \ldots, f_p) \in (A[[X_1, \ldots, X_q]])^p
$$
$X_j$ ($1 \leq j \leq q$) の正式な冪系列と、$A$ の係数が、すべての $f_j$ に当てはまる場合、*定数項* はありません。正式な冪系列のすべての系 (8) およびすべての系
$$
\mathbf{g} = (g_1, \ldots, g_q) \in (A[[X_1, \ldots, X_r]])^q
$$
定数項がない $q$ 形式冪系列の場合、形式冪系列 $f_j(g_1, \ldots, g_q)$ ($1 \leq j \leq p$) の $\mathbf{f} \circ \mathbf{g}$ (または $\mathbf{f}(\mathbf{g})$) 系で表します。
$$
(A[[X_1, \ldots, X_r]])^p
$$

(代数、章 IV, § 5, no. 5)。もし
$$
\mathbf{h} = (h_1, \ldots, h_r) \in (\mathbf{A}[[X_1, \ldots, X_s]])^r
$$
定数項のない 3 番目の系である場合、
$$(10)$$
$$(f \circ g) \circ h = f \circ (g \circ h).$$

For every integer $m$,
$$(f^{(m)} \circ g^{(m)}) \circ h^{(m)} = f^{(m)} \circ (g^{(m)} \circ h^{(m)})$$
where $f^{(m)}, g^{(m)}, h^{(m)}$ denote the systems of polynomials consisting of terms of total degree $\leq m$ in the systems of formal power series $f, g, h$. しかし明らかに、$(f \circ g) \circ h$ (それぞれ $f \circ (g \circ h)$) の系列の合計次数 $\leq m$ の項は、$(f^{(m)} \circ g^{(m)}) \circ h^{(m)}$ (それぞれ $f^{(m)} \circ (g^{(m)} \circ h^{(m)})$)、よっての主張と同じです。

すべての系 (8) について、ヤコビアン行列 $(\partial f_i / \partial X_j)$ ($1 \leq i \leq p, 1 \leq j \leq q$) を $M_f$ または $M_f(\mathbf{X})$ で表します。ここで、$i$ は行の添字であり、$j$ は列のそれです。 2 つの系 (8) と (9) の場合、$g$ には定数項がありません。
$$(11)$$
$$M_{f \circ g} = (M_f(g)). M_g$$
ここで、$M_f(g)$ は行列であり、その元は、$M_f$ の各系列元の $\mathbf{X}$ ($1 \leq j \leq q$) を $g$ に置き換えることで得られます。この公式は、代数、章 IV, § 5, no. 8 の公式 (9) を再定式化したものです。 $M_f$ の元の定数項の $M_f(0)$ 行列で表すことにします。次に、(11) から次のように推測します。
$$(12)$$
$$M_{f \circ g}(0) = M_f(0). M_g(0).$$

整数 $n > 0$ が与えられると、次のように書きます。
$$(13)$$
$$\mathbf{1}_n = \mathbf{X} = (X_1, \ldots, X_n) \in (\mathbf{A}[[X_1, \ldots, X_n]])^n,$$
これは、単一の列を含む行列と見なされます。

系 $\mathbf{f} = (f_1, \ldots, f_n) \in (\mathbf{A}[[X_1, \ldots, X_n]])^n$ ごとに、$M_f$ は位数 $n$ の平方行列です。 $J_f$ または $J_f(\mathbf{X})$ でその行列式を表し、$J_f(0)$ で $\det(M_f(0))$ に等しい $J_f$ の定数項を表します。 $(\mathbf{A}[[X_1, \ldots, X_n]])^n$ の定数項がなければ、$\mathbf{g} = (g_1, \ldots, g_n)$ が系である場合、(11) と (12) より、
$$(14)$$
$$J_{f \circ g} = J_f(g) \cdot J_g$$
$$(15)$$
$$J_{f \circ g}(0) = J_f(g) J_g(0).$$

#### 命題 5 {#ac-iii-s4-prop-5 .statement tag=04I3}

*$\mathbf{A}[[X_1, \ldots, X_n]]$の$n$系列の定数項を除いて、$\mathbf{A}$を可換環と$\mathbf{f} = (f_1, \ldots, f_n)$系とします。 $J_f(0)$ が $\mathbf{A}$ で可逆であるとします。すると、$\mathbf{A}[[X_1, \ldots, X_n]]$ には定数項 $\mathbf{g} = (g_1, \ldots, g_n)$ の $n$ 系列が存在せず、系が存在します*
$$(16)$$
$$f \circ g = \mathbf{1}_n.$$

この系はユニークで、

(17) $g \circ f = 1_1$。

$g$ の存在と一意性は、代数、章 IV, § 5, no. 9、命題 10 に続き、$n$ 正式な冪系列に適用されます。

$$
f_i(Y_1, \ldots, Y_n) - X_i \quad (1 \leq i \leq n).
$$

(15) と (16) から、$J_f(0)J_g(0) = 1$、したがって $J_g(0)$ も可逆であることがわかります。 $g \circ h = 1_1$ となるような $A[[X_1, \ldots, X_n]]$ に定数項が無く、 $n$ 系列の系 $h = (h_1, \ldots, h_n)$ が存在すると結論する。この関係と (16) から、(10) を使って次のようになります。

$$
h = 1_n \circ h = (f \circ g) \circ h = f \circ (g \circ h) = f \circ 1_n = f.
$$

Proposition 5 and formulae (10) and (15) show that under the law of composition $(f, g) \mapsto f \circ g$ the set of systems $f = (f_1, \ldots, f_n)$ of $n$ series without constant term in $A[[X_1, \ldots, X_n]]$ for which $J_f(0)$ is invertible in $A$, is a group.

### 5. 系の方程式が完成しました環

簡潔に言うと、以下では、環が可換で、線形トポロジー化され、ハウスドルフで完全であれば、*ヘンゼルの条件* を満たします。このような環で理想的な $m$ が与えられた場合、$m$ (または順序付けられた対 $(A, m)$) は、$m$ が $A$ で閉じられ、その元が位相幾何学的に一致する場合、満たす *ヘンセルの条件* となります。無能。トポロジー的にすべての冪零元のうち、$A$ からなるの理想的な $t$ は、ヘンゼルの条件 (no. 3) を満たします。

In particular, if $A$ is a commutative ring and $m$ an ideal of $A$ and $A$ is Hausdorff and complete with respect to the *m-adic* topology, the ordered pair $(A, m)$ satisfies Hensel’s conditions.

#### 命題 6 {#ac-iii-s4-prop-6 .statement tag=04I4}

*$A$を可換環、$B$環満たすをヘンゼルの条件、$u : A \to B$準同型とします。トポロジー的に冪零元の $B$ のすべての族 $x = (x_1, \ldots, x_n)$ に対して、$A[[X_1, \ldots, X_n]]$ から $B$ までの一意な準同型 $\tilde{u}$ が存在し、すべての $a \in A$ に対して $\tilde{u}(a) = u(a)$ が、$1 \leq i \leq n$ に対して $\tilde{u}(X_i) = x_i$ が存在します。さらに、$m$ が $A[[X_1, \ldots, X_n]]$ の定数項を持たない系列の理想を表す場合、$\tilde{u}$ は m 進数位相について連続です。

Let $a$ be the finitely generated ideal generated in $B$ by the $x_i$ ($1 \leq i \leq n$); for every open ideal $\mathfrak{H}$ of $B$, the images of the $x_i$ in $B/\mathfrak{H}$ are nilpotent, hence the ideal $(a + \mathfrak{H})/\mathfrak{H}$ is nilpotent in $B/\mathfrak{H}$ and there exists an integer $k$ such that, for $\sum_{i=1}^n p_i \geq k$, $x_1^{p_1} \cdots x_n^{p_n} \in \mathfrak{H}$. $m^k$ のすべての元は、形 $X_1^{p_1} \cdots X_n^{p_n} g(X_1, \ldots, X_n)$ の形式的な冪系列の有限和であるため、$\sum_{i=1}^n p_i \geq k$ では、$\tilde{u}$ が問題を解くと、$\tilde{u}(m^k) \subset \mathfrak{H}$ となることがわかります。 $\tilde{u}$ の連続性を証明します。 明らかに存在します一意な準同型

$$
\nu : A[X_1, \ldots, X_n] \to B
$$

$a \in A$ については $\nu(a) = u(a)$、$1 \leq i \leq n$ については $\nu(X_i) = x_i$ であり、上記の引数は、$\nu$ が m 進数位相によって $A[X_1, \ldots, X_n]$ に誘導された位相に関して連続であることを示しています。 $A[X_1, \ldots, X_r]$ は m 進数位相で $A[[X_1, \ldots, X_r]]$ に密であり、B はハウスドルフで完全であるため、これにより存在の証明と $\tilde{u}$ の一意性が完了します。

この命題は、§ 2, no. 9 の命題 11 の特殊なケース (i) として再び与えられることに注意してください。

$A$自体を線形トポロジー化すると、$\tilde{u}$の制限から$A\{X_1, \ldots, X_r\}$一致するに、no. 2の命題4の$u$から準同型が導出されます。 これは、この環が 0 の近傍の基本的な系と理想 $m^k \cap N_3$ (no. 2 の記法では、この位相が最小である) で位相が与えられる場合、$A[X_1, \ldots, X_r]$ が $A\{X_1, \ldots, X_r\}$ で密であるという事実からすぐに得られます。 no. 2 で定義された $A[[X_1, \ldots, X_n]]$ および位相の m 進数位相によって $A\{X_1, \ldots, X_r\}$ に誘導された位相の上界)。

$B = A$ と $u$ が恒等写像の場合、すべての正式な冪系列 $f \in A[[X_1, \ldots, X_r]]$ に対して、元 $\tilde{u}(f)$ には $f(x_1, \ldots, x_r)$ または $f(x)$ を書きます。 $A[[X_1, \ldots, X_r]]$ の正式な冪系列のすべての系 $\mathbf{f} = (f_1, \ldots, f_r)$ について、$\mathbf{f}(x)$ が $A^r$ の元 $(f_1(x), \ldots, f_r(x))$ を表すとすると、$x_i$ を$\mathbf{f}$の$X_i$。 $n \leq m$ で、F が $A[[X_1, \ldots, X_m]]$ の形式的な冪系列である場合、F は、$A[[X_1, \ldots, X_n]]$ の係数を伴う、$X_{n+1}, \ldots, X_m$ の形式的な冪系列と考えることができます。させて

$$
F(x_1, \ldots, x_n, X_{n+1}, \ldots, X_m)
$$

F の係数の $X_i$ を $1 \leq i \leq n$ に $x_i$ を代入することで得られる $A[[X_{n+1}, \ldots, X_m]]$ の正式な冪系列を表します。

$B$ を正式な冪系列 $A[[X_1, \ldots, X_r]]$ の環とし、$n$ を定数項を使わずに $B$ の系列の理想とすることで、$(B, n)$ はヘンゼルの式を満たすようにします。 条件 ($§ 2$、no. 6、系 ～ 命題 6)。 命題 6 は、定数項を使用せずに $x_i \in B$ を系列とすることで適用できます。したがって、すべての系列 $\mathbf{f} \in A[[X_1, \ldots, X_r]]$ に対して、$\tilde{u}(f)$ は、代数、章 IV、$§ 5$、no. 5 で定義される形式的な冪系列 $f(x_1, \ldots, x_n)$ です。これは、$f$ が多項式である場合、一般的な場合の命題から、$f \mapsto f(x_1, \ldots, x_n)$ が m 進数位相に関して $A[[X_1, \ldots, X_n]]$ で連続であることに注目することで明らかです。

#### 系 {#ac-iii-s4-n5-cor-1 .statement tag=04I5}

$A$ を環満たすヘンゼルの条件と $x = (x_1, \ldots, x_n)$ をトポロジー的に $A$ の冪零元の族とします。 $A[[X_1, \ldots, X_s]]$ の系列の定数項と $A[[X_1, \ldots, X_q]]$ の正式な冪系列の $f = (f_1, \ldots, f_p)$ 系を除いて、$g = (g_1, \ldots, g_q)$ を系とします。この場合、$g(x) = (g_1(x), \ldots, g_q(x))$ はトポロジー的には $A$ の冪零元の族であり、

$$
(f \circ g)(x) = f(g(x)).
$$

$g_i(x)$ がトポロジカルに零能であるという事実は、命題 6 からすぐに得られ、$A$ ではトポロジカルに冪零元の理想が閉じているという事実が得られます。 $f_j$ が多項式の場合、関係 (18) は明らかです。一方、$m$ と $m'$ が定数項を持たない系列の理想である場合、

$$
A[[X_1, \ldots, X_q]] \quad \text{and} \quad A[[X_1, \ldots, X_n]]
$$

それぞれ、明らかに関係 $f \in {m'}^k$ は $f(g_1, \ldots, g_q) \in {m'}^k$ を暗示します。したがって、上記の注意と命題 6 のおかげで、$A[[X_1, \ldots, X_q]]$ に $m$ 進数位相が与えられると、(18) の両辺は $f$ から $(A[[X_1, \ldots, X_q]])^p$ までの連続写像になります。 よって関係 (18)。

以下では、環 $A$ と $A$ の理想 $m$ について、曖昧さを避けるために、$A^n$ では $m^{x^n}$ 積集合 $\prod_{i=1}^n m$ で表します。ここで、$1 \leq i \leq n$ は $m_i = m$ です。

#### 命題 7 {#ac-iii-s4-prop-7 .statement tag=04I6}

*$A$ を環とし、$m$ を $A$ の理想とし、順序付けされた対 $(A, m)$ がヘンゼルの条件を満たすようにします。 $J_f(0)$ が $A$ で可逆となるように、$A[[X_1, \ldots, X_n]]$ の系列の定数項を除いて $f = (f_1, \ldots, f_n)$ を系とします。次に、すべての $x \in m^{x^n}$、$f(x) \in m^{x^n}$、$x \mapsto f(x)$ は、$m^{x^n}$ の全単射であり、逆全単射は $x \mapsto g(x)$ であり、$g$ は no. 4 の関係 (16) によって与えられます。

盗難が多項式である場合、$f(x) \in m^{x^n}$ が明らかであり、一般的な場合では命題 6 から続き、$m$ が $A$ で閉じられるという事実。 命題の残りの主張は、(16)、(17)、(18) の明らか帰結になります。

#### 系 {#ac-iii-s4-n5-cor-2 .statement tag=04I7}

※$q$を$m$に含まれる$A$の閉じた理想とする。したがって、関係 $x \equiv x' \pmod{q^{x^n}}$ は $f(x) \equiv f(x') \pmod{q^{x^n}}$ と同等です。*

すべての正式な冪系列 $f \in A[[X_1, \ldots, X_n]]$ に対して、

$$
f(X_1, \ldots, X_n) - f(Y_1, \ldots, Y_n) = \sum_{i=1}^n (X_i - Y_i) h_i(X_1, \ldots, X_n, Y_1, \ldots, Y_n)
$$

ここで、$h_i$ 属するから $A[[X_1, \ldots, X_n, Y_1, \ldots, Y_n]]$ (代数、章 IV, § 5, no. 8、命題 9); 関係 $x \equiv x' \pmod{q^{x^n}}$ は $f(x) \equiv f(x') \pmod{q^{x^n}}$ を暗示します。 逆は、置き換えること $f$ の「逆元」$g$ によって得られます。

#### 定理 2 {#ac-iii-s4-thm-2 .statement tag=04I8}

*$A$を環、$m$を$A$の理想とし、順序付けられた対$(A, m)$がヘンゼルの条件を満たすようにします。 $f = (f_1, \ldots, f_n)$ を $n$ 元の系とします

A\{X_1, \ldots, X_n\} とし、$a \in A^n$; $J_t(a) = e$と書きましょう。 $A\{X_1, \ldots, X_n\}$ には定数項を持たない制限形式冪系列の系 $g = (g_1, \ldots, g_n)$ が存在します。
(i) $M_g(0) = I$、(単位元行列)。
(ii) $x \in A^n$ 全員について、
$$(19)$$
$$f(a + ex) = f(a) + M_t(a) \cdot eg(x).$$
(iii) $h = (h_1, \ldots, h_n)$ を、定数項 (必ずしも制限されない) を持たない形式的な冪系列の系として、$g \circ h = 1_n$ (命題 5) とします。 $y \in m^{n \times n}$ 全員にとって、
$$(20)$$
$$f(a + eh(y)) = f(a) + M_t(a) \cdot ey.$$
フォーマルな冪系列 $f \in A[[X_1, \ldots, X_n]]$ ごとに、
$$(21)$$
$$f(X + Y) = f(X) + M_f(X) \cdot Y + \sum_{1 \leq i < j \leq n} G_{ij}(X, Y)Y_i Y_j,$$
ここで、$G_{ij}$ は正式に決定されています冪系列
$$A[[X_1, \ldots, X_n, Y_1, \ldots, Y_n]].$$
ff が制限されている場合、$M_f$ の元と $G_{ij}$ も同様です。これらの形式的な冪系列は多項式です iff が多項式であり、それらの一意性から、$A$ のすべての開いた理想 $\mathfrak{J}$ について、次のようになります。 $p_\mathfrak{J}: A \to A/\mathfrak{J}$ 標準写像、$p_\mathfrak{J}$ の $G_{ij}$ の像は、$p_\mathfrak{J}(F)$ の $Y_i Y_j$ の係数で、$F$ は正式な冪系列 $f(X + Y)$ $A[[X_1, \ldots, X_n, Y_1, \ldots, Y_n]]$に。 よって私たちの主張。

したがって、各系列 ft $(1 \leq i \leq n)$ に対して公式 (21) を書くと、すべての $x \in A^n$ (no. 2, 命題 4) が得られます。
$$(22)$$
$$f(a + ex) = f(a) + M_t(a) \cdot ex + e^2 r(x)$$
ここで、$r = (r_1, \ldots, r_r)$ は、制限された正式な冪系列の系であり、それぞれの合計は位数 $\geq 2$ です。 代数、章 III, § 6, no. 5 の式 (18) から、次のような平方行列 $M' \in \mathbf{M}_n(A)$ が存在することがわかります。
$$(23)$$
$$M_t(a) \cdot M' = eI_n,$$
よってこれを (22) で使用します
$$(24)$$
$$f(a + ex) = f(a) + M_t(a) \cdot ex + M_t(a) M' \cdot er(x).$$

$g = 1, + M' \cdot r$ と書くと、$g$ が条件 (i) と (ii) を満たすことがわかります。 (iii) を得るには、置き換える $x$ by $h(y)$ を実行すれば十分です。

#### 系 1 {#ac-iii-s4-thm-2-cor-1 .statement tag=04I9}

Let $A$ be a ring and $m$ an ideal of $A$ such that the ordered pair $(A, m)$ satisfies Hensel's conditions. $f \in A\{X\}$、$a \in A$とし、$e = f'(a)$と書きます。 $f(a) \equiv 0$ (修正 $e^2 m$) の場合、$f(b) = 0$ と $b \equiv a$ (修正 $em$) のような $b \in A$ が存在します。 b' が $\mathbf{A}$ の他の元で、$f(b') = 0$ と $b' \equiv a \pmod{\mathfrak{m}}$ である場合、$e(b - b') = 0$ です。 特に、$e$ が $\mathbf{A}$ の零の因子ではない場合、$b$ は一意です。

$f(a) = e^2 c$ を $c \in \mathfrak{m}$ とします。 $n = 1$ に対して公式 (20) は次のようになります
$$
f(a + eh(y)) = e^2(c + y)
$$
したがって、$y = -c$、$b = a + eh(-c)$ を取るだけで十分です。さらに、$b = a + ex, b' = a + ex', x \in \mathfrak{m}, x' \in m, f(b) = f(b') = 0$ の場合、(19) から $e^2(g(x) - g(x')) = 0$ と推定されます。 $u$ が制限されている $g(\mathbf{X}) - g(\mathbf{Y}) = (\mathbf{X} - \mathbf{Y})u(\mathbf{X}, \mathbf{Y})$ と、$v \in \mathbf{A}$ が反転可能な$u(0, 0) = 1$、$g(x) - g(x') = (x - x')v$ のように、$m$ が閉じているため、$v - 1 = u(x, x') - 1 \in \mathfrak{m}$ と $m$ は、次のジェイコブソン根基に含まれます。 $\mathbf{A}$; よって関係 $e(b - b') = 0$。

#### 注意 {#ac-iii-s4-n5-rem-1 .statement tag=04IA}

系は、$e$ が $\mathbf{A}$ で反転可能な場合に特に当てはまります。次に、ヘンゼルの定理から $b$ の存在も推定できます。 $(\mathbf{A}/\mathfrak{m})\{\mathbf{X}\}$ の $f(\mathbf{X})$ の標準像は形 $(\mathbf{X} - a)f_1(\mathbf{X}), \mathbf{X} - a$ と $f_1(\mathbf{X})$ が強く相対的に素であり、$f_1(\alpha) = f'(\alpha)$ は像であるためです。 $e$ (no. 1、例)。

例
(1) $p$ を素数数 $\neq 2$ と $n$ 整数とし、類を法とする。 $p$ は、素数体 $\mathbf{F}_p$ の平方 $\neq 0$ です。 $\mathbf{Z}_p$ が $p$ 進数整数 (§ 2, no. 12, 例 3) の環である場合、系 1 を多項式 $\mathbf{X}^2 - n$ に適用すると、$n$ が平方であることがわかります。 $\mathbf{Z}_p$;たとえば、7 は $\mathbf{Z}_3$ の平方です。
(2) $\mathbf{A} = \mathbf{K}[[\mathbf{Y}]]$ を、可換体 $\mathbf{K}$ の係数と不定の形式冪系列の環とする。 $(\mathbf{Y})$ 進数位相、環 $\mathbf{A}$ はハウスドルフであり、完全 (§ 2, no. 6、系から命題 6) および写像 $f(\mathbf{Y}) \mapsto f(0)$ 定義するによって$\mathbf{A}/(\mathbf{Y})$の移行から商環同型が体$\mathbf{K}$に。 系 1 までに、$F(\mathbf{Y}, \mathbf{X})$ が $\mathbf{A}$ の係数を含む$\mathbf{X}$ の多項式であり、$a$ が $\mathbf{K}$ の $F(0, \mathbf{X})$ の単純な根である場合、一意の形式冪が存在します。 系列 $f(\mathbf{Y})$ は、$f(0) = a$ と $F(\mathbf{Y}, f(\mathbf{Y})) = 0$ になります。

#### 系 2 {#ac-iii-s4-thm-2-cor-2 .statement tag=04IB}

Let $\mathbf{A}$ be a ring and $\mathfrak{m}$ an ideal of $\mathbf{A}$ such that the ordered pair $(\mathbf{A}, m)$ satisfies Hensel's conditions. $r, n$ を整数とし、$0 \leq r < n$ と $\mathbf{f} = (f_{r+1}, \ldots, f_n)$ が $n - r$ の系 $\mathbf{A}\{\mathbf{X}_1, \ldots, \mathbf{X}_n\}$ の元となるようにします。 $J^{(n-r)}_{\mathbf{f}}(\mathbf{X})$ は、$M_{\mathbf{f}}(\mathbf{X})$ からなる列添字 $j$ のマイナーを$r + 1 \leq j \leq n$ のように表します。 $a \in \mathbf{A}^n$ を、$J^{(n-r)}_{\mathbf{f}}(a)$ が $\mathbf{A}$ と $\mathbf{f}(a) \equiv 0 \pmod{\mathfrak{m}^{(n-r)}}$ で可逆であるようにします。 次に、$1 \leq k \leq r$、$\mathbf{x} \equiv a \pmod{\mathfrak{m}^n}$、$\mathbf{f}(\mathbf{x}) = 0$ に対して $x_k = a_k$ などの一意の $\mathbf{x} = (x_1, \ldots, x_n) \in \mathbf{A}^n$ が存在します。

Substituting $a$, for $X_k$ for $1 \leq k \leq r$ in the $f_i$ (no. 2, Remark 3 ), we see immediately that we may restrict our attention to the case where $r = 0$ to prove the corollary. 定理 1 と命題 7 は、$a + \mathfrak{m}^n$ の $\mathbf{f}$ 定義する全単射が $\mathbf{f}(a) + \mathfrak{m}^n = \mathfrak{m}^n$ にあることを示します。 系は、$0 \in \mathfrak{m}^n$ という事実から導き出されます。

#### 系 3 {#ac-iii-s4-thm-2-cor-3 .statement tag=04IC}

*記法と系 2 では、$a \in \mathbf{A}^n$ とします。 $e = J_r^{(n-r)}(\mathbf{a})$ ($\mathbf{A}$ で必ずしも反転可能ではない) を書き、$f(\mathbf{a}) \equiv 0$ (mod. $e^{2m^{\times(n-r)}}$) と仮定しましょう。次に、$\mathbf{A}[[X_1, \ldots, X_r]]$ には定数項 $\phi_i$ ($r + 1 \leq i \leq n$) のない $n - r$ 形式的な冪系列が存在し、すべての $t = (t_1, \ldots, t_r) \in m^{\times r}$ に対して、

$$
f_i(a_1 + e^2 t_1, \ldots, a_r + e^2 t_r, a_{r+1} + e \phi_{r+1}(t), \ldots, a_n + e \phi_n(t)) = 0
$$

$r + 1 \leq i \leq n$の場合。

*$1 \leq i \leq r$の場合は、$f_i(X) = X_i - a$、$u = (f_1, \ldots, f_n)$とします。その場合、$J_u(a) = e$ と定理 2 が系 $u$ に適用される可能性があります。 定理 2 の記法では、上記の定義から、$1 \leq i \leq r$ の場合は $g_i(X) = X$、$1 \leq i \leq r$ の場合はよって $h_i(X) = X_i$ となります。さらに、$M' \in \mathbf{M}_n(\mathbf{A})$ が $M_u(a) . M' = e I_n$ となる場合、$M'$ は形になります。

$$
\begin{pmatrix}
e I_r & 0 \\
* & *
\end{pmatrix}.
$$

置き換えること $y$ は公式 (20) で $M'.z$ (ここで $z = (z_1, \ldots, z_n) \in m^{\times n}$) により、次のようになります。

$$
f_i(a_1 + e^2 z_1, \ldots, a_r + e^2 z_r, a_{r+1} + e h_{r+1}(M'.z), \ldots, a_n + e h_n(M'.z))
= \& (a) + e^2 z_i \quad \text{for } 1 \leq i \leq n.
$$

仮定、$f_j(a) = e^2 b_j$まで、$b_j \in m$は$r + 1 \leq j \leq n$です。 $\psi_j(X_1, \ldots, X_r) = h_j(M'.X)$ と書いてみましょう

$$
\phi_j(X_1, \ldots, X_r) = \psi_j(X_1, \ldots, X_r, -b_{r+1}, \ldots, -b_n)
$$

$r + 1 \leq j \leq n$の場合。 $r + 1 \leq i \leq n$ については、(26) の $r + 1 \leq j \leq n$ に $z_j$ を $1 \leq j \leq r$ に $t_j$ を、$z_j$ に $b_j$ を代入すると、すべての $t \in m^{\times r}$ に対して関係 (25) が得られます。

### 6. 環の分解への申請

#### 補題 2 {#ac-iii-s4-lem-2 .statement tag=04ID}

*$\mathbf{A}$を環、$m$を$\mathbf{A}$の理想とし、順序付けられた対$(\mathbf{A}, m)$がヘンゼルの条件を満たすようにします。 $\mathbf{B}$ を商環 $\mathbf{A}/m$、$\pi : \mathbf{A} \to \mathbf{B}$ を標準準同型とします。 $\mathbf{B}$ のすべての冪等 $c$ に対して、$\pi(e) = c$ のような $\mathbf{A}$ の一意の冪等 $e$ が存在します。

$a$ を $\pi(a) = c$ となるようにします。 no. 5 の系 1 ～ 定理 2 は、$\mathbf{A}[X]$ および元 $a \in \mathbf{A}$ の多項式 $f(X) = X^2 - X$ に適用できます。次に、$f'(a) = 2a - 1$、そして$\mathbf{B}$の$\pi(2a - 1) = 2c - 1$と$(2c - 1)^2 = 1$と同様に、$2c - 1$は$\mathbf{B}$で反転可能であり、したがって$2a - 1$は$\mathbf{A}$で反転可能です(§ 2, no. 13, 補題 3)。 $f(a) \in m$として、no. 5の系1から定理2はすぐに存在を示し、$e$の一意性が存在します。

#### 命題 8 {#ac-iii-s4-prop-8 .statement tag=04IE}

*$\mathbf{A}$を環、$m$を$\mathbf{A}$の理想とし、順序対$(\mathbf{A}, m)$がヘンゼルの条件を満たすようにします。 $\mathbf{B}$ を商環 $\mathbf{A}/m$ および $\pi : \mathbf{A} \to \mathbf{B}$ 標準準同型とします。 *B が有限家族* $(\mathfrak{b}_i)_{i \in I}$ *イデアの直接の合成である場合、* $\pi(\mathfrak{a}_i) = \mathfrak{b}_i$ *すべて* $i \in I$ * そして A は家族* $(\mathfrak{a}_i)$ の直接の合成であるような、A のイデアの固有の家族* $(\mathfrak{a}_i)_{i \in I}$ が存在します。

$I = \sum_i c_i$ として、$c_i \in \mathfrak{b}_i$ をすべて $i$ とします。 $c_i$ は、$i \neq j$ に対して $c_i c_j = 0$ となるように、$B$ の冪等です。したがって、補題 2 までに、すべての $i$ に対して $\pi(e_i) = c_i$ となるような $A$ ($i \in I$) の冪等 $e_i$ が存在します。 $e_i e_j$ は冪等なので、
$$
\pi(e_i e_j) = c_i c_j = 0
$$
$i \neq j$、$e_i e_j = 0$、$i \neq j$ (補題 2)。 $1 - \sum_i e_i$ は冪等なので、
$$
\pi\left(1 - \sum_i e_i\right) = 1 - \sum_i c_i = 0,
$$
同様に$1 = \sum_i e_i$。したがって、$A$ は理想 $\mathfrak{a}_i = e_i A$ の直接の合成であり、$\pi(\mathfrak{a}_i) = \pi(e_i) B = \mathfrak{b}_i$ であることがわかります。

そんな分解の一意性を見せるのが残っています。さて、$A$ が、すべての $i$ に対して $\pi(\mathfrak{a}'_i) = \mathfrak{b}_i$ となるような理想の他の家族 $(\mathfrak{a}'_i)_{i \in I}$ の直接の合成であると仮定します。次に、$1 = \sum_i e'_i$ ここで $e'_i \in \mathfrak{a}'_i$、よって、$B$、$1 = \sum_i \pi(e'_i)$ で$\pi(e'_i) \in \mathfrak{b}_i$、これは $\pi(e'_i) = c_i$ を意味します。 $e'_i$ と $e_i$ はべき等であるため、必然的に $e'_i = e_i$ (補題 2) となり、証明が完成します。

#### 注意 {#ac-iii-s4-n6-rem-1 .statement tag=04IF}

命題 8 は再び、ハウスドルフである $A$ に準局所リングの構造を与え、$c$ 進数位相 ($A$ のヤコブソン根基) で完成します。これはすでに の帰結として取得されています。 § 2, no. 13、系から命題19。

### 練習問題 {#ac-iii-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
