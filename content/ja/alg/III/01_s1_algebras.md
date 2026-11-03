---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 1
section_title: Algebras
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 428-438, 618
pdf_pages: 0452-0462, 0642-0642
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF AN ALGEBRA
      page: 428
      pdf_page: 452
    - "no": 2
      title: SUBALGEBRAS. IDEALS. QUOTIENT ALGEBRAS
      page: 429
      pdf_page: 453
    - "no": 3
      title: DIAGRAMS EXPRESSING ASSOCIATIVITY AND COMMUTATIVITY
      page: 431
      pdf_page: 455
    - "no": 4
      title: PRODUCTS OF ALGEBRAS
      page: 432
      pdf_page: 456
    - "no": 5
      title: RESTRICTION AND EXTENSION OF SCALARS
      page: 433
      pdf_page: 457
    - "no": 6
      title: INVERSE AND DIRECT LIMITS OF ALGEBRAS
      page: 434
      pdf_page: 458
    - "no": 7
      title: BASES OF AN ALGEBRA. MULTIPLICATION TABLE
      page: 436
      pdf_page: 460
statements: 5
exercises: 1
content_sha256: 7c888b4279bf7cab34fe96178bb16bb9dc88d04dec76bce310a89d4d711a8a91
translated_from: content/en/alg/III/01_s1_algebras.md
translation_method: google
source_content_sha256: 820912e8d5d630a54cb7380bd85e9cf6d35d1c95d761b599b7ec5d3af2010845
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 36bdf8d6297f9b2ab21171ad641507b1ac795e4d051cf3c084419be46c38e22b
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 1。 代数

### 1. 代数中定義

#### 定義 1 {#alg-iii-s1-def-1 .statement tag=05YR}

$A$ を可換環とします。 $A$ 上の代数 (混乱を恐れない場合は、$A$-代数、または単に代数) は、構造を含む集合 $E$ で、次のように定義されます。
(1) $E$ 上の $A$ モジュール構造。
(2) $E \times E$ から $E$ への $A$ 双線形写像 (II, § 3, no. 5)。

この定義で発生する $E \times E$ から $E$ への $A$ 双線形写像は、 代数 $E$ の乗法と呼ばれます。通常は $(x, y) \mapsto x.y$ または単に $(x, y) \mapsto xy$ で表されます。

$(\alpha_i)_{i \in I}$ と $(\beta_j)_{j \in J}$ を、$A$、有限台 (I, § 2, no. 1) の 2 つのファミリーである元とします。次に、$E$の元のすべての家族$(x_i)_{i \in I}$と$(y_j)_{j \in J}$について、一般分配率公式 (I, § 3, no. 4)

$$
\left( \sum_{i \in I} \alpha_i x_i \right) \left( \sum_{j \in J} \beta_j y_j \right) = \sum_{(i, j) \in I \times J} (\alpha_i \beta_j)(x_i y_j)
$$

保持します。特に

$$
(\alpha x)y = x(\alpha y) = \alpha(xy) \quad \text{for } \alpha \in A, x \in E \text{ and } y \in E.
$$

$E \times E$ から $E$ への双線形写像 $(x, y) \mapsto yx$ と、$E$ 定義する上の $A$ 加群構造、$E$ 上の $A$ 代数構造は、与えられた代数の逆と呼ばれます。 構造。 集合 $E$ とこの新しい構造は反対多元環から代数 $E$ と呼ばれます。多くの場合、$E^0$ で表されます。 $A$-代数 $E$ は、その反対のものと同一である場合、他の語は、$E$ の乗法が可換である場合、可換と呼ばれます。 $E$ の $E^0$ への同型は、代数 $E$ の反自己同型とも呼ばれます。

代数 $E$ の乗法が結合的であるとき、$E$ は結合的 $A$-代数と呼ばれます。 $E$の乗法が単位元(必然的に一意(I, § 2, no. 1))を認めるとき、この元は$E$の単位元と呼ばれ、$E$は単位代数と呼ばれます。

#### 例 {#alg-iii-s1-n1-exa-1 .statement tag=05YS}

(1) すべての可換環 $A$ は、(結合および可換) $A$-代数として考えることができます。
(2) $E$ を擬似リング (I, § 8, no. 1) とする。 $E$ の乗法と、$E$ の定義する $E$ の結合$\mathbf{Z}$-代数構造のユニークな $\mathbf{Z}$ モジュール構造。
(3) $F$ を集合と $A$ 可換環とします。 集合 $A^F$ $F$ のすべての写像を $A$ に、積環構造 (I, § 8, no. 10) と積

