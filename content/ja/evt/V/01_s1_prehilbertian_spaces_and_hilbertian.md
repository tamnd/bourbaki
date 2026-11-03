---
book: evt
book_title: Topological Vector Spaces
chapter: V
chapter_title: HILBERTIAN SPACES (ELEMENTARY THEORY)
section: 1
section_title: Prehilbertian spaces and hilbertian spaces
lang: ja
source: evt-i-v
pdf_pages: 0259-0275, 0318-0328
extraction: ocr
subsections:
    - "no": 1
      title: Hermitian forms
      page: 0
      pdf_page: 259
    - "no": 2
      title: Positive hermitian forms
      page: 2
      pdf_page: 260
    - "no": 3
      title: Prehilbertian spaces
      page: 4
      pdf_page: 262
    - "no": 4
      title: Hilbertian spaces
      page: 6
      pdf_page: 264
    - "no": 5
      title: Convex subsets of a prehilbertian space
      page: 9
      pdf_page: 267
    - "no": 6
      title: Vector subspaces and orthoprojectors
      page: 12
      pdf_page: 270
    - "no": 7
      title: Dual of a hilbertian space
      page: 15
      pdf_page: 273
statements: 41
exercises: 37
content_sha256: 72cfa8f422ed49d187edb52f20f56b9e704ba41fadbc92d4af73bcfb90ee3835
translated_from: content/en/evt/V/01_s1_prehilbertian_spaces_and_hilbertian.md
translation_method: google
source_content_sha256: a3c6df7442ce70b3c022a53d8c8d5c5898d4f54434a40fd2c9ae5e5be4f6a2de
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 7db9815aa81630220883862630281963babf700b6cf14dbb18ffc73fd925f789
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 1。プレヒルバーティアン空間とヒルバーティアン空間

### 1. エルミート形

代数 (A, IX, § 3, No. 1) で与えられた次の定義を思い出します。

#### 定義 1 {#evt-v-s1-def-1 .statement tag=07X0}

E を体 K よりもベクトル空間とします。E 上のエルミート形 (左側) は、E × E から K への写像 f 満たす次の条件 (E の $x_1, x_2, x, y_1, y_2, y$ と K の $\lambda, \mu$ について):

(1)
$$
\begin{cases}
f(x_1 + x_2, y) = f(x_1, y) + f(x_2, y) \\
f(x, y_1 + y_2) = f(x, y_1) + f(x, y_2)
\end{cases}
$$

(2)
$$
\begin{cases}
f(\lambda x, y) = \overline{\lambda} f(x, y) \\
f(x, \mu y) = \mu f(x, y)
\end{cases}
$$

(3)
$$
f(x, y) = \overline{f(y, x)} .
$$

体 K が R のとき、E 簡約する上のエルミート形の概念は、E × E (A, III, § 6, No. 3) 上の対称双線形形式の双線形形式となります。

2 番目の条件 (1) と 2 番目の条件 (2) が他の 3 つから続くことに注意してください。

¹ ヒルバーティアン空間に特に興味のある読者のために、点は、§ 1 の No. 7 と § 4 の No. 8 のみが章 III と IV の結果に依存することを示します。これについては、読者は本書の最後にある「バナッハ空間のいくつかの重要な特性の概要」を参照してください。 章 I と II への唯一の言及は、凸集合と準ノルム (II、p. 1、p. 7) の定義、トポロジカル直和 (I、 p. 4)、完全な家族と位相的に独立した家族 (I、p. 12)。

(1) と (2) からすぐに次のように推測できます。

$$
f(\sum_j \lambda_j x_j, \sum_k \mu_k y_k) = \sum_{j,k} \overline{\lambda}_j \mu_k f(x_j, y_k).
$$

特に、E が有限次元で、$(e_j)_{1 \leq j \leq n}$ が E の基底である場合、$x = \sum_{j=1}^n \xi_j e_j$ と $y = \sum_{j=1}^n \eta_j e_j$ については、次のようになります。

$$
f(x, y) = \sum_{j,k} \alpha_{jk} \overline{\xi}_j \eta_k
$$

記法 $\alpha_{jk} = f(e_j, e_k)$ 付き;さらに、関係 (3) は、添字 $j, k$ の対ごとに $\alpha_{jk} = \overline{\alpha}_{kj}$ になります。これは、特に数 $\alpha_{jj}$ が現実であることを意味します。

(3) より、数 $Q(x) = f(x, x)$ はすべての $x \in E$ に対して実数です。さらに、*分極* として知られる次の公式を直ちに確立します公式

(5)
$$
4f(x, y) = \sum_{\varepsilon^2 = 1} \varepsilon Q(x + \varepsilon y) \quad \text{if } K \text{ is } \mathbf{R},
$$
(6)
$$
4f(x, y) = \sum_{\varepsilon^4 = 1, \varepsilon \in \mathbf{C}} \varepsilon Q(x + \overline{\varepsilon} y) \quad \text{if } K \text{ is } \mathbf{C}.
$$

#### 注意 {#evt-v-s1-n1-rem-1 .statement tag=07X1}

— 公式 (6) は、$E \times E$ 上のすべての *sesquilinear* 形に対して有効であることがわかります (つまり、すべての写像 $f$ 満たす (1) および (2) に対して有効ですが、必ずしも (3) であるとは限りません)。この注意は、$K = \mathbf{C}$ のとき、$f(x, x)$ がすべての $x \in E$ に対して実数であるようなセスキ線形形 $f$ は、必ず *エルミート* であることを示しています。 関係 (6) は、$y + \varepsilon x = \varepsilon(x + \overline{\varepsilon} y)$ があるので、$\overline{f(y, x)} = f(x, y)$ を与えます$\varepsilon^4 = 1$はいつでも$Q(\varepsilon z) = Q(z)$。

二極化公式から、特に、

#### 命題 1 {#evt-v-s1-prop-1 .statement tag=07X2}

*$f$ が $E$ のエルミート形、および $E$ の $M$ ベクトル部分空間で、すべての $x \in M$ が $f(x, x) = 0$ になる場合、すべての$f(x, y) = 0$ も得られます。 $M$ の点 $x, y$ の対。*

$f$ を $E$ でエルミート形とします。すべての $y \in E$ の $f(x, y) = 0$ は、$E$ のベクトル部分空間となるように、すべての $x \in E$ の $N$ が集合となります。 (3) から、$x_1 \equiv x_2$ (mod. $N$) と $y_1 \equiv y_2$ (mod. $N$) の場合、$f(x_1, y_1) = f(x_2, y_2)$ が得られます。したがって、商空間 $E/N$ では、すべての $x \in \dot{x}$ とすべての $y \in \dot{y}$ に $f(\dot{x}, \dot{y}) = f(x, y)$ を代入することで、定義するセスキリニア形 $f$ になります。 $f$ がエルミートであり、関係 «すべての $\dot{y} \in E/N$ に対して$f(\dot{x}, \dot{y}) = 0$» は、$E/N$ では$\dot{x} = 0$ を暗示し、他の語 (A, IX) $f$ は分離していることは明らかです。 $f$ はエルミート形と $f$ の *分離* であると言います。

### 2. ポジティブエルミート形

#### 定義 2 {#evt-v-s1-def-2 .statement tag=07X3}

*$E$を体$K$の上にベクトル空間とします。 $E$ のエルミート形 $f$ は、すべての $x \in E$ に対して $f(x, x) \geq 0$ であれば陽性であると言われます。*

ベクトル空間 $E$ 形ベクトル空間 *体* $\mathbf{R}$ ではエルミート形であることは明らかです (ただし、$K$ が体 $\mathbf{C}$ を超えてはなりません) $\mathbf{C}$) : この空間では、正のエルミート形は、def の結果として *尖った凸型固有円錐* (II, p. 10) を構成します。 2とプロップ。 1.

#### 命題 2 {#evt-v-s1-prop-2 .statement tag=07X4}

— *f が正のエルミート形の場合、*

$$
|f(x, y)|^2 \leq f(x, x) \ f(y, y)
$$

*E のすべての x と y に対して* (コーシー-シュワルツ不等式)。

まず、$f(y, y) \neq 0$ があると仮定します。 $\xi \in \mathbf{K}$ ごとに、

$$
f(y, y) \ f(x + \xi y, x + \xi y) \geq 0
$$

次のように書くことができます

$$
f(x, x) \ f(y, y) - |f(x, y)|^2 + (\xi f(y, y) + \overline{f(x, y)}) (\overline{\xi} f(y, y) + f(x, y)) \geq 0 .
$$

