---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 2
section_title: Maximal tori of compact Lie groups
lang: ja
source: lie-vii-ix
book_pages: 287-295, 391-394
pdf_pages: 0294-0302, 0398-0401
extraction: native+ocr
subsections:
    - "no": 1
      title: CARTAN SUBALGEBRAS OF COMPACT ALGEBRAS
      page: 287
      pdf_page: 294
    - "no": 2
      title: MAXIMAL TORI
      page: 288
      pdf_page: 295
    - "no": 3
      title: MAXIMAL TORI OF SUBGROUPS AND QUOTIENT GROUPS
      page: 291
      pdf_page: 298
    - "no": 4
      title: SUBGROUPS OF MAXIMAL RANK
      page: 292
      pdf_page: 299
    - "no": 5
      title: WEYL GROUP
      page: 293
      pdf_page: 300
    - "no": 6
      title: MAXIMAL TORI AND COVERING OF HOMOMORPHISMS
      page: 295
      pdf_page: 302
statements: 32
exercises: 11
content_sha256: c6f443d4778433bce8034afc57d220578ee6be77ffaa4b9ddf81f5c7c5cf72ae
translated_from: content/en/lie/IX/02_s2_maximal_tori_of_compact_lie_groups.md
translation_method: google
source_content_sha256: 09376883a430ceee6e2f9d7416163648064cb06680a75c0f4d800750884c66c2
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 5a375f892b1da4a9a918db010ac990f65bdbbe803b8308936081810d027442de
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 2。 コンパクト・リー群の最大トーラス

### 1. カルタン部分代数のコンパクト代数

#### 補題 1 {#lie-ix-s2-lem-1 .statement tag=019Z}

Gをリー群、KをGの圧縮部分群、FをL(G)上の不変双線形形式とする。 $x, y\in L(G)$ にしましょう。すべての $u\in L(K)$ に対して $F(u$,[(Ad $k$)$(x), y]) = 0$ となるような K の元 $k$ が存在します。

写像 $v \rightarrow$ F((Ad $v$)$(x), y$) K から $\mathbf{R}$ までは連続であるため、点 $k\in K$ のどこかで最小値を持ちます。 $u\in L(K)$を入れてください

$h(t) =$ F((広告exp($tu$)$.k$)$(x), y$)$,t\in \mathbf{R}$。

すべての $t$ に対して $h(t)\geq h(0)$ があります。さらに、Chap。 III, §3, no. 12、提案 44、

$\frac{dh}{dt}(0) = F([u$,(広告$k$)$(x)], y) = F(u$,[(広告$k$)$(x), y])$,

したがって、補題 (実数変数の写像、第 I, §1, no. 7、提案 7)。

#### 定理 1 {#lie-ix-s2-thm-1 .statement tag=01A0}

$\mathfrak{g}$ をコンパクトリー 代数とします。 The Cartan subalgebras of $\mathfrak{g}$ (Chap. VII, §2, no. 1, Def. 1) are its maximal commutative subalgebras; in particular, $\mathfrak{g}$ is the union of its Cartan subalgebras. 群 Int($\mathfrak{g}$) は、$\mathfrak{g}$ のカルタン部分代数の集合で推移的に動作します。

$\mathfrak{g}$ は還元的であるため、そのカルタン部分代数は可換です (第 2 章、コリント 3 章、VII, §2, no. 4)。逆に、$\mathfrak{t}$を$\mathfrak{g}$の可換部分代数とします。 §1, no. 3、提案 1 により、広告 $x$ はすべての $x\in \mathfrak{t}$ に対して半単純になります。章著VII, §2, no. 3、提案 10、$\mathfrak{g}$ 含む $\mathfrak{t}$ のカルタン部分代数が存在します。これは、定理の最初の主張を証明します。

