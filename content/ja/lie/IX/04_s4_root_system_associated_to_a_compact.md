---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 4
section_title: Root system associated to a compact group
lang: ja
source: lie-vii-ix
book_pages: 304-324, 396-405
pdf_pages: 0311-0331, 0403-0412
extraction: native+ocr
subsections:
    - "no": 1
      title: THE GROUP X(H)
      page: 304
      pdf_page: 311
    - "no": 2
      title: NODAL GROUP OF A TORUS
      page: 305
      pdf_page: 312
    - "no": 3
      title: WEIGHTS OF A LINEAR REPRESENTATION
      page: 307
      pdf_page: 314
    - "no": 4
      title: ROOTS
      page: 309
      pdf_page: 316
    - "no": 5
      title: NODAL VECTORS AND INVERSE ROOTS
      page: 311
      pdf_page: 318
    - "no": 6
      title: FUNDAMENTAL GROUP
      page: 314
      pdf_page: 321
    - "no": 7
      title: SUBGROUPS OF MAXIMAL RANK
      page: 316
      pdf_page: 323
    - "no": 8
      title: ROOT DIAGRAMS
      page: 317
      pdf_page: 324
    - "no": 9
      title: COMPACT LIE GROUPS AND ROOT SYSTEMS
      page: 319
      pdf_page: 326
    - "no": 10
      title: AUTOMORPHISMS OF A CONNECTED COMPACT LIE GROUP
      page: 322
      pdf_page: 329
statements: 60
exercises: 22
content_sha256: 896110693e96b77318d02d2a9eaa7d089391b32391b4503fcbb435687991bd2b
translated_from: content/en/lie/IX/04_s4_root_system_associated_to_a_compact.md
translation_method: google
source_content_sha256: e5b8a3582b57fb78f4dd12b6e9730ed0ae0bc70a11963071c72fa1b2877b4759
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: c769bbeed00e3b6d314e24ee44feaaece1c3c6514da0a5b0cb5edc9df5aa159e
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 4。 根系はコンパクト群に関連付けられています

パラグラフ 4 から 8 では、結合したコンパクト・リー群を G で、G の最大値トーラスを T で表します。 G (T) の $\mathfrak{g}$ (それぞれ $\mathfrak{t}$) リー代数を、複雑化したもの $\mathfrak{g}_{\mathbf{C}}$ (それぞれ $\mathfrak{t}_{\mathbf{C}}$) で表します。 $\mathfrak{g}$ のリー代数 (それぞれ $\mathfrak{t}$)、および W による T (§2, no. 5) に対する G のワイル群。

### 1. 群 X(H)

H をコンパクト・リー群とします。 H から位相的群 $\mathbf{C}^*$ までの連続準同型の (可換) 群を X(H) で表します。 章著。 III, §8, no. 1、木。 1、X(H)の元はリー群の射です。すべての $a\in X(H)$ について、$a$ の微分は $\mathbf{R}$ 線形写像 $L(a) : L(H)\rightarrow L(\mathbf{C}^*)$ です。 これから、$\mathbf{C}^*$ の指数写像が $\mathbf{C}$ から $\mathbf{C}^*$ までの写像 $z \rightarrow e^z$ と一致するように、$\mathbf{C}^*$ と $\mathbf{C}$ のリー代数を識別します。 次に、任意の元 $a\in X(H)$ に元 $L(a)\in$ Hom$_{\mathbf{R}}(L(H),\mathbf{C})$ が関連付けられます。ホム$_{\mathbf{C}}(L(H)_{(\mathbf{C})},\mathbf{C})$の$\delta (a)$元によって、それに対する対応するが表されます（つまり、$L(H)\subset L(H)_{(\mathbf{C})}$に対する制限が$L(a)$に等しい）。

すべての $x\in L(H)$ とすべての $a\in X(H)$ について、

$a$(exp$_Hx$) $=e^{\delta(a)(x)}$,

指数写像の関数性による (第 III, §6, no. 4 章、提案 10)。

群 X(H) を加法的に表すことがよくあります。この場合、$\mathbf{C}^*$ の元 $a(g)$ を $g^a$ で表します。この記法により、 公式が得られます

$$
g^{a+b}=g^ag^b,g\in H, a, b\in X(H)
$$

そして

(経験値$_Hx$)$^a=e^{\delta(a)(x)}, x\in L(H), a\in X(H)$。

H はコンパクトなので、X(H) の元は、絶対値値 1 の複素数の部分群 $\mathbf{U}=\mathbf{U}(1,\mathbf{C})$ に値が含まれるため、X(H) は連続 (または解析的) の群と識別できます。 準同型 H から $\mathbf{U}$ まで。したがって、すべての $a\in L(H)$、写像 $L(a)$ は、$\mathbf{C}$ の部分空間 $\mathbf{R}i$ に値がかかるため、$\delta (a)$ 写像 L(H) から $\mathbf{R}i$ になります。

H が可換である場合、X(H) は単純に H の (離散) 双対群です (スペクトル理論、II, §1, no. 1 章)。 If H is commutative and finite, X(H) can be identified with the dual finite group D(H) = Hom$_{\mathbf{Z}}(H,\mathbf{Q}/\mathbf{Z})$ (where, as in Algebra, Chap. VII, §4, no. 9, Example 1, we identify $\mathbf{Q}/\mathbf{Z}$ with a subgroup of $\mathbf{C}^*$ by the homomorphism $r \rightarrow$ exp(2$\pi ir$)).

コンパクト・リー群の任意の射 $f: H\rightarrow H'$ について、$X(H')$ から X(H) までの$X(f)$ 準同型 $a \rightarrow a\circ f$ で表します。 K が閉じた場合

通常のコンパクト・リー群 H の部分群、$\mathbf Z$ の完全系列モジュールがあります
$$
0\longrightarrow X(H/K)\longrightarrow X(H)\longrightarrow X(K).
$$

#### 命題 1 {#lie-ix-s4-prop-1 .statement tag=01JH}

— *任意のコンパクト・リー群* H について、*その* $\mathbf Z$-*加群* $X(H)$ * は有限型です。 * H * が接続されていれば無料です。

まず、H が接続されていると仮定します。 $X(H)$ のすべての元は H の導来群 $D(H)$ で消えるので、準同型 $X(H/D(H))\longrightarrow X(H)$ になります。 But $H/D(H)$ is connected and commutative, hence is a torus, and $X(H/D(H))$ is a free $\mathbf Z$-module of finite type (*Spectral Theories*, Chap. II, §2, no. 1, Cor. 2 of Prop. 1). 一般的なケースでは、数列の正確さから次のようになります。
$$
0\longrightarrow X(H/H_0)\longrightarrow X(H)\longrightarrow X(H_0),
$$
ここで、$X(H_0)$ は有限型を含まず、$X(H/H_0)$ は有限であるため、$X(H)$ は有限型を含みます。

#### 命題 2 {#lie-ix-s4-prop-2 .statement tag=01JI}

— *H を可換コンパクト・リー群とし、* $(a_i)_{i\in I}$ * $X(H)$ の元の族とする。 ** $a_i$ *生成する* $X(H)$ ** $\operatorname{Ker}a_i$ *簡約するから単位元の共通部分の場合に限ります。*

*スペクトル理論*著、第4章II, §1, no. 7、木曜日。 4、$a_i$の核の直交補数は、$a_i$によって生成された$X(H)$の部分群$A_i$です。 *locによって。引用*、Cor. Thの2。 4 の場合、$\bigcap\operatorname{Ker}a_i$ の直交補数は $A_i$ によって生成された $X(H)$ の部分群であるため、命題になります。

### 2. ノード群/トーラス

トーラス S の * 節点群* は、$\Gamma(S)$ で示され、指数関数写像 $\mathscr L(S)\longrightarrow S$ の核です。これは、$\mathscr L(S)$ の離散部分群であり、その階数は S の次元に等しく、$\mathbf R$ 線形写像 $\mathbf R\otimes_{\mathbf Z}\Gamma(S)\longrightarrow\mathscr L(S)$ は、$\Gamma(S)$ の拡大する標準単射を $\mathscr L(S)$ に変換します。全客観的です。 商同型への通路で誘導する
$$
\mathbf R/\mathbf Z\otimes_{\mathbf Z}\Gamma(S)\longrightarrow S.
$$

たとえば、$\mathbf U$ のノード群 $\Gamma(\mathbf U)$ は、$\mathscr L(\mathbf U)=i\mathbf R$ の部分群 $2\pi i\mathbf Z$ です。

