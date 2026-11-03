---
book: ens
book_title: Theory of Sets
chapter: IV
chapter_title: STRUCTURES
section: 2
section_title: Morphisms and derived structures
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 271-283, 290-294
pdf_pages: 0276-0288, 0295-0299
extraction: ocr
subsections:
    - "no": 1
      title: MORPHISMS
      page: 271
      pdf_page: 276
    - "no": 2
      title: FINER STRUCTURES
      page: 273
      pdf_page: 278
    - "no": 3
      title: INITIAL STRUCTURES
      page: 274
      pdf_page: 279
    - "no": 4
      title: EXAMPLES OF INITIAL STRUCTURES
      page: 276
      pdf_page: 281
    - "no": 5
      title: FINAL STRUCTURES
      page: 280
      pdf_page: 285
    - "no": 6
      title: EXAMPLES OF FINAL STRUCTURES
      page: 281
      pdf_page: 286
statements: 12
exercises: 11
content_sha256: 782f6e2fab340b20c82f3e1c8bf60654dae69b1acf012a99c0774fbd17c6259a
translated_from: content/en/ens/IV/02_s2_morphisms_and_derived_structures.md
translation_method: google
source_content_sha256: 5c7ff47f7a7c64e4e4d983dd7ce3ddd6c8c6e0cdf0393ed5ed3c52c0ad38c5b8
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 5566b021f76c601f85ee46ae0929a8b52b888ca3c8dc8869f801eb5478baec58
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 2. 态射和导出结构

### 1. 态射

在这个截面和下一个截面中，为了简单起见，我们将假设所考虑的结构种只有一个基集合（因此它是一个主体基集合）。读者可以毫无困难地将定义和结果扩展到一般情况。

令$\Sigma$为理论$\mathscr{T}$中的结构种，其强于集合论，并令$x$、$y$、$s$、$t$为与$\mathscr{T}$常数不同的四个不同字母。我们记得记号$\mathfrak{F}(x,y)$表示$x$的映射到$y$的集合（章II, § 5, no. 2）。假设我们在 $\mathscr{T}$ 中得到项 $\sigma\{x,y,s,t\}$ ，它满足以下条件 ：

$(\mathrm{MO}_{\mathrm{I}})$ *关系“$s$是$x$上类$\Sigma$的结构，$t$是$y$上类$\Sigma$的结构”意味着，在 E 中，关系 $\sigma\{x,y,s,t\}\subset\mathfrak{F}(x,y)$。*

$(\mathrm{MO}_{\mathrm{II}})$ *如果理论$\mathscr{T}'$比$\mathscr{T}$强，我们有三个集合E，E′，E″分别赋予类的结构，$\mathscr{S}$，$\mathscr{S}'$，$\mathscr{S}''$ $\Sigma$，则关系 $f\in\sigma\{E,E',\mathscr{S},\mathscr{S}'\}$ 和 $g\in\sigma\{E',E'',\mathscr{S}',\mathscr{S}''\}$ 意味着关系*

$$
g\circ f\in\sigma\{E,E'',\mathscr{S},\mathscr{S}''\}.
$$

$(\mathrm{MO}_{\mathrm{III}})$ *如果，在理论$\mathscr{T}'$强于$\mathscr{T}$，我们有两个集合E，E′分别赋予类$\Sigma$的结构，$\mathscr{S}$，$\mathscr{S}'$，则E 到 E′ 的双射 $f$ 为同构当且仅当 $f\in\sigma\{E,E',\mathscr{S},\mathscr{S}'\}$ 和 $f^{-1}\in\sigma\{E',E,\mathscr{S}',\mathscr{S}\}$。*

如果给定$\Sigma$和$\sigma$，关系$f\in\sigma\{x,y,s,t\}$可以用说表示，$f$是$x$的*态射*（或$\sigma$-*态射*），赋予$s$，转化为$y$，赋予$t$。如果（在理论$\mathscr{T}'$强于$\mathscr{T}$）E和E′是两个集合，并赋予结构$\mathscr{S},\mathscr{S}'$或类$\Sigma$，则项$\sigma\{E,E',\mathscr{S},\mathscr{S}'\}$是*E 到 E′ 的 $\sigma$-态射中的集合。*

*例*

#### 例 1 {#ens-iv-s2-n1-exa-1 .statement tag=03VL}

取$\Sigma$为序结构中的类，并让$\sigma\{x,y,s,t\}$表示$x$的所有映射$f$到$y$的集合，这样关系$(u,v)\in s$意味着$(f(u),f(v))\in t$。当记号为章III, § 1时，这意味着$u \leqslant v$蕴含$f(u) \leqslant f(v)$，即$f$是*递增*。公理$(\mathrm{MO_I})$、$(\mathrm{MO_{II}})$、$(\mathrm{MO_{III}})$的验证是显而易见的。

#### 例 2 {#ens-iv-s2-n1-exa-2 .statement tag=03VM}

将 $\Sigma$ 视为代数结构的类，它具有合成的单个（内部）律，在任何地方都有定义（§1, no. 4，例 2）。设A、A$'$为赋予类$\Sigma$的结构的两个集合，并令$p$、$p'$为这两个结构的合成律。考虑将 A 的映射 $f$ 转换为 A$'$，使得 $p'(f(x), f(y)) = f(p(x,\ y))$ 对于所有 $x \in \mathrm{A}$ 和所有 $y \in \mathrm{A}$。这些映射满足$(\mathrm{MO_I})$、$(\mathrm{MO_{II}})$和$(\mathrm{MO_{III}})$，被称为A到A$'$的*同态*。

#### 例 3 {#ens-iv-s2-n1-exa-3 .statement tag=03VN}

