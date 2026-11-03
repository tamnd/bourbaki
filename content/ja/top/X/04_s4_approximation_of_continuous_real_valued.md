---
book: top
book_title: General Topology
chapter: X
chapter_title: Function spaces
section: 4
section_title: Approximation of continuous real-valued functions
lang: ja
source: top-v-x
pdf_pages: 0314-0323, 0343-0352
extraction: ocr
subsections:
    - "no": 1
      title: APPROXIMATION OF CONTINUOUS FUNCTIONS BY FUNCTIONS BELONGING TO A LATTICE
      page: 0
      pdf_page: 314
    - "no": 2
      title: APPROXIMATION OF CONTINUOUS FUNCTIONS BY POLYNOMIALS
      page: 0
      pdf_page: 317
    - "no": 3
      title: 'APPLICATION : APPROXIMATION OF CONTINUOUS REAL-VALUED FUNCTIONS DEFINED ON A PRODUCT OF COMPACT SPACES'
      page: 0
      pdf_page: 320
    - "no": 4
      title: APPROXIMATION OF CONTINUOUS MAPPINGS OF A COMPACT SPACE INTO A NORMED SPACE
      page: 0
      pdf_page: 320
statements: 18
exercises: 21
content_sha256: 71fe88aa729069bcc50b5127488a214eaf162001a0a29404cce6ec4d80115e50
translated_from: content/en/top/X/04_s4_approximation_of_continuous_real_valued.md
translation_method: google
source_content_sha256: 949d16c80adeb3bf4fa8d42aa0a09edd31bc61679863b9e79f9e89c41e063551
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: f5acdd4be148ee64ac9b50ce1a734cb333c8c2a9d4a37cc914e07b688c953239
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 4. 連続実数値写像の近似

### 1. 連続写像 × 写像所属の格子への近似

この切断では、*コンパクト* 空間 $X$ 上で定義された連続実数値写像 (*) の集合 $\mathscr{C} = C(X; \mathbf{R})$ を研究し、$\mathscr{C}$ には *一様収束* の位相が備わっていると常に仮定します。 § 3, no. 2 から、この位相はノルムによって定義されることがわかります。

$$
||f|| = \sup_{x \in X} |f(x)|
$$

そして、このノルムは$\mathscr{C}$の$\mathbf{R}$-代数構造と互換性があります。このノルムとこの代数構造により、$\mathscr{C}$ は $\mathbf{R}$ ($§ 1$、no. 6、定理 2、系 1) に対する *完全な標準代数* です。

(*) この切断で考慮されている実数値写像は常に *有限* であると仮定されます。

$H$ が $\mathscr{C}$ の部分集合である場合、$X$ 上の連続実数値写像 $f$ は、$f$ が$H$ の閉包にある場合、$H$ の写像によって一様に近似できると言えます。 空間 $\mathscr{C}$、つまり、各 $\varepsilon > 0$ に対して、すべての $x \in X$ に対して $|f(x) - g(x)| \leq \varepsilon$ となるような写像 $g \in H$ が存在する場合。 $X$ 上のすべての連続実数値写像は、$H$ の写像によって一様に近似できるということは、$H$ が $\mathscr{C}$ で密であることを意味します。

集合 $\mathscr{C}$ では、関係 $f \leq g$ [すべての $x \in X$ に対して $f(x) \leq g(x)$ であることを意味します] は位数関係であり、これに対して $\mathscr{C}$ は格子です。明らかに $|||u| - |v||| \leq ||u - v||$ があるので、$u \to |u|$ は$\mathscr{C}$ の写像をそれ自体に一様に連続させます。したがって、

$$
(u, v) \to \sup (u, v) = \frac{1}{2}(u + v + |u - v|)
$$

そして

$$
(u, v) \to \inf (u, v) = \frac{1}{2}(u + v - |u - v|)
$$

$\mathscr{C} \times \mathscr{C}$ では一様に連続します。

命題 I。 $X$ を圧縮空間とし、$H$ を $X$ で定義された連続実数値写像の集合とします。 $f$ を $X$ 上の連続実数値写像とし、$x \in X$ ごとに写像 $u_x \in H$ が存在し、$u_x(x) > f(x)$ [それぞれ$u_x(x) < f(x)$]。 Then there exists a finite number of functions $u_{x_i} = f_i \in H$ ($1 \leq i \leq n$) such that, if $v = \sup(f_1, f_2, \ldots, f_n)$ [resp. $w = \inf(f_1, f_2, \ldots, f_n)$], we have $v(x) > f(x)$ [resp. $w(x) < f(x)$] for all $x \in X$.