トーリ $f:S\longrightarrow S'$ の任意の射について、$L(f)$ によって誘導される $\Gamma(f)$ 準同型 $\Gamma(S)\longrightarrow\Gamma(S')$ で表します。可換図式があります
$$
\begin{array}{ccccccccc}
0&\longrightarrow&\Gamma(S)&\longrightarrow&\mathscr L(S)&\xrightarrow{\exp_S}&S&\longrightarrow&0\\
&&\downarrow{\Gamma(f)}&&\downarrow{\mathscr L(f)}&&\downarrow f&&\\
0&\longrightarrow&\Gamma(S')&\longrightarrow&\mathscr L(S')&\xrightarrow{\exp_{S'}}&S'&\longrightarrow&0.
\end{array}
\tag{1}
$$

$a\in X(S)$ にしましょう。 a で定義される S から $\mathbf U$ までの適用から射までを見ると、 no. 1 写像 $\Gamma(S)$ から $2\pi i\mathbf Z$ の $\mathbf C$ 線形写像 $\delta(a):\mathscr L(S)_{\mathbf C}\longrightarrow\mathbf C$ がわかります。したがって、次のようにすることで、$X(S)\times\Gamma(S)$ 上で $\mathbf Z$ 双線形形式を定義する作成できます。
$$
\langle a,X\rangle=\frac{1}{2\pi i}\delta(a)(X),\qquad a\in X(S),\quad X\in\Gamma(S).
\tag{2}
$$

#### 命題 3 {#lie-ix-s4-prop-3 .statement tag=01BP}

$X(S)\times \Gamma (S)$ の双線形形式 $(a, X) \rightarrow  \langle a, X\rangle$ は反転可能です。

Recall (Algebra, Chap. IX) that, by definition, this means that the linear maps $X(S)\rightarrow$ Hom$_{\mathbf{Z}}(\Gamma (S),\mathbf{Z})$ and $\Gamma (S)\rightarrow$ Hom$_{\mathbf{Z}}(X(S),\mathbf{Z})$ associated to this bilinear form are bijective.

命題の結論が 2 つの鳥に当てはまる場合、積にも当てはまります、というのが明らかです。したがって、次元 $n$ のすべてのトーラスは $\mathbf{U}^n$ と同型であるため、$S =\mathbf{U}$ の場合に帰着します。この特定のケースでは、主張は明らかです。

$f: S\rightarrow S'$をトリの射とします。次に、線形写像 $X(f) : X(S')\rightarrow X(S)$ と $\Gamma (f) :\Gamma (S)\rightarrow \Gamma (S')$ のそれぞれは、もう一方の転置です。つまり、すべての $a'\in X(S')$ とすべての $X\in \Gamma$(S) について、

$$
\langle X(f)(a'), X\rangle =\langle a', \Gamma (f)(X)\rangle \tag{3}
$$

#### 命題 4 {#lie-ix-s4-prop-4 .statement tag=01BQ}

Sと$S'$をトリとする。 S から $S'$ まで、$M(S,S')$ 群、射、リー群で表します。 写像 $f \rightarrow X(f)$ と $f \rightarrow \Gamma (f)$ は、それぞれ$M(S,S')$ からホム$_{\mathbf{Z}}(X(S'),X(S))$ とホム$_{\mathbf{Z}}(\Gamma (S), \Gamma (S'))$ までの群の同型です。

$f$ が S から $S'$ までのリー群の射である場合、準同型 $X(f)$ は、スペクトル理論の意味で単に $f$ の双対です。 II, §1, no. 7。 写像 $\varphi  \rightarrow \widehat{\varphi}$ Hom$_{\mathbf{Z}}(X(S'),X(S))$ から $M(S,S')$ まで loc で定義されています。引用。 $M(S,S')$ から Hom$_{\mathbf{Z}}(X(S'),X(S))$ までの写像 $f \rightarrow X(f)$ の逆数です。したがって、後者は全単射です。 同一視する $\Gamma (S)$ (それぞれ $\Gamma (S')$) を X(S) (それぞれ $X(S')$) のデュアル $\mathbf{Z}$ モジュールで (提案 $3$) $,\Gamma (f)$ 一致すると転置準同型 $X(f)$ なので、命題です。

#### 注意 1 {#lie-ix-s4-n2-rem-1 .statement tag=01BR}

$f$ : S $\rightarrow S'$ をトリの射とします。 (1) に関連付けられたヘビ図式 (代数、章 X, §1, no. 2) は完全系列を与えます

0 $\longrightarrow$ カー$\Gamma (f)\longrightarrow$ カー $L(f)\longrightarrow$ カー $f\longrightarrow^d$ (4)

$\longrightarrow^d$ コーカー $\Gamma (f)\longrightarrow$ コーカー $L(f)\longrightarrow$ コーカー $f\longrightarrow 0$。

特に、$f$ が有限の核 N を持つ全射であると仮定すると、完全系列が得られます。

0 $\longrightarrow$ N $\longrightarrow^i$ S $\longrightarrow^fS'\longrightarrow 0$、

ここで、$i$ は標準単射です。次に、$L(f)$ は全単射であり、(4) は同型 $N\rightarrow$ コーカー $\Gamma (f)$ を与えるので、完全系列

0 $\longrightarrow \Gamma (S)\overset{\Gamma(f)}{\longrightarrow}\Gamma (S')\longrightarrow$ N $\longrightarrow 0$。 (5)

さらに、スペクトル理論、Chap. II, §1, no. 7、木曜日。 4、数列

0 $\longrightarrow X(S')\overset{X(f)}{\longrightarrow}$ X(S) $\longrightarrow^{X(i)}$ X(N) $\longrightarrow$ 0 (6)

正確です。

#### 注意 2 {#lie-ix-s4-n2-rem-2 .statement tag=01BS}

提案 4 により、$M(\mathbf{U},S)$ から $\Gamma (S)$ までの写像 $f \rightarrow \Gamma (f)(2\pi i)$ は同型です。 $a\in X(S) = M(S,\mathbf{U})$ と $f\in M(\mathbf{U},S)$ の場合、合成 $a\circ f\in M(\mathbf{U},\mathbf{U})$ は自己準同型 $u \rightarrow u^r$ で、$r=\langle a, \Gamma (f)(2\pi i)\rangle$ です。これからは $\mathbf{Z}$ とともに同一視する $M(\mathbf{U},\mathbf{U}) = X(\mathbf{U})$ となり、$\mathbf{Z}$ の元 $r$ は自己準同型 $u \rightarrow u^r$ に関連付けられます。したがって、上記の記法では、

$$
a\circ f=\langle a, \Gamma (f)(2\pi i)\rangle
$$

#### 注意 3 {#lie-ix-s4-n2-rem-3 .statement tag=01BT}

正確な数列 $0\rightarrow \Gamma (S)\rightarrow L(S)\longrightarrow^{exp_S}S\rightarrow 0$ は、$\Gamma (S)$ から S の基本群への同型写像に関連付けられており、続編では正準と呼ばれます。 トーリ $f: S\rightarrow S',\Gamma (f)$ の任意の射については、標準同型 $\Gamma (S)\rightarrow \pi_1(S)$ および $\Gamma (S')\rightarrow \pi_1(S')$ と、$f$ によって誘導される準同型 $\pi_1(f) :\pi_1(S)\rightarrow \pi_1(S')$ を介して識別できます。 Note that this gives another interpretation of the exact sequence (5) (cf. General Topology, Chap. XI, in preparation).

#### 注意 4 {#lie-ix-s4-n2-rem-4 .statement tag=01BU}

$\mathbf{Z}$-モジュール $\delta : X(S)\rightarrow$ Hom$_{\mathbf{C}}(L(S)_{(\mathbf{C})},\mathbf{C})$ および $\iota :\Gamma (S)\rightarrow L(S)_{(\mathbf{C})}(\iota$ の準同型は、$\Gamma (S)$ の標準単射によって $\mathbf{C}$ ベクトル空間の L(S)) 拡大するから同型に誘導されます。

$u:\mathbf{C}\otimes X(S)\rightarrow$ オム$_{\mathbf{C}}(L(S)_{(\mathbf{C})},\mathbf{C})$

$$
v:\mathbf{C}\otimes \Gamma (S)\rightarrow L(S)_{(\mathbf{C})}
$$

続編ではこれを正規と呼ぶことにします。 $\mathbf{C}$ の線形性によって X(S) と $\Gamma (S)$ の間のペアリングを $(\mathbf{C}\otimes X(S))\times (\mathbf{C}\otimes \Gamma$(S) の双線形形式 $\ll ,\gg$ に拡大するすると、次のようになります。

$$
\langle u(a), v(b)\rangle = 2\pi i\ll a, b\gg
$$

### 3. 線型表現中重み

この数 $k$ は、体 $\mathbf{R}$ または $\mathbf{C}$ のいずれかを表します。

V を $k$ 上の有限次元ベクトル空間とし、$\rho : G\rightarrow \mathbf{G}\mathbf{L}(V)$ を V 上の接続されたコンパクトなリー群 G の連続 (したがって実解析的、第 III, §8, no. 1 章、第 1 章) 表現とします。 定義する複素数ベクトル空間 $\widetilde{V}$ と連続表現 $\widetilde{\rho}: G\rightarrow \mathbf{G}\mathbf{L}( \widetilde{V})$ は次のようになります: $k=\mathbf{C}$、集合 $\widetilde{V} = V, \widetilde{\rho}=\rho$ の場合。 $k=\mathbf{R}$、集合 $\widetilde{V} = V_{(\mathbf{C})}$、$\widetilde{\rho}$ が $\rho$ と標準準同型 $\mathbf{G}\mathbf{L}(V)\rightarrow \mathbf{G}\mathbf{L}( \widetilde{V})$ の合成である場合。

For all $\lambda \in X(G)$, denote by $\widetilde{V}_{\lambda}(G)$ the vector subspace of $\widetilde{V}$ consisting of the $v\in \widetilde{V}$ such that $\widetilde{\rho}(g)v=g^{\lambda}v$ for all $g\in G$ (cf. Chap. VII, §1, no. 1). ロケ地にて。前述の提案 3、$\widetilde{V}_{\lambda}(G)$ の和 ($\lambda$ 所属から X(G) について) は直接的です。 さらに：

#### 補題 1 {#lie-ix-s4-lem-1 .statement tag=01BV}

G が可換である場合、$\widetilde{V}$ は $\lambda \in X(G)$ に対する $\widetilde{V}_{\lambda}(G)$ の直和です。

$\rho$は半単純(§1, no. 1)なので、$\rho$が単純な場合は補題を証明すれば十分です。その場合、End( $\widetilde{V}$) 簡約するの $\rho (G)$ の交換子環 Z が相同関係 (代数、Chap. VIII, §3, no. 2、Th. 1) になります。従って、準同型 $\widetilde{\rho}$ の像は GL( $\widetilde{V}$) の部分群 $\mathbf{C}^*.1_V$ に含まれ、$\widetilde{V} = \widetilde{V}_{\lambda}(G)$ となるような $\lambda \in X(G)$ が存在します。

#### 定義 1 {#lie-ix-s4-def-1 .statement tag=01BW}

G の最大トーラス T に対して、G の表現 $\rho$ の重みは、$\widetilde{V}_{\lambda}(T)\not= 0$ となる X(T) の元 $\lambda$ です。

$P(\rho ,T)$、または T の選択、T に対する $\rho$ の重みの集合について混同の可能性がない場合は $P(\rho )$ で表します。 補題 1 によって、

$$
\widetilde{V} =\bigoplus_{\lambda\in P(\rho ,T)}\widetilde{V}_{\lambda}(T) \tag{7}
$$

$T'$ を、(Int $g$)$T = T'($§2, no. 2 となるような G の他の最大値トーラスと G の $g$ 元とする。 2)。 $\lambda \in X(T)$ 全員にとって、

$\widetilde{\rho}(g)( \widetilde{V}_{\lambda}(T)) = \widetilde{V}_{\lambda'}(T')$、ここで $\lambda '=$ X(Int $g^{-1}$)$(\lambda )$。 (8)

その結果、

X(整数 $g$)$(P(\rho ,T')) = P(\rho ,T)$。 (9)

ワイル群 $W = W_G(T)$ は、$\mathbf{Z}$ モジュール X(T) の左側で $w \rightarrow X(w^{-1})$ によって動作します。従って、$t\in T, \lambda \in X(T), w\in W$ については、$t^{w\lambda}= (w^{-1}(t))^{\lambda}$ になります。

#### 命題 5 {#lie-ix-s4-prop-5 .statement tag=01BX}

集合 $P(\rho ,T)$ は、ワイル群 W の演算の下で安定しています。$n\in N_G(T)$ とし、$w$ を W の類とします。 $\lambda \in X(T)$ の場合、$\rho (n)( \widetilde{V}_{\lambda}(T)) = \widetilde{V}_{w\lambda}(T)$ と薄暗い $\widetilde{V}_{w\lambda}(T) =$ 薄暗い $\widetilde{V}_{\lambda}(T)$ があります。

公式 (9) は、$T'= T, g=n$ とともに、$P(\rho ,T)$ が $w$ の下で安定していることを意味します。さらに、$\widetilde{V}_{\lambda}(T)$ から $\widetilde{V}_{w\lambda}(T)$ までの $\widetilde{\rho}(n)$ 誘導する同型 (公式 (8))、したがって命題です。

#### 命題 6 {#lie-ix-s4-prop-6 .statement tag=01BY}

準同型 $\rho : G\rightarrow \mathbf{G}\mathbf{L}(V)$ は、$P(\rho ,T)$ 生成するの $\mathbf{Z}$ モジュール X(T) の場合にのみ単射的です。

準同型 $\rho$ は、T に対する制限が単射である場合にのみ単射です (§2, no. 6、提案 9)。さらに、標準準同型 $\mathbf{G}\mathbf{L}(V)\rightarrow \mathbf{G}\mathbf{L}( \widetilde{V})$ は単射なので、$\widetilde{\rho}$ により置き換える $\rho$ ができます。次に、(7) から、T に対する $\rho$ の制限の核は、$P(\rho ,T)$ の元の核の共通部分であることがわかります。従って、no. 1 の提案 2 から結論が得られます。

$\mathfrak{g}\mathfrak{l}( \widetilde{V})$ の $\mathfrak{t}$ の線型表現 $L(\rho )$ $\mathbf{C}$ の拡大するから準同型まで - リー代数

$$
\widetilde{L}(\rho ) :\mathfrak{t}_{\mathbf{C}}\rightarrow \mathfrak{g}\mathfrak{l}( \widetilde{V})
$$

さらに、$\mathfrak{t}_{\mathbf{C}}$ 上の X(T) 線型形式 $\delta (\lambda )$ のすべての元 $\lambda$ に次のように関連付けた (no. 1) を思い出してください。

(経験値$_Tx$)$^{\lambda}=e^{\delta(\lambda)(x)},x\in \mathfrak{t}$。 (10)

Recall finally (Chap. VII, §1, no. 1) that, for any map $\mu:\mathfrak{t}_{\mathbf{C}}\rightarrow \mathbf{C}$, we denote by $\widetilde{V}_\mu(\mathfrak{t}_{\mathbf{C}})$ the vector subspace of $\widetilde{V}$ consisting of the $v$ such that $(\widetilde{L}(\rho )(u))(v) =\mu(u).v$ for all $u\in \mathfrak{t}_{\mathbf{C}}$.

次に、(7) から推定して loc を求めます。引用、提案 3:

#### 命題 7 {#lie-ix-s4-prop-7 .statement tag=01BZ}

a) すべての $\lambda \in X(T)$ に対して、$\widetilde{V}_{\lambda}(T) = \widetilde{V}_{\delta(\lambda)}(\mathfrak{t}_{\mathbf{C}})$ があります。

b) マップ $\delta : X(T)\rightarrow$ Hom$_{\mathbf{C}}(\mathfrak{t}_{\mathbf{C}},\mathbf{C})$ は、$P(\rho ,T)$ から$\widetilde{V}$ の$\mathfrak{t}_{\mathbf{C}}$ の重みセットへの全単射を引き起こします。

注意まず、W が自己準同型 $L(w)_{(\mathbf{C})}$ の W のいずれかの元 $w$ の $\mathfrak{t}_{\mathbf{C}}$ に関連付けて $\mathfrak{t}_{\mathbf{C}}$ で動作する場合、写像 $\delta$ は X(T) 上の W の演算と互換性があります。ホム$_{\mathbf{C}}(\mathfrak{t}_{\mathbf{C}},\mathbf{C})$。

ここで$k=\mathbf{R}$と仮定します。 V の $x, y$ に対して $\sigma (x+iy) =x-iy$ によって定義される、V に対する $\widetilde{V}$ の共役を $\sigma$ で示します。すべての複素数ベクトル部分空間 $\widetilde{V}$ の E、$\widetilde{V}$ の最小の部分空間は、$\mathbf{R}$ および含む E より有理で、$E +\sigma (E)$ です。 特に、すべての $\lambda \in X(T)$ について、$\widetilde{V}$ の部分空間 $V(\lambda )_{(\mathbf{C})}$ が $\widetilde{V}_{\lambda}(T) + \widetilde{V}_{-\lambda}(T)$ ($\sigma ( \widetilde{V}_{\lambda}(T)) = \widetilde{V}_{-\lambda}(T)$ であることに注意してください) となるような、V の実数ベクトル部分空間 $V(\lambda )$ が存在します。 $V(\lambda ) = V(-\lambda )$ があり、$V(\lambda )$ は、$\rho$ によって誘発された V 上の T の表現の同型成分です。

### 4. 根

T を基準とした G の根は、G の随伴表現の非ゼロ重みです。T を基準とした G の根の集合は、$R(G,T)$ で示されるか、混乱の危険がない場合は単に R で示されます。提案 6、写像による

$$
\delta : X(T)\rightarrow \mathfrak{t}^*_{\mathbf{C}}
$$

$(\mathfrak{t}^*_{\mathbf{C}}$ は、分裂還元的代数 $(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ の集合 $R(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ 根への複素数ベクトル空間 $\mathfrak{t}_{\mathbf{C}})$ 写像 $R(G,T)$ の双対を表します。 VIII, §2, no. 2、注意 4)。入れたら

$$
\mathfrak{g}^{\alpha}= (\mathfrak{g}_{\mathbf{C}})_{\alpha}(T) = (\mathfrak{g}_{\mathbf{C}})_{\delta(\alpha)}(\mathfrak{t}_{\mathbf{C}}) \tag{11}
$$

すべての $\alpha \in R$ について、各 $\mathfrak{g}^{\alpha}$ は $\mathbf{C}($loc に対して次元 1 になります。前掲書、Th. 1) そして

$$
\mathfrak{g}_{\mathbf{C}}=\mathfrak{t}_{\mathbf{C}}\oplus \bigoplus_{\alpha\in R}\mathfrak{g}^{\alpha} \tag{12}
$$

それぞれの $\alpha \in R$ について、$V(\alpha )_{(\mathbf{C})}=\mathfrak{g}^{\alpha}+\mathfrak{g}^{-\alpha}$ となるような $\mathfrak{g}$ の 2 次元部分空間を $V(\alpha )$ で表します。 T の随伴表現に対する $\mathfrak{g}$ の非ゼロ同型成分は $\mathfrak{t}$ と $V(\alpha )$ です。さらに、K を $\mathfrak{g}$ の Killing 形に関連付けられた 2 次式形とします。それは否定的であり (§1, no. 3、提案 1)、その制限 $K(\alpha )$ から $V(\alpha )$ は否定的で分離しています。 T の各元 $t$ に対して、Ad $t$ は $K(\alpha )$ を安定させ、したがってリー群の射を与えます。

$$
\iota_{\alpha}: T\rightarrow \mathbf{S}\mathbf{O}(K(\alpha ))
$$

$\iota_{\alpha}=\rho_{\alpha}\circ \alpha$ のような固有の同型 $\rho_{\alpha}:\mathbf{U}\rightarrow \mathbf{S}\mathbf{O}(K(\alpha ))$ が存在します。実際、$X$ を $\mathfrak{g}^{\alpha}$ の非ゼロ元とし、$\mathfrak{g}$ に対する $\mathfrak{g}_{\mathbf{C}}$ の共役の下で、$Y$ を $X$ の像とします。次に$Y\in \mathfrak{g}^{-\alpha}$、$U=X+Y, V=i(X-Y)$を入れると$V(\alpha )$の基底$(U, V)$が得られます。 基底 $(U, V)$ に関して、広告 $t,t\in T$ によって誘導された $V(\alpha )$ の自己準同型の行列は、

$$
(\mathscr{R}(t^{\alpha})-\mathscr{I}(t^{\alpha}))
$$

$$
\mathscr{I}(t^{\alpha})\mathscr{R}(t^{\alpha})
$$

したがって主張です。

#### 命題 8 {#lie-ix-s4-prop-8 .statement tag=01C0}

Q(R) を G の根によって生成された X(T) の部分群とします。

a) G の中心 C(G) は T の閉じた部分群であり、根の核の共通部分に等しい。正規の写像 $X(T/C(G))\rightarrow X(T)$ は像 Q(R) と単射です。

b) コンパクト群 C(G) は、離散群 $X(T)/Q(R) ($ スペクトル理論の双対と同型です。 II, §1, no. 1、デフォルト。 2)。

c) Q(R) が X(T) に等しい場合に限り、C(G) 簡約するから単位元まで。

§2, no. 2 著、Cor. Thの2。 2、C(G)はTに含まれています。これは随伴表現の核なので、根の核の共通部分、他の語の部分群Q(R)の直交補数です。 X(T)。したがって、命題はスペクトル理論、第 4 章から続きます。 II, §1, no. 7、木。 4とno. 5、Th。 2.

#### 命題 9 {#lie-ix-s4-prop-9 .statement tag=01C1}

リー群 G のすべての自己同型、T 上の恒等式誘導するは、形 Int $t$ で、$t\in T$ です。

まず、C(G) 簡約する ～ 単位元、その他の語では、X(T) = Q(R) であると仮定します (提案 8)。 $f$ を T 上の恒等性を誘導する G の自己同型とし、$\varphi = L(f)_{(\mathbf{C})}$ とします。すると、$\varphi$ は $\mathfrak{g}_{\mathbf{C}}$ の自己同型となり、$\mathfrak{t}_{\mathbf{C}}$ に同一性が生じます。章著。 VIII, §5, no. 2、提案 2、各 $\mathfrak{g}^{\alpha}$ ホモテティー に $\varphi$ 誘導するが比 $\theta (\alpha )$ となるような一意な準同型 $\theta : Q(R)\rightarrow \mathbf{C}^*$ が存在します。 $\varphi$ は$\mathfrak{g}_{\mathbf{C}}$ の実数形 $\mathfrak{g}$ を安定に残すので、$\mathfrak{g}$ に関して$\mathfrak{g}_{\mathbf{C}}$ の活用$\sigma$ と可換です。でも$\sigma (\mathfrak{g}^{\alpha}) =\mathfrak{g}^{-\alpha}$なので、$\alpha \in R$全員に対して$\theta (-\alpha ) =\overline{\theta(\alpha)}$です。これは$\theta (\alpha )\theta (\alpha ) =\theta (\alpha )\theta (-\alpha ) = 1$を意味します。したがって、$\theta$ は $\mathbf{U}$ で値を取り、したがって双対性により対応するは T の元 $t$ となり、 (Ad $t$)$_{(\mathbf{C})}=\varphi$ となるため、Int $t=f$ となります。

一般的なケースでは、上記の内容は群 $G/C(G)$、その中心簡約するから単位元、そしてその最大値トーラス $T/C(G)$ に適用されます。 その結果、$f$ が T 上で恒等性を誘導する G の自己同型である場合、$f$ と Int $t$ が商への通過によって $G/C(G)$ の同じ自己同型を誘導するような T の要素 $t$ が存在することになります。 しかし、正規の射 $D(G)\rightarrow G/C(G)$ は有限のカバー (§1, no. 4、提案 4 の Cor. 1) であるため、$f$ と Int $t$ 誘導するは D(G) の同じ自己同型、したがって $D(G)\times C(G)$、したがって G の同じ自己同型となります (loc.引用）。

#### 系 {#lie-ix-s4-n4-cor-1 .statement tag=01C2}

$u$をGの自己同型、HをGの閉じた部分群、$u$の固定点のからなるとします。次に、$H_0$ が最大階数である場合に限り、自己同型 $u$ は内部になります。

$u$ が Int $g$ に等しい場合、$g\in G$ では、部分群 $H_0= Z(g)_0$ は最大階数 (§2, no. 2、Cor. 3) になります。逆に、H 含むが最大トーラス S である場合、自己同型 $u$ は $s\in S$ により形 Int $s$ になります (提案 9)。

### 5. 節ベクトルとその逆根

#### 補題 2 {#lie-ix-s4-lem-2 .statement tag=01C3}

S を T の閉じた部分群とし、Z(S) を G の正規化子とします。

(i) $R(Z(S)_0,T)$ は、$\alpha (S) =\{1\}$ となるような $\alpha \in R(G,T)$ の集合です。

(ii) $Z(S)_0$ の中心は、$\alpha \in R(Z(S)_0,T)$ の Ker$\alpha$ の共通部分です。

(iii) S が接続されている場合は、Z(S) が接続されます。

リー代数 $L(Z(S))_{(\mathbf{C})}$ は、$\mathfrak{g}_{\mathbf{C}}$ 上の S の不変量から構成されます (章 III, §9, no. 3、提案 8)。したがって、$\mathfrak{t}_{\mathbf{C}}$ の直和と $\alpha (S) =\{1\}$ に対する $\mathfrak{g}^{\alpha}$ であるため、(i) になります。 主張 (ii) は提案 8 (no. 4) から導かれ、主張 (iii) はすでに証明されています (§2, no. 2、Th. 2 の Cor. 5)。

#### 定理 1 {#lie-ix-s4-thm-1 .statement tag=01C4}

$\alpha \in R(G,T)$ にしましょう。 $\alpha$の核のセントラライザー$Z_{\alpha}$は、Gの接続された閉じた部分群です。その中心はカー$\alpha$です。その導来群 $D(Z_{\alpha}) = S_{\alpha}$ は、階数 1 の G の接続された閉じた半単純部分群です。$R(Z_{\alpha},T) =\{\alpha ,-\alpha \}$ と dim $Z_{\alpha}=$ dim T + 2 があります。

$Z'_{\alpha}$ を (Ker $\alpha$ )$_0$ の中心化者とします。 補題 2 により、これは G の接続された閉じた部分群であり、$R(Z'_{\alpha},T)$ は $\beta$((Ker$\alpha$ )$_0$) $=\{1\}$ となるように $\beta \in R(G,T)$ の集合です。明らかに、$\{\alpha ,-\alpha \} \subset R(Z'_{\alpha},T)$です。逆に、$\beta \in R(Z'_{\alpha},T)$ とします。 (Ker $\alpha$ )$_0$ は Ker $\alpha$ の有限添字であるため、$t\in$ Ker $\alpha$ に対して $t^{r\beta}= 1$ となる整数 $r\not= 0$ が存在します。 数列の正確さから

$0\longrightarrow \mathbf{Z}\longrightarrow X(T)\longrightarrow$ X(カー$\alpha$ )$\longrightarrow 0$

二元性による対応するから完全系列

0 $\longrightarrow$ カー$\alpha \longrightarrow$ T $\longrightarrow^{\alpha}\mathbf{U}\longrightarrow 0$、

したがって、$r\beta$ は $\alpha$ の倍数です。章著VIII, §2, no. 2、木曜日。 2 (i)、これは $\beta \in  \{\alpha ,-\alpha \}$ を意味します。したがって、$R(Z'_{\alpha},T) =\{\alpha ,-\alpha \}$。 (補題 2) から、$Z'_{\alpha}$ の中心は Ker$\alpha$ であるため、$Z'_{\alpha}= Z_{\alpha}$ になります。最後に、Cor.提案 4 の 1 (§1, no. 4)、$D(Z_\alpha)$ は、$G$ の接続された閉じた半単純部分群です。 $\mathscr{L}(Z_\alpha)(\mathbf C)=\mathfrak{g}^\alpha+\mathfrak{g}^{-\alpha}+[\mathfrak{g}^\alpha,\mathfrak{g}^{-\alpha}]$ なので、階数 $1$ です。

#### 系 {#lie-ix-s4-n5-cor-1 .statement tag=01C7}

— *次のプロパティを持つリー群* $\nu:\mathbf{SU}(2,\mathbf C)\to G$ の射が存在します:*

a) *像 of* $\nu$ *核 of* $\alpha$ と通勤します。

b) *すべて* $a\in\mathbf U$、*私たちは*
$$
\nu\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}\in\mathbf T
\quad\text{and}\quad
\alpha\circ\nu\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}=a^2.
$$

*もし* $\nu_1$ *と* $\nu_2$ *が 2 つの射から* $\mathbf{SU}(2,\mathbf C)$ *から* $G$ *前述のプロパティを使用すると、* $a\in\mathbf U$ *次のような* が存在します。
$$
\nu_2=\nu_1\circ\operatorname{Int}
\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}.
$$

