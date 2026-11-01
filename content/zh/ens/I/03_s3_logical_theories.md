---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION OF FORMAL MATHEMATICS
section: 3
section_title: Logical theories
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 28-36, 57-58
pdf_pages: 0035-0043, 0064-0065
extraction: ocr
subsections:
    - "no": 1
      title: THE AXIOMS
      page: 28
      pdf_page: 35
    - "no": 2
      title: FIRST CONSEQUENCES
      page: 29
      pdf_page: 36
    - "no": 3
      title: METHODS OF PROOF
      page: 30
      pdf_page: 37
    - "no": 4
      title: CONJUNCTION
      page: 33
      pdf_page: 40
    - "no": 5
      title: EQUIVALENCE
      page: 34
      pdf_page: 41
statements: 0
exercises: 5
content_sha256: 07a1a463dd41d7534ffe2fffc29b54090ed43cbdc5b50485da854761be653f4b
translated_from: content/en/ens/I/03_s3_logical_theories.md
translation_method: google
source_content_sha256: 37ec32a3c0cdf2c61a57848be909293d325cc40d690c0e328f7cb619bf02c9e1
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: bde532d91ecec524a7754ae46177e1bf1c039bc009e69ab585a3a904eabf6df1
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 3.逻辑理论

### 1.公理

*逻辑理论*是任何理论$\mathscr{T}$，其中概形下面的S1到S4提供隐式公理。

S1。 *如果$A$在$\mathscr{T}$中是关系，则关系$(A$或$A) \Rightarrow A$是$\mathscr{T}$* [^1]的公理。

S2。 *如果$A$和$B$是$\mathscr{T}$中的关系，则关系$A \Rightarrow (A$或B)是$\mathscr{T}$的公理。*

S3。 *如果$A$和$B$在$\mathscr{T}$中是关系，则关系$(A$或$B) \Rightarrow (B$或A)是$\mathscr{T}$的公理。*

S4。 *如果$A$、$B$、$C$在$\mathscr{T}$、关系中为关系*

$$(A \Rightarrow B) \Rightarrow ((C \text{ or } A) \Rightarrow (C \text{ or } B))$$

*是$\mathscr{T}$的公理。*

