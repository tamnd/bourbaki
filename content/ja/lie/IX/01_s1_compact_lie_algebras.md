---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 1
section_title: Compact Lie algebras
lang: ja
source: lie-vii-ix
book_pages: 281-287, 389-391
pdf_pages: 0288-0294, 0396-0398
extraction: native
subsections:
    - "no": 1
      title: INVARIANT HERMITIAN FORMS
      page: 281
      pdf_page: 288
    - "no": 2
      title: CONNECTED COMMUTATIVE REAL LIE GROUPS
      page: 282
      pdf_page: 289
    - "no": 3
      title: COMPACT LIE ALGEBRAS
      page: 283
      pdf_page: 290
    - "no": 4
      title: GROUPS WHOSE LIE ALGEBRA IS COMPACT
      page: 284
      pdf_page: 291
statements: 13
exercises: 9
content_sha256: d548700e586eb144923458b87c38067c075323fc3cd21ab76707fbb0f7420780
translated_from: content/en/lie/IX/01_s1_compact_lie_algebras.md
translation_method: google
source_content_sha256: 71ef208b41db85bf8bc8c5557777019fadb960c88536da1750a4c9288864f27c
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: d08aceb2d1d20ff816b242ac714f82f6d391b256bd484ac834762e8970734735
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 1。 コンパクトリー 代数

### 1. 不変エルミート形

この数において、文字$k$は体$\mathbf{R}$または$\mathbf{C}$を表します。 V を有限次元 $k$ ベクトル空間、 $\Phi$ を V、G 群、$\mathfrak{g}$ $\mathbf{R}$ リー代数上の分離$^2$ 正のエルミート形とします。 $\rho : G\rightarrow \mathbf{G}\mathbf{L}(V)$ 群準同型、$\varphi :\mathfrak{g}\rightarrow \mathfrak{g}\mathfrak{l}(V)$ 準同型/$\mathbf{R}$-リー代数。

a) 形 $\Phi$ は、$\rho (g)$ がすべての $g\in G$ について$\Phi$ に関してユニタリである場合に限り、G (それぞれ$\mathfrak{g}$) のもとで不変です (それぞれ$\varphi (x)$ はすべての$\Phi$ に関して反エルミート$^3$) $x\in \mathfrak{g}$）。確かに、$\Phi$ に対する V の自己準同型 $a$ の随伴物を $a^*$ で表します。 $g$ の $G,x$ の $\mathfrak{g},u$ と $v$ の V については、

$$
\Phi (\rho (g)u, \rho (g)v) =\Phi (\rho (g)^*\rho (g)u, v)
$$

$$
\Phi (\varphi (x)u, v) +\Phi (u, \varphi (x)v) =\Phi ((\varphi (x) +\varphi (x)^*).u, v)
$$

$^1$ この章全体で、代数、第 1 章を参照します。 VIII、新刊へ

(準備中)

$^2$ V でエルミート形 H が述べられていることを思い出してください (代数、IX 章、準備中)。

V の非ゼロのすべての元 $u$ について、

$H(u, v)\not= 0$ となるような $v\in V$ が存在します。

$^3$ 元 $a\in$ End(V) は、$\Phi$ に関して反エルミートであると言われます。

$\Phi$ に対する$a$ の随伴$a^*$ は、$-a$ に等しい。 $k=\mathbf{C}$ (それぞれ $k=\mathbf{R}$) のとき

また、V (それぞれ $\mathbf{C}\otimes_{\mathbf{R}}V$) の自己準同型 $ia$ がエルミートであることも意味します。したがって、$\rho (g)^*\rho (g) =$ Id$_V$ の場合に限り、V のすべての $u, v$ に対して $\Phi (\rho (g)u, \rho (g)v) =\Phi (u, v)$ となります。同様に、$\varphi (x) +\varphi (x)^*= 0$ の場合に限り、V のすべての $u, v$ に対して $\Phi (\varphi (x)u, v) +\Phi (u, \varphi (x)v) = 0$ となるため、主張となります。

