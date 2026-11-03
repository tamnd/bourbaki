---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THEORY OF SETS
section: 4
section_title: Union and intersection of a family of sets
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 90-101, 125-126
pdf_pages: 0097-0108, 0132-0133
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF THE UNION AND THE INTERSECTION OF A FAMILY OF SETS
      page: 90
      pdf_page: 97
    - "no": 2
      title: PROPERTIES OF UNION AND INTERSECTION
      page: 93
      pdf_page: 100
    - "no": 3
      title: IMAGES OF A UNION AND AN INTERSECTION
      page: 94
      pdf_page: 101
    - "no": 4
      title: COMPLEMENTS OF UNIONS AND INTERSECTIONS
      page: 96
      pdf_page: 103
    - "no": 5
      title: UNION AND INTERSECTION OF TWO SETS
      page: 96
      pdf_page: 103
    - "no": 6
      title: COVERINGS
      page: 98
      pdf_page: 105
    - "no": 7
      title: PARTITIONS
      page: 99
      pdf_page: 106
    - "no": 8
      title: SUM OF A FAMILY OF SETS
      page: 100
      pdf_page: 107
statements: 22
exercises: 8
content_sha256: b39f6c6abb88c1d3ac615ce60ab209c51129e67449dcd1907e28a27dcf1b7e48
translated_from: content/en/ens/II/04_s4_union_and_intersection_of_a_family_of.md
translation_method: google
source_content_sha256: 79a8f1cdc57e7dce0167dd11f3e335382fe0479c90c58a053fba7bbc5d06a5f5
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: dfb1370039f84c618d05d285108a1750f751c045bb9ebdb13d133bec9f7a2d68
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 4. 集合家庭的并和交

### 1. 集合家庭的并和交的定义

让X是一个家庭（§3, no. 4），I是指标集合。为了帮助直观地解释以下内容，我们将X称为*集合*家族。如果$(\mathrm{X}, \mathrm{I}, \mathfrak{G})$是集合* E的子集的*族（即，目标$\mathfrak{G}$使得关系$\mathrm{Y} \in \mathfrak{G}$暗示$\mathrm{Y} \subset \mathrm{E}$的族），我们将用$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}(\mathrm{X}_\iota \in \mathfrak{G})$或简单地用$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$来表示该族（§3, no. 6）；通过滥用记号，我们将用$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$来表示任何集合的家族，其中I作为其指标集合。

¶ 由于关系 $(\forall x)((\iota \in \mathrm{I}$ 和 $x \in \mathrm{X}_\iota) \Rightarrow (x \in \mathrm{X}_\iota))$ 为真，因此从 S5 (章 I, §4，无 2。) 关系

$$(\forall \iota)(\exists \mathrm{Z})(\forall x)((\iota \in \mathrm{I} \text{ and } x \in \mathrm{X}_\iota) \Rightarrow (x \in \mathrm{Z}))$$

是真的。凭借概形 S8 (§1, no. 6) 关系 $(\exists \iota)(\iota \in \mathrm{I}$ 和$x \in \mathrm{X}_\iota)$ 是$x$* 中的*集合化。

#### 定义 1 {#ens-ii-s4-def-1 .statement tag=03I1}

*令$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$为集合*的家族（分别为*集合* E的子集家族）。 *集合$\mathscr{E}_x((\exists \iota)(\iota \in \mathrm{I}$和$x \in \mathrm{X}_\iota))$，也就是说，所有$x$*中的集合*其中属于到家庭$(X_l)_{l\in I}$中至少一个集合，被称为家庭的并，并表示为*
$$\bigcup_{l\in I}X_l,$$[^1]

如果$(X_l)_{l\in I}$是集合$E$的子集族，那么它的并就是$E$的子集；请注意，它不依赖于 $E$，也不依赖于映射 $l\to X_l$ 的目标 $\mathfrak{G}$。

很明显，如果$I=\varnothing$，我们有$\displaystyle\bigcup_{l\in I}X_l=\varnothing$，因为关系$(\exists l)(l\in I\text{ and }x\in X_l)$则为假。

¶ 现在假设 $I\neq\varnothing$。如果$\alpha$是$I$中的元素，则关系
$$ (\forall l)((l\in I)\Longrightarrow(x\in X_l)) $$
意味着$x\in X_\alpha$，因此，根据 C52 (§1, no. 6)，这个关系是$x$中的*集合化。*

#### 定义 2 {#ens-ii-s4-def-2 .statement tag=03PT}

*令$(X_l)_{l\in I}$为集合的一个族，其指标集合$I$不为空。 集合 $\mathscr{E}_x((\forall l)((l\in I)\Longrightarrow(x\in X_l)))$，也就是说，所有$x$中的集合，其中属于到家庭$(X_l)_{l\in I}$的每个集合，称为家庭的交，并用*表示
$$\bigcap_{l\in I}X_l.$$

