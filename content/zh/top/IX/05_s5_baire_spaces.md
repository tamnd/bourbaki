---
book: top
book_title: General Topology
chapter: IX
chapter_title: Use of real numbers in general topology
section: 5
section_title: Baire spaces
lang: zh
source: top-v-x
pdf_pages: 0196-0201, 0256-0264
extraction: ocr
subsections:
    - "no": 1
      title: NOWHERE DENSE SETS
      page: 0
      pdf_page: 196
    - "no": 2
      title: MEAGRE SETS
      page: 0
      pdf_page: 198
    - "no": 3
      title: BAIRE SPACES
      page: 0
      pdf_page: 198
    - "no": 4
      title: SEMI-CONTINUOUS FUNCTIONS ON A BAIRE SPACE
      page: 0
      pdf_page: 200
statements: 16
exercises: 30
content_sha256: d3f463a6dcbe876f1e32c75cc25b13c7a4036c9195c4e6a5a170988e5a44876c
translated_from: content/en/top/IX/05_s5_baire_spaces.md
translation_method: google
source_content_sha256: 3b572897191a59b0bea951cffb8413b1fee09841bf812d8d9ace5e683fa0e3ca
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 5a4d72764001184943c30d880b316c4584d6d7514efc91cff3ca5e8d2623994d
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 5. 巴伊尔空间

### 1. 无处密集集合

#### 定义 1 {#top-ix-s5-def-1 .statement tag=0C6Y}

*如果拓扑空间$X$的子集$A$闭包没有内部点，则据说它是无处稠密的。*

等价地，当且仅当$A$的外部在$X$中稠密时，$A$在$X$中不稠密。

一个封闭的集合 $A$ 是无处稠密的当且仅当它没有内部点；也就是说，当且仅当它与其边界重合。任意子集$A$无处稠密当且仅当$A$的闭包无处稠密。无处稠密集合的每个子集都无处稠密。

#### 例 1 {#top-ix-s5-n1-exa-1 .statement tag=0C6Z}

$X$ 的空子集没有任何地方稠密。在 Hausdorff 空间 $X$ 中，单个点的集合由……组成不是稠密的，当且仅当点在 $X$ 中不是孤立的。稠密的子集永远不会无处稠密 (除非 $X = \emptyset$)。

#### 例 2 {#top-ix-s5-n1-exa-2 .statement tag=0C70}

开放或封闭集合的边界总是不密集的。

#### 例 3 {#top-ix-s5-n1-exa-3 .statement tag=0C71}

在空间$\mathbf{R}^n$中，维数$p < n$的每个线性子空间都是无处稠密集合（章VI, § 1, no. 4，命题2）。

#### 注 {#top-ix-s5-n1-rem-1 .statement tag=0C72}

任意子集的边界不必是无处稠密的：对于例，如果$A$和$\overline{C}A$都是稠密的集合，则$A$的边界是整个空间。

#### 命题 1 {#top-ix-s5-prop-1 .statement tag=0C73}

*The union of a finite number of nowhere dense sets is nowhere dense.*

足以证明两个无处稠密集合$A, B$的并无处稠密，并且不失一般性，我们可以假设$A$和$B$是闭集。 命题则相当于两个密开集合$\overline{C}A, \overline{C}B$的交密的说。现在，如果 $U$ 是非空开集合，则 $U \cap \overline{C}A$ 是开且非空，因此

$$
(U \cap \overline{C}A) \cap \overline{C}B = U \cap (\overline{C}A \cap \overline{C}B)
$$

是开放且非空的。

设$Y$为拓扑空间$X$的子空间。如果 $A$ 在被视为拓扑空间 $Y$ 的子集时不稠密，则 $Y$ 的子空间 $A$ 被认为是*相对于* $Y$ 来说是*不稠密的。

#### 命题 2 {#top-ix-s5-prop-2 .statement tag=0C74}

*设$Y$为拓扑空间$X$的子空间，并令$A$为$Y$的子集。如果 $A$ 相对于 $Y$ 不稠密，那么 $A$ 相对于 $X$ 也不稠密。相反，如果 $Y$ 在 $X$ 中开，且 $A$ 相对于 $X$ 不稠密，则 $A$ 相对于 $Y$ 不稠密。*

假设 $A$ 相对于 $Y$ 来说并不稠密。如果$X$包含中$A$的闭包$\overline{A}$是一个非空开集合$U$，则$U \cap A$不为空（通过闭包的定义）；因此$U \cap Y$是相对于$Y$的非空开集合，并且包含在$A$相对于$Y$的闭包$\overline{A} \cap Y$中，这与假设相反。