b) If the form $\Phi$ is invariant under G (resp. $\mathfrak{g}$), the orthogonal complement of a stable subspace of V is stable; in particular, the representation $\rho$ (resp. $\varphi$ ) is then semi-simple (cf. Algebra, Chap. IX); moreover, for all $g\in G$ (resp. $x\in \mathfrak{g}$), the endomorphism $\rho (g)$ (resp. $\varphi (x)$) of V is then semi-simple, with eigenvalues of absolute value 1 (resp. with purely imaginary eigenvalues); indeed $\rho (g)$ is unitary (resp. $i\varphi (x)$ is hermitian, cf. Algebra, Chap. IX).

c) $k=\mathbf{R}$ と仮定します。 G が連結リー群、$\rho$ がリー群の射、$\mathfrak{g}$ G のリー代数、および $\varphi$ が $\rho$ によって誘起される準同型である場合、$\Phi$ は、$\mathfrak{g}$ の下で不変である場合に限り、G の下で不変です (第 III, §6, no. 5、Cor. 3)。

d) There exists a separating positive hermitian form on V invariant under G if and only if the subgroup $\rho (G)$ of $\mathbf{G}\mathbf{L}(V)$ is relatively compact (Integration, Chap. VII, §3, no. 1, Prop. 1).

### 2. 接続可換実リー群

G を連結可換 (実数) リー群とします。指数関数写像

経験値$_G: L(G)\rightarrow G$

はリー群の射であり、離散核を伴う全射法 (第 III, §6, no. 4 、提案 11) であるため、L(G) は G の接続されたカバーであるという事実になります。

a) 次の条件は同等です: G は単純結合、exp$_G$ は同型、G は $\mathbf{R}^n(n=$ dim G と同型です)。 この場合、L(G) のベクトル空間構造を同型 exp$_G$ によって G に移すと、G 上のベクトル空間構造が得られます。これは、G の位相群構造と互換性のある唯一のものです。 単結合可換リー群はベクトル (嘘) 群と呼ばれます。 〜でない限り別途記載されているように、それらには常に上で定義された $\mathbf{R}$ ベクトル空間構造が与えられます。

b) exp$_G$ の$\Gamma (G)$ 核で表します。 位相章、将軍よりVII, §1, no. 1、木曜日。 1、群 G は、$\Gamma (G)$ が L(G) の格子であり、他の語 (前述) で、自由な $\mathbf{Z}$ モジュール $\Gamma (G)$ の階数が G の次元に等しい場合にのみコンパクトです。 L は有限次元 $\mathbf{R}$ ベクトル空間、$\Gamma$ は L の格子、商トポロジカル群 $L/\Gamma$ はコンパクトに接続された可換リー群です。

コンパクトに接続された可換リー群は、実トーラス、または (この章では) トーラスと呼ばれます。

c) 一般的な場合、E を $\Gamma$ (G) によって生成された L(G) のベクトル部分空間とし、V を相補的な部分空間とします。この場合、G はその嘘部分群 exp(E) と exp(V) の直接積です。 1 つ目はトーラス、2 つ目はベクトルです。最後に、G のすべての圧縮部分群は exp(E) に含まれます (exp(V) 上のその射影は必然的に単位元に縮小されるため)。したがって、部分群 exp(E) は G の一意の最大コンパクト部分群です。

たとえば、$G = C^*$ を考えてみましょう。 同一視する L(G) と $\mathbf{C}$ により、G の指数写像は $x \rightarrow e^x$ になります。次に、$\Gamma (G) = 2\pi i\mathbf{Z},E =i\mathbf{R}$、つまり exp(E) $=\mathbf{U}$; $V =\mathbf{R}$ を取得すると、exp(V) $=\mathbf{R}^*_+$ が得られ、一般位相章で構築された同型 $\mathbf{C}^*\rightarrow \mathbf{U}\times \mathbf{R}^*_+$ が回復します。 VIII, §1, no. 3、提案 1。

