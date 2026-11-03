---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 17
section_title: Reduced Norms and Traces
lang: ja
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.335-A VIII.353
pdf_pages: 0352-0370
extraction: native+ocr
subsections:
    - "no": 1
      title: Complements on Characteristic Polynomials
      page: 335
      pdf_page: 352
    - "no": 2
      title: Reduced Norms and Traces
      page: 339
      pdf_page: 356
    - "no": 3
      title: Properties of Reduced Norms and Traces
      page: 341
      pdf_page: 358
    - "no": 4
      title: The Reduced Norm is a Polynomial Function
      page: 344
      pdf_page: 361
    - "no": 5
      title: Transitivity of Reduced Norms and Traces
      page: 346
      pdf_page: 363
    - "no": 6
      title: Reduced Norms and Determinants
      page: 349
      pdf_page: 366
statements: 31
exercises: 7
content_sha256: d311e846122f01501183b355d74ebf4cb33f294aea20ff98ede7b090506a5bca
translated_from: content/en/alg/VIII/17_s17_reduced_norms_and_traces.md
translation_method: google
source_content_sha256: 08c1f7f51bd2df11d29e638f229d1b484c7cda3e1bc21277c413e8819b54daaf
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 5df044043a555888d53b2c90054ef1c05437fdf9c5687baa466df1516b49997c
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 17。 被約ノルムと痕跡

この切断では、Kは可換体、Aは有限次数の中心単純K-代数です。 A を縮小した次数を $n$ で表します。

### 1. 特性多項式の補数

L を可換環とし、M を有限階数 $m$ の空き L モジュールとします。 $u$ が M の自己準同型および $r$ 自然数である場合、自由な L モジュール $\wedge^r(M)$ の自己準同型 $\wedge^r(u)$ のトレースを $c_r(u)$ で表します。特に、私たちは、

(1) $c_0(u) = 1,c_1(u) =$ Tr($u$)$,c_m(u) =$ det($u$)、

$c_r(u) = 0$ は $r > m$ です。 III, §8, No. 4, p. 527 の命題 7 により、End(M) から L へのマッピング $u\mapsto$ det($u$) は、次数 $m$ (IV, §5, No. 9, p. 55) の同次多項式マッピングになります。 より一般的には、End(M) から L までの $0\leqslant r\leqslant m$、写像 $c_r$ が次数 $r$ の同次多項式写像となるようなすべての整数 $r$ について、これは、III, §8, No. 5、p. 529 の命題 10 から続きます。

$u$ を M の内部同型性とし、$\overline{u}$ をスカラー (II, §5, No. 1, p. 277) の拡張によって $u$ から推定される L[X]加群 $M[X] = M\otimes_LL[X]$ の内部同型性とする。 (III, §8, No. 11、p. 541、定義 3 および (50)) を思い出してください。$u$ の特性多項式は、M[X] の L[X]自己準同型 $X-\overline{u}$ の行列式 $\chi_u(X)$ であり、 関係があります

$$
\chi_u(X) =\sum_{r=0}^m(-1)^rc_r(u) X^{m-r} \tag{2}
$$

#### 命題 1 {#alg-viii-s17-prop-1 .statement tag=00KD}

L を可換環とし、M を有限階数 m $\geqslant 1$ の自由 L 加群、M の u 自己準同型とします。M 満たす関係の一意な自己準同型 $\tilde{u}$ が存在します。

$$
\tilde{u}(x) \wedge w = x \wedge \wedge^{m-1}(u)(w)
$$

$x \in M$ と $w \in \wedge^{m-1}(M)$ の場合。さらに、関係もあります

$$
u \circ \tilde{u} = \tilde{u} \circ u = \det(u)_M,
$$
$$
\det(\tilde{u}) = \det(u)^{m-1},
$$
$$
\tilde{u} = \sum_{r=0}^{m-1} (-1)^r c_{m-1-r}(u) u^r.
$$

#### 補題 1 {#alg-viii-s17-lem-1 .statement tag=00KE}

p を $0 \leqslant p \leqslant m$ となるように整数とします。 $\wedge^p(M)$ の任意の w について、$h_p(w)$ を $\wedge^{m-p}(M)$ から $\wedge^m(M)$ までの線形写像 $w' \mapsto w \wedge w'$ とします。 $\wedge^p(M)$から$\operatorname{Hom}_L(\wedge^{m-p}(M), \wedge^m(M))$までの線形写像$h_p : w \mapsto h_p(w)$は同型です。

$(e_i)_{i \in I}$ を M の基底とします。私たちは集合 I に合計位数を与えます。 I、集合 $e_J = e_{i_1} \wedge \cdots \wedge e_{i_r}$ の任意の部分集合 J について、$(i_1, \ldots, i_r)$ は増加する位数の J の元の数列です。 L モジュール $\wedge^{m-p}(M)$ は基底元 $e_S$ として認められ、S は I の部分集合の集合を $m - p$ 元と実行します。 $\wedge^m(M)$には$\{e_I\}$が基底として含まれています。従って、公式を特徴とする $\operatorname{Hom}_L(\wedge^{m-p}(M), \wedge^m(M))$ からなるの線形写像 $e_J^*$ の基底が存在します。

$$
e_J^*(e_S) = \begin{cases}
e_I & \text{if } I = J \cup S, \\
0 & \text{otherwise},
\end{cases}
$$

ここで、J は p 元で I の部分集合の集合を通過します。 III, §7, No. 8, p. 519 の公式 (20) から、p 元を持つ I のすべての部分集合 J に対して、$h_p(e_J) \in \{e_J^*, -e_J^*\}$ が得られます。 $\wedge^p(M)$ の元 $e_J$ 形基底なので、線形写像 $h_p$ は全単射です。

命題 1 を証明しましょう。 u と $\tilde{u}$ を M の自己準同型とします。 関係 (3) は次と同等です。

$$
h_1 \circ \tilde{u} = \operatorname{Hom}(\wedge^{m-1}(u) \cdot 1_{\wedge^m(M)}) \circ h_1;
$$