现在假设$Y$在$X$中开，并且$A \subset Y$相对于$X$来说并不稠密。如果 $U$ 在 $Y$ 中开且不为空，则 $U$ 在 $X$ 中开，因此包含是一个非空集合 $V$，它在 $X$ 中开（以及 $Y$ 中的 *更不必说*）并且不满足$A$；因此$A$相对于$Y$来说并不稠密。

如果$Y$未在$X$中打开，则命题2的第二个部分显然无效；例如，考虑$Y \neq \emptyset$在$X$和$A = Y$中不稠密的情况。

### 2. 微薄集合

#### 定义 2 {#top-ix-s5-def-2 .statement tag=0C75}

*子集* $A$ *拓扑空间* $X$ *如果它是无处稠密的可数族并，则据说是贫乏的集合。*

Equivalently, $A$ is meagre if it is contained in a countable union of closed sets each of which has no interior points.

微薄的集合完全可以在 $X$ 中“密集”；甚至整个空间$X$本身也可以是微薄的集合。

后一种可能性的例由任何*可数*Hausdorff空间提供，没有孤立的点，例如有理线$\mathbf{Q}$。但是拓扑空间 $X$ 是 $X$ 中微不足道的集合 ，它不必是可数的（参见习题 9）。

Every subset of a meagre set in a space $X$ is meagre, and the union of a *countable* family of meagre sets is meagre.

设$Y$为$X$的子空间。如果 $A$ 当被视为拓扑空间 $Y$ 的子集时是微不足道的，则 $Y$ 的子集 $A$ 被称为“相对于* $Y$ 微不足道”。由no. 1的命题2得出，如果$A$是$Y$的子集，相对于$Y$是微薄的，那么$A$相对于$X$是微薄的；如果$Y$也在$X$中*开*，则$Y$的每个子集$A$（相对于$X$微薄）相对于$Y$微薄。

### 3. 巴伊尔空间

#### 定义 3 {#top-ix-s5-def-3 .statement tag=0C76}

*拓扑空间* $X$ *如果满足以下两个等价条件中的一个或另一个，则称为贝尔空间：*

