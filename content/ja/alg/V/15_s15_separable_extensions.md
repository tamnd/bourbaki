---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 15
section_title: Separable extensions
lang: ja
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.118-A V.126, A V.175-A V.177
pdf_pages: 0232-0240, 0289-0291
extraction: ocr
subsections:
    - "no": 1
      title: Characterization of the nilpotent elements of a ring
      page: 118
      pdf_page: 232
    - "no": 2
      title: Separable algebras
      page: 119
      pdf_page: 233
    - "no": 3
      title: Separable extensions
      page: 121
      pdf_page: 235
    - "no": 4
      title: Mac Lane's separability criterion
      page: 122
      pdf_page: 236
    - "no": 5
      title: Extensions of a perfect field
      page: 125
      pdf_page: 239
    - "no": 6
      title: The characterization of separability by automorphisms
      page: 125
      pdf_page: 239
statements: 21
exercises: 12
content_sha256: 661c90dee025f9bb89a79c6cabe8264203cc246c24767579d1392c61d33d2a59
translated_from: content/en/alg/V/15_s15_separable_extensions.md
translation_method: google
source_content_sha256: 29004e5cd09fd460bf5167f0e6481b43d3d6e1b88934fe63c99d9a4a216f82d7
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 78a281ca2f8acafc27fb02319d1c9267c9e812bacb3e66beca42e0123f271c66
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 15。 分離拡大

### 1. 特徴付け/冪零元/環

#### 命題 1 {#alg-v-s15-prop-1 .statement tag=06TN}

— *A を A の可換環および x 元とします。x がゼロポテントであるためには、$1 - xT$ が環 $A[T]$ で可逆であることが必要かつ十分です。*

$A[T]$ は形式的な冪系列環 $A[[T]]$ の部分環であり、$1 - xT$ は $A[[T]]$ の逆数 $\sum_{n=0}^{\infty} x^n T^n$ を持っていることに注意してください (IV, p. 30、提案 5)。 $A[T]$ において $1 - xT$ が可逆であるためには、 $\sum_{n=0}^{\infty} x^n T^n$ が多項式であること、つまり x が零能であることが必要かつ十分です。

#### 命題 2 {#alg-v-s15-prop-2 .statement tag=06TO}

— *A を可換環とします。 A の冪零元の集合は、A のすべての素イデアルの集合の共通部分に等しい A のイデアルです。*

x を A の冪零元とし、p を A の素イデアルとします。 $x \mod p$ の剰余類は整域 $A/p$ の冪零元であるため、零です。したがって、$x \in p$ になります。

x を A の非零元要素とします。提案 1 により、$A[T]$ の主イデアル $(1 - xT)$ は $A[T]$ とは異なります。クルールの定理 (I, p. 104) により、$A[T]$ 含む $1 - xT$ の最大理想 m が存在します。この場合、m は $A[T]$ の素イデアルであるため、$p = A \cap m$ は A の素イデアルです。 $1 \notin m$ と $1 - Tx \in m$ があるため、$Tx \notin m$ と *なおさら* $x \notin p$ になります。

したがって、A の冪零元の集合 $\mathfrak{n}$ は、A のすべての素イデアルの集合の共通部分であることを示しました。理想のすべての共通部分は理想であるため、$\mathfrak{n}$ も理想です。

#### 系 {#alg-v-s15-n1-cor-1 .statement tag=06TP}

— *可換環が還元される* (*V*、p. 34、定義 2) *それが体* の積の部分環と同型であることが必要かつ十分です。

条件で十分であることは明らかです。

$\mathbf{A}$ を減らしてみましょう。 提案 2 により、$\mathbf{A}$ の素イデアルの集合の共通部分 $n$ は 0 に減らされます。 $\mathbf{A}$ のすべての素イデアル $\mathfrak{p}$ について、$k(\mathfrak{p})$ を $\mathbf{A}/\mathfrak{p}$ と $\mathbf{A}$ から $k(\mathfrak{p})$ への正準準同型性の分数体である $\varphi_n$ とします。 $\varphi$ を $\mathbf{A}$ の準同型から $\prod_{\mathfrak{p}} k(\mathfrak{p})$ にすると、添字 $\mathfrak{p}$ の成分は $\varphi_{\mathfrak{p}}$ になります。 $\varphi_{\mathfrak{p}}$ の核は $\mathfrak{p}$ であるため、$\varphi$ のそれは $n = 0$ です。したがって、$\varphi$ は、$\mathbf{A}$ の同型から $\prod_{\mathfrak{p}} k(\mathfrak{p})$ の部分環になります。

