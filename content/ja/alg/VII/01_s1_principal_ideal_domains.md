---
book: alg
book_title: Algebra
chapter: VII
chapter_title: MODULES OVER PRINCIPAL IDEAL DOMAINS
section: 1
section_title: Principal ideal domains
lang: ja
source: alg-iv-vii
source_edition: 2003, Springer
pdf_pages: 0360-0365, 0407-0413
extraction: ocr
subsections:
    - "no": 1
      title: Definition of a principal ideal domain
      page: 0
      pdf_page: 360
    - "no": 2
      title: Divisibility in principal ideal domains
      page: 0
      pdf_page: 360
    - "no": 3
      title: Decomposition into irreducible factors in principal ideal domains
      page: 3
      pdf_page: 362
    - "no": 4
      title: Divisibility of rational integers
      page: 5
      pdf_page: 364
    - "no": 5
      title: Divisibility of polynomials in one indeterminate over a field
      page: 5
      pdf_page: 364
statements: 15
exercises: 28
content_sha256: cd658633084604d1c9a9b31c784f6303458502e2eeab3444212b4d49354d376c
translated_from: content/en/alg/VII/01_s1_principal_ideal_domains.md
translation_method: google
source_content_sha256: fccb95f1c743016175d920f3d9b4107ca71a6669ffca75cd9cc5695d9f404b32
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: d09846d07d2c1528650b5a94f69ad5a73c6944df993567f92019a43eb5ba9e55
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 1。 主イデアル整域

### 1. 主イデアル整域中定義

(I、p. 104) を思い出してください。可換環 $A$ の理想は、いくつかの $a \in A$ に対して形 $(a) = Aa$ を持つ場合、*主要*であると言われます。

#### 定義 1 {#alg-vii-s1-def-1 .statement tag=070X}

*主イデアル整域は整域 (I、p. 116) であり、すべての理想が主要です。*

#### 例 {#alg-vii-s1-n1-exa-1 .statement tag=070Y}

有理数整数の環 $\mathbf{Z}$ は主イデアル整域 (I, p. 111) です。 $K$ が可換体の場合、$K$ 上の 1 つの不定数における多項式環 $K[X]$ は主イデアル整域 (IV、p. 11、提案 11)。同じことが正式な冪系列 $K[[X]]$ の環にも当てはまり、この環のすべての理想には形 $(X^n)$ があります (IV、p. 38、提案 12)。 \* p 進数体の整数の環は主イデアル整域です。 \*

$\mathbf{Q}(i)$ が既約多項式 $X^2 + 1$ の根 $i$ を隣接することによって有理数数の体 $\mathbf{Q}$ から得られる体を表す場合、元 $a + bi$ $\mathbf{Q}(i)$、ここで $a$ と $b$ は有理数整数、形部分環 $\mathbf{Q}(i)$ の $\mathbf{A}$、« ガウス整数 » と呼ばれ、主イデアル整域 (VII, p. 50、例 7)。対照的に、体 $\mathbf{Q}(\rho)$ では、$\rho$ が $X^2 + 5$ の根である場合、部分環 $B$ からなる元 $a + bp$ (a と b の有理整数) は成立しません。 主イデアル整域 (VII、p. 51、例 12)。

体 $K$ を超える 2 つの不定数の多項式環 $K[X, Y]$ は主イデアル整域ではありません。確かに、非零定数は、$X$ と $Y$ の両方割るを成す唯一の元であり、$X$ と $Y$ によって生成される理想的な生成するはありません。

### 2. 主イデアル整域の割り算

Let $A$ be a principal ideal domain and let $K$ be its field of fractions (I, p. 116); we will see that the ordered group $\mathscr{P}^*$ of principal fractional ideals (*VI*, p. 6) of $K$ is lattice ordered; more precisely:

#### 命題 1 {#alg-vii-s1-prop-1 .statement tag=070Z}