写像 $h_1$ は、補題 1 により M から $\operatorname{Hom}_L(\wedge^{m-1}(M), \wedge^m(M))$ まで同型になります。その結果、M のすべての自己準同型 u に対して、M 満たす関係の一意な自己準同型 $\tilde{u}$ が存在します (3)。

$x_1, . . . , x_m$ を M の元とします。(3) の $u(x_1)$ と $w$ と $x_2\wedge  \cdots  \wedge x_m$ を含む置き換える $x$ とします。私たちは得る

$\widetilde{u}(u(x_1))\wedge x_2\wedge  \cdots  \wedge x_m=u(x_1)\wedge  \cdots  \wedge u(x_m) =$ デット($u$)$x_1\wedge  \cdots  \wedge x_m$。

その結果、$h_1(\widetilde{u}\circ u(x_1)) =h_1$(det($u$)$x_1$)となり、補題 1 により関係 $\widetilde{u}\circ u=$ det($u$)$_M$ が得られます。

L[X]モジュール M[X] (VIII, p. 335) の U 自己準同型 $X-\overline{u}$ で表します。上記を U に適用すると、関係を満たす L[X]-モジュール M[X] の自己準同型 $\widetilde{U}$ が存在します。

$$
\widetilde{U}(x_1)\wedge x_2\wedge  \cdots  \wedge x_m=x_1\wedge (Xx_2-u(x_2))\wedge  \cdots  \wedge (Xx_m-u(x_m)) \tag{9}
$$

M の $x_1, . . . , x_m$ と

(10) $\widetilde{U}\circ U =$ デット(X $-\overline{u}$)$_{M[X]}$。

$\widetilde{U}$ を End(M)[X] (VIII, p. 9) の元として見てみましょう。 公式 (9) と補題 1 により、次数 $\leqslant m-1$ となるので、次のように書くことができます。

$$
\widetilde{U} =\sum^{m-1}_{r=0}(-1)^ru_rX^{m-1-r} \tag{11}
$$

ここで、$u_r$ は M の自己準同型です。 公式 (2) により、関係 (10) は等式を与えます。

$$
(\sum^{m-1}_{r=0}(-1)^ru_rX^{m-1-r})(X-u) =\sum_{r=0}^m(-1)^rc_r(u)X^{m-r} \tag{12}
$$

環エンド(M)[X]。各辺のXの単項式の係数を特定すると、関係が得られます。

(13) $u_r+u_{r-1}\circ u=c_r(u)_M$ の $1\leqslant r\leqslant m-1$

そして

$$
u_0=c_0(u)_M,u_{m-1}\circ u=c_m(u)_M \tag{14}
$$

これから推測すると、

$$
u_{m-1}=\sum^{m-1}_{r=0}(-1)^rc_{m-1-r}(u)u^r \tag{15}
$$

さて、定数項を同一視するとすると、等式 (9) と (11) は $u_{m-1}=\widetilde{u}$ を意味します。 公式 (6) が続きます。

特に、End(M) の $\widetilde{u}$ 属するから部分代数は $u$ によって生成され、従って $u$ と可換です。すでに関係 $\widetilde{u}\circ u=$ det($u$)$_M$ を確立しています。 公式 (4) が続きます。

最後に、$x_1, . . . , x_m$ を M の元とします。公式 (3) では、$x_1$ と置き換える $x$、$\widetilde{u}(x_2)\wedge  \cdots  \wedge \widetilde{u}(x_m)$ と$w$ が関係します。これにより、

$$
\widetilde{u}(x_1)\wedge \widetilde{u}(x_2)\wedge  \cdots  \wedge \widetilde{u}(x_m) =x_1\wedge u\circ (\widetilde{u}(x_2))\wedge  \cdots  \wedge u\circ (\widetilde{u}(x_m))
$$

= det($u$)$^{m-1}x_1\wedge x_2\wedge  \cdots  \wedge x_m$

従って、公式 (5)。

#### 注意 1 {#alg-viii-s17-n1-rem-1 .statement tag=00KF}

M 一致するの自己準同型 $\widetilde{u}$ と、III, §8, No. 6、p. 532 の $u$ の共転置と呼ばれるもの。

#### 注意 2 {#alg-viii-s17-n1-rem-2 .statement tag=00KG}

公式 (1)、(2)、(4)、および (6) から、関係 $\chi_u(u) = 0$、したがってケイリー-ハミルトン定理 (III, §8, No. 11, p. 541) の他の証明が推定されます。

#### 注意 3 {#alg-viii-s17-n1-rem-3 .statement tag=00KH}

End(M)からLまでの写像$c_r$は$0\leqslant r\leqslant m-1$の次数$r$の同次多項式写像なので、公式(6)より写像$u\mapsto \widetilde{u}$が求まります。エンド(M)からエンド(M)までは次数$m-1$の同次多項式写像です。

B を環 L 以上代数とします。 B が、B の部分環 $L\cdot 1$ をもつ階数 $m\geqslant 1$ と同一視する L の自由な L モジュールであるとします。$b$ を B の元とします。上記を自己準同型に適用しますL モジュール B の $\gamma (b) :x\mapsto bx$。 集合 $\gamma_r(b) =c_r(\gamma (b))$ $0\leqslant r\leqslant m$。特に、$\gamma_m(b) = N_{B/L}(b)$ (III, §9, No. 3、p. 543) があります。 $b$ (前述) の特性多項式は次のように書くことができます。

(16) パソコン$_{B/L}(b; X) =\sum_{r=0}^m(-1)^r\gamma_r(b) X^{m-r}$。

BからEnd$_L(B)$までの写像$\gamma$はL線形なので、BからLまでの写像$\gamma_r$は次数$r$の同次多項式写像です。特に、BからLまでの写像$b\mapsto N_{B/L}(b)$は、次数$m$の同次多項式写像です。

B のいずれかの元 $b$、集合