取$\Sigma$为拓扑结构的类（§1, no. 4，例3）。设A、A$'$为两个集合，分别赋予拓扑V、V$'$。考虑将 A 的映射 $f$ 转换为 A$'$，使得关系 $\mathrm{X}' \in \mathrm{V}'$ 蕴含 $\overset{-1}{f}(\mathrm{X}') \in \mathrm{V}$（在其他字中，使得拓扑中每个开路集合的逆像 V$'$是拓扑V中的开放集合）。这些映射，其中满足$(\mathrm{MO_I})$、$(\mathrm{MO_{II}})$和$(\mathrm{MO_{III}})$，是A到A$'$的*连续*映射（相对于拓扑V和V$'$） （cf. *一般拓扑*、章I, § 2）。

#### 注 {#ens-iv-s2-n1-rem-1 .statement tag=03VO}

对于给定的结构种$\Sigma$，我们可能有机会定义各种项$\sigma \} x,\ y,\ s,\ t \{$，其中满足条件$(\mathrm{MO_I})$、$(\mathrm{MO_{II}})$和$(\mathrm{MO_{III}})$。例如，如果$\Sigma$是拓扑结构的类，上面的记号是例3，则A到A$'$的映射$f$被称为“开”，如果关系 $\mathrm{X} \in \mathrm{V}$蕴含$f(\mathrm{X}) \in \mathrm{V}'$（在其他字中，如果每个开集合的$f$下的像都是开集合）。很容易检查到类$\Sigma$的开放映射还有满足条件$(\mathrm{MO_I})$、$(\mathrm{MO_{II}})$和$(\mathrm{MO_{III}})$。 \* 而且，可以证明连续的映射不一定是开的，开的映射也不一定是连续的。 \* 因此，给定的结构种 *并不意味着* 明确定义的概念或态射。

☡

当涉及序结构、代数结构和拓扑结构时，始终应理解态射是上面例中定义的那些，除非明确说明相反。

双射（章II, § 3, no. 8、推论至命题8）的条件$(\mathrm{MO_{III}})$和刻画意味着以下标准：

CST8。 *设*E，E$'$ *为两个集合，每个结构或类$\Sigma$。设$f$是* E *到* E$'$ *的$\sigma$态射，并让$g$是* E$'$ *到* E的$\sigma$态射。 *如果$g \circ f$是* E *自身的恒等映射，并且如果$f \circ g$是* E$'$ *的恒等映射到其自身，则$f$是* E *到* E$'$的同构，*并且$g$是逆同构。*

应该注意的是，E 到 E$'$ 的双射可能是 $\sigma$ 态射，而逆双射不一定是 $\sigma$ 态射。 \* 例如，拓扑空间 A 到拓扑空间 A$'$ 的双射映射可以是连续的，而逆双射不是连续的（*一般拓扑*、章 I, § 2, no. 1、注 1）。 \*

☡

#### 注 {#ens-iv-s2-n1-rem-2 .statement tag=03VP}

当结构种$\Sigma$有多个主基集合$x_1, \ldots, x_n$和辅助基集合$\mathrm{A}_1, \ldots, \mathrm{A}_m$时，$\sigma$态射为系统$(f_1, \ldots, f_n)$，其中$f_i$是$x_i$的映射变成$y_i$$(1 \leqslant i \leqslant n)$，而映射满足条件的系统类似于$(\mathrm{MO_{II}})$和$(\mathrm{MO_{III}})$，读者可以很容易地指出他自己。

### 2. 更细结构

对于这个截面的其余部分，我们假设我们得到了相对于这个结构种的$\sigma$态射的结构种、$\Sigma$和概念； *将引入的所有概念不仅取决于$\Sigma$，还取决于所设想的$\sigma$态射的概念。*通常我们会说“态射”来代替“$\sigma$-态射”。

¶ 设 E 为集合，并令 $\mathscr{S}_1$、$\mathscr{S}_2$ 为 E 上类 $\Sigma$ 的两个结构。 结构 $\mathscr{S}_1$ 据说是 *更细* 比 $\mathscr{S}_2$ （并且$\mathscr{S}_2$*比$\mathscr{S}_1$更粗糙*）如果赋予$\mathscr{S}_1$的E的恒等映射到赋予$\mathscr{S}_2$的E上，则为态射。

当有必要避免歧义时，我们会说$\mathscr{S}_1$比$\mathscr{S}_2$是更细*相对于所考虑的$\sigma$态射的概念*；对于在此截面中定义的所有其他概念也类似。

假设 $\mathscr{S}_1$ 比 $\mathscr{S}_2$ 更细。如果E$'$是赋予类$\Sigma$的结构$\mathscr{S}'$的集合，并且如果$f$是赋予$\mathscr{S}_2$的E的态射，转化为赋予$\mathscr{S}'$的E$'$，则$f$也是E的态射，赋予$\mathscr{S}_1$，变成E$'$，赋予$\mathscr{S}'$；这是从前面的定义和$(\mathrm{MO_{II}})$得出的。同样，如果 $g$ 是 E$'$ 的态射，赋有 $\mathscr{S}'$，转入 E，赋有 $\mathscr{S}_1$，则 $g$ 也是 E$'$ 的态射，赋有 $\mathscr{S}'$，转入 E，赋有$\mathscr{S}_2$。

因此，E 上的 *更细* 结构（类 $\Sigma$）、以 E 作为源的 *更多* 态射，以及以 E 作为目标的 *更少* 态射。

关系“$\mathscr{S}_1$比$\mathscr{S}_2$粗糙”是E上类$\Sigma$的所有结构的集合上$\mathscr{S}_1$和$\mathscr{S}_2$之间的*序关系*；因为它通过$(\mathrm{MO_{III}})$自反，通过$(\mathrm{MO_{II}})$传递，并且如果类$\Sigma$的结构既是更细又比另一个粗糙，那么两个结构由于$(\mathrm{MO_{III}})$而相同。与一般的定义 (章 III, § 1, no. 14) 一致，E 上的类 $\Sigma$ 中的两个结构被称为“可比较”，如果一个比另一个更细 ；如果结构比另一个更细*（或*更粗糙*）并且与其不同，则称结构*严格更细*（或*严格更粗糙*）于另一个。

*例*

#### 例 1 {#ens-iv-s2-n2-exa-1 .statement tag=03VQ}

当且仅当 $s \subset s'$ 时，集合 A 上具有图 $s$ 的订单结构比具有图 $s'$ 的订单结构更精细。 在其他字中，关系$x \leqslant y$相对于$s$意味着$x \leqslant y$相对于$s'$；这与章 III, § 1, no. 4、例 3 中给出的定义一致。

#### 例 2 {#ens-iv-s2-n2-exa-2 .statement tag=03VR}

考虑集合 A 上相同类 $\Sigma$ 的两个代数结构 F、F'，其中 F 和 F' 是这两个结构的合成的（到处定义的）律的图。在这种情况下，从态射的定义（no. 1，例2），F是更细比F'当且仅当$F \subset F'$。但由于 F 和 F' 都是具有相同域 $A \times A$ 的函数图，因此我们必须有 $F = F'$。在其他字中，类$\Sigma$中的两个*可比较*结构必然*相同*。

#### 例 3 {#ens-iv-s2-n2-exa-3 .statement tag=03VS}

令 V、V' 为同一集合 A 上的两个拓扑。说 V 比 V' 更细意味着，在这种情况下 (no. 1, 例 3)，凭借态射的定义， $V' \subset V$；在其他字中，A的每个子集在拓扑V'中是开集合，也是拓扑V中的开集合（因此，更细拓扑，越开集合有）。

#### 注 {#ens-iv-s2-n2-rem-1 .statement tag=03VT}

我们刚刚遇到了例 (例 2)，其中相同类 $\Sigma$ 的两个可比较的结构必然是相同的。还有许多其他这样的例：线性序结构，\*紧凑拓扑，Fréchet空间结构（态射是连续的线性映射），由除法环上的绝对值（或评估）定义的拓扑，等等。\*

对于这样的结构种$\Sigma$，E到E'的态射$f$是*双射的*，是一个*同构*；因为如果我们通过 $f$ 将迁移转换为 E' 结构 $\mathscr{S}$，我们就得到类 $\Sigma$ 的结构，即更细比 E' 上的结构 $\mathscr{S}'$ ，因此重合与 $\mathscr{S}'$。

### 3. 初始结构

考虑一个$(A_\iota)_{\iota \in I}$集合的家庭，每个家庭都被赋予结构$\mathscr{S}_\iota$类$\Sigma$。令 E 为集合，对于每个 $\iota \in I$，令 $f_\iota$ 为映射 *of* E *进入* $A_\iota$。 E 上类 $\Sigma$ 的结构 $\mathscr{S}$ 被认为是*关于家庭的首字母结构* $(A_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in I}$，如果它具有以下性质 ：

(IN) 给定任何集合 E'、E' 上类 $\mathscr{S}'$ 的任何结构，以及任何映射 $g$ *of* E' *进入* E，关系

“$g$ 是 E' 的态射到 E”

*等于* 关系

“对于每个$\iota \in I, f_\iota \circ g$，E'的态射进入$A_\iota$”。

CST9。 *如果在* E *上存在一个相对于族* $(\mathrm{A}_\iota,\ \mathscr{S}_\iota,\ f_\iota)_{\iota \in \mathrm{I}}$的初始结构，*它是类* $\Sigma$ *在* E *上的所有结构中最粗糙的，其中映射* $f_\iota$ *中的每个态射，因此是独特的。*

令$\mathscr{I}$为E上的初始结构，并令$\mathscr{S}$为E上类$\Sigma$的结构，其中每个$f_\iota$为态射。如果$i$表示E的恒等映射，赋有$\mathscr{S}$，代入E，赋有$\mathscr{I}$，那么对于所有$\iota \in \mathrm{I}$，$f_\iota \circ i$是态射，条件（IN）表明$i$是态射，这意味着（no. 2）$\mathscr{S}$比$\mathscr{I}$*更细*。另一方面，应用（IN）对于$g$是E（赋予$\mathscr{I}$）的恒等映射到其自身的情况，我们看到（通过$(\mathrm{MO_{III}})$）每个$f_\iota$都是E的态射到$\mathrm{A}_\iota$，这完成证明。

可能会发生 E 上存在类 $\Sigma$ 的结构，它是类 $\Sigma$ 的所有结构中最粗糙的，其中 $f_\iota$ 是态射，但是这个结构不是初始的结构相对于 $(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)$ (习题 6)。

我们有以下*传递性标准*：

CST10。 *设*E*为集合，让*$(\mathrm{A}_\iota)_{\iota \in \mathrm{I}}$*为集合的一个家庭，并且对于每个*$\iota \in \mathrm{I}$*让*$\mathscr{S}_\iota$*为类*$\Sigma$*上的结构*$\mathrm{A}_\iota$。 *让*$(\mathrm{J}_\lambda)_{\lambda \in \mathrm{L}}$*成为*I的划分，*并让*$(\mathrm{B}_\lambda)_{\lambda \in \mathrm{L}}$*成为由*L索引的集合族。 *对于每个* $\lambda \in \mathrm{L}$ *让* $h_\lambda$ *成为映射 of* E *进入* $\mathrm{B}_\lambda$，*并且对于每个* $\lambda \in \mathrm{L}$ *和每个* $\iota \in \mathrm{J}_\lambda$ *让* $g_{\lambda\iota}$ *成为映射 of* $\mathrm{B}_\lambda$ *进入*$\mathrm{A}_\iota$，*并让*$f_\iota = g_{\lambda\iota} \circ h_\lambda$。 *假设，对于每个*$\lambda \in \mathrm{L}$，*存在一个初始结构*$\mathscr{S}'_\lambda$*在*$\mathrm{B}_\lambda$*相对于家庭*$(\mathrm{A}_\iota, \mathscr{S}_\iota, g_{\lambda\iota})_{\iota \in \mathrm{J}_\lambda}$。 *那么以下叙述是等价的*：

(a) *对于家庭* $(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in \mathrm{I}}$ *在* E *上存在初始结构* $\mathscr{I}$；

(b) *对于家庭* $(\mathrm{B}_\lambda, \mathscr{S}'_\lambda, h_\lambda)_{\lambda \in \mathrm{L}}$ *在* E *上存在初始结构* $\mathscr{I}'$。

*此外，这些叙述意味着*$\mathscr{I} = \mathscr{I}'$。

设F为集合赋予类$\Sigma$的结构，并令$u$为F的映射入E。由定义关系观察“$h_\lambda \circ u$为F的态射入E” $\mathrm{B}_\lambda$”等价于关系“对于所有$\iota \in \mathrm{J}_\lambda$，$g_{\lambda\iota} \circ h_\lambda \circ u = f_\iota \circ u$是F到$\mathrm{A}_\iota$的态射”。 关系

(1) “对于所有 $\lambda \in \mathrm{L}$，$h_\lambda \circ u$ 是 F 的态射到 $\mathrm{B}_\lambda$”

因此相当于关系

(2) “对于所有 $\iota \in \mathrm{I}$，$f_\iota \circ u$ 是 F 的态射到 $\mathrm{A}_\iota$”。

现在，说$\mathscr{I}'$是$(\mathrm{B}_\lambda, \mathscr{S}'_\lambda, h_\lambda)_{\lambda \in \mathrm{L}}$族的首字母结构，意味着关系(1)等价于关系“$u$是F到E的态射赋予$\mathscr{I}'$”；说$\mathscr{I}$是$(A_i,\,\mathscr{S}_i,\,f_i)_{i\in I}$族的首字母结构，意味着关系(2)等价于关系“$u$是F到E的态射赋予$\Gamma$”。因此，鉴于初始结构的唯一性的性质。

### 4. 例 / 初始结构

I。 *结构的逆像。*当I是单个元素的集合由……组成时，相对于$(A,\,\mathscr{S},\,f)$的初始结构称为$f$下的*逆像结构 $\mathscr{S}$*（如果存在）。

\* 拓扑在任何映射 $f$ 下总是有逆像；但对于序结构或代数结构则并非如此。 \*

II。 *归纳结构。* 设A为集合，赋予类$\Sigma$的结构$\mathscr{S}$，设B为A的子集，设$j$为B的典范嵌入到A中。然后结构 B（如果存在）的$j$下的逆像称为B上$\mathscr{S}$诱导的*结构。*

序结构诱导结构相同的类在定义它的集合的每个子集上；但结构或有向集合的情况并非如此。 \* 拓扑诱导拓扑在定义它的集合的每个子集上，但紧凑的拓扑通常不会诱导紧凑的拓扑。 集合 A 上的代数结构通常不会在任意子集 B 上有相同的类的诱导结构；如果 A 上给定的结构由合成的律组成，并且这些合成到处都有定义，那么 B 必须相对于这些律中的每一个保持稳定，但是这个必要的条件并不总是足够的。 \*

通用准则 CST10 为我们提供了以下用于诱导结构的 *传递性准则*：

CST11。 *设B为A的子集，令C为B的子集，并令$\mathscr{S}$为A上的类$\Sigma$结构，其中诱导结构$\mathscr{S}'$与 B 上的类相同。那么类 $\Sigma$ 的 $\mathscr{S}$ 诱导结构在 C 当且仅当 $\mathscr{S}'$ 诱导结构 C上的类$\Sigma$，以及$\mathscr{S}$和$\mathscr{S}'$在C上诱发的结构是相同的。*

CST12。 *设A、A'为具有类$\Sigma$的结构$\mathscr{S}$、$\mathscr{S}'$的两个集合。设 B 为 A 的子集，B' 为 A' 的子集。假设 B（或 B'）上有类 $\Sigma$ 的 $\mathscr{S}$（或 $\mathscr{S}'$）诱导结构。如果$f$是A到A'的态射，使得$f(B)\subset B'$，则B到B'的映射，其中重合和B上的$f$是态射（相对于由$\mathscr{S}$诱导的结构和$\mathscr{S}'$).*

