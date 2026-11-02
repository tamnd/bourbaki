---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 2
section_title: Convex sets
lang: ja
source: evt-i-v
book_pages: TVS II.7-TVS II.21
pdf_pages: 0044-0058, 0102-0109
extraction: ocr
subsections:
    - "no": 1
      title: Definition of a convex set
      page: 7
      pdf_page: 44
    - "no": 2
      title: Intersections of convex sets. Products of convex sets
      page: 9
      pdf_page: 46
    - "no": 3
      title: Convex envelope of a set
      page: 9
      pdf_page: 46
    - "no": 4
      title: Convex cones
      page: 10
      pdf_page: 47
    - "no": 5
      title: Ordered vector spaces
      page: 12
      pdf_page: 49
    - "no": 6
      title: Convex cones in topological vector spaces
      page: 13
      pdf_page: 50
    - "no": 7
      title: Topologies on ordered vector spaces
      page: 15
      pdf_page: 52
    - "no": 8
      title: Convex functions
      page: 16
      pdf_page: 53
    - "no": 9
      title: Operations on convex functions
      page: 18
      pdf_page: 55
    - "no": 10
      title: Convex functions over an open convex set
      page: 18
      pdf_page: 55
    - "no": 11
      title: Semi-norms and convex sets
      page: 19
      pdf_page: 56
statements: 51
exercises: 43
content_sha256: dbd72474c2fdb1c3ff4aa363b1abff32ea46d0435599f840d90c99ca072d3cc6
translated_from: content/en/evt/II/02_s2_convex_sets.md
translation_method: google
source_content_sha256: a0e92c270cc61535db50016db128351dc2a69eca0c0c5a5f6017a665abb322f1
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 85f1758a455d5b5f566893884281177f833ad54ee785e4c7e6e65819c33f6ba8
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 2。 Convex 集合

### 1. 凸の定義集合

For any two 点 $x, y$ of an affine 空間 $E$, 集合 of 点 $\lambda x + \mu y$ where $\lambda \geq 0, \mu \geq 0, \lambda + \mu = 1$ is called the closed segment with end 点 $x$ and $y$; $x = y$のときは簡約するから点です。 このセグメントの $x$ の補数は、$x$ で開き、$y$ で閉じた端点 $x, y$ を持つセグメントと呼ばれます。 $x = y$ の場合は空です。 最後に、終端点 $x, y$ を持つ閉セグメント内の $\{ x, y \}$ の補数は、終端点 $x, y$ を持つ開セグメントと呼ばれます。 $x = y$のときは空です。

#### 定義 1 {#evt-ii-s2-def-1 .statement tag=07B4}

— アフィン空間 $E$ の部分集合 $A$ は、$A$ の 2 つの点 $x, y$ ごとに、終端点 $x, y$ を持つ閉セグメントが $A$ に含まれる場合、凸になります。

$(1 - \lambda) a + \lambda x = a + \lambda (x - a)$ と同様に、この定義は次と同等です。 集合 $A$ は、点 $a \in A$、$A$ の変換に中心 $a$ のホモテティー と比率を乗じた場合、凸になります。 $\lambda$ ここで、$0 < \lambda < 1$ は $A$ に含まれています (他の語では、$A$ はこれらの相同性に対して安定です)。

#### 例 1 {#evt-ii-s2-n1-exa-1 .statement tag=07B5}

$E$ のすべての線形アフィン多様体 (特に空の集合) は凸です。

#### 例 2 {#evt-ii-s2-n1-exa-2 .statement tag=07B6}

$\mathbf{R}$ の空でない凸集合は区間 (GT、IV, § 2.4、提案 1) だけです。

#### 例 3 {#evt-ii-s2-n1-exa-3 .statement tag=07B7}

Let $E$ be a vector space and $\|x\|$ a norm on $E$; the unit ball $B$, formed by the points $x$

$\|x\| \leq 1$ は関係 $\|x\| \leq 1, \|y\| \leq 1$ から凸であるため、$0 \leq \lambda \leq 1$ は次のようになります。
$$
\|\lambda x + (1 - \lambda) y\| \leq \lambda \|x\| + (1 - \lambda) \|y\| \leq \lambda + (1 - \lambda) = 1 .
$$

#### 注意 {#evt-ii-s2-n1-rem-1 .statement tag=07B8}

— $A$ をベクトル空間 $E$ の凸部分集合とします。任意のスカラー $\alpha > 0$ と $\beta > 0$ に対して、$\alpha A + \beta A = (\alpha + \beta) A$ が得られます。他の語では、任意の $x \in A, y \in A$ に対して、$(\alpha + \beta) z = \alpha x + \beta y$ となるような $z \in A$ が存在します。実際、この関係は $z = \frac{\alpha}{\alpha + \beta} x + \frac{\beta}{\alpha + \beta} y$ と書くことができ、def を使用すると $\frac{\alpha}{\alpha + \beta} > 0, \frac{\beta}{\alpha + \beta} > 0$ と $\frac{\alpha}{\alpha + \beta} + \frac{\beta}{\alpha + \beta} = 1$ が続き、そこから主張が続きます。 1.

#### 命題 1 {#evt-ii-s2-prop-1 .statement tag=07B9}

*Let $(x_i)$ be a family of 点 of a convex 部分集合 $A$;正の質量 $\lambda_i$ (添字、cf. A、II, § 9.3 の有限多数を除く $\sum_i \lambda_i = 1$ と $\lambda_i = 0$) 属するから $A$ を使用して形成された $x_i$ の各重心 $\sum_i \lambda_i x_i$。*

Clearly we need only consider the case when 添字 are $1, 2, ..., p$ and $\lambda_i > 0$ for each $i$; $p = 1$ の場合、命題は自明です。 $p$の帰納法までに結果を証明します。 $\mu = \sum_{i=1}^{p-1} \lambda_i > 0$ と $y = \sum_{i=1}^{p-1} \frac{\lambda_i}{\mu} x_i$ を入れます。 帰納法の仮定は $y \in A$ を意味します。 Now as $\lambda_p = 1 - \mu$ and $\sum_{i=1}^p \lambda_i x_i = \mu y + (1 - \mu) x_p$, its follows from def. 1 $\sum_{i=1}^p \lambda_i x_i$ 属するから $A$ まで。

#### 命題 2 {#evt-ii-s2-prop-2 .statement tag=07BA}

*Let $E$ and $F$ be two affine 空間 and $f$ be an affine 線形写像 of $E$ in $F$; then 像 of a convex 部分集合 of $E$ under $f$, and 逆像 of a convex 部分集合 of $F$ under $f$ are both convex.*

終端点 $x, y$ を持つ閉セグメントの $f$ の下にある像は、終端点 $f(x), f(y)$ を持つ閉セグメントなので、最初の主張です。 We deduce that 逆像 of a closed segment of $F$ under $f$ 含む each closed segment whose end 点属する to it;プロップの 2 番目の主張。 2が続きます。