$$
\widetilde{b}=\sum^{m-1}_{r=0}(-1)^r\gamma_{m-1-r}(b)b^r \tag{17}
$$

命題 1 により、B から B への線形写像 $\gamma (\widetilde{b})$ は写像 $\gamma (b)$ の共転置です。これから推測すると、

$$
b\widetilde{b}=\widetilde{b}b= N_{B/L}(b) \tag{18}
$$

さらに、BからBへの写像$b\mapsto \widetilde{b}$は、次数$m-1$の同次多項式写像です。

### 2. 被約ノルムと痕跡

縮小された次数 $n$ の可換体 K 上の中心単純代数を A で表すことを思い出してください。

#### 命題 2 {#alg-viii-s17-prop-2 .statement tag=00KI}

$a$ を A の元と Pc($a; X$) の特性多項式とします。 K[X] には Pc($a; X$) $= P(X)^n$ となるような一意のモニック多項式 P が存在します。

A) P の一意性は、以下の補題 2 から続きます。

#### 補題 2 {#alg-viii-s17-lem-2 .statement tag=00KJ}

P と Q を K[X] のモニック多項式とし、$s$ は厳密には正の整数です。 $P^s= Q^s$ の場合、P = Q となります。

$\mathscr{I}$ を K[X] の既約モニック多項式の集合とします。 P と Q はモニックであるため、$\mathbf{N}^{(\mathscr{I})}$ の元 $(a_F)$ と $(b_F)$ が存在し、$P =\prod_{F\in\mathscr{I}}F^{a_F}$ と $Q =\prod_{F\in\mathscr{I}}F^{b_F}$ が存在します。 分解の等式 $P^s= Q^s$ と一意性から、$F\in \mathscr{I}$ ごとに $sa_F=sb_F$ が得られ、既約の因子になります。 $s$ は厳密に正であるため、結果的に $F\in \mathscr{I}$ ごとに $a_F=b_F$ が得られ、従って P = Q となります。

B) P の存在を証明しましょう。

VIII, p. 252 の定理 1 により、有限次数の K のガロア拡大 L と L-代数 $\theta : A_{(L)}\rightarrow \mathbf{M}_n(L)$ の同型が存在します。 III, §9, No. 1, p. 542 の公式 (12) より、多項式 Pc($a; X$) は、L-代数 $A_{(L)}$ の元 $1\otimes a$ の特性多項式でもあり、よって元 L代数$\mathbf{M}_n(L)$の$\theta (1\otimes a)$。

集合 P(X) = det(X$I_n-\theta (1\otimes a)$);それは L[X] のモニック多項式です。 III, §9, No. 3、p. 545 の例 3 までに、

(19) パソコン($a; X$)$= P(X)^n$。

G を K 上の L のガロア群とします。$\sigma \in G$ について、環 L[X] の $\overline{\sigma}$ 自己同型で、L に $\sigma$ が付いた一致すると表します。 Xを修正。すると、K[X] は、L[X] の多項式 Q の集合となり、$\sigma \in G$ (V, §10, No. 1, p. 56, 定理 1) ごとに $\overline{\sigma}(Q) = Q$ が得られます。多項式 Pc($a; X$) $= P(X)^n$ 属するから K[X] なので、$\sigma \in G$ ごとに $\overline{\sigma}(P)^n= P^n$ が得られます。したがって、補題 2 までに、$\sigma \in G$ ごとに $\overline{\sigma}(P) = P$ が得られるため、P 属するから K[X] になります。

#### 定義 1 {#alg-viii-s17-def-1 .statement tag=00RM}

$a$ を代数 A の元とします。$a$ (A に関して) の縮小特性多項式は、関係を満たす、Pcrd$_{A/K}(a; X)$ で示される K[X] の一意のモニック多項式です。

(20) PC$_{A/K}(a; X) =$ Pcrd$_{A/K}(a; X)^n$。

$a$ を A の元とします。A は K に対して次数 $n^2$ を持つため、多項式 Pc$_{A/K}(a; X)$ は次数 $n^2$ となるため、Pcrd$_{A/K}(a; X)$ は次数のモニック多項式になります。 $n$;次のように書きましょう

(21) Pcrd$_{A/K}(a; X) = X^n+\sum^{n-1}_{r=0}(-1)^rb_r(a)X^{n-r}$。

私たち集合

(22) Trd$_{A/K}(a) =b_1(a)$、Nrd$_{A/K}(a) =b_n(a)$。

#### 定義 2 {#alg-viii-s17-def-2 .statement tag=00KK}

A の Trd$_{A/K}(a)$ 簡約トレースを、Nrd$_{A/K}(a)$ を (K-代数 A に関して) 被約ノルムと呼びます。

混乱の危険がない場合は、記法から A と K を省略し、単に Pcrd($a; X$)、Trd($a$)、および Nrd($a$) と書きます。

次の公式は、III, §9, No. 1、p. 542 の公式 (20) と (22) および公式 (7) と (8) の結果です。

(23) 取引$_{A/K}(a) =n$ 取引$_{A/K}(a)$、

(24) $N_{A/K}(a) =$ (Nrd$_{A/K}(a)$)$^n$。

#### 命題 3 {#alg-viii-s17-prop-3 .statement tag=00KL}

A の元 $a$ は、その被約ノルムが非零である場合に限り、反転可能です。特に、A の非零元 $a$ ごとに Nrd$_{A/K}(a)\not= 0$ がある場合に限り、A は体になります。

A の元 $a$ は、そのノルムが非零 (III, §9, No. 4、p. 545、命題 3) である場合にのみ反転可能です。したがって、命題 3 は公式 (24) から続きます。

#### 注意 {#alg-viii-s17-n2-rem-1 .statement tag=00KM}

L を 1 つの変数 X の有理分数の体 K(X) とします。 A の縮小特性多項式元 $a$ は、単に L-代数 $A_{(L)}$ の元 $X\otimes 1-1\otimes a$ の被約ノルムです。これは、縮小特性多項式の定義と公式 (III, §9, No. 3, p. 544) から続きます。