A-加群構造 (II, § 1, no. 5) は結合的で可換な A-代数です。

(4) E を A-代数とします。内部の法則 $(x, y) \mapsto xy + yx$ と $(x, y) \mapsto xy - yx$ 定義する (E の A-加群構造を含む) E 上の 2 つの A-代数構造ですが、これらは一般に結合しません。最初の法則

$$(x, y) \mapsto xy + yx$$

は常に可換です。

#### 定義 2 {#alg-iii-s1-def-2 .statement tag=05YT}

*2 つの代数* E, E' *上可換環* A, *準同型 of* E *into* E' *は写像* $f : E \to E'$ *そのような*
(1) *f は * A* モジュール準同型* です。
(2) $f(xy) = f(x)f(y)$ *すべて* $x \in E$ * そして* $y \in E$。

明らかに 2 つの A-代数準同型のうち合成は A-代数準同型です。すべての全単射語代数準同型は同型です。したがって、A-代数準同型は、A-代数構造 (*集合理論*, IV, 2, no. 1) の種の *射* と見なすことができます。以下では常に、この射の選択が作成されたと仮定します。 E、E'が2つのA-代数である場合、$\operatorname{Hom}_{A\text{-alg}}(E, E')$はEのA-代数準同型の集合をE'に表します。

E、E' をそれぞれ単位元を持つ 2 つの代数とします。 E の準同型から E' の写像単位元から E' の単位元までを *unital 準同型* (または *unital 代数射*) と呼びます。

### 2. 部分代数。理想。 商代数

Aを可換環、EをA-代数とします。 F が E の乗法で安定している W のサブ A モジュールである場合、E 定義するの乗法の F × F に制限 (F の A-加群構造を含む) F の A-代数構造。 この構造を伴う F は、A-代数 E の *部分代数* と呼ばれます。 E の部分代数のすべての共通部分は E の部分代数です。 E の元の各ファミリー $(x_i)_{i \in I}$、E の部分代数の共通部分含むについて、すべての $x_i$ はファミリー $(x_i)_{i \in I}$ と $(x_i)_{i \in I}$ によって *生成* された E の部分代数と呼ばれ、*生成する系* と呼ばれます。この部分代数の (または *生成するファミリー*)。 $u : E \to E'$ が A-代数準同型である場合、E のすべての部分代数 F の像 $u(F)$ は E' の部分代数です。

E を *連想* 代数とします。 E のすべての部分集合 M に対して、M のすべての元と置換可能な E の元の集合 $M'$ は、E の M の *セントラライザー* 部分代数 (I, § 1, no. 5) と呼ばれる E の部分代数です。 E の $M'$ のセントラライザー $M''$ は、M の *bicentralizer* とも呼ばれます。明らかに$M \subset M''$。したがって、$M'$ はその二分化器 $M''$ に含まれており、これはまさに $M''$ の集中化器です。しかし、関係 $M \subset M''$ は $M'' \subset M'$ を意味するので、$M' = M''$ (cf. *集合理論*, III, § 1, no. 7, 命題 2) となります。 F が E の部分代数である場合、F の *中心* は F の共通部分 $F \cap F'$ であり、E のセントラライザー $F'$ であることに注意してください。

F は *可換* なので、$F \subset F'$、したがって $F' \supset F''$; F のバイセントラライザー $F''$ は、この場合、F の *中心* です。

特定の非結合代数 (例: リー代数) の場合、部分代数と中心のセントラライザーの概念は異なって定義されます (*リー群とリー代数*、I, § 1, no. 6)。

A-代数 E の部分集合 $a$ は、$a$ が E のサブ A 加群であり、関係 $x \in a,\ y \in E$ が $yx \in a$ (それぞれ $xy \in a$) を暗示するとき、E の *左イデアル* (それぞれ *右イデアル*) と呼ばれます。 $a$ が E の左イデアルであるか、反対多元環 $E^0$ の右イデアルであると言うのは同じことになります。 E の *両側イデアル* は E の部分集合 $a$ であり、これは左イデアルと右イデアルの両方です。 E が結合的で単位元 $e$ を認めるとき、$\alpha \in A$ と $x \in E$ については、(2) (no. 1) によって $\alpha x = (\alpha e)x = x(\alpha e)$ となり、したがって *環* E (I, § 8, no. 6) の (右、左、両面) 理想は、 *代数* E の (右、左、両面) イデアル。代数 E の左 (それぞれ右、両面) イデアルのすべての和とすべての共通部分は、左 (それぞれ右、両面) イデアルです。 E の左 (それぞれ右、それぞれ両面) イデアルの共通部分含む部分集合 X は、X によって *生成された E の左 (それぞれ右、それぞれ両側) イデアルと呼ばれます。

