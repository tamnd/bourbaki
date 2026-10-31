---
book: alg
book_title: Algebra
chapter: I
chapter_title: ALGEBRAIC STRUCTURES
section: 4
section_title: Groups and groups with operators
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 30-52, 132-140
pdf_pages: 0054-0076, 0156-0164
extraction: ocr
subsections:
    - "no": 1
      title: GROUPS
      page: 30
      pdf_page: 54
    - "no": 2
      title: GROUPS WITH OPERATORS
      page: 31
      pdf_page: 55
    - "no": 3
      title: SUBGROUPS
      page: 32
      pdf_page: 56
    - "no": 4
      title: QUOTIENT GROUPS
      page: 34
      pdf_page: 58
    - "no": 5
      title: DECOMPOSITION OF A HOMOMORPHISM
      page: 37
      pdf_page: 61
    - "no": 6
      title: SUBGROUPS OF A QUOTIENT GROUP
      page: 38
      pdf_page: 62
    - "no": 7
      title: THE JORDAN-HÖLDER THEOREM
      page: 41
      pdf_page: 65
    - "no": 8
      title: PRODUCTS AND FIBRE PRODUCTS
      page: 45
      pdf_page: 69
    - "no": 9
      title: RESTRICTED SUMS
      page: 47
      pdf_page: 71
    - "no": 10
      title: MONOGENOUS GROUPS
      page: 48
      pdf_page: 72
statements: 63
exercises: 26
content_sha256: cd1580cf47d594bf748d080a2b9ee183400f7afde632699698346cccdd70935f
translated_from: content/en/alg/I/04_s4_groups_and_groups_with_operators.md
translation_method: google
source_content_sha256: d6bc940de2b7bc4d5c77deed1610950a126e1ac53cd26ce4b8099a1f2945d150
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 7c4b599e3e0b738d053218e3dcfd82f3525f081f0a567faaf116f8e2551d0ee6
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 4。 群和群与操作员

### 1.群

回忆一下下面的定义（§ 2, no. 3，定义 6）。

#### 定义 1 {#alg-i-s4-def-1 .statement tag=058H}

*集合与合成的结合律律，拥有单位元素，并且在其下每个元素都是可逆的，称为群。*

在其他字，群是一个*幺半群*（§ 2, no. 1，定义1），其中每个元素都是可逆的。 集合上的合成的律，其中确定群结构称为*群运算*。如果G和H是两个群，则G进入H的岩浆同态也称为*群同态*。这样同态$f$映射单位元素到单位元素；对于，令$e$（或$e'$）为G（或H）的单位元素；将G和H的群运算乘法，$e \cdot e = e$，从而$f(e) \cdot f(e) = f(e)$，然后乘以$f(e)^{-1}, f(e) = e'$。因此 $f$ 是单位的。然后从§ 2的no. 3得出$f(x^{-1}) = f(x)^{-1}$对于所有$x \in G$。

#### 例 {#alg-i-s4-n1-exa-1 .statement tag=058I}

在可逆元的任何幺半群 E 集合中，由 E 上的群诱导出结构。特别是，集合 F 的双射映射自身的集合（或 F 的 *置换* 的集合）是律 $(f, g) \mapsto f \circ g$ 下的群，称为 *对称群集合* F，记为$\mathfrak{S}_F$。

在本段中，除非另有说明，群的合成的律将始终被写为“乘法”，并且$e$将表示这样的群运算的单位元素。

如果 G 的底层集合是有限的，则群 G 被称为“有限”；否则它被称为*无限*； 群的基数称为群的*阶*。

如果合成的律在G上确定群结构在G上，则相反的律也是如此。 群 G 的映射与每个 $x \in G$ 关联，$x$ 的倒数是 G 的 *同构* 到相反的群 (§ 2, no. 3, 命题 4)。

根据我们的一般约定（*集合理论*，II, § 3, no. 1），我们将在映射$x \mapsto x^{-1}$下用G的子集A的$A^{-1}$像来表示。但对于注来说，重要的是，尽管有记号的类比，$A^{-1}$绝对不是G的子集之间合成$(X, Y) \mapsto XY$的律下A的逆元素（回想一下，XY是$xy$的集合和$x \in X, y \in Y$）：这个律下的单位元素是$\{e\}$，这个律下的$\mathscr{P}(G)$唯一的可逆元是集合单个元素的由……组成（而且，这样的A肯定有逆$A^{-1}$）。身份

$(AB)^{-1}=B^{-1}A^{-1}$ 适用于$A\subset G$、$B\subset G$。如果$A=A^{-1}$，$A$ 称为$G$ 的对称子集。对于所有 $A\subset G$、$A\cup A^{-1}$、$A\cap A^{-1}$ 和 $AA^{-1}$ 都是对称的。

### 2. 群与操作员

#### 定义 2 {#alg-i-s4-def-2 .statement tag=058J}

令$\Omega$为集合。 群$G$与$G$上$\Omega$的作用一起，相对于群运算可分配，称为群，运算符位于$\Omega$。

下面$x^\alpha$将表示$\alpha\in\Omega$和$x\in G$的合成。 分配律则由恒等式$(xy)^\alpha=x^\alpha y^\alpha$表示。

在群和运算符$G$中，每个运算符定义底层*群结构*的一个*自同态*；这些自同态将有时称为群与运算符$G$的*同位*。

如果群运算是可交换的，则带有运算符 $G$ 的群称为*可交换*（或 *阿贝尔的*）。

接下来，群$G$将被识别为群，其中$\varnothing$中的运算符是通过给$G$赋予$\varnothing$在$G$上唯一的作用而获得的。这使我们能够将群视为群与运算符的特殊情况，并将其应用于定义以及我们将说明的与后者相关的结果。

#### 例 {#alg-i-s4-n2-exa-1 .statement tag=058K}

在可交换的群 $G$ 中，乘法书写，$(xy)^n=x^ny^n$ 对于所有 $n\in\mathbf{Z}$（§ 2, no. 8，方程 (1)）； $G$上的$\mathbf{Z}$的作用$n\mapsto(x\mapsto x^n)$因此定义，以及群运算、群的结构以及$G$上的运算符。

#### 定义 3 {#alg-i-s4-def-3 .statement tag=058L}

设$G$和$G'$为群，运算符位于$\Omega$中。 群的同态与$G$的运算符进入$G'$是群*$G$的*同态进入*群*$G'$，这样

$$
f(x^\alpha)=(f(x))^\alpha
$$

对于所有 $\alpha\in\Omega$ 和所有 $x\in G$。

带有运算符 $G$ 的群的 *自同态* 是群 $G$ 的自同态，它与 $G$ 的所有 *同位性 * 可*置换*。

由于群与运算符 $G$ 的两个同位不一定是可置换的，因此 * $G$ 的位似一般不等于群与运算符 $G$ 的自同态。*

带有运算符的群的恒等映射是带有运算符的群的同态； 群与运算符的两个同态的合成也是一个。为了使映射成为带有运算符的群的同构，它是带有运算符的群的双射同态是充分必要的，并且逆映射是带有运算符的群的同构。

更一般地，令 G（或 G'）为群，运算符为 $\Omega$（或 $\Omega'$）。设$\phi$为$\Omega$的映射到$\Omega'$。 G 到 G' 的 $\phi$ 同态是群 G 到群 G' 的同态，使得

$$
f(x^\alpha) = (f(x))^{(\phi(\alpha))}
$$

对于所有 $\alpha \in \Omega$ 和所有 $x \in G$。

在本段的其余部分中，我们将得到集合 $\Omega$。 除非另外提到的群考虑了运算符将承认$\Omega$作为运算符的集合。

### 3.子群

#### 定义 4 {#alg-i-s4-def-4 .statement tag=058M}

*设 G 为群且带有运算符。 G 的稳定子群是 G 的子集 H，具有以下属性*：

(i) $e \in H$；
(ii) $x, y \in H \implies xy \in H$；
（三）$x \in H \implies x^{-1} \in H$；
(iv) $x \in H$和$\alpha \in \Omega$意味着$x^\alpha \in H$。

如果 H 是 G 的稳定子群，则由群的结构在 G 上使用算子在 H 上诱导的结构是群的结构，并且 H 到 G 的典范嵌入是同态群与操作员。

令 G 为群。 G 的稳定子群，作用为$\varnothing$ (no. 2)，即子集的 G 满足条件 (i), (ii), (iii) of 定义 4，称为G 的 *子群*。当我们谈到运算符的群的子群时，我们总是指 G 的底层群的子群。运算符 G 的群的子群不一定是 G 的稳定子群。

*例* (1)。令$\Sigma$为结构的类（*集合理论*，IV, § 1, no. 4），以及集合E上的类$\Sigma$的S结构（*loc.cit.*）。 S的*自同构*集合是$\mathscr{G}_E$子群。

#### 命题 1 {#alg-i-s4-prop-1 .statement tag=058N}

*设 G 为带有运算符的群，G 的 H 子集在 G 的同位下是稳定的。以下条件是等价的*：

(a) *H 是 G* 的稳定子群。
(b) *H 非空且关系* $x \in H, y \in H \implies xy \in H$ *和* $x^{-1} \in H$。
(c) *H 非空且关系* $x \in H, y \in H \implies xy^{-1} \in H$。
(d) *H 在 G 上的律下是稳定的，并且由 G 上的合成的律在 H 上诱导的合成律是群运算*。

显然（a）意味着（b）。我们证明（b）蕴涵（a）。只要证明 G 的 H 包含单位元素就足够了。由于子集 H 非空，所以设 $x \in H$。然后是$x^{-1} \in H$和$e = xx^{-1} \in H$。显然（b）暗示着（c）。我们证明（c）蕴涵（b）。首先，由于 H 非空，因此包含元素 x。因此 xx^{-1} = e 是 H 的元素。对于 H 的每个元素 x，$x^{-1} = ex^{-1}$ 属于到 H；因此关系$x \in H, y \in H$意味着$x(y^{-1})^{-1} = xy \in H$。显然（a）意味着（d）。我们证明(d)蕴含(a)：H到G的典范嵌入是群同态；因此$e \in H$和关系$x \in H$意味着$x^{-1} \in H$（no. 1）。

