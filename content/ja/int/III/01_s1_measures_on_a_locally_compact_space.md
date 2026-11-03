---
book: int
book_title: Integration
chapter: III
chapter_title: MEASURES ON LOCALLY COMPACT SPACES
section: 1
section_title: Measures on a locally compact space
lang: ja
source: int-i-vi
pdf_pages: 0046-0068, 0100-0104
extraction: ocr
subsections:
    - "no": 1
      title: Continuous functions with compact support
      page: 0
      pdf_page: 46
    - "no": 2
      title: Approximation properties
      page: 4
      pdf_page: 49
    - "no": 3
      title: Definition of a measure
      page: 7
      pdf_page: 52
    - "no": 4
      title: Product of a measure by a continuous function
      page: 10
      pdf_page: 55
    - "no": 5
      title: Real measures. Positive measures
      page: 11
      pdf_page: 56
    - "no": 6
      title: Absolute value of a complex measure
      page: 13
      pdf_page: 58
    - "no": 7
      title: Definition of a measure by extension
      page: 15
      pdf_page: 60
    - "no": 8
      title: Bounded measures
      page: 16
      pdf_page: 61
    - "no": 9
      title: Vague topology on the space of measures
      page: 18
      pdf_page: 63
    - "no": 10
      title: Compact convergence in $\mathscr{M}(X; \mathbf{C})$
      page: 21
      pdf_page: 66
statements: 41
exercises: 18
content_sha256: a59d0786dfe655562095940003194cb630e36bad698dd40c2adf0f6eb99e568c
translated_from: content/en/int/III/01_s1_measures_on_a_locally_compact_space.md
translation_method: google
source_content_sha256: a5649ad91c991534fecdc842feb81de5c325d32e755f63251c2a1e0724811493
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 18c0ce06b002517c46d49ad6ea9775d3b977d054d03e14c9f906f8796bfa860c
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 1。局所コンパクト化対策空間

### 1. コンパクトなサポートで連続写像

#### 定義 1 {#int-iii-s1-def-1 .statement tag=08L4}

— X をトポロジー 空間とし、E を $\mathbf{R}$ 上の $\overline{\mathbf{R}}$ またはベクトル空間とし、f を E への X の写像とする。 $X - S$ で $f(x) = 0$ となるように X で閉じた最小の集合 S (他の語では、$f(x) \neq 0$ のようなすべての $x \in X$ の集合の X での閉包) は f のサポートと呼ばれ、Supp(f) と表されます。

X を局所的にコンパクトな空間とし、E を $\mathbf{R}$ または $\mathbf{C}$ 上のトポロジカルベクトル空間とします。 $\mathscr{C}(X;E)$ は、E への X の連続写像のベクトル空間を表すことを思い出してください。 $E = \mathbf{R}$ または $E = \mathbf{C}$ の場合、混乱が生じない限り、この記法での E の言及は省略します。 コンパクトなサポートを備えた連続マッピングによって形成された $\mathscr{C}(X;E)$ の部分空間を $\mathscr{K}(X;E)$ で表すことにします。 X のすべての部分集合 A について、$\operatorname{Supp}(f) \subset A$ のような写像 f によって形成される $\mathscr{C}(X;E)$ (それぞれ $\mathscr{K}(X;E)$) の部分空間を $\mathscr{C}(X,A;E)$ (それぞれ $\mathscr{K}(X,A;E)$) で表します。 $E = \mathbf{R}$ または $E = \mathbf{C}$ の場合、混乱が生じない限り、$\mathscr{K}(X;\mathbf{R})$ または $\mathscr{K}(X;\mathbf{C})$ (それぞれ $\mathscr{K}(X,A;\mathbf{R})$ または $\mathscr{K}(X,A;\mathbf{C})$) の代わりに $\mathscr{K}(X)$ (それぞれ $\mathscr{K}(X,A)$) と書きます。 $\mathscr{K}(X;\mathbf{R})$の写像$\geq 0$によって形成される尖った凸円錐を$\mathscr{K}_+(X)$で表します。

X のすべてのコンパクトな部分集合 K について、空間 $\mathscr{K}(X,K;E)$ は、連続関数空間 $\mathscr{C}(K;E)$ の部分空間 (つまり、K の境界 $^1$ でゼロである、K から E への連続写像の部分空間) と識別される可能性があります。 $\mathscr{C}(K;E)$にKの一様収束の位相が備わっている場合、$\mathscr{K}(X,K;E)$は$\mathscr{C}(K;E)$の閉じた部分空間になります。 特に、E がフレシェ空間 (それぞれバナッハ空間) である場合、$\mathscr{K}(X,K;E)$ も同様です。なぜなら、E の位相が準規範 $p_n$ (それぞれノルム $x \mapsto \|x\|$) によって定義される場合、$\mathscr{K}(X,K;E)$ の位相となるからです。定義されています

(1) 原文はfrontièreで、「辺境」とも訳される(GT, I, §1, No. 6, Def. 11)。

準規範 $f \mapsto \sup_{x \in K} p_n(f(x))$ (それぞれノルム $f \mapsto \sup_{x \in K} \|f(x)\|$、$\|f\|$ で示される) による。

空間 $\mathscr{K}(X; E)$ は、部分空間 $\mathscr{K}(X, K; E)$ の増加する有向族の和集合で、$K$ は $X$ のコンパクト部分集合の集合を上回ります。さらに、$K_1 \subset K_2$ が 2 つのコンパクトな $X$ の 2 つの部分集合である場合、上で定義したトポロジーでは標準単射 $\mathscr{K}(X, K_1; E) \to \mathscr{K}(X, K_2; E)$ が連続です。 $E$ が *局所凸* である場合、$\mathscr{K}(X, K; E)$ (TVS、II, §4, No. 4) の局所凸トポロジの *直接極限*² を $\mathscr{K}(X; E)$ で定義するにすることができます。 〜でない限りは反対のことを明示的に述べていますが、$\mathscr{K}(X; E)$ をトポロジカルなベクトル空間とみなすとき、これは常に位相に問題となります。

#### 命題 1 {#int-iii-s1-prop-1 .statement tag=08L5}

*$X$ を局所コンパクト空間、$E$ をハウスドルフ局所凸空間とします。*

(i) *局所凸空間 $\mathscr{K}(X; E)$ はハウスドルフです。 $X$ の各コンパクト部分集合 $K$ について、$\mathscr{K}(X; E)$ のそれによって誘起される $\mathscr{K}(X, K; E)$ の位相は、$K$ における一様収束の位相であり、部分空間 $\mathscr{K}(X, K; E)$ のそれぞれは で閉じられます。 $\mathscr{K}(X; E)$.*

(ii) *$E$ が局所凸空間 $E_i$ ($1 \leq i \leq n$) の有限数の積である場合、写像 $f \mapsto (\mathrm{pr}_i \circ f)$ は空間の同型です。 $\mathscr{K}(X; E)$ から積空間 $\prod_{1 \leq i \leq n} \mathscr{K}(X; E_i)$.*

(iii) *$X$ がローカルコンパクト空間のファミリー $(X_\lambda)_{\lambda \in L}$ の和である場合、写像 $f \mapsto (f|X_\lambda)_{\lambda \in L}$ はトポロジカル直和上の空間 $\mathscr{K}(X; E)$ の同型になります。 $(\mathscr{K}(X_\lambda; E))_{\lambda \in L}$ 家族の空間.*

