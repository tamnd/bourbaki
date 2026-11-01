---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION OF FORMAL MATHEMATICS
section: 5
section_title: Equalitarian theories
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 44-49, 59-60
pdf_pages: 0051-0056, 0066-0067
extraction: ocr
subsections:
    - "no": 1
      title: THE AXIOMS
      page: 44
      pdf_page: 51
    - "no": 2
      title: PROPERTIES OF EQUALITY
      page: 45
      pdf_page: 52
    - "no": 3
      title: FUNCTIONAL RELATIONS
      page: 47
      pdf_page: 54
statements: 3
exercises: 7
content_sha256: 9f887798ee81c2cddecc64c29a07eb517d52fd3fc20aaadf490c16080ad13eb4
translated_from: content/en/ens/I/05_s5_equalitarian_theories.md
translation_method: google
source_content_sha256: 8cbe15ed2020b27b62da706075017d090591d51c972f6b3ce0f6ebf686257ba1
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 163565f2de504223d424150b57271ca36b965d07ce495f64136ea29bc0fe23a0
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 5. 平等的理论

### 1. 公理

*平等的理论*是一个$\mathscr{T}$，其关系符号为权2，写作$=$（读作“等于”），其中概形S1到S5（§§3和4），与下面的概形S6和S7一起提供隐式公理。若$T$和$U$在$\mathscr{T}$中为项，则凭借CF4，集合$= TU$在$\mathscr{T}$中为关系（称为等式*的*关系）；实际上它用$T = U$或$(T) = (U)$表示。

S6。 *设$x$为字母，$\mathscr{T}$中$T$和$U$为项，$R\{x\}$为$\mathscr{T}$中的关系；那么关系 $(T = U) \Rightarrow (R\{T\} \Leftrightarrow R\{U\})$ 是一个公理。*

S7。 *如果$R$和$S$是$\mathscr{T}$中的关系并且$x$是一个字母，那么关系$((\forall x)(R \Leftrightarrow S)) \Rightarrow (\tau_x(R) = \tau_x(S))$是一个公理。*

为了证明规则S6是概形，令$A$是$\mathscr{T}$的公理，由应用S6获得；那么$\mathscr{T}$中有关系$R$，$\mathscr{T}$中有项$T$和$U$，还有一个字母$x$，这样$A$就是$(T = U) \Rightarrow ((T|x)R \Leftrightarrow (U|x)R)$。我们将证明，如果$y$是一个字母，并且$\mathscr{T}$中有$V$项，则可以通过应用S6获得关系$(V|x)A$。通过CS1（§1, no. 2），我们可以假设$x$与$y$不同，并且不会出现在$V$中。令$T'$、$U'$、$R'$分别表示组合、$(V|y)T$、$(V|y)U$、$(V|y)R$。通过 CS2 和 CS5 (§1, no. 2)，$(V|y)A$ 与

$$(T' = U') \Rightarrow ((T'|x')R' \Leftrightarrow (U'|x')R')$$

证明已完成。 S7为概形的验证类似。

直观上，概形 S6 意味着如果两个对象相等，则它们具有相同的属性。 概形 S7 更远离日常直觉；这意味着，如果一个对象$x$的两个属性$R$和$S$是等价的，那么可区分的对象、$\tau_x(R)$和$\tau_x(S)$（分别从对象、满足、$R$和满足中选择） $S$，如果这样的对象存在）是相等的。读者会注认为S7中量词$\forall x$的存在是必不可少的（cf.习题7）。

关系 $= TU$ 的否定由 $T \neq U$ 或 $(T) \neq (U)$ 表示（其中符号 $\neq$ 读作“不同于”）。

¶ 从 S6 我们推导出以下标准：

C43。 *设$x$为字母，$\mathscr{T}$中的$T$和$U$为项，$\mathscr{T}$中的$R\{x\}$为关系。然后关系*

$$(T = U \text{ and } R\{T\}), \qquad (T = U \text{ and } R\{U\})$$

*是等价的。*

因为如果我们连接假设 $T = U$ 和 $R\{T\}$，则 $R\{U\}$ 在 S6 中为真；因此 $(T = U$ 和 $R\{U\})$ 为真。

