---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 1
section_title: Elements and subsets of a set
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 347-351
pdf_pages: 0352-0356
extraction: ocr
statements: 0
exercises: 0
content_sha256: 3f84591fd946a3a76f1687347a6aa78bc34a2b33684a37576f839ef1bd49e7a7
translated_from: content/en/ens/ER/01_s1_elements_and_subsets_of_a_set.md
translation_method: google
source_content_sha256: 0e243e5f12383731f0a5a2c71334e71b3cefa638eb23c7b52b81096a04bed198
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: d9a7b490910d1b7555ed3f3be709196d001e362a6c5aa69e84586b678f6b7347
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 1. 元素和子集 / 集合

1. *集合* 由 *元素* 组成，*元素* 能够拥有某些 *属性*，并在它们之间或与其他集合的元素之间具有某些 *关系*。

2. 集合和元素在数学论证中用图形符号表示，通常是字母（来自各种字母表）或字母和其他符号的组合。一个或多个集合的元素之间的关系通过将表示这些元素的符号插入到关系的概形特性中来表示，并考虑[^1]；属性也类似。

字母可以表示集合的*固定*元素或*任意*元素（也称为*变量*、*参数*或*通用*元素）。当任意元素被关系（或性质）中的固定元素替换时，任意元素被认为被赋予这个固定元素作为*值*。

在序中，为了表示关系中出现的元素没有明确写下来，我们用记号表示关系，例如$\mathrm{R}\{x, y, z\}$（如果$x, y, z$是元素）。

3. 关系或性质，其中任意元素特征[^2]被称为“身份”，如果它成为真正的命题，无论我们赋予这些任意元素什么值。如果 R 和 S 表示两个关系 （或属性），则只要输入这些关系中的任意元素以 R 为真的方式固定，如果 S 为真，则称 R *暗示* S。 关系（或属性）如果 R 和 S 彼此隐含对方，则称其为“等价”。

4. 令变量$x$、$y$、$z$之间的$\mathrm{R}\{x,\ y,\ z\}$为关系。短语“对于所有$x$，$\mathrm{R}\{x,\ y,\ z\}$”是关系*在$y$和$z$*之间，如果R对于$y$的值为真，则对于给定的值的系统，这将被认为是正确的。 $z$ 和*每*值 $x$。短语“存在$x$使得$\mathrm{R}\{x,\ y,\ z\}$”（或“对于某些$x$，$\mathrm{R}\{x,\ y,\ z\}$”）再次是在$y$和$z$之间的关系，对于给定的值的系统将被认为是正确的$y$ 和 $z$ 如果这些变量因此被固定，则 $x$ 中*至少有一个* 值 R 为真。对于任何数变量之间的关系也是如此。

如果$\overline{\mathrm{R}}$表示R的*否定*，那么“对于所有$x$，R”的否定就是“存在$x$使得$\overline{\mathrm{R}}$”； “存在$x$使得R”的否定是“对于所有$x$，$\overline{\mathrm{R}}$”。

5. 如果 R、S 表示两个关系，我们将“R 和 S”视为*单个* 关系，只要 *R * 和 * S 都为真，就认为它为真。同样，“R 或 S”是关系，只要关系 R、S 中的*至少一个*为真，就被认为是真的（特别是，当它们都为真时。字“或”因此在这里不具有有时在普通语言中所具有的析取意义）。令$\overline{\mathrm{R}}$、$\overline{\mathrm{S}}$分别表示R、S的否定。那么“R和S”的否定是“$\overline{\mathrm{R}}$或$\overline{\mathrm{S}}$”，“R或S”的否定是“$\overline{\mathrm{R}}$和$\overline{\mathrm{S}}$”。

6. 通过在符号“$=$”（读作“等于”）的两侧写上两个符号，我们将关系称为*等式*的关系，这意味着这两个符号代表*相同*元素。这个关系的否定是通过在符号“$\neq$”的每一侧写上相同的符号来获得的（读作“不等于”或“不同于”）。

7. 给定集合 E 和 E 的泛型元素的 *性质*，E 的元素具有此性质形式一个新的集合，称为 E 的 *子集*。两个“等价”属性因此定义 *相同* E 的子集，反之亦然。