令$j$（或$j'$）为B（或B'）到A（或A'）的典范嵌入。到定义，我们就有了$f\circ j=j'\circ g$。由于$f$和$j$是态射，所以$f\circ j$乘以(MO$_{\mathrm{II}}$)；但是，$j'\circ g$是态射，映射$g$是态射乘以初始结构的定义。

III。 *乘积结构。*令$(A_i)_{i\in I}$为集合的一个族，并且在每个集合$A_i$上令$\mathscr{S}_i$为类$\Sigma$的结构。令$E=\prod_{i\in I}A_i$为$(A_i)_{i\in I}$族的*乘积*（章II, § 5），并令$\operatorname{pr}_i$表示$E$到$A_i$的投影。相对于族$(A_i,\mathscr{S}_i,\operatorname{pr}_i)_{i\in I}$的初始结构（如果存在）称为结构$\mathscr{S}_i$的*乘积*。

\* 一个拥有序结构的家庭总是承认乘积结构，但对于一个总序结构的家庭来说并不总是如此。 群结构的家庭总是承认乘积结构，但对于分裂的环结构家庭则不一定如此。拓扑族总是承认乘积结构，但对于局部紧凑空间的结构族来说并不总是如此；在这种情况下，如果族是*有限*，则存在相同的类的乘积结构，但如果族是*无限*，则不需要有一个（cf.*一般拓扑*，章I, § 9, no. 7，提案14）。 \*