如果$I=\varnothing$，关系$(\forall l)((l\in I)\Longrightarrow(x\in X_l))$不是$x$中的集合化；因为它是一个真正的关系，并且不存在集合$Y$使得$x\in Y$是一个真正的关系，因为$Y$将是所有对象中的集合（cf.§1, no. 7， 注）。

如果$(X_l)_{l\in I}$是集合$E$的子集族，并且如果$I\neq\varnothing$，关系“$x\in E$和$(\forall l)((l\in I)\Longrightarrow(x\in X_l))$”相当于
$$ (\forall l)((l\in I)\Longrightarrow(x\in X_l)); $$
因此它是$x$中的集合化，以及所有$x$中的集合，其中满足这个关系等于$\displaystyle\bigcap_{l\in I}X_l$。如果$I=\varnothing$、关系“$x\in E$和$(\forall l)((l\in I)\Longrightarrow(x\in X_l))$”等价于$x\in E$；因而，$x$中有集合化，所有$x$中的集合，其中满足这个关系是$E$。因此我们可以声明以下定义：

#### 定义 3 {#ens-ii-s4-def-3 .statement tag=03PU}

*设$(X_l)_{l\in I}$是子集和集合$E$的一个家庭。 集合*
$$\mathscr{E}_x\left(x\in E\text{ and }(\forall l)((l\in I)\Longrightarrow(x\in X_l))\right),$$

*在所有$x$中的其他字、集合，其中属于到* E *以及每个集合* $X_\iota$，*被称为家族的交，并用*$\bigcap\limits_{\iota \in I} X_\iota$表示。

因而，对于 E 的 $(X_\iota)_{\iota \in \emptyset}$ 子集族，我们有

$$\bigcap_{\iota \in \emptyset} X_\iota = E.$$

但对于E的子集的$(X_\iota)_{\iota \in I}$族，其指标集合不为空，交$\bigcap\limits_{\iota \in I} X_\iota$既不依赖于E，也不依赖于$\iota \rightarrow X_\iota$的目标；这证明了在定义 2 和 3 中使用相同的记号是合理的。

#### 命题 1 {#ens-ii-s4-prop-1 .statement tag=03PV}

*设*$(X_\iota)_{\iota \in I}$*为集合的一个家庭，并让$f$为集合*K的映射*I。 *然后*

$$\bigcup_{\varkappa \in K} X_{f(\varkappa)} = \bigcup_{\iota \in I} X_\iota,$$

*并且，如果*$I \neq \emptyset$，

$$\bigcap_{\varkappa \in K} X_{f(\varkappa)} = \bigcap_{\iota \in I} X_\iota.$$

设$x$为$\bigcap\limits_{\iota \in I} X_\iota$的元素。存在指标$\iota \in I$使得$x \in X_\iota$。由于$f\langle K \rangle = I$，存在指标$\varkappa \in K$使得$\iota = f(\varkappa)$，从而$x \in X_{f(\varkappa)}$因而

$$x \in \bigcup_{\varkappa \in K} X_{f(\varkappa)}.$$

相反，如果$x \in \bigcup\limits_{\varkappa \in K} X_{f(\varkappa)}$，则存在$\varkappa \in K$使得$x \in X_{f(\varkappa)}$，因而，从$f(\varkappa) \in I$开始，$x \in \bigcup\limits_{\iota \in I} X_\iota$。因而

$$\bigcup_{\varkappa \in K} X_{f(\varkappa)} = \bigcup_{\iota \in I} X_\iota.$$

¶ 现在假设 $I \neq \emptyset$，并令 $x$ 为 $\bigcap\limits_{\iota \in I} X_\iota$ 的元素。对于 K 的每个元素 $\varkappa$，我们有 $f(\varkappa) \in I$，因此有 $x \in X_{f(\varkappa)}$，因而

$$x \in \bigcap_{\varkappa \in K} X_{f(\varkappa)}.$$

相反，令$x$为$\bigcap\limits_{\varkappa \in K} X_{f(\varkappa)}$的元素。如果$\iota$是I中的任意元素，则存在K的元素$\varkappa$，使得$\iota = f(\varkappa)$、从而$x \in X_\iota$，因而$x \in \bigcap_{\iota \in I} X_\iota$。因而

$$\bigcap_{\varkappa \in K} X_{f(\varkappa)} = \bigcap_{\iota \in I} X_\iota.$$

对于给定集合的子集的家庭，很明显，命题 1 的第二个部分在没有限制 $I \neq \emptyset$ 的情况下仍然有效。

#### 推论 {#ens-ii-s4-n1-cor-1 .statement tag=03I2}