ここで、$\mathfrak{t}$ と $\mathfrak{t}'$ を $\mathfrak{g}$ の 2 つのカルタン部分代数とします。 $u(\mathfrak{t}) =\mathfrak{t}'$ となる $u\in$ Int($\mathfrak{g}$) が存在することを証明します。 §1, no. 3 の提案 1 により、$\mathfrak{g}$ は L(G) の形式であると仮定できます。ここで、G は接続されたコンパクトなリー群であり、$\mathfrak{g}$ 上の分離不変対称双線形形式 F を選択できます。 $x$ (それぞれ $x'$) を $\mathfrak{g}$ の正則元とし、$\mathfrak{t}=\mathfrak{g}^0(x)$ (それぞれ $\mathfrak{t}'=\mathfrak{g}^0(x')$) とします (第 2 章、VII, §3, no. 3)。 適用補題 1 K = G の場合、[(Ad $k$)$(x), x']$ は F に関して $\mathfrak{g}$ に直交し、したがって零となるような $k\in G$ が存在することがわかります。 (広告 $k$)$(x)\in \mathfrak{g}^0(x') =\mathfrak{t}'$ なので、(広告 $k$)$(x)$ が正規なので、$\mathfrak{g}^0$((広告 $k$)$(x)$) $=\mathfrak{t}'$ となります。 私たちは結論する、(広告$k$)$(\mathfrak{t}) =\mathfrak{t}'$、したがって定理です。

#### 系 {#lie-ix-s2-n1-cor-1 .statement tag=01A1}

$\mathfrak{t}$と$\mathfrak{t}'$を$\mathfrak{g},\mathfrak{a}$のカルタン部分代数、$\mathfrak{t}$の部分集合、$\mathfrak{g}$の$u$自己同型とし、$\mathfrak{a}$を$\mathfrak{t}'$に加えます。 $u\circ v$ が $\mathfrak{t}$ を$\mathfrak{t}'$ に取り、一致するが $\mathfrak{a}$ で $u$ になるような Int($\mathfrak{g}$) の元 $v$ が存在します。

G = Int($\mathfrak{g}$) と置き、G の $\mathfrak{a}$ の固定子 $Z_G(\mathfrak{a})$ を考えます。これは G の嘘部分群であり、そのリー代数 $\mathfrak{z}_{\mathfrak{g}}(\mathfrak{a})$ は $\mathfrak{a}$ のすべての元と交換する $\mathfrak{g}$ の元で構成されます (章 III, §9, no. 3、提案 7)。すると、$\mathfrak{t}$と$u^{-1}(\mathfrak{t}')$は、コンパクトリー代数$\mathfrak{z}_{\mathfrak{g}}(\mathfrak{a})$の2つのカルタン部分代数になります。 Thさんより1、$v(\mathfrak{t}) =u^{-1}(\mathfrak{t}')$となるような$Z_G(\mathfrak{a})$のうち元$v$が存在します。そのような元には、望ましい特性があります。

### 2. 最大トーラス

G をリー群とします。 G のトーラスは閉じた部分群、つまりトーラス (§1, no. 2) であり、他の語は任意の可換接続コンパクト部分群です。 G のトーラスの集合のうち極大元を包含順に並べたものを、G の最大トーラスと呼びます。

#### 定理 2 {#lie-ix-s2-thm-2 .statement tag=01A2}

G を接続されたコンパクト・リー群とします。

a) G の最大トーラスのリー代数は、L(G) のカルタン部分代数です。

b) $T_1$ と $T_2$ を G の 2 つの最大トーラスとする。 $T_2=gT_1g^{-1}$ となるような $g\in G$ が存在する。

c) G はその最大トーラスの和集合です。

Let $\mathfrak{t}$ be a Cartan subalgebra of L(G); the integral subgroup of G whose Lie algebra is $\mathfrak{t}$ is closed (Chap. VII, §2, no. 1, Cor. 4 of Prop. 4) and commutative (Th. 1), and hence is a torus of G. T が G の最大トーラスである場合、そのリー代数は可換であるため、L(G) のカルタン部分代数に含まれます (Th. 1)。 したがって、G の最大トーラスは、L(G) のカルタン部分代数に関連付けられた G の積分部分群であるため、a) となります。 主張 b) Th から続きます。 1、 標準準同型 $G\rightarrow$ Int(L(G)) は全射法であるため (III, §6, no. 4 章、提案 10 の Cor. 4)。

G の最大トーラスの X 和集合で表し、T を G の最大トーラスとします。 $G\times T$ から G までの連続写像 $(g, t) \rightarrow gtg^{-1}$ は像 X を持ち、したがって G で閉じられます。したがって、c) を証明するには、X が G で開いていることを証明すれば十分です。 X は内部自己同型の下で不変なので、すべての $a\in T, X$ が $a$ の近傍であることを示せば十分です。 G の次元について帰納法によって議論し、2 つのケースを区別します。

$1)a$ は G の中心ではありません。H を G の $a$ の中心化者の同一性成分とします。これは、G の連結コンパクト部分群であり、G は含む T、したがって $a$ とは異なります。 Ad $a$ は半単純 (§1, no. 1) であるため、H のリー代数は Ad $a-1$ のゼロスペースです。これは第 2 章から続きます。 VII, §4, no. 2、提案4、Hの共役の和集合Yは$a$の近傍である。 帰納法の仮定、$H\subset X$、そして$Y\subset X$までに。したがって、X は $a$ の近傍です。

