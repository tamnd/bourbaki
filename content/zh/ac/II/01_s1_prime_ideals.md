---
book: ac
book_title: Commutative Algebra
chapter: II
chapter_title: LOCALIZATION
section: 1
section_title: Prime ideals
lang: zh
source: ac-i-vii
book_pages: 51-55, 121-123
pdf_pages: 0071-0075, 0141-0143
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF PRIME IDEALS
      page: 51
      pdf_page: 71
    - "no": 2
      title: RELATIVELY PRIME IDEALS
      page: 53
      pdf_page: 73
statements: 9
exercises: 11
content_sha256: 073f55ca472d68cec3af3765faa5a12d42263fbbb8df8b539da3985b7513b8be
translated_from: content/en/ac/II/01_s1_prime_ideals.md
translation_method: google
source_content_sha256: 556d7efab2e0c3d357dfbbd27923b000a4c0af8dc523529bed393394168a1056
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 1e14dd89f1564f36c4034ff4b327c085de2eae1bf7a9d9eadb761b831238efaf
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 1. 素理想

### 1. 定义素理想

#### 定义 1 {#ac-ii-s1-def-1 .statement tag=0450}

如果环 $A/p$ 是整环，则环 $A$ 的理想 $p$ 称为素数。

通过这个定义，如果以下两个条件成立，则环$A$的理想$p$是素数：
(1) $p \neq A$；
(2) 如果$x, y$是$A$的两个元素，使得$x \notin p$和$y \notin p$，则$xy \notin p$。

这些条件也可以用说表示，$\mathfrak{g}p$属于到$\mathfrak{g}p$的元素的任何有限族的乘积，因为应用这个条件到空集产生$1 \notin p$。

$A$ 的最大理想 $m$ 是素数，因为 $A/m$ 是域；那么从克鲁尔的定理 (代数, 章 I, § 8, no. 7, 定理 2) 可以得出，每个理想

(*) 除了位于两个星号之间的叙述：\* ... *，此章的结果仅取决于本书的I至VI和章I, §§ 1–3。

至少一个素理想中包含*不同于*$\mathbf{A}$。特别是，对于环$\mathbf{A}$中存在素理想，$\mathbf{A}$不减少到0是充分必要的。

令$f : \mathbf{A} \to \mathbf{B}$为环同态，且$q$为$\mathbf{B}$的理想。 集合$p = f^{-1}(q)$；通过取商从 $f$ 导出的同态 $\overline{f} : \mathbf{A}/p \to \mathbf{B}/q$ 是单射的。 Suppose that $q$ is prime; as the ring $\mathbf{B}/q$ is an integral domain, so is $\mathbf{A}/p$, being isomorphic to a subring of $\mathbf{B}/q$; consequently the ideal $p = f^{-1}(q)$ is prime. 特别地，令$\mathbf{A}$为$\mathbf{B}$的子环；对于$\mathbf{B}$的每个理想$q$，$q \cap \mathbf{A}$都是素理想$\mathbf{A}$。 如果$f$是满射，则$\overline{f}$是同构； 条件“p 是素数”和“$q$ 是素数”则等价。 因而，如果$p$和$a$是$\mathbf{A}$的理想，使得$a \subset p$，则$p$为素数的充分必要条件是$p/a$为$\mathbf{A}/a$中的素数。

#### 命题 1 {#ac-ii-s1-prop-1 .statement tag=0451}

*设$\mathbf{A}$为环，$a_1, a_2, \ldots, a_n$为$\mathbf{A}$的理想，$p$为$\mathbf{A}$的素理想。如果$p$包含乘积$a_1 a_2 \ldots a_n$，则包含至少$a_i$之一。*

事实上，假设 $p$ 包含都没有 $a_i$。对于$1 \leq i \leq n$，则存在元素$s_i \in a_i \cap p$；那么$s = s_1 s_2 \ldots s_n$包含在$a_1 a_2 \ldots a_n$中，而不包含在$p$中，这是荒谬的。

#### 推论{#ac-ii-s1-n1-cor-1 .statement tag=0452}

*设$m$为$\mathbf{A}$的极大理想；对于每个整数$n > 0$，唯一的素理想包含$m^n$是$m$。*

这样的理想$p$必须将包含$m$乘以命题1应用于$a_i = m$以获得$1 \leq i \leq n$；因为 $m$ 是最大的，$p = m$。

#### 命题 2 {#ac-ii-s1-prop-2 .statement tag=0453}

