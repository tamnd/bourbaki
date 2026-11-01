---
book: top
book_title: General Topology
chapter: V
chapter_title: One-parameter groups
section: 3
section_title: Topological characterization of the groups R and T
lang: zh
source: top-v-x
pdf_pages: 0023-0025, 0031-0034
extraction: ocr
statements: 5
exercises: 8
content_sha256: 25d200f869648d78d992f7261dbc1f0933bd8bfa0b04f4830a6556325ca90fec
translated_from: content/en/top/V/03_s3_topological_characterization_of_the.md
translation_method: google
source_content_sha256: b250fd39401223e4fa03cf5ea015761d2798fe7a40dda8dc19bea27b8a96e356
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: c73eb6576552fe447d8c74921e0079b24c50eee8ac940c44fd57f6a5b126ba51
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 3. 群 $\mathbf{R}$ 和 $\mathbf{T}$ 的拓扑刻画

#### 定理 1 {#top-v-s3-thm-1 .statement tag=0BVN}

*拓扑群* $G$ *其中存在单位元素的邻域同胚于* $\mathbf{R}$ *局部同构于* $\mathbf{R}$。

这个定理的意义在于，它允许我们从群$G$的纯拓扑性质推导出$G$的*群结构*的性质。

我们在这里关注群$\mathbf{R}$所特有的​​现象，当$n > 1$（cf.章VIII, § 1, no. 4）时，群$\mathbf{R}^n$没有类似物。 群与$\mathbf{R}$ 局部同构，有时称为*单参数群*。

为了证明定理 1，我们需要将约化证明为§ 2的命题 2。 到假设，单位元素$e$的开邻域$U$与$G$的开区间有同态$\varphi$到$\mathbf{R}$的开区间。 通过映射$\varphi$的逆，我们可以得到迁移到$U$区间$\varphi(U)$的线性阶结构； $U$ 的拓扑（由 $G$ 诱导）则具有 $U$ 的所有开区间的基由……组成 (章)

IV、no. 4、命题 5)。我们可以找到 e 的对称邻域 V，使得 V.V ⊂ U 且V 是开区间；因为存在开区间 V' 包含 e 使得 V'.V' ⊂ U ∩ U^{-1}, V'.V'^{-1} ⊂ U 和 V'^{-1}.V' ⊂ U;取 V = V' ∪ V'^{-1}，V 是开对称的，满足 V.V ⟧ ⊂ U 并且连通，因此是一个区间 (章 IV, § 2, no. 5， 定理 4)

我们证明，如果 x, y, z 属于到 V，关系 x < y 意味着 xz < yz 且 zx < zy。事实上，函数 f_1(z) = Φ(yz) − Φ(xz) 和 f_2(z) = Φ(zy) − Φ(zx) 在 V 上连续；对于 z = e，它们 > 0 并且不会在 V 中消失 [例如，如果我们有 φ(yz) = φ(xz)，我们应该有 yz = xz，因此 y = x]。由于 f_1(V) 和 f_2(V) 相连 (章 I, § 11, no. 2, 命题 4)，因此是 R 中的区间 (章 IV, § 2, no. 5, 定理 4)，并且由于这些区间每个包含数 > 0 并且不包含 0，它们包含在 R^*_+ 中：也就是说，对于所有 z ∈ V，我们有 f_1(z) > 0 和 f_2(z) > 0。

如果 x 和 y 是 V 的两个元素，使得 x ≥ e 且 y ≥ e，则特别有 xy ≥ e。设 E 表示 U 的元素的（线性有序）集合，且≥ e，令 I 表示 V 的元素的集合，且≥ e；则满足§ 2的公理(GR_I)、(GR_{II})、(GR_{IIIa})和(GR_{IVa})(取ω为元素e，合成的律为群G)。从前面的内容可以清楚地看出 (GR_I)、(GR_{II}) 和 (GR_{IVa})。对于 (GR_{IIIa})，注足够了，如果 e < x < y (x ε V, y ε V)，我们有 x^{-1} ε V，因而 x^{-1} < e < x^{-1}y 且 x^{-1}y < y；因而 z = x^{-1}y 属于到 I 并且我们有 xz = y。因而，通过 § 2 的命题 2，存在 I 的严格递增的映射 f 到 R 的区间上，左端点为 0，使得只要 x、y 和 xy 属于 ，f(e) = 0 且 f(xy) = f(x) + f(y) I（只要 x 和 y 属于到 W ∩ I，W 是 e 的邻域，使得 W.W ⊂ V，就会出现这种情况）。

对于每一个不属于到 I 的元素 x ∈ V，我们有 x < e，因而 x^{-1} > e；因而，我们可以将V的扩展 f 到严格递增的映射 $\overline{f}$放到R的区间上，方法是将$\overline{f}(x) = -f(x^{-1})$放入V中所有x < e。 $\overline{f}(V)$所包含的开区间$\overline{f}$下的逆像是V的开区间，因而$\overline{f}$在V上连续；相反，V开区间的$\overline{f}$下的像是$\overline{f}(V)$的开区间，因而$\overline{f}$是群R中V到0的邻域的同胚。另一方面，它很容易被检查（如命题 6 of § 1, no. 4，通过考虑各种可能的情况），每当 x、y 和 xy 都在属于到 V 时，我们就有$\overline{f}(xy) = \overline{f}(x) + \overline{f}(y)$；因此我们结论认为$\overline{f}$，限制于G中e的合适邻域，是G与R的局部同构（章III, § 1, no. 3，命题3）。

Q.E.D.

#### 定理 2 {#top-v-s3-thm-2 .statement tag=0BVO}

*连接群* $G$ *其中存在单位元素的邻域同构于* $\mathbf{R}$的开区间 *同构于* $\mathbf{R}$ *或* $\mathbf{T}$。

这是前面的定理的直接的推论，以及§ 1, no. 4的命题7。

#### 注 1 {#top-v-s3-rem-1 .statement tag=0BVP}

要判断满足定理 2 的条件的群$G$是否同构于$\mathbf{T}$或$\mathbf{R}$，只需看$G$是否是紧的即可。

#### 注 2 {#top-v-s3-rem-2 .statement tag=0BVQ}

定理 2 特别表明，每个与群$\mathbf{R}$*同构的*的拓扑群*必然与$\mathbf{R}$同构的*。

#### 注 3 {#top-v-s3-rem-3 .statement tag=0BVR}

前面的群$\mathbf{R}$和$\mathbf{T}$的拓扑刻画涉及拓扑空间$\mathbf{R}$作为辅助集合。可以通过不涉及任何辅助集合的公理来表征$\mathbf{R}$和$\mathbf{T}$的拓扑群结构（参见习题4和5）。

### 习题{#top-v-s3-exercises}

§ 3](exercises/s3/)参见[习题。