### 2. 分離可能代数

#### 定義 1 {#alg-v-s15-def-1 .statement tag=06TQ}

*$\mathbf{A}$を体$K$の上に可換代数とします。このとき、$A$ は $K$ 上で可分であると言われます。あるいは、環 $L \otimes_K \mathbf{A}$ が $K$* の拡大 $L$ ごとに還元される場合、$K$-代数も可分であると言われます。

すべての可分な代数は明らかに還元されます。部分的な逆については、Th を参照してください。 3 (*V*、p. 125)。

#### 例 {#alg-v-s15-n2-exa-1 .statement tag=0DI7}

*1*) $\mathbf{A}$ を多項式代数 $K[X_i]_{i \in I}$ とします。 $K$ 環 $L \otimes_K \mathbf{A}$ のすべての拡大 $L$ は、$L[X_i]_{i \in I}$ (III, p. 449, 注意 2) と同型であるため、整域 (*IV*, p. 9、提案 8)。他の語では、体 $K$ 上のすべての多項式代数は分離可能な $K$-代数です。

2) $\mathbf{A}$ を体 $K$ 上の有限次数の可換代数とします。 $\mathbf{A}$ が分離可能であるためには、それが etale (*V*, p. 34, Th. 4) であることが必要かつ十分です。

3) $E$ を体 $K$ の代数拡大とします。 $L$ が $K$ の拡張である場合、リング $L \otimes_K E$ は部分リング $L \otimes_K F$ の和集合であり、ここで $F$ は $E$ の有限次数のすべての部分拡張のセットに及びます。したがって、リング $L \otimes_K E$ は、$K$ を超える有限次数の $E$ のすべてのサブエクステンション $F$ について、これが $L \otimes_K F$ に当てはまる場合にのみ縮小されます。 例 2 を考慮すると、上記の定義の意味で、$E$ は分離可能な代数であることがわかります。 1 は、定義の意味で可分代数拡大である場合に限ります。 *V*、p. 36 の 1 つ。

#### 命題 3 {#alg-v-s15-prop-3 .statement tag=06TR}

*$K$を体*とします。

a) *可分な $K$-代数のすべての部分代数は可分です*。

b) *分離可能な $K$-代数の直接極限はすべて分離可能です*。

c) *分離可能な $K$-代数のすべての積は分離可能です*。

d) *$\mathbf{A}$ を $K$-代数、$K'$ 拡大を $K$ とします。 $\mathbf{A}$ が分離可能であるためには、$\mathbf{A}$ からスカラーの拡大によって得られる $K'$-代数 $\mathbf{A}_{(K')}$ が分離可能であることが必要かつ十分です*。

$L$ を $K$ の拡大とします。 $\mathbf{A}$ を、$\mathbf{A}$ の $K$ と $B$ 部分代数上の分離可能な代数とします。次に、環 $L \otimes_K \mathbf{A}$ は還元され、$L \otimes_K B$ は $L \otimes_K \mathbf{A}$ の部分環と同型であるため、還元されます。したがって、$B$ は分離可能であり、*a)* が証明されます。 *同様に* $b$) は、$L \otimes_K \varprojlim A_i$ の標準同型と $\varprojlim L \otimes_K A_i$ (II, p. 290, 提案 7) および $c$) を使用して証明できます。これは、$L \otimes_K \left( \prod_{i \in I} A_i \right)$ が以下と同型であることを指摘することで証明されます。 $\prod_{i \in I} (L \otimes_K A_i)$ の部分環 (II、p. 306、提案 15)。