(i) $\mathscr{K}(X; E)$ では、一様収束 *in* $X$ の位相は、$\mathscr{K}(X; E)$ のベクトル空間構造と互換性があることに注意してください。これは、$f \in \mathscr{K}(X; E)$ ごとに (コンパクトな) $S$、集合がサポートされているためです。 $f(X) = f(S) \cup \{0\}$ はコンパクトであるため、$E$ に制限されます (TVS、III, §3, No. 1、提案 1)。この位相 $\mathscr{T}_0$ は局所的に凸であり、$K$ における一様収束の各 $\mathscr{K}(X, K; E)$ 位相上で誘導するであるため、$\mathscr{K}(X; E)$ 上の直接の極限位相 $\mathscr{T}$ にも同じことが当てはまります。 (TVS、II, §4, No. 4、*注意*);さらに、$\mathscr{T}$ は $\mathscr{T}_0$ よりもより細かいであり、$\mathscr{T}_0$ はハウスドルフであるため、$\mathscr{T}$ はハウスドルフです。最後に、写像 $f \in \mathscr{K}(X; E)$ 属するから $\mathscr{K}(X, K; E)$ の終点までを仮定します。 定義までに、$f \in \mathscr{K}(X, K'; E)$ となるような $X$ のコンパクトな部分集合 $K' \supset K$ が存在します。上記により、$f$ 属するから空間 $\mathscr{K}(X, K'; E)$ の $\mathscr{K}(X, K; E)$ の終結まで、したがって属するから $\mathscr{K}(X, K; E)$ となります。

(ii) 直接極限 (TVS、II, §4, No. 4、提案 5) の連続性の基準は、写像 $f \mapsto (\mathrm{pr}_i \circ f)$ が連続であること、および逆行列写像にも同じことが当てはまることをすぐに示します (後者の場合、すべての写像について、 $f_i \in \mathscr{K}(X; E_i)$、1 は $f'_i$ 写像で表されます

² *限界誘導*、S、A、GT では「直接極限」と訳されます。

X を E に変換し、$j \neq i$ に対して $\mathrm{pr}_i \circ f'_i = f_i$ と $\mathrm{pr}_j \circ f'_i = 0$ が成り立つと、写像 $f_i \mapsto f'_i$ はそれぞれ連続します)。

(iii) X の各コンパクト部分集合 K は、$(X_\lambda)_{\lambda \in L}$ の有限部分族 $(X_\lambda)_{\lambda \in H}$ の $X_\lambda$ とのみ交差し、$\lambda \in H$ に対して集合 $K_\lambda = K \cap X_\lambda$ を写像とすると、明らかになります。 $f \mapsto (f|X_\lambda)_{\lambda \in H}$は、$\mathscr{K}(X, K; E)$の$\prod_{\lambda \in H} \mathscr{K}(X_\lambda, K_\lambda; E)$上の同型です。逆に、すべての写像 $f_\lambda \in \mathscr{K}(X_\lambda; E)$ について、$f''_\lambda$ を X の写像として、$\mu \neq \lambda$ に対して $f''_\lambda|X_\lambda = f_\lambda$ と $f''_\lambda|X_\mu = 0$ が成り立つようにします。 $\mathscr{K}(X_\lambda; E)$から$\mathscr{K}(X; E)$に写像$f_\lambda \mapsto f''_\lambda$が連続するのは明らかです。 主張 (iii) は、これらの注意と直接の連続性の基準極限 (TVS、II, §4, No. 4、提案 5) から導かれます。

#### 命題 2 {#int-iii-s1-prop-2 .statement tag=08L6}

— *X を局所コンパクト空間、E をハウスドルフ局所凸空間とします。*

(i) *E がフレシェ空間の場合、空間 $\mathscr{K}(X; E)$ はバレルになります。*

(ii) *X がパラコンパクトである場合、$\mathscr{K}(X; E)$ のすべての有界集合 B に対して、$B \subset \mathscr{K}(X, K; E)$ となるような X のコンパクト部分集合 K が存在します。

E がフレシェ空間であるとします。次に、X のすべてのコンパクト部分集合 K について、$\mathscr{K}(X, K; E)$ はフレシェ空間であるため、バレル化され、バレル化された空間の直接の極限がバレル化されることがわかります (TVS、III, §4, No. 1、提案 3 の Cor. 3)、よって (i)。

X がパラコンパクトである場合、X は *無限で可算* な局所コンパクト空間の族 $(X_\lambda)_{\lambda \in L}$ の和であることがわかります (GT, I, §9, No. 10, Th. 5)。したがって (提案 1、(iii))、$\mathscr{K}(X; E)$ は、部分空間 $\mathscr{K}(X_\lambda; E)$ ($\lambda \in L$) の族の *位相幾何学直和* です。トポロジー 直和 (TVS、III, §1, No. 4、提案 5) の有界集合の特徴付けにより、$\mathscr{K}(X; E)$ のすべての有界集合は、部分空間の *有限* 数の和に含まれます。 $\mathscr{K}(X_\lambda; E)$ そして、$\mathscr{K}(X_\lambda; E)$ のすべての有界集合が部分空間 $\mathscr{K}(X_\lambda, K_\lambda; E)$ に含まれ、$K_\lambda$ が $X_\lambda$ にコンパクトになることを証明すれば十分です。したがって、X は無限に可算であり、他の場合では、語は比較的コンパクトな開いた集合 $U_n$ の数列の和集合であり、$\overline{U}_n \subset U_{n+1}$ (GT, I, §9, No. 9, 提案 15) である場合に帰着します。しかし、$\mathscr{K}(X; E)$ は、空間 $\mathscr{K}(X, \overline{U}_n; E)$、よって主張 (ii) (TVS、III, §1, No. 4、提案 6) の数列の *厳密な* 直接の極限です。

$\mathscr{K}(X; E)$ の部分集合 H は、それがコンパクトで、$H \subset \mathscr{K}(X, K; E)$ となるような X のコンパクト部分集合 K が存在する場合、*厳密にコンパクト* であると言えます。 命題 2 から、X が *パラコンパクト* ローカルコンパクト空間であり、E がハウスドルフである場合、$\mathscr{K}(X; E)$ の *すべてのコンパクト集合* は *厳密にコンパクト * であることがすぐにわかります。ローカルコンパクトの例を与えることができます

3 *Dénombrable à l'infini*、「σ-コンパクト」とも訳される (GT、I, §9, No. 9、定義 5)。

空間 $X$ (準コンパクトではない) なので、$\mathscr{K}(X; \mathbf{R})$ には *コンパクトだが厳密にはコンパクトではない * (練習問題 3 と 4) 集合が存在します。

We recall that, by virtue of Ascoli’s theorem (GT, X, §2, No. 5, Cor. 3 of Th. 2), a strictly compact subset $H$ of $\mathscr{K}(X; E)$ contained in $\mathscr{K}(X, K; E)$ is characterized by the following conditions: $1^\circ$ it is closed; $2^\circ$ it is equicontinuous; $3^\circ$ for every $x \in K$, the set $H(x)$ is relatively compact in $E$.

#### 系 {#int-iii-s1-n1-cor-1 .statement tag=08L7}

*$X$ をパラコンパクト、ローカルコンパクト空間とします。 $E$ が準完全局所凸空間である場合、空間 $\mathscr{K}(X; E)$ は準完全です。*

命題 2, (ii) のおかげで、$X$ のすべてのコンパクト部分集合 $K$ について、$\mathscr{K}(X, K; E)$ は $C(K; E)$ の閉じた部分空間であり、$C(K; E)$ のすべての有界部分集合が以下から構成されるため、これは準完全であることに注意するだけで十分です。 写像は $E$ の同じ境界部分集合で値を取得します。

### 2. 近似特性

#### 補題 1 {#int-iii-s1-lem-1 .statement tag=08L8}

*$X$を局所的にコンパクトな空間、$K$を$X$のコンパクト部分集合、$(V_k)_{1 \leq k \leq n}$を$X$のオープン集合による$K$の有限カバーとする。次に、$X$から$[0, 1]$までの$n$連続写像$f_k$が存在し、$f_k$のサポートが$1 \leq k \leq n$の$V_k$に含まれ、すべての$x \in X$に対して$\sum_{k=1}^n f_k(x) \leq 1$が含まれるようになり、 $x \in K$全員に対して$\sum_{k=1}^n f_k(x) = 1$。

なぜなら、$X'$ を無限遠$\omega$ (GT, I, §9, No. 8, Th. 4) で$X$ 点に隣接することによって得られるコンパクト空間とする。 集合 $V_0 = X' - K$ と $V_k$ ($1 \leq k \leq n$) 形 $X'$ のオープンカバー。 $(f_k)_{0 \leq k \leq n}$ を、$X'$ のこのカバーに従属する単位元の連続する分割とします (GT、IX, §4, No. 3、提案 3)。 写像 $f_k$ と添字 $k \geq 1$ 満たす条件の補題。

#### 補題 2 {#int-iii-s1-lem-2 .statement tag=08L9}

*$X$を局所的にコンパクトな空間、$K$を$X$のコンパクトな部分集合、$E$を局所的に凸な空間、$q$を$E$上の連続半ノルム、$\Phi$を等連続の集合の写像の $X$ から $E$ へ、そのサポートは $K$ に含まれます。次に、$\varepsilon > 0$ ごとに、以下の特性を持つ単位元 $(\varphi_j)_{0 \leq j \leq n}$ の連続する分割が $X$ に存在します。
(i) $1 \leq j \leq n$ の場合は $\operatorname{Supp}(\varphi_j) \subset K$。
(ii) *$1 \leq j \leq n$ について、$x_j$ が $\operatorname{Supp}(\varphi_j)$ のいずれかの点である場合、すべての写像 $f \in \Phi$ およびすべての $x \in X$ について、
$$
q\left(f(x) - \sum_{j=1}^n \varphi_j(x) f(x_j)\right) \leq \varepsilon.
$$*

$K$ の境界までのすべての $y$ 所属について、すべての $f \in \Phi$ について $f(y) = 0$ が存在するため、$X$ には $y$ の開いた近傍 $V_y$ が存在し、すべての $z \in V_y$ とすべての $f \in \Phi$ について、 $q(f(z)) \leq \varepsilon/2$。 $y$ が $K$ の境界を越えるため、$K'$ を $V_y$ のいずれかの所属ではなく、$K$ の点の集合とします。 $K'$は$K$の内部にコンパクトに収まります。 集合 $\Phi$ は $K$ で等連続です。したがって、$K$に含まれる$X$のオープン集合の$K'$からなるの有限のオープンカバー$(U_j)_{1 \leq j \leq n}$が存在し、同じ$U_j$の点$x, y$の対ごとに、 $f \in \Phi$ごとに$q(f(x) - f(y)) \leq \varepsilon/2$。 補題 1 により、$X$ の $\varphi_j$ から $[0, 1]$ ($1 \leq j \leq n$) への $\operatorname{Supp}(\varphi_j) \subset U_j$ などの $n$ 連続マッピングが存在します。
$$
\sum_{j=1}^n \varphi_j(x) \leq 1 \text{ on } X \text{ and } \sum_{j=1}^n \varphi_j(x) = 1 \text{ on } K'.
$$
したがって、$x_j \in \operatorname{Supp}(\varphi_j)$ ($1 \leq j \leq n$) と $f \in \Phi$ については、すべての $x \in U_j$ について、
$$
q(f(x)\varphi_j(x) - f(x_j)\varphi_j(x)) = \varphi_j(x)q(f(x) - f(x_j)) \leq \frac{\varepsilon}{2}\varphi_j(x),
$$
そしてこの関係は、$x \notin U_j$ 以降 $\varphi_j(x) = 0$ になっても当てはまります。 加法までに、$x \in X$ ごとに、
$$
q\left(f(x)(1 - \varphi_0(x)) - \sum_{j=1}^n \varphi_j(x)f(x_j)\right) \leq \frac{\varepsilon}{2}(1 - \varphi_0(x)),
$$
ここで$\varphi_0 = 1 - \sum_{j=1}^n \varphi_j$; $x \in K'$ ではよって (1)、それ以降は $\varphi_0(x) = 0$;
(1) は$x \notin K$にも当てはまり、最初のメンバーは零になります。 最後に、$x \in K - K'$ については、$K'$ の定義によって $q(f(x)\varphi_0(x)) \leq \varepsilon/2$ が得られるため、この場合、この関係と (2) は再び (1) を意味します。

$X$ を局所的にコンパクトな空間とします。すべてのバナッハ空間 $E$ (実数または複素数) について、$X$ の連続かつ有界の写像を $E$ に$\mathscr{C}^b(X; E)$ ベクトル空間で表します。 $X$の一様収束の位相は$\mathscr{C}^b(X; E)$のベクトル空間構造(実数、複素数)と互換性があり、ノルムによって定義されることがわかっています。
$$
||f|| = \sup_{x \in X} ||f(x)||.
$$
さらに、このように定義された正規化空間は、Banach 空間 (GT、X, §3, No. 2、および No. 1、提案 2 の Cor. 2) です。 $\mathscr{K}(X; E)$ 上のこのノルム ($X$ の一様収束の他の語、位相) によって定義される位相は、No. 1 で定義された$\mathscr{K}(X; E)$ 上の直接の極限位相より粗いです。

#### 命題 3 {#int-iii-s1-prop-3 .statement tag=08LA}

— $X$ を局所コンパクト空間、$X'$ $X$ 無限遠点 $\omega$ (GT, I, §9, No. 8,

Th. 4)、E a Banach 空間。正規の空間 $C^b(X;E)$ における $\mathscr{K}(X;E)$ の終結は、X で連続する写像のベクトル空間であり、E に値があり、点 $\omega$ で 0 になる傾向があります。

$f \in C^b(X;E)$ を $\mathscr{K}(X;E)$ の終結で写像とします。すべての $\varepsilon > 0$ に対して、写像 $g \in \mathscr{K}(X;E)$ が存在し、すべての $x \in X$ に対して $\|f(x) - g(x)\| \leq \varepsilon$ になります。 K が g のサポートである場合、すべての $x \in \mathbf{C}K$ に対して $\|f(x)\| \leq \varepsilon$ となるため、$x$ が $\omega$ になる傾向があるのと同様に、$f(x)$ も 0 になる傾向があります。逆に、f がこの性質を持つ場合、すべての $\varepsilon > 0$ に対して、すべての $x \in \mathbf{C}K$ に対して $\|f(x)\| \leq \varepsilon$ となるようなコンパクトな集合 $K \subset X$ が存在します。 補題 1 までに、X から $[0,1]$ までの継続的な写像時間が存在し、コンパクトなサポートがあり、K の 1 に相当します。次に、$\mathbf{C}K$では$\|f(x)h(x)\| \leq \varepsilon$、Kでは$f(x) = f(x)h(x)$です。 $fh$ にはコンパクトなサポートがあり、すべての $x \in X$ に対して $\|f(x) - f(x)h(x)\| \leq 2\varepsilon$ があるため、命題が証明されます。

写像が無限大 $\omega$ で点で零になる傾向によって形成される $C^b(X;E)$ の $C^0(X;E)$ 部分空間で表すことにします。したがって、これは標準的な空間 $\mathscr{K}(X;E)$ の完成です。

#### 命題 4 {#int-iii-s1-prop-4 .statement tag=08LB}

— X を局所的にコンパクトな空間、E を局所的に凸な空間とします。すると、空間 $\mathscr{K}(X;E)$ はコンパクト収束の位相に対して $C(X;E)$ で密になります。

すべてのコンパクト集合 $K \subset X$ に対して、補題 1 による K 上の 1 に等しい写像 $h \in \mathscr{K}(X;\mathbf{R})$ が存在します。 属するから $\mathscr{K}(X;E)$ までのすべての写像 $f \in C(X;E)$ 写像 $hf$ は、K の f、よっての主張に等しい。

#### 命題 5 {#int-iii-s1-prop-5 .statement tag=08LC}

— X を局所的にコンパクトな空間、E を局所的に凸な実数 (それぞれ複素数) 空間とします。すべてのコンパクト X の部分集合 K、ベクトル空間 $\mathscr{K}(X,K;\mathbf{R}) \otimes_{\mathbf{R}} E$ (それぞれ $\mathscr{K}(X,K;\mathbf{C}) \otimes_{\mathbf{C}} E$) (X の写像の集合で E、cf. A、II, §7, No. 7、Prop の Cor. に識別されます。 15) $\mathscr{K}(X,K;E)$ は密です。 ベクトル空間 $\mathscr{K}(X;\mathbf{R}) \otimes_{\mathbf{R}} E$ (それぞれ $\mathscr{K}(X;\mathbf{C}) \otimes_{\mathbf{C}} E$) は $\mathscr{K}(X;E)$ に密集しています。

2 番目の主張は最初の帰結であることが明らかなので、後者を証明するだけで十分です。 $\Phi$ を 1 つの $\mathscr{K}(X,K;E)$ の 1 つの元 $f$ に減じて補題 2 を適用します。その後、$x \in X$ ごとに、

$$
q\left(f(x) - \sum_{j=1}^n \varphi_j(x)f(x_j)\right) \leq \varepsilon,
$$

ここで、$\varphi_j$ 属するから $\mathscr{K}(X,K;\mathbf{R})$ です。 写像 $x \mapsto \sum_{j=1}^n \varphi_j(x)f(x_j)$ は正規的に元 $\sum_{j=1}^n \varphi_j \otimes f(x_j)$ と識別される可能性があるため、これは $\mathscr{K}(X,K;E)$ の位相の定義により命題であることが証明されます。

### 3. 小節の定義

#### 定義 2 {#int-iii-s1-def-2 .statement tag=08LD}

— *$\mathscr{K}(X; \mathbf{C})$ 上の *連続線型形式、*X 局所的にコンパクトな空間*、*メジャー* (または *複雑なメジャー*) *オン X*。

If $\mu$ is a measure on a locally compact 空間 $X$, 値 of the measure for 写像 $f \in \mathscr{K}(X; \mathbf{C})$ is called the *integral of f with respect to* $\mu$;一般的な記法 $\mu(f)$ と $\langle f, \mu \rangle$ のほかに、記法 $\int f d\mu$、$\int f \mu$、$\int f(x) d\mu(x)$、$\int f(x) \mu(x)$ も使用します。文字$x$の使用については、S、I, §1, No. 1を参照してください。

By virtue of the criterion for continuity in direct 極限 (TVS, Ch. II, §4, No. 4, Prop. 5), to say that $\mu$ is a measure on $X$ means that $\mu$ is 線型形式 on $\mathscr{K}(X; \mathbf{C})$ 満たす the following 条件: $X$ のすべてのコンパクト部分集合 $K$ に対して、数 $M_K$ が存在し、すべての写像 $f \in \mathscr{K}(X; \mathbf{C})$ *そのサポートは $K$ に含まれます。

$$
| \mu(f) | \leq M_K \cdot \| f \| \quad \text{(where } \| f \| = \sup_{x \in X} |f(x)| ).
$$

より一般的には:

#### 命題 6 {#int-iii-s1-prop-6 .statement tag=08LE}

— *Let X be a locally compact 空間, ($K_\alpha$) a family of compact 部分集合 of X whose interiors $\overset{\circ}{K}_\alpha$ 形 an open covering of X. For 線型形式 $\mu$ on $\mathscr{K}(X; \mathbf{C})$ to be a measure on X, it is necessary and sufficient that, for every $\alpha$, there exist 数 $M_\alpha$ such that*

$$
| \mu(f) | \leq M_\alpha \cdot \| f \|
$$

*写像* $f \in \mathscr{K}(X, K_\alpha; \mathbf{C})$ごと。

条件が明らかに必要であるため、$X$ のすべてのコンパクト部分集合 $K$ について (5) が (4) を意味することを証明するだけで十分です。さて、$K$ は、開いた集合 $\overset{\circ}{K}_{\alpha_i}$ ($1 \leq i \leq n$) の有限数によってカバーされます。 適用補題 1 of No. 2 to $K$ and to the $\overset{\circ}{K}_{\alpha_i}$, there exist continuous 写像 $g_i \geq 0$ on $X$ such that $\operatorname{Supp}(g_i) \subset K_{\alpha_i}$, $0 \leq \sum_{i=1}^n g_i(x) \leq 1$ for all $x \in X$ と $\sum_{i=1}^n g_i(x) = 1$ は $x \in K$ です。したがって、写像 $f \in \mathscr{K}(X, K; \mathbf{C})$ ごとに $f = \sum_{i=1}^n f g_i$ と書くことができ、$f g_i \in \mathscr{K}(X, K_{\alpha_i}; \mathbf{C})$ と $\| f g_i \| \leq \| f \|$ が得られます。 $M_K = \sum_{i=1}^n M_{\alpha_i}$ の場合、関係 (4) になります。

$\mathscr{M}(X; \mathbf{C})$、または混乱が生じない場合は単に$\mathscr{M}(X)$で、$X$の措置のベクトル空間、その他の語、$\mathscr{K}(X; \mathbf{C})$の*二重*を表します。

$\mathscr{K}(X;\mathbf{C})$ の *有界* 部分集合のすべての集合 $\mathscr{S}$ について、$\mathscr{M}(X;\mathbf{C})$ に局所的に凸な $\mathscr{S}$ トポロジーが定義されていることがわかります (TVS、III, §3, No. 1、提案 1 の Cor.)。 $\mathscr{M}(X;\mathbf{C})$ に $\mathscr{S}$ トポロジーを装備することで得られるトポロジー ベクトル空間を $\mathscr{M}_{\mathscr{S}}(X;\mathbf{C})$ または $\mathscr{M}_{\mathscr{S}}(X)$ で表します。

#### 命題 7 {#int-iii-s1-prop-7 .statement tag=08LF}

*$\mathscr{K}(X;\mathbf{C})$ をカバーする$\mathscr{K}(X;\mathbf{C})$ の有界部分集合の各集合 $\mathscr{S}$ について、空間 $\mathscr{M}_{\mathscr{S}}(X;\mathbf{C})$ はハウスドルフで準完全です。*

これは、$\mathscr{K}(X;\mathbf{C})$ がバレル化されているという事実から生じます (TVS、III, §4, No. 2、Th. 1 の Cor. 4)。

*例の対策* — I。 *原子的手段。* X を局所的にコンパクトな空間、$a$ を X の点とします。 $\mathscr{K}(X;\mathbf{C})$ の $\mathbf{C}$ へのマッピング $f\mapsto f(a)$ は、$a$ を含むX のすべてのコンパクトサブセット K について$M_K=1$ で条件 (4) を明らかに満たすため、$\varepsilon_a$ で示される X に関する測度になります。それは、点$a$における*ディラック測度*、または点$a$に配置された*単位質量によって定義される測度*と呼ばれます。

より一般的には、$\alpha$ を X の写像から $\mathbf{C}$ にすると、X のすべてのコンパクト部分集合 K に対して、
$$
\sum_{x\in K}|\alpha(x)|<+\infty.
$$
その後、写像 $f\in\mathscr{K}(X,K;\mathbf{C})$、和ごとに
$$
\mu(f)=\sum_{x\in X}\alpha(x)f(x)
$$
と等しいと定義されています
$$
\sum_{x\in K}\alpha(x)f(x);
$$
$\mu$ が $\mathscr{K}(X;\mathbf{C})$ の線型形式であること、そして $f\in\mathscr{K}(X,K;\mathbf{C})$ については、
$$
|\mu(f)|\leq\left(\sum_{x\in K}|\alpha(x)|\right)\cdot\|f\|,
$$
その他語条件 (4) は満たされます。

X から $\mathbf{C}$ へのマッピング $\alpha$ が存在する場合、X のメジャー $\mu$ は *アトミック* であると言われます。
$$
\sum_{x\in K}|\alpha(x)|<+\infty
$$
X のすべてのコンパクトなサブセット K に対して、$\mu$ が上記で定義された測度に等しいようにします。 N が $x\in X$ の集合で、$\alpha(x)\neq0$、$\alpha$ に課せられた条件は、X のすべてのコンパクト部分集合 K について、$K\cap N$ が *可算* であることを意味します。 $\mu$ は、点* $x\in N$ に配置された *大衆* $\alpha(x)$ によって定義されるとも言われています。 $N\cap K$ がすべてのコンパクト集合 $K\subset X$ に対して *有限* であると仮定すると、明らかに
$$
\sum_{x\in K}|\alpha(x)|<+\infty;
$$
N が X の *閉じた* で *離散 * 部分空間であると言うのは同じことになります。その場合、X のすべての点にはコンパクトな近傍含むがあり、N の点の有限の数だけがあり、逆に、これが当てはまる場合、すべてのコンパクトはX のうち部分集合は、そのような近傍の有限の数でカバーできます。 N が閉じていて離散的である場合、$\mathbf C N$ 上の $\alpha(x)=0$ など、写像 $\alpha$ によって定義されるすべての原子メジャーは、X (cf. §2, No. 5) 上の離散メジャーと呼ばれます。

### II。 *ルベーグ測度* 写像 $f\in\mathscr K(\mathbf R;\mathbf C)$ ごとに、$\mathbf R$ のコンパクトな区間 $[a,b]$ が存在し、その外側に $f$ は零です。整

$$
\mathrm I(f)=\int_{-\infty}^{+\infty}f(x)\,dx=\int_a^b f(x)\,dx
$$

したがって、 は定義されます。さらに、平均 (FRV、II, §1, No. 5、提案 6) の定理により、$|\mathrm I(f)|\leq(b-a)\|f\|$ になります。これは、$f\mapsto\mathrm I(f)$ が $\mathbf R$ の測度であることを示しており、これは *ルベーグ測度* と呼ばれます。

$\mathbf R$ のすべての区間 J (有界かどうか) について、同様に、J* 上の *ルベーグ測度、$\mathscr K(J;\mathbf C)$ 上の測度 $f\mapsto\int_Jf(x)\,dx$、線型形式 (J に含まれるコンパクトな区間 $[a,b]$ が存在し、その外側に $f$ が含まれるため、意味を持つ積分) を呼び出します。 零）。

### III。 $g$ を、区間 $I\subset\mathbf R$ を $\mathbf C$ に圧縮した連続写像とし、I に連続導関数を持ちます。 $\mathbf C$ のコンパクトな部分空間である $\Gamma=g(I)$ としましょう。 写像

$$
f\mapsto\int_I f(g(t))g'(t)\,dt
$$

$\mathscr C(\Gamma;\mathbf C)$ から $\mathbf C$ への変換は、平均の定理により連続的な線型形式であるため、$\Gamma$* に対する *複素測度になります。この尺度に対する積分は $\int_\Gamma f(z)\,dz$、さらにけれどもと書かれますが、これは $\Gamma$ だけでなく $g$ にも依存します。

#### 注意 {#int-iii-s1-n3-rem-1 .statement tag=08LG}

局所的にコンパクトな空間 X 定義するに X のメジャー $\mu$ (X の位相とともに) 構造 $\mathscr S$ を与える。 $X_1$ を 2 番目の集合、$\varphi$ を X から $X_1$ への全単射写像とします。一般的な定義 (S, R, §8) に準拠して、X の$X_1$ 構造 $\mathscr S$ を$\varphi$ によって *転送*して得られる構造 $\mathscr S_1$ は次のように定義されます。 X の位相は $\varphi$ によって $X_1$ に輸送されます。 $\mathscr K(X_1;\mathbf C)$ の写像は写像 $f$ となり、$f\circ\varphi$ 属するから $\mathscr K(X;\mathbf C)$ となり、$X_1$ のメジャー $\mu_1$ は $\mu_1(f)=\mu(f\circ\varphi)$ によって定義されます。

特に、構造 $\mathscr S$ の *自己同型* は、それ自体に対する X の同型写像 $\sigma$ であり、次のようになります。

$$
\mu(f)=\mu(f\circ\sigma)
$$

写像 $f\in\mathscr K(X;\mathbf C)$ごとに;したがって、測度 $\mu$ は *同同型* $\sigma$ の下で不変であると言われます。

#### 例 {#int-iii-s1-n3-exa-1 .statement tag=08LH}

$\mathbf{R}$ のルベーグ測度は、加法群 $\mathbf{R}$ のすべての変換の下で不変です。実際、すべての写像 $f \in \mathscr{K}(\mathbf{R}; \mathbf{C})$ とすべての実数 $a$ について、

$$
\int_{-\infty}^{+\infty} f(x + a)\, dx = \int_{-\infty}^{+\infty} f(t)\, dt
$$

変数変更公式 (FRV, II, §2, No. 1, 公式 (1)) によって。 一般化については、第 3 章を参照してください。 VII, §1, No. 2、木曜日。 1.

### 4. 写像による小節の積

$X$ を局所的にコンパクトな空間、$g$ を $X$ から $\mathbf{C}$ への連続写像とする。 $f \mapsto gf$ が$\mathscr{K}(X; \mathbf{C})$ の線形写像であることは明らかです。この写像が連続であることを示しましょう。実際、$X$ のすべてのコンパクト部分集合 $K$、およびすべての写像 $f \in \mathscr{K}(X, K; \mathbf{C})$ に対して、$gf \in \mathscr{K}(X, K; \mathbf{C})$ が得られます。さらに、$b_K = \sup_{x \in K} |g(x)|$ の場合、$\|gf\| \leq b_K \|f\|$、よっては私たちの主張 (TVS、II, §4, No. 4、提案 5)。したがって、この連続線形写像 (TVS、II, §6, No. 4) の転置は、$\mathscr{M}(X; \mathbf{C})$ の線形写像となり、$\mu \mapsto g \cdot \mu$ (混乱が生じない場合は $\mu \mapsto g\mu$) と表されます。したがって、$\nu = g \cdot \mu$ の場合、写像 $f \in \mathscr{K}(X; \mathbf{C})$ ごとに、

$$
\langle f, \nu \rangle = \langle gf, \mu \rangle
$$

またはもう一度

$$
\int f(x)\, d\nu(x) = \int f(x)g(x)\, d\mu(x)
$$

(形 $d\nu(x) = g(x)\, d\mu(x)$ では省略されます)。 $g \cdot \mu$ は、写像 $g$ による測度 $\mu$ の積である、あるいは、$\mu$ に対する稠密度 $g$ による測度であるとも言われています (cf. Ch. V, §5, No. 2, Def. 2)。 $g_1, g_2$ が $X$ から $\mathbf{C}$ に続く 2 つの写像で、$\mu_1, \mu_2$ が $X$ の 2 小節である場合、

$$
(g_1 + g_2) \cdot \mu = g_1 \cdot \mu + g_2 \cdot \mu, \quad g \cdot (\mu_1 + \mu_2) = g \cdot \mu_1 + g \cdot \mu_2,
$$
$$
(g_1 g_2) \cdot \mu = g_1 \cdot (g_2 \cdot \mu).
$$

さらに、$1 \cdot \mu = \mu$ (ここで 1 は、$X$ の 1 に等しい定数写像を示します)。 集合 $\mathscr{M}(X; \mathbf{C})$ は、合成 $(g, \mu) \mapsto g \cdot \mu$ の外部法則とその添加物構造を備えており、環 $\mathscr{C}(X; \mathbf{C})$ を上回る加群になります。

### 5. 本当の対策。積極的な対策

X をローカルコンパクト空間とします。実数ベクトル空間 $\mathscr{K}(X; \mathbf{R})$ は、複合体ベクトル空間 $\mathscr{K}(X; \mathbf{C})$ の基礎となる実数ベクトル空間の部分空間です。さらに、写像 $(f_1, f_2) \mapsto f_1 + i f_2$ は、実際のトポロジカルベクトル空間 $\mathscr{K}(X; \mathbf{C})$ 上の積トポロジカルベクトル空間 $\mathscr{K}(X; \mathbf{R}) \times \mathscr{K}(X; \mathbf{R})$ の *同型* です (No. 1、提案 1)。

すべての (複素) メジャー $\mu \in \mathscr{M}(X; \mathbf{C})$、$\mu$ から $\mathscr{K}(X; \mathbf{R})$ の制限 $\mu_0$ は、$\mathscr{K}(X; \mathbf{R})$ から $\mathbf{C}$ への連続 $\mathbf{R}$ 線形マッピングです。さらに、この制限決定する $\mu$ は、$f = f_1 + i f_2$ と $\mathscr{K}(X; \mathbf{R})$ に $f_1, f_2$ がある場合、$\mu(f) = \mu_0(f_1) + i \mu_0(f_2)$ になります。逆に、$\mu_0$ を $\mathscr{K}(X; \mathbf{R})$ から $\mathbf{C}$ への連続 $\mathbf{R}$ 線形写像とする。 写像であることは明らかです

$$
f_1 + i f_2 \mapsto \mu_0(f_1) + i \mu_0(f_2)
$$

はXの（複素）対策です。したがって、X のすべての小節は、制限から $\mathscr{K}(X; \mathbf{R})$ で識別される可能性があります。

$\mu$をXのメジャーとします。 $\mu$ の *共役メジャー * を、写像 $f \in \mathscr{K}(X; \mathbf{C})$ ごとに $\overline{\mu}(f) = \overline{\mu(\overline{f})}$ で定義されたメジャー $\overline{\mu}$ を呼び出します。なぜなら、$\overline{\mu}$ が C 線形形式であり、$\mathscr{K}(X; \mathbf{C})$ で連続であることは明らかだからです。明らかに $\overline{\mu} = \mu$、そして 2 小節 $\mu, \nu$ と $\mathbf{C}$ の 2 つのスカラー $\alpha, \beta$ について、

$$
(\alpha \mu + \beta \nu) = \overline{\alpha} \cdot \overline{\mu} + \overline{\beta} \cdot \overline{\nu}.
$$

より一般的には、写像 $g \in \mathscr{C}(X; \mathbf{C})$ ごと、および X の各小節 $\mu$ に対して、

$$
g \cdot \overline{\mu} = \overline{g} \cdot \overline{\mu},
$$

定義 (No. 4) から明らかと同様です。

X のメジャー $\mu$ は、$\overline{\mu} = \mu$ であれば *本物* であると言われます。前述のことから、すべての写像 $f \in \mathscr{K}(X; \mathbf{R})$ に対して、$\mu(f)$ は *本物* 数であると言うのと同じです。 制限から $\mathscr{K}(X; \mathbf{R})$ で実測度を特定すると、X の実測度の集合は、局所的に凸な実測度空間 $\mathscr{K}(X; \mathbf{R})$ の *双対* であると言えます。それは、$\mathscr{M}(X; \mathbf{R})$ (混乱を引き起こさない場合は、ときどき $\mathscr{M}(X)$) で示される実際のベクトル空間です。 $\mathbf{R}$ のルベーグ測度は、点 $a \in X$ ごとのディラック測度 $\varepsilon_a$ と同様に、*実際の* 測度です。 $g \in \mathscr{C}(X; \mathbf{R})$ と $\mu$ が実際の尺度である場合、(7) により $g \cdot \mu$ も同様になります。

$\mu$ を X の (複素) メジャーとします。前の定義から、メジャー $\mu_1 = (\mu + \overline{\mu})/2$ と $\mu_2 = (\mu - \overline{\mu})/2i$ は *本物* であることがわかります。それらはそれぞれ、$\mu$の*実数部分*と*虚数部分*と呼ばれ、それぞれ$\mathscr{R}\mu$と$\mathscr{I}\mu$で表されます。これらの措置は、写像 $f \in \mathscr{K}(X; \mathbf{R})$ ごとに、

$$
\mu_1(f) = \mathscr{R}(\mu(f)) , \quad \mu_2(f) = \mathscr{I}(\mu(f)).
$$

明らかに
$$
\mu = \mu_1 + i \mu_2,\quad \overline{\mu} = \mu_1 - i \mu_2.
$$

コンパクトサポートを備えた $X$ 上の連続実数値写像の空間 $\mathscr{K}(X; \mathbf{R})$ は、明らかに位数関係 $f \leq g$ に対する *Riesz 空間* です。 写像 $f \geq 0$ 所属から $\mathscr{K}(X; \mathbf{R})$ ごとに $\mu(f) \geq 0$ であれば、$X$ における実際の測定値 $\mu$ は *正* であると言えます。したがって、リース空間 $\mathscr{K}(X; \mathbf{R})$ では正の線型形式 (Ch. II, §2, No. 1、Def. 1)。逆に:

#### 定理 1 {#int-iii-s1-thm-1 .statement tag=08LI}

*リース空間 $\mathscr{K}(X; \mathbf{R})$ のすべてのプラス線型形式は、$X$ の (プラスの) 実測値です。*

なぜなら、$\mu$ を $\mathscr{K}(X; \mathbf{R})$ の正の線型形式とし、$K$ を $X$ の圧縮部分集合とするからです。 $K$ 上の $f_0(x) = 1$ (No. 2、補題 1) のように、コンパクトなサポートを備えた $X$ から $[0, 1]$ への連続する写像 $f_0$ が存在します。 写像 $g \in \mathscr{K}(X, K; \mathbf{R})$ ごとに、$-\|g\|f_0 \leq g \leq \|g\|f_0$ が得られ、その結果、$|\mu(g)| \leq \|g\| \cdot \mu(f_0)$ となり、定理が証明されます。

$\mathscr{M}_+(X)$ は、$X$ のポジティブ指標の尖った凸円錐 (または、同じことになるが、リース空間 $\mathscr{K}(X; \mathbf{R})$ のポジティブ指標の円錐線型形式) を示します。

#### 定理 2 {#int-iii-s1-thm-2 .statement tag=08LJ}

*ローカル コンパクト空間 $X$ のすべての実際のメジャーは、2 つのポジティブ メジャーの差です。*

定理 1 と Ch.1 を考慮してII, §2, No. 2、木曜日。 1、すべては、$X$ 上の実際の測定値 $\mu$ が、リース空間 $\mathscr{K}(X; \mathbf{R})$ 上の *比較的限定された* 線型形式であるという証明に帰着します。 $f$ を $X$ 上の連続写像 $\geq 0$ とし、コンパクトなサポート $K$ を付けます。 $\mathscr{K}(X; \mathbf{R})$の関係 $0 \leq g \leq f$は$\|g\| \leq \|f\|$を暗示し、$g$のサポートが$K$に含まれていることを意味します。 仮定までに、写像 $h \in \mathscr{K}(X, K; \mathbf{R})$ ごとに $|\mu(h)| \leq M_K \cdot \|h\|$ となるような数 $M_K \geq 0$ が存在します。従って $|\mu(g)| \leq M_K \cdot \|g\| \leq M_K \cdot \|f\|$ となり、定理が証明されます。

従って、$X$ 上の実測度の空間 $\mathscr{M}(X; \mathbf{R})$ は、リース空間 $\mathscr{K}(X; \mathbf{R})$ 上の比較的有界な線形形式の空間と同一です。 $\mathscr{M}(X; \mathbf{R})$ で、順序関係 $\mu \leq \nu$ は、$\nu - \mu$ が正の尺度であること、またはすべての関数 $f \in \mathscr{K}_+(X)$ について $\mu(f) \leq \nu(f)$ を意味していることを思い出してください。

#### 定理 3 {#int-iii-s1-thm-3 .statement tag=08LK}

* 局所的にコンパクトな空間 $X$ 上の実際のメジャーの空間 $\mathscr{M}(X; \mathbf{R})$ は完全に格子順序付けされています。*

これはCh.から続きます。 II, §2, No. 2、木。 1.

第 3 章記法に準拠II, §1、私たちは定義する、$X$ の *実際の* メジャー $\mu$ ごとに、

$$
\mu^+ = \sup(\mu, 0),\quad \mu^- = \sup(-\mu, 0),\quad |\mu| = \sup(\mu, -\mu);
$$

次に$\mu = \mu^+ - \mu^-,\ |\mu| = \mu^+ + \mu^-$と$\inf(\mu^+, \mu^-) = 0$。さらに、写像 $f \in \mathscr{K}_+(\mathrm{X})$ ごとに、

$$
\int f\, d\mu^+ = \sup_{0 \leq g \leq f,\ g \in \mathscr{K}(\mathrm{X})} \int g\, d\mu
$$

そして

$$
\int f\, d|\mu| = \sup_{|g| \leq f,\ g \in \mathscr{K}(\mathrm{X})} \int g\, d\mu,
$$

よって、特に、

$$
\left| \int f\, d\mu \right| \leq \int |f|\, d|\mu|
$$

写像 $f \in \mathscr{K}(\mathrm{X}; \mathbf{R})$ ごとに。

この不等式は、$f \in \mathscr{K}(\mathrm{X}; \mathbf{C})$ の場合にも当てはまります。なぜなら、絶対値値 1 (不等式のどちら側でも変更ではない) の $f$ に複素数を掛けると、$\int f\, d\mu \geq 0$ と仮定できるからです。それから

$$
\left| \int f\, d\mu \right| = \int f\, d\mu = \int (\Re f)\, d\mu \leq \int |\Re f|\, d|\mu| \leq \int |f|\, d|\mu|.
$$

### 6. 複素測度の絶対値値

$\mu$ を局所的にコンパクトな空間 $\mathrm{X}$ 上の複素測度であるとします。 写像 $f \in \mathscr{K}_+(\mathrm{X})$ ごとに、正の実数

$$
L(f) = \sup_{|g| \leq f,\ g \in \mathscr{K}(\mathrm{X}; \mathbf{C})} \left| \int g\, d\mu \right|
$$

関係 $|g| \leq f$ は $\operatorname{Supp}(g) \subset \operatorname{Supp}(f)$ と $\|g\| \leq \|f\|$ を意味するため、主張は No. 3 の公式 (4) から求まります。 $L$ を 1 つの方法でのみ、$\mathrm{X}$ のプラスの尺度に拡張できることを示しましょう。 No. 5の観点から、Th。 1およびCh. II, §2, No. 1、提案 3、$f_1,\ f_2$ が $\mathscr{K}_+(\mathrm{X})$ の 2 つの写像である場合、$L(f_1 + f_2) = L(f_1) + L(f_2)$ であることを示せば十分です。ここで、$|g_1| \leq f_1$ と $|g_2| \leq f_2$ の場合、$g_1$ と $g_2$ が $\mathscr{K}(\mathrm{X}; \mathbf{C})$ の写像である場合、絶対値値 1 の複素数 $\zeta$ に対して $|g_1 + \zeta g_2| \leq f_1 + f_2$ が得られます。

$$
|\mu(g_1 + \zeta g_2)| = |\mu(g_1) + \zeta \mu(g_2)| \leq L(f_1 + f_2).
$$

さらに、$\zeta$ が次のように選択されたと仮定できます。
$$
|\mu(g_1) + \zeta \mu(g_2)| = |\mu(g_1)| + |\mu(g_2)|;
$$
$|\mu(g_i)|$ は任意に $L(f_i)$ ($i = 1, 2$) に近いので、これは $L(f_1) + L(f_2) \leq L(f_1 + f_2)$ であることを証明します。 一方、$|g| \leq f_1 + f_2$ となるような写像 $g \in \mathscr{K}(X; \mathbf{C})$ を考えてみましょう。 写像 $g_i$ は、$f_1(x) + f_2(x) \neq 0$ の点で $g f_i/(f_1 + f_2)$ に等しく、その他の場所 ($i = 1, 2$) では 0 に等しく、X では連続です。なぜなら、$f_i/(f_1 + f_2)$ ($i = 1, 2$) は $f_1(x) + f_2(x) \neq 0$ の点ごとに連続であるからです。 $x \in X$ごとに$|g_i(x)| \leq |g(x)|$、これは点での$g_i$の連続性を証明します。ここで、点には$g(x) = 0$もあるので、$f_1(x) + f_2(x) = 0$($i = 1, 2$)です。 $|g_i| \leq f_i$ ($i = 1, 2$) と $g = g_1 + g_2$ であることは明らかです。
$$
|\mu(g)| \leq |\mu(g_1)| + |\mu(g_2)| \leq L(f_1) + L(f_2);
$$
$|\mu(g)|$ は任意に $L(f_1 + f_2)$ に近いので、
$$
L(f_1 + f_2) \leq L(f_1) + L(f_2),
$$
これで、主張の証明が完了します。

$\mu$ が実測度の場合、公式 (9) から $|\mu| \leq L$ が得られます。一方、No. 5 の最後の部分により、$g \in \mathscr{K}(X; \mathbf{C})$ と $|g| \leq f \in \mathscr{K}_+(X)$ であれば $|\int g \, d\mu| \leq \int |g| \cdot d|\mu| \leq \int f \, d|\mu|$、したがって定義 $L \leq |\mu|$ までに、他の場合は語 $L = |\mu|$ になります。

任意の複素測度 $\mu$ に対する正の測度 $L$ を再び $|\mu|$ で表し、$|\mu|$ が $\mu$ の絶対的な値であると言います。従って、$|\mu|$ の定義を書くことができます
$$
|\mu|(f) = \sup_{|g| \leq f,\ g \in \mathscr{K}(X; \mathbf{C})} |\mu(g)|,
$$
従って、写像 $g \in \mathscr{K}(X; \mathbf{C})$ ごとに、
$$
\left| \int g \, d\mu \right| \leq \int |g| \, d|\mu|.
$$

すべてのスカラー $\alpha \in \mathbf{C}$ と $X$ のすべてのメジャー $\mu$ について、
$$
|\alpha \mu| = |\alpha| \cdot |\mu|.
$$

一方、$\mu$と$\nu$が$X$の2小節で、$f$が$\mathscr{K}_+(X)$の写像、$g$が$\mathscr{K}(X; \mathbf{C})$の写像で$|g| \leq f$となる場合、
$$
\left| \int g \, d(\mu + \nu) \right| = \left| \int g \, d\mu + \int g \, d\nu \right| \leq \int f \, d|\mu| + \int f \, d|\nu|,
$$

よって

$$(15)$$
$$|\mu + \nu| \leq |\mu| + |\nu|.$$

同じ記法では、関係 $|g| \leq f$ と $|\overline{g}| \leq f$ は同等であるため、

$$(16)$$
$$|\overline{\mu}| = |\mu|.$$

(14)、(15)、(16) から次のことがわかります。

$$(17)$$
$$|\mathscr{R}\mu| \leq |\mu|,\quad |\mathscr{I}\mu| \leq |\mu|,\quad |\mu| \leq |\mathscr{R}\mu| + |\mathscr{I}\mu|.$$

#### 命題 8 {#int-iii-s1-prop-8 .statement tag=08LL}

*$\mu$ が $X$ のメジャーである場合、写像 $h \in \mathscr{C}(X; \mathbf{C})$ ごとに、*

$$(18)$$
$$|h \cdot \mu| \leq |h| \cdot |\mu|.$$

なぜなら、$f \in \mathscr{K}_+(X)$ と $g \in \mathscr{K}(X; \mathbf{C})$ が $|g| \leq f$ である場合、(13) より、$|\int gh d\mu| \leq \int |gh| d|\mu| \leq \int f|h| d|\mu|$ となり、(18) が証明されます。

### 7. 拡大までの小節の定義

$X$ を局所的にコンパクトな空間とします。 $V$ が $\mathscr{K}(X; \mathbf{C})$ の*稠密* 線形部分空間である場合、$X$ の 2 つのメジャー $\mu_1, \mu_2$ と $V$ の一致するが等しく、$V$ のすべての線型形式が連続していることは明らかです。 $\mathscr{K}(X; \mathbf{C})$ の位相は、(一方向のみで) $X$ の小節まで拡張される可能性があります。積極的な対策としては、次のような基準が便利です。

#### 命題 9 {#int-iii-s1-prop-9 .statement tag=08LM}

*$V$ を、次の性質を持つ $\mathscr{K}(X; \mathbf{R})$ の線形部分空間とします。
(P) $X$ の各コンパクト部分集合 $K$ に対して、$f \geq 0$ となり、すべての $x \in K$ に対して $f(x) > 0$ となるような写像 $f \in V$ が存在します。
これらの条件の下では、$\mathscr{K}(X; \mathbf{R})$ の順序によって誘発される順序に対して、$V$ 上のすべての正の線型形式が表されます (Ch. II, §2, No. 1、デフォルト。 1) は、$X$ で正の尺度に拡張される可能性があります (これは、$\mathscr{K}(X; \mathbf{R})$ で $V$ が密である場合に固有です)。
写像 $f \in \mathscr{K}(X; \mathbf{R})$ ごとに、$K$ をサポートすると、$f \leq g$ となるような写像 $g \in V$ が存在します。なぜなら、$V$には写像$h \geq 0$が存在し、すべての$x \in K$に対して$h(x) > 0$となるからです。 設定 $\alpha = \inf_{x \in K} h(x)$ であるため、$\alpha > 0$ があり、写像 $g = (\alpha^{-1} \|f\|)h$ が要件を満たします。 その後、Th を適用するだけで十分です。 No. 5 の 1 および TVS の提案 1、II, §3, No. 1.*

### 8. 限定された措置

X をローカルコンパクト空間とします。 $\mathscr{C}^b(X; \mathbf{C})$ の$\mathscr{K}(X; \mathbf{C})$ の位相は、$\mathscr{K}(X; \mathbf{C})$ の直接の極限位相よりも粗いため、X の測定は、X の一様収束の位相に対して連続するとは限りません。

#### 定義 3 {#int-iii-s1-def-3 .statement tag=08LN}

*局所的にコンパクトな空間 X は、一様収束の位相に対して $\mathscr{K}(X; \mathbf{C})$ で連続である場合、有界であると言われます。

有限の数 $M \geq 0$ が存在し、すべての写像 $f \in \mathscr{K}(X; \mathbf{C})$ に対して、

$$
|\mu(f)| \leq M \|f\|
$$

(ここで、$\|f\|$ は No. 2 の公式 (3) によって定義されます)。

したがって、$\mu$ が制限された尺度であると言うのは、$\mu$ 属するを空間 $\mathscr{K}(X; \mathbf{C})$ を $\|f\|$ で正規化したものであることを意味します。この双対を $\mathscr{M}^1(X; \mathbf{C})$ (または、混乱が生じない場合は単に $\mathscr{M}^1(X)$) で表すことにします。 $\mathscr{M}^1(X; \mathbf{C})$ にはノルムが装備されており、$\|\mu\|$ は数 $M \geq 0$ の最小のであり、写像 $f \in \mathscr{K}(X; \mathbf{C})$ ごとに不等式 (19) が成り立つことがわかります。

$$
\|\mu\| = \sup_{\|f\| \leq 1,\ f \in \mathscr{K}(X; \mathbf{C})} |\mu(f)| .
$$

このノルムを装備した$\mathscr{M}^1(X; \mathbf{C})$は、バナッハ空間であることが知られています（TVS、III, §3, No. 8、提案12のCor.2）。

公式 (20) による $\|\mu\|$ の定義は、X のすべての小節 $\mu$ に拡張でき、言葉の乱用により、$\|\mu\|$ は再び $\mu$ のノルムであると言われます。 $\mu$ が有限であるためには、$\|\mu\|$ が有限であることが必要かつ十分です。

X がコンパクトな場合、X のすべての小節は有界になります。

#### 例 {#int-iii-s1-n8-exa-1 .statement tag=08LO}

— 1) 点 $a \in X$ の単位元質量によって定義される尺度 $\varepsilon_a$ は有界であり、$\|\varepsilon_a\| = 1$ です。

2) $\mathbf{R}$ のルベーグ測度は有界ではありません。実際、整数 $n > 0$ ごとに $[0, 1]$ の値を含む写像 $f \in \mathscr{K}(\mathbf{R}; \mathbf{C})$ が存在し、区間 $[ -n, n ]$ (No. 2, 補題 1) では 1 に等しくなります。したがって $\|f\| = 1$ と

