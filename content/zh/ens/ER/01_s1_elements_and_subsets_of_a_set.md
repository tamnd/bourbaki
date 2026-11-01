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
content_sha256: b286c2427a8a2e454cf8702806c13dc2528da59144cb0a9f845ba40885c34527
translated_from: content/en/ens/ER/01_s1_elements_and_subsets_of_a_set.md
translation_method: google
source_content_sha256: 0e243e5f12383731f0a5a2c71334e71b3cefa638eb23c7b52b81096a04bed198
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: d9a7b490910d1b7555ed3f3be709196d001e362a6c5aa69e84586b678f6b7347
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 1. 元素和子集的集合

1. A *set* consists of *elements* which are capable of possessing certain *properties* and of having certain *relations* between themselves or with elements of other sets.

2. Sets and elements are denoted in mathematical arguments by graphical symbols, which in general are letters (from various alphabets) or combinations of letters and other signs. Relations between elements of one or more sets are denoted by inserting the symbols which denote these elements into a scheme characteristic of the relation considered [^1]; and similarly for properties.

字母可以表示集合的*固定*元素或*任意*元素（也称为*变量*、*参数*或*通用*元素）。当任意元素被关系（或性质）中的固定元素替换时，任意元素被认为被赋予这个固定元素作为*值*。

在序中，为了表示关系中出现的元素没有明确写下来，我们用记号表示关系，例如$\mathrm{R}\{x, y, z\}$（如果$x, y, z$是元素）。

3. A relation or a property in which arbitrary elements feature [^2] is said to be an *identity* if it becomes a true proposition whatever values we give to these arbitrary elements. If R and S denote two relations (or properties), R is said to *imply* S if S is true whenever the arbitrary elements which enter in these relations are fixed in such a way that R is true. The relations (or properties) R and S are said to be *equivalent* if each implies the other.

4. Let $\mathrm{R}\{x,\ y,\ z\}$ be a relation between the variables $x$, $y$, $z$. The phrase "for all $x$, $\mathrm{R}\{x,\ y,\ z\}$" is a relation *between $y$ and $z$*, which will be considered to be true for a system of given values of these latter variables if R is true for these values of $y$ and $z$ and *every* value of $x$. The phrase "there exists $x$ such that $\mathrm{R}\{x,\ y,\ z\}$" (or "for some $x$, $\mathrm{R}\{x,\ y,\ z\}$") is again a relation between $y$ and $z$, which will be considered to be true for a system of given values of $y$ and $z$ if, these variables being thus fixed, there is *at least one* value of $x$ for which R is true. Similarly for a relation between any number of variables.

如果$\overline{\mathrm{R}}$表示R的*否定*，那么“对于所有$x$，R”的否定就是“存在$x$使得$\overline{\mathrm{R}}$”； “存在$x$使得R”的否定是“对于所有$x$，$\overline{\mathrm{R}}$”。

5. If R, S denote two relations, we regard "R and S" as a *single* relation, which is considered as true whenever *both* R *and* S are true. Likewise, "R or S" is a relation which is considered to be true whenever *at least one* of the relations R, S is true (and, in particular, whenever they are both true. The word "or" thus does not have the disjunctive sense here which it sometimes has in ordinary speech). Let $\overline{\mathrm{R}}$, $\overline{\mathrm{S}}$ denote the negations of R, S, respectively. Then the negation of "R and S" is "$\overline{\mathrm{R}}$ or $\overline{\mathrm{S}}$", and the negation of "R or S" is "$\overline{\mathrm{R}}$ and $\overline{\mathrm{S}}$".

6. By writing two symbols one on each side of the sign "$=$" (read "equals"), we have a relation called the relation of *equality*, which means that the two symbols represent the *same* element. The negation of this relation is obtained by writing the same symbols one on each side of the sign "$\neq$" (read "is not equal to" or "is different from").

7. Given a set E and a *property* of a generic element of E, those of the elements of E which have this property form a new set, called a *subset* of E. Two *equivalent* properties therefore define the *same* subset of E, and conversely.

设A为E的子集。当$x$是E的泛型元素时，性质“$x$属于到A”（即“$x$是A的元素”）写为“$x \in A$”； 元素中的集合有这个性质显然只是A。

这个性质的否定写成“$x \notin A$”（读作“$x$不属于到A”）； E 的元素的集合具有这个性质，称为 A 的*补集*，写为 $\complement A$ 或 $E - A$。

8. Some properties, for example $x = x$, are true for *all* elements of E. Any two such properties are equivalent, and the subset they define is the set E itself.

另一方面，对于例 $x \neq x$，某些性质对于 E 的*任何* 元素来说并不成立。同样，任何两个这样的性质是等价的，并且子集和定义被称为 E 的*空子集*，用 $\emptyset$ 表示。

注 E 和 $\emptyset$ 彼此“互补”。

9. Let $a$ be a determinate element of E. Some properties, for example $x = a$, are true only for the *single* element $a$. Any two such properties are equivalent; the subset they define is denoted by $\{a\}$, and is called the subset *consisting of a alone*.

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

15. 根据恒等式 (8) 我们结论 ，如果 E 的子集 A 是通过应用 *仅* 运算 $\complement$、$\cup$、$\cap$ 从其他子集 X、Y、Z 获得任意序），则替换子集 X，Y，Z 各自的补码可以得到补码 $\complement A$，运算 $\cup$，$\cap$ 分别可以通过 $\cap$，$\cup$ 得到，而保留运算的序。这就是*二元性规则*。给定上述形式的子集之间的等式 $A = B$，考虑等效的等式 $\complement A = \complement B$。如果我们通过应用对偶规则得到的表达式替换$\complement A$和$\complement B$，然后我们分别通过X，Y，Z替换$\complement X$，$\complement Y$，$\complement Z$，反之亦然，我们得到等式称为$A = B$ 的*对偶*。我们可以对关系$A \subset B$做同样的事情，但是我们必须注意替换符号“$\subset$”被“$\supset$”。

上述带有相同数的身份是彼此的对偶。

16. 在某些问题中，我们必须考虑集合 E 的固定子集 A。如果X是E的任意子集，则集合$A \cap X$称为X在A上的*踪迹*，有时表示为$X_A$；在这种情况下，它被认为是 A 的子集。对于所有子集 X，E 的 Y 我们有

$$(X \cup Y)_A = X_A \cup Y_A, \qquad (X \cap Y)_A = X_A \cap Y_A,$$

和
$$\complement_A X_A = (\complement_E X)_A,$$

其中$\complement_E X$表示E中X的补集，$\complement_A X_A$表示A中$X_A$的补集。

如果$\mathfrak{S}$表示E的子集的集合，则$\mathfrak{S}$的集合在A上的迹线的集合$\mathfrak{S}_A$称为A上$\mathfrak{S}$的*迹线*。

[^1]: 当表示元素的符号是多个符号的组合并且要插入到关系中代替单个字母时，习惯上将其放在序中的括号中以避免可能的混淆。
[^2]: 需要强调的是，当我们谈到集合 E 的泛型* 元素的 *性质时，这绝不意味着性质对于 E 的*每个* 元素都是正确的，而只是意味着它对于 *每个* 元素 *有一定的意义* E；对于其中一些元素来说可能是正确的，而对于其他人来说可能是错误的。对于关系也是如此。