この不等式で置き換えること $\xi$ を $-\overline{f(x, y)}/f(y, y)$ で計算すると (7) が得られます。 $f(x, x) \neq 0$ の場合も同様に議論します。

最後に、$f(x, x) = f(y, y) = 0$ の場合、すべての $\xi \in \mathbf{K}$ に対して $f(x + \xi y, x + \xi y) \geq 0$ が得られ、次のように書くことができます。

$$
\xi f(x, y) + \overline{\xi} f(x, y) \geq 0 .
$$

この不等式では、置き換えること $\xi$ を $-\overline{f(x, y)}$ により、$-2 \ |f(x, y)|^2 \geq 0$ が得られるため、$f(x, y) = 0$ になります。この場合も (7) が得られます。

#### 系 1 {#evt-v-s1-prop-2-cor-1 .statement tag=07X5}

— *f が正のエルミート形の場合、f(x, x) = 0 となるような E 内のすべての x の集合 N 一致すると、E 内のすべての y について f(x, y) = 0 となるような E 内のすべての x のベクトル部分空間。*

#### 系 2 {#evt-v-s1-prop-2-cor-2 .statement tag=07X6}

— *正のエルミート形が分離するには、 関係 x \neq 0 が f(x, x) > 0 を意味することが必要かつ十分です。*

これは cor の直後に続きます。 1.

E 上のすべての正のエルミート形 f について、f (V, p. 2) に関連付けられた分離のエルミート形は、E/N 上では明らかに正のエルミート形です。

#### 命題 3 {#evt-v-s1-prop-3 .statement tag=07X7}

— *f を E の正のエルミート形とします。* を置きます

$$
p(x) = f(x, x)^{1/2}
$$

*すべての x \in E について。そのとき、p は E 上の準ノルムであり、f が分離している場合に限り、ノルムになります。*

不等式 $p(x + y) \leq p(x) + p(y)$ を証明すれば十分です。しかし、私たちは持っています

$$
f(x + y, x + y) = f(x, x) + f(y, y) + f(x, y) + \overline{f(x, y)}
$$

そして、コーシー・シュワルツ著不等式

$$
f(x + y, x + y) \leq f(x, x) + f(y, y) + 2(f(x, x) f(y, y))^{1/2}
$$
$$
= (f(x, x)^{1/2} + f(y, y)^{1/2})^2 .
$$

#### 注意 {#evt-v-s1-n2-rem-1 .statement tag=07X8}

— 1) f が正で分離していると仮定し、x、y を 2 ベクトル $\neq 0$ とします。 Cauchy-Schwarz の証明不等式は、(7) の 2 つの要素が等しい場合、$f(x + \xi y, x + \xi y) = 0$、したがって $x + \xi y = 0$ となるようなスカラー $\xi$ が存在し、他の語、$x$、$y$ は *線形依存* であることを示しています。 逆は明らかです。 不等式 (8) の証明は、$x$ と $y$ が線形従属である場合にのみ、等式 $p(x + y) = p(x) + p(y)$ が可能であることを示しています。 $y = \lambda x$ の場合、その前の等式は $|1 + \lambda| = 1 + |\lambda|$ と書くことができ、$\lambda$ が *実数で正* であることを意味します。

2) $f$ を $E$ の正のエルミート形式とし、$E$ に半ノルム $x \mapsto f(x, x)^{1/2}$ を割り当てます。 $f$ が、$f$ に関連付けられた $E/N$ で定義された正の分離エルミート形式である場合、ノルム $x \mapsto f(\dot{x}, \dot{x})^{1/2}$ を $E/N$ に割り当てることで得られる正規化空間は、$E$ (II, p. 5) に関連付けられた正規化空間になります。

#### 定義 3 {#evt-v-s1-def-3 .statement tag=07X9}

*$E$を体$K$の上にベクトル空間とします。 $E$ の準ノルム $p$ は、すべての $x \in E$* に対して $p(x) = f(x, x)^{1/2}$ となるような、$E$ に正のエルミート形 $f$ が存在する場合、プレヒルバーティアンであると言われます。

$E$ の準ノルム $p$ に対して、すべての $x \in E$ に対して $p(x) = f(x, x)^{1/2}$ となるような正のエルミート形 $f$ が最大 1 つ存在することに注目してください。これは、分極公式 (V、p. 2) から導き出されます。

### 3. プレヒルバーティアン空間

#### 定義 4 {#evt-v-s1-def-4 .statement tag=07XA}

*プレヒルバーティアン空間は、$K$ を超えるベクトル空間の構造と、正のエルミート形を伴う集合 $E$ です。 $K$ が $\mathbf{R}$ (それぞれ $K$ が $\mathbf{C}$) であるとき、$E$ は実数 (複素数) プレヒルバーティアン空間であると言います。

#### 例 1 {#evt-v-s1-n3-exa-1 .statement tag=07XB}

形 $(\lambda, \mu) \mapsto \overline{\lambda} \mu$ 定義する $K$ のプレヒルバーティアン構造は *標準* と言われています。 $K$ がプレヒルバーティアン空間とみなされる場合、常に 〜でない限りを意味します。そうでない場合は、この構造があることを示します。

#### 例 2 {#evt-v-s1-n3-exa-2 .statement tag=07XC}

$I$ を $\mathbf{R}$ の区間 (有界かどうか)、$E$ を $\mathbf{C}$ の値で $I$ に定義された規制対象写像 (FVR、II、p. 4) の集合とします。コンパクトなサポート。 $E$ が $\mathbf{C}$ よりもベクトル空間であることは明らかです。 $f$ をセスキ線形形 $(x, y) \mapsto \int_1^1 \overline{x(t)}\ y(t)\ dt$ とします。 $f$ が $E$ で正のエルミート形であるのは明らかであり、したがって定義するはこの空間でプレヒルバーティアン構造です。

#### 例 3 {#evt-v-s1-n3-exa-3 .statement tag=07XD}

$n \geqslant 0$を整数とします。私たちは、エルミート形によって、空間 $K^n$ にプレヒルバーティアン定義する空間構造です

$$
(x, y) \mapsto \sum_{j=1}^n \overline{x_j} y_j
$$

($x = (x_1, ..., x_n)$ と $y = (y_1, ..., y_n)$ の場合)。 $K$ が $\mathbf{R}$ の場合、これは 2 つのベクトルの $\mathbf{R}^n$ (GT、VI, § 2, No. 2) のスカラー 積であることがわかります。

#### 例 4 {#evt-v-s1-n3-exa-4 .statement tag=07XE}

$\ell^2$ (または $\ell^2(\mathbf{N})$) を数列の集合 、元の $K$ の $x = (x_n)_{n \in \mathbf{N}}$ とし、$\sum_{n=0}^\infty |x_n|^2$ を有限とします。 エルミート形 $(x, y) \mapsto \sum_{n=0}^\infty \overline{x_n} y_n$ により、$\ell^2$ は $K^\mathbf{N}$ のベクトル部分空間であり、定義するは $\ell^2$ のプレヒルバーティアン空間構造であることがわかります。 (cf. V、p. 18)。

#### 例 5 {#evt-v-s1-n3-exa-5 .statement tag=07XF}

$E$ を、$E$ 上の実際のプレヒルバーティアン空間、$f$ 対応する対称双線形形式とします。 $E_{(c)}$ を $E$ のベクトル空間複素数とします。 写像 $x \mapsto 1 \otimes x$ によって、同一視する $E$ と $E_{(c)}$ の部分集合が、$E_{(c)}$ のすべての元が $E$ の $x_1, x_2$ を持つ $x_1 + ix_2$ として一意に書くことができます。 写像 $f$ 拡大するは $E_{(c)}$ のエルミート形 $f_{(c)}$ に固有。我々は持っています、

$$
f_{(c)}(x_1 + ix_2, y_1 + iy_2) = f(x_1, y_1) + f(x_2, y_2) + i(f(x_1, y_2) - f(x_2, y_1)) .
$$

特に、私たちは、
$$
f_{(\mathbf{C})}(x_1 + ix_2, x_1 + ix_2) = f(x_1, x_1) + f(x_2, x_2) \geqslant 0,
$$
従って、$f_{(\mathbf{C})}$ は正です。 $E_{(\mathbf{C})}$ と $f_{(\mathbf{C})}$ は、$E$ の *プレヒルバーティアン空間複雑化* であると言います。