Thさんより§3, no. 6の1と提案6、リー群の射が存在します
$$
\nu:\mathbf{SU}(2,\mathbf C)\to S_\alpha
$$
それは離散核で全射です。この場合、$\nu^{-1}(\mathbf T\cap S_\alpha)$ は $\mathbf{SU}(2,\mathbf C)$ の最大値トーラスになります (§2, no. 3、提案 1)。 $\mathbf{SU}(2,\mathbf C)$ の最大トーラスは共役 (§2, no. 2, Th. 2) であるため、必要に応じて置き換えること $\nu$ $\nu\circ\operatorname{Int}s$ ($s\in\mathbf{SU}(2,\mathbf C)$ を使用)、$\nu^{-1}(\mathbf T\cap S_\alpha)$ は対角線行列の群であると仮定できます。 $\mathbf{SU}(2,\mathbf C)$に。それから
$$
\nu\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}\in\mathbf T
$$
$a\in\mathbf U$ と写像全員に
$$
\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}
\longmapsto
\alpha\circ\nu\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}
$$
は $\mathbf{SU}(2,\mathbf C)$ の根であるため、2 つの写像の 1 つに等しい
$$
\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}\longmapsto a^2
$$
または
$$
\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}\longmapsto a^{-2}
$$
(§3, no. 6、公式 (19))。最初のケースでは、準同型 $\nu$ には必要なプロパティがあります。 2 番目のケースでは、準同型 $\nu\circ\operatorname{Int}\theta$ がそれらを持っています (上記引用、公式 (18))。