*$K$ を主イデアル整域 $A$ の分数の体とし、$(x_i)_{i \in I}$ を共通のの分母 $b \in K^*$ を持つ $K$ の元の族とする (他の場合は語) $i$ 全員に $bx_i \in A$)。それから：*

a) ファミリ $(x_i)$ は $K$ に gcd を持っています。
b) $(x_i)$ のすべての gcd は形 $d = \sum a_i x_i$ で表現できます。ここで、$a_i$ は $A$ の元であり、有限を除いてその多くはすべて零です。

確かに、$A$ の理想 $\sum Abx$ が主要であり、形 $Ad'$ も同様です。 $d' = bd \ (d \in K)$を入れます。 関係 $d' = \sum a_i b x_i$ から $d = \sum a_i x_i$ を導き出し、ここで $a_i \in A$ です。したがって、$x_i$ 割る $d$ のすべての共通の因子になります。一方、$bd$は$bx$の共通の因子なので、構成により、$d$は$x_i$の共通の因子になります。

#### 注意 {#alg-vii-s1-n2-rem-1 .statement tag=0710}

提案 1 は、制限なしで、$A$ の元の任意のファミリ $(x_i)$ ($b = 1$ を取る)、および $K$ の元の任意の有限ファミリ $(x_i)$ ($x_i = c_i b_i$ の場合) にも適用されます。 $c_i \in A$ と $b_i \in A$ を計算し、$b$ を $b_i$ の積とします)。

#### 系 {#alg-vii-s1-n2-cor-1 .statement tag=0711}

— $(x_i)$ を、整域 $B$ に部分環として含まれる主イデアル整域 $A$ の元の任意のファミリーとし、$d$ を $A$ のファミリー $(x_i)$ の gcd とします。次に、ファミリー $(x_i)$ には $B$ に gcd があり、$d$ もそのうちの 1 つです。

確かに、$d$は$B$の$x_i$の共通の因子です。一方、関係 $d = \sum a_i x_i$ は、$B$ 割る $d$ の $x_i$ のすべての共通の因子を示します。

この系の重要な適用は、$A = K[X]$ と $B = E[X]$ のときです。ここで、$K$ は体、$E$ は $K$ の拡大 (IV、p. 12、Cor. 1) です。

提案 1 の最初の主張は、順序付き群 $\mathscr{P}^*$ が格子順序付け ($VI,$ p. 10) であることを示しています。特に、$K$ の元のすべての有限族は lcm を認めます。したがって、$VI$、pp. 10 ～ 17 に (DIV) で示されている結果を主イデアル整域に適用できます。

次の結果は、提案 I の 2 番目主張の帰結です。

#### 定理 1 (« ベズーの正体 ») {#alg-vii-s1-thm-1 .statement tag=0712}

— 主イデアル整域 $A$ の元 $x_i \ (i \in I)$ は、$A$ の元 $a_i \ (i \in I)$ が存在し、$\sum a_i x_i = 1$ となるような有限に多くの零が存在する場合に限り、集合的に互いに素です。

条件の必然性は提案 1 にすぎません。逆に、$\sum a_i x_i = 1$ の場合、$x_i$ 割るのすべての共通の因子が 1 となるため、1 は $x_i$ の gcd になります。

#### 命題 2 {#alg-vii-s1-prop-2 .statement tag=0713}

— $a, b, d, m$ と $p$ を元 of 体 of 分数 $K$ of 主イデアル整域 $A$ とします。
a) « $d$ は $a$ の gcd であり、 $b$ » は « $(d) = (a) + (b)$ » と同等です。
b) « $m$ は $a$ の lcm であり、$b$ » は « $m = (a) \cap (b)$ » と同等です。
c) « $p$ は $A$ の既約元である » は、« $(p)$ は $A$ の最大理想値非零である » および « $(p)$ は $A$ の非零主要理想値である » と同等です。