d) 注意最後に、exp$_G: L(G)\rightarrow G$ は G の普遍的なカバーであるため、$\Gamma (G)$ は G の基本的な群と自然に識別できます。

### 3. コンパクトリー 代数

#### 命題 1 {#lie-ix-s1-prop-1 .statement tag=019D}

$\mathfrak{g}$ を (実数) リー代数とします。次の条件は同等です。

(i) $\mathfrak{g}$ はコンパクト・リー群のリー代数と同型です。

(ii) The group Int($\mathfrak{g}$) (Chap. III, §6, no. 2, Def. 2) is compact.

(iii) $\mathfrak{g}$ has an invariant bilinear form (Chap. I, §3, no. 6) that is symmetric, positive and separating.

(iv) $\mathfrak{g}$ is reductive (Chap. I, §6, no. 4, Def. 4); for all $x\in \mathfrak{g}$, the endomorphism ad $x$ is semi-simple, with purely imaginary eigenvalues.

(v) $\mathfrak{g}$ は還元的であり、その Killing 形 B は負です。

(i) $=\Rightarrow$ (ii): if $\mathfrak{g}$ is the Lie algebra of a compact Lie group G, the group Int($\mathfrak{g}$) is separating and isomorphic to a quotient of the compact group $G_0$ (Chap. III, §6, no. 4, Cor. 4), hence is compact.

(ii) $=\Rightarrow$ (iii): 群 Int($\mathfrak{g}$) がコンパクトな場合、$\mathfrak{g}$ 上に対称な双線形形式が存在します。これは正であり、Int($\mathfrak{g}$) (no. 1) の下で不変であり、したがって、次の随伴表現でも不変です。 $\mathfrak{g}$。

(iii) $=\Rightarrow$ (iv): (iii) が満たされる場合、$\mathfrak{g}$ の随伴表現は半単純 (no. 1) であるため、$\mathfrak{g}$ は還元的です。さらに、自己準同型と $x$、$x\in \mathfrak{g}$ は、示されているプロパティ (no. 1) を持ちます。

(iv) $=\Rightarrow$ (v): すべての $x\in \mathfrak{g}, B(x, x) =$ Tr((ad $x$)$^2$);従って、$B(x, x)$ は、広告 $x$ の平方の固有値の和であり、従って、これらが純粋に架空の場合は負になります。

(v) $=\Rightarrow$ (i): $\mathfrak{g}$ が還元的であると仮定します。従って、可換部分代数 $\mathfrak{c}$ および半単純部分代数 $\mathfrak{s}$ の積 (第 I, §6, no. 4、提案 5)。 $\mathfrak{s}$ の殺害形は、形 B から $\mathfrak{s}$ の制限であるため、B が負の場合は負であり、分離します。 $\mathbf{G}\mathbf{L}(\mathfrak{s})$ の部分群 Int($\mathfrak{s}$) は閉じられており (これは、Aut($\mathfrak{s}$)、Chap. III, §10, no. 2、Cor. 2 の恒等式成分です)、分離する正の形 $-B$ を不変のままにします。従って、これはコンパクトであり、$\mathfrak{s}$ はコンパクト・リー群 Int($\mathfrak{s}$) のリー代数と同型です。さらに、$\mathfrak{c}$ は可換であるため、トーラス T のリー代数と同型です。従って、$\mathfrak{g}$ はコンパクト・リー群 Int($\mathfrak{s}$)$\times T$ のリー代数と同型です。

#### 定義 1 {#lie-ix-s1-def-1 .statement tag=019E}

コンパクトリー 代数$^4$ は、命題 1 の (i) ～ (v) の性質を持つリー代数です。

従って、コンパクトリー 代数は、可換代数の積と、コンパクトな半単純代数です。他の語では、リー代数は、それが還元的であり、その派生であるリー代数がコンパクトである場合にのみコンパクトです。

コンパクト・リー群のリー代数はコンパクトです。