标准 CST10 为乘积结构产生以下 *结合性标准*：

CST13。 *令$(A_i)_{i\in I}$为集合的一个族，对于每个指标$i\in I$，令$\mathscr{S}_i$为$A_i$上类$\Sigma$的结构。令 $(J_\lambda)_{\lambda\in L}$ 为 $I$ 的划分。假设在每个部分乘积$B_\lambda=\prod_{i\in J_\lambda}A_i$，家庭$(\mathscr{S}_i)_{i\in J_\lambda}$承认乘积结构$\mathscr{S}'_\lambda$。那么，当且仅当家庭$(\mathscr{S}'_\lambda)_{\lambda\in L}$承认乘积结构$\mathscr{S}'$，以及$E=\prod_{i\in I}A_i$的典范映射时，$(\mathscr{S}_i)_{i\in I}$承认乘积结构$\mathscr{S}$，赋予$\mathscr{S}$，到$F=\prod_{\lambda\in L}B_\lambda$，赋予$\mathscr{S}'$（章II, § 5, no. 5），则同构。*

另一个 CST10 的应用给出了以下关于由乘积结构引起的结构的标准：

CST14。 *令$(A_i)_{i\in I}$为集合的一个族，对于每个$i\in I$，令$\mathscr{S}_i$为$A_i$上类$\Sigma$的结构。对于每个 $i\in I$，令 $B_i$ 为子集 / $A_i$。假设$B_i$上的每个$\mathscr{S}_i$诱导结构$\mathscr{S}'_i$，并且在乘积$E=\prod_{i\in I}A_i$上存在结构$\mathscr{S}_0$，即家庭的乘积 $(\mathscr{S}_i)$。那么下面的叙述是等价的：*