当形式$T = U$中的关系在理论$\mathscr{T}$中得到证明时，人们常常（滥用语言）说$T$和$U$“相同”或“相同”。同样，当$T \neq U$在$\mathscr{T}$中为真时，我们说$T$和$U$“不同”，而不是说，即$T$与$U$不同。

### 2. 等式的性质

从现在开始我们只考虑平等的理论。令$\mathscr{T}$是这样一个理论，并让$\mathscr{T}_0$是一个理论，其符号是$\mathscr{T}$的符号，其唯一公理是概形S1到S7提供的公理。理论 $\mathscr{T}_0$ 比 $\mathscr{T}$ (§2, no. 4) 弱，并且没有常数。以下三个定理是$\mathscr{T}_0$中的定理。

#### 定理 1 {#ens-i-s5-thm-1 .statement tag=03P3}

$x = x$。

让$S$表示$\mathscr{T}_0$中的关系$x = x$。根据C27（§4, no. 1），对于$\mathscr{T}_0$中的每个关系$R$，$(\forall x)(R \Leftrightarrow R)$是$\mathscr{T}_0$中的定理，因此，根据S7，$\tau_x(R) = \tau_x(R)$，即$(\tau_x(R)|x)S$，是定理在$\mathscr{T}_0$。将$R$视为关系“而不是$S$”并考虑C26 (§4, no. 1)，我们看到$(\forall x)S$在$\mathscr{T}_0$中是定理。因此，根据 C30 (§4, no. 3)，$S$ 是 $\mathscr{T}_0$ 中的定理。

关系 $(\forall x)(x = x)$ 也是 $\mathscr{T}_0$ 中的定理；如果$T$在$\mathscr{T}_0$中是项，那么$T = T$在$\mathscr{T}_0$中是定理（cf.§4, no. 3）。可以以同样的方式将变换后来的定理转换为没有字母出现的定理或元数学判据。从现在开始，我们将不再显式地执行这些转换，但我们通常会隐式地使用它们。

#### 定理 2 {#ens-i-s5-thm-2 .statement tag=03P4}

$(x = y) \Leftrightarrow (y = x)$。

假设关系 $x = y$ 为真。 S6 出发，关系

$$(x = y) \Rightarrow ((x|y)(y = x) \Leftrightarrow (y|y)(y = x)),$$

那就是

$$(x = y) \Rightarrow ((x = x) \Leftrightarrow (y = x)),$$

是真的。因此$(x = x) \Leftrightarrow (y = x)$为真。由定理 1 可知 $y = x$ 为真，定理被证明。

#### 定理 3 {#ens-i-s5-thm-3 .statement tag=03P5}

$((x = y) \text{ and } (y = z)) \Rightarrow (x = z)$。

让我们连接假设 $x = y$、$y = z$ 到公理或 $\mathscr{T}_0$。到 S6 关系 $(x = y) \Rightarrow ((x = z) \Leftrightarrow (y = z))$ 为真。因而

$$(x = z) \Leftrightarrow (y = z),$$

因而 $x = z$ 为真。

C44。 *设$x$为字母，$T$、$U$、$V\{x\}$为$\mathscr{T}_0$中的项。那么关系$(T = U) \Rightarrow (V\{T\} = V\{U\})$就是$\mathscr{T}_0$中的定理。*

让$y$和$z$是两个不同的字母，它们不同于$x$以及$T$、$U$、$V$中出现的字母。毗邻假设$y = z$。然后，到了S6，

$$((Y|z)(V\{y\} = V\{z\})) \Leftrightarrow (V\{y\} = V\{z\}),$$

也就是说$(V\{y\} = V\{y\}) \Leftrightarrow (V\{y\} = V\{z\})$，为真。现在，$V\{y\} = V\{y\}$ 到定理 1 为真；因而 $V\{y\} = V\{z\}$ 为真。

由此可见，$(y = z) \Rightarrow (V\{y\} = V\{z\})$ 是 $\mathscr{T}_0$ 中的定理，比如 $A$。但$(T|y)(U|z)A$恰好

