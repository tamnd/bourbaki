---
book: int
book_title: Integration
chapter: III
chapter_title: MEASURES ON LOCALLY COMPACT SPACES
section: 3
section_title: Integrals of continuous vector-valued functions
lang: ja
source: int-i-vi
book_pages: INT III.32-INT III.40, INT III.60
pdf_pages: 0077-0085, 0105-0105
extraction: ocr
subsections:
    - "no": 1
      title: Definition of the integral of a vector-valued function
      page: 32
      pdf_page: 77
    - "no": 2
      title: Properties of the vectorial integral
      page: 34
      pdf_page: 79
    - "no": 3
      title: Criteria for the integral to belong to $E$
      page: 37
      pdf_page: 82
    - "no": 4
      title: Continuity properties of the integral
      page: 39
      pdf_page: 84
statements: 17
exercises: 4
content_sha256: d1255a4873e4839cb79c98563b8d333bd8f568dfcef2d90b8dfea0882d04c104
translated_from: content/en/int/III/03_s3_integrals_of_continuous_vector_valued.md
translation_method: google
source_content_sha256: fe78ffc7611951df252f5590889a4a16218a67a71377a0b79b5c7914e9bc3371
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: dcfdb067acfb5e608ed295619461df34eeb02cc653d96fc5b750293097f805f9
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 3。連続ベクトル値の積分写像

*この切断を通して、Xは局所的にコンパクトな空間、Eは$\mathbf{R}$または$\mathbf{C}$上で局所的に凸な空間を表します。 E の双対 (E 上の連続線型形式の空間) を $E'$ で表し、$E'$ の代数双対 ($E'$ 上のすべての線型形式の空間) を ${E'}^*$ で表します。 $z \in E$、$z' \in E'$、${z'}^* \in {E'}^*$ の場合は、$\langle z, z' \rangle = z'(z)$、$\langle {z'}^*, z' \rangle = {z'}^*(z')$ と書きます。

E がハウスドルフである場合、E は、$E'$ で線型形式 $z' \mapsto \langle z, z' \rangle$ を伴う元 $z \in E$ を識別することによって、${E'}^*$ の線形部分空間で識別され、${E'}^*$ は弱い位相を備えていることを思い出してください。 $\sigma({E'}^*, E')$ は、弱体化された位相 $\sigma(E, E')$ を装備した E の完成と標準的に識別される可能性があります。

### 1. ベクトル値写像の積分の定義

E への X の写像 f は、すべての $z' \in E'$、X 写像 $x \mapsto \langle f(x), z' \rangle$ が $\mathbf{C}$ になる場合 (他の語写像 $z' \circ f$、 $\langle f, z' \rangle$ とも表されます) は連続です。すべての $z' \in E'$ に対して、写像 $x \mapsto \langle f(x), z' \rangle$ がコンパクト サポートを持っている場合、X の E への写像 f は *スカラー的にコンパクト サポート* であると言えます。 X の写像の $\widetilde{\mathscr{K}}(X; E)$ 空間を *弱連続でスカラー的にコンパクトなサポート* とする E を表します。 $\widetilde{\mathscr{K}}(X; E) \supset \mathscr{K}(X; E)$ であることは明らかですが、これら 2 つの空間は必ずしも同一ではありません (以下の *例* 2 を参照)。ただし、E が有限次元の場合は等しくなります。

弱連続である写像の定義では(コンパクトサポートのスカラー的に)、Eの位相はEの双対$E'$の仲介を通じてのみ介入することに注意してください。したがって、これらの写像のうち集合は、E の位相が双対が同じである局所的に凸な位相に置き換えられても変更されません。

E と F が双対性において 2 つのベクトル空間である場合、E への X の写像が $\sigma(E, F)$ に対して *連続* であると言うのと、それが *弱連続 * であると言うのは同じ意味であることに注意します。

$f$ を $X$ から $E$ への写像とし、弱連続でコンパクトなサポートのスカラーとし、$\mu$ を $X$ のメジャーとします。 $z' \in E'$ ごとに $z' \circ f \in \mathscr{K}(X)$ があります。 集合