$2)a$ は G の中心です。L(G) のすべての $x$ について、$a$ exp $x$ 属するから X であることを証明すれば十分です。これで、L(G) の元 $x$ 属するから G (Th. 1) のカルタン部分代数までです。 対応する積分部分群 $T'$ 含む経験値 $x$; T に対しては共役なので、含む $a$ となり、必要に応じて $a$ exp $x$ となります。

#### 系 1 {#lie-ix-s2-thm-2-cor-1 .statement tag=01A3}

a) G の指数写像は全射です。

b) すべての $n\geq 1$、写像 $g \rightarrow g^n$ について、G からそれ自体までは全射です。

確かに、exp(L(G)) 含む G のすべての最大トーラス、したがって a)。 主張 b) は、L(G) の $x$ に対して公式 (exp $x$)$^n=$ exp $nx$ から続きます。

#### 注意 1 {#lie-ix-s2-n2-rem-1 .statement tag=01A4}

exp$_G(K) = G$となるL(G)のコンパクト部分集合Kが存在します。実際、T が G の最大値トーラスである場合、exp$_T(C) = T$ のようなコンパクトな部分集合 $C\subset L(T)$ が存在します。 $K =\bigcup_{g\in G}$(広告$g$)$(C)$を取るだけで十分です。

#### 系 2 {#lie-ix-s2-thm-2-cor-2 .statement tag=01A5}

G の最大トーラスの共通部分は G の中心です。

$x$ を G の中心の元とします。 Th 著$2c)$、G 含む $x$ の最大トーラス T が存在します。次に $x$ 属するが T のすべての共役になり、したがって G のすべての最大トーラスになります。 逆に、G のすべての最大トーラスに対して $x$ 属するの場合、G のすべての元と Th によって可換になります。 $2c)$。

#### 系 3 {#lie-ix-s2-thm-2-cor-3 .statement tag=01A6}

$g\in G$ を中心者とし、C を中心者とします。次に、$g$ 属するから $C_0$; 群 $C_0$ は、G 含む $g$ の最大トーラスの和集合です。

G 含む $g$ (Th. $2c$)$)$ の最大トーラス T が存在し、したがって $C_0$ に含まれます。さらに、群 $C_0$ は接続されたコンパクト・リー群であるため、その最大トーラス (Th. $2c$)$)$ の和集合です。これらすべて含む $g$ (Cor. 2) は、まさに G 含む $g$ の最大のトーラスです。

#### 系 4 {#lie-ix-s2-thm-2-cor-4 .statement tag=01A7}

$g\in G$ にしましょう。 $g$ が正規 (章 VII, §4, no. 2、定義 2) の場合、属するから一意の最大値トーラスになり、これがセントラライザーの識別子成分になります。 それ以外の場合は、無限に多くの最大トーラスが属するになります。

Ad $g$ は半単純であるため、Ad $g-1$ の nilspace の次元は、$g$ のセントラライザー C の nilspace でもあります。ロケ地にて。引用、提案 8、および Th. $1,g$ は、$C_0$ が G の最大トーラスである場合に限り、正規です。結論は Cor から得られます。 3.

#### 系 5 {#lie-ix-s2-thm-2-cor-5 .statement tag=01A8}

a) S を G のトーラスとします。S のセントラライザーが接続されています。それは G 含む S の最大トーラスの和集合です。

b) $\mathfrak{s}$ を L(G) の可換部分代数とします。 Gの$\mathfrak{s}$のフィクサーが接続されています。それは、リー代数含む $\mathfrak{s}$ である G の最大トーラスの和集合です。

a)を証明するには、Gの元$g$がSを集中させる場合、G含むSと$g$の最大トーラスが存在することを証明すれば十分です。ここで、C が $g$ のセントラライザーである場合、$g\in C_0$ (Cor. 3) と $S\subset C_0$ が存在します。 T が接続されたコンパクト・リー群 $C_0$ 含む S の最大トーラスである場合、$g\in T$ (Cor. 2) が得られるため、a) になります。 主張 b) は、第 3 章の観点から、リー代数 $\mathfrak{s}$ による積分部分群の閉包に適用される a) から続きます。 III, §9, no. 3、提案9。

#### 注意 2 {#lie-ix-s2-n2-rem-2 .statement tag=01A9}

