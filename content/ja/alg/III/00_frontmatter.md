---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 0
section_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
kind: front
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: "427"
pdf_pages: 0451-0451
extraction: ocr
statements: 0
exercises: 0
content_sha256: 13089e1f7f998b3b30ce0a8a3e49405d21399c94c4139b0d32500f4f12bbb054
translated_from: content/en/alg/III/00_frontmatter.md
translation_method: google
source_content_sha256: 6265d61279faab9dcf08066eb99e498297b3d05106b7e1efab665fe26a7b784b
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 17bdb0afaf523b8a8c5a5b8d01f03a2b48f616c6705935996df7865a5d4964e4
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 章 III

# テンソル代数、外装代数、対称代数

章 I で導入された指数記法を思い出してください。これを頻繁に使用します (I, § 7, no. 8)。

$(x_\lambda)_{\lambda \in L}$ をペアごとに置換可能な元の環 $A$ の族とします。 有限台の写像 $\alpha : L \to N$ ごとに次のように書きます

$$
x^\alpha = \prod_{\lambda \in L} x_\lambda^{\alpha(\lambda)}.
$$

$\beta$ が $L$ の他の写像を有限台の $N$ にすると、$\alpha + \beta$ は写像を表します

$$
\lambda \mapsto \alpha(\lambda) + \beta(\lambda)
$$

$L$ を $N$ に。この合成法則により、有限サポートの $L$ から $N$ への写像の集合 $N^{(L)}$ は、 $L$ から導出される自由可換モノイドであり、

$$
x^\alpha x^\beta = x^{\alpha + \beta}.
$$

すべての $\alpha \in N^{(L)}$ については、$|\alpha| = \sum_{\lambda \in L} \alpha(\lambda) \in N$ と書きます。次に$|\alpha + \beta| = |\alpha| + |\beta|$; $|\alpha|$は「マルチインデックス」$\alpha$の位数と呼ばれます。すべての $\lambda \in L$ について、$\delta_\lambda$ は $N^{(L)}$ の元を表し、$\mu \neq \lambda$ に対して $\delta_\lambda(\lambda) = 1$、$\delta_\lambda(\mu) = 0$ (クロネッカー 添字) を表します。 $\lambda \in L$ の $\delta_\lambda$ は、位数 1 の $N^{(L)}$ の元だけです。 $N^{(L)}$ には、$N^L$ での積の順序付けによって誘発された順序付けが与えられ、関係 $\alpha \leq \beta$ は次と等価になります。 「$\lambda \in L$全員に対して$\alpha(\lambda) \leq \beta(\lambda)$」;この場合、マルチインデックス $\lambda \mapsto \beta(\lambda) - \alpha(\lambda)$ は $\beta - \alpha$ で表されるため、$\alpha + (\beta - \alpha) = \beta$ などの一意のマルチインデックスになります。すべての $\alpha \in N^{(L)}$ に対して、複数インデックス $\beta \leq \alpha$ は有限の数のみです。 $\delta_\lambda$ は集合 $N^{(L)} - \{0\}$ の最小の元です。 関係 $\alpha \leq \beta$ は $|\alpha| \leq |\beta|$ を意味し、$\alpha \leq \beta$ と $|\alpha| = |\beta|$ の両方である場合は、$\alpha = \beta$ になります。

最後に、$\alpha! = \prod_{\lambda \in L} (\alpha(\lambda))!$ と書きます。これは、$0! = 1$ から意味を持ちます。

§ 4 から § 8 まで、$A$ は可換環を表し、〜でない限り別途記載がある場合、考慮される代数は結合的かつ単体であるとみなされ、代数準同型は単体であるとみなされます。