ベクトル空間 $E$ のプレヒルバーティアン空間構造が 1 つだけ検討されている場合、値、対 $(x, y)$、点、$E$、エルミート形定義する当該構造は、混乱が生じない限り、$\langle x|y \rangle_E$ または単に $\langle x|y \rangle$ で表されます。 この数は、$x$と$y$の*スカラー積* $^1$ ($y = x$の場合、$x$の*スカラー平方*)と呼ばれます。 2 つのベクトル $x, y$ は、$\langle x|y \rangle = 0$ の場合 *直交* であると言われます。 写像 $x \mapsto \|x\| = \langle x|x \rangle^{1/2}$ は、ベクトル空間 $E$ (V、p. 3) の *準標準* です。プレヒルバーティアン空間は、常にこの準ノルムが割り当てられて考慮されます (従って、対応する位相および均一構造も考慮されます)。

これらの記法を使用して、プレヒルバート空間 $E$ で、コーシー-シュワルツ不等式は次のように書くことができます。
$$
|\langle x|y \rangle| \leqslant \|x\| \cdot \|y\|.
$$

その結果、スカラー 積は、$E \times E$ 上の *連続セスキ線形形* になります (II, p. 5、提案 4)。

$E$ がハウスドルフである位数では、$x \mapsto \|x\|$ が $E$ 上の *ノルム* であることが必要かつ十分です。他の語では、エルミート形 $(x, y) \mapsto \langle x|y \rangle$ *ポジティブで分離*。これは、*$0$ が $E$ の唯一のベクトルであり、それ自体に直交するというに相当します*。

一般的な定義 (S, IV, § 1, No. 5) によれば、プレヒルバーティアン空間 $E$ からプレヒルバーティアン空間 $F$ への同型は、$E$ からの全単射線形写像 $u$ です。 $F$そのような
$$
\langle u(x)|u(y) \rangle = \langle x|y \rangle
$$
$E$ のすべての $x$ と $y$ に対して。これから、すべての $x \in E$ に対して $\|u(x)\| = \|x\|$ が推定され、$u$ は、$E$ と $F$ のトポロジカルベクトル空間構造に対して明らかに同型であると推測されます。 $E$ と $F$ がハウスドルフである場合、$u$ は $E$ から $F$ への *アイソメトリ* です。逆に、$u$ が $E$ から $F$ への全単射線形写像であり、すべての $x \in E$ に対して $\|u(x)\| = \|x\|$ である場合、分極公式 (V, p. 2) は、$u$ がプレヒルバーティアン空間同型 $E$ から $F$ まで。

$E$ を *複素* プレヒルバーティアン空間とし、$\langle x|y \rangle$ を $E$ のスカラー 積とします。 集合 $E$ では、加法群の法則と外部合成 $(\lambda, x) \mapsto \overline{\lambda} x$ の法則を同じにして、$\mathbf{C}$ に関して 2 番目の定義するベクトル空間構造ができます (A, II, § 1, No. 13) このベクトル空間構造では、$(x, y) \mapsto \langle y|x \rangle$ は *正のエルミート*

1 $\langle y|x \rangle$ に対して $(x|y)$ と書くことがときどき起こるかもしれません。 V、p. 2 の公式 (4) が次の同等の形を取ることに注目してください。
$$
\begin{align*}
\langle \sum_i \lambda_i x_i | \sum_j \mu_j y_j \rangle &= \sum_{i,j} \overline{\lambda}_i \mu_j \langle x_i|y_j \rangle. \\
(\sum_i \lambda_i x_i | \sum_j \mu_j y_j) &= \sum_{i,j} \lambda_i \overline{\mu}_j (x_i|y_j).
\end{align*}
$$

形。この新しいベクトル空間構造と新しいエルミート形を E に代入することで得られるプレヒルバーティアン空間 $\overline{E}$ は、E に共役と言われます。 E から $\overline{E}$ への同型 $u$ は、 E からそれ自体への半線形マッピング ($\mathbf{C}$ の自己同型 $\xi \mapsto \overline{\xi}$ に関して) $\langle u(y)|u(x) \rangle = \langle x|y \rangle$ または $\langle u(x)|u(y) \rangle = \overline{\langle x|y \rangle}$ (E の $x, y$ の場合)。このような写像は、プレヒルバート型空間 E の半自己同型であると言われています。

E がプレヒルバーティアン空間の場合、E の M ベクトル部分空間、スカラー 積 $\langle x|y \rangle$ から $M \times M$ の制限は M 上の正のエルミート形であり、それは定義するプレヒルバーティアンになります。 M では空間構造;この構造は E の構造によって誘発される、または M は E の前ヒルバーティアン部分空間であると言います。

### 4. ヒルバーティアン空間

#### 定義 5 {#evt-v-s1-def-5 .statement tag=07XG}

*ヒルベルト空間* (または *ヒルベルト空間*) *はハウスドルフで完全なプレヒルベルト空間です*。 *ベクトル空間 E (K 以上) 上のノルムがプレヒルバーティアンであり、正規化された空間 E が完全である場合、ヒルバーティアンであると言います*。

E がヒルバーティアン空間で、M が E の閉じたベクトル部分空間である場合、M に誘発されるプレヒルバーティアン空間構造は実際にはヒルバーティアン空間構造です。この場合、誘導された構造を持つ M は E の *ヒルベルト部分空間* であると言います。

#### 例 1 {#evt-v-s1-n4-exa-1 .statement tag=07XH}

V、p. 4 の例 1、3、4 で定義されたプレヒルバーティアン空間は、ヒルバーティアン空間です。一方、例 2 で定義されるプレヒルバーティアン空間はハウスドルフでも完全でもありません。ヒルバーティアン空間の *複雑化* は、ヒルバーティアン空間です。

#### 例 2 {#evt-v-s1-n4-exa-2 .statement tag=07XI}

\* X をハウスドルフ トポロジカル空間とし、$\mu$ を X の正の尺度とします。 $L^2(X, \mu)$ を、$\mathbf{C}$ の値を含む、X 上のすべての平方 $\mu$ 可積分関数の $\mu$ に対して、同値類の空間からなるとします。 これは複素ヒルバーシアン空間で、そのスカラー 積は次の式で与えられます。

$$
\langle f|g \rangle = \int_X \overline{f(x)}\ g(x)\ d\mu(x) .
$$

#### 例 3 {#evt-v-s1-n4-exa-3 .statement tag=07XJ}

\* $n \geqslant 1$ を整数とし、U を $\mathbf{R}^n$ のオープン集合とします。 $\mathbf{R}^n$ のルベーグ測度によって導かれる U の測度を $\mu$ とし、$\mathscr{H}^0 = L^2(U, \mu)$ を置きます。 $\mathscr{H}^1$ は、すべての写像 $f \in \mathscr{H}^0$ のうちの空間を次の性質で表すものとします。 $1 \leqslant i \leqslant n$ の場合、次のような写像 $g_i \in \mathscr{H}^\circ$ が存在します。

$$
\int_U g_i(x)\ h(x)\ d\mu(x) = - \int_U f(x)\ D_i h(x)\ d\mu(x)
$$

U でコンパクトにサポートされた、類 $C^1$ のすべての写像 $h$ に対して。 写像 $g_i$ は、$\mu$ に関して同値まで一意に定義され、$D_i f$ または $\partial f / \partial x_i$ で示されます。 (i 番目の偏導関数)。 整数 $s \geqslant 1$ の帰納法までに、定義する $\mathscr{H}^s$ をすべての写像 $f \in \mathscr{H}^1$ の集合として、$D_i f \in \mathscr{H}^{s-1}$ を$1 \leqslant i \leqslant n$ とします。私たちは公式により $\mathscr{H}^s$ にスカラー 積定義するを計算します。

$$
\langle f|g \rangle = \sum_{k=0}^s \sum_{1 \leqslant i_1 \leqslant \ldots \leqslant i_k \leqslant n} \int \overline{D_{i_1} \ldots D_{i_k} f} \cdot D_{i_1} \ldots D_{i_k} g\ d\mu .
$$

次に、$\mathscr{H}^s$ は、添字 s の *Sobolev 空間* と呼ばれる複素ヒルベルト空間です。

#### 例 4 {#evt-v-s1-n4-exa-4 .statement tag=07XK}

\* X を、有限次元 $n$ の純粋な類 $C^r$ ($r \geqslant 1$ を含む) の差分多様体とします。