*(EB)* *在* $X$ *中稠密开集合的每个可数交在* $X$中稠密。
*(EB')* *闭合集合的每个可数并，在* $X$ 中没有内部点 *在* $X$ 中没有内部点。

公理 (EB) 可以用另外两个等价形式来表示：

*(EB'')* ** $X$ 中的每个非空开集合 *都是非微薄的。*

事实上，当且仅当集合包含在没有内部点的封闭集合的可数并中时，集合才是微不足道的。

(EB'') *$X$中微薄的集合的补集在$X$中是稠密的。*

这表示微薄的集合不能包含是一个非空开集合，因此等价于 (EB")。

#### 命题 3 {#top-ix-s5-prop-3 .statement tag=0C77}

*Baire 空间 $X$ 的每个非空开子空间 $Y$ 都是Baire 空间。*

这是从 (EB") 得出的，对于 $Y$ 中的每个开路（分别为微量）集合在 $X$ 中都是开路（分别为微量）。

从命题 3 可以得出，Baire 空间的每个点都有一个邻域的基本系统，每个空间都是一个Baire 空间。反过来：

#### 命题 4 {#top-ix-s5-prop-4 .statement tag=0C78}

*如果拓扑空间$X$的每个点都有邻域，即Baire空间，则$X$是Baire空间。*

令$A$为$X$中的非空开集合，令$x \in A$并令$V$为$x$的开邻域，即Baire空间。如果$A$在$X$中微薄，那么$V \cap A$在$V$中微薄而在$V$中开放，这与假设相反。

#### 命题 5 {#top-ix-s5-prop-5 .statement tag=0C79}

*在 Baire 空间 $X$ 中，微薄的集合的补码是 Baire 空间。*

令$A$为$X$中微薄的集合；那么它在$X$中的补集$Y = \complement_A$在$X$中是稠密的。令$B$相对于$Y$来说是微不足道的集合； $B$ 相对于 $X$ 来说也微不足道，因此 $A \cup B$ 相对于 $X$ 来说微不足道。因此，$X$中$A \cup B$的补集，也是$Y$中$B$的补集，在$X$中是稠密的，并且在$Y$中是*更不必说*稠密的。因此 $Y$ 是 Baire 空间。

#### 定理 1（贝尔）{#top-ix-s5-thm-1 .statement tag=0C7A}

(i) *每个局部紧凑空间$X$都是Baire空间。* (ii) *每个拓扑空间$X$存在一个度量，与$X$的拓扑兼容并且定义在完整的$X$结构上公制空间，是贝尔空间。*

我们将证明在每种情况下都满足公理（EB）。 令$(A_n)$为$X$中密集开集合的序列，并令$G$为任意非空开集合。 然后我们可以归纳非空开集合的定义序列$(G_n)$使得$G_1 = G$和$\overline{G}_{n+1} \subset G_n \cap A_n$：因为从假设$G_n$不为空，$G_n \cap A_n$是非空开集合；并且由于 $X$ 在所设想的两种情况下都是“常规”，因此存在一个非空开集合 $G_{n+1}$，使得 $\overline{G}_{n+1} \subset G_n \cap A_n$。 因此，集合$G_n$的集合$G \cap \bigcap_{n=1}^\infty A_n$包含交，等于集合$\overline{G}_n$的交；因此只要证明$\bigcap_{n=1}^\infty \overline{G}_n \neq \varnothing$就足够了。 现在，如果$X$是局部紧致的，我们可以假设$\overline{G}_2$是紧致的；在紧凑空间 $\overline{G}_2$ 中，非空封闭集合的 $\overline{G}_n (n \geq 2)$ 形式递减序列，因此根据公理 (C'')，它们的交不为空 (cf. 章 I, § 9, no. 1， 定义1]。 If $X$ is a complete metric space (with respect to a metric compatible with its topology) we may suppose that $\overline{G}_n$ has been chosen so that its diameter (with respect to this metric) tends to 0 as $n$ tends to $+\infty$; the $\overline{G}_n$ therefore form a Cauchy filter base which converges to a point $x$, and $x$ necessarily belongs to the intersection of the sets $\overline{G}_n$.

Q.E.D.

#### 注 {#top-ix-s5-n3-rem-1 .statement tag=0C7B}

存在 Baire 空间，而属于既不属于这两个类别，特别是 Baire 空间，它既不可度量，也不局部紧凑 (习题 16)；还有可度量的 Baire 空间，它们没有与其拓扑 (习题 14) 兼容的完整度量空间结构。

### 4. 半连续函数在 BAIRE 空间

#### 定理 2 {#top-ix-s5-thm-2 .statement tag=0C7C}

令$X$为贝尔空间，并让$(f_\alpha)$为$X$上的下半连续实值族函数，这样，在$X$的每个点$x$，上包络$\sup_\alpha f_\alpha(x)$是有限的。然后，$X$包含中的每个非空开集合都是一个非空开集合，族$(f_\alpha)$统一有界于其上。

这个定理也可以在形式中表示，邻域中点的集合（其中族$(f_\alpha)$均匀有界于其上）是密集开集合。

令$f = \sup_\alpha f_\alpha$为家庭$(f_\alpha)$的上层信封。 函数 $f$ 是下半连续 (章 IV, § 6, no. 2, 定理 4)，并且在 $X$ 的每点处有限。因此，在家庭 $(f_\alpha)$ 由单个函数 $f$ 组成的情况下，进行证明就足够了。令$A_n$为点$x \in X$中的集合，使得$f(x) \leq n$； $A_n$是闭集（章IV, § 6, no. 2，命题1），假设意味着$X$是集合$A_n$的并；因此，至少其中一个 $A_n$ 具有内部点，因此存在一个非空开集合，其上有 $f$ 边界（由整数 $n$）。如果我们将此结果应用于$X$的任何非空开子集（这个子空间也是no. 3的命题 3的贝尔空间），我们有定理。

在定理的应用中，通常情况是$f_\alpha$在$X$上连续。

#### 注 {#top-ix-s5-n4-rem-1 .statement tag=0C7D}

如果我们不假设 $X$ 是 Baire 空间，定理可能是假的。对于例，如果对于每个有理数数$p/q$（$p, q$互质整数，$q > 0$）我们放置$f(p/q) = q$，我们在有理数线$Q$上有一个下半连续函数$f$在每个点 (cf. 章 IV, § 6, no. 2) 处都是有限的；但$Q$中不存在非空开集合，$f$在其上有界。

### 习题{#top-ix-s5-exercises}

参见[习题为 § 5](exercises/s5/)。