$$
\int_{-\infty}^{+\infty} f(x)\, dx \geq \int_{-n}^{n} f(x)\, dx = 2n ,
$$

これは、有限の数 M 満たす関係 (19) が存在しないことを証明します。

3) 実直線 $\mathbf{R}$、写像に

$$
f \mapsto \int_{-\infty}^{+\infty} \frac{f(x)\,dx}{1 + x^2}
$$

写像 $f \in \mathscr{H}(\mathbf{R}; \mathbf{C})$ ごとに、

$$
\left| \int_{-\infty}^{+\infty} \frac{f(x)\,dx}{1 + x^2} \right| \leq \|f\| \int_{-\infty}^{+\infty} \frac{dx}{1 + x^2} = \pi \cdot \|f\|.
$$

関係 $\|f\| \leq 1$ と $\|\overline{f}\| \leq 1$ は同等であるため、(20) から次のようになります。

(21)
$$
\|\overline{\mu}\| = \|\mu\|
$$
$X$ の $\mu$ 小節ごとに。

#### 命題 10 {#int-iii-s1-prop-10 .statement tag=08LP}

— *$X$* の $\mu$ 小節ごとに、

(22)
$$
\|\mu\| = \sup_{0 \leq f \leq 1,\ f \in \mathscr{H}(X; \mathbf{R})} |\mu|(f).
$$