(25) パソコン$_{A/K}(a; X) = N_{A_{(L)}/L}(X\otimes 1-1\otimes a)$。

#### 例 1 {#alg-viii-s17-n2-exa-1 .statement tag=00RN}

VIII, p. 120 の定理 1 までに、A が $\mathbf{M}_r(D)$ と同型となるような整数 $r\geqslant 1$ と体 D が存在します。 $d$ を K に対する D の縮小した次数とします。 $r=n/d$ があります。 M を有限長 $\ell$ の A-加群とします。 公式を証明します

(26) PC$_{M/K}(a_M; X) =$ Pcrd$_{A/K}(a; X)^{d\ell}$

A のすべての元 $a$ に対して、A-加群 $A_s$ には長さ $r$ (VIII、p. 121、補題 2) が含まれます。 A-加群 $M^r$ と $A^{\ell}_s$ は同じ長さを持っているため、同型であり、次のようになります。

パソコン$_{M/K}(a_M; X)^r=$ パソコン$_{A/K}(a; X)^{\ell}$

III, §9, No. 2、p. 542の公式 (15) 作。 $rd=n$ があるので、公式 (20) と補題 2 (VIII, p. 339) から公式 (26) が続きます。

#### 例 2 {#alg-viii-s17-n2-exa-2 .statement tag=00RO}

A が有限次元 K-ベクトル空間 V の自己準同型の代数端$_K(V)$ である特定のケースを考えてみましょう。 M を単純A-加群 V とすると、関係が得られます。

Pcrd$_{A/K}(u; X) =\chi_u(X)$,

(27) Nrd$_{A/K}(u) =$ det($u$)、

Trd$_{A/K}(u) =$ Tr($u$)

V の自己準同型 $u$ ごとに。

### 3. 被約ノルムのプロパティとトレース

#### 命題 4 {#alg-viii-s17-prop-4 .statement tag=00KN}

L を K の拡大とし、中央単純代数 A の $a$ 元とします。関係があります。

(28) Pcrd$_{A_{(L)}/L}(1\otimes a; X) =$ Pcrd$_{A/K}(a; X)$、

(29) 取引$_{A_{(L)}/L}(1\otimes a) =$ 取引$_{A/K}(a)$、

(30) Nrd$_{A_{(L)}/L}(1\otimes a) =$ Nrd$_{A/K}(a)$

(「スカラーの拡大の下での不変性」)。

等式 (28) の両辺は、定義 (VIII、p. 340 の公式 (20)) と関係による$n$ 番目の冪が同じです。

Pc$_{A_{(L)}/L}(1\otimes a; X) =$ Pc$_{A/K}(a; X)$ (III, §9, No. 3、p. 544、公式 (21))。したがって、等式 (28) は、VIII、p. 339 の補題 2 から続きます。 公式 (29) と (30) は (28)、(21)、(22) から続きます。

#### 系 1 {#alg-viii-s17-prop-4-cor-1 .statement tag=00KO}

LをKの拡大とします。Vを、Aからエンド$_L(V)$までのLと$\theta$K-代数準同型にわたる次元$n$のベクトル空間とします。 A の元 $a$ ごとに、

(31) Pcrd$_{A/K}(a; X) =\chi_{\theta(a)}(X)$、

(32) Trd$_{A/K}(a) =$ Tr($\theta (a)$)、

(33) Nrd$_{A/K}(a) =$ det($\theta (a)$)。

$\theta '$ を、$\lambda \in L$ と $a\in A$ に対して $\theta '(\lambda \otimes a) =\lambda \theta (a)$ となるような、$A_{(L)}$ から End$_L(V)$ までの L 代数準同型性とします。 代数 $A_{(L)}$ は、VIII、p. 222 の 2 つである系によって単純です。したがって、準同型 $\theta '$ は単射法です。しかし、体 L 上の代数 $A_{(L)}$ と End$_L(V)$ は同じ次数を持ち、$n^2$ に等しいため、$\theta '$ は同型になります。 系 1 は、上記の命題 4 と例 2 から続きます。

#### 系 2 {#alg-viii-s17-prop-4-cor-2 .statement tag=00KP}

$a$ と $a'$ を A の元と K の $\lambda$ 元とします。関係になります。

(34) Pcrd$_{A/K}(a;a) = 0$、

(35) Pcrd$_{A/K}(\lambda a;\lambda X) =\lambda^n$ Pcrd$_{A/K}(a; X)$、

(36) 取引$_{A/K}(a+a') =$ 取引$_{A/K}(a) +$ 取引$_{A/K}(a')$、

取引$_{A/K}(\lambda a) =\lambda$ 取引$_{A/K}(a)$、

(37) 取引$_{A/K}(aa') =$ 取引$_{A/K}(a'a)$、

(38) Nrd$_{A/K}(aa') =$ Nrd$_{A/K}(a)\cdot$ Nrd$_{A/K}(a')$、

Nrd$_{A/K}(\lambda a) =\lambda^n$ Nrd$_{A/K}(a)$、

(39) Trd$_{A/K}(1) =n$、Nrd$_{A/K}(1) = 1$。

A は中心単純であり、K に対して次数 $n$ が減少しているため、K の拡張 L と L 上の次元 $n$ のベクトル空間 V が存在し、$A_{(L)}$ は代数 End$_L(V)$ (VIII, p. 252、定理) と同型です。 1)。 系 2 は、系 1 とトレースのプロパティと自己準同型の行列式から続きます。 特に、公式 (34) は、ケイリー – ハミルトンの定理 (III, §8, No. 11、p. 541、命題 20、cf.、また VIII、p. 338、注意 2) から続きます。

#### 系 3 {#alg-viii-s17-prop-4-cor-3 .statement tag=00RP}

$A^o$ を A の反対多元環とします。A のすべての $a$ について、次のようになります。

(40) Pcrd$_{A^o/K}(a; X) =$ Pcrd$_{A/K}(a; X)$、

