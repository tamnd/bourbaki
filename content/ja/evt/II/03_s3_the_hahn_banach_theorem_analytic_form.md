---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 3
section_title: The Hahn-Banach Theorem (analytic form)
lang: ja
source: evt-i-v
book_pages: TVS II.21-TVS II.23, TVS II.72-TVS II.74
pdf_pages: 0058-0060, 0109-0111
extraction: ocr
subsections:
    - "no": 1
      title: Extension of positive linear forms
      page: 21
      pdf_page: 58
    - "no": 2
      title: The Hahn-Banach theorem (analytic form)
      page: 22
      pdf_page: 59
statements: 6
exercises: 8
content_sha256: df2bdceaaaa78d80e60fd79a98741d05bf8dc725430f40c27d46ca4ca150c1b8
translated_from: content/en/evt/II/03_s3_the_hahn_banach_theorem_analytic_form.md
translation_method: google
source_content_sha256: 62f888c305293cb384c8f41fb0d8824e2a25c39637bd4054f2e1ce6efe281846
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 33eb1a1c5eef4c15a4d2b1278a19d00974adca0e51e2d87f9b0a6bdfbcb9fa01
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 3。ハーン・バナッハ定理 (分析的形)

### 1. 拡大 / 陽性線型形式

#### 命題 1 {#evt-ii-s3-prop-1 .statement tag=07DQ}

— E を事前に順序付けされたベクトル空間とし、V を E のベクトル部分空間とし、E のすべての元がその上で V の元によって制限されるようにします。 V の事前順序付けされたベクトル空間構造に対して正である V 上の線型形式 f が与えられると (E のそれによって誘導される)、E 上に正の線型形式の空ではない集合 $S_f$ が存在し、それぞれは f の拡大になります。 $h \in S_f$ の場合、$a \in E$ の値 $h(a)$ は区間 $[\alpha', \alpha'']$ にあります。

$$
\alpha' = \sup_{z \in V, z \leq a} f(z), \quad \alpha'' = \inf_{y \in V, y \geq a} f(y).
$$

I。特殊なケース。

まず$E = V + \mathbf{R}a$とします。 $a \in V$ の場合、命題は自明なので、$a \notin V$ の場合に限定します。 V の条件は、$y \in V$ の集合 $A''$ が、$a \leq y$ が空ではないことを意味します。同様に、$z \in V$ の集合 $A'$ は、$-z \geq -a$ (\emph{i.e.} $z \leq a$) が空ではありません。 $y \in A''$ と $z \in A'$ の場合は $z \leq a \leq y$ なので、仮定 $f(z) \leq f(y)$ になります。したがって、$\alpha', \alpha''$ は有限であり、$\alpha' \leq \alpha''$ です。 拡大する $f$ である E 上の任意の線型形式 $f_1$ は、$f_1(a)$ によって完全に決定され、すべての $\lambda \in \mathbf{R}$ とすべての $x \in V$ について、次のようになります。

$$
f_1(x + \lambda a) = f(x) + \lambda f_1(a).
$$

したがって、$f_1$ は、関係の場合にのみ正になります。

$$
x \in V, \quad \lambda \in \mathbf{R}, \quad x + \lambda a \geq 0
$$

暗示する

$$
f(x) + \lambda f_1(a) \geq 0.
$$

$f(\mu x) = \mu f(x)$ と関係 $x \geq 0$ と $\mu x \geq 0$ は $\mu > 0$ と同等であるため、特定のケース $\lambda = 0, \lambda = 1$ と $\lambda = -1$ では (2) が (3) を意味することを示すだけで十分です。 $\lambda = 0$ の場合、(2) が (3) を意味するという事実は、仮定から $f$ が正であることを示します。 $\lambda = 1$ について、(2) が (3) を意味すると言うことは、$-x \in A'$ については $f_1(a) \geq f(-x)$、\emph{つまり} $f_1(a) \geq \alpha'$ があることを意味します。 $\lambda = -1$ の場合、(2) は (3) を意味します。これは、$x \in A''$ の場合、$f(x) \geq f_1(a)$、\emph{すなわち} $f_1(a) \leq \alpha''$ があることを意味します。したがって、この場合は命題が証明されます。

II。一般的なケース。

$\mathfrak{F}$ を対 $(W, g)$ の集合とします。ここで、$W$ は $E$ 含む $V$ のベクトル部分空間であり、$g$ は正の線型形式です$f$の拡大である$W$。 $W \subset W'$ で、$g'$ が $g$ の拡大である場合、位数 $\mathfrak{F}$ は $(W, g) \leq (W', g')$ となります。明らかに $\mathfrak{F}$ は帰納的であり、th によるものです。 Sの2、III, § 2.4、極大元$(W_0, g_0)$があります。 $W_0 \neq E$ と仮定します。次に、ベクトル $b \notin W_0$ が存在し、$W_1 = W_0 + \mathbf{R}b$ の場合、上記の特殊なケースは、$W_1$ に正の線型形式、つまり $g_0$ の拡大が存在することを示しています。これ矛盾する仮定その $(W_0, g_0)$ が最大です。したがって、$W_0 = E$、および命題の最初の部分が証明されます。 $a \in V$ の場合、2 番目の主張は $\alpha' = \alpha'' = f(a)$ に対して明らかに真です。逆に、$a \notin V$ に $V_1 = V + \mathbf{R}a$ を入れると、2 番目の主張は証明の特別なケース I から続きます。

#### 系 {#evt-ii-s3-n1-cor-1 .statement tag=07DR}

互換性のある予約注文構造を持つトポロジー ベクトル空間 $E$ では、$P$ を $E$ の元 $\geq 0$ の集合とします。 $V$ を $E$ 含むのベクトル部分空間、$P$ の少なくとも 1 つの内部点 $x_0$ とします。次に、$V$ のすべてのポジティブな線型形式は、$E$ のポジティブな線型形式に拡張できます。

プロップにより。 1 すべての $x \in E$ に対して、$x' - x \in P$ となるような $x' \in V$ が存在することを示すだけで十分です。ここで、$U$ を $E$ の $0$ の近傍として、$x_0 + U \subset P$ とします。次に、$x + x_0 + U \subset x + P$、したがって、$0 < \varepsilon < 1$ と点 $y = x_0 + (1 - \varepsilon)x$ 属するから $x + P$ となるような $\varepsilon$ が存在します。その後、形 $x + \lambda(y - x)$ 属するから $x + P$ までの点ごとに $\lambda > 0$ になります。 $\lambda = 1/\varepsilon$ を取ると、$x + \lambda(y - x) = \lambda x_0 \in V$ となり、そこから結論が得られます。

$E$ が有限次元のものであっても、$P \cap V$ 含むであっても、$V$ 含むが $P$ の内点であると仮定しない場合、系の結論は必ずしも有効ではありません。 点 $V$ の内部 (II、p. 91、演習 25、b))。

