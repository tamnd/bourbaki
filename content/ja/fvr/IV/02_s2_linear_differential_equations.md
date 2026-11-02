---
book: fvr
book_title: Functions of a Real Variable
chapter: IV
chapter_title: DIFFERENTIAL EQUATIONS
section: 2
section_title: LINEAR DIFFERENTIAL EQUATIONS
lang: ja
source: fvr-i-vii
book_pages: 177-198, 204-206
pdf_pages: 0192-0213, 0219-0221
extraction: ocr
subsections:
    - "no": 1
      title: EXISTENCE OF INTEGRALS OF A LINEAR DIFFERENTIAL EQUATION
      page: 177
      pdf_page: 192
    - "no": 2
      title: LINEARITY OF THE INTEGRALS OF A LINEAR DIFFERENTIAL EQUATION
      page: 179
      pdf_page: 194
    - "no": 3
      title: INTEGRATING THE INHOMOGENEOUS LINEAR EQUATION
      page: 182
      pdf_page: 197
    - "no": 4
      title: FUNDAMENTAL SYSTEMS OF INTEGRALS OF A LINEAR SYSTEM OF SCALAR DIFFERENTIAL EQUATIONS
      page: 183
      pdf_page: 198
    - "no": 5
      title: ADJOINT EQUATION
      page: 186
      pdf_page: 201
    - "no": 6
      title: LINEAR DIFFERENTIAL EQUATIONS WITH CONSTANT COEFFICIENTS
      page: 188
      pdf_page: 203
    - "no": 7
      title: LINEAR EQUATIONS OF ORDER $n$
      page: 192
      pdf_page: 207
    - "no": 8
      title: LINEAR EQUATIONS OF ORDER $n$ WITH CONSTANT COEFFICIENTS
      page: 194
      pdf_page: 209
    - "no": 9
      title: SYSTEMS OF LINEAR EQUATIONS WITH CONSTANT COEFFICIENTS
      page: 196
      pdf_page: 211
statements: 25
exercises: 10
content_sha256: 7db2cc47dbc08ce9014b4f07d6741439760a5f957be1266e3cfdcd86e9369184
translated_from: content/en/fvr/IV/02_s2_linear_differential_equations.md
translation_method: google
source_content_sha256: bb9011131c235f557b70d1568fb503a2bded76eb3a6bc7fabc1b5db368218573
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: f39d7504f4c54a1effe9e74fbf96c72461cd9d9b45309ed285580a4ba104d764
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 2。線形微分方程式

### 1. 線形微分方程式の積分の存在

E を体 $\mathbf{R}$ 上の完全な正規化空間とし、$\mathbf{R}$ で J 区間を点に減らないものとします。微分方程式は

$$
\frac{d\mathbf{x}}{dt} = \mathbf{f}(t, \mathbf{x})
$$

(1) ここで、$f$ は $J \times E$ で定義されており、すべての $t \in J$ について、写像 $x \mapsto f(t, x)$ が $E$ からそれ自体への *連続アフィン線形写像* [^1] である場合、*線型* 方程式です。 $b(t) = f(t, 0)$ 写像 $x \mapsto f(t, x) - f(t, 0) = f(t, x) - b(t)$ は、$E$ からそれ自体までの連続線形写像になります。今後、この写像を$A(t)$で表し、点$x \in E$の値を$A(t).x$（または単に$A(t)x$）と書きます。したがって、線形微分方程式 (1) は次のように書くことができます。

$$
\frac{dx}{dt} = A(t).x + b(t)
$$

(2)

ここで、$b$ は $J$ から $E$ への写像です。 $b = 0$ のとき、線形微分方程式 (2) は *均質* であると言います。

#### 例 1 {#fvr-iv-s2-n1-exa-1 .statement tag=08CO}

$E$ が有限次元 $n$ $\mathbf{R}$ 1 同一視できる自己準同型 $A(t)$ のとき、*行列* $\left(a_{ij}(t)\right)$ ** $E$ の任意の基底に関して (*Alg.*、 II、p. 343);検討中の$E$の基底に関して、ベクトル$x \in E$とその成分の列行列$(x_j)$を同一視すると、式$A(t).x$は代数の一般規則に適合します（*Alg.*、 II、p. 343、小道具 2)。この場合、式(2)はスカラー微分方程式の系に相当します。

$$
\frac{dx_i}{dt} = \sum_{j=1}^n a_{ij}(t)x_j + b_i(t) \qquad (1 \leq i \leq n).
$$

(3)

#### 例 2 {#fvr-iv-s2-n1-exa-2 .statement tag=08CP}

$G$ を、$\mathbf{R}$ と $a(t)$、$b(t)$、$c(t)$ の 3 つの写像を $J$ から $G$ までの*完全正規化代数* とします。方程式

$$
\frac{dx}{dt} = a(t)x + x b(t) + c(t)
$$

は線形微分方程式です。ここで $A(t)$ は、それ自体に対する $G$ の線形写像 $x \mapsto a(t)x + x b(t)$ です。

For every $t \in J$, $A(t)$ is an element of the set $\mathscr{L}(E)$ of continuous linear maps from $E$ to itself (continuous endomorphisms of $E$); one knows (*Gen. トップ。*、X、p. 298) $\mathscr{L}(E)$ は、*ノルム* $\|U\| = \sup_{\|x\| \leq 1} \|Ux\|$ が体 $\mathbf{R}$ を超える * 完全な標準代数* であり、その $\|UV\| \leq \|U\|\ \|V\|$ です。

*この切断全体を通して、次の条件が満たされていると仮定します。*

a) *写像* $t \mapsto A(t)$ *of* $J$ *into* $\mathscr{L}(E)$ *規制されています*。

b) *写像* $t \mapsto b(t)$ *of* $J$ *into* $E$ *規制されています*。

$E$ が次元 $n$ を持つとき、$\mathscr{L}(E)$ は $\mathbf{R}^{n^2}$ (トポロジー ベクトル空間として) と同型であり、条件 *a*) は、行列 $A(t)$ の元 $a_{ij}(t)$ がそれぞれ a であることを意味します。 *規制* 写像 $J$。

$\|A(t')\mathbf{x} - A(t)\mathbf{x}\| \leq \|A(t') - A(t)\|\|\mathbf{x}\|$、写像から
$$
t \mapsto A(t).\mathbf{x} + \mathbf{b}(t)
$$
$\mathbf{x} \in E$ごとに規制されています。さらに、
$$
\|A(t)\mathbf{x}_1 - A(t)\mathbf{x}_2\| = \|A(t)(\mathbf{x}_1 - \mathbf{x}_2)\| \leq \|A(t)\|\|\mathbf{x}_1 - \mathbf{x}_2\|
$$
$E$ の任意の $t \in J$ と $\mathbf{x}_1, \mathbf{x}_2$ について。他の語では、(2)の右辺は補題の条件、IVの1、p. 165を満たし、$J \times E$の規制された写像$\|A(t)\|$に関してリプシッツです。 帰結 (IV、p. 173、cor. 2):

#### 定理 1 {#fvr-iv-s2-thm-1 .statement tag=08CQ}

*$t \mapsto A(t)$ *を* $J$ *into* $\mathscr{L}(E)$の規制された写像とし、*および* $t \mapsto \mathbf{b}(t)$ *$J$ *into* $E$の規制された写像とします。 *すべての点* $(t_0, \mathbf{x}_0)$ *of* $J \times E$ *一次方程式* (2) *すべての* $J$ *および等しい* $\mathbf{x}_0$ *点* $t_0$ で定義された解を 1 つだけ認めます。

### 2. 線形微分方程式の積分の線形性

Solving a linear differential equation (2) is a linear problem (*Alg.*, II, p. 240); the homogeneous linear equation
$$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x}
$$
is said to be *associated* with the inhomogeneous equation (2); and one knows (*Alg.*, II, p. 241, prop. 14) that if $\mathbf{u}_1$ is an integral of the inhomogeneous equation (2) then every integral of this equation is of the form $\mathbf{u} + \mathbf{u}_1$ where $\mathbf{u}_1$ is a solution of the associated homogeneous equation (4), and conversely. この小節では、最初に *均質* 方程式 (4) の積分を勉強します。

#### 命題 1 {#fvr-iv-s2-prop-1 .statement tag=08CR}

*集合* $\mathscr{I}$ *同次一次方程式の積分* (4)、*$J$ で定義*、*は空間* $C(J; E)$ の *$J$ *から* $E$ への連続写像のベクトル部分空間です。

証明は明らかです。

#### 定理 2 {#fvr-iv-s2-thm-2 .statement tag=08CS}

*すべての点* $(t_0, \mathbf{x}_0)$ * $J \times E$ * を * $\mathbf{u}(t, t_0, \mathbf{x}_0)$ * 均一方程式の積分* とします* (4) * 上で定義* $J$ * $\mathbf{x}_0$ * $t_0$ に等しい*。
1. *すべての点* $t \in J$ *写像* $\mathbf{x}_0 \mapsto \mathbf{u}(t, t_0, \mathbf{x}_0)$ * は、全単射共連続線形写像* $C(t, t_0)$ *of* $E$ *それ自体に対して*です。
2. *写像* $t \mapsto C(t, t_0)$ *of* $J$ *into* $\mathscr{L}(E)$ *同次線形微分方程式の積分と同じ*
$$
\frac{dU}{dt} = A(t)\ U
$$
*これは値* $I$ **(* $E$ * の同一性写像)* * 点* $t_0$ を必要とします。
3. *点* $s, t, u$ *のうち* $J$
$$
C(s, u) = C(s, t)C(t, u), \qquad C(s, t) = (C(t, s))^{-1}.
$$