*设$\mathbf{A}$为环，$a$$\mathbf{A}$的非空集合，其在加法和乘法下闭集，以及$(p_i)_{i \in I}$$\mathbf{A}$的非空有限理想族。假设$a$包含在$p_i$的并中，并且$p_i$中最多有两个不是素数。那么$a$包含在$p_i$之一中。*

我们以归纳对$n = \mathrm{Card}(I)$争论；如果 $n = 1$ 则命题是微不足道的。假设$n \geq 2$；如果存在指标$j$使得$a \cap p_j \subset \bigcup_{i \neq j} p_i$、集合$a$（即$a \cap p_i$的并，其中$i \in I$）包含在$\bigcup_{i \neq j} p_i$中，因此包含在归纳假设的$p_i$之一中。假设这样的指标不存在；对于每个$j \in I$，让$y_j$是$a \cap p_j$的元素，而不是属于到$i \neq j$的任何$p_i$。设$k$为$I$的元素，如果$n > 2$则$p_k$为素数，如果$n = 2$则任意选择；让$z = y_k + \prod_{i \neq k} y_i$。那么$z \in a$，因为$a$在加法和乘法下是封闭的；如果$j \neq k$、$\prod_{i \neq k} y_i$属于到$p_j$，但是$y_k \notin p_j$、从而$z \notin p_j$。另一方面，$\prod_{i \neq k} y_i$ 不会属于到 $p_k$，因为因子 $y_i \ (i \neq k)$ 属于都不是它，并且如果 $n - 1 > 1$ 则 $p_k$ 是质数；因为$y_k \in p_k$、$z$不属于到$p_k$且命题成立。

### 2. 相对基本的理想

设$A$为环；如果 $a + b = A$，则 $A$ 的两个理想 $a, b$ 被称为*相对素数*。为此，$a + b$ 不包含在任何素理想中 (*代数*, 章 I, § 8, no. 7, 定理 2)，在其他字中，$a$ 和 $b$ 中都不包含素理想包含，这是必要且充分的。两个不同的最大理想互质。

如果 $A$ 是 *主理想整环* (*代数*, 章 VII, § 1)，则 $A$ 的两个元素 $a, b$互质，根据 Bezout 恒等式 (*loc.cit.*, no. 2, 定理 1)，理想$Aa$和$Ab$互质。

#### 命题 3 {#ac-ii-s1-prop-3 .statement tag=0454}

*设$a$和$b$为环$A$的两个相对素理想。令$a'$和$b'$为$A$的两个理想，使得$a$（或$b$）的每个元素在$a'$（或$b'$）中都有幂。那么 $a'$ 和 $b'$ 互质。*

在给定的假设下，每个素理想包含$a'$包含$a$和每个素理想包含$b'$包含$b$。如果一个素理想包含$a'$和$b'$，那么它就是包含$a$和$b$，这是荒谬的，因为$a$和$b$是相对素数；因此 $a'$ 和 $b'$ 互质。

#### 命题 4 {#ac-ii-s1-prop-4 .statement tag=0455}

*令$a, b_1, \ldots, b_n$为环$A$的理想。如果 $a$ 与每个 $b_i$ ($1 \leq i \leq n$) 互质，则它与 $b_1 b_2 \ldots b_n$ 互质。

设$p$为$A$的素理想。如果$p$包含$a$和$b_1 b_2 \ldots b_n$它是包含$b_i$之一（no. 1，命题1），这是荒谬的，因为$a$和$b_i$互质。

#### 命题 5 {#ac-ii-s1-prop-5 .statement tag=0456}

*令$(a_i)_{i \in I}$为环$A$的非空有限理想族。以下属性是等效的 =
(a) 对于 $i \neq j$，$a_i$ 和 $a_j$ 互质。
(b) *典范同态* $\phi : A \to \prod_{i \neq I} (A/a_i)$ (*代数*, 章 11, § 1, no. 7) 是满射。
*如果这些成立，则 $a_i$ 的交 $a$ 等于它们的乘积，并且典范同态* $\phi : A/a \to \prod_{i \in I} (A/a_i)$ (*代数*, 章 II, § 1, no. 7) 是双射的。*

我们通过归纳对$I$中元素的$n$数进行争论，$n = 1$的情况是微不足道的。首先考虑案例$n = 2$。那么 (a) 和 (b) 的等价由序列的精确性得出

$$
0 \longrightarrow A/(a_1 \cap a_2) \xrightarrow{\psi} (A/a_1) \oplus (A/a_2) \longrightarrow A/(a_1 + a_2) \longrightarrow 0
$$