#### 注 {#alg-i-s4-n3-rem-1 .statement tag=058O}

(1) 类似地可以证明条件 (b) 等价于条件
(c') $H \neq \varnothing$ 和关系 $x \in H$ 和$y \in H$ 意味着$y^{-1}x \in H$。
(2) 对于G的每个子群 H，有以下关系
$$(1)$$
$$H.H = H \quad \text{and} \quad H^{-1} = H.$$
对于 $H.H \subset H$ 和 $H^{-1} \subset H$ 由 (b) 得出。作为 $e \in H, H.H \supset e.H = H$ 并取逆变换将 $H^{-1} \subset H$ 包含到 $H \subset H^{-1}$、从而公式 (1)。

如果H是G的稳定子群并且K是H的稳定子群，则显然K是G的稳定子群。

G的集合$\{e\}$是最小的稳定子群。G的稳定子群族的交是稳定子群。因此，G 的最小的稳定子群 H 包含给定的 G 子集 X；它被称为* X生成的*稳定子群，而X被称为H的*生成的系统*（或*生成的集合*）。

#### 命题 2 {#alg-i-s4-prop-2 .statement tag=058P}

*设X是群的非空子集，具有运算符G和$\hat{X}$，X生成的G上$\Omega$的作用下的稳定子集。 X生成的稳定子群是集合$Y = \hat{X} \cup \hat{X}^{-1}$生成的G上律下的稳定子集。*

后者子集Z是有限序列的合成的集合，其所有的项都是$\hat{X}$的元素或$\hat{X}$的元素的逆：这样的合成的逆是合成相同的形式（§ 2, no. 3，推论1到命题5），并且Z在$\Omega$的作用下是稳定的，正如通过应用§ 3, no. 4，命题1与G的同位性所见，因此（命题1）Z是G 的*稳定子群*。相反，每个稳定子群包含X显然包含Y，因此Z。

#### 推论 1 {#alg-i-s4-prop-2-cor-1 .statement tag=058Q}

*设 G 为带有运算符的群，G 的X子集在$\Omega$ 的作用下稳定。由X生成的子群和由X重合生成的稳定版子群。*

#### 推论 2 {#alg-i-s4-prop-2-cor-2 .statement tag=058R}

*设 G 为成对可置换元素的 G 由……组成的群和 X 子集。由X生成的G的子群是可交换的。*

集合 $Y = X \cup X^{-1}$ 由成对可置换元素 (§ 2, no. 3, 命题 5) 和律组成，在由 Y 生成的稳定子集上诱导是可交换的（§ 1, no. 5，推论 2）。

如果 G 是具有运算符的群，则成对可置换元素的 G 由……组成的子集生成的稳定子群不一定是可交换的。

#### 推论 3 {#alg-i-s4-prop-2-cor-3 .statement tag=058S}

令$f : G \to G'$为带有运算符的群的同态和G的X子集。X生成的G的稳定子群的f下的像是$f(X)$生成的G'的稳定子群。

让$X' = f(X)$。然后是$\hat{X}' = f(\hat{X})$和${X'}^{-1} = f(X^{-1})$。因此
$$
f(\hat{X} \cup \hat{X}^{-1}) = \hat{X}' \cup \hat{{X}'}^{-1}.
$$
然后从 § 1, no. 4、命题 1 得出推论。

例 (2)。令 G 为 G 的群，x 元素。由 $\{x\}$ 生成的子群（更简单地称为由 x 生成的子群）是 $x^n, n \in \mathbf{Z}$ 的集合。由$\{x\}$生成的稳定子集（在G上的律下）是$x^n$的集合，其中$n \in \mathbf{N}^*$。这两个集合总体上是不同的。

因此，在加法群$\mathbf{Z}$中，元素x生成的子群是$xn, n \in \mathbf{Z}$的集合$x.\mathbf{Z}$，而x生成的稳定的子集是$xn, n \in \mathbf{N}^*$的集合。如果$x \neq 0$，这两个集合总是不同的。

G 的稳定子群的右向族的并显然是稳定的子群。由此可见，如果 P 是 G 和 H 的子集，则 G 的稳定子群不满足 P，G 包含 H 的稳定子群的集合且不满足 P，按包含排序，是归纳的（集合理论，III, § 2, no. 4）。 应用 Zorn 的引理（集合理论，III, § 2, no. 4），我们得到以下结果：

#### 命题 3 {#alg-i-s4-prop-3 .statement tag=058T}

设G为群，且有算子，G和H的P子集是不满足P的稳定子群G。G包含H的稳定子群的集合且不满足P有极大元素。

### 4.商群

#### 定理 1 {#alg-i-s4-thm-1 .statement tag=058U}

令 R 为群上的等价关系，且具有运算符 G；如果 R 与 G 上的群运算左（或右）相容的（§ 3, no. 3）并与 $\Omega$ 的作用兼容，则 e 的等价类是 G 的稳定子群 H，并且关系 R 相当于 $x^{-1}y \in H$（或 $yx^{-1} \in H$）。相反，如果 H 是 G 的稳定子群，则关系 $x^{-1}y \in H$（分别为 $yx^{-1} \in H$）为等价关系，其左（或右）与 G 上的群运算兼容，并且与 $\Omega$ 的作用兼容，并且在其下 H 为e 的等价类。

我们将注意力限制在关系 R 与 G 上的律左兼容的情况（右兼容关系的情况紧随 G 上的替换律的相反的律）。 关系 $y \equiv x \pmod{R}$ 等价于 $x^{-1}y \equiv e \pmod{R}$，因为 $y \equiv x$ 意味着 $x^{-1}y \equiv x^{-1}x = e$，反之，$x^{-1}y \equiv e$ 意味着 $y = x(x^{-1}y) \equiv x$。如果 H 表示 e 的等价类，则关系 R 相当于 $x^{-1}y \in H$。我们证明H是G的稳定子群。对于每个算子$\alpha$，关系$x \equiv e$意味着$x^\alpha \equiv e^\alpha = e$，因此$H^\alpha \subset H$并且H在$\Omega$的作用下是稳定的。只要建立(命题 1)，$x \in H$和$y \in H$隐含$x^{-1}y \in H$，即$x \equiv e$和$y \equiv e$隐含$x \equiv y$，即R的传递性的推论。

反之，令 H 为 G 的稳定子群； 关系 $x^{-1}y \in H$ 自 $x^{-1}x = e \in H$ 起自反；它是对称的，因为 $x^{-1}y \in H$ 蕴含 $y^{-1}x = (x^{-1}y)^{-1} \in H$；它是及物性的，因为$x^{-1}y \in H$和$y^{-1}z \in H$意味着$x^{-1}z = (x^{-1}y)(y^{-1}z) \in H$；它与G上的合成的律兼容，对于所有$z \in G$，$x^{-1}y = (zx)^{-1}(zy)$；最后，对于每个运算符$\alpha$，关系$y \in xH$意味着$y^\alpha \in x^\alpha H^\alpha \subset x^\alpha H$，因此等价关系$x^{-1}y \in H$与G上的$\Omega$的作用兼容。

设G为G的群且H子群； 关系 $x^{-1}y \in H$（分别为 $yx^{-1} \in H$）也可写成等效的形式 $y \in xH$（分别为 $y \in Hx$）。 G 的每个子群 H 因此定义 G 上有两个等价的关系，即$y \in xH$和$y \in Hx$：这些关系下的等价类分别是集合$xH$，称为H*的*左陪集（或*模 H*) 和集合 $Hx$，它们被称为 *H* 的右陪集（或 *模 H*）。通过对这些关系（*集合理论*，II, § 6, no. 4）*饱和*子集$A \subset G$，我们分别获得集合AH和HA。 映射 $x \mapsto x^{-1}$ 变换左陪集模 H 变为右陪集模 H，反之亦然。

左陪集（mod.H）集合的基数称为子群H相对于G的*指标*，记为$(G:H)$；它也等于右陪集集合的基数。

如果G的子群K包含H，则它是H的左（或右）陪集的并。由于K的左陪集是通过左平移从K获得的，因此K的左陪集中包含的H的左陪集的集合具有独立于后者的基数。因此（*集合理论*，III, § 5, no. 8，命题9）：

#### 命题 4 {#alg-i-s4-prop-4 .statement tag=058V}

*令 H 和 K 为群 G 中的两个子群，使得 H $\subset$ K。那么*
$$
(G:H) = (G:K)(K:H).
$$

#### 推论{#alg-i-s4-n4-cor-1 .statement tag=058W}

*如果G是阶g的有限群并且H是阶h的G的子群，那么*
$$
h \cdot (G:H) = g
$$
（特别是，H的阶和指标是G的阶的*除子*）。

定理 1 允许我们使用运算符 G 确定等价关系与群上的律兼容：如果 R 是这样的关系，则它与 G 上的群运算左右兼容，并与 G 上的作用兼容$\Omega$。因此，如果 H 是 $e$ (mod. R) 的类，则 H 是稳定的子群，使得关系 $y \in xH$ 和 $y \in Hx$ 等价（因为两者都等价于 R）；因此 $xH = Hx$ 对于所有$x \in G$。相反，如果是这样，则等效的关系$y \in xH, y \in Hx$中的一个或另一个与群运算兼容，因为它与此律（$\S$3，no. 4）左右兼容，并且与$\Omega$的作用兼容。由于方程 $xH = Hx$ 等价于 $xHx^{-1} = H$，因此我们得出以下定义：

#### 定义 5 {#alg-i-s4-def-5 .statement tag=058X}

