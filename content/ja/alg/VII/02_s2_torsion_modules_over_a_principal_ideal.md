---
book: alg
book_title: Algebra
chapter: VII
chapter_title: MODULES OVER PRINCIPAL IDEAL DOMAINS
section: 2
section_title: Torsion modules over a principal ideal domain
lang: ja
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A VII.6-A VII.14, A VII.54-A VII.59
pdf_pages: 0365-0373, 0413-0418
extraction: ocr
subsections:
    - "no": 1
      title: Modules over a product of rings
      page: 6
      pdf_page: 365
    - "no": 2
      title: Canonical decomposition of a torsion module over a principal ideal domain
      page: 7
      pdf_page: 366
    - "no": 3
      title: 'Applications : I. Canonical decompositions of rational numbers and of rational functions in one indeterminate'
      page: 10
      pdf_page: 369
    - "no": 4
      title: 'Applications : II. The multiplicative group of units of the integers modulo a'
      page: 12
      pdf_page: 371
statements: 22
exercises: 15
content_sha256: 617c3619ab884e3beafbd3f0758fad6625755761d2a66cb5aa1a3ee93cb1138d
translated_from: content/en/alg/VII/02_s2_torsion_modules_over_a_principal_ideal.md
translation_method: google
source_content_sha256: 798b6543b06067240b5dab1244bfefa178a908e9f4cf2fdc3e29b8faab35c2bc
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: c1b62c226e6da33c4011f6bfd886dac80311c6087d146f41c0a2fa6d263f3f65
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 2。 捩れ加群主イデアル整域

### 1. 環の積を超える加群

Let $A$ be a ring and $(b_i)_{i \in I}$ a direct decomposition of $A$, that is (I, p. 110, Def. 7) a finite family of two-sided ideals of $A$ such that the natural homomorphism from $A$ into the product of the $A/b_i$ is bijective. *locより。前掲*、提案 10 では、$i \neq j$ に対して $b_i = A(1 - e_i)$、$\sum_{i \in I} e_i = 1$、$e_i e_j = 0$ など、$A$ の中心冪等の族 $(e_i)_{i \in I}$ が存在します。

左のすべての $A$ モジュール $M$ について、$M_i$ が $b_i m = 0$ となるような $m \in M$ の集合を表すものとします。 $b_i$ は両面理想なので、これは $M$ の部分加群です。さらに、$a, b \in A$ と $a - b \in b_i$ の場合、相似関係は $a_{M_i}$ と $b_{M_i}$ 一致するになります。したがって、$M_i$ には独特の $(A/b_i)$ モジュール構造があり、$M_i$ の $A$ モジュール構造は準同型 $A \to A/b_i$ を介して誘導されます。

#### 命題 1 {#alg-vii-s2-prop-1 .statement tag=0724}

$A$ モジュール $M$ は、その部分加群 $M_i$ の直和です。

$p_i : M \to M$ をホモテティー $m \mapsto e_i m$ とします。 写像 $p_i$ は、$e_i$ が中心であるため、$A$ は線形です。 $i \neq j$ の $e_i^2 = e_i$、$\sum_{i \in I} e_i = 1$、$e_i e_j = 0$ から、

$$
p_i \circ p_i = p_i , \quad \sum_{i \in I} p_i = 1_M , \quad p_i \circ p_j = 0 \quad \text{for} \quad i \neq j ,
$$

そして、$p_i$ 形は、和が恒等である射影子の直交族です (II、p. 209、定義 7)。 *locより。前掲*、提案 12、加群 M は部分加群 $p_i(M) = e_iM$ の直和です。 加法では、$e_iM$ は $b_i = A(1 - e_i)$ によって全滅します。 $i \neq j$と$m \in M$の場合、$(1 - e_i)e_jm = e_jm$、よって、$e_jM$の非零元は$1 - e_i$によって全滅するため、$b_i$によってなおさらが消滅します。したがって、$e_iM = M_i$、命題が証明されます。

#### 注意 1 {#alg-vii-s2-n1-rem-1 .statement tag=0725}