*让*$(X_\iota)_{\iota \in I}$*成为集合的一个家庭，使得*$X_\iota = X_\varkappa$*对于指标*$(\iota, \varkappa)$中的每个对。 *然后对于每个* $\alpha \in I$ *我们有*

$$\bigcup_{\iota \in I} X_\iota = X_\alpha, \qquad \textit{and (if } I \neq \emptyset) \qquad \bigcap_{\iota \in I} X_\iota = X_\alpha.$$

应用命题 1 到I 的常数映射 $\iota \to \alpha$ 到$\{\alpha\}$。

#### 定义 4 {#ens-ii-s4-def-4 .statement tag=03I3}

*设*$\mathfrak{F}$*为集合的集合，并让*$\Phi$*为由*$\mathfrak{F}$的恒等映射定义的集合族。 * $\Phi$ * 的集合 * 并和（如果 * $\mathfrak{F}$ * 不为空） * $\Phi$ * 的集合交分别称为 * 并 * 和 * 交 * * $\mathfrak{F}$的集合，*和由*$\bigcup_{X \in \mathfrak{F}} X$*和*$\bigcap_{X \in \mathfrak{F}} X$表示。

如果紧接命题 1，如果$(X_\iota)_{\iota \in I}$是集合的族，则该族的并和（如果$I \neq \emptyset$）交分别等于集合的并和交这个家的元素集合。

### 2. 并和交的性质

如果$(X_\iota)_{\iota \in I}$和$(Y_\iota)_{\iota \in I}$是集合的族，具有相同的指标集合I，并且如果每个$\iota \in I$都有$Y_\iota \subset X_\iota$，那么很明显

$$\bigcup_{\iota \in I} Y_\iota \subset \bigcup_{\iota \in I} X_\iota, \qquad \text{and (if } I \neq \emptyset) \qquad \bigcap_{\iota \in I} Y_\iota \subset \bigcap_{\iota \in I} X_\iota.$$

¶ 令$(X_\iota)_{\iota \in I}$ 成为集合的一个家庭。如果$J \subset I$，我们有

$$\bigcup_{\iota \in J} X_\iota \subset \bigcup_{\iota \in I} X_\iota, \qquad \text{and (if } J \neq \emptyset) \qquad \bigcap_{\iota \in J} X_\iota \supset \bigcap_{\iota \in I} X_\iota.$$

#### 命题 2 {#ens-ii-s4-prop-2 .statement tag=03I4}

*设*$(X_\iota)_{\iota \in I}$*是集合的一个家庭，其指标集合*I*是并的一个家庭*$(J_\lambda)_{\lambda \in L}$*的集合。然后*

$$\bigcup_{\iota \in I} X_\iota = \bigcup_{\lambda \in L} \left( \bigcup_{\iota \in J_\lambda} X_\iota \right),$$

*和*（*如果* $L \neq \emptyset$ 和 $J_\lambda \neq \emptyset$ *对于每个* $\lambda \in L$）

$$\bigcap_{\iota \in I} X_\iota = \bigcap_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_\iota \right)$$

（并和交的“结合性”）。

令$x$为$\bigcup_{\iota \in I} X_\iota$的元素。存在指标$\iota \in I$使得$x \in X_\iota$。由于I是$(J_\lambda)_{\lambda \in L}$族的并，因此存在指标$\lambda \in L$使得$\iota \in J_\lambda$，从而$x \in \bigcup_{\iota \in J_\lambda} X_\iota$，因而

$$x \in \bigcup_{\lambda \in L} \left( \bigcup_{\iota \in J_\lambda} X_\iota \right).$$

相反，令$x$为这个集合的元素。存在指标$\lambda \in L$使得$x \in \bigcup_{\iota \in J_\lambda} X_\iota$，因此存在指标$\iota \in J_\lambda$（因此存在$\iota \in I$）使得$x \in X_\iota$；由此可见

$$x \in \bigcup_{\iota \in I} X_\iota.$$

现在假设每个$\lambda \in L$都有$L \neq \emptyset$和$J_\lambda \neq \emptyset$。然后$I \neq \emptyset$。令$x$为$\bigcap_{\iota \in I} X_\iota$的元素。如果$\lambda \in L$，则每个$\iota \in J_\lambda$有$x \in X_\iota$（从$J_\lambda \subset I$开始），从而$x \in \bigcap_{\iota \in J_\lambda} X_\iota$。由于最后一个包含对于所有 $\lambda \in L$、$x$ 属于到 $\bigcap_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_\iota \right)$ 都是正确的。相反，令$x$为后者集合的元素，并令$\iota$为I的任意元素。存在$\lambda \in L$使得$\iota \in J_\lambda$；从 $x \in \bigcap_{\iota \in J_\lambda} X_\iota$ 开始，我们就有了 $x \in X_\iota$，这对于所有 $\iota \in I$ 都是如此。因而$x \in \bigcap_{\iota \in I} X_\iota$。这样就完成了证明。