$b$ を A-代数 E の *両側* 理想とする。 $x \equiv x' \pmod{b}$ と $y \equiv y' \pmod{b}$ の場合、
$$
x(y - y') \in b \quad \text{and} \quad (x - x')y' \in b
$$
したがって $xy \equiv x'y' \pmod{b}$ です。 したがって、内部法則は商 A-加群 $E/b$ で定義できます。これは、E の乗法法則 $(x, y) \mapsto xy$ の商を同値関係 $x \equiv x' \pmod{b}$ (I, § 1, no. 6) で定義できます。 この商法則が $(E/b) \times (E/b)$ から $E/b$ への A 双線形写像であることがすぐに検証されます。したがって、$E/b$ では A-加群構造、$E/b$では A-代数構造で定義するとなります。 $E/b$は、この代数構造とともに、代数Eの*商代数*を両面イデアル$b$により呼びます。 標準写像 $p : E \to E/b$ は代数準同型です。

E、$E'$ を 2 つの A-代数と $u : E \to E'$ 代数準同型とします。 像 $u(E)$ は $E'$ の部分代数であり、核 $b = u^{-1}(0)$ は E の両面イデアルです。さらに、$u$ の正規の分解では次のようになります。
$$
E \xrightarrow{p} E/b \xrightarrow{v} u(E) \xrightarrow{j} E'
$$
$v$ は *代数同型* です。より一般的には、語 "環" が "代数" に置き換えられても、章 I, § 8, no. 9 のすべての結果 (およびその証明) は依然として有効です。

Aを可換環、EをA-代数とします。 集合 $\tilde{E} = A \times E$ に、定義する合成の次の法則:
$$
\begin{align*}
(\lambda, x) + (\mu, y) &= (\lambda + \mu, x + y) \\
(\lambda, x)(\mu, y) &= (\lambda \mu, xy + \mu x + \lambda y) \\
\lambda(\mu, x) &= (\lambda \mu, \lambda x).
\end{align*}
$$

これら合成の法則を含む$\tilde{E}$は、$A$を超える代数であり、$(1,0)$はこの代数の単位元であることがすぐに検証されます。 集合 $\{0\} \times E$は$\tilde{E}$の両面理想であり、$x \mapsto (0,x)$は代数$E$の部分代数$\{0\} \times E$の同型であり、これにより$E$と$\{0\} \times E$は特定された。 $\tilde{E}$は単位元と隣接して$E$から派生して代数と呼ばれます。 $E$ がそうである場合に限り、それは結合的 (または可換的) になります。

### 3. 図式連想性を表現し、 可換性

$A$ を可換環とし、$E$ を $A$ モジュールとします。 $E \times E$ から $E$ への双線形写像が与えられることは、$A$ 線形写像が与えられることと同等です。

$$
m : E \otimes_A E \to E
$$

(II, § 3, no. 5)。したがって、$E$ 上の $A$-代数構造は、$E$ に $A$ 加群構造と、$E \otimes_A E$ から $E$ への $A$ 線形写像を与えることによって定義されます。

$E'$ を他の $A$-代数、$m' : E' \otimes_A E' \to E'$ を $E'$ の乗法を定義する $A$ 線形写像とします。 写像 $f : E \to E'$ は、$f$ が写像で可換図式をレンダリングする場合に限り、$A$-代数準同型写像です。

$$
\begin{array}{ccc}
E \otimes_A E & \xrightarrow{f \otimes f} & E' \otimes_A E' \\
\downarrow m & & \downarrow m' \\
E & \xrightarrow{f} & E'
\end{array}
$$

$A$-代数 $E$ が結合的であるためには、(テンソル積、cf. II, § 3, no. 8 の結合性を考慮して) $A$ 線形写像の図式が必要かつ十分です。

$$
\begin{array}{ccc}
E \otimes_A E \otimes_A E & \xrightarrow{m \otimes 1_E} & E \otimes_A E \\
\downarrow 1_E \otimes m & & \downarrow m \\
E \otimes_A E & \xrightarrow{m} & E
\end{array}
$$