プロップにより。 1、$\mathbf{u}(t, t_0, \mathbf{x}_1) + \mathbf{u}(t, t_0, \mathbf{x}_2)$ (それぞれ $\lambda \mathbf{u}(t, t_0, \mathbf{x}_0)$) は (4) の積分で、$t_0$ で値 $\mathbf{x}_1 + \mathbf{x}_2$ (それぞれ $\lambda \mathbf{x}_0$) をとります。 IV、p. 179 の 1 は、$\mathbf{u}(t, t_0, \mathbf{x}_1 + \mathbf{x}_2)$ (それぞれ $\mathbf{u}(t, t_0, \lambda \mathbf{x}_0)$) と同一です。したがって、写像 $\mathbf{x}_0 \mapsto \mathbf{u}(t, t_0, \mathbf{x}_0)$ は E の線形写像 $C(t, t_0)$ であり、$\mathbf{u}(t, t_0, \mathbf{x}_0) = C(t, t_0). \mathbf{x}_0$ と書き込むことができます。

$\mathscr{L}(E) \times \mathscr{L}(E)$ の $\mathscr{L}(E)$ への写像 $(X, Y) \mapsto XY$ は連続しているため (*Gen. Top.*、X、p. 298、prop. 8)、J の $\mathscr{L}(E)$ への写像 $t \mapsto A(t)U$ はすべての $U \in \mathscr{L}(E)$ で規制されています。さらに (*Gen.Top.*、X、p. 296)

$$
\| A(t)X - A(t)Y \| = \| A(t)(X - Y) \| \leq \| A(t) \| \| X - Y \|,
$$

したがって、これを適用できます。 IV、p. 179 のI を同次一次方程式 (5) に代入します。 $V(t)$ を J で定義されたこの方程式の積分とし、$t_0$ における $I$ に等しいものとします。 1 つは (I、p. 6、提案 3) を持っています。

$$
\frac{d}{dt} (V(t)\mathbf{x}_0) = \frac{dV(t)}{dt} \mathbf{x}_0 = A(t)(V(t)\mathbf{x}_0)
$$

$t = t_0$ には $V(t)\mathbf{x}_0 = I\mathbf{x}_0 = \mathbf{x}_0$ があります。までに。 IV、p. 179 の 1 つは、すべての $\mathbf{x}_0 \in E$、つまり $V(t) = C(t, t_0)$ に対して $V(t).\mathbf{x}_0 = C(t, t_0)\mathbf{x}_0$ を持っていなければなりません。これは、$C(t, t_0)$ 属するから $\mathscr{L}(E)$ まで、その他の語では、$\mathbf{x}_0 \mapsto C(t, t_0).\mathbf{x}_0$ が E 上で連続であること、写像 $t \mapsto C(t, t_0)$ が (5) の積分であり、$t_0$ での $I$ に等しいことが証明されます。

最後に、(4) の積分 $s \mapsto C(s, u).\mathbf{x}_0$ は点 $t$ で $C(t, u).\mathbf{x}_0$ に等しいため、定義により、

$$
C(s, u).\mathbf{x}_0 = C(s, t)(C(t, u).\mathbf{x}_0) = (C(s, t)C(t, u)).\mathbf{x}_0
$$

任意の $\mathbf{x}_0 \in E$、よっての場合、最初の関係 (6)。 $C(s, s) = I$ 以降、J の任意の $s$ と $t$ には $C(s, t)C(t, s) = I$ があります。これは (*集合理論*, II, p. 86, 系) $C(t, t_0)$ がそれ自体に対する E の全単射写像であり、逆数写像 $C(t_0, t)$ であることが証明されます。これで定理の証明が完了です。

$C(t, t_0)$ は、IV、p. 178 の方程式 (2) の *分解* であると言われています。

#### 系 1 {#fvr-iv-s2-thm-2-cor-1 .statement tag=08CT}

*J で定義された連続写像 $t \mapsto C(t, t_0).\mathbf{x}_0$ をすべての点 $\mathbf{x}_0 \in E$ に関連付ける写像は、(4) の積分のベクトル空間 $\mathscr{I}$ に標準化された空間 E の同型であり、コンパクトな位相が与えられています。収束*

それは確かに、$\mathscr{I}$ 上の E の全単射線形写像です。今、$C(t, t_0)$ はコンパクトな集合 $K \subset J$ で境界付けられているため、任意の $t \in K$ と $\mathbf{x}_0 \in E$ に対して $\| C(t, t_0).\mathbf{x}_0 \| \leq M \| \mathbf{x}_0 \|$ となり、この写像が連続であることがわかります。そしてそれ以来

$$
C(t_0, t_0).\mathbf{x}_0 = \mathbf{x}_0,
$$

逆数写像も連続であることは明らかです。

#### 系 2 {#fvr-iv-s2-thm-2-cor-2 .statement tag=08CU}

*$J \times J$から$\mathscr{L}(E)$への写像$(s, t) \mapsto C(s, t)$は連続です。*

By (6) we have $C(s, t) = C(s, t_0) \left( C(t, t_0) \right)^{-1}$; now, the map $(X, Y) \mapsto XY$ of $\mathscr{L}(E) \times \mathscr{L}(E)$ into $\mathscr{L}(E)$ is continuous, as is the map $X \mapsto X^{-1}$ of the (open) group of invertible elements of $\mathscr{L}(E)$ onto itself (TG, IX, p. 40, prop. 14).

写像に注目してください。
$$
t \mapsto C(t_0, t) = (C(t, t_0))^{-1}
$$
$-(C(t, t_0))^{-1} (dC(t, t_0)/dt)(C(t, t_0))^{-1}$ (可算集合の補数) (I, p. 8, prop. 4) に等しい導関数、つまり (IV, p. 179, 公式 (5) による) $-C(t_0, t) A(t)$ に等しい導関数を認めます。

#### 系 3 {#fvr-iv-s2-thm-2-cor-3 .statement tag=08CV}

※KをJに含まれるコンパクト区間とし、$k = \sup_{t \in K} \|A(t)\|$とします。 K* のすべての t と $t_0$ について
$$
\|C(t, t_0) - I\| \leq e^{k|t-t_0|} - 1 .
$$ (7)

確かに、すべての $t \in K$ に対して $\|A(t)x_0\| \leq k \|x_0\|$。したがって、K では、$x_0$ に等しい定数写像は、IV、p. 18 の式 (4) によって $k \|x_0\|$ 以内の近似積分になります。 IV、p. 170 の公式 (15) までに、次のようになります。
$$
\|C(t, t_0)x_0 - x_0\| \leq \|x_0\| (e^{k|t-t_0|} - 1)
$$
K の任意の $t$ と $t_0$、および E の $x_0$ に対して、$\mathscr{L}(E)$ のノルムの定義による不等式 (7) と同等です。

#### 命題 2 {#fvr-iv-s2-prop-2 .statement tag=08CW}

*B を E の連続自己準同型とし、t から独立し、すべての $t \in J$ について A(t) と可換であるとします。この場合、B はすべての t に対して $C(t, t_0)$ と、J では $t_0$ で通勤します。

確かに(5)までに
$$
\frac{d}{dt}(BC) = BAC = ABC \quad \text{and} \quad \frac{d}{dt}(CB) = ACB ,
$$
それで $\frac{d}{dt}(BC - CB) = A(BC - CB)$;しかし $BC(t_0, t_0) - C(t_0, t_0)B = 0$ なので、すべての $t \in J$ に対して (IV、p. 179、th. 1) $BC(t, t_0) - C(t, t_0)B = 0$ です。

小道具の重要な例。 2 は、E が複素数* $\mathbf{C}$ の *体に関して標準的なベクトル空間の構造を与えられており、すべての $t \in J$ について、$A(t)$ がこのベクトル空間について E の自己準同型であるということです。 構造;これは、$A(t)$ が E の連続する自己準同型 $x \mapsto tx$ と交換することを意味します (ベクトル空間構造 *over* $\mathbf{R}$)。次に、$C(t, t_0)$ はこの自己準同型と可換です。つまり、J の任意の $t$ と $t_0$ について、写像 $C(t, t_0)$ は、$\mathbf{C}$ にわたる E の正規のベクトル空間構造に対して連続する自己準同型です。

### 3. 不均一一次方程式の積分

不均一一次方程式の積分

$$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x} + \mathbf{b}(t)
$$

簡約する関連する一次方程式を積分する

$$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x}
$$

そしてプリミティブを評価します。の記法と。 IV、p. 179の2つ、IV、p. 179、$\mathbf{z} = C(t_0, t).\mathbf{x}$の2番目の公式から$\mathbf{x} = C(t, t_0).\mathbf{z}$、よってを入れましょう。 $\mathbf{x}$ が (2) の積分である場合、$\mathbf{z}$ は方程式 $\frac{d}{dt}\left(C(t, t_0).\mathbf{z}\right) = A(t)C(t, t_0).\mathbf{z} + \mathbf{b}(t)$ の積分です。双線形写像以降

