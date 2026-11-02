---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 2
section_title: Examples of algebras
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 438-457, 618-626
pdf_pages: 0462-0481, 0642-0650
extraction: ocr
subsections:
    - "no": 1
      title: ENDOMORPHISM ALGEBRAS
      page: 438
      pdf_page: 462
    - "no": 2
      title: MATRIX ELEMENTS
      page: 438
      pdf_page: 462
    - "no": 3
      title: QUADRATIC ALGEBRAS
      page: 439
      pdf_page: 463
    - "no": 4
      title: CAYLEY ALGEBRAS
      page: 441
      pdf_page: 465
    - "no": 5
      title: CONSTRUCTION OF CAYLEY ALGEBRAS. QUATERNIONS
      page: 443
      pdf_page: 467
    - "no": 6
      title: ALGEBRA OF A MAGMA, A MONOID, A GROUP
      page: 446
      pdf_page: 470
    - "no": 7
      title: FREE ALGEBRAS
      page: 448
      pdf_page: 472
    - "no": 8
      title: DEFINITION OF AN ALGEBRA BY GENERATORS AND RELATIONS
      page: 450
      pdf_page: 474
    - "no": 9
      title: POLYNOMIAL ALGEBRAS
      page: 452
      pdf_page: 476
    - "no": 10
      title: TOTAL ALGEBRA OF A MONOID
      page: 454
      pdf_page: 478
    - "no": 11
      title: FORMAL POWER SERIES OVER A COMMUTATIVE RING
      page: 455
      pdf_page: 479
statements: 17
exercises: 25
content_sha256: c9a2ebf8174ef66c28a2cedfccdb03962fe0627f38bdae486b7e67483d16e9c2
translated_from: content/en/alg/III/02_s2_examples_of_algebras.md
translation_method: google
source_content_sha256: 523c00d5d47e83c328fe974b4b99f51c3c18998f5e378badbbbbd303ed1feec8
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 771d514ecacec1b3feb8d82f5bd6ba06e6ea30bcf3c108e1428802ce5bd38791
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 2。 代数中例

この段落全体を通じて、A は可換環を示します。

### 1. 自己準同型環

B を 1 で示される単位元との結合A-代数とし、M を右B-加群とします。 環 $E = \mathrm{End}_B(M)$ には B の中心を超える加群構造があることがわかります。今、A の B の準同型 $h : \alpha \mapsto \alpha . 1$ の像は B の中心 (§ 1, no. 1) に含まれます。したがって、$h$ は E A-加群構造を与えます。さらに、Eの$\alpha \in A$と$f, g$については、

$$
\alpha(f \circ g) = f \circ (\alpha g) = (\alpha f) \circ g;
$$

したがって、E の乗法と E の A-加群構造定義する E の結合A-代数構造です。 Mの恒等写像はこの代数の単位元です。

### 2. 行列元

B を、B (II, § 10, no. 7) 上の位数 n の平方行列の単位結合A-代数および$\mathbf{M}_n(B)$ 集合とします。この場合、$\mathbf{M}_n(B)$ には $\alpha . (b_{ij}) = (\alpha b_{ij})$ ($\alpha \in A, b_{ij} \in B, 1 \leq i \leq n, 1 \leq j \leq n$) によって定義される A-加群構造が含まれます。この構造と行列乗法定義するは、$\mathbf{M}_n(B)$ の単位結合 A-代数構造です。 $\mathbf{M}_n(B)$ から $\mathrm{End}_B(B_d^n)$ (II, § 10, no. 7) への正規の全単射は A-代数同型です。

$B = A$、A-代数 $\mathbf{M}_n(A)$ が行列単位 (II, § 10, no. 3) の標準基底 $(E_{ij})$ からなるを認めるとき。 対応する乗法表は

$$
E_{ij} E_{hk} = \delta_{jh} E_{ik}.
$$

単位元 $I_n$ は $\sum_{i=1}^n E_{ii}$ に等しい。

### 3. 二次代数

$\alpha, \beta$ を A の 2 つの元と $A^2$ の $(e_1, e_2)$ 標準基底とします。 A 上の型 $(\alpha, \beta)$ の二次代数は A-加群 $A^2$ で、代数構造は乗法表 (§ 1, no. 7) で定義されます

$$
e_1^2 = e_1, \quad e_1 e_2 = e_2 e_1 = e_2, \quad e_2^2 = \alpha e_1 + \beta e_2.
$$

二次代数と同型の A-代数 E は、二次代数とも呼ばれます。 It amounts to the same to say that E admits a basis of two elements one of which is the unit element.

2 つの元の基底を認めるすべての単位 A-代数は二次代数 (練習問題 1) であることがわかります。

A-代数の基底 $(e_1, e_2)$ に乗法表 (2) がある場合、それは型 $(\alpha, \beta)$ の基底と呼ばれます。言葉の乱用により、型 $(\alpha, \beta)$ の基底があるとき、二次代数は型 $(\alpha, \beta)$ であると言われます。

#### 命題 1 {#alg-iii-s2-prop-1 .statement tag=05YX}

*二次代数 E は結合性と可換性を持ちます。*

E が可換であるという事実は、(2) の方程式 $e_1 e_2 = e_2 e_1$ からわかります。同様に、結合性を検証するには、$x, y, z$ がそれぞれ $e_1$ または $e_2$ に等しいときの $x(yz) = (xy)z$ を確認するだけで十分です。さて、この関係は、元 $x, y, z$ の少なくとも 1 つが $e_1$ に等しい場合には明らかです。 E は可換であるため、$x = y = z = e_2$ にも当てはまります。 よって命題。

$e$ は二次代数 E の単位元を表し、$(e, i)$ は型 $(\alpha, \beta)$ の E の基底とします。したがって、E 含む $e$ の 1 つおきの基底は、形 $(e, j)$ と $j = \gamma e + \delta i$ (II, § 7, no. 2、系 ～ 命題 3) です。さらに、$(e, j)$ が E の基底であるためには、$\delta$ が A で可逆であることが必要かつ十分です。 条件で十分なのは明らかです。逆に、$\bar{i}$が$E/Ae$の$i$の標準像である場合、$\bar{i}$と$\bar{j} = \delta \bar{i}$はそれぞれ$E/Ae$の形基底、よっては条件の必要性が生じます。それから

$$
j^2 = (\gamma^2 + \alpha \delta^2)e + (2\gamma \delta + \beta \delta^2)i = (\alpha \delta^2 - \gamma^2 - \beta \gamma \delta)e + (2\gamma + \beta \delta)j;
$$

したがって、E は型であることがわかります。

$$
(\alpha \delta^2 - \gamma^2 - \beta \gamma \delta, 2\gamma + \beta \delta)
$$

