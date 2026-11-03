---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IV
chapter_title: COXETER GROUPS AND TITS SYSTEMS
section: 2
section_title: Tits Systems
lang: ja
source: lie-iv-vi
pdf_pages: 0028-0039, 0057-0072
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITIONS AND FIRST PROPERTIES
      page: 0
      pdf_page: 28
    - "no": 2
      title: AN EXAMPLE
      page: 0
      pdf_page: 30
    - "no": 3
      title: DECOMPOSITION OF G INTO DOUBLE COSETS
      page: 0
      pdf_page: 31
    - "no": 4
      title: RELATIONS WITH COXETER SYSTEMS
      page: 0
      pdf_page: 32
    - "no": 5
      title: SUBGROUPS OF G CONTAINING B
      page: 0
      pdf_page: 34
    - "no": 6
      title: PARABOLIC SUBGROUPS
      page: 0
      pdf_page: 35
    - "no": 7
      title: SIMPLICITY THEOREMS
      page: 0
      pdf_page: 36
statements: 30
exercises: 29
content_sha256: 20b5423fe766d52ab8aa8ebe2ae1267581eeeb59fc61e632f4409e8b9b2edb45
translated_from: content/en/lie/IV/02_s2_tits_systems.md
translation_method: google
source_content_sha256: d7aeccab1a27d0a0619f437c65961e9feffe9a183de0171b993a7c7681af0384
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 2a68a5d5f7a50069af75ce5f334c0dbd28650881ac38d0d85dbdacbac55927fe
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 2。おっぱい系

この段落では、G、B、N、S、T、W の文字は、以下のno. 1 に示す意味を持ちます。

### 1. 定義と最初のプロパティ