对于给定集合的子集家庭，命题 2 中的第二个部分仍然有效，在 L 和 $J_\lambda$ 上没有限制。

### 3. 并与交的像

#### 命题 3 {#ens-ii-s4-prop-3 .statement tag=03I5}

*设*$(X_\iota)_{\iota \in I}$*是集合*A的子集的一个家庭，*并且让*$\Gamma$*是在*A*和*B之间的对应。*然后*

$$\Gamma \left\langle \bigcup_{\iota \in I} X_\iota \right\rangle = \bigcup_{\iota \in I} \Gamma \langle X_\iota \rangle, \qquad \Gamma \left\langle \bigcap_{\iota \in I} X_\iota \right\rangle \subset \bigcap_{\iota \in I} \Gamma \langle X_\iota \rangle.$$

关系 $(\exists x)\left(x \in \bigcup_{\iota \in I} X_\iota \text{ and } y \in \Gamma(x)\right)$ 相当于

$$(\exists x)(\exists \iota)(\iota \in I \text{ and } x \in X_\iota \text{ and } y \in \Gamma(x)),$$

因此为 $(\exists \iota)(\iota \in I$ 和 $y \in \Gamma\langle X_\iota \rangle)$，因此相当于 $y \in \bigcup_{\iota \in I} \Gamma\langle X_\iota \rangle$；这就证明了第一个公式。至于第二个公式，我们对所有$\iota \in I$，从而有$\bigcap_{\iota \in I} X_\iota \subset X_\iota$（§3，命题2）

$$\Gamma\left\langle \bigcap_{\iota \in I} X_\iota \right\rangle \subset \Gamma\langle X_\iota \rangle,$$

因而

$$\Gamma\left\langle \bigcap_{\iota \in I} X_\iota \right\rangle \subset \bigcap_{\iota \in I} \Gamma\langle X_\iota \rangle.$$

¶ 如果 $\Gamma$ 是任意对应 （特别是任意函数），则公式

$$\Gamma\left\langle \bigcap_{\iota \in I} X_\iota \right\rangle = \bigcap_{\iota \in I} \Gamma\langle X_\iota \rangle$$

通常是*假*。

\* 例如，在平面$\mathbf{R}^2$中，$y = x$和$y = x + 1$行中的第一个投影等于$\mathbf{R}$，但这些行中的交是空的，因此交[^2]的第一个投影也是空的。 \*

然而，我们有以下重要结果：

#### 命题 4 {#ens-ii-s4-prop-4 .statement tag=03I6}

*设$f$是*A*的映射*进入*B*并让*$(Y_\iota)_{\iota \in I}$*成为*B的子集的一个家庭。*然后*$\overset{-1}{f}\left\langle \bigcap_{\iota \in I} Y_\iota \right\rangle = \bigcap_{\iota \in I} \overset{-1}{f}\langle Y_\iota \rangle.$

为了证明这一点，令 $x$ 为 $\bigcap_{\iota \in I} \overset{-1}{f}\langle Y_\iota \rangle$ 的元素。我们对所有 $\iota \in I$、从而 $f(x) \in \bigcap_{\iota \in I} Y_\iota$ 有 $f(x) \in Y_\iota$，因而

$$x \in \overset{-1}{f}\left\langle \bigcap_{\iota \in I} Y_\iota \right\rangle.$$

因而$\bigcap_{\iota \in I} \overset{-1}{f}(Y_\iota) \subset \overset{-1}{f}\left\langle \bigcap_{\iota \in I} Y_\iota \right\rangle$；这个关系与命题 3 一起给出结果。

#### 推论 {#ens-ii-s4-n3-cor-1 .statement tag=03I7}

*如果$f$是* A *的单射*进入* B *并且如果* $(X_\iota)_{\iota \in I}$ *是* A *的子集的一个家庭，其指标集合* I *不为空，则* $f\left\langle \bigcap_{\iota \in I} X_\iota \right\rangle = \bigcap_{\iota \in I} f\langle X_\iota \rangle$。

因为我们可以将$f = i \circ g$，其中$i$是$f\langle A \rangle$的典范嵌入写入B，而$g$是A的双射写入$f\langle A \rangle$。如果 $h$ 表示 $g$ 的倒数映射，则对于 A 的每个子集 X，我们都有 $f\langle X \rangle = \overset{-1}{h}\langle X \rangle$，因此我们又回到命题 4。

### 4. 并和交的补集

#### 命题 5 {#ens-ii-s4-prop-5 .statement tag=03I8}

