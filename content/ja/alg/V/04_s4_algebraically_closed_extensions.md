---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 4
section_title: Algebraically closed extensions
lang: ja
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.19-A V.24, A V.150
pdf_pages: 0133-0138, 0264-0264
extraction: ocr
subsections:
    - "no": 1
      title: Algebraically closed fields
      page: 19
      pdf_page: 133
    - "no": 2
      title: Splitting extensions
      page: 21
      pdf_page: 135
    - "no": 3
      title: Algebraic closure of a field
      page: 22
      pdf_page: 136
statements: 20
exercises: 2
content_sha256: 53057f614a43a7f262acba5a458ee37e82e86835bb7af1d612a963b5cd48f1d2
translated_from: content/en/alg/V/04_s4_algebraically_closed_extensions.md
translation_method: google
source_content_sha256: 532bb2954789915d393a9084c98ffe495892d82e18cded4cc49d55be2b67ab31
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 9ff05312eb65f2a26abad5ea8997b860182157cecf39a88352a09417580f5025
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 4。 代数閉拡大

### 1. 代数閉体

#### 命題 1 {#alg-v-s4-prop-1 .statement tag=06ID}

— K を体とします。この場合、次のプロパティは同等です。
(AC) K[X] の K[X] 分裂のすべての非定数多項式を次数 1 の多項式の積に変換します (区別できるかどうか)。
(AC') K[X] のすべての非定数多項式は、K に少なくとも 1 つの根を持ちます。
(AC'') K[X] の既約多項式はすべて次数 1 です。

(AC) K のすべての代数拡大は次数 1 です (他の語では、K は K のすべての拡大体で比較的代数的に閉じています)。

まず、性質 (AC)、(AC')、(AC'') の同値を証明しましょう。明らかに (AC) は (AC) を意味します。 K[X] のすべての非定数多項式は既約多項式 (IV, p. 13、提案 13) で割り切れ、K[X] の次数 1 のすべての多項式は明らかに K の根を認めているため、(AC) は (AC') を含意していることがわかります。 条件 (AC') は、n 上の帰納法によって、K[X] の次数 n のすべての多項式が次数 1 (IV, p. 14, 定数 1) の n 個の多項式のうちの積であることを意味します。したがって、(AC') (AC) を意味します。

(AC) と (AC) が同等であるかどうかはまだわかりません。 (AC'') が成り立つ場合、K の拡大体 L のすべての元は、K に対して代数的である次数 1 (V, p. 16, Th. 1) となり、したがって K に対して属するとなり、(AC) が成立します。逆に、f を K[X] の次数 $n \geq 1$ の既約多項式とする。 商代数 K[X]/(f) は K 上の次数 n であり、体であるため、K の次数 n の代数拡大 (V, p. 18、提案 2)。これで、(AC) が (AC'') を意味することは明らかです。

#### 定義 1 {#alg-v-s4-def-1 .statement tag=06IE}

体 K は、(等価な) 性質 (AC)、(AC')、(AC)、(AC) を持つ場合、代数的に閉じていると言われます。

\* 例 1. — 複素数の体 C は代数的に閉じています (Gen. Top.、VIII、p. 100)。 \*

K の拡大体 E で相対的に代数的に閉じている体 K は、必ずしも代数的に閉じているわけではありません (実際には、すべての体はそれ自体で相対的に代数的に閉じており、代数的に閉じていない体が存在します。たとえば、Q や $\mathbf{F}_p$ \* または R *)。しかし：

#### 命題 2 {#alg-v-s4-prop-2 .statement tag=06IF}

$\Omega$ を代数閉体とし、$\Omega$ の K 部分体とします。すると、$\Omega$におけるKの相対代数閉包$\bar{K}$は代数閉体になります。

f を $\bar{K}[X] \subset \Omega[X]$ の非定数多項式とする。 $\Omega$ は代数的に閉じているため、多項式 f は $\Omega$ に少なくとも 1 つの根を持ち、この根は $\bar{K}$ に対して代数的であるため、属するから $\bar{K}$ になります (V、p. 19、提案 4)。したがって、$\bar{K}$ は (AC') を満たします。

\* 例 2. — 提案 2 により、Q 上の代数であるすべての複素数 (しばしば簡単に代数数と呼ばれます) の集合は代数閉体です。 \*

#### 命題 3 {#alg-v-s4-prop-3 .statement tag=06IG}

すべての代数閉体は無限です。

Kを有限体とし、$f(X) = 1 + \prod_{a \in K} (X - a)$とします。 The polynomial $f \in K[X]$ is non-constant and $f(a) = 1$ for each $a \in K$. So 体 K does not 満たす (AC') and hence is not algebraically closed.

#### 定理 1 (シュタイニッツ) {#alg-v-s4-thm-1 .statement tag=06IH}

K を体、E を K の代数拡大、K の $\Omega$ 代数閉拡大とします。この場合、E から R への K 準同型性が存在します。

V、p. 13、Scholium により、$\Omega$ の拡大体 $\Omega'$ と E の $\Omega'$ への K 準同型性 u が存在します。 $x \in E$ にしましょう。 x は K に対して代数的であるため、u(x) は u(K) に対して代数的であり、*なおさら* は $\Omega$ (V, p. 17, Cor. 2) に対して代数的です。 $\Omega$ は代数的に閉じているため、$u(x) \in O$ になります。したがって、$u$ 写像 $E$ は $O$ になります。

### 2. 分裂拡大

#### 定義 2 {#alg-v-s4-def-2 .statement tag=06II}

*K を $K[X]$ の非定数多項式の族である体および $(f_i)_{i \in I}$ とします。 $(f_i)_i$ の分裂拡大により、以下の特性を持つ $K$ の拡大 $E$ が理解されます:*

*a) 各 $i \in I$ について、$E[X]$ の多項式 $f_i$ 分裂を次数 1 の多項式の積に変換します。*

*b) それぞれの $i \in I$ について、$R_i$ を $E$ の $f_i$ の根の集合とし、その後 $E = K \left( \bigcup_{i \in I} R_i \right)$ とします。*

ときどき項 « 分解体 » が « 分裂拡大 » の代わりに使用されます。

#### 注意 {#alg-v-s4-n2-rem-1 .statement tag=0EEN}

*1) それぞれの $i \in I$ について、$c_i$ を $K$ の非ゼロ元とし、$f'_i = c_i f_i$ とします。すると、家族 $(f_i)_i$ のすべての分裂拡大は家族 $(f'_i)_{i \in I}$ にとっても分裂拡大であり、その逆も明らかです。特に、分裂拡大を研究する際には、モニック多項式の場合を極限理解することができます。*