逆に、$M'_i$ を各 i の $(A/b_i)$ 加群とし、A-加群 $M'_i$ の A-加群 M、直和を考えます。次に、$M'_i$ を使用して一致するの上に部分加群 $M_i$ が構築されます ($i \neq j$ の場合、$b_i + b_j = A$ により $M'_j$ の非零元が$b_i$ によって消滅されないことに注意するだけで十分です)。したがって、大まかに言えば、A-加群 M または環 $A/b_i = A_i$ よりも加群の家族 $(M_i)$ を考慮することは同じことになります。

#### 注意 2 {#alg-vii-s2-n1-rem-2 .statement tag=0726}

上記により、M の成分 $M_i$ に対する M の証明、射影子は相似関係になります。

#### 注意 3 {#alg-vii-s2-n1-rem-3 .statement tag=0727}

A-加群 M は、それぞれの $M_i$ が環状である場合にのみ環状です。$M = Am$ の場合、$M_i = A_i e_i m$ です。逆に、$M_i = A_i m_i$ と $m = \sum_{i \in I} m_i$ の場合は、$M = Am$ です。実際、$n \in M$ が各 i について $a_i m_i$ に射影され、$a \in A$ が各 i について $a_i$ mod $b_i$ に合同である場合、am と n はそれぞれの $M_i$ で同じ像を持ち、したがって一致するになります。

#### 注意 4 {#alg-vii-s2-n1-rem-4 .statement tag=0728}

M と N を 2 つの A-加群とし、成分 $(M_i)$ と $(N_i)$ とします。 $u \in \mathrm{Hom}_A(M, N)$ を M から N までの A 線形写像とします。次に、すべての i とすべての $m \in M_i$ について、$u(m) \in N_i$ があるため、誘導するは $A_i$ 線形写像 $u_i \in \mathrm{Hom}_{A_i}(M_i, N_i)$ になります。 写像 $u \mapsto (u_i)$ が Z モジュールの同型 (A が可換である場合、それぞれ A-加群) であることを確認するのは簡単です。

$$
\mathrm{Hom}_A(M, N) \to \prod_{i \in I} \mathrm{Hom}_{A_i}(M_i, N_i).
$$

### 2. 主イデアル整域上の捩れ加群の正規分解

M を可換環 A 以上の加群とします。それぞれの $a \in A$ について、$M(\alpha)$ は M の自己準同型 $x \mapsto \alpha x$ の核を表します。$a$ と $\beta$ が A の 2 つの元である場合、次のようになります。 $\alpha$ 割る $\beta$、そして明らかに$M(a) \subset M(\beta)$。特に、n は有理数整数 $\geq 1$, 部分加群 $M(\alpha^n)$ 形増加する数列の集合を通過します。したがって、$M(\alpha^n)$ のうちの和集合 $M$ は、M の部分加群であり、M の元のうちのからなるは、a の冪によって消滅されます。 M の各部分加群 N について、$N_1 = N \cap M_a$ であることは明らかです。

#### 定義 1 {#alg-vii-s2-def-1 .statement tag=0729}

$\pi$ を主イデアル整域 A の既約元とします。 A-加群 M は rr-primary *if* と呼ばれ、すべての $x \in M$ に対して、$\pi^n x = 0$ となるような整数 $n \geq 1$ が存在します (他の語では、M が部分加群 $M_\pi$ に等しい場合)。

明らかに、形 $A/(\pi^s)$ のすべての循環加群は rr-primary です。任意の A-加群 M の場合、部分加群 $M_\pi$ が rr-primary です。

#### 補題 1 {#alg-vii-s2-lem-1 .statement tag=072A}