#### 命題 2 {#lie-ix-s1-prop-2 .statement tag=019F}

a) リー代数の有限数の積は、それぞれの因子がコンパクトである場合に限り、 コンパクトリー 代数になります。

b) コンパクトリー 代数の部分代数はコンパクトです。

c) $\mathfrak{h}$ をコンパクトリー 代数 $\mathfrak{g}$ の理想とする。この場合、代数 $\mathfrak{g}/\mathfrak{h}$ はコンパクトであり、拡大 $\mathfrak{h}\rightarrow \mathfrak{g}\rightarrow \mathfrak{g}/\mathfrak{h}$ は自明です。

主張 a) と b) は、提案 1 の特徴付け (iii) から導かれます。 部分 c) は、a) と、還元的リー代数では、すべての理想は直因子であるという事実から導かれます (I, §6, no. 4 章、提案 5 の修正)。

#### 命題 3 {#lie-ix-s1-prop-3 .statement tag=019G}

G をリー群とし、接続された成分の群を有限とします。次の条件は同等です。

(i) リー代数 L(G) はコンパクトです。

(ii) 群 Ad(G) はコンパクトです。

(iii) G の随伴項表現の下に、L(G) 不変量上に分離正対称双線形形式が存在します。

\*(iv) G は、左と右の平行移動の下でリーマン計量不変量を持ちます。\*

(i) $=\Rightarrow$ (ii): L(G) がコンパクトな場合、群 Ad(G$_0$) $=$ Int(L(G)) はコンパクトです。 Ad(G) には有限の添字があるので、この後者の群もコンパクトです。

(ii) $=\Rightarrow$ (iii): これは no. 1 から続きます。

(iii) $=\Rightarrow$ (i): Int(L(G)) $\subset$ Ad(G) なので、これは提案 1 の特徴付け (iii) に従います。

\*(iii) $\Leftarrow \Rightarrow$ (iv): これは第 2 章の続きです。 III, §3, no. 13.\*

### 4. リー代数がコンパクトな群

#### 定理 1 {#lie-ix-s1-thm-1 .statement tag=019H}

(H. Weyl) G を接続されたリー群とし、そのリー代数はコンパクト半単純であるとします。この場合、G はコンパクトであり、その中心は有限です。

G は半単純なので、その中心 D は離散的です。さらに、剰余群 $G/D$ は Ad(G) と同型であるため (Chap. III, §6, no. 4、Cor. 4)、コンパクトです (提案 3)。最後に、群 $G/D$ は、その導来群と等しくなります (III, §9, no. 2 章、提案 4 の修正)。 定理は、「統合」第 1 章から続きます。 VII, §3, no. 2、提案 5。

#### 命題 4 {#lie-ix-s1-prop-4 .statement tag=019I}

G を接続されたリー群とし、そのリー代数はコンパクトです。 トーラス T、簡易接続コンパクト半単純リー が存在します。

$^4$ 実際のトポロジベクトル空間できないはコンパクトなトポロジ空間であることに注意してください。

〜でない限りは 0 に減らされます。 群 S、ベクトル群 V、および有限核を伴う全射射 $f: V\times T\times S\rightarrow G$。 G がコンパクトであれば、群 V は単位元に減ります。

C (それぞれ S) を単結合のリー群とし、そのリー代数は L(G) の中心 (それぞれ派生した代数) と同型です。このとき、C はベクトル群であり、S は有限中心 (Th. 1) を持つコンパクトな群であり、G は中心となる離散部分群 D によって $C\times S$ の商と識別できます (積分、第 3 章、積分)。 VII, §3, no. 2、補題 4)。 S 上の D の射影の像は中心であり、したがって有限であるため、$D\cap C$ は D の有限添字のものです。 $C'$ を $D\cap C$ と V によって生成された C のベクトル部分空間とします。補完的な部分空間。このとき、群 $T = C'/(D\cap C)$ はトーラスで、G は有限群による積群 $V\times T\times S$ の商と同型です。

