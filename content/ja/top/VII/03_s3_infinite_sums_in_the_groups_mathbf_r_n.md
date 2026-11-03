---
book: top
book_title: General Topology
chapter: VII
chapter_title: The additive groups $\mathbf{R}^n$
section: 3
section_title: Infinite sums in the groups $\mathbf{R}^n$
lang: ja
source: top-v-x
pdf_pages: 0089-0092, 0101-0102
extraction: ocr
subsections:
    - "no": 1
      title: SUMMABLE FAMILIES IN $\mathbf{R}^n$
      page: 0
      pdf_page: 89
    - "no": 2
      title: SERIES IN $\mathbf{R}^n$
      page: 0
      pdf_page: 92
statements: 9
exercises: 2
content_sha256: e08522358fe6ae3579cced4f0f13a949a09becbaf885a3c223d082e9efc06510
translated_from: content/en/top/VII/03_s3_infinite_sums_in_the_groups_mathbf_r_n.md
translation_method: google
source_content_sha256: 469c822cd0058ba2bb0510721ee43c3d335b871a5db27467e63bfe955b6c2715
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 8f5866fca8b3ac47f58bf58f532cda52e5db69da60827c0d3661e2dd21fc53a5
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 3. 無限和群 $\mathbf{R}^n$

### 1. $\mathbf{R}^n$ のサマブルファミリー

$\mathbf{R}^n$ のすべての点には近傍の *可算* 基本系があるため、加法群 $\mathbf{R}^n$ の点の族 $(x_t)$ は、添字の集合の場合にのみ合計可能です。 $X_t \neq 0$ が *可算* であるような $t$ (章 III, § 5, no. 2, 系から命題 1)。したがって、本質的に、$\mathbf{R}^n$ での要約可能なファミリーの研究は、要約可能な数列の研究に縮小されます。それにも関わらず、章 IV, で与えられたのと同じ理由により、$\mathbf{R}$ の加算可能なファミリーに関連して、以下の制限を添字集合の基数に課すことはありません。

#### 命題 1 {#top-vii-s3-prop-1 .statement tag=0BZK}

*family* $(x_i)_{i \in I}$ *of 点* $x_i = (x_{i,k})_{1 \leq k \leq n}$ *of* $\mathbf{R}^n$ *それぞれ* $n$ *ファミリー* $(x_{i,k})_{i \in I}$ *of 実数が* $\mathbf{R}$ で合計可能である場合にのみ、合計可能です。

これは、章 III, § 5, no. 4、命題 4 から続きます。

命題 1 の条件は次のように変形できます。

#### 定理 1 {#top-vii-s3-thm-1 .statement tag=0BZL}

*家族* $(x_i)_{i \in I}$ *of 点 of* $\mathbf{R}^n$ *家族* $(||x_i||)$ *of ユークリッドノルムの* $x_i$ *が $\mathbf{R}$ で合計可能である場合に限り、合計可能です。

これは、実数 (章 IV, § 7, no. 2, 定理 3) の族の合計可能性について、命題 1、条件から問題なく続きます。

$$
\sup_{1 \leq k \leq n} |x_{i,k}| \leq ||x_i|| \leq \sum_{i=1}^n |x_{i,i}|,
$$

と比較原理 (章 IV, § 7, no. 1, 定理 2)。

最初に次の命題を確立することで、多少異なる方法で進めることもできます。

#### 命題 2 {#top-vii-s3-prop-2 .statement tag=0BZM}

*もし* $(x_i)_{i \in I}$ *が* $\mathbf{R}^n$の点の有限族である場合、*その後*

$$
\sum_{i \in I} ||x_i|| \leq 2n \cdot \sup_{J \subset I} \left| \sum_{i \in J} x_i \right|.
$$

$x_i = (x_{ij})_{1 \leq j \leq n}$ の場合、$||x_i|| \leq \sum_{j=1}^n |x_{ij}|$ があるため、

$$
\sum_{i \in I} ||x_i|| \leq \sum_{j=1}^n \left( \sum_{i \in I} |x_{ij}| \right).
$$

現在$\sum_{i \in I} |x_{ij}| = \sum_{i \in I} x_{ij}^+ + \sum_{i \in I} x_{ij}^-$、以降、$I$の部分集合$J$ごとに、

$$
-\sum_{i \in I} x_{ij}^- \leq -\sum_{i \in J} x_{ij}^- \leq \sum_{i \in J} x_{ij}^+ \leq \sum_{i \in I} x_{ij}^+
$$

それは次のとおりです

$$
\sum_{i \in I} |x_{ij}| \leq 2 \cdot \sup_{J \subset I} \left| \sum_{i \in J} x_{ij} \right|.
$$

しかし、$\left| \sum_{i \in J} x_{ij} \right| \leq \left| \sum_{i \in J} x_{ij} \right|$ であるため、不等式 (1) になります。

