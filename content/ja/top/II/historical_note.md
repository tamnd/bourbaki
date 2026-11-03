---
book: top
book_title: General Topology
chapter: II
chapter_title: Uniform Structures
section: 0
section_title: Historical Note
kind: historical
lang: ja
source: top-i-iv
book_pages: 216-218
pdf_pages: 0222-0224
extraction: ocr
statements: 0
exercises: 0
content_sha256: 594e0a7e2b41c86ce23d1577ebb4eb66465bef878664b39c0d6e1b52220b8a46
translated_from: content/en/top/II/historical_note.md
translation_method: google
source_content_sha256: 4e43b73e243b41231bf1da68ca84b8cfa71daa18e36ce5e144a610b1fa309a6d
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 10cef2262a1302fcbd4a3f284001f9a5d85514c9e678ccd3eb4076022de72b19
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

# 歴史注意

(括弧内の数は、この注意の最後にある参考文献を参照します。)

均一空間に関する主要な概念と結果は、実数変数の理論から徐々に現れてきており、体系的に研究されるようになったのは近年のことです。 コーシーは、系列の理論を厳密な基底（cf.、歴史的な注意から章IおよびIV）に当てはめようとする際、点を開始点として採用したが、これは彼が自明のことだと考えていたようである。 数列 $(a_n)$ の収束に十分な条件は、$n$ が十分大きいであるときはいつでも、$|a_{n+p} - a_n|$ が好きなだけ小さいということです (例 [2] を参照)。 Together with Bolzano [1] he was undoubtedly one of the first to state this principle explicitly and to recognize its importance; hence the name of "Cauchy sequences" given to sequences of real numbers which satisfy the condition in question, and by extension to sequences $(x_n)$ of points in a metric space (Chapter IX) such that the distance from $x_{n+p}$ to $x_n$ is as small as we please whenever $n$ is large enough; and hence finally the name of "Cauchy filter" given to the generalization of Cauchy sequences which has been studied in this chapter.

後に、直感的な実数の概念が適切とは見なされなくなり、分析のための堅実な基底を提供するために、位数の合理的な数の項で定義する実数が試みられたとき、最も豊かな分析を提供したのはコーシーの原理でした。 定義は 19 世紀後半に提唱されました。この定義は、カントール [3] によるもの (そして特にハイネ [5] によってカントールの考えに沿って開発され、特に M\'eray によって独自に開発されたもの) は、合理的な数 (カントールの「基本的な数列」) のすべてのコーシー 数列に実数対応するを作成することで構成されています。用語); $|a_n - b_n|$ が零になる傾向がある場合に限り、有理数数の 2 つのコーシー 数列 $(a_n)$ と $(b_n)$ に同じ実数対応するを適用します。ここでの本質的な考え方は、ある点の視点 (実際には、この章、§ 1, no. 1、例 1 で定義される「均一構造」の点の視点) から、有理数数の集合 $\mathbf{Q}$ は次のとおりであるということです。 実数の集合は、$\mathbf{Q}$から「完備」によって得られる「完全」集合です。

一方、ハイネは、主にワイエルシュトラスとカントールの考えに触発された研究で、1 つ以上の実変数の実数値写像の定義する一様連続性を初めて示し、$\mathbf{R}$ の有界閉区間上で連続であるすべての実数値写像がこの上で一様連続であることを証明しました。 区間: こちらは「ハイネの定理」です。 § 4 の定理 2 により、この結果は $\mathbf{R}$ の有界で閉じた区間 ("Borel-Lebesgue 定理"、章 IV, § 2、定理 2; cf. 歴史的) のコンパクトさに関連しています。 注意から章 I と IV)、そしてハイネの定理の証明も、いくつかの修正を加えれば、ボレル・ルベーグ定理を証明するのに役立ちます (そして、これは、一部の著者にとって、後者定理を「 「ハイネ・ボレル定理」）。

These ideas became extended to more general spaces when metric spaces came to be studied, first in particular cases and then in general (cf. Chapter IX); in a metric space a distance is given (i.e. a real-valued function of pairs of points, satisfying certain axioms) which defines both a topology and a uniformity. これら空間のうちの一般的な定義を最初に示したフレシェは、コーシーの原理 [6] の重要性を認識し、計量空間定理が § 4 の定理 3 に相当することも証明しました ([6] および [7])。 ハウスドルフは、彼の「メンゲンレーレ」で計量空間の理論を大幅に開発し ([8]; cf. [8 a] も)、特に、前述したカントールの構成をこれらの空間に適用することで、「不完全」計量から「完全」計量空間を取得できることに気づきました。 空間 (つまり、コーシーの原理が無効な場合)。

メトリクス空間は、「均一空間」の特定の型です。後者は、かなり最近になって A. Weil によって完全に一般的に定義されました [9]。これ以前は、概念と「均一構造」の結果は、計量空間との関連でのみ使用できました。この事実は、多くの現代の作品において、計量空間と計量可能空間 (特にコンパクトな計量可能空間) が重要な部分を演じていることを説明しています。 位相、距離が実際には役に立たない問題。制服空間の定義を取得すると、これらの空間を、メートル法空間のほぼ全体の理論に拡張することは困難ではありません (特に、自由に使えるフィルター 概念を持っている場合)。 Hausdorff による (そして同様に、たとえば Alexandroff-Hopf の Topologie [10] で与えられたコンパクト メトリック空間の結果を任意のコンパクト空間に拡張する)。これがこの章年に私たちが行ったことです。特に、均一空間 (§ 3, 定理 3) の完成時の定理は、カントールの実数の構成を本質的な修正なしで転置したものにすぎません。

[1] B. Bolzano、Rein Analytischer Beweis des Lehrsatzes、dass zwischen je zwei Werthen、die ein entgegengesetztes Resultat gewähren、wenigstens eine reelle Wurzel liegt、Ostwald’s Klassiker、no. 153、ライプツィヒ、1905 年。

[2] A.-L。 Cauchy、Sur la convergence des series [Exercices d’Analyse、2e Année、Paris、1827、p. 221 = Oeuvres (II)、vol. 7、パリ (ゴティエ ヴィラール) 1889、p. 267]。

[3] G. Cantor、Gesammelte Abhandlungen、ベルリン (Springer)、1932 年。

[4] E. ハイネ、「Über trigonometrische Reihen」、Crelle’s Journal、71 (1870)、353-365 ページ。

[5] E. ハイネ、『Die Elemente der Functionenlehre』、Crelle’s Journal、74 (1872)、172-188 ページ。

[6] M. Fréchet、Sur quelques 点 du calcul fonctionnel、Rend。パレルモ、22 (1906)、1-74 ページ。

[7] M. Fréchet、「Les ensembles abstraits et le calcul fonctionnel」、Rend。パレルモ、30 (1910)、1-26 ページ。

[8] F. ハウスドルフ、Grundzüge der Mengenlehre、ライプツィヒ (ファイト)、1914 年。

[8 a] F. ハウスドルフ、メンゲンレーレ、ベルリン (デ グリュイター)、1927 年。

[9] A. Weil、「構造制服とトポロジー一般」、Act。科学的。 et Ind.、no. 551、パリ (ヘルマン)、1937 年。

[10] P. Alexandroff および H. Hopf、Topologie I、ベルリン (Springer)、1935 年。
