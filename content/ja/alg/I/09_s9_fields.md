---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 9
section_title: Fields
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 114-118, 174-179
pdf_pages: 0138-0142, 0198-0203
extraction: ocr
subsections:
    - "no": 1
      title: FIELDS
      page: 114
      pdf_page: 138
    - "no": 2
      title: INTEGRAL DOMAINS
      page: 116
      pdf_page: 140
    - "no": 3
      title: PRIME IDEALS
      page: 116
      pdf_page: 140
    - "no": 4
      title: THE FIELD OF RATIONAL NUMBERS
      page: 117
      pdf_page: 141
statements: 17
exercises: 21
content_sha256: 450a4277ef6dd2bd877041bdfcecf1c00eb3decba3d2142cbb81a1614a396de6
translated_from: content/en/alg/I/09_s9_fields.md
translation_method: google
source_content_sha256: 622420ff5a6f546db44026f2ba8fbe2960bad17825f8f2a2110f89182676f0dd
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: f107c9c6363815e4313f4403b010b717a6b65a3d0e93dbe2e6c5b40f54b905af
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 9。 体

### 1. 体

#### 定義 1 {#alg-i-s9-def-1 .statement tag=05IF}

*環 $K$ は、$0$ のみで構成されず、$K$ のゼロ以外のすべての元が反転可能な場合、体と呼ばれます。

The set of non-zero elements of the field $K$, with multiplication, is a group, which is precisely the multiplicative group $K^*$ of the ring $K$ (§ 8, no. 1). 体の反対環は体です。 乗法が可換である場合、体は *可換* と呼ばれます。このような体はその反対のものと同一視されます。 非可換フィールドときどきは *スキュー 体* と呼ばれます。

#### 例 {#alg-i-s9-n1-exa-1 .statement tag=05IG}

*(1)* *合理的数* の no. 4 体で定義するとします。 *一般位相* では、実数の体 (*一般位相*、IV, § 1, no. 3)、複素数の体 (*一般位相*、VIII, § 1, no. 1) および四元数の体も定義されます(*一般位相*、VIII, § 1, no. 4)。これらの体は、クォータニオンの体を除いて可換です。*
*(2)* 環 $\mathbf{Z}/2\mathbf{Z}$ は明らかに体です。

$K$ を体とします。 $K$ のすべての部分環 $L$、つまり体は、$K$ の *部分体* と呼ばれ、$K$ は、$L$ の *拡大体* と呼ばれます。 $L$ が $K$ の部分環であることと、$L$ の 0 以外のすべての元 $x$ が $x^{-1} \in L$ であると言うのは同じことになります。 $(L_i)_{i \in I}$ が $K$ の部分体のファミリーである場合、$\bigcap_{i \in I} L_i$ は $K$ の部分体です。したがって、$K$ の部分集合 $X$ ごとに、$K$ 含む $X$ の最小の部分体が存在します。それは *$X$ によって生成されたと言われています。

#### 命題 1 {#alg-i-s9-prop-1 .statement tag=05IH}

※$K$を体とします。 $K$ の部分集合 $X$ ごとに、セントラライザー (§ 8, no. 5、例 3) $X$ の $X'$ は $K$ の部分体になります。*

私たちは、$X'$ が $K$ の部分環であることを知っています (*loc. cit.*)。一方、$x \neq 0$ が $z \in X$ で置換可能である場合、$x^{-1}$ (I, § 2, no. 3、命題 5) も置換可能であるため、$X'$ 含むは $X'$ のすべての非ゼロ元の逆数になります。

#### 系 {#alg-i-s9-n1-cor-1 .statement tag=05II}

* 体 $K$ の中心は、$K$ の (可換) 部分体です。*

#### 定理 1 {#alg-i-s9-thm-1 .statement tag=05IJ}

$\mathbf{A}$を環とします。次の条件は同等です。

(a) $\mathbf{A}$ は体です。
(b) $\mathbf{A}$ は 0 に減らされず、$\mathbf{A}$ の残りのイデアルは 0 と $\mathbf{A}$ だけです。

$\mathbf{A}$ が体であるとします。この場合、$\mathbf{A}$ は 0 に減らされません。$a$ を 0 とは異なる $\mathbf{A}$ の左イデアルとします。$a$ 所属から $a$ までの非ゼロが存在します。すべての $x \in \mathbf{A}$、$x = (xa^{-1})a \in a$ について。したがって$a = \mathbf{A}$です。

