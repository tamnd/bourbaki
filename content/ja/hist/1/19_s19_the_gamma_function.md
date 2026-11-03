---
book: hist
book_title: Elements of the History of Mathematics
chapter: "1"
chapter_title: ELEMENTS OF THE HISTORY OF MATHEMATICS
section: 19
section_title: The Gamma Function
lang: ja
source: hist
pdf_pages: 0205-0205
extraction: ocr
statements: 0
exercises: 0
content_sha256: 491b335a249b930ae027055a6c216076eae0a4c4f0de0de3a4d9558e8826079c
translated_from: content/en/hist/1/19_s19_the_gamma_function.md
translation_method: google
source_content_sha256: 7092fa519a4f115973a096a09aabbecb5a46cdac0f410b2a08e230e4c0142ff8
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 290b32e11751c8fd3c8d181ff0f4ef487723b427200e93b1c655c60dfd2c4e86
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 19. ガンマ写像。

数列 $(u_n)$ を、実パラメータ $\lambda$ に依存し、$\lambda = n$ の$u_n$ に等しい積分の値で「補間」するというアイデアは、Wallis に遡ります (cf. pp. 187 ff.)。 1730 年にオイラーにとって主要な指針となったのはこの考えです ([108 a]、(1)、v. XIV、pp. 1-24)、彼は階乗の数列を補間するというアイデアを思いつきました。 彼はまず、$n!$ が無限の積 $\prod_{k=1}^{\infty} \left( \frac{k+1}{k} \right)^n \frac{k}{k+n}$ に等しいこと、この積が $n$ のすべての値 (整数かどうか) に対して定義されること、特に $n = \frac{1}{2}$ については、公式から値 $\frac{1}{2} \sqrt{\pi}$ がかかることを述べています。ウォリス。 この結果をウォリスの結果と類推することで、彼は、後者によってすでに考慮されている積分$\int_0^1 x^e (1-x)^n dx$ ($n$ 整数、$e$ 任意) を再び取り上げることになります。 オイラーは二項展開によって値 $\frac{n!}{(e+1)(e+2)\cdots(e+n)}$ を取得します。変数の変更は、積分$\int_0^1 \left( \frac{1-x^z}{z} \right)^n dx$、よっての「第2オイラー積分」$n! = \int_0^1 (\log \frac{1}{x})^n dx$の$z$が0になる傾向があるため、$n!$が極限であることを示します。同じ方法とウォリスの公式の使用により、彼は公式$\int_0^1 \sqrt{\log \frac{1}{x}} dx = \frac{1}{2} \sqrt{\pi}$を取得します。 オイラーは後の研究でこれらの積分に頻繁に戻ります。彼はこのようにして補語の関係を発見します ([108 a]、(1)、v. XV、p. 82、および v. XVII、p. 342)、公式 $B(p, q) = \Gamma(p) \Gamma(q) / \Gamma(p + q)$ ([108 a]、(1)、v. XVII、p. 355)、およびルジャンドル ガウスの特定のケース公式対応するから $x = 1$ ([108 a]、(1)、v. XIX、p. 483);もちろん、収束の問題を心配する必要はありません。

ガウスは、超幾何写像に関する彼の研究に関連して $\Gamma$ 写像の研究を続けました。そのうち写像 $\Gamma$ は極限の場合です ([124 a]、v. III、pp. 125-162)。この研究中に、彼は乗法に対して一般的な公式を獲得します（$p = 2$に対して間もなく前ににルジャンドルがすでに指摘しています）。その後の$\Gamma$の作業は、主にこの写像の拡大を複雑な領域に関係させています。対数凸面性質が、関数方程式 $f(x+1) = x f(x)$ のすべての解のうち、$\Gamma(x)$ (実数領域で) から因子までを特徴づけていることが注目されたのはつい最近のことです ([26]、pp. 149-164)。そしてアーティンは、$\Gamma(x)$ に関するすべての古典的な結果がこの性質にどのように単純に関連付けられるかを示しました [7 d]。
