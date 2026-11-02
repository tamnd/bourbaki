---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: SPACES OF CONTINUOUS LINEAR MAPPINGS
section: 6
section_title: Borel's graph theorem
lang: ja
source: evt-i-v
book_pages: TVS III.49-TVS III.50
pdf_pages: 0166-0169, 0181-0182
extraction: ocr
subsections:
    - "no": 1
      title: Borel’s graph theorem
      page: 34
      pdf_page: 166
    - "no": 2
      title: Locally convex Lusin spaces
      page: 34
      pdf_page: 166
    - "no": 3
      title: Measurable linear mappings on a Banach space $^1$
      page: 36
      pdf_page: 168
statements: 8
exercises: 6
content_sha256: e9eff302cfb7516bcba9f06804d52dc348b5db0d54c47c59c44fbd04adf6dafe
translated_from: content/en/evt/III/06_s6_borel_s_graph_theorem.md
translation_method: google
source_content_sha256: 207efa273694316acd7d5b27dedee7a3292c04e1a0a2e90cfe57fd450ad44773
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 32098450ee9e29cad47f06670bde699ca267356417fa2a07f7336d7c42f9d6b4
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 6。ボレルのグラフ定理

### 1. ボレルのグラフ定理

#### 定理 1 {#evt-iii-s6-thm-1 .statement tag=07Q4}

— E を局所凸空間とし、これは Banach 空間の帰納極限、F を Souslin 局所凸空間、たとえばルーシン空間 (GT、IX, § 6, No. 2、および No. 4)、および u 線形写像 E から F への変換とします。u のグラフの場合が E × F の Borel 部分集合である場合、u は連続です。

E_i をバナッハ空間の族とし、(u_i) を連続線形写像 u_i の族とする: E_i → E とし、E の位相が u_i が連続である最も細かい局所凸位相となるようにします。合成された写像 u ∘ u_i が連続であること、または実際 (GT, IX, § 2, No. 6, 提案 10) 制限 of u ∘ u_i からすべての閉じた部分空間 G of E_i 満たすの可算性の最初の公理が連続であることを証明するだけで十分です。この制限のグラフは、連続写像 u_i × Id_F : G × F → E × F の下での u のグラフの逆像なので、G × F のボレル集合です。 加法では、G × F はスーリン空間であり、すべてのボレルですスーリン空間の部分集合はスーリン空間 (GT、IX, § 6, No. 3、提案 10) です。 Th. th から 1 が続きます。 4、GT、IX, § 6, No. 8。

#### 注意 {#evt-iii-s6-n1-rem-1 .statement tag=07Q5}

(III、p. 12)、すべてのホモロジー ハウスドルフおよび半完全空間、たとえばすべてのフレシェ空間は、バナッハ空間の帰納極限であることを思い出してください。 \* これは、再帰フレシェ空間 (IV, p. 23, prop. 4) の強い双対にも当てはまります。 \*

### 2. 局所凸ルシン空間

#### 命題 1 {#evt-iii-s6-prop-1 .statement tag=07Q6}

— E を局所凸ハウスドルフ空間とします。 Fréchet 空間満たすの可算性の第一公理である数列 (E_n)_{n \in \mathbf{N}} と、E = \bigcup_{n \in \mathbf{N}} u_n(E_n) となる連続線形写像 u_n : E_n → E が存在するとします。するとEはルーシン空間になります。

P_n を u_n の核とします。次に、u_n 定義する商空間 E_n/P_n から u_n(E_n) への全単射連続写像です。 Since E_n/P_n is a Fréchet space satisfying the first axiom of countability (GT, IX, § 3, No. 1), hence a polish space (GT, IX, § 6, No. 1, def. 1), u_n(E_n) is a Lusin subspace of E (GT, IX, § 6, No. 4, prop. 11). 従って、GT、IX, § 6, No. 7、cor によって。の。レギュラー（GT、III, § 3, No. 1）の3、空間Eはルーシン空間です。

#### 例 1 {#evt-iii-s6-n2-exa-1 .statement tag=07Q7}

すべてのフレシェ空間満たすの可算性の最初の公理はポリッシュ空間であるため、ルーシン空間です。 Consequently, so are the spaces $\mathscr{C}(X)$, where X is locally compact and has a countable base (the topology of $\mathscr{C}(X)$ being that of compact convergence, cf. GT, X, § 3, No. 3, corollary and § 1, No. 6, cor. 3); \* the spaces $\mathscr{C}_0^\infty(U)$, where U is an open subset of $\mathbf{R}^n$ (III, p. 9) and $\mathscr{H}(U)$, where U is an open subset of $\mathbf{C}^n$ (III, p. 10).

提案 1 は、空間 $\mathscr{C}_0^\infty(U)$、U は $\mathbf{R}^n$ のオープン集合、$\mathscr{G}_s(I)$、I は $\mathbf{R}$ と $s \geq 1$ のコンパクト区間、および $\mathscr{H}(K)$、K はコンパクトであることを示しています。 $\mathbf{C}^n$ の部分集合はすべてルーシン空間 (III、p. 10) です。 \*