$\mathbf{A}$ が条件 (b) を満たすとします。 $x \neq 0$ を $\mathbf{A}$ に入れます。 $x$ が可逆であることを証明する必要があります。左の理想は $Ax$ 含む $x$ であるため、零、よって $Ax = \mathbf{A}$ ではありません。したがって、$x'x = 1$ となるような $x' \in \mathbf{A}$ が存在します。その後、$1 \neq 0$から$x' \neq 0$になります。 適用上記の結果を$x'$に当てはめると、$x''x' = 1$となるような$x'' \in \mathbf{A}$が存在することが分かります。次に$x'' = x'' . 1 = x''x'x = 1 . x = x$、したがって$xx' = 1$です。したがって、$x'$ は $x$ の逆数です。

#### 注意 {#alg-i-s9-n1-rem-1 .statement tag=05IK}

定理 1 では、左の理想を右の理想に置き換えることができます。 章 VIII, § 5, no. 2 では、0 と $\mathbf{A}$ とは異なる *両側* 理想を持たない非ゼロ環 $\mathbf{A}$ を研究します。このような環 (*準単純* と呼ばれる) は、必ずしも体 * であるとは限りません (たとえば、有理数係数を持つ位数 2 の正方行列の環 $\mathbf{M}_2(\mathbf{Q})$ は準単純ですが、体ではありません)*。

#### 系 1 {#alg-i-s9-thm-1-cor-1 .statement tag=05IL}

$\mathbf{A}$を環、$a$を$\mathbf{A}$の両面理想とします。 環 $\mathbf{A}/a$ が体になるためには、$a$ が $\mathbf{A}$ の最大左理想であることが必要かつ十分です。

$\mathbf{A}/a$ の左イデアルは形 $b/a$ で、$b$ は $\mathbf{A}$ 含む $a$ ($§ 8$、no. 8、系 ～ 命題 5) の左イデアルです。 $\mathbf{A}/a \neq 0$ ということは $a \neq \mathbf{A}$ を意味します。この仮定の下で、$\mathbf{A}$ 含む $a$ の唯一残った理想が $a$ と $\mathbf{A}$ (定理 1)、よってである場合に限り、$\mathbf{A}/a$ は体になります。 系。

#### 系 2 {#alg-i-s9-thm-1-cor-2 .statement tag=05IM}

$\mathbf{A}$を0ではない可換環とします。可換体の上に$\mathbf{A}$の準同型が存在します。

クルルの定理 ($§ 8$, no. 6, 定理 1) によれば、$\mathbf{A}$ には最大の理想$a$ が存在します。すると、$\mathbf{A}/a$ は体 (系 1) になります。

#### 系 3 {#alg-i-s9-thm-1-cor-3 .statement tag=05IN}

$a$ を整数 $\geqslant 0$ とします。 環 $\mathbf{Z}/a\mathbf{Z}$ が体になるためには、$a$ が素数であることが必要かつ十分です。

これは、系 1 と $§ 8$、no. 11 から続きます。

$p$ 素数体 $\mathbf{Z}/p\mathbf{Z}$ は $\mathbf{F}_p$ で表されます。

#### 定理 2 {#alg-i-s9-thm-2 .statement tag=05IO}

$\mathbf{K}$ を体、$\mathbf{A}$ をゼロ以外の環とします。 $f$ が $\mathbf{K}$ の準同型から $\mathbf{A}$ になる場合、$\mathbf{A}$ の部分環 $f(\mathbf{K})$ は体となり、$f$ 定義する同型は $\mathbf{K}$ になります。 $f(\mathbf{K})$。

$a$ を $f$ の核とします。次に、$\mathbf{A}$の$f(1) = 1 \neq 0$に対して$1 \notin a$、そして$a$は$\mathbf{K}$の左イデアルなので、定理による$a = \{0\}$は1です。したがって、$f$は単射なので、$\mathbf{K}$の同型は部分環になります。 $\mathbf{A}$中$f(\mathbf{K})$;したがって、後者の環は体になります。

### 2. 整域

#### 定義 2 {#alg-i-s9-def-2 .statement tag=05IP}

*環 $\mathbf{A}$ は、可換で非ゼロ、かつ 2 つの非ゼロの積 $\mathbf{A}$ の元が非ゼロの場合、整域 (または完全性領域) と呼ばれます。

有理数整数の環 $\mathbf{Z}$ は整域です。それは可換で非ゼロです。 2 つの整数 $> 0$ のうち積はゼロ以外です。ゼロ以外のすべての整数は形 $a$ または $-a$ で、$a > 0,\ b > 0$、よっての主張には $a > 0$ と $(-a)b = -ab,\ (-a)(-b) = ab$ が含まれます。

すべての可換体は整域です。 整域の部分環は整域です。特に、可換体の部分環は整域です。逆に、すべての整域 $\mathbf{A}$ は可換体の部分環と同型であることを示します。 (§ 8, no. 12) を思い出してください。$\mathbf{A}$ は、分数の合計環のうちの部分環と同一視されています。 主張は次の命題から続きます。

