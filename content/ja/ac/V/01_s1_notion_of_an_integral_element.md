---
book: ac
book_title: Commutative Algebra
chapter: V
chapter_title: INTEGERS
section: 1
section_title: Notion of an integral element
lang: ja
source: ac-i-vii
book_pages: 303-324, 355-362
pdf_pages: 0322-0343, 0374-0381
extraction: ocr
subsections:
    - "no": 1
      title: INTEGRAL ELEMENTS OVER A RING
      page: 303
      pdf_page: 322
    - "no": 2
      title: THE INTEGRAL CLOSURE OF A RING. INTEGRALLY CLOSED DOMAINS
      page: 308
      pdf_page: 327
    - "no": 3
      title: EXAMPLES OF INTEGRALLY CLOSED DOMAINS
      page: 309
      pdf_page: 328
    - "no": 4
      title: COMPLETELY INTEGRALLY CLOSED DOMAINS
      page: 312
      pdf_page: 331
    - "no": 5
      title: THE INTEGRAL CLOSURE OF A RING OF FRACTIONS
      page: 314
      pdf_page: 333
    - "no": 6
      title: NORMS AND TRACES OF INTEGERS
      page: 316
      pdf_page: 335
    - "no": 7
      title: EXTENSION OF SCALARS IN AN INTEGRALLY CLOSED ALGEBRA
      page: 318
      pdf_page: 337
    - "no": 8
      title: INTEGERS OVER A GRADED RING
      page: 320
      pdf_page: 339
    - "no": 9
      title: 'APPLICATION: INVARIANTS OF A GROUP OF AUTOMORPHISMS OF AN ALGEBRA'
      page: 323
      pdf_page: 342
statements: 69
exercises: 29
content_sha256: e7322eee64ceb43d98b0cbd5eae55e7a6fd34247c600ea8aa57880fab093e205
translated_from: content/en/ac/V/01_s1_notion_of_an_integral_element.md
translation_method: google
source_content_sha256: 7deb20eda4181c66deed788db2dd8c9dfd03ddc75e31d67d9679866d4b1220a1
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 1e600f0c483156c8100d64f79e5ba8d9bb88379510809703be4bca05d037fb37
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 1. 積分元の概念

### 1. 環を超える積分元

#### 定理 1 {#ac-v-s1-thm-1 .statement tag=04MS}

$\mathbf{A}$ を、$\mathbf{A}$ (必ずしも可換ではない) および $\mathbf{R}$ の環、$\mathbf{R}$ 代数、および $x$ 元とします。次のプロパティは同等です。

(E₁) $x$ は、多項式環 $\mathbf{A}[X]$ のモニック多項式の根です。
(E₂) $\mathbf{R}$ の部分代数 $\mathbf{A}[x]$ は有限生成された $\mathbf{A}$ 加群です。
(E₃) 有限生成された $\mathbf{A}$ 加群である環 $\mathbf{A}[x]$ 上に忠実な加群が存在します。

まず、(E₁) が (E₂) を意味することを示しましょう。しましょう
$$
X^n + a_1 X^{n-1} + \ldots + a_n
$$
$\mathbf{A}[X]$ で $x$ を根とするモニック多項式であること。すべての整数 $q \geq 0$ について、$M_q$ を $1, x, \ldots, x^n + q$ によって生成された $\mathbf{R}$ のサブ$\mathbf{A}$ モジュールとします。それから
$$
x^{n+q} = -a_{n+q-1} x^{n+q-1} - \ldots - a_n x^q \in M_{-1}
$$
$q \geq 1$、よって、$q$の帰納法までに、
$$
M_q = M_{q-1} = \cdots = M_0.
$$

(*) この章と次の結果は、書籍 I から VI 以外の書籍、章 I, § 4、章 111、§ 5 には依存しません。

We conclude that $A[x]$ is equal to $M_0$ and is therefore a finitely generated $A$-module.

可換環 $A[x]$ はそれ自体に対する忠実な加群であるため、($E_{II}$) は ($E_{III}$) を暗示します。

最後に、($E_{III}$) が ($E_1$) を意味するという事実は、次のより正確な補題から導かれます。

#### 補題 1 {#ac-v-s1-lem-1 .statement tag=04MT}

*$A$ を、$R$ の $A$ および $x$ 元に対して、環、$R$ 代数 (可換である必要はありません) とします。 $M$ を、有限生成された $A$ 加群である $A[x]$ 上の忠実な加群とします。 $q$ が $xM \subset qM$ となるような $A$ の理想である場合、$x$ は、$A$ のすべての $\notin$ に係数が含まれるモニック多項式の根であり、その係数は支配的な係数以外です。 属する ～ $q$.*

$(u_i)_{1 \leq i \leq n}$ を、$M = \sum_{i=1}^n Au_i$ となるような $M$ の元の有限族とする。すべての $i$ に対して、次のような仮定によって元の $q$ の有限族 $(q_{ij})_{1 \leq j \leq n}$ が存在します。

$$
xu_i = \sum_{j=1}^n q_{ij}u_j \quad \text{for} \quad 1 \leq i \leq n.
$$

Therefore (*代数*, 章 III, § 8) if $d$ is 行列式 of 行列 $(q_{ij} - \delta_{ij}x)$ with 元 in $A[x]$ ($\delta_{ij}$ denoting the Kronecker 添字), thenすべての $i$ に対して $du_i = 0$、したがって $dM = 0$; $M$ は忠実な $A[x]$ モジュールであると想定されているため、必然的に $d = 0$ になります。 This means that $x$ is 根 of the polynomial $\det(q_{ij} - \delta_{ij}X)$ in $A[X]$ which, up to a sign, is a monic polynomial whose coefficientsother than the dominant 係数属する to $q$.

#### 定義 1 {#ac-v-s1-def-1 .statement tag=04MU}

*$A$ を環 、$R$ を $A$-代数 (可換である必要はありません) とします。 元 $x \in R$ は、定理 1 の同等の性質 ($E_1$)、($E_{II}$)、($E_{III}$) を満たす場合、$A$ の積分と呼ばれます。*

$P$ が $A[X]$ の *モニック* 多項式である形 $P(x) = 0$ の関係は、$A$ の係数との *積分依存関係の方程式* とも呼ばれます。

*例*

#### 例 1 {#ac-v-s1-n1-exa-1 .statement tag=04MV}

$K$ を (可換) 体 、$R$ を $K$-代数とする。 元 $x \in R$ が $K$ に関して整数であると言うのは、 $x$ が環 $K[X]$ の *非定数* 多項式の根であるというというと等価です。 $R$ が $K$ の *拡大* (*代数*、章 V, § 3, no. 3)、元 $x \in R$ が $K$ で積分である場合に導入された用語を一般化すると、元の *代数* 元とも呼ばれます。 $K$よりも$R$。

*(2)* The elements *of* $\mathbf{Q}(i)$ which are integral over $\mathbf{Z}$ are the elements of the form $a + ib$ where $a \in \mathbf{Z}$ and $b \in \mathbf{Z}$ ("*Gaussian integers*"'); the elements of $\mathbf{Q}(\sqrt{5})$ which are integral over $\mathbf{Z}$ are the elements *of* the form $(a + b\sqrt{5})/2$ where $a$ and $b$ belong to $\mathbf{Z}$ and are both even or both odd (for these two examples see Exercise 1).

(3) $\mathbf{Z}$ 上の複素数積分は代数整数とも呼ばれます。

Remarks
(1) Let $A'$ be the subring of $R$ (contained in the centre of $R$) the image of $A$ under the ring homomorphism $A \to R$ which defines the $A$-algebra structure on $R$. Clearly it is equivalent to say that an element of $R$ is integral over $A$ or that it is integral over $A'$.

#### 例 2 {#ac-v-s1-n1-exa-2 .statement tag=04MW}

Let $R'$ be a sub-A-algebra of $R$; the elements of $R'$ which are integral over $A$ are just the elements of $R$ which are integral over $A$ and belong to $R'$; this often allows us not to specify the algebra to which an integral element over $A$ belongs, when no confusion can arise.

#### 命題 1 {#ac-v-s1-prop-1 .statement tag=04MX}

*$A$ を $A$ (必ずしも可換ではない) および $R$ の環、$R$ 代数および $x$ 元とします。 $x$ が $A$ に対して積分であるためには、$A[x]$ が有限生成された $A$ 加群である $R$ の部分代数 $R'$ に含まれることが必要かつ十分です。

性質 (E_{II}) のおかげで、条件は明らかに必要です。また、(E_{III}) によっても十分です。なぜなら、$R'$ は忠実な $A[x]$ モジュールだからです ($R$ の含む単位元であるため)。

#### 系 {#ac-v-s1-n1-cor-1 .statement tag=04MY}

*$A$ をネーター 環、$R$ を $A$-代数 (必ずしも可換であるとは限らない)、および $R$ の $x$ 元とします。 $x$ が $A$ に対して積分であるためには、$R$ 含む $A[x]$ の有限生成された部分加群が存在することが必要かつ十分です。

条件は (E_{II}) のおかげで必要です。 $A[x]$ が有限生成A-加群のサブ A モジュールである場合、それ自体が有限生成A-加群 (*代数*, 章 VIII, § 2, no. 3, 命題 7) である場合には十分です。

$A$ がネーター できないである仮定は、主張 (練習問題 2) から省略されます。

#### 定義 2 {#ac-v-s1-def-2 .statement tag=04MZ}

※$A$を環とします。 $R$ のすべての元が $A$ 上で積分である場合、$A$-代数 $R$ (必ずしも可換であるとは限らない) は、$A$ 上で積分と呼ばれます。 $R$ が有限生成された $A$ モジュールである場合、$R$ は $A$ に対して有限と呼ばれます。*

命題 1 から、すべての有限 $A$-代数は積分であることがわかります。 $R$ が可換で有限の $A$-代数である場合、$R$ は明らかに有限に生成される $A$-代数です。 逆は誤りです。

*例 (4)* $M$ が有限生成された $A$ 加群である場合、$M$ の自己準同型の代数 $\mathrm{End}_A(M)$ は、(E_{III}) により $A$ にわたって積分です。特に、すべての整数 $n$、行列環 $M_n(A) = \mathrm{End}_A(A^n)$ は $A$ に対して積分 (さらには有限) です。

#### 命題 2 {#ac-v-s1-prop-2 .statement tag=04N0}

*$A, A'$ を 2 つの環、$R$ $A$-代数、$R$ $A'$-代数 (必ずしも可換であるとは限らない)、および $f : A \to A'$ と $g : R \to R'$ を 2 つの環準同型とします。 図式

$$
\begin{array}{ccc}
A & \xrightarrow{f} & A' \\
| & & | \\
\mathbf{R} & \xrightarrow{g} & \mathbf{R}'
\end{array}
$$

可換です。 元 $x \in R$ が $A$ に対して整数である場合、$g(x)$ は $A'$ に対して整数です。

$1 \leq i \leq n$ に対して $a_i \in A$ が $x^n + a_1 x^{n-1} + \cdots + a_n = 0$ の場合、次のように推測されます。

$$
(g(x))^n + f(a_1)(g(x))^{n-1} + \cdots + f(a_n) = 0.
$$

#### 系 1 {#ac-v-s1-prop-2-cor-1 .statement tag=04N1}

*$A$ を環、$B$ (可換) $A$-代数、$C$ (必ずしも可換ではない) $B$-代数とする。すると、$A$ に対して積分であるすべての元 $x \in C$ は、$B$ に対して積分になります。*

#### 系 2 {#ac-v-s1-prop-2-cor-2 .statement tag=04N2}

*$K$を、$K$の体、$L$拡大、$x, x'$$L$の2つの元、つまり$K$を超える共役（代数、章）とします。 V, § 6, no. 2）。 $A$ が $K$ の部分環で、$x$ が $A$ に対して積分である場合、$x'$ も$A$ に対して積分です。*

$A$ の $f(x) = x'$ と元が $f$ の下で不変となるような、$K(x)$ の $K(x')$ への $K$ 同型同型$f$ が存在します。

