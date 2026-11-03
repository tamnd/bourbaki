---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 3
section_title: Products of sets
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 357-362
pdf_pages: 0362-0367
extraction: ocr
statements: 0
exercises: 0
content_sha256: 12cdeef2da89aa773416e275f67d996347452d4fed1983e167b2669235e09b0c
translated_from: content/en/ens/ER/03_s3_products_of_sets.md
translation_method: google
source_content_sha256: 911c36b076fa6fa142fe625cbd3bb6de17b251c6493dfaffdaf76058fad82252
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: f504b8e89b3ab31360333e9601a1059c80d7b33a69723ed9d365576150318345
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 3. 乘积 / 集合

1. 设 E、F 为两个集合，它们可能不同，也可能不同。 *有序对* $(x,y)$，其第一个元素 $x$ 是 E 的任意元素，第二个元素 $y$ 是 F 的任意元素，是新的集合的元素，称为E的*乘积为F*，记为$E\times F$； E和F称为$E\times F$的*因子*。仅当两个有序对具有相同的第一个元素和相同的第二个元素时，才认为它们是相同的；在其他字、关系“$(x,y)=(x',y')$”等价于关系“$x=x'$和$y=y'$”。如果$z$是$E\times F$中的任意元素，则关系“$x$是有序对$z$的第一个元素”是$x$中的泛函关系；将$E\times F$的确定映射放到E上，称为*第一个坐标函数*，或*第一个投影*，用$\operatorname{pr}_1$表示。我们也说“$x$是$z$”或“$x = \mathrm{pr}_1 z$”的第一个坐标（或投影），而不是说“$x$是有序对$z$”的第一个元素。同样，我们定义*第二个坐标函数*，或*第二个投影*，它是$\mathrm{E} \times \mathrm{F}$的映射*到*$\mathrm{F}$，用$\mathrm{pr}_2$表示。

关系“$x = \mathrm{pr}_1 z$和$y = \mathrm{pr}_2 z$”相当于“$z = (x, y)$”。

函数$\mathrm{pr}_1$的扩张到子集的集合用相同的符号表示，按照一般惯例，再次称为*第一个投影*（这里我们不使用项“坐标”）；对于第二个投影的扩张也是如此。

2. E 的泛型元素 $x$ 与 F 的泛型元素 $y$ 之间的关系 R 为对 $(x, y)$ 的性质，因此定义子集为乘积 $\mathrm{E} \times \mathrm{F}$，称为R的*图*。相反，$\mathrm{E} \times \mathrm{F}$的每个子集A都是$x$和$y$之间的关系$(x, y) \in \mathrm{A}$的图。

设A为E的子集，设B为F的子集。我们用$\mathrm{E} \times \mathrm{F}$的$\mathrm{A} \times \mathrm{B}$子集表示，关系“$x \in \mathrm{A}$和$y \in \mathrm{B}$”在$x$和$y$之间定义。

3. 以下命题、X、X$'$表示E中的任意子集，Y、Y$'$表示F中的任意子集，Z表示$\mathrm{E} \times \mathrm{F}$中的任意子集。

(a) 关系“$\mathrm{X} \times \mathrm{Y} = \emptyset$”*等于*“$\mathrm{X} = \emptyset$或$\mathrm{Y} = \emptyset$”。

(b) 如果$\mathrm{X} \times \mathrm{Y} \neq \emptyset$，关系“$\mathrm{X} \times \mathrm{Y} \subset \mathrm{X}' \times \mathrm{Y}'$”“等于”“$\mathrm{X} \subset \mathrm{X}'$ 和$\mathrm{Y} \subset \mathrm{Y}'$”。

(c) 对于所有 X, X$'$, Y 我们有

$$(\mathrm{X} \times \mathrm{Y}) \cup (\mathrm{X}' \times \mathrm{Y}) = (\mathrm{X} \cup \mathrm{X}') \times \mathrm{Y}. \tag{22}$$