G を G の群と B 部分群とします。群 $B \times B$ は、$b, b' \in B$ と $g \in G$ に対して $(b, b').g = bg{b'}^{-1}$ だけ G に作用します。 G の $B \times B$ の軌道は、$g \in G$ の集合 $BgB$ であり、B に対する G の二重剰余類と呼ばれます。それらは G の形分割です。 対応する商は $B \backslash G / B$ で表されます。 C と $C'$ が二重剰余類である場合、$CC'$ は二重剰余類の和集合です。

#### 定義 1 {#lie-iv-s2-def-1 .statement tag=0AN8}

A おっぱい系は 4 倍体 $(G, B, N, S)$ で、G は群、B と N は G の 2 つ部分群、S は $N/(B \cap N)$、満たすの部分集合です。以下の公理です。

(T1) 集合 $B \cup N$ 生成する G と $B \cap N$ は N の通常の部分群です。
(T2) 集合 S 生成する群 $W = N/(B \cap N)$ であり、位数 2 の元で構成されます。
(T3) $s \in S$ と $w \in W$ に対して $sBw \subset BwB \cup BswB$。
(T4) $s \in S$、$sBs \notin B$ 全員に。

群 $W = N/(B \cap N)$ は、シジュウカラ系 $(G, B, N, S)$ のワイル群と呼ばれるときどきです。

5 W のすべての元は $B \cap N$ を法とする剰余類であり、したがって G の部分集合です。したがって、$BwB$ などの積は意味を成します。より一般的には、W の任意の部分集合 A について、BAB 部分集合 $\bigcup_{w \in A} BwB$ で表します。

#### 注意 1 {#lie-iv-s2-n1-rem-1 .statement tag=0AN9}

no. 5 (Th. 3 の Cor.) で、$(G, B, N)$ が与えられた場合、$(G, B, N, S)$ がシジュウカラ系であるような、$N/(B \cap N)$ の部分集合 $S$ が最大 1 つ存在することがわかります。

#### 注意 2 {#lie-iv-s2-n1-rem-2 .statement tag=0ANA}

$(G, B, N, S)$ をおっぱい系とし、$Z$ を$B$ に含まれる$G$ の通常の部分群とします。 $G' = G/Z, B' = B/Z, N' = N/(Z \cap N)$ を、$S'$ を $N'/(B' \cap N')$ の $S$ の像とします。すると、$(G', B', N', S')$ がシジュウカラ系であることがすぐにわかります。

この段落全体を通して、$(G, B, N, S)$ はシジュウカラ系を表し、集合 $T = B \cap N$ と $W = N/T$ です。二重剰余類とは、$B$に対する$G$の二重剰余類を意味します。 $w \in W$ については、集合 $C(w) = BwB$;これはダブルコセットです。

公理 (T1) から (T4) のいくつかの基本的な帰結を演繹します。 $W$ の $w, w', \ldots$ 元と $S$ の $s, s', \ldots$ 元で表します。次の関係は明らかです。

$$
C(1) = B, \quad C(ww') \subset C(w).C(w'), \quad C(w^{-1}) = C(w)^{-1}.
$$

公理(T3)は形でも書けます

$$
C(s).C(w) \subset C(w) \cup C(sw).
$$

さらに、$C(sw) \subset C(s).C(w)$ は (1) により、また $C(s).C(w)$ は二重剰余類の和集合であるため、可能性は 2 つだけです。

$$
C(s).C(w) = \begin{cases}
C(sw) & \text{if } C(w) \not\subset C(s).C(w) \\
C(w) \cup C(sw) & \text{if } C(w) \subset C(s).C(w).
\end{cases}
$$

(T4) までに、$B \neq C(s).C(s)$; (3) に $w = s$ を代入し、 関係 $s^2 = 1$ を使用すると、次のようになります。

$$
C(s).C(s) = B \cup C(s).
$$

この公式は、$B \cup C(s)$が$G$の部分群であることを示しています。右側の(4)の両辺に$C(w)$を掛け、公式(3)と関係を使う

$$
B.C(w) = C(w),
$$

私たちは得る

$$
C(s).C(s).C(w) = C(w) \cup C(sw).
$$

集合の逆数を公式 (2)、(3)、(5) に入力し、次に置き換えること $w$ を $w^{-1}$ で計算すると、公式が得られます。

$$
C(w).C(s) \subset C(w) \cup C(ws)
$$
$$
C(w).C(s) = \begin{cases}
C(ws) & \text{if } C(w) \not\subset C(w).C(s) \\
C(w) \cup C(ws) & \text{if } C(w) \subset C(w).C(s)
\end{cases}
$$
$$
C(w).C(s).C(s) = C(w) \cup C(ws).
$$

#### 補題 1 {#lie-iv-s2-lem-1 .statement tag=0ANB}

$s_1, \ldots, s_q \in S$ と $w \in W$ とします。私たちは持っています
$$
C(s_1 \ldots s_q).C(w) \subset \bigcup_{(i_1, \ldots, i_p)} C(s_{i_1} \ldots s_{i_p} w),
$$
ここで、$(i_1, \ldots, i_p)$ は、区間 $[1, q]$ の真に増加する数列の整数の集合を表します。

私たちは$q$について帰納法によって議論しますが、$q = 0$の場合は自明です。 $q \geqslant 1$ の場合、$C(s_1 \ldots s_q).C(w) \subset C(s_1).C(s_2 \ldots s_q).C(w)$ があります。 帰納法の仮定までに、$C(s_2 \ldots s_q).C(w)$ は $C(s_{j_1} \ldots s_{j_p} w)$ の和集合に含まれます。
$$
2 \leq j_1 < \cdots < j_p \leq q.
$$
(T3) により、集合 $C(s_1 s_{j_1} \ldots s_{j_p} w)$ と $C(s_{j_1} \ldots s_{j_p} w)$ の和集合に集合 $C(s_1).C(s_{j_1} \ldots s_{j_p} w)$ が含まれます。これは補題を証明します。

### 2. 例

$k$ を $k^n$ の体、$n$ 整数 $\geq 0$、$(e_i)$ 標準基底とします。 $G = \mathbf{GL}(n, k)$、$B$ を $G$ の上三角部分群とし、$N$ を $G$ からなるの行列の部分群とし、各行に 0 以外の元が 1 つだけ存在するようにします。 列。 $N$ の元は行 $ke_i$ を並べ替えます。これにより、全射準同型 $N \to \mathscr{S}_n$ が生じ、その核は対角行列の部分群 $T = B \cap N$ となり、$\mathscr{S}_n$ と同一視する $W = N/T$ が可能になります。 $j$ と $j+1$ の転置に対する $W$ 対応するの $s_j$ ($1 \leq j \leq n-1$) 元で表します。 $S$を$s_j$の集合とします。 *quadruple* $(G, B, N, S)$ *はおっぱい系* です。確かに：

公理 (T1) は Cor. *代数*、第 4 章の提案 14 の 2 II, § 10, no. 13。

公理 (T2) は *代数*、第 4 章で証明されています。 I、p. 97を修正。
公理(T4)は明らかです。
公理 (T3) を検証することが残っています。つまり、
$$
s_j B w \subset B w B \cup B s_j w B \quad \text{for } 1 \leq j \leq n-1, w \in W,
$$
または同様に、
$$
s_j B \subset B B' \cup B s_j B', \quad \text{with } B' = w B w^{-1}.
$$
$G_j$ を $G$ からなるの元の部分群として、$i \neq j, j+1$ の$e_i$ を固定し、$e_j$ と $e_{j+1}$ にまたがる平面を安定させます。この群は $\mathbf{GL}(2, k)$ と同型です。 $G_j B = B G_j$ であることを確認します。 $s_j \in G_j$ なので、$s_j B \subset B G_j$ があり、それを証明すれば十分です
$$
G_j \subset (B \cap G_j)(B' \cap G_j) \cup (\cap G_j) s_j (B' \cap G_j).
$$
同一視する $G_j$ と $\mathbf{GL}(2, k)$; 群 $B \cap G_j$ は、$\mathbf{GL}(2, k)$ の上三角部分群 $B_2$ と同一視され、群 $B' \cap G_j$ は、$w(j) < w(j+1)$ のときは $B_2$ と下三角部分群と同一視されます。それ以外の場合は $B_2^-$ 。最初のケースでは、証明されるべき公式は次のように書くことができます

$$
\mathbf{GL}(2, k) = B_2 \cup B_2 s B_2 \quad \text{where } s = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix};
$$

