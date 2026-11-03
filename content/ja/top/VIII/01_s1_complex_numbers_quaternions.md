---
book: top
book_title: General Topology
chapter: VIII
chapter_title: Complex numbers
section: 1
section_title: Complex numbers, quaternions
lang: ja
source: top-v-x
pdf_pages: 0106-0111, 0129-0131
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF COMPLEX NUMBERS
      page: 0
      pdf_page: 106
    - "no": 2
      title: THE TOPOLOGY OF $\mathbf{C}$
      page: 0
      pdf_page: 108
    - "no": 3
      title: THE MULTIPLICATIVE GROUP $\mathbf{C}^*$
      page: 0
      pdf_page: 109
    - "no": 4
      title: THE DIVISION RING OF QUATERNIONS
      page: 0
      pdf_page: 110
statements: 9
exercises: 5
content_sha256: 8726f6b58fb5016183513b5de922efcc94a79288fee2ac8b1687c0dbec6bd80e
translated_from: content/en/top/VIII/01_s1_complex_numbers_quaternions.md
translation_method: google
source_content_sha256: e5059e22ac4891308f9c35de29452c98d7b526ede462c73990757938a2903d64
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 6cd6351ef7d3955825b48406f1742a8176c0bd16934568cf3a6d759d15f58171
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 1. 複素数、四元数

### 1. 複素数中定義

多項式 $X^2 + 1$ には、すべての $x \in \mathbf{R}$ に対して $x^2 + 1 \geq 1$ があるため、$\mathbf{R}$ には根がありません。 it is therefore irreducible over $\mathbf{R}$. [これは、あらゆる順序体に当てはまる類似の結果の特殊なケースです。]

#### 定義 1 {#top-viii-s1-def-1 .statement tag=0BZV}

*体* $\mathbf{R}[X]/(X^2 + 1)$ *は複素数の体と呼ばれ、* $\mathbf{C}$ で表されます。 *標準像の* $X$ *in* $\mathbf{C}$ *は* $i$で表され、*つまり* $\mathbf{C}$ *は体* $\mathbf{R}$ *代数随伴 of 根* $i$ *of多項式* $X^2 + 1$。 * $\mathbf{C}$ * のうち * 元は複素数* と呼ばれます。

代数的な観点から、点体 $\mathbf{C}$ の重要性は、次の基本的な定理によるものです。

#### 定理 1 {#top-viii-s1-thm-1 .statement tag=0BZW}

（ダランベール＝ガウス）。 *体* $\mathbf{C}$ *of 複素数は代数的に閉じています*。

証明の場合、(i) $\mathbf{R}$ のすべての元 $\geq 0$ が *平方根* を持ち、(ii) $\mathbf{R}$ の係数を含む *奇数* 次数のすべての多項式が * 少なくとも 1 つあることを確立するだけで十分です。 $\mathbf{R}$の根*。これらの最初の主張は、章 IV, § 3, no. 3 ですでに証明されています。 2 番目に関しては、$f(X) = a_0 X^n + a_1 X^{n-1} + \cdots + a_n$ が実数係数を持つ奇数次数 $n$ ($a_0 \neq 0$) の多項式である場合、$x \neq 0$ に対して $f(x) = a_0 x^n g(x)$ と書くことができます。

$$
g(x) = 1 + \frac{a_1}{a_0 x} + \cdots + \frac{a_n}{a_0 x^n}
$$

$x$ が $+\infty$ または $-\infty$ になる傾向があるように、$+1$ になる傾向があります。したがって、数 $a > 0$ があり、$f(a)$ は $a_0$ の符号を持ち、$f(-a)$ は $-a_0$ の符号を持ちます。

したがって、ボルツァーノの定理 (章 IV, § 6, no. 1、定理 2) によれば、$f$ には $[—a, a]$ に少なくとも 1 つの根があります。

#### 注意 1 {#top-viii-s1-n1-rem-1 .statement tag=0BZX}

定理 1 は、体 $\mathbf{C}$ の位相のプロパティを使用することで、順序体の理論を援用せずに証明できます。これは以下で定義されます (no. 2)。 § 2、練習問題 2、および代数位相に特化したこの系列の部分を参照してください。ダランベール-ガウスの定理は、写像の次数の結果の帰結として表示されます。

#### 注意 2 {#top-viii-s1-n1-rem-2 .statement tag=0BZY}

$\mathbf{C}$ は $\mathbf{R}$ 上の次数 2 であるため、$\mathbf{C}$ は同型まで、$\mathbf{R}$ 自体を除く$\mathbf{R}$ の唯一の代数拡大であり、$\mathbf{C}$ には体は含まれないということになります。 $\mathbf{R}$と$\mathbf{C}$以外の含む$\mathbf{R}$。