それぞれの $x \in X$ について、$G_x$ をすべての $z \in X$ のオープン集合からなるとし、$u_x(z) > f(z)$ [それぞれ$u_x(z) < f(z)$]。 仮定による$x \in G_x$なので、$x$が$X$を通過するため、$X$は集合$G_x$の和集合になります。 $X$ はコンパクトなので、$G_{x_i}$ が $X$ をカバーするような、点 $x_i$ ($1 \leq i \leq n$) の有限の数が存在し、写像 $f_i = u_{x_i}$ 満たすであることは明らかです。 命題中条件。

定理 I (ディニ)。 $X$ をコンパクト空間とし、$H$ を関係 $\leq$ (それぞれ $\geq$) に関して方向付けられた $X$ 上の連続実数値写像の集合とします。 $H$ の上部 (下部) エンベロープ $f$ が $X$ で有限かつ連続である場合、$f$ は写像所属から $H$ によって一様に近似できます (または同等に、$H$ の切断フィルターは収束します) $X$では$f$まで一律）。

任意の $\varepsilon > 0$ が与えられると、各 $x \in X$ に対して $u_x(x) > f(x) - \varepsilon$ となる写像 $u_x \in H$ が存在します。 命題 I と、$H$ が関係 $\leq$ に対して向けられているという事実により、すべての $x \in X$ に対して $g(x) > f(x) - \varepsilon$ となるような $g \in H$ が存在します。一方、定義までに$g(x) \leq f(x)$が得られるため、定理が証明されます。

#### 系 {#top-x-s4-n1-cor-1 .statement tag=0CEW}

$(u_n)$ を、$X$ 上の連続実数値写像の増加する (それぞれ減少する) 数列とします。 数列 $(u_n)$ の上部 (または下部) 包絡線 $f$ が $X$ で有限かつ連続である場合、数列 $(u_n)$ は $X$ で $f$ に一様に収束します。

$\mathbf{R}_+$ の写像 $x/(n + x)$ の減少列の例が示すように、$X$ がコンパクトであると仮定されなくなった場合、定理 1 の結論は必ずしも有効ではなくなることは明らかです。

#### 命題 2 {#top-x-s4-prop-2 .statement tag=0CEX}

$X$ を圧縮空間とし、$H$ を $X$ 上の連続実数値写像の集合とします。次のように、任意の 2 つの写像 $u \in H, v \in H$、写像 $\sup(u, v)$ および $\inf(u, v)$ が与えられると、 $H$に。次に、$X$ 上の連続実数値写像 $f$ は、各実数 $\varepsilon > 0$ と各対 $x, y$ について、写像所属から $H$ によって一様に近似できます。 $X$の点には、$|f(x) - u_{x, y}(x)| < \varepsilon$と$|f(y) - u_{x, y}(y)| < \varepsilon$のような写像$u_{x, y} \in H$があります。

条件は明らかに必要です。それが十分であることを示しましょう。それぞれの $\varepsilon > 0$ について、すべての $z \in X$ に対して $|f(z) - g(z)| < \varepsilon$ となるような写像 $g \in H$ があることを示します。 $x$ を $X$ のいずれかの点とし、$H_x$ をすべての写像 $u \in H$ のうちの集合とし、$u(x) < f(x) + \varepsilon$ とします。 仮定までに、$y \in X$、写像 $u_{x, y}$ 属するから$H_x$までとなり、$u_{x, y}(y) > f(y) - \varepsilon$になります。したがって、命題 1 により、$H_x$ の写像の有限数が存在し、その上部包絡線 $v_x$ はすべての $z \in X$ に対して $v_x(z) > f(z) - \varepsilon$ となる。一方、$H_x$の定義によって$v_x(x) < f(x) + \varepsilon$が得られます。最後に、仮定による$v_x \in H$。したがって、命題 1 は、写像 $v_{x_i}$ の有限数が​​存在し、その下側包絡線 $g$ がすべての $z \in X$ に対して $g(z) < f(z) + \varepsilon$ となることを示します。しかし、すべての $z \in X$ とすべての添字 $i$ に対して $v_{x_i}(z) > f(z) - \varepsilon$ があるため、すべての $z \in X$ に対して $g(z) > f(z) - \varepsilon$ もあります。 仮定による$g \in H$なので、証明は完了です。