In particular 像 of a convex 集合 under ホモテティー or a translation is a convex 集合.

#### 命題 3 {#evt-ii-s2-prop-3 .statement tag=07BB}

*アフィン空間 $E$ では、$H$ を関係 $g(x) = 0$ によって定義される超平面とします。ここで、$g$ は $E$ 上の非定数アフィン写像です。 Then the half-spaces defined by 関係 $g(x) \geq 0, g(x) \leq 0, g(x) > 0, g(x) < 0$ are convex.*

For these are 逆像 under $g$ of 区間 of $\mathbf{R}$ and thus are convex.

記法の小道具付き。 3 アフィン空間の部分集合 $M$ の点は、 $g(x) \geq 0, g(x) \leq 0$ で定義される半角スペースの 1 つに $M$ が含まれる場合、 超平面 $H$ の *同じ側* (それぞれ *厳密に同じ側*) にあります。 (それぞれ $g(x) > 0$ または $g(x) < 0$)。

#### 命題 4 {#evt-ii-s2-prop-4 .statement tag=07BC}

* $A$ の点、アフィン空間 $E$ の凸部分集合は、$A$ が $H$ を満たさない場合に限り、超平面 $H$ と厳密に同じ側にあります。*

明らかに条件が必要です。逆に、それが満たされると仮定し、$g(x) = 0$ を H を定義する方程式とします ($g$ は $\mathbf{R}$ における E のアフィン線形写像です)。 集合 $g(A)$は$\mathbf{R}$に凸なので、区間、$0 \notin g(A)$になります。したがって、$g(x)$ はすべての $x \in A$ に対して固定符号です。

### 2. 凸集合の共通部分。凸の積集合

#### 命題 5 {#evt-ii-s2-prop-5 .statement tag=07BD}

— *共通部分の凸ファミリーの *共通部分アフィン空間* の凸部分集合 E *は凸*です。

命題は def の直後に続きます。 II、p. 7 の 1。

#### 命題 6 {#evt-ii-s2-prop-6 .statement tag=07BE}

— *$(E_i)_{i \in I}$ *をベクトル空間の族とし、それぞれ* $i \in I$ について、*$A_i$ *$E_i$ の空でない部分集合とします。 *その後、集合* $A = \prod_{i \in I} A_i$ *は$E = \prod_{i \in I} E_i$に凸です、*すべて* $i \in I$、*集合* $A_i$ *は$E_i$に凸です*。

実際、それぞれの射影 $\mathrm{pr}_i$ は線形写像であり、$A_i = \mathrm{pr}_i A$ と $A = \bigcap_{i \in I} \mathrm{pr}_i^{-1}(A_i)$ があります。 命題は小道具から続きます。上記の2と5。

#### 系 {#evt-ii-s2-n2-cor-1 .statement tag=07BF}

— *空間* $\mathbf{R}^n$ *すべての平行面* (GT、VI, § 1.3) * は凸の部分集合* です。

なぜなら、それは直方体のアフィン線形写像の下にある像であり、この最後の部分は支柱によって凸になっているからです。 6.

#### 命題 7 {#evt-ii-s2-prop-7 .statement tag=07BG}

— *A *と* B *を 2 つの凸部分集合 of ベクトル空間* E とします。 *任意の実数* $\alpha, \beta$ *集合* $\alpha A + \beta B$ *(集合 of 点 of 形* $\alpha x + \beta y$, *どこに* $x$ *A、*、および*で変化します $y$ *B*で) は凸*です。

For $\alpha A + \beta B$ is the image of the convex subset $A \times B$ of $E \times E$ under the linear mapping $(x, y) \mapsto \alpha x + \beta y$ of $E \times E$ in $E$.

### 3. 集合の凸エンベロープ

#### 定義 2 {#evt-ii-s2-def-2 .statement tag=07BH}

— *アフィン空間* E の部分集合* A * が与えられると、*すべての凸集合含む* A の共通部分を呼びます、* A の凸包絡線、*つまり* (II, p. 9, 提案 5) *それは最小の凸集合含む* A.

#### 命題 8 {#evt-ii-s2-prop-8 .statement tag=07BI}

— *任意の家族* $(A_i)_{i \in I}$ *アフィン空間* E の凸部分集合の、* $\bigcup_{i \in I} A_i$ の凸包絡線は、*正確に線形結合* $\sum_{i \in I} \lambda_i x_i$ の集合、*ここで* $x_i \in A_i, \lambda_i \geq 0$ *すべての* $i \in I$ ($\lambda_i = 0$ *有限多数の添字* を除く) *および* $\sum_{i \in I} \lambda_i = 1$。

これら線形結合のうち集合を C で表すと、明らかに C はすべての凸集合に含まれており、含むはすべての $A_i$ (II、p. 8、提案 1) です。一方、$i$ごとに$A_i \subset C$。まだ証明されていないことは、C が凸であるということだけです。 $x = \sum \lambda_i x_i$、$y = \sum \mu_i y_i$をCの2つの点、$\alpha$を数とし、$0 < \alpha < 1$となるように、i∈Iごとにγ_i = αλ_i + (1 - α) μ_iを書き、Jを次のようにします。 γ_i ≠ 0 である I の添字の集合 (有限)。 αx + (1 - α)y = ∑_{i∈J} γ_i z_i と書くことができます。

$$ z_i = \gamma_i^{-1}(\alpha\lambda_i x_i + (1 - \alpha) \mu_i y_i) $$

すべての i ∈ J に対して属するを A_i に変換します。しかし、$\sum_{i\in J} \gamma_i = \alpha \sum_{i\in I} \lambda_i + (1 - \alpha) \sum_{i\in I} \mu_i = 1$、そして私たちは$ax + (1 - \alpha) y \in C$であることがわかります。 命題が証明されました。

#### 系 1 {#evt-ii-s2-prop-8-cor-1 .statement tag=07BJ}

*E の部分集合 A の凸包絡線は、線形結合 $\sum_i \lambda_i x_i$ の集合と同一です。ここで、$(x_i)$ は、A の点、数 $\lambda_i > 0, \text{ for all } i$ および $\sum_i \lambda_i = 1$ の任意の有限族です。*

凸型集合 A によって生成されるアフィン線形多様体 (A, II, § 9.3) の次元は、A の *次元* と呼ばれます。

E をベクトル空間とします。 E の集合 A の平衡包絡線の凸包絡線 C は、A の *平衡凸包絡線* (または *対称凸包絡線*) と呼ばれます。明らかに、含む A は最小の対称凸集合です。 属するの平衡包絡線のすべての点が、$a \in A$ の端 a と −a を持つセグメントになるため、これは $A \cup (-A)$ の凸包絡線でもあります。 集合 C 一致する線形結合 $\sum_i \lambda_i x_i$ の集合で、$x_i \in A$ と $\sum_i |\lambda_i| \leq 1$;なぜなら、この点の集合が凸であり、 含む A と −A であることは明らかだからです。それが C に含まれていることを証明できれば十分であり、そのためには $\mu = \sum_i |\lambda_i| > 0$ である線形結合のみを考慮する必要があります。 $\lambda_i \geq 0$ の場合、$\sum_i \lambda_i x_i = \mu \cdot \sum_i \alpha_i y_i$ を $\alpha_i = \lambda_i/\mu$ と $y_i = x_i$ で書くことができます。そして$\alpha_i = -\lambda_i/\mu$; $\lambda_i < 0$なら$y_i = -x_i$;明らかに$\sum_i \alpha_i = 1$、そして私たちの主張が証明されました。

