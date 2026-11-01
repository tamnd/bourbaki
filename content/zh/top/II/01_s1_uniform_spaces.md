---
book: top
book_title: General Topology
chapter: II
chapter_title: Uniform Structures
section: 1
section_title: Uniform spaces
lang: zh
source: top-i-iv
book_pages: 169-174, 206-207
pdf_pages: 0175-0180, 0212-0213
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF A UNIFORM STRUCTURE
      page: 169
      pdf_page: 175
    - "no": 2
      title: TOPOLOGY OF A UNIFORM SPACE
      page: 171
      pdf_page: 177
statements: 14
exercises: 5
content_sha256: 9a2557bfcd76a2f6f891611eebd969ad628a5c78d7a2c75f04d68d3b1baef1eb
translated_from: content/en/top/II/01_s1_uniform_spaces.md
translation_method: google
source_content_sha256: 0fd087b92f4bcb3cb8327201790fedf19f1e8b4d6d6fa498400dbc46a4cbcd83
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 623fc7ee6e2a4c2c10c2c88142566378cfd0e4860fbb22db0a1d91e084815486
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 1. 制服空间

### 1. 制服定义结构

#### 定义 1 {#top-ii-s1-def-1 .statement tag=0BCY}

*均匀结构*（或*均匀性*）*在集合*$X$*是结构由集合*$\mathfrak{U}$*的子集*$X \times X$*满足公理*$(\mathrm{F}_1)$*和* $(\mathrm{F}_{\mathrm{II}})$ *of 章 I, § 6, no. 1 并且还满足以下公理*：

(U₁) *每集合属于到* $\mathfrak{U}$ *包含对角线* $\Delta$。

(U2) *如果* $V \in \mathfrak{U}$ *则* $\overline{V}^{-1} \in \mathfrak{U}$。

(U₃) *对于每个* $V \in \mathfrak{U}$ *存在* $W \in \mathfrak{U}$ *使得* $W \circ W \subset V$。

![图2](../images/chapter_ii_uniform_structures.png)

$\mathfrak{U}$的集合称为$\mathfrak{U}$在$X$上定义的均匀性的周围。具有均匀性的集合称为均匀空间。

