---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THEORY OF SETS
section: 2
section_title: Ordered pairs
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 72-75, 123-124
pdf_pages: 0079-0082, 0130-0131
extraction: ocr
subsections:
    - "no": 1
      title: THE AXIOM OF THE ORDERED PAIR
      page: 72
      pdf_page: 79
    - "no": 2
      title: PRODUCT OF TWO SETS
      page: 74
      pdf_page: 81
statements: 4
exercises: 2
content_sha256: cdf5aa56506061e259095a64cd33871f0a191fe09e05d6879d8f7024963fe4a8
translated_from: content/en/ens/II/02_s2_ordered_pairs.md
translation_method: google
source_content_sha256: 30cc0208eaab54246e96f854154d361c7bc5ca97861fad03285d7ff5c5137aa4
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 0f2c415b9c3e468c68f94caad5757f77fcc008980d0031c1d06ddff66afa6f13
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 2.有序对

### 1. 有序对公理

正如我们在§1, no. 1中所说，符号$\supset$是集合论中权2的实数符号。如果T，U是项，则$\supset$TU是项，实际上用(T, U)表示。在这个记号中，有序对*的*公理如下：

A3。 $(\forall x)(\forall x')(\forall y)(\forall y')(((x, y) = (x', y')) \Rightarrow (x = x' \quad \text{and} \quad y = y'))$。

由于关系“$x = x'$和$y = y'$”通过C44暗示$(x, y) = (x', y')$（章I, § 5, no. 2），关系$(x, y) = (x', y')$“等价”于“$x = x'$和$y = y'$”。

¶ 关系 $(\exists x)(\exists y)(z=(x,y))$ 写作“$z$ 是 *有序对*”。如果$z$是有序对，则关系

$$
(\exists y)(z=(x,y)),\qquad(\exists x)(z=(x,y))
$$

分别对$x$和$y$起作用；这是A3的直接的推论。 项

$$
\tau_x((\exists y)(z=(x,y)))\qquad\text{and}\qquad\tau_y((\exists x)(z=(x,y)))
$$

分别用$\operatorname{pr}_1z$和$\operatorname{pr}_2z$表示，称为$z$的*第一坐标*（或*第一投影*）和*第二坐标*（或*第二投影*）。如果 $z$ 为有序对，则关系 $(\exists y)(z=(x,y))$ 相当于 $x=\operatorname{pr}_1z$，关系 $(\exists x)(z=(x,y))$ 相当于 $y=\operatorname{pr}_2z$ (章 I, §5, no. 3)。

¶ 关系 $z=(x,y)$ 相当于“$z$ 是有序对，以及$x=\operatorname{pr}_1z$ 和 $y=\operatorname{pr}_2z$”；对于后者关系相当于

$$
(\exists x')(\exists y')(\exists x'')(\exists y'')(z=(x',y')\text{ and }z=(x,y'')\text{ and }z=(x'',y));
$$

由A3可知，“$z=(x',y')$和$z=(x,y'')$和$z=(x'',y)$”相当于“$z=(x,y)$和$x=x'$和$x=x''$和$y=y'$和$y=y''$”；因此，通过 C33 (章 I, §4, no. 3)，“$z$ 是有序对，$x=\operatorname{pr}_1z$ 和 $y=\operatorname{pr}_2z$”相当于

$$
z=(x,y)\text{ and }(\exists x')(\exists y')(\exists x'')(\exists y'')(x=x'\text{ and }x=x''\text{ and }y=y'\text{ and }y=y''),
$$

这证明了我们的断言。显然我们有

$$
\operatorname{pr}_1(x,y)=x,\qquad \operatorname{pr}_2(x,y)=y,
$$

关系 $z=(\operatorname{pr}_1(z),\operatorname{pr}_2(z))$ 相当于“$z$ 有序对”。

¶ 令 $R\{x,y\}$ 为关系，其中字母 $x$ 和 $y$ 不同，并且出现在 $R$ 中。令$z$为一个字母，与$x$和$y$不同，$R$中没有出现。让$S\{z\}$表示关系

$$
(\exists x)(\exists y)(z=(x,y)\text{ and }R\{x,y\});
$$

这是关系，其中包含比$R$少一个字母，并且*等于*“$z$是有序对和$R\{\operatorname{pr}_1z,\operatorname{pr}_2z\}$”，这是因为$z=(x,y)$相当于“$z$是有序对和$x=\operatorname{pr}_1z$”， $y=\operatorname{pr}_2z$”，以及判据 C33 (章 I, §4, no. 3) 和 C47 (章 I, §5, no. 3)。紧接着 $R\{x, y\}$ 等价于 $S\{(x, y)\}$，并且也等价于