设A为E的子集。当$x$是E的泛型元素时，性质“$x$属于到A”（即“$x$是A的元素”）写为“$x \in A$”； 元素中的集合有这个性质显然只是A。

这个性质的否定写成“$x \notin A$”（读作“$x$不属于到A”）； E 的元素的集合具有这个性质，称为 A 的*补集*，写为 $\complement A$ 或 $E - A$。

8. 有些属性，例如 $x = x$，对于 E 的*所有* 元素都成立。任何两个这样的属性都是等价的，并且子集它们定义就是集合 E 本身。

另一方面，某些属性，例如 $x \neq x$，对于 E 的*任何* 元素来说并不成立。同样，任何两个这样的属性是等价的，并且子集和定义被称为 E 的*空子集*，用 $\emptyset$ 表示。

请注意，E 和 $\emptyset$ 是彼此的“互补”。

9. 令 $a$ 为 E 的确定的元素。某些属性，例如 $x = a$，仅对于*单个* 元素 $a$ 为真。任何两个这样的属性都是等价的； 子集、定义用$\{a\}$表示，称为单独*的子集*由……组成。

10、元素均为集合E的*子集*的集合，称为E的子集*的*集合，记为$\mathfrak{P}(E)$。对于所有 $x \in E$，我们都有 $\emptyset \in \mathfrak{P}(E)$、$E \in \mathfrak{P}(E)$ 和 $\{x\} \in \mathfrak{P}(E)$。如果$x$表示E的泛型元素，X表示$\mathfrak{P}(E)$的泛型元素，则$x$和X之间的关系“$x \in X$”称为隶属度*关系。

11. 令$x$和$y$为E的两个元素，并令X为$\mathfrak{P}(E)$的泛型元素。那么等式“$x = y$”的关系“等价”于关系“对于所有X，使得$x \in X$，我们有$y \in X$”。

12. 设X，Y为集合E中的两个子集。如果性质$x \in X$意味着性质$x \in Y$，则字如果X的每一个元素属于到 Y，那么我们说X *包含在* Y 中，或者说 Y *包含于* X，或者X *是* Y 的子集。X 和 Y 之间的这个关系称为*包含于*的关系（Y中的X），并用“$X \subset Y$”或“$Y \supset X$”表示。它的否定用“$X \not\subset Y$”或“$Y \not\supset X$”表示。

对于 E 的所有子集 X，我们有 $\emptyset \subset X$ 和 $X \subset E$。会员资格“$x \in X$”的关系相当于“$\{x\} \subset X$”。

关系“$X \subset Y$和$Y \subset Z$”意味着“$X \subset Z$”。

关系“$X \subset Y$”不排除“$X = Y$”的可能性。 关系“$X \subset Y$和$Y \subset X$”相当于“$X = Y$”。

13. 令X和Y为E的任意两个子集。所有元素中具有性质“$x \in X$或$x \in Y$”的集合用$X \cup Y$表示，称为的*并* X和Y。所有具有性质“$x \in X$和$x \in Y$”的元素中的集合用$X \cap Y$表示，称为X和Y的*交*。

E的多个子集中的并和交以同样的方式定义。

如果$x$、$y$、$z$是E的三个元素，则并$\{x\} \cup \{y\} \cup \{z\}$用$\{x, y, z\}$表示。类似地，对于（单独命名）元素中的任何数。

设X和Y是E的两个子集。根据$X \cap Y \neq \emptyset$或$X \cap Y = \emptyset$，我们说X和Y*相交*或者是*不相交的*。

14. 以下命题、X中的叙述中，Y、Z表示相同集合E中的任意子集。

(a) 我们有$\emptyset = \complement E$，$\quad E = \complement \emptyset$。

(b) 对于所有X，我们有

(1)
$$\complement(\complement X) = X;$$

(2)
$$X \cup X = X, \qquad X \cap X = X;$$

(3)
$$X \cup (\complement X) = E, \qquad X \cap (\complement X) = \emptyset;$$

(4)
$$X \cup \emptyset = X, \qquad X \cap E = X;$$

(5)
$$X \cup E = E, \qquad X \cap \emptyset = \emptyset.$$

