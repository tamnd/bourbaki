---
book: top
book_title: General Topology
chapter: VIII
chapter_title: Complex numbers
section: 2
section_title: Angular measure, trigonometric functions
lang: ja
source: top-v-x
pdf_pages: 0111-0121, 0131-0131
extraction: ocr
subsections:
    - "no": 1
      title: THE MULTIPLICATIVE GROUP U
      page: 0
      pdf_page: 111
    - "no": 2
      title: ANGLES
      page: 0
      pdf_page: 113
    - "no": 3
      title: ANGULAR MEASURE
      page: 0
      pdf_page: 114
    - "no": 4
      title: TRIGONOMETRIC FUNCTIONS
      page: 0
      pdf_page: 115
    - "no": 5
      title: ANGULAR SECTORS
      page: 0
      pdf_page: 118
    - "no": 6
      title: CROSSES
      page: 0
      pdf_page: 119
statements: 5
exercises: 4
content_sha256: 2431111a4b16abd45bc5e27733b932dfa8576c448a531290531df02a867a69b7
translated_from: content/en/top/VIII/02_s2_angular_measure_trigonometric_functions.md
translation_method: google
source_content_sha256: 021b6d0e671c54e66a21fa0d56b2ec8b29291d75506ee737a931d924894ce940
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 31ea173109d07b8bcd9cf4ff40494a5ed0312144cfaa9bad7309f222693cfbab
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 2. 角度測定、三角法写像

### 1. 乗法群U

#### 定理 1 {#top-viii-s2-thm-1 .statement tag=0C09}