#### 系 2 {#evt-ii-s2-prop-8-cor-2 .statement tag=07BK}

* f をアフィン空間 F 内のアフィン空間 E のアフィン線形写像とします。 E の各部分集合 A について、f(A) の凸包絡線は、A の凸包絡線 f の下の像になります。

線形写像とバランスの取れた凸エンベロープにも同様の主張があります。

### 4. 凸円錐

#### 定義 3 {#evt-ii-s2-def-3 .statement tag=07BL}

* アフィン空間 E の部分集合 C は、C が中心 x_0 のすべての相似性に対して不変で、比率 > 0 の場合、頂点 x_0 を持つ円錐です。*

この番号と次の番号では、考慮されている円錐の頂点を E の原点として選択したと仮定します。 *つまり* E がベクトル空間であると仮定し、円錐について話すとき、この円錐には頂点 0 があることを理解してください。 $\lambda > 0$ (それぞれ $\lambda \geq 0$) に対して、集合 of 点 of 形 $\lambda a$、ここで $a$ は非 null ベクトルは、0 から始まる *開いたハーフライン* (それぞれ *閉じたハーフライン*) と呼ばれます。

頂点 0 の円錐 C は、$0 \in C$ の場合は *尖っている*、それ以外の場合は *尖っていない*と言われます。尖った円錐は、単一の点 $\{0\}$ か、0 から始まる閉じた半線の集合の和集合です。非尖った円錐は、0 から始まる開いた半線の和集合 (おそらく空) です。 C が非尖った円錐の場合、$C \cup \{0\}$ は次のようになります。尖った円錐形。 C が尖った円錐である場合、$C - \{0\}$ は尖っていない円錐です。

C が尖っていない *凸* 円錐である場合、$C \cup \{0\}$ は尖った凸円錐です。ただし、C が尖った凸円錐である場合、$C - \{0\}$ は必ずしも凸であるとは限りません。 0 を通る含むどの線移行にも該当しない場合、尖った凸円錐は *適切* であると言います。

#### 命題 9 {#evt-ii-s2-prop-9 .statement tag=07BM}

*尖った凸円錐 C は、C の 0 の補数である非尖円錐 $C'$ が凸である場合にのみ適切です。*

C 含むが 0 を通る線であれば、明らかに $C'$ は凸ではありません。ここで、C が適切であると仮定し、x、y を $C'$ の 2 つの点とします。終端点 x, y を持つ閉じたセグメントは C に含まれます。 含む 0 の場合、$0 < \lambda < 1$ を持つ$\lambda$ に対しては $\lambda x + (1 - \lambda) y = 0$、したがって $\mu < 0$ を持つ$x = \mu y$ になります。したがって、C 含むは、仮定とは反対に、0 と x を通る線です。

#### 命題 10 {#evt-ii-s2-prop-10 .statement tag=07BN}

* E の部分集合 C は、すべての $\lambda > 0$ に対して $C + C \subset C$ と $\lambda C \subset C$ である場合に限り、凸円錐になります。*

条件 $\lambda C \subset C$ のすべての $\lambda > 0$ がコーンを特徴づけます。 C が凸の場合、$C + C = \frac{1}{2}C + \frac{1}{2}C = C$ (II、p. 8、*注意*) になります。逆に、円錐 C が $C + C \subset C$ である場合、$0 < \lambda < 1$ には $\lambda C + (1 - \lambda) C = C + C \subset C$ があり、C が凸であることがわかります。

#### 系 1 {#evt-ii-s2-prop-10-cor-1 .statement tag=07BO}

*If C is a non-empty convex cone, the vector space generated by C is the set $C - C$ (the set of points $x - y$ where x, y vary in C).*

なぜなら、$V = C - C$ の場合、V は空ではなく、すべての $\lambda \neq 0$ と $V + V = C + C - (C + C) \subset C - C = V$ に対して $\lambda V = V$ があり、V がベクトル部分空間であることがわかります。最後に、ベクトル部分空間と含む C も含む V になります。

#### 系 2 {#evt-ii-s2-prop-10-cor-2 .statement tag=07BP}

*Cが尖った凸円錐の場合、Cに含まれる最大のベクトル部分空間は集合$C \cap (-C)$となります。

なぜなら、$W = C \cap (-C)$ の場合、W は空ではなく、すべての $\lambda \neq 0$ に対して $\lambda W = W$ も同様です。
$$
W + W \subset (C + C) \cap (-(C + C)) \subset C \cap (-C) = W,
$$
これは、W がベクトル部分空間であることを示しています。明らかに、C に含まれるすべてのベクトル部分空間は W にも含まれます。

明らかに、$f$ がベクトル空間 F の E の線形写像である場合、E の凸円錐 C の $f(C)$、像は F の凸円錐です。E の凸円錐 (頂点 0 を持つ) のすべての共通部分は凸円錐です。凸円錐含む A の E 共通部分のすべての部分集合 A (これらは存在し、E 自体もそのような円錐の 1 つです) は、含む A である最小の凸円錐です。それは A によって *生成された* 凸円錐と呼ばれます。

#### 命題 11 {#evt-ii-s2-prop-11 .statement tag=07BQ}

*$(C_i)_{i \in I}$ を E の凸円錐のファミリーとします。 $C_i$ の和集合によって生成される凸円錐は、点 $\sum_{i \in J} x_i$ の集合と同一です。ここで、J は、すべての $i \in J$ の I および $x_i \in C_i$ のいずれかの有限部分集合です。

実際、そのような点のC、集合は、$C_i$の凸円錐含む和集合であり、含むこの和集合のいずれかの凸円錐に含まれることは明らかです。

#### 系 {#evt-ii-s2-n4-cor-1 .statement tag=07BR}

— *E の任意の部分集合 A について、A によって生成された凸円錐は、線形結合* $\sum_{i \in J} \lambda_i x_i$ の集合と同一です。*ここで* $(x_i)_{i \in J}$ *は A の点の任意の有限の空でない族であり、ここで* $\lambda_i > 0$ *すべて* $i \in J$ です。

A の凸円錐含む点 $x \neq 0$ の場合、点 $\lambda x$ の半線 $C_x$ も含むここで、$\lambda$ は正の数の集合で変化し、 $C_x$ は凸円錐です。

#### 命題 12 {#evt-ii-s2-prop-12 .statement tag=07BS}

— *A が E の凸集合である場合、A によって生成される凸円錐は * $C = \bigcup_{\lambda > 0} \lambda A$ と同一です。