$\mathbf{R}$ は $\mathbf{C}$ の部分体と識別される可能性があり、すべての $z \in \mathbf{C}$ は形 $x + iy$ で一意に記述できることがわかっています。ここで、$x$ と $y$ は実数です。 $x$ は、$z$ の実数部分と呼ばれ、$\Re(z)$ で表されます。 $y$ $z$ の仮想の部分は、$\Im(z)$ で示されます。 形 $iy$ ($y$ 実数) の複素数は純粋虚数と呼ばれます。 関係 $x + iy = 0$ ($x, y$ 実数) は、$x = 0$ および $y = 0$ と同等です。

$i^2 = -1$, $\mathbf{C}$ の元 (実数と虚数部分で与えられる場合) 満たす以降、次の計算規則になります。

$$
(x + iy) + (x' + iy') = (x + x') + i(y + y')
$$
$$
(x + iy)(x' + iy') = (xx' - yy') + i(xy' + x'y').
$$

特に、$(x + iy)(x - iy) = x^2 + y^2 \in \mathbf{R}$ なので、$x + iy \neq 0$ の場合、

$$
\frac{1}{x + iy} = \frac{x}{x^2 + y^2} - i \frac{y}{x^2 + y^2}.
$$

$\mathbf{C}$ の多項式 $X^2 + 1$ の 2 番目の根は $-i$ です。従って、すべての実数を不変のままにする恒等写像を除く、$\mathbf{C}$ の唯一の自己同型は、写像 $z = x + iy$ から $x - iy$ です。後者は$\overline{z}$で示され、（一般的な定義と一致して）複素数共役から$z$と呼ばれます。私たちは持っています

$$
\Re(z) = \frac{1}{2}(z + \overline{z}) \quad \text{and} \quad \Im(z) = \frac{1}{2i}(z - \overline{z}).
$$

この自己同型の理由により、$f(z)$ が実数係数の多項式である場合、すべての $z \in \mathbf{C}$ に対して $f(\overline{z}) = \overline{f(z)}$ が得られます。

実数 $z \overline{z} = x^2 + y^2$ は、混乱の危険がない場合は、$z$ の代数ノルム、または単にノルムと呼ばれます。それは実数 $\geq 0$ で、$z = 0$ の場合にのみ消えます。 $z$ が実数の場合、$z$ の絶対値値への実数 $\sqrt{z \overline{z}} = \sqrt{x^2 + y^2} \geq 0$ 簡約するを、今でも$z$ の絶対値値と呼び、$z$ が任意の場合、$|z|$ で表します。 複素数。 関係 $|z| = 0$ は $z = 0$ と同等です。 $z$ と $z'$ が 2 つの複素数である場合、$zz'$ の共役は $\overline{zz'}$ であるため、$|zz'|^2 = zz'\overline{zz'} = |z|^2|z'|^2$、従って $|zz'| = |z|\cdot|z'|$: *積の絶対値は次のようになります。 因子の絶対値値の積。* 特に、$z \neq 0$ と $z' = 1/z$ の場合、$|1/z| = |1/z|$ になります。

最後に、すべての複素数 $z, z'$ に対して、*三角形不等式* が得られます。
$$
|z + z'| \leq |z| + |z'|.
$$

### 2. $\mathbf{C}$の位相

実平面$\mathbf{R}^2$の$\mathbf{C}$上への写像$(x, y) \to x + iy$は*全単射*です。これにより、全単射は *輸送* から $\mathbf{R}^2$ の $\mathbf{C}$ 位相 (cf. 章 VI, § 1, no. 5) になります。したがって、$\mathbf{C}$ で定義された位相は、$\mathbf{C}$ (章 VI, § 1, no. 5) の環構造と互換性があるため、$\mathbf{C}$ (章 III, § 6, no. 7) の体構造と *互換性* があります。 (3)、$1/z$は$\mathbf{C}$の0の補数$\mathbf{C}^*$で連続です。

集合 $\mathbf{C}$ にこの位相と、前に定義した体構造 (no. 1, 定義 1) を与えると、*トポロジカル体* (章) の $\mathbf{C}$ 構造を定義したことになります。 III, § 6, no. 7);私たちが$\mathbf{C}$の位相について話すとき、それは常に上記の位相を意味します。