(41) 取引$_{A^o/K}(a) =$ 取引$_{A/K}(a)$、

(42) Nrd$_{A^o/K}(a) =$ Nrd$_{A/K}(a)$。

K の選ぶ拡大 L、次元のベクトル空間 V L 上の$n$、および A からエンド$_L(V)$ までの準同型 $\theta$ (VIII, p. 252、定理 1)。 $V^*$をVの双対ベクトル空間とします。 A の元 $a$ を $V^*$ の自己準同型 $^t\theta (a)$ に送信する写像は、$A^o$ から End$_L(V^*)$ までのK-代数準同型です。 系 3 は、III, §8, No. 4、p. 528 の系 1 および系 3 から続きます。

したがって、トレースノルムと$a$の特性多項式は、$a$をAの元と見なしても、$A^o$の元と見なしても同じです。 A が中心単純であると仮定されていない場合 (III, §9、p. 644、練習問題 1)、この性質は必ずしも成り立ちません。

#### 命題 5 {#alg-viii-s17-prop-5 .statement tag=00KQ}

A の任意の $x$ について、$t_x$ を A の線型形式 $y\mapsto$ Trd$_{A/K}(xy)$ とします。

a) 写像 $t:x\mapsto t_x$ は、A からそのデュアル Hom$_K(A,K)$ までの $(A,A)$ バイモジュールの同型です。

b) A の $h$ を線型形式とします。以下のプロパティは同等です。

(i) $h(x) =\lambda$ Trd$_{A/K}(x)$ となるような K の元 $\lambda$ が存在します。

$x\in A$ごとに。

(ii) A のすべての $x, y$ に対して $h(xy) =h(yx)$ が得られます。

(II, §1, No. 14, p. 225–226) $A^*=$ Hom$_K(A,K)$ 上の $(A$, A)-bimodule 構造が関係によって定義されていることを思い出してください。

$$
\langle atb, c\rangle =\langle t, bca\rangle \tag{43}
$$

$a, b, c\in A$と$t\in A^*$の場合。特に、A の $x$ ごとに、

$\langle at_xb, c\rangle =\langle t_x, bca\rangle =$ Trd$_{A/K}(xbca)$,

$\langle t_{axb}, c\rangle =$ Trd$_{A/K}(axbc)$,

そして、これら 2 つの元は、VIII、p. 342 の公式 (37) と等しくなります。したがって、$at_xb=t_{axb}$ があり、これは、$t$ が $(A$ の準同型、A) A から $A^*$ までの双モジュールであることを意味します。

私たちは、体 K と同型 $\theta$ の選ぶ拡大 L を L-代数 $A_{(L)}$ から行列環 $\mathbf{M}_n(L)$ (VIII, p. 252、定理 1)。 体 L に対するベクトル空間 $A_{(L)}$ の双対で、同一視するベクトル空間 $(A^*)_{(L)}$ となります。これらの規則により、VIII、p. 341 の命題 4 までに、

(44) 取引$_{A_{(L)}/L}= 1_L\otimes$ 取引$_{A/K}$。

$t_{(L)}$ を、スカラーの拡大によって $t$ から推定された $A_{(L)}$ から $A^*_{(L)}$ までの L 線形マッピングとします。 公式 (44) と系 1 により、

(45) $\langle t_{(L)}(x), y\rangle =$ Trd$_{A_{(L)}/L}(xy) =$ Tr($\theta (x)\theta (y)$)

$A_{(L)}$の$x, y$用。 II, §10, No. 11、p. 358、写像 $t_{(L)}$ のうち、命題 7 は全単射です。従って、$t$ は全単射であることがわかります。私たちは a) を証明しました。

$h$ を $A^*$ に入れます。上記より、$h$が$t_a$に等しいようなAの元$a$が存在します。 a) により、

$$
h(xy)-h(yx) =t_a(xy-yx) =t_{ax}(y)-t_{xa}(y)
$$

従って、関係「A の $x, y$ に対して $h(xy) =h(yx)$」は「$x\in$ A ごとに $t_{ax-xa}= 0$」と等しく、部分 a) の証明により、これは、$a$ 属するから中心 K を意味します。 A. これは、公式 (36) を考慮して b) を証明します。

#### 系 {#alg-viii-s17-n3-cor-1 .statement tag=00KR}

形 $xy-yx$ の元によって生成される A の線形部分空間は、$x$ と $y$ が A を通過するもので、非零線型形式の超平面、核です。 TRD$_{A/K}$。

#### 注意 {#alg-viii-s17-n3-rem-1 .statement tag=00KS}

VIII、p. 340 の公式 (23) までに、

取引$_{A/K}(a) =n$ 取引$_{A/K}(a)$

$a\in A$ごとに。 体 K の特性が 0 または割る $n$ に等しい素数数 $p$ に等しい場合、命題 5 のトレースを使用して置き換える簡約トレースができます。一方、K の特性が素数の場合は、 数と割る $n$ の場合、$a\in A$ ごとに Tr$_{A/K}(a) = 0$ が得られます。

### 4. 被約ノルムは多項式関数

#### 補題 3 {#alg-viii-s17-lem-3 .statement tag=00KT}

L を K の拡大とし、I を集合と $\mathbf{T}= (T_i)_{i\in I}$ を変数ファミリーとします。 $K(\mathbf{T})\cap L[\mathbf{T}] = K[\mathbf{T}]$ があります。

P と Q を $K[\mathbf{T}]$ の $Q\not= 0$ の元とします。 P = QR となる $L[\mathbf{T}]$ の多項式 R の係数は、K に係数をもつ線形方程式の系の解です。 従って、P = QR となる多項式 $R\in L[\mathbf{T}]$ が存在する場合、$K[\mathbf{T}]$ にも多項式が存在します。 (II, §8, No. 5、p. 321、命題 6)。これは、$K(\mathbf{T})\cap L[\mathbf{T}]\subset K[\mathbf{T}]$ が含まれていることを証明します。逆の包含は明らかです。

