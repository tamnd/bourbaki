---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION OF FORMAL MATHEMATICS
section: 2
section_title: Theorems
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 24-28, 56-57
pdf_pages: 0031-0035, 0063-0064
extraction: ocr
subsections:
    - "no": 1
      title: AXIOMS
      page: 24
      pdf_page: 31
    - "no": 2
      title: PROOFS
      page: 25
      pdf_page: 32
    - "no": 3
      title: SUBSTITUTIONS IN A THEORY
      page: 26
      pdf_page: 33
    - "no": 4
      title: COMPARISON OF THEORIES
      page: 26
      pdf_page: 33
statements: 1
exercises: 1
content_sha256: e96d55a9c0ab725d5ea0f4da6612f79d67e1629c3e6ac6b1d2259e09741a646e
translated_from: content/en/ens/I/02_s2_theorems.md
translation_method: google
source_content_sha256: c8b7ac12f220f9f720128bb004ee9ac705cf905ac08dfbc648d08a0ff3975ca7
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 66bd22e85783bc15a195a63fd0733581a23180b2dc674a3418c8f52598a8b5cf
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 2. THEOREMS

*从现在开始，如果$A$是关系，我们就写not($A$)而不是$\neg A$。如果$A$和$B$是关系，我们应该写“($A$)或($B$)”而不是$\vee AB$，并且写($A$)$\Rightarrow$($B$)而不是$\Rightarrow AB$。 有时我们将省略括号。在每种情况下，读者都能够毫无困难地确定考虑组装。*

### 1. 公理

我们已经看到了理论$\mathscr{T}$中的具体符号确定项和关系。对于构造$\mathscr{T}$，我们进行如下操作：

(1) 首先我们在$\mathscr{T}$中记下关系的某个数；这些被称为 $\mathscr{T}$ 的*显式公理*。显式公理中出现的字母称为 $\mathscr{T}$ 的*常数*。

(2) 我们制定一个或多个规则[^1]，称为$\mathscr{T}$的*概形*，它必须具有以下属性： (a) 这样的规则$\mathscr{R}$的应用在$\mathscr{T}$中提供关系； (b) 如果$\mathscr{T}$中$T$是项，$x$是字母，并且由应用概形$\mathscr{R}$构造的$\mathscr{T}$中$R$是关系，则关系 $(T|x)R$也可以由应用$\mathscr{R}$构造。

在我们设想的所有情况下，验证这些条件总是很容易的。

由$\mathscr{T}$的应用概形构造的每个关系称为$\mathscr{T}$的*隐式公理*。

直观上，公理要么代表不言而喻的断言，要么代表人们希望从中得出推论的假设。这些常量表示明确定义的对象，显式公理所表达的属性应该为真。另一方面，如果字母$x$不是一个常数，则代表一个完全未确定的对象；如果通过公理假设对象$x$的性质为真，则该公理必然是隐式的，因此性质对于任何对象$T$都保持为真。

### 2. PROOFS

理论$\mathscr{T}$中的*示范性文本*包括：

(1) $\mathscr{T}$中关系和项的辅助形成构造。

(2)*$\mathscr{T}$中的*证明，即$\mathscr{T}$中关系的序列出现在辅助形成构造中，使得对于序列中的每个关系$\mathbf{R}$至少满足以下条件之一：

(a$_1$)$\mathbf{R}$是$\mathscr{T}$的显式公理。

(a$_2$)$\mathbf{R}$是将$\mathscr{T}$的概形应用到项或关系的结果，这些项或关系出现在辅助形成构造中。

(b) 序列中有两个关系、$\mathbf{S}$、$\mathbf{T}$位于$\mathbf{R}$之前，使得$\mathbf{T}$为$\mathbf{S} \Rightarrow \mathbf{R}$。

¶ $\mathscr{T}$ 中的 *定理* 是关系 *，它出现在* $\mathscr{T}$ 中的证明中。

因此，这个概念本质上取决于所考虑的理论在描述时的状态。 A relation in a theory $\mathscr{T}$ *becomes* a theorem in $\mathscr{T}$ when one succeeds in inserting it into a proof in $\mathscr{T}$. 说$\mathscr{T}$中的关系“不是$\mathscr{T}$中的定理”不能，无论$\mathscr{T}$理论的发展阶段如何，都没有任何意义。