#### 注意 {#top-x-s4-n1-rem-1 .statement tag=0CEY}

集合 $H$ が命題 2 の条件を満たすとき、それは順序 $f \leq g$ に関して格子です。ただし、2 つの写像のうち $H$ の最小の上界 (それぞれ最大の下界) が必ずしも当てはまるとは限らず、$C$ の部分集合 $H$ は、この順序に関して格子である可能性があることに注意する必要があります。 $H$ の $u, v$ は、$C$ の最小の上界 (それぞれ最大の下界) と同じです。 \* 例は、$\mathbf{R}$ のコンパクト区間を $\mathbf{R}$ に凸にした写像によって提供されます。 \*

#### 系 {#top-x-s4-n1-cor-2 .statement tag=0CEZ}

$H$ が、$u \in H$ と $v \in H$ のときはいつでも、$\sup(u, v) \in H$ と $\inf(u, v) \in H$ が存在するようなものであるとします。そして、$X$ の任意の 2 つの異なる点 $x, y$ と任意の 2 つの実数 $\alpha, \beta$ が与えられると、$g(x) = \alpha$ と $g(y) = \beta$ のような写像 $g \in H$ が存在します。次に、$X$ 上のすべての連続実数値写像は、写像所属から $H$ によって一様に近似できます。

#### 定義 1 {#top-x-s4-def-1 .statement tag=0CF0}

*X が任意の集合である場合、A の任意の 2 つの異なる要素 x、y が与えられ、f(x) ≠ f(y) となるような関数 f ∈ H が存在する場合、集合 Y への X の写像の集合 H は、X の部分集合 A の要素を分離するといいます (または A の要素の分離集合である)。

たとえば、X が完全に正規の空間 (章 IX, § 1, no. 5) である場合、X のすべての連続写像の集合を [0, 1] にすると、X の点が分離されます。

#### 定理 2 (石) {#top-x-s4-thm-2 .statement tag=0CF1}

*X を圧縮空間とし、H を $\mathscr{C}(X; \mathbf{R})$ のベクトル部分空間とします。1) H に対する定数写像属する。 2) $u \in H$ の場合、$|u| \in H$; 3) H は X の点を分離します。次に、X 上のすべての連続実数値写像は、H の写像で一様に近似できます。

H が系から命題 2 の条件を満たすことを示すだけで十分です。 $u \in H$ と $v \in H$ の場合、仮定までに、次のようになります。

$$
\sup (u, v) = \frac{1}{2} (u + v + |u - v|) \in H
$$
そして
$$
\inf (u, v) = \frac{1}{2} (u + v - |u - v|) \in H.
$$

一方、x と y を X の任意の 2 つの異なる点とし、α、β を任意の 2 つの実数とします。 仮定までに、$h(x) \neq h(y)$ となる写像 $h \in H$ があります: $h(x) = \gamma$ と $h(y) = \delta$ とします。 H には定数属するがあるため、写像
$$
g(z) = \alpha + (\beta - \alpha) \frac{h(z) - \gamma}{\delta - \gamma}
$$
属するは H であり、$g(x) = \alpha$ と $g(y) = \beta$ になります。

### 2. 連続写像の多項式による近似

集合 X で定義された実数値写像の集合 H が与えられると、X で定義された実数値写像は、写像の実数係数を持つ多項式 (それぞれ定数項を持たない多項式) であると言います。 H の形 $x \to g(f_1(x), f_2(x), \ldots, f_n(x))$ の場合、g は n 内の多項式 (または定数のない多項式項) であり、実数係数で不定 (n は任意) であり、H に対する $f_i$ ($1 \leq i \leq n$) 属するです。

#### 定理 3 (ヴァイエルシュトラス ストーン) {#top-x-s4-thm-3 .statement tag=0CF2}

*Xをコンパクトな空間とし、HをXの点を分離するX上の連続実数値写像の集合とします。次に、X 上のすべての連続実数値写像は、H の写像の多項式 (実数係数) によって一様に近似できます。

定理の等価な主張は、含む定数写像と、X の点を分離する$\mathscr{C}(X; \mathbf{R})$ の * 任意の部分代数が $\mathscr{C}(X; \mathbf{R})$ に密であることです*。