なぜなら、公式 (12) が定義するメジャーの絶対値であることを考慮すると、(22) の 2 番目の要素は次のように書くことができます。

$$
\sup_{0 \leq f \leq 1,\ f \in \mathscr{H}(X; \mathbf{R})} \left( \sup_{|g| \leq f,\ g \in \mathscr{H}(X; \mathbf{C})} |\mu(g)| \right) = \sup_{\|g\| \leq 1,\ g \in \mathscr{H}(X; \mathbf{C})} |\mu(g)|.
$$

#### 系 1 {#int-iii-s1-prop-10-cor-1 .statement tag=08LQ}

— *$X$の各小節$\mu$、$\mu$と$|\mu|$のノルムは等しい。 $\mu$ は、$|\mu|$ が制限されている場合にのみ制限されます。*

#### 系 2 {#int-iii-s1-prop-10-cor-2 .statement tag=08LR}

— *コンパクト空間 $X$ の各小節 $\mu$ について、*

(23)
$$
\|\mu\| = |\mu|(1) = \int d|\mu|.
$$

この公式は、第 3 章で一般化されます。 IV, §4, No. 7。

*コンパクト* 空間 $X$ では、$X$ 複素数 $\mu(1)$ 上のすべての (複素) メジャー $\mu$ について、$\mu$ の *総質量* と呼ばれます。 $\mu$ が *正* の場合、その総質量はそのノルムに等しくなります。 $\mu$ が、総質量が 1 に等しい*コンパクト* 空間 $X$ における正の尺度である場合、連続写像 $f \in \mathscr{C}(X; \mathbf{C})$ に対するその値 $\mu(f)$ は、その尺度に関する $f$ の *平均* であるとも言えます。 $\mu$。

