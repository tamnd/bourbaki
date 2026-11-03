---
book: top
book_title: General Topology
chapter: II
chapter_title: Uniform Structures
section: 0
section_title: Historical Note
kind: historical
lang: zh
source: top-i-iv
book_pages: 216-218
pdf_pages: 0222-0224
extraction: ocr
statements: 0
exercises: 0
content_sha256: 1726a8bf0d00675ae65cad1a6457dd83982a8e2d37c9492ae606637a0994067d
translated_from: content/en/top/II/historical_note.md
translation_method: google
source_content_sha256: 4e43b73e243b41231bf1da68ca84b8cfa71daa18e36ce5e144a610b1fa309a6d
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 977a791f1ac2acb34821c6064c015911ccb9ff6b9643acbc4ebd7ccec9e12a28
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

# 历史注记

（括号内的数指本注末尾的参考书目。）

均匀空间的主要概念和结果是从实变量理论逐渐出现的，直到最近几年才被系统研究。柯西试图将级数的理论放在严格的基上（cf.历史注记到章I和IV），他认为点原理是不言而喻的，也就是说，对于序列 $(a_n)$ 的收敛，必要且充分的条件是当 $n$ 为足够大时，$|a_{n+p} - a_n|$ 尽可能小（参见示例 [2]）。与博尔扎诺 [1] 一起，他无疑是最先明确阐述此原理并认识到其重要性的人之一；因此，“柯西序列”的名称被赋予了实数的序列，其中所涉及的满足条件，以及在度量空间中的扩张到点的序列$(x_n)$ (章IX)使得当$n$足够大时从$x_{n+p}$到$x_n$的距离尽可能小；因此最终将柯西序列的推广命名为“柯西滤波器”，这已在本章中进行了研究。

后来，当实数的直觉概念不再被认为是足够的，并尝试为阶中的理性数的项中的定义实数来为数学分析提供可靠的基时，这就是柯西的原理提供了十九世纪下半叶提出的定义中最肥沃的一个。这个定义，归因于康托[3]（并由海涅[5]沿着康托的思想发展，并由M\'eray等人独立发展）在于将实数对应制作为理性数的每个柯西序列（康托的“基本序列”） 术语);当且仅当$|a_n - b_n|$趋于零时，实数对应与有理数的两个柯西序列$(a_n)$和$(b_n)$相同。这里的本质思想是，从某个点的角度来看（实际上是这个章、§ 1, no. 1、例1中定义的“统一结构”的点角度），有理数的集合$\mathbf{Q}$是“不完整”，实数中的集合是“完整”集合，是从$\mathbf{Q}$“完备的”得到的。

另一方面，海涅是第一个对一个或多个实变量的实值函数提出定义一致连续性的人，他的工作主要受到Weierstrass和Cantor [4]的思想的启发，他证明了在$\mathbf{R}$的有界封闭区间上连续的每个实值函数在此上一致连续区间：这是“海涅的定理”。通过 § 4 的定理 2，该结果与 $\mathbf{R}$ 的有界封闭区间的紧致性相关 ("Borel-Lebesgue 定理", 章 IV, § 2, 定理 2; cf. 历史注记到章I和IV），海涅的定理的证明经过一些修改也可以用来证明Borel-Lebesgue定理（对于一些作者来说，这似乎是充分的理由将后者定理称为“海涅-博雷尔定理”）。

当度量空间被研究时，这些想法被扩展到更普遍的空间，首先是特定情况，然后是一般情况（cf.章IX）；在度量空间中，给出一个距离（即点、满足某些公理的对的实值函数），其中定义既是拓扑又是均匀性。 Fréchet是第一个给出这些空间的一般定义的人，认识到柯西原理的重要性[6]，并且还证明了度量空间定理相当于§ 4的定理3（[6]和[7]）。 豪斯多夫在他的“Mengenlehre”（[8]；cf.[8a]）中相当大地发展了度量空间理论，并且特别认识到人们可以将前面描述的康托构造应用于这些空间，从而从“非完备”度量空间（即柯西原理在其中无效的度量空间）获得“完备”度量空间。

度量空间是“统一空间”的特定型；后者由 A 完全概括地定义。 韦尔在最近的日期[9]。 在此之前，概念和“均匀结构”的结果只能与度量空间一起使用，这一事实解释了度量空间和可度量空间（特别是紧凑可度量空间）在许多关于拓扑的现代作品中所扮演的重要部分，在问题中距离没有真正的用处。 一旦拥有统一的空间的定义，就没有困难（特别是如果一个人还拥有可供使用的过滤器概念）扩展到这些空间几乎整个度量空间的理论，例如给定的由 Hausdorff 提出（类似地，例如，将 Alexandroff-Hopf 的拓扑 [10] 中给出的紧凑度量空间的结果扩展到任意紧凑空间）。 这就是我们在这个章所做的；特别是，完成均匀空间（§ 3，定理3）后的定理只不过是康托尔的构造对实数的转置，没有任何本质的修改。

[1] B. Bolzano，Rein analytischer Beweis des Lehrsatzes，dass zwischen je zwei Werthen，die ein entgegengesetztes Resultat gewähren，wenigstens eine reelle Wurzel liegt，Ostwald’s Klassiker，no. 153，莱比锡，1905。

[2] A.-L。柯西，《系列收敛》[Exercices d’Analyse，2e Année，巴黎，1827 年，p. 221 = Oeuvres (II)，卷。 7，巴黎（Gauthier-Villars）1889，p. 267]。

[3] G. Cantor，Gesammelte Abhandlungen，柏林（施普林格），1932 年。

[4] E. Heine，《超三角学 Reihen》，Crelle’s Journal，71 (1870)，第 353-365 页。

[5] E. Heine，Die Elemente der Functionenlehre，Crelle’s Journal，74 (1872)，第 172-188 页。

[6] M. Fréchet，《Sur quelques 点 du calcul fonctionnel》，Rend。巴勒莫，22 (1906)，第 1-74 页。

[7] M. Fréchet，Les ensemblesabstraitsetlecalculfonctionnel，Rend。巴勒莫，30 (1910)，第 1-26 页。

[8] F. Hausdorff，Grundzüge der Mengenlehre，莱比锡（Veit），1914 年。

[8a] F. Hausdorff，Mengenlehre，柏林（de Gruyter），1927 年。

[9] A. Weil，Sur les espaces à 结构uniforme et sur la topologie générale，法案。科学。 et Ind.，no. 551，巴黎（赫尔曼），1937 年。

[10] P. Alexandroff 和 H. Hopf，拓扑学I，柏林（施普林格），1935 年。