ここで、定理 1 は次の命題と等価です ($\mathbf{R}^n$ は完全な群であるため): ファミリー $(x_i)$ は、次の場合に限り、コーシーの基準 (章 III, § 5, no. 2, 定理 1) を満たします。家族 $(||x_i||)$ もコーシーの基準を満たします。ここで、三角形不等式は、この条件で十分であることを示し、不等式(1)は、それが必要であることを示しています。

さらに不等式もあります

$$
\left| \sum_i x_i \right| \leq \sum_i ||x_i||
$$

これは、有限部分和の類似の不等式から移行から極限になります。

#### 系 {#top-vii-s3-n1-cor-1 .statement tag=0BZN}

*ファミリー* $(x_i)$ *of 点 of* $\mathbf{R}^n$ *ファミリーの有限部分和の集合が * $\mathbf{R}^n$ で囲まれる場合に限り、合計可能です。

定理 1 と三角形不等式により、この条件が必要になります。 不等式 (1) と定理 1 で十分です。

#### 命題 3 {#top-vii-s3-prop-3 .statement tag=0BZO}

*$(x_\lambda)_{\lambda \in L}$ * を * $\mathbf{R}^m$ の点の加算可能な族とし、$(y_\mu)_{\mu \in M}$ * $\mathbf{R}^n$ の点の加算可能な族とする*、そして * $f$ * の双線形写像とする* $\mathbf{R}^m \times \mathbf{R}^n$ *に* $\mathbf{R}^p$。 *その後、家族* $(f(x_\lambda, y_\mu))_{(\lambda, \mu) \in L \times M}$ *合計可能で、次のようになります*

$$
\sum_{(\lambda, \mu) \in L \times M} f(x_\lambda, y_\mu) = f \left( \sum_{\lambda \in \mu} x_\lambda, \sum_{\mu \in M} y_\mu \right).
$$

族 $(f(x_\lambda, y_\mu))$ が加算可能であることを示すには、$\mathbf{R}^n$ の点 $f(x_\lambda, y_\mu)$ の座標によって形成される $p$ 族のそれぞれが加算可能であることを命題 1 によって確立するだけで十分です。他の語では、次の場合に限定できます。 $f$ は双線形 *形* です。しかし、そのような形 $f$ については、

$$
f(x, y) = \sum_{i, j} a_{ij} x_i y_j,
$$

したがって、ケース $f(x, y) = x_i y_j$ に戻ります。このケースでは、結果はすでに証明されています (章 IV, § 7, no. 3, 命題 1)。

写像 $f$ を特殊化すると、特に次の結果が得られます。

#### 系 1 {#top-vii-s3-prop-3-cor-1 .statement tag=0BZP}

** $(a_\lambda)_{\lambda \in L}$ * が実数の加算可能な族であり、* $(x_\mu)_{\mu \in M}$ * が* $\mathbf{R}^n$ の点の加算可能な族である場合、 *その場合、族* $(a_\lambda x_\mu)_{(\lambda, \mu) \in L \times M}$ * は加算可能であり、次のようになります*

$$
\sum_{(\lambda, \mu) \in L \times M} a_\lambda x_\mu = \left( \sum_{\lambda \in L} a_\lambda \right) \left( \sum_{\mu \in M} x_\mu \right).
$$

#### 系 2 {#top-vii-s3-prop-3-cor-2 .statement tag=0BZQ}

*もし* $(x_\lambda)_{\lambda \in L}$ *と* $(y_\mu)_{\mu \in M}$ *が* $\mathbf{R}^n$の点の2つの加算可能な族である場合、*その族* $(x_\lambda | y_\mu)$ *(cf. 章 VI, § 2, no. 2)* *は* $\mathbf{R}$で加算可能であり、*そして次のようになります*

$$
\sum_{(\lambda, \mu) \in L \times M} (x_\lambda | y_\mu) = \left( \sum_{\lambda \in L} x_\lambda \middle| \sum_{\mu \in M} y_\mu \right).
$$

### 2. 系列 $\mathbf{R}^n$

一般的な項が $x_m = (x_{mi})_{1 \leq i \leq n}$ である系列は、$n$ 系列 $(x_{mi})_{m \in \mathbf{N}}$ のそれぞれが $\mathbf{R}$ に収束する場合に限り、$\mathbf{R}^n$ に収束します。

#### 定義 1 {#top-vii-s3-def-1 .statement tag=0BZR}

* $\mathbf{R}^n$ の点の系列 * ユークリッドのノルムの項の系列が収束する場合、絶対収束するといいます。

#### 命題 4 {#top-vii-s3-prop-4 .statement tag=0BZS}

*系列 of 点 of* $\mathbf{R}^n$ *絶対的に収束する場合に限り、可換収束します。*

上記の章 III, § 5, no. 7 と定理 1 の命題 9 の帰結です。

章 IV, § 7 で与えられた例は、$\mathbf{R}^n$ の系列が *絶対収束* ではなく *収束* する可能性があることを示しています。

### 練習問題 {#top-vii-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