#### 系 3 {#int-iii-s1-prop-10-cor-3 .statement tag=08LS}

— ローカルコンパクト空間 $X$ 上の各実際のメジャー $\mu$ に対して、

$$
\| \mu \| = \sup_{\| f \| \leq 1,\ f \in \mathscr{K}(X; \mathbf{R})} | \mu(f) | .
$$

$\mu$ が実測度であり、$f \in \mathscr{K}_+(X)$ である場合、$|\mu|(f)$ については、公式 (22) と式 (9) を使用するだけで十分です。

したがって、有界実測度の集合は、標準の空間 $\mathscr{K}(X; \mathbf{R})$ の双数です。混乱が生じない場合は、$\mathscr{M}^1(X, \mathbf{R})$、または $\mathscr{M}^1(X)$ と表されます。 標準単射 $\mathscr{M}^1(X, \mathbf{R}) \to \mathscr{M}^1(X; \mathbf{C})$ は、(24) によるアイソメ図です。

#### 命題 11 {#int-iii-s1-prop-11 .statement tag=08LT}

— $\mu$ と $\nu$ が $X$ に対する 2 つのポジティブな指標である場合、 $\| \mu + \nu \| = \| \mu \| + \| \nu \|$ です。

たとえば、写像 $f \in \mathscr{K}(X; \mathbf{R})$ では、関係 $\leq$ に対して $0 \leq f \leq 1$ 形有向集合 $S$ となります。したがって、$X$ の正の測度 $\mu$ については、(22) と単調極限定理から $\| \mu \| = \lim_{f \in S} \mu(f)$ が得られます。その後、命題の結論がすぐに続きます。