それはコルから続きます。 G の極大トーラスは可換極大部分群であることがわかります。 逆は真ではありません。たとえば、群 $\mathbf{S}\mathbf{O}(3,\mathbf{R})$ では、最大トーラスは次元 1 であるため、対角線行列のできない含む部分群は、$(\mathbf{Z}/2\mathbf{Z})^2$ と同型です。さらに、$g\in \mathbf{S}\mathbf{O}(3,\mathbf{R})$ が非スカラー 対角行列である場合、$g$ はセントラライザーが接続されていない $\mathbf{S}\mathbf{O}(3,\mathbf{R})$ の正則元です (cf. Cor. 4)。

#### 系 6 {#lie-ix-s2-thm-2-cor-6 .statement tag=01AA}

G の最大のトーリは、独自の中心化者であり、リー代数の固定者です。

T を G の最大のトーラスとそのセントラライザー C とします。 L(T) は L(G) のカルタン部分代数であるため、L(T) = L(C) となり、C が接続されているため、C = T となります (Cor. 5)。

#### 系 7 {#lie-ix-s2-thm-2-cor-7 .statement tag=01AB}

T と $T'$ を G の 2 つの最大トーラスとし、T の A 部分集合と A を $T'$ に取り込む G の $s$ 自己同型とします。 $s\circ$ (Int $g$) が T を $T'$ に取り、A の $s$ で一致するとなるような $g\in G$ が存在します。

C を A のセントラライザーとします。すると、T と $s^{-1}(T')$ は $C_0$ の 2 つの最大トーラスになります。 (Int $g$)$(T) =s^{-1}(T')$ が目的のプロパティを持つように、$C_0$ のすべての元 $g$ が一致します。

#### 系 8 {#lie-ix-s2-thm-2-cor-8 .statement tag=01AC}

Hをコンパクト・リー群、TをHの最大値トーラスとします。次に、$H = N_H(T).H_0$と$N_H(T)$の単射を$N_H(T)/N_{H_0}(T)$から$H/H_0$までのH誘導する同型にします。

$h\in H$ にしましょう。この場合、$h^{-1}Th$ は $H_0$ の最大トーラスであるため、(Th. 2) $hg\in N_H(T)$ となるような $g\in H_0$ が存在します。したがって、$h$ 属するから $N_H(T).H_0$ となり、最初の主張になります。 2 つ目はすぐに続きます。

#### 注意 3 {#lie-ix-s2-n2-rem-3 .statement tag=01AD}

G を接続されたリー群とし、そのリー代数はコンパクトです。 G のカルタン部分群は積分部分群であり、そのリー代数は L(G) のカルタン部分代数です (したがって、接続されたコンパクト群のカルタン部分群はその最大トーラスです)。 定理 2 とその帰結は、「最大トーラス」という表現をすべて「カルタン部分群」に置き換えた場合でも、G に対して引き続き有効です。 これは、§1, no. 4 の提案 5 を考慮すると、G はベクトル群 V の直接積であり、接続されたコンパクト群 K であり、G のカルタン部分群は、最大トーラスを持つ V の積であるという事実からすぐに得られます。 K. さらに、それはコルから続くことに注意してください。 6 上記の G のカルタン部分群は、L(G) のカルタン部分代数のフィクサーとしても定義できます。

$^*4)$ 部分定理 2 の c) は次のように証明することもできます。 G に不変リーマン計量を与えます (§1, no. 3、提案 3)。次に、G の任意の元 $g$ について、G の $g$ および単位元までの最大測地線移行が存在し (ホップリノウ定理)、そのような測地線の閉包が $G$ のサブトーラスであることを検証できます。\*

### 3. 部分群と剰余群の最大トーラス

#### 命題 1 {#lie-ix-s2-prop-1 .statement tag=01AE}

G と $G'$ を 2 つ接続したコンパクト・リー群とします。

a) $f: G\rightarrow G'$ をリー群の全射法射とします。 $G'$ の最大トーラスは、G の最大トーラスの $f$ の下にある像です。 $f$ の核が G の中心にある場合 (たとえば離散)、G の最大トーラスは、$G'$ の最大トーラスの $f$ の下にある逆像です。

b) H を G の接続された閉じた部分群とします。H のすべての最大値トーラスは共通部分であり、H は G の最大値トーラスです。

c) H を G の接続された閉じた法線部分群とします。H の最大トーラスは、G の最大トーラスの H と共通部分です。

