---
book: int
book_title: Integration
chapter: I
chapter_title: INEQUALITIES OF CONVEXITY
section: 0
section_title: INEQUALITIES OF CONVEXITY
kind: front
lang: ja
source: int-i-vi
pdf_pages: 0016-0022
extraction: ocr
subsections:
    - "no": 1
      title: The fundamental inequality of convexity
      page: 0
      pdf_page: 16
    - "no": 3
      title: The semi-norms $N_p$
      page: 4
      pdf_page: 19
statements: 0
exercises: 0
content_sha256: 5a2f005f8dab0fea5099e6f91910bd16162fb092101bebc53c49f87beeb68e70
translated_from: content/en/int/I/00_frontmatter.md
translation_method: google
source_content_sha256: f9fb1f9ad9415bc967e08205858a5af5eecf03e7f2b0b9123eb6a2caf75a5af8
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: 56a18de05305b0ca4767c1a3051879386aa11cb208cfe4db02662f6ec445fde9
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 章 I

# 凸性の不等式

### 1. 凸性の基本不等式

X を集合とします。 X で定義されたすべての有限数値写像$^1$ のベクトル空間 $\mathbf{R}^X$ において、P を X のすべての正の実数値写像の集合とします。一方、$M$ を、P 上で定義された値 $\geqslant 0$ を使用して、次のような数値写像、$^2$ が有限であるかどうかとしましょう。

$1^\circ$ $M(0) = 0$、および $M$ は正に同次です。つまり、実数 $\lambda > 0$.$^3$ ごとに $M(\lambda f) = \lambda M(f)$ です。

$2^\circ$ $M$ は P では増加するであり、他の語関係 $f \leqslant g$ は $M(f) \leqslant M(g)$ を暗示します。

$3^\circ$ $M$ は P に凸で、その他の語 (TVS、II, §2, No. 8) は関係 $M(f + g) \leqslant M(f) + M(g)$ を満たします。

*例.* — X が有限の集合であるとします。たとえば、$\mathbf{N}$ の区間 $[1, n]$ です。 $x_i$ ($1 \leqslant i \leqslant n$) でベクトル $\mathbf{x} \in \mathbf{R}^n$、写像の座標を表します
$$
M_1(\mathbf{x}) = \sum_{i=1}^n x_i \quad \text{and} \quad M_\infty(\mathbf{x}) = \sup_{1 \leqslant i \leqslant n} x_i
$$
ベクトル $\mathbf{x}$ の集合 P にある前の条件の満たすの座標は $\geqslant 0$ です。

*注意.* — S を P に含まれる尖った凸円錐とします (つまり、$\lambda \geqslant 0$ に対して $S + S \subset S$ と $\lambda S \subset S$、cf. TVS、II, §2, No. 4 となるような集合)。 $M$ を数値写像 (有限かどうか) とし、値 $\geqslant 0$ を S で定義し、S で満たす、上記の条件 $1^\circ, 2^\circ$ と $3^\circ$ を定義します。次に、$M$ は、拡張された写像 (これを再び $M$ で示します) が同じ条件を満たすように、集合 P 全体に拡張できます。すべての写像 $f \in P$ から集合について、それで十分です。 $f \leqslant g$ のような写像 $g \in S$ が存在しない場合は $M(f) = +\infty$、その逆の場合は $M(f) = \inf_{g \in S, f \leqslant g} M(g)$ です。この手順は第 3 章で適用されます。 IV, §1 から定義するは、正の写像の*上積分*。

(1) 有限数値関数 ($\mathbf{R}$ に値を含む写像) は、「実数値写像」 (cf. GT、IV, §5, No. 1) とも訳される場合があります。

(2) 関数 numérique —「数値写像」—は、$\overline{\mathbf{R}}$ (TG、IV, §5, No. 1) の値を含む写像を意味します。 「有限であるか否か」というフレーズは、写像が無限の値になる可能性があることを思い出させるために、ときどきに追加されています。

(3) $\overline{\mathbf{R}}$、積では、$0 \cdot (+\infty)$ などは定義されていないことに注意してください (GT、IV, §4, No. 3)。