如果$V$是$X$上的均匀性的随行，我们可以用说来表达关系$(x, x') \in V$“$x$和$x'$是$V$-闭”。

#### 注 1 {#top-ii-s1-n1-rem-1 .statement tag=0BCZ}

为了使语言更具表现力，我们可以在某些叙述中使用表达式“$x$足够接近$y$”和“$x$和$y$尽可能接近”。对于例，我们可以说关系

只要 $x$ 和 $y$ 足够接近，如果存在随行人员 $V$，使得关系 $(x, y) \in V$ 蕴含$R \{ x, y \}$，则 R $\{ x, y \}$ 为真。

#### 注 2 {#top-ii-s1-n1-rem-2 .statement tag=0BD0}

公理 (U_{II}) 和 (U_{III}) 的合取等价于以下公理（假设一致结构的其他公理）：

(U_a) 对于每个$V \in \mathfrak{U}$，存在$W \in \mathfrak{U}$使得$W \circ \overline{W} \subset V$(*)。

显然 (U_{II}) 和 (U_{III}) 意味着 (U_a)。相反，如果 (U_a) 满足，我们有 $\overline{W} = \Delta \circ W \subset V$，通过 (U_I)；因此 $W \subset \overline{V}$ ，因此 [by (F_1)] $\overline{V} \in \mathfrak{U}$。设 $W' = W \cap \overline{W}$；然后根据刚刚证明的公理(F_{II})$W' \in \mathfrak{U}$，我们有$W' \circ W' \subset W \circ \overline{W} \subset V$。

Throughout this chapter we shall write $\overline{V}^2$ instead of $V \circ V$, and in general $\overline{V}^{n-1} = \overline{V} \circ V = V \circ \overline{V}^{n-1}$, for each integer $n > 1$ and each subset $V$ of $X \times X$.

#### 注 3 {#top-ii-s1-n1-rem-3 .statement tag=0BD1}

如果$X$不为空，则公理（U_I）意味着$\mathfrak{U}$中没有集合为空，因此$\mathfrak{U}$是$X \times X$上的过滤器。 空集上只有一种一致性，即$\mathfrak{U} = \{ \emptyset \}$。

#### 定义 2 {#top-ii-s1-def-2 .statement tag=0BD2}

均匀性的基本随从系统是任何随从集合$\mathfrak{B}$，使得每个随从包含集合属于到$\mathfrak{B}$。

公理（U_{III}）表明，如果$n$是任何整数$> 0$并且$V$贯穿基本的随从系统，则集合$\overline{V}^n$又是形式基本的随从系统。

使得 $V = \overline{V}^1$ 的周围$V$ 称为对称。如果 $V$ 是任意环绕体，则 $V \cap \overline{V}^1$ 和 $V \cup \overline{V}^1$ 是对称环绕体，公理 (F_{II}) 和 (U_{II}) 表明对称环绕体形式是基本的系统环绕体。

$X \times X$ 子集集合 $\mathfrak{B}$是$X$上一致的基本随行系统当且仅当$\mathfrak{B}$满足章I, § 6, no. 3的公理（B_I），并且还满足以下条件公理：

(U'_I) $\mathfrak{B}$ 包含对角线 $\Delta$ 的每集合。

(U'_II) 对于每个$V \in \mathfrak{B}$，都存在$V' \in \mathfrak{B}$，使得$V' \subset \overline{V}^1$。

(U'_III) 对于每个$V \in \mathfrak{B}$，都存在$W \in \mathfrak{B}$，使得$\overline{W}^2 \subset V$。

如果$X$不为空，则$X$上制服结构的随行人员的基本系统是由该结构的随行人员形成的过滤器的基（章I, § 6, no. 3，命题3）。

(*) 我们记得（集合理论，R，§ 3，第4和10），如果$V$和$W$是$X \times X$中的两个子集，则对$(x, y) \in X \times X$中的集合，使得对于一些$z \in X$，$(x, z) \in W$和$(z, y) \in V$由$V \circ W$或$VW$表示，并且对$(x, y) \in X \times X$的集合使得$(y, x) \in V$由$\overline{V}^1$表示。

例的均匀性。 \* 1) 在实数的集合 $\mathbf{R}$ 上，我们可以定义一个均匀性，称为*加性均匀性*，如下：对于每个 $\alpha > 0$ 令 $V_\alpha$ 为所有$\mathbf{R} \times \mathbf{R}$ 由……组成的子集对$(x, y)$使得$|x - y| < \alpha$；由于$\alpha$贯穿所有实数$> 0$中的集合，$V_\alpha$形式是$\mathbf{R}$上加法均匀性的基本系统。类似地，我们可以在有理数的集合$\mathbf{Q}$上实现定义均匀性（再次称为*加性均匀性*）；我们将研究这些结构，以及*群*上的类似制服结构、章III和IV。 \*
2) 令$X$为集合，并令$R$为$X$上的*等价关系*；设$C$为$R$在$X \times X$中的图。然后$\Delta \subset C$和$\overset{2}{C} = \overset{-1}{C} = C$； （*集合理论，R，§ 5, no. 1*）； $X \times X$的子集的集合仅由集合$C$组成，因此是$X$上均匀性的基本随行人员系统。特别是，如果我们将$R$视为等式的关系，那么$C = \Delta$和相应的一致性的随行人员是$X \times X$的*所有子集*，其中包含$\Delta$；这种均匀性被称为$X$上的*离散*均匀性，而赋予这种均匀性的集合$X$被称为*离散均匀性空间*。
3) 在有理整数的集合$\mathbf{Z}$上，我们可以得到定义的一致性，这在数的理论中很重要，如下：给定素数数$p$，令$W_n$为所有的集合对$(x, y) \in \mathbf{Z} \times \mathbf{Z}$使得$x \equiv y \pmod{p^n}$，对于每个整数$n > 0$。很容易验证集合$W_n$（对于固定的$p$）形式是$\mathbf{Z}$上均匀性的基本系统，称为*$p$-adic*均匀性（cf.章） III, § 6、习题 23 及章 IX, § 3, no. 2）。

根据一般定义（*集合理论，R，§ 8, no. 5*），如果$X$和$X'$是两个集合，每个集合都具有均匀性，其随行人员的集合是$U$和$U'$分别地，如果$g(U) = U'$，则$X$到$X'$的双射$f$是$X$到$X'$均匀性的*同构*，其中$g = f \times f$。

对于例，如果$X$和$X'$是两个等价的集合，则$X$的每一个双射到$X'$上都是$X$的离散均匀性的同构到$X'$。

### 2. 制服拓扑空间

#### 命题 1 {#top-ii-s1-prop-1 .statement tag=0BD3}

*令$X$为集合赋予统一的结构$U$，并且对于每个$x \in X$令$\mathfrak{B}(x)$为子集$V(x)$的集合或$X (*)$，其中$V$贯穿$U$随行人员集合。然后$X$上有一个唯一的拓扑，这样，对于每个$x \in X$，$\mathfrak{B}(x)$是拓扑中$x$的邻域过滤器。*

我们必须证明章 I, § 1, no. 2 的 $\mathfrak{B}(x)$ 满足条件 (V_I)、(V_{II})、(V_{III}) 和 (V_{IV})。前三个都是如此

(*) 我们回忆一下（*集合理论，R，§ 3, no. 7*），如果$V$是$X \times X$中的任何子集并且$x$是$X$中的任何元素，那么$V(x)$表示集合所有$y \in X$使得$(x, y) \in V$。

这些条件紧随$\mathfrak{U}$满足$(\mathbf{F}_I),\ (\mathbf{F}_{II})$和$(\mathbf{U}_I)$的随行人员。对于$(\mathbf{V}_{IV})$，令$V$为$\mathfrak{U}$的随从，$W$为$\mathfrak{U}$的随从，使得$\dot{W} \subset V$；那么如果$(x, y) \in W$和$(y, z) \in W$我们有$(x, z) \in V$，那么$W(y) \subset V(x)$对于所有$y \in W(x)$，因此$V(x) \in \mathfrak{B}(y)$对于所有$y \in W(x)$。这样就完成了证明。

#### 定义 3 {#top-ii-s1-def-3 .statement tag=0BD4}

* 命题 1 中定义的拓扑称为拓扑，由统一结构 $\mathfrak{U}$ 诱发。*

#### 例 1 {#top-ii-s1-n2-exa-1 .statement tag=0BD5}

由实数的集合上的加性均匀性引起的拓扑是实直线的拓扑（章I, § 1, no. 2）；类似地，由有理数的集合上的加性均匀性引起的拓扑是有理线的拓扑。*

#### 例 2 {#top-ii-s1-n2-exa-2 .statement tag=0BD6}

在任意集合 $X$、拓扑上，由离散均匀性 (no. 1、例 2) 引起的离散拓扑。

以后，当我们谈到制服空间$X$的拓扑时，我们总是指由空间制服结构引起的拓扑，除非则明确说明相反。将这个拓扑放在集合$X$上获得的拓扑空间是有时，称为拓扑空间*底层*所讨论的制服空间。对于例，当我们说一致的空间是*Hausdorff*，或*紧凑*，或*局部紧凑*等时，我们的意思是底层拓扑空间有这个性质。

如果$X$和$X'$是两个一致空间，则$X$的一致结构到$X'$的一致同构$f$也是$X$的*同胚* $X'$；我们说$X$是制服空间$X$到制服空间$X'$的*同构*。应该注意的是，$X$到$X'$的同胚不一定是$X$一致的结构到$X'$的同构。

在其他字中，相同集合$X$上的*不同*均匀性可以诱导相同的拓扑。 *对于例，在 ]0、+∞[ 上，*加法* 和 *乘法* 均匀性（不同：章 III, § 6、习题 17）诱导相同拓扑。*
对于另一个例，请参见 § 2, no. 2、注 1。

#### 命题 2 {#top-ii-s1-prop-2 .statement tag=0BD7}

*令$X$为制服空间。对于$X$的每个对称随行$V$和$X \times X$的每个子集$M$，$VMV$是乘积空间$X \times X$中$M$的邻域，并且闭包空间中的$M$由公式*给出

$$
\overline{M} = \bigcap_{V \in \mathscr{S}} VMV
$$

*其中 $\mathscr{S}$ 表示集合的对称随行人员 $X$。*

设$V$是$X$的对称周边。 关系$(x, y) \in VMV$表示$M$有元素$(p, q)$使得$(x, p) \in V$和$(q, y) \in V$：在其他字（$V$对称）$x \in V(p)$和$y \in V(q)$，是$(x, y) \in V(p) \times V(q)$。由于$V(p) \times X(q)$是$X \times X$中$(p, q)$的邻域，因此证明了命题的第一个部分。 关系$(x, p) \in V, (y, q) \in V$也可以写成$p \in V(x), q \in V(y)$或$(p, q) \in V(x) \times V(y)$。由于$V$贯穿$\mathscr{S}$，集合$V(x) \times V(y)$形式是$X \times X$中$(x, y)$的邻域的基本系统；因为如果$U, U'$是任意两个随行人员，则总有一个对称的随行人员$V \subset U \cap U'$，因此$V(x) \times V(y) \subset U(x) \times U'(y)$。因此，对于每个 $V \in \mathscr{S}$，$V(x) \times V(y)$ 满足 $M$ 当且仅当 $(x, y) \in \overline{M}$，且公式 (1) 成立。

#### 推论 1 {#top-ii-s1-prop-2-cor-1 .statement tag=0BD8}

*如果$A$是$X$的任意子集且$V$是$X$的任意对称周边，则$V(A)$是$X$中$A$的邻域，并且*

$$
\overline{A} = \bigcap_{V \in \mathscr{S}} V(A) = \bigcap_{U \in \mathfrak{U}} V(A)
$$

*其中 $\mathfrak{U}$ 表示 $X$ 中所有随行人员的集合。*

如果$M = A \times A$，则对于任意$V \in \mathscr{S}$，$VMV = V(A) \times V(A)$；对于关系“存在$p \in A$使得$(x, p) \in V$”通过定义等价于$x \in V(A)$。现在推论来自章 I, § 4, no. 2、命题 5 和 no. 3、命题 7。

据说$V(A)$是*$A$的*V邻域。

如果$V$是在$X \times X$中*开放*的随行人员，则对于每个$x \in X$，$V(x)$在$X$中开放（章I, § 4, no. 2，命题4的推论），因而$V(A)$，是并 $V(x)$ 因为$x$ 贯穿$A$，在$X$ 中*开放*。另一方面，如果$V$是$X \times X$中的封闭随行体，则对于$X$（习题3）的每个子集$A$，$V(A)$不需要在$X$中封闭。

还应该注意的是，由于$V$贯穿$X$随行人员的集合，集合$V(A)$不一定是形式$X$中$A$的邻域的基本系统 （习题2）。

#### 推论 2 {#top-ii-s1-prop-2-cor-2 .statement tag=0BD9}

*$X$随行人员在$X \times X$形式的内部装饰（或关闭），以及$X$随行人员的基本系统。*

如果 $V$ 是 $X$ 的任意随缘，则存在对称随缘 $W$，使得 $W \subset V$；由于$W$是$W$（命题2）的邻域，$V$的内部在$X \times X$包含$W$中，因此是一个随行人员。此外，我们有 $W \subset W \subset W \subset V$ 乘命题 2，因而 $V$ 包含随行人员结束。

#### 推论 3 {#top-ii-s1-prop-2-cor-3 .statement tag=0BDA}

*每件制服空间满足公理*$(O_{III})$。

如果$x$是$X$中的任意一个点，并且$V$穿过在$X \times X$关闭的$X$的随行人员，则集合$V(x)$形式是系统的基本系统根据推论 2，$X$ 中的 $x$ 的邻域，并且它们在 $X$ 关闭（章 I, , no. 2，推论到命题 4）

#### 命题 3 {#top-ii-s1-prop-3 .statement tag=0BDB}

*制服空间$X$是Hausdorff当且仅当其制服结构的所有随从中的交是$X \times X$的对角线$\Delta$。每件 Hausdorff 制服空间都是常规的。*

后者叙述紧随推论3到命题2。我们已经看到，封闭的随行人员形式是随行人员的基本系统（命题2，推论2）；如果它们的交是$\Delta$，那么$\Delta$在$X \times X$闭合，因而$X$是豪斯多夫（章I, § 8, no. 1，命题1）。相反，如果$X$是Hausdorff，那么对于每个点$(x, y) \notin \Delta$，都有一个$X$的随从$V$，使得$y \notin V(x)$，或等效的$(x, y) \notin V$；因而，$\Delta$ 是所有随行人员的交。

如果制服空间$X$是Hausdorff，我们说$X$的制服结构是*Hausdorff*。如果$\mathfrak{B}$是这个结构的基本随从系统；那么 $X$ 是 Hausdorff 当且仅当 $\mathfrak{B}$ 的所有集合中的交是 $\Delta$。

### 习题 {#top-ii-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