ベクトルファイバー 空間 $\Lambda^n T(X)$ では、L を零切断の補数とします。 $\Lambda^n T(X)$ から実数 $\lambda \neq 0$、写像 $u \mapsto \lambda u$ ごとに、L が安定します。

$\alpha$を複素数とします。 $u \in L$ の $\omega(\lambda u) = |\lambda|^{\alpha} \omega(u)$ とゼロ以外の実数 $\lambda$ が L で写像 $\omega$ と評価される複素数は、位数 $\alpha$ の稠密度と呼ばれます。 X。 X の開いたカバー $(U_i)_{i \in I}$ が存在し、$U_i$ 上の座標 $\xi_i = (\xi_i^1, ..., \xi_i^n)$ のすべての $i \in I$ 系と複素数値が存在する場合、位数 1 の稠密度 $\omega$ は局所的に積分可能であると言います。 写像 $f_i$ $\xi_i(U_i)$ 満たす次の条件:

a) 写像 $f_i$ は、ルベーグ測度 $\mu$ に関して $\mathbf{R}^n$ のオープン集合 $\xi_i(U_i)$ で局所的に積分可能です。

b) $x \in U_i$ とします。 $(\partial_{1,i,x}, ..., \partial_{n,i,x})$ が $U_i$ の座標 $(\xi_i', ..., \xi_i^n)$ の系に関連付けられた $T_x X$ の基底である場合、次のようになります。
$$
\omega(\partial_{1,i,x} \wedge ... \wedge \partial_{n,i,x}) = f_i(\xi_i^1(x), ..., \xi_i^n(x)) .
$$

次に、X には 1 つだけの小節 $\tilde{\omega}$ が存在し、すべての $i \in I$ について、$\tilde{\omega}$ から $U_i$ の制限の $\xi_i$ の下の像が小節 $f_i \cdot \mu$ (cf.) に等しくなります。 VAR、R、10.4.3)。

$\mathscr{V}$ (それぞれ $\mathscr{N}$) を次数 1/2 の測定可能な密度 $\omega$ のベクトル空間とし、次数 1 の密度 $|\omega|^2$ に関連付けられた測度が有界である (それぞれ null) とします。 $\omega_1$ と $\omega_2$ を $\mathscr{V}$ に入れます。この場合、$\omega = \overline{\omega_1} \omega_2$ は位数 1 の稠密度であり、$\omega$ に関連付けられたメジャー $\tilde{\omega}$ は有界です。 数 $\int_X \tilde{\omega}$ は、$\omega_1$ の類 $\dot{\omega}_1$ と $\dot{\omega}_2$ および $\mathscr{N}$ を法とする$\omega_2$ にのみ依存し、$\langle \omega_1 | \omega_2 \rangle$ または $\langle \dot{\omega}_1 | \dot{\omega}_2 \rangle$ で表されます。 次に、写像 $(\dot{\omega}_1, \dot{\omega}_2) \mapsto \langle \dot{\omega}_1 | \dot{\omega}_2 \rangle$ は複素ヒルバーシアン空間構造をベクトル空間 $\Omega_{1/2}(X) = \mathscr{V}/\mathscr{N}$ に代入します。

#### 例 5 {#evt-v-s1-n4-exa-5 .statement tag=07XL}

\* D を、$\mathbf{C}$ で中心 0、半径 1 の開いた円盤とします。 *Hardy 空間* $H^2(D)$ は、すべての正則写像 $f : D \to \mathbf{C}$ で構成されます。
$$
\sup_{0 < R < 1} \int_0^1 |f(R \cdot e(\theta))|^2 d\theta < + \infty .
$$
$f_1$ と $f_2$ 属するから $H^2(D)$ の場合、極限
$$
\langle f_1 | f_2 \rangle = \lim_{R \to 1} \int_0^1 \overline{f_1(R \cdot e(\theta))} \cdot f_2(R \cdot e(\theta)) \, d\theta
$$
存在します。 写像 $(f_1, f_2) \mapsto \langle f_1 | f_2 \rangle$ は、複素ヒルバーシアン空間構造をベクトル空間 $H^2(D)$ に代入します。

写像 $f : D \to \mathbf{C}$ から属する $H^2(D)$ については、$\sum_{n=0}^\infty |a_n|^2 < + \infty$ となるような複素数の数列 $(a_n)_{n \in \mathbf{N}}$ が存在することが必要かつ十分です。
$$
f(z) = \sum_{n=0}^\infty a_n z^n
$$
すべての$z \in D$に。次に、$\|f\|^2 = \sum_{n=0}^\infty |a_n|^2$ があり、これは $H^2(D)$ から同型をヒルバート空間 $\ell^2$ (V, p. 4) に与えます。

すべてのハウスドルフ プレヒルバーティアン空間は、同型まで決定されたヒルバーティアン空間のどこでも密な部分空間と同型です。正確に ：

#### 命題 4 {#evt-v-s1-prop-4 .statement tag=07XM}

— *E を、E*(GT, IX, § 3, No. 3) の標準的な空間完成であるハウスドルフ プレヒルベルト空間, $\hat{E}$ とする。スカラー 積* $(x, y) \mapsto \langle x|y \rangle$ *拡大するは正に連続し、* $\hat{E}$ ではエルミート形、* $\hat{E}$ では定義するヒルバーシアン空間構造です。

$(x, y) \mapsto \langle x|y \rangle$ から $\hat{E} \times \hat{E}$ までの拡大の存在は、このセスキ線形形と $E \times E$ (GT, III, § 6, No. 5, th. 1) の連続性から生じます。さらに、この拡大 (これも $(x, y) \mapsto \langle x|y \rangle$ で示されます) は、エルミート形であり、拡大の恒等原理により、関係 $\langle x|x \rangle = \|x\|^2$ を満たします ($\|x\|$ は $\hat{E}$ ではノルムです)。 E 上のノルムを連続性によって拡張することで得られます) ;これは、関係 $\langle x|x \rangle = 0$ が $\hat{E}$ の $x = 0$ を暗示しているため、形 $(x, y) \mapsto \langle x|y \rangle$ が正で分離しており、その結果、定義するが空間構造のヒルバーティアンであることを証明します。 $\hat{E}$。 Q.E.D.

このヒルバーティアン空間は、ハウスドルフプレヒルバーティアン空間 E の *完成* であると言われています。

\* *例 6*。 — U を $\mathbf{R}^n$ ($n \geqslant 1$) のオープン部分集合とします。 $\mathscr{C}_0^1(\mathrm{U})$ を、U でのコンパクトなサポートを持つ類 $\mathrm{C}^1$ のすべての写像のベクトル空間とします。定義するは、$\mathscr{C}_0^1(\mathrm{U})$ 上のハウスドルフプレヒルバーティアン空間構造で、そのスカラー 積は次の式で与えられます。

$$
\langle f|g \rangle = \sum_{i=1}^{n} \int_{\mathrm{U}} \overline{\mathrm{D}_i f(x)} . \mathrm{D}_i g(x) \, dx .
$$

このプレヒルバーティアン空間は完全ではありません。その完成は、U に関連付けられた *ディリクレ空間* と呼ばれます。 \*

#### 系 {#evt-v-s1-n4-cor-1 .statement tag=07XN}

— *V を K に対してベクトル空間とし、f を V で正のエルミート形とします。*
a) *ヒルベルト空間 E と線形写像* $u : V \to E$ *そのような* $f(x, y) = \langle u(x)|u(y) \rangle$ *x、V の y について、そして u(V) が E で密であるような* が存在します。
b) *a) と同様に 2 つの対* $(E_i, u_i)$ *満たす条件がある場合、一意の同型* $\phi$ *ヒルベルト空間* $E_1$ *ヒルベルト空間* が存在します。 $E_2$ *そのような* $u_2 = \phi \circ u_1$。

N を、$f(x, x) = 0$ となるようなすべての $x \in V$ の集合とします。 定義するはポジティブで、空間 V/N のエルミート形を $x \in \dot{x}$ と $y \in \dot{y}$ に対して $\langle \dot{x}|\dot{y} \rangle = f(x, y)$ だけ分離します。 E を、V から E へのV/N および$u$ 写像 $x \mapsto x + N$ のヒルベルト空間完成とします。そのとき、*a*) の条件が​​満たされます。