*2) Iが有限であるとして、$f = \prod_{i \in I} f_i$を置きます。多項式の分解の一意性を $E[X]$ の既約因子に使用すると (IV, p. 13、提案 13)、多項式 $f$ の分裂拡大が次のとおりであることを簡単に示すことができます。 分裂拡大家族のための $(f_i)_i$ そしてその逆。他の語では、有限族の場合は単一の多項式の場合に還元される可能性があります。*

*3) $f \in K[X]$ を次数 $\geq 1$ の多項式とし、$E$ を $f$ の分裂拡大とします。 $x_1, \ldots, x_n$ が $E$ で根オフである場合、$E = K(x_1, \ldots, x_n)$ があり、$[E : K]$ は有限です ($V$, p. 18, Th. 2)。しかし、$E$ が単一の根によって生成された部分体 $K(x_1), \ldots, K(x_n)$ とは異なる場合もあります。これは、$f$ が既約$^1$ である場合でも発生する可能性があります。ただし、$f$ が既約の場合、体 $K(x_i)$ はすべて、$K$ に対して同じ次数 $n$ を持ち、$E$ がそれらの 1 つと等しいときはいつでも、$[E : K] = n$ があり、したがって $E = K(x_1) = \cdots = K(x_n)$ となることに注意してください。

#### 命題 4 {#alg-v-s4-prop-4 .statement tag=06IJ}

*K を $K[X]$ の非定数多項式の族である体および $(f_i)_{i \in I}$ とします。その場合、家族 $(f_i)_{i \in I}$ には分裂拡大が存在します。*

多項式 $f_i$ をモニック (注意 1) とみなすことができます。 $i \in I$ とし、$f_i$ の次数を $d_i$ とします。 IV、p. 73、提案 5 により、0 に減らされない $K$ 上の可換代数 $A$ と、次のような $A_i$ の要素 $\xi_{i,1}, \ldots, \xi_{i,d_i}$ が存在します。

*a) 代数 $A_i$ は $(\xi_{i,1}, \ldots, \xi_{i,d_i})$ によって生成されます;*