$$
\varphi(z') = \int \langle f(x), z' \rangle d\mu(x) = \mu(z' \circ f).
$$

$\varphi$ が $E'$ の線型形式であることは明らかであり、したがって ${E'}^*$* の *元です。

#### 定義 1 {#int-iii-s3-def-1 .statement tag=08NN}

*すべての写像 $f \in \widetilde{\mathscr{K}}(X;E)$ について、$\mu$ に関する $f$ の積分を呼び、* で定義される ${E'}^*$ の $\int f d\mu$ または $\int f(x) d\mu(x)$、または $\int f \mu$、または $\int f(x)\mu(x)$、元で表します。

$$
\left\langle \int f d\mu, z' \right\rangle = \int \langle f, z' \rangle d\mu \quad \text{for all } z' \in E'.
$$

たとえ$E$が*ハウスドルフ*であり$f \in \mathscr{K}(X;E)$であっても、*どちらかが必ずしも$\int f d\mu \in E$を持っているわけではない*ことに注意してください(Exer. 1; cf. No. 3)。

#### 例 {#int-iii-s3-n1-exa-1 .statement tag=08NO}

— 1) $E$ が $\mathbf{C}$ およびハウスドルフ上で *有限次元* であると仮定します。したがって、$(e_i)_{1 \leq i \leq n}$ が $E$ の基底である場合、写像

$$
(\xi_1, \ldots \xi_n) \mapsto \sum_{i=1}^n \xi_i e_i
$$

$E$ に対する $\mathbf{C}^n$ の *同型* です。次に、$E$ 上のすべての線型形式は連続であり、他の語では、$E'$ が $E$ の代数双対 $E^*$ と同一であり、${E'}^*$ が$E$ と正準的に同一化できることがわかります。 $(e'_i)_{1 \leq i \leq n}$ を $E'$ と $(e_i)$ の双対である基底とします。 $X$ から $E$ への写像 $f$ がコンパクト サポートの弱連続かつスカラーであるためには、写像 $f_i = e'_i \circ f$ がコンパクト サポートで連続であることが必要かつ十分です。すべての $x \in X$ に対して $f(x) = \sum_{i=1}^n f_i(x) e_i$ が得られ、

$$
\int f d\mu = \sum_{i=1}^n \mu(f_i) e_i.
$$

2) *漠然と* 位相 (§ 1, No. 9) を装備して、$X$ の$E$ 空間 $\mathscr{M}(X; \mathbf{C})$ を実行しましょう。 $E$ の二重 $E'$ は、空間 $\mathscr{K}(X; \mathbf{C})$ で正規に識別される可能性があります (TVS、II, § 6, No. 2、提案 3)。 $X$ の $E$ への写像 $x \mapsto \varepsilon_x$ は *連続* (§ 1, No. 9、提案 13) ですが、$X$ がコンパクトでない場合、そのサポートはコンパクトではありません。ただし、すべての写像 $f \in E'$ 写像 $x \mapsto \langle \varepsilon_x, f \rangle = f(x)$ には定義がコンパクト サポートを備えているため、これは *スカラー的にコンパクト* サポートです。さらに、

$$
\int \langle \varepsilon_x, f \rangle d\mu = \int f(x) d\mu(x) = \langle \mu, f \rangle
$$

写像 $f \in \mathscr{K}(X; \mathbf{C}) = E'$ ごとに、次のことが証明されます。

$$
\int \varepsilon_x d\mu(x) = \mu
$$

$X$ のすべての小節 $\mu$ に対して。

3) $E$ がハウスドルフである場合、すべての点 $y \in X$ とすべての写像 $f \in \widetilde{\mathscr{K}}(X; E)$ について、次のようになります。

$$
\int f d\varepsilon_y = f(y)
$$

なぜなら$\int \langle f, z' \rangle d\varepsilon_y = \langle f(y), z' \rangle$ by 定義だからです。

#### 注意 1 {#int-iii-s3-n1-rem-1 .statement tag=08NP}