A の縮小特性多項式元 $a$ は次のように書けることを思い出してください。

(46) カード$_{A/K}(a; X) =\sum_{r=0}^n(-1)^rb_r(a) X^{n-r}$

そして私たちが持っていること

$b_0(a) = 1,b_1(a) =$ Trd$_{A/K}(a),b_n(a) =$ Nrd$_{A/K}(a)$。

#### 命題 6 {#alg-viii-s17-prop-6 .statement tag=00KU}

$0\leqslant r\leqslant n$ となるすべての整数 $r$ について、A から K までの写像 $b_r$ は、次数 $r$ の同次多項式写像になります。特に、被約ノルムは、A から K までの次数 $n$ の同次多項式写像です。

$(e_i)_{i\in I}$ を K 上の A の基底および変数の族である $\mathbf{T}= (T_i)_{i\in I}$ とします。

#### 補題 4 {#alg-viii-s17-lem-4 .statement tag=00KV}

$u$ を中心単純 $K(\mathbf{T})$-代数 $A_{(K(\mathbf{T}))}$ の元 $\sum_{i\in I}T_i\otimes e_i$ とします。 P を $u$ の縮小特性多項式とする。次に、P 属するから環 $K[\mathbf{T}][X]$; 環 $K[\mathbf{T},X]$ の元として見れば、次数 $n$ と同質です。

K の選ぶ拡大 L と $A_{(L)}$ から $\mathbf{M}_n(L)$ までの L-代数同型写像 $\theta$ です。 $\theta$ からスカラーの拡大によって演繹された $L(\mathbf{T})$-代数の $\overline{\theta}: A_{(L(\mathbf{T}))}\rightarrow \mathbf{M}_n(L(\mathbf{T}))$ 同型で表します。 VIII、p. 342 の系 1 までに、

(47) $P(X) =\chi_{\overline{\theta}(u)}(X) =$ デット(X$I_n-\overline{\theta}(u)$) $=$ デット$(XI_n-\sum_{i\in I}T_i\theta (1\otimes e_i))$。

行列 $\theta (1\otimes e_i)$ 属するから $\mathbf{M}_n$(L) なので、この公式は、P が $L[\mathbf{T},X]$ の次数 $n$ の同次多項式であることを示します。また、属するから $K(\mathbf{T})[X]$ まであり、それぞれ $c_j$ 属するから共通部分 $K(\mathbf{T})\cap L[\mathbf{T}]$ として、$P(X) =\sum_{j\geqslant 0}c_jX^j$ と書くこともできます。 補題 3 までに、元 $c_j$ 属するから $K[\mathbf{T}]$ まで。 補題 4が続きます。

#### 補題 5 {#alg-viii-s17-lem-5 .statement tag=00KW}

K のすべての拡大 $K'$ と ${K'}^I$ のすべての元 $(t_i)_{i\in I}$ について、

(48) カード$_{A_{(K')}/K'}(\sum_{i\in I}t_i\otimes e_i)= P((t_i)_{i\in I},X)$。

$\varphi : K[\mathbf{T}]\rightarrow K'$ を、$i\in I$ ごとに $T_i$ を $t_i$ に送信する一意の K-代数準同型とします。それは $K[\mathbf{T}$]-代数の $K'$ 構造上の定義するです。 $K'$-代数 $A_{(K[\mathbf{T}])(K')}$ は $A_{(K')}$ (スカラーの拡大の推移性) と識別でき、ここで元 $1\otimes (\sum T_i\otimes e_i)$ は $A_{(K')}$ の元 $\sum t_i\otimes e_i$ と識別されます。 $\varphi$ から推定された $\overline{\varphi}: K[\mathbf{T}][X]\rightarrow K'[X]$ K-代数準同型で表します。 III, §9, No. 3、p. 544の公式 (21)より、$K'$-代数$A_{(K')}$に対する$\sum t_i\otimes e_i$の特性多項式は、$\sum T_i\otimes e_i$の特性多項式の$\overline{\varphi}$により像になります。 $K[\mathbf{T}$]-代数 $A_{(K[\mathbf{T}])}$、つまり $P^n$ を尊重します。その他の語では、

(49) パソコン$_{A_{(K')}/K'}(\sum_{i\in I}t_i\otimes e_i; X)= P((t_i)_{i\in I},X)^n$;

補題 5 は、VIII、p. 339 の補題 2 から続きます。

補題 5 の特定のケース $K'= K$ を考えてみましょう。

(50) カード$_{A/K}(\sum_{i\in I}t_ie_i; X)= P((t_i)_{i\in I},X)$

$K^I$ の元 $(t_i)_{i\in I}$ ごとに。 $K[\mathbf{T},X]$ の多項式 P は次数 $n$ と同次であるため、次のように一意に展開できます。

$$
P(\mathbf{T},X) =\sum_{r=0}^n(-1)^rB_r(\mathbf{T}) X^{n-r} \tag{51}
$$

ここで、$B_r$ は、$K[\mathbf{T}]$ の次数 $r$ の同次多項式です。 公式 (46)、(50)、(51) までに、

$$
b_r(\sum_{i\in I}t_ie_i)= B_r((t_i)_{i\in I})
$$

$K^I$ の元 $(t_i)_{i\in I}$ ごとに。 命題 6が続きます。

#### 注意 {#alg-viii-s17-n4-rem-1 .statement tag=00KX}

$K'$を可換K-代数とします。 $A_{(K')}$ のすべての元 $t$ は、$(t_i)\in {K'}^I$ の場合、$\sum_{i\in I}t_i\otimes e_i$ と書くことができます。 補題 5 の証明から、特性多項式 Pc$_{A_{(K')}/K'}(t; X)$ は $P((t_i),X)^n$ に等しいことがわかります。

### 5. 推移性/被約ノルムと痕跡

#### 命題 7 {#alg-viii-s17-prop-7 .statement tag=00KY}

L を A の最大可換半単純部分代数と L の $a$ 元とします。私たちは持っています

(52) Pcrd$_{A/K}(a; X) =$ PC$_{L/K}(a; X)$、

(53) Trd$_{A/K}(a) =$ Tr$_{L/K}(a)$、

(54) Nrd$_{A/K}(a) = N_{L/K}(a)$。

VIII、p. 262 の命題 3 により、L モジュール A と $L^n$ は同型です。したがって、関係となります。

パソコン$_{A/K}(a; X) =$ パソコン$_{L/K}(a; X)^n$。

多項式 Pc$_{L/K}(a; X)$ はモニックであるため、簡約特性多項式 Pcrd$_{A/K}(a; X)$ (VIII, p. 339, 補題 2) に等しくなります。これにより、公式 (52) が得られます。 (52) の各辺で $X^{n-1}$ の係数 (それぞれ定数項) を比較すると、公式 (53) (それぞれ (54)) が得られます。

#### 系 {#alg-viii-s17-n5-cor-1 .statement tag=00KZ}

D を K 上の有限次数の体と中心 K とします。 $a$ を K の元および D 含む $a$ の L 最大可換部分体とします。私たちは持っています

Pcrd$_{D/K}(a; X) =$ PC$_{L/K}(a; X)$、

(55) トレ$_{D/K}(a) =$ トレ$_{L/K}(a)$、

Nrd$_{D/K}(a) = N_{L/K}(a)$。

実際、D の最大可換部分体 L は、VIII, p. 265 の系 2 による D の最大可換性半単純部分代数です。

#### 命題 8 {#alg-viii-s17-prop-8 .statement tag=00L0}

BをAの単純部分代数とします。Bの中心をLで、AのBの交換子環を$B'$で表します。次に、$B'$ は、体 L を超える中央の単純代数です。 次数を $r$ で減じたものとします。 B の元 $b$ ごとに、関係が得られます。

(56) Pcrd$_{A/K}(b; X) = N_{L[X]/K[X]}$(Pcrd$_{B/L}(b; X)$)$^r$,

(57) 取引$_{A/K}(b) =r$ 取引$_{L/K}$(取引$_{B/K}(b)$)、

(58) Nrd$_{A/K}(b) = N_{L/K}$(Nrd$_{B/L}(b)$)$^r$。

#### 補題 6 {#alg-viii-s17-lem-6 .statement tag=00L1}

$K'$ を K 上の有限次数 $d$ の可換代数とします。

$$
P(X) = X^s+a_1X^{s-1}+\cdots +a_s
$$

$K'$ に係数を含むモニック多項式。 K[X] の多項式 Q = $N_{K'[X]/K[X]}(P)$ は次数 $sd$ のモニックであり、Q(X) の $X^{sd-1}$ の係数は Tr$_{K'/K}(a_1)$ に等しく、Q の定数項は次のようになります。 $N_{K'/K}(a_s)$。