$\mathscr{T}$中的定理也称为“$\mathscr{T}$中的*true*关系”（或“命题”、“引理”、“推论”等）。令$\mathscr{T}$中的$\mathbf{R}$为关系，$\mathbf{x}$为字母，$\mathscr{T}$中的$\mathbf{T}$项；如果$(\mathbf{T}|\mathbf{x})\mathbf{R}$在$\mathscr{T}$中是定理，则$\mathbf{T}$被认为是$\mathscr{T}$中的*满足关系*$\mathbf{R}$（或者是*$\mathbf{R}$的*解），当考虑$\mathbf{R}$时如$\mathbf{x}$中的关系。

¶ 如果 $\mathscr{T}$ 中的否定为定理，则关系在 $\mathscr{T}$ 中被称为“假”。当一个人写出关系时，$\mathscr{T}$ 理论就被称为“矛盾”，而关系在 $\mathscr{T}$ 中既正确又错误。

在这里，我们再次处理概念，这取决于理论的特定发展状态。读者应该提防这种混淆（不幸的是，字“假”的直观含义暗示了这一点），即相信一旦证明关系$\mathbf{R}$在$\mathscr{T}$中为假，就可以确定$\mathbf{R}$在$\mathscr{T}$中“不为真”（严格来说，这个短语*在数学中*没有精确的含义，因为我们有上面已经说过了）。

¶ 接下来我们将给出元数学判据，称为*演绎判据*，这将使我们能够缩短证明。这些判据将由字母 C 后跟数表示。

C1（*三段论*）。 *令$\mathbf{A}$和$\mathbf{B}$在理论$\mathscr{T}$中为关系。如果$\mathbf{A}$和$\mathbf{A} \Rightarrow \mathbf{B}$在$\mathscr{T}$中是定理，那么$\mathbf{B}$在$\mathscr{T}$中是定理。*

Let $R_1$, $R_2$, ..., $R_n$ be a proof in $\mathscr{T}$ in which $A$ appears, and let $S_1$, $S_2$, ..., $S_p$ be a proof in $\mathscr{T}$ in which $A \Rightarrow B$ appears. 显然，$R_1$，$R_2$，...，$R_n$，$S_1$，$S_2$，...，$S_p$在$\mathscr{T}$中是证明，其中$A$和$A \Rightarrow B$都出现了。 因此

$$R_1, \; R_2, \; \ldots, \; R_n, \; S_1, \; S_2, \; \ldots, \; S_p, \; B$$

是$\mathscr{T}$中的证明，因此$B$是$\mathscr{T}$中的定理。

### 3. 代换理论

设$\mathscr{T}$是一个理论，$A_1$，$A_2$，...，$A_n$是其显式公理，$x$是一个字母，$T$项是$\mathscr{T}$。令$(T|x)\mathscr{T}$为符号和概形与$\mathscr{T}$相同的理论，其显式公理为$(T|x)A_1$，$(T|x)A_2$，...，$(T|x)A_n$。

C2。 *令$A$为理论$\mathscr{T}$中的定理，令$T$为$\mathscr{T}$的项，令$x$为字母。那么理论上$(T|x)\mathscr{T}$中$(T|x)A$就是定理。*

将$A$出现的$\mathscr{T}$中的$R_1$、$R_2$、…、$R_n$设为证明。考虑序列$(T|x)R_1$、$(T|x)R_2$、...、$(T|x)R_n$，由于 CF8 (§ 1, no. 4)，它是 $\mathscr{T}$ 中关系的序列。我们将证明这个序列在理论$(T|x)\mathscr{T}$中是证明；这将确立标准。如果$R_k$是$\mathscr{T}$的隐式公理，那么$(T|x)R_k$又是$\mathscr{T}$（no. 1）的隐式公理，因此也是$(T/x)\mathscr{T}$的隐式公理。如果$R_k$是$\mathscr{T}$的显式公理，则$(T|x)R_k$是$(T|x)\mathscr{T}$的显式公理。最后，如果$R_k$前面有关系、$R_i$和$R_j$，其中$R_j$是$R_i \Rightarrow R_k$，那么$(T|x)R_k$前面有$(T|x)R_i$和$(T|x)R_j$，后者与$(T|x)R_i \Rightarrow (T|x)R_k$相同（标准 CS5）。

C3。 *令$A$为理论$\mathscr{T}$的定理，令$T$为$\mathscr{T}$的项，令$x$为不是$\mathscr{T}$常数的字母。那么 $(T|x)A$ 就是 $\mathscr{T}$ 的定理。*

这直接从 C2 得出，因为 $x$ 并不出现在 $\mathscr{T}$ 的显式公理中。更具体地，如果$\mathscr{T}$包含没有显式公理，或者如果显式公理包含没有字母，则标准C3适用而在字母$x$上没有限制。

### 4. COMPARISON OF THEORIES