$H_0$ を H の写像のすべての多項式の集合とし、$\overline{H}_0$ を $\mathscr{C}$ の $H_0$ の閉包とします。 g が実数係数を持つ n 変数の多項式である場合、$(u_1, u_2, \ldots, u_n) \to g(u_1, u_2, \ldots, u_n)$ は $\mathscr{C}^n$ から $\mathscr{C}$ への連続写像であり、これは写像 $H_0^n$ から $H_0$ になり、したがって写像 $\overline{H}_0^n$ になります。 $\overline{H}_0$ (章 I, § 2, no. 1、定理 1)。特に、$\overline{H}_0$ は $\mathscr{C}$ のベクトル部分空間であり、明らかに定理 2 の最初と 3 番目の条件を満たします。 2 番目の条件も満たすことを示し、これにより $\overline{H}_0 = \mathscr{C}$ が証明されます。

すべての写像 $u \in \overline{H}_0$ は $X$ で制限されているため、次の補題を証明するだけで十分です。

#### 補題 1 {#top-x-s4-lem-1 .statement tag=0CF3}

*それぞれの実数 $\varepsilon > 0$ と各コンパクト区間 $I \subset \mathbf{R}$ には、すべての $t \in I$ に対して $|p(t) - |t|| \leq \varepsilon$ となるような定数項を持たない多項式 $p(t)$ が存在します。

形 $I = [-a, +a]$ の区間に対して補題を証明するだけで十分です。したがって、区間 $I = [-1, +1]$ に対して $at$ により置き換えること $t$ を証明するだけで十分です。 $|t| = \sqrt{t^2}$ なので、補題 1 は次の結果の帰結になります。

#### 補題 2 {#top-x-s4-lem-2 .statement tag=0CF4}

*$(P_n)$ を、定数項を持たない多項式の数列とします*
$$
(1) \quad p_0(t) = 0, \quad p_{n+1}(t) = p_n(t) + \frac{1}{2} (t - (p_n(t))^2), \qquad n \geq 0.
$$
*区間 $[0, 1]$ 数列 $(p_n)$ では増加するとなり、$\sqrt{t}$ に一様収束します。

補題 2 を証明するには、すべての $t \in [0, 1]$ について、
$$
(2) \qquad 0 \leq \sqrt{t} - p_n(t) \leq \frac{2 \sqrt{t}}{2 + n \sqrt{t}},
$$
(2) は、$0 \leq \sqrt{t} - p_n(t) \leq 2/n$ を意味します。

(2)を$n$の帰納法までに証明します。 $n = 0$も同様です。 $n \geq 0$ の場合、帰納的仮定 (2) から $0 \leq \sqrt{t} - p_n(t) \leq \sqrt{t}$、したがって $0 \leq p_n(t) \leq \sqrt{t}$ が得られ、したがって (1) から次のようになります。
$$
\sqrt{t} - p_{n+1}(t) = (\sqrt{t} - p_n(t)) (1 - \frac{1}{2} (\sqrt{t} + p_n(t))),
$$
$\sqrt{t} - p_{n+1}(t) \geq 0$ と (2) から
$$
\begin{align*}
\sqrt{t} - p_{n+1}(t) &\leq \frac{2 \sqrt{t}}{2 + n \sqrt{t}} \left( 1 - \frac{\sqrt{t}}{2} \right) \\
&\leq \frac{2 \sqrt{t}}{2 + n \sqrt{t}} \left( 1 - \frac{\sqrt{t}}{2 + (n+1) \sqrt{t}} \right) \\
&= \frac{2 \sqrt{t}}{2 + (n+1) \sqrt{t}}.
\end{align*}
$$
Q.E.D.

$X$ がコンパクトでない場合、定理 3 の結論は必ずしも有効ではありません。たとえば、有界で定数できないではない $\mathbf{R}$ 上の連続実数値写像は、多項式 (cf. 練習問題 6) によって $\mathbf{R}$ で一様に近似されます。

#### 命題 3 {#top-x-s4-prop-3 .statement tag=0CF5}