#### 命題 2 {#alg-i-s9-prop-2 .statement tag=05IQ}

*$\mathbf{A}$が整域の場合、分数$\mathbf{K}$と$\mathbf{A}$の合計環は可換環となります。

環 $\mathbf{K}$ は可換です。 $\mathbf{A} \neq \{0\}$ 以降はゼロではありません。 $\mathbf{A}$ が整域であるため、$\mathbf{A}$ のゼロ以外のすべての元はキャンセル可能であり、$\mathbf{K}$ は分数 $a/b$ と $b \neq 0$ で構成されます。ここで、$a/b \neq 0$ は $a \neq 0$ を意味し、分数 $b/a$ は $a/b$ の逆数になります。

整域の分数の合計環は、分数*の*体と呼ばれます。そのような環は、分数の体においてその像と同一視されます。

#### 命題 3 {#alg-i-s9-prop-3 .statement tag=05IR}

*$\mathbf{B}$ を非ゼロ環とし、$\mathbf{A}$ を $\mathbf{B}$ の可換部分環として、$\mathbf{A}$ のすべての非ゼロ元が $\mathbf{B}$ で可逆であるようにします。
(a) $\mathbf{A}$ は整域です。
(b) *$\mathbf{A}'$を分数$\mathbf{A}$の体とします。 The canonical injection of $\mathbf{A}$ into $\mathbf{B}$ can be extended uniquely to an isomorphism $f$ of $\mathbf{A}'$ onto a subfield of $\mathbf{B}$.
(c) *The elements of $f(\mathbf{A}')$ are the $xy^{-1}$ where $x \in \mathbf{A},\ y \in \mathbf{A},\ y \neq 0$.*

主張 (a) は明らかです。 The canonical injection of $\mathbf{A}$ into $\mathbf{B}$ extends uniquely to a homomorphism $f$ of $\mathbf{A}'$ into $\mathbf{B}$ (§ 8, no. 12, Theorem 5). 主張 (b) は、no. 1、定理 2 から続きます。 $\mathbf{A}'$ の元は、$x \in \mathbf{A},\ y \in \mathbf{A},\ y \neq 0$ と $f(x/y) = xy^{-1}$、よってを含む分数 $x/y$ です (c)。

### 3. 最高の理想

#### 命題 4 {#alg-i-s9-prop-4 .statement tag=05IS}

※$\mathbf{A}$を可換環、$\mathfrak{p}$を$\mathbf{A}$の理想とします。次の条件は同等です。
(a) *環 $\mathbf{A}/\mathfrak{p}$ は整域です。
(b) $\mathbf{A} \neq \mathfrak{p}$、$x \in \mathbf{A} - \mathfrak{p}$ と $y \in \mathbf{A} - \mathfrak{p}$ の場合は、$xy \in \mathbf{A} - \mathfrak{p}$。
(c) $\mathfrak{p}$ は、$\mathbf{A}$ の準同型の核が体になります。*

(c) ⇒ (b) ⇒ (a) の意味は明らかです。 If $A/p$ is an integral domain, let $f$ be the canonical injection of $A/p$ into its field of fractions and $g$ the canonical homomorphism of $A$ onto $A/p$; then $p$ is the kernel of $f \circ g$, whence the implication (a) ⇒ (c).

#### 定義 3 {#alg-i-s9-def-3 .statement tag=05IT}

*可換環 $A$ において、命題 4 のイデアル $p$ 満たす条件を素イデアルと呼びます。

#### 例 {#alg-i-s9-n3-exa-1 .statement tag=05IU}

(1) $A$を可換環とします。 $m$ が $A$ の最大理想である場合、$m$ は素数です。 環 $A/m$ は体 (no. 1、系 1 ～ 定理 1) です。

(2) $A$ が整域の場合、$A$ の理想$\{0\}$ は素数です (ただし、環 $\mathbf{Z}$ の例が証明しているように、一般に極大ではありません)。

### 4. 合理的数の体

#### 定義 4 {#alg-i-s9-def-4 .statement tag=05IV}

*The field of fractions of the ring $\mathbf{Z}$ of rational integers is called the field of rational numbers and is denoted by $\mathbf{Q}$. $\mathbf{Q}$ の元は有理数数と呼ばれます。*

従って、すべての有理数数は形 $a/b$ であり、ここで $a$ と $b$ は $b \neq 0$ を伴う有理数整数 (そして $b > 0$ を関係とみなすこともできます)

$$
a/b = (-a)/(-b)
$$

証明します）。 $\mathbf{Q}_+$ は、$a \in \mathbf{N}$ と $b \in \mathbf{N}^*$ を使用して、形 $a/b$ の有理数数の集合を表すために使用されます。

関係があります:

(1) $$ \mathbf{Q}_+ + \mathbf{Q}_+ = \mathbf{Q}_+ $$
(2) $$ \mathbf{Q}_+ \cdot \mathbf{Q}_+ = \mathbf{Q}_+ $$
(3) $$ \mathbf{Q}_+ \cap (-\mathbf{Q}_+) = \{0\} $$
(4) $$ \mathbf{Q}_+ \cup (-\mathbf{Q}_+) = \mathbf{Q} $$
(5) $$ \mathbf{Q}_+ \cap \mathbf{Z} = \mathbf{N} $$

最初の 2 つは、式 $a/b + a'/b' = (ab' + a'b)/bb'$、$(a/b)(a'/b') = aa'/bb'$、$0 \in \mathbf{Q}_+$、$1 \in \mathbf{Q}_+$ と、$\mathbf{N}$ が加法および乗法では安定しており、$\mathbf{N}^*$ が乗法では安定であるという事実から導かれます。明らかに $0 \in \mathbf{Q}_+$、よって $0 \in (-\mathbf{Q}_+)$; $x$ を $\mathbf{Q}_+ \cap (-\mathbf{Q}_+)$ にしましょう。その場合、$b \neq 0,\ b' \neq 0$ と $x = a/b = -a'/b'$ を伴う正の整数 $a, b, a', b'$ が存在します。次に $ab' + ba' = 0$、よって $ab' = 0$ ($ab' \geq 0$ と $ba' \geq 0$ の場合)、従って $b' \neq 0$ から $a = 0$ になります。他には語、$x = 0$。最後に、明らかに $\mathbf{N} \subset \mathbf{Z}$ と $\mathbf{N} \subset \mathbf{Q}_+$ です。逆に、$x$ 属するから $\mathbf{Z} \cap \mathbf{Q}_+$ の場合、それは有理数整数です。 $a \geq 0,\ b > 0$ と $x = a/b$、よって $a = bx$ を伴う 2 つの有理数整数 $a$ と $b$ が存在します。 $x \notin \mathbf{N}$ の場合、$-x > 0$、よって $-a = b(-x) > 0$ となり、その結果、仮定とは逆に $a < 0$ となります。

2 つの有理数数 $x$ と $y$ が与えられると、$y - x \in \mathbf{Q}_+$ であれば $x \leq y$ と書きます。式 (1)、(3)、(4) から、$x \leq y$ が次の合計順序であることが簡単に推測できます。

Q、(5) から、この関係誘導するは、Z 上の通常の位数関係であることがわかります。 最後に、(1) から、関係 $x \leq y$ と $x' \leq y'$ は $x + x' \leq y + y'$ を暗示していることがわかり、(2) から、関係 $x \leq y$ がわかります。すべての $z \geq 0$ には $xz \leq yz$ が、$z \leq 0$ (cf. VI, § 2, no. 1) には $xz \geq yz$ が含まれます。

$x$ を有理数数とします。 $x$ は、$x \geq 0$ の場合 *正*、$x > 0$ の場合 *厳密に正*、$x \leq 0$ の場合 *負*、$x < 0$ の場合 *厳密に負* であると言われます。† 正の有理数数の集合は $\mathbf{Q}_+$ で、負の数の場合は$-\mathbf{Q}_+$。 $\mathbf{Q}^*$ が非ゼロ有理数数の集合を表す場合、厳密に正の数の集合 $\mathbf{Q}_+^*$ は $\mathbf{Q}^* \cap \mathbf{Q}_+$ に等しく、$-\mathbf{Q}_+^*$ は厳密に負の数の集合です。

集合 $\mathbf{Q}_+^*$ と $\{1, -1\}$ は乗法群 $\mathbf{Q}^*$ の部分群です。 Every rational number $x \neq 0$ can be expressed in one and only one way in the form $1.y, (-1).y$, where $y > 0$; hence the multiplicative group $\mathbf{Q}^*$ is the product of the subgroups $\mathbf{Q}_+^*$ and $\{1, -1\}$, the component of $x$ in $\mathbf{Q}_+^*$ is called the *absolute value* of $x$ and is denoted by $|x|$; the component of $x$ in $\{-1, 1\}$ (equal to 1 if $x > 0$, to $-1$ if $x < 0$) is called the *sign* of $x$ and denoted by $\operatorname{sgn}\, x$.

通常、これら 2 つの写像は、設定 $|0| = 0$ と $\operatorname{sgn}\, 0 = 0$ によって $\mathbf{Q}$ 全体に拡張されます。

### 練習問題 {#alg-i-s9-exercises}

[§ 9 に対して練習問題](exercises/s9/)を参照してください。