$$
(U, y) \mapsto U.y
$$

$\mathscr{L}(\mathbf{E}) \times \mathbf{E}$ から $\mathbf{E}$ への変換は連続 (\emph{Gen. Top.}, X, p. 297, prop. 6) し、$\mathbf{z}$ は微分を認めます (J の可算部分集合を除く) し、双線形写像を微分するために公式を使用します。 (I、p. 6、提案 3)

$$
\frac{d}{dt}\left(C(t, t_0).\mathbf{z}\right) = \frac{dC(t, t_0)}{dt}.\mathbf{z} + C(t, t_0).\frac{d\mathbf{z}}{dt} = A(t)C(t, t_0).\mathbf{z} + C(t, t_0).\frac{d\mathbf{z}}{dt}
$$

((5) (IV, p. 179) によると、置き換えること $dC(t, t_0)/dt$ by $A(t)C(t, t_0)$)。 $\mathbf{z}$ から簡約するを$C(t, t_0).d\mathbf{z}/dt = \mathbf{b}(t)$ に、または再度簡約するを計算する等式

$$
\frac{d\mathbf{z}}{dt} = C(t_0, t).\mathbf{b}(t)
$$

IV、p. 179 の 2 番目の公式 (6) まで。 Now the right-hand side of equation (8) is a regulated function on J, having been obtained by substituting the regulated functions $U$ and $y$ in the continuous bilinear function $U.y$ (\emph{cf.} II, p. 55, cor. 2); equation (8) thus has one and only one integral taking the value $\mathbf{x}_0$ at $t_0$, given by the formula

$$
\mathbf{z}(t) = \mathbf{x}_0 + \int_{t_0}^t C(t_0, s).\mathbf{b}(s)\,ds.
$$

$C(t, t_0).\int_{t_0}^t C(t_0, s).\mathbf{b}(s)\,ds = \int_{t_0}^t C(t, t_0)C(t_0, s).\mathbf{b}(s)\,ds$ (II, p. 59, 公式 (9)) があるため、(IV, p. 179 の最初の公式 (6) を考慮して) 次の結果が得られます。

#### 命題 3 {#fvr-iv-s2-prop-3 .statement tag=08CX}

※記法となります。 2* (IV, p. 179)、*すべての点* $(t_0, \mathbf{x}_0)$ *of* $J \times \mathbf{E}$ *一次方程式の積分* (2) *上で定義* $J$ *と等しい* $\mathbf{x}_0$ *at* $t_0$ *は公式* で与えられる

$$
\mathbf{u}(t) = C(t, t_0).\mathbf{x}_0 + \int_{t_0}^t C(t, s).\mathbf{b}(s)\,ds.
$$

写像 $\mathbf{z}$ を新しい未知の写像として取ることで構成される公式 (10) につながる方法は、よく「パラメーターの変化の方法」と呼ばれます。

### 4. スカラー微分方程式の線形系の積分の基礎系

この小節と次のケースでは、E が複素数の体 $\mathbf{C}$ の有限次元のベクトル空間 (つまり、$\mathbf{R}$ の次元 2n) であり、すべての $t \in J$ について、$A(t)$ が$\mathbf{C}$ に対するベクトル空間構造に対する E の自己準同型 。 次に、E の基底に対して (体 $\mathbf{C}$ を超える) 行列 $(a_{ij}(t))$ を使用して同一視する $A(t)$ を実行できます。今回の $a_{ij}$ は、J で定義および規制されている $n^2$ 複合体写像です。 $x_j$ ($1 \leq j \leq n$) を、選択した基底に関するベクトル $x \in E$ の (複素数) 成分を表すとします。一次方程式です。

$$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x} + \mathbf{b}(t)
$$

再び系と同等になります

$$
\frac{dx_i}{dt} = \sum_{j=1}^n a_{ij}(t)x_j + b_i(t) \qquad (1 \leq i \leq n).
$$

定理 1 (IV、p. 179) と 2 (IV、p. 179) およびプロップ。 2 (IV, p. 181) は、E のすべての $\mathbf{x}_0 = (x_{k0})_{1 \leq k \leq n}$ に対して、方程式の積分 $\mathbf{u} = (u_k)_{1 \leq k \leq n}$ が 1 つだけ存在することを示します。

$$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x}
$$

E で定義され、点 $t_0$ で $\mathbf{x}_0$ に等しい。この積分は次のように書くことができます

$$
\mathbf{u}(t, t_0, \mathbf{x}_0) = C(t, t_0).\mathbf{x}_0,
$$

$C(t, t_0)$ は位数 $n$ の可逆平方行列 $(c_{ij}(t, t_0))$ であり、そのエントリは $J \times J$ 上の連続複素数写像であり、$t \mapsto c_{ij}(t, t_0)$ は J 上の規制された写像のプリミティブです。

特定のケースでは、 $n = 1$ 系 (3) 簡約するが 1 つのスカラー方程式に変換されます。

$$
\frac{dx}{dt} = a(t)x + b(t)
$$

$a(t)$ と $b(t)$ は J) で複雑に規制されています写像; (1 つの元) 行列 $C(t, t_0)$ が $\exp \left( \int_{t_0}^t a(s)\, ds \right)$ に等しいことを即座に検証します。したがって、点 $t_0$ における $x_0$ に等しい (11) の積分は、公式によって明示的に与えられます。

$$
u(t) = x_0 \exp \left( \int_{t_0}^t a(s)\, ds \right) + \int_{t_0}^t b(s) \exp \left( \int_{t_0}^\tau a(\tau)\, d\tau \right) ds.
$$

In the space $\mathscr{C}(J; E)$ of continuous maps from J into E, endowed with the topology of compact convergence, the set $\mathscr{I}$ of integrals of equation (4) is a vector subspace (over $\mathbf{C}$) isomorphic to E, therefore to $\mathbf{C}^n$ (IV, p. 180, cor. 1, and IV, p. 181, prop. 2).

この空間 (体 $\mathbf{C}$ 以上) の基底 $(\mathbf{u}_j)_{1 \leq j \leq n}$ を (4) の積分の * 基礎系* と呼びます。

#### 命題 4 {#fvr-iv-s2-prop-4 .statement tag=08CY}

*For the $n$ integrals $\mathbf{u}_j$ ($1 \leq j \leq n$) of equation (4) to form a fundamental system it is necessary and sufficient that their values $\mathbf{u}_j(t_0)$ at a point $t_0 \in J$ be linearly independent vectors in $E$.*

実際、整 $t \mapsto C(t, t_0).\mathbf{x}_0$ をすべての $\mathbf{x}_0 \in E$ に関連付ける写像は、 $E$ の $\mathscr{I}$ 上の同型です (IV、p. 180、cor. 1 および IV、p. 181、prop. 2)。

$(\mathbf{e}_j)_{1 \leq j \leq n}$ が $\mathbf{C}$ 上の $E$ のいずれかの基底である場合、$n$ の積分
$$
\mathbf{u}_j(t) = C(t, t_0).\mathbf{e}_j \qquad (1 \leq j \leq n)
$$
したがって、形は基本的な系です。 基底 $(\mathbf{e}_j)$ に関して$C(t, t_0)$ をその行列と同定すると、整$\mathbf{u}_j$ は正確に行列 $C(t, t_0)$ の *列* になります。 点 $t_0$ で値 $\mathbf{x}_0 = \sum_{j=1}^n \lambda_j \mathbf{e}_j$ を取る (4) の積分は、$C(t, t_0).\mathbf{x}_0 = \sum_{k=1}^n \lambda_k \mathbf{u}_k(t)$ になります。

(4) 1 つの項の *任意の* $n$ 整 $\mathbf{u}_j$ ($1 \leq j \leq n$) と、$E$ の基底 $(\mathbf{e}_j)_{1 \leq j \leq n}$ に関する点 $t \in J$ におけるこれらの $n$ 積分のうちの *行列式* が与えられると、 行列式
$$
\Delta(t) = (\mathbf{u}_1(t), \ \mathbf{u}_2(t), \ \ldots, \ \mathbf{u}_n(t))
$$
基底 $(\mathbf{e}_j)$ に対する $n$ ベクトル $\mathbf{u}_j(t)$ (*Alg.*、III、p. 522)。 1 つは (*Alg.*, III, p. 523, prop. 2) です。
$$
\Delta(t) = \Delta(t_0) \det \left( C(t, t_0) \right).
$$

By prop. 4 of IV, p. 184, for $(\mathbf{u}_j)_{1 \leq j \leq n}$ to be a fundamental system of integrals of (4) it is necessary and sufficient that the determinant $\Delta(t)$ of the $\mathbf{u}_j$ be $\neq 0$ at some one point $t_0$ of $J$; the formula (14) then shows that $\Delta(t) \neq 0$ at every point of $J$, in other words, that the vectors $\mathbf{u}_j(t)$ ($1 \leq j \leq n$) are always linearly independent.

#### 命題 5 {#fvr-iv-s2-prop-5 .statement tag=08CZ}

*行列 $C(t, t_0)$ の行列式は公式* によって与えられます
$$
\det \left( C(t, t_0) \right) = \exp \left( \int_{t_0}^t \operatorname{Tr}(A(s)) \, ds \right).
$$
(15)

