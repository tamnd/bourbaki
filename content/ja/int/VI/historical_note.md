---
book: int
book_title: Integration
chapter: VI
chapter_title: VECTORIAL INTEGRATION
section: 0
section_title: Historical Note
kind: historical
lang: ja
source: int-i-vi
pdf_pages: 0463-0465
extraction: ocr
statements: 0
exercises: 0
content_sha256: d6323b79c771d4d68be834dca98aebda332fa298e51cc82d6a9bddb682623e08
translated_from: content/en/int/VI/historical_note.md
translation_method: google
source_content_sha256: ddd2484b153907abc4b504e7847024232e7bbd05fcbac91aba31ada63b157656
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: ff0d8fe6143fcade689ee1440b0fdf58f8bedb74c3973fc110a2176db2d0cb84
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

# 歴史注意

(注意 — ローマ数字は、この注意の最後にある参考文献を指します。)

19 世紀に「ベクトル計算」が開発されたため、ベクトル値の写像を積分する必要があるのが現在の慣例でしたが、それが有限次元空間での値と写像だけの問題である限り、この演算は問題を提起しませんでした。 問題。 It is only with Hilbert's spectral theory that one meets operations that lead naturally to a more general concept of integral: this theory in effect leads to associating, with every continuous Hermitian form $\Phi(x, y)$ on a Hilbert space $\mathbf{H}$, a family $(E(\lambda))_{\lambda \in \mathbf{R}}$ of orthogonal projectors having the property that, for every pair $(x, y)$ of vectors of $\mathbf{H}$, the function $\lambda \mapsto (E(\lambda)x|y)$ is of bounded variation and $\Phi(x, y) = \int \lambda d(E(\lambda)x|y)$; if one associates with $\Phi$ the Hermitian operator $A$ such that $\Phi(x, y) = (Ax|y)$, it was tempting to write the preceding formula as $A = \int \lambda dE(\lambda)$. しかし、バナッハ空間における写像と値の（「強力な」）積分の後で 1935 年頃から、人は次のような方法でベクトル値写像の積分 (またはベクトル測度に関する積分) を定義することに夢中になり始めました。先ほどのような公式を正当に書きます。 この拡大は、基本的にゲルファンド (III)、ダンフォード、ペティス (IV) および (V) によって達成されました。彼らの結果は、Banach 空間について記載されていますが、拡大するは、より一般的な局所凸型空間に対して問題なく適用されます。

体積を「スライス」に分解し、その体積の積分を各スライスの積分に還元し、その後 1 回の積分を行うという考え方は、無限小計算の始まり以来、分析で使用されてきました (カヴァリエリの「不可分なものの計算」は、この原理の最初の概要にすぎず、アルキメデスにまで遡ることができます (ヒストを参照)。 注意 (本 IV)、Chs. I–III))。 But in the classical applications, the 'slices' were always of a very special and very regular nature (most often open subsets of analytic surfaces, depending analytically on a parameter); it could scarcely have been otherwise in the absence of a general theory of integration. The general problem of the disintegration of a measure was posed and solved by von Neumann in 1932, in connection with ergodic theory (I); at about the same time (and independently) Kolmogoroff, while laying down axiomatic foundations for the Theory of Probability, was led to define in a general way the concept of 'conditional probability' and to prove its existence, a problem essentially equivalent to that of disintegration of a measure (II).

(I) J. von NEUMANN、「Zur Operatorenmethod in der Klassischen Mechanik」、Ann。 of Math.、(2)、33 (1932)、587 ～ 642 ページ。

(II) A. コルモゴロフ、Grundbegriffe der Wahrscheinlichkeitsrechnung、ベルリン (Springer)、1933 年。

(III)I。 GELFAND、Abstrakte Funktionen und lineare Operatoren、Mat. Sborn.、(N.S.)、4 (1938)、235 ～ 284 ページ。

(IV) N. DUNFORD、線形の均一性空間、Trans。アメール。数学。 Soc.、44 (1938)、305 ～ 356 ページ。

(V) N. ダンフォードと B. ペティス、加算可能写像上のリニア演算、トランス。アメール。数学。 Soc.、47 (1940)、323 ～ 392 ページ。