$d$ の記法を使用します)。 $K'$ 環 $L' \otimes_{K'} A_{(K')}$ と $L' \otimes_K A$ のすべての拡大 $L'$ については、同型です (II、p. 278、提案 2)。 $A$ が分離可能な $K$-代数である場合、$A_{(K')}$ は分離可能な $K'$-代数であると結論する考えます。逆に、 $A_{(K')}$ が分離可能な $K'$-代数 であると仮定します。前述の注意は、サブ拡張として $K$ 含む $K'$ の拡大 $L'$ ごとに $L' \otimes_K A$ が削減されることを示しています。 $L$ を $K$ の拡大とします。 Scholium (V, p. 13) によると、部分拡張として $K$ 含む $K'$ の拡大 $L'$ と、$L$ から $L'$ への $K$ 準同型性が存在します。したがって、環 $L \otimes_K A$ は、$L' \otimes_K A$ の部分環と同型であるため、縮小されます。これは、$A$ が可分な $K$-代数であることを証明します。

#### 命題 4 {#alg-v-s15-prop-4 .statement tag=06TS}

— *$A$ を体 $K$ の分離可能な代数とし、$B$ を $A$ の分数の合計環とします。その場合、$K$-代数 $B$ は分離可能です。*

$S$を$A$のキャンセル可能元の集合とします。 $A$ は $B$ (I、p. 113) の部分環と識別されました。さらに、$S$ のすべての元は $B$ で反転可能であり、$B$ のすべての元には $a \in A$ と $s \in S$ を含む形 $a s^{-1}$ があります。 $L$ を $K$ の拡大と $x$ $L \otimes_K B$ の冪零元とします。その場合、$x$は形に書かれる可能性があります
$$
x = \sum_{i=1}^n y_i \otimes a_i s_i^{-1}
$$
$1 \leq i \leq n$ に対して $y_i \in L, a_i \in A, s_i \in S$ を使用します。 $s = s_1 \ldots s_n$とすると
その後、$x(1 \otimes s)$ 属するから部分環 $L \otimes_K A$ の $L \otimes_K B$ へ。 $x(1 \otimes s)$ は零であり、$A$ は $K$ で分離可能であるため、$x(1 \otimes s) = 0$ が得られ、$s$ は$B$ で可逆であるため、$x = 0$ がわかります。これにより、環 $L \otimes_K B$ が減少し、よって命題となることがわかります。

#### 命題 5 {#alg-v-s15-prop-5 .statement tag=06TT}

— *$K$ を体および $A, B$ 可換$K$-代数とする。 $A$ が約定され、$B$ が分離可能であれば、$A \otimes_K B$ が約定されます。*

コルによって。提案 2 の (V, p. 119) $A$ は、積 $\prod_{i \in I} L_i$ の部分代数と同型です。ここで、$L_i$ は、$i \in I$ に対する $K$ の拡大です。したがって、$A \otimes_K B$ は $\left( \prod_{i \in I} L_i \right) \otimes_K B$ の部分環と同型であり、後者の環は $\prod_{i \in I} (L_i \otimes_K B)$ の部分環と同型です (II、p. 306、提案 15)。 $B$ は分離可能なので、環 $L_i \otimes_K B$ はそれぞれ約分され、$\prod_{i \in I} (L_i \otimes_K B)$ と $A \otimes_K B$ の *なおさら* も同様になります。

#### 系 1 {#alg-v-s15-prop-5-cor-1 .statement tag=06TU}

— *$K$ を $K$ および $f$ の体、$L$ 分離拡大を $K[X]$ の多項式とします。 $f$ の $K[X]$ に倍数因子がない場合、$L[X]$ にも倍数因子がありません。*

$f$ に $K[X]$ に倍数因子がない場合、商環 $K[X]/(f)$ が減らされます。 for $f$ は、対において既約多項式 $f_i$ の積は互いに素であるため、

K[X]/(f) は、I、p. 110、提案 9 により、体 K[X]/(f_i) の積と同型です。提案 5 により、環 L[X]/(f) は L ⊗_K K[X]/(f ) と同型であり、縮小されます。 g が g^2 割る f となるような L[X] の非定数多項式である場合、L[X]/(f) の fg^{-1} の剰余類は非ゼロ冪零元です。したがって、 f には L[X] に倍数因子がありません。

#### 系 2 {#alg-v-s15-prop-5-cor-2 .statement tag=06TV}

— A と B を 2 可換K-代数とします。 *A と B が分離可能な場合*、同じことが A ⊗_K B にも当てはまります。

L を K の拡大とします。 環 L ⊗_K A は分離可能であるため、A は削減されます。ここで、提案 5 は、環 (L ⊗_K A) ⊗_KB (L ⊗_K (A ⊗_K B) と同型) が削減される、よって系を示しています。

### 3. 分離拡大

Kを体とします。 K の任意の拡大は K-代数なので、Def で導入された分離可能性の概念です。 1 (V, p. 119) は特に K の拡大の場合に当てはまります。 例 3 (V, p. 119) により、代数拡大の場合の分離可能性の定義は § 7 の分離可能性と一致します。 (V、p. 36、定義 1)。

#### 命題 6 {#alg-v-s15-prop-6 .statement tag=06TW}

— *体* K のすべての純粋な拡大は分離可能です。
これは例 1 (V, p. 119) と提案 4 (V, p. 120) から一気に続きます。

#### 命題 7 {#alg-v-s15-prop-7 .statement tag=06TX}

— E を体、G を E の *自己同型* の群、K を G の不変量の E からなるの *部分体* とします。このとき、E は K の分離拡大です。

L を K の拡大とします。 L の代数閉拡大 Ω が存在します。その K に対する超越性次数は、K に対する E の超越性と少なくとも等しいです。 1 (V, p. 117) E から R への K 準同型性 u が存在します。 A = Ω ⊗_K E から Ω への写像 λ ⊗ x から λ へのΩ代数準同型性を v で表します。 λ ∈ Ω および x ∈ Ω の場合は u(x)。 v の核に a を書きます。

すべての s ∈ G について、h_s を 0-代数 A の自己同型 Id, ⊗ s とします。 A の Ω への準同型写像 v ∘ h_s のカーネルは、A の素イデアル a_s = h_s^{-1}(a) です。 A の理想的な b = ⋂_{s ∈ G} a_s が自己同型 h_s の下で安定していることは明らかです。 したがって、(V, p. 63, Cor.) 理想 b は形 c ⊗_K E になります。ここで、c は Ω の理想です。 b ⊂ a ≠ A なので、 c ≠ Ω; Ω が体であるため、c = 0 となり、b = 0 となります。

したがって、A の素イデアルの族 (a_s)、_s ∈ G は零共通部分を持ちます。提案 2 (V, p. 118) により、環は約定され、なおさら同じことが A の部分環 L ⊗_K E にも当てはまります。L は K の任意の拡大であるため、これは E が K 上で分離可能であることを証明します。

#### 命題 8 {#alg-v-s15-prop-8 .statement tag=06TY}

— L を体 K の拡大とします。L が K 上で分離可能である場合、L のすべての部分拡張は K 上で分離可能です。逆に、L のすべての有限生成された部分拡張が K 上で分離可能である場合、L は K 上で分離可能です。

これは、提案 3、a) および b) (V、p. 119) からすぐに得られます。

したがって、可分性は«有限指標»の性質と呼ばれることがあります。

#### 命題 9 {#alg-v-s15-prop-9 .statement tag=06TZ}

— L を体 K の拡大とし、M を可換L-代数 (たとえば、L の拡大) とします。 M が L で分離可能であり、L が K で分離可能である場合、M は K で分離可能です。

K' を K の拡大とします。L は K の分離拡大であるため、環 $K' \otimes_K L$ は減算されます。 M は分離可能な L-代数であるため、提案 5 (V, p. 120) は環 $(K' \otimes_K L) \otimes_L M$ が還元されることを示しています。ここで、環 $K' \otimes_K M$ は $(K' \otimes_K L) \otimes_L M$ (II、p. 278、提案 2) と同型であるため、簡約されます。これは、M が K に関して分離可能であることを証明します。

拡大 M が K 上で分離可能である場合、それは必ずしも L 上で分離可能ではありません (cf. ただし、V、p. 124、Cor. 3)。たとえば、p が素数数の場合、$F_p$ 上の 1 つの不定数 X における有理分数の体 $F_p(X)$ は、$F_p$ (V, p. 121、提案 6) 上で分離可能ですが、これは p 根です。代数拡大/$F_p(X^p)$;特に $F_p(X)$ は $F_p(X^p)$ 上で分離できません。

後で (V、p. 137 提案 5) 複合材料拡大の分離性を検討します。

### 4. マクレーンの分離可能性基準

#### 定理 1 {#alg-v-s15-thm-1 .statement tag=06U0}

— K を標数 0 の体とします。K のすべての換算された K-代数、特にすべての拡大は K 上で分離可能です。

まず、K のすべての拡大 L が分離可能であることを示します。 B を K (V, p. 109, Th. 1) に対する L の超越基底とし、$L_1 = K(B)$ とします。このとき、$L_1$ は K 上で分離可能です (V, p. 121、提案 6)。さらに、L は $L_1$ の代数拡大であり、$L_1$ は標数 0 の体です。したがって、L は $L_1$ (V、p. 37、Cor.) 上で分離可能です。したがって、提案 9 により、L は K 上で分離可能です。

ここで、A を体 K よりも減じた代数とします。提案 2 (V, p. 119) では、A が $\prod_{i \in I} L_i$ の部分代数と同型であるような、K の拡大の族 $(L_i)_{i \in I}$ が存在します。 代数 $L_i$ のそれぞれは、これまで述べてきたことによって K 上で分離可能であるため、提案 3 a) および c) (V、p. 119) により、A は同じ性質を持ちます。

#### 定理 2 {#alg-v-s15-thm-2 .statement tag=06U1}

— K を特性 $p \neq 0$ の体、K と A 可換K-代数の完全閉包 $K^{p^{-\infty}}$ とします。次のプロパティは同等です。
a) A は分離可能です。
b) K' が完全で、$K' \otimes_K A$ が縮小されるような K の拡大 K' が存在します。
c) 環 $K^{p^{-\infty}} \otimes_K A$ が減少します。