集合 C は明らかに円錐です。 C が凸であることを示すだけで十分です。 $\lambda x, \mu y$ を C ($\lambda > 0, \mu > 0, x \in A, y \in A$) の 2 つの点とします。 $\alpha, \beta$ を 2 数 $> 0$ として、$\alpha + \beta = 1$ とします。次に、$\alpha \lambda x + \beta \mu y = (\alpha \lambda + \beta \mu) z$、$z \in A$、および$\alpha \lambda + \beta \mu > 0$。したがって$\alpha \lambda x + \beta \mu y \in C$です。

#### 注意 {#evt-ii-s2-n4-rem-1 .statement tag=07BT}

— 1) prop の仮説を使用します。 12 の場合、$0 \notin A$ の場合、円錐 C は尖っていないため、$C \cup \{0\}$ は *適切* です。

2) A を E の任意の凸集合とします。 空間 $F = E \times \mathbf{R}$ の凸集合 $A_1 = A \times \{1\}$ と、$A_1$ によって生成される頂点 0 の凸円錐 C を考えてみましょう。提案 12 は、$A_1$ が F の C および超平面 $E \times \{1\}$ の共通部分であることを示しています。したがって、E のすべての凸集合は、F の頂点 0 を持つ凸円錐の共通部分の E 上の射影と見なすことができ、 超平面 $E \times \{1\}$。

### 5. 注文しましたベクトル空間

$x \leqslant y$ または $y \geqslant x$ で示される、ベクトル空間 E 上の *事前順序* 構造は、次の 2 つの公理を満たす場合、E のベクトル空間構造と *互換性* があります。

*(EO$_I$)* *もし* $x \leqslant y$ *その後* $x + z \leqslant y + z$ *すべて* $z \in E$。

*(EO$_II$)* *If* $x \geqslant 0$ *then* $\lambda x \geqslant 0$ *すべてのスカラー* $\lambda \geqslant 0$。

これら 2 つの構造を運ぶベクトル空間 E は、*予約済みベクトル空間* と呼ばれます (それぞれ、E の予約注文の関係が位数の場合に *注文済みベクトル空間*) と呼ばれます。

公理 (EO$_I$) は、E の事前順序構造と加法群構造が互換性がある、つまり、これら 2 つの構造を運ぶ E は *事前順序付けされた群* (A、VI、p. 3) であることを意味することに注意してください。

#### 例 {#evt-ii-s2-n5-exa-1 .statement tag=07BU}

— A 上で定義されたすべての有限実数値写像の空間 $E = \mathbf{R}^A$ において、« for all $t \in A$, $x(t) \leqslant y(t)$ » によって与えられる位数の関係は、E のベクトル空間構造と互換性があります。

#### 命題 13 {#evt-ii-s2-prop-13 .statement tag=07BV}

— (i) *事前注文されたベクトル空間 E の元* $\geqslant 0$ の *集合 P は、尖った凸円錐* です。

(ii) *逆に、P が E の尖った凸円錐である場合、関係* $y - x \in P$ * は E の事前注文関係であり、E のベクトル空間構造と* 互換性があり、P が集合である事前注文構造は、定義するだけです。 元 $\geqslant 0$ の。

(iii) 関係 $y - x \in P$ は、P が尖った凸円錐である場合、P が適切な円錐である場合に限り、E 上で位数関係になります。

(i) 公理 (EO_I) と (EO_{II}) は、すべての $\lambda > 0$ に対して $P + P \subset P$ と $\lambda P \subset P$ を意味します。 $0 \in P$ より、P は尖った凸円錐であることがわかります (II、p. 11、提案 10)。

(ii) 逆に、P が尖った凸円錐の場合、関係 $P + P \subset P$ は、関係 $y - x \in P$ が E の加法群構造と互換性のある事前注文であることを意味します (A、VI、p. 3、提案 3)。明確に書くと、$x \leqslant y$、集合 P は $x \geqslant 0$ の集合と同じです。さらに、すべての $\lambda \geqslant 0$ に対して関係 $\lambda P \subset P$ は、公理 (EO_{II}) が満たされていることを示します。

(iii) P が適切であるということは、$P \cap (-P) = \{0\}$ (II, p. 11, cor. 2) であることを意味し、したがって $y - x \in P$ は位数関係である。

#### 例 {#evt-ii-s2-n5-exa-2 .statement tag=07BW}

\* H を実際のヒルベルト空間とします。 H の連続自己準同型のベクトル空間 $\mathscr{L}(H)$ では、正のエルミート自己準同型形は適切な尖った凸円錐です。したがって、この円錐定義する位数構造は、$\mathscr{L}(H)$ のベクトル空間構造と互換性があり、関係 $A \leqslant B$ は、$B - A$ が正のエルミート自己準同型であることを意味します。 \*

ベクトル空間 E の任意の尖った凸円錐 P について、集合 $P \cap (-P)$ は E のベクトル部分空間、H (II、p. 11、cor. 2) です。 $E/H$ の P の標準像 $P'$ は凸円錐で、E の $P'$ の逆像は P です。 したがって、$P' \cap (-P') = \{0\}$、および $E/H$ の $P'$ 定義する位数構造は、 ベクトル空間構造と互換性があります。

予約注文されたベクトル空間の線型形式 $f$ は、E の $x \geqslant 0$ が $f(x) \geqslant 0$ を意味する場合、E は正であると言われます。あるいは、E の元 $\geqslant 0$ の凸円錐 P が、$f(x) \geqslant 0$ となる$x$ の半分の空間に含まれる場合。明らかに、E に対する双対 $E^*$ では、正の線型形式の集合は尖った凸円錐です。

### 6. トポロジカルな凸円錐ベクトル空間

#### 命題 14 {#evt-ii-s2-prop-14 .statement tag=07BX}

トポロジー ベクトル空間 E では、凸集合 (それぞれ凸円錐) の閉包は凸集合 (それぞれ同じ頂点を持つ凸円錐) です。

なぜなら、A を凸集合とします。 写像 $(x, y) \mapsto \lambda x + (1 - \lambda) y$ ($0 < \lambda < 1$) は、A の $E \times E$ と写像 $A \times A$ で連続します。したがって (GT, I, § 2.1, th. 1) $\overline{A}$ では写像 $\overline{A} \times \overline{A}$ となり、$\overline{A}$ が凸であることがわかります。同様に、C が頂点 0 の凸円錐の場合、すべての $\lambda > 0$ に対して $\overline{C} + \overline{C} \subset \overline{C}$ と $\lambda \overline{C} \subset \overline{C}$ が適用されます。

#### 定義 4 {#evt-ii-s2-def-4 .statement tag=07BY}

トポロジカルベクトル空間 E の任意の集合 A について、すべての閉じた凸型集合含む A の共通部分は、A の凸型閉じ包絡線と呼ばれます。 最小の凸閉集合含むAです。

プロップから。図１４において、Ａの凸状閉包絡線は、Ａの凸状包絡線の閉包である。それは明らかに、$\overline{A}$ の凸状の閉じた包絡線と同じです。