#### 系 3 {#ac-v-s1-prop-2-cor-3 .statement tag=04N3}

*$A$ を環、$B$ a (可換) $A$-代数、$C$ a (必ずしも可換ではない) $B$-代数とする。 $C$ が $A$ に対して整数である場合、$C$ は $B$ に対して整数です。*

#### 命題 3 {#ac-v-s1-prop-3 .statement tag=04N4}

*$(R_i)_{1 \leq i \leq n}$ を (必ずしも可換であるとは限らない) $A$-代数の有限族とし、$R = \prod_{i=1}^n R_i$ をその積とします。 For an element $x = (x_i)_{1 \leq i \leq n}$ of $R$ to be integral over $A$, it is necessary and sufficient that each of the $x_i$ be integral over $A$. $R$ が $A$ に対して整数であるためには、$R_i$ のそれぞれが $A$ に対して整数であることが必要かつ十分です。*

最初の主張を証明するだけで明らかに十分です。 条件は命題 2 によって必要です。逆に、各 $x_i$ が $A$ に関して積分である場合、$R_i$ の部分代数 $A[x_i]$ は有限生成された $A$ 加群であり、したがって、部分代数 $\prod_{i=1}^n A[x_i]$ も同様です。 $R$; $A[x]$ はこの部分代数に含まれているため、$x$ は $A$ から命題 1 までの積分です。

#### 命題 4 {#ac-v-s1-prop-4 .statement tag=04N5}

*$A$を環、$R$を$A$-代数（必ずしも可換であるとは限らない）、$(x_i)_{1 \leq i \leq n}$をペアごとに置換可能な$R$の元の有限族とする。すべての $i$ について、$x_i$ が $A[x_1, \ldots, x_{i-1}]$ に対して整数である場合 (特に、すべての $x_i$ が $A$ に対して整数である場合)、$R$ の部分代数 $A[x_1, \ldots, x_n]$ は、有限生成された $A$ 加群になります。

$n$ については帰納法で、命題は $n = 1$ に対して (E_{II}) であると主張します。 帰納法の仮定は、$B = A[x_1, \ldots, x_{n-1}]$ が有限生成A-加群であることを意味します。 $x_n$ は $B$ に対して積分であるため、$B[x_n] = A[x_1, \ldots, x_n]$ は有限生成された B-加群であり、したがって有限生成A-加群 (代数, 章 II, § 1, no. 13, 命題 25) でもあります。

#### 系 1 {#ac-v-s1-prop-4-cor-1 .statement tag=04N6}

Let $A$ be a ring and $R$ a (Commutative)A-algebra. The set of elements $\& R$ integral over $A$ is a subalgebra of $R$.

実際、$x, y$ が $A$ について積分した $R$ の 2 つの元である場合、命題 4 から$A[x, y]$ は有限生成A-加群であることがわかります。 含む $x + y$ と $xy$ のように、系は命題 1 から続きます。

非可換代数では、$A$ 上の 2 つの積分元の和と積は、$A$ (練習問題 4) 上で必ずしも積分ではありません。

#### 系 2 {#ac-v-s1-prop-4-cor-2 .statement tag=04N7}

$A$ を環、$R$ A-代数 (必ずしも可換であるとは限らない)、および $E$ 集合 $\&$ 元 $\& R$ とします。これらはペアごとに置換可能であり、$A$ について整数です。このとき、$E$ によって生成された部分 A 代数 $B \& R$ は、$A$ 上で積分です。

$B$ 属するのすべての元を、$E$ の有限部分集合によって生成された $B$ の部分 A 代数に変換します。

注意 (3) 命題 4 から、$A$ 上のすべての可換A-代数積分は、$A$ 上の有限部分代数の右有向族の和集合であることがわかります。

#### 命題 5 {#ac-v-s1-prop-5 .statement tag=04N8}

$A$ を環と $A$ および $R$ 2 (可換) A-代数とします。 $R$ が $A$ に対して積分である場合、$R \otimes_A A'$ は $A'$ に対して積分です。

$R \otimes_A A'$ の任意の元 $x' = \sum_{i=1}^n x_i \otimes a'_i$ を考えます。ここで、$x_i$ 属するから $R$ と $a'_i$ から $A'$ です。 $x_i \otimes a'_i = (x_i \otimes 1)a'_i$ と $x_i \otimes 1$ は $A'$ (命題 2) に対して積分であるため、$x$ も同様です。

#### 系 {#ac-v-s1-n1-cor-2 .statement tag=04N9}

$R$ を環および $A, B, C$ 部分環 $\& R$ として、$A \subset B$ とします。 If $B$ is integral over $A$, $C[B]$ is integral over $C[A]$.

$B \otimes_A C[A]$ は $C[A]$ の命題 5 による積分であるため、$R$ (A-代数とみなされる) の $B \otimes_A C[A]$ の標準像 $C[B]$ も命題 2 の積分です。

#### 命題 6 {#ac-v-s1-prop-6 .statement tag=04NA}

$A$ を環、$B$ (可換)A-代数、$C$ を (必ずしも可換ではない)B 代数とする。 $B$ が $A$ に対して積分であり、$C$ が $B$ に対して積分である場合、$C$ は $A$ に対して積分です。

すべての $x \in C$ が $A$ に対して整数であることを検証するだけで十分です。 仮定までに、$B$ に係数が入り、$x$ が根となるモニック多項式 $X^n + b_1 X^{n-1} + \cdots + b$ が存在します。この場合、$x$ は $B' = A[b_1, \ldots, b_n]$ の積分であるため、$B'[x]$ は有限生成された B-加群になります。しかし、$B$ は $A$ に対して整数であるため、$B'$ は有限生成A-加群 (命題 4) です。 結論する B'[x] も有限生成A-加群 (代数, 章 11, § 1, no. 13, 命題 25) であるため、x は A に関して整数です。

#### 系 {#ac-v-s1-n1-cor-3 .statement tag=04NB}

*A を環とし、R、R' 2 (可換)A-代数を A 上で積分します。すると、R $\otimes_A$ R' は A 上で積分になります。*

$R \otimes_A R$ は R (命題 5) に関する積分であるため、結論は命題 6 から得られます。

### 2. 環の一体型クロージャ。完全に閉じられたドメイン

#### 定義 3 {#ac-v-s1-def-3 .statement tag=04NC}

*A を環、R a (可換)A-代数とします。 A 上の積分 (no. 1, 系 1 から命題 4) の R からなるの元の部分 A 代数 A' は、R における A の積分閉包と呼ばれます。 A' が R の A の標準像に等しい場合、A は R で積分的に閉じていると呼ばれます。*

注意

(1) $h : A \to R$ が R 上の A-代数構造を定義する環準同型である場合、R における A の積分閉包は、R における $h(A)$ の積分閉包でもあります。一方、R' が R の部分代数である場合、R' における A の積分閉包は $A' \cap R'$ です。

(2) A が体の場合、R における A の積分閉包 $A'$ は、A (no. 1, 例 1) に対して代数的な R の元で構成されます。 体拡大 (代数, 章 V, § 3, no. 3) に使用される用語を一般化すると、A' は代数 R の体 A の代数閉包とも呼ばれ、A は $A' = A$ の場合 R で代数的に閉じられていると呼ばれます。

#### 定義 4 {#ac-v-s1-def-4 .statement tag=04ND}

*A が整域の場合、分数の体における A の積分閉包は A の積分閉包と呼ばれます。 整域がその積分閉包と等しい場合、積分閉包と呼ばれます。

代数的に閉じていない体の例が示すように、積分閉領域は必ずしもどの環含むでも閉じているわけではないことに注意してください。

#### 命題 7 {#ac-v-s1-prop-7 .statement tag=04NE}

※Aを環、RをA-代数とします。 R における A の積分閉包 A' は、R では部分環積分閉包です。*

R における A' の積分閉包は、A に対して no. 1, 命題 6 によって積分されます。したがって、それは A' に等しくなります。

#### 系 {#ac-v-s1-n2-cor-1 .statement tag=04NF}

*整域 A の積分閉包は積分閉領域です。*

K を A の分数の体と、A の積分閉包である B とします。