$\nu_1$ と $\nu_2$ が $\mathbf{SU}(2,\mathbf C)$ から $G$ 満たすまでの 2 つの射である場合、条件は両方とも写像 $\mathbf{SU}(2,\mathbf C)$ から $S_\alpha$ (条件 a)) となるため、両方とも$S_\alpha$。 したがって、$\nu_2=\nu_1\circ\varphi$ となるような$\mathbf{SU}(2,\mathbf C)$ の自己同型$\varphi$ が存在し、no. 4 の提案 9 を使用して結論を​​導き出します。

前述の系から、$\mathbf U$ から $\mathbf T$ までの準同型 $\nu_{\mathbf T}$ は次のように定義されます。
$$
\nu_{\mathbf T}(a)=\nu\begin{pmatrix}a&0\\0&\bar a\end{pmatrix}
$$
$a\in\mathbf U$ については、選択または $\nu$ から独立しています。 元の$\Gamma(\nu_{\mathbf T})$、$\Gamma(\mathbf U)=2\pi i\mathbf Z$の$2\pi i$の下の$K_\alpha\in\Gamma(\mathbf T)$像で表します。それは、根* $\alpha$ に関連付けられた *節ベクトルと呼ばれます。 We have $\langle\alpha,K_\alpha\rangle=2$, in other words (no. 2, formula (2)) $\delta(\alpha)(K_\alpha)=4\pi i$; since $K_\alpha$ belongs to the intersection of $\mathfrak t$ and the $\mathscr L(S_\alpha)(\mathbf C)$, we have
$$
K_\alpha=2\pi iH_{\delta(\alpha)},
\tag{13}
$$
where $H_{\delta(\alpha)}$ is the *inverse root associated to the root* $\delta(\alpha)$ of $(\mathfrak g_{\mathbf C},\mathfrak t_{\mathbf C})$ (Chap. VIII, §2, no. 2). 他の語では、$\Gamma(\mathbf T)\otimes\mathbf R$がペアリングを介して$X(T)\otimes \mathbf{R}$の双対と同一視されると、$\langle ,\rangle ,K_{\alpha}$はその逆の根$\alpha^{\vee}\in (X(T)\otimes \mathbf{R})^*$と同一視されます。

#### 注意 {#lie-ix-s4-n5-rem-1 .statement tag=01C5}

$x\in \mathbf{R}$ の皆様には、

$($ exp(2$\pi ix$) 0 $)_{2\pi ix}$

$\nu$ 0 exp($-2\pi ix$)$=\nu_T(e$ ) = exp($xK_{\alpha}$)。 (14)

特に：

$\nu (-0$1 $-01)=\nu_T(-1) =$ 経験値$(\frac{1}{2}K_{\alpha})$。 (15)

したがって、$\nu$ は $K_{\alpha}\notin2\Gamma$(T) の場合にのみ単射的であり、他の語では $\langle \lambda , K_{\alpha}\rangle \notin2\mathbf{Z}$ となるような $\lambda \in X(T)$ が存在する場合に限ります。 When $\mathfrak{g}_{\mathbf{C}}$ is simple, $\nu$ is injective unless $\mathfrak{g}_{\mathbf{C}}$ is of type $B_n, C(G) =\{1\}$ and $\alpha$ is a short root (cf. Chap. VI, Plates).

この段落の残りの部分では、$\alpha \in R(G,T)$ に対して節ベクトル $K_{\alpha}$ の $R^{\vee}(G,T)$ 集合で表します。 これは、$\Gamma (T)$ の $\mathfrak{t}_{\mathbf{C}}$ への標準注入により、$\delta (R)$ の逆根系 $R^{\vee}(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}}) =\{H_{\delta(\alpha)}\}$ の比率 $2\pi i$ との相似性が識別される、$\Gamma (T)$ のサブセットです。 したがって、$R^{\vee}(G,T)$ 生成するは $\mathbf{R}$ ベクトル空間 $L(T\cap D(G))$ であるため、X(T) の直交補数は $X(T/(T\cap D(G)))$ になります。

Aut(T) 群 of 自己同型 of リー群 T で表します。 Weyl 群 $W = W_G(T) ($§2, no. 5) は Aut(T) の部分群と識別できます。 On the other hand, recall (Chap. VIII, §2, no. 2, Remark 4) that the Weyl group $W(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ of the split reductive algebra $(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ operates on $\mathfrak{t}_{\mathbf{C}}$, and thus is canonically identified with a subgroup of $\mathbf{G}\mathbf{L}(\mathfrak{t}_{\mathbf{C}})$.

#### 命題 10 {#lie-ix-s4-prop-10 .statement tag=01C6}

写像 $u \rightarrow L(u)_{(\mathbf{C})}$ Aut(T) から $\mathbf{G}\mathbf{L}(\mathfrak{t}_{\mathbf{C}})$ 誘導する同型 W から分解的簡約リー代数 $(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ のワイル群まで。すべての $\alpha \in R$ について、$W_{Z_{\alpha}}(T)$ は位数 2 であり、$W_{Z_{\alpha}}(T)$ の非同一要素の前の同型の下にある像は反映 $s_{H_{\delta(\alpha)}}$ です。

検討中の写像は単射的です。その像が $W(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ に等しいことを示す必要があります。

$g\in N_G(T)$ にしましょう。第15章の記法とVIII, §5, no. 2、Ad $g\in$ Aut($\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}}$)$\cap$ Int($\mathfrak{g}_{\mathbf{C}}$) があるため、Ad $g\in$ Aut$_0(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}}) ($loc になります。引用、no. 5、提案 11)。ロケ地にて。引用、no. 2、提案 4、広告 $g$ 属するから $W(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ によって誘導された $\mathfrak{t}_{\mathbf{C}}$ の自己同型。したがって、$\mathbf{G}\mathbf{L}(\mathfrak{t}_{\mathbf{C}})$のWの像は$W(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$に含まれます。

$\alpha \in R(G,T)$ を、Cor のプロパティを持つリー群の射を $\nu :\mathbf{S}\mathbf{U}(2,\mathbf{C})\rightarrow G$ とします。 Thの。 1. $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ の要素 $\theta$ の $\nu$ の下の画像は次の性質を持ちます (§3, no. 6、式 (17))。

a) (Int$\nu (\theta )$)$(t) =t$ $t\in$ Ker$\alpha$ の場合、

b) (Int$\nu (\theta )$)$(t) =t^{-1}$ $t\in T\cap S_{\alpha}$ の場合。