*设 G 为群且带有运算符。如果对于所有 $x \in G$ 都有 $xHx^{-1} = H$，则 G 的稳定子群 H 称为 G 的正常（或不变）稳定子群。*

如果 $\Omega = \varnothing$，G 的正规稳定子群称为 G 的*正规*（或*不变*）*子群*。在交换性群中，每个子群都是正规的。

为了验证稳定的子群 H 是正常的，只需证明 $xHx^{-1} \subset H$ 对于所有 $x \in G$ 即可；如果是这样，那么 $x^{-1}Hx \subset H$ 对于所有 $x \in G$，即 $H \subset xHx^{-1}$，因此$H = xHx^{-1}$。

设 H 为 H 定义的 G 和 R 等价关系 $y \in xH$ 的正规稳定子群；在商集$G/R$上，内部律，律与R除以群G的商，是结合律； e 的类是该商律的单位元素； G 中的两个倒数元素的类是 $\Omega$ 的商律和作用下的倒数，G 上的 $\Omega$ 作用与 R 的商，相对于内部律是可分配的$G/R$（$\S$3，no. 5）。因此，总结所获得的结果：

#### 定理 2 {#alg-i-s4-thm-2 .statement tag=058Y}

*设 G 为群且带有运算符。为了使G上的等价关系R与$\Omega$的群运算和作用兼容，它是形式$x^{-1}y \in H$是必要且充分的，其中H是G的正常稳定子群（关系$x^{-1}y \in H$此外相当于$yx^{-1} \in H$对于这样的子群）。 合成在$G/R$上的商律和$\Omega$在$G/R$上的作用与$\Omega$在G上的商通过这样的关系R得到$G/R$结构群带运算符，称为商结构，商通道的典范映射是群带运算符的同态。*

#### 定义 6 {#alg-i-s4-def-6 .statement tag=058Z}

*由 G 的正常子群 H 定义的群与运算符 G 与等价关系的商，与商结构称为商群与 G 的运算符与 H 并用 $G/H$ 表示。 典范映射 $G \to G/H$ 称为典范同态*

设 G 为群，H 为 G 的正规子群。商 $G/H$ 及其群结构被 H 称为 G 的 *商群*。对于从 $G/H$ 到群的映射，使用运算符为同态群对于运算符，其合成与 G 到 $G/H$ 的典范映射为一是充分必要的：这证明了名称“商群”的合理性（*集合理论*, IV, $\S$ 2, no. 6）。

由 G 的正常稳定子群定义的等价关系用$x \equiv y \pmod{H}$或$x \equiv y(H)$表示。

#### 命题 5 {#alg-i-s4-prop-5 .statement tag=0590}

令 $f : G \to G'$ 为群的同态，且具有运算符，且 $H$ 和 $H'$ 分别为 $G$ 和 $G'$ 的正常稳定子群，使得 $f(H) \subset H'$。 映射 $f$ 与$H$ 和$H'$ 定义的等价关系兼容。令$\pi : G \to G/H$和$\pi' : G' \to G'/H'$为典范同态。由 $f$ 乘以经过得出的映射 $\bar{f} : G/H \to G'/H'$ 所得商为同态。

如果$x \equiv y \pmod{H}$，则$x^{-1}y \in H$，从而
$$
f(x)^{-1}f(y) = f(x^{-1})f(y) = f(x^{-1}y) \in f(H) \subset H'
$$
因此$f(x) \equiv f(y) \pmod{H'}$。第二个断言由商律（$§ 1$，no. 6）的泛性质得出。

#### 注 {#alg-i-s4-n4-rem-1 .statement tag=0591}

(1) 如果$A$是群$G$中的任意子集且$H$是$G$的正常子群，则$AH = HA$；这个集合是通过使$A$相对于关系$x \equiv y \pmod{H}$饱和而获得的。

(2) 如果$H$是有限指标的$G$的正常子群，则商群$G/H$是阶$(G:H)$的有限群。

注如果 $H$ 是群 $G$ 的正常子群并且 $K$ 是 $H$ 的正常子群，则 $K$ 不一定是子群的正常子群 $G$（I、$§ 5$、习题10）。

使用运算符将​​ $G$ 设为群。 $G$的正常马厩子群每个家庭的交是一个正常马厩子群。因此，对于$G$的每一个子集$X$，都存在最小的正常稳定子群包含$X$，称为正常稳定子群*由*$X$生成。

在群和运算符$G$中，稳定的子群、$G$和$\{e\}$是正常的。

#### 定义 7 {#alg-i-s4-def-7 .statement tag=0592}

*带有运算符的群* $G$ *被称为简单if* $G \neq \{e\}$ *并且除了* $G$ *和* $\{e\}$ 之外，不存在* $G$ *正常稳定的子群。

### 5.分解同态

#### 命题 6 {#alg-i-s4-prop-6 .statement tag=0593}

*设* $G$ *为群运算符和* $G'$ *岩浆与作用乘以* $\Omega$，*以指数形式写入*。 *让*$f : G \to G'$*成为玛格纳*$G$*进入岩浆*$G'$*的同态，这样，对于所有*$\alpha \in \Omega$*和所有*$x \in G$，$f(x^\alpha) = f(x)^\alpha$。 *那么* $f(G)$ *是* $G'$ *在* $G'$ *上的律和* $\Omega$的作用的稳定子集； *集合* $f(G)$ *诱导的律是带有运算符的群，而映射* $x \mapsto f(x)$ *of* $G$ *进入* $f(G)$ *是带有运算符的群的同态*。

凭借$§ 1$、no. 4、命题 1，$f(G)$ 是$G'$ 上内部律下$G'$ 的稳定子集。对于每个元素 $x \in G$ 和每个运算符 $\alpha$，
$f(x)^\alpha = f(x^\alpha) \in f(G)$，因此$f(G)$在$G'$上的$\Omega$的作用下是稳定的。乘法写出$G'$的内部律，
$$
(f(x)f(y))f(z) = f(xy)f(z) = f((xy)z) = f(x(yz)) = f(x)f(yz)
= f(x)(f(y)f(z))
$$
对于 $G$ 中的所有元素 $x, y, z$；因此，在 $f(G)$ 上导出的律是结合律。

令$e$为$G$中的单位元素。它的像$f(e)$是$f(G)$（$§ 2$，no. 1）中的单位元素。 $f(G)$ 的每个元素在 $f(G)$ ($§ 2$, no. 3) 中都是可逆的。因此，$G'$上的内部律在$f(G)$上感应出律为群运算。对于$G$中的所有元素$x$和$y$以及每个运算符$\alpha$，

$$
(f(x)f(y))^\alpha = (f(xy))^\alpha = f((xy)^\alpha) = f(x^\alpha y^\alpha) = f(x^\alpha)f(y^\alpha) = (f(x))^\alpha(f(y))^\alpha
$$

这表明$\Omega$的作用相对于$f(G)$上的群运算是可分配的。因此，$f(G)$ 与诱导的律是群运算符，并且显然映射 $x \mapsto f(x)$ 是群的同态运算符。

#### 定义 8 {#alg-i-s4-def-8 .statement tag=0594}

*使用运算符将​​ $f : G \to G'$ 设为群中的同态。 $G'$单位元素逆像称为$f$核。*

$f$的核通常用$\mathrm{Ker}(f)$表示，$f$的像$f(G)$通常用$\mathrm{Im}(f)$表示有时。

#### 定理 3 {#alg-i-s4-thm-3 .statement tag=0595}

*使用运算符将 $f : G \to G'$ 设为群中的同态。*
(a) *$\mathrm{Ker}(f)$ 是 $G$ 的正常稳定子群；*
(b) *$\mathrm{Im}(f)$ 是 $G'$ 的稳定子群；*
(c) *映射$f$与$\mathrm{Ker}(f)$在$G$上定义的等价关系兼容；*
(d) *映射 $\tilde{f} : G/\mathrm{Ker}(f) \to \mathrm{Im}(f)$ 由 $f$ 通过经过通过运算符得出商为群的同构；*
(e) *$f = i \circ \tilde{f} \circ \pi$，其中$i$是$\mathrm{Im}(f)$到$G'$的典范嵌入，$\pi$是$G$到$G/\mathrm{Ker}(f)$的典范同态。*

断言 (b) 源自命题 6。$G$ 上的等价关系 $f(x) = f(y)$ 与群以及$G$ 上的运算符结构兼容。到定理 2 (no. 4)，因此它是形式$y \in xH$，其中$H$是$G$的正常稳定子群，$H$是单位元素的类， 从而$H = \mathrm{Ker}(f)$。 断言 (a)、(c) 和 (d) 然后是。 断言 (e) 是显而易见的（*集合理论*，II, § 6, no. 5）。

### 6.子群商群

#### 命题 7 {#alg-i-s4-prop-7 .statement tag=0596}

*设$G$和$H$为两个带有运算符的群，将$G$的$f$同态转换为$H$和$f$的$N$核。*
(a) *令 $H'$ 为 $H$ 的稳定子群。 逆像 $G' = f^{-1}(H')$ 是 $G$ 的稳定子群，如果 $H'$ 在 $H$ 中正常，则 $G'$ 在 $G$ 中正常。此外，$N$是$G'$的正常子群。如果 $f$ 是满射，则 $H' = f(G')$ 和 $f$ 定义同构的 $G'/N$ 到 $H'$ 上的经过的商。*
(b) *令 $G'$ 为 $G$ 的稳定子群。 像 $H' = f(G')$ 是 $H$ 和 $f^{-1}(H') = G'N = NG'$ 的稳定子群。特别是，$f^{-1}(H') = G'$当且仅当$N \subset G'$。如果 $f$ 是满射且 $G'$ 在 $G$ 中是正规的，则 $H'$ 在 $H$ 中是正规的。*

(a) 设$x$和$y$在$G'$和$\alpha \in \Omega$中；那么$f(x) \in H'$和$f(y) \in H'$，从而$f(xy^{-1}) = f(x)f(y)^{-1} \in H'$，即$xy^{-1} \in G'$；因此$G'$是$G$的子群。现在 $f(x^\alpha) = f(x)^\alpha \in H'$、从而 $x^\alpha \in G'$，因此 $G'$ 是稳定的。假设$H'$在$H$中是正规的，令$x \in G', y \in G$；然后 $f(x) \in H'$ 和
$$
f(yxy^{-1}) = f(y)f(x)f(y)^{-1} \in H'
$$
从而$yxy^{-1} \in G'$；因此$G'$在$G$中是正常的。对于所有 $n \in N, f(n) = e \in H'$、从而 $N \subset G'$；正如$N$在$G$中是正常的，在$G'$中也是正常的。最后，如果 $f$ 是满射，
$$
f(f^{-1}(A)) = A \text{ for every subset } A \text{ of } H,
$$
从而$H' = f(G')$； $f$到$G'$的限制是$G'$的同态$f'$到核$N$的$H'$，因此经过上有$f'$定义 $G'/N$ 的商同构到 $H'$。

(b) 设$a$和$b$在$H'$中，$\alpha$在$\Omega$中； $G'$中存在$x, y$、$a = f(x)$和$b = f(y)$、从而$ab^{-1} = f(xy^{-1}) \in H'$，因此$H'$是$H$的子群，对于$a^\alpha = f(x^\alpha) \in H'$来说是稳定的。让$x \in G$；那么$x \in f^{-1}(H')$当且仅当$f(x) \in H' = f(G')$，即当且仅当$G'$中存在$y$和$f(x) = f(y)$； 关系$f(x) = f(y)$相当于$n \in N$与$x = yn$存在；最后，$x \in f^{-1}(H')$等价于$x \in G'N = NG'$。显然关系 $G' = G'N$ 相当于 $G' \supset N$。最后假设$f$是满射，$G'$在$G$中是正规的；让 $a \in H'$ 和 $b \in H$；存在$x \in G'$和$y \in G$以及$a = f(x)$和$b = f(y)$，从而$bab^{-1} = f(yxy^{-1}) \in f(G') = H'$。因此 $H'$ 在 $H$ 中是正常的。

#### 推论 1 {#alg-i-s4-prop-7-cor-1 .statement tag=0597}

*假设 $f$ 是满射。设 $\mathscr{G}$（分别为 $\mathscr{G}'$）为稳定的集合（分别为正常稳定）子群为 $G$ 包含 $N$ 和$\mathfrak{H}$（分别为$\mathfrak{H}'$）稳定的集合 （分别为正常稳定）子群或 $H$，这些集合按包含顺序排列。 映射 $G' \mapsto f(G')$ 是有序的集合同构 $\Phi : \mathscr{G} \to \mathfrak{H}$； 逆同构$\Psi : \mathfrak{H} \to \mathscr{G}$是映射$H' \mapsto f^{-1}(H')$。进一步$\Phi$和$\Psi$诱导同构$\Phi' : \mathscr{G}' \to \mathfrak{H}'$和$\Psi' : \mathfrak{H}' \to \mathscr{G}'$。