命題 1. — $\varphi(t_1, t_2, \ldots, t_n)$ を、$t_i \geq 0$ ($1 \leq i \leq n$) に対して定義され連続する有限数値写像とします。次のようになります。
$1^\circ$ 関係 $t_i > 0$ ($1 \leq i \leq n$) は $\varphi(t_1, t_2, \ldots, t_n) > 0$ を暗示します。
$2^\circ$ 写像 $\varphi$ は確実に均一です。
$3^\circ$ 集合 $K \subset \mathbf{R}^n$ は関係 $t_i \geq 0$ ($1 \leq i \leq n$) で定義され、$\varphi(t_1, t_2, \ldots, t_n) \geq 1$ は凸です。
これらの条件の下で、$f_1, f_2, \ldots, f_n$ が $X$ で定義された $n$ 有限写像 $\geq 0$ である場合、$1 \leq i \leq n$ に対して $M(f_i) < +\infty$ となるように、

$$
M(\varphi(f_1, f_2, \ldots, f_n)) \leq \varphi(M(f_1), M(f_2), \ldots, M(f_n)).
$$

ハーン・バナッハ定理 (TVS、II, §5) により、$K$ は $n$ ハーフスペース $t_i \geq 0$ ($1 \leq i \leq n$) の共通部分であり、閉じたハーフスペース $(U_\iota)_{\iota \in I}$、$U_\iota$ のファミリーであることがわかります。 形の関係によって定義

$$
\alpha_{\iota 1} t_1 + \alpha_{\iota 2} t_2 + \cdots + \alpha_{\iota n} t_n - \beta_\iota \geq 0,
$$

ここで、$\alpha_{\iota k}$ はすべて零ではありません。 仮定までに、$t = (t_i)$が$1 \leq i \leq n$に対して$t_i > 0$となる場合、$\varphi(t_1, \ldots, t_n) > 0$となるため、関係$\lambda \geq \lambda_0$が$\lambda t \in K$を暗示するような$\lambda_0 > 0$が存在します。これは、各 $\iota \in I$、関係 $t_i \geq 0$ ($1 \leq i \leq n$) が $\alpha_{\iota 1} t_1 + \cdots + \alpha_{\iota n} t_n \geq 0$ を暗示し、したがって $1 \leq k \leq n$ に対して $\alpha_{\iota k} \geq 0$ を意味することを示しています。したがって、$K$ は、$\beta_\iota \geq 0$ となるような半角スペース $t_i \geq 0$ ($1 \leq i \leq n$) と $U_\iota$ の共通部分であることは明らかです。さらに、原点は属するから $K$ ではないため、$\beta_\iota > 0$ となるような添字 $\iota$ が少なくとも 1 つ存在します。

ここで、$C$ を、関係 $t_i \geq 0$ ($1 \leq i \leq n+1$)、$t_{n+1} \leq \varphi(t_1, t_2, \ldots, t_n)$ (凸集合 $K \times \{1\}$ によって$\mathbf{R}^{n+1}$ で生成された凸円錐の閉包) によって定義される $\mathbf{R}^{n+1}$ の凸円錐とします。 $C$ は関係 $t_i \geq 0$ ($1 \leq i \leq n+1$) によっても定義されるのは明らかであり、

$$
\beta_\iota t_{n+1} \leq \alpha_{\iota 1} t_1 + \cdots + \alpha_{\iota n} t_n \quad (\iota \in I, \ \beta_\iota \geq 0).
$$

したがって、$x \in X$ ごとに、

$$
\beta_\iota \varphi(f_1(x), \ldots, f_n(x)) \leq \alpha_{\iota 1} f_1(x) + \cdots + \alpha_{\iota n} f_n(x)
$$

$\iota \in I$ 全員のために。 $\beta_\iota > 0$ となるすべての添字 $\iota$ について、(4) と $M$ の仮説から、$M(\varphi(f_1, f_2, \ldots, f_n))$ は有限であり、