如果$\mathscr{T}$的所有符号都是$\mathscr{T}'$的符号，$\mathscr{T}$的所有显式公理是$\mathscr{T}'$中的定理，并且$\mathscr{T}$的概形是概形，则称理论$\mathscr{T}'$比理论$\mathscr{T}$“更强” $\mathscr{T}'$。

C4。 *如果理论$\mathscr{T}'$比理论$\mathscr{T}$更强，则$\mathscr{T}$的所有定理都是$\mathscr{T}'$的定理。*

令 $\mathscr{T}$ 中的 $R_1$、$R_2$、...、$R_n$ 为证明。我们将逐步证明，每个 $R_i$ 都是 $\mathscr{T}'$ 中的定理。假设对于 $R_k$ 之前的关系来说，这是正确的。如果$R_k$是$\mathscr{T}$的公理，那么它就是$\mathscr{T}'$乘假设的定理。如果$R_k$前面有关系、$R_i$和$R_i \Rightarrow R_k$，我们已经知道$R_i$和$R_i \Rightarrow R_k$在$\mathscr{T}'$中是定理，因此$R_k$在定理中$\mathscr{T}'$凭借C1。因此，在任何情况下，$R_k$都是$\mathscr{T}'$中的定理，并且证明是完整的。

如果$\mathscr{T}$和$\mathscr{T}'$两个理论中的一个比另一个更强，则$\mathscr{T}$和$\mathscr{T}'$被称为“等价”。那么$\mathscr{T}$的每个定理都是$\mathscr{T}'$的定理，反之亦然。

C5。 *设$\mathscr{T}$为理论，$A_1$、$A_2$、...、$A_n$为其显式公理，$a_1$、$a_2$、...、$a_h$为其常量，并令$T_1$、$T_2$、...、$T_h$为项在$\mathscr{T}$。假设*

$$(T_1|a_1) \, (T_2|a_2) \, \ldots \, (T_h|a_h)A_i \qquad (\text{for} \quad i = 1, 2, \ldots, n)$$

*在理论$\mathscr{T}'$中是定理，$\mathscr{T}$的符号是$\mathscr{T}'$的符号，$\mathscr{T}$的概形是$\mathscr{T}'$的概形。那么，如果$\mathscr{T}$中$A$是定理，*

$$(T_1|a_1) \, \ldots \, (T_h|a_h)A$$

*是$\mathscr{T}'$中的定理。*

因为$\mathscr{T}'$比理论$(T_1|a_1) \ldots (T_n|a_n) \mathscr{T}$强，我们可以应用C2和C4。

当我们使用这个过程从$\mathscr{T}$中的定理推出$\mathscr{T}'$中的定理时，我们说*我们是$\mathscr{T}'$中的应用$\mathscr{T}$*的结果。直观上，$\mathscr{T}$的公理表达了$a_1, a_2, ..., a_h$的性质，$A$表达了性质，即这些公理的推论。如果$\mathscr{T}'$中的对象$T_1, T_2, ..., T_h$具有$\mathscr{T}$的公理所表示的性质，那么它们也有性质$A$。

\*对于例，在群$\mathscr{T}$的理论中，显式公理包含两个常数G和$\mu$（合成的群和律）。在集合论$\mathscr{T}'$，我们定义两个项：实直线和实数的加法。如果我们在$\mathscr{T}$的显式公理中分别用这些项代替G和$\mu$，我们在$\mathscr{T}'$中得到定理。而且，概形与$\mathscr{T}$、$\mathscr{T}'$的符号相同。因此，我们可以“将群理论的结果应用到实数的加法群”。我们说我们已经为集合论中的群理论构建了一个*模型*。 （注由于群的理论比集合论强，所以我们也可以将集合论的结果应用到群的理论。）\*

#### 注 {#ens-i-s2-n4-rem-1 .statement tag=03G7}

在C5的假设下，如果$\mathscr{T}$理论被证明是矛盾的，$\mathscr{T}'$也是如此。因为如果$A$和“不是$A$”是$\mathscr{T}$中的定理，那么$(T_1|a_1) \ldots (T_h|a_h)A$和$\mathrm{not}(T_1|a_1) \ldots (T_h|a_h)A$是$\mathscr{T}'$中的定理。 \* 对于例，如果群的理论是矛盾的，那么集合论也会是矛盾的。 \*

### 习题{#ens-i-s2-exercises}

参见[习题为 § 2](exercises/s2/)。

[^1]: For the sake of brevity, these rules are expressed by using the symbols mentioned in § 1, no. 1 (and especially bold-faced italic letters); but it would be easy to avoid the use of these symbols completely in the formulation of the rules (see § 3, no. 1, note (*) on p. 28).