我々はすでに a) (提案 *1*) を証明しました。 $a$ と $b$ の共通の倍数は $(a) \cap (b)$ の元であるため、そして仮定までに理想的な $(a) \cap (b)$ が主、つまり $(a) \cap (b) = (m)$ であるため、$m$ は次の Icm であるということになります。 $a$ と $b$ は b) を証明します。最後に、$p \neq 0$ が $A$ の既約元であると言うことは、定義 (VI, p. *17*) によって、$(p)$ が包含順に並べられた主な理想群 $\neq A$ の $A$ の極大元であることを意味します。 $A$ には主イデア以外のイデアがないので、これは、$(p)$ が VI, p. 17 の注意による、$A$, よって c) の最大イデアルであることを意味します。

主イデアル整域 $A$ では、有限イデアルの数の和 (それぞれ共通部分) は、これらのイデアルの gcd (それぞれ lcm) とも呼ばれます。

#### 命題 3 {#alg-vii-s1-prop-3 .statement tag=0714}

*$a, b, c$ を体の分数の主イデアル整域 $A$ の元とし、$d$ を $a$ と $c$ の gcd とする。この場合、合同式 $ax \equiv b \pmod{c}$ は、$d$ 割る $b$ の場合に限り、解 $x_0 \in A$ になります。この場合、満たす $ax \equiv b \pmod{c}$ は、正確に満たす $x \equiv x_0 \pmod{cd}$* である $A$ の元 $x$ です。

$ax \equiv b \pmod{c}$、$x \in A$ の場合、$b = ax + cy$ となるような $y \in A$ が存在するため、$d$ 割る $b$ となります。逆に、$d$ 割る $b$ の場合、$b = ax_0 + cy_0$ と $x_0, y_0 \in A$ (提案 *1*)、つまり $ax_0 \equiv b \pmod{c}$;さらに、関係 $ax \equiv b \pmod{c}$ は $a(x - x_0) \equiv 0 \pmod{c}$ と等価です。 $a = da'$と$c = dc'$を入れると、後者は$a'(x - x_0) \equiv 0 \pmod{c'}$になります。しかし、$a'$と$c'$は互いに素であるため、これは（$x \in A$の場合）$x - x_0 \equiv 0 \pmod{c'}$と等価です（VI、p. 14、Prop.*10*（DIV）およびVI、p. 15、Cor.2からProp.11まで） (DIV))。

#### 命題 4 {#alg-vii-s1-prop-4 .statement tag=0715}

*$(a_i)$, $i \leq n$ を、主イデアル整域 $A$ の対の互いに素な元の有限族とする。すると、$A / \left( \prod_{r=1}^n a_r \right)$ から積 $\prod_{r=1}^n A/(a_r)$ への標準準同型 (I, p. 110) は、$A$-代数の同型になります。

これは、I、p. 110、提案 9、および提案 2 *a)* に続きます。

$a_i$ が対で互いに素であると仮定しない場合、提案 4 の結論は無効です (cf. VII、p. 24、提案 9)。

### 3. 分解を主イデアル整域で既約因子に

分解に関するVI、p. *18*の結果を既約元、主イデアル整域に適用します。提案 2 により、$A$ の元 $p \neq 0$ は、環 $A/(p)$ が体 (I, p. *115*, Cor. 1) である場合に限り、つまり合同式 $ax \equiv b \pmod{p}$ が認める場合に限り、既約です。それぞれの $b \in A$ と、$p$ の倍数ではないそれぞれの $a \in A$ の $A$ に解が入ります。

#### 定義 2 {#alg-vii-s1-def-2 .statement tag=0716}

※$A$を整域とします。 $A$の既約元の代表者のうち系は、$A$の既約元の$(p_\alpha)$の家族であり、$A$の各既約元はちょうど1つの$p_\alpha$の仲間です。*

#### 定理 2 {#alg-vii-s1-thm-2 .statement tag=0717}