d) *環* $K' \otimes_K A$ *は、* 有限次数および* $p$* 高さの基数* $\leqslant 1$ の * $K$ * の拡大* $K'$ ごとに減らされます。

e) *すべてのファミリー* $(a_i)_{i \in I}$、* $A$ の元について * $K$、*ファミリー* $(a_i^p)_{i \in I}$、* $K$ にわたって直線的にフリー。

f) *基底* $(a_i)_{i \in I}$、*ベクトル* $K$*-space* $A$ *家族* $(a_i^p)_{i \in I}$、* $K$ 上で直線的に自由であることは残念です。

$K$ の拡大 $K'$ が完全体である場合、含むは$K^{p^{-\infty}}$ と同型の部分拡張 $K$ ($V$、p. 6、提案 3)。さらに、$K$ のすべての $p$ ラジカル拡張は、$K^{p^{-\infty}}$ の部分拡張と同型です ($V$、p. 26、提案 3)。これらの注意は $a) \Rightarrow b) \Rightarrow c) \Rightarrow d)$ の意味を示しています。

d) が e) を意味することを証明しましょう。 $(a_i)_{i \in I}$ を $A$ の線形自由族とし、$(A_i)_{i \in I}$ を $\sum \lambda_i a_i^p = 0$ となるような $K$ の有限台の族とする。 $K'$ を、元 $\lambda_i^{p^{-1}}$ によって生成された $K^{p^{-\infty}}$ のサブ拡張子とします。身長有限次数、高さ$\leqslant 1$です。 $K' \otimes_K A$に$x = \sum_{i \in I} \lambda_i^{p^{-1}} \otimes a_i$を入れます。我々は持っています