G がコンパクトであれば、$V\times T\times S ($一般位相、第 4 章もコンパクトです。 III, §4, no. 1、コル。提案 2 の 2)、従って V も同様であり、これは $V =\{e\}$ を意味します。

#### 系 1 {#lie-ix-s1-prop-4-cor-1 .statement tag=019J}

G を接続されたコンパクト・リー群とします。このとき、$C(G)_0$ はトーラスで、D(G) は接続されたコンパクト半単純リー 群であり、$C(G)_0\times D(G)$ から G までの射 $(x, y) \rightarrow xy$ は有限被覆です。

提案 4 の記法により、$V =\{e\}$ と部分群が得られます。G の $f(T)$ と $f(S)$ はコンパクトなので閉じられます。 したがって、$f(T) =$ $C(G)_0,f(S) = D(G)$ を示すだけで十分です。 さて、$L(G) = L(f(T))\times L(f(S))$; S は半単純で T は可換であるため、これは $L(f(T)) =\mathscr{C}(L(G)) = L(C(G)_0)$ (第 III, §9, no. 3 章、提案 8) と $L(f(S)) =\mathscr{D}L(G) = L(D(G))$ (第 III, §9, no. 2 章、提案 4 の修正) を意味し、したがって前述の主張が成り立ちます。

#### 系 2 {#lie-ix-s1-prop-4-cor-2 .statement tag=019K}

中心と連結コンパクト半単純リー 群の基本波群は有限です。ユニバーサルカバーはコンパクトです。

提案 4 の記法により、群 V と T は単位元に減らされます。したがって、S は G の普遍的な被覆であり、G の基本群は Ker $f$ と同型であるため、有限です。 G が半単純であるため、G の中心 D は離散的であり、D は有限です。

#### 系 3 {#lie-ix-s1-prop-4-cor-3 .statement tag=019L}

接続されたコンパクト・リー群 G の基本群は、C(G) の次元に等しい階数の有限型の $\mathbf{Z}$ 加群です。

確かに、コルの記法では。 1、$C(G)_0$ の基本群は $\mathbf{Z}^n$ と同型で、$n=$ は $C(G)_0$ であり、D(G) の基本群は有限です (Cor. 2)。

#### 系 4 {#lie-ix-s1-prop-4-cor-4 .statement tag=019M}

G を接続されたコンパクト・リー群とします。次の条件は同等です。

(i) G は半単純です。

(ii) C(G) は有限です。

(i) $\pi_1(G)$ は有限です。

G を単純結合すると、半単純になります。

これはコルからの続きです。 1から3まで。

#### 系 5 {#lie-ix-s1-prop-4-cor-5 .statement tag=019N}

G を接続されたコンパクト・リー群とします。この場合、Int(G) はリー群 Aut(G) の単位成分になります (第 III, §10, no. 2 章)。

$f\in$ Aut(G)$_0$ とします。次に、$f$ 誘導する自己同型 $f_1$ の $C(G)_0$ と自己同型 $f_2$ の D(G) があり、$f_1\in$ Aut(C(G)$_0$)$_0, f_2\in$オート(D(G))$_0$。 Aut(C(G)$_0$) は離散であるため (一般位相、章 VII, §2, no. 4、提案 5)、$f_1=$ Id が得られます。 D(G) は半単純なので、第 3 章によります。 III, §10, no. 2、コル。 Thの2。 1 すべての $x\in$ D(G) に対して $f_2(x) =gxg^{-1}$ となるような D(G) の元 $g$ が存在します。すべての $x\in C(G)_0$ について、$gxg^{-1}=x$ = $f_1(x)$ となります。 $G = C(G)_0.D(G)$ 以降、すべての $x\in G$ に対して $gxg^{-1}=f(x)$ となるため、$f=$ Int $g$ となります。

#### 命題 5 {#lie-ix-s1-prop-5 .statement tag=019O}

G をリー群とし、そのリー代数はコンパクトです。