同様に、最小の対称凸閉包絡線集合を含む A、A の対称凸閉包絡線 (または平衡凸閉閉包絡線) と呼びます。それは A の対称凸包絡線の閉包です (II, p. 10)。これは、$\overline{A}$ の対称凸型閉包絡線でもあります。

#### 命題 15 {#evt-ii-s2-prop-15 .statement tag=07BZ}

— $A_i$ ($1 \leq i \leq n$) を、ハウスドルフ位相ベクトル空間 E のコンパクト凸集合の有限数とします。その場合、$A_i$ の凸包絡線和集合はコンパクトです (したがって、凸閉包絡線と同じです)これ和集合)。

B を、点 $(\lambda_1, \lambda_2, ..., \lambda_n)$ ($\lambda_i \geq 0$ ($1 \leq i \leq n$) および $\sum_{i=1}^n \lambda_i = 1$) によって定義される $\mathbf{R}^n$ のコンパクト集合とします。 定義する公式 $(\lambda_1, \lambda_2, ..., \lambda_n, x_1, x_2, ..., x_n) \mapsto \sum_{i=1}^n \lambda_i x_i$ による E の $B \times \prod_{i=1}^n A_i \subset \mathbf{R}^n \times E^n$ の連続写像。 $\bigcup_{i=1}^n A_i$ の凸包絡線 C は、この写像の下では $B \times \prod_{i=1}^n A_i$ の像です。 $B \times \prod_{i=1}^n A_i$ はコンパクト、E はハウスドルフであるため、C はコンパクトということになります。

#### 系 1 {#evt-ii-s2-prop-15-cor-1 .statement tag=07C0}

— ハウスドルフ位相幾何学ベクトル空間では、有限集合の凸包絡線はコンパクトです。

#### 系 2 {#evt-ii-s2-prop-15-cor-2 .statement tag=07C1}

— トポロジー ベクトル空間 E では、有限集合の凸包絡線はプレコンパクトです。