*$(K_i)_{i \in I}$ *を* $\mathbf{R}$のコンパクトな区間、$K = \prod_{i \in I} K_i$ *それらの積*の族とし、$X$を* $K$のコンパクトな部分空間とします。 *その後* $X$ 上のすべての連続実数値写像は * 座標* $x_i = \mathrm{pr}_i x$ の多項式によって一様に近似できます。

なぜなら、$x = (x_i)$ と $y = (y_i)$ が $X$ の 2 つの異なる点である場合、 $x_i \neq y_i$ となるような添字 $i$ が少なくとも 1 つ存在します。したがって、連続写像 $\mathrm{pr}_i$ の族は定理 3 の条件を満たします。

#### 命題 4 {#top-x-s4-prop-4 .statement tag=0CF6}

*$X$ *をコンパクトな空間とし、* $A$を* $X$の閉じた部分空間とし、*そして* $H$ *を連続実数値写像の集合とする* $X$ *これを分離します* $C_A$ の点 * そして、* $A$ * は集合* の共通部分である* $\overline{u}^{-1}(0)$ * $u$ * $H$ を通過します。 *その後、すべての連続実数値写像 on* $X$ *これは零 on* $A$ * $H$ の写像の定数項を使わずに多項式で一様に近似できます。

まず、$A$ が単一の点 $x_0$ で構成される特定のケースを考えてみましょう。この仮説は、$H$ が $X$ の点を分離することを意味します。なぜなら、$x \neq x_0$の場合、仮定までには写像 $u \in H$があり、$u(x) \neq 0 = u(x_0)$になります。したがって、各 $\varepsilon > 0$ と $f(x_0) = 0$ のような $X$ 上の各連続実数値写像 $f$ について、 $|f(x) - g(x)| \leq \varepsilon$ となるような $H$ の写像に多項式 $g$ が存在します (定理 3)。すべて$x \in X$。特に $|g(x_0)| \leq \varepsilon$ なので、

$$
|f(x) - (g(x) - g(x_0))| \leq 2\varepsilon
$$

すべての$x \in X$;そして、$g(x) - g(x_0)$ は定数項を持たない $H$ の写像の多項式であるため、この場合、結果が確立されます。

一般的なケースでは、$X$ の同値関係 $R$ の類が集合 $A$ と $x \notin A$ の集合 $\{x\}$ であると考えます。 商空間 $X/R$ はハウスドルフ (章 I, § 8, no. 6、命題 15) なのでコンパクトです。 $\varphi : X \to X/R$を標準写像とします。 $A$ に消える、$X$ の連続実数値写像 $f$ は、形 $f = f_1 \circ \varphi$ で書くことができます。ここで、$f_1$ は、$X/R$ に消える連続実数値写像です。 点 $x_0' = \varphi(A)$。 適用結果は空間 $X/R$ と点 $x_0'$ ですでに証明されており、最終結果が得られます。

### 3. 応用 : コンパクト空間の積で定義された連続実数値写像の近似

#### 定理 4 {#top-x-s4-thm-4 .statement tag=0CF7}

$(X_i)_{i \in I}$ をコンパクト空間の族とし、
$$
X = \prod_{i \in I} X_i.
$$
次に、$X$ 上のすべての連続実数値写像は、形の写像の有限数の和によって一様に近似できます。
$$
(x_i) \to \prod_{\alpha \in J} u_\alpha(x_\alpha),
$$
ここで、$J$ は $I$ の (任意の) 有限部分集合であり、$u_\alpha$ は各 $\alpha \in J$ の $X_\alpha$ 上の連続実数値写像です。

$X$ で連続する「1 つの変数の写像」$(x_i) \to u_\alpha(x_\alpha)$ (任意の$\alpha \in I$) の集合 $H$ を考えます。この集合は、$X$ の点を分離します。$x = (x_i)$ と $y = (y_i)$ が $X$ の 2 つの別個の点である場合、$x_\alpha \neq y_\alpha$ となるような $\alpha \in I$ が存在し、連続実数値写像が存在します。 $X_\alpha$ の $h_\alpha$ は $h_\alpha(x_\alpha) \neq h_\alpha(y_\alpha)$ になります。 写像 $x \to h_\alpha(\operatorname{pr}_\alpha x)$ 次に属するから $H$ となり、$x$ と $y$ で別個の値が取られます。 $H$ の写像のすべての多項式は定理で記述された形であるため、結果は定理 3 から得られます。

すべての $X_i$ がコンパクトではない場合、定理 4 の結論は必ずしも有効ではありません (cf. 練習問題 9)。