这些规则实际上是概形；让我们验证一下，S2 的例。设$R$为应用S2得到的关系；那么$\mathscr{T}$中有关系$A$和$B$，使得$R$是关系$A \Rightarrow (A$或B）。令$T$为$\mathscr{T}$中的项，令$x$为字母，令$A'$和$B'$为关系$(T|x)A$和$(T|x)B$；则$(T|x)R$与$A' \Rightarrow (A'$或$B')$相同，因此可以通过应用S2获得。

直观上，规则S1到S4仅仅表达了字通常的数学语言[^2]中“或”和“暗示”的含义。

如果逻辑理论$\mathscr{T}$是矛盾的，*$\mathscr{T}$中的每个关系都是$\mathscr{T}$中的定理。*因为让$A$是$\mathscr{T}$中的关系，这样$A$和“不是$A$”是$\mathscr{T}$中的定理，并令$B$为$\mathscr{T}$中的任意关系。通过S2，（不是$A$）$\Rightarrow$（（不是$A$）或$B$）在$\mathscr{T}$中等于定理；因此，通过C1（§ 2, no. 2），“（不是$A$）或$B$”，即$A \Rightarrow B$，是$\mathscr{T}$中的定理。 C1 的第二次应用显示$B$ 是$\mathscr{T}$ 中的定理。

¶ *从现在开始$\mathscr{T}$将表示逻辑理论。*

### 2. 第一推论

C6。 *令$\mathscr{T}$中的$A$、$B$、$C$为关系。如果$A \Rightarrow B$和$B \Rightarrow C$在$\mathscr{T}$中是定理，则$A \Rightarrow C$在$\mathscr{T}$中是定理。*

因为$(B \Rightarrow C) \Rightarrow ((A \Rightarrow B) \Rightarrow (A \Rightarrow C))$是$\mathscr{T}$的公理，在S4中，替换，$A$由$B$，$B$由$C$，$C$由“不是$A$”。通过 C1 (§ 2, no. 2)，$(A \Rightarrow B) \Rightarrow (A \Rightarrow C)$ 是 $\mathscr{T}$ 中的定理。进一步应用 C1 完成证明。

C7。 *如果$A$和$B$在$\mathscr{T}$中为关系，则$B \Rightarrow (A$或B)在$\mathscr{T}$中为定理。*

对于$B \Rightarrow (B$或A)和$(B$或$A) \Rightarrow (A$或B)来说，根据S2和S3是$\mathscr{T}$的公理。现在使用C6。

C8。 *如果$\mathscr{T}$中$A$是关系，则$A \Rightarrow A$在$\mathscr{T}$中是定理。*

对于 $A \Rightarrow (A$ 或 A) 和 $(A$ 或 $A) \Rightarrow A$ 是公理，由 S2 和 S1 得出。现在使用C6。

C9。 *如果$\mathscr{T}$中$A$是关系且$B$定理，则$A \Rightarrow B$在$\mathscr{T}$中是定理。*

对于$B \Rightarrow ((\text{not } A)$或B)来说，C7乘以定理，因此“（不是$A$）或$B$”，也就是说，$A \Rightarrow B$，C1乘以定理。

C10。 *如果$\mathscr{T}$中的$A$是关系，则“$A$或（不是$A$）”是$\mathscr{T}$中的定理。*

对于“（不是$A$）或$A$”，C8 为定理；现在使用S3和C1。

C11。 *如果$A$在$\mathscr{T}$中为关系，则“$A \Rightarrow$（不是$A$）”在$\mathscr{T}$中为定理。*

对于这个关系是“（不是$A$）或（不是$A$）”，结果来自C10。

C12。 *令$A$和$B$为$\mathscr{T}$中的两个关系。然后关系*

$$(A \Rightarrow B) \Rightarrow ((\text{not } B) \Rightarrow (\text{not } A))$$

*是 $\mathscr{T}$ 中的定理。*

对于

$$((\text{not } A) \text{ or } B) \Rightarrow ((\text{not } A) \text{ or } (\text{not not } B))$$

是定理，由 C11、S4 和 C1 组成。另一方面，

$$((\text{not } A) \text{ or } (\text{not not } B)) \Rightarrow ((\text{not not } B) \text{ or } (\text{not } A))$$

是 S3 的公理。因此

$$((\text{not } A) \text{ or } B) \Rightarrow ((\text{not not } B) \text{ or } (\text{not } A))$$

是 C6 的定理。于是就有了这样的结果。

C13。 *设$\mathscr{T}$中的$A$、$B$、$C$为关系。如果$A \Rightarrow B$在$\mathscr{T}$中是定理，那么$(B \Rightarrow C) \Rightarrow (A \Rightarrow C)$在$\mathscr{T}$中是定理。*

对于 $(\text{not } B) \Rightarrow (\text{not } A)$ 来说，由 C12 和 C1 得到定理。因此，通过 S4 和 C1，$(C \text{ or } (\text{not } B)) \Rightarrow (C \text{ or } (\text{not } A))$ 为定理。通过双应用S3和C6我们推断

$$((\text{not } B) \text{ or } C) \Rightarrow ((\text{not } A) \text{ or } C)$$

是定理；但这是给定的关系。

¶ *从现在开始，我们通常会使用* C1 *和* C6 *而不明确引用它们。*

### 3.证明方法

I。 *辅助假设的方法。*这取决于以下规则：

C14（*演绎*的标准）。 *设$\mathscr{T}$中$A$为关系，$\mathscr{T}'$为$\mathscr{T}$的$A$与公理邻接所得的理论。如果$B$在$\mathscr{T}'$中是定理，那么$A \Rightarrow B$在$\mathscr{T}$中是定理。*

令$B$出现的$\mathscr{T}'$中的$B_1$、$B_2$、…、$B_n$为证明。我们将逐步证明关系$A \Rightarrow B_k$是$\mathscr{T}$中的定理。假设这对于$B_i$之前的关系成立，让我们证明$A \Rightarrow B_i$在$\mathscr{T}$中是定理。如果$B_i$是$\mathscr{T}'$的公理，那么$B_i$要么是$\mathscr{T}$的公理，要么是$A$。在这两种情况下，$A \Rightarrow B_i$ 是 $\mathscr{T}$ 应用 C9 或 C8 中的定理。如果$B_i$前面有关系、$B_j$和$B_j \Rightarrow B_i$，我们就知道$A \Rightarrow B_j$和$A \Rightarrow (B_j \Rightarrow B_i)$是$\mathscr{T}$中的定理。因此，$(B_j \Rightarrow B_i) \Rightarrow (A \Rightarrow B_i)$ 是 C13 的 $\mathscr{T}$ 中的定理。因此，对于C6来说，$A \Rightarrow (A \Rightarrow B_i)$，即“$(\text{not } A)$或$(A \Rightarrow B_i)$”，在$\mathscr{T}$中是定理，因此对于S3来说，“$(A \Rightarrow B_i)$或$(\text{not } A)$”也是如此。现在，$(\text{not } A) \Rightarrow ((\text{not } A) \text{ or } B_i)$，即$(\text{not } A) \Rightarrow (A \Rightarrow B_i)$，是 S2 的$\mathscr{T}$中的定理。通过应用 S4 我们可以看到

$$((A \Rightarrow B_i) \text{ or } (\text{not } A)) \Rightarrow ((A \Rightarrow B_i) \text{ or } (A \Rightarrow B_i))$$

是$\mathscr{T}$中的定理，因此“$(A \Rightarrow B_i)$或$(A \Rightarrow B_i)$”是$\mathscr{T}$中的定理。到 S1 时，我们结论 $A \Rightarrow B_i$ 是 $\mathscr{T}$ 中的定理。

在实践中，我们将通过诸如“假设 $A$ 为真”之类的短语来表明我们将使用此标准。这句话的意思是，推理暂时会在$\mathscr{T}'$理论中进行，直到关系$B$被证明为止。当实现这一点时，就可以确定$\mathscr{T}$中的$A \Rightarrow B$是定理，并且此后继续在$\mathscr{T}$中进行推理，而一般不会表明人们已经放弃了$\mathscr{T}'$理论。作为新公理引入的关系$A$称为*辅助假设*。 \* 对于例，当我们说“让$x$是实数”时，我们正在构建一个理论，其中关系“$x$是实数”是辅助假设。 \*

II。 *归谬法的方法。*这是建立在以下规则之上的：

C15。 *设$\mathscr{T}$中的$A$为关系，并令$\mathscr{T}'$为通过将公理*“不是$A$”*与$\mathscr{T}$的公理邻接而获得的理论。如果$\mathscr{T}'$矛盾，那么$A$就是$\mathscr{T}$中的定理。*

对于 $A$ 来说，$\mathscr{T}'$ 中有定理；因而，（辅助假设的方法）“（不是$A$）$\Rightarrow A$”在$\mathscr{T}$中是定理。到了S4，

$$(A \text{ or } (\text{not } A)) \Rightarrow (A \text{ or } A)$$

$\mathscr{T}$ 中有定理；通过C10，“$A$或$A$”是$\mathscr{T}$中的定理。现在使用S1。

在实践中，我们将通过诸如“假设 $A$ 为假”之类的短语来表明我们将使用此标准。这句话的意思是，推理暂时在$\mathscr{T}'$理论中进行，直到形式$B$中的两个定理和“不是$B$”被证明为止。当实现这一点后，就可以确定$\mathscr{T}$中的$A$是定理，这通常用诸如“现在这个（即前面的记号、$B$和“不是$B$”）是荒谬的；因而$A$是真的”这样的短语来表示。然后继续原来的理论$\mathscr{T}$。

¶ 作为这些方法的首次应用，让我们建立以下判据 ：

C16。 *如果$A$在$\mathscr{T}$中是关系，则*（不是$A$）$\Rightarrow A$ *在$\mathscr{T}$中是定理。*

假设“not not $A$”为真；那么我们必须证明$A$。假设 $A$ 为假。在这样定义的理论中，“非非$A$”和“非$A$”是定理，这是荒谬的；因而 $A$ 为真。

C17。 *如果$A$和$B$在$\mathscr{T}$中是关系，那么*

$$((\text{not } B) \Rightarrow (\text{not } A)) \Rightarrow (A \Rightarrow B)$$

*$\mathscr{T}$等于定理。*

假设 $(\text{not }B) \Rightarrow (\text{not }A)$ 为真。我们必须证明 $A \Rightarrow B$ 是正确的。假设 $A$ 为真，让我们证明 $B$ 为真。假设“not $B$”为真。那么“not $A$”就是真的，这是荒谬的。

III。 *方法案例分离。*这取决于以下规则：

C18。 *令$\mathscr{T}$中的$A$、$B$、$C$为关系。如果“$A$或$B$”$A \Rightarrow C$、$B \Rightarrow C$在$\mathscr{T}$中为定理，则$C$在$\mathscr{T}$中为定理。*

因为，到了S4，“$(A\text{ or }B) \Rightarrow (A\text{ or }C)$”和“$(C\text{ or }A) \Rightarrow (C\text{ or }C)$”在$\mathscr{T}$中是定理。通过S3和S1，可以得出$(A\text{ or }B) \Rightarrow C$在$\mathscr{T}$中是定理；因此结果。

To prove $C$ it is therefore enough, when we have at our disposal a theorem “$A$ or $B$”, first to prove $C$ by adjoining $A$ to the axioms of $\mathscr{T}$, and then to prove $C$ by adjoining $B$ to the axioms of $\mathscr{T}$. 这个方法的有趣特征在于，如果“$A$或$B$”为真，我们不能一般断言$A$为真或$B$为真。

特别地，通过C10，如果“$A \Rightarrow C$”和“$(\text{not }A) \Rightarrow C$”在$\mathscr{T}$中都是定理，则$C$在$\mathscr{T}$中是定理。

IV。 *辅助常数的方法。*这是基于以下规则：

C19。 *令$x$为字母，并令$A$和$B$为$\mathscr{T}$中的关系，这样：*

(1) *字母$x$不是$\mathscr{T}$的常数，并且不会出现在$B$中；*
(2) *$\mathscr{T}$中有项$T$，使得$(T|x)A$在$\mathscr{T}$中有定理。*

*令$\mathscr{T}'$为将$\mathscr{T}$的$A$与公理邻接而得到的理论。如果$B$在$\mathscr{T}'$中是定理，则$B$在$\mathscr{T}$中是定理。*

事实上，$A \Rightarrow B$ 是$\mathscr{T}$ 中的定理（演绎的标准）。由于$x$不是$\mathscr{T}$的常数，因此根据C3，$(T|x)(A \Rightarrow B)$在$\mathscr{T}$中等于定理。由于$x$没有出现在$B$中，所以通过CS5（§ 1, no. 2），$(T|x)(A \Rightarrow B)$与$((T|x)A) \Rightarrow B$相同。最后，$(T|x)A$在$\mathscr{T}$中是定理，因此$B$也是如此。

直观上，方法在于在序中使用任意对象$x$（*辅助常量*）来证明$B$，该对象应该被赋予某些属性，用$A$表示。 \* 对于例，在几何中的证明中，除其他外，还涉及线$D$，我们可以在这条线上“取”点$x$； 关系$A$则为$x \in D$。 \* 在序中，人们应该能够在证明的过程中使用被赋予某些属性的对象，显然这样的对象应该存在。 定理$(T|x)A$，称为合法性*定理，保证了这种存在。

在实践中，我们将通过诸如“让$x$成为一个对象，使得$A$”之类的短语来使用这个方法。与助词假设的方法相比，论证的结论不涉及$x$。

### 4.合取

设$A$，$B$为组合。大会

$$
\text{not } ((\text{not } A) \text{ or } (\text{not } B))
$$

将用“$A$和$B$”表示。

CS6。  令 $A$、$B$、$T$ 为组合，$x$ 为字母。  然后组装

$$
(T|x)(A\text{ and }B)
$$

与“$(T|x)A$和$(T|x)B$”相同。

这是 CS5 (§ 1, no. 2) 的直接的推论。

CF9。  如果$A$、$B$在$\mathscr{T}$中为关系，则“$A$和$B$”在$\mathscr{T}$中为关系（称为$A$和$B$的合取）。

这紧接着 CF1 和 CF2 (§ 1, no. 4)。

C20。  如果$A$、$B$在$\mathscr{T}$中为定理，则“$A$和$B$”在$\mathscr{T}$中为定理。

假设“$A$和$B$”为假，也就是说，

$$
\text{not not } ((\text{not } A) \text{ or } (\text{not } B))
$$

是真的。  由C16可知“$(\text{not } A)$或$(\text{not } B)$”，即$A \Longrightarrow (\text{not } B)$为真，因此“非$B$”为真；但这是荒谬的。  因此“$A$和$B$”为真。

C21。  如果$A$、$B$在$\mathscr{T}$中是关系，则

$$
(A\text{ and }B) \Longrightarrow A,\qquad (A\text{ and }B) \Longrightarrow B
$$

定理位于 $\mathscr{T}$ 中。

关系 $(\text{not } A) \Longrightarrow ((\text{not } A) \text{ or } (\text{not } B))$、$(\text{not } B) \Longrightarrow ((\text{not } A) \text{ or } (\text{not } B))$ 是 $\mathscr{T}$ 中的定理，由 S2 (no. 1) 和 C7 (no. 2) 组成。  现在 C11 的 $\mathscr{T}$ 中的 $((\text{not } A) \text{ or } (\text{not } B)) \Longrightarrow (\text{not } (A\text{ and }B))$ 是定理。  因此$(\text{not } A) \Longrightarrow (\text{not } (A\text{ and }B))$、$(\text{not } B) \Longrightarrow (\text{not } (A\text{ and }B))$在$\mathscr{T}$中是定理。  结果是应用 C17。

¶ 我们将用“$A$和$B$和$C$”（分别是“$A$或$B$或$C$”）关系“$A$和（$B$和$C$）”（分别表示） “$A$或（$B$或$C$）”）。更一般地说，如果

$$A_1, \quad A_2, \quad \ldots, \quad A_n$$

是关系，我们用“$A_1$和$A_2$，以及...和$A_p$”来表示关系，这是按照“$A_1$和$A_2$以及...和$A_h$”与“$A_1$”表示相同的关系的约定逐步构建的和（$A_2$ 和...和 $A_h$）”。 关系“$A_1$或$A_2$或...或$A_h$”的定义类似。 关系“$A_1$和$A_2$和...和$A_h$”在$\mathscr{T}$中是定理当且仅当关系$A_1$、$A_2$、...、$A_h$中的每一个在定理中$\mathscr{T}$。

由此可见，每个逻辑理论$\mathscr{T}$等价于一个至多有一个显式公理的逻辑理论$\mathscr{T}'$。如果 $\mathscr{T}$ 没有明确的公理，这一点是清楚的。如果 $\mathscr{T}$ 具有显式公理 $A_1$、$A_2$、...、$A_h$，则令 $\mathscr{T}'$ 为与 $\mathscr{T}$ 具有相同符号和概形的理论，以及显式公理“$A_1$ 和 $A_2$ 和 ... ” $A_h$”。立即可见，$\mathscr{T}$（或$\mathscr{T}'$）的每个公理都是$\mathscr{T}'$（或$\mathscr{T}$）的定理。

令$\mathscr{T}_0$为无显式公理的理论，其符号与$\mathscr{T}$相同，且S1、S2、S3、S4为其唯一的概形。然后研究原理中的$\mathscr{T}$约化，再到$\mathscr{T}_0$的研究：对于$\mathscr{T}$中的关系$A$为定理，存在公理$A_1$，$A_2$，...是充分必要的， $\mathscr{T}$的$A_h$使得$(A_1$和$A_2$以及...和$A_h) \Rightarrow A$是$\mathscr{T}_0$中的定理。这个条件显然已经足够了。反过来假设$A$是$\mathscr{T}$中的定理，令$A_1$、$A_2$、...、$A_h$为$\mathscr{T}$中证明中出现的$\mathscr{T}$的公理，则包含$A$。令$\mathscr{T}'$（或$\mathscr{T}''$）是从$\mathscr{T}_0$通过邻接公理$A_1$、$A_2$、...、$A_h$（分别是公理“$A_1$和$A_2$和...”构建的理论$A_h$”）。 $\mathscr{T}$中$A$的证明是$\mathscr{T}'$中$A$的证明，因而$A$在$\mathscr{T}'$中是定理，因此在$\mathscr{T}''$中，因为（如上所述） $\mathscr{T}'$ 和 $\mathscr{T}''$ 等效。根据演绎、$(A_1$和$A_2$以及...的标准，$A_h) \Rightarrow A$在$\mathscr{T}_0$中为定理。

如果$\mathscr{T}$是矛盾的，那么从前面所说的可知，在$\mathscr{T}$中存在$\mathscr{T}$和关系$R$的公理合取$A$，使得$A \Rightarrow (R$和（不是$R$））是定理在$\mathscr{T}_0$。因而

$$((\text{not } R) \text{ or } (\text{not not } R)) \Rightarrow (\text{not } A)$$

在$\mathscr{T}_0$中是定理，并且由于“（不是$R$）或（不是$R$）”在$\mathscr{T}_0$中是定理，所以“不是$A$”在$\mathscr{T}_0$中是定理。相反，如果存在$\mathscr{T}$的公理合取$A$，使得$\mathscr{T}_0$中的“非$A$”为定理，则$A$和“非$A$”在$\mathscr{T}$中为定理，因此$\mathscr{T}$是矛盾的。

### 5.等价

设$A$和$B$为组合。大会

$$(A \Rightarrow B) \text{ and } (B \Rightarrow A)$$

将用$A \Leftrightarrow B$表示。

CS7。 *令$A$、$B$、$T$为组合，并令$x$为字母。那么组装$(T|x)(A \Leftrightarrow B)$与$(T|x)A \Leftrightarrow (T|x)B$相同。*

这紧接着 CS5 (§ 1, no. 2) 和 CS6 (no. 4)。

CF10。 *如果$A$和$B$在$\mathscr{T}$中是关系，则$A \Leftrightarrow B$在* **T**中是关系。

这紧接着 CF5 (§ 1, no. 4) 和 CF9 (no. 4)。

¶ 如果$A \Leftrightarrow B$在$\mathscr{T}$中是定理，我们可以说$A$和$B$在$\mathscr{T}$中“等价”；如果$x$是一个不是$\mathscr{T}$常数的字母，并且如果$A$和$B$被视为$x$中的关系，则$\mathscr{T}$中每个满足一个的项也满足另一个。

¶ 由判据 C20, C21 (no. 4)可知，在序中，要证明形式$A \Leftrightarrow B$的$\mathscr{T}$中的定理，必须且充分能够证明$A \Rightarrow B$和$B \Rightarrow A$ $\mathscr{T}$。这通常是由 $\mathscr{T}$ 邻接公理 $A$ 推导出来的理论中的证明 $B$ 完成的，然后是由 $\mathscr{T}$ 邻接公理 $B$ 推导出来的理论中的证明 $A$ 来完成的。这些注立即引向下面的判据，我们将其证明留给读者：

C22。 *令$\mathscr{T}$中的$A$、$B$、$C$为关系。如果$A \Leftrightarrow B$在$\mathscr{T}$中是定理，则$B \Leftrightarrow A$在$\mathscr{T}$中是定理。如果$A \Leftrightarrow B$和$B \Leftrightarrow C$在$\mathscr{T}$中是定理，则$A \Leftrightarrow C$在$\mathscr{T}$中是定理。*

C23。 *令$A$、$B$等价于$\mathscr{T}$中的关系，令$C$等价于$\mathscr{T}$中的关系。那么以下是$\mathscr{T}$中的定理：*

$$(\text{not } A) \Leftrightarrow (\text{not } B); \qquad (A \Rightarrow C) \Leftrightarrow (B \Rightarrow C);$$
$$(C \Rightarrow A) \Leftrightarrow (C \Rightarrow B);$$
$$(A \text{ and } C) \Leftrightarrow (B \text{ and } C); \qquad (A \text{ or } C) \Leftrightarrow (B \text{ or } C).$$

C24。 *令$\mathscr{T}$中的$A$、$B$、$C$为关系。那么以下是$\mathscr{T}$中的定理：*

$$(\text{not not } A) \Leftrightarrow A; \qquad (A \Rightarrow B) \Leftrightarrow ((\text{not } B) \Rightarrow (\text{not } A));$$
$$(A \text{ and } A) \Leftrightarrow A; \qquad (A \text{ and } B) \Leftrightarrow (B \text{ and } A);$$
$$(A \text{ and } (B \text{ and } C)) \Leftrightarrow ((A \text{ and } B) \text{ and } C);$$
$$(A \text{ or } B) \Leftrightarrow \text{not } ((\text{not } A) \text{ and } (\text{not } B));$$
$$(A \text{ or } A) \Leftrightarrow A; \qquad (A \text{ or } B) \Leftrightarrow (B \text{ or } A);$$
$$(A \text{ or } (B \text{ or } C)) \Leftrightarrow ((A \text{ or } B) \text{ or } C);$$
$$(A \text{ and } (B \text{ or } C)) \Leftrightarrow ((A \text{ and } B) \text{ or } (A \text{ and } C));$$
$$(A \text{ or } (B \text{ and } C)) \Leftrightarrow ((A \text{ or } B) \text{ and } (A \text{ or } C));$$
$$(A \text{ and } (\text{not } B)) \Leftrightarrow \text{not } (A \Rightarrow B);$$
$$(A \text{ or } B) \Leftrightarrow ((\text{not } A) \Rightarrow B).$$

C25。 *如果$A$在$\mathscr{T}$中是定理并且$B$在$\mathscr{T}$中是关系，那么*

$$(A \text{ and } B) \Leftrightarrow B$$

* $\mathscr{T}$ 中的定理。如果“不是$A$”在$\mathscr{T}$中是定理，则$(A$或$B) \Rightarrow B$在$\mathscr{T}$中是定理。*

¶ *在原理中，从现在开始，级数、判据* C1 *到* C25 *将在没有参考的情况下使用。*

### 习题 {#ens-i-s3-exercises}

§ 3](exercises/s3/)参见[习题。

[^1]: 这个概形可以不使用字母$A$或缩写符号$\Rightarrow$来表达，如下：*每当我们有关系时，我们通过从左到右写，*$\vee$，$\neg$，得到定理， $\vee$，*然后给定关系三次*。读者可以按照习题类似的方式翻译其他概形的表达方式。
[^2]: 在日常用语中，字“或”根据上下文有两种不同的含义：当我们通过字“或”连接两个叙述时，我们可能意味着断言两者中的至少一个（也可能两者一起），或者我们可能意味着断言其中一个而排除另一个。