(d) 对于所有X、X$'$、Y、Y$'$，我们有

$$(\mathrm{X} \times \mathrm{Y}) \cap (\mathrm{X}' \times \mathrm{Y}') = (\mathrm{X} \cap \mathrm{X}') \times (\mathrm{Y} \cap \mathrm{Y}'). \tag{23}$$

(e) 对于所有 X，Y 我们有

$$\overset{-1}{\mathrm{pr}_1}(\mathrm{X}) = \mathrm{X} \times \mathrm{F}, \qquad \overset{-1}{\mathrm{pr}_2}(\mathrm{Y}) = \mathrm{E} \times \mathrm{Y}. \tag{24}$$

(f) 如果$\mathrm{Y} \neq \emptyset$，那么对于所有X，我们有

$$\mathrm{pr}_1(\mathrm{X} \times \mathrm{Y}) = \mathrm{X}. \tag{25}$$

(g) 对于所有 Z，我们有

$$\mathrm{Z} \subset \mathrm{pr}_1(\mathrm{Z}) \times \mathrm{pr}_2(\mathrm{Z}). \tag{26}$$

(h) 设$a$为E的元素。则集合$\{a\} \times \mathrm{F}$的映射$(a, y) \rightarrow y$*到*F上（即$\mathrm{pr}_2$到子集$\{a\} \times \mathrm{F}$的限制）为*一对一*。

4.映射

(27) $$(x, y) \to (y, x)$$

是 $\mathrm{E} \times \mathrm{F}$ *到* $\mathrm{F} \times \mathrm{E}$ 的*一对一* 映射，并且被称为*规范*。当E和F相同集合时，映射(27)称为*正则对称*；那么它就是*对合*。在这种对称性下固定的$\mathrm{E} \times \mathrm{E}$的元素$(x, y)$是那些具有性质$x = y$的；这些元素中的集合$\Delta$被称为$\mathrm{E} \times \mathrm{E}$的*对角的*。 映射 $x \to (x, x)$ 是 E 到 $\Delta$ 的*双射*，称为 E 到$\mathrm{E} \times \mathrm{E}$ 的*映射* 对角的。

如果Z是$\mathrm{E} \times \mathrm{F}$中的任意子集，则$\mathrm{E} \times \mathrm{F}$的典范映射下的Z的像到$\mathrm{F} \times \mathrm{E}$表示为$\overset{-1}{\mathrm{Z}}$。如果 X 是 E 的任意子集，Y 是 F 的任意子集，则

$$\overset{-1}{\overgroup{\mathrm{X} \times \mathrm{Y}}} = \mathrm{Y} \times \mathrm{X}.$$

如果关系 R 在 $x$ 和 $y$ 之间，视为有序对 $(x, y)$ 的性质，定义子集 A 的 $\mathrm{E} \times \mathrm{F}$，则*相同* 关系，视为对$(y, x)$中的性质、$\mathrm{F} \times \mathrm{E}$中的定义子集$\overset{-1}{\mathrm{A}}$。 R相当于关系$(x, y) \in \mathrm{A}$、$(y, x) \in \overset{-1}{\mathrm{A}}$中的每一个。如果 E 和 F 相同集合，则 $\mathrm{A} = \overset{-1}{\mathrm{A}}$ 时，关系 R 和相应的子集 A 被称为“对称”。对角的 $\Delta$（由等式的关系定义）是对称的。如果 Z 是 $\mathrm{E} \times \mathrm{E}$ 中的任意子集，则 $\mathrm{Z} \cup \overset{-1}{\mathrm{Z}}$ 和 $\mathrm{Z} \cap \overset{-1}{\mathrm{Z}}$ 是对称的。

5. 令 A 为集合 E 的子集，并令 $f$ 为 A 到集合 F 中的映射。关系泛型元素 $x$ 之间的“$x \in \mathrm{A}$ 和 $y = f(x)$” E 的泛型元素 $y$ 的 F 定义子集 $\mathrm{E} \times \mathrm{F}$ 称为函数 $f$ 的*图*。如果B是E的子集，其中包含A，并且如果$g$是$f$到B的*扩张*（§ 2, no. 13），那么$f$的图*包含于*在$g$的图中。

