---
book: top
book_title: General Topology
chapter: V
chapter_title: One-parameter groups
section: 2
section_title: Measurement of magnitudes
lang: ja
source: top-v-x
pdf_pages: 0018-0023, 0031-0031
extraction: ocr
statements: 5
exercises: 2
content_sha256: 0706f492e818d7f27978a901c520a91f7e5df8069c8998d9b810de47cdf47e55
translated_from: content/en/top/V/02_s2_measurement_of_magnitudes.md
translation_method: google
source_content_sha256: 4c0d4a053c85b93dc23047deb4096b5b7869ee2eb4c5bc580d37bfd28b4c40a9
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 66490d9fab0931c2f84dd4da270ce709ab5c81b3df61f8c51deae11c34452ce8
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 2. 大きさの測定

私たちは、大きさの測定の問題が実数の概念の起源であることを (cf. 歴史的な注意から章 IV まで) 見てきました。より正確には、実際的または理論的な目的で徐々に研究されるようになったさまざまな型の大きさは、最初は互いに別々に考慮され、すべての型を同じ数系で測定する可能性が実験事実として現れ、前にギリシャ人は厳密な実証を行うという大胆なアイデアを思いつきました。 彼らが確立した公理理論では、大きさの概念は合成の法則（同じ型の大きさの「加法」）と順序関係（関係「AはBより小さい」、大きさの比較の関係と呼ばれる）に関連していました。 以下では、同じ問題を検討します。つまり、合成の内部法則と、位数の集合Eの順序関係に課せられる条件を調査します。これは、によって誘導される構造を備えたRの部分集合E'と同型である必要があります。 Rの加法と関係$\leq$。 E 上の合成の指定された法則が可換であるとは演繹的に仮定しないので、乗法記法を使用します。しかし、これを除けば、私たちは古典的な議論からほとんど離れることはありません。

E を $x \leq y$ と書かれた順序関係によって線形に順序付けされた集合とし、E が最小の要素 $\omega$ を持つと仮定します。 I を、$\omega \in I$ となり、関係 $x \in I$ と $y \leq x$ が $y \in I$ を意味するような E の部分集合とします。また、E に関する合成法則 $(x, y) \to xy$ が与えられ、積 $xy$ が I の要素のすべてのペアに対して定義されているとします ($xy$ は E に属しますが、必ずしも I に属するわけではありません)。 さらに、次の仮定を作成します。

(GR_I) $\omega$ は単位元 [すべての $x \in I$ に対して $\omega x = x \omega = x$] であり、合成の法則は結合的です [次の意味で: $x \in I, y \in I, z \in I, xy \in I$ と $yz \in I$ の場合、その後 $x(yz) = (xy)z$ の場合]。

(GR_{II}) I の元の間の関係 $x < y$ は、すべての $z \in I$、関係 $xz < yz$、$zx < zy$ を意味します。

(GR_{III}) I の元 $> \omega$ の集合は空ではなく、最小の元がありません。そして、$x < y$ となるような I の任意の元 $x, y$ が与えられると、$xz \leq y$ となるような $z > \omega$ が存在します。