— $\mathbf{A}$ を主イデアル整域とし、$(p_\alpha)$ を $\mathbf{A}$ の既約元の代表者の系とします。すると、$A$ の体の分数のすべての非零元 $x$ は形で一意に表現できます。

$$
x = u \prod_{\alpha} p_{\alpha}^{n_{\alpha}},
$$

ここで、$u$ は $\mathbf{A}$ の可逆元であり、$n_{\alpha}$ は整数であり、そのほとんどはすべて零です。 $x$ ～ 属する ～ $\mathbf{A}$ については、すべての $n_{\alpha}$ が正であることが必要かつ十分です。

分解についての定理を、既約元 (VI、p. 18、Th. 2) の和として使用します。上記の主張は単なる翻訳です。 $\mathscr{P}^*$ は群で順序付けされた格子であるため、この定理の仮説が実際に満たされていることを確認するには、$\mathbf{A}$ 含む極大元の主イデアルのすべての空でない集合を位数で示すだけで十分です。次の補題からは次のようになります。

#### 補題 1 {#alg-vii-s1-lem-1 .statement tag=0718}

$A$ を環として、$A$ のすべての左イデアルが有限に生成されるようにします。すると、$\mathbf{A}$ の左イデアルのすべての空でない集合 $\Phi$ は、包含順に並べると、極大元になります。

Zorn の補題 (集合理論, III, p. 154, Th. 2) によれば、$\Phi$ が帰納的であることを証明するのに十分です。ここで、$(a_\lambda)$ が $\Phi$ の元の完全順序族である場合、イデア $a_i$ の和集合 $a$ は、$\mathbf{A}$ の左イデアルであるため、生成元 $(a_i)_{1 \leq i \leq n}$ の有限系が認められます。それぞれの $a_i$ 属するから理想 $a_{\lambda_i}$ まで、そして家族 $(a_\lambda)$ は完全に順序付けられているため、$a_i$ は理想 $a_{\lambda_i}$ のすべての属するから最大の 、たとえば $a_1$ になります。次に、$a = a_1$ 属するから $\Phi$ となり、これは確かに帰納的集合になります。

後で、$B$ 含む極大元の理想のすべての空でない集合が得られるように、ネーター 環と呼ばれる環 $B$ を研究します。

#### 注意 {#alg-vii-s1-n3-rem-1 .statement tag=0719}

家族 $(u, (n_\alpha))$ は、$x$ の分解から既約の因子と呼ばれます。言葉の乱用により、公式 (1) は $x$ の分解が既約の因子になるとも言います。 $x = u \prod_{\alpha} p_{\alpha}^{n_{\alpha}}$と$y = v \prod_{\alpha} p_{\alpha}^{m_{\alpha}}$が$x$と$y$の分解を既約因子にすると、$x$から割る$y$に必要十分な条件は、 $n_{\alpha} \leq m_{\alpha}$、すべての$\alpha$;これから公式を導き出します

$$
\gcd(x, y) = \prod_{\alpha} p_{\alpha}^{\inf(n_{\alpha}, m_{\alpha})}
$$
$$
\operatorname{lcm}(x, y) = \prod_{\alpha} p_{\alpha}^{\sup(n_{\alpha}, m_{\alpha})}
$$

性質はThで表されます。 2 は、主イデアル整域よりも一般的な環の類に当てはまります。後でそれらを独自の因数分解ドメインとして研究します。そして、任意の多数の不定数における多項式環と正式な冪系列環が固有の因数分解領域であることがわかります (Comm. Alg., VII, § 3)。

### 4. 有理数の割り算整数

切断 1 で指摘したように、有理数整数の環 $\mathbf{Z}$ は主イデアル整域です。 分数の体は $\mathbf{Q}$ です。 乗法群 $\mathbf{Z}$ の可逆元の $U$ には、元 1 と $-1$ が 2 つあります。有理数数 $> 0$ 含むの群 $Q_+^*$ は、$\mathbf{Q}$ の関連元のそれぞれの類から正確に 1 つの元です。したがって、通常はこれと同一視される $\mathbf{Q}$ の主分数イデアルの乗法群 $\mathscr{P}^* = Q^*/U$ と同型です。特に、体 $\mathbf{Q}$ (環 $\mathbf{Z}$ に関して) で gcd または lcm が使用される場合は常に、これらは元 $\geqslant 0$ であることが理解されます。この規則により、有理数数の族の gcd と lcm について話すことができます。