これは、たとえば、$B_2$ が射影線 $\mathbf{P}_1(k)$ 上の $\mathbf{GL}(2, k)$ の作用に対して点の固定群であり、この点の補数に推移的に作用するという事実から導き出されます。 2 番目の場合、証明される公式は次のように書くことができます

$$
\mathbf{GL}(2, k) = B_2 B_2^- \cup B_2 s B_2^-;
$$

$B_2^- = s B_2 s$ 以降、これは前の公式の右側に $s$ を乗算した結果になります。

### 3. G の分解を二重剰余類に

#### 定理 1 {#lie-iv-s2-thm-1 .statement tag=0ANC}

※$G = \mathrm{BWB}$ございます。 写像 $w \mapsto C(w)$ は、$B$ に対する $G$ の二重剰余類の $W$ から集合 $B \backslash G / B$ までの全単射です。

$\mathrm{BWB}$ が $x \mapsto x^{-1}$ の下で安定していることは明らかであり、補題 1 は積の下で安定していることを示しています。 含む $B$ と $N$ なので、$G$ に等しいです。

$w \neq w'$なら$C(w) \neq C(w')$であることを証明する必要があります。このため、整数 $q$ 帰納法によって次の主張を証明します。

(A_q) $w$ と $w'$ が $l_S(w) \geq l_S(w') = q$ のように $W$ の元である場合、$C(w) \neq C(w')$ になります。

($l_S(w)$ の定義については、§ 1, no. 1 を参照してください。)

この主張は $q = 0$ ではクリアであり、その後 $w' = 1$ と $w \neq 1$ が続き、したがって $C(w') = B$ と $C(w) \neq B$ になります。

(A_q) の仮説が $q \geq 1$ と $w, w'$ 満たすであると仮定します。 $sw'$ が長さ $q - 1$ であるような $s \in S$ が存在します。私たちは持っています

