---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 8
section_title: Determinants
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 522-541, 637-644
pdf_pages: 0546-0565, 0661-0668
extraction: ocr
subsections:
    - "no": 1
      title: DETERMINANTS OF AN ENDOMORPHISM
      page: 522
      pdf_page: 546
    - "no": 2
      title: CHARACTERIZATION OF AUTOMORPHISMS OF A FINITE-DIMENSIONAL FREE MODULE
      page: 523
      pdf_page: 547
    - "no": 3
      title: DETERMINANT OF A SQUARE MATRIX
      page: 524
      pdf_page: 548
    - "no": 4
      title: CALCULATION OF A DETERMINANT
      page: 526
      pdf_page: 550
    - "no": 5
      title: MINORS OF A MATRIX
      page: 528
      pdf_page: 552
    - "no": 6
      title: EXPANSIONS OF A DETERMINANT
      page: 530
      pdf_page: 554
    - "no": 7
      title: APPLICATION TO LINEAR EQUATIONS
      page: 534
      pdf_page: 558
    - "no": 8
      title: CASE OF A COMMUTATIVE FIELD
      page: 536
      pdf_page: 560
    - "no": 9
      title: THE UNIMODULAR GROUP $\mathbf{SL}(n, A)$
      page: 537
      pdf_page: 561
    - "no": 10
      title: THE $\mathbf{A}[X]$-MODULE ASSOCIATED WITH AN $\mathbf{A}$-MODULE ENDOMORPHISM
      page: 538
      pdf_page: 562
    - "no": 11
      title: CHARACTERISTIC POLYNOMIAL OF AN ENDOMORPHISM
      page: 540
      pdf_page: 564
statements: 36
exercises: 26
content_sha256: bdd50ebe8b8d502fc1d5571b2da45039d40d32f867d53cb96142a1ff8b331296
translated_from: content/en/alg/III/08_s8_determinants.md
translation_method: google
source_content_sha256: a8722fe29a021a8f3f62eb7c41ed5736542a85db99ded2b20167525ac22836eb
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: ddf102d095c63323d2124712286ba0164e11cd4b241d6ae23dc9c4581fa6117f
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 8。 行列式

### 1. 行列式/自己準同型

$M$ を、$n$ 元の有限基底と $M$ の $u$ 自己準同型を持つ $A$ モジュールとします。 $A$ 加群 $\bigwedge^n(M)$ は単一の自由加群であり、$A$ (no. 8、系 1 ～ 定理 1) と同型です。 $\bigwedge^n(u)$ は、この加群の自己準同型であるため、一意に決定される比率 $\lambda \in A$ のホモテティー $z \mapsto \lambda z$ です (II, § 2, no. 3、命題 5)。

#### 定義 1 {#alg-iii-s8-def-1 .statement tag=0642}

*無料の $A$ モジュールの行列式自己準同型 $u$ 有限次元の $M$ $n$* (II, § 7, no. 2、系 ～ 命題 3 および注意 1)、 * $\det u$ で表され、 * $\bigwedge^n(u)$ * が比のホモテティー となるようなスカラー $\lambda$ です* $\lambda$。

§ 7, no. 2 の公式 (4) により、$\det u$ は次のような一意のスカラーになります。

(1)
$$
u(x_1) \wedge u(x_2) \wedge \cdots \wedge u(x_n) = (\det u) \cdot x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$
$n$ 元の $M$ の数列 $(x_i)_{1 \leq i \leq n}$ ごとに。 $\det(u) = 1$ の場合、$u$ は *ユニモジュラー* と言われます。

#### 命題 1 {#alg-iii-s8-prop-1 .statement tag=0643}

(i) *$u$ と $v$ が有限次元の自由 $A$ 加群 $M$ の 2 つの自己準同型である場合、*

(2)
$$
\det(u \circ v) = (\det u)(\det v).
$$

(ii) $\det(1_M) = 1$; *すべての自己同型* $u$ *の* $M$、$\det u$ *は反転可能* $A$ *および*

(3)
$$
\det(u^{-1}) = (\det u)^{-1}.
$$

$n$ が $M$ の次元である場合、これは関係 $\bigwedge^n(u \circ v) = (\bigwedge^n(u)) \circ (\bigwedge^n(v))$ § 7, no. 2、公式 (3)) の直後に続きます。

$M$ を、有限基底 $(e_i)_{1 \leq i \leq n}$ を持つ自由な $A$ モジュールとしましょう。与えられた数列 $(x_i)_{1 \leq i \leq n}$ の $n$ 元の $M$、 行列式のこの数列 *に関して*、与えられた基底 $(e_i)$ について混乱が生じない場合、$\det(x_1, x_2, \ldots, x_n)$ で示されます。 基底は、自己準同型の行列式、$M$ の $u$ で、$1 \leq i \leq n$ に対して $u(e_i) = x_i$ になります。その後、公式までに (1)

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = \det(x_1, x_2, \ldots, x_n) \ e_1 \wedge e_2 \wedge \cdots \wedge e_n
$$

そして、この関係は、$M^n$の写像$(x_i) \mapsto \det(x_1, x_2, \ldots, x_n)$を$A$に特徴づけます。この写像が *交代的 n 線形形式 * であることを示しています。 § 7, no. 4, 命題 7 のおかげで、交代的 $n$ 線形形式の $A$ 加群は $\bigwedge^n(M)$ の双対と正準的に同型であり、$\bigwedge^n(M)$ は $A$ と同型であることがわかります。 交代的 $M^n$ 上の n-線形形式を書くことができます*

$$(x_1, \ldots, x_n) \mapsto \alpha \det(x_1, x_2, \ldots, x_n)$$

一部の$\alpha \in A$。

#### 命題 2 {#alg-iii-s8-prop-2 .statement tag=0644}

*$M$ を、有限の基底 $(e_i)_{1 \leq i \leq n}$ および $v$ 自己準同型の $M$ を持つ自由な $A$ モジュールとします。 数列 $(x_i)_{1 \leq i \leq n}$ の $n$ 元の $M$ ごとに、*

$$
\det(v(x_1), \ldots, v(x_n)) = (\det v) \det(x_1, \ldots, x_n).
$$

$u$ が $M$ の自己準同型で、すべての $i$ に対して $u(e_i) = x_i$ となる場合、

$$
v(x_i) = (v \circ u)(e_i)
$$

したがって、(5) は (2) から導かれます。

### 2. 有限次元の自由加群の自己同型の特徴付け

#### 定理 1 {#alg-iii-s8-thm-1 .statement tag=0645}

*$M$ を有限次元の自由 $A$ 加群、$M$ の $u$ 自己準同型とする。次の条件は同等です:*
(a) $u$ は全単射です。
(b) $u$ は右反転可能です (II, § 1, no. 9、系 1 ～ 命題 15)。
(c) $u$ は反転可能なままです (II, § 1, no. 9、系 2 ～ 命題 15)。
(d) $u$ は全射です。
(e) $\det u$ は $A$ で反転可能です。

$(e_i)_{1 \leq i \leq n}$ を $M$ の基底とします。 $1 \leq i \leq n$ に対して $x_i = u(e_i)$ の場合、

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = (\det u) e_1 \wedge e_2 \wedge \cdots \wedge e_n.
$$

§ 7, no. 9、定理 2 により、$M$ の $x_i$ から形基底に必要かつ十分な条件は、$\det u$ が $A$ の可逆元であることです。これは (a) と (e) の同値を証明します。 (a) は明らかに条件 (b)、(c)、および (d) のそれぞれを暗示していることに注目してください。 条件 (b)、(c)、および (d) のそれぞれが (e) を意味することを証明することはまだ残っています。 Now, if there exists an endomorphism $v$ of $M$ such that $v \circ u = 1_M$ or $u \circ v = 1_M$, then $(\det v)(\det u) = 1$ and hence $\det u$ is invertible in $A$. $u$ が全射である場合、$\bigwedge^n(u)$ (§ 7, no. 2, 命題 3) も同様です。他の語ホモテティー では、$A$ の det $u$ が全射であり、これはすぐに det $u$ が可逆であることを意味します。

#### 命題 3 {#alg-iii-s8-prop-3 .statement tag=0646}