$$
x^p = \sum_{i \in I} \lambda_i \otimes a_i^p = 1 \otimes \sum_{i \in I} \lambda_i a_i^p = 0
$$

仮定 d) までに、すべての $i \in I$ に対して $x = 0$、よって $A_i = 0$ が得られます。

明らかに e) は f) を暗示しますが、f) が a) を暗示することはまだわかりません。したがって、$(a_i)_{i \in I}$ を $K$ 上の $A$ の基底とし、ファミリ $(a_i^p)_{i \in I}$ が $K$ 上で線形自由になるようにします。 $L$ を $K$ の拡大とし、$x$ を $L \otimes_K A$ の元として、$x^p = 0$ とします。 $i \in I$ をすべて $A_i \in L$ で$x = \sum_{i \in I} \lambda_i \otimes a_i$ と書きます。 $x^p = \sum_{i \in I} \lambda_i^p \otimes a_i^p = 0$ があり、家族 $(a_i^p)_{i \in I}$ は $K$ を超えて直線的に自由であるため、すべての $i \in I$ に対して $\lambda_i^p = 0$、よって $\lambda_i = 0$ が得られます。 $x = 0$ となります。したがって、$x^p = 0$ は $L \otimes_K A$ の $x = 0$ を暗示しており、そこからすぐに $L \otimes_K A$ が減少することがわかります。

#### 系 1 (マクレーン) {#alg-v-s15-thm-2-cor-1 .statement tag=06U2}

— *$K$ *を特性指数* $p$ の体、$\Omega$ * $K$ * および* $L$ * $\Omega$ の部分拡張* の *完全な拡大とします。 *次の条件は同等です*:

a) $L$ *$K$ 上で分離可能です。

b) $L$ *$K^{p^{-\infty}}$ *$K$ から直線的に互いに素です。

c) $L$ *$K$ *すべて* $p$*の根元拡張* $K$ *に含まれる* $\Omega$、*有限次数と高さ* $\leqslant 1$ に対して線形に素です。