### 2. ハーン・バナッハ定理 (分析的形)

#### 定理 1 (ハーン・バナッハ) {#evt-ii-s3-thm-1 .statement tag=07DS}

$p$ をベクトル空間 $E$ 上のサブリニア写像とします。 $V$ を $E$ のベクトル部分空間と $V$ 上の $f$ 線型形式とすることで、すべての $y \in V$ に対して $f(y) \leq p(y)$ が得られます。次に、$E$ には $f$ の拡大である線型形式 $h$ が存在し、$x \in E$ に対して $h(x) \leq p(x)$ が存在します。

対 $(x, a)$ の集合は、$p(x) \leq a$ が凸ベクトル空間 $E_1 = E \times \mathbf{R}$ の部分集合 $P$ (II、p. 17、提案 19) であり、明らかに尖っています。コーン。 $V_1$ を点 $(y, a) \in V_1$ ごとに $E_1$ と $g(y, a) = -f(y) + a$ の部分空間 $V \times \mathbf{R}$ とします。この場合、$g$ は、$P \cap V_1$ によって定義される $V_1$ の予約注文構造に対して正の線型形式になります。 $(y, a) \in P \cap V_1$ の場合、$a \geq p(y) \geq f(y)$、したがって $g(y, a) \geq 0$ です。次に $(x, a) \in E_1$ を見てみましょう。 $P$ で定義された予約注文の場合、$(x, a)$ は $V_1$ の点より小さいことがわかります。 $(x', a') \in V_1$ の場合、次に $(x, a) \leq (x', a')$ の場合、および $a' \geq p(-x) + a$ を考慮して $p(x' - x) \leq a' - a$ の場合に限り、$V_1$ の $(0, a')$ が要件を満たしていることがわかります。したがって、propを適用することができます。 I/II、p. 21; $g$を延長する$E_1$には線型形式$u$があり、$P$で定義された予約注文がポジティブです。したがって、$u(0, 1) = g(0, 1) = 1$ と $u$ は形 $u(x, a) = -h(x) + a$ であり、$h$ は拡大する $f$ の $E$ 上の線型形式です。さらに、すべての $x \in E$ とすべての $a \geq p(x)$ に対して、$h(x) \leq a$ があり、したがって $h(x) \leq p(x)$ になります。 Q.E.D.

#### 系 1 {#evt-ii-s3-thm-1-cor-1 .statement tag=07DT}

— $p$ をベクトル空間 $E$ の準標準とします。 $V$ を $E$ のベクトル部分空間と、$V$ の $f$ 線型形式とし、すべての $y \in V$ について $|f(y)| \leq p(y)$ とします。次に、$f$の拡大である$E$に定義された線型形式$h$が存在し、$x \in E$に対して$|h(x)| \leq p(x)$となるようなものです。

$E$ の準ノルム $q$ と線型形式 $g$ の場合、関係 $g \leq q$ は $|g| \leq q$ と同じです。 系は th から続きます。 1.

#### 系 2 {#evt-ii-s3-thm-1-cor-2 .statement tag=07DU}

— $p$ をベクトル空間 $E$ の準標準とします。 点 $x_0 \in E$ が与えられると、$E$ に対して定義された線型形式 $f$ が存在し、すべての $x \in E$ に対して $f(x_0) = p(x_0)$ と $|f(x)| \leq p(x)$ が存在します。

コルを適用します。 1 から $x_0$ によって生成されたベクトル部分空間、$V$、および $V$ で定義された線型形式 $\xi x_0 \mapsto \xi p(x_0)$ まで。

#### 系 3 {#evt-ii-s3-thm-1-cor-3 .statement tag=07DV}

— $V$ を標準空間 $E$ のベクトル部分空間とし、$f$ を $V$ にわたる連続的な線型形式とします。その場合、拡大する $f$ である $E$ 上に定義された連続線型形式 $h$ が存在し、同じノルム (GT, X, § 3.2) です。

コルを適用します。 1、$p(x) = \|f\| \cdot \|x\|$を計算すると、$\|h\| \leq \|f\|$が得られます。しかし明らかに$\|h\| \geq \|f\|$と系が続きます。

コルの結論。 3 は、ノルム空間から任意のノルム空間 (IV, p. 55, exerc. 16, c) および V, p. 65, exerc. への連続線形写像には必ずしも有効ではありません。 22）。

### 練習問題 {#evt-ii-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