*$M$を有限次元の自由$A$加群とする。 $M$ の各自己準同型 $u$ について、次の条件は同等です:*
  (f) $u$ は単射です。
  (g) det $u$ は、$A$ の零の因子ではありません。

定理 1 の証明と同じ記法では、$u$ が単射であるためには、$x_i$ が線形独立であることが必要かつ十分です。 § 7, no. 9、命題 12 によって、関係 $\lambda x_1 \wedge x_2 \wedge \cdots \wedge x_n = 0$ ($\lambda \in A$ とともに) $\lambda = 0$ が暗示されることがこれに必要かつ十分です。しかし、$e_1 \wedge \cdots \wedge e_n$ は $\Lambda^n(M)$ の基底であるため、これは $\lambda (\det u) = 0$ と同等です。 よって命題。

#### 注意 {#alg-iii-s8-n2-rem-1 .statement tag=0647}

$A$ が体のとき、定理 2 の条件 (e) は、両方とも $\det u \neq 0$ を意味するため、命題 3 の条件 (g) と等価です。従って、この場合、定理 1 と命題 3 のすべての条件は同等です (cf. II, § 7, no. 4、系 ～ 命題 9)。

### 3. 行列式/平方行列

#### 定義 2 {#alg-iii-s8-def-2 .statement tag=0648}

*$I$ を、環 $A$ にわたる型 $(I, I)$ の有限集合、$A$ 可換環および $X$ 平方行列とします。 (II, § 10, no. 7)。 $A^I$の標準基底に対する行列が$X$である$A$モジュール$A^I$の自己準同型$u$の行列式は、$X$の行列式と呼ばれます$\det X$.* で示されます。

$X = (\xi_{ij})_{(i,j) \in I \times I}$ と $(e_i)_{i \in I}$ が $A^I$ の標準基底である場合、自己準同型 $u$ は次のように求められます。
$$
u(e_i) = \sum_{j \in J} \xi_{ji} e_j.
$$

$I = \{1, n\} \subset \mathbf{N}$のとき、$i \in I$に$x_i = u(e_i)$と書くと、$X$の行列式が関係で定義されます。
$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = (\det X) e_1 \wedge e_2 \wedge \cdots \wedge e_n
$$
他の語では、$A^n$の標準基底に対して、$\det X$は行列式$\det(x_1, x_2, \ldots, x_n)$に等しい。その結果:

#### 命題 4 {#alg-iii-s8-prop-4 .statement tag=0649}

*$A^n$の$n$ベクトル$x_1, \ldots, x_n$について、$X(x_1, \ldots, x_n)$は位数$n$の平方行列を表します。その$i$番目の列は$x_i$ は $1 \leq i \leq n$ です。それでは写像*
$$
(x_1, \ldots, x_n) \mapsto \det(X(x_1, \ldots, x_n))
$$
*$(A^n)^n$ の $A$ は交代的および $n$ 線形です。*

特に、列が 2 つ等しい行列の行列式は、零です。 行列の列に対して置換が実行された場合、新しい行列の行列式は古いものに $\varepsilon_{\sigma}$ を乗じたものに等しくなります。 行列の 1 つ列に、別の添字の列のスカラー 倍数が追加された場合、新しい行列の行列式は古いものと等しくなります。

より一般的には、$M$ を有限次元 $n$ の空き $A$ モジュールとし、$(e_i)_{i \in I}$ を $M$ の基底とします。 $M$ のすべての自己同型 $u$ について、$X$ が基底 $(e_i)$ に関して $u$ の行列である場合、

$$
\det(u) = \det(X)
$$

定義からはすぐに以下のようになります。

$I = \{1, n\}$、$X$の行列式も

$$
\det(\xi_{ij})_{1 \leq i \leq n, 1 \leq j \leq n}
$$

混乱が生じない場合は、単に $\det(\xi_{ij})$ または

$$
\begin{vmatrix}
\xi_{11} & \xi_{12} & \ldots & \xi_{1n} \\
\xi_{21} & \xi_{22} & \ldots & \xi_{2n} \\
\ldots & \ldots & \ldots & \ldots \\
\xi_{n1} & \xi_{n2} & \ldots & \xi_{nn}
\end{vmatrix}
$$

$X = 1$、行列 $X$ の場合、ユニモジュラーと呼ばれます。

#### 例 {#alg-iii-s8-n3-exa-1 .statement tag=064A}

(1) The determinant of the empty matrix is equal to 1; the determinant of a square matrix of order 1 is equal to the unique element of this matrix. 位数 2 の行列について

$$
\begin{pmatrix}
\xi_{11} & \xi_{12} \\
\xi_{21} & \xi_{22}
\end{pmatrix}
$$

次に、上記の記法で、

$$
x_1 \wedge x_2 = (\xi_{11} e_1 + \xi_{21} e_2) \wedge (\xi_{12} e_1 + \xi_{22} e_2) = \xi_{11} \xi_{22} e_1' \wedge e_2 + \xi_{21} \xi_{12} e_2 \wedge e_1
$$

よって

$$
\begin{vmatrix}
\xi_{11} & \xi_{12} \\
\xi_{21} & \xi_{22}
\end{vmatrix} = \xi_{11} \xi_{22} - \xi_{12} \xi_{21}.
$$

nos の結果の一部を行列の言語に翻訳します。 1 と 2:

#### 命題 5 {#alg-iii-s8-prop-5 .statement tag=064B}

*$X$ と $Y$ が同じ有限インデックス集合で可換環 $A$ 上の 2 つの正方行列である場合、*

$$
\det(XY) = (\det X)(\det Y).
$$

X が可逆であるためには、det X が A の可逆元であることが必要かつ十分です。

(9) $$
\det(X^{-1}) = (\det X)^{-1}.
$$

これは、no. 1、命題 1 および no. 2、定理 1 の直後に続きます。

#### 系 {#alg-iii-s8-n3-cor-1 .statement tag=064C}

*2 つの類似した正方行列は等しい行列式となります。*

P が可逆平方行列の場合、(8) と (9) により $\det(PXP^{-1}) = \det X$ になります。

#### 命題 6 {#alg-iii-s8-prop-6 .statement tag=064D}

*有限位数の平方行列 X の列が線形独立であるためには、det X が A の零の因子にならないことが必要かつ十分です。*

これは、no. 2、命題 3 から続きます。

### 4. 行列式の計算

#### 補題 1 {#alg-iii-s8-lem-1 .statement tag=064E}

*A を可換環 、M 自由A-加群を基底 $(e_j)_{j \in J}$ とします。ここで、インデックス付け集合 J は完全に順序付けされています。すべての整数 $p \leq \mathrm{Card}(J)$、すべての交代的 p 線形写像 $f : M^p \to N$ (N は A-加群)、および M $(1 \leq i \leq p)$ の p 元 $x_i = \sum_{j \in J} \xi_{ji} e_j$ のすべての族について、

$$
f(x_1, x_2, \ldots, x_p)
= \sum_{j_1 < j_2 < \cdots < j_p} \left( \sum_{\sigma \in S_p} \varepsilon_\sigma \cdot \xi_{j_{\sigma(1)}, 1} \xi_{j_{\sigma(2)}, 2} \cdots \xi_{j_{\sigma(p)}, p} \right) f(e_{j_1}, \ldots, e_{j_p})
$$

*ここで* $(j_k)_{1 \leq k \leq p}$ *は、真に増加するの集合、pの数列、Jの元を通過します。*

今

$$
f(x_1, \ldots, x_p) = \sum_{(j_k)} \xi_{j_1, 1} \xi_{j_2, 2} \cdots \xi_{j_p, p} f(e_{j_1}, e_{j_2}, \ldots, e_{j_p})
$$

ここで、$(j_k)_{1 \leq k \leq p}$ は J の p 元の *すべて* 数列を通過します。その場合、§ 7, no. 4 から f の系を適用する 1 から命題 7 で十分です。

特に、J が有限で、n 元があり、$x_i = \sum_{j \in J} \xi_{ji} e_j$ $(1 \leq i \leq n)$ が M の n 元である場合、次のようになります。