### 4. コンパクト空間の連続写像を正規化空間に近似

$X$ をコンパクト空間とし、$Y$ を体 $\mathbf{R}$ (章 IX, § 3) 上の標準ベクトル空間とします。 空間 $C(X; Y)$ は常に、ノルム $\|u\| = \sup_{x \in X} \|u(x)\|$ ($§ 3$, no. 2) によって定義される一様収束の位相を運ぶと仮定されます。

$X$ に定義された連続実数値写像の集合 $H$、写像所属 ～ $H$ の有限族 $(u_i)_{1 \leq i \leq n}$、および点の有限族 $(a_i)_{1 \leq i \leq n}$ が与えられるとします。 $Y$: $X$ から $Y$ への写像 $x \to \sum_{i=1}^n a_i u_i(x)$ は連続です。それを$\sum_{i=1}^n a_i u_i$で表し、$Y$の係数で$H$の写像の線形結合であると言います。連続写像 $f : X \to Y$ は、$f$ が次のベクトル部分空間の閉包にある場合、$H$ の写像の線形結合によって一様に近似できると言います ($Y$ には係数が含まれます)。この線形結合によって結成された$C(X; Y)$。

#### 命題 5 {#top-x-s4-prop-5 .statement tag=0CF8}

$X$ を圧縮空間、$Y$ を $\mathscr{C}(X; \mathbf{R})$ の $\mathbf{R}$ および $H$ 部分集合の正規化空間とします。 $X$ 上のすべての連続実数値写像が $H$ の写像で一様に近似できる場合、$X$ から $Y$ へのすべての連続実数値写像 $f$ は、線形結合で一様に近似できます。 $H$の写像と$Y$の係数。

任意の実数 $\varepsilon > 0$ が与えられると、各 $x \in X$ に対して、$f$ の振動が $\leq \varepsilon$ である $x$ のオープン近傍が存在します。 したがって、各 $A_i$ の $f$ の振動が $\leq \varepsilon$ となるように、$X$ を覆う有限の開いた$(A_i)_{1 \leq i \leq n}$ が存在します。 $a_i$ を $A_i$ ($1 \leq i \leq n$) の $f$ の値とし、$(u_i)_{1 \leq i \leq n}$ をカバー$(A_i)$ (章 IX, § 4, no. 4、系まで) に従属する単位元の連続分割とする。 命題 4）。 $x$ を $X$ のいずれかの点とします。 $x \notin A_i$ のような各添字 $i$ には $u_i(x) = 0$ があり、$x \in A_i$ のような各添字 $i$ には $\|f(x) - a_i\| \leq \varepsilon$ があります。それは次のとおりです

$$
\left\| f(x) - \sum_{i=1}^n a_i u_i(x) \right\| = \left\| \sum_{i=1}^n (f(x) - a_i) u_i(x) \right\| \leq \varepsilon \sum_{i=1}^n u_i(x) = \varepsilon.
$$

一方、仮定によって、次のような写像 $v_i \in H$ が存在します。

$$
|u_i(x) - v_i(x)| \leq \frac{\varepsilon}{\sum_{j=1}^n \|a_j\|}
$$

すべての$x \in X$ ($1 \leq i \leq n$);したがって、私たちは

$$
\left\| f(x) - \sum_{i=1}^n a_i v_i(x) \right\| \leq 2\varepsilon \quad \text{for all } x \in X,
$$

そして証明が完成しました。

命題 5 から、$\mathscr{C}(X; \mathbf{R})$ の特定の部分集合 $H$ が密であることを証明した各命題には、$X$ の連続写像を任意のノルムに変換する類似の対応する命題が存在することがわかります。 空間 $Y$。 このように対応するから定理3まで命題だけを明示的に書きます。 $X$ の実数値関数のセット $H$ が与えられると、$Y$ に係数を持つ $H$ の関数の多項式は、$H$ に属する有限 (おそらく空) 関数族の積の、$Y$ に係数を持つ線形結合として定義されます。 それから：

#### 命題 6 {#top-x-s4-prop-6 .statement tag=0CF9}

$X$ を圧縮空間とし、$H$ を $X$ の点を分離する $X$ 上の連続実数値写像の集合とします。次に、$X$ のすべての連続写像を、$\mathbf{R}$ にわたるノルム空間 $Y$ に変換することは、$H$ の写像と $Y$ の係数の多項式によって一様に近似できます。

