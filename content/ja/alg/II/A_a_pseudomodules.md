---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 0
section_title: Pseudomodules
appendix: true
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 378-379, 425
pdf_pages: 0402-0403, 0449-0449
extraction: ocr
subsections:
    - "no": 1
      title: ADJUNCTION OF A UNIT ELEMENT TO A PSEUDO-RING
      page: 378
      pdf_page: 402
    - "no": 2
      title: PSEUDOMODULES
      page: 378
      pdf_page: 402
statements: 0
exercises: 1
content_sha256: 5fa5c5588a55a43921a3984eb8e6bda8f97d3cd993d8676f830fe2648f7f4405
translated_from: content/en/alg/II/A_a_pseudomodules.md
translation_method: google
source_content_sha256: db883a717633a15e64137f982b71d8ce6f40a59783e9d1c7d5ac706248c39106
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 78ecdfd53924c02f1aa87d86e159a72aa74daf26d166519e1b32e698c1066880
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 付録

# 擬加群

### 1.  単位元の随伴を疑似リングに

A を擬似リング (I, § 8, no. 1) とします。 集合 $A' = \mathbf{Z} \times A$ に、定義する次の合成の法則:

$$
\begin{cases}
(m, a) + (n, b) = (m + n, a + b) \\
(m, a)(n, b) = (mn, mb + na + ab).
\end{cases}
$$

これら 2 つの法則と合成の $A'$ は環で、元 $(1, 0)$ は単位元であることがすぐに検証されます。 集合 $\{0\} \times A$ は、$A'$ の両側イデアルであり、$i : x \mapsto (0, x)$ は、サブ擬似リング $\{0\} \times A$ 上の擬似リング A の同型であり、これによって A と $\{0\} \times A$ が識別されます。 $A'$は、擬似環Aに単位元を隣接させて派生した環と呼ばれます。

A がすでに単位元 $\varepsilon$ を持っている場合、$A'$ の元 $e = (0, \varepsilon)$ は $A'$ の所属から中心のべき等です。

$$
A = eA' = A'e.
$$

この場合、$(eA', (1 - e)A')$ は $A'$ の直接の分解 (I, § 8, no. 11) であり、環 $(1 - e)A'$ は $\mathbf{Z}$ と同型です。

### 2. 擬加群

単位元の有無にかかわらず、疑似環 A が与えられると、A 上の左擬加群は可換群 E (加法的に書かれた) であり、A を演算子の集合と § 1, no. 1、定義 1 の満たす公理 $(\mathrm{M}_I), (\mathrm{M}_{II})$ および $(\mathrm{M}_{III})$ として認めます。 A 上の擬加群も同様に定義されます。

$A'$ を、単位元を A に隣接させることで得られる環とします。 E が A 上で左擬加群である場合、E 上の左の $A'$ モジュール構造は、すべての $x \in E$ とすべての元 $(n, a) \in A'$ について、次のように書くことによってそれに関連付けられます。

$$
(n, a) . x = nx + ax.
$$

§ 1, no. 1、定義 1 の公理 $(\mathrm{M}_I)$ から $(\mathrm{M}_{IV})$ は直ちに検証されます。

さらに、この加群構造の演算子の集合を $\{0\} \times A$ ($A$ で識別される) に制限すると、最初に与えられた $E$ 擬加群構造が得られます。

$E$ の部分集合 $M$ が擬加群 $E$ の演算子を使用して部分群となる場合 (この場合、誘導される構造も明らかに $A$ よりも左擬加群構造になります)、次のことが必要かつ十分です。 $M$ は、付随した $A'$ モジュール $E$ の部分加群であり、このサブ $A'$ モジュールは擬加群 $M$ に関連付けられます。さらに、商 $A'$ モジュール $E/M$ は、演算子 $E/M$ を使用して剰余群に関連付けられます。これは明らかに $A$ よりも擬加群です。

$E, F$ が $A$ 上の 2 つの擬加群である場合、演算子を持つ群の準同型 $E \to F$ は、擬加群にそれぞれ関連付けられた $A'$ モジュールの $A'$ 線形マッピング $E \to F$ と同一です。 $E$と$F$。 $(E_i)_{i \in I}$ が $A$ 上の擬加群の族である場合、演算子 $\prod_{i \in I} E_i$ と $\bigoplus_{i \in I} E_i$ を持つ群は $A$ 上の擬加群であり、付随した $A'$ モジュールはそれぞれ積と関連する $A'$ モジュール $E_i$ の直和。 擬加群の逆および直接極限にも同様の結果があります。したがって、$A$ 上の擬加群の理論は、完全に $A'$ モジュールのものに削減できます。

### 練習問題 {#alg-ii-a0-exercises}

[練習問題付録 0](exercises/a0/)を参照してください。