#### 系 1 {#int-iii-s1-prop-11-cor-1 .statement tag=08LU}

— $\mu$ と $\nu$ が $X$ に対して $\mu \leq \nu$ となる 2 つの肯定的な指標である場合、$\| \mu \| \leq \| \nu \|$。特に、$\nu$ が有界であれば、$\mu$ も有界です。
なるほど、$\| \nu \| = \| \mu \| + \| \nu - \mu \|$。

#### 系 2 {#int-iii-s1-prop-11-cor-2 .statement tag=08LV}

— $X$ の実際のメジャー $\mu$ ごとに、

$$
\| \mu \| = \| \mu^+ \| + \| \mu^- \|.
$$

(提案 10 の補正 1) については、$\mu$ のノルムは $|\mu| = \mu^+ + \mu^-$ のノルムと等しいです。

#### 命題 12 {#int-iii-s1-prop-12 .statement tag=08LW}

— $\mu$ が $X$ の有界メジャーであり、$g$ が $X$ から $\mathbf{C}$ への有界連続写像である場合、メジャー $g \cdot \mu$ は有界であり、$\| g \cdot \mu \| \leq \| g \| \cdot \| \mu \|$ です。

写像 $f \in \mathscr{K}(X; \mathbf{C})$ ごとに、

$$
|\mu(fg)| \leq \| \mu \| \cdot \| fg \| \leq \| \mu \| \cdot \| g \| \cdot \| f \|.
$$