条件 (GR_{II}) は、I の元間の不等式が項に項を乗算できることを意味します: $x < y$ と $x' < y'$ は $xx' < yy'$ ($xx' < yx'$ と$yx' < yy'$）。特に、すべての $x > \omega$ ($x \in I, y \in I$) に対して $y < yx$ があります。

I の元の有限列 $(x_i)_{1 \leq i \leq p}$ を考えると、この数列 $\prod_{i=1}^p x_i$ の $p$ 積を帰納法で定義する定義する $\left( \prod_{i=1}^{p-1} x_i \right) x_p$ に等しいとみなすことができます。 積 $\prod_{i=1}^{p-1} x_i$ が定義され、属する ～ I: したがって、$\prod_{i=1}^p x_i$ が定義されている場合、$2 \leq q \leq p - 1$ に対して、積 $\prod_{i=1}^q x_i$ がそれぞれ定義され、属する ～ I が定義されます。 すべての $x_i$ が同じ元 $x \in I$ に等しいとすると、特に、$x^p$ が定義されている場合、$x^q$ が定義され、$2 \leq q \leq p - 1$ に対して属するが I になることがわかります。 従来、すべての $x \in I$ に対して、定義する $x^0$ は $\omega$ に等しいと考えられます。 (GR$_\text{II}$) により、$x > \omega$ の場合、$x^p$ が定義されている場合、$1 \leq q \leq p - 1$ に対して $\omega < x^q < x^p$ が得られます。 $x < y$ で、$y^p$ が定義されている場合、($p$ の帰納法までに) $x^p$ と $x^p < y^p$ が定義されていることがわかります。 一方、結合性条件 (GR$_\text{I}$) は、$n$ の帰納法によって、$x^{m+n}$ が定義されている場合、$x^m x^n$ も定義され、$x^{m+n} = x^m x^n$ も定義されることを意味します。 逆に、(GR$_\text{I}$) と (GR$_\text{II}$) により、$x^m x^n$ が定義され、属するから I までの場合、$x^{m+n}$ が定義され、$x^{m+n} = x^m x^n$ が得られます。これもまた、$n$ の帰納法によって証明されます。$x^{n-1} \leq x^n$ があるため、$x^m x^{n-1}$ が定義され、属するから I になります。 仮定、$x^m x^{n-1} = x^{m+n-1} \in I$ により、$(x^{m+n-1})x = x^{m+n}$ は定義され、前の結果により $x^m x^n$ と等しくなります。 同様に、$n$ の帰納法によって、$x^{mn}$ が定義されている場合、$(x^m)^n$ が定義され、$x^{mn} = (x^m)^n$ が定義されることがわかります。逆に、$(x^m)^n$ が定義され、属する ～ I の場合、$x^{mn}$ が定義され、$(x^m)^n$ と等しくなります。

最後に、公理 (GR$_\text{III}$) は、$x > \omega$ のようなすべての $x \in I$ に対して、$y^2 \leq x$ のような $y > \omega$ が存在することを意味します。なぜなら、$x > \omega$ の場合、$z < x$ となるような $z > \omega$ が存在し、その後 $zt \leq x$ となるような $t > \omega$ が存在します。 $y$ を 2 つの元 $z, t$ のうち小さい方とします。 $n$ の帰納法までに、$u^{2^n} \leq x$ となるような $u > \omega$ が存在すると推測します。

それでは、次の仮定をご紹介します。

(GR$_\text{IV}$) (『アルキメデスの公理』)。 *すべて* $x \in I$ *および* $y \in I$ *そのような* $x > \omega$、*存在する* 整数* $n > 0$ *そのような* $x^n$ *が定義されており* $x^n > y$。

E を実数 $\geq 0$ の集合とし、含む 0 と任意に小さい数 $> 0$ とする場合、I は E の共通部分で、左側の終点が 0 である R の区間となります。 含む少なくとも 1 つの他の数、合成の法則は、I の元の加法となり、$x \in I$ と $y \in I$ のときは常に $x + y \in E$ であると仮定すると、公理は次のようになります。 (GR$_\text{I}$)、(GR$_\text{II}$)、(GR$_\text{III}$)、(GR$_\text{IV}$)が満たされます(*)。

(*) 実験科学で生じる「大きさ」の集合において、公理 (GR$_\text{I}$) と (GR$_\text{II}$) は一般に、少なくとも近似的に実験による検証が可能です。一方、「好きなだけ小さい」大きさの存在を仮定する公理 (GR$_\text{III}$) も、明らかにできない同様に確立されます。それは純粋に*先験的* 仮定です。公理 (GR$_\text{IV}$) に関しては、「小さすぎない」大きさについては実験によって検証できる事実の「外挿」と考えることができます。

逆に:

#### 命題 1 {#top-v-s2-prop-1 .statement tag=0BVG}

E を最小の元 ω で線形順序付けされた集合とします。 I を E の部分集合とし、ω ∈ I とし、関係 x ∈ I、y ≤ x は y ∈ I を意味します。 (x, y) → xy を E 上の合成の法則とし、x ∈ I および y ∈ I に対して定義します。次に、公理 (GR_I)、(GR_{II})、(GR_{III})、(GR_{IV}) が満たされる場合、実数の集合 R_+ に I の真に増加する写像 f が存在します。 ≥ 0、つまり

$$
f(xy) = f(x) + f(y)
$$

x ∈ I、y ∈ I、xy ∈ I の場合は常に;さらに、R のすべての区間 [0, f(b)] を持つ f(I) の共通部分は、この区間で密です。ここで、b は I の任意の元を表します。

y ≠ ω である I の任意の 2 つの元 x, y を与えて、y^n が定義され、≤ x (*) となるように (x : y) 最大の整数 n ≥ 0 で表します。この整数は (GR_{IV}) によって存在します。 (x : y) = p の場合、y^{p+1} が定義され、> x となります。 x ∈ I、y ∈ I、xy ∈ I の場合、次のようになります。

(I)
$$
(x : z) + (y : z) \leq (xy : z) \leq (x : z) + (y : z) + 1.
$$

(x : z) = p、(y : z) = q とします。この場合、z^p ≤ x、z^q ≤ y になります。 xy ∈ I であるため、z^p z^q が定義され、属するから I までであるため、z^{p+q} が定義され、z^{p+q} = z^p z^q ≤ xy;さらに、z^{p+q+2} が定義されている場合、z^{p+1} > x および z^{q+1} > y であるため、z^{p+q+2} > xy となります。

次に不等式を確立します

(2)
$$
\begin{cases}
(x : y) (y : z) \leq (x : z), \\
((x : y) + 1) ((y : z) + 1) \geq (x : z) + 1.
\end{cases}
$$

(x : y) = p および (y : z) = q とします。この場合、y^p ≤ x かつ z^q ≤ y となり、(z^q)^p が定義され ≤ x となります。それは属するしたがって I になります。その結果、z^{pq} が定義され、z^{pq} = (z^q)^p ≤ x となり、最初の不等式が続きます。一方、z^{(p+1)(q+1)} が定義されている場合、y^{p+1} > x および z^{q+1} > y であるため、z^{(p+1)(q+1)} > x になります。従って、2 番目の不等式です。

$\tilde{\mathscr{X}}$ は、関係 ≥ に関して、I の元 > ω の順序集合の切断のフィルターを表すものとします。 区間 ]ω, z[、z は、すべての元の集合 > ω、形基底の $\tilde{\mathscr{X}}$ を通過します。 a > ω となる 2 つの元 a と I の x が与えられた場合、比 $\frac{(x : z)}{(a : z)}$ は z ≤ a に対して定義され、有理数数 > 0 であることを示します。

(*) E=Iが自然整数の集合、合成の法則が加法のとき、(x:y)はx/yの積分部分になります。

は $z$ の写像で、$\mathfrak{F}$ に関して *極限* があります。これは、$x = \omega$ であれば、すべての $z$ に対して $(x : z) = 0$ であることは明らかです。 $x > \omega$ の場合、写像 $z \to \frac{(x : z)}{(a : z)}$ ($\leq x$ と $\leq a$ である $z > \omega$ のうち集合に限定) の下の $\mathfrak{F}$ の像 $\mathscr{G}$ がコーシーフィルターであることを示します。 *乗法* 群 $\mathbf{R}_+^*$ の一様構造に対する基底は、実数 $> 0$ に収束します。 注意まず、$u > \omega$ が与えられると、$(u : z)$ は$\mathfrak{F}$ に対して極限 $+\infty$ を持ちます。$z^{2^n} \leq u$ となる$z > \omega$ が存在するため、$(u : z) \geq 2^n > n$ になります。ここで、数 $\varepsilon > 0$ を任意に取ります。 $(x : t) \geq 1 / \varepsilon$ と $(a : t) \geq 1 / \varepsilon$ のような $t > \omega$ が存在します。ダブル不等式を考えてみましょう

$$
\frac{(x : t)}{(a : t) + 1} \cdot \frac{(t : z)}{(t : z) + 1} \leq \frac{(x : z)}{(a : z)} \leq \frac{(x : t) + 1}{(a : t)} \cdot \frac{(t : z) + 1}{(t : z)},
$$

これは不等式 (2) からすぐに得られます。 $z \leq z_0$ が $(t : z) \geq 1 / \varepsilon$ を暗示するような $z_0 > \omega$ が存在します。

$$
\frac{1}{(1 + \varepsilon)^2} \frac{(x : t)}{(a : t)} \leq \frac{(x : z)}{(a : z)} \leq (1 + \varepsilon)^2 \frac{(x : t)}{(a : t)},
$$

これは、$\mathscr{G}$ が乗算均一性のコーシー フィルター 基底であることを示しています。

元 $a > \omega$ (「メジャーの単位元」) を一度修正し、それぞれの $x \in I$ を置きます

$$
f(x) = \lim_{z \in \mathfrak{F}} \frac{(x : z)}{(a : z)}.
$$

すでに証明されていることから、$x > \omega$、$f(a) = 1$に対して$f(\omega) = 0$、$f(x) > 0$が得られます。 割る不等式 (1) を $(a : z)$ まで実行し、$\mathfrak{F}$ に関して極限に渡すと、次のことがわかります。

$$
f(xy) = f(x) + f(y)
$$

$x \in I, y \in I$ と $xy \in I$ のときはいつでも。同様に、関係 $x \leq y$ は、$(a : z)$ と移行から極限で割ることにより $(x : z) \leq (y : z)$、よってを意味し、$f(x) \leq f(y)$ となるため、$f$ は *増加する* になります。 $I$。 $f$ は $I$ の *真に増加する* であると推測します。なぜなら、$x < y$ の場合、$xz \leq y$、よって $f(xz) \leq f(y)$ となるような $z > \omega$ が存在します。そして$xz \in I$以降、

$$
f(x) + f(z) = f(xz) \leq f(y);
$$

でも$f(z) > 0$なので、確かに$f(x) < f(y)$です。

最後に$b \in I$なら、この区間には$f(I)$の共通部分と$\mathbf{R}$の$[0, f(b)]$区間が密集しています。なぜなら、$n$ が任意の整数 $> 0$ である場合、$f(x) \leq 2^{-n}$ となるような $x > \omega$ が存在します ($x^{2^n} \leq a$ となるような $x$ を取ります)。 $p$ が $x^{p+1} > b$ となる最小の整数である場合、$1 \leq q \leq p$ には $(p+1)f(x) > f(b)$ と $qf(x) \leq f(b)$ が存在します。したがって、$[0, f(b)]$ と長さ $> 2^{-n}$ 含むに含まれるすべての区間には、形 $qf(x) = f(x^q) \in f(I)$ の少なくとも 1 つの点が含まれます。したがって、命題 1 の証明は完了です。

#### 注意 1 {#top-v-s2-rem-1 .statement tag=0BVH}

関係 $x \in I, y \in I, xy \in I, yx \in I$ 暗示
$$
f(xy) = f(x) + f(y) = f(yx),
$$
したがって、$f$ は真に増加するであるため、$yx = xy$ となります。他の語、法則は、区間 $[0, b]$ 上の $E$ の合成の法則によって誘導されます (例: $b^2 \leq a$ となるように) は *可換* です。

#### 注意 2 {#top-v-s2-rem-2 .statement tag=0BVI}

$f$ と同じ条件を満たす $I$ の $\mathbf{R}_+$ へのすべての写像 $g$ は、$\lambda > 0$ である形 $x \to \lambda f(x)$ になります。 $\lambda = g(a) > 0$、関係 $z^p \leq x \leq z^{p+1}, z^q \leq a \leq z^{q+1}$ が仮定によって暗示される場合、
$$
pg(z) \leq g(x) \leq (p+1)g(z), \qquad qg(z) \leq g(a) \leq (q+1)g(z),
$$
よって
$$
\lambda \frac{(x : z)}{(q : z) + 1} \leq g(x) \leq \lambda \frac{(x : z) + 1}{(q : z)},
$$
したがって、$\tilde{x}$ に関して移行から極限は、$g(x) = \lambda f(x)$ になります。

$f(I)$ が $\mathbf{R}_+$ の *区間* である条件を求めましょう。明らかに、次の 2 つの条件が必要です。

(GR_{IIIa}) * $I$ の元 $> \omega$ の集合は空ではなく、最小の元もありません。そして、$x < y$ となるような $I$ の任意の 2 つの元 $x, y$ が与えられると、 $z \in I$ は $xz = y$* になります (大きさの「減算」)。

(GR_{IVa}) *$I$ の元によって上に囲まれている、$I$ の元のすべての増加する数列は、$I$* に少なくとも上界を持ちます。

これらの条件も十分であること、さらに、公理 (GR_{IV}) (アルキメデスの公理) を省略できることを示します。正確には、次の命題を証明します。

#### 命題 2 {#top-v-s2-prop-2 .statement tag=0BVJ}

*If a linearly ordered set $E$ and a subset $I$ of $E$ satisfy the axioms (GR_I), (GR_{II}), (GR_{IIIa}) and (GR_{IVa}), there exists a strictly increasing mapping $f$ of $I$ onto an interval of $\mathbf{R}$, with $0$ as its left-hand end-point, such that $f(\omega) = 0$ and $f(xy) = f(x) + f(y)$ whenever $x, y$ and $xy$ belong to $I$.*

まず公理 (GR_{IV}) が満たされることを示しましょう。私たちは矛盾によって議論します: $x > \omega$、$x^n$ が定義され、すべての整数 $n > 0$ に対して $x^n \leq y$ が定義されるような $x, y \in I$ が存在すると仮定します。 増加する数列 $(x^n)$ には、(GR$_{\text{IV}_a}$) による少なくとも上界 $b \in I$ があります。 $x < b$ 以降、(GR$_{\text{III}_a}$) によって $xc = b$ となるような $c \in I$ が存在し、$x > \omega$ 以降は $c < b$ になります。さて、すべての $n$ に対して、(GR$_{\text{II}}$) によって $x^{n+1} \leq b = xc$、よって $x^n \leq c$ が得られます。したがって、$x^n$ の上界 $b$ は $\leq c$ となり、これは矛盾です。

したがって、命題を適用する 1 のポジションにあります。 $\gamma = f(c)$ ($c > \omega$) が $f(I)$ の任意の要素であり、$\beta$ が $0 < \beta < \gamma$ のような実数である場合、$f(b) = \beta$ のような $b \in I$ が存在することを示すことが残っています (IV, § 2, no. 4 章、命題 1)。 $f(I)$と$[0, \gamma]$の共通部分が$[0, \gamma]$に密であるため、$f(x_n)$が極限として$\beta$を持つように、$I$の元の増加する数列$(x_n)$が存在します。 $b$ を $I$ の数列 $(x_n)$ のうち最小の上界とします。すべての $n$ に対して $f(b) \geq f(x_n)$ があるため、$f(b) \geq \beta$ になります。しかし、$f(b) > \beta$は不可能です。そうでなければ、$\beta < f(y) < f(b)$のような$y \in I$が存在します。そして、$\beta$は数列$(f(x_n))$の最小の上界であるため、すべての$n$、よってに対して$f(x_n) < f(y) < f(b)$が必要です。 $n$全員に対して$x_n < y < b$、これは不合理です。 したがって、$f(b) = \beta$、および命題 2 が証明されます。

#### 注意 {#top-v-s2-n0-rem-3 .statement tag=0BVK}

$I = E$、像 $f(I) = f(E)$ が $\mathbf{R}_+$ の全体である場合、$b > \omega$ の場合、すべての $n$ に対して $b^n$ が定義されるため、すべての $n$ に対して $n \cdot f(b)$ 属するから $f(E)$ が定義されます。これは、$f(b) > 0$ のため、$f(E)$ が上に制限されていないことを意味します。

### 練習問題 {#top-v-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