$$
\beta_\iota M(\varphi(f_1, f_2, \ldots, f_n)) \leq \alpha_{\iota 1} M(f_1) + \alpha_{\iota 2} M(f_2) + \cdots + \alpha_{\iota n} M(f_n),
$$

そしてこの関係も、$\beta_\iota = 0$ であれば明らかな方法で検証されます。したがって、座標が点であることがわかります。

$$
M(f_1), M(f_2), \ldots, M(f_n), \quad M(\varphi(f_1, f_2, \ldots, f_n))
$$

属するから $C$ まで、これは命題であることを証明します。

2. ヘルダーとミンコフスキーの不等式

このNo.および次のNo.において、$X$と$P$はNo. 1と同じ意味であり、$M$はNo. 1に記載されている条件を満たす、$P$で定義された写像を示します。

命題 2. — *$\alpha$ と $\beta$ を 2 つの数として、$0 < \alpha < 1$、$0 < \beta < 1$、$\alpha + \beta = 1$ とします。 $f$ と $g$ が $X$ で定義された 2 つの有限写像 $\geq 0$ であり、$M(f)$ と $M(g)$ が有限である場合、*

$$
M(f^\alpha g^\beta) \leq (M(f))^\alpha (M(g))^\beta
$$

(*ヘルダーの不等式*)。