$K''$ で $K'$-代数 $K'[T]/(P(T))$ を、$K''$ での T の標準類を $t$ で表します。 数列 $(1, t, . . . , t^{s-1})$ は $K'$ に対する $K''$ の基底であり、この基底の $t$ による乗法の行列は形の乗法です。

$$
\tau = \begin{pmatrix}
0 & 0 & \cdots & 0 & -a_s \\
1 & 0 & \cdots & 0 & -a_{s-1} \\
0 & 1 & \cdots & 0 & -a_{s-2} \\
\vdots & \vdots & \ddots & \vdots & \vdots \\
0 & \cdots & \cdots & 1 & -a_1
\end{pmatrix}.
$$

$XI_n - \tau$ の行列式は、最初の行に沿って展開することにより、$s$ の帰納法によって計算されます。 $\det(XI_n - \tau) = P(X)$ を取得します。他の語には、$P(X) = Pc_{K''/K'}(t; X)$があります。特に$\operatorname{Tr}_{K''/K'}(t) = -a_1$と$N_{K''/K'}(t) = (-1)^s a_s$。 推移性公式 (III, §9, No. 4、p. 548、系) までに、

$$
\operatorname{Tr}_{K''/K}(t) = -\operatorname{Tr}_{K'/K}(a_1), \quad N_{K''/K}(t) = (-1)^{sd} N_{K'/K}(a_s),
$$
$$
Q(X) = Pc_{K''/K}(t; X).
$$

一方、$[K'' : K] = [K'' : K'][K' : K] = sd$ なので、$Q(X)$ は次数 $sd$ のモニック多項式になります。 補題 6が続きます。

命題 8 を証明しましょう。 環 $B$ は単純なので、その中心 $L$ は体 (VIII, p. 121, 系 1) です。 VIII、p. 259、交換子環の定理 5 により、$A$ の $B$ の $B'$ は、中心 $L$ を含む単純な環となり、等式が得られます。 $[A : K] = [B : K][B' : K]$。 $L$に対する$B'$の減少次数を$r$で表し、$L$に対する$B$の減少$s$を、$K$に対する$L$の減少次数を$d$で表します。我々は持っています