*b*) の仮説の下では、N は $u_1$ の核と $u_2$ に等しい。したがって、$u_1(V)$ から $u_2(V)$ までの全単射線形写像 $\phi_0$ が存在し、すべての $x \in V$ に対して $u_2(x) = \phi_0(u_1(x))$ になります。 $\phi_0$ がプレヒルバーティアン空間の同型であること、つまりアイソメトリであることをすぐに検証します。 $u_i(V)$ は $i = 1, 2$ に対して $E_i$ で密であるため、$E_1$ から $E_2$ へのアイソメトリ $\phi$ に特有の $\phi_0$ 拡大するが続き、*b*) が続きます。

ヒルバート空間 E は V (形 *f* の場合) の *分離完了* であると言います。

#### 例 7 {#evt-v-s1-n4-exa-7 .statement tag=07XO}

G を群 (単位元 1 を伴う) とし、G から複素ヒルベルト空間 E の自己同型の群に $\pi$ 準同型を代入します。 $\pi$ は E の G の *unitary 表現* であると言います。 $a \in E$ としましょう。私たちは置きます

$$
\phi(x) = \langle a|\pi(x).a \rangle
$$

$x \in G$ 全員のために。この場合、 $\phi : G \to \mathbf{C}$ は *正定値 * であり、他の語は関係を満たします。

(PD) $\mathbf{C}$ の $\lambda_1, ..., \lambda_n$ と $G$ の $x_1, ..., x_n$ ごとに、

$$
\sum_{i,j=1}^n \overline{\lambda_i} \lambda_j \phi(x_i^{-1} x_j) \geqslant 0 .
$$

実際、(11) の最初のメンバーは正確に $\| \sum_{i=1}^n \lambda_i \pi(x_i) . a \| ^2$ です。

逆に、$\phi$ を $G$ 上の正定値写像とします。 $C^{(G)}$ をすべての写像のベクトル空間とし、$G$ に有限台を加えます。私たちは定義するエルミート形 $\Phi$ により $G$

$$
\Phi(u, v) = \sum_{x,y \in G} \overline{u(x)} \ v(y) \ \phi(x^{-1} y)
$$

関係 (PD) は、$\Phi$ が正であることを表します。プロップの系による。 4 では、ヒルバーティアン空間 $E$ と線形写像 $\rho : C^{(G)} \to E$ が存在し、次のような密な像が存在します。

$$
\Phi(u, v) = \langle \rho(u)|\rho(v) \rangle \quad \text{for} \quad u, v \quad \text{in} \quad C^{(G)} .
$$

すべての $x \in G$ について、$u \in C^{(G)}$ と $y \in G$ の $\gamma_x u(y) = u(x^{-1} y)$ によって定義される $C^{(G)}$ の $x$ による左の翻訳を $\gamma_x$ とします。 $\Phi(\gamma_x u, \gamma_x v) = \Phi(u, v)$があります。次に、支柱の系の主張 b)を適用します。 4 から $\rho$ および $\rho \circ \gamma_x$: $\rho \circ \gamma_x = \pi(x) \circ \rho$ となるようなヒルバーシアン空間 $E$ の一意の自己同型 $\pi(x)$ が存在します。 $\pi$ は $G$ から $E$ の自己同型の群になる準同型であることがすぐにわかります。

$\delta$ を、$G$ の $x \neq 1$ に対して $\delta(1) = 1, \delta(x) = 0$ によって定義された $C^{(G)}$ の元とします。すべての $u \in C^{(G)}$ に対して $u = \sum_{x \in G} u(x) . \gamma_x \delta$ があるので、$a = \rho(\delta)$ を入れると $\rho(u) = \sum_{x \in G} u(x) \ \pi(x) . a$ になります。

公式 (12) と (13) は、すべての $x \in G$ に対して $\phi(x) = \langle a|\pi(x).a \rangle$ を意味します。すべての $x \in G$ のベクトル $\pi(x).a$ の集合が $E$ の合計であることに注目します。

### 5. プレヒルバーティアン空間の凸部分集合

プレヒルバーティアン空間 $E$ の任意の 2 つの点 $x, y$ に対して計算する $\| x - y \| ^2 = \langle x - y|x - y \rangle$ と $\| x + y \| ^2 = \langle x + y|x + y \rangle$ を実行すると、直ちに「中央値の同一性」が得られます。

$$
\| \frac{1}{2}(x + y) \| ^2 + \| \frac{1}{2}(x - y) \| ^2 = \frac{1}{2} (\| x \| ^2 + \| y \| ^2 ) .
$$

このアイデンティティから、次のことが推測されます命題 :