確かに、$\delta(t) = \det \left( C(t, t_0) \right)$ を置くと、行列式の導関数は公式になります (I, p. 8, 公式 (3))
$$
\frac{d \delta}{dt} = \operatorname{Tr} \left( \frac{dC(t, t_0)}{dt} (C(t, t_0))^{-1} \right) \delta(t)
$$

つまり、$C(t, t_0)$ によって満たされるIV, p. 179 の微分方程式 (5) により、

$$
\frac{d \delta}{dt} = \operatorname{Tr}(A(t)) \delta(t).
$$

$\delta(t_0) = 1$ 公式 (15) は、スカラー線形方程式の積分の式 (12) (IV, p. 183) から得られます。

先ほど見たように、(4) 決定するこの方程式のすべての積分を $n$ 線形独立積分で指定します。ここで、$1 \leq p \leq n$ について、方程式 (4) の $p$ 線形独立積分 $\mathbf{u}_j$ ($1 \leq j \leq p$) の知識簡約するについて、この方程式の $n - p$ スカラー方程式の同次線形系の知識への積分であることを示します。 区間 $K \subset J$ に $n - p$ 写像があるとします。

$$
\mathbf{u}_{p+k} \quad (1 \leq k \leq n - p)
$$

of $K$ into $E$, which are primitives of regulated functions on $K$, and such that, for every $t \in K$, the $n$ vectors $\mathbf{u}_j(t)$ ($1 \leq j \leq n$) form a basis of $E$.

すべての点 $t_1 \in J$ に対して、$J$ の $t_1$ の区間 $K$、近傍が常に存在し、その上に、前述のプロパティを持つ $n - p$ 写像 $\mathbf{u}_{p+k}$ ($1 \leq k \leq n - p$) が定義されています。 For, let $(\mathbf{e}_i)_{1 \leq i \leq n}$ be a basis of $E$; there exist $n - p$ vectors of this basis which form with the $\mathbf{u}_j(t_1)$ ($1 \leq j \leq p$) a basis of $E$ (Alg., II, p. 292, th. 2); suppose for example that they are $\mathbf{e}_{p+1}, \ldots, \mathbf{e}_n$; since the determinant $\det(\mathbf{u}_1(t), \ldots, \mathbf{u}_p(t), \mathbf{e}_{p+1}, \ldots, \mathbf{e}_n)$ (with respect to the basis $(\mathbf{e}_i)$) is a continuous function of $t$ and does not vanish for $t = t_1$ there exists a neighbourhood $K$ of $t_1$ on which it does not vanish; one can then take $\mathbf{u}_{p+k}(t) = \mathbf{e}_{p+k}$ ($1 \leq k \leq n - p$) for $t \in K$.

位数 $n$ の可逆行列 $B(t)$ が存在します。その元は、$1 \leq j \leq n$ に対して $B(t).\mathbf{e}_j = \mathbf{u}_j(t)$ となるように、$K$ 上の規制された写像のプリミティブです。 $x = B(t).y$ を入れましょう。この場合、$y$ は式 $\frac{dB}{dt}.y + B(t).\frac{dy}{dt} = A(t)B(t).y$ を満たし、次のように書くこともできます。

$$
\frac{dy}{dt} = (B(t))^{-1} \left( A(t)B(t) - \frac{dB}{dt} \right) .y = H(t).y
$$

ここで、$H(t) = (h_{jk}(t))$ は行列で、$K$ に規制されているエントリがあります。 $B(t)$ の定義により、この線形方程式は $p$ 定数ベクトル $\mathbf{e}_j$ ($1 \leq j \leq p$) を積分として認めます。 1 つの結論するはすぐに $1 \leq k \leq p$ に対して必然的に $h_{jk}(t) = 0$ になります。したがって、$y$ の成分 $y_k$ (基底 $(\mathbf{e}_i)$ に関して) 添字 $k \geq p + 1$ 満たすは、$n - p$ 方程式の同次線形系となります。この系の解が決定されると、 添字 $j \leq p$ の $dy_j/dt$ は $y_k$ と $k \geq p + 1$ の線形写像であることがわかり、これらの写像のプリミティブは次のようになります。 $y_j$ は添字 $j \leq p$ です。

特に、IV、p. 183 の方程式 (4) の$n - 1$ 線形独立積分がわかっている場合、この方程式簡約するを単一の同次スカラー方程式のそれに積分し、次に $n$ プリミティブを評価します。

#### 注意 1 {#fvr-iv-s2-n4-rem-1 .statement tag=08D0}

上記のすべては、E が体 $\mathbf{R}$ に対して次元 $n$ であり、$A(t)$ が $t \in J$ ごとに E の自己準同型である場合にも当てはまります。つまり、全体を通して置き換える $\mathbf{C}$ $\mathbf{R}$ を実行するだけで済みます。

#### 注意 2 {#fvr-iv-s2-n4-rem-2 .statement tag=08D1}

$A(t) = (a_{ij}(t))$ を位数 $n$ の平方行列とし、そのエントリは$J$ の $t$ の写像で規制される実数 (または複素数) とし、$C(t, t_0) = (c_{ij}(t, t_0))$ をその解決策行列とします。 対応するリニア系 (3) (IV、p. 22)。 F を $\mathbf{R}$ (それぞれ $\mathbf{C}$) 上の任意の完全ノルム空間とし、線形微分方程式の系を考えてみましょう

$$
\frac{dy_i}{dt} = \sum_{j=1}^n a_{ij}(t) y_j
$$

ここで、未知の写像 $y_j$ は、F でその値をとります。この系の解 $(\mathbf{u}_j)_{1 \leq j \leq n}$ が明らかであり、$1 \leq j \leq n$ ($\mathbf{d}_j$ は F で任意) に対する $\mathbf{u}_j(t_0) = \mathbf{d}_j$ は次の式で与えられます。

$$
\mathbf{u}_i(t) = \sum_{j=1}^n c_{ij}(t, t_0) \mathbf{d}_j \qquad (1 \leq i \leq n).
$$

We consider in particular the case where $A(t)$ is an endomorphism of a vector space E of finite dimension $n$ over $\mathbf{C}$, such that there exists a basis of E with respect to which the matrix of $A(t)$ has real elements for every $t \in J$. Then the above shows (by th. 1 of IV, p. 179) that the resolvent matrix $C(t, t_0)$ with respect to the same basis also has real elements: it suffices to consider the vector space $E_0$ over $\mathbf{R}$ generated by the basis of E under consideration, and to remark that the restriction of $A(t)$ to $E_0$ is an endomorphism of this vector space.

### 5. 随伴方程式

空間 E が $\mathbf{C}$ に対する有限次元 $n$ であると常に仮定し、$E^*$ をその双対 (A、II、p. 40) とします。これは、$\mathbf{C}$ に対する次元 $n$ の空間です。 (Alg.、II、p. 299、th. 4); $E \times E^*$ で定義された正規双線形形式 $\langle \mathbf{x}, \mathbf{x}^* \rangle$ (Alg.、II、p. 234) は、この積上で連続です ($\mathbf{x} \in E$ と $\mathbf{x}^* \in E^*$ の成分の多項式です)。

同次一次方程式 (4) (IV, p. 183) が与えられるとします。ここで、$t \mapsto A(t)$ は J の $\mathscr{L}(E)$ への調整された写像であり、J の $E^*$ への調整された写像のプリミティブである写像 $t \mapsto \mathbf{v}(t)$ が存在するかどうかを見てみましょう。 J、および $\mathbf{u}$ が (4) の任意の解である場合、スカラー 写像 $t \mapsto \langle \mathbf{u}(t), \mathbf{v}(t) \rangle$ が J 上で定数になるようにします。この写像の導関数は、$\mathbf{u}$ と $\mathbf{v}$ が微分可能であるすべての点で零になるはずであると書くのと同じことになります。つまり、

$$
\left\langle \frac{d\mathbf{u}}{dt}, \mathbf{v}(t) \right\rangle + \left\langle \mathbf{u}(t), \frac{d\mathbf{v}}{dt} \right\rangle = 0
$$

そんな点で。

さて、(4) により、$-B(t)$ は $A(t)$ の転置である $\left\langle \frac{d\mathbf{u}}{dt}, \mathbf{v}(t) \right\rangle = \langle A(t).\mathbf{u}(t), \mathbf{v}(t) \rangle = -\langle \mathbf{u}(t), B(t).\mathbf{v}(t) \rangle$ (代数、II、p. 234)。 関係、$\mathbf{v}$ は満たすでなければならないということは、次のように書くことができます

$$
\left\langle \mathbf{u}(t), \frac{d\mathbf{v}}{dt} - B(t).\mathbf{v}(t) \right\rangle = 0
$$

まったく点ここで、$A(t)$ は連続であり、$\mathbf{v}(t)$ は微分可能です。さて、そのような点 $t$ と *任意の* 点 $\mathbf{x}_0 \in \mathrm{E}$ が存在します。 $\mathbf{u}(t) = \mathbf{x}_0$ となる (4) の IV、p. 179、解 $\mathbf{u}$ の 1 つ。従って、*すべて* $\mathbf{x}_0 \in \mathrm{E}$ に対して $\left\langle \mathbf{x}_0, \frac{d\mathbf{v}}{dt} - B(t).\mathbf{v}(t) \right\rangle = 0$ が必要であり、これには $\frac{d\mathbf{v}}{dt} - B(t).\mathbf{v}(t) = 0$ が伴います。その結果：