#### 推论 2 {#alg-i-s4-prop-7-cor-2 .statement tag=0598}

*设$f : G \to H$为带有运算符的群的同态，$f$的$N$核，$G'$为$G$的稳定子群，$L$为子群的正常稳定子群 $G'$。那么$LN, L.(G' \cap N)$和$f(L)$分别是$G'N, G'$和$f(G')$的正常稳定子群，并且与算子$G'N/LN, G'/L.(G' \cap N)$和$f(G')/f(L)$的三个商群是同构的。

让$H' = f(G')$和$f'$表示$G'$到$H'$的同态，其中重合和$f$在$G'$； $f'$中的核是$G \cap N$和$f'(L) = f(L)$；到命题 7，$f'(L)$ 是 $H'$ 的正常稳定子群，并且
$$
{f'}^{-1}(f'(L)) = L.(G' \cap N)
$$
是正常稳定的子群 $G'$。设$\lambda$是$H'$到$H'/f'(L) = f(G')/f(L)$的典范同态：因为$\lambda \circ f'$与核是满射
$$
{f'}^{-1}(f'(L)) = L.(G' \cap N),
$$

将$G'/L\cdot(G'\cap N)$的定义同构转移到$f(G')/f(L)$。 命题 7，(b)，$f^{-1}(H')=G'N$；如果$f''$是$G'N$的同态到$H'$，其中重合与$G'N$上的$f$，$G'N$的同态$\lambda\circ f''$到$f(G')/f(L)$是满射核$f^{-1}(f(L))=LN$；这证明了 $LN$ 是 $G'N$ 的正常稳定子群，并且$\lambda\circ f''$ 定义同构 $G'N/LN$ 到$f(G')/f(L)$。

#### 推论 3 {#alg-i-s4-prop-7-cor-3 .statement tag=0599}

令 $f:G\to H$ 为群的同态（带运算符），$N$ 为核，$X$ 子集为 $G$，使得 $f(X)$ 生成 $H$ 且$Y$子集共$N$其中生成$N$。然后$X\cup Y$生成$N$。

令$G'$为$X\cup Y$生成的$G$的稳定子群。如$Y\subset G'$、$N\subset G'$。

如 $f(X)\subset f(G')$、$f(G')=H$、从而 $G'=f^{-1}(H)=G$。

#### 注 {#alg-i-s4-n6-rem-1 .statement tag=059A}

在命题7的记号中，$H$的子群逆像是$G$的子群的事实从以下更一般的事实得出。

如果 $A$ 和 $B$ 是 $H$ 的子集并且 $f$ 是满射，那么

$$
f^{-1}(A\cdot B)=f^{-1}(A)\cdot f^{-1}(B),\qquad
f^{-1}(A^{-1})=f^{-1}(A)^{-1}.
$$

显然$f^{-1}(A)\cdot f^{-1}(B)\subset f^{-1}(A\cdot B)$；另一方面，如果$z\in f^{-1}(A\cdot B)$，则存在$a\in A$和$b\in B$使得$f(z)=ab$；由于$f$是满射，因此存在$x\in G$使得$f(x)=a$；写$y=x^{-1}z$、$f(y)=a^{-1}f(z)=b$和$z=xy$、从而$z\in f^{-1}(A)\cdot f^{-1}(B)$。 关系 $x\in f^{-1}(A^{-1})$ 相当于$f(x)\in A^{-1}$，因此相当于$f(x^{-1})\in A$，即$x^{-1}\in f^{-1}(A)$，最后相当于$x\in f^{-1}(A)^{-1}$。

#### 命题 8 {#alg-i-s4-prop-8 .statement tag=059B}

设$G$为带有运算符的群，以及$A$和$B$两个稳定的子群$G$。假设关系$a\in A$和$b\in B$隐含$aba^{-1}\in B^{*}$（在其他字中，$A$归一化$B$）$^{*}$。那么$AB=BA$是$G$的稳定子群，$A\cap B$是$A$的正常稳定子群，$B$是$AB$的正常稳定子群。将$A$的典范嵌入代入$AB$，将经过上的定义除以$A/(A\cap B)$的同构到$AB/B$的商。

公式

$$
(ab)(a'b')=aa'({a'}^{-1}ba'\cdot b')
$$

$$
(ab)^{-1}=a^{-1}(ab^{-1}a^{-1})
$$

$$
(ab)^\alpha=a^\alpha b^\alpha
$$