### 9. 空間の対策について曖昧な位相

$X$ をローカルコンパクト空間とします。 空間 $\mathscr{M}(X; \mathbf{C})$ では、$\mathscr{K}(X; \mathbf{C})$ の点ごとの収束の位相を考えることができます。これを、$\mathscr{M}(X; \mathbf{C})$ の曖昧な位相と呼びます。

$\mathscr{K}(X; \mathbf{C}) = \mathscr{K}(X; \mathbf{R}) + i \mathscr{K}(X; \mathbf{R})$ 以降、$\mathscr{M}(X; \mathbf{C})$ のあいまいな位相は *準規範* $\sup_{1 \leq i \leq n} |\mu(f_i)|$ によって定義されます。ここで、$(f_i)_{1 \leq i \leq n}$ は $\mathscr{K}(X; \mathbf{R})$ (または $\mathscr{K}_+(X)$) の写像のいずれかの有限列です。 $\mathscr{M}(X; \mathbf{C})$ 上のフィルター $\mathfrak{F}$ がメジャー $\mu_0$ に *漠然と収束* すると言うことは、次のことを意味します。

$$
\mu_0(f) = \lim_{\mu, \mathfrak{F}} \mu(f)
$$

写像 $f \in \mathscr{K}(X; \mathbf{R})$ ごとに。 写像 $f \in \mathscr{K}(X; \mathbf{C})$ ごとに、写像 $\mu \mapsto \mu(f)$ は、空間 $\mathscr{M}(X; \mathbf{C})$ で *漠然と連続* 線型形式になります。

#### 命題 13 {#int-iii-s1-prop-13 .statement tag=08LX}

*X を局所コンパクト空間とし、$x \in X$ ごとに、$\varepsilon_x$ を点 x でのディラック測度とする。 写像 $x \mapsto \varepsilon_x$ は、X の小節の空間 $\mathscr{M}(X; \mathbf{C})$ の部分空間への X の同型写像であり、曖昧な位相を備えています。さらに、$X'$がX点を無限遠$\omega$で隣接して得られるコンパクト空間を表す場合、xが$\omega$になる傾向があるように、$\varepsilon_x$は0になる傾向があります。

写像 $f \in \mathscr{K}(X; \mathbf{C})$、$\langle f, \varepsilon_x \rangle = f(x)$ ごとに; $f$ は連続であるため、これは写像 $x \mapsto \varepsilon_x$ が連続であることを証明します。 $x, y$ が X の 2 つの異なる点である場合、$f(x) = 1, f(y) = 0$ (No. 2, 補題 1) となる写像 $f \in \mathscr{K}(X; \mathbf{C})$ が存在します。これは、$\varepsilon_x \neq \varepsilon_y$ であることを証明します。したがって、写像 $x \mapsto \varepsilon_x$ は単射法です。さらに、写像 $f \in \mathscr{K}(X; \mathbf{C})$ ごとに、$x$ が $\omega$ になる傾向があるように、$\langle f, \varepsilon_x \rangle$ は定義までに 0 になる傾向があるため、$x \mapsto \varepsilon_x$ に値 0 を代入することで連続性によって $X' = X \cup \{ \omega \}$ まで拡張できます。 点 $\omega$。すべての $x \in X$ に対して $\varepsilon_x \neq 0$ であるため、この拡張された写像も単射法です。したがって、$\mathscr{M}(X; \mathbf{C})$ は曖昧な位相 (GT, I, §9, No. 4, Cor. 2 of Th. 2) のハウスドルフであるため、これはコンパクトな空間 $X'$ の $\mathscr{M}(X; \mathbf{C})$ の部分空間への同型写像です。

#### 命題 14 {#int-iii-s1-prop-14 .statement tag=08LY}

*局所的にコンパクトな空間Xに関する対策の空間$\mathscr{M}(X; \mathbf{C})$では、曖昧な位相*から推定されるユニフォーム構造に対する積極的対策のコーン$\mathscr{M}_+(X)$が完成します（したがって、$\mathscr{M}(X; \mathbf{C})$では*漠然と閉じられています*）。

というのは、$\mathscr{M}_+(X)$ 上のあいまいな一様性構造に対する Cauchy フィルター $\Phi$ を考えてみましょう。 定義により、写像 $f \in \mathscr{K}(X; \mathbf{C})$ ごとに $\mu_0(f) = \lim_{\mu, \Phi} \mu(f)$ が存在し、拡大不等式の原理により、写像 $f \in \mathscr{K}_+(X)$ ごとに $\mu_0(f) \geq 0$ が存在します。したがって、$\mu_0$ は X (No. 5、Th. 1) に対するプラスの尺度であることがわかります。

空間 $\mathscr{M}(X; \mathbf{C})$ (または $\mathscr{M}(X; \mathbf{R})$) 自体は、曖昧なユニフォーム構造 (TVS、II, §6, No. 7) に対して*必ずしも完全ではない*ことに注意する必要があります。

#### 系 {#int-iii-s1-n9-cor-1 .statement tag=08LZ}

*A と B が 2 つで、$\mathscr{M}_+(X)$ の漠然と閉じている部分集合である場合、$A + B$ は $\mathscr{M}_+(X)$ で漠然と閉じています (したがって、$\mathscr{M}(X; \mathbf{C})$ でも同様です)。

これは実際には、局所的に凸状の空間における弱く完全で適切な錐体の一般的な性質です (TVS、II, §6, No. 8、提案 11 の Cor. 2)。

#### 命題 15 {#int-iii-s1-prop-15 .statement tag=08M0}

— $H$ を $\mathscr{M}(X; \mathbf{C})$ の部分集合とします。次のプロパティは同等です。

a) $H$ は漠然と境界が定められています。
b) $H$ は漠然と比較的コンパクトです。
c) $H$ は等連続です。
d) $X$ のすべてのコンパクト部分集合 $K$ に対して、すべての小節 $\mu \in H$ およびすべての写像 $f \in \mathscr{K}(X, K; \mathbf{C})$ に対して $|\mu(f)| \leq M_K \|f\|$ となるような数 $M_K \geq 0$ が存在します。

$\mathscr{K}(X; \mathbf{C})$ はバレル化された空間 (No. 1、提案 2) であるため、プロパティ a)、b)、および c) の同値は TVS、III, §4, No. 1、Scholium から続きます。

d) が a) を意味することは明らかです。最後に、$H$ が等連続である場合、$\mu \in H$ から $\mathscr{K}(X, K; \mathbf{C})$ までの尺度の制限の集合も等連続です、$\mathscr{K}(X, K; \mathbf{C})$ は標準の空間であるため、よって条件 d)。