$E$ が局所凸空間で、$N$ が $E$ の $\{0\}$ の閉包である場合、$E_1 = E/N$ が $E$ に関連付けられたハウスドルフ局所凸空間である場合、双対 $E'$ がと $E'_1$ は同一です。 写像 $f$ ～ 属する ～ $\widetilde{\mathscr{K}}(X; E)$ の場合、$f_1 = \pi \circ f$ ($\pi : E \to E_1$ は標準準同型) 属する ～ $\widetilde{\mathscr{K}}(X; E_1)$、この場合は $\int f d\mu = \int f_1 d\mu$ であることが必要十分です。したがって、私たちは極限局所的に凸な *Hausdorff* のみを考慮することができます空間。

#### 注意 2 {#int-iii-s3-n1-rem-2 .statement tag=08NQ}

$E$ を局所凸空間 *over* $\mathbf{C}$ とし、$E_0$ を局所凸空間 *over* $\mathbf{R}$ の基礎となる $E$ とします。 写像 $z' \mapsto \Re z'$ は、$E$ 上のすべての連続 (複素数) 線型形式 $z'$ に対して、$E_0$ 上の連続 (実数) 線型形式 $z \mapsto \Re \langle z, z' \rangle$ となる対応するが双対の $\mathbf{R}$ 同型であることがわかっています。 $E'$ を $E_0$ のデュアル $E'_0$ (TVS、II, §8, No. 1) に接続します。同様に、実数ベクトル空間$E'_0$の代数双対$E'_0*$は、$E'$の代数双対$E'*$の基礎となる実数空間と正準的に同一視される可能性があります。したがって、$\mu$ が *実際の尺度* であり、$\widetilde{\mathscr{K}}(X; E)$ で $f$ 写像である場合、$f$ が $E_0$ でその値を取り、正規の双線形形式を計算すると、公式 (1) が再び有効になります。 2 つのメンバーは、それぞれ、最初のメンバーについては $E'_0$ と $E'_0*$ の間の双対性、および 2 番目のメンバーについては $E_0$ と $E'_0$ の間の双対性と相対的に存在します。

### 2. ベクトル積分の性質

#### 命題 1 {#int-iii-s3-prop-1 .statement tag=08NR}

— *写像*

$$
(f, \mu) \mapsto \int f d\mu
$$

$\widetilde{\mathscr{K}}(X; E) \times \mathscr{M}(X; \mathbf{C})$ から $E'*$ は *双線形* です。

命題はDefからすぐに続きます。 No. 1 の 1 つ。

$u$ を、局所的に凸な空間 $F$ への $E$ の連続線形写像とする。 転置 $^t u$ は $F$ の双対 $F'$ の線形写像を $E$ の双対 $E'$ に変換したものであることがわかります。 (代数的な意味で) $^t u$ の $^{tt} u$ 写像 ${E'}^* \to {F'}^*$、転置で表すことにします。 $E$ と $F$ がハウスドルフであり、正規的にそれぞれ ${E'}^*$ と ${F'}^*$ の部分空間と識別される場合、$^{tt} u$ 拡大する写像 $u$。これら記法:

#### 命題 2 {#int-iii-s3-prop-2 .statement tag=08NS}

— $u$ を、局所的に凸な空間 $F$ への $E$ の連続線形写像とする。 写像 $f \in \widetilde{\mathscr{K}}(X;E)$、写像 $u \circ f$ 属する ～ $\widetilde{\mathscr{K}}(X;F)$ ごとに、

$$
\int u(f(x))\, d\mu(x) = ^{tt} u \left( \int f(x)\, d\mu(x) \right).
$$