*对于每个家庭* $(X_\iota)_{\iota \in I}$ *集合* E 子集，*我们有*

$$\complement_E\left(\bigcup_{\iota \in I} X_\iota\right) = \bigcap_{\iota \in I} (\complement_E X_\iota), \qquad \complement_E\left(\bigcap_{\iota \in I} X_\iota\right) = \bigcup_{\iota \in I} (\complement_E X_\iota).$$

让$x \in \complement_E\left(\bigcup_{\iota \in I} X_\iota\right)$。然后$x \in E$，并且对于每个$\iota \in I$，$x \notin X_\iota$，从而$x \in \complement_E X_\iota$；因而

$$x \in \bigcap_{\iota \in I} (\complement_E X_\iota).$$

相反，令$x$为$\bigcap_{\iota \in I} (\complement_E X_\iota)$的元素；到定义或交为止，我们有 $x \in E$。此外，如果我们有$x \in \bigcup_{\iota \in I} X_\iota$，就会存在指标$\varkappa \in I$，使得$x \in X_\varkappa$，其中与……矛盾假设$x \in \bigcap_{\iota \in I} (\complement_E X_\iota)$；因而

$$x \in \complement_E\left(\bigcup_{\iota \in I} X_\iota\right).$$

这就证明了第一个公式；第二个是直接的推论，考虑到E的每子集X有关系$\complement_E(\complement_E X) = X$。

### 5. 两个集合中的并和交

如果 A, B 是集合，我们写

$$A \cup B = \bigcup_{X \in \{A, B\}} X, \qquad A \cap B = \bigcap_{X \in \{A, B\}} X.$$

很明显，$A \cup B$是所有对象中的集合，其中属于要么到$A$，要么到$B$（或者可能到两者），而$A \cap B$是所有对象中的集合，其中属于对两者$A$ 和 $B$。特别是$\{x, y\} = \{x\} \cup \{y\}$。

¶ 让$\{x, y, z\} = \{x, y\} \cup \{z\}$。 集合 $\{x, y, z\}$ 是集合，其元素仅有$x$、$y$ 和$z$。同样我们写

$$\{x, y, z, t\} = \{x, y, z\} \cup \{t\},$$

等等。

¶ 如果现在 $A$、$B$、$C$、$D$ 是集合，我们写

$$A \cup B \cup C = \bigcup_{X \in \{A,\, B,\, C\}} X, \qquad A \cap B \cap C = \bigcap_{X \in \{A,\, B,\, C\}} X;$$

$$A \cup B \cup C \cup D = \bigcup_{X \in \{A,\, B,\, C,\, D\}} X, \qquad A \cap B \cap C \cap D = \bigcap_{X \in \{A,\, B,\, C,\, D\}} X;$$

等等。

¶ 设 $A, B, C$ 为集合。从命题 1 和 2 我们推导出公式

$$A \cup B = B \cup A, \qquad A \cap B = B \cap A,$$
$$A \cup (B \cup C) = (A \cup B) \cup C = A \cup B \cup C,$$
$$A \cap (B \cap C) = (A \cap B) \cap C = A \cap B \cap C.$$

这些公式也是标准C24中规定的定理的直接的推论（章I, §3, no. 5）。同样证明公式

$$A \cup (B \cap C) = (A \cup B) \cap (A \cup C), \qquad A \cap (B \cup C) = (A \cap B) \cup (A \cap C)$$

（并超过交以及交超过并的“分配律”；cf.§5, no. 6）。

¶ 关系 $A \subset B$ 相当于 $A \cup B = B$ 和 $A \cap B = A$。如果$A$和$B$是集合$E$的子集，我们从命题5（或从标准C24）推出公式

$$\complement_E(A \cup B) = (\complement_E A) \cap (\complement_E B), \qquad \complement_E(A \cap B) = (\complement_E A) \cup (\complement_E B);$$

此外，我们还有

$$A \cup (\complement_E A) = E, \qquad A \cap (\complement_E A) = \emptyset.$$

¶ 如果$\Gamma$是$E$和$F$之间的对应，并且如果$A$、$B$是$E$的子集，则从命题 3得出：

$$\Gamma\langle A \cup B \rangle = \Gamma\langle A \rangle \cup \Gamma\langle B \rangle, \qquad \Gamma\langle A \cap B \rangle \subset \Gamma\langle A \rangle \cap \Gamma\langle B \rangle,$$

并且，如果 $f$ 是 F 到 E 的映射，

$$\overset{-1}{f}\langle \mathrm{A} \cap \mathrm{B} \rangle = \overset{-1}{f}\langle \mathrm{A} \rangle \cap \overset{-1}{f}\langle \mathrm{B} \rangle$$

从命题 4.