（代数，章II, § 1, no. 7，公式（30））。此外，存在$e_1 \in a$和$e_2 \in a_2$使得$1 = e_1 + e_2$；那么，对于所有$x \in a = a_1 \cap a_2$，$x = xe_1 + xe_2$；但通过定义$xe_1 \in a_1 a_2$和$xe_2 \in a_1 a_2$，因此$x \in a_1 a_2$； 从而$a \subset a_1 a_2$和逆命题包含很明显。

一般情况下，假设条件(a)成立，令$k$为$I$和$b_k = \bigcap_{i \neq k} a_i$的元素； 归纳假设意味着$b_k = \prod_{i \in I} a_i$，并且从命题 4可以得出$a$和$b$互质；然后

$$
a = \bigcap_{i \in I} a_i = a, \quad \cap b_k = a_k b_k = \prod_{i \in I} a_i,
$$

由参数的第一个部分得出，并且出于同样的原因典范同态 $A/a \twoheadrightarrow (A/a_k) \times (A/b_k)$ 是双射的；由归纳假设典范同态 $A/b_k \to \prod_{i \neq k} (A/a_i)$ 是双射，因此合数同态是

$$
A/a \to (A/a_k) \times (A/b_k) \to (A/a_k) \times \prod_{i \neq k} (A/a_i) = \prod_{i \in I} (A/a_i)
$$

正好是$\psi$；即，(b) 成立。相反，假设 (b) 成立。我们证明$a_i$在对中必然互质。相反的情况下，对于$i \neq j$，将存在理想的$c \neq A$包含$a_i$和$a_j$。我们集合$a_h' = a_h$对于$h$不等于$i$或$j$和$a_i' = a_j' = c$； 典范同态 $\phi': A \to \prod_{i \in I} (A/a_i')$ 可以写成复合映射

$$
A \xrightarrow{\phi} \prod_{i \in I} (A/a_i) \xrightarrow{f} \prod_{i \in I} (A/a_i')
$$

$f$为典范同态$A/a_i \to A/a_i'$中的乘积；显然$\phi'$不是满射，$+(A)$到$(A/a_i') \times (A/a_i')$的投影是乘积$(A/c) \times (A/c)$的对角线，这与自$c \neq A$以来的乘积不同。由于 $f$ 是满射，这表明 $\phi$ 不是满射。

#### 命题 6 {#ac-ii-s1-prop-6 .statement tag=0457}

*设$(a_i)_{i \in I}$为环$A$的非空有限理想族，它们在对互质；设$a$为$a_i$的交。对于每个$A$-模$M$，典范映射$M \to \prod_{i \in I} (M/a_i M)$是满射，其核是$aM$。*

显然$M$到$\prod_{i \in I} (M/a_i M)$的典范映射是$aM$上的零；然后，通过商，它定义同态$A : M/aM \to \prod_{i \in I} (M/a_i M)$。 另一方面，通过命题 5，典范同态
$$
\psi : A/a \to \prod_{i \in I} (A/a_i)
$$
是双射的。 那么$1_M \otimes \psi : M \otimes (A/a) \to M \otimes \prod_{i \in I} (A/a_i)$也是如此。 Now $M \otimes (A/a)$ is identified with $M/aM$ and $M \otimes \prod_{i \in I} (A/a_i)$ with $\prod_{i \in I} M \otimes (A/a_i)$, which is itself identified with $\prod_{i \in I} (M/a_i M)$. 立即验证，上述标识变换$1_M \otimes \psi$变为$\lambda$、从而命题。

#### 例 {#ac-ii-s1-n2-exa-1 .statement tag=0458}

令$K$为域，$a, (1 \leq i \leq m)$与$K$不同元素，并且对于每个$i$，令$g_i$为$K[X]$中的多项式；主理想$(X - a_i) = m_i$在$K[X]$中最大，因此，对于$m$整数$\geq 1$的每个系统$(n_i)_{1 \leq i \leq m}$，理想$m_i^{n_i}$在对中相对素。那么从命题 5 可以得出，存在一个多项式$f \in K[X]$，使得$f(X) \equiv g_i(X) \pmod{(X - a_i)^{n_i}}$对应$1 \leq i \leq m$，两个这样的多项式的差可以被$\omega(X) = \prod_{i=1}^m (X - a_i)^{n_i}$整除。如果所有$n_i$都等于1，我们发现问题可以通过拉格朗日插值公式（*代数*，章IV, § 2, no. 4）显式求解。

### 习题{#ac-ii-s1-exercises}

§ 1](exercises/s1/)参见[习题。