$K$ が標数 0 である場合は、慣例により $L$ が $K$ (Th. 1) と $K^{p^{-\infty}} = K$ で分離可能であるため、自明です。 $p \neq 1$ と仮定して、まず a) が b) を意味することを示しましょう。 $L$ が $K$ 上で分離可能であると仮定し、$(a_i)_{i \in I}$ を $K$ 上の $L$ の基底とします。 $(\lambda_i)_{i \in I}$ を、$\sum_{i \in I} \lambda_i a_i = 0$ となるような $K^{p^{-\infty}}$ の元の有限台の族とする。 λ_i = μ_i^{p^{-f}} となるような K の整数 $f \geqslant 0$ と元 μ_i が存在します。我々は持っています

$$
\sum_{i \in I} \mu_i a_i^{p^f} = \left( \sum_{i \in I} \lambda_i a_i \right)^{p^f} = 0
$$

そしてTh。 2 は、f 上の帰納法によって、族 $(a_i^{p^f})_{i \in I}$ が K 上で線形自由であることを意味します。したがって、すべての $i \in I$ に対して $\mu_i = 0$、よって $\lambda_i = 0$ が得られます。最後に、L は K 上で $K^{p^{-\infty}}$ から直線的に互いに素になります。

b) が c) を意味することは明らかです。最後に c) が成り立つと仮定し、K' を有限次数の K の拡大と高さ $\leq 1$ の p-ラジカルとする。 環 $K' \otimes_K L$ は $\Omega$ の部分環と同型であるため、縮小されます。さて、それはThから続きます。 2 L は K 上で分離可能です。

#### 系 2 {#alg-v-s15-thm-2-cor-2 .statement tag=06U3}

— *K を特性指数 p の体、K の完全閉包 $K^{p^{-\infty}}$、および K の L 分離拡大とします。すると、環 $L \otimes_K K^{p^{-\infty}}$ は体になります。さらに、L が K 上の代数である場合、$L \otimes_K K^{p^{-\infty}}$ は L の完全閉包です。*

$p = 1$ の場合は自明なので、$p \neq 1$ と仮定します。 $\Omega$ を L の完全な終結とします。コル著1 $L \otimes_K K^{p^{-\infty}}$ の K-代数準同型が $L[K^{p^{-\infty}}]$ に存在し、$x \in L$ と $y \in K^{p^{-\infty}}$ には写像 $x \otimes y$ から $xy$ が存在します。 $K^{p^{-\infty}}$ は K 上の代数であるため、環 $L[K^{p^{-\infty}}]$ は $\Omega$ の部分体 (V, p. 18、Cor. 1)。さらに、L が K 上の代数であると仮定すると、$L[K^p]$ は完全体 $K^{p^{-\infty}}$ の代数拡大であるため、完全体 (V, p. 43, Cor. 1) となります。最後に、体 $L[K^{p^{-\infty}}]$ は L (V, p. 25, Cor.) の ap-radical 拡張であるため、L の完全な閉包になります。

#### 系 3 {#alg-v-s15-thm-2-cor-3 .statement tag=06U4}

— *L を K の代数拡大とし、M を可換 L-代数 (例えば L の拡大) とします。 M が K 上で分離可能であれば、L 上でも分離可能です。*

代数 L は M の部分代数と K 同型であるため、 L は K の分離拡大です。 したがって (Cor. 2) $K^{p^{-\infty}} \otimes_K L$ に対する $L^{p^{-\infty}}$ の L 同型が存在します。したがって、環 $L^{p^{-\infty}} \otimes_L M$ は $(K^{p^{-\infty}} \otimes_K L) \otimes_L M$ と同型であり、$K^{p^{-\infty}} \otimes_K M$ (II, p. 278、提案 2) と同型であり、後者の環は M が K 上で分離可能であるため還元されます。 したがって、環 $L^{p^{-\infty}} \otimes_L M$ は還元され、M が証明されるL (V, p. 122, Th. 2) 上で分離可能です。

#### 注意 {#alg-v-s15-n4-rem-1 .statement tag=06U5}

— マクレーンの基準は、L 以外の K の拡大を導入せずに定式化することができます。 Cor の c) による。 1、L と $K^P$ が K 上で線形互いに素である場合に限り、L は K 上で分離可能です。 写像 $x \mapsto x^p$ は部分体 $L^P$ 上で L の同型であるため、次が得られます。基準 (cf. V、p. 177、代数の類似基準の例 11):