(11) $$
x_1 \wedge x_2 \wedge \cdots \wedge x_n
= \left( \sum_{\sigma \in S_n} \varepsilon_\sigma \xi_{j_{\sigma(1)}, 1} \xi_{j_{\sigma(2)}, 2} \cdots \xi_{j_{\sigma(n)}, n} \right) e_{j_1} \wedge e_{j_2} \wedge \cdots \wedge e_{j_n}
$$

ここで、$(j_k)_{1 \leq k \leq n}$ は、増加する位数、よってに配置された J の n 元のうちの一意の数列です。

(12) $$
\det(x_1, x_2, \ldots, x_n) = \sum_{\sigma \in S} \varepsilon_\sigma \cdot \xi_{j_{\sigma(1)}, 1} \xi_{j_{\sigma(2)}, 2} \cdots \xi_{j_{\sigma(n)}, n}.
$$

補題 1 の記法で、式 (10) と (12) を比較すると、次のようになります。

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_p = \sum_{H \in \mathscr{F}_p(J)} \det(x_{H,1}, x_{H,2}, \ldots, x_{H,p}) e_H
$$

where $\mathscr{F}_p(J)$ is the set of subsets of $J$ with $p$ elements and, for every subset $H \in \mathscr{F}_p(J)$, we write $x_{H,i} = \sum_{j \in H} \xi_{ji} e_j$ and $e_H = e_{j_1} \wedge e_{j_2} \wedge \cdots \wedge e_{j_p}$, $(j_k)_{1 \leq k \leq p}$ being the sequence of elements of $H$ arranged in increasing order, it being understood that $\det(x_{H,1}, \ldots, x_{H,p})$ is taken with respect to the basis $(e_{jk})_{1 \leq k \leq p}$.

#### 命題 7 {#alg-iii-s8-prop-7 .statement tag=064F}

*$I$ を可換環 $A$ 上の型 (I, I) の有限集合と $X = (\xi_{ji})_{(j, i) \in I \times I}$ 平方行列とします。それから*

$$
\det X = \sum_{\sigma \in S_I} \varepsilon_\sigma \left( \prod_{i \in I} \xi_{\sigma(i), i} \right)
$$

*ここで、$\sigma$ は $I$ の置換の群 $S_I$ を通過し、$\varepsilon_\sigma$ は $\sigma$* (I, § 5, no. 7) の署名です。

注意は、$I = \{1, n\} \subset \mathbf{N}$ で公式 (12) を適用するだけで十分である場合に限定されます。ここで、$(e_i)_{1 \leq i \leq n}$ は $A^n$ の標準基底で、$x_i$ は $X$ (cf.) の列です。 no. 3、公式 (6))。

特に、位数の行列の行列式については、

$$
X = \begin{pmatrix}
\xi_{11} & \xi_{12} & \xi_{13} \\
\xi_{21} & \xi_{22} & \xi_{23} \\
\xi_{31} & \xi_{32} & \xi_{33}
\end{pmatrix}
$$

私たちは持っています

$$
\det(X) = \xi_{11} \xi_{22} \xi_{33} + \xi_{12} \xi_{23} \xi_{31} + \xi_{21} \xi_{32} \xi_{13} - \xi_{13} \xi_{22} \xi_{31} - \xi_{12} \xi_{21} \xi_{33} - \xi_{11} \xi_{23} \xi_{32}.
$$

#### 命題 8 {#alg-iii-s8-prop-8 .statement tag=064G}

*可換環を超えるすべての平方行列 $X$ について、転置行列 ${}^t X$ の行列式は、$X$ の行列式と等しくなります。*

$X$ が型 (I, I) であるとします。 置換 $\sigma, \tau$ または $S_I$ の順序付けられたすべての対について (乗法は可換であるため)

$$
\prod_{i \in I} \xi_{\sigma(i), i} = \prod_{j \in I} \xi_{\sigma(\tau(j)), \tau(j)}.
$$

特に $\tau = \sigma^{-1}$ を取り上げます。 $\varepsilon_{\sigma^{-1}} = \varepsilon_\sigma$ という事実を使用すると、次のことがわかります。

$$
\det X = \sum_{\sigma \in S_I} \varepsilon_\sigma \left( \prod_{i \in I, i} \xi_{i, \sigma(i)} \right),
$$

これは命題を証明します。

#### 系 1 {#alg-iii-s8-prop-8-cor-1 .statement tag=064H}

$\mathbf{A}^n$ の n ベクトル $x_1, \ldots, x_n$ について、$1 \leq i \leq n$ に対して、$Y(x_1, \ldots, x_n)$ は i 番目の行が $x_i$ である位数 n の平方行列を表します。それから写像
$$
(x_1, \ldots, x_n) \mapsto \det(Y(x_1, \ldots, x_n))
$$
$(\mathbf{A}^n)^n$ から $\mathbf{A}$ は交代的で n 線形です。

#### 系 2 {#alg-iii-s8-prop-8-cor-2 .statement tag=064I}

可換環 $\mathbf{A}$ 上の有限位数の平方行列 $X$ については、次の条件が等価です。
(i) $X$ の行は線形独立です。
(ii) $X$ の列は線形独立です。
(iii) $\det X$ は、$\mathbf{A}$ の零の因子ではありません。

これは、上記の no. 3、命題 6、および命題 8 の直後に続きます。

#### 系 3 {#alg-iii-s8-prop-8-cor-3 .statement tag=064J}

$u$ を有限次元自由 $\mathbf{A}$ 加群 $M$ の自己準同型と双対 $M^*$ (II, § 2, no. 5, 定義 5) の $^t u$ 転置自己準同型とします。それから
$$
\det(^t u) = \det(u).
$$
$X$ が $M$ の基底に対して $u$ の行列である場合、$^t X$ は双対基底に対して$^t u$ の行列 (II, § 10, no. 4, 命題 3); $\det(u) = \det(X)$ と $\det(^t u) = \det(^t X)$ のように、結論は命題 8 から導き出されます。

### 5. 行列の未成年者

$X$ を型 (I, J) の長方形行列 $(\xi_{ij})_{(i,j) \in I \times J}$ とし、そのインデックス付け集合 I と J は完全に順序付けされています。 $H \subset I$ と $K \subset J$ が元の同じ数 $p$ を持つ有限部分集合である場合、一意の増加する全単射 $\phi : H \to K$ (集合理論, III, § 5, no. 3, 命題 6); $(\xi_{i,\phi(j)})_{(i,j) \in H \times H}$ に等しい型 (H, H) の $X_{H,K}$ 平方行列で表します。 $X$ 属するから可換環 $\mathbf{A}$ の元を、行列式 $\det(X_{H,K})$ を添字の行列 $X$ H, K のマイナーと呼びます。これらの行列式（Iの部分集合とJのすべての注文対（H、K）に対して、それぞれ$p$元の$X$位数$p$の未成年者とも呼ばれます。 これで記法:

#### 命題 9 {#alg-iii-s8-prop-9 .statement tag=064K}

$M$ を、基底 $(e_i)_{i \in J}$ (有限またはその他) を持つ $\mathbf{A}$ モジュールとし、そのインデックス付け集合 $J$ は完全に順序付けされています。 整数 $p > 0$ ごとに、$(e_H)_{H \in \mathfrak{S}_p(J)}$ を $\wedge^p(M)$ (§ 7, no. 8) の対応する基底とします。 $(x_i)_{1 \leq i \leq p}$ を $p$ の数列 、$M$ の元とします。させてください
$$
x_i = \sum_{j \in J} \xi_{ji} e_j \quad \text{for } i \in I = \{1, p\}
$$

そして、$X$ は型 $(J, I)$ の行列 $(\xi_{ji})$ を表すものとします。それから

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_p = \sum_{H \in \mathfrak{F}_p(J)} (\det X_{H,I}) e_H.
$$

where $H$ runs through the set $\mathfrak{F}_p(J)$ of subsets of $J$ with $p$ elements.

これは、no. 4 の公式 (12) と no. 3 の公式 (6) の直後に続きます。

#### 命題 10 {#alg-iii-s8-prop-10 .statement tag=064L}