#### 命題 6 {#fvr-iv-s2-prop-6 .statement tag=08D2}

*J の $\mathrm{E}^*$ への J の写像 $t \mapsto \mathbf{v}(t)$ (J 上の規制された写像のプリミティブ) は、方程式 * (4) のすべての解 $\mathbf{u}$ に対して、$\langle \mathbf{u}(t), \mathbf{v}(t) \rangle$ が J 上で定数になるようなものです* (4) * IV、p. 183 の場合に限り$\mathbf{v}$ は、一次一次方程式*の解です

$$
\frac{d\mathbf{x}}{dt} = B(t).\mathbf{x} \tag{16}
$$

*ここで、$-B(t)$は$A(t)$の転置です。*

式 (16) は、(4) の *随伴* と呼ばれます。明らかに (4) は (16) の随伴です。 The elements of the matrix $B(t)$ being regulated functions of $t$ on J, the results obtained above on linear equations apply to (16). 特に、点 $t_0$ で値 $\mathbf{x}_0^*$ を取る (16) の積分は、$H(t, t_0).\mathbf{x}_0^*$ と書くことができます。ここで、$H(t, t_0)$ は、$\mathrm{E}^*$ の全単射線形写像であり、方程式の積分と同じです。

$$
\frac{dV}{dt} = B(t)V \tag{17}
$$

これには点 $t_0$ で値 $I$ かかります。結果として、1 つは (IV の記法、p. 179) を獲得しました。

$$
\left\langle C(t, t_0).\mathbf{x}_0, H(t, t_0).\mathbf{x}_0^* \right\rangle = \left\langle \mathbf{x}_0, \mathbf{x}_0^* \right\rangle
$$

任意の $\mathbf{x}_0 \in \mathrm{E}$ と $\mathbf{x}_0^* \in \mathrm{E}^*$ について、次のことがわかります。

$$
H(t, t_0) = \check{C}(t, t_0) \tag{18}
$$

($C(t, t_0)$の*逆勾配*)。特に、随伴方程式 (16) の積分の基本的な系がわかっていれば、行列 $H(t, t_0)$ が決定され、$C(t, t_0)$ も決定され、その結果、方程式 (4) の *すべて* の積分も決定されます。

#### 注意 {#fvr-iv-s2-n5-rem-1 .statement tag=08D3}

Let E and F be two complete normed spaces over $\mathbf{R}$ (or over $\mathbf{C}$), and $(\mathbf{x}, \mathbf{y}) \mapsto \langle \mathbf{x}, \mathbf{y} \rangle$ a *continuous* bilinear form on $\mathrm{E} \times \mathrm{F}$, such that the relation “$\langle \mathbf{x}, \mathbf{y} \rangle = 0$ for all $\mathbf{y} \in \mathrm{F}$” (resp. $\langle \mathbf{x}, \mathbf{y} \rangle = 0$ for all $\mathbf{x} \in \mathrm{E}$”) implies $\mathbf{x} = 0$ (resp. $\mathbf{y} = 0$). さらに、すべての $t \in \mathrm{J}$ に対して、それ自体への F の連続線形写像 $B(t)$ が存在し、すべての $(\mathbf{x}, \mathbf{y}) \in \mathrm{E} \times \mathrm{F}$ に対して $\langle A(t).\mathbf{x}, \mathbf{y} \rangle + \langle \mathbf{x}, B(t).\mathbf{y} \rangle = 0$ になると仮定します。 このような状況では、前にのように、規制された写像のプリミティブであるJをFに変換する写像$t \mapsto \mathbf{v}(t)$に関して、$\langle \mathbf{u}(t), \mathbf{v}(t) \rangle$が(4)の*すべての*整$\mathbf{u}$に対して*定数*であるためには、$\mathbf{v}$が(16)の積分であることが必要かつ十分であることがわかります。もう一度、(4) の *随伴* と呼びます。

### 6. 定数係数を使用した線形微分方程式

もう一度、E が $\mathbf{R}$ 上の任意の完全なノルム空間であると仮定します。 A を t から独立した A の連続自己準同型とし、同次一次方程式を考慮します。

$$
\frac{d\mathbf{x}}{dt} = A.\mathbf{x}.
$$

E が有限次元の場合、方程式 (19) は、係数 $a_{ij}$ が定数であるスカラー微分方程式の同次系 (3) (IV, p. 183) と等価です。

までに。 1 (IV, p. 179)、(19) のすべての積分はすべての $\mathbf{R}$ で定義されます。までに。 2 (IV, p. 179) 点 $t_0 \in \mathbf{R}$ で値 $\mathbf{x}_0$ をとった (19) の積分は、$C(t, t_0)\mathbf{x}_0$ と書くことができます。ここで、$C(t, t_0)$ は、次の方程式を満たす E 自体に対する E の全単射両連続線形写像です。

$$
\frac{dU}{dt} = AU
$$

そしてそれは $C(t_0, t_0) = I$ になります。さらに、私たちはアイデンティティを持っています

$$
C(t + \tau, t_0 + \tau) = C(t, t_0)
$$

任意の $\tau \in \mathbf{R}$ について: 確かに、(20) によって $dC(s, t_0 + \tau)/ds = AC(s, t_0 + \tau)$ が得られ、A は定数なので、また、

$$
\frac{dC(t + \tau, t_0 + \tau)}{dt} = AC(t + \tau, t_0 + \tau);
$$

さらに

$$
C(t_0 + \tau, t_0 + \tau) = I = C(t_0, t_0).
$$

よって点 $t_0$ における I に等しい (20) の積分は一意であるため、恒等式 (21) が得られます。

$C_0(t) = C(t, 0)$ を置くと $C(t, t_0) = C_0(t - t_0)$ になります。さらに、すべての $\lambda \in \mathbf{R}$ について、$C_0(\lambda t)$ は方程式の積分と同じです。

$$
\frac{dU}{dt} = \lambda AU
$$

これは、点 0 で値 I がかかります。次の定義を作成します。

#### 定義 1 {#fvr-iv-s2-def-1 .statement tag=08D4}

*E の連続自己準同型 A が与えられた場合、E の $e^A$ または $\exp A$ 自己同型は、値 I を求める式 (20) の積分の点 $t = 1$ における値に等しいと表します。 点 $t = 0$.*

これで記法注意の先行 def が表示されます。 1 それを示す

$$
C(t, t_0) = \exp \left( A(t - t_0) \right).
$$

たった今導入した指数記法は、次の特性によって正当化されます。これらは、z 実数または複素数 (cf. III、p. 98、および 106) について、写像 exp z の特性と完全に類似しています。

#### 命題 7 {#fvr-iv-s2-prop-7 .statement tag=08D5}

1' *写像* $X \mapsto e^X$ *は * $\mathscr{L}(E)$ * の写像 * から * E * の自己同型の群 (* $\mathscr{L}(E)$ の *可逆元) です。

2 *写像* $t \mapsto e^{Xt}$ *of* $\mathbf{R}$ *into* $\mathscr{L}(E)$ *微分可能、かつ*

$$
\frac{d}{dt} (e^{Xt}) = X e^{Xt} = e^{Xt} X.
$$ (24)

3 *すべてに* $X \in \mathscr{L}(E)$ *1 つは持っています*

$$
e^X = \sum_{n=0}^{\infty} \frac{X^n}{n!}
$$ (25)

*右辺は* $\mathscr{L}(E)$ のすべての境界部分集合に絶対的かつ一様に収束します。 *特に* $e^{It} = e^t I$ *$t \in \mathbf{R}$の場合。

4) *もし* X *そして* Y *通勤する* Y *そして* $e^Y$ *通勤* $e^X$, *そして*

$$
e^{X+Y} = e^X e^Y.
$$ (26)

関係 (24) は、$C(t, 0)$ の式 (23) と、この写像が (20) の積分であるという事実から得られます。 n での再帰により、(24) から $t \mapsto e^{Xt}$ は $\mathbf{R}$ で無限微分可能であることが導き出されます。

$$
D^n (e^{Xt}) = X^n e^{Xt}.
$$

テイラーの公式によって、次のように書くことができます。

$$
e^X = I + \frac{X}{1!} + \frac{X^2}{2!} + \cdots + \frac{X^n}{n!} + X^{n+1} \int_0^1 \frac{(1-t)^n}{n!} e^{Xt} \, dt.
$$ (27)

一方、cor. IV、p. 181の3は$\| e^{Xt} \| \leq \exp (\| X \| |t| )$を示しています。したがって、公式 (27) の余り $r_n(X) = X^{n+1} \int_0^1 \frac{(1-t)^n}{n!} e^{Xt} \, dt$ は不等式を満たします。

$$
\| r_n(X) \| \leq \frac{\| X \|^{n+1}}{(n+1)!} e^{\| X \| }
$$

よっては、公式 (25) を導き出し、右辺の系列は、$\mathscr{L}(E)$ のすべての有界部分集合に絶対的かつ一様に収束します。 対の元 $X,\ T$ の $\mathscr{L}(E)$ ごとに、次のようになります。

$$
e^{X+T} - e^X = \sum_{n=1}^{\infty} \frac{1}{n!} ((X+T)^n - X^n ).
$$