a) T を G の最大値トーラスとする。この場合、L(T) は L(G) (no. 2、Th. $2a$)$)$ のカルタン部分代数であるため、$L(f(T))$ は $L(G')$ のカルタン部分代数になります (Prop. VII, §2, no. 1、Cor. 2 の 2 章)。 4);したがって、$f(T)$ は、$G'$ (no. 2、Th. $2a$)$)$ の最大トーラスであることがわかります。 If Ker $f$ is central in G, it is contained in T (Cor. 2 of Th. 2), so $T =f^{-1}(f(T))$.

逆に、$T'$ を $G'$ の最大値トーラスとします。 $f(T) = T'$ となる G の最大トーラス T が存在することを示します。 $T_1$ を G の最大値トーラスとします。その場合、$f(T_1)$は$G'$の最大トーラスであり、$T'=g'f(T_1)g^{'-1}$(Th.$2b$)$)$となるような$g'\in G'$が存在します。 $g\in G$ が $f(g) =g'$ である場合、$T =gT_1g^{-1}$ を含む $T'=f(T)$ が得られます。

b) S を H の最大値トーラスとする。これは G のトーラスなので、G 含む S の最大トーラス T が存在します。そのとき、$T\cap H$ は H 含む S の可換部分群であるため、S (no. 2, 注意 2) に等しくなります。

c) §1, no. 3 により、提案 $2c), L(G)$ は理想を伴う L(H) の直接の積です。したがって、L(H)のカルタン部分代数はL(G)のカルタン部分代数のL(H)と共通部分です。したがって、$G, T\cap H$ 含むの最大トーラス T に対して、H および $S = T\cap H$ (no. 2, 注意 2) の最大トーラス S です。

#### 注意 1 {#lie-ix-s2-n3-rem-1 .statement tag=01AF}

命題 1 は、コンパクトリー 代数と接続された群に直ちに一般化します。特に、G がリー代数がコンパクトな連結リー群である場合、G のカルタン部分群 (cf. 注意 3, no. 2) は、連結コンパクト・リー群 Ad(G) の最大トーラスの正確に逆像 (G から標準準同型の下)広告(G))。

#### 注意 2 {#lie-ix-s2-n3-rem-2 .statement tag=01AG}

G を、群 D(G) と $f: \widetilde{D}(G)\rightarrow G$ の普遍的なカバーであるコンパクト・リー群、$\widetilde{D}(G)$ と、$\widetilde{D}(G)$ から D(G) および D(G) から G への標準射の合成であるとします。すると、写像 $T\rightarrow f^{-1}(T)$ は、から全単射になります。 G の最大トーラスの集合から $\widetilde{D}(G)$ の最大トーラスの集合。 逆全単射は、$\widetilde{D}(G)$ の最大トーラス $\widetilde{T}$ と G の最大トーラス $C(G)_0.f( \widetilde{T})$ を関連付けます。

### 4. 最大階数のうち部分群

接続されたリー群 G の階数をそのリー代数の階数と呼び、それを rk G で表すことにします。 2 a)、接続されたコンパクト・リー群の階数は、その最大トーラスの共通の次元です。

G を G の接続されたコンパクト・リー群 、H を閉じた部分群とします。H が接続されている場合、rk $H\leq$ rk G になります (H の最大のトーラスは G のトーラスであるため)。 Thさんより2 c)、H が接続されており、最大階数 (つまり、階数 rk G) であるということは、H が G の最大トーラスの和集合であることを意味します。 命題 1 からすぐに推論します。

#### 命題 2 {#lie-ix-s2-prop-2 .statement tag=01AH}

$f$ : G $\rightarrow G'$ を、核が中心となる接続されたコンパクト・リー群の全射射とします。 写像 $H \rightarrow f(H)$ と $H' \rightarrow f^{-1}(H')$ は、最大階数の G の接続された閉じた部分群の集合と、$G'$ の類似の集合の間の逆全単射です。

#### 命題 3 {#lie-ix-s2-prop-3 .statement tag=01AI}

G を接続されたコンパクト・リー群とし、H を最大階数の接続された閉じた部分群とします。

a) コンパクトな多様体 $G/H$ は簡易接続されています。

b) 準同型 $\pi_1(H)\rightarrow \pi_1(G)$ は、H から G への標準単射によって誘導され、全射的です。

H が接続されているので、完全系列 (一般位相、章 XI、準備中)

$$
\pi_1(H)\rightarrow \pi_1(G)\rightarrow \pi_1(G/H,\overline{e})\rightarrow 0
$$