$$(T = U) \Rightarrow (V\{T\} = V\{U\}).$$

¶ 形式 $T = U$ 的关系，其中 $T$ 和 $U$ 是 $\mathscr{T}$ 中的项，称为*方程*； 关系 $T = U$ 的 *解*（在 $\mathscr{T}$ 中），被视为字母 $x$ 中的方程，因此在 $\mathscr{T}$ 中为 (§2, no. 2) 项 $V$，使得 $T\{V\} = U\{V\}$ 为定理 $\mathscr{T}$。

¶ 设$T$和$U$为$\mathscr{T}$中的两个项，并令$x_1$、$x_2$、...、$x_n$为出现在$T$但不在$U$中的字母。如果关系

$$(\exists x_1)\ldots(\exists x_n)(T = U)$$

是 $\mathscr{T}$ 中的定理，我们说 *U 可以放入形式* $T$（$\mathscr{T}$ 中）。令$R$为$\mathscr{T}$中的关系，并令$y$为字母。令$V$为$R$的解（$\mathscr{T}$中），视为$y$中的关系。如果$R$的每一个解（在$\mathscr{T}$中），被视为$y$中的关系，都可以放入形式$V$，那么$V$就被称为*完整的解*（或*一般解*) 的$R$（在$\mathscr{T}$）。

### 3. 功能性关系

令 $R$ 为集合，$x$ 为字母。令$y$和$z$是与$x$不同且未出现在$R$中的不同字母。令 $y'$、$z'$ 为另外两个具有相同属性的字母。通过 CS8、CS9 (§4, no. 1)、CS2、CS5 (§1, no. 2) 和 CS6 (§3, no. 4)、组合

$$(\forall y)(\forall z)(((y|x)R \text{ and } (z|x)R) \Rightarrow (y = z))$$

和

$$(\forall y')(\forall z')(((y'|x)R \text{ and } (z'|x)R) \Rightarrow (y' = z'))$$

是相同的。若$\mathscr{T}$中$R$为关系，则定义的集合为$\mathscr{T}$中的关系，表示为“最多存在一个$x$使得$R$”；字母$x$没有出现在这个关系中。当关系在$\mathscr{T}$中是定理时，$R$在$X$中被称为“单值”在$\mathscr{T}$中。要证明$R$在$\mathscr{T}$理论中是单值，只需在$\mathscr{T}$公理$(y|x)R$和$(z|x)R$邻接得到的理论中证明$y = z$就足够了，其中$y$和$z$是不同的字母来自$x$，并且既没有出现在$R$中，也没有出现在$\mathscr{T}$的显式公理中。

C45。 *设$\mathscr{T}$中的$R$为关系，$x$为不是$\mathscr{T}$常数的字母。如果$R$在$\mathscr{T}$中的$x$中是单值，则$R \Rightarrow (x = \tau_x(R))$在$\mathscr{T}$中是定理。相反，如果对于 $\mathscr{T}$ 中的某些项 $T$ 而不是包含 $x$，$R \Rightarrow (x = T)$ 是 $\mathscr{T}$ 中的定理，则 $R$ 在 $x$ 中是单值$\mathscr{T}$.*

假设 $R$ 在 $x$ 和 $\mathscr{T}$ 中是单值，让我们证明

$$R \Rightarrow (x = \tau_x(R))$$

是 $\mathscr{T}$ 中的定理。毗邻假设 $R$。那么通过 S5 $(\tau_x(R)|x)R$ 为真，因此“$R$ 和 $(\tau_x(R)|x)R$”为真。现在，由于 $R$ 在 $x$ 中是单值，

$$(R \text{ and } (\tau_x(R)|x)R) \Rightarrow (x = \tau_x(R))$$

是 C30 (§4, no. 3) 的 $\mathscr{T}$ 定理。因此$x = \tau_x(R)$为真。

¶ 相反，假设$R \Rightarrow (x = T)$ 是$\mathscr{T}$ 中的定理。令 $y$、$z$ 为与 $x$ 不同的不同字母，且既未出现在 $R$ 中，也未出现在 $\mathscr{T}$ 的显式公理中。由于$x$不是$\mathscr{T}$的常数，并且不会出现在$T$、关系中