¶ 我们还在补语上记录以下命题 ：

#### 命题 6 {#ens-ii-s4-prop-6 .statement tag=03PW}

*设$f$是*A*到*B的映射。*对于*B的每个子集*Y*，*我们有*

$$\overset{-1}{f}\langle \mathrm{B} - \mathrm{Y} \rangle = \overset{-1}{f}\langle \mathrm{B} \rangle - \overset{-1}{f}\langle \mathrm{Y} \rangle.$$

对于$x$属于到$\overset{-1}{f}\langle \mathrm{B} - \mathrm{Y} \rangle$当且仅当$f(x)$属于到B但不到Y，即当且仅当$x$属于到$\overset{-1}{f}\ \langle \mathrm{B} \rangle$但不到$\overset{-1}{f}\ \langle \mathrm{Y} \rangle$。

#### 推论 {#ens-ii-s4-n5-cor-1 .statement tag=03PX}

*让$f$成为* A *到* B的单射。*对于* A的每个子集* X *，*我们有$f\langle \mathrm{A} - \mathrm{X} \rangle = f\langle \mathrm{A} \rangle - f\langle \mathrm{X} \rangle$。*

将$f = i \circ g$写入B，其中$i$是$f\langle \mathrm{A} \rangle$的典范嵌入，我们将约化推论到命题6应用到$\overset{-1}{g}$。

¶ 交 $\mathrm{X} \cap \mathrm{A}$ 被有时称为 A 上 X 的*踪迹*。如果 $\mathfrak{F}$ 是集合的族，则集合属于到 $\mathfrak{F}$ A 上踪迹的集合称为 A 上的*踪迹* A 上的$\mathfrak{F}$。

### 6. 覆盖物

#### 定义 5 {#ens-ii-s4-def-5 .statement tag=03PY}

*集合$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$的族据说是集合* E *（或覆盖* E）*如果$\mathrm{E} \subset \bigcup\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota$的覆盖。如果 $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ 和 $(\mathrm{Y}_\varkappa)_{\varkappa \in \mathrm{K}}$ 是* E 的覆盖，*这些覆盖中的第二个被认为比第一个覆盖更细（或者是第一个覆盖的精炼，或者精炼第一个），如果对于每个$\varkappa \in \mathrm{K}$，存在$\iota \in \mathrm{I}$使得*

$$\mathrm{Y}_\varkappa \subset \mathrm{X}_\iota.$$

如果$\mathfrak{R}$恒等映射定义的集合族是E的覆盖，换句话说，如果$\mathrm{E} \subset \bigcup\limits_{\mathrm{X} \in \mathfrak{R}} \mathrm{X}$，则集合$\mathfrak{R}$是E的覆盖。

如果$\mathfrak{R}$、$\mathfrak{R}'$、$\mathfrak{R}''$是E的三个覆盖，使得$\mathfrak{R}'$细化$\mathfrak{R}$且$\mathfrak{R}''$细化$\mathfrak{R}'$，则显然$\mathfrak{R}''$细化$\mathfrak{R}$。

设$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$是E的覆盖。如果J是I的子集，使得$(\mathrm{X}_\iota)_{\iota \in \mathrm{J}}$仍然是E的覆盖，那么这个覆盖显然细化了$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$。

¶ 设$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$和$(\mathrm{Y}_\varkappa)_{\varkappa \in \mathrm{K}}$是集合E的覆盖。那么集合$(\mathrm{X}_\iota \cap \mathrm{Y}_\varkappa)_{(\iota, \varkappa) \in \mathrm{I} \times \mathrm{K}}$的族是E的覆盖。因为如果$x \in \mathrm{E}$，则存在指标$\iota \in \mathrm{I}$和$\varkappa \in \mathrm{K}$使得$x \in \mathrm{X}_\iota$和$x \in \mathrm{Y}_\varkappa$，因此$x \in \mathrm{X}_\iota \cap \mathrm{Y}_\varkappa$ 此外，很明显，覆盖层$(\mathrm{X}_\iota \cap \mathrm{Y}_\varkappa)_{(\iota, \varkappa) \in \mathrm{I} \times \mathrm{K}}$细化了覆盖层$(X_\iota)_{\iota \in I}$、$(Y_\varkappa)_{\varkappa \in K}$。相反，令 $(Z_\lambda)_{\lambda \in L}$ 为 E 的覆盖，它细化了每个覆盖$(X_\iota)_{\iota \in I}$、$(Y_\varkappa)_{\varkappa \in K}$；如果$\lambda \in L$，则存在指标、$\iota \in I$和$\varkappa \in K$，使得$Z_\lambda \subset X_\iota$和$Z_\lambda \subset Y_\varkappa$，从而$Z_\lambda \subset X_\iota \cap Y_\varkappa$；因此覆盖$(Z_\lambda)_{\lambda \in L}$是对