对于$a,a'\in A$、$b,b'\in B$以及$G$上的每个运算符$\alpha$，证明$AB$是$G$的稳定子群。设$a\in A$和$x\in A\cap B$；那么$axa^{-1}\in B$由对$A$和$B$所做的假设得出，并且显然$axa^{-1}$属于到$A$，因此$A\cap B$在$A$中是正常的。设$a\in A$和$b,b'$在$B$中； 公式$(ab)b'(ab)^{-1}=a(bb'b^{-1})a^{-1}$表明$B$在$AB$中是正常的。令$\phi$为AB到AB/B的典范同态的限制到$A$；那么$\phi(a) = aB$，因此$\phi$的核等于$A \cap B$。显然 $\phi$ 是满射，因此 $A/(A \cap B)$ 的定义同构到 $AB/B$。

#### 定理 4 {#alg-i-s4-thm-4 .statement tag=059C}

*设 G 为群且有运算符，N 为 G 的正常稳定子群。*

(a) *映射 $G' \mapsto G'/N$ 是 G 包含 N 稳定子群集合双射到 G/N 稳定子群集合。*

(b) *令 $G'$ 为 G 包含 N 的稳定子群。要使 $G'/N$ 在 $G/N$ 中正规，$G'$ 在 G 中正规，且群 $G/G'$ 和 $(G/N)/(G'/N)$ 是充分必要的同构。*

(c) *令$G'$为G的稳定子群。则$G'N$为G的稳定子群，且N在$G'N$中是正规的。此外，$G' \cap N$在$G'$和群中是正规的，$G'/(G' \cap N)$和$G'N/N$是同构的。*

让$f$表示G到$G/N$的典范同态。对于所有$x \in G$，$f(x) \in xN$；因此，对于 G 包含 N 的每个子群 $G'$，$f(G') = G'/N$。由于 $f$ 是满射，断言 (a) 从推论 1 到命题 7；类似地，等价“G'正常”$\Leftrightarrow$“G'/N正常”。假设$G'$是G包含N的正常稳定子群。通过no. 4，命题5应用于$\mathrm{Id}_G$，存在$G/N$的同态$u$到$G/G'$定义为$u(xN) = xG'$ 对于所有$x \in G$。 $u$ 与核 $G'/N$ 从而 $(G/N)/(G'/N)$ 所需的同构到 $G/G'$ 是直接的。最后，(c) 紧随命题 8。

### 7. 乔丹-霍尔德定理

#### 定义 9 {#alg-i-s4-def-9 .statement tag=059D}

*具有运算符 G 的群的合成列是 G 的稳定子群的有限序列 $(G_i)_{0 \leq i \leq n}$，其中$G_0 = G$ 和 $G_n = \{e\}$，并且$G_{i+1}$ 是$0 \leq i \leq n-1$ 的$G_i$ 的正常子群。商$G_i/G_{i+1}$称为级数的商。如果$\Sigma$是取自$\Sigma'$的级数，则合成列$\Sigma'$据说是更细比合成列$\Sigma$。

如果$(G_i)_{0 \leq i \leq n}$和$(H_j)_{0 \leq j \leq m}$分别是带有运算符G和H的两个群的合成列，则如果$m = n$并且存在$\mathbf{N}$的区间$\{0, n-1\}$的置换$\phi$，则称它们是等价的，使得带有运算符的群 $G_i/G_{i+1}$ 和 $H_{\phi(i)}/H_{\phi(i)+1}$ 对于所有 $i$ 是同构的。

注，一般来说，取自合成列$(G_i)$的级数不是合成列，因为对于$j > i + 1$，$G_j$通常不是$G_i$的正常子群。

#### 定理 5（施赖尔）{#alg-i-s4-thm-5 .statement tag=059E}

*给定群的两个合成列$\Sigma_1, \Sigma_2$和运算符G，存在两个分别与$\Sigma_1$和$\Sigma_2$等价的合成列、$\Sigma'_1, \Sigma'_2$、更细。

令$\Sigma_1 = (H_i)_{0 \leq i \leq n}$和$\Sigma_2 = (K_j)_{0 \leq j \leq p}$为给定的两个合成列，分别为$n + 1$和$p + 1$项；我们将看到，通过在 H_i 和 H_{i+1} 之间插入 $p - 1$ 子群 $H'_{i,j}$ (1 \leq j \leq p - 1) 可以形成合成列 $\Sigma'_1$，对于 0 \leq i \leq n - 1 和级数 \Sigma_2' 通过插入 n - 1 子群 K_{j,i}' (1 \leq i \leq n - 1) 在 K_j 和 K_{j+1} 之间，对于 0 \leq j \leq p - 1；从而得到pn的两个级数+G的1个稳定的子群；通过适当选择插入的稳定子群，我们将证明这些级数是等价的合成列。

为此注 H_i \cap K_j 是 H_i 和 K_j 的稳定子群，因此 (定理 4) H_{i+1}.(H_i \cap K_j) 是 H_i 包含 H_{i+1} 和 K_{j+1}.(H_i \cap) 的稳定子群 K_j) 是 K_j 包含 K_{j+1} 的稳定子群。如果我们写 H_{i,j}' = H_{i+1}.(H_i \cap K_j) 和 K_{j,i}' = K_{j+1}.(H_i \cap K_j)，H_{i,j+1}' 是 H_{i,j}' (0 \leq j \leq p - 1) 的稳定子群并且 K_{j,i+1}' 是稳定的K_{j,i}' 的子群 (0 \leq i \leq n - 1)。此外，H_{i,0}' = H_i、H_{i,p}' = H_{i+1}、K_{j,0}' = K_j 且 K_{j,p}' = K_{j+1}。为了显示定理，只需证明 H_{i,j+1}' (分别为 K_{j,i+1}') 是 H_{i,j}' (分别为 K_{j,i}') 的正常稳定子群并且商群 H_{i,j}'/H_{i,j+1}' 和K_{j,i}'/K_{j,i+1}' 是同构的 (0 \leq i \leq n - 1, 0 \leq j \leq p - 1)。这是从以下引理得出的，取H=H_i，H'=H_{i+1}，K=K_j，K'=K_{j+1}。

#### 引理 1（扎森豪斯）{#alg-i-s4-lem-1 .statement tag=059F}