実際、j をハウスドルフ完成 $\hat{E}$ における E の標準写像とします。 C が A の凸包絡線である場合、$j(C)$ は $\hat{E}$ の有限集合 $j(A)$ の凸包絡線であるため、$j(C)$ はコンパクト (cor. 1)、したがって C はプレコンパクト (GT、 II, § 4.2）。

#### 命題 16 {#evt-ii-s2-prop-16 .statement tag=07C2}

— A を、トポロジカルベクトル空間 E の少なくとも 1 つの内部点 $x_0$ を持つ凸部分集合とします。任意の点 $x \in \overline{A}$ について、終点点を持つ開いたセグメントのすべての点 $x_0, x$はAの内部にあります。

このセグメントの任意の点 y について、f を中心 y のホモテティー とし、x に対する変換 $x_0$ の比率 $\lambda < 0$ とします。 V が A に含まれる $x_0$ の開近傍である場合、$f(V)$ は x の近傍であるため、含む点 $f(z) \in A$ となります。今

$$
f(z) - y = \lambda (z - y) = \lambda (z - f(z)) + \lambda (f(z) - y),
$$

したがって $y - f(z) = \frac{\lambda}{\lambda - 1} (z - f(z))$ なので、y は中心 $f(z)$ と比 $\mu = \lambda / (\lambda - 1)$ のホモテティー g によって z に変換されます。 $0 < \mu < 1$ より、A に含まれる 0 の近傍に g 変換 V が代入されます。命題が証明されます。

#### 系 1 {#evt-ii-s2-prop-16-cor-1 .statement tag=07C3}

— The interior $\overset{\circ}{A}$ of a convex set $\overline{A}$, is itself a convex set; if $\overset{\circ}{A}$ is not empty, then it coincides with the interior of $\overline{A}$, and $\overline{A}$ is a convex set that coincides with the closure of $\overset{\circ}{A}$.

プロップから続きます。 16、$\overset{\circ}{A}$ が空でない場合、それは凸集合であり、$\overline{A}$ のすべての点は $\overset{\circ}{A}$ のクラスター 点です。次に、$\overline{A}$ 属するから $\overset{\circ}{A}$ のすべての内部点を示します。 x を $\overline{A}$ の内部点とし、明確にするために $x = 0$ と仮定します。 V を、$\overline{A}$ に含まれる 0 の対称近傍とし、$y \in \overset{\circ}{A} \cap V$ とします。現在$-y \in \overline{A}$なので、プロップにより。 16、$y \neq 0$ の場合、$0 \in \overset{\circ}{A}$ であることがわかります。 $y = 0$ の場合、これは明らかに真です。

#### 系 2 {#evt-ii-s2-prop-16-cor-2 .statement tag=07C4}

— *内部* $\dot{C}$ *凸円錐* C、*それ自体が凸円錐です。 * $\dot{C}$ *が空でない場合、それは* $\overline{C}$の内部を持つ一致する、*および* $\overline{C}$ *は* $\dot{C}$の閉包を持つ一致するの尖った凸円錐です。

比 $> 0$ と中心 0 変換 C の相似関係は、$\dot{C}$ に対しても同じなので、$\dot{C}$ は円錐になります。 系の残りは cor から続きます。 1 そして、C が空でない場合、$\overline{C}$ 含むが C の頂点であるという明白な指摘。

H を $\mathbf{R}$ 上のトポロジカルベクトル空間 E の閉じた超平面とします。方程式は形 $f(x) = \alpha$ で、ここで $f$ は E (I, p. 13, th. 1) の零と同一ではない連続線型形式です。したがって、$f(x) \leqslant \alpha$ と $f(x) \geqslant \alpha$ によってそれぞれ定義される閉じた半分空間は *閉じた* 凸型集合です。それぞれ $f(x) > \alpha$ と $f(x) < \alpha$ で定義されるそれらの補数は *開*凸集合です。これらのハーフスペースは、H によって *決定された * 閉じた (または開いた) ハーフ空間であると言います。

#### 命題 17 {#evt-ii-s2-prop-17 .statement tag=07C5}

— *トポロジー ベクトル空間* E では、* A を少なくとも 1 つの内部点を持つ集合とし、そのすべての点が超平面* H の同じ側にあるようにします。 *その後* H * が閉じられ、* A の内部点は * H の同じ側に * 厳密に位置し、 * そしてクラスターになります* A の点は * H の同じ側にあります。 *特に開いた (それぞれ閉じた) 半分空間は、閉じた超平面* によって決定されます。

実際、H 含むが原点であり、$f(x) = 0$ が H の方程式であると仮定します。明確にするために、すべての $x \in A$ に対して $f(x) \geqslant 0$ であると仮定します。 $f(y) > -1$ 含むの少なくとも 1 つの内部点となるように、点 y によって形成される半分の空間、そして翻訳により、$f(y) > 0$ となる点 y の半分の空間にも同じことが当てはまります。これは、H が閉じていることを示します (I、p. 11、系)。次に、$f$ は $\mathbf{R}$ (I、p. 13、系) 上の E の厳密な射であることがわかります。したがって、$f(\dot{A})$ は $\mathbf{R}$ のオープン集合です。これ集合できない含む 0 または、仮定とは逆に含む数 $< 0$ になります。したがって、それは開いた区間 $]0, +\infty[$ に含まれています。一方、$f(y) \geqslant 0$ が閉じている y の半分の空間と含む A なので、含む $\overline{A}$ となります。

#### 系 {#evt-ii-s2-n6-cor-1 .statement tag=07C6}

— *P を、トポロジカルベクトル空間* E の少なくとも 1 つの内部点を持つ尖った凸円錐とします。 *すると、各線型形式* f *E 上で同一ではなく、* E 上で * 零が正であり、* P (II, p. 13) によって定義される事前順序構造に対して正です。必ず連続*。 *さらに、x * が * P の内部にある場合 * $f(x) > 0$ *、そして * x * が* P のクラスター 点 *である場合* $f(x) \geqslant 0$。

プロップを適用します。 17 を、方程式 $f(x) = 0$ で H が超平面である場合 $A = P$ に当てはめます。

#### 注意 {#evt-ii-s2-n6-rem-1 .statement tag=07C7}

トポロジカルベクトル空間 E では、すべての凸集合 C が接続されます。実際、$a \in C$ の場合、C は、終わりが点 a で a で閉じているセグメントの和集合です。これらは接続されており、結果は GT、I, § 11.1、prop から得られます。 2.

### 7. 注文したトポロジベクトル空間

E を順序付きベクトル空間とします。 E の位相は、E のベクトル空間構造と互換性があり、次の公理に従う場合、E の順序付けられたベクトル空間構造と *互換性* があります。

(TO) * x の * 凸円錐 * $x \geqslant 0$ は * E で閉じられています。

互換性のある位相を持つ順序付けされたベクトル空間 E は、順序付けされたトポロジカルベクトル空間と呼ばれます。

#### 例 {#evt-ii-s2-n7-exa-1 .statement tag=07C8}

空間 $\mathbf{R}^n$ と通常の位相および位数構造、つまり位数の積因子の構造は、順序トポロジー ベクトル空間です。一方、$n \geq 2$ では、$\mathbf{R}^n$ が辞書編集上の位数 (S, III, § 2.6) を保持する場合、通常の位相は、$\mathbf{R}^n$ の順序付けられたベクトル空間構造と互換性がありません。

A を集合とします。 A で定義された実数値有界写像のベクトル空間 $\mathscr{B}(A ; \mathbf{R})$、位相はノルム $\|x\| = \sup_{t \in A} |x(t)|$ および位数構造によって定義され、積位数構造 $\mathbf{R}^A$ は、順序トポロジカルベクトル空間です。

順序トポロジー ベクトル空間 E では、元 $x \leq 0$ の集合が閉じています。翻訳は同型であるため、すべての $a \in E$、元 $x \geq a$ (それぞれ $x \leq a$) の集合が閉じていると推測します。 $\{0\}$ は集合 $x \geq 0$ と $x \leq 0$ の共通部分であるため、$\{0\}$ が閉じており、E がハウスドルフであることがわかります。

#### 命題 18 {#evt-ii-s2-prop-18 .statement tag=07C9}

順序トポロジー ベクトル空間 E では、H を関係 $\leq$ によって指示された集合とします。 H の切断フィルターの E に極限がある場合、この極限は H の上界です。

というのは、$b = \lim_{x \in H} x$ としましょう。 $x \in H$ のすべての $y \in H$、集合について、$x \geq y$ は H の切断フィルターの集合であるため、 b はこの集合のクラスター 点です。しかし、集合 $x \geq y$ が E で閉じているので、$b \geq y$ があり、したがって b は H の上界になります。一方、a が H の上界である場合、H は閉じた集合 $x \leq a$ に含まれます。 b は H のクラスター 点であるため、$b \leq a$ があり、証明が完成します (II, p. 72、演習 42)。

### 8. 凸写像

#### 定義 5 {#evt-ii-s2-def-5 .statement tag=07CA}

X をアフィン空間 E の凸部分集合とします。 X 上で定義された実数値有限写像は、X の任意の 2 つの異なる点 x、y および任意の場合、凸 (厳密に凸) になります。 実数 $\lambda, 0 < \lambda < 1$、次のとおりです。

(1)
$$
f(\lambda x + (1 - \lambda) y) \leq \lambda f(x) + (1 - \lambda) f(y)
$$
(それぞれ

(2)
$$
f(\lambda x + (1 - \lambda) y) < \lambda f(x) + (1 - \lambda) f(y)).
$$

$E = \mathbf{R}$のとき、凸写像のこの定義は、FVRのI、p. 32と同じです。さらに、すべてのアフィン線 $D \subset E$ について、f から $X \cap D$ までの制限が $X \cap D$ で凸（または厳密に凸）である場合に限り、f は X で凸（厳密に凸）です。

#### 例 {#evt-ii-s2-n8-exa-1 .statement tag=07CB}

f が E 上のアフィン線形写像である場合、f と $f^2$ は E 上で凸の写像です。これは f にとって明らかです。
$$
f(\lambda x + (1 - \lambda) y) = \lambda f(x) + (1 - \lambda) f(y);
$$
一方、$\alpha = f(x), \beta = f(y)$ の場合は、
$$
\lambda \alpha^2 + (1 - \lambda) \beta^2 - (\lambda \alpha + (1 - \lambda) \beta)^2 = \lambda(1 - \lambda) (\alpha - \beta)^2 \geq 0
$$

$0 < \lambda < 1$の場合。さらに、$f^2$ からアフィン線 $D \subset E$ への制限は、$f|D$ が定数でない場合、*厳密に凸です*。

$X$ 上で定義された実数値写像 $f$ は、 — $f$ が凸型 (つまり厳密に凸型) の場合、*凹型* (つまり *厳密に凹型*) になります。つまり、$X$ の 2 つの異なる点 $x, y$ と、$0 < \lambda < 1$ となるすべての数 $\lambda$ について、

$$
f(\lambda x + (1 - \lambda) y) \geqslant \lambda f(x) + (1 - \lambda) f(y)
$$

(それぞれ

$$
f(\lambda x + (1 - \lambda) y) > \lambda f(x) + (1 - \lambda) f(y)).
$$

$\mathbf{R}$ の $X$ の写像は、凸と凹の両方であれば *アフィン* です (*cf.* II、p. 78、演習 11)。

#### 命題 19 {#evt-ii-s2-prop-19 .statement tag=07CC}

*$X$ をアフィン空間 $E$ の凸集合とします。そして、$f$ を $X$ に対して定義された実数値写像とします。 Denote the set of points $(x, a) \in E \times \mathbf{R}$ for which $x \in X$ and $f(x) \leqslant a$ (resp. $x \in X$ and $f(x) < a$) by $F$ (resp. $F'$). したがって、次の条件は同等です*:

a) *写像 $f$ は凸*です。
b) アフィン空間 $E \times \mathbf{R}$ の *集合 $F$ は凸です*。
c) アフィン空間 $E \times \mathbf{R}$ の *集合 $F'$ は凸です*。

