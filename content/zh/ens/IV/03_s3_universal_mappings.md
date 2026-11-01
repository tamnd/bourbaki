---
book: ens
book_title: Theory of Sets
chapter: IV
chapter_title: STRUCTURES
section: 3
section_title: Universal mappings
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 283-288, 294-295
pdf_pages: 0288-0293, 0299-0300
extraction: ocr
subsections:
    - "no": 1
      title: UNIVERSAL SETS AND MAPPINGS
      page: 283
      pdf_page: 288
    - "no": 2
      title: EXISTENCE OF UNIVERSAL MAPPINGS
      page: 284
      pdf_page: 289
    - "no": 3
      title: EXAMPLES OF UNIVERSAL MAPPINGS
      page: 286
      pdf_page: 291
statements: 0
exercises: 3
content_sha256: ad3dc06b14025f9b403c65aea7683652e9b843b0a55de910b11cc592262cbe13
translated_from: content/en/ens/IV/03_s3_universal_mappings.md
translation_method: google
source_content_sha256: 02143cebc191d935f4dc730de8191e96a819d51f624ae1e4a809f5d496463365
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 4fb320e53393801938376200ddb3867d05a9c172ed4a22fb8ed49c4a886d092b
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 3. 普遍映射

### 1. 全集和映射

令$\mathscr{T}$为强于集合论的理论，并令E为$\mathscr{T}$中的项。令$\mathscr{T}$中的$\Sigma$为结构种。为了简单起见，我们自始至终假设$\Sigma$是在单个（主要）基集合上定义的，并且为了简洁起见，我们将“$\Sigma$-集合”表示“集合赋予了类$\Sigma$的结构”。此外，我们假设$\sigma$态射已经被定义为类$\Sigma$（§ 2, no. 1；如在§ 2中，我们应该说“态射”代替“$\sigma$-态射”）。最后，类$\Sigma$被定义在基集合$x$上并且$s$作为泛型结构（§ 1, no. 4），让我们假设项$\alpha\{x,s\}$被定义在$\mathscr{T}_{\Sigma}$、满足以下条件：

(QM$_{\mathrm{I}}$) *关系 $\alpha\{x,s\}\subset\mathscr{T}(E;x)$ 在 $\mathscr{T}_{\Sigma}$ 中为真。*

(QM$_{\mathrm{II}}$) *如果（理论上$\mathscr{T}'$强于$\mathscr{T}$）F和F′是两个集合，并且赋予类$\Sigma$的结构$\mathscr{S},\mathscr{S}'$，并且如果$f$是将 F 的态射转化为 F′，则关系 $\varphi\in\alpha\{F,\mathscr{S}\}$ 意味着 $f\circ\varphi\in\alpha\{F',\mathscr{S}'\}$。*

我们将用说表达关系$\varphi\in\alpha\{x,s\}$，$\varphi$是E到$x$的$\alpha$映射（赋予$s$）。

如果满足以下条件 ，则 E 到 $F_E$ 的 $\Sigma$ 集合 $F_E$ 和 $\alpha$ 映射 $\varphi_E$ 被称为*通用*：

$(AU)$ *对于 E 到 $\Sigma$ 集 F 的每个 $\alpha$-映射 $\varphi$，存在 $F_E$ 的唯一态射 $f$ 到 F 中，使得 $\varphi=f\circ\varphi_E$。*

对于 E，对 $(F_E,\varphi_E)$ 也被称为普遍映射问题* 的 *解（相对于 $\Sigma$、$\sigma$ 和 $\alpha$）。

¶ 设$(F'_E,\varphi'_E)$和$(F''_E,\varphi''_E)$为E的普遍映射问题中的两个解。条件$(AU)$则表明$F''_E$中存在$F'_E$的唯一态射$f_1$且将$F''_E$的唯一态射$f_2$化为$F'_E$，使得$\varphi''_E=f_1\circ\varphi'_E$和$\varphi'_E=f_2\circ\varphi''_E$。因此我们有$\varphi''_E=f_2\circ f_1\circ\varphi'_E$和$\varphi'_E=f_1\circ f_2\circ\varphi''_E$。 应用$(AU)$对于$F=F'_E$和$\varphi=\varphi'_E$的情况，我们发现$f_2\circ f_1$是$F'_E$自身的恒等映射。类似地，$f_1\circ f_2$ 是 $F''_E$ 的恒等映射自身。因而（§ 2, no. 1，标准 CST8）$f_1$ 是 $F'_E$ 到 $F''_E$ 的 *同构*，$f_2$ 是它的逆同构。该结果由说表示，对于 E，普遍映射问题的解 *直到同构* 都是唯一的。

