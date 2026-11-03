---
book: int
book_title: Integration
chapter: I
chapter_title: INEQUALITIES OF CONVEXITY
section: 0
section_title: Historical Note
kind: historical
lang: ja
source: int-i-vi
pdf_pages: 0023-0024
extraction: ocr
statements: 0
exercises: 0
content_sha256: 8bf32f4ccb5f16cb7635887602960ef21c45996f67a9fd37b77da90b185cbb1b
translated_from: content/en/int/I/historical_note.md
translation_method: google
source_content_sha256: 61a0e9809da1e06fbf74fbe28f6f19223c692979b397ccd8d7c3d2caf36893ee
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: 41ad9d7c47b75b7188c12771402fa43cb3439f51ac6cfc550e20628296093499
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

# 歴史注意

(注意 — ローマ数字は、この注意の最後にある参考文献を指します。)

2 つの正の量の算術平均と幾何平均の概念は古代にまで遡り、特にピタゴラス派はこれらをお気に入りの主題の 1 つとしました。また、これらの手段の間の不等式 $\sqrt{ab} \leq \frac{1}{2}(a + b)$ が彼らによく知られていた可能性もあります。いずれにせよ、それは、和が与えられる2つの数のうち積を最大化する問題に関連して、ユークリッドによって証明されます。マクローリンが、この問題から$n$数、そして対応する不等式の一般化について明確に言及しているのを見つけるには、1729年というかなり遅い日付まで待たなければならないようです（そして、これ、さらにはけれどもよりはるかに困難な極値問題さえも長い間扱われていました） 前に）。

18 世紀末以降、他の同様の不等式が解析と幾何学に登場しました。したがって、1789 年にルイリエは、不等式に関連する幾何学最大値問題を解きました。

$$
\sqrt{\left( \sum_{k=1}^n a_k \right)^2 + \left( \sum_{k=1}^n b_k \right)^2} \leq \sum_{k=1}^n \sqrt{a_k^2 + b_k^2};
$$

コーシーは 1821 年に特別な場合を証明した

$$
\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)
$$

ヘルダーの不等式; 1859 年に Buniakowsky が、1885 年に H. A. Schwarz がコーシーの不等式を積分に一般化しました。

それにもかかわらず、凸面の不平等が体系的な研究の対象となったのは、19 世紀の終わり近くになってからでした。 O. ヘルダーは 1888 年 (I)、単一変数の凸型写像を問題に導入するというアイデアを思いつきました。こうして彼は、凹型 $\log x$ から始まる幾何平均の不等式を取得しました。 適用写像 $x^r$ と同じ考えで、彼は自分の名前を冠した不等式を証明しました。それは 1 年前に L によってすでに発見されていました。 J. ロジャースは幾何平均の不等式から開始します (cf. Exer. 4)。 As for Minkowski’s inequality, it was proved by the latter in 1896 (for finite sums), in connection with his memorable works on the ‘Geometry of numbers’ ((II), pp. 115-117); however, while the idea of convexity (for functions of any number of variables) is one of the fundamental concepts of this work, it is rather surprising that Minkowski did not notice that his inequality may be obtained by Hölder’s method applied to $(1 + x^r)^{1/r}$ (he limited himself to applying the classical methods for seeking an extremum by means of the infinitesimal calculus).

For a deeper study of the inequalities of convexity and of their applications, the reader may consult the book of Hardy, Littlewood and Pólya devoted to the question, which also contains a very complete bibliography (III).

(I) O. ヘルダー、Ueber einen Mittelwertsatz、Göttinger Nachrichten (1889)、38-47 ページ。

(II) H. ミンコフスキー、ジオメトリ デア ザーレン、2 位。編、ライプツィヒ – ベルリン (トイブナー)、1910 年。

(III) G. H. Hardy、J. E. Littlewood、G. Pólya、『不平等』、ケンブリッジ (大学出版局)、1934 年。