![図式は集合 B'、B、A を表示しており、A 内に x と y がマークされています](https://i.imgur.com/3Q5z5QG.png)

図1

#### 命題 5 {#evt-v-s1-prop-5 .statement tag=07XP}

— $E$ をプレヒルバーティアン空間とします。 $d$ を実数 $> 0$、$\delta$ 実数として、$0 \leqslant \delta \leqslant d$ とします。 $B$ と $B'$ を $\| x \| < d$ で定義される $E$ の部分集合とします。

$$
\|x\| \leq d + \delta \text{ respectively, and let } A \text{ be a convex set contained in } B' - B. \text{ Then for every pair of points } x, y \text{ of } A, \text{ we have } \|x - y\| \leq \sqrt{12d\delta} \text{ (fig. 1).}
$$
実際には $\frac{1}{2}(x + y) \in A$ があるため、$\left\| \frac{1}{2}(x + y) \right\| \geq d$ になります。したがって、(14) から不等式が得られます。
$$
\left\| \frac{1}{2}(x - y) \right\|^2 = \frac{1}{2}(\|x\|^2 + \|y\|^2) - \left\| \frac{1}{2}(x + y) \right\|^2 \leq (d + \delta)^2 - d^2 \leq 3d\delta
$$
そこから命題が続きます。

#### 定理 1 {#evt-v-s1-thm-1 .statement tag=07XQ}

*E をプレヒルバーティアン空間とし、H を E の空でない凸型部分集合とし、H がハウスドルフであり E の完全な均一部分空間となるようにします。すべての $x \in E$ に対して、$\|x - p_H(x)\| = \inf_{y \in H} \|x - y\|$ となるような H に固有の点 $p_H(x)$ が存在します。 H の元 $p_H(x)$ は、H の一意元満たす関係* でもあります
$$
\Re \langle x - a | y - a \rangle \leq 0
$$
*全員に* $y \in H$。

![図式は、点 x、点 y、および a + λ(y − a) とラベル付けされた線分を示しています](https://i.imgur.com/3Q5z5QG.png)

図2

$d = \inf_{y \in H} \|x - y\|$ を置き、整数 $n > 0$ ごとに、$H_n$ を $\|x - y\| \leq d + n^{-1}$ となるような H の点 $y$ の集合とします。 集合 $H_n$ は H で閉じており、凸状で空ではありません。その直径は、支柱によって十分に大きいすべての $n$ に対して $\sqrt{12 \frac{d}{n}}$ によって制限されます。 5. 数列 $(H_n)_{n \geq 1}$ は減少する、集合 H はハウスドルフであり、これを完了すると、コーシー フィルター $(H_n)_{n \geq 1}$ の基底は H の点 $p_H(x)$ に収束します。 $\{ p_H(x) \} = \bigcap_{n \geq 1} H_n$ があるため、$p_H(x)$ は $\|x - a\| = d$ となる H の一意の点 $a$ です。

1 (GT, VIII, § 1, No. 1) $\Re(z)$ が複素数 z の実数部分を表すことを思い出してください。 z が実数の場合、$\Re(z) = z$ になります。

$y \in \mathbf{H}$ にしましょう。 $\mathbf{H}$ は凸であるため、E の点 $z(\lambda) = p_{\mathbf{H}}(x) + \lambda(y - p_{\mathbf{H}}(x))$ は、$0 < \lambda < 1$ となるすべての実数 $\lambda$ に対して $\mathbf{H}$ に属します。 したがって、
$$
\| x - z(\lambda) \|^{2} \geq \| x - p_{\mathbf{H}}(x) \|^{2} \quad \text{for} \quad 0 < \lambda < 1 ,
$$
それは与える
$$
\mathscr{R} \langle x - p_{\mathbf{H}}(x)|y - p_{\mathbf{H}}(x) \rangle = \lim_{\lambda \to 0} \frac{1}{2\lambda} \left\{ \| x - p_{\mathbf{H}}(x) \|^{2} - \| x - z(\lambda) \|^{2} \right\} \leq 0 .
$$
逆に、$a$ を $\mathbf{H}$ の点とし、すべての $y \in \mathbf{H}$ に対して $\mathscr{R} \langle x - a|y - a \rangle \leq 0$ とします。 $y \in \mathbf{H}$ ごとに、
$$
\| x - y \|^{2} = \| x - a \|^{2} + \| y - a \|^{2} - 2 \mathscr{R} \langle x - a|y - a \rangle \geq \| x - a \|^{2} ,
$$
そして、$\| x - a \| = d$、そして最後に$a = p_{\mathbf{H}}(x)$が証明の最初の部分に続きます。 Q.E.D.

以下では、$\mathbf{H}$ の E の写像 $p_{\mathbf{H}}$ を、E から $\mathbf{H}$ までの *射影* と呼びます。すべての $x \in \mathbf{H}$ に対して $p_{\mathbf{H}}(x) = x$ が当てはまります。

の最初の部分 。 1 は、空間 E に関するより一般的な仮説のもとで有効です (V、p. 67、演習 31)。

証明日。 1 は、特に次のことを確立します性質 :

#### 系 1 {#evt-v-s1-thm-1-cor-1 .statement tag=07XR}

*I をフィルター $\mathfrak{F}$ によって指示された集合とし、$(y_{i})_{i \in I}$ を $\mathbf{H}$ の点のファミリーとします。 $x \in \mathbf{E}$ にしましょう。 * があると仮定します。
$$
\lim_{i, \mathfrak{F}} \| x - y_{i} \| = \inf_{z \in \mathbf{H}} \| x - z \| .
$$
*その後、$y_{i}$はフィルター$\mathfrak{F}$に対して$p_{\mathbf{H}}(x)$になる傾向があります。*

#### 系 2 {#evt-v-s1-thm-1-cor-2 .statement tag=07XS}

*$\mathbf{E}$ のすべての $x, y$ について、*
$$
\| p_{\mathbf{H}}(x) - p_{\mathbf{H}}(y) \| \leq \| x - y \| .
$$
*特に、$\mathbf{E}$から$\mathbf{H}$までの写像$p_{\mathbf{H}}$は連続です。

$x, y$を$\mathbf{E}$の2つの点とします。 $a = p_{\mathbf{H}}(x) - x, b = p_{\mathbf{H}}(y) - p_{\mathbf{H}}(x), c = y - p_{\mathbf{H}}(y)$を入れます。 公式 (15) (V、p. 10) までに、$\mathscr{R} \langle a|b \rangle \geq 0$ と $\mathscr{R} \langle c|b \rangle \geq 0$ ができます。 $a + b + c = y - x$ もあります。これにより、
$$
\| x - y \|^{2} = \| a + b + c \|^{2} = \| b \|^{2} + \| a + c \|^{2} + 2 \mathscr{R} \langle a|b \rangle + 2 \mathscr{R} \langle c|b \rangle
$$
$$
\geq \| b \|^{2} = \| p_{\mathbf{H}}(x) - p_{\mathbf{H}}(y) \|^{2} .
$$
これは系 2 を証明します。

#### 命題 6 {#evt-v-s1-prop-6 .statement tag=07XT}

*$\mathbf{E}$ をプレヒルバーティアン空間とし、$\Phi$ を空ではない、空でないハウスドルフの有向減少する集合と $\mathbf{E}$ の完全凸部分集合とします。 $\mathbf{E}$ のすべての $x \in \mathbf{E}$ とすべての部分集合 $\mathbf{H}$ に、$d(x, \mathbf{H}) = \inf_{z \in \mathbf{H}} \| x - z \|$ を入れます。 集合 H 所属から $\Phi$ の共通部分 M が空でないという位数では、$\sup_{H \in \Phi} d(x_0, H)$ が有限であるような E に $x_0$ が存在することが必要十分です。 $x \in E$ ごとに、
$$
p_M(x) = \lim_{H \in \Phi} p_H(x)
$$
(有向集合 $\Phi$ に対して極限)。

M が空でない場合、すべての $H \in \Phi$ とすべての $x \in E$ に対して $d(x, H) \leq d(x, M)$ になります。

逆に、E に点 $x_0$ が存在し、すべての $H \in \Phi$ に対して $d(x_0, H) \leq C$ となるような実数 $C \geq 0$ が存在するとします。 $x \in E$ にしましょう。それから
$$
d(x, H) \leq \|x - x_0\| + C \quad \text{for all } H \in \Phi,
$$
従って、数 $d = \sup_{H \in \Phi} d(x, H)$ は有限です。 B をすべての $z \in E$ のうち集合とし、$\|x - z\| \leq d$ とします。 B は E において凸で閉じているため、$\Phi$ を超える H に対して、集合 $H \cap B$ は凸、ハウスドルフ、完全です。 $\varepsilon > 0$ にしましょう。 $d(x, H) \geq d - \varepsilon$ となるような集合 $H \in \Phi$ が存在し、$\varepsilon < d/2$ の場合、$H \cap B$ の直径は支柱によって $\sqrt{12 \varepsilon (d - \varepsilon)}$ によって制限されます。 5 (V、p. 9)。他の語では、すべての $H_0 \in \Phi$ に対して、閉じた集合 $H \cap B$、$H \in \Phi$ と $H \subset H_0$ に対して、ハウスドルフのコーシーフィルターの形基底と完全な空間 $H_0$。従って、集合 $H \cap B$ の共通部分 ($H \in \Phi$ の場合) 簡約するから点 y になります。 $y \in M$ と $\|x - y\| = d = d(x, M)$ が得られます。 M は $H_0$ で閉じているため、E で凸かつ完全なハウスドルフ集合となり、従って $y = p_M(x)$ になります。すべての $H \in \Phi$ に対して、$p_H(x) \in H \cap B$ があり、そこから $p_M(x) = \lim_{H \in \Phi} p_H(x)$ が得られます。

#### 命題 7 {#evt-v-s1-prop-7 .statement tag=07XU}

*E をハウスドルフ プレヒルベルト空間とし、$\Psi$ を E の非空、凸、完全な部分集合の空でない有向増加する集合とする。 $A = \bigcup_{H \in \Psi} H$ を置き、A の閉包 N が完全であると仮定する。すると N は凸であり、*
$$
p_N(x) = \lim_{H \in \Psi} p_H(x) \text{ for all } x \in E.
$$

A が凸であることは明らかであり、したがってその閉包 N は凸です (II, p. 13)。 記法の小道具付き。 6、$d(x, N) = \inf_{H \in \Psi} d(x, H)$、従って、$d(x, N)$は、$\Psi$の切断フィルターに関して、$d(x, H)$の極限になります。 $p_H(x) \in H$以降、
$$
\lim_{H \in \Psi} \|x - p_H(x)\| = \lim_{H \in \Psi} d(x, H) = d(x, N),
$$
それはcorから続きます。 $p_H(x)$のV、p. 11の1は、$\Psi$の切断フィルターに対して、$x$の$p_N(x)$がNに射影になる傾向があります。

### 6. ベクトル部分空間とオルソプロジェクター

E をプレヒルバーティアン空間とします。 E の 2 つのベクトル $x$ と $y$ は、$\langle x | y \rangle = 0$ の場合 *直交* であると言われることを思い出してください。それから
$$
\|x + y\|^2 = \|x\|^2 + \|y\|^2
$$
(« ピタゴラスの定理 »)

A を E の部分集合とします。E のベクトル x が A のすべてのベクトルに直交する場合、E のベクトル x は A に直交すると言います。A に直交するすべてのベクトルのうち集合は、$A^\circ$ で示される A の閉じたベクトル部分空間であり、 (言葉の乱用により) A の直交と呼ばれます。

A と B を E の 2 つの部分集合とします。A のすべてのベクトルが B のすべてのベクトルに直交する場合、A と B は直交すると言います。これは、$A \subset B^\circ$、または$B \subset A^\circ$ のというに相当します。 E がハウスドルフであり、A と B が直交している場合、0 はそれ自体に直交する E の唯一のベクトルであるため、$A \cap B$ は空であるか、簡約するが 0 になります。

#### 定理 2 {#evt-v-s1-thm-2 .statement tag=07XV}

*E を E のプレヒルバーティアン空間と M ベクトル部分空間とし、これはハウスドルフで完全です。このとき、E は M と M に直交する $M^\circ$ 部分空間の位相的直和です。 分解 $E = M \oplus M^\circ$ に関連付けられた E から M への射影子は、 で定義された E から M への射影 $p_M$ です。 1 (V、p. 10)。

まず、すべての $x \in E$ について $x - p_M(x)$ 属するから $M^\circ$ であることを示します。 $y \in M$ にしましょう。すべてのスカラー $\lambda \in K$、ベクトル $p_M(x) + \lambda y$ 属するを M にします。従って、公式 15 (V, p. 10) までに、

$$
\mathscr{R}(\lambda \langle x - p_M(x)|y \rangle) \leq 0
$$

すべての$\lambda \in K$に。特に、$\lambda = \overline{\langle x - p_M(x)|y \rangle}$ を結論するとすると、$\langle x - p_M(x)|y \rangle = 0$ となり、主張となります。

M はハウスドルフであるため、0 は M の唯一のベクトルであり、それ自体に直交するため、$M \cap M^\circ = \{0\}$ になります。 $x \in E$ ごとに、$p_M(x) \in M$ と $x - p_M(x) \in M^\circ$ があります。従って、E は M と $M^\circ$ の直和であり、$p_M$ は E から M への核 $M^\circ$ の射影子です。 $p_M$ は E から M への連続写像 (V, p. 11, cor. 2) なので、GT, III, § 6, No. 2 からたどると、E は M と $M^\circ$ のトポロジカル直和です。

#### 系 {#evt-v-s1-n6-cor-1 .statement tag=07XW}

*E をハウスドルフ プレヒルベルト空間とし、M を E の有限次元ベクトル部分空間とします。すると、E は M の直和と $M^\circ$ です。

E はハウスドルフなので、M も同様です。 M は有限次元なので完全です (I, p. 13)。従って、これを適用するだけで十分です。 2.

の記法と。 2、$M^\circ$ は M の直交補数であり、$p_M$ は E から M への直交投影子 (または直交射影子、または言葉の乱用により射影子) であると言います。 x が E のベクトルである場合、M のベクトル $p_M(x)$ は、M 上の x の直交射影とも呼ばれます。 $p_M$ は E から M への連続線形写像であり、cor によって $\|p_M\| = 1$ があることに注意してください。 V、p. 11の2つ。ただし、$M = \{0\}$の場合は$p_M = 0$になります。

ピタゴラス定理から、直和分解$E = M \oplus M^\circ$から推定される$E/M$から$M^\circ$への標準写像$\psi$は、$E/M$がEの準ノルムから商準ノルムに割り当てられている場合、等長であることがわかります。 (II、p. 4)。私たちは常にそのプレヒルバーティアン構造を $E/M$ に割り当てます。その $\psi$ はプレヒルバーティアン空間の同型です。次に、$E/M$ の商準ノルムがこのプレヒルバーティアン構造から推定されます。

E がヒルバーティアン空間で、M が E の閉ベクトル部分空間である場合、前述の結果をよく使用します。この場合、$M^\circ$ は E、$p_{M^\circ} = 1 - p_M$、$(M^\circ)^\circ = M$ の閉ベクトル部分空間です。

#### 命題 8 {#evt-v-s1-prop-8 .statement tag=07XX}

— E をヒルバーティアン空間、M を E の閉じたベクトル部分空間、I 空でない順序付け有向集合、および $(M_i)_{i \in I}$ を E の閉じたベクトル部分空間の族とする。 写像 $i \mapsto M_i$ が増加するで M が $\bigcup_{i \in I} M_i$ の閉包であるか、写像 $i \mapsto M_i$ が減少するで $M = \bigcap_{i \in I} M_i$ であると仮定します。 次に、すべての $x \in E$ に対して $p_M(x) = \lim_{i \in I} p_{M_i}(x)$ です。

Prop. 8 は props の直後に続きます。 6 (V、p. 11) と 7 (V、p. 12)。

#### 命題 9 {#evt-v-s1-prop-9 .statement tag=07XY}

— E をヒルバーティアン空間とし、M、N を E の 2 つ閉じたベクトル部分空間とします。

a) 次の条件は同等です。
(i) $p_M p_N = p_N p_M$;
(ii) $x \in M$ が $M \cap N$ に直交し、$y \in N$ が $M \cap N$ に直交する場合、x と y は直交します。
(iii) $M \cap N$ に直交する M のすべてのベクトルは N に直交します。
(iv) $M = (M \cap N) + (M \cap N^\circ)$。

b) a) の同等の条件が満たされる場合、E の $p_{M \cap N} = p_M p_N$、ベクトル部分空間 $M + N$ が閉じられ、$p_{M+N} = p_M + p_N - p_M p_N$ が得られます。