連続するすべての線型形式 $z' \in F'$ について、設定 $y' = z' \circ u = {}^t u(z') \in E'$、よっての最初の主張には $z' \circ u \circ f = y' \circ f$ があります。さらに、$z' \in F'$ 全員にとって、

$$
\left\langle \int (u \circ f)\, d\mu, z' \right\rangle = \int \langle u \circ f, z' \rangle\, d\mu = \int \langle f, {}^t u(z') \rangle\, d\mu \\
= \left\langle \int f\, d\mu, {}^t u(z') \right\rangle = \left\langle {}^{tt} u \left( \int f\, d\mu \right), z' \right\rangle,
$$

よって公式 (2)。

#### 命題 3 {#int-iii-s3-prop-3 .statement tag=08NT}

— 写像 $g \in \mathscr{C}(X;\mathbf{C})$ および写像 $f \in \widetilde{\mathscr{K}}(X;E)$、写像 $gf$ 属するから $\widetilde{\mathscr{K}}(X;E)$ ごと、および

$$
\int f\, d(g \cdot \mu) = \int fg\, d\mu.
$$

実際、$z' \in E'$、$\langle gf, z' \rangle = g \langle f, z' \rangle$、よってごとに最初の主張が発生します。さらに、

$$
\left\langle \int f\, d(g \cdot \mu), z' \right\rangle = \int \langle f, z' \rangle\, d(g \cdot \mu) = \int g \langle f, z' \rangle\, d\mu \\
= \int \langle gf, z' \rangle\, d\mu = \left\langle \int gf\, d\mu, z' \right\rangle,
$$

よって (3)。

#### 命題 4 {#int-iii-s3-prop-4 .statement tag=08NU}

— $\mu$ を $X$ 、$S$ のサポート、および $\widetilde{\mathscr{K}}(X;E)$ の $f$ 写像に対する前向きの尺度とします。 $E$ がハウスドルフで、空間 ${E'}^*$ に弱い位相 $\sigma({E'}^*, E')$ を装備するとします。

(i) f(S) によって生成された凸円錐の *整* $\int f\, d\mu$ *属するから閉包* C *in* E'** まで。

(ii) *もし* $\mu$ *が有界であれば、整* $\int f\, d\mu$ *属するから集合* $\| \mu \| \cdot D$、*ここで* D *は* f(S) *in* E'**の閉じた凸包絡線です。

E が複素数の場合、E にその基礎となる *real* ベクトル空間構造を装備しますが、これまで見てきたように、これは公式 (1) を変更しません。

(i) C は、含む f(S) である E'** の閉じた半空間の共通部分であり、0 までの閉じた超平面移行によって決定されることがわかります。したがって、$z' \in E'$ について、すべての $x \in S$ について関係 $\langle f(x), z' \rangle \geq 0$ が意味することを証明すれば十分です。

$$
\left\langle \int f\, d\mu, z' \right\rangle \geq 0;
$$

しかしそれ以来

$$
\left\langle \int f\, d\mu, z' \right\rangle = \int \langle f, z' \rangle\, d\mu,
$$

これは、§2, No. 3、Cor からの続きです。提案 8 の 2。

(ii) D は、含む f(S) である E'** の閉じた半空間の共通部分であることがわかります。したがって、$z' \in E'$ について、すべての $x \in S$ について関係 $\langle f(x), z' \rangle \leq a$ が意味することを示すだけで十分です。

$$
\left\langle \int f\, d\mu, z' \right\rangle \leq a \| \mu \|;
$$

しかし、これは§2, No. 3、Cor.提案 8 の 3。

#### 系 {#int-iii-s3-n2-cor-1 .statement tag=08NV}

*$\mu$ *を* X、$f$ *写像所属から* $\mathscr{K}(X;E)$、*および* D * f(X) *in* E'**の*閉じた凸包絡線とする。 *数* $a > 0$ *そのような* $\int f\, d\mu \in a \cdot D$ が存在します。

*もし* $\nu$ *が X に関する何らかのメジャーである場合、 *数* $a_1, a_2, a_3, a_4 > 0$ *そのような* $\int f\, d\nu \in a_1 D - a_2 D + i a_3 D - i a_4 D$ が存在します。

まず、$\mu$ が正であると仮定します。 仮定により、f のサポート K はコンパクトになります。 $\nu$ が K の比較的コンパクトな開いた近傍に対する $\mu$ の制限である場合、$\nu$ は有界であり、$\int f\, d\mu = \int f\, d\nu \in \| \nu \| \cdot D$ は提案 4 (ii) によって制限されます。 2 番目の結果は、複雑なメジャーは $\mu_j$ が正の $\mu_1 - \mu_2 + i \mu_3 - i \mu_4$ として記述できるため、これから得られます。

#### 命題 5 {#int-iii-s3-prop-5 .statement tag=08NW}

*空間* X * がコンパクトで、* f * を * X * ハウスドルフ局所凸空間* E への連続写像とする* f(X) *in* E'** *(for* $\sigma(E', E')$) *はベクトル* $\int f\, d\mu$ *すべての積極的な措置* $\mu$ * に* X * 総質量* 1 の集合に等しい。

C を E'** の f(X) の閉じた凸包絡線とします。 f(X) はコンパクトであり、E'** は *完全* であるため、C はコンパクトです。私たちはすでに知っています (提案 4) は、1 に等しい総質量の $X$ に対する正の測度の凸型集合 $H$ に対して、すべての測度 $\mu$ 所属に対して $\int f d\mu \in C$ が成り立ちます。一方、曖昧な位相に対して、$H$ は凸で *コンパクト* です。 (§ 1, No. 9、提案 15 の Cor. 3) であり、質量 1 と *有限* サポートの正の測度の凸集合 $H_0$ の閉包 (この位相) です (§ 2, No. 4、Th. 1 の Cor. 3)。さて、写像 $\mu \mapsto \int f d\mu$ の下の $H_0$ の像は、${E'}^*$ の $f(X)$ の凸包絡線 $C_0$ です。一方、この写像は$\langle \int f d\mu, z' \rangle = \int \langle f, z' \rangle d\mu$から定義まで$\mathscr{M}(X; C)$の曖昧な位相と${E'}^*$の位相$\sigma({E'}^*, E')$に対して連続しています。したがって、$H = \overline{H_0}$の像は*コンパクトな*凸型集合含む$C_0$であり、$C$に含まれます。 $C = \overline{C_0}$ 以降、この像は $C$ と等しくなります。

#### 命題 6 {#int-iii-s3-prop-6 .statement tag=08NX}

*$X$ のコンパクトなサポート $f$ を含むすべての連続写像を局所凸ハウスドルフ空間 $E$ に、$E$ のすべての連続半ノルム $q$ と、$X$ のすべての小節 $\mu$ について、 $\int f d\mu \in E$、*

$$
q \left( \int f d\mu \right) \leq \int (q \circ f) \ d|\mu|.
$$

$D$ を $z \in E$ の集合として、$q(z) \leq 1$ とします。 $D$ は閉じており、凸であり、含む 0 であるため、$D = D^{o o}$ (TVS、II, § 6, No. 3、Th. 1 の Cor. 3)。したがって、$z' \in D^o$ ごとに、

$$
\left| \left\langle \int f d\mu, z' \right\rangle \right| \leq \int (q \circ f) \ d|\mu|;
$$

それ以来

$$
\left\langle \int f d\mu, z' \right\rangle = \int \langle f, z' \rangle d\mu,
$$

そしてそれ以来、$D^o$の定義までに、

$$
|\langle f(x), z' \rangle| \leq q(f(x))
$$

すべての $x \in X$ について、望ましい不等式は § 1, No. 6 の不等式 (13) から続きます。

### 3. 属する ～ $E$ までの積分の基準

#### 命題 7 {#int-iii-s3-prop-7 .statement tag=08NY}

*$E$を局所凸ハウスドルフ空間、$f \in \mathscr{K}(X; E)$とする。 $E$ の完全な凸部分集合 $A$ に $f(X)$ が含まれる場合、$\int f d\mu \in E$。*

K を f のサポートとし、仮定によってコンパクトになります。 f は X − K 上の零であるため、f(X) は f(K) または f(K) ∪ {0} に等しいため、f が連続で E がハウスドルフであるためコンパクトです。 E の f(X) の閉じた凸包絡線 C は、(E の包絡線によって誘導される一様構造の場合) 事前圧縮されます (TVS、II, §4, No. 1、提案 3)。しかし、C は完全な空間 A の閉じた部分集合であるため、C は完全であり、したがってコンパクトです。 なおさら、C は、弱化された位相 σ(E, E') に対してコンパクトです。しかし、位相は σ(E'*, E') によって誘導されるため、C は位相 σ(E'*, E') の E'* における f(X) の閉じた凸包絡線です。したがって、証明は、No. 2の提案4の系によって締結されます。

#### 系 1 {#int-iii-s3-prop-7-cor-1 .statement tag=08NZ}

— E を局所凸ハウスドルフ空間とします。 E の完了 $\widehat{E}$ まで、写像 f ∈ $\mathscr{K}(X; E)$、$\int f d\mu$ 属するごとに。

E と $\widehat{E}$ の双対は同一であるため、f が $\widehat{E}$ でその値を取るものとみなしながら、提案 7 を適用するだけで十分です。

#### 系 2 {#int-iii-s3-prop-7-cor-2 .statement tag=08O0}

— E が局所凸空間の準完全ハウスドルフである場合、写像 f ∈ $\mathscr{K}(X; E)$ ごとに $\int f d\mu \in E$ になります。

提案 7 の証明の冒頭で述べたように、f(X) はコンパクトであり、E のその閉じた凸包絡線 C はプレコンパクトであるため、有界です。しかし、集合 C は閉じていて有界であるため、仮定までに完了し、提案 7 を適用するだけで十分です。

第 3 章で見てみましょう。 VI, §1, No. 2、$\int f d\mu$ から属するまでのその他の基準は、$\mathscr{K}(X; E)$ の基準だけでなく、$\widetilde{\mathscr{K}}(X; E)$ の写像に特に適用されます。

系 2 of 命題 7 は、次の 2 つの場合に適用されます。
東経 1 度はバナッハ空間です。 2° E はバレル型ハウスドルフ局所凸型空間 G の双対であり、E は $\mathscr{S}$ トポロジーを備えています。ここで、$\mathscr{S}$ は有界の部分集合による G のカバーです (TVS、III, §4, No. 2、Th. 1 の Cor. 4)。たとえば、Cor.提案 7 の 2 は、E がバナッハ空間の弱いデュアル、または曖昧な位相を備えた対策 $\mathscr{M}(Y; \mathbf{C})$ の空間である場合に適用できます。

X = $\mathbf{R}$、$\mu$ が$\mathbf{R}$ のルベーグ測度、E がバナハ空間である場合、$\mathscr{K}(X; E)$ の写像の積分$\int f d\mu$ は積分にほかなりません。

$$
\int_{-\infty}^{+\infty} f(x)\, dx
$$

FRV で定義、II, §2, No. 1;これは、公式 (1) から、および FRV、I, §1, No. 2、Cor から続きます。提案 2 の。

### 4. 積分の連続特性

#### 命題 8 {#int-iii-s3-prop-8 .statement tag=08O1}

— E がハウスドルフであると仮定します。 $\mu$ を X のメジャーとします。 The mapping $f \mapsto \int f d\mu$ of $\mathscr{K}(X;E)$ into $\widehat{E}$ (No. 3, Cor. 1 of Prop. 7) is the unique continuous linear mapping $\Phi$ such that $\Phi(g \cdot a) = \mu(g) \cdot a$ for every vector $a \in E$ and every function $g \in \mathscr{K}(X;\mathbf{C})$.

写像 $f \mapsto \int f d\mu$ の連続性を証明するには、その制限から $\mathscr{K}(X,K;E)$ が X のすべてのコンパクト部分集合 K に対して連続であることを示すだけで十分です (TVS、II, §4, No. 4、提案 5)。 E の位相が半規範 $(q_\alpha)$ の族によって定義される場合、$\mathscr{K}(X,K;E)$ は半規範の族によって定義されることに注意してください。

$$
p_\alpha(f) = \sup_{x \in K} q_\alpha(f(x)) .
$$

ここで、$h$ を、X から $[0,1]$ への連続した写像とし、コンパクトなサポートと K 上の $h(x) = 1$ を使用します。 No. 2、提案 6 により、すべての写像 $f \in \mathscr{K}(X,K;E)$ に対して、

$$
q_\alpha \left( \int f d\mu \right) = q_\alpha \left( \int h f d\mu \right) \leq \int h(x) q_\alpha(f(x)) d|\mu|(x) \leq |\mu|(h) \cdot p_\alpha(f)
$$

($q_\alpha$ は連続性によって $\widehat{E}$ に拡張されます)、これは $f \mapsto \int f d\mu$ の連続性を証明します。一方、主張の記法では、

$$
\int (g(x) \cdot a) d\mu(x) = \mu(g) \cdot a
$$

No. 1、例 1 およびNo. 2 の提案 2 により、標準単射 $\mathbf{C} \cdot a \to E$ に適用されます。さらに、$a_i \in E$と$g_i \in \mathscr{K}(X;\mathbf{C})$が線形結合$\sum_i g_i \cdot a_i$によって形成される$\mathscr{K}(X;E)$の部分空間が$\mathscr{K}(X;E)$に密集しており（§1, No. 2、提案5）、証明が完成します。

#### 命題 9 {#int-iii-s3-prop-9 .statement tag=08O2}

— E がハウスドルフであると仮定します。 $f$ を、コンパクトなサポートを備えた E への X の連続する写像とします。 空間 $\mathscr{M}(X;\mathbf{C})$ に厳密にコンパクトな収束 (§1, No. 10) の位相が装備されている場合、$\mathscr{M}(X;\mathbf{C})$ から $\widehat{E}$ への写像 $\mu \mapsto \int f d\mu$ は、すべての$\Psi(\varepsilon_x) = f(x)$ となるような固有の連続線形写像 $\Psi$ になります。 $x \in X$。

$z' \in E'$ ごとに、

$$
\left\langle \int f d\varepsilon_x, z' \right\rangle = \int (z' \circ f) d\varepsilon_x = z'(f(x)) = \langle f(x), z' \rangle ,
$$

よって $\int f\, d\varepsilon_x = f(x)$。 We know, moreover, that the set of point measures is total in $\mathscr{M}(X; \mathbf{C})$ for the topology of strictly compact convergence (§ 2, No. 4, Cor. 4 of Th. 1). したがって、すべては証明線形写像 $u : \mu \mapsto \int f\, d\mu$ の連続性に帰着します。 For this, consider the linear mapping $v : z' \mapsto \langle f, z' \rangle$ of $E'$ into $\mathscr{K}(X; \mathbf{C})$, and let us show that the image under $v$ of an equicontinuous subset $H$ of $E'$ is contained in a strictly compact subset of $\mathscr{K}(X; \mathbf{C})$. なぜなら、$K$ が $f$ のサポートである場合、$z' \in H$ に対する写像 $\langle f, z' \rangle$ は $K$ に含まれるサポートを持っています。一方、これらの写像形は等連続集合であり、$z'(f(x))$ の各 $x \in X$ 集合は有界です。したがって、私たちの主張は、アスコリの定理（GT、X, § 2, No. 5、Th.2のCor.3）に続きます。 さて、No. 1の公式(1)から、$u$は(代数的な意味で)転置$^t v$の制限から$\mathscr{M}(X; \mathbf{C})$にほかならないことがわかります。したがって、その連続性は前述のことから得られます (TVS、IV, § 1, No. 3、提案 6)。

#### 系 {#int-iii-s3-n4-cor-1 .statement tag=08O3}

— *With hypotheses and notations as in Prop. 9, the restriction of the mapping* $\mu \mapsto \int f\, d\mu$ *to the set* $\mathscr{M}_+(X)$ *of positive measures, or to a vaguely bounded subset B of* $\mathscr{M}(X; \mathbf{C})$, *is vaguely continuous.*

というのは、§ 1, No. 10、小道具から続きます。図 17 と図 18 から、$\mathscr{M}_+(X)$ または $B$ において、厳密にコンパクトな収束の位相によって引き起こされる位相は、曖昧な位相によって引き起こされる位相と同じであることがわかります。

ただし、曖昧な位相に対して写像 $\mu \mapsto \int f\, d\mu$ は必ずしも $\mathscr{M}(X; \mathbf{C})$ のすべてで連続しているとは限りません (Exer. 2)。

### 練習問題 {#int-iii-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