したがって、Ker $\delta (\alpha )\subset \mathfrak{t}_{\mathbf{C}}$ 上の Ad $\nu (\theta )$ 誘導するのアイデンティティ、および $[\mathfrak{g}^{\alpha},\mathfrak{g}^{-\alpha}]$ 上の誘導する写像 $x \rightarrow  -x$ であるため、反射 $s_{H_{\delta(\alpha)}}$ を伴う一致するになります。したがって、W 含むの像はすべて $s_{H_{\delta(\alpha)}}$ であるため、$W(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ に等しくなります。特に、$W_{Z_{\alpha}}(T)$ は位数 2 であるため、単位と Int $\nu (\theta )$ で構成されます。これで命題の証明が完了です。

#### 系 {#lie-ix-s4-n5-cor-2 .statement tag=01JJ}

G が半単純であると仮定します。すると、G のすべての元は、G の 2 つの元の交換子になります。

$c$ をワイル群 $W(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ (章 V, §6, no. 1) のコクセター変換とし、$n$ を $N_G(T)$ の元とし、W の類は、で定義された同型によって $c$ と識別されます。 命題。 T から T まで $f_c$ 射 $t \rightarrow (n, t)$ で表します。 $x\in \mathfrak{t}_{\mathbf{C}}$ の場合、$L(f_c)_{(\mathbf{C})}(x) =$ (広告 $n$)$(x)-x=$ $c(x)-x$ があります。

Thさんより第1章$\mathfrak{t}_{\mathbf{C}}$ の V, §6, no. 2、自己準同型 $c$ には 1 に等しい固有値がありません。従って、$L(f_c)$ は全射であり、従って $f_c$ も同様です。従って、T のすべての元は、G の 2 つの元の交換子であり、Th から見ると系を意味します。 2、§2, no. 2。

### 6. 基本群

次の命題において、$f(G,T)$は$\Gamma (T)$から$\pi_1(G)$までの準同型を表します。これは、$\Gamma (T)$から$\pi_1(T)$までの標準同型（no. 2、注意3）と準同型の合成です。 $\pi_1(\iota )$、$\iota$ は標準単射 $T\rightarrow G$ です。

#### 命題 11 {#lie-ix-s4-prop-11 .statement tag=01C8}

準同型 $f(G,T) :\Gamma (T)\rightarrow \pi_1(G)$ は全射です。その核は、節ベクトル $(K_{\alpha})_{\alpha\in R(G,T)}$ の家族によって生成された $\Gamma (T)$ の部分群 $N(G,T)$ です。

準同型 $f(G,T)$ は、提案 3 (§2, no. 4) により全射です。 $A(G,T)$ 主張で表します: 「$f(G,T)$ の核は $K_{\alpha}$ によって生成されます」。これはまだ証明されておらず、いくつかのケースを区別します。

$a) G$は単純接続です。 $\rho :\mathfrak{g}_{\mathbf{C}}\rightarrow \mathfrak{g}\mathfrak{l}(V)$ を有限次元複素数ベクトル空間 V 上の $\mathfrak{g}_{\mathbf{C}}$ の線型表現とします。 $\mathfrak{g}$ に限定すると、実数ベクトル空間 $V_{(\mathbf{R})}$ で $\mathfrak{g}$ の表現が得られます。 G は単純結合なので、$\rho = L(\pi )$ となるような $V_{(\mathbf{R})}$ 上の G の解析的線型表現 $\pi$ が存在します。 no. 3 の提案 7 から、$\mathfrak{t}^*_{\mathbf{C}}$ 含むの X(T) の像 $\delta (X(T))$ は、V の $\rho$ のすべての重みになります。これは、$\mathfrak{g}_{\mathbf{C}}$ のすべての表現 $\rho$ に当てはまります。 VIII, §7, no. 2、木曜日。 1 $\delta$(R) の重みの $\delta (X(T))$ 含む群、これは $\lambda \in \mathfrak{t}^*_{\mathbf{C}}$ の定義集合によるもので、他のすべての $\alpha \in R$ に対して $\lambda (H_{\delta(\alpha)})\in \mathbf{Z}$ になります。 $\alpha \in R$ 全員に対して語、$\lambda (K_{\alpha})\in 2\pi i\mathbf{Z}$。従って、群 X(T) 含む $X(T)\otimes \mathbf{Q}$ のすべての元 $\lambda$ は、すべての $\alpha \in R$ に対して $\langle \lambda , K_{\alpha}\rangle  \in \mathbf{Z}$ となり、双対性によって $\Gamma (T)$ が $K_{\alpha}$ によって生成されることを意味します。 主張 $A(G,T)$。

$b) G$ は、単純に接続された群 $G'$ とトーラス S の直接積です。そのとき、T は、$S,\Gamma (T)$ を持つ $G'$ の最大トーラス $T'$ の直接積です。 $\Gamma (T')\times \Gamma$(S)、$\pi_1(G)$と$\pi_1(G')\times \pi_1$(S)、$f(G,T)$と準同型、成分、$f(G',T')$、$f(S,S)$。 $f(S,S)$ は全単射なので、正準写像 $\Gamma (T')\rightarrow \Gamma (T)$ 写像 Ker $f(G',T')$ は Ker $f(G,T)$ に全単射されます。さらに、G の導来群 $G'$ の $K_{\alpha}$ 属するからリー代数なので、$\Gamma (T')$ の像となるので、$A(G',T')$ は $A(G,T)$ を意味するので、明らかになります。 主張 $A(G,T)$、a) を考慮して。