$\mathbf{Z}$ の既約整数 $> 0$ は、まさに私たちが素数数 (I, p. 50) と呼んだものです (これらのときどきは有理素数数と呼ばれます)。したがって、$\mathbf{Z}$ のすべての既約元は、形 $p$ または $-p$ になります。ここで、$p$ は素数数であり、集合 $P$ は素数数です。 $\mathbf{Z}$の既約元の代表者のうち系。

#### 命題 5 {#alg-vii-s1-prop-5 .statement tag=071A}

— 素数数の集合は無限です。

実際、別個の素数数の任意の有限族 $(p_i)$ ($1 \leq i \leq n$) を考えると、数 $\left( \prod_{i=1}^n p_i \right) + 1$ (つまり $> 1$) の素数因子 $q$ は、そうでない場合、すべての $p_i$ とは別個です。 割る 1 になります。

### 5. 体上の不定数における多項式の割り算

可換体 $K$ 上の 1 つの不確定要素における多項式環 $K[X]$ は主イデアル整域 (IV、p. 11、提案 11)。 その分数の体は、$K$の係数を含む$X$の有理数写像の体$K(X)$です。 次数 0 の多項式の環 $K[X]$ 含む部分環、つまり $K$ で識別される定数の体。 $K^*$ の元は $K$ で反転可能であるため、$K[X]$ でも反転可能です。逆に、公式 $\deg(uv) = \deg(u) + \deg(v)$ は、すべての可逆多項式が次数 0 を持つことを示します。従って、$K[X]$の可逆元の群$U$は、正確に$K^*$です。 従って、2 つの関連多項式は、非零定数因子だけが異なります。特に、関連多項式含むのすべての類は固有のモニック多項式です。 The subgroup of the multiplicative group $K(X)^*$ generated by the monic polynomials thus contains a unique element from each class of associate rational functions, and consequently is isomorphic to the group

$$
\mathscr{P}^* = K(X)^*/U
$$

$K(X)$ の主分数イデアルの。特に、(環 $K[X]$ に関して) 体 $K(X)$ の gcd または lcm が言及されるときは常に、これらはモニック多項式 (または 0) の商であることが理解されます。この規則により、有理数写像の族の gcd または lcm について話すことができます。

The irreducible elements of $K[X]$ are precisely the irreducible polynomials in the usual sense (IV, p. 13, Def. 2), and the set of monic irreducible polynomials is a system of representatives of irreducible elements of $K[X]$.

最初の次数多項式は常に既約です。 $K$ が代数閉体の場合、逆は真になります (V、p. 19、提案 1)。従って、この場合、$K[X]$ の次数 $n$ のすべての多項式 $p(X)$ は、形で一意に書くことができます (因子の位数まで)。

$$
p(X) = c(X - a_1)(X - a_2) \ldots (X - a_n)
$$

ここで、$c$ と $a_i$ は $K$ の元です。

#### 命題 6 {#alg-vii-s1-prop-6 .statement tag=071B}

任意の体 $K$ について、$K[X]$ のモニック既約多項式の *集合* は無限大です。

実際、別個のモニック既約多項式の任意の空でない有限族 $(p_i)$ ($1 \leq i \leq n$) が与えられると、多項式 $\left( \prod_{i=1}^n p_i \right) + 1$ は可逆ではなく、この多項式の任意のモニック既約因子 $q$ は必然的にすべてのモニック既約多項式とは異なります。 $p_i$、それ以外の場合は割る 1 になります。

### 練習問題 {#alg-vii-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
