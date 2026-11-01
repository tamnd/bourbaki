---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 5
section_title: Properties of integers
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 171-183, 235-240
pdf_pages: 0177-0189, 0241-0246
extraction: ocr
subsections:
    - "no": 1
      title: OPERATIONS ON INTEGERS AND FINITE SETS
      page: 171
      pdf_page: 177
    - "no": 2
      title: STRICT INEQUALITIES BETWEEN INTEGERS
      page: 173
      pdf_page: 179
    - "no": 3
      title: INTERVALS IN SETS OF INTEGERS
      page: 174
      pdf_page: 180
    - "no": 4
      title: FINITE SEQUENCES
      page: 175
      pdf_page: 181
    - "no": 5
      title: CHARACTERISTIC FUNCTIONS OF SETS
      page: 175
      pdf_page: 181
    - "no": 6
      title: EUCLIDEAN DIVISION
      page: 176
      pdf_page: 182
    - "no": 7
      title: EXPANSION TO BASE $b$
      page: 177
      pdf_page: 183
    - "no": 8
      title: COMBINATORIAL ANALYSIS
      page: 179
      pdf_page: 185
statements: 30
exercises: 18
content_sha256: 1a0fb63325e91b9ead970ba30755d1526d8670647a32bf48ee4049c9fa72434e
translated_from: content/en/ens/III/05_s5_properties_of_integers.md
translation_method: google
source_content_sha256: 3be04f126cfae8abc23e921d976ad2b92ca04282828df49f6677b21e985508ca
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 223e990c4ca269254299e4cbdeda1692ea92fac2d4d6a7b5cc4d04d3c3b896d7
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 5. 整数的特性

### 1. 运算整数且有限集合

#### 命题 1 {#ens-iii-s5-prop-1 .statement tag=03LP}

*令$(a_i)_{i \in I}$为整数的有限族。那么基数$\sum_{i \in I} a_i$和$\prod_{i \in I} a_i$是整数。*

让我们首先证明，如果$a$和$b$是整数，那么$a + b$也是。我们于 $b$ 乘归纳出发。自 $a + 0 = a$ 起，断言对于 $b = 0$ 成立。如果$a + b$是整数，那么$(a + b) + 1$也是§ 4, no. 1，命题1）。但是$(a + b) + 1 = a + (b + 1)$（§ 3, no. 3，命题5的推论）；因而，$a + (b + 1)$ 是整数，因此对于所有整数 $b$，$a + b$ 是整数。

接下来我们通过归纳对$n = \mathrm{Card}\ (\mathrm{I})$证明$\sum\limits_{i \in \mathrm{I}} a_i$是整数。如果$n = 0$，那么$\mathrm{I} = \emptyset$和$\sum\limits_{i \in \mathrm{I}} a_i = 0$，这很清楚。如果$\mathrm{Card}\ (\mathrm{I}) = n + 1$，我们可以写成$\mathrm{I} = \mathrm{J} \cup \{k\}$，其中$\mathrm{Card}\ (\mathrm{J}) = n$和$k \notin \mathrm{J}$。然后

$$\sum_{i \in \mathrm{I}} a_i = a_k + \sum_{i \in \mathrm{J}} a_i$$

（$\S\,3$、no. 3、命题 5）。归纳假设即$\sum\limits_{i \in \mathrm{J}} a_i$为整数；因而，来自证明第一段的$a_k + \sum\limits_{i \in \mathrm{J}} a_i$也是如此。这表明对于所有 $n$，$\sum\limits_{i \in \mathrm{I}} a_i$ 都是整数。

由于两个整数$a$和$b$的乘积$ab$是整数有限族中的和，并且全部等于$a$（$\S\,3$，no. 4， 命题 6，推论2)，$ab$ 是整数。我们用归纳对$n = \mathrm{Card}\ (\mathrm{I})$证明$\prod\limits_{i \in \mathrm{I}} a_i$是整数。这对于 $n = 0$ 来说是正确的，因为那么

$$\prod_{i \in \mathrm{I}} a_i = 1.$$

如果$\mathrm{Card}\ (\mathrm{I}) = n + 1$，我们有（与上面相同的记号）

$$\prod_{i \in \mathrm{I}} a_i = a_k \cdot \prod_{i \in \mathrm{J}} a_i$$

($\S\,3$, no. 3, 命题 5)，因此归纳假设意味着$\prod\limits_{i \in \mathrm{I}} a_i$是整数。因而，对于所有 $n$，$\prod\limits_{i \in \mathrm{I}} a_i$ 都是整数。

#### 推论 1 {#ens-iii-s5-prop-1-cor-1 .statement tag=03LQ}