c) 一般的なケース。有限核を持つ全射射$p: G'\rightarrow G$が存在します。ここで、$G'$はトーラスによる単純結合群の直接積です(§1, no. 4、提案4)。 $T'$ が $G'$ の T の逆像 (これは、§2, no. 3 による $G'$ の最大値トーラス、提案 1)、および $p$ の N 核である場合、完全系列 $0\rightarrow N\rightarrow G'\rightarrow G\rightarrow 0$ が得られ、 $0\rightarrow N\rightarrow T'\rightarrow T\rightarrow 0$、したがって、正確な行を持つ可換図式 (no. 2、注意 1 および一般位相、第 XI、準備中)

0 $\longrightarrow \Gamma (T')\longrightarrow \Gamma (T)\longrightarrow$ N $\longrightarrow$ 0

$f(G',T')f(G,T)$ ID$_N$

0 $\longrightarrow \pi_1(G')\longrightarrow \pi_1(G)\longrightarrow$ N $\longrightarrow 0$。

ヘビ図式 (代数、章 X、p. 4、提案 2) からすぐに、$A(G',T')$ は $A(G,T)$ を意味するので、b) を考慮すると命題が得られます。

#### 系 1 {#lie-ix-s4-prop-11-cor-1 .statement tag=01C9}

G は、家族 $(K_{\alpha})_{\alpha\in R(G,T)}$ 生成する $\Gamma (T)$ の場合にのみ単純接続されます。

#### 系 2 {#lie-ix-s4-prop-11-cor-2 .statement tag=01CA}

H を G 含む T の接続された閉じた部分群とします。 完全系列があります

$$
0\longrightarrow N(H,T)\longrightarrow N(G,T)\longrightarrow \pi_1(H)\longrightarrow \pi_1(G)\longrightarrow 0
$$

これは代数章の続きです。 X、p. 4、提案 2 (ヘビ図式)、可換式図式に適用

0 $\longrightarrow N(H,T)\longrightarrow \Gamma (T)\longrightarrow \pi_1(H)\longrightarrow$ 0

0 $\longrightarrow N(G,T)\longrightarrow \Gamma (T)\longrightarrow \pi_1(G)\longrightarrow 0$。

#### 注意 {#lie-ix-s4-n6-rem-1 .statement tag=01CB}

$\pi_2(G/H)$ は零であることが示されます (cf. 練習問題 2 of §5)。前述の数列の正確性により、$\pi_2(G/H)$ から $N(G,T)/N(H,T)$ までの同型が得られます。

#### 系 3 {#lie-ix-s4-prop-11-cor-3 .statement tag=01CC}

準同型 $\pi_1(D(G))\rightarrow \pi_1(G)$ 対応する $\pi_1(D(G))$ から $\pi_1(G)$ の捩れ部分群までの G 誘導する同型に D(G) を含めること。

実際、$T\cap D(G)$ は D(G) (§2, no. 3, Prop. $1c$)$)$ の最大トーラスです。 完全系列から

$$
0\longrightarrow \Gamma (T\cap D(G))\longrightarrow \Gamma (T)\longrightarrow \Gamma (T/(T\cap D(G)))\longrightarrow 0
$$

命題 11 の場合、完全系列が得られます

$$
0\longrightarrow \pi_1(D(G))\longrightarrow \pi_1(G)\longrightarrow \Gamma (T/(T\cap D(G)))\longrightarrow 0
$$

したがって、$\pi_1(D(G))$ は有限であり、$\Gamma (T/(T\cap D(G)))$ は自由であるため、系となります。

### 7. 最大階数のうち部分群

Recall (Chap. VI, §1, no. 7) that a subset P of $R = R(G,T)$ is said to be closed if $(P + P)\cap R\subset P$, and symmetric if $P =-P$.

#### 命題 12 {#lie-ix-s4-prop-12 .statement tag=01CD}

$\mathscr{H}$ を、包含順に並べた G 含む T の接続された閉じた部分群の集合とします。 写像 $H \rightarrow R(H,T)$ は、$R(G,T)$ の対称閉対称部分集合の $\mathscr{H}$ から集合までの増加する全単射を包含順に並べたものです。

$H\in \mathscr{H}$ の場合、$L(H)_{(\mathbf{C})}$ は $\mathfrak{t}_{\mathbf{C}}$ の直和であり、$\alpha \in R(H,T)$ の $\mathfrak{g}^{\alpha}$ です。これは $\mathfrak{g}_{\mathbf{C}}$ の還元的部分代数であるため、R の部分集合 $R(H,T)$ は前述の条件を満たします (章 VIII, §3, no. 1、補題 2 および提案 2)。 逆に、P が R 満たすこれら条件の部分集合である場合、$\mathfrak{t}_{\mathbf{C}}\oplus \sum_{\alpha\in P}\mathfrak{g}^{\alpha}$ は部分代数です

$\mathfrak{g}_{\mathbf{C}}($場所の。これは、$\mathbf{R}$ (no. 3) に対して有理であり、したがって形 $\mathfrak{h}_{(\mathbf{C})}$ についても有理です。ここで、$\mathfrak{h}$ は $\mathfrak{g}$ の部分代数です。 H(P) を $\mathfrak{h}$ で定義される G の積分部分群とします。閉まっています（§2, no. 4、注意1）。 写像 $H \rightarrow R(H,T)$ と $P \rightarrow H(P)$ が増加するであり、互いに逆であることをすぐに検証します。

#### 系 1 {#lie-ix-s4-prop-12-cor-1 .statement tag=01CE}

G 含む T の閉じた部分群は有限個だけあります。

H をそのような部分群とします。次に $H_0\in \mathscr{H}$、そして $\mathscr{H}$ は有限です。さらに、H は $N_G(H_0)$ 含む $H_0$ の部分群であり、$N_G(H_0)/H_0$ は有限です (§2, no. 4、提案 4 および注意 2)。

#### 系 2 {#lie-ix-s4-prop-12-cor-2 .statement tag=01CF}

H を G 含む T の連結閉部分群とし、$W^H_G(T)$ を R の部分集合 $R(H,T)$ の $W_G(T)$ の固定群とする。 群 $N_G(H)/H$ は剰余群 $W^H_G(T)/W_H(T)$ と同型である。

実際、$N_G$(H) に適用された§2, no. 5 の提案 7 から、$N_G(H)/H$ は $W_{N(H)}(T)/W_H$(T) と同型であり、$W_{N(H)}(T)$ は $W_G(T)$ の元の集合であり、$N_G(T)$ の代表は H を正規化します。 $n\in N_G$(T)、$w$ を $W_G(T)$ の類とします。章著。 III, §9, no. 4、提案 11、$n$ は、(Ad $n$)$(L(H)) = L(H)$ の場合に限り H を正規化します。 no. 3 の提案 5 を考慮すると、これは R の部分集合 $R(H,T)$ が $w$ の下で安定であること、したがって系であることも意味します。

#### 注意 1 {#lie-ix-s4-n7-rem-1 .statement tag=01CG}

群 $W^H_G(T)$ は、T の部分群 C(H) の $W_G(T)$ の固定群でもあります。これは、no. 4 の提案 8 から続きます。

#### 命題 13 {#lie-ix-s4-prop-13 .statement tag=01CH}

H を最大階数の G の接続された閉じた部分群とし、C をその中心とします。次に、G の C 含む中心であり、H は C のセントラライザーのアイデンティティ成分です。

H の最大値トーラスを S とします。G の中心は S に含まれるので、C に含まれます。 $L = Z(C)_0$を入れてください。これは G 含む H の接続された閉じた部分群であるため、最大値階数であり、その中心は C に等しい。 S に対する H の $R_H$ と $R_L$ 根系と L で表します。次に$R_H\subset R_L\subset R(G,S)$。 C(H) = C(L) であるため、提案 8 (no. 4) は等式 $Q(R_H) = Q(R_L)$ を意味します。しかし、$Q(R_H)\cap R_L= R_H$ (章 VI, §1, no. 7、提案 23)、したがって $R_H= R_L$ および H = L (提案 12)。

#### 注意 2 {#lie-ix-s4-n7-rem-2 .statement tag=01CI}

$C =\bigcap_{\alpha\in P}$ Ker$\alpha$ となるような G の最大トーラス S と $R(G,S)$ の部分集合 P が存在する場合、G の部分群 C は根基であるとします。 no. 5 の提案 13 と補題 2 から、接続閉の集合部分群の最大値階数から集合まで写像 $H \rightarrow C(H)$ 誘導する全単射が成り立ちます。 G の根基部分群逆全単射は写像 $C \rightarrow Z(C)_0$ です。

#### 系 {#lie-ix-s4-n7-cor-1 .statement tag=01CJ}

$T\cap gTg^{-1}\not= C(G)$ が G とは異なる G の閉じた解析部分多様体の数の和集合となるような $g\in G$ の集合。

確かに、$A_g= T\cap gTg^{-1}$ を入れてください。 $T\subset Z(A_g)$ と $gTg^{-1}\subset Z(A_g)$ があります。従って、$xTx^{-1}=gTg^{-1}($§2, no. 2 となるような $x\in Z(A_g)$ が存在します。 2)、これは $g\in Z(A_g).N_G(T)$ を意味します。 G 含む T の閉じた部分群の有限 (Cor. 1) 集合を $\mathscr{A}$ で表し、G とは区別し、X = $\bigcup_{H\in\mathscr{A}}H.N_G(T)$ とします。これは G の閉じた部分多様体の有限和集合であり、G とは異なります。$A_g\not= C(G)$ の場合は $Z(A_g)\in \mathscr{A}$、$g$ 属するから X になります。逆に、$H\in \mathscr{A}$ を使用して$g\in H.N_G$(T) の場合、$A_g$ 含む C(H) となるので、$A_g\not= C(G)$ (提案 13)。

#### 命題 14 {#lie-ix-s4-prop-14 .statement tag=01CK}

X を T の部分集合とし、$R_X$ を根 $\alpha \in R(G,T)$ の集合とし、$\alpha (X) =\{1\}$ とします。 群 $Z_G(X)/Z_G(X)_0$ は、$\alpha \in R_X$ の反射 $s_{\alpha}$ によって生成された部分群によって X を固定し、$W_G(T)$ の部分群の商と同型です。

$H = Z_G(X)$を入れてください。 $L(H)_{(\mathbf{C})}$ は Ad(X) によって固定された $\mathfrak{g}_{\mathbf{C}}$ の点の集合であるため、$\mathfrak{t}_{\mathbf{C}}$ の和と $\alpha (X) =\{1\}$ の $\mathfrak{g}^{\alpha}$ です。その結果、$R(H_0,T) =$ $R_X$ となり、$\alpha \in R_X$ の反射 $s_{\alpha}$ によって$W_{H_0}(T)$ が生成されます。 §2, no. 5 の提案 7 を適用するだけで十分です。

以下 (§5, no. 3, Th. 1) で、G が単純接続されており、X 簡約するが点に接続されている場合、セントラライザー Z(X) が接続されていることがわかります。

### 8. 根図式

#### 定義 2 {#lie-ix-s4-def-2 .statement tag=01CL}

根図式 (または、混乱の危険がない場合は、単に図式) は、トリプル $D = (M,M_0,R)$ です。ここで、:

(RD$_0$) $M$ は有限型の自由な $\mathbf{Z}$ 加群であり、部分加群 $M_0$ は M の直因子です。

(RD$_I$) $R$ は、$M; R\cup M_0$ 生成するの $\mathbf{Q}$ ベクトル空間 $\mathbf{Q}\otimes M$ の有限部分集合です。

(RD$_{II}$) すべての $\alpha \in R$ に対して、M の $\alpha^{\vee}(M_0) = 0,\alpha^{\vee}(\alpha ) = 2$ と自己準同型 $x \rightarrow x-\alpha^{\vee}(x)\alpha$ が R を安定に保つように、$M^*=$ Hom$_{\mathbf{Z}}(M,\mathbf{Z})$ の元 $\alpha^{\vee}$ が存在します。

章著。 VI, §1, no. 1、$M^*$ のすべての $\alpha \in R$ 元 $\alpha^{\vee}$ は、$\alpha$ によって一意に決定されます。 M の $s_{\alpha}$ 自己準同型 $x \rightarrow x-\alpha^{\vee}(x)\alpha$ で表します。さらに (引用箇所)、$\mathbf{Q}$ ベクトル空間 $\mathbf{Q}\otimes M$ は、R によって生成された $\mathbf{Q}\otimes M_0$ およびベクトル部分空間 V(R) の直和であり、 R は V(R) の根系です (引用、定義 1)。

R の元は、根図式 D の根 、$M^*$ の逆数根の元 $\alpha^{\vee}$ と呼ばれます。 M の自己同型 $s_{\alpha}$ によって生成される群は D のワイル群と呼ばれ、W(D) で表されます。 W(D) の元誘導する $M_0$ の同一性、および V(R) の誘導する根系 R のワイル群の変換。

#### 例 1 {#lie-ix-s4-n8-exa-1 .statement tag=01CM}

有限型 M の自由な$\mathbf{Z}$ モジュールごとに、トリプル $(M,M,\emptyset )$ は根図式です。

#### 例 2 {#lie-ix-s4-n8-exa-2 .statement tag=01CN}

$D = (M,M_0,R)$ が根図式の場合、$M^*_0$ を $M^*$ の V(R) の直交補数とし、$R^{\vee}$ を D の逆数根の集合とします。すると、$D^{\vee}= (M^*,M^*_0,R^{\vee})$ は次のようになります。 根図式は、D の逆関数と呼ばれます。すべての $\alpha \in R$ について、$M^*$ の対称性 $s_{\alpha^{\vee}}$ は、M の対称性 $s_{\alpha}$ の反比例自己同型です。 写像 $w \rightarrow^tw^{-1}$ は、W(D) から $W(D^{\vee})$ までの同型です。さらに、$V(R^{\vee})$ は$\mathbf{Q}$ ベクトル空間の双対$V(R), R^{\vee}$ と自然に同一視でき、その後 R の逆元根系と同一視されます。

$M^*$ の双対が M と識別される場合、$D^{\vee}$ の逆数図式は D と識別されます。

#### 例 3 {#lie-ix-s4-n8-exa-3 .statement tag=01CO}

$(\mathfrak{g},\mathfrak{h})$ を分裂還元的 $\mathbf{Q}$-リー代数、$M\subset \mathfrak{h}$ を許容格子とします (VIII, §12, no. 6 章、定義 1)。 $M_0$を、$(\mathfrak{g},\mathfrak{h})$の根と$H_{\alpha},\alpha \in R(\mathfrak{g},\mathfrak{h})$の$R^{\vee}$集合に直交するMの部分群とします。すると、$(M,M_0,R^{\vee})$ は根図式で、$(M^*,M^*_0,R(\mathfrak{g},\mathfrak{h}))$ はその逆数図式です。

#### 例 4 {#lie-ix-s4-n8-exa-4 .statement tag=01CP}

Let V be a vector space over $\mathbf{Q}$ and R a root system in V; denote by P(R) the group of weights of R and by Q(R) the group of radical weights of R (Chap. VI, §1, no. 9). すると、$(Q(R),0,R)$ と $(P(R),0,R)$ は根図式になります。 根図式 $(M,M_0,S)$ は、M が S によって生成される (それぞれ $M^*$ が $S^{\vee}$ によって生成される) 場合に限り、 形 $(Q(R),0,R)$ (それぞれ $(P(R),0,R)$) の図式と同型です。

P(R) 含む $Q(R), (X,0,R)$ のすべての部分群 X は根図式であり、同型までのすべての図式 $(M,M_0,S)$ は $M_0= 0$ であり、他の語は S有限添字のMの生成する部分群はこのようにして生じます。

The root diagram $(M,M_0,R)$ is said to be reduced if the root system R is reduced (in other words (Chap. VI, §1, no. 4) if the relations $\alpha , \beta \in R,\lambda \in \mathbf{Z}$, $\beta =\lambda \alpha$ imply that $\lambda = 1$ or $\lambda =-1$). 例の図式 1)と3)が減少します。

### 9. コンパクト・リー群と根系

前の数で紹介した用語を使用すると、数 4 と 5 の結果の重要な部分は、次の定理に要約できます。

#### 定理 2 {#lie-ix-s4-thm-2 .statement tag=01CQ}

a$) (X(T),X(T/(T\cap D(G)),R(G,T)))$ は、根図式を縮小したものです。そのワイル群は $w\in W$ に対する $X(w)$ で構成されます。 群 X(C(G)) は、$R(G,T)$ によって生成された部分群による X(T) の商と同型です。