*L は、部分体 $L^P$ と L の K が $K^P$ 上で線形互いに素である場合に限り、K 上で分離可能です。*

### 5. 拡大/完全体

参照しやすいように、完全体の拡大の主なプロパティを要約します。

#### 定理 3 {#alg-v-s15-thm-3 .statement tag=06U6}

— K を完全体とします。
a) K のすべての代数拡大は完全体です。
b) K のすべての拡大は分離可能です。
c) K-代数が分離可能であるためには、それが削減されることが必要かつ十分です。
d) A と B を 2 で還元したK-代数とします。すると$A \otimes_K B$が減ります。
e) E と F が K の 2 つの拡大である場合、環 $E \otimes_K F$ は減算されます。

主張 a) は単なる Cor です。提案 11 の 1 (V、p. 43)。
主張 b) Th から続きます。 K が特性 0 で Cor からの場合、1 (V、p. 122)。 K が特性 $p \neq 0$ の場合、1 (V、p. 123)。
c)を証明しましょう。 K が特性 0 である場合は、Th から導かれます。 1 (V、p. 122)。したがって、K が標数 $p \neq 0$ の完全であり、A が縮小された K-代数である場合、A は K 上で分離可能であることを示すだけで十分です。ただし、これは Th の条件 a) と b) の同値から導き出されます。 2 (V, p. 122; b) で $K' = K$ を取ります)。
最後に、c) と提案 5 (V、p. 120) から d) が導かれ、e) は d) の特殊なケースです。

### 6. 特徴付けによる分離可能性の自己同型

#### 定理 4 {#alg-v-s15-thm-4 .statement tag=06U7}

— $\Omega$ を体 K の代数閉拡大とし、L を $\Omega$ のサブエクステンションとします。したがって、次の条件は同等です。
a) L は K 上で分離可能です。
b) $\Omega \otimes_K L$ から $\Omega$ への 0 代数準同型の核の共通部分は 0 に還元されます。
c) K 上で線形独立な L の任意の元 $a_1, \ldots, a_n$ に対して、 $\det(\sigma_i(a_j)) \neq 0$ となるような $\Omega$ の K 自己同型 $\sigma_1, \ldots, \sigma_n$ が存在します。
d) V を有限次元の L のサブ K 空間ベクトルとする。 V の $\Omega$ へのすべての K-線型写像は、$\Omega$ の K 自己同型の制限から V の線形結合 (R の係数を含む) です。

$d) \Rightarrow c)$: $a_1, \ldots, a_n$ を K 上で線形独立な L の元とし、V を $a_1, \ldots, a_n$ によって生成された L のベクトルサブ K 空間とします。 写像 $f \mapsto (f(a_1), \ldots, f(a_n))$ は、$\mathrm{Hom}_K(V, R)$ から $\Omega^n$ への R 線形全単射です。 d) が成り立つと仮定すると、$\Omega^n$ の元 $(\sigma_i(a_1), \ldots, \sigma_i(a_n))$ ($1 \leq i \leq n$ の場合) 形基底の $\Omega^n$ となるような $\Omega$ の K 自己同型 $a_1, \ldots, a_n$ が存在します。したがって、$\det(\sigma_i(a_j)) \neq 0$ があるため、d) は c) を意味します。

c) $\Rightarrow$ b): c) が成立し、x が $\Omega \otimes_K L$ であると仮定します。 形 $\sum_{j=1}^n x_j \otimes a_j$ に x を書き、$\Omega$ の $x_1, \ldots, x_n$ と L の元 $a_1, \ldots, a_n$ は K 上で線形独立です。 選ぶ K 自己同型 $\sigma_1, \ldots, \sigma_n$ の $\Omega$ は次のようになります。 $\det \sigma_i(a_j) \neq 0$; $\chi_1, \ldots, \chi_n$ を、$a \in \Omega$ と $b \in L$ に対して $\chi_i(a \otimes b) = a \cdot \sigma_i(b)$ となるような、$\Omega \otimes_K L$ の $\Omega$ への R 準同型写像とします。 $1 \leq i \leq n$ に対して $\chi_i(x) = 0$、他の語に対して、$1 \leq i \leq n$ に対して $\sum_{j=1}^n x_j \cdot \sigma_i(a_j) = 0$ があるとします。 行列 $(\sigma_i(a_j))$ にはゼロ以外の行列式があると仮定しているため、$1 \leq i \leq n$ には $x_i = 0$ があり、したがって $x = 0$ になります。