$a) \Rightarrow c)$ であることを示します。 $(x, a)$と$(y, b)$を$F'$と$0 < \lambda < 1$の2つの点とすると、$f(x) < a,\ f(y) < b$、$f$が凸の場合

$$
f(\lambda x + (1 - \lambda) y) \leqslant \lambda f(x) + (1 - \lambda) f(y) < \lambda a + (1 - \lambda) b
$$

これは、$E \times \mathbf{R}$ 属するから $F'$ の点 $\lambda(x, a) + (1 - \lambda)(y, b)$ を示しています。したがって、$F'$ は凸です。

次に、$c) \Rightarrow b)$ を示します。 $(x, a), (y, b)$ が 2$F$ の 2 つの点である場合、すべての $\varepsilon > 0$、$(x, a + \varepsilon)$、$(y, b + \varepsilon)$ 属するから$F'$ まで、$0 < \lambda < 1$ の場合、同じことが$(\lambda x + (1 - \lambda) y, \lambda a + (1 - \lambda) b + \varepsilon)$ にも当てはまります。 $F$ の定義により、これは $(\lambda x + (1 - \lambda) y, \lambda a + (1 - \lambda) b)$ 属するから $F$ を意味します。

最後に $b) \Rightarrow a)$、(上記の記法を使用)、$(\lambda x + (1 - \lambda) y, \lambda a + (1 - \lambda) b)$ 属するから $F$ の場合、

$$
f(\lambda x + (1 - \lambda) y) \leqslant \lambda a + (1 - \lambda) b
$$

$a \geqslant f(x)$ と $b \geqslant f(y)$ が提供されます。したがって、(1) が続き、$f$ は凸になります。

#### 系 {#evt-ii-s2-n8-cor-1 .statement tag=07CD}

*$f$ が $X$ で凸である場合、$x \in X$ のすべての $\alpha \in \mathbf{R}$、集合について、$f(x) \leqslant \alpha$ (それぞれ $f(x) < \alpha$) が凸*になります。

実際には、$F$ (それぞれ $F'$) の共通部分の $E$ と $E \times \mathbf{R}$ の超平面 $E \times \{\alpha\}$ が射影です。

#### 命題 20 {#evt-ii-s2-prop-20 .statement tag=07CE}

*$f$ を、アフィン * 空間 E の凸集合 $X$ 上で定義された凸写像とします。 次に、すべての家族 $(x_i)_{1 \leq i \leq p}$ の $p$ 点の X とすべての家族 $(\lambda_i)_{1 \leq i \leq p}$ の $p$ 実数、すべての $\geq 0$ について、$\sum_{i=1}^p \lambda_i = 1$ となるように、次のようになります。

(3)
$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) \leq \sum_{i=1}^p \lambda_i f(x_i).
$$

$f$ が厳密に凸であり、すべての $i$ に対して $\lambda_i > 0$ である場合、

(4)
$$
f\left( \sum_{i=1}^p \lambda_i x_i \right) < \sum_{i=1}^p \lambda_i f(x_i),
$$
〜でない限りすべての $x_i$ は等しいです。

不等式 (3) は II のプロップから続きます。上の 19 と II、p. 8、プロップ。 1. $x_i$ がすべて等しいわけではなく (これは $p \geq 2$ を意味します)、$\lambda_i$ がすべて $> 0$ であると仮定します。その場合、点 $z = \sum_{i=1}^p \lambda_i x_i$ は少なくとも 1 つの $x_i$ と異なります。明確にするために、$z \neq x_1$ と仮定し、$y_1 = \sum_{i=2}^p \frac{\lambda_i}{1 - \lambda_1} x_i$ に $z = \lambda_1 x_1 + (1 - \lambda_1) y_1$ を書き込みます。その後、$y_1 \neq x_1$、そして$0 < \lambda_1 < 1$として、仮定までに、
$$
f(z) < \lambda_1 f(x_1) + (1 - \lambda_1) f(y_1).
$$
しかし、(3) $f(y_1) \leq \sum_{i=2}^p \frac{\lambda_i}{1 - \lambda_1} f(x_i)$ によって、不等式 (4) が続きます。

### 9. 凸上演算写像

X をアフィン空間 E の凸集合とします。 $f_i (1 \leq i \leq p)$ が X 上で定義された有限個の凸写像で、$c_i (1 \leq i \leq p)$ が数 $\geq 0$ である場合、写像 $f = \sum_{i=1}^p c_i f_i$はXに凸です。

$(f_i)$ が X 上で定義された凸写像のファミリであり、X のファミリの上部包絡線である $g$ が有限である場合、$g$ は凸です。

最後に、H が X 上で定義された凸写像の集合であり、$\mathfrak{F}$ が X で有限実数値写像 $f_0$ に単純に収束する H 上のフィルターである場合、$f_0$ は X 上で凸です。

### 10. 開いた凸面集合の上に凸面写像

#### 命題 21 {#evt-ii-s2-prop-21 .statement tag=07CF}

$f$ を、トポロジカルベクトル空間 E の空でない開いた凸面集合 X 上で定義された凸面写像とします。そのとき、$f$ は、X の空ではない開いた部分集合 U に制限された場合に、上に有界される場合にのみ連続です。

条件は明らかに必要であり、それで十分であることを証明します。 $x_0 \in X$ を点として、$f$ が $x_0$ の近傍 V の上に境界があるようにします。まず、$f$ が $x_0$ で連続であることを示します。翻訳すると、$x_0 = 0$ と $f(x_0) = 0$ の場合に限定できます。さらに、近傍 V は均衡していると仮定できます (I、p. 7、提案 4)。 V で $f(x) \leq a$ だったとします。 $\varepsilon, 0 < \varepsilon < 1$ ごとに、$x \in \varepsilon V$ の場合、$x/\varepsilon \in V$ と $-x/\varepsilon \in V$ が観察されます。 適用不等式 (1) II、p. 16 から点 $x/\varepsilon$ と 0、そして数 $\lambda = \varepsilon$ から、$f(x) \leq \varepsilon f(x/\varepsilon) \leq \varepsilon a$ であることがわかります。 適用それを点 $x$ と $-x/\varepsilon$ および数 $\lambda = 1/(1 + \varepsilon)$ にすると、$f(x) \geq -\varepsilon f(-x/\varepsilon) \geq -\varepsilon a$ になります。したがって、$\varepsilon$ が十分に小さく、$f$ が $x = 0$ で連続である場合、$f(x)$ は$\varepsilon V$ において任意に小さくなります。