(a) 在集合$B=\prod_{i\in I}B_i\subset E$上，存在$\mathscr{S}_0$诱发的结构$\mathscr{S}$；

(b) 在集合$B$上存在结构$\mathscr{S}'$，它是结构$(\mathscr{S}'_i)$家族的乘积。

*此外，这些叙述意味着$\mathscr{S}=\mathscr{S}'$。*

令$j_\iota$为$\mathrm{B}_\iota$到$\mathrm{A}_\iota$的规范注入，令$j$为B到E的规范注入，令$p_\iota$为E到$\mathrm{A}_\iota$的投影，令$p'_\iota$为B到$\mathrm{B}_\iota$的投影。 那么对于所有$\iota \in \mathrm{I}$我们就有$p_\iota \circ j = j_\iota \circ p'_\iota$。 到 CST10，$\mathscr{S}$ 是相对于族 $(\mathrm{A}_\iota, \mathscr{S}_\iota, p_\iota \circ j)_{\iota \in \mathrm{I}}$ 的初始结构，$\mathscr{S}'$ 是相对于族 $(\mathrm{A}_\iota, \mathscr{S}_\iota, j_\iota \circ p'_\iota)_{\iota \in \mathrm{I}}$ 的初始结构。 于是就有了这样的结果。

¶ 逆像和乘积的概念通过以下标准相关：

CST15。 *令$(\mathrm{A}_\iota)_{\iota \in \mathrm{I}}$为集合的族，对于每个$\iota \in \mathrm{I}$令$\mathscr{S}_\iota$为$\mathrm{A}_\iota$上类$\Sigma$的结构，并令$f_\iota$为集合E的映射入$\mathrm{A}_\iota$。假设在乘积集合$\mathrm{A} = \prod_{\iota \in \mathrm{J}} \mathrm{A}_\iota$存在乘积结构$\mathscr{S}$家庭$(\mathscr{S}_\iota)_{\iota \in \mathrm{I}}$。那么存在相对于族$(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in \mathrm{I}}$的初始结构当且仅当结构$\mathscr{S}$在E到A的映射$x \to f(x) = (f_\iota(x))$下有逆像，并且这两个结构是相同的。*

从$f_\iota = \mathrm{pr}_\iota \circ f$开始，该标准是CST10的特例。

#### 注 {#ens-iv-s2-n4-rem-1 .statement tag=03VU}

设$(\mathscr{S}_\lambda)_{\lambda \in \mathrm{L}}$是类$\Sigma$在*相同*集合A上的结构家族；令$\mathrm{A}_\lambda$表示集合A赋予结构$\mathscr{S}_\lambda$，令$\mathrm{I}_\lambda$表示将A的恒等映射赋予$\mathrm{A}_\lambda$。设 B 为乘积集合 $\mathrm{A}^{\mathrm{L}} = \prod_{\lambda \in \mathrm{L}} \mathrm{A}_\lambda$，并令 $\Delta$ 为该乘积 (章 II, § 5, no. 3) 的对角线。令 $h$ 为 A 到 $\Delta$ 的对角线映射，使得 $h(x)$ 为元素 $(x_\lambda)_{\lambda \in \mathrm{L}}$，这样对于所有 $\lambda \in \mathrm{L}$ 都有 $x_\lambda = x$。假设B上存在族$(\mathscr{S}_\lambda)$的乘积结构$\mathscr{S}'$。由于$h$是单射的，标准CST 15表明，当且仅当由$\mathscr{S}'$在$\Delta$上存在结构$\mathscr{S}''$时，存在关于族$(\mathrm{A}_\lambda, \mathscr{S}_\lambda, \mathrm{I}_\lambda)_{\lambda \in \mathrm{L}}$的初始结构$\mathscr{S}$；那么$\mathscr{S}''$就与通过$h$将$\mathscr{S}$传输到$\Delta$得到的结构相同。特别是，当所有结构$\mathscr{S}_\lambda$相同时，$h$是A的*同构*（赋予这个结构）到$\Delta$。

我们还有以下标准：