相反，令C为$\mathrm{E} \times \mathrm{F}$的子集，使得对于每个$x \in \mathrm{E}$，存在*至多*一个*$y \in \mathrm{F}$使得$(x, y) \in \mathrm{C}$。那么集合* $\mathrm{pr}_1(\mathrm{C})$ 的泛型元素 $x$ * 和 F 的泛型元素 $y$ 之间的关系 $(x, y) \in \mathrm{C}$ 是 $y$ 中的泛函关系且将$\mathrm{pr}_1(\mathrm{C})$的确定映射放入图为C的F中。

$\mathrm{E} \times \mathrm{F}$的子集C具有“对于所有$x \in \mathrm{E}$而言，至多有一个$y \in \mathrm{F}$使得$(x, y) \in \mathrm{C}$”（作为$\mathfrak{P}(\mathrm{E} \times \mathrm{F})$的子集的集合）的属性，因此可以与*E子集到*F的*映射集一一对应。

令$f$为E到F的单射映射，并令$g$为$f$的逆，被视为E到$f(\mathrm{E})$的双射。如果C是$f$的图，那么$g$的图就是$\overset{-1}{\mathrm{C}}$。

6. 如果$f$是E到F的映射，C是它在E$\times$F中的图，关系“$y = f(x)$”等价于“$(x, y) \in \mathrm{C}$”。 关系“$y \in f(\mathrm{X})$”相当于“存在$x$使得$x \in \mathrm{X}$和$(x,\ y) \in \mathrm{C}$”。

现在令 K 为 E $\times$ F 的*任意* 子集，并令 X 为 E 的任意子集。令 K(X) 表示所有元素 $y$ 中的 F 由……组成的子集，其中满足关系“存在$x$使得$x \in \mathrm{X}$和$(x, y) \in \mathrm{K}$”；因此，这个关系相当于“$y \in \mathrm{K}(\mathrm{X})$”。 $\mathfrak{P}(\mathrm{E})$ 的映射 $\mathrm{X} \rightarrow \mathrm{K}(\mathrm{X})$ 到 $\mathfrak{P}(\mathrm{F})$ 据说是由 E $\times$ F 的子集* K *定义的。请注意，K(X) 是集合 $\mathrm{K} \cap (\mathrm{X} \times \mathrm{F})$ 的第二个投影。如果K是E的映射$f$到F的图，那么映射$\mathrm{X} \rightarrow \mathrm{K}(\mathrm{X})$是$f$到集合的规范扩张到子集。

7. 如果$x$是E的泛型元素，那么$x \rightarrow \mathrm{K}(\{x\})$就是E到$\mathfrak{P}(\mathrm{F})$的映射，其中值$\mathrm{K}(\{x\})$（也用$\mathrm{K}(x)$表示，滥用语言）被称为*K *at*的*截面 $x$。 关系 $(x,\ y) \in \mathrm{K}$ 相当于$y \in \mathrm{K}(x)$。

反之，E到$\mathfrak{P}(\mathrm{F})$的*每*映射$x \rightarrow \Phi(x)$可以这样得到；对于 E $\times$ F 的关系 $y \in \Phi(x)$ 定义子集 K，$\Phi(x)$ 恰好是 K 在 $x$ 处的截面。因此，E 到 $\mathfrak{P}(\mathrm{F})$ 的映射的集合 $\mathfrak{P}(\mathrm{E} \times \mathrm{F})$ 和集合是一对一的对应。