$$
l_S(w) > l_S(sw')
$$

したがって $w \neq sw'$ です。さらに、$sw \neq sw'$; § 1, no. 1 の公式 (3) により、

$$
l_S(sw) \geq l_S(w) - 1 \geq l_S(sw') = q - 1.
$$

帰納法の仮定までに、$C(sw')$ は $C(w)$ および $C(sw)$ とは区別されます。 公式 (2) より、次のようになります。

$$
C(sw') \cap C(s).C(w) = \varnothing.
$$

$C(sw') \subset C(s).C(w')$以来、ついにその$C(w) \neq C(w')$が完成しました。

#### 注意 {#lie-iv-s2-n3-rem-1 .statement tag=0AND}

公理 (T4) は、前の証明では使用されませんでした。

### 4. 関係コクセター付き系

#### 定理 2 {#lie-iv-s2-thm-2 .statement tag=0ANE}

対 $(W, S)$ はコクセター 系です。また、$s \in S$と$w \in W$の場合、関係$C(sw) = C(s).C(w)$と$l_S(sw) > l_S(w)$は等価です。

任意の $s \in S$ について、$P_s$ を元 $w \in W$ の集合とします。
$$
C(s).C(w) = C(sw).
$$
§ 1, no. 7 の $P_s$ 満たす条件 (A')、(B')、および (C) を検証します。 定理の 2 つの主張は、§ 1, no. 7 の提案 6 に続きます。

条件 (A') はクリアです。

(B')を検証します。 $P_s$ と $sP_s$ の共通のに元 $w$ があった場合、$w \in P_s$ と $sw \in P_s$ が得られます。
$$
C(s).C(w) = C(sw), \qquad C(s).C(sw) = C(w).
$$
$C(s).C(s).C(w) = C(w)$ が続き、公式 (5) によって、これは $C(w) = C(sw)$ を意味し、Th と矛盾します。 1.

検証します(C)。 $s, s' \in S$と$w, w' \in W$を$w' = ws'$とします。 仮定 $w \in P_s$ と $w' \notin P_s$ は次のことを意味します
$$
C(sw) = C(s).C(w) \tag{9}
$$
$$
C(w') \subset C(s).C(w') \tag{10}
$$
(3)による。

(9) と関係 $w = w's'$ から、次のことがわかります。
$$
C(s)w's'B = C(sw). \tag{11}
$$
公式 (2'), $C(w').C(s') \subset C(w') \cup C(w's')$ により、これは直ちに次のことを意味します。
$$
C(w')s'B \subset C(ws') \cup C(w). \tag{12}
$$
$C(w')$ は左剰余類 $gB$ の和集合であるため、
$$
C(s).C(w') = C(s)w'B,
$$
公式 (10) は、$C(s)w'$ が $C(w')$ と一致することを示し、*なおさら* は $C(s)w's'B$ が $C(w')s'B$ と一致することを示します。 公式 (11) および (12) から、二重剰余類 $C(sw)$ は二重剰余類 $C(ws')$ および $C(w)$ の 1 つに等しいことがわかります。 $sw \neq w$以来、Th。 1 により、結論するが $sw = ws'$ できるようになります。

#### 系 1 {#lie-iv-s2-thm-2-cor-1 .statement tag=0ANF}

*させて* $w_1, \ldots, w_q \in W$ *そしてさせて* $w = w_1 \ldots w_q$ *もしも*
$$
l_S(w) = l_S(w_1) + \cdots + l_S(w_q),
$$
*その後*
$$
C(w) = C(w_1) \ldots C(w_q).
$$

$w_i$ の減少した分解を取ると、1 つは減少した分解の場合に減少します。

$$
w = s_1 \ldots s_q, \quad \text{with } s_i \in S.
$$

$u = s_2 \ldots s_q$ の場合、$w = s_1 u$ と $l_S(s_1 u) > l_S(u)$ なので、定理で $C(w) = C(s_1).C(u)$ になります。必要な公式は、これから $q$ の帰納法によって続きます。

#### 系 2 {#lie-iv-s2-thm-2-cor-2 .statement tag=0ANG}

※$w \in W$と$T_w$を、§ 1, no. 4の補題2の手順で$w$に関連付けられた$W$の部分集合とする。 $t \in T_w$ の場合、*

$$
C(t) \subset C(w).C(w^{-1}).
$$

$t \in T_w$ の場合、次のような定義元 $w', w'' \in W$ と $s \in S$ が存在します。

$$
w = w' s w'', \quad l_S(w) = l_S(w') + l_S(w'') + 1 \quad \text{and} \quad t = w' s {w'}^{-1}.
$$

コル著1、

$$
C(w).C(w^{-1}) = C(w').C(s).C(w'').C({w''}^{-1}).C(s).C({w'}^{-1}).
$$

したがって、

$$
C(w).C(w^{-1}) \supset C(w').C(s).C(s).C({w'}^{-1}).
$$

(4)までに、$C(s) \subset C(s).C(s)$。したがって、

$$
C(w).C(w^{-1}) \supset C(w').C(s).C({w'}^{-1}) \supset C(t).
$$

#### 系 3 {#lie-iv-s2-thm-2-cor-3 .statement tag=0ANH}

*$w \in W$と$H_w$を、$C(w).C(w^{-1})$によって生成された$G$の部分群とします。次に:*

a) *$w$ の減額された分解 $(s_1, \ldots, s_q)$ については、*

$$
C(s_j) \subset H_w \quad \text{for } 1 \leq j \leq q.
$$

b) *群 $H_w$ 含む $C(w)$ は、$C(w)$ によって生成されます。*

a) を $j$ の帰納法までに証明します。 $k < j$の$H_w$に$C(s_k)$が含まれているとします。しましょう

$$
t = (s_1 \ldots s_{j-1}) s_j (s_1 \ldots s_{j-1})^{-1}.
$$

元 $t$ 属するから部分集合 $W$ の $T_w$ は、§ 1, no. 4 の補題 2 で定義されます。コル著2、$C(t) \subset H_w$、したがって$C(s_j) \subset H_w$。

$C(w) = C(s_1) \ldots C(s_q)$、cf. コリント以降。 1、$C(w) \subset H_w$があり、b)が続きます。

#### 例 {#lie-iv-s2-n4-exa-1 .statement tag=0ANI}

Th. 2 は、no. 2 で説明されているシジュウカラ系に適用され、*対称群* $\mathfrak{S}_n$ が、連続する元の転置の集合を持ち、*コクセター 群* であることを示しています。

### 5. 部分群の G 含む B

S の任意の部分集合 X について、X (cf. §1, no. 8) によって生成された W の W_X 部分群と、二重剰余類 C(w), w ∈ の G_X 和集合 BW_XB で表します。 W_X. G_∅ = B および G_S = G が得られます。

#### 定理 3 {#lie-iv-s2-thm-3 .statement tag=0ANJ}

a) S の任意の部分集合 X について、集合 G_X は、$\bigcup_{s \in X} C(s)$ によって生成された G の部分群です。

b) 写像 X ↦ G_X は、G 含む B の部分群の $\mathscr{P}(S)$ から集合までの全単射です。

c) (X_i)_{i \in I} を X の部分集合の家族とします。 $X = \bigcap_{i \in I} X_i$の場合は、$G_X = \bigcap_{i \in I} G_{X_i}$。

