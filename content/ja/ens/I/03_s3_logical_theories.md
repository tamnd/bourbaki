---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION OF FORMAL MATHEMATICS
section: 3
section_title: Logical theories
lang: ja
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
content_sha256: d4eabdac193ce5124cab829be17722b21a4dd7ef1e5bf765555bd7d708d99e50
translated_from: content/en/ens/I/03_s3_logical_theories.md
translation_method: google
source_content_sha256: 37ec32a3c0cdf2c61a57848be909293d325cc40d690c0e328f7cb619bf02c9e1
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 111dea2aa6f7ad31ef4ec52312e0fecc9958a2bc72d7950183452ab049ce7cc5
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 3. 論理理論

### 1. 公理

*論理理論* は、以下のスキーム S1 から S4 が暗黙の公理を提供する任意の理論 $\mathscr{T}$ です。

S1. *$A$ が $\mathscr{T}$ の関係である場合、関係 $(A$ または $A) \Rightarrow A$ は $\mathscr{T}$* [^1] の公理です。

S2. *$A$ と $B$ が $\mathscr{T}$ の関係である場合、関係 $A \Rightarrow (A$ または B) は $\mathscr{T}$ の公理です。

S3. *$A$ と $B$ が $\mathscr{T}$ の関係である場合、関係 $(A$ または $B) \Rightarrow (B$ または A) は $\mathscr{T}$ の公理です。

S4. *$A$、$B$、$C$が$\mathscr{T}$、関係の関係の場合*

$$(A \Rightarrow B) \Rightarrow ((C \text{ or } A) \Rightarrow (C \text{ or } B))$$

*は$\mathscr{T}$の公理です。*

これらのルールは実際にはスキームです。たとえば S2 についてこれを確認してみましょう。 $R$ を適用 S2 によって取得された関係とします。次に、$\mathscr{T}$ には関係 $A$ と $B$ があり、$R$ は関係 $A \Rightarrow (A$ または B) になります。 $T$ を $\mathscr{T}$ の項とし、$x$ を文字とし、$A'$ と $B'$ を関係 $(T|x)A$ と $(T|x)B$ とします。この場合、$(T|x)R$ は $A' \Rightarrow (A'$ または $B')$ と同じであるため、適用 S2 によって取得できます。

直観的には、ルール S1 から S4 は、数学の通常の言語 [^2] で「または」および「暗示する」という単語に付加される意味を単に表現しているだけです。