可換的であること。同様に、$A$-代数$E$が可換であるためには、$A$-線形写像の図式が必要かつ十分です。

$$
\begin{array}{ccc}
E \otimes_A E & \xrightarrow{\sigma} & E \otimes_A E \\
\downarrow m & & \downarrow m \\
E & & E
\end{array}
$$

ここで、$\sigma$ は、$x \in E, y \in E$ (II, § 3, no. 1、系 2 から命題 1) に対して $\sigma(x \otimes y) = y \otimes x$ によって定義された正規の $A$ 線形マッピングを表します。

すべての $c \in E$ について、$\eta_c$ は、条件 $\eta_c(1) = c$ によって定義される A の A-線型写像を E に表します。 $c$ が E の単位元になるためには、2 つの図式が必要かつ十分です

$$
\begin{array}{ccc}
A \otimes_A E & \xrightarrow{\eta_c \otimes 1_E} & E \otimes_A E \\
\downarrow i & & \downarrow m \\
E & & E \\
& \uparrow & \\
E \otimes_A A & \xrightarrow{1_E \otimes \eta_c} & E \otimes_A E \\
& \downarrow i' & \downarrow m \\
E & & E
\end{array}
$$

可換であること ($i$ と $i'$ は標準同型 (II, § 3, no. 4、命題 4) を表します)。

E を単位元 e を伴う A-代数とし、$\eta = \eta_e$ ($\eta_E$ とも表す) とします。次に、$\eta(\alpha \beta) = \eta(\alpha) \eta(\beta) = \alpha \eta(\beta)$、(2) (no. 1) により、

$$(\alpha e)(\beta e) = (\alpha \beta)e = \alpha(\beta e);$$

したがって、$\eta$ は A-代数準同型です。 E の A-加群構造が $\eta$ を使用して定義できることに注目してください。

$$(3)$$
$$\alpha x = \eta(\alpha) \cdot x \quad \text{for } \alpha \in A, x \in E$$

(ここで、右側の乗法は E にあります)。 準同型 $\eta$ の像は E の部分代数で、その元は E のすべての元と交換します。 準同型 $\eta$ の核は A-加群 E の元 e の消滅子です。 (3) により、A-加群 E (II, § 1, no. 12) の消滅子にもなります。

代数 E が単体かつ結合性の場合、$\eta$ は環準同型になります。逆に、環 A が可換であると仮定して、像 $\rho(A)$ が B の中心に含まれるように、$\rho : A \to B$ を環準同型とします。次に、A-代数構造は、 (cf. (3)) と書くことによって、結合的で単位的な B 上に定義されます。

$$\lambda x = \rho(\lambda) \cdot x \quad \text{for } \lambda \in A, x \in E.$$

### 4. 代数中積

$(E_i)_{i \in I}$ を同じ可換環 A 上の代数の族とします。積集合 $E = \prod_{i \in I} E_i$、積 A-加群構造 (II, § 1, no. 5) および乗法がすぐに検証されます。

$$(4)$$
$$((x_i), (y_i)) \mapsto (x_i y_i)$$

定義する A-代数構造;これにより、構造、集合 E は、代数 $(E_i)_{i \in I}$ の族の積代数と呼ばれます。

すべての代数 $E_i$ が結合的 (それぞれ可換、それぞれ単位) である場合、それらの積も同様です。また、I, § 8, no. 10、拡大するに記載の全ての性質を、代数の任意の積にそのまま適用します。

### 5. スカラーの制限と拡大

$A_0$ と A を 2 つの可換環と $\rho : A_0 \to A$ 環準同型とします。 E が A-代数の場合、E および外部法則で加法によって定義された $A_0$ モジュールを (II, § 1, no. 13 に準拠して) $\rho_* (E)$ で表します。

$$
\lambda . x = \rho(\lambda)x \quad \text{for all } \lambda \in A_0 \text{ and all } x \in E.
$$

Eの乗法と、$\rho_* (E)$の定義するの$A_0$加群構造、$\rho_* (E)$の$A_0$-代数構造。 $A_0$がAの部分環と$\rho$標準単射のとき、スカラーの環Aを$A_0$に限定すると、Eから代数$\rho_* (E)$が得られると言われます。言葉の乱用により、これも$\rho$が恣意的なのにときどきと言われます。

F を$A_0$-代数とする。 $A_0$-代数準同型性 $F \to \rho_* (E)$ は、半準同型性 ($\rho$ に対して) または F から A-代数 E への $\rho$-準同型性と呼ばれます。混乱がなければ、これは $A_0$ 準同型性とも呼ばれます。 E, $E'$ が 2 つの A-代数である場合、すべての A-代数準同型 $E \to E'$ も $A_0$-代数準同型性 $\rho_* (E) \to \rho_* (E')$ です。

ここで、2 つの可換環 A と B、および環準同型 $\rho : A \to B$ について考えてみましょう。すべての A-加群 E に対して、スカラーの環 A を B に拡張することで E から得られる B-加群 $\rho^*(E) = E \otimes_A B$ が定義されています (II, § 5, no. 1)。 E も A-代数である場合、$\rho^*(E)$ の B 代数構造では定義するとなります。このためには、$(E \otimes_A B) \otimes_B (E \otimes_A B)$ が $(E \otimes_A E) \otimes_A B$ (II, § 5, no. 1, 命題 3) と正準的に同型であることに注意してください。 E 上の $m : E \otimes_A E \to E$ 定義する乗法の場合、写像 $m \otimes 1_B : (E \otimes_A E) \otimes_A B \to E \otimes_A B$ は正規的に B-線型写像と識別されます。

$$
m' : \rho^*(E) \otimes_B \rho^*(E) \to \rho^*(E)
$$

$\rho^*(E)$ 上の目的の B 代数構造定義する。したがって、

(5)

$$
(x \otimes \beta)(x' \otimes \beta') = (xx') \otimes (\beta \beta')
$$

E の $x, x'$、B の $\beta$ および $\beta'$ について。 B 代数 $\rho^*(E)$ は、スカラーの環 A を B に拡張することによって ($\rho$ によって) A-代数 E から導出されると言われています。 $E_{(B)}$ または $E \otimes_A B$ とも表されます。 E が結合性 (可換性、単位性) の場合、$\rho^*(E)$ も同様です。

#### 命題 1 {#alg-iii-s1-prop-1 .statement tag=05YU}

すべての A-代数 E に対して、E の $E_{(B)}$ への標準写像 $\phi_E : x \mapsto x \otimes 1$ は、代数の A 準同型写像です。さらに、すべての B-代数 F とすべての $A$-準同型 $f : E \to F$ に対して、すべての $x \in E$ に対して $\bar{f}(x \otimes 1) = f(x)$ となるような $B$-準同型 $\bar{f} : E_{(B)} \to F$ が 1 つだけ存在します。

最初の主張は、$E_{(B)}$ の乗法の定義の直後に続き、$x \in E$ と $x' \in E$ に $(x \otimes 1)(x' \otimes 1) = (xx') \otimes 1$ が与えられます。すべての $x \in E$ に対する $E_{(B)}$ の $F$ 満たす関係 $\bar{f}(x \otimes 1) = f(x)$ への $B$ 線形写像 $\bar{f}$ の存在と一意性は、II, § 5, no. 1、命題 1 から続きます。ここでは、すべては $y$ の $\bar{f}(yy') = \bar{f}(y)\bar{f}(y')$ と $E_{(B)}$ の $y'$ を検証することになります。 形 $x \otimes 1$ ($x \in E$ 付き) 生成するの $B$ モジュール $E_{(B)}$ の元として、$y = x \otimes 1, y' = x' \otimes 1$ と $x \in E, x' \in E$ のケースに限定されるかもしれません。 $yy' = (xx') \otimes 1$、関係 $\bar{f}(yy') = \bar{f}(y)\bar{f}(y')$ のように、$f(xx') = f(x)f(x')$ から続きます。

$f \mapsto \bar{f}$ は正規の全単射であるとも言えます

$$
\text{Hom}_{A\text{-alg.}}(E, \rho_*(F)) \to \text{Hom}_{B\text{-alg.}}(\rho^*(E), F).
$$

したがって、$E_{(B)}$ と $\phi_E$ からなる順序ペアは、普遍写像問題 (集合論、IV, § 3, no. 1) の解です。ここで、$\Sigma$ は $B$-代数構造の種であり、$\alpha$ は $E$ からの $A$-準同型写像を a に写像します。 $B$-代数。

#### 系 {#alg-iii-s1-n5-cor-1 .statement tag=05YV}

*$E, E'$ を 2 つの $A$-代数とする。 代数 $u : E \to E', u \otimes 1_B$ のすべての $A$ 準同型性は、 代数 $v : E \otimes_A B \to E' \otimes_A B$ の固有の $B$ 準同型性であり、 図式* を可換にレンダリングします。

$$
\begin{array}{ccc}
E & \xrightarrow{\phi_E} & E \otimes_A B \\
u \downarrow & & \downarrow v \\
E' & \xrightarrow{\phi_{E'}} & E' \otimes_A B
\end{array}
$$

$C$ を 3 番目の可換環と $\sigma : B \to C$ 環準同型とします。正準 $C$ 準同型写像は明らかです

$$
\sigma^*(\rho^*(E)) \to (\sigma \circ \rho)^*(E)
$$

写像 $(x \otimes 1) \otimes 1$ ～ $x \otimes 1$ のすべての $x \in E$ (II, § 5, no. 1、命題 2) は代数同型です。

### 6. 代数の逆および直接極限

$I$ を事前順序付けされた集合とし、$(A_i, \phi_{ij})$ を *可換環* の逆数系とし、$I$ をインデックス付け集合とします。 $(E_i, f_{ij})$ を、インデックス集合 (II, § 6, no. 1) として$I$ をもつ$A_i$ 加群の逆系とし、さらに、各$E_i$ が$A_i$-代数構造を持っていると仮定します。 $i \leq j$、$f_{ij}$ は、代数 ($\phi_{ij}$ に対する) (no. 5) の $A_j$ 準同型写像です。 $A$ モジュール構造を持つ $A = \lim \leftarrow A_i$ と $E = \lim \leftarrow E_i$ を、$A_i$ モジュール $E_i$ (II, § 6, no. 1) の構造の逆極限とします。 $E$の合成の法則は、乗法(I, § 10, no. 1)でマグマとみなされる$E_i$の逆極限と考えられ、$E$の$A$モジュール構造であることがすぐに検証されます。 $E$ 上の定義すると $A$-代数構造; $(E_i, f_{ij})$ は $A_i$-代数の *逆系* と呼ばれ、$A$-代数 $E$ はその *逆極限* と呼ばれます。 $f_i : E \to E_i$、$\phi_i : A \to A_i$ が標準写像である場合、$f_i$ は代数の *$A$* 準同型写像です ($\phi_i$ に対して)。 $E_i$ が結合的 (可換的) であれば、$E$ も同様です。それぞれの $E_i$ が $i \leq j$ に対して単位元 $e_i$ と $f_{ij}(e_j) = e_i$ を認めた場合、$e = (e_i)$ は代数 $E$ の単位元になります。

$(E'_i, f'_{ij})$ を $A_i$-代数の他の逆数系とし、すべての $i$ について $u_i : E_i \to E'_i$ を $A_i$-代数準同型とし、これらの写像は *逆系* を形成します。この場合、$u = \lim u_i$ は *$A$*-代数準同型写像です。

ここで、すべての $A_i$ が *同じ* 可換 *環* $A$ と $\phi_{ij}$ から $\mathrm{Id}_A$ に等しいと仮定します。したがって、$E = \lim \leftarrow E_i$ は $A$-代数です。 $F$ を $A$-代数とし、すべての $i \in I$ について、$u_i : F \to E_i$ を $(u_i)$ が写像の逆系となるような $A$-代数準同型写像とする。すると、$u = \lim \leftarrow u_i$ は代数 $F$ の準同型が代数 $E$ になります。 *逆に*、すべての $A$-代数準同型 $v : F \to E$ について、$v_i = f_i \circ v$ の族は $v = \lim \leftarrow v_i$ のような $A$-代数準同型の逆系です。さらに、$\bar{f}_{ij} = \mathrm{Hom}(1_F, f_{ij})$, $(\mathrm{Hom}_{A\text{-alg.}}(F, E_i), \bar{f}_{ij})$ と書くと明らかに集合の逆系であるため、上記の注意はというによって標準写像 $v \mapsto (f_i \circ v)$ が *全単射* であることも表現できることがわかります。

$$
l_F : \mathrm{Hom}_{A\text{-alg.}}(F, \lim \leftarrow E_i) \to \lim \leftarrow \mathrm{Hom}_{A\text{-alg.}}(F, E_i).
$$

さらに、すべての $A$-代数準同型性 $w : F \to F'$ について、

$$
\bar{w}_i = \mathrm{Hom}(w, 1_{E_i}) : \mathrm{Hom}_{A\text{-alg.}}(F', E_i) \to \mathrm{Hom}_{A\text{-alg.}}(F, E_i)
$$

形写像と図式の逆系

$$
\begin{array}{ccc}
\mathrm{Hom}_{A\text{-alg.}}(F', \lim \leftarrow E_i) & \xrightarrow{l_{F'}} & \lim \leftarrow \mathrm{Hom}_{A\text{-alg.}}(F', E_i) \\
\downarrow \mathrm{Hom}(w, 1_E) & & \downarrow \lim \bar{w}_i \\
\mathrm{Hom}_{A\text{-alg.}}(F, \lim \leftarrow E_i) & \xrightarrow{l_F} & \lim \leftarrow \mathrm{Hom}_{A\text{-alg.}}(F, E_i)
\end{array}
$$

可換です。

ここで、$I$ が正しく*指示されている*と仮定します。 集合のインデックスとして $I$ を使用して、可換環 $(A_i, \phi_{ji})$ の直接系と $A_i$ モジュールの直接系 $(E_i, f_{ji})$ を考えてみましょう。それぞれの $E_i$ が $A_i$-代数構造を持ち、$i \leq j$ に対して、$f_{ji}$ が代数 ($\phi_{ji}$ に対して) (no. 5) の $A_i$-準同型写像であると仮定します。 $A = \lim \to A_i$、$E = \lim \to E_i$ としましょう。 $E$ は $A$ モジュール構造を持ち、$A_i$ モジュール $E_i$ (II, § 6, no. 2) の構造の直接の極限です。さらに、E 上の合成の法則は、E_i の直接の極限と考えられ、乗法 (I, § 10, no. 3) ではマグマと考えられ、E 上の A-加群構造、定義する A-代数 Eの構造; (E_i, f_{ji}) は A_i-代数の直接系と呼ばれ、A-代数 E はその直接の極限と呼ばれます。 f_i : E_i \to E、\phi_i : A_i \to A が標準写像である場合、f_i は代数 (\phi_i に対して) の A_i 準同型写像です。 E_i が結合的 (可換的) であれば、E も同様です。各 E_i が i \leq j に対して単位元 e_i および f_{ji}(e_i) = e_j を認める場合、E は I のすべての i に対して f_i(e_i) = e となるような単位元 e を認めます。

(E'_i, f'_{ji}) を A_i-代数の他の直接系とし、すべてについて u_i : E_i \to E'_i を A_i-代数準同型とし、これらの写像は直接系を形成します。その場合、u = \lim \to u_i は A-代数準同型となります。

ここで、すべての環 A_i が同じ環 A に等しく、\phi_{ji} が Id_A に等しいとします。したがって、E = \lim \to E_i は A-代数になります。 F を A-代数とし、すべてについて u_i : E_i \to F A-代数準同型とし、(u_i) が写像の直接系となるようにします。その場合、u = \lim \to u_i は代数 E の準同型から代数 F になります。逆に、すべての A-代数準同型 v : E \to F に対して、v_i = v \circ f_i の族は A-代数の直接系になります。 準同型は v = \lim \to v_i となります。さらに、 \vec{f}_{ij} = \mathrm{Hom}(f_{ij}, 1_F), (\mathrm{Hom}_{A\text{-alg.}}(E_i, F), \vec{f}_{ij}) と書くと、明らかに集合の逆系であることがわかります。 注意は、標準写像 v \mapsto (v \circ f_i) が全単射であることをというで表すこともできます。

$$
d_F : \mathrm{Hom}_{A\text{-alg.}}(\lim \to E_i, F) \to \lim \leftarrow \mathrm{Hom}_{A\text{-alg.}}(E_i, F).
$$

さらに、 A-代数準同型 w : F \to F' ごとに、

$$
\bar{w}_i = \mathrm{Hom}(1_{E_i}, w) : \mathrm{Hom}_{A\text{-alg.}}(E_i, F) \to \mathrm{Hom}_{A\text{-alg.}}(E_i, F')
$$

形写像と図式の逆系

$$
\begin{array}{ccc}
\mathrm{Hom}_{A\text{-alg.}}(\lim \to E_i, F) & \xrightarrow{d_F} & \lim \mathrm{Hom}_{A\text{-alg.}}(E_i, F) \\
\downarrow \mathrm{Hom}(1_E, w) & & \downarrow \lim \bar{w}_i \\
\mathrm{Hom}_{A\text{-alg.}}(\lim \to E_i, F') & \xrightarrow{d_{F'}} & \lim \mathrm{Hom}_{A\text{-alg.}}(E_i, F')
\end{array}
$$

可換です。

### 7. 代数の基底。 乗法表

定義により、A-代数 E の基底は、A-加群構造に対して E の基底になります。 (a_i)_{i \in I} を E の基底とします。注文されたすべての対 (i, j) \in I の元 of 環の一意のファミリー (\gamma^k_{ij})_{(i, j, k) \in I \times I \times I} が存在します。 \gamma^j_{ij} \neq 0 が有限であるような、I の k \times I, 集合

$$
a_i a_j = \sum_{k \in I} \gamma^k_{ij} a_k.
$$

$\gamma_{ij}^k$ は、基底 $(a_i)$ に対する代数 E の構造* の *定数と呼ばれ、関係 (7) は、代数 E の *乗法表* を構成します ( 基底 $(a_i)$)。

関係 (7) は、平方表の関係の右側から設定によって書き記されると想像できます。

$$
\begin{array}{c|ccc}
 & \cdots & a_j & \cdots \\
\hline
 & & & \\
\vdots & & & \\
\hline
a_i & & \sum_k \gamma_{ij}^k a_k & \\
\vdots & & &
\end{array}
$$

添字 $j$ の添字 $i$ と列の行に現れる元は積 $a_i a_j$ に等しいことが理解されます。

逆に、*A-加群* E、E の基底 $(a_i)_{i \in I}$、および A の元のファミリー $(\gamma_{ij}^k)$ が与えられ、$\gamma_{ij}^k \neq 0$ が有限であるような $k \in I$ のすべての順序付け対 $(i, j) \in I \times I$ 集合に対して、E には唯一の A-代数構造その下では関係 (7) が成立します。なぜなら、A-加群 $E \otimes_A E$ は自由で、基底 $(a_i \otimes a_j)_{(i, j) \in I \times I}$ (cf. II, § 3, no. 7、系 2 から命題) として認められるからです。 7)。

E を A-加群 E の A-代数および $(a_i)_{i \in I}$ 生成する系とします (たとえば、基底)。 E が *結合性* であるためには、 $a_i$ 満たすと *結合性関係* が必要かつ十分です

$$(8)$$
$$(a_i a_j) a_k = a_i (a_j a_k) \quad \text{for all } i, j, k$$

写像 $(x, y, z) \mapsto (xy)z - x(yz)$ は A-trilinear マッピングです
$$
E \times E \times E \to E
$$
したがって、定義する A-線型写像 $E \otimes_A E \otimes_A E \to E$;後者の写像が、A-加群 $E \otimes_A E \otimes_A E$ の形生成する系のすべての元 $a_i \otimes a_j \otimes a_k$ に対して零である場合、同じように零になります。

同様に、E が *可換*であるためには、 $a_i$ 満たすが *可換性関係* であることが必要かつ十分です

$$(9)$$
$$a_i a_j = a_j a_i \quad \text{for all } i, j.$$

証明も同様で、今回は A 双線形マッピング $(x, y) \mapsto xy - yx$ を考慮します。最後に、元 $e \in E$ が単位元になるためには、$a_i$ 満たす関係が必要かつ十分です。

$$(10)$$
$$a_i = e a_i = a_i e \quad \text{for all } i,$$

今回は、A-線型写像 $x \mapsto x - xe$ と $x \mapsto x - ex$ を考慮するとわかります。

$(a_i)_{i \in I}$ が E の基底であり、$(\gamma_{ij}^k)$ 対応するの定数族構造であるとき、関係 (8) は関係と等価です。

$$
\sum_r \gamma_{ij}^r \gamma_{rk}^s = \sum_r \gamma_{ir}^s \gamma_{jk}^r
$$

すべての$i, j, k, s$に。同様に、関係 (9) はすべての $i, j, k$ に対して $\gamma_{ij}^k = \gamma_{ji}^k$ と同等です。

$(a_i)_{i \in I}$ を A-代数 E の基底とします。 $\rho : A \to B$ が環準同型である場合、$(a_i \otimes 1)$ は B 代数 $\rho^*(E) = E \otimes_A B$ (II, § 5, no. 1, 命題 4) の基底です。 $(\gamma_{ij}^k)$ が基底 $(a_i)$ に対する構造の定数のファミリーである場合、ファミリー $(\rho(\gamma_{ij}^k))$ は基底 $(a_i \otimes 1)$ に対する $\rho^*(E)$ の構造の定数のファミリーです。

### 練習問題 {#alg-iii-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