$M$ と $N$ を、$u$ のそれぞれ次元 $m$ と $n$、$u : M \to N$ 線形写像と $X$ 行列の 2 つの空き $A$ モジュールとします。 基底 $(e_i)_{1 \leq i \leq m}$ の $M$ と基底 $(f_j)_{1 \leq j \leq n}$ の $N$ です。 Then, for every integer $p \leq \inf(m, n)$, the matrix of $\wedge^p(u)$ with respect to the basis $(e_K)_{K \in \mathfrak{F}_p(I)}$ of $\wedge^p(M)$ and the basis $(f_H)_{H \in \mathfrak{F}_p(J)}$ of $\wedge^p(N)$ (where we have written $I = \{1, m\}$ and $J = \{1, n\}$) is the matrix $(\det(X_{H,K}))$ of type $(\mathfrak{F}_p(J), \mathfrak{F}_p(I))$ (and hence with $\binom{n}{p}$ rows and $\binom{m}{p}$ columns).

$p$ 元を含む部分集合 $K \subset J$ の場合、$(j_k)_{1 \leq k \leq p}$ を増加する位数に配置された $K$ の元の数列とします。 定義作 $\wedge^p(u)$ 作、§ 7, no. 2 作、公式作 (4)

$$
\wedge^p(u)(e_K) = u(e_{j_1}) \wedge u(e_{j_2}) \wedge \cdots \wedge u(e_{j_p}).
$$

Hence the element of the matrix of $\wedge^p(u)$ which is in the row of index $H$ and the column of index $K$ is the component of index $H$ of the element $u(e_{j_1}) \wedge \cdots \wedge u(e_{j_p})$; it is therefore equal to $\det(X_{H,K})$ by Proposition 9.

行列 $(\det(X_{H,K}))$ は、行列 $X$ の $p$ 番目の外面冪と呼ばれ、$\wedge^p(X)$ で表されます。 $p = m = n$、$\wedge^n(X)$ は元 $\det(X)$ の単一で行列になります。

#### 命題 11 {#alg-iii-s8-prop-11 .statement tag=064M}

$M$ を有限次元 $n$ の自由な $A$ モジュールとします。 $M$ の自己準同型 $u$ ごと、および元の $\xi, \eta$ $A$ のすべての注文された対について、

$$
\det(\xi 1_M + \eta u) = \sum_{k \geq 0} \operatorname{Tr}(\wedge^k(u)) \xi^{n-k} \eta^k.
$$

$(e_i)_{1 \leq i \leq n}$ を $M$ の基底とし、$I = \{1, n\}$ とします。 (18) の左側を計算するにするには、 形積を行う必要があります。

$$
(\xi e_1 + \eta u(e_1)) \wedge (\xi e_2 + \eta u(e_2)) \wedge \cdots \wedge (\xi e_n + \eta u(e_n))
$$

これは項 $\xi^{n-p} \eta^p z_K$ の和に等しく、ここで

$$
z_K = x_1 \wedge x_2 \wedge \cdots \wedge x_n
$$

$x_i = u(e_i)$ は $i \in K$ 、$x_i = e_i$ は $i \in H = I - K$ で、整数 $p$ は区間 $[0, n]$ を通過し、各 $p$ について、$K$ は部分集合の集合を通過します。 I と $p$ 元。 $i_1 < i_2 < \cdots < i_{n-p}$ (それぞれ $j_1 < j_2 < \cdots < j_p$) が、H (それぞれ K) の元を増加する位数に並べると、 ($§ 7$, no. 8, 系 1 から定理 1 および公式 (19))

$$
z_K = \rho_{H, K} e_{i_1} \wedge e_{i_2} \wedge \cdots \wedge e_{i_{n-p}} \wedge u(e_{j_1}) \wedge \cdots \wedge u(e_{j_p}).
$$

しかし、$X$ が基底 $(e_i)$ に関して $u$ の行列である場合、命題 10 によって

$$
u(e_{j_1}) \wedge \cdots \wedge u(e_{j_p}) = \sum_{L \in \mathfrak{F}_p(I)} (\det X_{L, K}) e_L
$$

したがって

$$
z_K = \rho_{H, K} \sum_{L \in \mathfrak{F}_p(I)} (\det X_{L, K}) e_H \wedge e_L.
$$

Now $H \cap L \neq \varnothing$ except for $L = K$; it therefore follows from $§ 7$, no. 8, formula (20) that $z_K = (\det X_{K, K}) e_1 \wedge e_2 \wedge \cdots \wedge e_n$ and formula (18) then follows from Proposition 10 and the definition of the trace of a matrix (II, $§ 10$, no. 11, formulae (49) and (50)).

#### 系 {#alg-iii-s8-n5-cor-1 .statement tag=064N}

*命題 11 と同じ仮説の下、A-加群 $\bigwedge(M)$ の自己準同型 $\bigwedge(u)$ について

$$(19)$$
$$
\operatorname{Tr}(\bigwedge(u)) = \det(1_M + u).
$$

It suffices to replace $\xi$ and $\eta$ by 1 in (18) and observe that the matrix of $\bigwedge(u)$ with respect to the basis of the $e_H$ ($H \in \mathfrak{F}(I)$) is the diagonal matrix of the matrices of the $\bigwedge^k(u)$ for $\geq k$ 0 (II, $§ 10$, no. 7, *Example* IV).

### 6. 行列式の拡張

I を完全に順序付けされた有限インデックス付け集合とします。 For every 部分集合 H of I let H' denote the complement I - H. Let $X = (\xi_{ij})$ be 平方行列 of 型 (I, I), which can be considered as 行列 of 自己準同型 $u$ of $M = A^I$ with respect to 標準基底 $(e_i)_{i \in I}$ of M. Let $n = \operatorname{Card}(I)$ and let H be 部分集合 of I with $q \leq n$ 元 and K 部分集合 of I と $n - q$ 元;そうすれば (no. 5, 命題 10) と書くことができます

$$
(\bigwedge^q(u))(e_H) = \sum_R \det(X_{R, H}) e_R
$$
$$
(\bigwedge^{n-q}(u))(e_K) = \sum_S \det(X_{S, K}) e_S
$$

ここで、R (それぞれ S) は、$q$ (それぞれ $n - q$) 元とともに、I の部分集合の集合を通過します。 $§ 7$、no. 8、式 (19) および (20) から次のようになります。

$$
e_R \wedge e_S = 0
$$

$S = R'$、よって公式の場合を除く

$$
(20) \quad (\wedge^q(u)(e_H)) \wedge (\wedge^{n-q}(u)(e_K)) = \sum_R \rho_{R, R'} \det(X_{R, H}) \det(X_{R', K}) e_I
$$

where $R$ runs through the set $\mathscr{F}_q(I)$ of subsets of $I$ with $q$ elements.

$K = H'$ を取ると、$\wedge^n(u)$ (§ 7, no. 2, 公式 (4)) と § 7, no. 3, 系 1 から命題 5 の定義から、(20) の右辺は $\rho_{H, H'} \wedge^n(u)(e_I)$ になります。したがって (no. 1, 公式 (1) および § 7, no. 2, 公式 (4))

$$
(21) \quad \det(X) = \rho_{H, H'} \sum_{R \in \mathscr{F}_q; R' \neq R} \rho_{R, R'} \det(X_{R, H}) \det(X_{R', H'}).
$$

一方、$K \neq H'$ の場合は、$H \cap K \neq \varnothing$; (20) の左辺は $\pm \wedge^n(u)(e_H \wedge e_K)$ なので、それは零、よって

$$
(22) \quad \sum_R \rho_{R, R'} \det(X_{R, H}) \det(X_{R', K}) = 0 \quad \text{for } K \neq H'.
$$

(21) の右辺は、添字属するが H になる q 列と、H* の補数 H' が添字属するになる n - q 列による、行列 $X$ の行列式の *ラプラス展開* と呼ばれます。マイナー $\det(X_{R, H})$ と $\det(X_{R', H'})$ はときどきで *補完* と呼ばれます。

ラプラス展開の重要な単純なケースは、$I = \{1, n\}$ と $q = 1$、したがって $H = \{i\}$ である場合です。 $I$ の部分集合 $R = \{j\}$ ごとに、元が 1 つ、次に $\det X_{R, H} = \xi_{ji}$ が追加されます。 $\det X_{R', H'}$ のマイナーは、$X$ で添字 $j$ と添字の列を抑制することで得られた行列から正規 (no. 5) から派生した平方行列の行列式です。 $i$。これを平方行列を $X^{ji}$ で表します。明らかに$\rho_{H, H'} = (-1)^{i-1}$と$\rho_{R, R'} = (-1)^{j-1}$です。したがって、この場合 (21) は次のようになります。