ここで、$\overline{e}$ は G の単位元の $G/H$ の像です。 $G/H$ が接続されているため、これは直ちに主張 a) と b) の同値を意味します。さらに、$f: G'\rightarrow G$ が核を中心とする連結コンパクト・リー群の全射射である場合、G の証明命題 (形 $a$)$)$ は、G の証明と同じです。 $G'$ (提案 2)。したがって、まず Ad(G) によって置き換える G を求め、次に G が半単純であると仮定し、次にユニバーサルカバー (§1, no. 4、Cor. 2) による置き換えること G によって、G が単純接続されていると仮定することができます。しかし、主張 b) は些細なことです。

#### 命題 4 {#lie-ix-s2-prop-4 .statement tag=01AJ}

G をコンパクト・リー群、H を極大値階数の G の閉じた部分群に接続し、G における H の正規化子を N とします。そのとき、H は N における有限添字であり、N の単位成分です。

確かに、H のリー代数 L(G) の含むカルタン部分代数です。したがって、Chap. VII, §2, no. 1、コル。提案 4 の 4、H は N の単位成分です。N はコンパクトなので、H は N において有限添字です。

#### 注意 1 {#lie-ix-s2-n4-rem-1 .statement tag=01AK}

rk H = rk G となる G のすべての積分部分群 H は閉じています。実際、前の証明は、H が正規化器の恒等式成分であり、G の閉じた部分群であることを示しています。

#### 注意 2 {#lie-ix-s2-n4-rem-2 .statement tag=01AL}

提案 4 の記法では、G 含む H のすべての閉じた部分群 $H'$ と、$(H': H)$ が有限であるようなものは H を正規化し、したがって N に含まれます。同様に、$H'$ のノーマライザーは N に含まれています。特に、N は独自のノーマライザーです。

### 5. ワイル群

G を接続されたコンパクト・リー群 、T を G の最大値トーラスとします。G における T の正規化子を $N_G(T)$ で示します。提案 4 (no. 4) より、剰余群 $N_G(T)/T$ は有限です。これを $W_G$(T) または W(T) で表し、G の最大トーラス T のワイル群、または T に対する G のワイル群と呼びます。 T は可換なので、G の内部自己同型による T 上の $N_G(T)$ の演算です。 誘導するは、リー群の群 $W_G(T)$ の正典演算と呼ばれる商演算への通過によって。 Thの6。 no. 2 の 2、この演算は忠実です。関連する準同型 $W_G(T)\rightarrow$ Aut T は単射です。

$T'$ が G の他の最大値トーラスで、$g\in G$ が Int $g$ 写像 T から $T'$ (no. 2, Th. $2b$)$)$ である場合、Int $g$ 誘導する同型 $a_g$ $W_G(T)$ から $W_G(T')$ と $a_g(s)(gtg^{-1}) =gs(t)g^{-1}$ はすべての $s\in W_G(T)$ とすべての $t\in T$ です。

#### 命題 5 {#lie-ix-s2-prop-5 .statement tag=01J9}

$a)$ G のすべての共役類は T と一致します。

b) G の共役類の T を持つ共通部分は、ワイル群の軌道です。

$g\in G$ にしましょう。 Th 著no. 2 の 2 には、$g\in hTh^{-1}$ となるような $h\in G$ が存在するため、a) となります。ワイル群の定義により、T上の$W_G(T)$の同じ軌道にある任意の2つの元は、Gでは共役になります。逆に、$a, b$ を G の下の T 共役の 2 つの元とします。$b=hah^{-1}$ となるような $h\in G$ が存在します。 適用コル。 Thの7。 2 (no. 2) を $A =\{a\},s=$ Int $h, T'= T$ とすると、Int $hg$ 写像 T から T および $a$ から $b$ となるような $g\in G$ が存在することがわかります。 $W_G(T)$の$hg$の類、次に写像$a$から$b$、したがって命題です。

#### 系 1 {#lie-ix-s2-prop-5-cor-1 .statement tag=01JA}

T の G への標準注入は、商への通過によって、G の共役クラスの $T/W_G(T)$ から空間 $G/$Int(G) への同型写像を定義します。

実際、これは 2 つのコンパクトな空間 (cf. 一般位相、Chap. III、p. 29、Cor. 1) の間の全単射連続写像です。

#### 系 2 {#lie-ix-s2-prop-5-cor-2 .statement tag=01JB}

E を内部自己同型の下で安定な G の部分集合とする。このとき、T で $E\cap T$ が開いている (それぞれ閉じ、それぞれ密) 場合に限り、E は G で開いています (それぞれ閉じ、それぞれ密)。