d) X と Y を S の 2 つの部分集合とします。すると、$X \subset Y$ (それぞれ $X = Y$) の場合に限り、$G_X \subset G_Y$ (それぞれ $G_X = G_Y$) になります。

$G_X = (G_X)^{-1}$であることは明らかです。 補題 no. 1 の 1 は $G_X . G_X \subset G_X$ を示します。したがって、Cor を考慮して a) が続きます。 Thの1 2.

X ↦ G_X の単射性は、X ↦ W_X の単射性 (§1, no. 8、Th. 2) に続きます。逆に、H を G 含む B の部分群とします。U を $C(w) \subset H$ となるような $w \in W$ の集合とします。 H は二重剰余類の和集合なので、$H = BUB$ になります。 $X = U \cap S$ にしましょう。 $H = G_X$ を示します。明らかに、$G_X \subset H$です。一方、$u \in U$ と $(s_1, \ldots, s_q)$ を、あなたの分解を減じたものとします。コル。 Thの3。 2 は $C(s_j) \subset H$ を意味し、したがって $1 \leq j \leq q$ は $s_j \in X$ であることを意味します。したがって、$u \in W_X$、H は $u \in U$ の $C(u)$ の和集合であるため、$H \subset G_X$ が得られ、b) が証明されます。

主張 c) および d) は、W_X (§ 1, no. 8、Th. 2) の類似の特性から導き出されます。

#### 系 {#lie-iv-s2-n5-cor-1 .statement tag=0ANK}

集合 S は元 $w \in W$ で構成され、$w \neq 1$ と $B \cup C(w)$ は G の部分群になります。

$B \cup C(w)$ が G の部分群であるような元 $w \in W$ は、$W_X = \{1, w\}$ とともに $X \subset S$ が存在するものです。さらに、$w \neq 1$ の場合、必然的に Card(X) = 1、つまり $w \in S$ になります。

#### 注意 1 {#lie-iv-s2-n5-rem-1 .statement tag=0ANL}

上記の系は、S が (G, B, N) によって決定されることを示しています。このため、私たちはときどき、(G, B, N) はおっぱい系である、または (B, N) は G のおっぱい系であると言うことができます。

#### 命題 1 {#lie-iv-s2-prop-1 .statement tag=0ANM}

X を S の部分集合とし、W の像が W_X に等しい N' 部分群とします。すると、(G_X, B, N', X) はおっぱい系です。

$G_X = BW_XB = BN'B$ があります。これは、$G_X$ が $B \cup N'$ によって生成されることを示しています。公理 (T1) ～ (T4) の検証は現在明らかです。

#### 命題 2 {#lie-iv-s2-prop-2 .statement tag=0ANN}

X、Y ⊂ S、および $w \in W$ とします。私たちは持っています

$$
G_X w G_Y = BW_X w W_Y B.
$$

$s_1, \ldots, s_q \in X$と$t_1, \ldots, t_q \in Y$としましょう。 補題 1 は次のことを示しています
$$
C(s_1 \ldots s_q).C(w).C(t_1 \ldots t_q) \subset BW_X w W_Y B,
$$
そしてそれゆえに
$$
G_X w G_Y \subset BW_X w W_Y B.
$$
逆の包含は明らかです。

#### 注意 2 {#lie-iv-s2-n5-rem-2 .statement tag=0ANO}