要验证 E 的对 $(F_E,\varphi_E)$ 是普遍映射问题的解，通常可以方便地验证以下两个条件 ：

$(AU'_{\mathrm I})$ *对于每个$\Sigma$集合F和E到F的每个$\alpha$-映射$\varphi$，存在$F_E$到F的态射$f$使得$\varphi=f\circ\varphi_E$。*

$(AU'_{\mathrm{II}})$ *对于每个$\Sigma$集合F，$F_E$中的两个态射进入F并且同意$\varphi_E(E)$是相等的。*

因为如果满足这两个条件，则由$(AU'_{\mathrm I})$保证存在的态射$f$由$(AU'_{\mathrm{II}})$唯一。反之，显然$(AU)$蕴涵$(AU'_{\mathrm I})$；此外，如果$f$和$f'$是$F_E$中的两个态射进入F并且在$\varphi_E(E)$上一致，我们有$f\circ\varphi_E=f'\circ\varphi_E$，从而$f=f'$乘应用$(AU)$到$\alpha$-映射$f\circ\varphi_E$。因而$(AU)$意味着$(AU'_{\mathrm{II}})$。

### 2. 普遍映射的存在

普遍映射问题不一定有解（习题1）。然而，我们将证明以下条件暗示解的存在：

$(CU_{\mathrm I})$ *在 $\Sigma$ 集合的族中的每个乘积上，都存在类 $\Sigma$ (§ 2, no. 4) 的乘积结构。*

$(CU_{\mathrm{II})}$ *令$(F_i)_{i\in I}$为$\Sigma$集合族，对于每个$i\in I$，令$\varphi_i$为E到$F_i$的$\alpha$映射。那么 E 的映射 $(\varphi_i)_{i\in I}$ 到 $\prod_{i\in I}F_i$（赋予乘积结构）是一个 $\alpha$ 映射。*

如果结构在F上诱导结构在G上类$\Sigma$（$\S\,2$，no. 4），则$\Sigma$集合F的子集G将被称为$\Sigma$-*可允许*。

$(\mathrm{CU_{III}})$ *存在一个基数* $\mathfrak{a}$ *具有以下属性：对于每个* $\Sigma$-*集合* F *和每个* $\alpha$-*映射* $\varphi$ *of* E *到* F *存在一个* $\Sigma$-*可允许* F *的子集* G *其中包含* $\varphi(\mathrm{E})$，*有基数* $\leqslant \mathfrak{a}$，*使得* E *的映射*进入* G *与* $\varphi$ *是一个* $\alpha$-*映射，并且使得任意两个* G *的态射转化为* $\Sigma$-*集合，同意* $\varphi(\mathrm{E})$，*是相等的。*

CST22。 *如果满足条件* $(\mathrm{CU_I})$ *到* $(\mathrm{CU_{III}})$ *，则普遍映射问题对于* E *有解。*

我们首先要证明，如果存在满足 $(\mathrm{AU'_I})$ 的对 $(\mathrm{F_E},\ \varphi_\mathrm{E})$，则对于 E 也存在普遍映射问题的解。对于$(\mathrm{CU_{III}})$，存在$\Sigma$ 允许的子集 $\mathrm{F'_E}$ $\mathrm{F_E}$ 包含 $\varphi_\mathrm{E}(\mathrm{E})$，使得 E 的映射 $\varphi'_\mathrm{E}$ 进入与 $\varphi_\mathrm{E}$ 具有相同图的 $\mathrm{F'_E}$ 是一个 $\alpha$ 映射，并且使得 $\mathrm{F'_E}$ 的任意两个态射进入同意 $\varphi_\mathrm{E}(\mathrm{E})$ 的$\Sigma$集合是相等的。令$j$为$\mathrm{F'_E}$的典范嵌入入$\mathrm{F_E}$，从而得到$\varphi_\mathrm{E} = j \circ \varphi'_\mathrm{E}$。对于$\mathrm{F_E}$的每个态射$f$到$\Sigma$集合F，$f \circ j$是到F的$\mathrm{F'_E}$的态射，并且我们有$f \circ \varphi_\mathrm{E} = (f \circ j) \circ \varphi'_\mathrm{E}$。因此可知$(\mathrm{F'_E},\ \varphi'_\mathrm{E})$满足$(\mathrm{AU'_I})$和$(\mathrm{AU'_{II}})$。

我们仍然需要确定对 $(\mathrm{F_E},\ \varphi_\mathrm{E})$ 满足 $(\mathrm{AU'_I})$ 的存在。令$s \in \mathrm{S}(x)$为结构种$\Sigma$的典型刻画，并考虑具有以下性质的所有三元组$\lambda = (\mathrm{X},\ \mathrm{V},\ \mathrm{P})$的$\mathfrak{P}(\mathfrak{a}) \times \mathrm{S}(\mathfrak{a}) \times \mathfrak{P}(\mathrm{E} \times \mathfrak{a})$由……组成的子集L：“V是$\mathrm{X} \subset \mathfrak{a}$上类$\Sigma$的结构，P是E到X的$\alpha$映射的图（相对于结构V）”（观察我们有$\mathrm{S}(\mathrm{X}) \subset \mathrm{S}(\mathfrak{a})$，通过逐步论证很容易看出在梯队构造概形 S 的长度上）。对于每个$\lambda = (\mathrm{X},\ \mathrm{V},\ \mathrm{P}) \in \mathrm{L}$，我们用赋予结构V的$\mathrm{X}_\lambda$集合X表示，并用E的$\varphi_\lambda$映射表示为图为P的$\mathrm{X}_\lambda$。

令$\mathrm{F_E}$为$\Sigma$集合，即$\mathrm{X}_\lambda$的乘积（它存在于$(\mathrm{CU_I})$），并令$\varphi_\mathrm{E}$为E到$\mathrm{F_E}$的映射$x \to (\varphi_\lambda(x))$，这是一个$\alpha$-凭借$(\mathrm{CU_{II}})$进行映射。让我们证明对$(\mathrm{F_E},\ \varphi_\mathrm{E})$满足$(\mathrm{AU'_I})$。给定 E 的 $\alpha$-映射 $\varphi$ 到$\Sigma$-集合 F，令 G 为 F 的子集，满足 $(\mathrm{CU_{III}})$ 中所述的条件。令$j$为G到F中的典范嵌入，并令$\psi$为E到G中的映射，G与$\varphi$具有相同的图，因此$\varphi = j \circ \psi$。从$(\mathrm{CU_{III}})$得出$\psi$是E到G的$\alpha$映射。由于卡(G)$\leqslant \mathfrak{a}$，$\mathfrak{a}$的子集G$'$等价于G。令$g$为G的双射到G$'$。如果我们通过 G 上的类 $\Sigma$ 迁移 $g$ 结构，则存在 L 的定义元素 $\lambda$，使得 G$'$ （赋予传输结构) 等于 $\mathrm{X}_\lambda$ 并且$g \circ \psi = \varphi_\lambda$。那么$f = j \circ \overset{-1}{g} \circ \mathrm{pr}_\lambda$就是$\mathrm{F_E}$的态射进入F，使得$\varphi = f \circ \varphi_\mathrm{E}$，并且证明是完整的。

CST23。 *设* $(\mathrm{F_E},\ \varphi_\mathrm{E})$ *为* E 为普遍映射问题解。 *则* $\varphi_\mathrm{E}$ *为* E *的单射 *入* $\mathrm{F_E}$ *当且仅当，对于每个不同的对元素* $x$，$y$ *属于* E，*存在* $\alpha$-*映射* $\varphi$ *属于* E *到* $\Sigma$-*集合* F *使得* $\varphi(x) \neq \varphi(y)$。

由于 $\varphi_\mathrm{E}$ 是 $\alpha$ 映射，因此标准是直接的推论或定义。

¶ 在这种情况下，$\alpha$映射被认为是*分离*E的元素，并且我们通常不会在术语中对E的元素和$\varphi_\mathrm{E}$下的像进行任何区分。根据此约定，如果 $(\mathrm{F_E},\ \varphi_\mathrm{E})$ 是普遍映射问题的解，且满足条件 $(\mathrm{CU_{III}})$，则 E 的每个 $\alpha$ 映射到 $\Sigma$ 集合 F *扩展唯一到* 的态射 $\mathrm{F_E}$ *进入* F.

### 3. 例普遍映射

\* 例，对于大多数部分，将在本级数的其他地方详细处理。

I。 *自由代数结构。* 令 E 为集合，并令 $\Sigma$ 为代数结构的类，由合成中的一个或多个律定义。我们将类 $\Sigma$ 的 *同态* 视为态射进行考虑，并将 E 的 *任意* 映射 $\alpha$ 映射到 $\Sigma$ 集合（在其他字、$\alpha \{ x,\ s \} = \mathfrak{F}(\mathrm{E},\ x)$ 中）。所有常见的代数类结构满足$(\mathrm{CU_{III}})$；除了环结构除法之外，它们还有满足$(\mathrm{CU_I})$，而$(\mathrm{CU_{II}})$在这里是$(\mathrm{CU_I})$的微不足道的推论。

由于通常存在在集合上定义的类 $\Sigma$ 的结构以及至少两个元素，因此 $\alpha$ 映射将 E 的元素分开，因此可以将 E 视为嵌入在 $\mathrm{F_E}$ 中。 $\mathrm{F_E}$据说是由* E生成的*自由*$\Sigma$-*集合。因此，在代数中，我们谈论*自由半群*、*自由群*、*自由模*和*自由代数*。

II。 *分数的环和域。*设E为交换环且单位元素，并令S为E的乘法闭子集，且包含不为0。我们取$\Sigma$为交换环的结构种与单位元素，以及态射为环同态，其中变换单位元素变为单位元素。 $\alpha$-映射将是 E 的同态 $\varphi$ 到交换环 A 和单位元素，这样 $\varphi(1) = 1$ 和 $\varphi(\mathrm{S})$ 包含只有 A 的 *单位*。 条件 $(\mathrm{QM_{II}})$、$(\mathrm{CU_I})$到$(\mathrm{CU_{III}})$（与$\mathfrak{a} = \mathrm{Card}\ (\mathrm{E})\ \mathrm{Card}\ (\mathbf{N})$）立即得到验证。因此普遍映射问题总是有解 $(\mathrm{F_E},\ \varphi_\mathrm{E})$，但一般来说 $\varphi_\mathrm{E}$ 不是单射的。最常见的情况是$E$为整环；在这种情况下，$\varphi_E$是单射的。此外，如果我们取$S = E - \{0\}$，那么$F_E$就是域，称为$E$的分数*的*域。

III。 *两个模中的张量积。*令$E$为两个模中的乘积$A \times B$，其中交换环$C$有单位元素。将$\Sigma$作为$C$模块结构的类，将态射作为线性映射，将$\alpha$映射为$A \times B$的*双线性*映射到$C$模块。 条件 $(QM_{II})$ 显然是满意的，$(CU_I)$ 到 $(CU_{III})$（以及 $\mathfrak{a} = \mathrm{Card}\ (E)\ \mathrm{Card}\ (C)\ \mathrm{Card}\ (\mathbf{N})$）也是如此。通用$C$-模块$F_E$相应的到对$(A, B)$称为$A$和$B$的*张量积*，写作$A \otimes B$。 普遍映射$\varphi_E$写为$(x,\ y) \to x \otimes y$；它是双线性的，但一般来说不是单射的。

IV。 模运算符环*扩张。*设$A$为交换环和单位元素，设$B$为$A$包含单位元素子环 $A$，并令$E$为$B$模块。 类$\Sigma$是$A$模块结构的类，态射是$A$-*线性*映射，$\alpha$-映射是$B$-*线性*映射 $E$ 转换为 $A$ 模块。通用$A$-模块$F_E$相应的到$B$-模块$E$据说是通过*扩展到*$A$环运算符$B$或$E$获得的。

V。 *完成制服空间。*令$E$为制服空间。取$\Sigma$为完整豪斯多夫均匀空间的结构种，态射为均匀连续映射，将$E$均匀连续映射的$\alpha$映射为完整豪斯多夫均匀空间。完整豪斯多夫制服空间的$\Sigma$-允许子集在这里是*封闭*子集（相对于空间的拓扑），并且满足条件$(QM_{II})$和$(CU_I)$到$(CU_{III})$ （与$\mathfrak{a} = 2^{2^{\mathrm{Card}(E)}}$）。完整的 Hausdorff 制服空间是（最多同构）与 $E$ 相关的 Hausdorff 制服空间的*完备的*（*常规拓扑*、章 II, § 3, no. 7）。

VI。 *Stone-Čech 紧致化。* 令 $E$ 为完全正则的空间。 $\Sigma$是紧致空间的结构种，态射是连续映射（紧致空间到紧致空间），并且$\alpha$映射是$E$到紧致的连续映射空间。 $\Sigma$可允许的子集又是*封闭*子集，并且条件$(QM_{II})$、$(CU_I)$到$(CU_{III})$很容易验证（使用与例V中相同的基数）。紧致空间$F_E$是（直到同构）通过完成$E$相对于最粗糙均匀性而获得的“Stone-Čech紧致化”，其中$E$的所有连续映射到$\mathbf{R}$的区间$[0,\ 1]$都是均匀连续的（*一般拓扑*、章 IX, § 1、习题 7)； 映射 $\varphi_E$ 是单射的，因为 E 的任何两个不同的点都可以被 E 的连续映射分隔成 $[0, 1]$。

VII。 *自由拓扑群*。令E为完全正则空间，令$\Sigma$为豪斯多夫拓扑群结构的类，态射为连续同态；并取 $\alpha$-映射为 E 的连续映射到 Hausdorff 拓扑群。 条件 $(\mathrm{QM_{II}})$ 和 $(\mathrm{CU_I})$ 到 $(\mathrm{CU_{III}})$ 很容易验证，

$$\mathfrak{a} = \mathrm{Card\ (E)\ Card\ (\mathbf{N})}.$$

E 的这个普遍映射问题的解的豪斯多夫拓扑群 $\mathrm{F_E}$ 被称为由空间* E 生成的*自由拓扑群。因为 E 的任何两个不同的点都可以被 E 的连续映射分开， Hausdorff 拓扑群 **R**, 映射 $\varphi_\mathrm{E}$ 是单射；可以证明$\varphi_\mathrm{E}$是E到$\mathrm{F_E}$[^1]的子空间$\varphi_\mathrm{E}(\mathrm{E})$的同胚。除了将$\Sigma$视为豪斯多夫拓扑群的结构种之外，我们还可以取其他结构种，例如豪斯多夫拓扑阿贝尔的群、紧致群、豪斯多夫拓扑环、豪斯多夫拓扑环向量空间（在拓扑划分环之上，被视为辅助基集合）等。

VIII。 *拓扑群* 上的几乎周期性函数。令 E 为拓扑群。取$\Sigma$为紧致群结构的类，态射为连续同态，$\alpha$-映射为E的连续同态到紧致群。满足条件$(\mathrm{QM_{II}})$、$(\mathrm{CU_I})$到$(\mathrm{CU_{III}})$，满足$\mathfrak{a} = 2^{2^{\mathrm{Card\,(E)}}}$。 E 的普遍映射问题的紧致群 $\mathrm{F_E}$ 是解，称为与 E 伴随的*紧致群； 映射 $\varphi_\mathrm{E}$ 不一定是单射的。 E 上的每个连续实值函数，形式 $g \circ \varphi_\mathrm{E}$，其中 $g$ 是 E 上的连续实值函数，被称为 E 上的*几乎周期性函数*。

IX。 *阿尔巴尼亚品种*。设E是一个代数簇，令$\Sigma$是与E相同的基域上的阿贝尔的簇的结构种（阿贝尔的簇是赋予代数群结构的完全代数簇；它必然是可交换的）。 态射将一个阿贝尔的变体的有理映射转化为另一个（每个态射必然是同态的合成及其翻译）。 $\alpha$-映射是 E 到阿贝尔的变体的有理映射。 条件$(\mathrm{CU_I})$不满足，但E的普遍映射问题承认解$\mathrm{F_E}$，称为E的*阿尔巴尼亚簇*。一般来说，有理数映射$\varphi_\mathrm{E}$不是单射的。 \*

### 习题{#ens-iv-s3-exercises}

参见[习题为 § 3](exercises/s3/)。

[^1]: 参见 P. SAMUEL，“关于普遍映射和自由拓扑群”，*Bull。 阿米尔。 数学。 Soc.*，**54** (1948)，第 591-598 页。