M を主イデアル整域 A よりも加群とします。 $a \neq 0$ のようなすべての $a \in A$ について、$\alpha = \varepsilon \sum_{i=1}^r \pi_i^{n(i)}$ を $\alpha$ の分解として既約因子 (VII, p. 4) にします。 a によって消滅した M の要素のサブモジュール $N = M(a)$ は、サブモジュール $M(\pi_i^{n(i)})$ の直接和であり、各 $x \in M(\alpha)$ を $M(\pi_i^{n(i)})$ のコンポーネントに送信するマップは、形式 $x \mapsto \gamma_i x \ (\gamma_i \in A)$ になります。 さらに
$$
M(\pi_i^{n(i)}) = N \cap M_{\pi_i} = N_{\pi_i}
$$
注意まず、N は a によって消滅するので、自然な $A/(\alpha)$ モジュール構造になります。 VII、p. 3、標準準同型の提案 4 により、$A/(\alpha)$ から環 $A/(\pi_i^{n(i)})$ の積は環同型になります。今、適用 VII、p. 6 の提案 1 より、N は $M(\pi_i^{n(i)})$ の直和であると推測します。この分解のうち射影子は、VII、p. 7、注意 2 によって相同です。 $M(\pi_i^{n(i)}) \subset M(\alpha) \cap M_{\pi_i}$ が含まれていることは明らかです。逆に、$x \in M(\alpha) \cap M_{\pi_i}$ とします。 次に、x を消滅させる $\pi_i$ の冪 $\pi_i^s$ が存在します。 $s \geq n(i)$ と仮定します。 Bezout のアイデンティティによれば、$\pi_i^{n(i)} = \lambda \pi_i^s + pa$ のような $\lambda, \mu \in A$ が存在し、したがって $\pi_i^{n(i)} x = 0$ が存在し、最終的に $x \in M(\pi_i^{n(i)})$ になります。

#### 補題 2 {#alg-vii-s2-lem-2 .statement tag=072B}

M を整域 A に対して捩れ加群 (II, p. 313) とします。 M の元のすべての有限族 $(x_i)_{1 \leq i \leq n}$ に対して、A には元 $\gamma \neq 0$ が存在し、$x_i$ はすべて属するから $M(\gamma)$ になります。
実際、各添字 i に対して、A には $x_i$ を全滅させる元 $\alpha_i \neq 0$ が存在し、元 $\gamma = \prod_{i=1}^n \alpha_i$ がその要件に適合します。

#### 定理 1 {#alg-vii-s2-thm-1 .statement tag=072C}

M を主イデアル整域 A よりも捩れ加群とします。 A の各既約元 $\pi$ について、$M_\pi$ を M の部分加群元のからなるが $\pi$ の冪によって全滅するとします。 P が A の既約元の代表の系である場合、M は $\pi \in P$ の部分加群 $M_\pi$ の直和です。
$a \neq 0$ については元 $x \in M$ 属するから部分加群 $M(\alpha)$ ごとに、補題までに 1 は元の有限数の和となり、それぞれ属するは次のようになります。 部分加群 $M_\pi$ もいます。 一方、$\sum_{\pi \in P} x_\pi = \sum_{\pi \in P} y_\pi$ (すべての $\pi \in P$ が $x_\pi, y_\pi \in M_\pi$ であり、有限多数の $x_\pi$ と $y_\pi$ を除くすべてが 0) の場合、補助定理 2 は、A に $\gamma \neq 0$ が存在し、すべての $x_\pi$ と $y_\pi$ が同じサブモジュールに属することを示します。 $M(\gamma)$;補助定理 1 を $M(\gamma)$ に適用すると、すべての $\pi \in P$ に対して $x_\pi = y_\pi$ が得られ、証明が完了します。

明らかに、$\pi$ と $\pi'$ が 2 つ既約元に関連する場合、$M_\pi = M_{\pi'}$ になります。したがって、与えられた加群 M に対して、部分加群 $M_\pi$ は A の理想的な $(\pi)$ にのみ依存します。それは、加群 M の rr プライマリ成分と呼ばれ、$M_\pi$ の直和としての M の分解は、その rr プライマリ成分の直和としての M の標準分解と呼ばれます。

#### 系 1 {#alg-vii-s2-thm-1-cor-1 .statement tag=072D}

— *捩れ加群 M の各部分加群 N は、その部分加群 N ∩ M* の直和です。

これは、N ∩ M, が N の π 一次的 成分 N, であるという事実から導き出されます。

#### 系 2 {#alg-vii-s2-thm-1-cor-2 .statement tag=072E}

— *捩れ A-加群 M の *部分加群 N は、A* の既約元 π ごとに、N が M の直因子である場合にのみ、直因子です。

実際、N と N' が M の 2 つの部分加群である場合、$\mathscr{A}$ のすべての既約元 π について M, − N, ⊕ N'_π である場合に限り、M = N ⊕ N' になります (Cor. 1)。

#### 系 3 {#alg-vii-s2-thm-1-cor-3 .statement tag=072F}

— *N を捩れ A-加群 M の部分加群とします。A の既約元 π ごとに、N = 0 または $(M/N)_\pi = 0$ の場合、N は M* の直因子です。