ここで、$(X + T)^n - X^n = \sum_{(V_i)} V_1 V_2 \ldots V_n$ と書くことができます。ここで、和は、$\mathscr{L}(E)$ の元の $2^n - 1$ 数列 $(V_i)$ を引き継ぎ、$1 \leq i \leq n$ に対して $V_i = X$ または $V_i = T$ が代入されます。 $V_i$ は $T$ に等しい。 不等式
$$
\|(X + T)^n - X^n\| \leq (\|X\| + \|T\|)^n - \|X\|^n
$$
すぐに続きます、よって
$$
\|\exp(X + T) - \exp X\| \leq \exp \left( \|X\| + \|T\| \right) - \exp \|X\|
$$
これにより、写像 $X \mapsto \exp X$ の連続性が確立されます。

最後に、$X$ と $Y$ が交換する場合、$Y$ は $e^{Xt}$ と交換します (IV、p. 181、提案 2)。
$$
\frac{d}{dt} (e^{Xt} e^{Yt}) = X e^{Xt} e^{Yt} + e^{Xt} (Y e^{Yt}) = (X + Y) e^{Xt} e^{Yt}.
$$
一方、$t = 0$ に対して $e^{Xt} e^{Yt}$ は $I$ に等しいので、$e^{Xt} e^{Yt} = e^{(X+Y)t}$、よって公式 (26) となります。この後者から、特に任意の実数 $s$ と $t$ について、次のことが推測されます。
$$
e^{X(s+t)} = e^{Xs} e^{Xt}
$$
そしてそれも
$$
e^{-X} = (e^X)^{-1}.
$$

逆に、$X$ と $Y$ がもはや通勤すると仮定されない場合、(26) は有効であり続ける必要はないことに注意してください。実際、それは、$\exp X$ と $\exp Y$ が常に通勤することを意味しますが、単純な例 (IV、p. 204、演習 3) で示されるように、そうではありません。

ここで、$E$ が有限次元の体* $\mathbf{C}$ のベクトル空間と $E$ の $A$ 自己準同型 ($\mathbf{C}$ のベクトル空間構造について) はどちらであると仮定します。 $E$の基底に対する行列との同一視できる。すると、すべての $t \in \mathbf{R}$ について、$e^{At}$ は、同じ構造に対する $E$ の自己同型になります (IV、p. 181、提案 2)。 $r_k$ ($1 \leq k \leq q$) を、自己準同型 $A$ の *特性多項式* $\varphi(r) = \det(A - rI)$ ($A$ の「特性根」) の別個の根 ($\mathbf{C}$) とします。 $n_k$ が $r_k$ の重複度の位数である場合、$\sum_{k=1}^q n_k = n$ です。 (Alg., VII, 31, n° 3) 根 $r_k$ には対応する部分空間 $E_k$ の$E$、次元 $n_k$ があり、$E_k$ となることがわかります。は $A$ で *安定* であり、その $E$ は $E_k$ の *直和* です。 $E_k$ は、次のようにベクトル $\mathbf{x}$ の部分空間として定義できます。
$$
(A - r_k I)^{n_k} . \mathbf{x} = 0.
$$
$\mathbf{a}$ を $E$ の任意のベクトルとします。 $\mathbf{a}_k \in E_k$ の場合、$\mathbf{a} = \sum_{k=1}^q \mathbf{a}_k$ と書くことができます。したがって、点 $t = 0$ で値 $\mathbf{a}$ をとったIV、p. 188 の式 (19) の積分は、次のように与えられます。
$$
\mathbf{u}(t) = e^{At} . \mathbf{a} = \sum_{k=1}^q e^{At} . \mathbf{a}_k = \sum_{k=1}^q e^{r_k t} e^{(A - r_k I)t} . \mathbf{a}_k.
$$

しかし、$\mathbf{a}_k \in E_k$ 以来、人は

$$
e^{(A - r_k I)t} \cdot \mathbf{a}_k = \mathbf{a}_k + \frac{t}{1!}(A - r_k I) \cdot \mathbf{a}_k + \frac{t^2}{2!}(A - r_k I)^2 \cdot \mathbf{a}_k + \cdots
$$
$$
+ \frac{t^{n_k - 1}}{(n_k - 1)!}(A - r_k I)^{n_k - 1} \cdot \mathbf{a}_k .
$$

したがって、方程式 (19) のIV、p. 188 のすべての積分は次のように書くことができます。

$$
\mathbf{u}(t) = \sum_{k=1}^q e^{r_k t} \mathbf{p}_k(t)
$$

ここで、$\mathbf{p}_k(t)$ は $t$ の多項式、ベクトル空間 $E_k$ の係数、および次数 $\leq n_k - 1$ の多項式です。特に、$A$ の特性方程式のすべての根が *単純* である場合、空間 $E_k$ ($1 \leq k \leq n$) はすべて体 $\mathbf{C}$ 上の次元 1 であるため、$n$ ベクトルが存在します。 $c_k$ $n$ 写像 $e^{r_k t} c_k$ ($1 \leq k \leq n$) 形は、IV、p. 188 の方程式 (19) の積分の基本系となります。

自己準同型 $A$ の特性根は、IV、p. 188 の一次方程式* (19) の *特性根とも呼ばれます。 写像 $c e^{r t}$ がベクトル $c \neq 0$ に対する (19) の積分であると書くことによって、$A$ の特性方程式が得られることに気づくかもしれません。

When one has determined the roots $r_k$ ($1 \leq k \leq q$) explicitly, and thus the order of multiplicity $n_k$ of $r_k$, in practice one obtains the integrals of (19) by writing that this equation is satisfied by the expression (32) of IV, p. 191, where $\mathbf{p}_k$ is an arbitrary polynomial of degree $\leq n_k - 1$, with coefficients *in* $E$; on identifying the coefficients of $e^{r_k t}$ (for $1 \leq k \leq q$) in the two sides of the equation so obtained one obtains linear equations for the coefficients of the polynomials $\mathbf{p}_k$: one establishes easily that these equations determine the terms of degree $> 0$ of $\mathbf{p}_k$ as functions of the constant term, and that the latter is a solution of the equation $(A - r_k I)^{n_k} \cdot \mathbf{x} = 0$, which defines the subspace $E_k$ (method of "undetermined coefficients").

#### 注意 {#fvr-iv-s2-n6-rem-1 .statement tag=08D6}

この基底に対して$A$の行列が*実*元(*cf.* IV, p. 186, *注意* 2)となるような$E$の基底が存在するとき、$A$の特性方程式は成立します。本物の係数があります。 検討中の基底で表される$E$のすべての$\mathbf{x} = (\xi_k)_{1 \leq k \leq n}$について、$\overline{\mathbf{x}} = (\overline{\xi}_k)_{1 \leq k \leq n}$とします。 写像 $\mathbf{x} \mapsto \overline{\mathbf{x}}$ は、$E$ の反線形畳み込みです。 $r_k$ が特性方程式の非実数根であり、$E_k$ が対応する安定部分空間である場合、$\overline{r}_k$ は同じ重複度を持つ特性根であることがわかります (*Alg.*, VII)。 $r_k$としての$n_k$、および写像$\mathbf{x} \mapsto \overline{\mathbf{x}}$の下の$E_k$の像$E'_k$は、安定した部分空間対応するから$\overline{r}_k$です。 このことから、$\mathbf{u}_j$ ($1 \leq j \leq n_k$) が $E_k$ の値との $n_k$ 線形独立積分である場合、$2n_k$ 整 $\mathbf{u}_j + \overline{\mathbf{u}}_j,\ i(\mathbf{u}_j - \overline{\mathbf{u}}_j)$ は線形独立であり、$E$ の選択された基底に関して、 成分は、$E$ の *本物* 写像です。 $r_k$ が実数特性根 *注意* 2 の IV、p. 186 は、(同じ記法で) $E_k$ に値を含む$n_k$ 線形独立積分 $\mathbf{v}_j$ ($1 \leq j \leq n_k$) があることを示します。誰の成分は本物です。 このようにして、成分がすべて *実数* である (19) の積分の基本的な系が得られます。

### 7. 位数 $n$ の一次方程式

位数* $n$ の * 線形微分方程式を形の方程式と呼びます。

$$
D^n x - a_1(t) D^{n-1} x - \ldots - a_{n-1}(t) D x - a_n(t) x = b(t)
$$

ここで、$a_k$ ($1 \leq k \leq n$) と $b$ は、$\mathbf{R}$ の区間 $J$ で定義された実変数 $t$ の実数 (複素数) 写像です。 IV、p. 164 の一般的な手順は、この方程式が $n$ の最初の位数方程式の線形系と同等であることを示しています。

$$
\left\{
\begin{aligned}
\frac{dx_k}{dt} &= x_{k+1} & (1 \leq k \leq n-1) \\
\frac{dx_n}{dt} &= a_1(t)x_n + a_2(t)x_{n-1} + \cdots + a_n(t)x_1 + b(t)
\end{aligned}
\right.
$$

つまり、一次方程式に

$$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x} + \mathbf{b}(t)
$$

$\mathbf{x} = (x_1, x_2, \ldots, x_n) \in \mathbf{C}^n$、$\mathbf{b}(t) = (0, 0, \ldots, 0, b(t))$ を入れたところ、行列 $A(t)$ は次のように定義されます。