さて、$y$をXの点とします。 X が開いているので、$z = \rho y$ 属するから X までのような数 $\rho > 1$ があります。 $g$ を中心 $z$ のホモテティー $x \mapsto \lambda x + (1 - \lambda)z$ とし、変換 0 を $y$ に加える比率 $\lambda = 1 - \frac{1}{\rho}$ とします。 点 $g(x) \in g(V)$ ごとに、(1) から得られます。

$$
f(g(x)) \leq \lambda f(x) + (1 - \lambda) f(z) \leq \lambda a + (1 - \lambda) f(z) .
$$

したがって、$f$ は $y$ の近傍で境界があり、したがって最初の部分によって、$y$ で連続します。 命題が証明されました。

#### 系 {#evt-ii-s2-n10-cor-1 .statement tag=07CG}

*$\mathbf{R}^n$ の開いた凸集合 X 上に定義されたすべての凸写像 f は、X で連続します。

X は空ではないと仮定できます。そして、X, $n + 1$ アフィン独立な点 $a_i$ ($0 \leq i \leq n$) と、これら点, S, 含むの凸包絡線、点から形成される開いた空でない集合が存在します。 $\sum_{i=0}^n \lambda_i a_i$ と $0 < \lambda_i < 1$ はすべての $i$ と $\sum_{i=0}^n \lambda_i = 1$ に対応します。 II、p. 17、プロップにより。 20、$f$ は S の上で有界であるため、連続です。

無限次元のトポロジカルベクトル空間には、一般に線形非連続形 (II、p. 80、例題25)、したがってどの点でも連続しない凸状の写像が存在します。

### 11. 準標準と凸集合

E を $\mathbf{R}$ 以上ベクトル空間とします。 $\mathbf{R}$ の E の写像 $p$ は、すべての $\lambda \geq 0$ とすべての $x \in E$ について、

$$
p(\lambda x) = \lambda p(x) .
$$

E 上の正同次写像 $p$ は、E のすべての $x, y$ について II、p. 1 の公理 (SN$_{\text{II}}$) を満たす場合に限り、凸です。

$$
p(x + y) \leq p(x) + p(y) .
$$

実際、$p$ が凸の場合、E の $x, y$ については、

$$
p(\frac{1}{2}(x + y)) \leq \frac{1}{2}p(x) + \frac{1}{2}p(y)
$$

そして、(5) により、この関係は (6) と等価になります。逆に、(6) が成り立つ場合は、すべての $\lambda$ に対して $0 < \lambda < 1$ も成り立ちます。

$$
p(\lambda x + (1 - \lambda) y) \leq p(\lambda x) + p((1 - \lambda) y) = \lambda p(x) + (1 - \lambda) p(y)
$$

(5)を使って。

E 上の凸型の正に均一な写像は *サブリニア* と呼ばれます。

$p$ が E で定義されたサブリニア写像の場合。次に、$p(x) \leq a$ (それぞれ $p(x) < a$) が凸である点 $x \in E$ のすべての $a > 0$、集合 $V(p, a)$ (それぞれ $W(p, a)$) に対して、II, § 2.8、系によって計算されます。さらに、すべての $x \in E$ に対して、$p(\lambda x) = \lambda p(x) < a$ となるような $\lambda > 0$ が存在するため、この集合は *吸収性* です。

この結果の一部逆があります。

#### 命題 22 {#evt-ii-s2-prop-22 .statement tag=07CH}

*A を凸型集合、含む 0、ベクトル空間 E にします。すべての $x \in E$ に対して、* を置きます

$$
p_A(x) = \inf_{\rho > 0, x \in \rho A} \rho
$$
(0 $\leq p_A(x) \leq \infty$)。 *写像 $p_A$ は満たします*
$$
p_A(x + y) \leq p_A(x) + p_A(y), \qquad p_A(\lambda x) = \lambda p_A(x)
$$
*E のすべての $x, y$ と $\lambda > 0$ に対応します。 $V(p_A, \alpha)$ (それぞれ $W(p_A, \alpha)$) が $x \in E$ の集合を表し、それに対して $p_A(x) \leq \alpha$ (それぞれ $p_A(x) < \alpha$) が表される場合、*
$$
W(p_A, 1) \subset A \subset V(p_A, 1).
$$
*A が吸収性の場合、$p_A$ は有限* (したがって *サブリニア*) になります。

$\lambda > 0$ の場合、関係 $x \in \rho A$ と $\lambda x \in \lambda \rho A$ は等価であるため、$\lambda > 0$ に対して $p_A(\lambda x) = \lambda p_A(x)$ が得られます。 $x, y$ を E の 2 つの点とします。$x$ (それぞれ $y$) が A に吸収されない場合、$p_A(x) = +\infty$ (それぞれ $p_A(y) = +\infty$) と不等式 $p_A(x + y) \leq p_A(x) + p_A(y)$ は明らかに真です。 $x \in \alpha A$ と $y \in \beta A$ が存在する $\alpha > 0, \beta > 0$ が存在するとします。次に、$x + y \in \alpha A + \beta A = (\alpha + \beta) A$ (II、p. 8、*注意*);したがって、$p_A(x + y) \leq p_A(x) + p_A(y)$。 $A \subset V(p_A, 1)$ が含まれていることは明らかに真実です。 A が凸であり、含む 0 であるため、包含物 $W(p_A, 1) \subset A$ が続きます。最後に、A が吸収性であれば、$p_A$ は明らかに有限です。

(7) で定義される写像 $p_A$ は、凸面集合 A の *ゲージ* と呼ばれます。A が吸収性で対称であれば、$p_A$ は準ノルムです。

#### 命題 23 {#evt-ii-s2-prop-23 .statement tag=07CI}

*E をトポロジカルベクトル空間とします。 A が含む 0 である開凸集合である場合、$p_A$ は有限連続であり、$A = W(p_A, 1)$ です。 A が閉じた凸型集合含む 0 の場合、$p_A$ は下半連続であり、$A = V(p_A, 1)$* です。

A が開いており、含む 0 の場合、吸収性があります。 $x \in A$ の場合、$x / \rho \in A$ となるような $\rho < 1$ が存在し、したがって $p_A(x) < 1$ になります。これを (9) と組み合わせると、$A = W(p_A, 1)$ になります。凸型写像 $p_A$ は開いた集合 A で上に境界があるため、E で連続です (II, p. 18、提案 21)。

A が閉じていて含む 0 であるとします。$p_A(x) \leq 1$ を持つすべての $x \in E$ について、すべての $\rho > 1$ に対して $x \in \rho A$ が得られます。したがって、A が閉じているので $x \in A$ になります。 (9) を思い出してください。これは $A = V(p_A, 1)$ を示しています。したがって、すべての $\mu > 0$ に対して、$\mu A$ は $p_A(x) \leq \mu$ となる $x$ の集合です。 E の $p_A(x) \geq 0$ と同様に、これは $p_A$ が E で下位半連続であることを示しています (GT、IV, § 6.2)。

E 上の正のサブリニア写像 $p$ は、$W(p, 1) \subset A \subset V(p, 1)$ の各凸面集合 A のゲージです。

### 練習問題 {#evt-ii-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
