---
book: hist
book_title: Elements of the History of Mathematics
chapter: "1"
chapter_title: ELEMENTS OF THE HISTORY OF MATHEMATICS
section: 11
section_title: Uniform Spaces
lang: ja
source: hist
pdf_pages: 0147-0148
extraction: ocr
statements: 0
exercises: 0
content_sha256: 628b0fce48463761304cd3371844e960a2ba6b8ccdb5c4a82b744628414e233f
translated_from: content/en/hist/1/11_s11_uniform_spaces.md
translation_method: google
source_content_sha256: 2860052876fd130ce2e248a166f6a973e304ef320bb3054ac1d9d92b237812ff
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: fa3e8772f3b9820c15e624a7bcced03e874fbb3ae67fa0b306749a1f47b12cc2
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 11. 制服空間。

一様な空間に関係する主要な概念と命題は、実変数の理論から少しずつ出てきて、系統的に研究されるようになったのはつい最近のことである。 コーシーは、系列 (cf. p. 153) の集合を厳密に理論に引き上げようとして、数列 $(a_n)$ の収束に必要かつ十分な条件が、彼が明白であると考えていたと思われる原則を出発点として点としました。 $n$ が十分大きいである場合、$|a_{n+p} - a_n|$ は任意に小さくなければなりません (たとえば ([56 a], (2), v. VII、p. 267))。 ボルツァーノ [27 c] とともに、彼は間違いなくこの原則を明確に述べ、その重要性を認識した最初の一人でした。 よって 「コーシー 数列」という名前は、問題の満たす条件と拡大から数列までに実数の数列に与えられました。 $n$ が十分大きいの場合、$x_{n+p}$ と $x_n$ の間の距離が任意に小さくなるように、メトリック空間の点の $(x_n)$。そこから最終的に、制服空間のコーシー 数列を一般化するために「コーシー フィルター」という名前が付けられました。

その後、実数の直感的な概念では満足できなくなり、位数で分析に強固な基盤を与えるために合理的な数から始まる定義する実数が求められたとき、19世紀後半に提案された定義の中で最も実りあるものを提供したのはまさにコーシー原理でした。それはカントールの定義 ([47], pp. 93-96) (とりわけ、カントールの考えから、ハイネ [154 b] によって、そして独立してメレーによって開発された) であり、これによれば、すべてのコーシー 数列 (「基本的な数列」) に対して実数対応するが作成されます。カントールの用語) 理性数; $|a_n - b_n|$ が零になる傾向がある場合、同じ実数は、有理数数 $(a_n)$ と $(b_n)$ の 2 つのコーシー 数列に対して対応するになりますが、この場合のみです。ここでの本質的な考え方は、ある点の見方からすれば、有理数数の集合$\mathbf{Q}$は「不完全」であり、実数の集合は$\mathbf{Q}$を「完成」させることで導き出される「完全な」集合であるということです。

一方、ハイネは、主にヴァイエルシュトラスとカントールの考えに触発された研究で、1 つ以上の実変数の数値写像の定義する一様連続性を初めて発見し [154 a]、$\mathbf{R}$ の閉じた境界区間上で連続するすべての数値写像がそこで一様連続であることを証明しました [154 b]。 「ハイネの定理」です。この結果は、$\mathbf{R}$ (「Borel-Lebesgue 定理」、cf. p. 141) の閉じた有界区間のコンパクトさに関連しており、彼の定理の Heine によって与えられた証明も、いくつかの変更を加えて Borel-Lebesgue を証明するために使用できます。 定理 (これが、この定理に「ハイネ・ボレル定理」という名前を付ける十分な理由になると何人かの著者には思われました)。

これらのアイデアのうち、より一般的な空間への拡大は、最初にいくつかの特殊なケースが検討され、次に一般的に距離 (点、満たすの特定の公理の対の数値写像) が与えられ、同時に定義するが与えられる計量空間が検討されたときに作成されました。 位相とユニフォーム構造。これら空間のうちの一般的な定義を最初に述べたフレシェは、コーシーの原理 [115 a] の重要性を認識し、プレコンパクト (または「完全に有界」 [115 a および b]) 空間のすべての計量空間、概念についても導入しました。ハウスドルフは、彼の「メンゲンレーレ」[152 a および b] で、多くの理論の計量空間を開発しましたが、特に、これらの空間に、上で検討したカントール構成を適用できることを認識し、すべての非「完全」計量空間について推定できることを認識しました（つまり、コーシーの原則は無効です)、「完全な」指標空間。

メトリクス空間は、特定の種類の「均一空間」です。ユニフォーム空間は、A によって最近一般的な方法で定義されただけです。 ヴァイル [330 b]。 以前は、計量空間が扱われている場合に、概念の使い方と「均一構造」を参照する結果しか知られていませんでした。これは、距離が実際には役に立たない問題において、位相に関する多くの現代の研究において計量または計量可能空間 (特にコンパクト計量可能空間) が重要な役割を果たしていることを説明しています。 Once the definition of uniform spaces is stated, there is no difficulty (especially when the notion of filter is also available) in extending to these spaces nearly all the theory of metric spaces, as it is stated for example by Hausdorff (and to extend in the same way, for example, to all compact spaces, the results set out for compact metric spaces in the Topology of Alexandroff-Hopf [4]). 特に、均一空間の完成定理は、カントールの構成を実数に転置したものに他なりません。