$$
A(t) = \begin{pmatrix}
0 & 1 & 0 & \ldots & 0 \\
0 & 0 & 1 & \ldots & 0 \\
\vdots & \vdots & \vdots & \ddots & \vdots \\
0 & 0 & 0 & \ldots & 1 \\
a_n(t) & a_{n-1}(t) & a_{n-2}(t) & \ldots & a_1(t)
\end{pmatrix}.
$$

したがって、位数 $n$ の一次方程式の研究は、適用特定の線形方程式 (35) に対する上記の一般的な結果から構成されます。 写像 $a_j$ ($1 \leq j \leq n$) と $b$ が *規制* されているすべての区間 $J$ に対して、位数の連続導関数を持つ $J$ で定義された写像 $u$ が 1 つだけ存在します。 $n-1$、およびこの区間に対する位数 $n$ の規制導関数 (可算集合の点を除く)、$J$ の可算部分集合の補数に対する満たす (33)、など

$$
u(t_0) = x_0, \qquad Du(t_0) = x_0', \ldots, \quad D^{n-1}u(t_0) = x_0^{(n-1)}
$$

ここで、$t_0$ は $J$ の任意の点であり、$x_0, x_0', \ldots, x_0^{(n-1)}$ は任意の $n$ 複素数です。

等次方程式の $p$ 積分 $u_j$ ($1 \leq j \leq p$) について

$$
D^n x - a_1(t) D^{n-1} x - \ldots - a_{n-1}(t) D x - a_n(t) x = 0
$$

associated with (33) to be linearly independent (in the space $C(J; \mathbf{C})$ of continuous maps from $J$ into $\mathbf{C}$, considered as a vector space over $\mathbf{C}$), it is necessary and sufficient that the corresponding $p$ integrals $\mathbf{u}_j = (u_j, Du_j, \ldots, D^{n-1}u_j)$ of the homogeneous equation $d\mathbf{x}/dt = A(t).\mathbf{x}$ should be linearly independent (in the space $C(J; \mathbf{C}^n)$ of continuous maps from $J$ into $\mathbf{C}^n$). この条件が必要であることは明らかです。

逆に、すべての零ではなく、$n$ の複素定数 $\lambda_j$ があり、$J$ で$\sum_{j=1}^n \lambda_j u_j(t) = 0$ が同一である場合、$1 \leq k \leq n - 1$ のようなすべての整数 $k$ について、$J$ で$\sum_{j=1}^n \lambda_j D^k u_j(t) = 0$ であると推測されます。 $J$の$\sum_{j=1}^n \lambda_j \mathbf{u}_j(t) = 0$。

従って (IV, p. 180, cor. 1)

#### 命題 8 {#fvr-iv-s2-prop-8 .statement tag=08D7}

*$J$ で定義された同次一次方程式 (37) の積分の集合は、体 $\mathbf{C}$ にわたる次元 $n$ のベクトル空間です。

式 (37) の任意の $n$ 積分 $u_j$ ($1 \leq j \leq n$) が与えられると、この系の積分行列式 ($\mathbf{C}^n$ の標準基底に関して) 対応する $n$ 積分 $\mathbf{u}_j$ の *ロンスキー関数* と呼ばれます。方程式$d\mathbf{x}/dt = A(t).\mathbf{x}$、つまり写像

$$
W(t) = \begin{vmatrix}
u_1(t) & u_2(t) & \ldots & u_n(t) \\
Du_1(t) & Du_2(t) & \ldots & Du_n(t) \\
\vdots & \vdots & \ddots & \vdots \\
D^{n-1}u_1(t) & D^{n-1}u_2(t) & \ldots & D^{n-1}u_n(t)
\end{vmatrix}.
$$

$n$ 積分 $u_j$ が線形独立であるためには、$J$ 上の $W(t) \neq 0$ が必要かつ十分です。さらに、このためには、$J$ の *1 つだけ* $t_0$ で $W(t_0) \neq 0$ (IV、p. 184、提案 4) で十分です。さらに、1 つは (IV, p. 184, 提案 5) を持ちます。

$$
W(t) = W(t_0) \exp \left( \int_{t_0}^t a_1(s)\, ds \right).
$$ (38)

$\mathbf{C}^n$ の標準基底に関して、方程式 (35) の分解能 $C(t, t_0)$ をその行列で同一視する計算します。この行列の列 $\mathbf{v}_j(t, t_0)$ ($1 \leq j \leq n$) は、$n$ 線形独立積分になります

$$
\mathbf{v}_j(t, t_0) = (v_j(t, t_0), Dv_j(t, t_0), \ldots, D^{n-1}v_j(t, t_0))
$$

等次方程式 $d\mathbf{x}/dt = A(t).\mathbf{x}$ の対応するから $n$ への線形独立積分 $v_j(t, t_0)$ の式 (37) は次のようになります。

$$
D^{k-1}v_j(t_0, t_0) = \delta_{jk}
$$

(クロネッカー デルタ) $1 \leq j \leq n, 1 \leq k \leq n$ ($D^0 v_j = v_j$ を置くことに同意した場合)。特に、式 (35) に適用されるパラメータの変化 (IV、p. 182) の方法は、(33) の特定の積分として、点 $t_0$、写像での最初の $n-1$ 導関数とともに 0 に等しいという結果になります。

$$
w(t) = \int_{t_0}^t v_n(t, s)b(s)\, ds.
$$ (39)

方程式 $D^n x = b(t)$ 公式 (39) の特別なケースでは、再び、規制された写像 $b(t)$ の $n^{th}$ プリミティブを表す公式が得られます。これは、点 $t_0$ での最初の $n - 1$ 導関数で消滅します。
$$
w(t) = \int_{t_0}^t b(s) \frac{(t-s)^{n-1}}{(n-1)!} \, ds
$$
(II, p. 62, 公式 (19)): 点 $t_0$ で最初の $n - 2$ 導関数とともに消滅し、そこでの $n - 1$ 次導関数が 1 に等しい $D^n x = 0$ の積分は、実際には多項式です。 $(t-t_0)^{n-1}/(n-1)!$。

### 8. 定数係数を使用した位数 $n$ の一次方程式

式 (33) の係数 $a_j$ が定数の場合、対応する行列 $A$ は定数です。特性方程式は、$e^{rt}$ が解と書くことで得られ、次のようになります。
$$
r^n - a_1 r^{n-1} - \ldots - a_{n-1} r - a_n = 0.
$$
$r_j$ ($1 \leq j \leq q$) をこの方程式の個別の根とし、根 $r_j \left( \sum_{j=1}^q n_j = n \right)$ の$n_j$ ($1 \leq j \leq q$) 重複度とします。 IV、p. 188 から 194、それぞれの根 $r_j$ の結果により、対応するが得られ、同次方程式の場合
$$
D^n x - a_1 D^{n-1} x - \cdots - a_{n-1} D x - a_n x = 0
$$
$n_j$ の線形独立積分のうち系
$$
u_{jk}(t) = e^{r_j t} p_{jk}(t),
$$
ここで、$p_{jk}$ は、次数 $\leq n_j - 1$ ($1 \leq k \leq n_j$) の多項式 (複素数係数) です。さらに、そのようにして得られた$n$ 積分$u_{jk}$ ($1 \leq j \leq q,\ 1 \leq k \leq n_j$) は線形独立です。したがって、$n_j$ 多項式 $p_{jk}$ ($1 \leq k \leq n_j$) は、次数 $\leq n_j - 1$ の$t$ の多項式の空間で線形独立であるため、形基底 (以上)後者は次元 $n_j$ のものなので、この空間の $\mathbf{C}$) です。その他語:

#### 命題 9 {#fvr-iv-s2-prop-9 .statement tag=08D8}

*$r_j$ ($1 \leq j \leq q$) を特性方程式 (40) の個別の根とし、$n_j$ を根 $r_j$ ($1 \leq j \leq q$) の重複度とします。この場合、$n$ 写像 $t^k e^{r_j t}$ ($1 \leq k \leq n_j,\ 1 \leq j \leq q$) は、同次方程式 (41) の線形独立積分です。*

証明できるこの結果は、次の方法で直接得られます。式 (41) から、この方程式のすべての積分の $n^{th}$ 導関数は $\mathbf{R}$ で微分可能であることがわかり、そこからすぐに整数 $m > n$ の帰納法によって、(41) のすべての積分は位数 $m$ の導関数が許容されることがわかります。は $\mathbf{R}$ で *無限微分可能*です。 $\mathscr{D}$ を、$\mathbf{R}$ 上の無限微分可能な複素数値写像の $\mathbf{C}$ 上の (非トポロジカルな) ベクトル空間とします。 写像 $x \mapsto Dx$ はこの空間の自己準同型であり、式 (41) が書けます。

$$
f(D)x = 0 \tag{42}
$$

ここで、$f(D) = D^n - a_1 D^{n-1} - \ldots - a_{n-1} D - a_n$ (アルゴリズム、IV、p. 4)。

#### 命題 10 {#fvr-iv-s2-prop-10 .statement tag=08D9}

*g と h を、$f = gh$ のような 2 つの互いに素な多項式とする。 (42) の解の部分空間は、2 つの方程式の解の部分空間の直和です*

$$
g(D)x = 0, \qquad h(D)x = 0.
$$