b$) (\Gamma (T), \Gamma (C(G)_0),R^{\vee}(G,T))$ は削減された根図式です。そのワイル群は $w\in W$ の $\Gamma (w)$ で構成されます。 群 $\pi_1(G)$ は、$R^{\vee}(G,T)$ によって生成された部分群による $\Gamma (T)$ の商と同型です。

c) $\mathbf{Z}$ モジュール X(T) と $\Gamma (T)$ が他方の双対 (no. 2、提案 3) と同一視される場合、先行する根図式はそれぞれ他方の逆双と同一視されます。

$D^*(G,T)$ 図式 $(X(T),X(T/(T\cap D(G)),R(G,T)))$ および $D_*(G,T)$ 図式 $(\Gamma (T), \Gamma (C(G)_0),R^{\vee}(G,T))$ で表します。これらは、それぞれ G (T に対する) の反変図式および共変図式と呼ばれます。

#### 例 1 {#lie-ix-s4-n9-exa-1 .statement tag=01CR}

G が階数 1 の半単純である場合、$D^*(G,T)$ と $D_*(G,T)$ は必ず 2 つの図式 $\Delta_2= (\mathbf{Z},0,\{2,-2\})$、$\Delta_1= (\mathbf{Z},0,\{1,-1\})$ のいずれかと同型です。 G が $\mathbf{S}\mathbf{U}(2,\mathbf{C}), D_*(G,T)$ と同型の場合、(G は単純結合なので) は $\Delta_1$ と同型であるため、$D^*(G,T)$ は $\Delta_2$ と同型です。 G が $\mathbf{S}\mathbf{O}(3,\mathbf{R}), D^*(G,T)$ と同型の場合、($C(G) =\{1\}$ 以降) は $\Delta_1$ と同型であるため、$D_*(G,T)$ は $\Delta_2$ と同型です。

#### 例 2 {#lie-ix-s4-n9-exa-2 .statement tag=01CS}

G と $G'$ がそれぞれ最大トーラス T と $T'$ で 2 つ接続された 2 つコンパクト・リー群である場合、また $D^*(G,T) = (M,M_0,R)$ と $D^*(G',T') =$ $(M',M'_0,R')$ である場合、$D^*(G\times G',T\times T')$ は $(M\oplus M',M_0\oplus$ $M'_0,R\cup R')$ と識別できます。共変図式についても同様です。

#### 例 3 {#lie-ix-s4-n9-exa-3 .statement tag=01CT}

N を T の閉じた部分群、G の中心とし、$(M,M_0,R)$ を T に対する G の反変図式とします。すると、$T/N$ に対する $G/N$ の反変図式は $(M',M'_0,R)$ で識別できます。ここで、$M'$ は の部分群です。 $\lambda$ の M からなるは、$\lambda (N) =\{1\}$ と $M'_0= M'\cap M_0$ になります。

#### 例 4 {#lie-ix-s4-n9-exa-4 .statement tag=01CU}

同様に、N を有限のアーベル群および $\varphi :\pi_1(G)\rightarrow N$ 全射準同型とします。 Let $G'$ be the covering of G associated to this homomorphism; this is a connected compact Lie group, of which N is a central subgroup (General Topology, Chap. XI, in preparation), and G can be naturally identified with $G'/N$. $T'$ を $G'$ の最大値トーラス、つまり T の逆像とします。 $(P,P_0,S)$ が T に対する G の共変図式である場合、$T'$ に対する $G'$ の共変図式は $(P',P'_0,S)$ で識別できます。ここで、$P'$ は合成準同型 $\varphi \circ f(G,T) : P\rightarrow N$ の核です(cf. no. 6、提案 11)、および $P'_0= P_0\cap P'$。

#### 注意 1 {#lie-ix-s4-n9-rem-1 .statement tag=01CV}

$\mathfrak{c}$ を $\mathfrak{g}_{\mathbf{C}}$ の中心とします。次に$\mathfrak{c}= L(C(G))_{(\mathbf{C})}$。 T に対する G の図式と、還元的分裂代数 $(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}}):$ の直接および逆根系の間には、次の関係があります。

a) $\mathbf{C}\otimes \Gamma (T)$ から $\mathfrak{t}_{\mathbf{C}}$ までの正準同型性は、$\mathbf{C}\otimes \Gamma (C(G)_0)$ から $\mathfrak{c}$ までの全単射と $1\otimes R^{\vee}(G,T)$ から $2\pi i.R^{\vee}(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ までの全単射を引き起こします。

b) $\mathbf{C}\otimes X(T)$ から $\mathfrak{t}_{\mathbf{C}}$ の双対 $\mathfrak{t}^*_{\mathbf{C}}$ への正準同型性は、$\mathbf{C}\otimes X(T/(T\cap D(G)))$ から $\mathfrak{t}_{\mathbf{C}}\cap \mathscr{D}(\mathfrak{g})_{\mathbf{C}}$ の直交補数への全単射、および $1\otimes R(G,T)$ から $R(\mathfrak{g}_{\mathbf{C}},\mathfrak{t}_{\mathbf{C}})$ への全単射を引き起こします。

#### 注意 2 {#lie-ix-s4-n9-rem-2 .statement tag=01CW}

群 G が半単純であると仮定します。 R (それぞれ $R^{\vee}$) 根系 $R(G,T)$ (それぞれ $R^{\vee}(G,T)$) で表され、包含物が存在します。

$$
Q(R)\subset X(T)\subset P(R)Q(R^{\vee})\subset \Gamma (T)\subset P(R^{\vee})
$$

The finite abelian groups $P(R)/Q(R)$ and $P(R^{\vee})/Q(R^{\vee})$ are in duality (Chap. VI, §1, no. 9); if $\widehat{M}$ denotes the dual group of the finite abelian group M, we deduce from the preceding canonical isomorphisms

$$
\Gamma (T)/Q(R^{\vee})\rightarrow \pi_1(G)P(R^{\vee})/\Gamma (T)\rightarrow C(G)
$$

$$
P(R)/X(T)\rightarrow (\pi_1(G)\widehat{)}X(T)/Q(R)\rightarrow (C(G))\widehat{.}
$$

特に、$\pi_1(G)$ の位数および C(G) の積は、$R(G,T) ($loc の接続添字 $f$ と等しくなります。引用）。

ここで、$G'$ を他のとコンパクト・リー群、$T'$ を $G'$ の最大トーラスに接続します。 $f: G\rightarrow G'$ を $f(T) = T'$ となるようなリー群の同型とします。 T から $T'$ までを $f_T$ 同型で表し、それが定義するであることを示します。次に、$X(f_T)$ は $D^*(G',T')$ から $D^*(G,T)$ までの同型で、$D^*(f)$ で示され、$\Gamma (f_T)$ は $D_*(G,T)$ から $D_*(G',T')$ までの同型で、$D_*(f)$ で示されます。 $t\in T$ の場合、$g=f\circ$ Int $t=$ (Int $f(t)$)$\circ f$ を置くと、$D^*(g) = D^*(f), D_*(g) = D_*(f)$ になります。

#### 命題 15 {#lie-ix-s4-prop-15 .statement tag=01CX}

$\varphi$ を $D^*(G',T')$ から $D^*(G,T)$ までの同型とします (それぞれ $D_*(G,T)$ から $D_*(G',T')$ まで)。 $f(T) = T'$ と $\varphi = D^*(f)$ (それぞれ $\varphi = D_*(f)$) となるような同型 $f: G\rightarrow G'$ が存在します。 $f_1$ と $f_2$ が 2 つの同型である場合、$f_2=f_1\circ$ Int $t$ となる T の元 $t$ が存在します。

2 番目の主張は、提案 9 (no. 4) の直後に続きます。たとえば、共変図式の最初の証明を行います。 $G'$ (それぞれ $T'$) の $\mathfrak{g}'$ (それぞれ $\mathfrak{t}'$) リー代数で表し、その複雑化されたリー代数を $\mathfrak{g}'_{\mathbf{C}}$ (それぞれ $\mathfrak{t}'_{\mathbf{C}}$) で表します。 章著。 VIII, §4, no. 4、木。 2 (i) では、$\mathfrak{t}_{\mathbf{C}}$ を $\mathfrak{t}'_{\mathbf{C}}$ にマッピングし、$\Gamma (T)\subset \mathfrak{t}_{\mathbf{C}}$ で指定された同型写像 $\varphi :\Gamma (T)\rightarrow \Gamma (T')$ を誘導する同型写像 $\psi :\mathfrak{g}_{\mathbf{C}}\rightarrow \mathfrak{g}'_{\mathbf{C}}$ が存在します。 すると、$\mathfrak{g}$と$\psi^{-1}(\mathfrak{g}')$は、$\mathfrak{t}_{\mathbf{C}}$と同じ共通部分$\mathfrak{t}$を持つ$\mathfrak{g}_{\mathbf{C}}$の2つのコンパクトな形です。 §3, no. 2、提案 3 により、$\mathfrak{t}_{\mathbf{C}}$ に同一性を誘導する $\mathfrak{g}_{\mathbf{C}}$ の内部自己同型 $\theta$ が存在し、そのような$\theta (\mathfrak{g}) =\psi^{-1}(\mathfrak{g}')$ が存在します。 置き換えること $\psi$ by $\psi \circ \theta$ により、$\psi$ 写像 $\mathfrak{g}$ ～ $\mathfrak{g}'$ と仮定できます。 さらに、no. 2の提案4により、$\Gamma (f_T) =\varphi$となるような一意な準同型 $f_T: T\rightarrow T'$が存在します。 すると、$\psi$から$\mathfrak{t}$の制限は$L(f_T)$となり、§2, no. 6、提案8により、Tには誘導する$f_T$、$\mathfrak{g}_{\mathbf{C}}$には$\psi$という一意な準同型$f: G\rightarrow G'$が存在します。 $\varphi^{-1}$ と $\psi^{-1}$ に先行する適用から、$f$ の逆射が得られ、したがって同型になります。 すると$D_*(f) =\Gamma (f_T) =\varphi$、したがって命題になります。

T と $T'$ が G の 2 つの最大トーラスである場合、図式 $D^*(G,T)$ と $D^*(G,T')$ は同型であることに注意してください ($g\in G$ が $gTg^{-1}= T'$ である場合、Int $g$ は G から G への同型であり、写像 T から$T'$）。 $D^*(G,T)$ の $D^*(G)$ 同型類 (集合の cf. 理論、第 II, §6, no. 2 章) によって示されます。これは、G のみに依存する根図式であり、G の反変図式と呼ばれます。G の共変図式 $D_*(G)$ も同様に定義され、次が得られます。

#### 系 {#lie-ix-s4-n9-cor-1 .statement tag=01CY}

接続された 2 つのコンパクト・リー群 G と $G'$ は、図式 $D^*(G)$ と $D^*(G')$ (それぞれ $D_*(G)$ と $D_*(G')$) が等しい場合にのみ同型です。

#### 命題 16 {#lie-ix-s4-prop-16 .statement tag=01CZ}

縮小されたすべての根図式 D に対して、$D^*(G)$ (それぞれ $D_*(G)$) が D と同型となるような接続されたコンパクト・リー群 G が存在します。

a) 置き換えること D により、必要に応じてその逆数図式により、$D^*(G)$ が D と同型となるような G を構築することになります。 $D = (M,M_0,R)$を入れてください。この場合、$\mathbf{Q}\otimes M$ は、R によって生成された $\mathbf{Q}\otimes M_0$ およびベクトル部分空間 V(R) の直和です。 さらに、M の逆根は整数値をとるので、$\mathbf{Q}\otimes M_0$ と平行なV(R) 上の M の射影は R の重み P(R) の群に含まれるので、M は次の$M_0\oplus P(R)$ の部分群になります。有限の添字。 $D'$ 図式 $(M_0\oplus P(R),M_0,R)$ で表します。

b) Let $\mathfrak{a}$ be a complex semi-simple Lie algebra whose canonical root system is isomorphic to $R\subset \mathbf{C}\otimes V(R)$ (Chap. VIII, §4, no. 3), and let $\mathfrak{g}_1$ be a compact real form of $\mathfrak{a}($§3, no. 2, Th. 1). $G_1$ を単純結合実リー群とし、そのリー代数は $\mathfrak{g}_1$ と同型です。その場合、$G_1$ はコンパクトです (§1, no. 4、Th. 1)。 $T_1$ を $G_1$ の最大値トーラスとします。 Thさんより1、図式 $D^*(G_1,T_1)$ は $(P(R),0,R)$ と同型です。