$$(X_\iota \cap Y_\varkappa)_{(\iota, \varkappa) \in I \times K}.$$

¶ 设 $(X_\iota)_{\iota \in I}$ 为集合 A 的覆盖，并设 $f$ 为 A *到* 集合 B 的映射。则族 $(f\langle X_\iota \rangle)_{\iota \in I}$ 是 B (命题 3) 的覆盖，称为 *像下* $f$ *覆盖物*$(X_\iota)_{\iota \in I}$。如果$g$是集合C的映射进入集合A，则族$(\overset{-1}{g}\langle X_\iota \rangle)_{\iota \in I}$是C的覆盖，称为覆盖*$(X_\iota)_{\iota \in I}$下*$g$*下的*逆像。
¶ 设 E 和 F 为集合，令 $(X_\iota)_{\iota \in I}$ 为 E 的覆盖，$(Y_\varkappa)_{\varkappa \in K}$ 为 F 的覆盖。则族 $(X_\iota \times Y_\varkappa)_{(\iota, \varkappa) \in I \times K}$ 为 $E \times F$ 的覆盖，称为 E 的覆盖 $(X_\iota)_{\iota \in I}$ 和 F 的$(Y_\varkappa)_{\varkappa \in K}$ 覆盖的 *乘积*。

#### 命题 7 {#ens-ii-s4-prop-7 .statement tag=03PZ}

(1) *设* E *为集合和*$(X_\iota)_{\iota \in I}$ *覆盖*E。*如果*$f$*和*$g$*是两个函数，其域*E*使得*$f$*和*$g$*同意*$E \cap X_\iota$ *对于每个* $\iota \in I$，*然后* $f$ *和* $g$ *同意* E。

(2) *令* $(X_\iota)_{\iota \in I}$ *成为集合的族，并让*$(f_\iota)_{\iota \in I}$ *成为映射的族，具有相同的目标* F *使得对于每个* $\iota \in I$ ** $f_\iota$ *的域是* $X_\iota$，*并且对于每个对* $(\iota, \varkappa) \in I \times I$、$f_\iota$ *和* $f_\varkappa$ *同意* $X_\iota \cap X_\varkappa$。 *那么正好有一个函数* $f$ *带有域* $A = \bigcup_{\iota \in I} X_\iota$ *和目标* F *，其中扩展函数* $f_\iota$ $(i \in I)$ 中的每一个。

(1) 设$x$为E的任意元素，则存在$\iota \in I$使得$x \in X_\iota$、从而$f(x) = g(x)$乘以假设。
(2) 设$G_\iota$为$f_\iota$的图，设$G = \bigcup_{\iota \in I} G_\iota$；让我们证明 G 是一个函数图。如果$(x, y) \in G$和$(x, y') \in G$，I中存在两个指标、$\iota$、$\varkappa$，使得$(x, y) \in G_\iota$和$(x, y') \in G_\varkappa$。这意味着$x \in X_\iota$、$x \in X_\varkappa$、$y = f_\iota(x)$、$y' = f_\varkappa(x)$；但从$x \in X_\iota \cap X_\varkappa$开始，我们

$$f_\iota(x) = f_\varkappa(x),$$

也就是说，$y = y'$。图 G 的域为 $\mathrm{pr}_1 G = \bigcup_{\iota \in I} \mathrm{pr}_1 G_\iota = A$；因此函数$f = (G, A, F)$满足所需的条件。它的唯一性源自命题的第一个部分。

### 7. 划分

#### 定义 6 {#ens-ii-s4-def-6 .statement tag=03Q0}

*两个集合* A *和* B *据说是不相交的*（*或不相交*）*如果* $A \cap B = \emptyset$。 *如果*$A \cap B \neq \emptyset$，*我们说*A*满足*（*或相交*）B。*让*$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$*成为集合的一个族。如果条件* $\iota \in \mathrm{I}$、$\varkappa \in \mathrm{I}$、$\iota \neq \varkappa$ *暗示* $\mathrm{X}_\iota \cap \mathrm{X}_\varkappa = \emptyset$，则该家族的集合据说是相互不相交的。

令$f$为A到B的映射，并令$(\mathrm{Y}_\iota)_{\iota \in \mathrm{I}}$为B的不相交的子集互为族。命题4则表明A的子集族$(\overset{-1}{f}\langle \mathrm{Y}_\iota \rangle)_{\iota \in \mathrm{I}}$互为族集合不相交的。另一方面，如果$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$是A的互不相交的子集的族，则$(f \langle \mathrm{X}_\iota \rangle)_{\iota \in \mathrm{I}}$族的集合一般不互不相交的。