$G_X \backslash G / G_Y$ 集合、部分集合、$G$、形、$G_X g G_Y$、$g \in G$ で表します。同様に、定義する $W_X \backslash W / W_Y$ も同様です。前述の命題は、正規の全単射 $w \mapsto C(w)$ が $W$ から $B \backslash G / B$ 定義するへ、商 a *全単射* $W_X \backslash W / W_Y \to G_X \backslash G / G_Y$ に至ることを示しています。

#### 命題 3 {#lie-iv-s2-prop-3 .statement tag=0ANP}

*$X \subset S$と$g \in G$としましょう。 関係 $g B g^{-1} \subset G_X$ は $g \in G_X$ を意味します。*

$w \in W$ を $g \in C(w)$ となるようにします。 $B$ は $G_X$ の部分群であるため、仮定 $g B g^{-1} \subset G_X$ は $C(w).C(w^{-1}) \subset G_X$ を意味し、したがって Cor による $C(w) \subset G_X$ を意味します。 Thの3。 2 なので、$g$ 属するから $G_X$ となります。

### 6. パラボリック部分群

#### 定義 2 {#lie-iv-s2-def-2 .statement tag=0ANQ}

* $G$ の部分群は、$B$ の含む共役であれば放物線であると言われます。

すべての部分群、含むの放物線部分群が放物線であることは明らかです。

#### 命題 4 {#lie-iv-s2-prop-4 .statement tag=0ANR}

*$P$を$G$の部分群とします。*

a) *$P$ は、$P$ が共役から $G_X$ であるような $S$ の部分集合 $X$ が存在する場合に限り、放物線になります ($G_X$ の定義に対して cf. no. 5)。

b) *$X, X' \subset S$ と $g, g' \in G$ を $P = g G_X g^{-1} = g' G_{X'} {g'}^{-1}$ となるようにします。次に、$X = X'$ と $g' g^{-1} \in P$ です。*

主張 a) Th から続きます。 3、b)。
b) の仮説の下では、次のようになります。
$$
g^{-1} g' B {g'}^{-1} g \subset g^{-1} g' G_{X'} {g'}^{-1} = G_X,
$$
そして提案 3 は $g^{-1} g' \in G_X$ を示しています。したがって、Th による $G_{X'} = G_X$ と $X' = X$ です。 3、b)。最後に、
$$
g' g^{-1} = g . g^{-1} g' . g^{-1} \in g G_X g^{-1},
$$
これは b) を証明します。

放物線部分群 $P$ が共役から $G_X$ で、$X \subset S$ である場合、$P$ は *型 X* であると言われます。

#### 定理 4 {#lie-iv-s2-thm-4 .statement tag=0ANS}

(i) $P_1$ と $P_2$ を共通部分が放物線である $G$ の 2 つの放物線部分群とし、$g \in G$ を $gP_1g^{-1} \subset P_2$ となるようにします。続いて$g \in P_2$と$P_1 \subset P_2$。

(ii) 共通部分が放物線である 2 つの放物線部分群は共役ではありません。

(iii) $Q_1$と$Q_2$を、$G$の部分群$Q$に含まれる$G$の2つの放物線部分群とする。次に、$gQ_1g^{-1} = Q_2$ 属するから $Q$ のような任意の $g \in G$ です。

(iv) すべての放物線部分群は独自のノーマライザー $^6$ です。

主張 (i) は Props から続きます。 3 と 4 は (ii) を意味します。 (iii) の仮説では、$gQ_1g^{-1} \subset Q$ が得られますが、これは (i) によって $g \in Q$ を意味します。最後に、(iv) は (iii) から$Q_1 = Q_2 = Q$ を取得して続きます。

#### 命題 5 {#lie-iv-s2-prop-5 .statement tag=0ANT}

$P_1$ と $P_2$ を $G$ の 2 つの放物線部分群とします。次に、$T$の$P_1 \cap P_2$含む共役。

まず、$P_1$ と $P_2$ を $G$ の内部自己同型で変換すると、$B \subset P_1$ と仮定できます。 $g \in G$ を $gB_2g^{-1} \subset P_2$ となるようにします。 Thさんより1、$g = bn b'$となるような$n \in N$と$b, b' \in B$が存在します。 $N$では$T$が正常なので、

$$
P_2 \supset gB_2g^{-1} = bnBn^{-1}b^{-1} \supset bnTn^{-1}b^{-1} = bTb^{-1}
$$

そして

$$
P_1 \supset B \supset bTb^{-1},
$$

これは命題を証明します。

### 7. シンプルさ定理

#### 補題 2 {#lie-iv-s2-lem-2 .statement tag=0ANU}

$H$ を $G$ の通常の部分群とします。 $BH = G_X$ であり、$X$ のすべての要素が $S - X$ のすべての要素と交換できるような、$S$ のサブセット $X$ が存在します。