$$
(23) \quad \det X = \sum_{j=1}^n (-1)^{i+j} \xi_{ji} \det(X^{ji})
$$

そして同様に (22) から得られます。

$$
(24) \quad \sum_{j=1}^n (-1)^{ji} \xi_{ji} \det(X^{jk}) = 0 \quad \text{for } k \neq i.
$$

公式 (23) は、X の行列式の添字 i* の列による * 拡張として知られています。 スカラー $(-1)^{i+j} \det(X^{ji})$ は、$X$ の添字 $j$ および $i$ (または、言葉の乱用により、$\xi^{ji}$ の補因子) の *補因子* と呼ばれます。

$X$ の補因子 * の *行列は行列

$$
(25) \quad Y = ((-1)^{i+j} \det(X^{ji}))
$$

$j$ 番目の行と $i$ 番目の列の元は、添字 $j$ と $i$ の余因子です。式 (23) と (24) は公式と等価です

$$(26)$$
$$
{}^tY . X = (\det X) I_n.
$$

したがって：

#### 命題 12 {#alg-iii-s8-prop-12 .statement tag=064O}

*型 $(n, n)$ のすべての可逆平方行列 $X$ について、$X$ の逆数は公式で与えられます*

$$(27)$$
$$
X^{-1} = (\det X)^{-1} {}^t Y
$$

*ここで、$Y$は$X$の補因子行列です。*

$X$ の *転置* を考慮し、no. 5 の命題 8 を使用することにより、行の 2 つの相補的な集合に関連するラプラス展開、特に 1 行による $\det X$ の展開を取得できます。したがって、以下と同等の公式が存在します。

$$(28)$$
$$
X . {}^t Y = (\det X) I_n,
$$

上記記法で。

It is easily verified that if $X$ is the matrix of an endomorphism $u$ of a free $\mathbf{A}$-module $M$ of dimension $n$ with respect to a basis $(e_i)_{1 \leq i \leq n}$, ${}^t Y$ is the matrix of the endomorphism $\tilde{u}$ of $M$ defined by the following condition: for every set of $n$ elements $x, y_2, \ldots, y_n$ of $M$,

$$
\tilde{u}(x) \wedge y_2 \wedge \cdots \wedge y_n = x \wedge u(y_2) \wedge \cdots \wedge u(y_n).
$$

$\tilde{u}$ は、$u$ (cf. § 11, no. 11、系から命題 13) の *共転置* と呼ばれます。

#### 例 {#alg-iii-s8-n6-exa-1 .statement tag=064P}

(1) *Vandermonde determinant.* Given a sequence $(\zeta_i)_{1 \leq i \leq n}$ of $n$ elements of $\mathbf{A}$, the *Vandermonde determinant* of this sequence is the determinant

$$
V(\zeta_1, \zeta_2, \ldots, \zeta_n) = \begin{vmatrix}
1 & 1 & \ldots & 1 \\
\zeta_1 & \zeta_2 & \ldots & \zeta_n \\
\zeta_1^2 & \zeta_2^2 & \ldots & \zeta_n^2 \\
\vdots & \vdots & \ddots & \vdots \\
\zeta_1^{n-1} & \zeta_2^{n-1} & \ldots & \zeta_n^{n-1}
\end{vmatrix}
$$

それを示しましょう

$$(29)$$
$$
V(\zeta_1, \zeta_2, \ldots, \zeta_n) = \prod_{i < j} (\zeta_j - \zeta_i).
$$

$n = 1$に対して命題は明らかなので、$n$に対して帰納法で議論します。

For each index $k \geq 2$, we subtract from the row of index $k$ the row of index $k - 1$ multiplied by $\zeta_1$; the value of the determinant is unaltered and hence

$$
V(\zeta_1, \zeta_2, \ldots, \zeta_n) = \begin{vmatrix}
1 & 1 & \cdots & 1 \\
0 & \zeta_2 - \zeta_1 & \cdots & \zeta_n - \zeta_1 \\
0 & \zeta_2(\zeta_2 - \zeta_1) & \cdots & \zeta_n(\zeta_n - \zeta_1) \\
\cdots & \cdots & \cdots & \cdots \\
0 & \zeta_2^{n-2}(\zeta_2 - \zeta_1) & \cdots & \zeta_n^{n-2}(\zeta_n - \zeta_1)
\end{vmatrix}
$$

よって、最初の列で拡張し、こうして得られたマイナー ($2 \leq k \leq n$) から添字 $k - 1$ の列から因子 $\zeta_k - \zeta_1$ を取り出します。

$$
V(\zeta_1, \ldots, \zeta_n) = (\zeta_2 - \zeta_1)(\zeta_3 - \zeta_1) \cdots (\zeta_n - \zeta_1) V(\zeta_2, \ldots, \zeta_n)
$$

これは、帰納法によって (29) を確立します。

(2) 「行列の上三角行列」（II, § 10, no. 7、例IV）の形で表される位数$n$の平方行列を考えます。

$$
X = \begin{pmatrix} Y & T \\ 0 & Z \end{pmatrix}
$$

私たちはそれを示します

$$
\det X = (\det Y)(\det Z).
$$

$n$ を、行列 $X$ の位数、$Y$ の $h$、$\mathbf{A}^n$ の $(e_i)_{1 \leq i \leq n}$ 標準基底、および $x_i$ ($1 \leq i \leq n$) 列とします。 $X$; 仮定は、列 $x_1, \ldots, x_h$ 属するから $\mathbf{A}^n$ の部分加群と基底 $e_1, \ldots, e_h$、そして定義まで (no. 3, 公式 (6)) を意味します。

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = (\det Y)e_1 \wedge e_2 \wedge \cdots \wedge e_h.
$$

一方、添字 $i > h$ ごとに、$x_i = y_i + z_i$ と書くことができます。ここで、$y_i$ は $e_1, e_2, \ldots, e_h$ の線形結合で、$z_i$ は $e_{h+1}, \ldots, e_n$ の線形結合です。 (30) までに、すべての $i > h$ に対して $x_1 \wedge x_2 \wedge \cdots \wedge x_n \wedge y_i = 0$、したがって

$$
x_1 \wedge x_2 \wedge \cdots \wedge x_n = (\det Y)e_1 \wedge e_2 \wedge \cdots \wedge e_h \wedge z_{h+1} \wedge \cdots \wedge z_n.
$$

でも定義までに

$$
z_{h+1} \wedge z_{h+2} \wedge \cdots \wedge z_n = (\det Z)e_{h+1} \wedge e_{h+2} \wedge \cdots \wedge e_n
$$

よって公式 (30)。

$p$ の帰納法により、$X$ が行列の上三角行列の形に属する場合、次のことがわかります。

$$
X = \begin{pmatrix}
X_{11} & X_{12} & \cdots & X_{1p} \\
0 & X_{22} & \cdots & X_{2p} \\
\cdots & \cdots & \cdots & \cdots \\
0 & 0 & \cdots & X_{pp}
\end{pmatrix}
$$

(31) $$
\det X = (\det X_{11})(\det X_{22}) \ldots (\det X_{pp}).
$$

これは、特に三角形行列 (すべての $X_{ii}$ が位数 1 である)、さらに具体的には対角行列に適用できます。

(32) $$
\det(\operatorname{diag}(\alpha_1, \alpha_2, \ldots, \alpha_n)) = \alpha_1 \alpha_2 \ldots \alpha_n.
$$

(3) $M, M'$ を、それぞれ $M$ の次元 $n, n'$、$u$ 自己準同型、および $M'$ の $u'$ 自己準同型の 2 つの空き $A$ モジュールとします。それから