\* 第 3 章で見てみましょう。 IV, §4, No. 6、命題 15 の条件は、$X$ の各コンパクト部分集合 $K$ に対して、各小節 $\mu \in H$ に対して $|\mu|(K) \leq M_K$ となる定数 $M_K$ が存在するという条件とも等価です。

#### 系 1 {#int-iii-s1-prop-15-cor-1 .statement tag=08M1}

— $\nu$ を $X$ に対する肯定的な尺度とします。 $|\mu| \leq \nu$ が漠然とコンパクトになるように、$\mu$ の措置を集合実行します。

#### 系 2 {#int-iii-s1-prop-15-cor-2 .statement tag=08M2}

— $\|\mu\| \leq a$ ($a$ 任意の有限数 $> 0$) が漠然とコンパクトになるようなメジャー $\mu$ の集合。

#### 系 3 {#int-iii-s1-prop-15-cor-3 .statement tag=08M3}

— $X$ がコンパクトな場合、$X$ に対する積極的な手段 $\mu$ の集合により、$\|\mu\| = 1$ は漠然とコンパクトになります。

なぜなら、それは、関係 $\mu \geq 0$ と $\mu(1) = 1$ (No. 8、提案 10 の Cor. 2) によってそれぞれ定義される、$\|\mu\| \leq 1$ と漠然と閉じた集合のような、漠然とコンパクトな措置集合 (Cor. 2) の共通部分であるからです。

#### 系 4 {#int-iii-s1-prop-15-cor-4 .statement tag=08M4}

— 空間 $\mathscr{M}(X; \mathbf{C})$ では、写像 $\mu \mapsto \|\mu\|$ は曖昧な位相に対して下位半連続です。

これは系 2 の明らか帰結です。

$\mathscr{M}(X; \mathbf{C})$ の写像 $\mu \mapsto |\mu|$ 自体は、曖昧な位相に対して必ずしも連続的ではないことに注意する必要があります (Exer. 9)。

#### 命題 16 {#int-iii-s1-prop-16 .statement tag=08M5}

— $K$ を $X$ のコンパクトな部分集合、$H$ を漠然と境界のある $\mathscr{M}(X; \mathbf{C})$ の部分集合とします。すると、$\mathscr{K}(X, K; \mathbf{C})$が一様収束の位相と曖昧な位相を備えた$H$が装備されているとき、双線形形式$(f, \mu) \mapsto \langle f, \mu \rangle$は$\mathscr{K}(X, K; \mathbf{C}) \times H$で連続します。

なぜなら、次のような数 $M \geqslant 0$ が存在するからです。
$$
|\mu(f)| \leqslant M \|f\|
$$
写像 $f \in \mathscr{K}(X, K; \mathbf{C})$ およびすべての小節 $\mu \in H$ に対して (提案 15)。 $\mu_0$と$\mu$が所属から$H$までの2小節、$f_0$と$f$が$\mathscr{K}(X, K; \mathbf{C})$の写像の2小節である場合、
$$
|\mu(f) - \mu_0(f_0)| = |\mu(f - f_0) + \mu(f_0) - \mu_0(f_0)| \\
\leqslant M \|f - f_0\| + |\mu(f_0) - \mu_0(f_0)|,
$$
そして、$\|f - f_0\|$と$|\mu(f_0) - \mu_0(f_0)|$の場合、最後の数量は恣意的に小さくなり、命題が証明されます。

### 10. $\mathscr{M}(X; \mathbf{C})$ でのコンパクトなコンバージェンス

$\mathscr{M}(X; \mathbf{C})$ 上の *コンパクト収束* の位相は、$\mathscr{K}(X; \mathbf{C})$ のコンパクト部分集合における一様収束の位相であることを思い出してください。 $\mathscr{K}(X; \mathbf{C})$ の厳密にコンパクトな部分集合 (No. 1) における一様収束の $\mathscr{M}(X; \mathbf{C})$ 位相に対する厳密にコンパクトな収束の *位相* を呼びます。

#### 命題 17 {#int-iii-s1-prop-17 .statement tag=08M6}

* 空間 $\mathscr{M}(X; \mathbf{C})$ では、次のトポロジを考慮します。*
$\mathscr{T}_1$: * $\mathscr{K}(X; \mathbf{C})$ の合計部分集合 T における点ごとの収束の位相;*
$\mathscr{T}_2$: *曖昧位相;*
$\mathscr{T}_3$: *位相の厳密にコンパクトな収束;*
$\mathscr{T}_4$: *位相のコンパクトなコンバージェンス。*
*これらの各トポロジーは、次のトポロジーよりも粗くなっています。さらに:*
*(i)* *有限の集合は、$\mathscr{T}_2$、$\mathscr{T}_3$、$\mathscr{T}_4$ で同じです。*
*(ii)* *H が $\mathscr{M}(X; \mathbf{C})$ の漠然とした境界のある部分集合である場合、トポロジー $\mathscr{T}_1$、$\mathscr{T}_2$、$\mathscr{T}_3$、$\mathscr{T}_4$ によって H に誘導されるトポロジーは同一です。*

$\mathscr{M}(X; \mathbf{C})$ の漠然と境界のある部分集合 $H$ は等連続です (No. 9、提案 15)。従って、最初の主張は TVS、III, §3, No. 7、提案 9 から続き、2 番目は GT、X, §2, No. 4、Th から続きます。 1.

$X$ が *パラコンパクト* の場合、厳密にコンパクトな収束のトポロジーはコンパクトな収束のトポロジーと一致することを思い出してください (No. 1、提案 2)。

#### 命題 18 {#int-iii-s1-prop-18 .statement tag=08M7}

*円錐 $\mathscr{M}_+(X)$ では、次のトポロジー 一致するによって引き起こされるトポロジー:*
$\mathscr{T}_1$: * $\mathscr{K}(X; \mathbf{C})$ で密で、性質 (P) (No. 7、提案 9) を満たす、$\mathscr{K}(X; \mathbf{C})$ の線形部分空間 V における点収束の位相;*

\textit{\mathscr{T}_2: 曖昧な位相;}

\textit{\mathscr{T}_3: 厳密にコンパクトな収束の位相。}

すべてのフィルターは、それよりも限外フィルター より細かいの共通部分であるため (GT、I, §6, No. 4、提案 7)、$\mathfrak{U}$ が位相 $\mathscr{T}_1$ の尺度 $\mu_0$ に収束する $\mathscr{M}_+(X)$ の限外フィルターである場合、次のことを示すだけで十分です。 $\mathscr{T}_3$ に対しても $\mu_0$ に収束します。 $K$ を $X$ の圧縮部分集合とします。 仮定までに、$X$には$\geqslant 0$である写像$h \in V$が存在し、$K$には値$> 0$がかかります。つまり、すべての写像 $f \in \mathscr{K}(X, K; \mathbf{C})$ は $f = gh$ と $g \in \mathscr{K}(X, K; \mathbf{C})$ で記述でき、$c = \inf_{x \in K} h(x) > 0$ の場合は $\|g\| \leqslant c^{-1}\|f\|$ となります。 仮定までに、集合 $H_0 \in \mathfrak{U}$ が存在し、$\mu \in H_0$ の小節ごとに、

$$
0 \leqslant \mu(h) \leqslant \mu_0(h) + 1 = b.
$$

従って、写像 $f \in \mathscr{K}(X; \mathbf{C})$ ごとに、

$$
|\langle f, h \cdot \mu \rangle| = |\langle hf, \mu \rangle| \leqslant \|f\| \cdot \mu(h) \leqslant b \|f\|
$$

すべてのメジャー $\mu \in H_0$;これは、$\mu$ が $H_0$ を超える小節 $h \cdot \mu$ の集合 $H$ が \emph{曖昧な境界} であることを証明します。 $\mathfrak{U}_0$ が $H_0$ の $\mathfrak{U}$ によって誘発された限外濾過器である場合、写像 $\mu \mapsto h \cdot \mu$ の下の $\mathfrak{U}_0$ の像は、$H$ の$\mathfrak{F}$ の限外濾過器の基底であり、$H$ 以降はは厳密にコンパクトな収束 (提案 17 および No. 9、提案 15) の位相に対して比較的コンパクトであり、この位相に対して $\mathfrak{F}$ はメジャー $\nu_0$ に収束します。他の語では、任意の $\varepsilon > 0$ および $\mathscr{K}(X, K; \mathbf{C})$ の任意のコンパクト部分集合 $L$ に対して、$H_0$ 所属から $\mathfrak{U}$ までの部分集合 $N$ が存在します。 写像 $g \in L$ および $\mu, \mu'$ 所属から $N$ までの各対の小節には、$|\langle g, h \cdot \mu \rangle - \langle g, h \cdot \mu' \rangle| \leqslant \varepsilon$ があります。つまり、

$$
|\langle gh, \mu \rangle - \langle gh, \mu' \rangle| \leqslant \varepsilon.
$$

さて、上で写像 $g \mapsto gh$ がバナッハ空間 $\mathscr{K}(X, K; \mathbf{C})$ の \emph{自己同型} であることを見ました。したがって、$\mathfrak{U}$ は厳密にコンパクトな収束の位相に対する $\mathscr{M}_+(X)$ 上の \emph{Cauchy フィルター} であることを示しました。 \emph{A なおさら}、これは曖昧な収束のためのコーシー フィルターであり、No. 9 の提案 14 は、それが漠然と測度 $\mu_1$ に収束することを示しています。さらに、$V$ は $\mathscr{K}(X; \mathbf{C})$ で密であるため、仮定は $\mu_1 = \mu_0$ を意味します。最後に、$\mathfrak{U}$ は厳密にコンパクトな収束の位相に対するコーシー フィルターであるため、この位相に対しても $\mu_0$ に収束します (GT、X, §1, No. 5、提案 5)。

Q.E.D.

#### 系 {#int-iii-s1-n10-cor-1 .statement tag=08M8}

— *X がパラコンパクトである場合、コンパクト収束一致するの曖昧な位相と位相によって $\mathscr{M}_+(X)$ に誘導されるトポロジー。

ただし、X がパラコンパクトではない場合、コンパクト収束の位相と厳密にコンパクトな収束の位相によって $\mathscr{M}_+(X)$ に誘導されるトポロジーは異なる可能性があります (例 3)。

### 練習問題 {#int-iii-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