$BH$ は $G$ 含む $B$ の部分群であるため、$BH = G_X$ (Th. 3) のような $S$ のうちの一意の部分集合 $X$ が存在します。

$s_1 \in X$ と $s_2 \in S - X$ としましょう。 $n_1$と$n_2$をそれぞれ$s_1$と$s_2$の$N$の代表とします。次に、$n_1 \in G_X = BH$ が存在し、$bn_1 \in H$ となるような $b \in B$ が存在します。 $G$では$H$が正常なので、$G$の属するから$H$の元$h = n_2 b n_1 n_2^{-1}$となります。これはつまり、

$$
h \in C(s_2).C(s_1).C(s_2).
$$

$s_2 s_1 s_2$ の長さが 3 に等しい場合、Cor. Thの1 2 は次のことを意味します

$$
C(s_2).C(s_1).C(s_2) = C(s_2 s_1 s_2),
$$

(6) $H$ が群 $G$ の部分群である場合、$G$ の $H$ の正規化子は部分群 $\mathfrak{N}(H)$ からなる元 $g$ $G$ $gHg^{-1} = H$ のようになります。 部分群 $H'$ は、$H' \subset \mathfrak{N}(H)$ の場合に $H$ を正規化すると言われています。この場合、$HH' = H'H$ は $G$ の部分群で、$H$ が正規です。

したがって $h \in H \cap C(s_2 s_1 s_2)$ です。 $H \cap C(s_2 s_1 s_2)$ は空ではないので、$s_2 s_1 s_2 \in W_X$ です。 $(s_2, s_1, s_2)$ は縮小された分解であるため、仮定とは反対に、$s_2 \in X$ になります。

したがって、$l_S(s_2 s_1 s_2) \leq 2$; $l_S(s_2 s_1 s_2) = 1$ の場合は $s_1 s_2 \in S$ となり、$(s_1 s_2)^2 = 1$ または $s_1 s_2 = s_2 s_1$ となります。 $l_S(s_2 s_1 s_2) = 2$ の場合、§1, no. 5 の性質 (E) は、$s_1 \neq s_2$ 以降、$s_2 s_1 = s_1 s_2$ を意味します。 Q.E.D.

Th には、群 U の次の性質が入ります。以下の5:

(R) *U とは異なる U の通常の部分群 V について、交換子部分群* (cf. *代数*、章 I, §6, no. 8) *U/V は U/V* とは異なります。

すべての可溶性群は (R) を満たします。特に、すべてのアーベル群は (R) を満たします。対称群 $\mathfrak{S}_n$ が (R) を満たすことがわかります (cf. 例題 29)。

#### 定理 5 {#lie-iv-s2-thm-5 .statement tag=0ANV}

*Z を B の共役の共通部分とし、U を B の部分群とし、G_1 を G の U の共役によって生成された部分群とします。次の仮定を作成します。

(1) *U は B で正常であり、B = UT*。
(2) *U には性質 (R)* があります。
(3) *G_1 はその交換子部分群* に等しい。
(4) *コクセター 系 (W, S) は既約* (cf. §1, no. 9) です。

*すると、G_1 で正規化された G のすべての部分群 H は、Z または含む G_1* に含まれます。

*最初に G = G_1 T* を示します。 群 $G_1 T$ 含む B なので、それ自体のノーマライザー (Th. 4) です。しかし、N が $G_1$ と T を正規化すると、$G_1 T$ も正規化されるため、$N \subset G_1 T$ になります。 G は B と N によって生成されるので、$G = G_1 T$ になります。

*次は、集合*

$$
G' = G_1 H, \quad B' = B \cap G', \quad N' = N \cap G',
T' = T \cap G' = B' \cap N' \quad \text{and} \quad W' = N'/T'.
$$

$G'$ 含む $G_1$ から $G = G'T$ があり、したがって $N = N'T$ になります。 N に $N'$ を含めると、定義する、移行から商、同型 $\alpha : W' \to W$ になります。 $S' = \alpha^{-1}(S)$ にしましょう。

*今、(G', B', N', S') がシジュウカラ系* であることを示します。 $G = BNB$と$B = TU = UT$なので、$G = UNU$になります。 U は $G'$ の部分群であるため、$G' = UN'U$ となります。 $U \subset B'$ 以降、これは (T1) を証明します。 $\alpha$ が同型であるため、公理 (T2) は満たされます。 $w \in W$ と $w' = \alpha^{-1}(w)$ を $W'$ の対応する元とします。私たちは持っています

$$
BwB = BwB' = Bw'B', \quad \text{since } B = B'T.
$$