実際、条件 $(M/N)_\pi = 0$ は $N_\pi = M_\pi$ と Cor を意味します。 2が該当します。

M のすべての部分加群が直因子 (cf. A, VIII, § 3) である場合、A-加群 M は *半単純* と呼ばれます。

#### 系 4 {#alg-vii-s2-thm-1-cor-4 .statement tag=072G}

— *A を体ではない主イデアル整域とし、M を A-加群とします。この場合、M が捩れ加群であり、A* のすべての既約元 π に対して M, = M(π) である場合に限り、M は半単純になります。

まず、M が半単純であると仮定します。 x ∈ M とし、π を $\mathscr{A}$ の既約元とします。 N が M の $Annx$ の補数である場合、$\alpha \in \mathscr{A}$ と $y \in N$ を使用して $x = \alpha \pi x + y$ と書くことができます。しかし、それは $y = (1 - \alpha n)x$ を意味するので、
$$
\pi(1 - \alpha \pi)x \in A\pi x \cap N = 0 .
$$
まず第一に、M は捩れ加群であることがわかります。さらに$x \in M_\pi$なら$\pi(1 - \alpha \pi)x = 0$、したがって$\pi x = \alpha \pi^2 x = \alpha^2 \pi^3 x = \cdots = \alpha^n \pi^{n+1} x$は零と$M_\pi = M(\pi)$になります。

逆に、Cor. 2 既約元 π によって消滅した A-加群 M が半単純であることを証明すれば十分です。しかし、それは明らかです。なぜなら、M は体 $\mathscr{A}/(\pi)$ の上にベクトル空間の自然な構造を持ち、M の部分加群はこの構造の下で正確にベクトル部分空間であるからです。

#### 注意 1 {#alg-vii-s2-n2-rem-1 .statement tag=072H}

— 明らかに、τ 加群のすべての元 ≠ 0 の消滅子は、τ の主イデアル含む冪であるため、形 $A\pi^k$ (k > 0 整数) を持ちます。 x を M の元とします。それぞれの $\pi \in P$ について、$x_\pi$ を $M_\pi$ の x の成分とします。 x の消滅子は、非零 $x_\pi$ の消滅子の lcm ですが、上記により、この場合、非零 $x_\pi$ の消滅子の *積* と等しくなります (VI, p. 16, Prop. 12(DIV))。

#### 命題 2 {#alg-vii-s2-prop-2 .statement tag=072I}

— *M が主イデアル整域 A 上で有限生成された捩れ加群である場合、M の n 主要成分は、そのうちの有限数を除いて零であり、これらの成分 $M_\pi$ に対する M の射影子は相似関係* です。

これは、補題 1 からすぐに続きます。なぜなら、補題 2 までに、$M = M(\alpha)$ となるような $\mathscr{A}$ に $\alpha \neq 0$ が存在するからです。

#### 注意 2 {#alg-vii-s2-n2-rem-2 .statement tag=072J}

— VII、p. 7、注意 3 により、有限に生成された捩れ A-加群は、その π 原始成分のそれぞれが巡回である場合に限り、巡回です。

重要な特殊なケースとして、Th. 1 と提案 2 が適用されるのは $A = \mathbf{Z}$ の場合です。 $\mathbf{Z}$-モジュールは単なる *アーベル群* です。 アーベル群は、捩れ $\mathbf{Z}$ モジュールである場合、つまりすべての元が *有限位数* を持つ場合、*捩れ群* と呼ばれます。次に、$P$ は素数数 $> 0$ の集合とみなされます。各素数数 $p > 0$ について、そのすべての元が $p$ の冪である位数を持つ場合、(アーベル) 群は $p$-ねじれであると言われます。この用語では、Th. 1 は、*各捩れアーベル群が p ねじれ群* の直和であることを示しています。 有限群の場合は、I、p. 80、Thからも続きます。 4.

### 3. アプリケーション: I。有理数数と有理数写像の正規分解を 1 つの不定数で表現

#### 定理 2 {#alg-vii-s2-thm-2 .statement tag=072K}

*$A$を主イデアル整域、$K$をその体の派生、$P$を$A$の既約元の代表の系とします。 元 $x \in K$ が与えられると、$A$ ($p \in H$) には $P$、元 $a_0 \in A$、$a, \in A$ が$p$ で割り切れない有限部分集合 $H$ が存在します。 整数 $s(p) > 0$ ($p \in H$) そのような*