提案 1 によれば、すべては、$\mathbf{R}^2$ において、関係 $t_1 \geq 0$、$t_2 \geq 0$、$t_1^\alpha t_2^\beta \geq 1$ によって定義される集合が凸であるか、または再び (FRV、I, §4, No. 1、定義 1) であるという証明に帰着します。 写像 $u(t) = t^{-\alpha/\beta}$は$0 < t < +\infty$に凸です。さて、設定 $r = \alpha/\beta$ には $D^2 u(t) = r(r+1)t^{-r-2}$ があり、$r > 0$ から $]0, +\infty[$ には $D^2 u(t) > 0$ があり、これは命題であることが証明されます (FRV、I, §4, No. 4、提案 8 の裏付け)。

系。 — *$\alpha_i$ ($1 \leq i \leq n$) を $n$ 数 $\geq 0$ とする*
$$
\sum_{i=1}^n \alpha_i = 1,
$$
*そして、$f_i$ ($1 \leq i \leq n$) を $X$ で定義された $n$ 写像 $\geq 0$ とし、$M(f_i)$ が $1 \leq i \leq n$ に対して有限であるようにします。これら条件の下に、*

$$
M(f_1^{\alpha_1} f_2^{\alpha_2} \cdots f_n^{\alpha_n}) \leq (M(f_1))^{\alpha_1} (M(f_2))^{\alpha_2} \cdots (M(f_n))^{\alpha_n}.
$$

$i$ごとに$\alpha_i > 0$となる場合に注意を制限できます。 $n$については帰納法、適用不等式(5)から数$\alpha = \alpha_1$と$\beta = \sum_{i=2}^n \alpha_i$、そして写像$f = f_1$、$g = (f_2^{\alpha_2} f_3^{\alpha_3} \cdots f_n^{\alpha_n})^{1/\beta}$について議論するだけで十分です。

命題 3. — *$p$ を実数 $\geq 1$ とします。 $f$ と $g$ が $X$ で定義された 2 つの有限写像 $\geq 0$ である場合、*

$$
\left( M((f+g)^p) \right)^{1/p} \leq \left( M(f^p) \right)^{1/p} + \left( M(g^p) \right)^{1/p}
$$

(*ミンコフスキーの不等式*)。

$M(f^p)$ と $M(g^p)$ が有限である場合に注意を制限できます。提案 1 により、関係 $t_1 \geq 0,\ t_2 \geq 0,\ t_1^{1/p} + t_2^{1/p} \geq 1$ によって定義される $\mathbf{R}^2$ の集合が凸である、または再び写像 $u(t) = (1 - t^{1/p})^p$ が $0 \leq t \leq 1$ に対して凸であるという証明に還元されます。さて、

$$
D^2 u(t) = \left(1 - \frac{1}{p}\right)t^{1/p-2}(1-t^{1/p})^{p-2} \geq 0
$$

$0 < t \leq 1$、よって命題の場合。

### 3. 準規範 $N_p$

$p$ を実数 $\geq 1$ とし、$\mathscr{F}^p(X, M)$ を $X$ で定義された有限数値写像 $f$ の集合とし、$M(|f|^p)$ が *有限* であるようにします。 $g$ が写像所属 ～ $\mathscr{F}^p(X, M)$ であり、$|f| \leq |g|$ の場合、$f$ も属する ～ $\mathscr{F}^p(X, M)$ であることは明らかです。この注意とミンコフスキーの不等式は、$\mathscr{F}^p(X, M)$ の 2 つの写像のうち和も、この集合に対して属するであることを示しています。 $M$ が正に同次であるという事実を考慮すると、$\mathscr{F}^p(X, M)$ は、$X$ で定義されたすべての有限数値写像の空間 $\mathbf{R}^X$ の *線形部分空間* であることがわかります。

すべての数 $p > 0$ および $X$、集合で定義されたすべての有限数値写像 $f$ について

$$
N_p(f) = \left(M(|f|^p)\right)^{1/p};
$$

次に、すべてのスカラー $\lambda$ に対して $N_p(\lambda f) = |\lambda| N_p(f)$;さらに、$p \geq 1$ の場合、(7) により、

$$
N_p(f+g) \leq N_p(f) + N_p(g),
$$

これは、ベクトル空間 $\mathscr{F}^p(X, M)$ (TVS、II, §1) では、$N_p$ が *準標準* であることを証明しています。

**命題 4.** — *$p$ と $q$ を 2 つの実数 $> 0$ と集合 $1/r = 1/p + 1/q$ とします。 $X$ で定義された有限数値写像 $f, g$ について、*

$$
N_r(fg) \leq N_p(f) N_q(g)
$$

*ただし、$N_p(f)$ と $N_q(g)$ は有限であるとします。*

関係 (9) と書くことができます

$$
M(|f|^r |g|^r) \leq (M(|f|^p))^{r/p} (M(|g|^q))^{r/q},
$$

これは、他でもないヘルダーの不等式 (5) を数 $\alpha = r/p$ と $\beta = r/q$ 、および写像 $|f|^p$ と $|g|^q$ に適用したものです。

系。 — *次のように仮定します* $M(1) = 1$; *その後、すべての有限数値写像* $f$ *上で定義された* $X$、*写像* $p \mapsto N_p(f)$ *は増加するで* $]0, +\infty[$ になります。

Applying the inequality (9) to the case that $g = 1$, we see that $N_r(f) \leq N_p(f)$ for all $q > 0$; since the number $r$ defined by $1/r = 1/p + 1/q$ runs over the set of numbers such that $0 < r < p$ when $q$ runs over the set of numbers $> 0$, the corollary is proved.

命題 5. — *すべての有限数値写像* $f$ *上で定義* $X$、*集合* $I$ *of 値 of* $1/p$ ($p > 0$) *そのような* $N_p(f)$ *は有限である空か、区間のいずれかです。 * $I$ * が点に縮小されない場合、 写像* $\alpha \mapsto \log N_{1/\alpha}(f)$ * は $I$ 上に凸であるか、 * $I$ の内側にある* $-\infty$ に等しい。

$r$ と $s$ を 2 つの異なる数 $> 0$ として、$1/r$ と $1/s$ 属するから $I$ とします。すべては証明に帰着します。

$$
\frac{1}{p} = \frac{t}{r} + \frac{1-t}{s},
$$

$0 < t < 1$ を使用すると、

$$
\log N_p(f) \leq t \cdot \log N_r(f) + (1-t) \log N_s(f),
$$

あるいは、結局のところ、

$$
N_p(f) \leq (N_r(f))^t (N_s(f))^{1-t},
$$

$N_p$ の定義までに、関係が書き込まれる可能性があります

$$
M(|f|^p) \leq (M(|f|^r))^{tp/r} (M(|f|^s))^{(1-t)p/s}.
$$

設定 $\alpha = tp/r$ では、関係によって $1-\alpha = (1-t)p/s$ が得られ、定義する $p$ は $t, r, s$ の写像として計算されます。 よって $p = \alpha r + (1-\alpha)s$。ヘルダーの不等式は現在、

$$
M(|f|^{r\alpha}|f|^{s(1-\alpha)}) \leq (M(|f|^r))^{\alpha} (M(|f|^s))^{1-\alpha},
$$

それは他ならぬ不等式 (12) です。

練習問題

1) No. 1 の仮説を使用して、$M(|f|)$ が有限であるようなX 上の有界写像の集合は$\mathbf{R}^X$ の部分代数 A であり、X 上の有界写像の集合は次のようになります。 A における$M(|f|) = 0$ はイデアルです。さらに、$M(1)$ が有限である場合、A にX の一様収束の位相が備わっているとき、写像 $f \mapsto M(f)$ は連続であることを示せます。