#### 定理 2 {#evt-iii-s6-thm-2 .statement tag=07Q8}

— E を局所凸空間とし、これは E の増加する数列 $(E_n)_{n \in \mathbf{N}}$ の部分空間の帰納的極限であり、可算性の最初の公理であるフレシェ空間満たすのトポロジーを備えています。 E のすべてのコンパクト部分集合が $E_n$ の 1 つに含まれており、この空間でコンパクトであるとします。 F を可算性の最初の公理であるフレシェ空間満たすとします。次に、空間 $\mathscr{L}_c(E; F)$ はルーシン空間です。

空間 E はボーンロジカル (III, p. 12) であるため、空間 $\mathscr{L}_c(E; F)$ は完全です (III, p. 23、提案 12)。 線形写像 $j : f \mapsto (f|E_n)_{n \in \mathbf{N}}$ は $\mathscr{L}_c(E; F)$ から積空間 $\prod_{n \in \mathbf{N}} \mathscr{L}_c(E_n; F)$ への単射です。 Eのコンパクトな部分集合上の仮定と$\mathfrak{S}$トポロジーの定義のおかげで、$j$は$\mathscr{L}_c(E; F)$からその像への同型になります（積によって誘導された位相が付与されています） 位相);さらに、$\mathscr{L}_c(E; F)$ が完了しているため、この像は、$\prod_{n \in \mathbf{N}} \mathscr{L}_c(E_n; F)$ (GT、II, § 3, No. 4、提案 8) のクローズド部分空間です。 GT IX, § 6, No. 4 により、空間 $\mathscr{L}_c(E; F)$ のそれぞれがルーシン空間であることを証明するのに十分です。 証明の残りについては、E が可算性の最初の公理であるフレシェ空間満たすであると仮定します。

F は可算性の最初の公理であるフレシェ空間満たすであるため、バナッハ空間 $F_n$ の可算数積の閉部分空間と同型であり、それぞれは F の商 (II, p. 5)、従って、可算性の最初の公理を満たします。 線形写像 $j' : f \mapsto (\mathrm{pr}_n \circ f)_{n \in \mathbf{N}}$ は、$\mathscr{L}_c(E; F)$ から積空間 $\prod_{n \in \mathbf{N}} \mathscr{L}_c(E; F_n)$ への単射であり、$\mathfrak{S}$ トポロジの定義と、積のオープン集合を使用することにより、 $j'$は、$\mathscr{L}_c(E; F)$から像への同型です。また、$\mathscr{L}_c(E; F)$が完了しているため、この像は$\prod_{n \in \mathbf{N}} \mathscr{L}_c(E; F)$のクローズド部分空間となります。従って、空間 $\mathscr{L}_c(E; F_n)$ のそれぞれがルーシン空間 (GT, IX, § 6, No. 4) であることを証明すれば十分であり、その結果、F は可算性の最初の公理である Banach 空間満たすであると仮定できます。

空間 $\mathscr{L}_c(E; F)$ は、等連続で閉じた部分集合の可算族の和集合 (III、p. 19、cor. 1 および GT、X, § 2, No. 3、prop. 6)。しかし、$\mathscr{L}_c(E; F)$ のすべての等連続部分集合 H は計数可能であり、可算性の最初の公理 (III, p. 18, prop. 6 および GT, X, § 2, No. 4, th. 1) を満たします。 H が閉じている場合、$\mathscr{L}_c(E; F)$ の制服構造は完全な空間です。なぜなら、後者は完全だからです。他の語では、H はポリッシュ空間であり、*なおさら* はルーシン空間です。従って、通常の空間 $\mathscr{L}_c(E; F)$ は Lusin 空間 (GT、IX, § 6, No. 7、th. 3 の cor.) です。

#### 系 {#evt-iii-s6-n2-cor-1 .statement tag=07Q9}

— *E が th と同じであるという仮説。 2、加法では、E のすべての有界な部分集合が比較的コンパクトであると仮定します。このとき、E の強い双対は、ルーシン空間です。* *特に、モンテル空間でもある可算性の最初の公理であるフレシェ空間満たすの強い双対は、ルーシン空間です。

\* 例 2. — U を $\mathbf{R}^n$ のオープン部分集合にします。 系は、特にフレシェ空間 $E = \mathscr{C}_c^\infty(U)$ に適用されます。そのデュアル $\mathscr{C}_c^{-\infty}(U)$ (U でコンパクト サポートを備えたディストリビューションの空間) は Lusin 空間になります。

空間 $\mathscr{C}_c^\infty(U)$ は、可算性の最初の公理 (III, p. 9) である Fréchet 空間 $\mathscr{C}_{K_n}^\infty(U)$ 満たすの数列の厳密な帰納法極限です。それぞれの空間 $\mathscr{C}_{K_n}^\infty(U)$ がモンテル空間であることを示すことができます。 加法では、$\mathscr{C}_c^\infty(U)$ のすべての境界付き部分集合は、空間 $\mathscr{C}_{K_n}^\infty(U)$ の 1 つに含まれます (III、p. 5、提案 6)。次に、 の系を適用できます。 2. 次に、$\mathscr{C}_c^\infty(U)$ の二重$\mathscr{C}_c^{-\infty}(U)$ (U の分布の空間) は、強い位相のルーシン空間です。