論理的な理論 $\mathscr{T}$ が矛盾している場合、* $\mathscr{T}$ のすべての関係は $\mathscr{T}$ の定理になります。* $A$ は $\mathscr{T}$ の関係であり、$A$ と「$A$ ではない」とします。は $\mathscr{T}$ の定理であり、$B$ は $\mathscr{T}$ の任意の関係とします。 S2 により、($A$ ではない) $\Rightarrow$ (($A$ または $B$ ではない) は $\mathscr{T}$ の定理です。したがって、C1 (§ 2, no. 2) により、「($A$) または $B$」、つまり $A \Rightarrow B$ は、$\mathscr{T}$ の定理になります。 C1 を 2 回目に適用すると、$B$ は $\mathscr{T}$ の定理であることがわかります。

¶ *今後、$\mathscr{T}$ は論理値理論を表します。*

### 2. 最初帰結

C6. ※$\mathscr{T}$の$A$、$B$、$C$を関係とします。 $A \Rightarrow B$ と $B \Rightarrow C$ が $\mathscr{T}$ の定理である場合、$A \Rightarrow C$ は $\mathscr{T}$ の定理です。*

なぜなら、$(B \Rightarrow C) \Rightarrow ((A \Rightarrow B) \Rightarrow (A \Rightarrow C))$ は、S4 の「$A$ ではない」による $\mathscr{T}$、置き換えることによる、$A$ による $B$、$B$ による $C$、および $C$ の公理です。 C1 (§ 2, no. 2) により、$(A \Rightarrow B) \Rightarrow (A \Rightarrow C)$ は $\mathscr{T}$ の定理になります。 C1 をさらに適用すると、証明が完了します。

C7. *$A$と$B$が$\mathscr{T}$の関係である場合、$B \Rightarrow (A$またはB)は$\mathscr{T}$の定理です。

$B \Rightarrow (B$ または A) と $(B$ または $A) \Rightarrow (A$ または B) は、S2 と S3 により $\mathscr{T}$ の公理です。次にC6を使用します。

C8. *$A$が$\mathscr{T}$の関係である場合、$A \Rightarrow A$は$\mathscr{T}$の定理です。

$A \Rightarrow (A$ または A) および $(A$ または $A) \Rightarrow A$ は S2 と S1 による公理です。次にC6を使用します。

C9. *$A$ が $\mathscr{T}$ の関係および $B$ 定理である場合、$A \Rightarrow B$ は $\mathscr{T}$ の定理です。

$B \Rightarrow ((\text{not } A)$ または B) は C7 によって定理であるため、「($A$ ではない) または $B$」、つまり $A \Rightarrow B$ は C1 によって定理になります。

C10. *$A$ が $\mathscr{T}$ の関係である場合、「$A$ または ($A$ ではない)」は $\mathscr{T}$ の定理になります。

「($A$ではない)または$A$」の場合、C8では定理です。ここでは S3 と C1 を使用します。

C11. *$A$ が $\mathscr{T}$ の関係である場合、「$A \Rightarrow$ ($A$ ではない)」は $\mathscr{T}$ の定理です。

この場合、関係は「($A$ ではない) または ($A$ ではない)」となり、結果は C10 に従います。

C12. *Let $A$ and $B$ be two 関係 in $\mathscr{T}$.それでは関係*

$$(A \Rightarrow B) \Rightarrow ((\text{not } B) \Rightarrow (\text{not } A))$$

*is 定理 in $\mathscr{T}$.*

のために

$$((\text{not } A) \text{ or } B) \Rightarrow ((\text{not } A) \text{ or } (\text{not not } B))$$

is 定理, by C11, S4 and C1.一方、

$$((\text{not } A) \text{ or } (\text{not not } B)) \Rightarrow ((\text{not not } B) \text{ or } (\text{not } A))$$

は S3 による公理です。したがって、

$$((\text{not } A) \text{ or } B) \Rightarrow ((\text{not not } B) \text{ or } (\text{not } A))$$

はC6の定理です。したがって、結果は次のとおりです。

C13. *Let $A$, $B$, $C$ be 関係 in $\mathscr{T}$. If $A \Rightarrow B$ is 定理 in $\mathscr{T}$, then $(B \Rightarrow C) \Rightarrow (A \Rightarrow C)$ is 定理 in $\mathscr{T}$.*

For $(\text{not } B) \Rightarrow (\text{not } A)$ is 定理, by C12 and C1. Therefore $(C \text{ or } (\text{not } B)) \Rightarrow (C \text{ or } (\text{not } A))$ is 定理, by S4 and C1. By a double application of S3 and C6 we infer that

$$((\text{not } B) \text{ or } C) \Rightarrow ((\text{not } A) \text{ or } C)$$

定理です。 but this is the given 関係.

¶ *From now on, we shall generally use* C1 *and* C6 *without quoting them explicitly.*

### 3. 方法/証明

I。 *方法 of the auxiliary 仮定.* This rests on the following rule :

C14 (*Criterion of deduction*). *Let $A$ be 関係 in $\mathscr{T}$, and let $\mathscr{T}'$ be 理論 obtained by adjoining $A$ to the axioms of $\mathscr{T}$. If $B$ is 定理 in $\mathscr{T}'$, then $A \Rightarrow B$ is 定理 in $\mathscr{T}$.*

$B$が出現する$\mathscr{T}'$の$B_1$、$B_2$、...、$B_n$を証明とします。 $\mathscr{T}$ では関係 $A \Rightarrow B_k$ が定理であることを段階的に示していきます。これが$B_i$より前の関係でも成立していると仮定し、$A \Rightarrow B_i$が$\mathscr{T}$の定理であることを示しましょう。 $B_i$ が $\mathscr{T}'$ の公理である場合、$B_i$ は $\mathscr{T}$ の公理か、$A$ のいずれかです。どちらの場合も、$A \Rightarrow B_i$ は、適用 C9 または C8 によって、$\mathscr{T}$ の定理になります。 $B_i$ の前に関係 $B_j$ と $B_j \Rightarrow B_i$ がある場合、$A \Rightarrow B_j$ と $A \Rightarrow (B_j \Rightarrow B_i)$ は $\mathscr{T}$ の定理であることがわかります。したがって、$(B_j \Rightarrow B_i) \Rightarrow (A \Rightarrow B_i)$ は C13 による $\mathscr{T}$ の定理です。したがって、C6 により、$A \Rightarrow (A \Rightarrow B_i)$、つまり「$(\text{not } A)$ または $(A \Rightarrow B_i)$」は、$\mathscr{T}$ では定理となり、したがって S3 により「$(A \Rightarrow B_i)$ または $(\text{not } A)$」も同様となります。さて、$(\text{not } A) \Rightarrow ((\text{not } A) \text{ or } B_i)$、つまり$(\text{not } A) \Rightarrow (A \Rightarrow B_i)$は、S2による$\mathscr{T}$の定理です。 S4 を適用すると、次のことがわかります。

$$((A \Rightarrow B_i) \text{ or } (\text{not } A)) \Rightarrow ((A \Rightarrow B_i) \text{ or } (A \Rightarrow B_i))$$

は $\mathscr{T}$ の定理であるため、「$(A \Rightarrow B_i)$ または $(A \Rightarrow B_i)$」は $\mathscr{T}$ の定理になります。 S1 により、$A \Rightarrow B_i$ は $\mathscr{T}$ では定理となる結論するです。

実際には、「$A$ が true であると仮定する」などの表現でこの基準を使用することを示します。このフレーズは、関係 $B$が証明されるまで、当面推論は理論 $\mathscr{T}'$で実行されることを意味します。これが達成されると、$A \Rightarrow B$ が $\mathscr{T}$ の定理であることが確立され、その後、理論 $\mathscr{T}'$ を放棄したことを示すことなく、$\mathscr{T}$ で推論を続けます。新しい公理として導入された関係 $A$ を *補助仮定* と呼びます。 \* たとえば、「$x$ を実数にしましょう」と言うとき、関係 「$x$ は実数」が補助的な仮定である理論を構築しています。 \*

II. *方法の不合理な削減。* これは次の規則に基づいています。

C15. *$A$を$\mathscr{T}$の関係とし、$\mathscr{T}'$を$\mathscr{T}$の公理に「$A$ではない」公理*を隣接させることによって得られる理論とする。 $\mathscr{T}'$ が矛盾している場合、$A$ は $\mathscr{T}$ の定理になります。*

$A$ は $\mathscr{T}'$ の定理です。その結果、(補助仮定の方法)「($A$ではない)$\Rightarrow A$」は$\mathscr{T}$の定理になります。 S4までに、

$$(A \text{ or } (\text{not } A)) \Rightarrow (A \text{ or } A)$$

$\mathscr{T}$の定理です。 C10によると、「$A$または$A$」は$\mathscr{T}$の定理です。次に S1 を使用します。

実際には、「$A$ が偽であると仮定する」などの表現でこの基準を使用することを示します。このフレーズは、形$B$の2つの定理と「$B$ではない」ことが証明されるまで、当面推論は理論$\mathscr{T}'$で実行されることを意味します。これが達成されると、$A$ は $\mathscr{T}$ の定理であることが確立され、これは通常、「これ (つまり、前の記法、$B$、および「$B$ ではない」) は不合理です。従って、$A$ は真です」のようなフレーズで示されます。その後、元の理論 $\mathscr{T}$ に続きます。

¶ これら方法の最初の応用として、次の基準を確立しましょう。

C16. *$A$ が $\mathscr{T}$ の関係である場合、* ($A$ ではない) $\Rightarrow A$ * は $\mathscr{T}$ の定理です。*

なぜなら、「$A$ではない」が真であると仮定してください。次に、$A$ を証明する必要があります。 $A$ が false であるとします。このように定義された理論では、「$A$ ではない」と「$A$ ではない」は定理であり、これは不合理です。従って、$A$ は true です。

C17. *$A$ と $B$ が $\mathscr{T}$ の関係である場合、*

$$((\text{not } B) \Rightarrow (\text{not } A)) \Rightarrow (A \Rightarrow B)$$

*は $\mathscr{T}$ の定理です。*

$(\text{not }B) \Rightarrow (\text{not }A)$ が true であると仮定します。 $A \Rightarrow B$ が真実であることを示さなければなりません。 $A$ が true であると仮定し、$B$ が true であることを示しましょう。 「$B$ではない」が真実だと仮定します。そうすると「$A$ではない」が真となり、これは不合理です。

III。 *方法場合の分離。* これは次の規則に基づいています。

C18. ※$A$、$B$、$C$を$\mathscr{T}$の関係とします。 「$A$ または $B$」$A \Rightarrow C$、$B \Rightarrow C$ が $\mathscr{T}$ の定理である場合、$C$ は $\mathscr{T}$ の定理です。

なぜなら、S4 によれば、「$(A\text{ or }B) \Rightarrow (A\text{ or }C)$」と「$(C\text{ or }A) \Rightarrow (C\text{ or }C)$」は $\mathscr{T}$ の定理であるからです。 S3 と S1 により、$(A\text{ or }B) \Rightarrow C$ は $\mathscr{T}$ の定理であることがわかります。したがって結果です。

したがって、$C$ を証明するには、定理 「$A$ または $B$」が自由に使えるとき、まず$A$ を$\mathscr{T}$ の公理に隣接させて$C$ を証明し、次に$B$ を公理に隣接させて$C$ を証明すれば十分です。 $\mathscr{T}$ の公理。この方法の興味深い特徴は、「$A$ または $B$」が真である場合、できないは一般に、$A$ が真であるか、$B$ が真であると主張するという事実にあります。

特に、C10 では、「$A \Rightarrow C$」と「$(\text{not }A) \Rightarrow C$」が両方とも $\mathscr{T}$ の定理である場合、$C$ は $\mathscr{T}$ の定理になります。

IV。 *補助定数の方法* これは次の規則に基づいています。

C19. *$x$ を文字とし、$A$ と $B$ を $\mathscr{T}$ の関係とします:*

(1) *文字 $x$ は $\mathscr{T}$ の定数ではなく、$B$ には現れません。*
(2) *$\mathscr{T}$ には項 $T$ があり、$(T|x)A$ は $\mathscr{T}$ では定理になります。*

*$\mathscr{T}'$を$\mathscr{T}$の公理に$A$を隣接させて得られる理論とする。 $B$ が $\mathscr{T}'$ の定理である場合、$B$ は $\mathscr{T}$ の定理です。*

確かに、$A \Rightarrow B$は$\mathscr{T}$（減算基準）では定理です。 $x$ は $\mathscr{T}$ の定数ではないため、C3 により $(T|x)(A \Rightarrow B)$ は $\mathscr{T}$ の定理になります。 $x$は$B$には現れないため、CS5(§ 1, no. 2)では$(T|x)(A \Rightarrow B)$は$((T|x)A) \Rightarrow B$と同一です。最後に、$(T|x)A$ は $\mathscr{T}$ の定理であるため、$B$ も同様です。

直観的には、方法は、順序で、$B$ を証明するために、$A$ で示される特定の特性を備えていると考えられる任意のオブジェクト $x$ (*補助定数*) を使用することから構成されます。 \* たとえば、とりわけ線 $D$ を含む幾何学の証明では、この線上で点 $x$ を「取得」できます。 関係 $A$ は $x \in D$ になります。 \* In 順序 that one should be able to use an object endowed with certain properties during the course of 証明, it is clearly necessary that such objects should exist. 定理 $(T|x)A$ は、正当性 * の *定理と呼ばれ、この存在を保証します。

実際には、この方法を「$x$ を $A$ のようなオブジェクトにしましょう」のようなフレーズで使用することを示します。補助的な仮定の方法とは対照的に、議論の結論には$x$は含まれません。

### 4. 接続詞

$A$、$B$ をアセンブリとします。集会

$$
\text{not } ((\text{not } A) \text{ or } (\text{not } B))
$$

は「$A$と$B$」で表されます。

CS6。  $A$、$B$、$T$ をアセンブリ、$x$ を文字としましょう。  それからアセンブリ

$$
(T|x)(A\text{ and }B)
$$

「$(T|x)A$と$(T|x)B$」は同じです。

CS5(§ 1, no. 2)の明らか帰結です。

CF9。  $A$、$B$が$\mathscr{T}$の関係であれば、「$A$と$B$」は$\mathscr{T}$の関係になります（$A$と$B$の結合と呼ばれます）。

これは、CF1 と CF2 (§ 1, no. 4) の直後に続きます。

C20。  $A$、$B$が$\mathscr{T}$の定理であれば、「$A$、$B$」は$\mathscr{T}$の定理になります。

「$A$ と $B$」が false であると仮定します。つまり、

$$
\text{not not } ((\text{not } A) \text{ or } (\text{not } B))
$$

それは本当です。  By C16, “$(\text{not } A)$ or $(\text{not } B)$”, that is to say, $A \Longrightarrow (\text{not } B)$ is true, hence “not $B$” is true;しかし、これは不合理です。  したがって、「$A$ と $B$」は真です。

C21.  If $A$, $B$ are 関係 in $\mathscr{T}$, then

$$
(A\text{ and }B) \Longrightarrow A,\qquad (A\text{ and }B) \Longrightarrow B
$$

は $\mathscr{T}$ の定理です。

関係 $(\text{not } A) \Longrightarrow ((\text{not } A) \text{ or } (\text{not } B))$、$(\text{not } B) \Longrightarrow ((\text{not } A) \text{ or } (\text{not } B))$ は、S2 (no. 1) と C7 (no. 2) により、$\mathscr{T}$ の定理です。  現在、$((\text{not } A) \text{ or } (\text{not } B)) \Longrightarrow (\text{not } (A\text{ and }B))$ は C11 により $\mathscr{T}$ の定理です。  したがって、$(\text{not } A) \Longrightarrow (\text{not } (A\text{ and }B))$、$(\text{not } B) \Longrightarrow (\text{not } (A\text{ and }B))$は、$\mathscr{T}$の定理です。  結果は適用 C17 に続きます。

¶ 「$A$ および $B$ および $C$」 (それぞれ「$A$ または $B$ または $C$」) 関係 「$A$ および ($B$ および $C$)」 (それぞれ 「$A$ または($B$ または $C$)」)。より一般的に言えば、

$$A_1, \quad A_2, \quad \ldots, \quad A_n$$

関係は、「$A_1$ と $A_2$ と ... と $A_p$」 関係で表します。これは、「$A_1$ と $A_2$ と ... と $A_h$」 は、同じ関係を表すという規則によって段階的に構築されます。 "$A_1$ and ($A_2$ and ... and $A_h$)". 関係 「$A_1$ or $A_2$ or ... or $A_h$」も同様に定義されます。 関係 「$A_1$ と $A_2$ と ... と $A_h$」は、関係 $A_1$、$A_2$、...、$A_h$ がそれぞれ定理である場合に限り、$\mathscr{T}$ の定理になります$\mathscr{T}$に。

したがって、すべての論理理論 $\mathscr{T}$ は、明示的な公理を 1 つだけ持つ論理理論 $\mathscr{T}'$ と同等になります。 This is clear if $\mathscr{T}$ has no explicit axiom. $\mathscr{T}$ に明示的な公理 $A_1$、$A_2$、...、$A_h$ がある場合、$\mathscr{T}'$ を $\mathscr{T}$ と同じ符号とスキームを持つ理論とし、明示的な公理 "$A_1$ と $A_2$ そして ... そして$A_h$」。 $\mathscr{T}$ (それぞれ $\mathscr{T}'$) のすべての公理は、$\mathscr{T}'$ (それぞれ $\mathscr{T}$) の定理であることがすぐにわかります。

$\mathscr{T}_0$ を、$\mathscr{T}$ と同じ符号を持つ明示的な公理を持たない理論とし、唯一のスキームとして S1、S2、S3、S4 とします。 次に、$\mathscr{T}$ 簡約するの研究は、原則として $\mathscr{T}_0$ の研究に続きます。 関係 $A$ が $\mathscr{T}$ で定理となるためには、公理 $A_1$, $A_2$, ..., $A_h$ が存在することが必要かつ十分です。 $\mathscr{T}$ の場合、$(A_1$ と $A_2$ そして ... そして $A_h) \Rightarrow A$ は、$\mathscr{T}_0$ では定理になります。 明らかにこれ条件で十分です。 逆に、$A$ が$\mathscr{T}$ の定理であると仮定し、$A_1$、$A_2$、...、$A_h$ を、$A$ を含む$\mathscr{T}$ の証明に現れる$\mathscr{T}$ の公理とします。 Let $\mathscr{T}'$ (resp. $\mathscr{T}''$) be 理論 constructed from $\mathscr{T}_0$ by adjoining the axioms $A_1$, $A_2$, ..., $A_h$ (resp. the axiom "$A_1$ and $A_2$ and ... and $A_h$」）。 $\mathscr{T}$ の $A$ の証明は、$\mathscr{T}'$ の $A$ の証明です。従って、(上で述べたように) $\mathscr{T}'$ と $\mathscr{T}''$ は同等であるため、$A$ は $\mathscr{T}'$ の定理となり、その結果、$\mathscr{T}''$ の定理になります。 減算基準では、$(A_1$と$A_2$と...と$A_h) \Rightarrow A$は、$\mathscr{T}_0$の定理になります。

If $\mathscr{T}$ is contradictory, then it follows from what has been said that there exists a conjunction $A$ of axioms of $\mathscr{T}$ and 関係 $R$ in $\mathscr{T}$ such that $A \Rightarrow (R$ and (not $R$)) is 定理 in $\mathscr{T}_0$.従って

$$((\text{not } R) \text{ or } (\text{not not } R)) \Rightarrow (\text{not } A)$$

は$\mathscr{T}_0$の定理で、「($R$ではない)または($R$ではない)」は$\mathscr{T}_0$では定理であるため、「$A$ではない」は$\mathscr{T}_0$では定理です。逆に、「$A$ではない」が$\mathscr{T}_0$で定理となるような$\mathscr{T}$の公理の論理積$A$が存在する場合、$A$と「$A$ではない」は$\mathscr{T}$で定理となるため、$\mathscr{T}$矛盾しています。

### 5. 同値

$A$ と $B$ をアセンブリとします。集会

$$(A \Rightarrow B) \text{ and } (B \Rightarrow A)$$

は$A \Leftrightarrow B$で表されます。

CS7。 *$A$、$B$、$T$ をアセンブリ、$x$ を文字とします。この場合、アセンブリ $(T|x)(A \Leftrightarrow B)$ は $(T|x)A \Leftrightarrow (T|x)B$ と同一になります。*

これは、CS5 (§ 1, no. 2) と CS6 (no. 4) の直後に続きます。

CF10。 *$A$ と $B$ が $\mathscr{T}$ の関係である場合、$A \Leftrightarrow B$ は * **T** の関係です。

これは、CF5 (§ 1, no. 4) と CF9 (no. 4) の直後に続きます。

¶ $A \Leftrightarrow B$ が $\mathscr{T}$ の定理である場合、$A$ と $B$ は $\mathscr{T}$ で *同等* であると言えます。 $x$ が $\mathscr{T}$ の定数ではない文字で、$A$ と $B$ が $x$ の関係とみなされる場合、$\mathscr{T}$ のすべての項のうち、一方を満たすものは他方も満たします。

¶ 基準 C20、C21 (no. 4) から、順序で形 $A \Leftrightarrow B$ の $\mathscr{T}$ で定理を証明するには、$\mathscr{T}$ で $A \Rightarrow B$ と $B \Rightarrow A$ を証明できれば必要十分であることがわかります。これは、公理 $A$ に隣接して $\mathscr{T}$ から推論された理論の証明 $B$ によって行われ、次に公理 $\mathscr{T}$ から推論された理論の証明 $A$ によって行われます。 $B$。これら注意はすぐに次の基準につながりますが、その証明については読者にお任せします。

C22. ※$A$、$B$、$C$を$\mathscr{T}$の関係とします。 $A \Leftrightarrow B$ が $\mathscr{T}$ の定理である場合、$B \Leftrightarrow A$ は $\mathscr{T}$ の定理です。 $A \Leftrightarrow B$ と $B \Leftrightarrow C$ が $\mathscr{T}$ の定理である場合、$A \Leftrightarrow C$ は $\mathscr{T}$ の定理です。*

C23. *$A$、$B$ を $\mathscr{T}$ の関係と同等とし、$C$ を $\mathscr{T}$ の関係とします。次に、以下は $\mathscr{T}$ の定理です:*

$$(\text{not } A) \Leftrightarrow (\text{not } B); \qquad (A \Rightarrow C) \Leftrightarrow (B \Rightarrow C);$$
$$(C \Rightarrow A) \Leftrightarrow (C \Rightarrow B);$$
$$(A \text{ and } C) \Leftrightarrow (B \text{ and } C); \qquad (A \text{ or } C) \Leftrightarrow (B \text{ or } C).$$

C24. ※$\mathscr{T}$の$A$、$B$、$C$を関係とします。次に、以下は $\mathscr{T}$ の定理です:*

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

C25。 *$A$ が $\mathscr{T}$ の定理で、$B$ が $\mathscr{T}$ の関係である場合、*

$$(A \text{ and } B) \Leftrightarrow B$$

*は$\mathscr{T}$の定理です。 「$A$ ではない」が $\mathscr{T}$ の定理である場合、$(A$ または $B) \Rightarrow B$ は $\mathscr{T}$ の定理になります。*

¶ *原則として、この系列の残りの部分では、基準* C1 *から* C25 *が参照せずに使用されます*。

### 練習問題 {#ens-i-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。

[^1]: このスキームは、文字 $A$ や省略記号 $\Rightarrow$ を使用せずに、次のように表現できます。 * 関係があるときは、左から右に $\vee$、$\neg$、$\vee$、 * 続いて、指定された関係を 3 回* 書くことにより、定理が得られます。 The reader may, as an exercise, translate in a similar way the expressions of the other schemes.
[^2]: In everyday speech, the word "or" has two different meanings, according to the context : when we link two statements by the word "or" we may mean to assert at least one of the two (and possibly both together), or we may mean to assert one to the exclusion of the other.