すべての反転可能な $\delta \in A$ とすべての $\gamma \in A$ に対して。特に、$E$ が型 $(\alpha, 2\beta')$ である場合、$\gamma = -\beta'$ と $\delta = 1$ をとればわかるように、$i$ も型 $(\alpha + {\beta'}^2, 0)$ です。

#### 命題 2 {#alg-iii-s2-prop-2 .statement tag=05YY}

*$E$ を二次方程式の $A$-代数、$e$ をその単位元とします。すべての $u \in E$ について、$T(u)$ を無料の $A$ モジュール $E$ (II, § 4, no. 3) の自己準同型 $m_u : x \mapsto ux$ のトレースとします。すると、$s(u) = T(u).e - u$ によって定義された写像 $s$ は、すべての $u \in E$ に対して、代数 $E$ と $s^2(u) = u$ の自己同型になります。

$(e, i)$ を $E$ の型 $(\alpha, \beta)$ の基底とします。次に$T(e) = 2$、そのとき$s(e) = e$、そして$T(i) = \beta$、よって $s(i) = \beta e - i$。したがって、$(e, s(i))$ は $E$ の基底であり、その型は$\gamma = \beta$ と $\delta = -1$ を含む (3) によって与えられ、再び$(\alpha, \beta)$ が得られます。したがって、$s$ は代数 $E$ の自己同型になります。 $A$ モジュール $E$ の $m_{s(u)} = s m_u s^{-1}$、自己準同型 $m_u$、$m_{s(u)}$ は同じトレース (II, § 4, no. 3、命題 3)、よってを持っています。

$$
s^2(u) = T(u).e - s(u) = T(u).e - (T(u).e - u) = u
$$

$u \in E$ 全員のために。

自己同型 $s$ は、$A$-代数 $E$ の *共役* と呼ばれ、$s(u)$ は $u$ の *共役* と呼ばれます。

$u = \xi e + \eta i$、$A$に$\xi, \eta$がある場合、$s(u) = (\xi + \beta \eta)e - \eta i$、よって

(4)
$$
T(u)e = u + s(u) = (2\xi + \beta \eta)e
$$
(5)
$$
u.s(u) = (\xi^2 + \beta \xi \eta - \alpha \eta^2)e = N(u)e
$$

$N(u) = \xi^2 + \beta \xi \eta - \alpha \eta^2$ と書いたところ。 元 $T(u)$ と $N(u)$ (または、$A$ と $Ae$ が正規に識別される場合、元 $T(u)e$ と $N(u)e$) は、それぞれ $u$ の *トレース* と *ノルム* と呼ばれます。

$\beta = 0$の場合、上記の式は次のように簡略化されます。

(6)
$$
s(\xi e + \eta i) = \xi e - \eta i, \quad T(\xi e + \eta i) = 2\xi, \quad N(\xi e + \eta i) = \xi^2 - \alpha \eta^2.
$$

明らかに、$T$ は $E$* 上の *線型形式* であり、* $N$ は $E$ (IX, § 3, no. 4)* 上の *2 次関数形* です。 $E$ は可換かつ結合であるため、(5) から次のようになります。

(7)
$$
N(uv) = N(u)N(v).
$$

$u$ が $E$ で *反転可能* であるためには、 $N(u)$ が $A$ で *反転可能* であることが必要かつ十分です。なぜなら、$N(e) = 1$ として、条件の必然性が (7) から導かれ、$v = u^{-1}$ と書けるからです。逆に、$N(u)$ が $A$ で可逆である場合、(5) から、$u$ は可逆であることがわかり、

(8)
$$
u^{-1} = (N(u))^{-1}s(u).
$$

*$N(u)$ は、自己準同型 $m_u$ (cf. § 9 no. 3, 例 1) の行列式 (§ 8, no. 1) であることが証明できます。

次の命題は、可換体に対する二次代数の構造を与えます。

#### 命題 3 {#alg-iii-s2-prop-3 .statement tag=05YZ}

*E を型* $(\alpha, \beta)$ の 2 次式 A-代数とします。

(i) *A が体かつ含むではない元* $\zeta$ ** $\zeta^2 = \alpha + \beta \zeta$ である場合、*E は (可換) 体* (cf. V, § 3) です。

(ii) *環* A *含む元* $\zeta$ *そのような* $\zeta^2 = \alpha + \beta \zeta$ *かつ* $\beta - 2\zeta$ *可逆* (それぞれ零)、*E は* A $\times$ A *それぞれと同型である。は型* $(0, 0))$ です。

(i) を証明します。 $\xi, \eta$をAと$u = \xi e + \eta i$の2つの元とします。 $\eta \neq 0$ で $\theta = -\xi \eta^{-1}$ と書くと、(5) により $\mathrm{N}(u) = \eta^2 (\theta^2 - \beta \theta - \alpha)$、A の仮定によりよって $\mathrm{N}(u) \neq 0$ となります。 $\eta = 0$の場合は、$\mathrm{N}(u) = \xi^2$。いずれにせよ、$u \neq 0$ の場合、$\mathrm{N}(u) \neq 0$ であるため、$\mathrm{N}(u)$ は A で可逆であり、したがって $u$ は E で可逆です。

ここで (ii) を証明します。 標準基底 $(e_1, e_2)$ の代数 A $\times$ A は型 $(0, 1)$ です。 E が型であることを (公式 (3)) 見てきました。

$$
(\alpha \delta^2 - \gamma^2 - \beta \gamma \delta, 2\gamma + \beta \delta)
$$

A のすべての $\gamma \in A$ とすべての $\delta$ が可逆です。$\beta - 2\zeta$ が可逆の場合、$\delta = (\beta - 2\zeta)^{-1}$ と $\gamma = -\zeta (\beta - 2\zeta)^{-1}$ を取ります。それから$2\gamma + \beta \delta = 1$と

$$
\alpha \delta^2 - \gamma^2 - \beta \gamma \delta = \delta^2 (\alpha - \zeta^2 + \beta \zeta) = 0;
$$

したがって、E は型 $(0, 1)$ であり、したがって A $\times$ A と同型です。 $\beta - 2\zeta = 0$ の場合、E は型 $(\alpha + \zeta^2, 0)$ であり、したがって $\alpha + \zeta^2 = 2\zeta^2 - \beta \zeta = 0$ 以降型 $(0, 0)$ であることがすでに述べられています。

型 $(0, 0)$ の二次方程式 A-代数は、A 上の双対数* の *代数とも呼ばれます。

### 4. ケイリー 代数

#### 定義 1 {#alg-iii-s2-def-1 .statement tag=05Z0}

*Cayley 代数 over* A *は順序付き対* (E, s)、*ここで* E *は代数 over* A *with 単位元* e *and* s *は E の反自己同型です *そのような*

$$
u + s(u) \in Ae \quad \text{and} \quad u.s(u) \in Ae
$$

*全員に* $u \in E$。

$s$ は Cayley 代数 (E, s) の *活用* と呼ばれ、$s(u)$ は $u$ の *共役* と呼ばれます。 条件 $u + s(u) \in Ae$ は、$u$ と $s(u)$ が *置換可能*であることを意味します。私たちは書きます

(9) $$
T(u) = u + s(u)
$$
(10) $$
N(u) = u.s(u) = s(u).u
$$

そして、部分代数 $Ae$ のこれらの元は、それぞれ、$u$ の *Cayley トレース* と *ノルム* と呼ばれます。

二次代数 E とその共役 s (E は可換であるため反自己同型) (no. 3) の順序付き対からなるは Cayley 代数です。

(E, s) を Cayley 代数とします。 $s(e) = e,\ s(u + s(u)) = u + s(u)$ として、他の語 $s(u) + s^2(u) = u + s(u)$ または

$$
s^2(u) = u
$$

したがって、$s^2$ は E の恒等写像になります。

$$
T(s(u)) = T(u), \quad N(s(u)) = N(u).
$$

最後に、関係 $(u - u)(u - s(u)) = 0$ は次のようになります。

$$
u^2 - T(u).u + N(u) = 0
$$

$u \in E$の皆さんへ。

#### 命題 4 {#alg-iii-s2-prop-4 .statement tag=05Z1}

*E を A-代数とし、(E, s) と (E, s') が Cayley 代数となるような E の反自己同型性を s と s とします。 E が基底含む単位元 e を認める場合、s' = s.*

明らかに、すべての $u \in Ae$ に対して $s'(u) = s(u) = u$ です。 T, N (それぞれ T', N') がトレースであり、(E, s) (それぞれ (E, s')) がノルム写像である場合、(13) から次のことがわかります。

$$
(T(u) - T'(u)).u - (N(u) - N'(u)) = 0.
$$

B を E 含む e の基底とし、e とは異なる B の u 元とする。次に$T(u) - T'(u) = 0$、よって $s(u) = s'(u)$。 B 上の s と s の一致するなので、それらは等しいです。

以下では、$\bar{u} = s(u)$ と書きます。

$$
\left\{\begin{array}{lll}
u + \bar{u} = T(u), & u\bar{u} = \bar{u}u = N(u), & \bar{u} = u \\
u + v = \bar{u} + \bar{v}, & \alpha u = \alpha \bar{u}, & uv = \bar{v}.\bar{u}
\end{array}\right.
$$

Eの$u, v$、$\alpha \in A$。さらに

$$
T(e) = 2e, \quad N(e) = e.
$$

公式から

$$
T(uv) = uv + \overline{uv} = uv + \bar{v}.\bar{u} = uv + (T(v) - v)(T(u) - u),
$$

私たちはそれを推測します

$$
uv + vu = T(u)v + T(v)u + (T(uv) - T(u)T(v))
$$

よって、$u$と$v$を交換、

$$
T(vu) = T(uv).
$$

一方、$N(u + v) = (u + v)(\bar{u} + \bar{v}) = N(u) + N(v) + T(u\bar{v})$、よって

(18)
$$
T(v\bar{u}) = T(u\bar{v}) = N(u + v) - N(u) - N(v).
$$

ここで、(16) に $u$ を $\bar{u}$ で置き換えて適用すると、次のようになります。
$$
T(u\bar{v}) = T(u)T(v) + \bar{u}v + v\bar{u} - T(u)v - T(v)\bar{u} = T(u)T(v) - uv - \bar{v}.\bar{u};
$$
よって

(19)
$$
T(v\bar{u}) = T(u\bar{v}) = N(u + v) - N(u) - N(v) = T(u)T(v) - T(uv).
$$

最後に、明らかにすべての$\alpha \in A$に対して、

(20)
$$
N(\alpha u) = \alpha^2 N(u);
$$
特に $N(2u) = 4N(u)$ なので、公式 (19) は次のようになります。

(21)
$$
(T(u))^2 - T(u^2) = 2N(u).
$$

明らかに、$T$ は、$(Ae)$ モジュール $E$ の線型形式です。 $(u, v) \mapsto T(v\bar{u})$ はこの加群上の双線形形式であるため、*(18) と (20) から、$N$ は二次方程式形 (cf. IX, § 3, no. 4) であることがわかります。*

### 5. ケイリー代数の構成。クォータニオン

$(E, s)$ を $A$ 上の Cayley 代数とし、no. 4 の記法を使用し、$\gamma \in A$ とします。 $F$ を $A$ 上の代数とします。その基礎となる加群は $E \times E$ で、その乗法は次のように定義されます。

(22)
$$
(x, y)(x', y') = (xx' + \gamma \bar{y}'y, y\bar{x}' + y'x);
$$
明らかに、$(e, 0)$ は $F$ の単位元であり、$E \times \{0\}$ は $F$ の部分代数であり、$E$ と同型です。以下では、これを $E$ で *同一視する* するので、$x \in E$ は $(x, 0)$ と識別され、特に $e$ は $F$ の単位元と識別されます。

$t$ を、次のように定義される $F$ の置換とします。

(23)
$$
t((x, y)) = (\bar{x}, -y) \quad (x \in E, y \in E).
$$

#### 命題 5 {#alg-iii-s2-prop-5 .statement tag=05Z2}

(i) *注文された対 $(F, t)$ は、$A$* 上の Cayley 代数です。

(ii) *$j = (0, e)$とすれば、$x \in E, y \in E$は$(x, y) = xe + yj$となります。 Cayley トレースと $F$ のノルム $T_F$ および $N_F$ は次の式で与えられます*

(24)
$$
T_F(xe + yj) = T(x), \quad N_F(xe + yj) = N(x) - \gamma N(y).
$$

(iii) *$F$が結合的であるためには、$E$が結合的かつ可換的であることが必要かつ十分です。*

$(x, y) \in \mathbf{F}$の場合、

$$
(x, y) + t((x, y)) = (x + \overline{x}, 0) = T(x)e
$$
(25)
$$
(x, y)t((x, y)) = (x, y)(\overline{x}, -y) = (xx - \gamma \overline{y}y, y\overline{x} - yx)
= (\mathrm{N}(x) - \gamma \mathrm{N}(y), 0) = (\mathrm{N}(x) - \gamma \mathrm{N}(y))e.
$$
(26)

したがって、(i) と (ii) の両方を証明するには、$t$ が $\mathbf{F}$ の反自己同型であることを示せば十分です。明らかに $t$ は A-linear 全単射です。一方、
$$
t((x, y) \cdot (x', y')) = t((xx' + \gamma \overline{y}'y, y\overline{x}' + y'x)) = (\overline{x}'\overline{x} + \gamma \overline{y}y', -y\overline{x} - y'x)
= (\overline{x}', -y')(\overline{x}, -y) = t((x', y'))t((x, y))
$$
したがって、$t$ は反自己同型です。

(iii) を証明することはまだ残っています。 E は F の部分代数と同一視されるため、E は結合すると仮定できます。 $u = (x, y)$、$u' = (x', y')$、$u'' = (x'', y'')$ を F の元とします。
$$
\begin{cases}
(uu')u'' = ((xx' + \gamma \overline{y}'y)x'' + \gamma \overline{y}''(\overline{y}x' + y'x), \\
\phantom{(uu')u'' = } (y\overline{x}' + y'x)\overline{x}'' + y''(xx' + \gamma \overline{y}'y)) \\
u(u'u'') = (x(x'x'' + \gamma \overline{y}''y') + (\gamma(x''\overline{y}' + \overline{x}'\overline{y}'')y, \\
\phantom{u(u'u'') = } y(\overline{x}''\overline{x}' + \gamma \overline{y}'y'') + (y'\overline{x}'' + y''x')x).
\end{cases}
$$
(27)

これらの式を調べると、E の可換性は F の結合性を意味することがわかります。逆に、F が結合性である場合、式 (27) に $y = y' = 0$、$x'' = 0$、および $y'' = e$ を適用すると、$(0, x'x) = (0, xx')$、つまり E のすべての $x, x'$ に対して $x'x = xx'$ が得られます。したがって、E は可換です。

注意また、上記の記法では、E の $x, y$ について、
$$
yj = j\overline{y}, \quad x(yj) = (yx)j, \quad (xj)y = (x\overline{y})j, \quad (xj)(yj) = \overline{y}xe
$$
(28)
$$
j^2 = e.
$$
(29)

Cayley 代数 $(\mathbf{F}, t)$ は、* $(\mathbf{E}, s)$ * によって定義* $\gamma$ の * Cayley 拡大と呼ばれます。

#### 例 {#alg-iii-s2-n5-exa-1 .statement tag=05Z3}

(1) $\mathbf{E} = \mathbf{A}$ (したがって $s = 1_A$) を取ると、代数 $\mathbf{F}$ は基底 $(e, j)$ の *2 次式 A-代数* ですが、$j^2 = \gamma e$ です。

(2) E を型* $(\alpha, \beta)$ の *二次代数として、E の基礎となる加群が $\mathbf{A}^2$ となり、標準基底には乗法表 (2) (no. 3) が入ります。 s を E の共役とします (no. 3, 命題 2)。次に、すべての $\gamma \in \mathbf{A}$ について、$\gamma$ によって定義された $(\mathbf{E}, s)$ の Cayley 拡大 F は、型* $(\alpha, \beta, \gamma)$ の *四元数代数と呼ばれ、no. 3、命題 1、命題によって *連想*されます。上記5;その基礎となる加群は$\mathbf{A}^4$で、$(e, i, j, k)$が$\mathbf{A}^4$の標準基底を表す場合、対応する乗法表は次の式で与えられます。
$$
\left\{\begin{array}{lll}
i^2 = \alpha e + \beta i, & ij = k, & ik = \alpha j + \beta k, \\
ji = \beta j - k, & j^2 = \gamma e, & jk = \beta \gamma e - \gamma i, \\
ki = -\alpha j, & kj = \gamma i, & k^2 = -\alpha \gamma e.
\end{array}\right.
$$
(30)

さらに、$u = \rho e + \xi i + \eta j + \zeta k$ ($\mathbf{A}$ に $\rho, \xi, \eta, \zeta$ がある) については、次のようになります ($t(u)$ の代わりに $\bar{u}$ を書き、$\mathbf{A}$ を $\mathbf{Ae}$ で識別します):

$$
\left\{
\begin{array}{l}
u = (\rho + \beta \xi)e - \xi i - \eta j - \zeta k \\
T_F(u) = 2\rho + \beta \xi \\
N_F(u) = \rho^2 + \beta \rho \xi - \alpha \xi^2 - \gamma (\eta^2 + \beta \eta \zeta - \alpha \zeta^2).
\end{array}
\right.
$$

二次代数 E の式を考慮すると、(28) と (29) から式 (30) が得られ、(23) と (24) から式 (31) が得られます。

次に、F の $u, v$ について、

$$
N_F(uv) = N_F(u)N_F(v)
$$

結合性と、F の $N_F(u)$ 属するから中心であるという事実により、$N_F(uv) = uv.\overline{uv} = uv(\overline{v}.\overline{u}) = u(v\overline{v})\overline{u} = (u\overline{u})(v\overline{v})$ が得られます。

四元数代数と同型の A-代数は *四元数代数* とも呼ばれます。このような代数の基底が乗法表 (30) を持つ場合、それは型* $(\alpha, \beta, \gamma)$ の *基底と呼ばれます。言葉の乱用により、四元数代数は、型 $(\alpha, \beta, \gamma)$ の基底を持つとき、* 型* $(\alpha, \beta, \gamma)$ であると言われます。

$\beta = 0$ のとき、式 (30) と (31) は次のように簡略化されます。

$$
\left\{
\begin{array}{lll}
i^2 = \alpha e, & ij = k, & ik = \alpha j, \\
ji = -k, & j^2 = \gamma e, & jk = -\gamma i, \\
ki = -\alpha i, & kj = \gamma i, & k^2 = -\alpha \gamma e,
\end{array}
\right.
$$

そして

$$
\left\{
\begin{array}{l}
\bar{u} = \rho e - \xi i - \eta j - \zeta k \\
T_F(u) = 2\rho \\
N_F(u) = \rho^2 - \alpha \xi^2 - \gamma \eta^2 + \alpha \gamma \zeta^2.
\end{array}
\right.
$$

次に、上記の式の $(\alpha, \beta, \gamma)$ は全体的に $(\alpha, \gamma)$ に置き換えられます。 型 $(\alpha, \gamma)$ と $(\gamma, \alpha)$ の四元数代数が *同型* であるのは明らかです。

式 (32) は、$\mathbf{A}$ で $-1 \neq 1$ の場合、F が可換でないことを示していることに注意してください。

*A を実数と $\alpha = \gamma = -1, \beta = 0$ の体 $\mathbf{R}$ とすると、対応する代数 F はハミルトニアン四元数 * の *代数と呼ばれ、$\mathbf{H}$ で表されます。 If $u = \rho e + \xi i + \eta j + \zeta k$ ($\rho, \xi, \eta, \zeta$ in $\mathbf{R}$) is an element $\neq 0$ in $\mathbf{H}$, the formula $u\bar{u} = \bar{u}u = \rho^2 + \xi^2 + \eta^2 + \zeta^2$ (cf. (34)) shows that $N(u) \neq 0$ in $\mathbf{R}$, so that $u$ admits an *inverse* $u^{-1} = N(u)^{-1}\bar{u}$ in $\mathbf{H}$ and that $\mathbf{H}$ is therefore a *non-commutative field*.

(3) E が四元数代数 (cf. *例 2*) であるとすると、元 $\delta \in \mathbf{A}$ によって定義される E の Cayley 拡大は一般に非結合的です

(命題5);これは、A 上の八元数代数 (cf. 付録, no. 3) と呼ばれます。

### 6. マグマ、モノイドの代数、群

マグマは合成 (I, § 1, no. 1) の法則を含む集合であることを思い出してください。 S を乗算的に書かれたマグマとし、E = A^{(S)} を S (II, § 1, no. 11) の形式的な線形結合の元の A-加群とします。 標準写像 s \mapsto e_s は S から A^{(S)} に定義されており、ファミリー (e_s)_{s \in S} は A^{(S)} の基底 (正規と呼ばれます) であり、A^{(S)} のすべての元は形 $\sum_{s \in S} \alpha_s e_s$ に一意に書き込まれます。 (\alpha_s) は、有限台の A の元の家族です。次に、A-代数構造は、標準基底の乗法表として E 上で定義されます。

$$
e_s e_t = e_{st}.
$$

このように定義された代数 E は、A 上のマグマ S の代数と呼ばれます。 $x = \sum_{s \in S} \xi_s e_s$ と $y = \sum_{s \in S} \eta_s e_s$ が E の 2 つの元である場合、

$$
xy = \sum_{s \in S} \left( \sum_{tu = s} \xi_t \eta_u \right) e_s.
$$

S がモノイド (それぞれ群) の場合、E は A 上のモノイド (それぞれ群) S の代数と呼ばれます。この場合、結合代数 (§ 1, no. 7) になります。同様に、S が可換モノイドの場合、その代数は結合的で可換です。最後に、マグマ S が単位元 u を認める場合、$e_u$ は代数 E の単位元です。 元 $e_u$ が自由であるため、A は E の部分代数 Ae_u と同一視されます。

When A \neq \{0\}, S is sometimes identified with its image under the injection s \mapsto e_s, so that an element of E is written as $\sum_{s \in S} \alpha_s s$; but this identification is not possible (without causing confusion) when S is written additively. そして、$e_s$の代わりに$e^s$と書かれることもよくあります。

B を他の可換環および $\rho : A \to B$ 環準同型とします。 A と B 上の同じマグマ S の代数 E = A^{(S)} と E' = B^{(S)} を考え、$(e_s)_{s \in S}$ と $(e'_s)_{s \in S}$ をそれぞれの標準基底とします。 代数 B^{(S)} は、A-線型写像 j の下で、すべての $s \in S$ に対して $j(e_s \otimes 1) = e'_s$ となるように、代数 A^{(S)} \otimes_A B がスカラーの環を B (II, § 1, no. 11, 系 3 ～ 命題 17)。

#### 命題 6 {#alg-iii-s2-prop-6 .statement tag=05Z4}

*S をマグマ、F A-代数と f 準同型とします*

S を乗法構造のみで F に変換します。すると、可換図式をレンダリングする A-代数準同型 $\bar{f}: A^{(S)} \to F$ が 1 つだけ存在します。

$$
\begin{array}{ccc}
S & \xrightarrow{f} & F \\
| & & | \\
A^{(S)} & \xrightarrow{\bar{f}} & F
\end{array}
$$

(左側の垂直矢印は標準写像 $s \mapsto e_s$)。

$\bar{f}: A^{(S)} \to F$ を、$\bar{f}(e_s) = \bar{f}(s)$ (II, § 1, no. 11、系 3 ～ 命題 17) となるような一意の A-加群準同型とします。 $\bar{f}$ が代数準同型であることを検証するだけで十分であり、そのためには、定義と仮定 $f(st) = f(s)f(t)$ の直後に続く $\bar{f}(e_s e_t) = \bar{f}(e_s) \bar{f}(e_t)$ を証明するだけで十分です。

命題 6 は、$A^{(S)}$ と標準写像 $s \mapsto e_s$ の順序対からなるが普遍写像問題 (集合理論, IV, § 3, no. 1) の解であるという事実を表します。 $\Sigma$ は、A-代数構造の種であり、S の準同型をその乗法法則のみで A-代数に$\alpha$ 写像したものです。

#### 系 {#alg-iii-s2-n6-cor-1 .statement tag=05Z5}

S, S' を 2 つのマグマとし、$g: S \to S'$ 準同型とします。すると、可換図式をレンダリングする A-代数準同型 $u: A^{(S)} \to A^{(S')}$ が 1 つだけ存在します。

$$
\begin{array}{ccc}
S & \xrightarrow{g} & S' \\
| & & | \\
A^{(S)} & \xrightarrow{u} & A^{(S')}
\end{array}
$$

(垂直矢印は標準写像)。

$f$ を合成写像 $S \xrightarrow{g} S' \to A^{(S')}$ とする命題を適用する 6 で十分です。

In particular, if T is a stable subset of the magma S (I, § 1, no. 4), the set of elements $\sum_{s \in T} \alpha_s e_s$ of $A^{(S)}$ is a subalgebra of $A^{(S)}$ canonically isomorphic to the algebra $A^{(T)}$ and sometimes identified with the latter.

#### 例 {#alg-iii-s2-n6-exa-1 .statement tag=05Z6}

V を A-加群とし、S を左辺の V に作用するモノイドとします。これは、(I, § 5, no. 1) S の写像 $(s, x) \mapsto s.x$ が V に与えられ、S の $s, t$ に対して $s.(x + y) = s.x + s.y, s.(\alpha x) = \alpha(s.x)$ と $s.(t.x) = (st).x$ が、V と $\alpha \in A$ で $x, y$ が与えられ、e で示されることを意味します。 S の単位元、例: x ∈ V の場合、x = x。 f(s)(x) = s.x と書くと、f は S の準同型から代数 End_A(V) (その乗法法則のみ)、写像単位元 e から単位元 l_V になります。 適用命題 6、A-代数準同型 $\bar{f}: A^{(S)} \to \mathrm{End}_A(V)$ が得られ、V 左加群構造の基礎となる群が $A^{(S)}$ に渡されます。

これにより、簡約する演算子を使用した可換群から加群の研究が可能になります。なぜなら、M を可換群とし、演算子は加法的に記述され、そのすべての外部法則は乗法的に記述されます。 $\Omega$ を、M 上のさまざまな外部法則の演算子のドメインの和集合 (集合理論, II, § 4, no. 8) とします。これらのドメインのそれぞれは、$\Omega$ の部分集合で正規に識別されます。 Mo($\Omega$) を $\Omega$ 上に構築された自由モノイド (I § 7, no. 2) とします。 法則/作用

$$
(s, x) \mapsto s.x
$$

は、Mo($\Omega$) の語の長さ上の帰納法によって、演算子の定義域として Mo($\Omega$) を使用して M 上に定義されます。 s が長さ 0 の場合、それは空の語 e であり、すべての $x \in M$ に対して $e.x = x$ と書きます。 x が長さ $n \geq 1$ である場合、それは $s = tu$ と一意に書くことができます。ここで、u は長さ $n - 1$ で、t は長さ 1 であるため、$t \in \Omega$ となります。次に、$s.x = t.(u.x)$と書きます。任意の 2 つの語について、Mo($\Omega$) の $s'$、関係 $s.(s'.x) = (ss').x$ は、s の長さ上の帰納法によって検証されます。

次に、上記の適用方法により、左の $\mathbf{Z}^{(Mo(\Omega))}$ モジュール構造が M 上で得られ、演算子 (安定な部分群、準同型) を使用した群の理論における通常の概念が、演算子と演算子を使用した可換群についても同じであることが問題なく検証されます。したがって、加群はそれらと関連付けられています。

### 7. 無料代数

#### 定義 2 {#alg-iii-s2-def-2 .statement tag=05Z7}

*Iを集合とします。 M(I) (それぞれ Mo(I)、それぞれ $\mathbf{N}^{(I)}$) を、I から導出された自由マグマ (それぞれ自由モノイド、それぞれ自由可換モノイド) を表すものとします。 A 上の M(I) (それぞれ Mo(I)、それぞれ $\mathbf{N}^{(I)}$) の代数は、自由代数 (それぞれ自由結合代数、それぞれ自由可換結合代数 (または、言葉の乱用により自由) と呼ばれます) 可換代数)) の集合 I 環 A.*

A 上の I の自由代数 (それぞれ自由結合代数、それぞれ自由可換代数) を Lib_A(I) (それぞれ Libas_A(I)、それぞれ Libasc_A(I)) で表すことにします。 By composing the canonical mapping of I into M(I) (resp. Mo(I), resp. $\mathbf{N}^{(I)}$) with the canonical mapping of M(I) (resp. Mo(I), resp. $\mathbf{N}^{(I)}$) into Lib_A(I) (resp. Libas_A(I), resp. Libasc_A(I)), a canonical mapping is obtained of I into Lib_A(I) (resp. Libas_A(I), resp. Libasc_A(I)), which is injective if $A \neq \{0\}$. この標準写像の下の元 $i \in I$ の像を $X_i$ で表し、$X_i$ は Lib_A(I) (または Libas_A(I)、それぞれ ) の添字 i の不定数であると言います。 Libasc_A(I))。

Mo(I) と $\mathbf{N}^{(I)}$ はそれぞれ単位元を持っているため、Libas_A(I) と Libasc_A(I) は単位結合代数であり、さらに Libasc_A(I) は可換です。 e が Libas_A(I) の単位元 (または Libasc_A(I)) である場合、写像 $\alpha \mapsto \alpha e$ は、Libas_A(I) の中心の部分環上の A の同型です。 Libasc_A(I))、A (no. 1) と識別されます。

#### 命題 7 {#alg-iii-s2-prop-7 .statement tag=05Z8}

*Let I be a set and F an algebra (resp. unital associative algebra, resp. unital commutative associative algebra) over A. すべての写像 $f : I \to F$ に対して、Lib_A(I) (それぞれ Libas_A(I)、それぞれ Libasc_A(I)) の準同型 (それぞれ Unital 準同型) $\bar{f}$ が F に存在します。 $\bar{f}(X_i) = f(i)$ 全員 $i \in I$.*

$F_m$ を、集合 F に合成の乗法法則を与えることによって得られるマグマ (それぞれモノイド) とします。 There is one and only one homomorphism (resp. unital homomorphism) $g$ of M(I) (resp. Mo(I), resp. $\mathbf{N}^{(I)}$) into $F_m$ such that $g(i) = f(i)$ for all $i \in I$ (I, § 7, nos. 1, 2 and 7); 命題 7 は、no. 6、命題 6 から続きます。

#### 注意 {#alg-iii-s2-n7-rem-1 .statement tag=05Z9}

(1) 後で、Libas_A(I) の定義する同型を自由加群 $A^{(I)}$ (§ 5, no. 5) のテンソル代数に、また Libasc_A(I) の同型を対称に配置します。 $A^{(I)}$ の代数 (§ 6, no. 6)。

(2) $\rho$ を A の準同型を可換環 B に統合したものとします。 ご覧のとおり (§ 2, no. 6)、同型 $\sigma$ は、Lib_B(I) (それぞれ Libas_B(I)、それぞれ Libasc_B(I)) の $\rho$ から代数 $(\mathrm{Lib}_A(I))_{(B)}$ に導出されます。 (それぞれ $(\mathrm{Libas}_A(I))_{(B)}$、それぞれ $(\mathrm{Libasc}_A(I))_{(B)}$) $\rho$ を使用してスカラーを B まで拡張することによって取得されます。 $X_i^A, X_i^B$ がそれぞれ A と B に対する添字 $i$ 対応するの不定数である場合、$\sigma(X_i^B) = X_i^A \otimes 1$ です。

(3) J を I の部分集合とします。 M(J) はマグマ M(I) の安定した部分集合と同一視され、したがって (no. 6) Lib_A(J) は $i \in J$ のような $X_i$ によって生成された Lib_A(I) の部分代数と標準的に同一視されることがわかっています。 Lib_A(J) の元には、添字所属から J までの不定数のみが現れると言われています。マグマの代数のno. 6で与えられた定義は、Jが*有限*の集合、Iの部分集合を通過するとき、Lib_A(I)が部分代数Lib_A(J)の有向族の和集合であることを示しています。 Libas_A(I) と Libasc_A(I) にも同様の結果があります。

(4) M(I) (それぞれ Mo(I)、それぞれ $\mathbf{N}^{(I)}$) の元には、その *長さ* $l(s)$、つまり整数 $\geqslant 1$ (それぞれ $\geqslant 0$) が関連付けられており、$l(ss') = l(s) + l(s')$ (I, § 7、番号 1、2、および 7)。 If $e_s$ is the element of Lib_A(I) (resp. Libas_A(I), resp. Libasc_A(I)) corresponding to s, the *total degree* (or simply the *degree* of an element $x = \sum_s \alpha_s e_s \neq 0$ of Lib_A(I) (resp. Libas_A(A), resp. Libasc_A(I)) is the greatest of the numbers $l(s)$ when s runs through the (non-empty by hypothesis) set of elements such that $\alpha_s \neq 0$. たとえば、$i, j, k$ が I の 3 つの異なる元である場合、元 $(X_i(X_jX_k))X_i - (X_iX_j)(X_kX_i)$ は、Lib_A(I) の合計次数 4 のうちの元 $\neq 0$ です。

### 8. 生成元と関係による代数の定義

F を A 上の代数とし、F の元の族を $(x_i)_{i \in I}$ とします。no. 7、命題 7 により、すべての $i \in I$ に対して $f(X_i) = x_i$ となる一意な準同型 $f : \mathrm{Lib}_A(I) \to F$ が存在します。 $f$ が全射であるためには、$(x_i)_{i \in I}$ が F の生成する系であることが必要かつ十分です。

$U \in \mathrm{Lib}_A(I)$ の場合、$f(U)$ は、不定数 $X_i$* を元 $x_i$ に置き換えて U から導出された F の *元と呼ばれるか、不定数の値 $x_i$ を U の *値* と呼ばれます。 $X_i$;通常は $U((x_i)_{i \in I})$ で表されます。特に$U((X_i)_{i \in I}) = U$。 $\lambda$ が A 上の F の準同型を代数 $F'$ にすると、
$$
\lambda(U((x_i)_{i \in I})) = U((\lambda(x_i))_{i \in I}).
$$

特に、J が他の集合である $F = \mathrm{Lib}_A(J)$ の場合を考えてみましょう。すべての家族 $(H_i)_{i \in I}$ の元の $\mathrm{Lib}_A(J)$ とすべての家族 $(y_j')_{j \in J}$ の元の A-代数 $F'$、
$$
U((H_i)_{i \in I}))((y_j')_{j \in J}) = U((H_i((y_j')_{j \in J})))_{i \in I}).
$$
(37)

上記の記法において、$U((x_i)_{i \in I}) = 0$、または$f(U) = 0$のような$\mathrm{Lib}_A(I)$のすべての元 Uは、Fの族$(x_i)_{i \in I}$の*リレーター*と呼ばれます。これら元の両側イデアル$\mathrm{Ker}(f)$からなるは、 $(x_i)$の*関係者の理想*。

$(R_j)_{j \in J}$ を $\mathrm{Lib}_A(I)$ の元の家族とします。 $(x_i)_{i \in I}$がFの生成する系であり、$R_j$によって生成される$\mathrm{Lib}_A(I)$の両面理想が家族$(x_i)_{i \in I}$の関係者の理想と等しい場合、$((x_i)_{i \in I}, (R_j)_{j \in J})$は代数Fの*プレゼンテーション*と呼ばれます。 $x_i$ は *生成元* と呼ばれ、$R_j$ はプレゼンテーションの *リレーター* と呼ばれます。

ここで、集合 I と $\mathrm{Lib}_A(I)$ の元の家族 $(R_j)_{j \in J}$ を考えてみましょう。家族$(R_j)$によって生成された両面理想による$\mathrm{Lib}_A(I)$の商代数Eは、関係者家族*$(R_j)_{j \in J}$によって関連付けられた生成する系Iによって定義される*普遍代数と呼ばれます。明らかに、$\overline{X}_i$ が E の $X_i$ の像を表す場合、
$$
((\overline{X}_i)_{i \in I}, (R_j)_{j \in J})
$$
さらに、$(x_i)_{i \in I}$ が代数 F の元とすべての $j \in J$ に対する $R_j((x_i)_{i \in I}) = 0$ の族である場合、すべての $i \in I$ に対して $g(\overline{X}_i) = x_i$ となるような一意な準同型 $g : E \to F$ が存在します。 $((x_i)_{i \in I}, (R_j)_{j \in J})$ が F の表現であるためには、$g$ が *全単射* であることが必要かつ十分です。

これらの注意は、次のような言葉の乱用を正当化します。 という 「*$((x_i)_{i \in I}, (R_j)_{j \in J})$ は F* の表現である」の代わりに、「*F は関係 $R_j((x_i)_{i \in I}) = 0$* の影響を受けて、生成元 $x_i$ によって生成された代数である」とも言われています。 $R_j$ が形 $P_j - Q_j$ のとき、「*F は関係 $P_j((x_i)) = Q_j((x_i))$* の影響を受ける $x_i$ によって生成される代数 」とも言われます。

H を集合とします。 $\mathrm{Lib}_A(H)$ の元 S は A-代数に対する *普遍的な * 関連子であり、F は集合をインデックスとする H を持つ F の元の *すべての * ファミリー $(x_h)_{h \in H}$ に対する $S((x_h)_{h \in H}) = 0$ であると言いましょう。

#### 例 {#alg-iii-s2-n8-exa-1 .statement tag=05ZA}

(1) $H = \{1, 2, 3\}$ を取る。認める代数
$$
(X_1 X_2) X_3 - X_1 (X_2 X_3)
$$
普遍的な関係者としては、連想的な代数が挙げられます。 $X_1 X_2 - X_2 X_1$を普遍関係者として認める代数は可換代数です。 *代数は普遍的な関係者 $X_1 X_1$ と
$$
(X_1 X_2) X_3 + (X_2 X_3) X_1 + (X_3 X_1) X_2
$$
普遍的な関係者としてはリー代数.*

Let I be a set; let a family $(S_k)_{k \in K}$ of elements of Lib_A(H) be given and consider the set T of elements of Lib_A(I) of the form $S_k((U_h))_{h \in H}$, where k runs through K and, for each k, $(U_h)_{h \in H}$ runs through the set of families of elements of Lib_A(I) with H as indexing set; consider a family $(R_j)_{j \in J}$ with T as set of elements. 次に、F をファミリー $(R_j)_{j \in J}$ に関連する生成する系 I によって定義される普遍的な代数とし、$u : \mathrm{Lib}_A(I) \to F$ を標準準同型とすることで、Ker(u) はすべての $k \in K$ とすべてのファミリーに対して元 $S_k((U_h)_{h \in H})$ によって生成されます。 Lib_A(I) の元の $(U_h)_{h \in H}$;明らかに、それぞれの $S_k$ ($k \in K$) は F の *普遍的な関係子* です。 ここで、F' を生成する系 $(x_i)_{i \in I}$ を認める代数とし、それぞれの $S_k$ を普遍関係子とし、$u' : \mathrm{Lib}_A(I) \to F'$ をすべての $i \in I$ に対して $u'(X_i) = x_i$ となるように準同型とします。明らかに Ker(u) $\subset$ Ker(u') であるため、$u'$ は形 $u' = h \circ u$ で一意に書くことができます。ここで、$h : F \to F'$ は準同型であるため、すべての $i \in I$ に対して $h(\overline{X}_i) = x_i$ になります。 この理由から、F は、普遍関係子* $(S_k)_{k \in K}$ の族に対する生成する系 I*、*対応するによって定義される *普遍代数と呼ばれます。 By an abuse of language, F is sometimes called the universal algebra generated by I and subject to the *identities* $S_k((u_h)) = 0$ for every family $(u_h)_{h \in H}$ of elements of F.

*例* 2. L' を I によって生成された普遍的な代数とし、3 人家族ごとに L の元をアイデンティティ $(uv)w - u(vw) = 0$ に従属させ、L'' を隣接することによって得られる代数とします。 単位元からL';その場合、すべての $i \in I$ に対して $g(\overline{X}_i) = X_i$ となるような、Libas_A(I) 上に L '' の一意の単位同型 g が存在します。なぜなら、明らかに L'' は結合的であり、準同型 g の存在は、L' の定義とその前の注意から続きます。しかし、明らかに L'' は、Libas_A(I)、よっての結論を特徴付ける普遍性 (no. 7, 命題 7) を満たします。

以下の注意を考慮して、上記と同様の考察を結合代数 (それぞれ可換結合代数) に適用できます。文脈が、代数が単一の代数であることを十分に示している場合、言葉の乱用により、代数 $F$ の元 $(x_i)_{i \in I}$ のファミリーは、$x_i$ ($i \in I$) と単位元によって生成される部分代数は次のようになります。 $F$ に等しいものは、$F$ の生成する系と呼ばれることがよくあります。次に、$F$ を $A$ 上の単位結合代数とし、$(x_i)_{i \in I}$ を $F$ の元の族とする。 no. 7、命題 7 により、すべての $i \in I$ に対して $f(X_i) = x_i$ となるような固有の単位準同型 $f : \mathrm{Libas}_A(I) \to F$ が存在します。 $U \in \mathrm{Libas}_A(I)$ の場合、$f(U)$ は、不定数 $X_i$ を元 $x_i$ に置き換えて$U$ から導出された $F$ の元とも呼ばれ、$U((x_i)_{i \in I})$ によっても表されます。次に、リレーター、プレゼンテーション、ユニバーサル リレーターの概念は、直ちに連想代数に移ります。単純に $\mathrm{Libas}_A(I)$ までに置き換える $\mathrm{Lib}_A(I)$ を実行するだけで十分です。 *関係者の家族によって関連付けられた、生成する系 I によって定義された普遍的単一結合代数* $(R_j)_{j \in J}$ は、家族 $(R_j)$ によって生成された両面理想によって $\mathrm{Libas}_A(I)$ の商代数です。 生成する系 $I$, 対応するによって普遍関係子の族に対して生成される普遍単位結合代数も同様に定義されます。 $\mathrm{Libas}_A(I)$ を $\mathrm{Libasc}_A(I)$ に置き換えて、可換結合代数に対して類似の定義を記述するタスクは読者に委ねられます。

#### 例 3 {#alg-iii-s2-n8-exa-3 .statement tag=05ZB}

$L'$ を、$I$ によって生成された普遍的単位連想代数とし、$L'$ の 2 人元の各家族の同一性 $uv - vu = 0$ に従うものとします。 *例 2* のように、$L'$ は正準的に $\mathrm{Libasc}_A(I)$ と同型であることがわかります。

### 9. 多項式代数

$B$ を単位 *可換* 結合 $A$-代数とし、$(x_i)_{i \in I}$ を $B$ の元の族とする。 $x_i$ ($i \in I$) と単位元によって生成される $B$ の部分代数は、混乱が生じない場合には $A[(x_i)_{i \in I}]_B$ または単に $A[(x_i)_{i \in I}]$ で表されます。 したがって、すべての集合 $I$ について、代数 $\mathrm{Libasc}_A(I)$ は $A[(X_i)_{i \in I}]$ ($A[X_i]_{i \in I}$ によっても示される) に等しくなります。後者の記法は、不定を表すために選択された記法を示すという利点があり、この論文の残りの部分で一般に使用するものです。 $A[(X_i)_{i \in I}]$ の元は、*不定多項式* $X_i$ ($i \in I$) *$A$ に係数を加えたものと呼ばれます。 「$A[(X_i)_{i \in I}]$を多項式代数にしよう」と言われるとき、$X_i$は常に不定数であると理解されるのが慣例です。 $I$ の部分集合 $J$ ごとに、上記の記法を使用すると、添字 $i \in J$ および単位元の $X_i$ によって生成された $\mathrm{Libasc}_A(I)$ の代数で $\mathrm{Libasc}_A(J)$ を識別することになります。 (cf. no. 7、*注意 (3)*)。 $I = \{1, 2, \ldots, n\}$ には、$A[(X_i)_{i \in I}]$ の代わりに $A[X_1, X_2, \ldots, X_n]$ と書きます。

$I$ と $I'$ が 2 つの等能性集合である場合、代数 $\mathrm{Libasc}_A(I)$ と $\mathrm{Libasc}_A(I')$ は同型です。 $A[X]$ は、一意の不定を表す *single* 元、$X$ を含む不特定のインデックス集合に対する多項式代数対応するを表すためによく使用されます。同様に、$A[X, Y]$、$A[X, Y, Z]$、... は、2、3、... 元による不特定のインデックス集合に対する多項式代数対応するを表すために使用されます。上記の規則により、たとえば、$A \neq \{0\}$ の場合、$A[X]$ と $A[Y]$ は、$A[X, Y, Z]$ の (別個の) 部分代数であることに注意してください。

元
$$
X^\nu = \prod_{i \in I} X_i^{\nu(i)},
$$
ここで、$\nu$ は、多項式代数 $A[(X_i)_{i \in I}]$ の $\mathbf{N}^{(I)}$ 形基底を通過します。これらの元は不定数$X_i$の*単項式*と呼ばれ、数$|\nu| = \sum_{i \in I} \nu(i)$は単項式$X^\nu$の*次数* (または*合計次数*)と呼ばれます。 次数 0 の一意の単項式は $A[(X_i)_{i \in I}]$ の単位元です。多くの場合、$A$ の 1 である単位元と識別されます。 $A[(X_i)_{i \in I}]$ のすべての多項式 $u$ は次のように一意に書くことができます。
$$
u = \sum_{\nu \in \mathbf{N}^{(I)}} \alpha_\nu X^\nu
$$
$\alpha_\nu \in A$付き。 元 $\alpha_\nu$、零は、添字 $\nu \in \mathbf{N}^{(I)}$ の有限数を除き、$u$ の *係数* と呼ばれます。 元 $\alpha_\nu X^\nu$ は、$u$ の *項* と呼ばれます (元 $\alpha_\nu X^\nu$ は、「$X^\nu$ の項」と呼ばれることがよくあります)。特に、項 $\alpha_0 X^0$ ($\alpha_0 \in A$ と識別される) は、$u$ の *定数項* と呼ばれます。 $J$が$I$の部分集合である場合、$\nu \notin \mathbf{N}^{(J)}$が$\alpha_\nu = 0$の場合に限り、$u$は属するから$A[(X_i)_{i \in J}]$になります。したがって、$A[(X_i)_{i \in I}]$ は部分代数 $A[(X_i)_{i \in J}]$ の和集合であり、$J$ は $I$ の有限部分集合の集合を通過します。 $|\nu| > n$ に対して $\alpha_\nu = 0$ の場合、$u$ は次数* $\leq n$ の * 多項式であると言われます。 $\alpha_\nu = 0$ が (言葉の乱用によって) $u$ が * $X^\nu$ で *含むいや項と言われたとき。特に、$\alpha_0 = 0$ の場合、$u$ は *定数項* を持たない多項式であると言われます。

すべての *非ゼロ* 多項式 $u = \sum \alpha_\nu X^\nu$ について、$u$ の *次数* (または *合計次数*) は、$\alpha_\nu \neq 0$ などの複数インデックス $\nu$ の整数 $|\nu|$ の最大のです。

$F$ を単位結合 $A$-代数とし、$(x_i)_{i \in I}$ を *ペアごとに置換可能*な $F$ の元の族とする。 The subalgebra $F'$ of $F$ generated by the $x_i$ and the unit element is commutative (§ 1, no. 7), which allows us to define substituting the $x_i$ for the $X_i$ in the polynomial $u \in A[(X_i)_{i \in I}]$ (although $F$ is not necessarily commutative): $u((x_i)_{i \in I})$ is an element of $F'$ and therefore of $F$ and $h: u \to u((x_i)_{i \in I})$ is a homomorphism of $A[(X_i)_{i \in I}]$ into $F$. The elements of the kernel of $h$ are the relators of the family $(x_i)$ in $A[(X_i)_{i \in I}]$, also called *polynomial relators* (with coefficients in $A$) between the $x_i$. 準同型 $h$ の像は部分代数 $F'$ であり、$A[(x_i)_{i \in I}]$ でも表されます ($F$ が可換でない場合でも)。 $a$ が $x_i$ の間の多項式関係子のイデアルである場合、$A$ モジュールの完全系列が存在します。
$$
0 \longrightarrow a \longrightarrow A[(X_i)_{i \in I}] \xrightarrow{h} A[(x_i)_{i \in I}] \longrightarrow 0.
$$

#### 命題 8 {#alg-iii-s2-prop-8 .statement tag=05ZC}

*Let $A[(X_i)_{i \in I}]$ be a polynomial 代数, $J$ 部分集合 of $I$ and $K$ the complement of $J$ in $I$. $A' = A[(X_j)_{j \in J}]$ と書いて $X'_k$ ($k \in K$) で表すと、多項式代数 Libasc_{A'}(K) = A'[(X'_k)_{k \in K}] における * 不定数が存在し、固有の環同型が存在します。 A'[(X'_k)_{k \in K}] を A[(X_i)_{i \in I}] に変換すると、A' の恒等性をもつ一致すると、すべての k \in K について X_k に写像 X'_k が変換されます。

明らかに、A[(X_i)_{i \in I}] は、k \in K に対する X_k によって生成された A'-代数です。一方、X_k (k \in K) と A' の係数の間の多項式関係子として、一意に $\sum_v h_v((X_j)_{j \in J}) X^v$ と書くことができます。ここで、v は $\mathbf{N}^{(K)}$ の有限部分集合を通過します。 h_v は A[(X_j)_{j \in J}] の元であり、h_v は A の係数を含む X_j 間の多項式関係子でなければならず、したがってすべて零であり、これは命題を証明します。

命題 8 で説明した同型は、A' = A[(X_j)_{j \in J}] の係数を含む多項式を使用した A[(X_i)_{i \in I}] の同一視する元によく使用されます。 u が A[(X_i)_{i \in I}] の元 $\neq 0$ である場合、A'[(X_k)_{k \in K}] の元とみなされるその合計次数は、添字 i \in K の X_i に関してその次数とも呼ばれます。

#### 注意 {#alg-iii-s2-n9-rem-1 .statement tag=05ZD}

I と J を 2 つの集合とし、(P_j)_{j \in J} を $\mathbf{Z}[(X_i)_{i \in I}]$ の元の族とします。 Q が $Q((P_j)_{j \in J}) = 0$ となるような $\mathbf{Z}[(X_j)_{j \in J}]$ の元である場合、すべての族 $(b_i)_{i \in I}$ のペアごとに置換可能な環の元 B、
$$
Q((P_j((b_i)_{i \in I}))_{j \in J}) = 0.
$$
形 $Q((P_j)_{j \in J}) = 0$ が成立する関係はときどき多項式恒等式と呼ばれます。たとえば
$$
(X_1 + X_2)^2 - X_1^2 - X_2^2 - 2X_1X_2 = 0
$$
と
$$
Q = Y_1^2 - Y_2, \quad P_1 = X_1 + X_2, \quad P_2 = X_1^2 + X_2^2 + 2X_1X_2
$$
$$
X_1^n - X_2^n - (X_1 - X_2)(X_1^{n-1} + X_1^{n-2}X_2 + \cdots + X_2^{n-1}) = 0
$$
と
$$
Q = Y_1 - Y_2Y_3, \quad P_1 = X_1^n - X_2^n, \quad P_2 = X_1 - X_2,
$$
$$
P_3 = X_1^{n-1} + X_1^{n-2}X_2 + \cdots + X_2^{n-1}
$$
は多項式恒等式です。

### 10. モノイドの合計代数

A 上のモノイド S の代数は、(A-加群のように) 積の $A^S$ からなるの族 $(\alpha_s)_{s \in S}$ の有限台の部分加群です。この代数の乗法は関係 $(\alpha_s)(\beta_s) = (\gamma_s)$ によって定義されます。ここで、すべての $s \in S$ について、
$$
\gamma_s = \sum_{tu = s} \alpha_t \beta_u
$$

(cf. no. 6、公式 (35))。 (38) の右辺の和が意味を持つのは、$(\alpha_s)$ と $(\beta_s)$ が有限台のファミリーであり、従って二重ファミリー $(\alpha_t\beta_u)_{(t,u)\in S\times S}$ であるためです。しかし、(38) の右辺は、モノイド $S$ が次の条件を満たすとき、$A^S$ の *任意の* 元 $(\alpha_s),\ \beta_s)$ にとっても意味があります。

(D) *すべて* $s\in S$ について、*順序付けられた対* $(t,u)$ * $S\times S$ * のような* $tu=s$ の有限数のみが存在します。

次に、$S$ が条件 (D) を満たすと仮定します。 乗法法則は、公式によって積 A-加群 $A^S$ で定義できます (38)。 $A^S$ でこのように定義された乗法が A 双線形であるのは明らかです。また、$A^S$ の $\alpha,\beta,\gamma$ については、*連想* です。

$$
\sum_{uvw=t} \alpha_u\beta_v\gamma_w = \sum_{rw=t} \left( \left( \sum_{uv=r} \alpha_u\beta_v \right) \gamma_w \right) = \sum_{us=t} \left( \alpha_u \left( \sum_{vw=s} \beta_v\gamma_w \right) \right).
$$

この $A^S$ 上の乗法と A-加群構造は、したがって $A^S$ 上の定義するは A 上の単体 *結合代数* 構造です。 集合 $A^S$ は、この構造と合わせて、A 上のモノイド S の *合計代数* であると言えます。

A 上のモノイド S の *代数* $A^{(S)}$ (混乱を避けるために必要な場合は S の *制限された代数* とも呼ばれます) は、A 上の S の合計代数の *部分代数* であることは明らか (S が有限である場合、後者と同一です)。 *言葉の乱用*により、A 上の S の合計代数のすべての元 $(\xi_s)_{s\in S}$ は、S の制限された代数の元と同じ記法 $\sum_{s\in S} \xi_s e_s$ (または $\sum_{s\in S} \xi_s s$) で表されます。もちろん、この記法対応するに現れる合計記号は、代​​数的な演算ではなく、一般に項 $\neq 0$ の *無限* を引き継ぐからです。この記法により、Sの合計代数の乗法もno. 6の公式(35)で与えられます。

S が可換であれば、その合計代数 $A^S$ も可換です。 T が S の部分モノイドである場合、モノイドの合計代数 $A^T$ は、S の合計代数の部分代数と正準的に識別されます。 $\rho : A \to B$ が環準同型である場合、正準拡大 $\rho^S : A^S \to B^S$ はA 上の S の合計代数から B 上の S の合計代数への A 準同型性、つまり拡大する標準準同型 $A^{(S)} \to B^{(S)}$。

### 11. フォーマル冪系列可換環

集合 I ごとに、加法モノイド $N^{(I)}$ は no. 10 の条件 (D) を満たします。 I の有限部分集合 H の添字 $i$ を除く $s = (n_i)_{i\in I}$ と $n_i = 0$ の場合、関係 $s = t + u$ と $t = (p_i)_{i\in I}$ および $u = (q_i)_{i\in I}$ はすべての$p_i + q_i = n_i$ と同等です。 $i$;しかし、これは、$i \notin H$ の場合は $p_i = q_i = 0$、$i \in H$ の場合は $p_i \leq n_i, q_i \leq n_i$ を意味します。したがって、$N^{(I)}$ では $\prod_{i\in H} (n_i + 1)$ が対 $(t, u)$ に順序付けされ、$t + u = s$ になります。

したがって、$A$ 上のモノイド $\mathbf{N}^{(I)}$ の合計代数は、このモノイドの (制限された) 代数 $A[\mathbf{X}_i]_{i \in I}$ 含むと考えることができます。それは、$A$ の係数を伴う不確定項 $X_i \ (i \in I)$ の形式冪系列の代数と呼ばれる単位可換結合代数であり、$A[[\mathbf{X}_i]]_{i \in I}$ で示されます。その元は、$A$ の係数とともに不定形 $X_i \ (i \in I)$ で正式な冪系列と呼ばれます。このような元 $(\alpha_v)_{v \in \mathbf{N}^{(I)}}$ は、no. 10 で定められた規則に従って、$\sum_{v \in \mathbf{N}^{(I)}} \alpha_v X^v$ によって表されることもあります。 $\alpha_v$ は正式な冪系列の係数であり、$\alpha_v X^v$ はその項です。したがって、$X_i$ の多項式は、項 $\neq 0$ の有限数のみを含む形式的な冪系列です。

明らかに、代数同型 $A[[\mathbf{X}_i]]_{i \in I_1} \to A[[\mathbf{X}_i]]_{i \in I_2}$ は、すべての全単射 $\sigma : I_1 \to I_2$ から、写像の正式な冪系列 $\sum_{(n_i)} \alpha_{(n_i)} \cdot \prod_{i \in I_1} X_i^{n_i}$ から正式な冪系列 $\sum_{(n_i)} \alpha_{(n_i)} \cdot \prod_{i \in I_1} X_{\sigma(i)}^{n_i}$ までが正規に導出されます。

Let $J$ be a subset of $I$; the algebra $A[[\mathbf{X}_i]]_{i \in J}$ can be identified with a subalgebra of $A[[\mathbf{X}_i]]_{i \in I}$ consisting of the formal power series $\sum_{(n_i)} \alpha_{(n_i)} \cdot \prod_{i \in I} X_i^{n_i}$ where $\alpha_{(n_i)} = 0$ for every element $(n_i) \in \mathbf{N}^{(I)}$ such that $n_i \neq 0$ for at least one index $i \in I - J$. さらに、$K = I - J$ の場合、形式的な冪系列 $\sum_{(n_i)} \alpha_{(n_i)} \cdot \prod_{i \in I} X_i^{n_i}$ を形式的な冪系列 $\sum_{(m_k)} \beta_{(m_k)} \cdot \prod_{k \in K} X_k^{m_k}$ と識別することにより、$A[[\mathbf{X}_i]]_{i \in I}$ は正規的に $(A[[\mathbf{X}_j]]_{j \in J})[[\mathbf{X}_k]]_{k \in K}$ と識別されます。
$$
\beta_{(m_k)} = \sum_{(p_j)} \gamma_{(p_j)} \cdot \prod_{j \in J} X_j^{p_j}
$$
数列 $(n_i)$ は $\gamma_{(p_j)} = \alpha_{(n_i)}$ で、$i \in J$ は $n_i = p_i$、$i \in K$ は $n_i = m_i$ になります。

正式な冪系列 $u = \sum_v \alpha_v X^v$、項 $\alpha_v X^v$ が与えられると、$|v| = p$ は合計次数 $p$ の $u$ で項と呼ばれます。合計次数 $p$ のうち項が $u$ であり、残りの項が零である正式な冪系列 $u_p$ は、$u$ の同次部分と呼ばれます。 次数 $p$; $I$ が有限の場合、$u_p$ はすべての $p$ に対する多項式になります。 $u_0$ は、$A$ の元と識別されます ($u$ の定数項とも呼ばれます)。 $u$ と $v$ が 2 つの正式な冪系列と $w = uv$ である場合、
$$
w_p = \sum_{r=0}^p u_r v_{p-r}
$$
整数 $p \geq 0$ごとに。

すべての正式な冪系列 $u \neq 0$ に対して、$u_p \neq 0$ となるような最小の整数 $p \geq 0$ を、$u$ の合計位数 (または単に位数) と呼びます。この位数を $\omega(u)$ で表し、$u$ と $v$ を 2 つの正式な冪系列 $\neq 0$ とすると、
$$
\omega(u + v) \geq \inf(\omega(u), \omega(v)) \quad \text{if } u + v \neq 0 \\
\omega(uv) \geq \omega(u) + \omega(v) \quad \text{if } uv \neq 0.
$$

さらに、$\omega(u) \neq \omega(v)$ の場合、必然的に $u + v \neq 0$ となり、(40) の両辺は等しくなります。

0 の位数は *定義されていない*ことに注意してください。 By an abuse of language, it is a convention to say that "f is a formal power series of order $\geq p$ (resp. $> p$)" if the homogeneous part of f of degree n is zero for all $n < p$ (resp. $n \leq p$); 0 is therefore a "formal power series of order $> p$" for *every* integer $p \geq 0$.

J を I の部分集合とし、$A[[X_i]]_{i \in I}$ を上記のように $B[[X_k]]_{k \in K}$ で識別するとします。ここで、$K = I - J$ と $B = A[[X_j]]_{j \in J}$ です。 対応する上記の定義を $B[[X_k]]_{k \in K}$ に適用すると、正式な冪系列 $u \in A[[X_i]]_{i \in I}$ には新しい定義が追加されます。 項 $\alpha_{(n_i)} \cdot \prod_{i \in I} X_i^{n_i}$ は、添字の $X_i$ の * 次数 p であると言われます* $\sum_{i \in K} n_i = p$ の場合、$i \in K$ と、同じ項を持つ$B[[X_k]]_{k \in K}$ の正式な冪系列次数 $p$ は、$u$ と他の零は、添字* $i \in K$ の $X_i$ における次数 p の同次部分と呼ばれます。 $u \neq 0$ の場合、添字 $i \in K$ の $X_i$ に対する *位数* $\omega_K(u)$ は、整数 $p \geq 0$ の最小のであるため、$u$ の同種部分添字 $i \in K$ の $X_i$ の次数 $p$ は $\neq 0$ です。 $\omega$ を $\omega_K$ に置き換えても、不等式 (40) と (41) は維持されます。

### 練習問題 {#alg-iii-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