K は B の分数の体であり、命題を適用する 7 から $R = K$ までであれば十分です。

#### 命題 8 {#ac-v-s1-prop-8 .statement tag=04NG}

*$R$ を環、$(B_\lambda)_{\lambda \in L}$ を $R$ の部分環の家族、それぞれの $\lambda \in L$ を $A_\lambda$ を $B_\lambda$ の部分環とします。それぞれの$A_\lambda$が$B_\lambda$で一体的に閉じられている場合、$A = \bigcap_{\lambda \in L} A_\lambda$は$B = \bigcap_{\lambda \in L} B_\lambda$で一体的に閉じられています*。

これは、定義 3 と no. 1、系 1 から命題 2 の直後に続きます。

#### 系 {#ac-v-s1-n2-cor-2 .statement tag=04NH}

*空ではない、整域 $A$ の統合的に閉じられたサブドメインのファミリーのすべての共通部分は、統合的に閉じられたドメインです。*

命題を適用する 8 は、$R$ と、分数 $K$ の $A$ の体に等しい $B_\lambda$ を取り、$K$ で積分的に閉じられた $K$ の部分環が *なおさら* 積分であることに注意するだけで十分です。 分数の体が$K$に含まれているため、クローズドドメインです。

#### 命題 9 {#ac-v-s1-prop-9 .statement tag=04NI}

*$A$を環、$(R_i)_{1 \leq i \leq n}$を$A$-代数の有限族、$A'_i$を$R_i$、$(1 \leq i \leq n)$における$A$の積分閉包とする。この場合、$R = \prod_{i=1}^n R_i$ の $A$ の積分閉包は $\prod_{i=1}^n A'_i$ に等しくなります。*

これは、no. 1、命題 3 の明らか帰結です。

#### 系 1 {#ac-v-s1-prop-9-cor-1 .statement tag=04NJ}

*$A$ を、縮小されたネーター 環、$p_i$ $(1 \leq i \leq n)$ の別個の最小素数イデアル、整域 $A/p_i$ の分数の$K$、体とします（標準的に同型） 局所環 $A_{p_i}$ (章 IV, § 2, no. 5、命題 10)) および $A'_i$ $K$、$(1 \leq i \leq n)$ の $A$ の積分閉包。次に、分数 $B$ の$A$ の合計環の標準同型が $\prod_{i=1}^n K_i$ に (上記参照) 写像 $B$ の $A$ の積分閉包が積に環 $\prod_{i=1}^n A'_i$.*

#### 系 2 {#ac-v-s1-prop-9-cor-2 .statement tag=04NK}

*縮小されたネーター 環が分数の環で統合的に閉じられるためには、それが統合的に閉じられた (ネーター) 領域の直接の合成であることが必要かつ十分です。

### 3. 完全に閉じられたドメインの例

#### 命題 10 {#ac-v-s1-prop-10 .statement tag=04NL}

*すべての主イデアル整域は一体的に閉じられています。*

$A$ を主イデアル整域、$K$ を分数の体、および $K$ の $x$ 元とします。 $x = ab^{-1}$ (*代数*, 章 VII, § 1, no. 2, 命題 1 および章 VI, § 1, no. 11, 命題 9 となる) $A$ の 2 つの互いに素な元 $a, b$ が存在します。 (DIV))。 $x$ が $A$ について整数である場合、それは多項式の根になります

X^n + c_1 X^{n-1} + \ldots + c_n \text{ of } A[X]。次に、$a^n = b(-c_1 a^{n-1} - \ldots - c_n b^{n-1})$、これは $b$ 割る $a''$ であることを証明します。 $a$ と $b$ は相対的に素であるため、これは $A$ (代数, 章 VI, § 1, no. 12, 系 1 ～ 命題 11 (DIV)) で $b$ が可逆であることを意味します。したがって$x \in A$です。

#### 補題 2 {#ac-v-s1-lem-2 .statement tag=04NM}

*R を環とし、R[X] の多項式を P とします。 多項式環 R'[X] において、多項式 P が次数 1 のモニック多項式の積となるような環 R' 含む R が存在します。

P の次数 $n$ で帰納法を進めます。$n = 0$ と $n = 1$ では補題が明らかです。 したがって、$n > 1$ と仮定します。 $a$ を P によって生成された $R[X]$ の理想とし、$f$ を $B = R[X]/a$ 上の $R[X]$ の標準準同型とします。 P はモニックであるため、すべての多項式 $Q \in R[X]$、$\deg(PQ) = \deg(P) + \deg(Q)$、よって $a \cap R = 0$;したがって、制限 off to R は単射法です。 $f$ によって R を B の部分環 $f(R)$ と識別し、$b = f(X)$ と書くと、$b$ は B の P の根であり、P は $B[X]$ の多項式として考慮されることがわかります。 このとき、次数 $n - 1$ の $B[X]$ には、$P(X) = (X - b)Q(X)$ (代数, 章 IV, § 1, no. 4, 命題 5) となるようなモニック多項式 Q が存在します。 帰納法の仮定までに、$R'[X]$ で多項式 Q が次数 1 のモニック多項式の積となるような環 $R' \supseteq B$ が存在します。明らかに、$R'[X]$ では P は次数 1 のモニック多項式の積になります。

#### 命題 11 {#ac-v-s1-prop-11 .statement tag=04NN}

*A を環、R A-代数、R[X] の P と Q のモニック多項式とする。 PQ の係数が A に関して整数である場合、P と Q の係数は A に関して整数です。*

補題 2 を二重に適用すると、$R'[X]$ に次のような環 R' 含む R と R' の族元 $(a_i)_{1 \leq i \leq m}, (b_j)_{1 \leq j \leq n}$ が存在することがわかります。
$$
P(X) = \prod_{i=1}^\infty (X - a_i), \quad Q(X) = \prod_{j=1}^n (X - b_j);
$$
P Q の係数属するは R' の A の積分閉包 $A'$ に変換され、したがって (no. 2, 命題 7) 元 $a, (1 \leq i \leq m)$ および $b, (1 \leq j \leq n)$ 属するは A に対して積分されます。 P と Q の係数は A に関して積分であるということになります。 (no. 1、系 1 ～ 命題 4)。

