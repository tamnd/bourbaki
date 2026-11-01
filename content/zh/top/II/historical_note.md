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
content_sha256: e2bb07906d55270ba5395575556fb24743ad975d61e12b9bb12f206e8f2e1ada
translated_from: content/en/top/II/historical_note.md
translation_method: google
source_content_sha256: 4e43b73e243b41231bf1da68ca84b8cfa71daa18e36ce5e144a610b1fa309a6d
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 977a791f1ac2acb34821c6064c015911ccb9ff6b9643acbc4ebd7ccec9e12a28
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

# 历史注记

（括号内的数指本注末尾的参考书目。）

均匀空间的主要概念和结果是从实变量理论中逐渐出现的，直到最近几年才被系统研究。柯西试图将级数理论置于严格的基之上（cf.历史注记到章I和IV），他认为点原理似乎是不言而喻的，即对于序列 $(a_n)$ 的收敛性，条件是只要 $n$ 是足够大，$|a_{n+p} - a_n|$ 就尽可能小（参见例 [2]）。与博尔扎诺 [1] 一起，他无疑是最先明确阐述此原理并认识到其重要性的人之一；因此，“柯西序列”的名称被赋予了实数的序列，其中所涉及的满足条件，以及在度量空间中的点的扩张到序列$(x_n)$ (章IX)使得当$n$足够大时从$x_{n+p}$到$x_n$的距离尽可能小；因此最终将柯西序列的推广命名为“柯西滤波器”，在本章中对其进行了研究。

后来，当实数的直觉概念不再被认为是足够的，并尝试为阶中的理性数的项中的定义实数来为数学分析提供可靠的基时，这就是柯西的原理提供了十九世纪下半叶提出的定义中最肥沃的一个。这个定义，归因于康托[3]（并由海涅[5]沿着康托的思想发展，并由M\'eray等人独立发展）在于将实数对应制作为理性数的每个柯西序列（康托的“基本序列”） 术语);当且仅当$|a_n - b_n|$趋于零时，实数对应与有理数的两个柯西序列$(a_n)$和$(b_n)$相同。这里的本质思想是，从某个点的角度来看（实际上是这个章、§ 1, no. 1、例1中定义的“统一结构”的点角度），有理数的集合$\mathbf{Q}$是“不完整”，实数中的集合是“完整”集合，是从$\mathbf{Q}$“完备的”得到的。

另一方面，海涅是第一个对一个或多个实变量的实值函数提出定义一致连续性的人，其工作很大程度上受到Weierstrass和Cantor [4]的思想的启发，他证明了在有界闭区间$\mathbf{R}$上连续的每个实值函数在该区间上一致连续：这就是“海涅的” 定理”。通过 § 4 的定理 2，该结果与 $\mathbf{R}$ 有界闭区间的紧致性相关 ("Borel-Lebesgue 定理", 章 IV, § 2, 定理 2; cf. 历史注记至章I和IV），海涅的定理的证明经过一些修改也可以用来证明Borel-Lebesgue定理（对于一些作者来说，这似乎是充分的理由将后者定理称为“Heine-Borel” 定理”）。

当度量空间被研究时，这些想法被扩展到更普遍的空间，首先是特定情况，然后是一般情况（cf.章IX）；在度量空间中，给出一个距离（即对、点、满足某些公理的实值函数），其中定义既是拓扑又是均匀性。 Fréchet是第一个给出这些空间的一般定义的人，认识到柯西原理的重要性[6]，并且还证明了度量空间定理相当于§ 4的定理3（[6]和[7]）。 Hausdorff 在他的“Mengenlehre”（[8]；cf. 以及 [8 a]）中相当大地发展了度量空间的理论，并且特别意识到人们可以将前面描述的康托尔的构造应用到这些空间上，从而从“非完整”度量获得“完整”度量空间空间（即柯西的原理无效）。

度量空间是“统一空间”的特定型；后者由 A. Weil 在最近的日期进行了全面的概括定义 [9]。在此之前，概念和“统一结构”的结果只能与度量空间一起使用，这一事实解释了度量空间和可度量空间（特别是紧凑可度量空间）在许多关于拓扑的现代作品中所扮演的重要部分，在距离没有真正用处的问题上。一旦拥有统一的空间的定义，就没有困难（特别是如果一个人还拥有可供使用的滤波器的概念）扩展到这些空间几乎整个度量空间的理论，例如由 Hausdorff 提出（类似地，对于例，将 Alexandroff-Hopf 的拓扑 [10] 中给出的紧凑度量空间的结果扩展到任意紧凑空间）。这就是我们在这个章所做的事情；特别是，完成均匀空间（§ 3，定理3）后的定理只不过是康托尔的构造对实数的转置，没有任何本质的修改。

[1] B. Bolzano，Rein analytischer Beweis des Lehrsatzes，dass zwischen je zwei Werthen，die ein entgegengesetztes Resultat gewähren，wenigstens eine reelle Wurzel liegt，Ostwald’s Klassiker，no. 153，莱比锡，1905。

[2] A.-L。柯西，《系列收敛》[Exercices d’Analyse，2e Année，巴黎，1827 年，p. 221 = Oeuvres (II)，卷。 7，巴黎（Gauthier-Villars）1889，p. 267]。

[3] G. Cantor，Gesammelte Abhandlungen，柏林（施普林格），1932 年。

[4] E. Heine, Über trigonometrische Reihen, Crelle’s Journal, 71 (1870), pp. 353-365.

[5] E. Heine, Die Elemente der Functionenlehre, Crelle’s Journal, 74 (1872), pp. 172-188.

[6] M. Fréchet, Sur quelques points du calcul fonctionnel, Rend. Palermo, 22 (1906), pp. 1-74.

[7] M. Fréchet, Les ensembles abstraits et le calcul fonctionnel, Rend. Palermo, 30 (1910), pp. 1-26.

[8] F. Hausdorff，Grundzüge der Mengenlehre，莱比锡（Veit），1914 年。

[8a] F. Hausdorff，Mengenlehre，柏林（de Gruyter），1927 年。

[9] A. Weil，Sur les espaces à 结构uniforme et sur la topologie générale，法案。科学。 et Ind.，no. 551，巴黎（赫尔曼），1937 年。

[10] P. Alexandroff 和 H. Hopf，拓扑学I，柏林（施普林格），1935 年。