(c) 对于所有 X，Y 我们有

(6)
$$X \cup Y = Y \cup X, \qquad X \cap Y = Y \cap X \quad \text{(commutativity)};$$

(7)
$$X \subset X \cup Y, \qquad X \cap Y \subset X;$$

(8)
$$\complement(X \cup Y) = (\complement X) \cap (\complement Y), \qquad \complement(X \cap Y) = (\complement X) \cup (\complement Y).$$

(d) 关系 $X \subset Y$、$\complement X \supset \complement Y$、$X \cup Y = Y$、$X \cap Y = X$ *等效*。

(e) 关系 $X \cap Y = \emptyset$、$X \subset \complement Y$、$Y \subset \complement X$ *等效*。

(f) 关系 $X \cup Y = E$、$\complement X \subset Y$、$\complement Y \subset X$ *等效*。

(g) 对于所有X，Y，Z，我们有

(9)
$$\left.\begin{array}{l} X \cup (Y \cup Z) = (X \cup Y) \cup Z = X \cup Y \cup Z \\ X \cap (Y \cap Z) = (X \cap Y) \cap Z = X \cap Y \cap Z \end{array}\right\} \quad \text{(associativity)};$$

(10)
$$\left.\begin{array}{l} X \cup (Y \cap Z) = (X \cup Y) \cap (X \cup Z) \\ X \cap (Y \cup Z) = (X \cap Y) \cup (X \cap Z) \end{array}\right\} \quad \text{(distributivity)}.$$

(h) 关系“$X \subset Y$”意味着关系“$X \cup Z \subset Y \cup Z$”和“$X \cap Z \subset Y \cap Z$”。

(i) 关系“$Z \subset X$和$Z \subset Y$”相当于“$Z \subset X \cap Y$”。 关系“$X \subset Z$和$Y \subset Z$”相当于“$X \cup Y \subset Z$”。

15. 根据恒等式 (8) 我们结论如果 E 的子集 A 是通过应用 *仅* 运算 $\complement$, $\cup$, $\cap$ 从其他子集 X, Y, Z 获得序)，那么补集$\complement A$可以由替换子集X获得，Y、Z由各自的补集获得，运算$\cup$、$\cap$分别由$\cap$、$\cup$获得，同时保持序共运算。 这就是*二元性规则*。 给定上述形式的子集之间的等式$A = B$，考虑等效的等式$\complement A = \complement B$。 如果我们通过应用对偶规则得到的表达式替换$\complement A$和$\complement B$，然后我们分别通过X，Y，Z替换，$\complement X$，$\complement Y$，$\complement Z$，反之亦然，我们得到等式称为*双*$A = B$。 我们可以对关系$A \subset B$做同样的事情，但是我们必须注意替换符号“$\subset$”和“$\supset$”。

上述带有相同数的恒等式是互为对偶的。

16. 在某些问题中，我们必须考虑集合 E 的固定子集 A。如果X是E的任意子集，集合 $A \cap X$称为X在A上的*踪迹*，有时用$X_A$表示；在这种情况下，它被认为是 A 的子集。对于所有子集 X，E 的 Y 我们有

$$(X \cup Y)_A = X_A \cup Y_A, \qquad (X \cap Y)_A = X_A \cap Y_A,$$

和
$$\complement_A X_A = (\complement_E X)_A,$$

其中$\complement_E X$表示E中X的补集，$\complement_A X_A$表示A中$X_A$的补集。

如果$\mathfrak{S}$表示E的子集的集合，则$\mathfrak{S}$的集合在A上的迹线集合$\mathfrak{S}_A$称为A上$\mathfrak{S}$的*迹线*。

[^1]: 当表示元素的符号是多个符号的组合并且要插入到关系中代替单个字母时，习惯上将其放在序中的括号中以避免可能的混淆。
[^2]: 应该强调的是，当我们谈到集合 E 的泛型* 元素的 *性质时，这绝不意味着性质对于 E 的*每个* 元素都是正确的，而只是它对于 E 的*每个* 元素 *有一个含义*；对于其中一些元素来说可能是正确的，而对于其他人来说可能是错误的。 对于关系也是如此。