(1) $K = \mathbf{Q}$ と $f = X^3 - 2$ を例に考えます。

b) $A_i[X]$ に $f_i(X) = \prod_{k=1}^{d_i} (X - \xi_{i,k})$ があります。

$A$ を代数 $(A_i)_{i \in I}$ の家族のテンソル積とし、$\varphi_i$ を $A_i$ の標準準同型として $A$ (III, p. 470) とします。 代数 $A$ は可換であり、0 には減りません。クルールの定理 (I, p. 104) によれば、$A$ には最大理想$a$ が存在し、$E = A/a$ は体 $K$ の拡大です。

$A$ の $E$ への正準準同型性を $\psi$ で表し、$i \in I$ と $l \leq k \leq d_i$ に $x_{i,k} = \psi(\varphi_i(\xi_{i,k}))$ を代入します。 代数 $A$ は $\bigcup \varphi_i(A_i)$ によって生成されるため、拡大 $E$ は家族 $(x_{i,k})$ によって生成されます。 さらに、$i \in I$があります

$$
f_i(X) = \prod_{k=1}^{d_i} (X - x_{i,k}) \text{ in } E[X]. $$

したがって、$E$ は、家族 $(f_i)_{i \in I}$ の分裂拡大です。

#### 命題 5 {#alg-v-s4-prop-5 .statement tag=06IK}

— *K を、K の $K[X]$、E 拡大、およびそれぞれ $(f_i)_{i \in I}$ の分裂拡大である E の部分拡張である F、F' の非定数多項式の族、K を体、$(f_i)_{i \in I}$ とします。次に$F = F'$。

$R_i$ を E の $f_i$ と $R = \bigcup_{i \in I} R_i$ の根の集合とします。 $f_i$ は、$F[X]$ にある最初の多項式次数の積なので、$R_i \subset F$ になります。デフによる。 2、$F = K(R)$があります。同じようにして $F = K(R)$ を見つけます。

#### 系 {#alg-v-s4-n2-cor-1 .statement tag=06IL}

— *K を、$K[X]$ の非定数多項式の族である体 $(f_i)_{i \in I}$ と、$(f_i)_{i \in I}$ の拡張拡張である F、F' とします。 このとき、F に対する F の K 同型写像が存在します。

これは、提案 5 およびV、p. 13、Cor. から導き出されます。提案4の。

### 3. 体中代数閉包

#### 定義 3 {#alg-v-s4-def-3 .statement tag=06IM}

— *K を体とします。 K の代数閉包によって、代数的かつ代数的に閉じた K の任意の拡大を理解できます。

#### 例 1 {#alg-v-s4-n3-exa-1 .statement tag=06IN}

体 C の複素数は体の代数閉包実数の R (Gen. Top.、VIII、p. 100) \*

#### 例 2 {#alg-v-s4-n3-exa-2 .statement tag=06IO}

K を K の体と $\Omega$ 代数閉拡大とします。$\overline{K}$ が $\Omega$ における K の相対代数閉包である場合、V、p. 20、提案 2 により、K は K の代数閉包になります。 \* 特に体すべての代数数 (V、p. 20、例 2) は、有理数数の体 Q の代数閉包です。 \*

#### 命題 6 {#alg-v-s4-prop-6 .statement tag=06IP}

— *$\Omega$ を体 K の拡大とします。 $\Omega$ が K の代数閉包であるためには、それが代数的であること、および $K[X]$ の各非定数多項式が、$\Omega[X]$ の分裂を次の積に変換することが必要かつ十分です。 因子/次数 1.

条件は(AC)で必要となります。逆に、$\Omega$ が $K$ 上の代数であり、$K[X]$ 上のすべての非定数多項式が次数 1 の因子の $\Omega[X]$ の積であるとします。 $\Omega'$ を次の代数拡大とします。 $\Omega$ そして$x \in \Omega'$ にしましょう。 $x$ は $\Omega$ に対して代数的であり、$\Omega$ は $K$ に対して代数的であるため、$x$ は $K$ に対して代数的です (V、p. 19、提案 3)。 $f$ を $K$ 上の $x$ の最小多項式とします。 仮定により、$\Omega[X]$ の多項式 $f \in K[X]$ 分裂は、次数 1、よって $x \in \Omega$ の因子の積に変換されます。したがって、$\Omega' = \Omega$ が得られ、$\Omega$ は (AC) を満たすため代数的に閉じられます。