8. 由 E $\times$ F 的子集 K 定义的每个映射 $\mathrm{X} \rightarrow \mathrm{K}(\mathrm{X})$ 都具有以下属性，将 E 的映射的规范扩张的属性推广到 F 中（§2，第 4 和第 5 项）：
（一）$\mathrm{K}(\emptyset) = \emptyset$。
(b)“$\mathrm{X} \subset \mathrm{Y}$”意味着“$\mathrm{K}(\mathrm{X}) \subset \mathrm{K}(\mathrm{Y})$”。
(c) 对于所有 X，Y 我们有

(28) $$\mathrm{K}(\mathrm{X} \cup \mathrm{Y}) = \mathrm{K}(\mathrm{X}) \cup \mathrm{K}(\mathrm{Y}),$$
(29) $$\mathrm{K}(\mathrm{X} \cap \mathrm{Y}) \subset \mathrm{K}(\mathrm{X}) \cap \mathrm{K}(\mathrm{Y}).$$

如果 K 和 K$'$ 是 E $\times$ F 的两个子集，使得 $\mathrm{K} \subset \mathrm{K}'$，则对于所有 $\mathrm{X} \subset \mathrm{E}$，我们有 $\mathrm{K}(\mathrm{X}) \subset \mathrm{K}'(\mathrm{X})$；特别是，对于所有$x \in \mathrm{E}$，$\mathrm{K}(x) \subset \mathrm{K}'(x)$。相反，如果 $\mathrm{K}(x) \subset \mathrm{K}'(x)$ 对于所有 $x \in \mathrm{E}$，则$\mathrm{K} \subset \mathrm{K}'$。

9. E 的泛型元素和 F 的泛型元素之间的关系定义了 E $\times$ F 的子集 K 和 F $\times$ E 的子集 $\overset{-1}{\mathrm{K}}$，因此定义了 $\mathfrak{P}(\mathrm{E})$ 的 $\mathrm{X} \rightarrow \mathrm{K}(\mathrm{X})$ 到 $\mathfrak{P}(\mathrm{F})$ 的映射以及 $\mathfrak{P}(\mathrm{F})$ 到 $\mathfrak{P}(\mathrm{E})$ 的映射 $\mathrm{Y} \rightarrow \overset{-1}{\mathrm{K}}(\mathrm{Y})$。

如果K是E到F的映射$f$的图，映射$\mathrm{Y} \rightarrow \overset{-1}{\mathrm{K}}(\mathrm{Y})$是$f$的逆扩张。

需要注意的是，当$K$是$E \times F$的任意子集时，关系(18)和(19)不能推广到映射、$X \to K(X)$和$Y \to \overset{-1}{K}(Y)$。

10. 设E、F、G为三个集合，它们可能不同也可能不同，设A为$E \times F$的子集，并令B为$F \times G$的子集。然后$E \times G$的元素$(x, z)$，其中有性质“存在$y \in F$使得$(x, y) \in A$和$(y, z) \in B$”$E \times G$的形式子集，称为*B*和*A的*合成，并且用 $B \circ A$ 表示，或者在不存在混淆风险时简称为 BA。在这里，合成的序是必不可少的。

¶ $\mathfrak{P}(E)$ 的映射 $X \to BA(X)$ 到 $\mathfrak{P}(G)$ 是 $Y \to B(Y)$ 和 $X \to A(X)$ 的合成；在其他字中，对于所有 $X \subset E$ 我们有

$$(30) \qquad BA(X) = B(A(X)).$$

令H为另一个集合，不一定与E、F、G不同，并令C为$G \times H$的子集。那么我们就有$C \circ (B \circ A) = (C \circ B) \circ A$；这个集合也用$C \circ B \circ A$（或简称CBA）表示，称为在这个序中取的C、B、A的*合成*。

令$f$为E到F的映射，并令$g$为F到G的映射。如果A（或B）是$f$（或$g$）的图，则合成 BA是复合映射$g \circ f$的图。

11.我们有

$$(31) \qquad \overset{-1}{\overbrace{B \circ A}} = \overset{-1}{A} \circ \overset{-1}{B}.$$

设A、A′为$E \times F$的两个子集，且令B、B′为$F \times G$的两个子集。然后关系