$$
x = a_0 + \sum_{p \in H} a_p p^{-s(p)},
$$

*ここで、$H$ と $s(p)$ はこれらの条件によって一意に決定されます。

*さらに、$R_p$ が、$A (p \in P)$ の各剰余クラス mod $p$ の要素を 1 つだけ含む $A$ のサブセットを表す場合、各 $x \in K$ は次の形式で一意に表現できます*

$$
x = a + \sum_{p \in P} \left( \sum_{h=1}^{\infty} r_{ph} p^{-h} \right)
$$

*ここで、$h$ と $p$ はすべて $a \in A$ と $r_{ph} \in R_p$ であり、限られた多くの $r_{ph}$ はすべて零です。*

$K$ を $A$ モジュールとして考えてください。すると、$A$ は 1 によって生成された部分加群になります。 商加群 $K/A$ は、同値関係 $x' - x \in A$ によって$K$ の商になります。これは、VI、p. 6 の記法にも次のように書かれます。 $x \equiv x'$ (mod 1); $f$ は、$K$ から $M = K/A$ までの自然な準同型を表します。

商加群 $M$ は *捩れ加群* で、$M$ のすべての元には形 $f(a/b)$ ($a \in A, b \in A, b \neq 0$)、よって $b f(a/b) = f(a) = 0$ があります。したがって、Th。 VII、p. 8のいずれかが該当します。 $M_p$ ($p \in P$) を、$M$ の元の部分加群が $p$ の冪によって全滅するとします。すると、$f^{-1}(M_p)$は部分環、形の$K$、$a p^{-n}$の元の$A_p$で、$a \in A$と$n \geq 0$は整数です。 加群 $M$ は $M_p$ の直和であるため、すべての $x \in K$ は $A_p$ の和の元に一致する mod 1 です。他の語、公式 (1) は、$s(p)$ 整数 $> 0$、および $a$ で、$a$ は倍数ではない、$A$ の有限多数の元が成り立ちます。 $p$。