$$
[A : K] = n^2, \quad [B' : K] = r^2 d, \quad [B : K] = s^2 d,
$$

したがって、$n^2 = r^2 s^2 d^2$、つまり $n = rsd$ となります。

$b$ を $B$ の元とし、$P(X)$ を $L$-代数 $B$ 上の縮小特性多項式とする。 次数 $s$ のモニックです。 補題 6 により、多項式 $Q = N_{L[X]/K[X]}(P)$ は次数 $sd$ のモニックになります。したがって、多項式 $R = Q^r$ は次数 $rsd = n$ のモニックです。再び補題 6により、$R(X)$の$X^{n-1}$の係数は$-r \operatorname{Tr}_{L/K}(\operatorname{Trd}_{B/L}(b))$に等しく、$R(X)$の定数項は$(N_{L/K}((-1)^s \operatorname{Nrd}_{B/L}(b)))^r = (-1)^n N_{L/K}(\operatorname{Nrd}_{B/L}(b))^r$です。

$[A : K] = r^2 d[B : K]$ 以降、左側の $B$ モジュール $A$ には階数 $r^2 d$ (VIII、p. 124、命題 5) がありません。したがって、私たちは

$$
\operatorname{Pc}_{A/K}(b; X) = \operatorname{Pc}_{B/K}(b; X)^{dr^2}.
$$

III, §9, No. 4、p. 548 の系までに、

$$
\operatorname{Pc}_{B/K}(b; X) = N_{L[X]/K[X]}(\operatorname{Pc}_{B/L}(b; X)),
$$

そして P(X) は L-代数 B 上の $b$ の縮小特性多項式であるため、次のようになります。

(62) パソコン$_{B/L}(b; X) = P(X)^s$。

最後に、R(X) の公式 (60)—(62) と定義により、次のようになります。

(63) パソコン$_{A/K}(b; X) = N_{L[X]/K[X]}(P(X))^{dr^2s}= Q(X)^{dr^2s}= R(X)^{rsd}= R(X)^n$、

したがって、R(X) は、K-代数 A に対する $b$ の縮小特性多項式です。

公式 (56) を証明しました。 公式 (57) と (58) は、公式 (56) と補題 6 の直後に続きます。これは、Pcrd$_{A/K}(b; X)$ の $X^{n-1}$ の係数が $-$ Trd$_{A/K}(b)$ に等しく、定数項が $(-1)^n$ であるためです。 Nrd$_{A/K}(b)$。

### 6. 被約ノルムと行列式

この小節では、Dは中心KでKを超えた有限次数の体です。 乗法群 $D^*$ の $D^*_{ab}$ 商をその派生 (または交換子) 群で表し、$D^*$ から $D^*_{ab}$ までの $\pi$ 標準準同型で表します。 マッピング Nrd$_{D/K}$ は、$D^*$ から $K^*$ への群準同型性を引き起こします。 K は可換であるため、この準同型写像のカーネルには $D^*$ の派生群が含まれます。 従って、$D^*_{ab}$ から $K^*$ までの一意な準同型 Nrd が存在し、$x\in D^*$ ごとに Nrd$_{D/K}(x) =$ Nrd $\circ \pi (x)$ になります。

#### 命題 9 {#alg-viii-s17-prop-9 .statement tag=00L2}

V を体 D 上の有限次元右ベクトル空間とします。E を体 K 上の代数 End$_D(V)$ とします。それは中央のシンプルで有限次数です。 E のすべての可逆元 $u$ について、次のようになります。

(64) Nrd$_{E/K}(u) =$ Nrd(デット$u$)

(cf. VIII、p. 452、命題 2 は行列式 det $u$ の $u$ の定義です)。

D上のVの次元を$n$と同一視するEを行列環$\mathbf{M}_n(D)$で表します。D上のVの基底を使用します。乗法群GL$_n(D)$の代数Eは対角線によって生成されます。 行列と行列 $B_{ij}(\lambda )$ (II, §10, No. 13、p. 362、系 1)。従って、命題 9 は、以下の 2 つの具体的なケースから導き出されます。

A) $u$ が対角行列 diag($a_1, . . . , a_n$) であると仮定します。すべての $1\leqslant i\leqslant n$ について、$L_i$ を D 含む $a_i$ の最大可換部分体とします。 Lを$1\leqslant i\leqslant n$に対する$t_i\in L_i$の対角行列diag($t_1, . . . , t_n$)のEからなるの部分代数とします。 $d$ を K に対する D の縮小次数とします。$1\leqslant i\leqslant n$ (VIII, p. 265, 系 2) に対して $[L_i: K] =d$ が得られます。 K-代数 L は $L_1\times  \cdots  \times L_n$ と同型なので、次数 $nd$ の半単純です。今は$[E : K] =n^2[D : K] =n^2d^2= [L : K]^2$です。従って、L は E (VIII, p. 262, 命題 3) の最大可換半単純部分代数です。 VIII、p. 346の命題7までに、Nrd$_{E/K}(u) = N_{L/K}(u)$が完成しました。その結果、III, §9, No. 3、p. 544 の公式 (18) までに、

Nrd$_{E/K}(u) =\prod_{i=1}^nN_{L_i/K}(a_i) =\prod_{i=1}^n$ Nrd$_{D/K}(a_i)$

= Nrd$_{D/K}(a_1\cdots a_n) =$ Nrd($\pi (a_1\cdots a_n)$)。

さらに、VIII, p. 453 の命題 3 によって $u=\pi (a_1\cdots a_n)$ が求まり、この場合は公式 (64) が得られます。

B) $u$ が $B_{ij}(\lambda )$ に等しいと仮定します。ここで、$\lambda$ は D の元で、$i, j$ は区間 $[1, n]$ の相異なる整数です。 K に対する D の縮小次数を $d$ で表し、D から K までのスカラーの制限によって V から推定される K 上の M ベクトル空間で表します。このとき、M は単純な E モジュールであり、次のようになります。

(65) PC$_{M/K}(u; X) =$ Pcrd$_{E/K}(u; X)^d$

VIII、p. 341 の公式 (26) による。さらに、M は K 上の次元 $nd^2$ のベクトル空間であり、$u-1_M$ は M の冪零自己準同型です。従って、私たちは

(66) パソコン$_{M/K}(u; X) = (X-1)^{nd^2}$。

公式 (65) と (66) を比較すると、次のようになります。

(67) カード$_{E/K}(u; X) = (X-1)^{nd}$

特にNrd$_{E/K}(u) = 1$。 VIII、p. 453 の命題 3 による det $u= 1$ もあります。したがって、この場合には公式 (64) が成り立ちます。

#### 注意 {#alg-viii-s17-n6-rem-1 .statement tag=00L3}

E の元 $u$ が可逆でない場合 (VIII、p. 340、命題 3)、Nrd$_{E/K}(u) = 0$ が得られます。

### 練習問題 {#alg-viii-s17-exercises}

[§ 17 に対して練習問題](exercises/s17/)を参照してください。