#### 注意 1 {#alg-v-s4-n3-rem-1 .statement tag=06IQ}

$\Omega$ が $K$ に対して代数的であり、$K[X]$ のすべての非定数多項式が $\Omega$ に根をもつ場合、$\Omega$ は $K$ の代数閉包になります (V、p. 156、例 20)。

#### 命題 7 {#alg-v-s4-prop-7 .statement tag=06IR}

— *$\Omega$を体$K$の代数拡大とします。
a) $\Omega$ が代数的に閉じている場合、$K$ のすべての代数拡大は $\mathbf{R}$ の部分拡張と同型です。
b) 逆に、$K$ の有限次数のすべての代数拡大が$\Omega$ の部分拡張と同型であると仮定します。この場合、$\Omega$ は代数的に閉じています。*

主張 *a)* は Th から続きます。 1 (V、p. 20)。ここで *b)* の仮説を仮定し、非定数多項式 $f \in K[X]$ を考えてみましょう。 E を $f$ の分解体とします (V、p. 21、提案 4)。 E は $K$ (V, p. 18, Th. 2) 上の有限次数の代数であるため、E は $\Omega$ の部分拡張であると仮定できます。このとき、多項式 $f$ は $\Omega[X]$ の次数 1 の多項式の積であり、提案 6 は $\Omega$ が代数的に閉じていることを示しています。

これで、体の代数閉包の存在と一意性（同型まで）が証明できました。

#### 定理 2 (シュタイニッツ) {#alg-v-s4-thm-2 .statement tag=06IS}

— *$K$ を体とします。その場合、$K$の代数閉包が存在します。 $\Omega$ と $\Omega'$ が $K$ の 2 つの代数閉包である場合、 $\Omega'$ に対する $\Omega$ の $K$ 同型写像が存在します。

提案 6 によると、$K$ の代数閉包は、$K[X]$ のすべての非定数多項式の集合に対する分裂拡大に他なりません。 Th.したがって、2 は、V、p. 21、提案 4 およびV、p. 22、Cor. から導き出されます。

#### 系 {#alg-v-s4-n3-cor-1 .statement tag=06IT}

— *$K$と$K'$を、$K$の体、$\Omega$代数閉包、$K'$の$\Omega'$代数閉包を2つとします。 $K$ の $K'$ へのすべての同型 $u$ に対して、$u$ を拡張する $\Omega'$ への $\Omega$ の同型 $v$ が存在します。

Thを適用するだけで十分です。 2から代数閉包$\Omega$と$K$の$(\Omega', u)$。

#### 注意 2 {#alg-v-s4-n3-rem-2 .statement tag=06IU}

前述の系の記法には、同一性とは異なる一般に $\Omega$ の $K$ 自己同型が存在します。 したがって、$\Omega$ の同型性 $v$ の $\Omega'$ への同型性 $K$ の同型性 $u$ の $K'$ への拡張については、一般に一意性はありません。 同様の理由で、一般に、多項式の同じ族 $(f_i)_{i \in I}$ に対して、分裂拡大 $E'$ 上に分裂拡大 $E$ の 2 つ以上の同型が存在します。 対照的に、完全な閉包には一意性 (V, p. 5) があることを思い出してください。

#### 注意 3 {#alg-v-s4-n3-rem-3 .statement tag=06IV}

K を $K$ の体と $\Omega$ 代数閉包とします。 次に、$K[X]$ の非定数多項式の族 $(f_i)_{i \in I}$ の分割拡張に対して次の構成が与えられます。$R_i$ を $\Omega$ の $f_i$ の根の集合とし、$R = \bigcup_{i \in I} R_i$ とします。 このとき、$K(R)$ は $\Omega$ の一意の部分拡張であり、$(f_i)_{i \in I}$ の分裂拡大 (V、p. 22、提案 5) です。

#### 注意 4 {#alg-v-s4-n3-rem-4 .statement tag=06IW}

K を $K$ の有限体と $\Omega$ 代数閉包とします。この場合、$\Omega$ は無限大です ($V,$ p. 20、提案 3)。 K の有限次数のすべての拡大は有限体であるため、$\Omega$ は *無限* 次数の $K$ の代数拡大です。

### 練習問題 {#alg-v-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