b) $\Rightarrow$ a): 特性 0 の体のすべての拡大は分離可能 (V、p. 122、Th. 1) であるため、K が特性 $p \neq 0$ である場合を調べるだけで十分です。 X を $\Omega \otimes_K L$ から $\Omega$ へのすべての R 代数準同型写像の集合とし、 f​​ を $u \in \Omega \otimes_K L$ の $f(u) = (\chi(u))_{\chi \in X}$ によって定義される $\Omega \otimes_K L$ から $\Omega^X$ への準同型写像とする。 条件 b) は f が単射であることを意味し、したがって環 $\Omega \otimes_K L$ が約定されることを意味します。 したがって、Th の条件 b) となります。 2 (V, p. 122) は $K' = \Omega$ で満たされるため、L は K 上で分離可能です。

a) $\Rightarrow$ d): L が K 上で分離可能であるとします。V を、L の有限次元のベクトルサブ K 空間、$V_{(\Omega)} = \Omega \otimes_K V$ ベクトル V から導出された $\Omega$ 空間とします。スカラーの拡大と $V_{(\Omega)}$ の $f_0$ 線型形式により、$x \in \Omega, y \in V$ に対して $f_0(x \otimes y) = xy$ が得られます。 $\Omega$ の K 自己同型の G 群で表します。 $\sigma \in G$ には $\sigma_V = \sigma \otimes \mathrm{Id}_V$ と $g_\sigma = \sigma \circ f_0 \circ \sigma_V^{-1}$ を入れます。

$V_{(\Omega)}$ から $\Omega$ への各 $\sigma \in G$ 写像 $g_\sigma$ は $\Omega$ 線形であり、$x \in \Omega, y \in V$ の場合は写像 $x \otimes y$ から $x \cdot \sigma(y)$ です。したがって、$g_\sigma$ の核 $N_\sigma$ は、$V_{(\Omega)}$ のベクトル部分空間となり、$N = \cap_{\sigma \in G} N_\sigma$ についても同様です。 p が K の標数指数である場合、$\Omega$ における G の不変量の体は $K^{p^{-\infty}}$ に等しい (V, p. 112、提案 10)。すべての $\sigma \in G$ に対して $\sigma_V(N) = N$ があることは明らかです。したがって (V, p. 63, Cor.) ベクトル $\Omega$-スペース N は $N_0 = N \cap (K^{p^{-\infty}} \otimes V)$ によって生成されます。 L は K 上で分離可能であるため、体 $K^{p^{-\infty}}$ と L は K 上で線形互いに素 (V、p. 123、Cor. 1)。 $x \in \Omega$と$y \in V$には$K^{p^{-\infty}} \otimes_K V \subset K^{p^{-\infty}} \otimes_K L$と$f_0(x \otimes y) = xy$があります。したがって、$f_0$ から $K^{p^{-\infty}} \otimes_K V$ の制限は単射法であることがわかります。現在、$f_0 = g_1$はNでは零、$N_0 \subset K^{p^{-\infty}} \otimes_K V$ではなおさらです。したがって、$N_0 = 0$、よって $N = 0$ となります。 V は K に対して有限次元であるため、$V_{(\Omega)}$ は $\Omega$ に対して有限次元です。 線型形式 $g_\sigma$ の核の共通部分は零であるため、(II, p. 301, Th. 7) 家族 $(g_\sigma)_{\sigma \in G}$ 生成するは $V_{(\Omega)}$ の双対です。ここで、$u$ を V の K-線型写像から $\Omega$ にします。 $\tilde{u}$ を $V_{(\Omega)}$ で線型形式とし、$x \in \Omega$ と $y \in V$ では写像 $x \otimes y$ から $xu(y)$ とします。これまでに述べられたことにより、G の元 $\sigma_1, \ldots, \sigma_n$ と $\Omega$ の $\lambda_1, \ldots, \lambda_n$ が存在し、すべての $y \in V$ に対して $\tilde{u} = \sum_{i=1}^n \lambda_i g_{\sigma_i}$、よって $u(y) = \sum_{i=1}^n \lambda_i \sigma_i(y)$ が存在します。したがって、a) が d) を意味することを示しました。

### 練習問題 {#alg-v-s15-exercises}

[§ 15 に対して練習問題](exercises/s15/)を参照してください。