CST16。 *令$(\mathrm{A}_\iota)_{\iota \in \mathrm{I}}$、$(\mathrm{B}_\iota)_{\iota \in \mathrm{I}}$为集合的两个族，由相同的集合索引。对于每个$\iota \in \mathrm{I}$，令$\mathscr{S}_\iota$为$\mathrm{A}_\iota$上类$\Sigma$的结构，并令$\mathscr{S}'_\iota$为$\mathrm{B}_\iota$上类$\Sigma$的结构。假设$\mathrm{A} = \prod_{\iota \in \mathrm{I}} \mathrm{A}_\iota \left( \text{resp. on } \mathrm{B} = \prod_{\iota \in \mathrm{I}} \mathrm{B}_\iota \right)$乘积结构$\mathscr{S}$（$\mathscr{S}'$）上存在族$(\mathscr{S}_\iota)$（$(\mathscr{S}'_\iota)$）。对于每个$\iota \in \mathrm{I}$，令$f_\iota$为$\mathrm{A}_\iota$到$\mathrm{B}_\iota$的态射。那么映射 $f = (f_\iota)_{\iota \in \mathrm{I}}$ 就是 A 到 B 的态射。*

令$p_\iota$（或$q_\iota$）为A 到$\mathrm{A}_\iota$ 的投影（或B 到$\mathrm{B}_\iota$）。那么我们就有$q_\iota \circ f = f_\iota \circ p_\iota$。由于$f_\iota$和$p_\iota$是态射（标准

CST9), $f_i \circ p_i$ 乘以 (MO$_\Pi$) 为态射；因此 $f$ 等于 (IN) 态射。

#### 注 {#ens-iv-s2-n4-rem-2 .statement tag=03VV}

对于大多数常见的结构，CST16中给出的条件不仅是足够的，而且对于$f$成为态射（cf.习题7）来说也是必要的。特别是在以下情况下（例如，如果$\Sigma$是序结构的类，\*或群结构的类，或者拓扑结构*的类等；cf.） 习题 8) :

☡

¶ 存在一个族 $(a_i)_{i\in I}$，使得 $a_i\in A_i$ 对于所有 $i\in I$ 并且这样，如果我们放置 $r_i(x)=(y_\lambda)$，其中 $y_i=x_i$ 和 $y_\lambda=a_\lambda$ 每当 $\lambda\ne i$ 时，映射 $r_i$ 中的每一个都是态射 $A_i$ 变为$A$。因为如果$f=(f_i)$是$A$的态射到$B$，我们可以将所有$i\in I$写成$f_i=q_i\circ f\circ r_i$，并且足够了（MO$_\Pi$）。

¶ 请注意，如果满足以下条件，则 $r_i$ 为态射 ：

(a) 对于每个集合$E$赋予类$\Sigma$的结构，常数映射$z\mapsto a_i$是$E$的态射到$A_i$；即，对于每个$x\in I$，$p_x\circ r_i$是$A_i$到$A_x$的态射，因为当$x=i$时它是恒等映射，当$x\ne i$时它是常数映射$z\mapsto a_x$；通过乘积结构的定义，$r_i$因此是$A_i$的态射到$A$。

¶ 上面列出的例子不仅满足(a)，还满足以下条件：

(b) 每集合 $A'_i=A_i\times\prod_{x\ne i}\{a_x\}$、结构 $\mathscr{I}$ 诱导结构类 $\Sigma$。