これはコルからの続きです。 1 と、正規の写像 $\mathrm{T}\to \mathrm{T}/\mathrm{W}_{G}(\mathrm{T})$ および $\mathrm{G}\to \mathrm{G}/\mathrm{Int}(\mathrm{G})$ がオープンであるという事実 (*一般位相*、章 III、p. 10、補題 2)。

$\mathrm{G}$のリー代数を$\mathfrak{g}$で表し、$\mathrm{T}$のそれを$\mathfrak{t}$で表します。 $\mathbf{R}$ ベクトル空間 $\mathfrak{t}$ 上の群 $\mathrm{W}_{G}(\mathrm{T})$ の *正準表現* と呼ばれる、$\mathrm{T}$ 誘導する表現上の $\mathrm{W}_{G}(\mathrm{T})$ の演算。

#### 命題 6 {#lie-ix-s2-prop-6 .statement tag=01JC}

a) *$\mathfrak{g}$ (随伴表現) 上の $\mathrm{G}$ のすべての軌道は $\mathfrak{t}$ と一致します。*

b) *共通部分と $\mathrm{G}$ の軌道の $\mathfrak{t}$ は、$\mathfrak{t}$ の $\mathrm{W}_{G}(\mathrm{T})$ の軌道です。*

主張 a) Th から続きます。 1 (no. 1)。 $x,y$ を $\mathrm{Ad}(\mathrm{G})$ の下の $\mathfrak{t}$ 共役の 2 つの元とし、$h\in\mathrm{G}$ を $(\mathrm{Ad}\,h)(x)=y$ となるようにします。 Thの適用系 1 (no. 1) と $\mathfrak{a}=\{x\}$、$u=\mathrm{Ad}\,h$、$\mathfrak{t}'=\mathfrak{t}$ では、$\mathrm{Ad}\,hg$ 写像 $\mathfrak{t}$ ～ $\mathfrak{t}$ および $x$ ～ $y$ のような $g\in\mathrm{G}$ が存在することがわかります。次に、$hg\in\mathrm{N}_{G}(\mathrm{T})$ (章 III, §9, no. 4、提案 11)、および $\mathrm{W}_{G}(\mathrm{T})$ 写像 $x$ から $y$ の $hg$ の類、したがって命題です。

#### 系 {#lie-ix-s2-n5-cor-1 .statement tag=01JD}

*$\mathfrak{t}$の標準単射は$\mathfrak{t}/\mathrm{W}_{G}(\mathrm{T})$から$\mathfrak{g}/\mathrm{Ad}(\mathrm{G})$まで商準同型への通過により$\mathfrak{g}$定義するに。

これを写像を $j$ で表します。それは全単射的かつ連続的です (提案 6)。可換図式があります

$$
\begin{array}{ccc}
\mathfrak{t} & \xrightarrow{\ i\ } & \mathfrak{g} \\
{\scriptstyle p}\downarrow\phantom{{\scriptstyle p}} & & \phantom{{\scriptstyle q}}\downarrow{\scriptstyle q} \\
\mathfrak{t}/\mathrm{W}_{G}(\mathrm{T}) & \xrightarrow{\ j\ } & \mathfrak{g}/\mathrm{Ad}(\mathrm{G})
\end{array}
$$

ここで、$p$ と $q$ は商写像、$i$ は標準単射です。 $i$ と $q$ は適切であるため (*一般位相*、章 I, §10, no. 1、提案 2 および *一般位相*、章 III, §4, no. 1、提案 2 c))、$p$ は全射なので、次のようになります。 $j$ は適切であり (*一般位相*、章 I, §10, no. 1、提案 5)、従って同型写像です。

#### 命題 7 {#lie-ix-s2-prop-7 .statement tag=01JE}

*$H$ を $\mathrm{G}$ 含む $\mathrm{T}$ の閉じた部分群とします。*

a) *$\mathrm{W}_{H}(\mathrm{T})$ 部分群 $\mathrm{N}_{H}(\mathrm{T})/\mathrm{T}$ または $\mathrm{W}_{G}(\mathrm{T})$ で表します。 群 $H/H_{0}$ は剰余群 $\mathrm{W}_{H}(\mathrm{T})/\mathrm{W}_{H_{0}}(\mathrm{T})$ と同型です。*

b) *$H$ は、$H$ 属するから $\mathrm{W}_{H_{0}}(\mathrm{T})$ に代表者がいる $\mathrm{W}_{G}(\mathrm{T})$ のすべての元にのみ接続されます。*

主張 a) はコルから続きます。 Thの8。 2 (no. 2)、および主張 b) は a) の特殊なケースです。

### 6. 準同型の最大トーリとカバーリング

