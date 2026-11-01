---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION OF FORMAL MATHEMATICS
section: 4
section_title: Quantified theories
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 36-44, 58-59
pdf_pages: 0043-0051, 0065-0066
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF QUANTIFIERS
      page: 36
      pdf_page: 43
    - "no": 2
      title: AXIOMS OF QUANTIFIED THEORIES
      page: 37
      pdf_page: 44
    - "no": 3
      title: PROPERTIES OF QUANTIFIERS
      page: 38
      pdf_page: 45
    - "no": 4
      title: TYPICAL QUANTIFIERS
      page: 41
      pdf_page: 48
statements: 0
exercises: 8
content_sha256: fee7e4a802baf2980c983bef6327dd6ce58cb29ff638866b30bc00962c455082
translated_from: content/en/ens/I/04_s4_quantified_theories.md
translation_method: google
source_content_sha256: 07568a80b2b793e5dd22b88d7dc9caf03ded631f676da9f844c975c64e8b5a2c
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: f669200c3b67e15ed6ffc9a8c00d8dcb5296fe35fbf6e47651e76667b7a682b6
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 4.量化理论

### 1.量词的定义

在§ 3中起作用的唯一逻辑符号是$\neg$和$\vee$。我们现在要陈述的规则本质上涉及逻辑符号$\tau$和$\square$的使用。

¶ 如果 $R$ 是一个程序集且 $x$ 是一个字母，则程序集 $(\tau_x(R)|x)R$ 表示为“存在 $x$ 使得 $R$”，或表示为 $(\exists x)R$。大会

$$\text{"not } ((\exists x) \text{ not } R)\text{"}$$

由“对于所有$x$，$R$”表示，或由“给定任何$x$，$R$”，或由$(\forall x)R$表示。缩写符号$\exists$和$\forall$分别称为*存在量词*和*通用量词*。字母$x$不会出现在$\tau_x(R)$表示的组件中*因此不会出现*在$(\exists x)R$和$(\forall x)R$表示的组合中。