¶ 让$p'_i$表示$p_i$到$A'_i$中的限制。如果条件(a)和(b)都满足，则$p'_i$是$A'_i$的同构到$A_i$。因为从$p'_i=p_i\circ j_i$开始，其中$j_i$是$A'_i$到$A$的典范嵌入，$p'_i$是态射乘以(MO$_\Pi$)。我们还有$r_i=j_i\circ {p'_i}^{-1}$；因此，由于结构的定义，${p'_i}^{-1}$是$A_i$的态射变为$A'_i$。

最后，我们有以下标准，它在许多情况下表征态射 ：

**CST17.** — 令$A$和$B$为两个集合，赋予相同的类$\Sigma$的结构$\mathscr{S}_A$、$\mathscr{S}_B$。假设在$\mathscr{S}_A$和$\mathscr{S}_B$的$A\times B$、结构、$\mathscr{S}_{A\times B}$、乘积上存在。令$f$为$A$的映射到$B$，令$F$为其图，并令$\pi$为$A$的双射$x\mapsto (x,f(x))$到$F$。那么，要使$f$成为$A$的态射进入$B$，由$\mathscr{S}_{A\times B}$诱发的类$\Sigma$的$F$结构上存在充分必要，且当$F$为有了这个结构，$\pi$应该是$A$的同构到$F$。

为了证明充分性，令$j$是$F$到$A\times B$的典范嵌入。我们可以写成$f=\operatorname{pr}_2\circ j\circ\pi$，那么$f$就是三个态射中的假设合成。

¶ 为了证明必要性，令$\mathscr{S}_{\mathbf{F}}$为通过双射$\pi$(§ 1, no. 5)将结构$\mathscr{S}_{\mathbf{A}}$传输到F得到的类$\Sigma$中的结构。那么我们必须证明$\mathscr{S}_{\mathbf{F}}$是由$\mathscr{S}_{\mathbf{A} \times \mathbf{B}}$在F上诱导的。我们首先注意到$j$是F的态射到$\mathbf{A} \times \mathbf{B}$；因为$j \circ \pi$是A到$\mathbf{A} \times \mathbf{B}$的映射$x \to (x, f(x))$，因此凭借$f$上的假设和乘积结构的定义是态射；因此，通过结构$\mathscr{S}_{\mathbf{F}}$的定义，$j$为态射。仍有待证明，如果E是集合赋予类$\Sigma$的结构，并且如果$g$是E到F的映射使得$j \circ g$是E到$\mathbf{A} \times \mathbf{B}$的态射，那么$g$为态射；或者，等价地，$g_1 = \overset{-1}{\pi} \circ g$是E到A的态射。但是从$g_1 = \mathrm{pr}_1 \circ (j \circ g)$开始，这是从乘积结构的假设和定义得出的。

### 5. 最终结构

考虑一个由集合$(\mathbf{A}_\iota)_{\iota \in \mathbf{I}}$组成的家庭，每个家庭都拥有结构$\mathscr{S}_\iota$或类$\Sigma$。令 E 为集合，对于每个 $\iota \in \mathbf{I}$ 令 $g_\iota$ 为映射 *of* $\mathbf{A}_\iota$ *进入* E。 E 上类 $\Sigma$ 的结构 $\mathscr{T}$ 被认为是关于 E 上的 *最终结构家庭* $(\mathbf{A}_\iota, \mathscr{S}_\iota, g_\iota)_{\iota \in \mathbf{I}}$ 如果它具有以下性质 ：

(FI) 给定任何集合 E′、E 上类 $\Sigma$ 的任何结构 $\mathscr{S}'$，以及* E *到* E′ 中的任何映射 $f$，关系

$$\text{``}f \text{ is a morphism of E into E'''}$$

*等于* 关系

$$\text{``for all } \iota \in \mathbf{I}, f \circ g_\iota \text{ is a morphism of } \mathbf{A}_\iota \text{ into E'''}.$$

CST18。 *如果* E *上存在最终的结构，相对于家庭* $(\mathbf{A}_\iota, \mathscr{S}_\iota, g_\iota)_{\iota \in \mathbf{I}}$，*那么它是* E *上的类* $\Sigma$ *中最好的结构，其中每个映射* $g_\iota$ *都是态射，因此是唯一的。*

令$\mathscr{T}$为E上的最终结构，并令$\mathscr{S}$为E上类$\Sigma$的结构，其中每个$g_\iota$为态射。如果$i$表示赋予$\mathscr{T}$的E的恒等映射到赋予$\mathscr{S}$的E上，则对于每个$\iota \in \mathbf{I}$，$i \circ g_\iota$是态射。 条件 (FI) 然后显示 $i$ 是态射，这意味着 (no. 2) $\mathscr{S}$ 比 $\mathscr{T}$ *粗糙*。 应用 (FI) 再次对于$f$是E（赋予$\mathscr{T}$）的恒等映射到其自身的情况，我们看到（使用$(\mathrm{MO_{III}})$）每个$g_\iota$是$\mathbf{A}_\iota$的态射进入E。这就完成了证明。

可能会发生 E 上存在类 $\Sigma$ 的结构，这是 E 上所有类 $\Sigma$ 的结构中最好的，而 $g_\iota$ 是态射，但是这个结构不是最终的结构相对于家庭$(\mathbf{A}_\iota, \mathscr{S}_\iota, g_\iota)$（习题6）。

我们有以下*传递性标准*：

CST19。 *设*E*为集合，让*$(\mathrm{A}_\iota)_{\iota \in \mathrm{I}}$*为集合的一个家庭，并且对于每个*$\iota \in \mathrm{I}$*让*$\mathscr{S}_\iota$*为类*$\Sigma$*上的结构*$\mathrm{A}_\iota$。 *让*$(\mathrm{J}_\lambda)_{\lambda \in \mathrm{L}}$*成为*I的划分，*并让*$(\mathrm{B}_\lambda)_{\lambda \in \mathrm{L}}$*成为由*L索引的集合族。 *对于每个*$\lambda \in \mathrm{L}$，*让*$h_\lambda$*成为*$\mathrm{B}_\lambda$的映射*进入*E； *对于每个*$\lambda \in \mathrm{L}$*和每个*$\iota \in \mathrm{J}_\lambda$，*让*$g_{\iota\lambda}$*成为*$\mathrm{A}_\iota$的映射*放入*$\mathrm{B}_\lambda$，*并放入*$f_\iota = h_\lambda \circ g_{\iota\lambda}$。 *假设，对于每个*$\lambda \in \mathrm{L}$，*存在一个最终的结构*$\mathscr{S}'_\lambda$*在*$\mathrm{B}_\lambda$*相对于家庭*$(\mathrm{A}_\iota,\ \mathscr{S}_\iota,\ g_{\iota\lambda})_{\iota \in \mathrm{J}_\lambda}$。 *那么以下叙述是等价的*：

(a) *对于家庭* $(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in \mathrm{I}}$ *在* E *上存在最终的结构* $\mathscr{S}$。

(b) *对于家庭* $(\mathrm{B}_\lambda, \mathscr{S}'_\lambda, h_\lambda)_{\lambda \in \mathrm{L}}$ *在* E *上存在最终的结构* $\mathscr{S}'$。

*此外，这些叙述意味着*$\mathscr{S} = \mathscr{S}'$。

设F为集合赋予类$\Sigma$结构，设$u$为E的映射入F。由定义，关系》$u \circ h_\lambda$为$\mathrm{B}_\lambda$态射入F”相当于关系

“对于所有 $\iota \in \mathrm{J}_\lambda$，$u \circ h_\lambda \circ g_{\iota\lambda} = u \circ f_\iota$ 是 $\mathrm{A}_\iota$ 的态射进入 F”。

关系

(3) “对于所有 $\lambda \in \mathrm{L}$，$u \circ h_\lambda$ 是 $\mathrm{B}_\lambda$ 中的态射进入 F”

因此相当于关系

(4) “对于所有 $\iota \in \mathrm{I}$，$u \circ f_i$ 是 $\mathrm{A}_\iota$ 中的态射进入 F”。

说$\mathscr{S}'$对于$(\mathrm{B}_\lambda, \mathscr{S}'_\lambda, h_\lambda)_{\lambda \in \mathrm{L}}$来说是最终的结构，意味着关系(3)相当于关系“$u$是E（赋予$\mathscr{S}'$）到F的态射”；并说E是关于家庭$(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in \mathrm{I}}$的最终结构意味着关系（4）相当于关系“$u$是E（赋予$\mathscr{S}$）到F的态射”；因此，鉴于最终结构的唯一性中的性质。

### 6. 决赛例结构

I。 *结构的直接像。*当I是单个元素的集合由……组成时，相对于$(\mathrm{A}, \mathscr{S}, f)$的最终结构称为*$f$*下的*直接像结构* $\mathscr{S}$（当存在时）。

II。 *商结构.* 设A为集合，赋予类$\Sigma$的结构$\mathscr{S}$，令R为A上的等价关系，并令$\varphi$为A上的典范映射商集$\mathrm{E} = \mathrm{A}/\mathrm{R}$（章II, § 6, no. 2）。 映射 $\varphi$下的结构 $\mathscr{S}$的直接像被关系 R调用（当存在时）结构 $\mathscr{S}$的*商*。

\* 一般来说，序结构或代数结构不承认商结构关于任意等价关系（cf.章III, § 1，习题2）。另一方面，对于任意等价关系，拓扑总是承认商结构，但对于 Hausdorff 拓扑则不一定如此。 \*

设A、B为分别赋予类$\Sigma$的结构、$\mathscr{S}$、$\mathscr{S}'$的两个集合，设$f$为A到B的态射。 令R为等价关系$f(x) = f(y)$，令$\varphi$为A到$\mathrm{A}/\mathrm{R}$的典范映射，令$j$为$f(\mathrm{A})$到B的典范嵌入。 假设$\mathscr{S}$关于R承认商结构$\mathscr{S}_0$，并且关于$f(\mathrm{A})$承认$\mathscr{S}'$诱导结构$\mathscr{S}'_0$。 那么，在$f$（章II, § 6, no. 5）的*规范分解* $f = j \circ g \circ \varphi$中，$\mathrm{A}/\mathrm{R}$的双射$g$到与$f$相关联的$f(\mathrm{A})$是一个*态射*（但不是必然是同构），当$\mathrm{A}/\mathrm{R}$被赋予$\mathscr{S}_0$并且$f(\mathrm{A})$被赋予$\mathscr{S}'_0$时。 因为$j \circ g$是$\mathrm{A}/\mathrm{R}$的态射通过商结构的定义进入B，因此$g$是$\mathrm{A}/\mathrm{R}$的态射通过诱导结构的定义进入$f(\mathrm{A})$。

CST20。 *设* A、A′ *为两个集合，赋予类* $\Sigma$*的结构* $\mathscr{S}$、$\mathscr{S}'$，*并让* R (*分别* R′) *在* A (*分别* A′) 上为等价关系。 *假设存在商结构* $\mathscr{S}_0$ (*resp.* $\mathscr{S}'_0$) *of* $\mathscr{S}$ *by* R (*resp.* $\mathscr{S}'$ *by* R′)。 *如果*$f$*是*A*的态射*到*A′*，它与等价关系*R*和*R′相容的，*并且如果*$g$*是从*$f$*通过经过到商获得的映射，则* $g$ *是* $\mathrm{A}/\mathrm{R}$ *的态射 *到* $\mathrm{A}'/\mathrm{R}'$。

令$\varphi$（或$\varphi'$）为A到$\mathrm{A}/\mathrm{R}$的典范映射（或A′到$\mathrm{A}'/\mathrm{R}'$的典范映射）；那么我们就有$g \circ \varphi = \varphi' \circ f$。由于$\varphi'$和$f$是态射，所以$\varphi' \circ f$乘以($\mathrm{MO_{II}}$)。但是，$g \circ \varphi$是态射，$g$也是态射乘以商结构的定义。

¶ 传递性标准 CST19 特别产生以下标准：

CST21。 *设* A *为集合，赋予结构* $\mathscr{S}$ * of 类* $\Sigma$，*并让* R *在* A *上为等价关系，使得存在于* $\mathrm{A}/\mathrm{R}$ *商结构* $\mathscr{S}'$ *of* $\mathscr{S}$ *作者：R. *设* S *为* A *上的等价关系，比* R 更粗糙，*并让* $\mathrm{S}/\mathrm{R}$ *表示* $\mathrm{A}/\mathrm{R}$ *上的等价关系，这是* S *与* R 的商（章 II, § 6, no. 7）。 *则存在于* $(\mathrm{A}/\mathrm{R})/(\mathrm{S}/\mathrm{R})$ *商结构* $\mathscr{S}''$ *of* $\mathscr{S}'$ *by* $\mathrm{S}/\mathrm{R}$ *当且仅当存在于* $\mathrm{A}/\mathrm{S}$ *商结构* $\mathscr{S}_0$ *of* $\mathscr{S}$ *由* S，*和典范映射的* $\mathrm{A}/\mathrm{S}$（*赋予* $\mathscr{S}_0$）*到* $(\mathrm{A}/\mathrm{R})/(\mathrm{S}/\mathrm{R})$（*赋予* $\mathscr{S}''$）*为同构。*

令$\varphi$为A到$A/R$的规范映射，令$\psi$为$A/R$到$(A/R)/(S/R)$的规范映射。 根据 CST19，当且仅当 $\mathscr{S}''$ 是相对于 $(A,\mathscr{S},\psi\circ\varphi)$ 的最终结构时，$\mathscr{S}''$ 是 $\mathscr{S}'$ 除$S/R$ 的商。 该标准是根据关系 $\psi(\varphi(x))=\psi(\varphi(y))$ 等价于 S 的事实得出的。

#### 注 {#ens-iv-s2-n6-rem-1 .statement tag=03VW}

令A为集合赋予类$\Sigma$的结构$\mathscr{S}$，并令R为A上的等价关系，使得R上存在$\mathscr{S}$的$E=A/R$商结构$\mathscr{S}'$。令$\varphi$为A到E的典范映射。一般来说，不存在$\varphi$(章II, § 3, no. 8)的*截面*$s$，即E到A的*态射*。让我们假设这样的截面$s$存在，并且在$s(E)$上存在由$\mathscr{S}$诱发的结构$\mathscr{S}''$。那么，如果 $j$ 表示 $s(E)$ 的典范嵌入到 A 中，并且如果 $s=j\circ f$，则双射 $f$ 是 E 到 $s(E)$ 的 *同构*。因为$f$是由结构的定义诱导的态射，并且$g=\varphi\circ j$是由于(MO$_{\mathrm{II}}$)而在E上的$s(E)$的态射。由于$g\circ f$和$f\circ g$分别是E和$s(E)$的恒等映射，因此断言是CST8的推论。

### 习题{#ens-iv-s2-exercises}

参见[习题为 § 2](exercises/s2/)。