c) M が N に直交する場合に限り、$p_M p_N = 0$ が得られます。そうであれば、E のベクトル部分空間 $M + N$ は閉じており、$p_{M+N} = p_M + p_N$ です。

$L = M \cap N$、$M_1 = M \cap L^\circ$、$N_1 = N \cap L^\circ$を入れます。 条件 (ii) は、$M_1$ と $N_1$ が直交していることを意味し、(iii) は、$M_1$ と N が直交していることを意味します。 $N = N_1 + L$があり、$M_1$はLと直交しているので、(ii)と(iii)の同値が証明されました。 条件 (iii) が満たされると、$M_1 = M \cap N^\circ$ が得られ、$M = L + M_1$ なので、条件 (iv) が満たされます。逆に、(iv) から、M の部分空間 $M \cap N$ と $M \cap N^\circ$ が直交であるため、$M_1 = M \cap N^\circ$ が結論するとなり、したがって $M_1 \subset N^\circ$、つまり関係 (iii) となります。

条件 (iv) が満たされると仮定します。すべての $y \in M$ に対して $p_N(y) = p_L(y)$ となるのは明らかであり、したがってすべての $x \in E$ に対して $p_N p_M(x) = p_L p_M(x)$ になります。ただし、$x \in E$、ベクトル、$p_L p_M(x)$、属するからL、ベクトルごとに
$$
x - p_L p_M(x) = (x - p_M(x)) + (p_M(x) - p_L(p_M(x)))
$$
属する ～ $M^\circ + L^\circ = L^\circ$;したがって、$p_L p_M(x) = p_L(x)$ になります。最後に$p_N p_M = p_L p_M = p_L$。 条件 (ii) は (iv) と等価であり、M と N で対称であるため、$p_M p_N = p_L$ も得られます。最後に $p_M p_N = p_N p_M = p_{M \cap N}$ が得られ、(i) が得られます。

逆に、条件 (i) が満たされるとします。 $x \in M$ にしましょう。私たちは持っています
$$
p_M(p_N(x)) = p_N(p_M(x)) = p_N(x)
$$
それで$p_N(x) \in M$。 $x - p_N(x) \in M$を結論する、したがって$x$は元の和、$M \cap N$の$p_N(x)$、および$M \cap N^\circ$の元$x - p_N(x)$となり、(iv)が得られます。

a) と b) の最初の部分を証明しました。ここで、$p_M$ と $p_N$ が通勤し、$q = p_M + p_N - p_M p_N$ を置くと仮定します。 代数 $\mathscr{L}(E)$ では $p_M$ と $p_N$ がべき等であるため、q も同様です。したがって、(GT, III, § 6, No. 2) q の像は E の閉じたベクトル部分空間です。

$q$ の像が $M + N$ に含まれていることは明らかです。ただし、$p_N(x) = x$ があるため、すべての $x \in N$ に対して $q(x) = x$ になります。 $q = p_M + p_N - p_N p_M$ もあるので、すべての $x \in M$ に対して $q(x) = x$ が得られます。 $q$の像は$M + N$に等しいという結論する。 $M + N$ の直交は $M^\circ \cap N^\circ$ に等しく、$q$ の核は明らかに含む $M^\circ \cap N^\circ$ であるため、$q = p_{M+N}$ となります。これは b) を証明します。

$p_N$ の像 $N$ が $p_M$ の核 $M^\circ$ に含まれる場合に限り、つまり $M$ が $N$ に直交する場合に限り、$p_M p_N = 0$ になります。 主張 c) の残りは b) の特殊なケースになります。

#### 注意 {#evt-v-s1-n6-rem-1 .statement tag=07XZ}

— $E$ をヒルバーティアン空間と $M, N$ の 2 つが閉じた $E$ ベクトル部分空間とします。 関係 $M \subset N$ は、$M$ と $N^\circ$ の直交性、つまり、prop による関係 $p_M p_{N^\circ} = 0$ の直交性に相当します。 9、c）。 $p_{N^\circ} = 1 - p_N$ があるので、*関係* $M \subset N$ *と* $p_M = p_M p_N$ *は等価*であることが結論する (« 3 つの垂線定理 »、*cf.* 図 3)。