$s(p)$ と $a$ ではこれらの条件が、完全に決定する $H$ と $s(p)$ であることがわかります。実際、$H$ は $p \in P$ の集合となり、$M_p$ の $f(x)$ の成分は $\neq 0$ になります。一方、$s$ と $s'$ が s \geq s' となる 2 つの整数 $> 0$ であり、$a$ と $a'$ が $p$ で割り切れない $A$ の元である場合、次のようになります。 $ap^{-s} \equiv a'p^{-s'} \pmod{1}$ であれば、$a \equiv a'p^{s-s'} \pmod{p^s}$ と推測します。 $s > s'$ なら $a \equiv 0 \pmod{p}$ となり、仮説に反します。この議論は、各 $a_i$ が明確に定義された mod $p^{s(p)}$ であることも示しています。

証明を完了するには、まず、$A$ の各剰余類 mod $p^i$ に、$0 \leq h \leq s-1$ の $r_h \in R_p$ を含む形 $\sum_{h=0}^{s-1} r_h p^h$ の一意元が存在することに注意します。実際、$s$ で帰納法まで進みます ($R_p$ の定義から $s = 1$ に続き、性質が続きます) : let $x \in A$; 仮定により、$x$ mod $p^{s-1}$ の剰余類には形 $\sum_{h=0}^{s-2} r_h p^h$ ($r_h \in R_p$) の一意元があります。その場合、$x - \sum_{h=0}^{s-2} r_h p^h$ は $p^{s-1}$ の倍数 $ap^{s-1}$ です。現在、$a \equiv r_s \pmod{p}$ のような $R_p$ のうち、一意元 $r_s$ が存在します。 よって $x \equiv \sum_{h=0}^{s-1} r_h p^h \pmod{p^s}$。 公式 (2) を取得するには、この事実を公式 (1) の各 $a_p$ に適用するだけで十分です。上記を考慮すると、一意性は明らかです。

以下は Th の最も重要なアプリケーションです。 2：

I。 *環 A は有理数整数の環 Z であり、K = Q* です。 P を素数数 > 0 の集合とし、各 $p \in P$ について $R_p$ を $\mathbf{Z}$ の区間 $(0, p-1)$ とします。したがって、正規の分解が得られます。

$$
x = a + \sum_{p \in P} \left( \sum_{h=1}^{\infty} e_{ph} p^{-h} \right)
$$

$a \in \mathbf{Z}$、$e_{ph} \in \mathbf{Z}$、$0 \leq e_{ph} \leq p-1$と。

II。 *環 A は、可換体 E 上の 1 つの不定多項式の環 E[X]、および K = E(X)* です。 P を $E[X]$ (VII, p. 5) のモニック既約多項式の集合とします。 $p \in P$ の場合、多項式 (IV、p. 10) のユークリッドの除算により、$R_p$ を次数の多項式の集合が $p$ の多項式よりも厳密に小さいとみなすことができます。したがって、有理数写像 $r(X) \in E(X)$ の分解 (正規と呼ばれます) が得られます。

$$
r(X) = a(X) + \sum_{p \in P} \left( \sum_{h=1}^{\infty} v_{ph}(X) \cdot p(X)^{-h} \right)
$$

ここで、$a(X)$ は多項式、$v_{ph}(X)$ は、すべての $p$ と $h$ について、厳密に $p(X)$ よりも小さい次数の多項式です。特に、体 E が *代数的に閉じている*場合、$p(X)$ は $a \in E$ とともに形 $X - a$ を持ち、したがって $v_{ph}(X)$ は定数になります。

したがって、体 E 上のベクトル空間 $E(X)$ には、単項式 $X^n$ ($n \geq 0$ 整数) の基底からなると形の有理数写像があると言えます。 $X^m / (p(X))^h$、ここで、$p \in P$、$h$、および$m$は、$h \geq 1$と$0 \leq rn < \deg(p)$を含む整数です。

### 4. アプリケーション: II。 整数の単位元の乗法群を法 a

a を有理数整数 > 1 とし、$(\mathbf{Z}/a\mathbf{Z})^*$ を環 $\mathbf{Z}/a\mathbf{Z}$ の可逆元の乗法群とします。 $a = \prod p_i^{n(i)}$ が a の分解を素数因子に変換したものである場合、環 $\mathbf{Z}/a\mathbf{Z}$ は環 $\mathbf{Z}/p_i^{n(i)}\mathbf{Z}$ の積と同型です (VII, p. 3、提案 4)。 群 $(\mathbf{Z}/a\mathbf{Z})^*$ は、群 $(\mathbf{Z}/p_i^{n(i)}\mathbf{Z})^*$ の積と同型です。したがって、私たちは群 $(\mathbf{Z}/p^n\mathbf{Z})^*$ の研究に帰着します。ここで、p は素数数です。 (V、p. 80) $(\mathbf{Z}/p^n\mathbf{Z})^*$ の位数 $\varphi(p^n)$ が $p^n - p^{n-1} = p^{n-1}(p-1)$ であることを思い出してください。

まず、$p > 2$; と仮定します。 $(\mathbf{Z}/p^n\mathbf{Z})^*$から$(\mathbf{Z}/p\mathbf{Z})^*$までの群の自然な準同型$\mathbf{Z}/p^n\mathbf{Z} \to \mathbf{Z}/p\mathbf{Z}$制限するから準同型、その核をU$(p^n)$と表します。 by VII, p. 3, 提案 3 剰余類 mod $p^n$ of 整数 m は、m が p と互いに素である場合にのみ、つまり $m$ mod の剰余類である場合に限り、可逆です$p$ は反転可能です。 U$(p^n)$ は 1 mod p に合同な整数のすべての剰余類 mod $p^n$ から成り、$p^{n-1}$ 元もあり、完全系列があるということになります。

(3)
$$
\{1\} \to \mathrm{U}(p^n) \to (\mathbf{Z}/p^n\mathbf{Z})^* \to (\mathbf{Z}/p\mathbf{Z})^* \to \{1\}.
$$

同様に、$n \geq 2$ について、U$(2^n)$ が $(\mathbf{Z}/2^n\mathbf{Z})^*$ から $(\mathbf{Z}/4\mathbf{Z})^*$ までの自然準同型写像のカーネルを表すものとします。これは次数 $2^{n-2}$ のグループで、1 mod 4 に合同な整数のすべての剰余クラス mod $2^n$ で構成されており、正確な配列が存在します。

(4)
$$
\{1\} \to \mathrm{U}(2^n) \to (\mathbf{Z}/2^n\mathbf{Z})^* \to (\mathbf{Z}/4\mathbf{Z})^* \to \{1\}.
$$

#### 補題 3 {#alg-vii-s2-lem-3 .statement tag=072L}

x、y、k を $k \geq 0$ を伴う整数とし、$p > 2$ を素数数とします。 $x \equiv 1 + py \mod p^2$なら$x^{p^k} \equiv 1 + p^{k+1}y \mod p^{k+2}$。 ** $x \equiv 1 + 4y \mod 8$ の場合は $x^{2^k} \equiv 1 + 2^{k+2}y \mod 2^{k+3}$。

最初の主張を証明するには、$k \geq 1$と$x \equiv 1 + p^ky \mod p^{k+1}$なら$x^p \equiv 1 + p^{k+1}y \mod p^{k+2}$であることを示し、整数kについて帰納法によって議論するだけで十分です。すべての $a \in \mathbf{Z}$ と $k \geq 1$ では、明らかになります。
$$
(1 + p^ka)^p \equiv 1 + p^{k+1}a \mod p^{k+2},
$$
したがって
$$
(1 + p^ky + p^{k+1}z)^p = (1 + p^k(y + pz))^p \equiv \\
= 1 + p^{k+1}(y + pz) \equiv 1 + p^{k+1}y \mod p^{k+2}.
$$
同様に、$k \geq 1$ については、
$$
(1 + 2^{k+1}a)^2 \equiv 1 + 2^{k+2}a \mod 2^{k+3},
$$
それで
$$
(1 + 2^{k+1}y + 2^{k+2}z)^2 \equiv 1 + 2^{k+2}y \mod 2^{k+3},
$$
よって 2 番目の主張 by 帰納法 k 上。

#### 命題 3 {#alg-vii-s2-prop-3 .statement tag=072M}

$p > 2$ を素数、$n > 0$ を整数とします。その場合、群 $U(p^n)$ は次数 $p^{n-1}$ の巡回です。 $n \geq 2$ の場合、1 mod $p$ に合同な整数 $x$ の剰余クラス mod $p^n$ は、$x$ が 1 mod $p^2$ に合同でない場合に限り、$U(p^n)$ の生成関数になります。 $m > 1$ を整数とします。その場合、群 $U(2^m)$ は位数 $2^{m-2}$ の巡回です。 $m \geq 3$ の場合、剰余類 mod $2^m$ of 整数 $x$ が 1 mod 4 に合同である場合、$x$ が 1 mod 8 に合同でない場合に限り、$U(2^m)$ の生成元となります。

$U(p^n)$ の次数は $p^{n-1}$ であるため、$U(p^n)$ のすべての要素 $u$ の次数は $p$ のべき乗であり、$u^{p^{n-2}} \neq 1$ の場合にのみ、$u$ は $U(p^n)$ の生成子になります。 ここで、$u$ が $x = 1 + py$ の類である場合、$y \not\equiv 0 \mod p$ の場合に限り、補題 3、よって $u$ 生成する $U(p^n)$ により、$u^{p^{n-2}}$ は $1 + p^{n-1}y$ の類になります。その他の語 $x \not\equiv 1 \mod p^2$。 たとえば、類 $1 + p$ 生成する $U(p^n)$ です。 同様に、$x$ mod $2^n$ 生成する $U(2^n)$ の類 $u$ は、$u^{2^{n-3}} \neq 1$ の場合に限ります。これは、$x$ が 1 mod 8 に補題 3 により合同ではないことを意味します。これは$x = 5$によって満たされます。

#### 補題 4 {#alg-vii-s2-lem-4 .statement tag=072N}

$A$ を主イデアル整域とし、$0 \to N \to M \to P \to 0$ を $A$ モジュールの完全系列とします。 $aN = 0$ と $bP = 0$ となるような互いに素な元 $a, b \in A$ が存在するとします。それから完全系列分裂。 加法で $N$ と $P$ が両方とも循環的である場合、$M$ は循環的です。

加群 $M$ は、$abM = 0$ なので、捩れです。最初の主張は Cor から続きます。 VII、p. 9の3つ。 $N$ と $P$ が循環的である場合、それらは有限に生成されるため、$M$ (II、p. 17、Cor. 5) も同様です。 $M$ の各 $p$-プライマリー 成分は、$N$ または $P$ のいずれかの $p$-プライマリー 成分と同型であるため、VII、p. 10 の注意 2 から次のようになります。 $M$ は周期的です。

#### 定理 3 {#alg-vii-s2-thm-3 .statement tag=072O}

$a = \prod p_i^{n(i)}$ が整数 $a > 1$ の素数分解である場合、環 $\mathbf{Z}/a\mathbf{Z}$ の可逆元の群 $(\mathbf{Z}/a\mathbf{Z})^*$ は群 $(\mathbf{Z}/p_i^{n(i)}\mathbf{Z})^*$ の積と同型です。 $p > 2$ が素数数および $n \geq 1$ 整数である場合、群 $(\mathbf{Z}/p^n\mathbf{Z})^*$ は位数 $p^n \ ^1(p - 1)$ の巡回です。 グループ $(\mathbf{Z}/2\mathbf{Z})^*$ は自明です。 $n \geq 2$ の場合、群 $(\mathbf{Z}/2^n\mathbf{Z})^*$ は、5 mod $2^n$ の剰余クラスによって生成される次数 $2^n \ ^2$ の環状群と、1 および $-1$ mod $2^n$ の剰余クラスからなる次数 2 の環状群の直接積です。

$U(p^n)$ の位数 $p^n \ ^1$ と $(\mathbf{Z}/p\mathbf{Z})^*$ の $p - 1$ は互いに素です。 $U(p^n)$ と $(\mathbf{Z}/p\mathbf{Z})^*$ は循環的であるため (提案 3 と V、p. 78、補題 1)、群 $(\mathbf{Z}/p^n\mathbf{Z})^*$ は循​​環的です (補題 4 を完全系列 (3) に適用します)。 $n \geq 2$ の場合、準同型 $v : (\mathbf{Z}/2^n\mathbf{Z})^* \to (\mathbf{Z}/4\mathbf{Z})^*$ から部分群 $(1, -1)$ の制限は全単射です。したがって、群 $(\mathbf{Z}/2^n\mathbf{Z})^*$ は、この部分群の直接の積と $v$ の核 $U(2^n)$ です。結果は提案 3 から導き出されます。

#### 注意 {#alg-vii-s2-n4-rem-1 .statement tag=072P}

$p > 2$ を素数数とし、$x$ を 1 mod $p$ に合同で 1 mod $p^2$ には合同ではない整数とする。 完全系列があります

$$
\{0\} \to \mathbf{Z}/p^n \ ^1\mathbf{Z} \xrightarrow{u} (\mathbf{Z}/p^n\mathbf{Z})^* \xrightarrow{\nu} (\mathbf{Z}/p\mathbf{Z})^* \to \{1\}
$$

群の場合、$v$ は自然な射影で、$u$ は写像 $r \mapsto x^r$ によって商に誘導されます。 $\mathbf{Z}_p$ を $p$ 進数整数 ($V$、p. 96) の環とし、$x$ を $x - 1 \in p\mathbf{Z}_p$ と $x - 1 \notin p^2\mathbf{Z}_p$ となるように $\mathbf{Z}_p$ の元とします。 移行を反転して極限、完全系列 (5) 誘導する完全系列

$$
\{0\} \to \mathbf{Z}_p \xrightarrow{u} \mathbf{Z}_p^* \xrightarrow{v} (\mathbf{Z}/p\mathbf{Z})^* \to \{1\}
$$

ここで、$v$ は自然な写像と連続的な写像 $u$ 拡大する写像 $n \mapsto x^n$ ($n \in \mathbf{Z}$) です。 $n \in \mathbf{Z}_p$の代わりに$x^n = u(x)$を入れることがよくあります。

同様に、$x \in \mathbf{Z}_2$ と $x - 1 \in 4\mathbf{Z}$ および $x - 1 \notin 8\mathbf{Z}_2$ の場合、分裂完全列になります。

$$
\{0\} \to \mathbf{Z}_2 \xrightarrow{u} \mathbf{Z}_2^* \xrightarrow{v} (\mathbf{Z}/4\mathbf{Z})^* \to \{1\}.
$$

ここで、$u$ は写像 $n \mapsto x^n$ の連続する拡大です。

### 練習問題 {#alg-vii-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