$$(y|x)R \Rightarrow (y = T), \qquad (z|x)R \Rightarrow (z = T)$$

定理位于 $\mathscr{T}$ 中。毗邻假设 $(y|x)R$ 和 $(z|x)R$。那么$y = T$和$z = T$为真，因此$y = z$为真。

¶ 令 $\mathscr{T}$ 中的 $R$ 为关系。 关系

$$\text{“}(\exists x)R \text{ and there exists at most one } x \text{ such that } R\text{”}$$

表示为“恰好存在一个$x$使得$R$”。如果这个关系是$\mathscr{T}$中的定理，则$R$被称为理论$\mathscr{T}$中*$x$中的*泛函关系。

C46。 *令$\mathscr{T}$中的$R$为关系，并令$x$为不是$\mathscr{T}$常数的字母。如果$R$在$\mathscr{T}$中的$x$中起作用，则$R \Leftrightarrow (x = \tau_x(R))$在$\mathscr{T}$中是定理。相反，如果对于 $\mathscr{T}$ 中的某些项 $T$ 而不是包含 $x$，*

$$R \Leftrightarrow (X = T)$$

*在$\mathscr{T}$中是定理，则$R$在$\mathscr{T}$中的$x$中起作用。*

假设$R$在$x$和$\mathscr{T}$中起作用。那么 $R \Rightarrow (x = \tau_x(R))$ 就是 $\mathscr{T}$ 中的定理通过 C45。另一方面，$(\exists x)R$在$T$中是定理。 S6 关系

$$(x = \tau_x(R)) \Rightarrow (R \Leftrightarrow (\exists x)R)$$

$\mathscr{T}$ 中有定理。如果我们邻接假设$x = \tau_x(R)$，则$R$为真。因此$(x = \tau_x(R)) \Rightarrow R$在$\mathscr{T}$中是定理。

¶ 相反，如果 $R \Leftrightarrow (x = T)$ 在 $\mathscr{T}$ 中是定理，则通过 C45，$R$ 在 $\mathscr{T}$ 中的 $x$ 中是单值。而且，$(T|x)R \Leftrightarrow (T = T)$在$\mathscr{T}$中是定理；因此$(T|x)R$和$(\exists x)R$在$\mathscr{T}$中是定理。

¶ 如果关系 $R$ 在 T 中的 $x$ 中起作用，则 $R$ 相当于关系 $x = \tau_x(R)$，这通常更易于管理。一般引入缩写符号$\Sigma$来表示项$\tau_x(R)$。这样的符号在$\mathscr{T}$中被称为*功能符号*。

直观上，$\Sigma$代表具有由$R$定义的性质的唯一对象。 \* 对于例，在“$y$是实数$\geqslant 0$”是定理、关系“$x$是实数$\geqslant 0$和$y = x^2$”的理论中， $x$。 相应的功能符号被视为$\sqrt{y}$或$y^{1/2}$。 \*

C47。 *令$x$为不是$\mathscr{T}$常数的字母，令$R\{x\}$和$S\{x\}$为$\mathscr{T}$中的两个关系。如果$R\{x\}$在$\mathscr{T}$中的$x$中起作用，则关系$S\{\tau_x(R)\}$相当于$(\exists x)(R\{x\}$和$S\{x\})$。*

因为从C46和C43可以得出，$(R\{x\}$和$S\{x\})$等价于$(R\{x\}$和$S\{\tau_x(R)\})$；因为 $S\{\tau_x(R)\}$ 不包含 $x$，

$$(\exists x)(R\{x\} \ \text{ and } \ S\{\tau_x(R)\})$$

相当于 C33 (§ 4, no. 3) 的 $(S\{\tau_x(R)\}$ 和 $(\exists x)R)$；结果表明 $(\exists x)R$ 为真，因为 $R$ 在 $x$ 中起作用。

### 习题 {#ens-i-s5-exercises}

*总共习题为* § 5，$\mathscr{T}$ *表示平等的理论。*

请参阅[习题为 § 5](exercises/s5/)。