c) $T_0$ を次元のトーラスと$M_0$ の階数に等しいとします。この場合、$D^*(T_0,T_0)$ は $(M_0,M_0,\emptyset )$ と同型であるため、$D^*(G_1\times T_0,T_1\times T_0)$ は $D'$ (例 2) と同型です。

d) 最後に、N を M に直交する $T_1\times T_0$ の有限部分群とします。$G = (G_1\times T_0)/N, T = (T_1\times T_0)/N$ を置きます。このとき、G は接続されたコンパクト・リー群、T は G の最大値トーラス、そして $D(G,T)$ は D (例 3) と同型です。

#### スクリウム {#lie-ix-s4-n9-sch-1 .statement tag=01D0}

従って、同型までの接続されたコンパクト・リー群の分類は、縮小された根図式の分類に縮小されます。コンパクト半単純リー 群対応するを縮小された根図式 $(M,M_0,R)$ に接続すると、$M_0= 0$ になります。このような図式を与えることは、$\mathbf{Q}$ および $Q(R)\subset M\subset P(R)$ のような V の部分群 M に対してベクトル空間 V の約根系 R を与えることと同等です。

#### 注意 3 {#lie-ix-s4-n9-rem-3 .statement tag=01D1}

$T'$ を、G、B の最大他のトーラス (それぞれ $B'$) 根系 $R(G,T)$ (それぞれ $R(G',T')$) の基底とします (第 2 章 VI, §1, no. 5、定義 2)。 Int $g$ 写像 T が $T'$ に、B が $B'$ になるような元 $g\in G$ が存在し、これらの元形は Int(T) を法とする一意の剰余類です (T と $T'$ は共役なので、 $T = T'$ と仮定することができ、VI, §1, no. 5、注意 4 およびno. 4 の提案 9 を適用するだけで十分です。 従って、Int $g$ によって引き起こされる T から $T'$ までの同型は、$g$ の選択とは独立しています。従って、$D_*$(Int $g$) と $D^*$(Int $g$) にも同じことが当てはまります。 第 2 章の言い換えVIII, §5, no. 3、注釈 2 を準用して、G の正準最大トーラス、$G,. .$ の正準共変および反変ルート図を定義できるようになりました。

### 10. 連結コンパクト・リー群の自己同型

Denote by Aut(G) the Lie group of automorphisms of G (Chap. III, §10, no. 2), and by Aut(G$,T$) the closed subgroup of Aut(G) consisting of the elements $u$ such that $u(T) = T$. 私たちは、Aut(G) の単位成分が内部自己同型の部分群 Int(G) であることを見てきました (§1, no. 4、提案 4 の Cor. 5)。 G の部分群 H の Int(G) の Int$_G(H)$ 像で表します。

D を T に対する G の共変図式とします。 Aut(D) によってその自己同型の群が示され、W(D) によってその Weyl 群が示されます。 写像 $u \rightarrow D_*(u)$ は Aut(G$,T$) から Aut(D) までの準同型です。 no. 9 の提案 15 は直ちに次のようになります。

#### 命題 17 {#lie-ix-s4-prop-17 .statement tag=01D2}

準同型 Aut(G$,T$)$\rightarrow$ Aut(D) は全射であり、核 Int$_G(T)$ です。

Aut(G$,T$)$\cap$ Int(G) = Int$_G(N_G(T))$ であり、Aut(D) の Int$_G(N_G(T))$ の像が W(D) であることに注意してください (no. 5、提案 10)。従って、命題 17 は同型となります。

Aut(G$,T$)$/$(Aut(G$,T$)$\cap$ Int(G)) $\rightarrow$ Aut(D)$/W(D)$。

さらに、Aut(G) = Int(G).Aut(G$,T$)となります。確かに、Aut(G) に対して $u$ 属するであれば、$u(T)$ は T の最大値トーラスであるため、T に対して共役となり、他の式では $u(T) =v$(T) となるような G の内部自己同型 $v$ が存在します。 語 $v^{-1}u\in$ オート(G$,T$)。従って、Aut(G)$/$Int(G) は Aut(G$,T$)$/$(Aut(G$,T$)$\cap$Int(G)) と識別できるため、上記を考慮すると、完全系列となります。

$1\rightarrow$ Int(G) $\rightarrow$ Aut(G) $\rightarrow$ Aut(D) $/W(D)\rightarrow 1$。 (16)

その結果:

#### 命題 18 {#lie-ix-s4-prop-18 .statement tag=01K9}

群 Aut(G)$/$Int(G) は Aut(D)$/W(D)$ と同型です。

特に、G が半単純であると仮定します。 群 Aut(D) は、$A(R(G,T))$ (第 VI, §1, no. 1) の部分群 、元 $u$ のからなると識別でき、$u(X(T))\subset X(T)$ および部分群 W(D) は次のように識別できます。 $W(R(G,T))$。

#### 系 {#lie-ix-s4-n10-cor-1 .statement tag=01D3}

G が単純結合の場合、または C(G) 簡約するから単位元の場合、群 Aut(G)$/$Int(G) は、$R(G,T)$ のディンキングラフの自己同型の群と同型です。

これは前章と第 2 章の続きです。 VI, §4, no. 2、コル。提案 1 の。

これから、拡大 (16) が切断を認めることを示します。

すべての $\alpha \in R(G,T)$ について、$V(\alpha )_{(\mathbf{C})}=\mathfrak{g}^{\alpha}+\mathfrak{g}^{-\alpha}$ となるような $\mathfrak{g}$ の 2 次元ベクトル部分空間を $V(\alpha )$ で表します。 $\mathfrak{g}$ の殺害形に関連する 2 次式形を K で示します。

#### 定義 3 {#lie-ix-s4-def-3 .statement tag=01D4}

$(G,T)$ のフレーミングは対 $(B,(U_{\alpha})_{\alpha\in B})$ で、B は $R(G,T)$ の基底 (章 VI, §1, no. 5、定義 2)、そして全体として $\alpha \in B,U_{\alpha}$ は $V(\alpha )$ の元です。 $K(U_{\alpha}) =-1$。

G のフレーミングは、$(G,T)$ のフレーミングと合わせて、G の最大トーラス T です。

#### 補題 3 {#lie-ix-s4-lem-3 .statement tag=01D5}

$B_0$を$R(G,T)$の基底とします。 群 Int$_G(T)$ は、形 $(B_0,(U_{\alpha})_{\alpha\in B_0})$ の $(G,T)$ のフレームの集合に対して単純推移的に動作します。

すべての $\alpha \in B_0$ について、二次方程式形 K から $V(\alpha )$ の $K(\alpha )$ 制限で表します。 $V(\alpha )$ 定義する射 $\iota_{\alpha}: T\rightarrow \mathbf{S}\mathbf{O}(K(\alpha ))$ の T の演算。 no. 4 で、$\iota_{\alpha}$ が根 $\alpha$ と同一視されるように、$\mathbf{S}\mathbf{O}(K(\alpha ))$ が $\mathbf{U}$ と同一視されることがわかりました。 $B_0$ は R の基底であるため、根によって生成された $\mathbf{Z}$ モジュール Q(R) の基底、したがって部分加群の $X(T/C(G))$ の X(T) の基底です。 したがって、射の積 $\iota_{\alpha}$ は、群 $\mathbf{S}\mathbf{O}(K(\alpha ))$ の積への同型を $T/C(G)$ から誘導します。 しかし、後者の群は、最初の成分が $B_0$ である $(G,T)$ のフレームの集合に対して単純推移的に動作します。

#### 命題 19 {#lie-ix-s4-prop-19 .statement tag=01D6}

群 Int(G) は、G のフレームの集合に対して単純推移的に動作します。

$e= (T,B,(U_{\alpha}))$ と $e'= (T',B',(U'_{\alpha}))$ を G の 2 つのフレームとします。 G には (Int $g$)$(T) = T'$ となる元 $g$ が存在し、これらの元形は $N_G(T)$ を法とする単一剰余類です。したがって、$T = T'$ と仮定し、変換 $e$ から $e'$ までの Int$_G(N_G(T))$ の一意元が存在すると証明しなければならない仮定することができます。章著。 VI, §1, no. 5、注意 4、$w(B) = B'$となるようなW(R)の一意元 $w$が存在します。 W(R) は $N_G(T)/T$ で識別できるため、$w=$ Int $n$ である $n\in N_G(T)$ が存在し、$n$ は T を法として一意に決定されます。 したがって、$B = B'$ と仮定でき、証明しなければならないの一意元が存在すると仮定できます。 Int$_G(T)$ 変換 $e$ を $e'$ にすると、単純に補題 3 になります。

#### 系 {#lie-ix-s4-n10-cor-2 .statement tag=01D7}

$e$ を $(G,T)$ のフレームとし、E を $e$ を安定に残す G の自己同型の群とします。この場合、Aut(G) は Int(G) による E の半直接積であり、Aut(G$,T$) は Int(G) $\cap$ Aut(G$,T$) $=$ Int$_G(N_G(T))$ による E の半直接積です。

確かに、Aut(G) 変換 $e$ のすべての元は G のフレームに変換されます。 提案 19 により、Aut(G) モジュロ Int(G) のすべての剰余類は単一の点で E と一致するため、最初の主張が生じます。 2番目も同様に証明されます。

#### 注意 {#lie-ix-s4-n10-rem-1 .statement tag=01D8}

G と $G'$ を 2 つ接続されたコンパクト・リー群とし、$e=$ $(T,B,(U_{\alpha}))$ と $e'= (T',B',(U'_{\alpha}))$ をそれぞれ G と $G'$ のフレームとします。 X を、$e$ から $e'$ かかる G から $G'$ までの同型の集合とします。 写像 $f \rightarrow D^*(f)$ (それぞれ $D_*(f)$) は、$D^*(G',T')$ から $D^*(G,T)$ までの同型 (それぞれ $D_*(G,T)$ から $D_*(G',T')$) の X から集合までの全単射です。 写像 $B'$ から B (それぞれ B から $B'$)。実際、これは提案 15 および補題 3 からすぐに続きます。

### 練習問題 {#lie-ix-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