$$(\exists z)(z = (x, y) \text{ and } S\{z\})$$

由C47。

这意味着我们可以将对象、$x$和$y$之间的关系解释为由这些对象组成的有序对的性质。

### 2.两个集合的积

#### 定理 1 {#ens-ii-s2-thm-1 .statement tag=03PC}

*关系*

$$(\forall X)(\forall Y)(\exists Z)(\forall z)((z \in Z) \Leftrightarrow (\exists x)(\exists y)(z = (x, y) \text{ and } x \in X \text{ and } y \in Y)$$

*是真的。在其他字中，对于所有*X*和所有*Y*关系*“$z$*是有序对和*$\mathrm{pr}_1 z \in X$*和*$\mathrm{pr}_2 z \in Y$”*是集合化在*$z$。

让$A_y$表示形式$(x, y)$的所有对象中的集合对于$x \in X$（cf.§1, no. 6，标准C53）。令R为关系$z \in A_y$，相当于$(\exists x)(z = (x, y)$和$x \in X)$。很明显关系

$$(\forall y)(\exists A)(\forall z)(R \Rightarrow (z \in A))$$

根据 S5 (章 I, §4, no. 2)，这是正确的。然后从S8得出关系$(\exists y)(y \in Y$并且R$)$是$z$中的集合化。但这个关系相当于$(\exists x)(\exists y)(y \in Y$和$x \in X$和$z = (x, y))$；因此结果。

#### 定义 1 {#ens-ii-s2-def-1 .statement tag=03PD}

*给定两个集合* X *和* Y，*集合*

$$\mathscr{E}_z((\exists x)(\exists y)(z = (x, y) \text{ and } x \in X \text{ and } y \in Y))$$

*称为* X *和* Y *的乘积，并表示为* X $\times$ Y。

因此，关系$z \in X \times Y$相当于“$z$是有序对和$\mathrm{pr}_1 z \in X$和$\mathrm{pr}_2 z \in Y$”。 集合X和Y被称为X$\times$Y的*第一个*和*第二个因子*。

#### 命题 1 {#ens-ii-s2-prop-1 .statement tag=03PE}

*如果* A$'$、B$'$ *为非空集合，关系* A$' \times$ B$' \subset$ A $\times$ B *等价于*“A$' \subset$ A *和* B$' \subset$ B”。

首先，关系$z \in A' \times B'$相当于“$z$是有序对和$\mathrm{pr}_1 z \in A'$和$\mathrm{pr}_2 z \in B'$”；因此，在 A$'$ 和 B$'$ 上没有任何限制，关系“A$' \subset$ A 和 B$' \subset$ B”意味着

$$A' \times B' \subset A \times B.$$

相反，让我们首先证明，如果$B' \neq \emptyset$（$A'$上没有限制），关系$A' \times B' \subset A \times B$意味着$A' \subset A$。设$x$为$A'$的元素；从$B' \neq \emptyset$开始，有一个对象$y$，它是$B'$的元素；我们有$(x, y) \in A' \times B'$，因此有$(x, y) \in A \times B$，因此有$x \in A$；因而$A' \subset A$。类似地，如果$A' \neq \emptyset$，关系$A' \times B' \subset A \times B$意味着$B' \subset B$。于是就有了这样的结果。

#### 命题 2 {#ens-ii-s2-prop-2 .statement tag=03PF}

*设*A*和*B*为两个集合。 关系* $A \times B = \emptyset$ *相当于*“$A = \emptyset$ *或* $B = \emptyset$”。

对于关系$z \in A \times B$意味着$\mathrm{pr}_1 z \in A$和$\mathrm{pr}_2 z \in B$；因而$A \neq \emptyset$和$B \neq \emptyset$。相反，关系“$x \in A$和$y \in B$”意味着$(x, y) \in A \times B$，因此意味着$A \times B \neq \emptyset$。在其他字中，关系$A \times B \neq \emptyset$相当于“$A \neq \emptyset$和$B \neq \emptyset$”；因此结果。

如果 A, B, C 是集合，我们写

$$(A \times B) \times C = A \times B \times C;$$

$A \times B \times C$的元素$((x, y), z)$写作$(x, y, z)$，称为*三重*。同样，如果 A，B，C，D 是集合，我们写

$$(A \times B \times C) \times D = A \times B \times C \times D;$$

等等。

### 习题{#ens-ii-s2-exercises}

§ 2](exercises/s2/)参见[习题。
