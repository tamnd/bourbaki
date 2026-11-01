---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: ""
chapter_title: ""
section: 0
section_title: INTRODUCTION TO CHAPTERS IV, V AND VI
kind: introduction
lang: zh
source: lie-iv-vi
pdf_pages: 0006-0007
extraction: ocr
statements: 0
exercises: 0
content_sha256: 310c6966b98c37f7265c00e1d6a0c3fc887961aa7234371ccd15303884e5d8d7
translated_from: content/en/lie/00_introduction.md
translation_method: google
source_content_sha256: 6039920d984a1193244721622035fbdcfccd3343c37bff11d7a710933b56f4fb
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 1e7442fc6eb462da48ef7be807ad9d17b90bc0f51ebcdf0af828a00e47451f3b
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 章 IV、V 和 VI 简介

对半单（解析或代数）群及其李代数的研究导致了对根系、Coxeter群和Tits系统的考虑。 章 IV、V 和 VI 专门用于这些结构。

为了方便读者，我们在下面给出几个例。

I。令$g$为复半单李代数，且$h$为$g^1$的嘉当子代数。 $g$的根相对于$h$是$h$上的非零线性形式$\alpha$，因此对于所有$h \in h$，存在$g$的非零元素$x$以及$[h, x] = \alpha(h)x$。这些根形式约化根系$R$在向量空间$h^*$与$h$对偶。给$R$确定$g$直到同构，每个约化根系与这样得到的根系同构。 $g$的自同构使$h$稳定，$h^*$的定义自同构使$R$不变，以这种方式获得$R$的每个自同构。 $R$ 的 Weyl 群由 $g$ 的内自同构定义的 $h^*$ 的所有自同构组成，使 $h$ 保持稳定；这是 Coxeter 群。

令$G$为与李代数$g$的连通复形李群，并令$\Gamma$为元素$h$的$G$由……组成的子群，使得$\exp_G(2\pi i h) = 1$。令$R^-$为$h$与$R$相反的根系，令$Q(R^-)$为由$R^-$生成的$h$的子群，并令$P(R^-)$为与子群相关联由 $R$ 生成 $h^*$ 的子群 $Q(R)$（即 $h \in h$ 的集合，使得对于所有 $\lambda \in Q(R)$，$\lambda(h)$ 为整数）。然后$P(R^-) \supset \Gamma \supset Q(R^-)$。此外，$G$的中心与$P(R^-)/\Gamma$以及$G$的基本群与$\Gamma/Q(R^-)$自然同构。特别是，如果$G$是伴随群，则$\Gamma$等于$P(R^-)$；如果$G$是单连通的，则$\Gamma$等于$Q(R^-)$。最后，$G$的有限维线性表示的权是与$\Gamma$相关联的$h^*$的子群的元素。

II。令$G$为半单连接紧实李群，并令$g$为其李代数。令$T$为$G$的最大环面，其中李代数$t$，并令$X$为$T$的特征标的群。令$R$为$X$的非零元素$\alpha$的集合，使得对于所有$t \in T$，存在$g$的非零元素$x$，且$(\mathrm{Ad}\, t).x = \alpha(t)x$。 认同$X$，实数有格子向量空间$V = X \otimes_{\mathbf{Z}} \mathbf{R}$；那么 $R$ 就是 $V$ 中的约化根系。设$N$为$G$中$T$的归一化器； 作用

1 在本简介中，我们自由使用传统的术语以及章IV、V和VI中定义的概念。

N 在 T 定义同构上从群 N/T 到 R 的 Weyl 群。我们有 P(R) ⊃ X ⊃ Q(R)；此外，如果 G 是单连通的，则 X = P(R)，如果 G 约化到单位元素的中心，则 X = Q(R)。

$g$的复数李代数$g_{(C)}$是半单，$t_{(C)}$是它的嘉当子代数。 There exists a canonical isomorphism from $V_{(C)}$ to the dual of $t_{(C)}$ that transforms R into the root system of $g_{(C)}$ with respect to $t_{(C)}$.

III。设 G 是交换域 $k$ 上的连通半单代数群。令 T 为 G 分裂的的环面集合 $k$ 的极大元素，并令X 为 T 的特征标群（从 T 到乘法群同态）。我们认同X与真实向量空间$V = X \otimes_{\mathbf{Z}} \mathbf{R}$中的格子。 G 的根相对于 T 是 X 的非零元素 $\alpha$，因此对于所有 $t \in T$，存在 G 的李代数 $g$ 的非零元素 $x$，其中$(\mathrm{Ad}\, t).x = \alpha(t)x$。这给出了 V 中的根系 R，它不一定被约简。设 N 为 G 中 T 的归一化器，Z 为 T 的中心化器，并令 $N(k)$ 和 $Z(k)$ 为它们在 $k$ 上的有理点的群。 T 定义同构从 $N(k)/Z(k)$ 到 R 的 Weyl 群上的 $N(k)$ 作用。

令U为G的单能子群的集合的极大元素，在$k$上定义并由Z归一化。放置$P = Z.U$。然后是$P(k) = Z(k).U(k)$和$P(k) \cap N(k) = Z(k)$。而且，存在R的基$(\alpha_1, \ldots, \alpha_n)$，使得U中T的权是R对于这个基的正根；如果S表示$N(k)/Z(k)$的元素的集合，即对应，通过上面定义的同构，到与根$\alpha_i$相关的对称性$s_{\alpha_i} \in W(R)$，则四元数$(G(k), P(k), N(k), S)$是山雀系统。

IV。在局部域上的半单代数群的理论中，遇到Tits系统，其Weyl群是根系的仿射Weyl群。对于例，令$G = \mathbf{SL}(n+1, \mathbf{Q}_p)$（与$n \geq 1$）。设 B 为矩阵 $(a_{ij}) \in \mathbf{SL}(n+1, \mathbf{Z}_p)$ 的群，使得 $i < j$ 为 $a_{ij} \in p\mathbf{Z}_p$，并令 N 为矩阵的 G 由……组成的子群，每一行中只有一个非零元素和列。那么存在 $N/(B \cap N)$ 的子集 S，使得四元数 $(G, B, N, S)$ 是 Tits 系统。 群$W = N/(B \cap N)$是型$A_n$的根系的仿射Weyl群；这是一个无限 Coxeter 群。

在准备这些章的过程中，与 J. Tits 的多次交谈为我们提供了宝贵的帮助。我们非常诚挚地感谢他。