*并* E *有限族* $(\mathrm{X}_i)_{i \in \mathrm{I}}$ *有限集合是有限集合。*

对于和族$(\mathrm{X}_i)$的S是有限的；并且由于 S 到 E 上存在映射 (章 II, $\S\,4$, no. 8), 集合 E 是有限的 ($\S\,4$, no. 2, 命题 2, 推论 3)。

#### 推论 2 {#ens-iii-s5-prop-1-cor-2 .statement tag=03LR}

*有限集合的有限族中的乘积是有限的集合。*

#### 推论 3 {#ens-iii-s5-prop-1-cor-3 .statement tag=03LS}

*如果$a$和$b$为整数，则$a^b$为整数。*

因为$a^b$是整数有限族中的乘积，全部等于$a$（$\S\,3$，no. 5，命题10）。

#### 推论 4 {#ens-iii-s5-prop-1-cor-4 .statement tag=03LT}

*有限集合* E *的子集的集合是有限的。*

因为它的基数是 $2^{\mathrm{Card}\ (\mathrm{E})}$ ($\S\,3$, no. 5, 命题 12)。

### 2. 严格不等式整数之间

#### 命题 2 {#ens-iii-s5-prop-2 .statement tag=03LU}

*令$a$和$b$为两个整数。那么$a < b$当且仅当存在整数$c > 0$使得$b = a + c$。*

如果$a < b$，则存在基数$c \leqslant b$（因此$c$是整数（§ 4, no. 2，命题2））使得$b = a + c$（§ 3, no. 6，命题13）；如果$a \neq b$，我们必须有$c \neq 0$。相反，如果$b = a + c$和$c \neq 0$，则$c \geqslant 1$，从而$a < a + 1 \leqslant a + c = b$。

#### 命题 3 {#ens-iii-s5-prop-3 .statement tag=03LV}

*令$(a_i)_{i \in I}$和$(b)_{i \in I}$为整数的两个有限族，使得$a_i \leqslant b_i$对应于每个$i \in I$，$a_i < b_i$对应于至少一个指标$i$。然后*

$$\sum_{i \in I} a_i < \sum_{i \in I} b_i.$$

*如果每个$i \in I$也有$b_i > 0$，那么*

$$\prod_{i \in I} a_i < \prod_{i \in I} b_i.$$

令$j$为指标，使得$a_j < b_j$，并令$J = I - \{j\}$。然后

$$b_j = a_j + c_j$$

$c_j > 0$ (命题 2)，因此 (§ 3, no. 6，命题 14)

$$\sum_{i \in I} b_i = a_j + c_j + \sum_{i \in J} b_i \geqslant c_j + a_j + \sum_{i \in J} a_i = c_j + \sum_{i \in I} a_i.$$

从$c_j > 0$开始，命题的第一个部分是从命题2开始的。同样

$$\prod_{i \in I} b_i = (a_j + c_j) \prod_{i \in J} b_i = a_j . \prod_{i \in J} b_i + c_j . \prod_{i \in J} b_i \geqslant \prod_{i \in I} a_i + c_j . \prod_{i \in J} b_i.$$

由于$c_j$和所有$b_i$都是$\neq 0$，所以乘积$c_j . \prod_{i \in J} b_i$是$\neq 0$（§ 3, no. 4，命题7）；因此，命题的第二个部分。

#### 推论 1 {#ens-iii-s5-prop-3-cor-1 .statement tag=03LW}