さて、Bezout 恒等式 (Alg., VII. 2, th. 1) により、$p(D)g(D) + q(D)h(D) = 1$ となる 2 つの多項式 $p(D)$ と $q(D)$ が存在します。 (42) の解 $x$ ごとに $x = y + z$ を書くことができます。ここで $y = p(D)g(D)x$ と $z = q(D)h(D)x$ です。そして$h(D)y = p(D)(f(D)x) = 0$と$g(D)z = q(D)(f(D)x) = 0$。一方、$g(D)x = 0$ と $h(D)x = 0$ の両方が一致する場合、次のように推測されます。

$$
x = p(D)(g(D)x) + q(D)(h(D)x) = 0,
$$

これで証明が完了します。

前述の記法を使用すると、次のように書くことができます。

$$
f(D) = \prod_{j=1}^q (D - r_j)^{n_j}
$$

そしてプロップ。 10は、$q$の帰納法により、(42)の解の部分空間が$q$方程式の解の部分空間の直和であることを示しています。

$$
(D - r_j)^{n_j} x = 0 \qquad (1 \leq j \leq q). \tag{43}
$$

さて、複素数 $r$ ごとに、1 つは

$$
D(e^{rt} x) = e^{rt}(D + r)x \tag{44}
$$

したがって、(43) は次と同等です

$$
D^{n_j}(e^{-r_j t} x) = 0
$$

したがって、解写像 $e^{r_j t} p_j(t)$ となります。ここで、$p_j$ は、次数 $\leq n_j - 1$ の多項式の集合を実行します。したがって、プロップを回収します。 IV、p. 194の9。

同次方程式 (41) が解かれていると仮定すると (つまり、特性根が見つかったと仮定すると)、パラメーターの変化方法によって不均質方程式の解を見つけることができることがわかります。

$$
D^n x - a_1 D^{n-1} x - \ldots - a_{n-1} Dx - a_n x = b(t) \tag{45}
$$

ここで、$b(t)$ は *任意の* 規制された写像 (IV、p. 182) です。 $b(t)$ が区間 J 上で *無限微分可能* である場合、(45) のすべての積分は J 上で無限微分可能であることに注意してください。 特定のケース $b(t) = e^{\alpha t} p(t)$ では、$p$ は多項式 (複素数係数) であり、$\alpha$ は任意の多項式です複素数の場合、(45) の積分は次の方法によってより簡単に得られます。 $x = e^{\alpha t} y$ を入れます。方程式

$$
f(D)x = e^{\alpha t} p(t)
$$

(44) によって次のように書くことができます

$$
f(\alpha + D)y = p(t)
$$

または、多項式 $f(D)$ にテイラーの公式を適用すると、

$$
\frac{f^{(n)}(\alpha)}{n!} D^n y + \frac{f^{(n-1)}(\alpha)}{(n-1)!} D^{n-1} y + \cdots + \frac{f'(\alpha)}{1!} Dy + f(\alpha) y = p(t). \tag{46}
$$

$m$ を多項式 $p(t) = \sum_{k=0}^m \lambda_k t^{m-k}$ の次数とします。 $f(\alpha) \neq 0$ (つまり、$\alpha$ が特性根ではない場合) の場合、係数に対して、(46) の解である多項式 $u(t) = \sum_{k=0}^m c_k t^{m-k}$ *of 次数* $m$ が 1 つだけ存在します。 $c_k$は一次方程式の系によって決定されます

$$
f(\alpha)c_k + \binom{m-k+1}{1} f'(\alpha)c_{k-1} + \binom{m-k+2}{2} f''(\alpha)c_{k-2} + \cdots
+ \binom{m}{k} f^{(k)}(\alpha)c_0 = \lambda_k \qquad (0 \leq k \leq m)
$$

これは明らかに唯一の解を認めます。一方、$\alpha$ が特性根で、$h$ がその重複度である場合、前述の計算は、$D^h y = v(t)$ のすべての解が整数となるような次数 $m$ の多項式が 1 つだけ存在することを示します。他の語では、(46) のすべての多項式解は次数 $m + h$ (「共鳴」) になります。

### 9. 定数係数をもつ一次方程式の系

n° 8 の記法を使って、形の $m$ の微分方程式の系をより一般的に考えてみましょう。

$$
\sum_{k=1}^n p_{jk}(D) x_k = b_j(t) \qquad (1 \leq j \leq m) \tag{47}
$$

ここで、未知数 $x_k$ ($1 \leq k \leq n$) と右辺 $b_j$ ($1 \leq j \leq m$) は実変数 $t$ の複素数写像であり、$p_{jk}(D)$ は *定数* (複素数) の多項式 (任意の次数) です。微分演算子 $D$ ($1 \leq j \leq m,\ 1 \leq k \leq n$) の係数。

次の例が示すように、そのような系は、IV、p. 1164 (公式 (5)) で考慮されたものと同じ型ではありません。

$$
\begin{cases}
D x_1 = a(t) \\
D^2 x_1 + D x_2 + x_2 = b(t).
\end{cases}
$$

写像 $b_j(t)$ が区間 J 上で *無限微分可能* である場合に限定し、J 上で無限微分可能である解 $(x_k)_{1 \leq k \leq n}$ のみを探します。 $\mathbf{b}(t) = (b_1(t), \ldots, b_m(t))$、(J から $\mathbf{C}^m$ に写像)、および $\mathbf{x} = (x_1, x_2, \ldots, x_n)$、系 (47) を入れると、次のように書くことができます。

$$
P(D) \mathbf{x} = \mathbf{b}(t)
$$

ここで、$P(D)$ は m 行と n 個の列を持つ行列 $(p_{jk}(D))$ で、その係数属するから環 $\mathbf{C}[D]$ は D の多項式であり、$\mathbf{C}$ には係数が含まれます。 $f_j(D)$ ($1 \leq j \leq r \leq \operatorname{Min}(m, n)$) を行列 $P(D)$ の非零 *類似不変量* とします。 (*Alg.*, VII, p. 32) これらは、$1 \leq j \leq r - 1$ に対して $f_j$ 割る $f_{j+1}$ ($r$ は $P(D)$ の *階数*) となるような、よく決定されたモニック多項式であることがわかります。さらに、位数 m と n の 2 つの正方行列 $U(D)$ と $V(D)$ がそれぞれ *反転可能* (位数 m と n の正方行列の環で、*環には係数が入っています)複素数係数*) を持つ D の多項式の $\mathbf{C}[D]$ であり、$1 \leq j \leq r$ の対角線項 $q_{jj}(D) = f_j(D)$ を除いて、行列 $Q(D) = (q_{jk}(D)) = U(D) P(D) V(D)$ のすべての要素は零になります。ここで $\mathbf{y} = V^{-1}(D) \mathbf{x}$ を置きます。式 (49) は次の式と等価です。

$$
U(D) (P(D)(V(D) \mathbf{y})) = U(D) \mathbf{b}
$$

つまり、

$$
Q(D) \mathbf{y} = U(D) \mathbf{b}
$$

$U(D)$ は反転可能なので。さて、$\mathbf{y} = (y_1, y_2, \ldots, y_n)$ の場合、および

$$
U(D) \mathbf{b}(t) = (c_1(t), \ldots, c_m(t)),
$$

そうすると、式 (50) が書けます。

$$
f_j(D) y_j = c_j(t) \quad \text{for } 1 \leq j \leq r \tag{51}
$$
$$
0 = c_j(t) \quad \text{for } r + 1 \leq j \leq m. \tag{52}
$$

The system thus does not admit any indefinitely differentiable solutions unless the conditions (52) are satisfied; the determination of the $y_j$ for indices $j \leq r$ then reduces to integrating the r linear differential equations with constant coefficients (51); the $y_j$ for indices $> r$ are arbitrary indefinitely differentiable functions. このようにして (50) の解 $\mathbf{y}$ が決定されると、公式 $\mathbf{x} = V(D) \mathbf{y}$ から (47) の解が推定されます。

#### 注意 1 {#fvr-iv-s2-n9-rem-1 .statement tag=08DA}

一部の多項式 $f_j(D)$ は簡約するから非零の定数になります。その後、対応する $y_j$ が完全に決定されます。

#### 注意 2 {#fvr-iv-s2-n9-rem-2 .statement tag=08DB}

When the $b_j$ are all zero, that is, if the system (47) is *homogeneous*, the conditions (52) are always satisfied; if, further, $r = n$, one sees that the set of solutions of (47) is a vector space over $\mathbf{C}$, of dimension equal to the *sum of the degrees* of the $f_j(D)$, that is, to the *degree* of $\det(P(D))$.

#### 注意 3 {#fvr-iv-s2-n9-rem-3 .statement tag=08DC}

多項式 $p_{jk}(D)$ を考えると、系 (47) は、右辺が無限に微分可能である (または特定の位数で微分可能) 場合に解を許容しますが、右辺が任意に規定されている場合には写像を許容しません。これは、例 (48) で示されます。 $a(t)$ がプリミティブではない場合、解。ここでは、右辺が恣意的に規制されている写像ときに入る補足的な可能性条件を求めることは約束しません。

### 練習問題 {#fvr-iv-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。

[^1]: $E$ が有限次元の場合、$E$ からそれ自体へのすべてのアフィン線形写像は連続であることを思い出してください (*Gen. トップ.*、VI、p. 33、および 37)。