これから、結論するから $G' \cap BwB = B'w'B'$ になります。これは、移行から商全単射上の G 定義するに $G'$ が含まれることを意味します。

B'\setminus G'/B' から B\setminus G/B まで。公理 (T3) がすぐに続きます。公理 (T4) は B = B'T から得られます。

部分群 G'ではHが正常です。 補題 2 を (G', B', N', S') に適用すると、B'H = G'_X' となるような S' の部分集合 X' が存在し、S' - X' のすべての元は、X' のすべての元と可換になります。 仮定 (4) を考慮すると、可能性は 2 つだけです。

a) X' = \varnothing、つまり B'H = B' なので、H \部分集合 B' \部分集合 B. g \in G の場合、g = g_1 t、g_1 \in G_1、t \in T、および H \部分集合 g_1 B g_1^{-1} になります。G_1 は H を正規化しているためです。 H \部分集合 g B g^{-1}、Z は g B g^{-1} の共通部分なので、H \部分集合 Z が得られます。

b) X' = S'、つまり B'H = G'。 G = G'T なので、次のようになります。

$$ G = B'HT = HB'T = HB. $$

B が U を正規化すると、U のすべての共役は、h \in H を持つ形 hUh^{-1} になります。そのような部分群は群 UH に含まれるため、G_1 の定義によって G_1 \部分集合 UH になります。したがって、同型となります。

$$ U/(U \cap H) \cong UH/H = G_1 H/H \cong G_1/(G_1 \cap H). $$

仮定 (3) により、G_1/(G_1 \cap H) はその交換子部分群に等しくなります。 仮定 (2) は、群 U/(U \cap H) が G_1/(G_1 \cap H)、簡約するから単位元と同型であることを示しています。したがって、G_1 \cap H = G_1 および G_1 \部分集合 H となり、証明が完成します。

#### 系 {#lie-iv-s2-n7-cor-1 .statement tag=0ANW}

Th の仮定の下にあります。 5、群 G_1/(G_1 \cap Z) は単純な非アーベル行列か、簡約する ～ 単位元のいずれかです。

Th. 5 は、G_1/(G_1 \cap Z) が単純であること、または簡約する ～ 単位元であることを示しています。一方、仮定 (3) は、交換子部分群と等しいことを意味します。したがって系です。

#### 注意 1 {#lie-iv-s2-n7-rem-1 .statement tag=0ANX}

仮定 (2)、(3)、(4) は、(G'、B'、N'、S') がおっぱいであるという証明では使用されていません系。

#### 注意 2 {#lie-iv-s2-n7-rem-2 .statement tag=0ANY}

Z \cap U = \{1\} と仮定します。 B では Z と U が正規であるため、Z のすべての元は U のすべての元と可換となり、したがって G_1 のすべての元と可換になります。前述の系を考慮すると、G_1 \cap Z は G_1 の中心であることがわかります。

#### 注意 3 {#lie-iv-s2-n7-rem-3 .statement tag=0ANZ}

仮定 (3) は次の条件によって暗示されます。

(3') U は、u \in U と b \in B \cap G_1 を使用して交換子 b^{-1} u^{-1} b u によって生成されます。

#### 例 1 {#lie-iv-s2-n7-exa-1 .statement tag=0AO0}

k を体、n 整数 \geqslant 0、G = \mathbf{GL}(n, k) とし、(G, B, N, S) を no. 2 で説明したおっぱい系とします。 U を、G の厳密に上三角部分群、つまり、対角要素が 1 に等しい B の部分群行列のからなるとします。 Th の条件 (1)。 5 は明らかであり、U は可溶なので (2) も同様です。 条件 (4) は、$n \geq 2$ であれば満たされます。 $n \geq 3$ とカード$(k) \geq 4$ であれば (3) が満たされることを示すことができます (cf. *代数*、章 II, § 10、演習 13)。これらの条件の下で、$G_1 / (G_1 \cap Z)$ は *単純* であり、$G_1 \cap Z$ は $G_1$ (cf. *注意* 2) の中心であることが結論するわかります。

$k$ が可換の場合、$G_1 = \mathbf{SL}(n, k)$ (cf. *代数*、III, § 8, no. 9 章)。

#### 例 2 {#lie-iv-s2-n7-exa-2 .statement tag=0AO1}

$g$ を $\mathbf{C}$ 上の単純なリー代数とし、$G$ を $g$ の内部自己同型の群とします (cf. 章 III, § 6, no. 2、提案 2)。 Th を使用することによって。 5、$G$ が単純な非アーベルであることを示すことができます。*

### 練習問題 {#lie-iv-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