将来的には、位相空間としてみなされる集合 $\mathbf{C}$ と $\mathbf{R}^2$ を一般に *識別* することになります。 $\mathbf{C}$ のサブフィールド $\mathbf{R}$ は、$\mathbf{R}^2$ の横座標で識別されます。このため、これは *実軸* と呼ばれます。同様に、縦軸は *虚数軸* と呼ばれます (これは $\mathbf{C}$ のサブフィールドでは *ないことに注意してください)。 原点 0 と方向比 $(1, 0)$ ($\mathbf{R}_+$ で識別) を持つ光線は、*正の実半軸*と呼ばれます。同じ原点と方向の比率$(-1, 0)$を持つ反対の光線は、*負の実半軸*と呼ばれます。

図解の目的で、$\mathbf{R}^2$ (初等解析幾何学でよく知られている) の表現と、$\mathbf{C}$ の実軸と虚軸をそれぞれ表す 2 つの直交する座標軸が描かれた平面の点を使用します (図 7)。

すべてのトポロジー 体と同様に、複素数係数をもつ$n$ 複素変数のすべての *有理数写像* は、分母が消えない $\mathbf{C}^n$ のすべての点で *連続* です。

![図式は x と y というラベルの付いた軸を持つ複素平面を示し、 点は z = x + iy というラベルが付いています。](https://i.imgur.com/3Q5z5QG.png)

図7。

$\mathbf{C}$ の置換 $z \to \overline{z}$ は連続であるため、トポロジカル体 $\mathbf{C}$ の自己同型です。

実際、それは位相体 $\mathbf{C}$ のうち、同一性自己同型を除く唯一の自己同型です (練習問題 4 を参照)。

写像 $\Re(z), \Im(z)$ は、$\mathbf{R}^2$ の射影をその因子に加えたものであり、したがって連続しています。 $\mathbf{R}^2$ の点 $(x, y)$ のユークリッドノルム (章 VI, § 2, no. 1) であるため、絶対値値 $|z|$ にも同じことが当てはまります。

絶対的な値の性質は、$\mathbf{C}$ の位相がその体構造 (cf. 章 IX, § 3, no. 2) と互換性があるという事実の他の証明につながります。 $z + z'$ の連続性は三角形不等式 $|z + z'| \leq |z| + |z'|$ から得られます。 $zz'$ のそれは関係から続きます
$$
|zz' - z_0z'_0| = |z_0(z' - z'_0) + (z - z_0)z'_0 + (z - z_0)(z' - z'_0)| \\
\leq |z_0| \cdot |z' - z'_0| + |z'_0| \cdot |z - z_0| + |z - z_0| \cdot |z' - z'_0|;
$$
最後に、関係から$z^{-1}$の連続性が続きます。
$$
|z_0^{-1} - z^{-1}| = |z|^{-1} \cdot |z - z_0| \cdot |z_0|^{-1}.
$$

### 3. ザ乗法群 $\mathbf{C}^*$

章 III, § 6, no. 7 から、非ゼロ複素数の乗法群 $\mathbf{C}^*$ で誘発された位相は $\mathbf{C}^*$ の群構造と互換性があることがわかります。 $\mathbf{C}^*$ は $\mathbf{C}$ でオープンであるため、$\mathbf{C}^*$ は局所的にコンパクトなトポロジー 群 (章 I, § 9, no. 7, 命題 13) であるため、完全です (乗法均一性に関して; cf. 章 III, § 6, no. 8, 命題 8）。 実数 $> 0$ の乗法群 $\mathbf{R}_+^*$ は、$\mathbf{C}^*$ のクローズド部分群です。 他の部分群は、絶対値 1 の複素数の集合 $\mathbf{U}$ であり、$\mathbf{R}^2$ の単位元円 $S_1$ と同一視され、したがってコンパクトな群です。 さらに：

#### 命題 1 {#top-viii-s1-prop-1 .statement tag=0BZZ}

*トポロジカル群 $\mathbf{C}^*$ は、トポロジカル群 $\mathbf{R}^*$ および $\mathbf{U}$ の積と同型です。*

写像 $z \to \left( |z|, \frac{z}{|z|} \right)$ は $\mathbf{C}^*$ の $\mathbf{R}_+^* \times \mathbf{U}$ (章 VI, § 2, no. 3, 命題 3) への同相写像です。そしてすぐに、それは群構造の同型であることがわかります。

トポロジー 群 $\mathbf{R}_+^*$ は、加法群 $\mathbf{R}$ (章 V, § 4, 定理 1) と同型であることがすでに知られています。したがって、トポロジカル群 $\mathbf{C}^*$ の研究は、§ 2 で検討する $\mathbf{U}$ の研究に縮小されます。

### 4. クォータニオンの除算環

定理 1 から、体 $\mathbf{R}$ は最大順序体であるため、$\mathbf{R}$ 上の有限階数の唯一の非可換除算環は (同型まで) $\mathbf{R}$ 上の四元数の除算環になります。それは $\mathbf{H}$ で示され、実四元数の分割リング (または、混乱を恐れない場合は単に四元数の分割リング) と呼ばれます。 $\mathbf{H}$ は体 $\mathbf{R}$ 上の階数 4 なので、$\mathbf{R}^4$ (章 VI, § 1, no. 5) と同相の $\mathbf{H}$ で定義する位相ができます。 正確に言うと、通常は同一視する $\mathbf{H}$ で、$\mathbf{R}^4$、元 $i, i, j, k$、標準基底、$\mathbf{H}$ はそれぞれベクトル、$e_0, e_1, e_2, e_3$、標準基底、$\mathbf{R}^4$ と識別されます。

$\mathbf{H}$ の標準基底の乗法表は次の式で与えられることを思い出してください。

$$
i^2 = j^2 = k^2 = -1, \quad ij = -ji = k,
jk = -kj = i, \quad ki = -ik = j.
$$

$\mathbf{H}$の位相は、$\mathbf{H}$の環構造（章VI, § 1, no. 5）だけでなく、その割り算環構造とも互換性があります。なぜなら、$x$ がゼロ以外の四元数である場合、$x^{-1}$ の座標は $x$ の座標の有理数写像であり、その分母は消えません。したがって、この位相を備えた割り算環 $\mathbf{H}$ は、非可換位相割り算環です。 $\mathbf{H}$ の四元数 $a + bi$ (実数 $a, b$) 形 a (トポロジカル) 部分体は、体 $\mathbf{C}$ と同型であり、よく識別されます。

したがって、局所的にコンパクトで接続されたトポロジー分割環の 3 番目の例があり、その他は $\mathbf{R}$ と $\mathbf{C}$ です。実際、これら 2 つの特性を持つ唯一の位相分割環がこれらです。

代数から、四元数 $x = x_0 + x_1 i + x_2 j + x_3 k$ の被約ノルムが

$$
N(x) = x_0^2 + x_1^2 + x_2^2 + x_3^2 = ||x||^2
$$

(したがって、ユークリッドの平方 $x$ のノルムです)。以来

$$
N(xy) = N(x)N(y),
$$

したがって、ノルムのすべての四元数の集合は 1 であり、これは球 $S_3$ と同一であり、形はゼロ以外の四元数乗法群 $\mathbf{H}^*$ のコンパクトな部分群です。

#### 命題 2 {#top-viii-s1-prop-2 .statement tag=0C00}

非ゼロ四元数の乗法群 $\mathbf{H}^*$ は、その部分群 $\mathbf{R}_+^*$ および $S_3$ の積と同型の位相位相群です。

すべての四元数 $x / o$ は、$x \cdot z$ として書くことができます。ここで、$z$ はノルム 1 の四元数です。 $H^*$ の $\|xx'\| = \|x\|\cdot\|x'\|$、写像 $x \to (\|x\|, x_1, x_2)$ から $\mathbf{R}_+^* \times S_2$ へは群構造の同型であり、章 VI, § 2, no. 2、命題 2 からは準同型です$H^*$から$\mathbf{R}_+^* \times S_2$へ。

#### 注意 1 {#top-viii-s1-n4-rem-1 .statement tag=0C01}

関係 $\|x + y\| = \|x\| + \|y\|$ と $\|xy\| = \|x\|\cdot\|y\|$ を使用すると、no. 2 の複素数の体と同様に、$\mathbf{R}^4$ の位相が $H$ (cf.) の割り算環構造と互換性があることを直接証明できます。 章 IX, § 3, no. 2）。

#### 注意 2 {#top-viii-s1-n4-rem-2 .statement tag=0C02}

証明されたことから、球体$S_1$と$S_n$は位相と互換性のある群構造を運ぶことができるということになります。 1 と 3 以外の各整数 $n$ について、$S_n$ の位相と互換性のある $S_n$ には群構造が存在しないことがわかります。

#### 注意 3 {#top-viii-s1-n4-rem-3 .statement tag=0C03}

群 $S_2$ のすべての点は $\mathbf{R}^3$ (章 VI, § 2, no. 4、命題 5) と同型の近傍を持ちますが、$S_4$ は局所的に $\mathbf{R}^3$ と同型ではありません。なぜなら、もしそうなら、それは接続されているので (章 VII, § 2, no. 2, 定理 1)、アーベルになりますが、これは当てはまりません。$i$ と $j$ 属するから $S_3$ と $ij \neq ji$ (cf.) であるからです。 章 V, § 3）。

### 練習問題 {#top-viii-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