2) X を $\mathbf{R}$ の区間 $[0, +\infty[$ とします。S は、X 上で $0 \leq f(x) \leq kx$ となるように、X で定義された写像によって形成される凸円錐です (有限の数 $k > 0$ の場合は、 $f$）。 集合 $M(f) = 0$ は $f \in S$ に、$M(f) = +\infty$ はすべての正の写像 $f$ が S に対して所属ではなく X に定義されています。 $M$ が No. 1 の条件を満たすことを示し、 数 $r > 0$ が 1 に等しくない場合は、$M(x) = 0$、および $M(x^r) = +\infty$。

3) 例を与えます。ここで、X は 2 つの元を持つ集合であり、$N_p(\mathbf{x})$ はすべての $p > 0$ とすべての $\mathbf{x} \in \mathbf{R}^2$ に対して有限ですが、写像となるような $p$ の値が存在する場合です。 $p \mapsto N_p(\mathbf{x})$ はこれらの点では微分できません。

4) 幾何平均の不等式から不等式 (6)を推定します。

$$
z_1^{\alpha_1} z_2^{\alpha_2} \cdots z_n^{\alpha_n} \leq \alpha_1 z_1 + \cdots + \alpha_n z_n \quad \text{(where } \sum_{i=1}^n \alpha_i = 1 \text{)}
$$

(FRV、III, §1, No. 1、提案 2)。 ($1 \leq i \leq n$が$M(f_i) = 1$の場合は簡約する)。

5) $\alpha$ を実数 $> 1$ とし、$\beta = 1 - \alpha < 0$ とします。 $g$ を、X で定義された有限の写像とし、すべての $x \in X$ に対して $g(x) > 0$ となり、$M(g) > 0$ となるようにします。 $M(f)$ が有限であるように、X で定義されたすべての有限写像 $f \geq 0$ について、

$$
M(f^\alpha g^\beta) \geq (M(f))^\alpha (M(g))^\beta
$$

(Hölder の不等式を適切に適用します)。

6) ヘルダーの不等式からミンコフスキーの不等式を推定します (ヘルダーの不等式を利用して、$M((f+g)^{p-1})$ に対する上界を見つけます)。 写像 $f, g$ のすべての対に対して $M(f+g) = M(f) + M(g)$ が定義され、$X$ には $\geq 0$ が定義されると仮定すると、同様に Exer から推測できます。 5 不等式

$$
(M((f+g)^p))^{1/p} \geq (M(f^p))^{1/p} + (M(g^p))^{1/p}
$$

次の場合:

a) $X$ で定義された$0 < p < 1$、$f$、$g$ は有限写像 $\geq 0$ で、すべての$x \in X$ に対して$f(x) + g(x) > 0$ となり、$M(f^p)$ と$M(g^p)$ は有限になります。

b) $X$ で定義された$p < 0$、$f$、および$g$ の有限写像。すべての$x \in X$、$M(f^p)$、および$M(g^p)$ に対して$f(x) > 0$ と$g(x) > 0$ が有限であるように、 $M((f+g)^p) > 0$。