a) G が接続されていると仮定します。すると、G は最大のコンパクト部分群 K になります。それはつながっています。 G が直接積 $N\times K$ であるような G の閉じた中心ベクトル部分群 (no. 2) N が存在します。

b) G の接続された成分の群が有限であると仮定します。それから：

(i) G のすべてのコンパクト部分群は、最大コンパクト部分群に含まれます。

(ii) $K_1$ と $K_2$ が G の 2 つの極大コンパクト部分群である場合、$K_2=gK_1g^{-1}$ となるような $g\in G$ が存在します。

(iii) K を G の最大コンパクト部分群とします。その場合、$K\cap G_0$ は $K_0$ に等しくなります。 $G_0$の最大のコンパクト部分群です。

(iv) G に正規な $G_0$ の閉中心ベクトル部分群 N が存在し、G の任意の極大コンパクト部分群 K に対して、$G_0$ は $K_0$ の N による直接積であり、G は K による N の半直接積です。

a) 提案 4 の記法を維持します。V 上の Ker $f$ の射影は、ベクトル群 V の有限部分群であるため、単位元に還元されます。したがって、Ker $f$ は $T\times S$ に含まれるため、G はベクトル群 $N =f(V)$ の直接積とコンパクト群 $K =f(T\times S)$ です。 G のすべての圧縮部分群は N 上に射影を持ち、それは単位元に還元されるため、K に含まれます。これは a) を証明します。

b) ここで、$G/G_0$ が有限であると仮定します。 $a), G_0$ は、最大のコンパクトな部分群 M とベクトル部分群 P の直接の積です。 部分群 G の M は明らかに正常です。 $\mathfrak{n}$ を L(G) の L(M) の補数であるベクトル部分空間とし、G の随伴表現の下で安定します (no. 1 と no. 3、提案 3)。これはL(G)の理想であり、$L(G) = L(M)\times \mathfrak{n}$があります。 N を G の積分部分群とリー代数 $\mathfrak{n}$ とします。章著III, §6, no. 6、提案 14、G では正常です。 カーネルL(M)を使用したL(G)のL(P)への射影は、$\mathfrak{n}$からL(P)までの同型性を引き起こします。 $G_0$ の P への射影は N から P へのエタール射を誘発するということになります。 P は単純結合であるため、これは同型写像であり、N はベクトル群です。 $M\times N$ から $G_0$ までの射 $(x, y) \rightarrow xy$ は単射エタール射 ($M\cap N$ が単位元に還元されるため)、したがって同型です。 It follows that N is a closed subgroup of G and that the quotient $G/N$ is compact, since $G_0/N$ is compact and $G/G_0$ is finite (General Topology, Chap. III, §4, no. 1, Cor. 2 of Prop. 2).

統合による、第 3 章VII, §3, no. 2、提案 3、G のすべてのコンパクト部分群は最大コンパクト部分群に含まれており、これらは共役であり、G の任意の最大コンパクト部分群 K について、G は K による N の半直接積です。 $G_0$ には N が含まれているため、N と $G_0\cap K$ の半直積になります。 $K/(G_0\cap K)$ は $G/G_0$ と同型であるため、有限であるため、$G_0\cap K$ は接続されており、したがって $K_0$ に等しいことがわかります。最後に、a) により、$K_0$ は明らかに $G_0$ の最大のコンパクトなサブグループです。

#### 系 {#lie-ix-s1-n4-cor-1 .statement tag=019P}

N が b) (iv) の条件を満たし、$K_1$ と $K_2$ が G の 2 つの極大コンパクト部分群である場合、$nK_1n^{-1}= K_2$ となる $n\in$ N が存在します。

実際、(ii) により、$gK_1g^{-1}= K_2$ となる元 $g\in G$ が存在します。 (iv) により、$g=nk$ となるような $n\in N$ と $k\in K_1$ が存在します。 元 $n$ には必要なプロパティが含まれます。

### 練習問題 {#lie-ix-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