絶対値 1 の複素数の (乗法的、位相的群 $U$ は、 実数 mod 1 の (加法的、位相的群 $T$) と同型です。

$U = S_1$ はコンパクトで接続されており、$\mathbf{R}$ の開いた区間 (章 VI, § 2, no. 4, 命題 5) と同型の単位元 -1 の近傍を持ちます。したがって、定理は、章 V, § 2、定理 2 で与えられる $T$ のトポロジカル特徴付けの帰結です。

#### 系 {#top-viii-s2-n1-cor-1 .statement tag=0C0A}

非ゼロ複素数の乗法群 $C^*$ は、群 $\mathbf{R} \times T$ (cf. § 1, no. 3, 命題 1) と同型です。

#### 注意 {#top-viii-s2-n1-rem-1 .statement tag=0C0B}

群 $C^*$ と $\mathbf{R} \times T$ の同型は、体 $C$ のすべての「二項方程式」$z^n = a$ の根の存在を意味します。この事実と $C$ のローカル互換性を使用して、ダランベール-ガウス (練習問題 2) の定理の他の証明を取得できます。

群 $\mathbf{U}$ には、群 $\mathbf{T}$ の異なる同型が*2つ* だけあります。なぜなら、$g, g'$が$\mathbf{T}$の2つの同型を$\mathbf{U}$に重ねたもので、$h'$が$g'$の逆数である場合、$h' \circ g$は$\mathbf{T}$の自己同型であるため、(章) VII, , no. 4, 命題 6) $g'(x) = g(x)$ または $g'(x) = g(-x)$ のいずれかが同じです。 $g$ は、$i$ が点 $\frac{1}{4}$ の類 mod 1 の $g$ の下で像となるようなものであると常に仮定できます。次に、$\varphi$ が $\mathbf{T}$ 上の $\mathbf{R}$ の標準準同型を表す場合、加法群 $\mathbf{R}$ の乗法群 $\mathbf{U}$ のすべての厳密な射は形のものになります。 $x \to g(\varphi(x/a))$、ここで $a$ は実数 $\neq 0$ (章 VII, § 2, no. 3、命題 4); 区間 $]-\frac{1}{2}|a|, \frac{1}{2}|a|[$ は、この厳密な射によってその像に 1 対 1 でマッピングされる $\mathbf{R}$ の最大の対称開いた区間であり、$g(\varphi(\frac{1}{4})) = i$ があることに注意してください。 準同型 $x \to g(\varphi(x))$ を $x \to e(x)$ で表します。したがって、$\mathbf{R}$ から $\mathbf{U}$ へのすべての厳密な射は、形 $x \to e(x/a)$ になります。ここで、$a \neq 0$ です。 写像 $e(x)$ は $\mathbf{R}$ で連続しており、複素数値であり、恒等式を満たします。

(1) $$ |e(x)| = 1, $$
(2) $$ e(x + y) = e(x)e(y), $$

関係と一緒に

(3) $$ e(0) = 1,\quad e(\frac{1}{4}) = i,\quad e(\frac{1}{2}) = -1,\quad e(\frac{3}{4}) = -i,\quad e(1) = 1. $$

(1) と (2) から次のことがわかります。

(4) $$ e(-x) = \frac{1}{e(x)} = \overline{e(x)}, $$

そして(2)と(3)から

$$
e(x + \frac{1}{4}) = ie(x),\quad e(x + \frac{1}{2}) = -e(x),
$$
$$
e(x + \frac{3}{4}) = -ie(x),\quad e(x + 1) = e(x).
$$

したがって、写像 $e(x)$ は *周期的* であり、主周期として 1 を持ちます。

#### 注意 {#top-viii-s2-n1-rem-2 .statement tag=0C0C}

写像 $x + iy \to e^{x}e(y)$ は、乗法群 $\mathbf{C}^*$ に対する加法群 $\mathbf{C}$ の厳密な射であり、その制限から 0 の適切な近傍は、次のような$\mathbf{C}$ のローカル同型です。 $\mathbf{C}^*$。その結果 (章 VII, § 2, no. 3) $\mathbf{C}^*$ に対する $\mathbf{C}$ のすべての厳密な射は形 $x + iy \to e^{\alpha x + \beta y}e(\gamma x + \delta y)$ であり、$\alpha, \beta, \gamma, \delta$ は $\alpha \delta - \beta \gamma \neq 0$ のような任意の実数です。これらの準同型のうち、$z \to e^z$ で示されるのは 1 つだけであることが後でわかります。

$$
\lim_{z \to 0} \frac{e^z - 1}{z} = 1;
$$

そしてこの準同型の実軸に対する制限は$e^x$(よって記法)と同じです。

### 2. 角度

体 $\mathbf{R}$ が順序付けされているため、$e_1 \wedge e_2$ を正の二ベクトルとして ($e_1, e_2$ は標準基底のベクトルである) として、実数平面 $\mathbf{R}^2$ の向きを変えることができます。 方向付けされた実数平面 $\mathbf{R}^2$ (以下では $\mathbf{C}$ で識別) で、原点 o (*) に対する任意の光線ペア $(\Delta_1, \Delta_2)$ の角度 $(\Delta_1, \Delta_2)$ を定義できます。 すべての角度の集合 $\mathfrak{A}$ には、アーベル群の構造が含まれます (加算的に記述されます)。

$$
(\Delta_1, \Delta_3) = (\Delta_1, \Delta_2) + (\Delta_2, \Delta_3),
$$

特に $(\Delta_1, \Delta_1) = 0$ と $(\Delta_2, \Delta_1) = - (\Delta_1, \Delta_2)$ です。

平面角 $\varpi$ は、$\mathfrak{A}$ の方程式 $2\theta = 0$ の解 $\neq 0$ です。それは、負の実半軸が正の実半軸となす角度です。

$z$ が非ゼロ複素数の場合、$\mathrm{Am}(z)$ で示される $z$ の振幅 (または引数) は、原点 o で $z$ を通過する光線が正の実半軸となす角度です。 写像 $z \to \mathrm{Am}(z)$ は乗法群 $\mathbf{C}^*$ の加法群 $\mathfrak{A}$ の準同型であるため、次のようになります。

$$
\mathrm{Am}(zz') = \mathrm{Am}(z) + \mathrm{Am}(z') \quad \text{and} \quad \mathrm{Am}(\overline{z}) = \mathrm{Am}(z^{-1}) = - \mathrm{Am}(z).
$$

角度 $\delta = \mathrm{Am}(i)$ は正の直角と呼ばれます。それは方程式$2\theta = \varpi$の$\mathfrak{A}$の解の1つであり、もう1つは$- \delta = \delta + \varpi$です。

準同型 $z \to \mathrm{Am}(z)$ は、$\mathbf{C}^*$ の部分群 $\mathbf{U}$ に制限されており、$\mathbf{U}$ の群構造の $\mathfrak{A} \ (***)$ の同型です。もし私たちが

(*) 代数から、変換 $\Delta_1$ を含む回転が存在する場合、2 つの対 $(\Delta_1, \Delta_2)$ と $(\Delta'_1, \Delta'_2)$ を同等とみなすことにより、原点 o を持つ光線のすべての対 $(\Delta_1, \Delta_2)$ の集合上で同値関係が定義されることがわかります。 $\Delta'_1$ と $\Delta_2$ を同時に $\Delta'_2$ にします。 対 $(\Delta_1, \Delta_2)$ の角度、または $\Delta_2$ が $\Delta_1$ と作る角度は、対 $(\Delta_1, \Delta_2)$ の定義同値類になります。

(**) これは、体 $\mathbf{R}$ がピタゴラス行列であるため、原点 o を持つすべての光線が円 $S_1$ と交わるからです。

この同型写像を使用して、$\mathbf{U}$ のトポロジーをグループ $\mathfrak{A}$ に移すと、後者のグループはコンパクトなトポロジーグループになり、$\mathbf{C}^*$ の $\mathfrak{A}$ への写像 $z \to \mathrm{Am}\,(z)$ はトポロジーグループ $\mathfrak{A}$ へのトポロジーグループ $\mathbf{C}^*$ の厳密な射です。

$\theta \to f(\theta)$ で、$\mathfrak{A}$ の $\mathbf{U}$ への同型性を表します。これは、$\mathbf{U}$ の $\mathfrak{A}$ への同型性 $z \to \mathrm{Am}\,(z)$ の逆です。 定義により、$\Re(f(\theta))$ は $\cos \theta$ で示され、角度 $\theta$ の余弦と呼ばれます。 $\Im(f(\theta))$ は $\sin \theta$ で示され、角度 $\theta$ のサインと呼ばれます。 これらの写像は、トポロジー 群 $\mathfrak{A}$ と、次の満たす関係 (*loc. cit.*) 上で連続しており、上記の定義の明らか帰結です。

$$
\begin{align*}
\cos 0 &= 1, & \sin 0 &= 0, & \cos \varpi &= -1, & \sin \varpi &= 0, \\
\cos(-\theta) &= \cos \theta, & \sin(-\theta) &= -\sin \theta, \\
\cos(\theta + \theta') &= \cos \theta \cos \theta' - \sin \theta \sin \theta', \\
\sin(\theta + \theta') &= \sin \theta \cos \theta' + \sin \theta' \cos \theta, \\
\cos^2 \theta + \sin^2 \theta &= 1.
\end{align*}
$$

定義により、角度 $\theta \in \mathfrak{A}$ の正接は、$\cos \theta \neq 0$ のときはいつでも $\sin \theta / \cos \theta$ (*loc. cit.*) と定義され、$\tan \theta$ で表されます。それは連続した写像であり、角度 $\delta$ と $-\delta$ に対して値 $\infty$ を取ることで、$\tilde{\mathbf{R}}$ (章 VI, § 3, no. 4) に連続して拡大するになります。 $\tan (\theta + \varpi) = \tan \theta$があります。 $\cot \theta$ で示される $\theta$ の余接は、$\tilde{\mathbf{R}}$ の元は $1 / \tan \theta$ に等しいです。

$\mathrm{Am}\,(z) = \theta$ の場合、$z = |z| (\cos \theta + i \sin \theta)$ があることに注意してください。この式は、複素数 $z \neq 0$ の三角関数形と呼ばれます。

### 3. 角度測定

no. 1 の定理 1 により、角度の位相位相群 $\mathfrak{A}$ は $\mathbf{T}$ と同型になります。 $\mathfrak{A}$ に対する $\mathbf{R}$ のすべての厳密射は、$\mathbf{U}$ の $\mathfrak{A}$ への同型射 $z \to \mathrm{Am}\,(z)$ を $\mathbf{U}$ への $\mathbf{R}$ の厳密射を合成することによって取得できます。 $\hat{x}(x) = \mathrm{Am}\,(e(x))$ を置くと、$\mathfrak{A}$ に対する $\mathbf{R}$ の厳密な射はすべて、$x \to g(x/a)$ ($a \neq 0$) の形式になります。 実数 $a > 0$ が与えられた場合、すべての角度 $\theta$ 対応するを準同型 $x \to \hat{x}(x/a)$ により、実数 mod $a$ の類 (つまり、元の元) に固定されます。 $\mathbf{Z}/a\mathbf{Z}$) これは、基底 $a$ に対する $\theta$ の尺度と呼ばれます。言葉の乱用により、この類のすべての実数は $\theta$ の単位とも呼ばれます。角度 $\hat{x}(x/a)$ は、メジャー $x$ の角度と呼ばれます (基底 $a$ に対して)。 $x$ が $\theta$ の尺度で、$x'$ が $\theta'$ の尺度 (同じ基底と比較して) である場合、$x + x'$ は $\theta + \theta'$ の尺度、$-x$ は $\theta$ の尺度です。 角度の主な尺度 (基底 $a$ に対する) は、区間 $[0, a[$ にある尺度の 1 つです。

基底 $a$ の選択。 私たちは常に基底 $a > 1$ に制限します。 それぞれの $a > 1$ は角度 $\omega = \frac{\pi}{a}$ に対応し、その主尺度は 1 であり、これは底 $a$ に対する角度尺度の単位と呼ばれます。逆に、各角度 $\omega \neq 0$ には、$\frac{\pi}{a} = \omega$ のような固有の $a > 1$ が対応するため、角度測定単位の知識によって底 $a > 1$ が完全に決定されます。

数値計算では通常、$a = 360$ または $a = 400$ のいずれかを使用します。角度尺度の対応する単位元は、次数 ($a = 360$) または等級 ($a = 400$) と呼ばれます。

解析において、そして実際、数値計算が関与しない数学のすべての分野において、基底 $a$ は条件によって定義されます。

$$
\lim_{x \to 0} \frac{e(x/a) - 1}{x} = i
$$

広く使われています。この基底は$2\pi$で表されます。角度尺度の対応する単位元はラジアンと呼ばれ、その尺度はラジアン尺度と呼ばれます。前述の複合体 $z$ の $e^z$ の定義を使用すると、すべての $x \in \mathbf{R}$ に対して $e(x) = e^{2\pi ix}$ が得られます。

基底 $a$ が選択されると、角度について話すときは、通常、基底 $a$ に対するこの角度の尺度を意味します。 (数値計算が関与しない場合はいつもそうなのですが) 基底 $a$ がずっと固定されており、同じ角度に対して合同な mod $a$ 対応するである 2 つの実数を覚えていれば、この言葉の乱用には何の欠点もありません。

たとえば、複素数 $z \neq 0$ の振幅によって通常理解されるのは、この角度のラジアン単位であり、検討中の質問に応じて規則によって決定されます。これらの規則が作成されると、このようにして選択された振幅の尺度は Am $(z)$ で示されます。

### 4. 三角関数写像

写像 $\cos \theta, \sin \theta, \tan \theta, \cot \theta$ ($\mathscr{A}$ で定義) を $\mathbf{R}$ の準同型 $x \to \frac{\pi}{a}(x/a)$ で$\mathscr{A}$ に合成すると、写像

$$
\cos \left( \frac{x}{a} \right), \quad \sin \left( \frac{x}{a} \right), \quad \tan \left( \frac{x}{a} \right), \quad \cot \left( \frac{x}{a} \right)
$$

こうして得られたものはそれぞれ、基底 $a$ に対する *数* $x$ のコサイン、サイン、タンジェント、コタンジェントと呼ばれ、$\cos_a x$、$\sin_a x$、$\tan_a x$、$\cot_a x$ と書きます。 写像 $x \to \cos_a x + i \sin_a x$ は $\theta \to \cos \theta + i \sin \theta$ と $x \to \tilde{\sigma}(x/a)$ の合成であるため、$\cos \theta$ と $\sin \theta$ の no. 2 の定義から、同一性が得られます。

$$
e\left( \frac{x}{a} \right) = \cos_a x + i \sin_a x,
$$

これは以下と同等です

$$
\cos_a x = \Re \left( e\left( \frac{x}{a} \right) \right), \qquad \sin_a x = \Im \left( e\left( \frac{x}{a} \right) \right),
$$

また、(4) により、次と同等になります。

$$
\cos_a x = \frac{1}{2} \left( e\left( \frac{x}{a} \right) + e\left( -\frac{x}{a} \right) \right), \qquad \sin_a x = \frac{1}{2i} \left( e\left( \frac{x}{a} \right) - e\left( -\frac{x}{a} \right) \right).
$$

したがって、アイデンティティ

$$
\cos_b x = \cos_a \left( \frac{ax}{b} \right), \qquad \sin_b x = \sin_a \left( \frac{ax}{b} \right).
$$

数値計算が関与しない数学分野で生じる唯一の三角関数写像は、上で参照した基底 $2\pi$ に関連するものです。これらの写像は、$\cos_{2\pi} x$、$\sin_{2\pi} x$、$\tan_{2\pi} x$、$\cot_{2\pi} x$ の代わりに、単に $\cos x$、$\sin x$、$\tan x$、$\cot x$ で表されます。数値計算のために、三角関数の表写像対応するから基底 $a = 360$ および $a = 400$ があります。そして式 (6) により、三角関数写像の値を他の基底と比較して推定することができます。

先ほど思い出した*角度*の余弦と正弦の間の関係は、明らかにこれらの角度を測定する*数*の余弦と正弦の間に同じ関係を生じさせます。特に、私たちは

$$
\begin{align*}
\cos_a (x + y) &= \cos_a x \cos_a y - \sin_a x \sin_a y, \\
\sin_a (x + y) &= \sin_a x \cos_a y + \sin_a y \cos_a x, \\
\cos_a (-x) &= \cos_a x, \qquad \sin_a (-x) = -\sin_a x, \\
&\cos_a^2 x + \sin_a^2 x = 1.
\end{align*}
$$

写像 $\cos_a x$ と $\sin_a x$ は $\mathbf{R}$ で連続し、周期 $a$ で周期的です。さらに、$a$ はこれら写像の*主期間* であり、関係 $\cos_a x = \cos_a y$ は $\sin_a x = \sin_a y$ または

$$
\sin_a x = -\sin_a y,\quad \text{i.e.,}
$$

$$
e\left(\frac{x}{a}\right) = e\left(\frac{y}{a}\right)\quad \text{or}\quad e\left(\frac{x}{a}\right) = e\left(-\frac{y}{a}\right),
$$

それでどちらかが

$$
x \equiv y \pmod{a}\quad \text{or}\quad x \equiv -y \pmod{a};
$$

そして同様に

$$
\sin_a x = \sin_a y
$$

は、$x \equiv y \pmod{a}$ または $x + y \equiv \frac{1}{2} a \pmod{a}$ のいずれかに相当します。

このことから、$\cos_a x$ は区間 $[0, \frac{1}{2} a]$ で同じ値を 2 回取ることはありません。したがって、この区間に限定すると、この区間の区間 $[-1, +1]$ への*全単射* 写像になります。 $\cos_a 0 = 1$ と $\cos_a (\frac{1}{2} a) = -1$ なので、$x \to \cos_a x$ は $[0, \frac{1}{2} a]$ *上* $[-1, 1]$ (章 IV, § 2, no. 6、定理 5 および注意) の *真に減少する* 写像です。 $x = a/4$には$\cos_a x = 0$、$0 \leq x < a/4$には$\cos_a x > 0$、$a/4 < x \leq a/2$には$\cos_a x < 0$があります。 $\cos_a (-x) = \cos_a x$ 以来、$\cos_a x$ が区間 $[- \frac{1}{2} a, 0]$ で、したがって$\mathbf{R}$ 全体にわたって周期性によってどのように変化するかを推測できます (図 8)。 $\sin_a x = -\cos_a(x + a/4)$ なので、$\sin_a x$ が $\mathbf{R}$ でどのように変化するかを推測することもできます (図 8)。

![y = sin_a x および y = cos_a x を示すグラフ](https://i.imgur.com/3Q5z5QG.png)

図8。

写像 $\tan_a x$ は、$\mathbf{R}$ から $\tilde{\mathbf{R}}$ への連続した写像です。 値 $\frac{1}{4} a + \frac{1}{2} k a \ (k \in \mathbf{Z})$ には値 $\infty$ かかります。 $\frac{1}{2} a$ は $\tan_2 x$ の期間であるため、*主要期間* となります。 区間 $[0, \frac{1}{4} a]$ では、$\sin_a x$ は 0 から 1 に増加し、$\cos_a x$ は 1 から 0 に減少します。したがって、$\tan_a x$ は $[0, \frac{1}{4} a[$ で *真に増加する* となり、写像この区間では *真に増加する* になります。 $[0, +\infty[$;したがって、$\tan_a x$ は区間の真に増加するになります。

![y および x というラベルが付いた曲線を示し、軸に -a/4、0、a/4、a/2、3a/4 とマークされたグラフ](../images/complex_numbers_9.png)

図9。

]— $\frac{1}{4} a, + \frac{1}{4} a$[。これは、この区間の $\mathbf{R}$ への同写写像です (図 9)。

### 5. 角度セクター

原点 o を持つ 2 つの別個の閉じた光線 $\Delta_1, \Delta_2$ が与えられた場合、$x$ を角度 $(\widehat{\Delta_1, \Delta_2})$ の主尺度とします (基底 $a$ に対して、きっぱりと選択されます)。角度 $(\widehat{\Delta_1, \Delta})$ の主測度 $y$ が $0 \leq y \leq x$ (それぞれ $0 < y < x$) を満たすような、原点 o を持つ閉じた (それぞれ開いた) 光線 $\Delta$ の和集合は、原点 $\Delta_1$ と端を持つ閉じた (それぞれ開いた) 角度セクター S です。 $\Delta_2$、代数で定義されています。なぜなら、回転によって、S が点を通る光線を含む通さない場合に常に簡約するすることができるからです — 1. $\alpha$ と $\beta$ が、それぞれ $\Delta_1$ と $\Delta_2$ が正の実半軸となす角度である場合、閉角度セクター S は次のようになります。 $\tan \frac{1}{2} \alpha \leq \tan \frac{1}{2} \theta \leq \tan \frac{1}{2} \beta$ のように、正の実半軸と角度 $\theta$ を作る閉じた半線 $\Delta$ の和集合。ここで、$u, v, t$ がそれぞれ区間 ]— $\frac{1}{2} a, + \frac{1}{2} a$[ にある $\alpha, \beta, \theta$ の測度である場合、これらの不等式は $\tan_a \frac{1}{2} u \leq \tan_a \frac{1}{2} t \leq \tan_a \frac{1}{2} v$ と等価です。そして、$\tan_a x$ は区間 ]— $\frac{1}{4} a, + \frac{1}{4} a$[ の増加する写像であるため、$u \leq t \leq v$ または $0 \leq t - u \leq v - u$ とも等価です。 $x = v - u, y = t - u$ 以降、結果は閉じた角度セクターについて証明されており、開いた角度セクターについても証明が同様です。

閉じた角度セクターは、$\mathbf{R}^2$ の閉じた集合であり、同じ原点と同じ端を持つ開いた角度セクターは、$\mathbf{R}^2$ のその内部です。

図10。

(章 VI, § 2, no. 3、命題 3)。主尺度 $x$ を持つ角度 $(\widehat{\Delta_1, \Delta_2})$ は、扇形 S の角度と呼ばれます。 S は、$x < \frac{1}{2} a$ の場合は突出、$x = \frac{1}{2} a$ の場合は平坦 (または閉じた半平面) であると言われます。 $x > \frac{1}{2} a$ の場合は再入可能。突角セクターは、$x < \frac{1}{4} a$ の場合は鋭角、$x = \frac{1}{4} a$ の場合は右、$x > \frac{1}{4} a$ の場合は鈍角です。扇形 S の二等分線は、$\Delta_1$ と角度 $y = \frac{1}{2} x$ を作る光線 $\Delta$ です。

2 つの別個の閉じた光線 $\Delta_1, \Delta_2$ 決定する 2 つの閉じた角度セクター。彼らの和集合は実際の平面$\mathbf{R}^2$であり、彼らの共通部分は$\Delta_1 \cup \Delta_2$です。

### 6. 十字架

また、代数では、極大順序体上の 2 次元ベクトル空間の線の対の交差も定義しました (*)。この定義は、特に実平面 $\mathbf{R}^2$ に当てはまります。すべての十字の集合 $\mathscr{A}_0$ には、アーベル群の構造が含まれます (加算的に記述) によって定義されます。

$$
(\overline{D_1, D_3}) = (\overline{D_1, D_2}) + (\overline{D_2, D_3})
$$

特に $(\overline{D_1, D_1}) = 0$ と $(\overline{D_2, D_1}) = - (\overline{D_1, D_2})$ です。

右十字 $\delta_0$ は、$\mathscr{A}_0$ の方程式 $2\theta = 0$ の解 $\neq 0$ です。それは、虚軸が実軸と作る十字です。

(*) 同値関係は、変換という直接の類似点が存在する場合、$(D_1, D_2)$ と $(D'_1, D'_2)$ の 2 つの対が同等であるとみなして、$(D_1, D_2)$ のすべての非等方性対の集合上で定義されていることを思い出します。 $D_1$ から $D'_1$ へ、$D_2$ から $D'_2$ へ同時に。 対 $(D_1, D_2)$ のクロスは、対の同値類になります。

光線 $\Delta$ が正の実半軸となす角度、つまり線 D がなす角度を対応するにすることで、群 $\mathfrak{A}$ の角度の定義する標準準同型 $\varphi$ を十字の群 $\mathfrak{A}_0$ に加えます。 含む $\Delta$ は実軸で作成します。十字 $\theta_0$ は 2 つの角 $\theta$ と $\theta + \omega$ の $\varphi$ の下にある像です。したがって、$\mathfrak{A}_0$ は、部分群 $\{0, \omega\}$ による $\mathfrak{A}$ の商と同型です。 $\varphi$ に関連付けられた全単射準同型を使って剰余群 $\mathfrak{A}/\{0, \omega\}$ の $\mathfrak{A}_0$ 位相を輸送にすると、$\mathfrak{A}_0$ はコンパクトな位相位相群になり、$\varphi$ は厳密な位相位相になります。 $\mathfrak{A}$の$\mathfrak{A}_0$への射。

If we compose the homomorphism $\varphi$ of $\mathfrak{A}$ onto $\mathfrak{A}_0$ with the homomorphism $x \to \tilde{\sigma}(x/a)$ of $\mathbf{R}$ onto $\mathfrak{A}$, we have a homomorphism $x \to \tilde{\sigma}_0(x/a)$ of $\mathbf{R}$ onto $\mathfrak{A}_0$; every cross $\theta_0 \in \mathfrak{A}_0$ corresponds, under this homomorphism, to a class of real numbers mod $\frac{1}{2} a$, which is called the measure of the cross $\theta_0$ (relative to the base $a$); by abuse of language, every number in this class is called a measure of $\theta_0$, and that one which belongs to the interval $[0, \frac{1}{2} a[$ is called the principal measure of $\theta_0$;十字$\tilde{\sigma}_0(x/a)$は小節$x$の十字です。 $\theta_0$ のすべての尺度は、準同型 $\varphi$ の下の像が $\theta_0$ である 2 つの角度 $\theta, \theta + \omega$ のいずれかの尺度でもあります。

ここでも、基底 $a$ が選択されると、十字架について話すとき、通常、言葉の乱用により、基底 $a$ に対するこの十字架の尺度を意味します。

#### 注意 {#top-viii-s2-n6-rem-1 .statement tag=0C0D}

各複素数$z \neq 0$を、oと$z$を通る線が実軸と作る十字にマッピングすることにより、$\mathfrak{A}_0$への$\mathbf{C}^*$の準同型写像を定義できます。 明らかに、この準同型性は、$\varphi$ と $\mathbf{C}^*$ の準同型性 $z \to \mathrm{Am}\,(z)$ を $\mathfrak{A}$ に合成したものです。したがって、これは位相群 $\mathfrak{A}_0$ への位相群 $\mathbf{C}^*$ の厳密な射であり、関連する全単射準同型写像は、商群 $\mathbf{C}^*/\mathbf{R}^*$ の $\mathfrak{A}_0$ への同型写像です。

D が実軸と交差 $\theta_0$ する線を表し、$(a, b)$ が D の方向比の対である場合、十字の接線 $\theta_0$ ($\tan\,\theta_0$ で示される) は $\tilde{\mathbf{R}}$ の元 $b/a$ (もし $= \infty$ の場合) であることがわかります。 $a = 0$)、これは線 D の傾きとも呼ばれます。 $\theta$ と $\theta + \omega$ が、$\varphi$ の下の像が $\theta_0$ である 2 つの角度である場合、$\tan\,\theta_0 = \tan\,\theta = \tan(\theta + \omega)$ が得られます。

写像 $\theta_0 \to \tan\,\theta_0$ は、$\mathfrak{A}_0$ から $\tilde{\mathbf{R}}$ への同相写像であり、トポロジカル空間 $\mathbf{C}^*/\mathbf{R}^*$ は単なる実射影線 $\mathbf{P}_1$ であり、章 VI, § 3, no. 3、写像からの直線 (次のようにみなされる) $\mathbf{P}_1$の点)の傾きは、$\tilde{\mathbf{R}}$に対する$\mathbf{P}_1$の準同型写像です。 ここで、写像 $\theta_0 \to \tan\,\theta_0$ によって $\mathfrak{A}_0$ の群構造を $\tilde{\mathbf{R}}$ に移すと、$\tilde{\mathbf{R}}$ で、$t_1, t_2$ が $\mathbf{R}$ と $t_1 t_2 \neq 1$ に属する場合、2 つの要素 $t_1, t_2$ の積が $\frac{t_1 + t_2}{1 - t_1 t_2}$ となるアーベル位相群の構造を定義したことになります。これらの条件を満たさないペア$(t_1, t_2)$の場合、$t_1$と$t_2$の積は、関数$\frac{x + y}{1 - xy}$を$\tilde{\mathbf{R}} \times \tilde{\mathbf{R}}$まで連続的に拡張することで得られ、引き続き$\frac{t_1 + t_2}{1 - t_1 t_2}$で表されます。

### 練習問題 {#top-viii-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