このことから、次のように推測できます。

#### 命題 7 {#top-x-s4-prop-7 .statement tag=0CFA}

$X$ を圧縮空間とし、$H$ を $X$ の点を分離する $X$ 上の連続複素数値写像の集合とします。次に、$X$ のすべての連続写像を、$\mathbf{C}$ にわたる正規化された空間 $Y$ に、写像 $f \in H$ とその共役 $\overline{f}$ と係数の多項式によって一様に近似できます。 $Y$。

$Y$ も $\mathbf{R}$ 上の正規空間であることに注意し、公式を使用して関数 $f \in H$ の実数部と虚数部のセットに命題 6 を適用するだけで済みます。

$$
\Re f = \frac{1}{2} (f + \overline{f}), \quad \Im f = \frac{1}{2i} (f - \overline{f}).
$$

#### 系 1 {#top-x-s4-prop-7-cor-1 .statement tag=0CFB}

$X$ が空間 $\mathbf{C}^n$ のコンパクト部分集合である場合、$X$ のすべての連続写像 $(z_1, z_2, \ldots, z_n) \to f(z_1, z_2, \ldots, z_n)$ を体 $\mathbf{C}$ にわたる正規化された空間 $Y$ は次のように一様に近似できます。 $z_k$ と $\overline{z}_k$ の多項式、$Y$ の係数。

一般に、たとえ$Y = \mathbf{C}$であっても、変数$z_k$単独の多項式($Y$に係数を使用)で$f$を一様に近似することは不可能であることが後でわかります。

#### 系 2 {#top-x-s4-prop-7-cor-2 .statement tag=0CFC}

$X$ を局所コンパクト空間とし、$C_0(X)$ を無限遠で 0 になる傾向がある $X$ から $\mathbf{C}$ への連続写像のノルム $\mathbf{C}$-代数とする。 $A$ を $X$ の点を分離する $C_0(X)$ の部分代数とします。これは、(i) $f \in A$ のときは常に$\overline{f} \in A$、(ii) $x \in X$ ごとに、$f(x) \neq 0$ となるような$f \in A$ が存在します。すると$A$は$C_0(X)$に密集します。

$X'$ が$\omega$ から$X$ に点を無限遠で結合して得られる圧縮空間である場合、$C_0(X)$ は、$C(X; \mathbf{C})$ からなるの写像で消える連続写像の部分空間と識別できます。 $C_0(X)$ の $\omega$、ノルムは、によって定義されます

$$
\|f\| = \sup_{x \in X} |f(x)| = \sup_{x \in X} |f(x)|.
$$

命題 7 のおかげで、すべての $f \in C_0(X)$ は、写像所属から $A$ までの複素数係数の多項式で一様に近似できます。さらに、$f(\omega) = 0$ なので、no. 2、命題 4 の引数は、これらの多項式には定数項がないと仮定し、その後、属するから $A$ になると仮定できることを示しています。

他の命題 7 の適用は次のとおりです。

#### 命題 8 {#top-x-s4-prop-8 .statement tag=0CFD}

P を、$\mathbf{R}^m$ から $\mathbf{C}$ へのすべての周期連続写像の集合とし、その含む $\mathbf{Z}^m$ の周期の群とします。次に、P までのすべての写像所属は、形の写像の複素数係数を使用して、$\mathbf{R}^m$ 線形結合で一様に近似できます。

$$
(x_1, x_2, \ldots, x_m) \to e(h_1 x_1 + h_2 x_2 + \cdots + h_m x_m),
$$

ここで、$h_i$ は有理数整数です (このような線形結合は m 個の変数の三角多項式と呼ばれます)。

P (一様収束の位相を備えている) が、コンパクト空間 $\mathbf{T}^m$ のすべての連続写像の $\mathbf{C}$ (章 VII, § 1, no. 6)、および命題を適用する 7 のすべての写像の空間と正準的に同型であることを観察するだけで済みます。 $\mathbf{T}^m$の写像の集合を$\mathbf{C}$に、対応するを写像の$\mathbf{R}^m$の$(x_1, x_2, \ldots, x_m) \to e(x_i) \quad (1 \leq i \leq m)$を$\mathbf{C}$にします。

### 練習問題 {#top-x-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