G を接続されたコンパクト・リー群、T を G の最大値トーラスとします。G の導来群 D(G) とその普遍的なカバー $\widetilde{D}(G)$ を考えます。 $p: \widetilde{D}(G)\rightarrow G$ を正規の射 $\widetilde{D}(G)\rightarrow D(G)$ と $D(G)\rightarrow G$ の合成とします。このとき、$\widetilde{D}(G)$ は接続されたコンパクト・リー群 (§1, no. 4、提案 4 の Cor. 2) です。さらに、$p$ の下での T の逆像 $\widetilde{T}$ は、$\widetilde{D}(G)$ の最大トーラス (no. 3、提案 1)。

#### 補題 2 {#lie-ix-s2-lem-2 .statement tag=01AO}

H をリー群のリー群、$f_T: T\rightarrow H$、$\widetilde{f}: \widetilde{D}(G)\rightarrow H$ 射とし、すべての $t\in \widetilde{T}$ に対して $f_T(p(t)) = \widetilde{f}(t)$ とします。 リー群 $f: G\rightarrow H$ の $f\circ p= \widetilde{f}$ と、T に対する $f$ の制限が $f_T$ となるような一意な準同型が存在します。

$Z = C(G)_0$を入れてください。 §1, no. 4、Cor.提案 4 の 1、リー群 $g: Z\times \widetilde{D}(G)\rightarrow G$ の射で、$g(z, x) =z^{-1}p(x)$ がカバーになります。その核は対 $(z, x)$ で構成され、$p(x) =z$ に対して $x\in p^{-1}(Z)\subset \widetilde{T}$ が含まれます。 $Z\times \widetilde{D}(G)$ から H 写像 Ker $g$ から $\{e\}$ までの射 $(z, x) \rightarrow f_T(z^{-1}) \widetilde{f}(x)$ なので、$z\in Z$ に対して $f\circ p= \widetilde{f}$ と $f(z) =f_T(z)$ となるような G から H までの射 $f$ が存在します。 しかし、$t\in p( \widetilde{T})$ には $f(t) =f_T(t)$ もあります。 $T = Z.p( \widetilde{T})$, $f$ の制限から T は確かに $f_T$ です。

#### 命題 8 {#lie-ix-s2-prop-8 .statement tag=01AP}

G を接続されたコンパクト・リー群、T を G の最大トーラス、H リー群およびリー代数の $\varphi : L(G)\rightarrow L(H)$ 準同型とします。 リー群 $f: G\rightarrow H$ のうち $L(f) =\varphi$ となる射が存在するのは、$L(f_T) =\varphi |L(T)$ となるリー群 $f_T: T\rightarrow H$ のうち射が存在する場合に限ります。次に$f_T=f|T$。

$f: G\rightarrow H$ が $L(f) =\varphi$ のようなリー群の射である場合、$f$ の T に対する制限 $f_T$ は、$L(f_T) =\varphi |L(T)$ のような T から H への一意の射です。 逆に、$f_T: T\rightarrow H$ を $L(f_T) =\varphi |L(T)$ となるようなリー群の射とします。 $\widetilde{D}(G)$ と $p$ を上記の通りとします。 $L( \widetilde{D}(G))$ から L(G) の派生代数 $\mathfrak{b}$ までの写像 $L(p)$ 誘導する同型。 $L( \widetilde{f}) = (\varphi |\mathfrak{b})\circ L(p)$ となるようなリー群 $\widetilde{f}: \widetilde{D}(G)\rightarrow H$ の射が存在します (第 1 章、III, §6, no. 1)。 $\widetilde{T}$ から H 誘導するまでの射 $t \rightarrow \widetilde{f}(t)$ と $t \rightarrow f_T(p(t))$ は、リー代数の準同型と同じなので、一致するになります。 適用補題 2 から、L(T) と $\mathfrak{b}$ に $L(f)$ と $\varphi$ 一致するが存在するように、射 $f: G\rightarrow H$ の存在を推定します。 $L(G) =\mathfrak{b}+ L(T)$ なので、$L(f) =\varphi$ になります。

#### 命題 9 {#lie-ix-s2-prop-9 .statement tag=01AQ}

G を連結したコンパクト・リー群、T を G、H リー群、$f: G\rightarrow H$ 射の最大値トーラスとします。次に、$f$ は、T への制限が単射である場合にのみ単射です。

確かに、Th による。 2 (no. 2) T 簡約するから単位元を持つ共通部分の場合に限り、G 簡約するから単位元の通常の部分群 Ker $f$。

### 練習問題 {#lie-ix-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