设H和K是群的两个稳定子群，分别是H和K的算子G和H'和K'正常稳定子群；则 H'.(H \cap K') 是 H'.(H \cap K) 的正规稳定子群，K'.(K \cap H') 是 K'.(K \cap H) 和商群的正规稳定子群，带有运算符 (H'.(H \cap K))/(H'.(H \cap K')) 和 (K'.(K \cap H))/(K'.(K \cap H')) 是同构的。

由定理 4 可知，H' \cap K = H' \cap (H \cap K) 是 H \cap K 的正规稳定子群；类似地，K' \cap H 是 K \cap H 的正常稳定子群；因此 (no. 6, 推论 2) (H' \cap K)(K' \cap H) 是 H \cap K 的正常稳定子群。通过定理 4 应用于群 H，

$$
H'.(H' \cap K).(K' \cap H) = H'.(H \cap K')
$$

是 H' 的正常稳定子群。(H \cap K) 和商群

$$
(H'.(H \cap K))/(H'.(H \cap K))
$$

同构于

$$
(H \cap K)/((H' \cap K).(K' \cap H)).
$$

在最后一个商中，一方面是 H 和 H'，另一方面是 K 和 K' 对称出现；将它们排列即可获得所述结果。

#### 定义 10 {#alg-i-s4-def-10 .statement tag=059G}

具有运算符 G 的群的 Jordan-Hölder 级数是严格递减分解级数 \Sigma，这样不存在与 \Sigma 不同的严格递减分解级数和与 \Sigma 不同的更细。

#### 命题 9 {#alg-i-s4-prop-9 .statement tag=059H}

为了使 G 的分解级数成为 Jordan-Hölder 级数，级数的所有商都是简单的是充分必要的。

分解级数是严格递减当且仅当其连续商都没有减少到单位元素。如果严格递减合成列 $\Sigma$ 不是 Jordan-Hölder 级数，则存在严格递减合成列 $\Sigma'$，其更细比 $\Sigma$ 且与 $\Sigma$ 不同。因此$\Sigma$中有两个连续的项$G_i, G_{i+1}$在$\Sigma'$中不连续；设$H$为$\Sigma'$中$G_i$之后的第一个项； $H$是$G_i$、包含$G_{i+1}$的正常稳定版子群，与后者不同；因此$H/G_{i+1}$是$G_i/G_{i+1}$的正常稳定子群，与后者和单位元素不同；因此$G_i/G_{i+1}$并不简单。相反，如果 $\Sigma$ 是严格递减合成列，其中一个商 $G_i/G_{i+1}$ 不简单，则该商包含是除自身和 $\{e\}$ 之外的正规稳定子群，其 $G_i$ 中的逆像是正规稳定$G_i$ 的子群 $H$，不同于 $G_i$ 和 $G_{i+1}$ (定理 4)；只需在$G_i$和$G_{i+1}$之间插入$H$即可获得与$\Sigma$和更细区别于$\Sigma$的严格递减合成列。

#### 定理 6（乔丹-霍尔德）{#alg-i-s4-thm-6 .statement tag=059I}

*两个 Jordan-Hölder 级数或群与运算符是等效的。*

令$\Sigma_1, \Sigma_2$为群的两个Jordan-Hölder级数，运算符为$G$；通过应用定理 5 得到两个*等价* 合成列 $\Sigma'_1, \Sigma'_2$，分别比更细比$\Sigma_1$和$\Sigma_2$；由于后者是 Jordan-Hölder 级数，$\Sigma'_1$ 与 $\Sigma_1$ 相同，或者是通过重复某些项衍生而来； $\Sigma'_1$的商级数是从$\Sigma_1$的商中通过插入与群$\{e\}$同构的项的数而导出；由于$\Sigma_1$是严格递减，$\Sigma_1$的商的级数是通过抑制后者*所有*项同构于$\{e\}$而从$\Sigma'_1$的商导出的。对于 $\Sigma_2$ 和 $\Sigma'_2$ 也是如此。由于$\Sigma'_1$和$\Sigma'_2$的商级数仅在项的阶不同（最多同构），$\Sigma_1$和$\Sigma_2$也是如此； 定理得证。

#### 推论{#alg-i-s4-n7-cor-1 .statement tag=059J}

*设 $G$ 为群，其中存在 Jordan-Hölder 级数的算子。如果 $\Sigma$ 是 $G$ 中的任意严格递减合成列，则存在比 $\Sigma$ 的 Jordan-Hölder 级数更细。*

Let $\Sigma_0$ be a Jordan-Hölder series of $G$; by Theorem 5, there exist two equivalent composition series, $\Sigma'$ and $\Sigma'_0$ respectively finer than $\Sigma$ and $\Sigma_0$; the argument of Theorem 6 shows that, by suppressing from $\Sigma'$ the repetitions, a sequence $\Sigma''$ is obtained which is equivalent to $\Sigma_0$ and hence a Jordan-Hölder series, since all its quotients are simple (Proposition 9). 由于$\Sigma$是严格递减，$\Sigma''$比$\Sigma$是更细，从而是推论。

#### 注 {#alg-i-s4-n7-rem-1 .statement tag=059K}

群与运营商并不总是拥有 Jordan-Hölder 级数； 例由有理整数的加法群$\mathbf{Z}$给出：序列$(2^n \cdot \mathbf{Z})_{n \geq 0}$是$\mathbf{Z}$的（正常）子群的严格递减无限序列；对于所有$p$，这个序列形式的第一个$p$项与群$\{0\}$严格递减合成列；如果$\mathbf{Z}$存在乔丹-霍尔德级数，则根据定理6的推论，它至少有$p+1$项；荒谬，因为 $p$ 是任意的。

另一方面，在每个*有限*群中都存在一个Jordan-Hölder级数，且算子G：如果$G \ne \{e\}$，在与G不同的G的正常稳定子群中，令$H_1$为最大子群；类似地，定义$H_{n+1}$由归纳作为$H_n$正常子群的集合中的极大元素，与$H_n$不同，当$H_n \ne \{e\}$时； $H_n$的阶的序列是严格递减，因此存在$n$使得G的$H_n = \{e\}$和序列由……组成和$H_i$（$1 \leq i \leq n$）通过其形成乔丹-霍尔德级数。

#### 定义 11 {#alg-i-s4-def-11 .statement tag=059L}

设 G 为带有运算符的群； G 的长度是整数 $n$ 的上界，因此存在G $(G_i)_{0\leq i\leq n}$ 的严格递减合成列。

如果 G 承认 Jordan-Hölder 级数，则 G 的长度是该级数的连续商的数，如下从定理 6 的推论。如果 G 不承认 Jordan-Hölder 级数，则其长度是无限的；到命题 9，对于 G 的每严格递减级数，都存在严格的更细严格递减级数。 单位元素中的群由……组成是唯一具有长度零运算符的群。当且仅当它是长度 1 时，带有运算符的群才是简单的。

设 G 为带有运算符的群，H 为 G 的正常稳定子群，K 为商 G/H 和 $\pi:G\to K$ 典范同态。让

$$
\Sigma'=(H_i)_{0\leq i\leq n}
$$

是 H 的分解级数且

$$
\Sigma''=(K_j)_{0\leq j\leq p}
$$

是 K 的合成列。为 $0\leq i\leq p$ 写 $G_i=\pi^{-1}(K_i)$，为 $p\leq i\leq n+p$、合成列写$G_i=H_{i-p}$

$$
\Sigma=(G_i)_{0\leq i\leq n+p}
$$

得到G。 $\Sigma$的商序列是通过将$\Sigma''$的商序列与$\Sigma'$的商序列并列而获得。如果$\Sigma'$和$\Sigma''$是Jordan-Hölder级数，$\Sigma$是G的Jordan-Hölder级数，通过命题9。如果H或K承认任意长度的合成列，G也如此。我们已经证明：

#### 命题 10 {#alg-i-s4-prop-10 .statement tag=059M}

令 G 为带有算子的群，H 为 G 的正常稳定子群。G 的长度是 H 和 G/H 的长度的和。

#### 推论{#alg-i-s4-n7-cor-2 .statement tag=059N}

令G为带有运算符的群和G的$(G_i)_{0\leq i\leq n}$合成列。G的长度是$G_i/G_{i+1}$、$0\leq i\leq n-1$的长度的和。

如果 G 和 $G'$ 与算子同构群并且 G 承认 Jordan-Hölder 级数，那么 $G'$ 以及 G 和 $G'$ 的 Jordan-Hölder 级数是等价的。然而，非同构群可以有等价的Jordan-Hölder级数；对于 $\mathbf{Z}/4\mathbf{Z}$ 和 $(\mathbf{Z}/2\mathbf{Z})\times(\mathbf{Z}/2\mathbf{Z})$、cf. no. 10 也是如此。

### 8. 乘积和纤维乘积

设$(G_i)_{i \in I}$是带有运算符的群族。令$G$为$G_i$的乘积幺半群。考虑$G$上的$\Omega$的作用定义为

$$
((x_i)_{i \in I})^\alpha = (x_i^\alpha)_{i \in I} \quad (\alpha \in \Omega, x_i \in G_i).
$$

这样结构 $G$ 就是群与运算符。对于所有 $i \in I$，投影映射 $\mathrm{pr}_i : G \to G_i$ 是带有运算符的群的同态。

#### 定义 12 {#alg-i-s4-def-12 .statement tag=059O}

*群与运算符* $G = \prod_{i \in I} G_i$ *上面定义的是乘积群以及* $G_i$ 的运算符。 *映射* $\mathrm{pr}_i : G \to G_i$ *被称为* 投影同态。

带有运算符的群的乘积的特殊情况是集合 $E$ 的映射群 $G^E$ 由……组成转换为群，其中运算符 $G$、律定义如下：

$$
(fg)(x) = f(x)g(x) \quad (f, g \in G^E, x \in E)
$$
$$
f^\alpha(x) = f(x)^\alpha \quad (f \in G^E, \alpha \in \Omega, x \in E).
$$

设$(\phi_i : H \to G_i)_{i \in I}$是同态和群的运算符族。 $H$ 的映射 $h \mapsto (\phi_i(h))_{i \in I}$ 到 $\prod_{i \in I} G_i$ 是群的同态与运算符。这是所有$i$中唯一的同态$\Phi : H \to \prod_{i \in I} G_i$满足$\mathrm{pr}_i \circ \Phi = \phi_i$。这证明了“乘积群与运算符”的名称是合理的（*集合理论*，IV, § 2, no. 4）。

令 $(\phi_i : H_i \to G_i)_{i \in I}$ 成为群的同态与运算符的族。 $\prod_{i \in I} H_i$的映射$\prod_{i \in I} \phi_i : (h_i)_{i \in I} \mapsto (\phi_i(h_i))_{i \in I}$到$\prod_{i \in I} G_i$是群的同态与运算符。

#### 命题 11 {#alg-i-s4-prop-11 .statement tag=059P}

*设* $(\phi_i : H_i \to G_i)_{i \in I}$ *是同态的群与运算符的族，并设* $\Phi = \prod_{i \in I} \phi_i$。 *然后：*

(a) $\mathrm{Ker}(\Phi) = \prod_{i \in I} \mathrm{Ker}(\phi_i)$； *特别是，如果所有* $\phi_i$ *都是单射的，则$\Phi$ *是单射的*。

(b) $\mathrm{Im}(\Phi) = \prod_{i \in I} \mathrm{Im}(\phi_i)$； *特别是，如果所有* $\phi_i$ *都是满射，则$\Phi$ *也是满射*。

这是直接的。

特别地，令 $(G_i)_{i \in I}$ 为带有运算符的群族，并且对于所有$i$，令$H_i$为$G_i$的稳定（或正常稳定）子群。 乘积 $\prod_{i \in I} H_i$ 是$\prod_{i \in I} G_i$ 的子群和$\prod_{i \in I} G_i$ 的典范映射到$\prod_{i \in I} (G_i / H_i)$ 定义，当经过与同构的商
$$
\left( \prod_{i \in I} G_i \right) / \left( \prod_{i \in I} H_i \right)
$$
到$\prod_{i \in I} (G_i / H_i)$。对于例，令$J$为$I$的子集。 $(x_i)_{i \in I}$的$\prod_{i \in I} G_i$由……组成的子群$G_J$，使得$i \notin J$的$x_i = e_i$是正常稳定的子群。 映射 $\iota_J$ 与 $x = (x_j)_{j \in J}$ 元素 $y = (y_i)_{i \in I}$ 关联，使得 $i \notin J$ 的 $y_i = e_i$ 和 $i \in J$ 的 $y_i = x_i$，是 $\prod_{j \in J} G_j$ 的同构到$G_J$。 映射 $\mathrm{pr}_{I-J}$ 定义当经过到商群 $G / G_J$ 的商同构 $\theta_J$ 到 $\prod_{i \in I-J} G_i$ 时。 合成$\mathrm{pr}_J \circ \iota_J$是$\prod_{j \in J} G_j$中的恒等映射。由于 $\theta_J$，$G / G_J$ 通常与 $\prod_{i \in I-J} G_i$ 等同，并且由于 $\iota_J$，$\prod_{i \in J} G_i$ 与 $G_J$ 等同。

如果$J_1$和$J_2$是$I$的不相交的子集，则从定义可以得出，$G_{J_1}$的每个元素与$G_{J_2}$的每个元素进行通勤。

#### 定义 13 {#alg-i-s4-def-13 .statement tag=059Q}

*令 $G$ 为群，有操作员，$(H_i)_{i \in I}$ 为 $G$ 的正常稳定族子群。令$p_i : G \to G / H_i$为典范同态。如果同态 $g \mapsto (p_i(g))_{i \in I}$ 是 $G$ 的同构到 $\prod_{i \in I} G / H_i$，$G$ 被称为商群 $(G / H_i)$ 族的内部乘积（或乘积）。*

令$G$和$H$为带有运算符的群，并令$\phi$和$\psi$为$G$到$H$的两个同态。 $G$中元素$x$的集合使得$\phi(x) = \psi(x)$是$G$的稳定子群，称为$\phi$和$\psi$的*重合群*。特别地，使用运算符令$\phi_1 : G_1 \to H$和$\phi_2 : G_2 \to H$为群的同态； 同态 $\phi_1 \circ \mathrm{pr}_1$ 的群和 $G_1 \times G_2$ 的 $\phi_2 \circ \mathrm{pr}_2$ 到 $H$ 的重合被称为 $G_1$ 和 $G_2$ 相对于 $H$ 的 *纤维乘积* $\phi_1$ 和 $\phi_2$。当$\phi_1$和$\phi_2$没有歧义时，用$G_1 \times_H G_2$表示，$\mathrm{pr}_1$和$\mathrm{pr}_2$至$G_1 \times_H G_2$的限制、$p_1$和$p_2$也称为投影同态。然后$\phi_1 \circ p_1 = \phi_2 \circ p_2$。 $G_1 \times_H G_2$中的元素是有序对$(g_1, g_2) \in G_1 \times G_2$，使得$\phi_1(g_1) = \phi_2(g_2)$。如果$f_i$是群的同态，且带有运算符$K$到$G_i$（$i = 1, 2$）和$\phi_1 \circ f_1 = \phi_2 \circ f_2$，则存在且仅有一个$K$到$G_1 \times_H G_2$的同态和$f$，这样$f_i = p_i \circ f$ 对应 $i = 1, 2$。

### 9. 限制和

令$(G_i)_{i \in I}$为群的运算符族，对于$i \in I$，令$H_i$为$G_i$的稳定子群。 $(x_i)_{i \in I}$的$\prod_{i \in I} G_i$由……组成的子集使得$i \in I$的集合和$x_i \notin H_i$是有限的，如果$I$是有限的，则$\prod_{i \in I} G_i$的稳定子群等于$\prod_{i \in I} G_i$。相对于$H_i$*，它被称为$G_i$的*受限和。当对于除有限数之外的所有$i$，$H_i$ 是$G_i$ 的正常稳定子群时，受限制的和是乘积的正常稳定子群。当，对于所有$i$，子群$H_i$减少到$G_i$的单位元素时，$G_i$相对于$H_i$的直和被简单地称为$G_i$的*受限和*并且有时表示为 $\prod_{i \in I} G_i$。对于由 $\iota_{i_0}(x) = (x_i)_{i \in I}$ 定义的所有 $i_0 \in I$、映射 $\iota_{i_0}: G_{i_0} \to \prod_{i \in I} G_i$，其中 $x_{i_0} = x$ 和 $x_i = e_i$（如果 $i \neq i_0$）是群的单同态，运算符称为 *典范嵌入*。 $G_i$ 与稳定的子群 $\operatorname{Im}(\iota_i)$ 相同。 子群$G_i$都是正常的。对于$i \neq j$、元素、$G_i$、$G_j$通勤和$G_i \cap G_j = \{e\}$。 群$\prod_{i \in I} G_i$由集合$\bigcup_{i \in I} G_i$生成。

#### 命题 12 {#alg-i-s4-prop-12 .statement tag=059R}

*令$(\phi_i: G_i \to K)_{i \in I}$是群的同态族，其运算符使得对于所有$i \in I$和$j \in I$以及$i \neq j$、$x \in G_i$、$y \in G_j$、元素$\phi_i(x)$和$K$通勤$\phi_j(y)$；存在且仅有一个群的同态，将$\prod_{i \in I} G_i$的$\Phi$算子放入$K$，使得所有$i \in I$都有$\phi_i = \Phi \circ \iota_i$。对于 $\prod_{i \in I} G_i$ 中的每元素 $x = (x_i)_{i \in I}$，$\Phi(x) = \prod_{i \in I} \phi_i(x_i)$。*

如果$\Phi$和$\Phi$是解到问题，则它们在$\bigcup_{i \in I} G_i$上是重合，因此在$\prod_{i \in I} G_i$、$\Phi$的从而唯一性上。现在我们证明$\Phi$的存在性：对于$\prod_{i \in I} G_i$的每个元素$x = (x_i)_{i \in I}$，令$\Phi(x) = \prod_{i \in I} \phi_i(x_i)$（§ 1, no. 5）。显然 $\Phi \circ \iota_i = \phi_i$ 对于所有 $i$ 和 $\Phi$ 都具有同位交换； 公式 $\Phi(xy) = \Phi(x)\Phi(y)$ 由§ 1, no. 5、公式 (9) 推出。

#### 定义 14 {#alg-i-s4-def-14 .statement tag=059S}

*令 $G$ 为群，包括运算符和 $(H_i)_{i \in I}$ 子群 $G$ 的稳定族。如果$H_i$的每一个元素对于$j \neq i$来说可以与$H_j$的每一个元素进行置换，$G$被称为子群$(H_i)$族的内部受限和（或受限和）将$\prod_{i \in I} H_i$的唯一同态转化为$G$，其限制到每个$H_i$的典范嵌入为同构。*

当$I$有限时，我们还滥用语言说*内部直接乘积*（或*直接乘积*，或*乘积*）而不是内部受限和。 G 的每个稳定子群 H，如果存在 G 的稳定子群 H'，使得 G 是 H 和 H' 的直乘积，则称为 G 的 *直因子*。

#### 命题 13 {#alg-i-s4-prop-13 .statement tag=059T}

*令 G 为具有运算符的群和$(H_i)_{i \in I}$ G 的稳定子群族，使得$H_i$的每个元素对于$H_j$的每个元素都可以置换为$j \neq i$。为了使 G 成为子群 $(H_i)_{i \in I}$ 族的受限和，G 的每个元素 x 可以在形式 $\prod_{i \in I} y_i$ 中唯一表达是充分必要的，其中 $(y_i)_{i \in I}$ 是元素的有限支撑的族G 的 $y_i \in H_i$ 对于所有 i.*

显而易见。

#### 命题 14 {#alg-i-s4-prop-14 .statement tag=059U}

*设 G 为带有运算符的群和 $(H_i)_{i \in I}$ G 的稳定子群的有限族。为了使 G 成为子群 $(H_i)$ 族的受限制和，每个 $H_i$ 是正规的并且 G 是乘积是充分必要的的商群 $(G/H^i)$，其中 $H^i$ 是由 $H_j$ 为 $j \neq i$ 生成的子群。*

条件显然是必要的。相反，假设G是$K_i = G/H^i$的乘积，并让G等同于$K_i$的乘积。然后将$H_i$与$K_i$的子群进行识别，因此，对于$i \neq j$，$H_i$的每个元素可以与$H_j$的每个元素进行置换；另一方面，$H^i$与$j \neq i$的$K_j$的乘积相同，因此$H_i = K_i$对于所有$i$，G是$H_i$的直接乘积。

#### 命题 15 {#alg-i-s4-prop-15 .statement tag=059V}

*令 G 为带有运算符的群以及 G 的正常稳定子群的 $(H_i)_{1 \leq i \leq n}$ 序列，使得*
$$
(H_1 H_2 \ldots H_i) \cap H_{i+1} = \{e\} \quad \text{for } 1 \leq i \leq n-1,
$$
*集合$H_1 H_2 \ldots H_n$是G的正常稳定子群，$H_i$的限制和。*

到 $n$ 的归纳时，$n = 2$ 立即减少为证明命题。我们首先证明，如果 $x \in H_1$ 和 $y \in H_2$，则 x 和 y 是*可置换的*；对于$xyx^{-1}y^{-1} = (xyx^{-1})y^{-1} = x(yx^{-1}y^{-1})$，因此（因为$H_1$和$H_2$是正常的）$xyx^{-1}y^{-1} \in H_1 \cap H_2$，即$xyx^{-1}y^{-1} = e$，乘以假设。此外，$H_1 H_2$是G的子集，在G的同位性下是稳定的。由此可知（通过no. 3，命题1）$H_1 H_2$是G的稳定子群，并且立即验证该子群是正常的。最后假设$xy = x'y'$，还有$x \in H_1, x' \in H_1, y \in H_2, y' \in H_2$；然后${x'}^{-1}x = y'y^{-1}$，因此${x'}^{-1} \in H_1 \cap H_2 = \{e\}$，$x' = x$，类似地$y' = y$；因此，$H_1 H_2$是$H_1$和$H_2$的直接乘积。

当群考虑可交换时，使用项*直和*而不是直接乘积。

### 10.单一群

设 $a \in \mathbf{Z}$；因为$a\mathbf{Z}$是$\mathbf{Z}$的子群，关系在$\mathbf{Z}$的元素$x, y$之间，其中指出“存在$z \in \mathbf{Z}$使得$x - y = az$”是等价关系，我们一劳永逸地同意这样写如$x \equiv y \pmod{a}$或$x \equiv y(a)$，称为*同余模*$a$。 替换$a$乘以$-a$，得到等价的关系，因此可以假设$a \geqslant 0$；对于$a = 0$，$x \equiv y(0)$意味着$x = y$，因此只有在$a \neq 0$时才能获得与等式不同的关系：因此，我们将在下文中假设$a > 0$除非另有说明。

对于$a > 0$，$\mathbf{Z}$与同余$x \equiv y(a)$的商，即群$\mathbf{Z}/a\mathbf{Z}$，称为有理整数模*$a$的*群。

#### 命题 16 {#alg-i-s4-prop-16 .statement tag=059W}

*令$a$为整数$> 0$。 整数 $r$ $0 \leqslant r < a$ 形式系统等价关系 $x \equiv y \pmod{a}$ 代表元$\mathbf{Z}$。*

如果$x$是整数$\geqslant 0$，则存在(*集合理论*，III, § 5, no. 6)整数$q$和$r$，使得$x = aq + r$和$0 \leqslant r < a$和$x \equiv r \pmod{a}$。 If $x$ is 整数 $\leqslant 0$, 整数 $-x$ is $\geqslant 0$ and by the above there exists 整数 $r$ such that $0 \leqslant r < a$ and $-x \equiv r \pmod{a}$. Writing $r' = 0$ if $r = 0$ and $r' = a - r$ if $r > 0$, then

$$
x \equiv -r \equiv r' \pmod{a}
$$

and $0 \leqslant r' < a$.我们现在证明，如果 $0 \leqslant r < r' < a$，则$r \not\equiv r' \pmod{a}$。 Now $r' - r < na$ for $n \geqslant 1$ and $r' - r > na$ for $n \leqslant 0$, 从而 $r' - r \notin a\mathbf{Z}$.

#### Corollary {#alg-i-s4-n10-cor-1 .statement tag=059X}

*令$a$为整数$> 0$。 群 $\mathbf{Z}/a\mathbf{Z}$ of rational 整数 modulo $a$ is 群 of 阶 $a$.*

#### 命题 17 {#alg-i-s4-prop-17 .statement tag=059Y}

*令$\mathrm{H}$为$\mathbf{Z}$中的子群。 There exists one and only one 整数 $a \geqslant 0$ such that $\mathrm{H} = a\mathbf{Z}$.*

如果$\mathrm{H} = \{0\}$，则$\mathrm{H} = 0\mathbf{Z}$。假设$\mathrm{H} \neq \{0\}$。 子群$\mathrm{H}$有元素$x \neq 0$。然后$x > 0$或$-x > 0$，因此$\mathrm{H}$有元素$> 0$。令$\mathrm{H}$中的$a$为最小的元素$> 0$。 $a$生成的子群$a\mathbf{Z}$包含在$\mathrm{H}$中；我们证明$\mathrm{H} \subset a\mathbf{Z}$。让$y \in \mathrm{H}$。到命题 16，存在整数$r$，使得$y \equiv r \pmod{a}$和$0 \leqslant r < a$。 *更不必说* $y \equiv r \pmod{\mathrm{H}}$，从而$r \in \mathrm{H}$。但这只有在 $r = 0$ 且因此 $y \in a\mathbf{Z}$ 时才有可能。 整数$a$是唯一的：如果$\mathrm{H} = \{0\}$，则必然$a = 0$，如果$\mathrm{H} \neq \{0\}$，整数$a$是$\mathbf{Z}/\mathrm{H}$的阶。

#### 定义 15 {#alg-i-s4-def-15 .statement tag=059Z}

*如果群承认单个元素的生成元由……组成中的系统，则称为单生的。有限单生群称为循环。*

每个单生群都是可交换的（no. 3，推论 2 到命题 2）。单源群的每个商群都是单源的（no. 3，推论3到命题2）。

加法群 $\mathbf{Z}$ 是单生的：它是由 $\{1\}$ 生成的。对于每个正整数 $a$，群 $\mathbf{Z}/a\mathbf{Z}$ 都是单生的，因为它是 $\mathbf{Z}$ 的商。

#### 命题 18 {#alg-i-s4-prop-18 .statement tag=05A0}

* 阶 a 的有限单生群与 $\mathbf{Z}/a\mathbf{Z}$ 同构的。无限单生群同构于 $\mathbf{Z}$。*

设G是单生群（乘法写）和G的x生成元。恒等式$x^m x^n = x^{m+n}$（§ 1, no. 3，公式（1））表明映射$n \mapsto x^n$是$\mathbf{Z}$的同态进入G。 像是 G 包含于 x 的子群，因此它是 G。通过 no. 5，定理 3，群 G 同构于 $\mathbf{Z}$ 除以子群的商，这必然是形式$a\mathbf{Z}$（命题17）。如果 $a > 0$，群 G 是阶 a 的有限，并且如果 $a = 0$，群 G 与 $\mathbf{Z}$ 同构的。

#### 命题 19 {#alg-i-s4-prop-19 .statement tag=05A1}

*设a为整数 > 0。设H为$\mathbf{Z}/a\mathbf{Z}$中的子群，b为H中的阶，c为$\mathbf{Z}/a\mathbf{Z}$中的指标。那么$a = bc$，$H = c\mathbf{Z}/a\mathbf{Z}$和H同构于$\mathbf{Z}/b\mathbf{Z}$。

相反，令 b 和 c 为两个整数 > 0，使得 $a = bc$。那么$a\mathbf{Z} \subset c\mathbf{Z}$和$c\mathbf{Z}/a\mathbf{Z}$就是$\mathbf{Z}/a\mathbf{Z}$、阶b和指标c的子群。

$a = bc$乘no. 4，推论命题4。到no. 7、定理4，H为形式$H'/a\mathbf{Z}$，其中$H'$为$\mathbf{Z}$的子群，$\mathbf{Z}/H'$为与 $(\mathbf{Z}/a\mathbf{Z})/H$ 同构的，因此与阶同构 c.根据命题 17 和命题 16 的推论，$H' = c\mathbf{Z}$ 因此 H 是单生的。最后，H 同构于 $\mathbf{Z}/b\mathbf{Z}$ 命题 18。相反，如果 $a = bc$，则 $a\mathbf{Z} \subset c\mathbf{Z}$ 对于 $a \in c\mathbf{Z}$： 商群 $(\mathbf{Z}/a\mathbf{Z})/(c\mathbf{Z}/a\mathbf{Z})$ 同构于 $\mathbf{Z}/c\mathbf{Z}$ (no. 7, 定理) 4) 以及阶 c (no. 4，命题 4 的推论) 和指标 b (no. 4，命题 4 的推论)。

#### 推论 {#alg-i-s4-n10-cor-2 .statement tag=05A2}

*单源群的每个子群都是单源的。*

设a和b为两个整数$\neq 0$。 关系 $b \in a\mathbf{Z}$ 也可写作：*b 是 a* 的倍数，也可写成 *除 b* 或 *是 b* 的除子。

#### 定义 16 {#alg-i-s4-def-16 .statement tag=05A3}

*整数 $p > 0$ 称为素数，如果 $p \neq 1$ 并且除了 p 之外不承认除子 > 1。*

#### 命题 20 {#alg-i-s4-prop-20 .statement tag=05A4}

*整数$p > 0$是质数当且仅当群$\mathbf{Z}/p\mathbf{Z}$是一个简单的群。*

这是从命题 19 开始的。

#### 推论{#alg-i-s4-n10-cor-3 .statement tag=05A5}

*每个可交换简单群都是素数阶的循环。*

令G为群。然后$G \neq \{e\}$；设 $a \neq e$ 为 G 的元素。 由 a 生成的子群是正规的，因为 G 是可交换的，它不会减少到 $\{e\}$，因此等于 G。因此 G 是单生的，因此与形式 $\mathbf{Z}/p\mathbf{Z}$ 的群同构$p > 0$，因为$\mathbf{Z}$不简单，$p$必然是素数。

#### 注 {#alg-i-s4-n10-rem-1 .statement tag=05A6}

素数阶的有限群G必然是循环的。 G 除了 G 和 $\{e\}$ 之外不承认任何子群，因此它是由每个元素 $\neq e$ 生成的。

#### 引理 2 {#alg-i-s4-lem-2 .statement tag=05A7}

设$a$为整数$> 0$。通过与群$\mathbf{Z}/a\mathbf{Z}$序列$(s_i)_{1 \leq i \leq n}$的每个合成列$(\mathbf{H}_i)_{0 \leq i \leq n}$关联，其中$s_i$是$\mathbf{H}_{i-1}/\mathbf{H}_i$的阶，在以下之间获得一对一的对应 $\mathbf{Z}/a\mathbf{Z}$的合成列和整数$> 0$的有限序列$(s_i)$使得$a = s_1 \ldots s_n$。当且仅当 $s_i$ 是质数时，合成列 $(\mathbf{H}_i)_{0 \leq i \leq n}$ 是 Jordan-Hölder 级数。

如果$(\mathbf{H}_i)_{0 \leq i \leq n}$是$\mathbf{Z}/a\mathbf{Z}$中的合成列，则从no. 4、命题4到$n$上的归纳，得出$a = \prod_{i=1}^n (\mathbf{H}_{i-1} : \mathbf{H}_i)$。

相反，令$(s_i)_{1 \leq i \leq n}$为整数$> 0$的序列，使得$a = s_1 \ldots s_n$。如果$(\mathbf{H}_i)_{0 \leq i \leq n}$是$\mathbf{Z}/a\mathbf{Z}$的合成列，使得$(\mathbf{H}_{i-1} : \mathbf{H}_i) = s_i$对应于$1 \leq i \leq n$，那么必然是$((\mathbf{Z}/a\mathbf{Z}) : \mathbf{H}_i) = \prod_{1 \leq j \leq i} s_j$，正如归纳在$i$、从而$\mathbf{H}_i = \left( \prod_{j=1}^i s_j \right) \mathbf{Z}/a\mathbf{Z}$上看到的那样(命题 19)，它显示了所讨论的映射的单射性。我们现在展示它的满射性。将$0 \leq i \leq n$写入$\mathbf{H}_i = \left( \prod_{j=1}^i s_j \right) \mathbf{Z}/a\mathbf{Z}$，可得到$\mathbf{Z}/a\mathbf{Z}$的合成列，使得$(\mathbf{H}_{i-1} : \mathbf{H}_i) = s_i$（命题19）。第二个断言源自命题20和no. 7、命题9。

让$\mathfrak{P}$表示素数数的集合。

#### 定理 7（分解进入素数因子）{#alg-i-s4-thm-7 .statement tag=05A8}

*令$a$严格为正整数。存在且仅有一个整数 $> 0$ 的族 $(v_p(a))_{p \in \mathfrak{P}}$，使得 $p \in \mathfrak{P}$ 与 $v_p(a) \neq 0$ 的集合是有限的并且*

$$
a = \prod_{p \in \mathfrak{P}} p^{v_p(a)}.
$$

由于群 $\mathbf{Z}/a\mathbf{Z}$ 是有限的，因此它承认 Jordan-Hölder 级数。 引理 2 那么意味着$a$ 是素数整数的乘积，从而族$(v_p(a))$ 的存在；此外，对于定理 7 的每个家庭$(v_p(a))_{p \in \mathfrak{P}}$ 满足条件，对于所有$p \in \mathfrak{P}$，整数 $v_p(a)$ 等于 Jordan-Hölder 级数的因子数 $\mathbf{Z}/a\mathbf{Z}$ 同构于 $\mathbf{Z}/p\mathbf{Z}$ (引理 2)。因此，家族$(v_p(a))$的唯一性源自Jordan-Hölder定理（no. 7，定理6）。

#### 推论{#alg-i-s4-n10-cor-4 .statement tag=05A9}

*令$a$和$b$为两个整数$> 0$。然后$v_p(ab) = v_p(a) + v_p(b)$。对于 $a$ 到除 $b$，对于每个素数数 $p$，$v_p(a) \leq v_p(b)$ 是充分必要的。*

在任意群$G$中，如果元素$x \in G$生成的（单生）子群是有限的阶$d$，则$x$称为*阶*的元素 $d$；因此，数$d$是最小的整数$> 0$使得$x^d = e$；如果$x$生成的子群是无限的，则$x$被称为*无限阶*。这些定义与命题 4 (no. 4) 一起，特别意味着在有限群 G 中，每个元素 G 的阶是 G 的阶的除子。

#### 命题 21 {#alg-i-s4-prop-21 .statement tag=05AA}

在阶 n 的有限群 G 中，$x^n = e$ 对于所有 $x \in G$。

如果$p$是$x$的阶，则$n = pq$，$q$整数，因此$x^n = (x^p)^q = e$。

### 习题{#alg-i-s4-exercises}

§ 4](exercises/s4/)参见[习题。