(33) $$
\det(u \otimes u') = (\det u)^{n'} (\det u')^n.
$$

なぜなら、$u \otimes u' = (u \otimes 1_{M'}) \circ (1_M \otimes u')$ と書くと、2 つの自己準同型 $u, u'$ のうちの 1 つが同一性である場合に導かれるからです。 For example if $u' = 1_{M'}$ and $X$ is the matrix of $u$ with respect to a basis $(e_i)$ of $M$, then the matrix of $u \otimes 1_{M'}$ with respect to the tensor product of $(e_i)$ and a basis of $M'$ can be written as a matrix (with $n'$ rows and $n'$ columns) of matrices with $n$ rows and $n$ columns

$$
\begin{pmatrix}
X & 0 & \ldots & 0 \\
0 & X & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & X
\end{pmatrix}
$$

よって、*例 2* のおかげで、

$$
\det(u \otimes 1_{M'}) = (\det X)^{n'} = (\det u)^{n'}
$$

これにより、すぐに公式 (33) が得られます。

### 7. 一次方程式への応用

(*可換*) 環 $A$ (II, § 2, no. 8) 上の $n$ 未知数における $n$ スカラー線形方程式の系を考えてみましょう。

(34) $$
\sum_{j=1}^n \lambda_{ij} x_j = \eta_i \quad (1 \leq i \leq n).
$$

$L$ を位数 $n$ の平方行列 $(\lambda_{ij})$ とします。いつものように行列を $\xi_i$ の 1 つ列からなる (それぞれ $\eta_i$) と $\mathbf{A}^n$ の元 $x = (\xi_i)$ (それぞれ $\mathbf{A}^n$ の元 $y = (\eta_i)$) と識別することで、 系 (34) (II, § 10, no. 3、命題 2) と書かれることもあります

(35)
$$
L.x = y.
$$

$u$ を $\mathbf{A}^n$ の自己準同型 $x \mapsto L.x$ とし、標準基底に対して $L$ を行列とします。式 (35) にすべての $y \in \mathbf{A}^n$ に対して (少なくとも) 1 つの解があるということは、$u$ が全射であることを意味します。 定理 no. 2 の 1 は、次の命題を意味します。

#### 命題 13 {#alg-iii-s8-prop-13 .statement tag=064Q}

*$n$ 可換環上の未知数における $n$ 線形方程式の系が、右辺に関係なく少なくとも 1 つの解を許容するには、系の行列の行列式が可逆であることが必要かつ十分です。この場合、系は 1 つの解を許可します。*

If $\det L$ is not a divisor of zero in $\mathbf{A}$, equation (34) is equivalent to the equation
$$
(\det L)L.x = (\det L)y.
$$
If $M$ is the cofactor matrix of $L$, we derive from (34) and formula (26) of no. 6 the relation
(36)
$$
(\det L)x = {}^tM.y
$$
which may also be written
(37)
$$
(\det L)\xi_i = \sum_{j=1}^n (-1)^{i+j}(\det L^{ij})\eta_j = \det L_i \quad (1 \leq i \leq n)
$$
where $L_i$ denotes the matrix obtained by replacing the column of $L$ of index $i$ by $y$. 式 (37) は、系 (34) の *Cramer の公式 * と呼ばれます。 (34) のすべての解は (37) の解でもあります。 逆に、no. 6 の公式 (28) を考慮して (36) から導き出します。
(38)
$$
(\det L)(L.x - y) = 0
$$
したがって、$\det L$ が $\mathbf{A}$ の零の因子ではない場合、系 (34) と (37) は *同等* です。 $\det L$ が可逆である場合、(34) の一意の解は次の式で与えられます。
(39)
$$
\xi_i = (\det L)^{-1}(\det L_i) \quad (1 \leq i \leq n).
$$
$\det L$ が可逆であるような系 (34) は *Cramer 系* とも呼ばれます。

特に $y = 0$ とします。次に、no. 2 の命題 3 から次のことがわかります。

#### 命題 14 {#alg-iii-s8-prop-14 .statement tag=064R}

*$n$ 可換環上の未知数における $n$ 方程式の同次線形系が非ゼロ解を許容するには、その行列の行列式が零の因子であることが必要かつ十分です。

### 8. 可換体の場合

上記はすべて、環 $\mathbf{A}$ が可換体の場合に適用されます。ただし、単純化と追加の結果があります。

したがって、この場合、§ 7, no. 9 の命題 12 は次のように定式化できます。

#### 命題 15 {#alg-iii-s8-prop-15 .statement tag=064S}

$\mathbf{E}$ を可換体よりもベクトル空間にします。 $p$ ベクトル $x_i \in \mathbf{E}$ ($1 \leq i \leq p$) が線形独立であるためには、$x_1 \wedge x_2 \wedge \cdots \wedge x_p \neq 0$ が必要かつ十分です。

#### 系 {#alg-iii-s8-n8-cor-1 .statement tag=064T}

$X$ を可換体上の型 $(m, n)$ の行列とします。 The rank of $X$ is equal to the greatest integer $p$ such that there exists at least one minor of $X$ of order $p$ which is $\neq 0$.

$X$の階数は、$X$(II, § 10, no. 12、定義7)の線形独立列の最大値数です。 系は、no. 5 の命題 15 と公式 (17) から続きます。

ここで、可換体 $\mathbf{K}$ 上の $n$ 未知数における $m$ 線形方程式の系の場合を考えてみましょう。

$$
\sum_{j=1}^n \lambda_{ij} \xi_j = \eta_i \quad (1 \leq i \leq m).
$$

(41)

#### 命題 16 {#alg-iii-s8-prop-16 .statement tag=064U}

$L = (\lambda_{ij})$ を系 (41) の行列 (型 $(m, n)$ のうち) とします。 $M$を、$L$に$(n+1)$番目の列$(\eta_i)$(II, § 10, no. 1)を加えて得られる型$(m, n+1)$の行列とします。 $p$ を $L$ の階数とします (適用系から命題 15 で計算)。行を抑制することにより、$L$ のマイナー $\Delta$、行列の行列式、および $L$ の添字 $\geq p + 1$ の列が $\neq 0$ であるとします (これは、適切な手段によって常に可能です) $L$ の行には置換、$L$ の列には適切な置換)。次に、系 (41) が少なくとも 1 つの解を持つためには、位数 $p + 1$ の $M$ の部分行列の位数 $p + 1$ の $M$、行列式のすべてのマイナーが必要かつ十分です。 列には添字 $1, 2, \ldots, p$ と $n+1$ があり、零になります。そうであれば、系 (41) の解は、最初の $p$ 方程式の系からなるのものになります。書かれていれば

$$
\sum_{j=1}^p \lambda_{ij} \xi_j = \eta_i - \sum_{k=p+1}^n \lambda_{ik} \xi_k \quad (1 \leq i \leq p)
$$

この系のすべての解は、 添字 $k > p$ の $\xi_k$ 、任意の値および適用を計算するまでのクラマーの公式 (no. 7、公式 (37)) から取得することで得られます。 添字 $j \leq p$ の $\xi_j$。

私たちは (II, § 10, no. 12, 命題 12) 、系 (41) が少なくとも 1 つの解を持つには、行列 $L$ と $M$ が同じ階数を持つことが必要かつ十分であることを知っています。 $L$ の行と列を主張の満たす条件に並べ替えて、$a_i$ ($1 \leq i \leq p$) が $L$ の最初の $p$ 列を表すとします。 $y = (\eta_i)$ $M$ の $(n+1)$ 番目の列。 $L$ のすべての列は $a_i$ の仮定線形結合によるものであるため、$M$ が $L$ と同じ階数 $p$ を持つということは、$y$ が$a_i$ の線形結合、または (命題 15) の $a_1 \wedge \cdots \wedge a_p \wedge y = 0$。 主張の可能性条件は、no. 5 の公式 (17) を考慮した、後者の関係の翻訳です。さらに、$M$ の最初の $p$ 行は線形独立であるため、添字 $> p$ の行はそれらの線形結合であり、したがって (42) のすべての解は (41) の解でもあります。 最後の主張は、命題の 13 の no. 7 の明らか帰結になります。

### 9. ユニモジュラー 群 $\mathbf{SL}(n, A)$

$\mathbf{M}_n(A)$ が $A$ 上の位数 $n$ の正方行列の環を表すとします。 写像 $\det : \mathbf{M}_n(A) \to A$ を考えてみましょう。 The group $\mathbf{GL}(n, A)$ of invertible elements of $\mathbf{M}_n(A)$ (isomorphic to the group of automorphisms of the $A$-module $A^n$ (II, § 10, no. 7)) is just the inverse image under this mapping of the multiplicative group $A^*$ of invertible elements of $A$ (no. 3, Proposition 5). 一方、注意は、写像 $\det : \mathbf{GL}(n, A) \to A^*$ は群準同型 (no. 3、命題 5) です。

さらに、写像 $\det : \mathbf{M}_n(A) \to A$ は*全射*です(したがって、準同型 $\det : \mathbf{GL}(n, A) \to A^*$も同様です)。以来、$\lambda \in A$全員にとって、

$$
\det(\operatorname{diag}(\lambda, 1, \ldots, 1)) = \lambda
$$

no. 6 の公式 (32) のおかげで。

全射準同型 $\det : \mathbf{GL}(n, A) \to A^*$ の *核* は、*ユニモジュラー* 行列で構成される $\mathbf{GL}(n, A)$ の通常の部分群です。それは $\mathbf{SL}_n(A)$ または $\mathbf{SL}(n, A)$ で表され、*ユニモジュラー 群* または正方行列の位数 $n$ $A$ の *特別な線形群* と呼ばれることがよくあります。

このNo. $A$ が *体* である場合を調べます。 $1 \leq i \leq n, 1 \leq j \leq n$ の場合、$E_{ij}$ は位数 $n$ の平方行列を表し、その元は、添字 $i$ と列の行を除くすべて零であることを思い出してください。 添字 $j$、これは 1 に等しい。 $I_n$ が位数 $n$ の単位元行列を表す場合、 *個別* 添字 $i, j$ のすべての注文された対とすべての $\lambda \in A$ (II, § 10, no. 13) に対して $B_{ij}(\lambda) = I_n + \lambda E_{ij}$ を書き込みます。

#### 命題 17 {#alg-iii-s8-prop-17 .statement tag=064V}

※$K$を可換体とします。ユニモジュラー 群 $\mathbf{SL}(n, K)$ は、行列 $B_{ij}(\lambda)$ と $i \neq j$ および $\lambda \in K$* によって生成されます。

II, § 10, no. 13、命題 14 までに、$\mathbf{GL}(n, K)$ のすべての行列は、形 $B_{ij}(\lambda)$ の行列の積と、形 $\operatorname{diag}(1, 1, \ldots, 1, \alpha)$ の $\alpha \in K^*$ の行列であることがわかります。 これで、$\det(B_{ij}(\lambda)) = 1$ と $\det(\operatorname{diag}(1, \ldots, 1, \alpha)) = \alpha$ (no. 6, *例 2*) が明らかになります。 よって命題。

#### 系 {#alg-iii-s8-n9-cor-1 .statement tag=064W}

*群* $\mathbf{SL}(n, K)$ * は $\mathbf{GL}(n, K)$ の交換子の群です。 *ただし、* $n = 2$ * および * $K$ * が 2 元* の体である場合を除きます。

$\mathbf{SL}(n, K)$ は、$\mathbf{GL}(n, K)$ の準同型の核から、可換群 $K^*$ への、$\mathbf{SL}(n, K)$ 含む交換子群 $\Gamma$ の $\mathbf{GL}(n, K)$ (I, § 6, no. 2)。 $\mathbf{SL}(n, K) = \Gamma$ を証明するには、$\lambda \in K^*$、$B_{ij}(\lambda)$ 属する ～ $\Gamma$ のすべてについて、命題 17 までに証明すれば十分です。さて、$B_{ij}(\lambda)$は$B_{ij}(\lambda) = Q . B_{ij}(1) . Q^{-1}$以降の$\mathbf{GL}(n, K)$の$B_{ij}(1)$の共役であり、$Q$は自己同型の$v$の標準基底$(e_i)$に関して行列を表します。 $K^n$ は、$k \neq i$ に対して $v(e_i) = \lambda e_i, v(e_k) = e_k$ になります。一方、$u_{ij}$ ($i \neq j$ の場合) を $K^n$ の自己同型とし、$k \notin \{i, j\}$ を$u_{ij}(e_i) = -e_j, \ u_{ij}(e_j) = e_i, \ u_{ij}(e_k) = e_k$ とし、属するから $\mathbf{SL}(n, K)$ とします。次に $B_{ji}(\lambda) = U_{ij} B_{ij}(-\lambda) U_{ij}^{-1}$、ここで $U_{ij}$ は標準基底に対する $u_{ij}$ の行列です。同様に、$1 < i < j$ の場合は $B_{1j}(\lambda) = U_{1i} B_{ij}(\lambda) U_{1i}^{-1}$、最後に $2 < j$ の場合は $B_{12}(\lambda) = U_{2j} B_{1j}(\lambda) U_{2j}^{-1}$ となります。これは、すべての $B_{ij}(\lambda)$ が $\mathbf{GL}(n, K)/\Gamma$ に同じ像 $s$ を持っていることを証明し、$s$ が単位元であることを示します。

まず、$K$ 含む元 $\lambda$ が 0 と 1 とは異なると仮定します。次に $1 = \lambda + (1 - \lambda)$、右側の 2 つの項は $\neq 0$ です。 関係 $B_{12}(1) = B_{12}(\lambda) B_{12}(1 - \lambda)$ は、$s^2 = s$ であるため、$s$ は単位元であることを示します。

今、$n \geq 3$ だとしましょう。 積 $B_{21}(1) B_{31}(1)$ は、自己同型の行列 $K^n$ の $u$ であり、$i \neq 1$ に対して $u(e_1) = e_1 + e_2 + e_3, u(e_i) = e_i$ になります。 $S$ が自己同型の行列 $u'$ $K^n$ で、$i \neq 2$ が $u'(e_2) = e_2 + e_3, u'(e_i) = e_i$ である場合、$S . B_{21}(1) B_{31}(1) . S^{-1} = B_{21}(1)$;また、$s^2 = s$ も推定され、証明が完成します。

#### 注意 {#alg-iii-s8-n9-rem-1 .statement tag=064X}

(1) $\mathbf{GL}(2, \mathbf{F}_2) = \mathbf{SL}(2, \mathbf{F}_2)$;これは、位数 6 の解ける群であり、その交換子群は添字 2 (II, § 10、練習問題 14) です。

(2) 上記と同じ記法を用いて、I, § 5, no. 7, 命題 9 のように、$i < j, j - i > 1$ に対して$u_{ij} = u_{j-1, j} u_i, _{j-1} u_{j-1, j}^{-1}$ が成り立つことが証明できます。したがって、*群* $\mathbf{SL}(n, K)$ *は行列* $B_{12}(\lambda)$ *および* $U_{i, i+1}$ *$1 \leq i \leq n - 1$ によって生成されます。

### 10. $\mathbf{A}[X]$ モジュールは $\mathbf{A}$ モジュール自己準同型に関連付けられています

$M$ を $\mathbf{A}$ モジュール、$u$ 自己準同型を $M$ とします。 $\mathbf{A}$ 上の 1 つの不確定な $X$ で多項式環 $\mathbf{A}[X]$ を考えてみましょう。すべての多項式 $p \in \mathbf{A}[X]$ とすべての $x \in M$ について、次のように書きます。

$$
p . x = p(u)(x).
$$

$\mathbf{A}[X]$ の 2 つの多項式 $p, q$ に対して $(pq)(u) = p(y) \circ q(u)$ として、$\mathbf{A}[X]$ モジュール構造は$M$ で定義されます。 集合 $M$ は、この構造と合わせて $M_u$ で表されます。 $M$ で与えられる $\mathbf{A}$ モジュール構造は、$M_u$ から $\mathbf{A}$ までの演算子の環を制限することによって得られます。 $M_u$ の部分加群は、$u$ では *安定* である $M$ の部分加群であることに注意してください。

$A[X] \times M$ の $M$ への写像 $(p, x) \mapsto p.x$ は $A$ 双線形であるため、定義するは正準的に $A$ 線形写像 $\phi : A[X] \otimes_A M \to M$ となります。
$$
\phi(p \otimes x) = p.x = p(u)(x).
$$
一方、$A[X] \otimes_A M$ は標準的に $A[X]$ モジュール構造 (II, § 5, no. 1) を持ちます。この $A[X]$ モジュールを $M[X]$ で表すことにします。 写像 $\phi : M[X] \to M_u$ は $A[X]$ 線形です。なぜなら、$A[X]$ と $x \in M$ の $p, q$ については、
$$
\phi(q(p \otimes x)) = \phi((qp) \otimes x) = (qp).x = q(u)(p(u)(x)) = q.\phi(p \otimes x).
$$
さらに、$u$ は $M_u$ の $A[X]$ 準同型写像です。
$$
u(p.x) = u(p(u)(x)) = (up(x))(x) = p.u(x).
$$
最後に、$M[X]$ の $A[X]$ 準同型性 $\bar{u}$ は、 (II, § 5, no. 1) と書くことによって定義されます。
$$
\bar{u}(p \otimes x) = p \otimes u(x).
$$
さらに、式 (44) と (45) から、$A[X]$ 線形写像 $u, \bar{u}$ と $\phi$ は関係によって関連付けられることがわかります。
$$
\phi \circ \bar{u} = u \circ \phi.
$$
$\psi$ が $M[X]$ の $A[X]$ 準同型性 $X - \bar{u}$ を表すとすると、$\psi(p \otimes x) = (Xp) \otimes x - p \otimes u(x)$ になります。次の命題があります:

#### 命題 18 {#alg-iii-s8-prop-18 .statement tag=064Y}

*$A[X]$準同型写像中数列*
$$
M[X] \xrightarrow{\psi} M[X] \xrightarrow{\phi} M_u \longrightarrow 0
$$
正確です。

すべての $x \in M$ に対して $\phi(1 \otimes x) = x$ であるため、明らかに $\phi$ は全射的です。一方、
$$
\phi(X(p \otimes x)) = X.\phi(p \otimes x) = u(\phi(p \otimes x)),
$$
他の語、$\phi \circ X = u \circ \phi = \phi \circ \bar{u}$では(46)。これは $\phi \circ \psi = 0$ であることを証明します。 $\operatorname{Ker} \phi \subset \operatorname{Im} \psi$ を検証する必要があります。この注意点として、$A$ モジュール $A[X]$ の単項式 $X^k$ ($k \geq 0$) 形基底なので、すべての元 $z \in M[X]$ は形 $z = \sum_k X^k \otimes x_k$ で一意に書くことができます。 $(x_k)$ は、$M$、有限台の元の家族です。 $z \in \operatorname{Ker} \phi$ の場合、$\phi(z) = \sum_k u^k(x_k) = 0$ と書くことができます。
$$
z = \sum_k (X^k \otimes x_k - 1 \otimes u^k(x_k)) = \sum_k (X^k - \bar{u}^k)(1 \otimes x_k).
$$
しかし、$M[X]$ の $A[X]$ 準同型性 $X$ と $\bar{u}$ は置換可能であるため、

$$
X^k - \bar{u}^k = (X - \bar{u}) \circ \left( \sum_{j=0}^{k-1} X^j \bar{u}^{k-j-1} \right)
$$

これは、$z = \psi(y)$ となるような $y \in M[X]$ が存在することを証明します。

ここで、$M'$ を他の $A$-モジュール、および $M'$ の $u'$ 自己準同型とします。 $M'_{u'}$、$\phi'$、$\bar{u}'$、$\psi'$を$M'$と$u'$から$M_u$、$\phi$、$\bar{u}$、$\psi$として求めた加群と写像とします。は$M$と$u$から得られます。次に:

#### 命題 19 {#alg-iii-s8-prop-19 .statement tag=064Z}

*M から M' への写像 g が M_u から M'_u への A[X] 準同型であるためには、g が $g \circ u = u' \circ g$ となるような M から M' への A 準同型であることが必要かつ十分です。この場合、$\bar{g}$ が M[X] から M'[X] への A[X] 準同型写像であり、$1_{A[x]} \otimes g$ (II, § 5, no. 1) に等しい場合、図式*

$$
\begin{array}{cccccc}
M[X] & \xrightarrow{\psi} & M[X] & \xrightarrow{\phi} & M_u & \longrightarrow 0 \\
\downarrow \bar{g} & & \downarrow \bar{g} & & \downarrow g & \\
M'[X] & \xrightarrow{\psi'} & M'[X] & \xrightarrow{\phi'} & M'_{u'} & \longrightarrow 0
\end{array}
$$