*令$a$、$a'$和$b$为整数，使得$a < a'$和$b > 0$。然后$a^b < {a'}^b$.*

我们只需将$a^b$和${a'}^b$表示为整数有限族的乘积（§ 3, no. 5，命题10）和应用命题3，注意到，关系$a < a'$意味着$a' > 0$。

#### 推论 2 {#ens-iii-s5-prop-3-cor-2 .statement tag=03LX}

*令$a$、$b$和$b'$为整数，使得$a > 1$和$b < b'$；然后$a^b < a^{b'}$.*

因为存在整数 $c > 0$ 使得 $b' = b + c$ (命题 2)；从$c \geqslant 1$开始，我们有$a^c \geqslant a > 1$，从而$a^{b'} = a^b a^c > a^b$。

#### 推论 3 {#ens-iii-s5-prop-3-cor-3 .statement tag=03LY}

*令$a$、$b$、$b'$为整数*（分别为*整数，使得$a > 0$*）。 *然后$a + b = a + b'$*（或*$ab = ab'$*）*当且仅当$b = b'$。*

#### 推论 4 {#ens-iii-s5-prop-3-cor-4 .statement tag=03LZ}

*如果$a$和$b$是整数使得$a \leqslant b$，则存在唯一的整数$c$使得$b = a + c$。*

$c$的存在来自§ 3, no. 6的命题13，而唯一性则来自上述推论3。

¶ 整数 $c$，使得 $b = a + c$（其中 $a \leqslant b$）被称为整数 $b$ 和 $a$ 的*差*，并写作 $b - a$。容易验证，如果$a$，$b$，$a'$，$b'$是整数使得$a \leqslant b$和$a' \leqslant b'$，那么

$$(b - a) + (b' - a') = (b + b') - (a + a').$$

### 3. 集合 / 整数之间的间隔

整数中的每一个集合，即基数的集合，都是良序的（§ 3, no. 2，定理 1）。此外，对于每个整数$a$关系，“$x$是基数，$x \leqslant a$”在$x$中是集合化（§ 3, no. 2，注之后定理1），并且$x$的集合，其中满足这个关系是整数的集合（§ 4, no. 2，命题2），因此可以用$[0, a]$表示。

#### 命题 4 {#ens-iii-s5-prop-4 .statement tag=03M0}

*令$a$和$b$为整数。那么映射$x \rightarrow a + x$就是区间$[0, b]$到区间$[a, a + b]$的严格递增同构，而$y \rightarrow y - a$就是逆同构。*

显然关系$0 \leqslant x \leqslant b$意味着$a \leqslant a + x \leqslant a + b$。 映射 $x \rightarrow a + x$ 是严格递增的（因此是单射）乘以 no. 2 的命题 3。最后，关系$a \leqslant y \leqslant a + b$隐含$y = a + x$与$x \geqslant 0$和$a + x \leqslant a + b$，从而$x \leqslant b$（no. 2，命题3）。这样就完成了证明。

#### 命题 5 {#ens-iii-s5-prop-5 .statement tag=03M1}

*如果$a$和$b$是整数使得$a \leqslant b$，那么区间$[a, b]$是一个有限的集合，其元素的数是$b - a + 1$。*

到命题 4，我们可以将我们限制在$a = 0$的情况。 证明于 $b$ 归纳发布。如果$b = 0$，结果就清楚了。 关系$0 \leqslant x \leqslant b + 1$相当于“$0 \leqslant x < b + 1$或$x = b + 1$”，关系$0 \leqslant x < b + 1$相当于$0 \leqslant x \leqslant b$（§ 4, no. 2、命题2）；在其他字中，$[0, b + 1]$是$[0, b]$和$\{b + 1\}$的并，而这两个集合是不相交的。由$[0, b + 1]$的元素归纳假设数等于$(b + 1) + 1$，证明命题。

#### 命题 6 {#ens-iii-s5-prop-6 .statement tag=03M2}

*对于每个有限的集合* E *，它是全序的并且有 n 元素* $(n \geqslant 1)$，*在区间* $[1, n]$ 上存在一个唯一的同构 * E *。

由于 E 和 $[1, n]$ 是良序的（§ 4, no. 4、命题 3，推论 1）并且具有与元素相同的数 (命题 5)，因此结果由 § 2, no. 5 的定理 3 和推论 2 得出命题 2 个，共 § 4, no. 2。

### 4. 有限序列

A *有限序列*（集合* E 的元素的 *有限序列）是一个族（分别是 E 的元素的族），其指标集合 I 是有限的集合整数。 I的元素数称为序列的*长度*。

设$(t_i)_{i \in I}$为长度$n$中的有限序列。到 no. 3 的命题 6 时，在整数 I 的集合上存在间隔 $[1, n]$ 的唯一同构 $f$。对于每个 $k \in [1, n]$，$t_{f(k)}$ 被认为是序列* 的 *kth 项； $t_{f(1)}$（或$t_{f(n)}$）是序列的*第一个*（或*最后一个*）*项*。

令$\mathrm{P}\{i\}$为关系，使得元素$i$，其中$\mathrm{P}\{i\}$为真形式，整数的有限集合。 有限序列 $(t_i)_{i \in I}$ 通常写作$(t_i)_{\mathrm{P}\{i\}}$。对于例、$\mathrm{I} = [a, b]$时，常使用记号$(t_i)_{a \leqslant i \leqslant b}$。同条件下，表示集族的积$(\mathrm{X}_i)_{i \in I}$记号

$$\prod_{\mathrm{P}\{i\}} \mathrm{X}_i \quad \text{and} \quad \prod_{i=a}^{b} \mathrm{X}_i$$

被使用；类似的记号代表并，交，基数乘积，基数和，代数\*中的\*合成律，等等。

### 5. 特征函数集合

设E为非空集合，E的A子集。E的子集A的*特征函数*是E的映射$\varphi_\mathrm{A}$进入集合$\{0, 1\}$，定义为

$$\varphi_\mathrm{A}(x) = 1 \quad \text{if} \quad x \in \mathrm{A}; \qquad \varphi_\mathrm{A}(x) = 0 \quad \text{if} \quad x \in \mathrm{E} - \mathrm{A}.$$

¶ 显然关系 $\varphi_\mathrm{A} = \varphi_\mathrm{B}$ 等价于 $\mathrm{A} = \mathrm{B}$。我们为所有$x \in \mathrm{E}$提供了$\varphi_\mathrm{E}(x) = 1$，为所有$x \in \mathrm{E}$提供了$\varphi_{\emptyset}(x) = 0$；这些是 E 上唯一的常数特征函数。以下命题是定义的直接的推论 ：

#### 命题 7 {#ens-iii-s5-prop-7 .statement tag=03M3}

*对于非空集合* E 的子集* A、B *中的每个对，*我们有*

(1) $$\varphi_{\mathrm{E-A}}(x) = 1 - \varphi_{\mathrm{A}}(x),$$

(2) $$\varphi_{\mathrm{A} \cap \mathrm{B}}(x) = \varphi_{\mathrm{A}}(x)\varphi_{\mathrm{B}}(x),$$

(3) $$\varphi_{\mathrm{A} \cup \mathrm{B}}(x) + \varphi_{\mathrm{A} \cap \mathrm{B}}(x) = \varphi_{\mathrm{A}}(x) + \varphi_{\mathrm{B}}(x)$$

*对于所有人*$x \in \mathrm{E}$。

### 6. 欧几里得除法

#### 定理 1 {#ens-iii-s5-thm-1 .statement tag=03M4}

*设a和b为整数，使得$b > 0$。则存在整数 q 和 r，使得 $a = bq + r$ 和 $r < b$，并且整数 q 和 r 由这些条件唯一确定。*

$q$和$r$上的条件相当于$bq \leqslant a < b(q + 1)$和$r = a - bq$（no. 2、命题2）。因此我们必须找到$q$使得$bq \leqslant a < b(q + 1)$；在其他字中，$q$必须是最小的整数使得$a < b(q + 1)$，这表明$q$和$r = a - bq$是唯一确定的。为了证明它们的存在，我们注存在整数$p$使得$a < bp$，对于例$a + 1$（从$b > 0$开始）。令 $m$ 为这些整数中最小的一个。我们有$m \neq 0$，因此我们可以将$m = q + 1$写成$q \leqslant m$（§ 4, no. 2，命题2）；由此可见$bq \leqslant a < b(q + 1)$。

#### 定义 1 {#ens-iii-s5-def-1 .statement tag=03M5}

*当记号等于定理1时，r称为a除以b的余数。如果$r = 0$，我们说a是b的倍数，或者a可以被b整除，或者b是a的除子，或者b除a，或者b是a的因子。 数 q 称为 a 除以 b 的商，并用 $\dfrac{a}{b}$ 或 $a/b$ 表示。*

如果 $a$ 不是 $b$ 的倍数，数 $q$ 称为 *a 与 b* 的商的积分部分（cf. *一般拓扑*、章 IV, § 8, no. 2）。

*在这个章*中，写下$a/b$或$\dfrac{a}{b}$将意味着$b$除$a$。

关系 $a = bq$ 和 $q = a/b$ 等效（如果 $b > 0$）。 $b$的倍数$a$每倍数$a'$是$b$的倍数，并且

$$a'/b = (a'/a)\,(a/b) \qquad \text{if} \qquad a \neq 0.$$

另外，如果$c$和$d$是$b$的倍数，那么$c+d$和$c-d$（如果$d\leq c$）是$b$的倍数，并且我们有

$$\frac{c+d}{b}=\frac{c}{b}+\frac{d}{b},\qquad \frac{c-d}{b}=\frac{c}{b}-\frac{d}{b}.$$

整数是 2 的倍数被认为是*偶数*，而其他的则是*奇数*。到定理 1 时，奇数整数为形式 $2n+1$。

### 7. 展开至基 $b$

#### 命题 8 {#ens-iii-s5-prop-8 .statement tag=03M6}

*令$b$为整数$>1$。对于每个整数$k>0$，令$E_k$为与$[0,b-1]$相同的区间系列$(J_h)_{0\leq h\leq k-1}$的字典乘积（§ 2, no. 6）。对于每个$r=(r_0,r_1,\ldots,r_{k-1})\in E_k$，让*

$$f_k(r)=\sum_{h=0}^{k-1}r_hb^{k-h-1};$$

*那么映射$f_k$是有序的集合$E_k$到区间$[0,b^k-1]$的同构。*

证明于 $k$ 归纳发布。对于$k=1$，它是定义的直接的推论。对于每 $r=(r_0,\ldots,r_{k-1},r_k)\in E_{k+1}$ 投入

$$\varphi(r)=(r_0,\ldots,r_{k-1})\in E_k.$$

那么映射$r\mapsto(\varphi(r),r_k)$就是$E_{k+1}$的同构到$E_k$和$J=[0,b-1]$的字典顺序乘积上；这是来自定义的直接的。我们可以写

$$f_{k+1}(r)=b\cdot f_k(\varphi(r))+r_k;$$

让我们证明$E_{k+1}$中的关系$r<r'$蕴涵$f_{k+1}(r)<f_{k+1}(r')$。事实上，我们要么有$\varphi(r)<\varphi(r')$，要么有$\varphi(r)=\varphi(r')$和$r_k<r'_k$。在第一种情况下，归纳假设意味着 $f_k(\varphi(r))<f_k(\varphi(r'))$，因而 (§ 4, no. 2, 命题 2) $f_k(q(r'))\geq f_k(\varphi(r))+1$；因而

$$f_{k-1}(r')\geq b\cdot f_k(\varphi(r))+b>f_{k+1}(r),$$

从$r_k\leq b-1$（no. 2，命题3）开始。另一方面，如果$\varphi(r)=\varphi(r')$和$r_k<r'_k$，则显然$f_{k+1}(r)<f_{k+1}(r')$。现在归纳假设表明$f_k(\varphi(r))\leq b^k-1$，从而

$$f_{k+1}(r)\leq b(b^k-1)+b-1=b^{k+1}-1.$$

由此可见，$f_{k+1}$是$E_{k+1}$的同构到区间$[0,b^{k+1}-1]$的子集；但这个区间和$E_{k+1}$有相同的数元素，即$b^{k+1}$（no. 3，命题5）；因而$f_{k+1}$是双射（§ 4, no. 2，命题2，推论4），证明是完整的。
¶ 我们注现在，对于每一个整数 $a$，我们就有 $a < b^a$。这由$a$上的归纳证明；对于$a = 0$，结果很明显，假设$a < b^a$意味着$a + 1 \leqslant b^a < b \cdot b^a = b^{a+1}$（no. 2、命题 3 和§ 4, no. 2、命题 2）。因而，至少存在整数$k$使得$a < b^k$，并且命题8则表明存在唯一的有限序列$(r_h)_{0 \leqslant h \leqslant k-1}$使得$0 \leqslant r_h \leqslant b - 1$对于$0 \leqslant h \leqslant k - 1$并且
$$a = \sum_{h=0}^{k-1} r_h b^{k-h-1}.$$
此外，我们必须有$r_0 > 0$，否则凭借命题 8 就有$a < b^{k-1}$。表达式
$$\sum_{h=0}^{k-1} r_h b^{k-h-1}$$
称为整数$a$的*展开到基$b$*。

\* 在所有不涉及数值计算的部分数学中，命题8主要在应用于*素的*数$b$时有用。 \*

当整数 $b$ 足够小以使其可行时，我们可以用称为*数字*的独特符号来表示每个整数 $< b$。代表0和1的数字通常是0和1。令$a$为整数，令$\sum_{h=0}^{k-1} r_h b^{k-h-1}$为其展开至基$b$。如果展开中出现的整数$k$足够小，可以实现，通常将整数$a$与从左到右写$r_0 r_1 \ldots r_{k-2} r_{k-1}$然后每个整数写替换所获得的一系列符号相关联$r_i$ 由代表它的数字组成；如此获得的符号称为与$a$相关的*数字符号*。然后经常通过它出现的项与关系中的数字符号来替换$a$。

对于例，若C、Q、F、D为数字，则数字符号CQ、CQF、CQFD分别与$\mathrm{C}b + \mathrm{Q}$、$\mathrm{C}b^2 + \mathrm{Q}b + \mathrm{F}$、$\mathrm{C}b^3 + \mathrm{Q}b^2 + \mathrm{F}b + \mathrm{D}$相关联。

从命题 8 可以看出，与整数 $a$ 相关的数字符号是唯一的，并且如果 $a < b^k$ 则包含最多为 $k$ 位。请注意，与整数 $b^k$ 关联的数字符号由数字 1 后跟 $k$ 数字 0 组成。

这个用数字符号来表示的整数表示系统，称为对基$b$*的计数*系统。在实际数值计算中，使用以下系统：(*a*)系统至基2，或*二元系统*，其中数字为0和1； (*b*) *十进制系统*，其中数字为$0$、$1$、$2$、$3$、$4$、$5 = 4 + 1$、$6 = 5 + 1$、$7 = 6 + 1$、$8 = 7 + 1$、 $9 = 8 + 1$，其中$b$为整数$9 + 1$（系统中的数字符号因此为10）。

自中世纪以来，十进制系统一直用于数值计算，每当我们有机会明确写下整数时，我们都会在级数中使用它。我们建议读者参考本篇级数中的部分，专门讨论方法的数值计算，以获得与和相关的数值符号、差值、乘积以及由数值符号给出的两个整数的商的积分部分。

### 8. 组合分析

#### 命题 9 {#ens-iii-s5-prop-9 .statement tag=03M7}

*让* $\mathrm{E}$ *和* $\mathrm{F}$ *成为两个集合，* $\mathfrak{a}$ *和* $\mathfrak{b}$ *他们的基数，* $f$ *将* $\mathrm{E}$ *投射到* $\mathrm{F}$ *使得集合* $\overset{-1}{f}(y)$，*其中* $y \in \mathrm{F}$，*都具有相同的基数* $\mathfrak{c}$。 *然后*$\mathfrak{a} = \mathfrak{b}\mathfrak{c}$。

对于家庭$(\overset{-1}{f}(y))_{y \in \mathrm{F}}$是$\mathrm{E}$的划分，每个元素其中划分是基数$\mathfrak{c}$的集合；因此得到结果（§ 3, no. 4，命题 6，推论 2）。

#### 定义 2 {#ens-iii-s5-def-2 .statement tag=03M8}

*设* $n$ *为整数。* *乘积* $\prod_{i < n} (i + 1)$ *表示为* $n!$（读为“阶乘$n$”）。

我们有$0! = 1$（章II, § 5, no. 3）和$1! = 1$。对于每个整数$n$，我们有$(n + 1)! = n!\,(n + 1)$。这个关系与关系$0! = 1$一起表征了项$n!$，正如$n$上的归纳很容易看出。

#### 命题 10 {#ens-iii-s5-prop-10 .statement tag=03M9}

*设*$m$*和*$n$*为整数，使得*$m \leqslant n$。 *则* $n!/(n - m)!$ *是集合* $\mathrm{A}$ *和* $m$ *元素的单射映射数到集合* $\mathrm{B}$ *和* $n$ *元素.*

The proof is by induction on the number $m \leqslant n$ of elements of $\mathrm{A}$. 如果$m = 0$，结果就很明显了。 假设$m + 1 \leqslant n$。 令$\mathrm{A}$与$m + 1$元素成为集合，令$\mathrm{A}'$与$m$元素成为$\mathrm{A}$的子集，并令$\{a\} = \mathrm{A} - \mathrm{A}'$。 Let $\mathrm{F}$, $\mathrm{F}'$ be the sets of injective mappings of $\mathrm{A}$, $\mathrm{A}'$ respectively into $\mathrm{B}$, and let $\varphi$ be the mapping $f \to f\,|\mathrm{A}'$ which maps each function $f \in \mathrm{F}$ to its restriction to $\mathrm{A}'$. 对于$\overset{-1}{\varphi}(f')$的每个$f' \in \mathrm{F}'$元素$f$由其值$f(a)$唯一确定；由于$f$是单射的，所以我们必须有$f(a) \in \mathrm{B} - f'(\mathrm{A}')$。 由此可见，$\overset{-1}{\varphi}(f')$ 与 $\mathrm{B} - f'(\mathrm{A}')$ 具有相同的元素数 $n - m$。 因而，到命题 9 时，$\mathrm{F}$ 有

$$(n - m)\,\frac{n!}{(n - m)!} = \frac{n!}{(n - m - 1)!}$$

元素凭借感应假设。这样就完成了证明。

#### 推论{#ens-iii-s5-n8-cor-1 .statement tag=03MA}

*有限集合的置换的数且 n 元素等于 n!.*

为此，数等于集合的单射的数自身（§ 4, no. 2，命题2，推论4）。

#### 命题 11 {#ens-iii-s5-prop-11 .statement tag=03MB}

*让* E *是一个有限的集合，n为元素，并让*$(p_i)_{1 \leqslant i \leqslant h}$*为整数的有限序列，使得*$\sum_{i=1}^{h} p_i = n$。 *然后数覆盖物* $(X_i)_{1 \leqslant i \leqslant h}$ *的* E *相互不相交的集合* $X_i$ *使得* $\mathrm{Card}\,(X_i) = p_i$ *对于* $1 \leqslant i \leqslant h$ *等于*

$$n! \Big/ \prod_{i=1}^{h} p_i!.$$

令 G 为 E 的置换的集合，并令 P 为覆盖$(X_i)_{1 \leqslant i \leqslant h}$ 的集合，其中满足条件命题。 由于 $\sum_{i=1}^{h} p_i = n$，P 不为空。 令$(A_i)_{1 \leqslant i \leqslant h}$为P的元素。对于每个置换$f \in G$，族$(f(A_i))_{1 \leqslant i \leqslant h}$再次属于到P；让我们用$\varphi(f)$来表示它。 对于每个元素$(X_i)_{1 \leqslant i \leqslant h}$，让我们对置换$f \in G$进行计算数，这样$\varphi(f) = (X_i)$。 当且仅当对于每个指标$i$我们有$f(A_i) = X_i$，我们才会有$\varphi(f) = (X_i)$。 Hence the set of permutations $f$ under consideration is equipotent to the product of the sets of bijections of $A_i$ onto $X_i$ (Chapter II, § 4, no. 7, Proposition 8); consequently the set $\overset{-1}{\varphi}((X_i)_{1 \leqslant i \leqslant h})$ has $\prod_{i=1}^{h} p_i!$ elements (Corollary to Proposition 10). 由于 G 有 $n!$ 元素，因此现在的结果是从命题 9 得出的。

#### 推论 1 {#ens-iii-s5-prop-11-cor-1 .statement tag=03MC}

*设* A *为集合，n 元素，并令 p 为整数* $\leqslant n$。 *那么* A *的子集的数有p元素是*$\dfrac{n!}{p!(n-p)!}$。

将 $h = 2$、$p_1 = p$、$p_2 = n - p$ 放入命题 11。

¶ The number of subsets containing $p$ elements in a set of $n$ elements (where $p \leqslant n$) is denoted by $\begin{pmatrix} n \\ p \end{pmatrix}$ and is called the *binomial coefficient with indices n and p*. 从关系 $\begin{pmatrix} n \\ p \end{pmatrix} = \dfrac{n!}{p!(n-p)!}$ 紧接着是 $\begin{pmatrix} n \\ p \end{pmatrix} = \begin{pmatrix} n \\ n-p \end{pmatrix}$。

This is also a consequence of the fact that, if E is a set with $n$ elements, $X \to E - X$ is a bijection of the set of subsets of E consisting of $p$ elements onto the set of subsets of $n - p$ elements.

我们为自然整数的每个对放置$\binom{n}{p} = 0$，使得$p > n$。 按照此约定，对于*每个*自然的整数$p$，$n$元素的集合中的$p$元素中的子集数是$\binom{n}{p}$。

#### 推论 2 {#ens-iii-s5-prop-11-cor-2 .statement tag=03RG}

*设*E*和*F*分别是全序有限集合和*$p$*和*$n$*元素。那么* E *的严格递增的映射的数变成* F *是* $\binom{n}{p}$。

对于这样的映射是E到F的单射（§ 1, no. 12，命题11），并且由于E和F是良序的（§ 4, no. 4，推论1到命题3），对于$p$的每个子集X F 的元素恰好有一个 E 的严格递增的映射到 X (§ 2, no. 5, 定理 3)。

#### 命题 12 {#ens-iii-s5-prop-12 .statement tag=03RH}

*对于每个整数* $n$，*我们有*

$$\sum_p \binom{n}{p} = 2^n.$$

因为如果E是$n$元素的集合，等式的左侧是E的子集的数。现在§ 3, no. 5的应用命题12。

#### 命题 13 {#ens-iii-s5-prop-13 .statement tag=03RI}

*如果* $n$ *和* $p$ *是整数，那么*

$$\binom{n+1}{p+1} = \binom{n}{p+1} + \binom{n}{p}.$$

令E为集合和$n + 1$元素，令P为E包含$p + 1$元素的所有子集的集合，令$a$为E的元素，并把

$$\mathrm{E}' = \mathrm{E} - \{a\}.$$

令P′（或P”）表示E的$p + 1$元素的子集的集合，其中包含$a$（分别不包含$a$）。 集合 P″ 是 E′ 的 $p + 1$ 元素的子集的集合，因此有 $\binom{n}{p+1}$ 元素。 映射$\mathrm{X} \to \mathrm{X} \cap \mathrm{E}'$是P′的双射到E′的$p$元素的子集的集合，因此P′有$\binom{n}{p}$元素。 现在的结果是 P 是不相交的集合 P′ 和 P” 的并。

命题13也可以通过公式$\binom{n}{p} = \dfrac{n!}{p!(n-p)!}$对$p \leqslant n$的简单计算来证明。

#### 命题 14 {#ens-iii-s5-prop-14 .statement tag=03RJ}

*设*$n$*为整数*$> 0$。 *然后数*$a_n$（分别$b_n$）*有序对*$(i, j)$*整数使得*$1 \leqslant i \leqslant j \leqslant n$（分别$1 \leqslant i < j \leqslant n$）*是*$\frac{1}{2}n(n+1)$（（分别$\frac{1}{2}n(n-1)$））。

对于$b_n$是$[1, n]$中2元素子集数；因此

$$b_n = \frac{n!}{2!(n-2)!} = \frac{1}{2} n(n-1).$$

由此推导出$a_n$的值，注意有序对$(i, j)$的集合，使得$1 \leqslant i \leqslant j \leqslant n$是有序对$(i, j)$的集合的并，使得$1 \leqslant i \leqslant j < n$和集合共对 $(i, i)$，其中 $1 \leqslant i \leqslant n$。因此$a_n = n + b_n = \frac{1}{2} n(n+1)$。

#### 推论{#ens-iii-s5-n8-cor-2 .statement tag=03RK}

*对于每个整数 $n > 0$，我们有*

$$\sum_{i=1}^{n} i = \frac{1}{2} n(n+1).$$

在整数$(i, j)$的有序对的集合A中，使得$1 \leqslant i \leqslant j \leqslant n$，让$A_k$表示对$(i, k)$的子集，其中$1 \leqslant i \leqslant k$（对于任意整数 $k \leqslant n$）。那么$A_k$有$k$元素。但$(A_k)_{1 \leqslant k \leqslant n}$是A的划分；因此结果。

#### 命题 15 {#ens-iii-s5-prop-15 .statement tag=03RL}

*设$n$和$h$为整数，并让*E *为集合以及$h$元素。那么* E *的映射 $u$的数*进入*$[0, n]$*使得*$\sum_{x \in E} u(x) \leqslant n$*（分别*$\sum_{x \in E} u(x) = n$，*对于$h > 0$）是*

$$\binom{n+h}{h} \left( \text{resp.} \ \binom{n+h-1}{h-1} \right).$$

让$A(h, n)$（或$B(h, n)$）表示E的映射$u$到$[0, n]$的数，使得$\sum_{x \in E} u(x) \leqslant n$（或$\sum_{x \in E} u(x) = n$代表$h > 0$）。我们首先显示$A(h-1, n) = B(h, n)$。为此，令 E′ 为 E 的子集，其中 $h - 1$ 元素，并令 $\{a\} = E - E'$。如果$u$是E到$[0, n]$的映射，使得$\sum_{x \in E} u(x) = n$，那么它的限制$u'$到E′使得$\sum_{x \in E'} u'(x) \leqslant n$，而且还有$u(a) = n - \sum_{x \in E'} u'(x)$。反之，E′的每一个映射$u'$进入$[0, n]$，满足E的$\sum_{x \in E'} u'(x) \leqslant n$定义唯一映射$u$进入$[0, n]$，其中$u'$是限制，并且这样： $\sum_{x \ni E} u(x) = n$。

我们注接下来，如果$\sum_{x \in E} u(x) \leqslant n$，那么要么$\sum_{x \in E} u(x) = n$，要么$\sum_{x \in E} u(x) \leqslant n-1$，并且这两种可能性是互斥的。因而

$$A(h, n) = A(h, n-1) + B(h, n) = A(h, n-1) + A(h-1, n).$$

从$A(0, 0) = 1 = \binom{0}{0}$开始，公式$A(h, n) = \binom{n+h}{h}$从上面开始，从命题13开始，到$n + h$上的归纳。

\* $h$ 中单项式 $X_1^{\alpha_1} X_2^{\alpha_2} \ldots X_h^{\alpha_n}$ 的数不定，总计次数 $\leqslant n$ 显然等于映射 $i \rightarrow \alpha_i$ 的数 $[1, h]$ 到 $[0, n]$ 使得$\sum_{i=0}^{h} \alpha_i \leqslant n$，因此等于$\binom{n+h}{h}$乘命题 15；这个数也是$h + 1$不定式中单项式的数，总次数$n$。 \*

### 习题 {#ens-iii-s5-exercises}

参见[习题为 § 5](exercises/s5/)。