![図式は部分空間 M、N、および射影 p_M(x)、p_N(x) を表示します](https://i.imgur.com/3Q5z5QG.png)

図3

### 7. ヒルバーティアンの双対空間

#### 定理 3 {#evt-v-s1-thm-3 .statement tag=07Y0}

*$E$をヒルバーティアン空間とします。すべての $x \in E$ について、$x^*$ を $E$ の連続する線型形式 $y \mapsto \langle x | y \rangle$ とします。 写像 $x \mapsto x^*$ は、全単射の半線形 (自己同型 $\xi \mapsto \bar{\xi}$ の場合) $E$ からその双対 $E'$ への写像、および正規化された空間 $E$ から正規化された空間へのアイソメです。 $E'$.*

写像 $x \mapsto x^*$ は (2) (V, p. 1) によって半線形であり、コーシー・シュワルツ不等式により、$\|x^*\| = \sup_{\|y\| \leq 1} |\langle x | y \rangle| = \|x\|$ が得られます。したがって、$x \mapsto x^*$ は $E$ から $E'$ へのアイソメトリです。特に、単射です。 証明を完了するには、$E'$ のすべての $x' \neq 0$ に対して、$x' = x^*$ となるような $x \in E$ が存在することを証明する必要があります。ただし、超平面 $H = \mathrm{Ker}\, x'$ は $E$ に閉店します。これに直交するのは線分$D$です。 $b$ を $D$ の非ゼロ元とします。 線型形式 $b^*$ の核は $H$ に等しいため、$x' = \lambda \cdot b^* = (\overline{\lambda} \cdot b)^*$ となるようなスカラー $\lambda \neq 0$ が存在します。 Q.E.D.

$E$ から双対の $E'$ への写像 $x \mapsto x^*$ は *正規* と言われます。 $E'$ から $E$ への逆写像は正準とも呼ばれ、$x' \mapsto {x'}^*$ で表されます。私たちは持っています

$$
\langle x | y \rangle = \langle y, x^* \rangle, \quad \langle x, x' \rangle = \langle {x'}^* | x \rangle
$$

$E$の$x, y$と$E'$の$x'$。 $x \in E$の$(x^*)^* = x$も。

K が $\mathbf{R}$ のとき、写像 $x \mapsto x^*$ は線形です。この写像によってEのスカラー積をE'に転送します。 $K = \mathbf{C}$のとき、Eのベクトル空間$\overline{E}$,共役をE'(V,p. 6)に写像$x \mapsto x^*$を同型と考えることができます。この写像によって、$\overline{E}$のスカラー積をE'に転送します。

考慮した 2 つのケースでは、E' はヒルベルト空間であり、次の式が得られます。

$$
\langle x^*|y^* \rangle = \overline{\langle x|y \rangle}, \quad \langle x'|x' \rangle = \|x'\|^2
$$

Eの$x, y$とE'の$x'$。

ベクトル $x \in E$ がベクトル $y \in E$ に直交するということは、II、p. 41 で定義された意味で、線型形式 $x^* \in E'$ が $y$ に直交するというというと同等です。 (これは、2 つのケースで語 « 直交» の使用を正当化します)。 M が E の閉じたベクトル部分空間である場合、E' (II, p. 44) で M に直交する部分空間 $M^\circ$ は、以下で定義される E の M の直交の $x \mapsto x^*$ の下で像になります。 V、p. 13 (これにより、2 つのケースで記法 $M^\circ$ の使用が正当化されます)。

#### 系 1 {#evt-v-s1-thm-3-cor-1 .statement tag=07Y1}

*ヒルバート型空間 E の点の族 $(x_i)_{i \in I}$ が合計であるという位数において、 $y \in E$ とすべての添字 $i \in I$ に対する関係 $\langle x_i|y \rangle = 0$ が次のことを意味することが必要かつ十分です。 $y = 0$.*

実際、これは、0 がすべての $x_i$ (II、p. 43 および IV、p. 1) と直交する E' の唯一のベクトルであることを示しています。

#### 系 2 {#evt-v-s1-thm-3-cor-2 .statement tag=07Y2}

*E と F を 2 ヒルベルト空間とします。 $u \in \mathscr{L}(E; F)$、$x \in E$、$y \in F$ には*を入力します

$$
\Phi_u(y, x) = \langle y|u(x) \rangle .
$$

*写像 $u \mapsto \Phi_u$ は、バナッハ空間 $\mathscr{L}(E; F)$ から空間への$F \times E$ 上のすべての連続セスキリニア $^1$ 形からノルムが付与された同型です*

$$
\|f\| = \sup_{\substack{x \in E, y \in F \\ \|x\| \leq 1, \|y\| \leq 1}} |f(y, x)| .
$$

$\Phi_u$ がすべての $u \in \mathscr{L}(E; F)$ に対してセスキ線形で連続であることは明らかです。逆に、$f$を$F \times E$上の連続セスキ線形とする。すべての $x \in E$ に対して、写像 $y \mapsto f(y, x)$ は、ヒルバート空間 F 上で連続する線型形式です。 3、すべての $x \in E$ に対して、F には一意元 $u(x)$ が存在し、すべての $y \in F$ に対して $f(y, x) = \langle u(x)|y \rangle$ になります。 写像 $u : x \mapsto u(x)$ E から F までは線形であり、次のようになります。

$$
\begin{align*}
\|f\| &= \sup_{\|x\| \leq 1} \sup_{\|y\| \leq 1} |f(y, x)| = \sup_{\|x\| \leq 1} \sup_{\|y\| \leq 1} |\langle y|u(x) \rangle| \\
&= \sup_{\|x\| \leq 1} \|u(x)\| ;
\end{align*}
$$

したがって、$u$ 属するから $\mathscr{L}(E; F)$、$f = \Phi_u$、$\|u\| = \|f\|$ となります。これはコルを証明します。 2.

$^1$ (A, IX, § 1, No. 5) を思い出してください。$F \times E$ 上のセスキ線形形式 (左側) $f$ は、$F \times E$ から K への写像であり、V の関係 (1) と (2) を満たします。 p. 1。

標準写像 E から双対 E'' (IV, p. 14) 写像 E から E''、他の語 (IV, p. 16) では、E は再帰的バナッハ空間です。実際、E が実数 (それぞれ複素数) ヒルベルト空間である場合、E' から E への標準写像 φ は、標準化された空間 E' から E へ (それぞれ E の共役空間 $\overline{E}$ へ) 同型です。 適用番目。 3 から E (それぞれ E) を見ると、正規化された空間 E' 上のすべての連続線型形式は、$x \in E$ を伴う形 $x' \mapsto \langle \phi(x')|x \rangle = \langle x, x' \rangle$ であることがわかり、したがって、主張が続きます。

帰結 (IV、p. 17、提案 6) のように:

#### 定理 4 {#evt-v-s1-thm-4 .statement tag=07Y3}

*ヒルバーティアン空間 E では、単位元ボールは弱くコンパクトです。*

#### 命題 10 {#evt-v-s1-prop-10 .statement tag=07Y4}

*ヒルバーティアン空間 E で、フィルター $\mathfrak{F}$ が $x_0$ に弱く収束し、さらに $\lim_{\mathfrak{F}} \|x\| = \|x_0\|$ の場合、E の最初の位相について $\mathfrak{F}$ は $x_0$ に収束します。

実際、$\|x - x_0\|^2 = \|x\|^2 - 2\Re \langle x|x_0 \rangle + \|x_0\|^2$。 $\langle x|x_0 \rangle$は$\mathfrak{F}$に対して仮定だけ$\|x_0\|^2$になる傾向があり、$\|x\|$は$\mathfrak{F}$に対して$\|x_0\|$になる傾向があるため、$\|x - x_0\|$は$\mathfrak{F}$に対して0になる傾向があるので、 命題。

#### 注意 {#evt-v-s1-n7-rem-1 .statement tag=07Y5}

— E がハウスドルフプレヒルバーティアン空間であり、E のヒルバーティアン空間完成である $\hat{E}$ である場合、E の双対 E' は $\hat{E}$ の双対と同一視できることがわかります (III, p. 16)。それは th から続きます。 3 (V、p. 15) では、E 上のすべての連続する線型形式は、$a \in \hat{E}$ である $x \mapsto \langle a|x \rangle$ として独自の方法で書くことができます。

### 練習問題 {#evt-v-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