$$\text{“}A \subset A' \text{ and } B \subset B'\text{”} \qquad \text{implies} \qquad \text{“}B \circ A \subset B' \circ A'\text{”}.$$

设A为$E \times F$的子集，$\Delta$为$E \times E$的对角线，$\Delta'$为$F \times F$的对角线。然后我们有

$$(32) \qquad A \circ \Delta = \Delta' \circ A = A.$$

12. 设E、F、G为三个集合，它们可能不同，也可能不同。它们的*乘积*$E \times F \times G$是有序*三元组*$(x, y, z)$的集合，其中$x \in E$、$y \in F$和$z \in G$，关系“$(x, y, z) = (x', y', z')$”相当于“$x = x'$和$y = y'$并且$z = z'$”。 $E \times F \times G$在E、F、G上的三个映射$(x, y, z) \to x$、$(x, y, z) \to y$、$(x, y, z) \to z$分别称为*第一、第二、*和*第三坐标函数*（或*投影*）；同样，例如，*投影与指标* 1, 2 是映射

$$
(x, y, z) \mapsto (x, y)
$$

$E \times F \times G$到$E \times F$，并用$\mathrm{pr}_{1,2}$表示。

第定义和命题。 2、3 和 4 很容易推广到三个集合中的乘积。

此外，我们可以不考虑三个集合中的乘积$E \times F \times G$，而是等效地考虑通过双应用运算形成两个集合的积而获得的乘积$(E \times F) \times G$。事实上，$(x, y, z) \mapsto ((x, y), z)$是$E \times F \times G$到$(E \times F) \times G$的一对一的映射，称为*规范*。类似地，我们将$E \times F \times G$的定义一对一映射放到集合$E \times (F \times G)$上，以及通过排列三个字母E、F、G从$E \times F \times G$、$(E \times F) \times G$和$E \times (F \times G)$获得的所有集合。

存在类似的定义以及超过三个集合的乘积属性。

13. 如果在任意集合$E'$中取其值的函数$f$定义在三个集合$E$、$F$、$G$中的乘积上，则称为*三个变量*的函数，每个变量都经过集合、$E$、$F$、$G$之一。 $f$的值在$E \times F \times G$的元素$(x, y, z)$处由$f(x, y, z)$表示。

令$a$为$E$中的任意元素。那么$(y, z) \mapsto f(a, y, z)$就是$F \times G$的映射到$E'$，称为由$f$相应的到$x$的值$a$确定的*部分映射（或函数）；它也是 $f$ 和映射 $(y, z) \mapsto (a, y, z)$ $F \times G$ 到 $E \times F \times G$ 的复合。

同样，如果$b$是$F$的元素，则$z \mapsto f(a, b, z)$是$G$的映射到$E'$，称为$f$相应的到值确定的部分映射 $x$、$y$ 中的$a$、$b$。

相反，令$g$是$E$的映射到$E'$。 那么$(x, y, z) \mapsto g(x)$是$E \times F \times G$到$E'$的映射$h$，使得由$h$确定的$E$到$E'$的每个部分映射，对应于$y$和$z$的任何值，与$g$相同。 这个事实通常用说来表达，即参数$x$的函数总是可以被设想为在给定时刻需要考虑的所有参数的函数，当然，其中包括$x$。

14. 令$f$、$g$、$h$分别为$E$的三个映射入$E'$、$F$入$F'$、$G$入$G'$。 $E \times F \times G$到$E' \times F' \times G'$的映射$(x, y, z) \mapsto (f(x), g(y), h(z))$记为$f \times g \times h$，称为$f$、$g$、$h$到乘积的*扩张*。如果 $f$、$g$、$h$ 三个都是单射（分别是满射、双射的），则 $f \times g \times h$ 是单射（分别是满射、双射的）。

在这个和之前的小节中，我们只考虑了*三*集合的情况，只是为了修正想法；类似的考虑适用于集合的任何有限数。