#### 命题 8 {#ens-ii-s4-prop-8 .statement tag=03Q1}

*设*$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$*是相互不相交的集合的一个族，并且让*$(f_\iota)_{\iota \in \mathrm{I}}$*是具有相同目标*F的函数的族，使得*$f_\iota$*的域是*$\mathrm{X}_\iota$*对于每个*$\iota \in \mathrm{I}$。 *那么恰好存在一个具有域* $\bigcup_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ *和目标* F *的函数 f，其中扩展每个函数* $f_\iota$ $(\iota \in \mathrm{I})$。

这是命题 7 中的推论，因为只要$\iota \neq \varkappa$，$f_\iota$ 和$f_\varkappa$ 就明确同意$\mathrm{X}_\iota \cap \mathrm{X}_\varkappa = \emptyset$。

#### 定义 7 {#ens-ii-s4-def-7 .statement tag=03Q2}

*集合* E *的划分是*非空*相互的不相交的子集 of* E *覆盖* E。

#### 例 {#ens-ii-s4-n7-exa-1 .statement tag=03I9}

对于每个非空集合 A，族 $(\{x\})_{x \in \mathrm{A}}$ 是 A 的划分。

如果$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$是集合E的划分，I的映射$\iota \rightarrow \mathrm{X}_\iota$到划分的元素$\mathrm{X}_\iota$集合$\mathfrak{F}$是双射。因此，如果给出$\mathfrak{F}$，则划分将被确定为指标集合之间的一对一对应。通常当我们谈到划分时，我们关心的是元素或划分的集合。

### 8. 集合一家人的和

#### 命题 9 {#ens-ii-s4-prop-9 .statement tag=03Q3}

*让*$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$*成为集合的一家人。那么存在集合* X *以及以下性质* ： X *是一个家庭的并* $(\mathrm{X}'_\iota)_{\iota \in \mathrm{I}}$ *相互不相交的集合，使得对于每个* $\iota \in \mathrm{I}$ *都存在一个一对一映射*$\mathrm{X}_\iota$*到*$\mathrm{X}'_\iota$。

让$\mathrm{A} = \bigcup_{\iota \in \mathrm{I}} \mathrm{X}_\iota$。如果$\iota \in \mathrm{I}$，映射$x \rightarrow (x, \iota)$$(x \in \mathrm{X}_\iota)$是$\mathrm{X}_\iota$的一对一映射到$\mathrm{A} \times \mathrm{I}$的子集$\mathrm{X}'_\iota$。并且，$\mathrm{A} \times \mathrm{I}$上第二个坐标函数下的$\mathrm{X}'_\iota$的像包含在集合$\{\iota\}$中；由此可见，每当$\iota \neq \varkappa$时，$\mathrm{X}'_\iota \cap \mathrm{X}'_\varkappa = \emptyset$。然后我们可以取$\mathrm{X} = \bigcup_{\iota \in \mathrm{I}} \mathrm{X}'_\iota$。

#### 定义 8 {#ens-ii-s4-def-8 .statement tag=03Q4}

*让*$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$*成为集合的一家人。该家庭的和是集合*$(\mathrm{X}_\iota \times \{\iota\})_{\iota \in \mathrm{I}}$家庭的并。

#### 命题 10 {#ens-ii-s4-prop-10 .statement tag=03IA}

*让*$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$*成为相互不相交的集合的一家人。设* A *为其并，* S *其和。那么存在* A *到* S 的双射映射。

对于每个$\iota \in \mathrm{I}$，令$f_\iota$是$\mathrm{X}_\iota$到$\mathrm{X}_\iota \times \{\iota\}$的双射。凭借命题 8，A到S中存在映射$f$，其中扩展全部为映射$f_\iota$。立即验证$f$是A到S上的双射映射。

通过滥用语言，如果在族的和上存在E的双射，则集合E被称为集合$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$族的*和*，如定义8中所定义。

请注意，如果$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$是集合的任意族，命题10的参数表明存在和S*onto*并A的映射。

### 习题{#ens-ii-s4-exercises}

参见[习题为 § 4](exercises/s4/)。

[^1]: 因此，概形 S8 允许我们对集合的族进行定义并，而无需*先验地*假设这些集合是相同集合的子集（这是在并的定义中制造的假设，如下所示） *结果摘要*，§4, no. 2）。
[^2]: 由于应用此公式而产生的一个著名错误是 H. 勒贝格试图证明平面内波莱尔集合轴上的投影又是波莱尔集合（这个叙述随后被证明是不正确的，它引发的讨论是“苏斯林”集合的理论的起源）：勒贝格断言投影交递减序列集合等于交投影 (*Journal de Mathématiques*, (6) **1** (1905), pp. 191-192)。