は*可換*です。

$g$ が A[X] 準同型であるためには、(43) により条件 $g \circ u = u' \circ g$ が明らかに必要です。 帰納法によって、整数 $n > 0$ ごとに $g \circ u^n = {u'}^n \circ g$ になることが暗示されるため、これで十分です。一方、すべての$x \in M$とすべての$p \in A[X]$については、

$$
\phi'(\bar{g}(p \otimes x)) = \phi'(p \otimes g(x)) = p(u')(g(x)) = g(p(u)(x)) = g(\phi(p \otimes x))
$$
そして
$$
\bar{u}'(g(p \otimes x)) = \bar{u}'(p \otimes g(x)) = p \otimes u'(g(x)) = p \otimes g(u(x)) = \bar{g}(\bar{u}(p \otimes x))
$$
これは、図式の可換性を証明します (48)。

### 11. 自己準同型の特性多項式

$M$ を、$M$ の次元 $n$ および $u$ 自己準同型の自由な $A$ モジュールとします。 2 つの不定変数 $A[X, Y]$ と $A[X, Y]$ モジュール $M[X, Y] = A[X, Y] \otimes_A M$ の多項式環を考えてみましょう。 $\bar{u}$ を、$u$ (II, § 5, no. 1) から正規に導出された $A[X, Y]$ モジュール $M[X, Y]$ の自己準同型とします。 no. 5、命題 11 から次のことがわかります。

$$
\det(X - Y \bar{u}) = \sum_{j=0}^n (-1)^j \mathrm{Tr}(\wedge^j(u)) X^{n-j} Y^j
$$

なぜなら、$U$ が $M$ の基底 $(e_i)_{1 \leq i \leq n}$ に対して $u$ の行列である場合、$U$ は、基底 $(1 \otimes e_i)_{1 \leq i \leq n}$ に対して$\bar{u}$ の行列であるからです。 $M[X, Y]$、したがって

$$
\mathrm{Tr}(\wedge^j(\bar{u})) = \mathrm{Tr}(\wedge^j(u)).
$$

#### 定義 3 {#alg-iii-s8-def-3 .statement tag=0650}

$M$ を有限次元の自由 $A$ 加群、および $M$ の $u$ 自己準同型とします。無料の$A[X]$モジュール$M[X]$の自己準同型$X - \bar{u}$の行列式は、$u$の特性多項式と呼ばれ、$\chi_u(X)$で表されます。

$M$ が階数 $n$ である場合、(49) から次のようになります。

$$
\chi_u(X) = \sum_{j=0}^n (-1)^j \operatorname{Tr}(\wedge^j(u)) X^{n-j}
$$

$\det(X - Y \bar{u}) = \det(X . I_n + Y U)$と$\det(X - \bar{u}) = \det(X . I_n - U)$の場合。したがって、$\chi_u(X)$ は、$X^{n-1}$ の係数が $-\operatorname{Tr}(u)$ で、定数項が $(-1)^n \det(u)$ である、次数 $n$ のモニック多項式であることがわかります。

#### 命題 20 (「ケイリー – ハミルトン定理」) {#alg-iii-s8-prop-20 .statement tag=0651}

有限次元の自由 $A$ 加群の各自己準同型 $u$ に対して、$\chi_u(u) = 0$。

命題 18 の記法 ($§ 3$、no. 10) では、すべての $x \in M$ に対して、$\chi_u(u)(x)$ は $\chi_u(X) \otimes x$ の $\phi$ の下にある像です。しかし、$v$ が $M[X]$ の自己準同型、つまり $X - \bar{u}$ (no. 6) の共転置である場合、

$$
\chi_u(X) \otimes x = \chi_u(X)(1 \otimes x) = (X - \bar{u})(v(1 \otimes x))
$$

そして結論はno. 10の命題18から続きます。

### 練習問題 {#alg-iii-s8-exercises}

[§ 8 に対して練習問題](exercises/s8/)を参照してください。
