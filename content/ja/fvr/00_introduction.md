---
book: fvr
book_title: Functions of a Real Variable
chapter: ""
chapter_title: ""
section: 0
section_title: INTRODUCTION
kind: introduction
lang: ja
source: fvr-i-vii
book_pages: 1-2
pdf_pages: 0016-0017
extraction: ocr
statements: 0
exercises: 0
content_sha256: 8498678cc53b81ecac96adb6bfb4281a3cd5c3d5eac55538c43738b2e434ff15
translated_from: content/en/fvr/00_introduction.md
translation_method: google
source_content_sha256: 85e0ba02d9e87d1ef4af523569a61f14e491623624b2c9c740da85ac45ab1be5
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: dfacd0018c87417c3904e886ec636f135123bf9daff40d3163aa03041ebb2485
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 導入

この本の目的は、1 つの実数変数の微小な性質を初歩的に研究することです。これらのプロパティの拡大からいくつかの実数変数の写像まで、またはより一般的な空間で定義された写像までは、後の書籍でのみ扱われます。

これから実証する結果は、実数変数の関係から (有限) 実数値写像に特に役立ちます。しかし、それらのほとんどは、$\mathbf{R}$ 上のトポロジー ベクトル空間で値を取る実数変数の写像に対するさらなる引数なしで拡大するです (以下を参照)。これらの写像は分析で頻繁に発生するため、実数値写像に固有ではないすべての結果を記載します。

The notion of a topological vector space, of which we have just spoken, is defined and studied in detail in Book V of this Series; but we do not need any of the results of Book V in this Book; some definitions, however, are needed, and we shall reproduce them below for the convenience of the reader.

(可換) 体 K (Alg., II, p. 193) 上でベクトル空間の定義を繰り返すことはしません。 $^1$ トポロジカル体 K 上のトポロジカルベクトル空間 E は、位相を備えた K 上のベクトル空間であり、写像 $x + y$ と $xt$ がそれぞれ $E \times E$ と $E \times K$ で連続します。特に、そのような位相は、E の加法群の構造と互換性があります。この本で考慮されるすべてのトポロジー ベクトル空間は、暗黙的にハウスドルフであると想定されています。トポロジカルな群 E が完了すると、トポロジカルなベクトル空間 E が完了したと言われます。値体 K (Gen. Top.、IX、p. 169) $^2$ 上のすべての正規化ベクトル空間は、K 上のトポロジカルベクトル空間です。

E を実数体 $\mathbf{R}$ を超えるベクトル空間 (位相の有無にかかわらず) とします。 x、y が任意の点の場合、点 $xt + y(1-t)$ の E 集合で、t は閉じた空間を通過します。

$^1$ The elements (or vectors) of a vector space E over a commutative field K will usually be denoted in this chapter by thick minuscules, and scalars by roman minuscules; most often we shall place the scalar t to the right in the product of a vector x by t, writing the product as $xt$; on occasion we will allow ourselves to use the left notation $tx$ in certain cases where it is more convenient; also, sometimes we shall write the product of the scalar $1/t$ ($t \neq 0$) and the vector x in the form $x/t$.

$^2$ E 上のノルムは、E 上で定義された実数写像 $\|x\|$ であり、非負の有限値をとり、関係 $\|x\| = 0$ は $x = 0$ と等価であり、次のようになります。

$$
\|x + y\| \leq \|x\| + \|y\| \quad \text{and} \quad \|xt\| = \|x\| \cdot |t|
$$

すべての $t \in K$ ($|t|$ は K の $t$ の絶対的な値です)。

$\mathbf{R}$ のセグメント [0, 1] は、端点 $x, y$ を持つ *閉じたセグメント* と呼ばれます。 One says that a subset $A$ of $E$ is *convex* if for any $x, y$ in $A$ the closed segment with endpoints $x$ and $y$ is contained in $A$. たとえば、アフィン線形多様体は凸です。閉じたセグメントも同様です。 $\mathbf{R}^n$ の平行六面体 (*Gen. 上.*、VI、p. 34）が凸です。 凸集合のすべての共通部分は凸です。

体 $\mathbf{R}$ 上の位相幾何学的ベクトル空間 $E$ は、原点 (したがって、$E$ の任意の点) が *凸* 近傍の基本系を持つ場合、*局所的に凸*であると言います。すべての *正規化* 空間は局所的に凸です。実際、ボール $\|x\| \leq r \ (r > 0)$ 形は $E$ の 0 の近傍の基本的な系であり、これらのそれぞれは凸であり、関係 $\|x\| \leq r,\ \|y\| \leq r$ は次のことを意味します。

$$
\|xt + y(1-t)\| \leq \|x\| t + \|y\| (1-t) \leq r
$$

$0 \leq t \leq 1$の場合。

最後に、(可換) *トポロジカル体* $K$ 上の *トポロジカル代数* $A$ は、$K$ 上の代数に位相が付与されており、そのために写像 $x + y,\ xy$ と $xt$ が連続しています。それぞれ$A \times A,\ A \times A$と$A \times K$。 $A$ に $K$ よりも位相とベクトル空間構造だけを与えると、$A$ はトポロジカルなベクトル空間になります。 *値体* $K$ (*Gen. Top.*、IX、p. 175) 上のすべての *ノルム代数* は、$K$ 上のトポロジー 代数です。
