---
book: fvr
book_title: Functions of a Real Variable
chapter: VII
chapter_title: THE GAMMA FUNCTION
section: 0
section_title: Historical Note
kind: historical
lang: ja
source: fvr-i-vii
book_pages: 329-331
pdf_pages: 0344-0346
extraction: ocr
statements: 0
exercises: 0
content_sha256: c3cac46ee2ab26cf49df5b5654de0d7777d456ac07ac47ab61fd42310aa10387
translated_from: content/en/fvr/VII/historical_note.md
translation_method: google
source_content_sha256: 7c83612bea7e1b59873862456e66760a322c976bfe451e25a58e19896cc17b96
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 132c38067af463bb164cf6b6989b657bf4935a538cbc3a181e3c2755899c73e3
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

# 歴史注意

(注：ローマ数字は、この注意の最後にある参考文献を指します。)

実パラメータ $\lambda$ に依存し、$\lambda = n$ の $u_n$ に等しい積分の値で数列 $(u_n)$ を「補間」するというアイデアは、Wallis (III、p. 55) に遡ります。 1730 年にオイラー ((I)、v. XIV、p. 1-24) が集合自身で階乗の数列を補間したとき、主にこの考えがオイラーを導いたのです。彼は、$n!$ は無限の積 $$
\prod_{k=1}^{\infty} \left( \frac{k+1}{k} \right)^n \frac{k}{k+n},
$$ に等しいと述べ、その積は $n$ (整数かどうか) のすべての値に対して定義され、特に値 $n = \frac{1}{2}$ については値が必要であると述べました。ウォリスの公式による$\frac{1}{2} \sqrt{\pi}$。この結果とウォリスの結果との類似性により、彼は積分を再考するようになりました。
$$
\int_0^1 x^e (1-x)^n dx
$$
$(n$ 整数、$e$ 任意）後者はすでに考慮されています。オイラーは値を取得しました
$$
\frac{n!}{(e+1)(e+2)\ldots(e+n+1)}
$$
そのためには、二項展開を使用します。次に、変数の変更は、積分の $z$ が 0 になる傾向があるため、$n!$ が極限であることを示しました。
$$
\int_0^1 \left( \frac{1-x^z}{z} \right)^n dx,
$$
よって「第二オイラー積分」
$$
n! = \int_0^1 \left( \log \frac{1}{x} \right)^n dx;
$$
同じ方法によって、ウォリスの公式を使用して、彼は公式を取得しました
$$
\int_0^1 \sqrt{\log 1/x} dx = \frac{1}{2} \sqrt{\pi}.
$$
オイラーは後の著作でしばしばこれらの積分に戻りました。こうして彼は補語の関係 ((I), t. XV, p 82 および t. XVII, p. 342), 公式 $\mathbf{B}(p, q) = \Gamma(p)\Gamma(q)/\Gamma(p+q)$ ((I), t. XVII, p. 355)、およびルジャンドル ガウスの特定のケース公式対応するから $x = 1$ ((I), t. XIX, p. 483)。もちろん、これはすべて、収束の問題を心配する必要はありません。

ガウスは、超幾何学写像に関する彼の研究と関連して $\Gamma$ 写像の研究を追求しました。そのうちの $\Gamma$ 写像は極限の場合 (II) です。この研究の過程で、彼は将軍乗法公式を獲得しました（$p = 2$の少し前にルジャンドルがすでに指摘しています）。 $\Gamma$ の後の作業は、主にこの写像を複雑なドメインに拡張することに関係していました。対数凸の性質が、関数方程式 $f(x + 1) = x\, f(x)$ (III) の解のうち、定数因子までの $\Gamma(x)$ (実数領域) を特徴付けることが認識されたのはつい最近のことです。そして Artin は、$\Gamma(x)$ のすべての古典的な結果をこの性質に単純にリンクできる方法を示しました (IV)。私たちは彼の解説を非​​常に注意深く観察してきました。

(I)L。オイラー、オペラオムニア、ライプツィヒ-ベルリン（トイブナー）：t. XIV (1924)、t。 XV (1927)、t。 XVII (1915) と t. XIX (1932 年)。
(II)C.F.ガウス、ヴェルケ、t. III、ゲッティンゲン、1866 年。
(III) H. ボーアと J. モレルプ、レアボギ・マテマティスク分析、t。 III、コペンハーゲン、1922年、p. 149-164。
(IV) E. Artin、Einführung in die Theorie der Gammafunktion、ライプツィヒ (トイブナー)、1931 年。