同様に、$\mathbf{C}^n$ のすべてのオープン部分集合 U、および $\mathbf{C}^n$ のすべてのコンパクト部分集合 K について、$\mathscr{H}(U)$ の強い双対と $\mathscr{H}(K)$ の強い双対が Lusin 空間であることを証明します。 \*

#### 注意 {#evt-iii-s6-n2-rem-1 .statement tag=07QA}

— E を th のようにします。 2; F を局所凸ハウスドルフ空間とします。これは連続線形写像 $u_n : F_n \to F$ の像の数列の和集合であり、各 $F_n$ はフレシェ空間満たすです可算性の最初の公理。その場合、$\mathscr{L}_c(E ; F)$ はルーシン空間です。プロップのように。 1、まず簡約するがそれぞれの $u_n$ が単射である場合を考えます。次に、証明のように。 2 では、E は可算性の最初の公理であるフレシェ空間満たすであると仮定できます。次に、I、p. 20、プロップ。 1、$\mathscr{L}(E ; F)$は$\mathscr{L}(E ; F_n)$の和集合です。さらに、標準単射 $\mathscr{L}_c(E ; F_n) \to \mathscr{L}_c(E ; F)$ は連続です (GT、X, § 1, No. 4、提案 3)。 空間 $\mathscr{L}_c(E ; F_n)$ はそれぞれ th によるルーシン空間であるため。 2、$\mathscr{L}(E ; F_n)$ は、$\mathscr{L}_c(E ; F)$ のルーシン位相に対するルーシン空間でもあります (GT、IX, § 6, No. 4、提案 11)。従って、$\mathscr{L}_c(E ; F)$ は GT、IX, § 6, No. 7、系のおかげで Lusin 空間になります。 3.

### \*3. Banach 線形写像空間 $^1$ で測定可能

#### 命題 2 {#evt-iii-s6-prop-2 .statement tag=07QB}

— *E をバナッハ空間、F を局所凸空間、u 線形写像 E から F にするとします。F のすべての閉じた部分集合 B、E のすべてのコンパクト部分集合 X およびすべての小節 $\mu$ について仮定しますX、共通部分 $X \cap u^{-1}(B)$ は $\mu$ で測定可能です。その場合、u は連続です。*

まず、F が基礎体であると仮定します。 E のすべてのコンパクト部分集合 X と X のすべての小節 $\mu$ について、$u$ から X の制限は $\mu$ 測定可能です (INT、IV)。 $u$ が連続していないとします。次に、整数 $n$ ごとに $\sum_n \| x_n \| < \infty$ と $|u(x_n)| \geq n$ となるように、E で点 $(x_n)$ の数列を見つけることができます。立方体 $C = [0, 1]^{\mathbf{N}}$ から E への写像 $g : (t_n) \mapsto \sum_n t_n x_n$ を考えます。 $g$ が連続であることは明らかです。従って、$f = u \circ g$ は、C (INT、V) のすべてのメジャーで測定可能です。特に、Cの因子に対するルベーグ測度の積である$\mu$の測度についてはそうです。従って、$\mu(D) > \frac{1}{2}$ となり、D に対する $f$ の制限が連続であるような C のコンパクト部分集合 D が存在し、したがって有界でもあります。 M を D 上の $|f|$ の上界とし、$p \in \mathbf{N}$ を $p \geq 4M$ となるようにします。 $s = (s_n)$ と $t = (t_n)$ を、すべての $n \neq p$ に対して $s_n = t_n$ となるように、D の 2 つの点とします。それから

$$
f(s) - f(t) = u(\sum_n s_n x_n - \sum_n t_n x_n) = (s_p - t_p) u(x_p) .
$$

$|f(s) - f(t)| \leq 2M$ と $|u(x_p)| \geq p \leq 4M$ なので、次のようになります。

$$
|s_p - t_p| \leq \frac{1}{2} .
$$

Lebesgue-Fubini 定理 (INT、V、第 2 版、§ 8, No. 3、提案 7 の cor. 2) は、$\mu(D) \leq \frac{1}{2}$ を示唆しています。これは矛盾を生じます。したがって、$u$ は連続です。

一般的な場合、前述の引数により、すべての $v \in F'$ に対して、線型形式 $v \circ u$ は連続です。 $(x_n)_{n \in \mathbf{N}}$ を 0 に向かう E の点の数列とします。 F に位相 $\sigma(F, F')$ が割り当てられている場合、数列 $(u(x_n))_{n \in \mathbf{N}}$ は F で 0 になる傾向があります。したがって、この数列は $\sigma(F, F')$ に限定され、F (III、p. 27、cor. 3) に限定されます。 E はボーンロジカルなので (III, p. 12, prop. 2); 線形写像 $u : E \to F$ は連続です。 \*

$^1$ この切断の結果は統合の本に依存します。

練習問題

### 練習問題 {#evt-iii-s6-exercises}

[§ 6 に対して練習問題](exercises/s6/)を参照してください。