A を整域、K を分数の体、K' を K-代数とします (必ずしも可換であるとは限りません)。 K 上の代数元 $x \in K'$ が与えられると、$P(x) = 0$ 形が $K[X]$ のイデアル $a \neq 0$ となる多項式 $P \in K[X]$ が与えられ、必然的に主 (代数, 章 IV, § 1, no. 5, 命題 7）。 生成する a; という固有のモニック多項式が存在します。 代数、章、V, § 3, no. 1、定義 3 で導入された用語を一般化すると、このモニック多項式は K 上の x の最小多項式と呼ばれます。

#### 系 {#ac-v-s1-n3-cor-1 .statement tag=04NO}

*Aを整域、Kを分数の体、xをK-代数K*の元とします（可換である必要はありません）。 *x が A に関して整数である場合、$K$ に対する $x$ の最小多項式 $P$ の係数は、$A$ に関して積分です (したがって、$A$ が積分で閉じている場合、それらは属するから $A$ になります)。

仮定 (no. 1, 定理 1) によって、$Q(x) = 0$ となるようなモニック多項式 $Q \in A[X]$ が存在します。 $K[X]$ の $P$ 割る $Q$ のように、命題 11 から、$P$ の係数は $A$ に関して積分であることがわかります。

Let $A$ be a ring and $R$ a (commutative) $A$-algebra; the homomorphism $\phi : A \to R$ defining the $A$-algebra structure on $R$ can be extended uniquely to a homomorphism $A[X] \to R[X]$ of polynomial rings over $A$ and $R$, leaving $X$ invariant and hence $R[X]$ is given a canonical $A[X]$-algebra structure.

#### 命題 12 {#ac-v-s1-prop-12 .statement tag=04NP}

Let $A$ be a ring, $R$ an $A$-algebra and $P$ a polynomial in $R[X_1, \ldots, X_n]$. $P$ が $A[X_1, \ldots, X_n]$ に対して積分であるためには、$P$ の係数が $A$ に対して積分であることが必要かつ十分です。

$R[X_1, \ldots, X_n]$ の多項式を $R[X_1, \ldots, X_{n-1}]$ の係数を含む $X$ の多項式として考えると、$n = 1$ に対して証明命題に縮小されることがすぐにわかります。 次に、$P$ を $R[X]$ の多項式とします。 no. 1, 命題 5 からすぐに、$P$ の係数が $R$ の $A$ の積分閉包 $B$ にある場合、属するから $B[X] = B \otimes_A A[X]$ までの元 $P$ は積分であることがわかります。 $A[X]$以上。 逆に、$P$ が $A[X]$ に対して整数であると仮定し、次のようにします。

$$
Q(Y) = Y^m + F_1 Y^{m-1} + \cdots + F,
$$

$P$ を根とした、係数 $F_i \in A[X]$ のモニック多項式になります。 $r$ を、多項式 $P$ および $F_i$ ($1 \leq i \leq m$) のすべての次数より厳密に整数大きくすると、次のように書きます。

$$
P_1(X) = P(X) - X^r.
$$

すると、$P_1$ は多項式の根になります

$$
Q_1(Y) = Q(Y + X') = Y^m + G_1 Y^{m-1} + \cdots + G,
$$

$A[X]$ に係数が入っています。したがって、次のように書くこともできます

$$
-P_1(P_1^{m-1} + G_1 P_1^{m-2} + \cdots + G_{m-1}) = G_r
$$

ここで、$r$の選択は、$-P_1$が$R[X]$のモニック多項式であり、多項式$F_k(X) X^{r(m-k)}$の$G_m(X) = Q(X^r)$、次数が$k \geq 1$に対してすべて$< rm$であることを意味します。 結論するまず第一に、多項式は

$$
P_1^{m-1} + G_1 P_1^{m-2} + \cdots + G_{m-1}
$$

of $R[X]$ is also monic; moreover, as the coefficients of $G_i$ belong to $A$, Proposition 11 shows that $P_1$ has coefficients integral over $A$ and the coefficients of $P$ are therefore certainly integral over $A$.

#### 命題 13 {#ac-v-s1-prop-13 .statement tag=04NQ}

$A$を環、$\mathbf{R}$を$A$代数、$A'$を$\mathbf{R}$の$A$の積分閉包とします。すると、$\mathbf{R}[X_1, \ldots, X_n]$ の $A[X_1, \ldots, X_n]$ の積分閉包は $A'[X_1, \ldots, X_n]$ に等しくなります。

これは、no. 2 の命題 12 と定義 3 から続きます。

#### 系 1 {#ac-v-s1-prop-13-cor-1 .statement tag=04NR}

$A$ を整域とし、$A'$ をその積分閉包とします。すると、多項式環 $A[X_1, \ldots, X_n]$ の積分閉包は $A'[X_1, \ldots, X_n]$ になります。

$n$ について帰納法が議論すると、問題は直ちに $n = 1$ のケースに還元されます。 $K$ を $A$ の分数の体とし、これは $A'$ の分数の体とします。 元 $P$ の体の分数 $K(X)$ の $A[X]$ が $A[X]$ に関して整数である場合、属するから多項式環 $K[X]$ となり、後者は主イデアル整域 (代数、章 IV, § 1, no. 5、命題 7)、したがって一体的に閉じています (命題 10)。 系は、命題 13 から $\mathbf{R} = K$ に適用されます。

#### 系 2 {#ac-v-s1-prop-13-cor-2 .statement tag=04NS}

$A$を整域とします。 多項式環 $A[X_1, \ldots, X_n]$ が一体的に閉じられるためには、$A$ が一体的に閉じられることが必要十分です。

#### 系 3 {#ac-v-s1-prop-13-cor-3 .statement tag=04NT}

$K$ が体の場合、すべての多項式代数 $K[X_1, \ldots, X_n]$ は積分閉領域になります。

### 4. 完全に一体化したクローズドドメイン

#### 定義 5 {#ac-v-s1-def-5 .statement tag=04NU}

整域 $A$ は、次の条件が満たされる場合、完全に積分閉と呼ばれます: すべての冪 $x^n$ が満たされるように、体の分数 $K$ の $A$ のすべての元 $x$ ($n \geqslant 0$) は、$K$、属する ～ $A$ の有限生成されたサブ A モジュールに含まれます。

$x^n$ が有限生成された $K$ のサブ A モジュールに含まれているという仮定は、すべての $n \geqslant 0$ に対して $dx^n \in A$ となる非ゼロの元 $d \in A$ が存在するというというによっても表現できることに注意してください。後者の条件は $x^n \in Ad^{-1}$ を意味します。逆に、$(b_i)_{1 \leqslant i \leqslant m}$ が $K$ の元の有限列である場合、$1 \leqslant i \leqslant m$ には $db_i \in A$、サブ A モジュール $M$ にはよって $dM \subset A$ となるような $d \in A$ が存在します。 $K$ は $b_i$ によって生成されます。

明らかに、完全に積分的に閉じられた領域は積分的に閉じられています。逆に、no. 1の系から命題1は、積分閉領域ネーターが完全に積分閉であることを示しています。 \* 一方、高さ $\geqslant 2$ (章 VI, § 4, no. 4) の評価の環は積分的に閉じられていますが、完全に積分的に閉じられていません。 \* $(A_i)$ が、分数 $K$ の同じ体を持つ完全に積分的に閉じられたドメインのファミリーである場合、$A = \bigcap_i A_i$ は完全に積分的に閉じられます。 なぜなら、$x \in K$が、$A$、$dx^n$、属するから$A$のすべての$n > 0$、仮定の一部の非ゼロ$d$について、仮定は、すべての$i$、したがって$x \in A$について$x \in A$であることを意味します。

#### 命題 14 {#ac-v-s1-prop-14 .statement tag=04NV}

※$A$を完全に一体的に閉じた領域とする。次に、すべての多項式環 $A[X_1, \ldots, X_n]$ (それぞれ、正式な冪系列 $A[[X_1, \ldots, X_n]]$ のすべての環) は完全に一体的に閉じられます。*

$n$ 上の帰納法までに、$A[X]$ (それぞれ $A[[X]]$) が完全に積分的に閉じていることを証明するのに十分です。 Then let $P$ be an element of the field of fractions of $A[X]$ (resp. $A[[X]]$) and suppose that there exists a non-zero element $Q \in A[X]$ (resp. $Q \in A[[X]]$) such that $Q P^m \in A[X]$ (resp. $Q P'' \in A[[X]]$) for every integer $m \geq 0$. $K$ が $A$ の分数の体である場合、$A[X]$ (それぞれ $A[[X]]$) は $K[X]$ (それぞれ $K[[X]]$) の部分環であり、$K[X]$ (それぞれ $K[[X]]$) は次のようになります。 主イデアル整域 (*代数*、章 VII, § 1, no. 1) は一体的に閉じています (no. 4、命題 10) およびネーター (*代数*、章 VIII, § 2, no. 3) なので完全に一体的に閉じています。それなら私たちはすでにそれを見ました

$P \in K[X]$ (それぞれ $P \in K[[X]]$)。 $P = \sum_{k=0}^{\infty} a_k X^k$ ($a_k \in K$) と $Q = \sum_{k=0}^{\infty} b_k X^k$ ($b_k \in A$) を考えて、$a_i$ がすべての属するから $A$ に当てはまらないと仮定して *不合理な還元* によって議論します。その場合、$a_i \notin A$ となるような少なくとも添字 $i$ が存在します。書いたら

$$
P_1 = \sum_{k=0}^{i-1} a_k X^k \in A[X],
$$

仮定の直後に、すべての $m \geq 0$ に対して $Q(P - P_1)^m \in A[X]$ (それぞれ $Q(P - P_1)^m \in A[[X]]$) が続きます。 $j$ を $b_j \neq 0$ となる最小の整数とします。明らかに、最小の次数のうち係数 $\neq 0$ の $Q(P - P_1)^m$ 項は $b_j a_i^m X^{j + mi}$ であるため、すべての $m \geq 0$ では $b_j a_i^m \in A$ になります。しかし、$A$ は完全に一体的に閉じているため、これは仮定とは反対に、$a_i \in A$ を意味します。

#### 命題 15 {#ac-v-s1-prop-15 .statement tag=04NW}

*$A$ をフィルタリングされた環とし、そのフィルタリングは網羅的であり、$A$ のすべての主理想がフィルタリングによって定義される位相の下で閉じられるようにします。関連する等級付けされた環 $\mathrm{gr}(A)$ (章 III, § 2, no. 3) が完全に積分的に閉じられた領域である場合、$A$ は完全に積分的に閉じられた領域です。*

$(A_n)_{n \in \mathbf{Z}}$ を $A$ で定義された濾過とします。 $\bigcap_{n \in \mathbf{Z}} A_n$ は理想 (0) (章 III, § 2, no. 5) の閉包であり、仮定は最初に濾過 $(A_n)$ が分離されていることを意味し、$\mathrm{gr}(A)$ が整域であるため、次に$A$ (章) になります。 III, § 2, no. 3、系 ～ 命題 1)。 $x = b/a$ を体の分数 $K$ の $A$ ($a \in A, b \in A$) の元とし、$A$ の元 $d \neq 0$ が存在し、すべての$dx^n \in A$ が成立します。 $n \geq 0$。私たちは$b \in A a$、そして仮定までに理想的な$A a$が閉じていることを証明しなければならない、すべての$n \in \mathbf{Z}, b \in A a + A$にとってそれを示すだけで十分です。 $A$ の濾過が徹底的であるため、$b \in A a + A_q$ のような整数 $q \in \mathbf{Z}$ が存在します。したがって、関係 $b \in A a + A_q$ が $b \in A a + A_{q+1}$ を意味することを証明すれば十分です。

次に、$b = a y + z$ が $y \in A, z \in A_{q+1}$ であるとします。 次に、すべての $n \geq 0$、よってに対して仮定 $dx^n \in A$ により、すべての $n \geq 0$ に対して直ちに $d(x - y)^n \in A$ が得られます。他の語、$dz^n = a^n t_n$ では、すべての $n \geq 0$ に対して $t_n \in A$ です。 明らかに極限が $z \neq 0$ の場合に注意を払うことができます。 $v$ が $A$ (章 III, § 1, no. 2) の位数写像を表し、$v(d) = n_1,\ v(z) = n_2 \geq m,\ v(a) = n_3$ と書きましょう。 $d', z', a'$ を $A_{n_1}/A_{n_1+1},\ A_{n_2}/A_{n_2+1},\ A_{n_3}/A_{n_3+1}$ の $d, z, a$ のそれぞれの像とします。 すべての $n \geq 0,\ v(dz^n) = n_1 + nn_2$ (章 III, § 2, no. 3、命題 1) に対して、$dz^n$ の $\mathrm{gr}(A)$ の標準像は $d'{z'}^n$ です。同様に、$a^n t_n$ の $\mathrm{gr}(A)$ の標準像は、$t'_n \in \mathrm{gr}(A)$ である形 ${d'}^n t'_n$ であることがわかり、$a' \neq 0$ として、すべての $n \geq 0,\ d'(z'/a')^n \in \mathrm{gr}(A)$ についてそれが推測されます。 したがって、$\mathrm{gr}(A)$ が完全に積分的に閉じているという仮定は、$z' = a's'$ となるような $s' \in \mathrm{gr}(A)$ の存在を意味します。 $s'$ を均質な元の和に分解すると、さらに ($z'$ と $a'$ が均質であるため) $s'$、つまり元 $s \in A$ の像が均質であると仮定できることがわかります。次に$v(as) = v(z) = n_2$と$z \equiv as \pmod{A_{n_2+1}}$。 $n_2 \geq m, a fortiori$ $z \equiv as \pmod{A_{m+1}}$ なので、$b \equiv a(y+s) \pmod{A_{m+1}}$ となります。

### 5. 分数の環の統合クロージャ

Let $A$ be a ring, $R$ an $A$-algebra and $S$ a multiplicative subset of $A$. (章 II, § 2, no. 8) $S^{-1}R$ には標準的な $S^{-1}A$-代数構造があることを思い出してください。

#### 命題 16 {#ac-v-s1-prop-16 .statement tag=04NX}

*$A$を環、$R$を$A$-代数、$A'$を$R$の$A$の積分閉包、$S$を$A$の乗算部分集合とする。すると、$S^{-1}R$ における $S^{-1}A$ の積分閉包は $S^{-1}A'$ になります。*

$b/s$ を $S^{-1}A'$ ($s \in S,\ b \in A'$) の元とします。 図式から

$$
\begin{array}{ccc}
A & \xrightarrow{i_A^S} & S^{-1}A \\
\downarrow h & & \downarrow S^{-1}h \\
R & \xrightarrow{i_R^S} & S^{-1}R
\end{array}
$$

は可換であり、$b/1$ は$S^{-1}A$ (no. 1, 命題 2) に対して整数です。 $1/s \in S^{-1}A$ と同様に、$b/s = (b/1)(1/s)$ は $S^{-1}A$ に対して積分です。

逆に、$r/t \ (r \in R,\ t \in S)$ を $S^{-1}A$ について整数である $S^{-1}R$ の元とします。この場合、$r/1 = (t/1)(r/t)$ は $S^{-1}A$ に対して積分になります。次に、形の関係です。

$$
(r/1)^n + (a_1/s)(r/1)^{n-1} + \cdots + (a_n/s) = 0,
$$

ここで、$a_i \in A \ (1 \leq i \leq n)$ と $s \in S$ です。この関係とも書かれるかもしれません

$$
(sr^n + a_1 r^{n-1} + \ldots + a_n)/s = 0
$$

したがって、${s'}^n(sr^n + a_1 r^{n-1} + \ldots + a_n) = 0$ となるような $s' \in S$ が存在します。私たちは$(s'sr)^n + s'a_1(s'sr)^{n-1} + \ldots + {s'}^ns^{n-1}a_n = 0$と推測します。 定義までに、したがって $s'sr \in A'$、よって $r/1 \in S^{-1}A'$、$r/t \in S^{-1}A'$ になります。

#### 系 1 {#ac-v-s1-prop-16-cor-1 .statement tag=04NY}

$A$ を整域、$A'$ をその積分閉包、$S$ を $0 \notin S$ となるような $A$ の乗法部分集合とします。すると、$S^{-1}A$の積分閉包は$S^{-1}A'$になります。

The field of fractions $R$ of $A$ is also the field of fractions of $S^{-1}A$ since $0 \notin S$ (Chapter II, § 1, no. 1, Remark 7); 次に、命題 16 が $R$ に適用されます。

#### 系 2 {#ac-v-s1-prop-16-cor-2 .statement tag=04NZ}

$A$を整域、$K$を分数の体、$R$代数を$K$、そして$B$を$R$の$A$の積分閉包とします。 $K$ (no. 1, 例 1) の代数である $R$ の元は、形 $a^{-1} b$ の元です。ここで、$b \in B$ と $a \in A, a \neq 0$; $L$が$R$の$K$の代数閉包であれば、$B$に含まれる$K$の上に$L$の基底が存在します。

最初の主張は、$S = A - \{0\}$ の場合に適用された命題 16 の後に続きます。 $(x_i)_{i \in I}$ が $K$ 上の $L$ の基底である場合、$A$ のすべての $i \in I$ 元 $a_i \neq 0$ に対して $a_i x_i \in B$ が存在します。その場合、$(a_i x_i)_{i \in I}$ は $K$ の $L$ の基底でもあります。

#### 系 3 {#ac-v-s1-prop-16-cor-3 .statement tag=04O0}

$A$ を $A$ の最大理想の整域と $\Omega$ 集合とします。 $A$ が一体的に閉じられるためには、$m \in \Omega$、$A_m$ がすべて一体的に閉じられることが必要十分です。

系 1 から、条件が必要であることがわかります。 $A = \bigcap_{m \in \Omega} A_m$ (章 II, § 3, no. 3、公式 (2)) には条件で十分であり、no. 2 の命題 8 に系を適用するだけで十分です。

#### 系 4 {#ac-v-s1-prop-16-cor-4 .statement tag=04O1}

$A$を整域、$K$を分数の体、$S$を$A$の乗算部分集合として$0 \notin S$とします。

(i) $B$ を $A$ の積分である $K$ の部分環とし、$\mathfrak{f}$ を $A$ モジュール $B/A$ の消滅子とします。次に、$S^{-1}\mathfrak{f}$ は $(S^{-1}A)$ モジュール $S^{-1}B/S^{-1}A$ の消滅子に含まれており、$B$ が有限生成された $A$ モジュールである場合、この消滅子に等しくなります。

(ii) $A'$ を $A$ の積分閉包とします。 $S^{-1}A$ を一体的に閉じるには、$A$ モジュール $A'/A$ の消滅子 $\mathfrak{f}$ が $S$ を満たすだけで十分です。この条件は、$A'$ が有限生成された $A$ モジュールである場合にも必要です。

(i) $\mathfrak{f}B \subset A$、$(S^{-1}\mathfrak{f})(S^{-1}B) \subset S^{-1}A$、したがって$S^{-1}\mathfrak{f}$ は$\operatorname{Ann}(S^{-1}B/S^{-1}A)$ に含まれます。 $B$ が有限生成された $A$ 加群である場合、方程式 $S^{-1}\mathfrak{f} = \operatorname{Ann}(S^{-1}B/S^{-1}A)$ は、章 II, § 2, no. 4 の公式 (9) の特殊なケースであり、$S^{-1}B/S^{-1}A$ は$S^{-1}(B/A)$ と正規に識別されます。

(ii) 系 1 $S^{-1}A'$ により、$S^{-1}A$ の積分閉包になります。 関係 $\mathfrak{f} \cap S \neq \varnothing$ と $S^{-1}\mathfrak{f} = S^{-1}A$ は等しいので (章 II, § 2, no. 5, 注意) (ii) は (i) の明らか帰結です。

$B$ が $A$ について整数である $K$ の部分環である場合、$B/A$ の消滅子 $f$ (トランスポーター $A : B$ (章 I, § 2, no. 10) に定義等しい) は次のようになります。 ときどきは、$A$の$B$の*指揮者*と呼ばれています。

#### 系 5 {#ac-v-s1-prop-16-cor-5 .statement tag=04O2}

*$A$を整域、$A'$をその統合クロージャ、$A$モジュール$A'/A$の$f$消滅子とします。 $A'$ が無限に生成される $A$ モジュールであるとします。 $A_p$ が積分的に閉じていない主要なイデア $p \in A$ は、含む $f$ であるものです。*

これは、$S = A - p$ に適用された系 **4 (ii)** の直後に続きます。

系 5 $f \neq 0$ の仮説の下では、$A'$ は有限生成された $A$ モジュールであり、$K/A$ のすべての元 ($A$ の分数の $K$ 体) には消滅子があることに注意してください。 $\neq 0$。

*代数幾何学では、系 5 と上記の注意は、アフィン多様体 $V$ が正規ではない形閉集合が $V$ とは異なり、点であることを示しています。* \*

### 6. ノルムと整数の痕跡

#### 命題 17 {#ac-v-s1-prop-17 .statement tag=04O3}

*$A$ を環、$B$ を (可換) $A$-代数、位数 $n$ の $B$ の $X$ 平方行列とします。次のプロパティは同等です。

(a) $X$ は $A$ に対して積分です。

(b) すべての $x \in M$ と $M$ の $X.x \in M$ が $B$ モジュール $B^n$ の生成元の系であるような、$B^n$ の有限生成されたサブ$A$ モジュール $M$ が存在します。

(c) $X$ の特性多項式の係数は、$A$ にわたって積分されます。*

$\chi(T) = \det(T.1 - X)$ が $X$ の特性多項式である場合、Cayley-Hamilton 定理は $\chi(X) = 0$ (*代数*, 章 VII, § 5, no. 4, *注意* 1) を示し、$\chi$ はモニック多項式であるため、(c) が示すように(a) no. 1、命題による 6.

2 番目に (a) が成り立つとします。 $(e_i)_{1 \leq i \leq n}$ が $B^n$ の標準基底である場合、$X^k.e_i$ ($1 \leq i \leq n, k \geq 0$) によって生成される $B$ のサブ$A$ 加群 $M$ は、$A$-代数のため、有限生成される $A$ 加群です$A[X]$ は、有限生成された $A$ モジュール (no. 1、定理 1) です。 $M$ 含むと $e_i$ のように、(a) は (b) を暗示していることがわかります。 逆は、no. 1、定理 1、条件 (E_{III}) の帰結です。

Finally let us prove that (a) implies (c); as $X$ is integral over $A$ and *a fortiori* over the polynomial ring $A[T]$, $T.1 - X$ is also integral over $A[T]$ and by no. 3, Proposition 12 the problem is seen to reduce (by replacing $X$ by $T.1 - X$ and $A$ by $A[T]$) to proving that, if $X$ is integral over $A$, $d = \det(X)$ is an element of $B$ which is integral over $A$. さて、上で、$X$ によって定義された $B^n$ の自己準同型 $u$ が、有限生成されたサブ$A$ モジュール $M$ 含む $e_i$ を安定に残すことを見てきました。 $n$ベクトル$x_1 \wedge x_2 \wedge \ldots \wedge x_n$、$1 \leq i \leq n$の$x_i \in M$、したがって、$\bigwedge^n(B^n)$の生成するは、有限生成されたサブ$A$モジュール含む$e_1 \wedge e_2 \wedge \ldots \wedge e$で、$\bigwedge^n u$下で安定します。比率$d$のホモテティー未満の語。の消滅子として

$$
e_1 \wedge e_2 \wedge \ldots \wedge e,
$$

B 簡約するから 0、条件 (E_{III}) の no. 1、定理 1 は、d が A に関して整数であることを証明します。

#### 系 1 {#ac-v-s1-prop-17-cor-1 .statement tag=04O4}

A を整域、K を分数の体、K' を有限次元 K-代数とします (必ずしも可換であるとは限りません)。 x \in K' が A に関して積分である場合、特性多項式 Pc_{K'/K}(x; X) (代数, 章 VIII, § 12, no. 2) の係数は A に関して積分です。

z \mapsto M(z) が代数 K' の正則表現である場合 (行列表現; cf. 代数, 章 VIII, § 13 とみなされる) Pc_{K'/K}(x; X) は次のようになります。 定義行列 M(x) の特性多項式。 x が A に対して積分である場合、行列 M(x) は A (no. 1, 命題 2) に対して積分であり、命題を適用する 17 で十分です。

#### 系 2 {#ac-v-s1-prop-17-cor-2 .statement tag=04O5}

系 1 と同じ仮説と記法を使用すると、Tr_{K'/K}(x) と N_{K'/K}(x) は A に関して積分になります。

Tr_{K'/K}(x) と N_{K'/K}(x) は、符号内では Pc_{K'/K}(x; X) の係数 (代数, 章 VIII, § 12, no. 1、式 (4)) であるため、整数です。

#### 注意 (1) {#ac-v-s1-n6-rem-1 .statement tag=04O6}

K' が K 上の単純な中心代数で、K' の x \が A 上で積分である場合、x の縮小特性多項式 (代数, 章 VIII, § 12, no. 3) の係数は A 上で整数です。この多項式の冪は Pc_{K'/K}(x; X) に等しいためです。 (上記引用、命題 8) そして、命題を適用する 17 と no. 3、命題 11 で十分です。

#### 命題 18 {#ac-v-s1-prop-18 .statement tag=04O7}

A を積分閉領域、K を分数の体、K' を有限次元可分 K-代数 (代数, 章 VIII, § 7, no. 5)、A' を K' における A の積分閉包とする。すると、A'は無限に生成されるA-加群に含まれます。

命題は、次のより正確な補題から導き出されます。

#### 補題 3 {#ac-v-s1-lem-3 .statement tag=04O8}

命題 18 の仮説の下で、(w_1, ..., w_n) を A' に含まれる K 上の K' の基底とします (no. 5, 系 2 ～ 命題 16)。その場合、K 上の K' の一意の基底 (w_1^*, ..., w_n^*) があり、これについては Tr_{K'/K}(w_i w_j^*) = \delta_{ij} (クロネッカー 添字) となります。 d = D_{K'/K}(w_1, ..., w_n) が基底 (w_1, ..., w_n) (代数, 章 IX, § 2) の判別式である場合、 d \neq 0 および

$$
\sum_{i=1}^n Aw_i \subset A' \subset \sum_{i=1}^n Aw_i^* < d^{-1} \left( \sum_{i=1}^n Aw_i \right).
$$

特に、d が A の可逆元である場合、A' は基底 (w_1, ..., w_n) で自由A-加群になります。

K' は分離可能な K-代数であるため、 d \neq 0 (代数, 章 IX, § 2, 命題 5) および K 双線形形式

$$(x, y) \mapsto \operatorname{Tr}_{K'/K}(xy)$$

したがって、K' 以上は非縮退です (*loc. cit.*, 命題 4)。これは、基底 $(w_i^*)_{1 \leq i \leq n}$ (*代数*、章 IX, § 1, no. 6、系 ～ 命題 6) の存在と一意性を示します。そうなると、(2) の最初の包含は明らかです。 $x$ を $A'$ の元とします。 $\xi_i \in K$ を $x = \sum_{i=1}^n \xi_i w_i^*$ と書きましょう。すべての $i$、$\xi_i = \mathrm{Tr}_{K'/K}(xw_i)$ に対して、$\xi_i$ は $A$ (系 2 から命題 17) に対して積分であり、$A$ が積分的に閉じているため、$1 \leq i \leq n$ に対して $\xi_i \in A$ は整数です。これは 2 番目の包含物 (2) を示しています。最後に、$\alpha_{ji} \in K$ を $w_j^* = \sum_{i=1}^n \alpha_{ji} w_i$ と書きましょう。次に、すべての $j$ と $k$ に対して $$\sum_{i=1}^n \alpha_{ji} \mathrm{Tr}_{K'/K}(w_i w_k) = \delta_{jk}$$ です。クラマーの公式は、$\alpha_{ji}$ 属するから $d^{-1}A$、よってが 3 番目の包含であることを示しています (2)。 (2) からすぐに最後の主張が続き、この場合は $A' = \sum_{i=1}^n Aw_i$ になります。

仮説と記法に続く 2 つの帰結では、命題 18 の結果が得られます。

#### 系 1 {#ac-v-s1-lem-3-cor-1 .statement tag=04O9}

*$A$ がネーター 環の場合、$A$ モジュール $A'$ は有限生成され、特に環 $A'$ はネーター になります。

$A'$ は、有限生成された $A$ モジュールの部分加群です。

#### 系 2 {#ac-v-s1-lem-3-cor-2 .statement tag=04OA}

* $A$ が主イデアル整域の場合、$A'$ は階数 $n$ の空き $A$ モジュールです。* 空き $A$ モジュールの各部分加群は空きになります (*代数*、章 VII, § 3、 定理 1）。

#### 系 3 {#ac-v-s1-lem-3-cor-3 .statement tag=04OB}

*Let $E$ be an extension of degree $n$ of the field $Q$ of rational numbers. The additive group of the integral closure in $E$ of the ring $Z$ of rational integers is a free commutative group of rank $n$.*

$Z$ は積分的に閉じられており (no. 3、命題 10)、$Q$ が特性 0 であるため、$E$ は分離可能です。 したがって、系 2 は、$A = Z$、$K = Q$、$K' = E$ の場合に適用できます。

*注意 (2)*。 $K'$ が $K$ (練習問題 20) の拡大体であっても、$K'$ が $K$ 上で分離していると仮定されていない場合、系 1 の結論は必ずしも真ではありません。 On the other hand, if $A$ is a *finitely generated integral $K_0$-algebra*, where $K_0$ is a *field*, the integral closure of $A$ in *any* extension of finite degree of the field of fractions of $A$ is a finitely generated $A$-module and a Noetherian ring, as we shall see in § 3, no. 2, Theorem 2.

### 7. 一体的に閉じたスカラーの拡大代数

#### 命題 19 {#ac-v-s1-prop-19 .statement tag=04OC}

*$k$ を、$k$ および$R$ の統合的に閉じた$k$-代数の体、$L$ 分離拡大とします。 環 $L \otimes_k R$ が整域の場合、一体的に閉じられます。*

K を R の分数の体とします。 k が体, L $\otimes_k$ であるため、R は正準的に L $\otimes_k$ K および L のサブ k-代数、R は L $\otimes_k$ R のサブ k-代数と同一視されます。 Moreover, since an element s $\# 0$ of R is not a divisor of 0 in R, 1 $\otimes s$ is not a divisor of zero in L $\otimes_k$ R since L is flat over k (Chapter I, § 2, no. 3); identifying s with 1 $\otimes s$, it is therefore seen that, if S = R - {0}, L $\otimes_k$ K is identified with S$^{-1}$(L $\otimes_k$ K); as L $\otimes_k$ R is assumed to be an integral domain, L $\otimes_k$ K is thus identified with a subring of the field of fractions $\Omega$ of L $\otimes_k$ R.

(1) L が k の有限拡大であると仮定します。その場合、L $\otimes_k$ K は K 上の有限階数の代数となり、仮定までに 0 の因子はなくなります。したがって、それは体 (代数, 章 V, § 2, no. 1, 命題 1) であるため、この場合は分数の $\Omega$ L $\otimes_k$ R の体となります。 ($w_1, \ldots, w_r$) を k 上の L の基底とします。したがって、これは K 上の L $\otimes_k$ K の基底でもあります。 $\mathrm{Tr}_{L/k}(w_i w_j^*) = \delta_{ij}$ (no. 6, 補題 3) となる L の基底 ($w_1^*, \ldots, w_n^*$) が存在します。すべての $z \in L \otimes_k K$ は一意に記述できます $z = \sum_{i=1}^u a_i w_i$ ここで $a_i \in K$;それから

$$
\mathrm{Tr}_{(L \otimes K)/K}(z w_j^*) = \sum_{i=1}^n a_i \mathrm{Tr}_{(L \otimes K)/K}(w_i w_j^*)
$$

そして、L のように、トレース $\mathrm{Tr}_{(L \otimes K)/K}$ と $\mathrm{Tr}_{L/K}$ 一致する (代数、章 VIII, § 12, no. 2、公式 (13)) が最後に$\mathrm{Tr}_{(L \otimes K)/K}(z w_j^*) = a_j$、$1 \leq j \leq n$ になります。 一方、注意は、Lの元はkに対して整数であり、したがってRに対しても整数です(no. 1、系1から命題2)。したがって (no. 1, 命題 5) L $\otimes_k$ R は R に関して整数です。 したがって、$z \in L \otimes_k K$ が L $\otimes_k$ R に対して積分であると仮定します。この場合、z も R (no. 1, 命題 6) に関して整数であるため、$z w_j^*$ も同様であり、したがって $1 \leq j \leq n$ (no. 6, 系 2 ～ 命題 17) についても $a_j = \mathrm{Tr}_{(L \otimes K)/K}(z w_j^*)$ となります。 R は積分的に閉じているため、すべての $j$ に対して $a_j \in R$、したがって $z \in L \otimes_k R$ となり、この場合命題が証明されます。

(2) ここで、L が K の有限生成された分離拡大であると仮定します。その場合、k (代数, 章 V, § 9, no. 3, 定理 2) を超える L の分離超越基底 ($x_1, \ldots, x_d$) が存在します。 L と K は体 $\Omega$ (代数, 章 V, § 5, no. 4) において代数的に k 上で互いに素であるため、$x_i$ は K 上で代数的に独立です。したがって、$R[x_1, \ldots, x_d]$ は一体的に閉じています (no. 3、系 2 ～ 命題 13)。 T を元 $\neq 0$ 環 $A = k[x_1, \ldots, x_d] \subset L$ の集合とすると、体 $k_1 = k(x_1, \ldots, x_d) \subset L$ は $T^{-1}k[x_1, \ldots, x_d]$ に等しくなります。それから

$$
k_1 \otimes_k R = (T^{-1}A) \otimes_k R = T^{-1}A \otimes_A (A \otimes_k R) = T^{-1}(A \otimes_k R)
= T^{-1}R[x_1, \ldots, x_d]
$$

テンソル積の結合性により、この領域は積分的に閉じています (no. 5、系 1 ～ 命題 16)。しかし、$L \otimes_k R$ は

L \otimes_{k_1} (k, \otimes_k R) および定義 L により、$k_1$ の有限分離拡大になります。したがって、(1) から、$L \otimes_k R$ は積分的に閉じていることがわかります。

(3) *一般的な場合* $z$ が $L \otimes_k R$ について整数である $\Omega$ の元である場合、形 $z^m + b_1 z^{m-1} + \ldots + b_m = 0$ の関係を満たします。ここで、$b_i$ 属する ～ $L \otimes_k R$ です。その場合、$1 \leq i \leq m$ および$z$ から $L' \otimes_k K$ に対して $b_i$ 属するから $L' \otimes_k R$ となるように、$k$ 上に L の有限生成された部分拡張 $L'$ が存在します。次に、(2) から、$z \in L' \otimes_k R$、したがって $L \otimes_k R$ は積分的に閉じていることがわかります。

\* V をアフィン既約代数多様体、$k$ を V の定義体と、$k$ 上で定義された V の正則写像の $R$ 環とします。 R が整数で閉じている場合、V は $k$* に対する *normal と呼ばれます。 命題 19 は、V が $k$ までは正常である場合、$k$ のすべての分離拡大 L では正常のままであることを示しています。 \*

#### 系 {#ac-v-s1-n7-cor-1 .statement tag=04OD}

*k を体とし、R と S の 2 つを一体的に閉じた K-代数とします。 環 $R \otimes_k S$ が整域で、分数 K の体と R と S の L がそれぞれ k 上で分離可能であるとします。 したがって、環 $R \otimes_k S$ は完全に閉じられた領域です。*

As R and S are identified with subalgebras of $R \otimes_k S$, K and L are identified with subfields of the field of fractions $\Omega$ of $R \otimes_k S$ which are linearly disjoint over $k$ (*Algebra*, Chapter V, § 2, no. 3, Proposition 5). 次に、命題 19 から、$R \otimes_k L$ と $K \otimes_k S$ は一体的に閉じた領域であることがわかります。それらの共通部分は $R \otimes_k S$ (章 I, § 2, no. 6、命題 7) であるため、$R \otimes_k S$ は完全に閉じられたドメイン (no. 2、系 ～ 命題 8) です。

\* Given two irreducible affine varieties V, W defined over $k$, their product $V \times W$ is an affine variety and the ring of functions regular on $V \times W$ is identified with the tensor product over $k$ of the ring of functions regular on V and the ring of functions regular on W. 系から命題 19 は、V と W が $k$ に対して正常である場合、$V \times W$ は $k$ に対して正常であることを示しています。 \*

### 8. 整数がグレード環を上回る

*この番号ではすべての卒業が考慮されています。 型 $\mathbf{Z}$ です。 A が等級付けされた環および $i \in \mathbf{Z}$ である場合、$A_i$ は、次数の元環 A の$i$ の同種の集合を示します。

A を評価済み環とし、B を評価済み A-代数とします。 x を A に対して整数である B の *同次* 元とします。それから関係です

$$
x^n + a_1 x^{n-1} + \ldots + a_n = 0 \quad \text{where } a_i \in A \quad \text{for } 1 \leq i \leq n.
$$

$m = \deg(x)$ と $a'_i$ を次数 $mi$ の $a_i$ ($1 \leq i \leq n$) の同次成分とする。それから明らかに

$$
x^n + a'_1 x^{n-1} + \ldots + a'_n = 0
$$

他の語では、x は *同次* 係数との積分依存関係の方程式を満たします。

Let $\mathbf{A}[X, X^{-1}]$ denote the ring of fractions $S^{-1}\mathbf{A}[X]$ of the polynomial ring $\mathbf{A}[X]$ in one indeterminate, $S$ being the multiplicative subset of $\mathbf{A}[X]$ consisting of the powers $X^n$ of $X$ ($n \geq 0$); as $X$ is not a divisor of 0 in $\mathbf{A}[X]$ it is immediate that the $X^i$ ($i \in \mathbf{Z}$) form a basis over $\mathbf{A}$ of the $\mathbf{A}$-module $\mathbf{A}[X, X^{-1}]$. 同次成分 $a_i$ ($i \in \mathbf{Z}$) を持つすべての元 $a \in \mathbf{A}$ について、次のように書きます。

$$
j_{\mathbf{A}}(a) = \sum_{i \in \mathbf{Z}} a_i X^i \in \mathbf{A}[X, X^{-1}]
$$

$j_{\mathbf{A}} : \mathbf{A} \to \mathbf{A}[X, X^{-1}]$ が単射詞環準同型であるのは明らかです。

#### 命題 20 {#ac-v-s1-prop-20 .statement tag=04OE}

*$\mathbf{A} = \bigoplus_{i \in \mathbf{Z}} A_i$ を段階的環および $\mathbf{B}$ を (可換) 次数付き $\mathbf{A}$-代数とする。 $\mathbf{A}$ の元の $\mathbf{B}$ の集合 $\mathbf{A}'$ は、$\mathbf{B}$ の段階的な部分代数です。

$i < 0$ の $A_i = 0$ と $\mathbf{B}$ が減らされた環である場合、$i < 0$ の$A'_i = 0$。*

図式

$$
\begin{array}{ccc}
\mathbf{B} & & \mathbf{A} \\
& \rho & \\
& & \\
& & \\
\mathbf{A}[X, X^{-1}] \xrightarrow{\phi'} \mathbf{B}[X, X^{-1}] \\
\end{array}
$$

(ここで、$\rho$ は、$\mathbf{B}$ およびそこから正規に導出された $\rho'$ 準同型上の $\mathbf{A}$-代数構造を定義する準同型です) は、定義 (5) からすぐに検証されるように、可換です。 $x$ を $\mathbf{A}$ で積分した $\mathbf{B}$ の元とします。この場合、$j_{\mathbf{B}}(x)$ は $\mathbf{A}[X, X^{-1}]$ (no. 1, 命題 2) について積分であるため、no. 5, 命題 16 から、$X^m j_{\mathbf{B}}(x)$ が $\mathbf{B}[X]$ の元となるような整数 $m > 0$ が存在することがわかります。 $\mathbf{A}[X]$ にわたる積分。 次に、no. 3、命題 12 から、多項式 $X^m j_{\mathbf{B}}(x)$ の係数は $\mathbf{A}$ に関して整数であると推定します。これらの係数は $x$ の均質な成分により定義であるため、これらは $\mathbf{A}$ にわたって積分であることがわかり、これは $\mathbf{A}'$ が $\mathbf{B}$ の段階的な部分代数であることを証明します。

ここで、$x \in A'_i$ が $i < 0$ であると仮定します。この番号の冒頭の注意 $x$ が形 (4) の式を満たすことを示しています。ここで、$1 \leq k \leq n$ は $a_k' \in A_{kt}$ です。 $j < 0$ が $A_j = 0$ であれば、$x^n = 0$、$\mathbf{B}$ が減算された環であれば、$x = 0$ が結論するとなるため、この場合はすべての $i < 0$ が $A'_i = 0$ となります。

(章 II, § 2, no. 9) を思い出してください。$\mathbf{A} = \bigoplus_{i \in \mathbf{Z}} \mathbf{A}_i$ が段階的環で、$S$ が *均質* 元の $\mathbf{A}$ からなるの乗算部分集合である場合、段階的環構造は、次数 $i$ の同次元の集合 $(S^{-1}\mathbf{A})_i$ を形 $a/s$ の元の集合とすることで、$S^{-1}\mathbf{A}$ で定義されます。 $a \in \mathbf{A}$ と $s \in S$ は同種であり、$\deg(a) - \deg(s) = i$ となる

#### 補題 4 {#ac-v-s1-lem-4 .statement tag=04OF}

$\mathbf{A} = \bigoplus_{i \in \mathbf{Z}} \mathbf{A}_i$ を、$\mathbf{A}$ の同種元 $\neq 0$ の等級付けされた整域と $S$ 集合とします。

(i) $S^{-1}\mathbf{A}$ のすべての同次元 $\neq 0$ は可逆であり、環 $K_0 = (S^{-1}\mathbf{A})_0$ は体および $i \in \mathbf{Z}$ の集合で、$(S^{-1}\mathbf{A})_i \neq 0$ は部分群となる$\mathbf{Z}$ の $q\mathbf{Z}$ (ここで $q \geqslant 0$)。

(ii) $q \geqslant 1$ を仮定し、$t$ を $(S^{-1}\mathbf{A})_q$ の非ゼロ元とします。次に、多項式環 $K_0[X]$ から $S^{-1}\mathbf{A}$ への写像 $X$ から $t$ 拡大するから同型の $K_0[X, X^{-1}]$ の $K_0$ 準同型写像 $f$ が、 $S^{-1}\mathbf{A}$と$S^{-1}\mathbf{A}$は一体的に閉じられています。

(i) の主張は、定義と仮定から、$a/s$ と $a'/s'$ が 2 つの同種元 $\neq 0$ of $S^{-1}\mathbf{A}$ of 次数である場合、$\mathbf{A}$ は整域であることがわかります。 $i$ と $i'$、$aa'/ss'$ は同種の元 $\neq 0$ と次数 $i + i'$ の同種です。 (ii) を示すために、$t$ は $S^{-1}\mathbf{A}$ 準同型 $f$ 拡大するにおいて、準同型 $\tilde{f}: K_0[X, X^{-1}] \to S^{-1}\mathbf{A}$ と必然的に $\tilde{f}(X^{-1}) = t^{-1}$ に反転可能であることに注意します。一方、$q$の定義により、$S^{-1}\mathbf{A}$のすべての同次元$\neq 0$は次数$qn \ (n \in \mathbf{Z})$となるので、$\lambda \in K_0$である形$\lambda t^n$で一意に書くことができます。 ($S^{-1}\mathbf{A}$ は整域であるため);したがって、$\tilde{f}$ は全単射です。最後に、$K_0[X]$ が積分的に閉じている (no. 3, 命題 10) ため、$K_0[X, X^{-1}]$ (no. 5, 系 1 ～ 命題 16) も同様であることがわかり、補題の証明が完成します。

#### 命題 21 {#ac-v-s1-prop-21 .statement tag=04OG}

$\mathbf{A} = \bigoplus_{i \in \mathbf{Z}} \mathbf{A}_i$ を、$\mathbf{A}$ の同種元 $\neq 0$ の等級付けされた整域および $S$ 集合とします。 $\mathbf{A}$ の統合クロージャ $\mathbf{A}'$ は、$S^{-1}\mathbf{A}$ のグレード部分環になります。さらに$\mathbf{A}_i = 0$で$i < 0$、$\mathbf{A}'_i = 0$で$i < 0$となります。

$\mathbf{A} = \mathbf{A}_0$ の場合、命題は自明です。それ以外の場合は、補題 4 を適用する可能性があります。 環 $S^{-1}\mathbf{A}$ は完全に閉じたドメインであるため、$\mathbf{A} \subset S^{-1}\mathbf{A}$; $S^{-1}\mathbf{A}$ が採点されるため、$\mathbf{A}'$ は命題 20 によって採点されます。後者の主張も命題 20 から続きます。

#### 系 1 {#ac-v-s1-prop-21-cor-1 .statement tag=04OH}

仮説と命題 21 の記法で、$\mathbf{A}$ 属するから $\mathbf{A}$ にわたって積分である $S^{-1}\mathbf{A}$ のすべての同次元があれば、$\mathbf{A}$ は積分的に閉じられます。

次に、すべての $i \in \mathbf{Z}$ に対して $\mathbf{A}'_i \subset \mathbf{A}$ となり、したがって $\mathbf{A}' = \mathbf{A}$ になります。

#### 系 2 {#ac-v-s1-prop-21-cor-2 .statement tag=04OI}

$\mathbf{A} = \bigoplus_{i \in \mathbf{Z}} \mathbf{A}_i$ が統合的に閉じられた段階的ドメインである場合、ドメイン $\mathbf{A}_0$ は統合的に閉じられます。

The field of fractions $K_0$ of $\mathbf{A}$, is identified (in the notation of Proposition 21) with a subring of the ring of homogeneous elements of degree 0 of $S^{-1}A$; every element of $K_0$ integral over $A$, (and *a fortiori* over $A$) belongs therefore by hypothesis to $A$.

#### 系 3 {#ac-v-s1-prop-21-cor-3 .statement tag=04OJ}

*$A = \bigoplus_{i \in \mathbf{Z}} A_i$ を統合的に閉じた段階的ドメインとします。したがって、すべての整数 $d > 0$、環 $A^{(d)}$ (章 III, § 1, no. 3) は、統合的に閉じられた領域になります。*

$U$ を $A^{(d)}$ の同次元 $\neq 0$ の集合とし、$x$ を $A^{(d)}$ にわたる、したがって $A$ にわたる $U^{-1}A^{(d)}$ の同次元とします。 $x \in S^{-1}A$、$x$ 属するから $A$ by 仮定として。 次数は $d$ で割り切れるので、 属するから $A^{(d)}$ となり、系 1 から $A^{(d)}$ が積分で閉じていることがわかります。

### 9. 適用: 群の自己同型の代数の不変式

環 $K$、$K$-代数 $A$ および群 $G$ が与えられた場合、次の場合、$G$ は $A$ 上で動作すると言えます: (1) 集合 $A$ が群の演算子 $G$ (*代数*, 章 I, § 7, no. 2); (2) すべての $\sigma \in G$、写像 $x \mapsto \sigma.x$ は、$K$-代数 $A$ の *自己準同型* です (したがって、全単射なので *自己同型* です (*loc. cit.*))。 $G$ の下で *不変量* である $A$ の元の $A^G$、集合で表すことにします。明らかに、それは $A$ の *サブ K 代数 * です。

$A$ の $G$ の *軌道* ごとに、$G$ は $A$ 上の演算子の *局所有限* 群であると言います (*代数*, 章 I、*束* の修正) IV) は *有限* です。

#### 命題 22 {#ac-v-s1-prop-22 .statement tag=04OK}

*$A$ を (可換) $K$-代数、$G$ を $A$ 上の演算子のローカルな有限群とします。この場合、$A$ は部分代数 $A^G$ に対して積分されます。*

すべての $x \in A$ について、$x_i$ ($1 \leq i \leq n$) を、$G$ の下の $x$ の軌道の別個の元とします。すべての $\sigma \in G$ に対して、集合 $\{1, 2, \ldots, n\}$ の置換 $\pi_\sigma$ が存在し、$1 \leq i \leq n$ に対して $\sigma.x_i = x_{\pi_\sigma(i)}$ が成り立ちます。したがって、$x_i$ の基本対称写像は $A$ の元であり、$G$ では不変ですが、他の$A^G$ の語元では不変です。 $x$ はモニック多項式 $\prod_{i=1}^n (X - x_i)$ の根と、この多項式属するから $A^G$ の係数であるため、$x$ は $A^G$ にわたって整数です。

#### 定理 2 {#ac-v-s1-thm-2 .statement tag=04OL}

*$A$ を有限生成された $K$-代数、$G$ を $A$ の演算子の局所的有限群とします。この場合、$A$ は有限生成された $A$ モジュールです。さらに $K$ がネーター であれば、$A^G$ は有限生成される $K$-代数* です。

$(a_j)_{1 \leq j \leq m}$ を $K$-代数 $A$ の生成元の系とします。 *なおさら* $A = A^G[a_1, \ldots, a_l]$ と $a_j$ は $A^G$ 命題 22 で積分され、最初の主張は no. 1、命題 4 から続きます。2 番目は次の補題の帰結です。

#### 補題 5 {#ac-v-s1-lem-5 .statement tag=04OM}

*$K$ をネーター 環、$B$ を有限生成された $K$-代数、$C$ を B が C で積分となる B の部分 K-代数とする。すると、C は有限生成された A-代数になります。

$(x_i)_{1 \leq i \leq n}$ を K-代数 B の生成元の有限系とします。すべての i に対して、$P_i(x_i) = 0$ のようなモニック多項式 $P_i \in C[X]$ が仮定までに存在します。 C' を、$P_i$ ($1 \leq i \leq n$) の係数によって生成された C の部分 K 代数とします。明らかに、$x_i$ は C' と $B = C'[x_1, \ldots, x_n]$ に対して積分です。したがって、B は有限生成された C' 加群 (no. 1, 命題 4) です。一方、$C'$ はネーター 環 (章 III, § 2, no. 10、系 3 ～ 定理 2) です。したがって、C は有限生成された $C'$ 加群であり、これは C が有限生成された K-代数であることを証明します。

#### 注意 {#ac-v-s1-n9-rem-1 .statement tag=04ON}

$\sigma \in G$ の集合は、$1 \leq j \leq m$ の $\sigma a_j = a_j$ が A の元ごとに不変のままであることは明らかです。 $G$ の通常の部分群 $\mathscr{H}$ は、A の元ごとに不変のままですので、次の式で有限添字になります。 $G$ と A は、有限群の演算子 $G/\mathscr{H}$ を持っていると考えることができます。明らかに$A^{G/\mathscr{H}} = A^G$。

S を、S が安定している環 A と $G$ 群の乗算部分集合とします。その場合、すべての $\sigma \in G$ に対して、環 $S^{-1}A$ の一意な自己準同型 $z \mapsto q_z$ が存在し、すべての $a \in A$ に対して $q_z(a/1) = (a.a)/1$ が存在します。 $a \in A$ と $s \in S$ に対して公式 $\sigma.(a/s) = (\sigma.a)/(\sigma.s)$ によって与えられます (章 II, § 2, no. 1, 命題 2)。 $\tau$ が $G$ の他の元である場合、すべての $z \in S^{-1}A$ に対して明らかに $q_z(\tau.z) = (\sigma\tau).z$ であるため、群 $G$ は環 $S^{-1}A$ に作用します。

#### 命題 23 {#ac-v-s1-prop-23 .statement tag=04OO}

Let A be a K-algebra, $G$ a locally finite group of operators on A, S a multiplicative subset of A stable under $G$ and $S^G$ the set $S \cap A''$. 次に、$(S^G)^{-1}A$ から $S^{-1}A$ (章 II, § 2, no. 1、系 2 から命題 2) の標準写像は、写像 $(S^G)^{-1}A^G$ から $(S^{-1}A)^G$ である同型です。

すべての $s \in S$ について、$s, s_1, \ldots, s_q$ を $G$ の下の s の軌道の別個の元とします。 $ss_1 \ldots s_q \in S^G$ のように、最初の主張は章 11、§ 2, no. 3、命題 8 から続きます。$(S^G)^{-1}A$ と $S^{-1}A$ を正規に同一視すると、$(S^G)^{-1}A^G$ のすべての元は明らかに $G$ のもとで不変です。逆に、$a/t$ を $G$ ($a \in A, t \in S^G$) の下で不変である $(S^G)^{-1}A$ の元とします。 $a, (1 \leq j \leq m)$ が $G$ の下の $a$ の軌道の別個の元である場合、$1 \leq j \leq m$ に対して $a_j/t = a/t$ が存在するため、$1 \leq j \leq m$ に対して $s(a_j - a) = 0$ となるような $s \in S^G$ が存在します。他の語では、sa は $G$ で不変であり、$a/t = (sa)/(st)$ と同様に、確かに $a/t \in (S^G)^{-1}A^G$ です。

#### 系 {#ac-v-s1-n9-cor-1 .statement tag=04OP}

Aを整域、Kを分数の体、$G$をAのローカル演算子の有限群とします。すると、$G$はKで演算され、$K^G$は$A^G$の分数の体になります。

$- \{0\}$は$G$以下で安定しています。

### 練習問題 {#ac-v-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