CS8。 *设$R$为集合，$x$和$x'$为字母。如果$x'$没有出现在$R$中，则$(\exists x)R$和$(\forall x)R$分别与$(\exists x')R'$和$(\forall x')R'$相同，其中$R'$是$(x'|x)R$。*

因为 $(\tau_x(R)|x)R$ 与 CS1 (§ 1, no. 2) 的 $(\tau_x(R)|x')R'$ 相同，$\tau_x(R)$ 与 CS3 (§ 1, no. 2) 的 $\tau_{x}'(R')$ 相同。因此 $(\exists x)R$ 与 $(\exists x')R'$ 相同。由此可知 $(\forall x)R$ 与 $(\forall x')R'$ 相同。

CS9。 *令$R$和$U$为组合，并让$x$和$y$为不同的字母。如果$X$没有出现在$U$中，则$(U|y)(\exists x)R$和$(U|y)(\forall x)R$分别与$(\exists x)R'$和$(\forall x)R'$相同，其中$R'$是$(U|y)R$。*

因为，根据 CS2 (§ 1, no. 2)，$(U|y)(\tau x(R)|x)R$ 与

$$(T|x)(U|y)R,$$

其中 $T$ 是 $(U|y)\tau_x(R)$，即 $\tau_x(R')$，通过 CS4 (§ 1, no. 2)。因而$(U|y)(\exists x)R$与$(\exists x)R'$相同，因而$(U|Y)(\forall x)R$与$(\forall x)R'$相同。

CF11。 *如果$R$在理论$\mathscr{T}$中是关系并且$x$是一个字母，那么$(\exists x)R$和$(\forall x)R$在$\mathscr{T}$中是关系。*

这紧接着 CF3、CF8 和 CF2 (§ 1, no. 4)。

直观上，让我们将$R$视为表示$x$所表示的对象的性质。从项$\tau_x(R)$的直观意义来看，断言$(\exists x)R$意味着存在一个具有性质$R$的物体。 断言“非$(\exists x)$（非$R$）”意味着不存在性质“非$R$”的对象，因此每个对象都有性质$R$。

在逻辑理论$\mathscr{T}$中，如果我们有形式$(\exists x)R$的定理，其中字母$x$不是$\mathscr{T}$的常量，那么这个定理可以作为辅助常量方法中合法化的定理 (§ 3, no. 3)，因为它与$(\tau_x(R)|x)R$相同。令$\mathscr{T}'$为将$\mathscr{T}$的$R$与公理邻接而得到的理论。如果我们可以证明关系$S$，其中$x$没有出现，在理论上$\mathscr{T}'$中，那么$S$就是$\mathscr{T}$中的定理。

C26。 *令$\mathscr{T}$为逻辑理论，令$R$为$\mathscr{T}$中的关系，令$x$为字母。 关系 $(\forall x)R$ 和 $(\tau_x(\text{not } R)|x)R$ 在 $\mathscr{T}$ 中是等价的。*

因为 $(\forall X)R$ 与“not $(\tau_x(\text{not } R)|x)(\text{not } R)$”相同，因此与“not not $(\tau_x(\text{not } R)|x)R$”相同。

C27。 *如果在逻辑理论$\mathscr{T}$中$R$是定理，其中字母$x$不是常数，那么$(\forall x)R$在$\mathscr{T}$中是定理。*

对于 $(\tau_x(\text{not } R)|X)R$ 来说，$\mathscr{T}$ 中的定理，由 C3 (§ 2, no. 3) 表示。

另一方面，如果$x$是$\mathscr{T}$的常数，则$R$的真实性并不意味着$(\forall x)R$的真实性。直观上，$R$是$x$的真性质（$\mathscr{T}$的确定对象）这一事实显然并不意味着$R$是每个对象的真性质。

C28。 *令$\mathscr{T}$为逻辑理论，令$R$为$\mathscr{T}$中的关系，令$x$为字母。那么关系*“不是$(\forall x)R$”*和$(\exists x)(\text{not } R)$在$\mathscr{T}$中是等价的。*

因为“not $(\forall x)R$”与“not not $(\exists x)(\text{not } R)$”相同。

### 2. 量化理论公理

*量化理论*是任何理论$\mathscr{T}$，其中概形 S1 到 S4 (§ 3, no. 1) 和下面的概形 S5 提供隐式公理。

S5。 *如果$\mathscr{T}$中$R$是关系，如果$\mathscr{T}$中$T$是项，并且$x$是字母，则关系$(T|x)R \Rightarrow (\exists x)R$是公理。*

这个规则确实是概形。令 $A$ 为应用 S5 获得的 $\mathscr{T}$ 公理；那么$\mathscr{T}$中有关系$R$，$\mathscr{T}$中有项$T$，还有一个字母$x$，使得$A$是$(T|x)R \Rightarrow (\exists x)R$。令$U$为$\mathscr{T}$中的项，并令$y$为字母。我们将证明$(U|y)A$也可以通过应用 S5获得。使用CS1（§1, no. 2）和CS8（no. 1），我们可以将自己限制在$x$与$y$不同且未出现在$U$中的情况。令$R'$为关系$(U|y)R$和$T'$项$(U|y)T$。 判据 CS2 (§1, no. 2) 和 CS9 (no. 1) 表明 $(U|y)A$ 与 $(T'|x)R' \Rightarrow (\exists x)R'$ 相同。

概形 S5 表示，如果存在一个对象$T$，其中关系 $R$（被视为表达$x$ 的性质）为真，则$R$ 对于对象$\tau_x(R)$ 为真；这符合我们对$\tau_x(R)$（§1, no. 3，注）的直观含义。

### 3. 量词的性质

从现在开始我们只需要考虑量化理论。对于截面的其余部分，$\mathscr{T}$将表示这样的理论，而$\mathscr{T}_0$将表示没有显式公理的理论，其与$\mathscr{T}$具有相同的符号，并且其唯一的概形是S1到S5。 $\mathscr{T}$比$\mathscr{T}_0$强。

C29。 *设$R$为$\mathscr{T}$中的关系，并令$x$为字母。那么关系“不是$(\exists x)R$”和$(\forall x)(\text{not } R)$在$\mathscr{T}$中是等价的。*

证明$\mathscr{T}_0$理论中的准则，其中$x$不是常数就足够了。 定理 $R \Leftrightarrow (\text{not not } R)$ 给我们，通过 C3 (§2, no. 3)，定理
$$(\exists x)R \Rightarrow (\tau_x(R)|x)(\text{not not } R)$$
和
$$(\exists x)(\text{not not } R) \Rightarrow (\tau_x(\text{not not } R)|X)R.$$

应用 S5，我们在$\mathscr{T}_0$中推导出定理
$$(\exists x)R \Rightarrow (\exists x)(\text{not not } R), \quad (\exists x)(\text{not not } R) \Rightarrow (\exists x)R,$$
从而定理$(\exists x)R \Leftrightarrow (\exists x)(\text{not not } R)$。现在
$$(\exists x)(\text{not not } R)$$
在$\mathscr{T}_0$中相当于“not not $(\exists x)(\text{not not } R)$”，即“not $(\forall x)(\text{not } R)$”。于是就有了这样的结果。

判据 C28 和 C29 使我们能够从量词之一的属性推导出另一个的属性。

C30。 *设$\mathscr{T}$中的$R$为关系，$T$为$\mathscr{T}$中的项，$x$为字母。那么关系$(\forall x)R\Longrightarrow(T|x)R$就是$\mathscr{T}$中的定理。*

通过S5，$(T|x)(\text{not }R)\Longrightarrow(\tau_x(\text{not }R)|x)(\text{not }R)$是一个公理。这个关系与

$$
(\text{not }(T|x)R)\Longrightarrow\text{not}(\tau_x(\text{not }R)|x)R.
$$

因而$(\tau_x(\text{not }R)|x)R\Longrightarrow(T|x)R$是$\mathscr{T}$中的定理。现在使用 C26 (no. 1)。

令$\mathscr{T}$中的$R$为关系。根据C26，C27和C30，无论我们在$\mathscr{T}$中陈述定理$R$，还是定理$(\forall x)R$，或者元数学规则：如果$T$是任何，它都是相同的（假设字母$x$不是$\mathscr{T}$的常数） $\mathscr{T}$中有项，那么$(T|x)R$就是$\mathscr{T}$中的定理。

C31。 *设$R$和$S$为$\mathscr{T}$中的关系，并令$x$为不是$\mathscr{T}$常数的字母。如果$R\Longrightarrow S$（或$R\Longleftrightarrow S$）在$\mathscr{T}$中为定理，则*

$$
(\forall x)R\Longrightarrow(\forall x)S,\qquad(\exists x)R\Longrightarrow(\exists x)S
$$

$$
[\text{resp. }(\forall x)R\Longleftrightarrow(\forall x)S,\qquad(\exists x)R\Longleftrightarrow(\exists x)S]
$$

*定理在 $\mathscr{T}$ 中。*

假设$R\Longrightarrow S$是$\mathscr{T}$中的定理。让我们邻接假设$(\forall x)R$（其中$x$没有出现）。那么$R$，因而$S$，以及$(\forall x)S$，都是真的。因而，$(\forall x)R\Longrightarrow(\forall x)S$ 是$\mathscr{T}$ 中的定理。因而，如果$R\Longleftrightarrow S$在$\mathscr{T}$中是定理，那么也是

$$
(\forall x)R\Longleftrightarrow(\forall x)S.
$$

现在可以使用 C29 推导与$\exists$相关的规则。

C32。 *令$R$和$S$为$\mathscr{T}$中的关系，并令$x$为字母。然后关系*

$$
(\forall x)(R\text{ and }S)\Longleftrightarrow((\forall x)R\text{ and }(\forall x)S),
$$

$$
(\exists x)(R\text{ or }S)\Longleftrightarrow((\exists x)R\text{ or }(\exists x)S)
$$

*定理在 $\mathscr{T}$ 中。*

在$\mathscr{T}_0$中证明这些判据就足够了，其中$x$不是常数。如果$(\forall x)(R\text{ and }S)$为真，则“$R$和$S$”为真，因此关系$R$、$S$均为真。因而，关系、$(\forall x)R$、$(\forall x)S$均为真，因而“$(\forall x)R$和$(\forall x)S$”为真。类似地，如果“$(\forall x)R$和$(\forall x)S$”为真，则$(\forall x)(R\text{ and }S)$为真。因此第一个定理。第二个是应用 C29。

需要注意的是，如果$\mathscr{T}$中$(\forall x) (R$或S）是定理，我们可能不会结论使得$((\forall x)R$或$(\forall x)S)$在$\mathscr{T}$中是定理。直观上，说关系$(\forall x) (R$或S)为真，意味着对于每个对象$x$，关系、$R$、$S$至少有一个为真；但一般来说，两者中只有一个为真，并且是$R$还是$S$将取决于选择或$x$。同样，如果$((\forall x)R$和$(\exists x)S)$在$\mathscr{T}$中是定理，我们可能不会结论在$\mathscr{T}$中$(\exists x)(R$和S）是定理。但是，有以下标准：

C33。 *令$R$和$S$为$\mathscr{T}$中的关系，并令$x$为$R$中未出现的字母。然后关系*

$$(\forall x)(R \text{ or } S) \iff (R \text{ or } (\forall x)S),$$
$$(\exists x)(R \text{ and } S) \iff (R \text{ and } (\exists x)S)$$

*定理位于 $\mathscr{T}$。*

在$\mathscr{T}_0$中建立准则就足够了，其中$x$不是常数。令$\mathscr{T}'$为将$(\forall x)(R$或S)与$\mathscr{T}_0$的公理邻接而得到的理论。在 $\mathscr{T}'$ 中，“$R$ 或 $S$”，因而（不是 $R$）$\Rightarrow S$ 是定理。如果“not $R$”为真（假设，其中$x$不存在），则$S$以及$(\forall x)S$也为真。因而

$$(\text{not } R) \Rightarrow (\forall x)S$$

在$\mathscr{T}'$中是定理，因而$(\forall x)(R$或$S) \Rightarrow (R$或$(\forall x)S)$在$\mathscr{T}_0$中是定理。同样，如果“$R$或$(\forall x)S$”为真，则“$R$或$S$”为真，因而$(\forall x)(R$或S）为真。因而

$$(R \text{ or } (\forall x)S) \Rightarrow (\forall x)(R \text{ or } S)$$

$\mathscr{T}_0$ 中有定理。与$\exists$有关的规则遵循应用C29。

C34。 *令$R$为关系，令$x$和$y$为字母。然后关系*

$$(\forall x)(\forall y)R \iff (\forall y)(\forall x)R,$$
$$(\exists x)(\exists y)R \iff (\exists y)(\exists x)R,$$
$$(\exists x)(\forall y)R \implies (\forall y)(\exists x)R$$

*定理位于$\mathscr{T}$。*

在$\mathscr{T}_0$中证明这些定理就足够了，其中$x$和$y$不是常数。如果$(\forall x)(\forall y)R$为真，则$(\forall y)R$、$R$、$(\forall x)R$、$(\forall y)(\forall x)R$为真。同样，如果$(\forall y)(\forall x)R$为真，则$(\forall x)(\forall y)R$为真；第一个定理紧随其后。第二个现在是使用 C29。最后，由于$(\forall y)R \Rightarrow R$在$\mathscr{T}_0$中是定理，所以$(\exists x)(\forall y)R \Rightarrow (\exists x)R$在C31中也是如此；如果 $(\exists x)(\forall y)R$ 为真，则 $(\exists x)R$ 为真，因而 $(\forall y)(\exists x)R$ 也为真。因此第三个定理。

另一方面，如果$(\forall y)(\exists x)R$在$\mathscr{T}$中是定理，我们可能不会结论使得$(\exists x)(\forall y)R$在$\mathscr{T}$中是定理。直观上，说关系$(\forall y)(\exists x)R$为真意味着，给定任何对象$y$，存在一个对象$x$使得$R$是对象$x$和$y$之间的真关系。但一般来说，对象$x$将依赖于对象$y$的选择，而说$(\exists x)(\forall y)R$为真意味着存在一个*固定*对象$x$，使得$R$是该对象和*任何*对象$y$之间的真关系。

### 4.典型量词

令$A$和$R$为组合，并令$x$为字母。我们用 $(\exists_A x)R$ 表示组件 $(\exists x)(A$ 和 R)，并且组件

$$\text{“not } (\exists_A x) \text{ (not } R)\text{”}$$

$(\forall_A x)R$。缩写符号$\exists_A$和$\forall_A$称为*典型量词*。观察字母$x$没有出现在组合中，用$(\exists_A x)R$、$(\forall_A x)R$表示。

CS10。 *令$A$和$R$为组合，令$x$和$x'$为字母。如果$x$既没有出现在$R$中，也没有出现在$A$中，则$(\exists_A x)R$和$(\forall_A x)R$分别与$(\exists_{A'} x')R'$和$(\forall_{A'} x')R'$相同，其中$R'$是$(x'|x)R$，$A'$是$(x'|x)A$.*

CS11。 *令$A$、$R$、$U$为组合，并令$x$、$y$为不同的字母。如果$x$没有出现在$U$中，则组合、$(U|y)(\exists_A x)R$和$(U|y)(\forall_A x)R$分别与$(\exists_{A'} x')R'$和$(\forall_{A'} x')R'$相同，其中$R'$是$(U|y)R$，$A'$是$(U|y)A$.*

这些规则是判据 CS8、CS9 (no. 1)、CS5 (§ 1, no. 2) 和 CS6 (§ 3, no. 4) 中的直接的推论。

CF12。 *设$A$和$R$为$\mathscr{T}$中的关系，并令$x$为字母。然后*

$$(\exists_A x)R \quad \text{and} \quad (\forall_A x)R$$

*是关系在$\mathscr{T}$。*

这直接源自 CF11 (no. 1)、CF9 (§ 3, no. 4) 和 CF2 (§ 1, no. 4)。

直观地，将$A$和$R$视为表达$x$的属性。可能会发生这样的情况：在证明的级数中，我们只关心对象满足$A$。说存在一个对象满足$A$使得$R$意味着存在一个对象使得“$A$和$R$”； 从而定义共$\exists_A$。说所有对象其中满足$A$有性质$R$意味着不存在满足$A$“不$R$”； 从而定义共$\forall_A$。在实践中，这些符号会根据关系$A$的性质被各种短语代替。 \* 对于例：“对于所有整数$x$，$R$”； “存在集合 E 的元素 $x$，使得 $R$”；等等。 \*

C35。 *设$A$和$R$为$\mathscr{T}$中的关系，并令$x$为字母。那么关系 $(\forall_A x)R$ 和 $(\forall x)(A \Rightarrow R)$ 在 $\mathscr{T}$ 中是等价的。*

对于关系 $(\forall_A x)R$ 与

$$\text{"not}(\exists x)(A \text{ and } (\text{not } R))\text{"}.$$

现在，“$A$ and (not $R$)”在$\mathscr{T}_0$中相当于“not $(A \Rightarrow R)$”；因而“not $(\exists x)(A$ and (not $R$))”在 $\mathscr{T}_0$ 中等效于

$$\text{"not } (\exists x)(\text{not } (A \Rightarrow R))\text{"},$$

由C31（no. 3）组成，后者关系与$(\forall x)(A \Rightarrow R)$相同。因而，该标准在$\mathscr{T}_0$中建立，并因此在$\mathscr{T}$中建立。

我们经常需要证明形式$(\forall_A x)R$中的关系；一般我们会使用以下两个判据之一：

C36。 *设$A$和$R$为$\mathscr{T}$中的关系，并令$x$为字母。令$\mathscr{T}'$为将$\mathscr{T}$的$A$与公理邻接而得到的理论。如果$x$不是$\mathscr{T}$的常量，并且如果$R$在$\mathscr{T}'$中是定理，则$(\forall_A x)R$在$\mathscr{T}$中是定理。*

因为$A \Rightarrow R$在$\mathscr{T}$中是定理，根据演绎的标准，因此通过C27（no. 1）和C35，$(\forall_A x)R$在$\mathscr{T}$中是定理。

In practice, we indicate that we are going to use this rule by a phrase such as "Let $x$ be any element such that $A$". 在如此定义的理论$\mathscr{T}'$中，我们试图证明$R$。 当然，我们不能断言$R$本身就是$\mathscr{T}$中的定理。

C37。 *设$A$和$R$为$\mathscr{T}$中的关系，并令$x$为字母。令$\mathscr{T}'$为通过将关系$A$和“不是$R$”与$\mathscr{T}$的公理邻接而获得的理论。如果$x$不是$\mathscr{T}$的常数，且$\mathscr{T}'$矛盾，则$(\forall_A x)R$是$\mathscr{T}$中的定理。*

对于理论$\mathscr{T}'$来说，等价于将“非$(A \Rightarrow R)$”与$\mathscr{T}$的公理邻接而得到的理论。通过*归谬法*的方法，$A \Rightarrow R$在$\mathscr{T}$中是定理，因此通过C27（no. 1）和C35，$(\forall_A x)R$也是如此。

在实践中，我们说：“假设存在一个对象$x$满足$A$，其中$R$为假”，并试图建立矛盾。

典型量词的属性类似于量词的属性：

C38。 *令$A$和$R$为$\mathscr{T}$中的关系，并令$x$为字母。然后关系*

$$\text{not } (\forall_A x)R \Leftrightarrow (\exists_A x)(\text{not } R),$$
$$\text{not } (\exists_A x)R \Leftrightarrow (\forall_A x)(\text{not } R)$$

*定理在 $\mathscr{T}$ 中。*

C39。 *设$\mathscr{T}$中的$A$、$R$、$S$为关系，$x$为不是$\mathscr{T}$常数的字母。如果关系 $A \Rightarrow (R \Rightarrow S)$ [分别。 $A \Rightarrow (R \Leftrightarrow S)$]是$\mathscr{T}$中的定理，那么关系*

$$(\exists_A x)R \Rightarrow (\exists_A x)S, \qquad (\forall_A x)R \Rightarrow (\forall_A x)S$$
$$[\text{resp. } (\exists_A x)R \Leftrightarrow (\exists_A x)S, \qquad (\forall_A x)R \Leftrightarrow (\forall_A x)S]$$

*定理在 $\mathscr{T}$ 中。*

C40。 *设$\mathscr{T}$中的$A$、$R$、$S$为关系，$x$为字母。然后关系*

$$(\forall_A x)(R \text{ and } S) \Leftrightarrow ((\forall_A x)R \text{ and } (\forall_A x)S),$$
$$(\exists_A x)(R \text{ or } S) \Leftrightarrow ((\exists_A x)R \text{ or } (\exists_A x)S)$$

*定理在 $\mathscr{T}$ 中。*

C41。 *设$\mathscr{T}$中的$A$、$R$、$S$为关系，$x$为$R$中未出现的字母。然后关系*

$$(\forall_A x)(R \text{ or } S) \Leftrightarrow (R \text{ or } (\forall_A x)S),$$
$$(\exists_A x)(R \text{ and } S) \Leftrightarrow (R \text{ and } (\exists_A x)S)$$

*定理位于$\mathscr{T}$中。*

C42。 *设$A$、$B$、$R$为$\mathscr{T}$中的关系，并令$x$和$y$为字母。如果$x$没有出现在$B$中，并且如果$y$没有出现在$A$中，那么关系*

$$(\forall_A x)(\forall_B y)R \Leftrightarrow (\forall_B y)(\forall_A x)R,$$
$$(\exists_A)x(\exists_B y)R \Leftrightarrow (\exists_B y)(\exists_A x)R,$$
$$(\exists_A x)(\forall_B y)R \Rightarrow (\forall_B y)(\exists_A x)R$$

*定理位于 $\mathscr{T}$。*

通过例，我们来证明C42的部分。 关系

$$(\exists_A x)(\exists_B y) R$$

与$(\exists x)(A$、$(\exists y)(B$和$R))$相同，因此（因为$y$没有出现在$A$中）在$\mathscr{T}_0$中等价于

$$(\exists x)(\exists y)(A \text{ and } (B \text{ and } R))$$

由C33和C31。同样，$(\exists_B x)(\exists_A y)R$等价于

$$(\exists y)(\exists x)(B \text{ and } (A \text{ and } R)).$$

现在应用 C31 和 C34 (no. 3)。

\* 作为这些判据的应用的例，请考虑以下关系：“实值函数$(f_n)$的序列在$[0, 1]$中统一收敛到0”。这意味着“对于每个$\varepsilon > 0$，都存在整数$n$，这样对于每个$x \in [0, 1]$和每个整数$m \geqslant n$，我们都有$|f_m(x)| \leqslant \varepsilon$”。假设我们想取这个关系的否定（对于例，通过矛盾得到证明）；标准 C38 表明该否定等价于以下关系：“存在一个$\varepsilon > 0$，使得对于每个整数$n$，都存在一个$x \in [0, 1]$和一个$m \geqslant n$，其中$|f_m(x)| > \varepsilon$”。

### 习题 {#ens-i-s4-exercises}

*总共习题为* § 4、$\mathscr{T}$ *表示量化理论。*

§ 4](exercises/s4/)参见[习题。
