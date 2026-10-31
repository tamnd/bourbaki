---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 8
section_title: Restriction of the field ofscalars in vector spaces
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 317-325, 409-410
pdf_pages: 0341-0349, 0433-0434
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF K'-STRUCTURES
      page: 317
      pdf_page: 341
    - "no": 2
      title: Rationality for a subspace
      page: 318
      pdf_page: 342
    - "no": 3
      title: RATIONALITY FOR A LINEAR MAPPING
      page: 319
      pdf_page: 343
    - "no": 4
      title: RATIONAL LINEAR FORMS
      page: 320
      pdf_page: 344
    - "no": 5
      title: APPLICATION TO LINEAR SYSTEMS
      page: 321
      pdf_page: 345
    - "no": 6
      title: SMALLEST FIELD OF RATIONALITY
      page: 322
      pdf_page: 346
    - "no": 7
      title: CRITERIA FOR RATIONALITY
      page: 323
      pdf_page: 347
statements: 17
exercises: 5
content_sha256: 34c52afb0382f7f84bc0ecaa027d9a1dec6c2c897e8a5a761a8e28b906235523
translated_from: content/en/alg/II/08_s8_restriction_of_the_field_ofscalars_in.md
translation_method: google
source_content_sha256: 2ed7e12b55c05b782b900415fee46ae7d943593ea0d536d23f816f7a0166f2be
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: 79b57c2706451335f7a033ec69d26a6f2c2d3039850fb26bb0d73c0e50706880
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 8。 向量空间中标量的域的限制

在本段中，K 表示 K 的域和 K' 子域。在集合 V 上，K 定义上的右（左）向量空间结构，通过标量的限制，右（左）向量空间结构 K'。

### 1. K'-结构的定义

#### 命题 1 {#alg-ii-s8-prop-1 .statement tag=05V0}

令 V 为 K 上的右向量空间，V 的 V' 子集为 K' 上的向量子空间。以下条件是等效的：

(a) 将 $V'_{(K)} = V' \otimes_{K'} K$ 的 K-线性映射 $\lambda$ 代入 V，使得 $\lambda(x' \otimes \xi) = x'\xi$ 对于所有 $x' \in V', \xi \in K$ 是双射的。

(b) V' 到向量 K 空间 W 的每个 K'-线性映射 $f'$ 都可以唯一地扩展到 V 到 W 的 K-线性映射 f。

(c) V' 在 K' 上的每个基都是 V 在 K 上的基。

(d) 存在 V' 在 K' 上的基，这也是 V 在 K 上的基。

(e) 向量 K 空间 V 由 V' 生成，且在 K' 上自由的 V' 的每个子集在 K 上都是自由的。

我们知道（§ 5, no. 1）$V'_{(K)}$有一个右向量K空间结构，其下有$(x' \otimes \xi)\eta = x' \otimes (\xi\eta)$（K中的$\xi, \eta$，$x' \in V'$），并且对于V'的每个K'线性映射$f'$到向量K空间W，存在一个且仅有一个将$V'_{(K)}$的K-线性映射$\bar{f}'$代入W，使得$\bar{f}'(x' \otimes 1) = f'(x')$对应$x' \in V'$。如果 j 是 V' 到 V 的典范嵌入，则 $\lambda$ 只是相应的 K-线性映射 $\bar{j}$。如果 $\lambda$ 是双射的，则对于每个 K'-线性映射 $f': V' \to W, \bar{f}' \circ \lambda^{-1}$ 是 V 到 W 的唯一的K-线性映射延伸 $f'$；在其他字中，(a) 意味着(b)。相反，如果(b)成立，则特别存在V的K-线性映射$\mu$进入$V'_{(K)}$，使得$\mu(x') = x' \otimes 1$对于所有$x' \in V'$； $\mu \circ \lambda = 1_{V'_{(K)}}$是直接的；另一方面，$\lambda(\mu(x')) = x'$对于所有$x' \in V'$，并且，通过假设$j: V' \to V$可以唯一地扩展到V的自同态，必然有$\lambda \circ \mu = 1_V$，从而完成证明，即(a)和(b)是等价的。

对于 K' 上 V' 的每个基 B'，$V'_{(K)}$ 的元素 $v' \otimes 1$ 的集合 B（其中 $v'$ 穿过 B'），是 K 上 $V'_{(K)}$ 的基（§ 5, no. 1，命题 4），并且$\lambda(B) = B'$。为了使$\lambda$是双射的，$V'_{(K)}$的每个基的$\lambda$下的像必须是K上V的基，并且对于$V'_{(K)}$的单个基来说就足够了（§ 1, no. 11，推论2到命题17)。这就证明了(a)、(c)和(d)的等价。

由于在 K' 上自由的 V' 的每个子集都包含在 K' 上的 V' 的基 (§ 7, no. 1, 定理 2) 中，(c) 意味着 (e)。最后，假设(e)成立；如果 B' 是 V' 在 K' 上的基，则它是 V 在 K 上的自由子集；另一方面，B' 生成 V' 超过 K'，因此生成 V 超过 K 假设；因此B'是V除以K的基，这证明(e)蕴涵(c)。

#### 定义 1 {#alg-ii-s8-def-1 .statement tag=05V1}

*设 V 为域 K 上的右向量空间和 K 的 K' 子域。V 满足的每个向量子 K' 空间 V' 相当于命题 1 的条件称为 V 上的 K' 结构。*

#### 例 {#alg-ii-s8-n1-exa-1 .statement tag=05V2}

设 B 为 K 上 V 的基。对于 K 的*每个* 子域 K'，由 B 生成的 V 的向量子 K' 空间承认 B 为 K' 上的基，因此是 V 上的 K' 结构。 *对于例，如果 K 是可交换的并且 V 被视为多项式 K-代数 K[X_1, ..., X_n]，那么，对于 K 的每个子域 K'，K'[X_1, ..., X_n] 是 V 上的 K'-结构。*

### 2. 子空间的合理性

#### 定义 2 {#alg-ii-s8-def-2 .statement tag=05V3}

*设 V 大于 K 右向量空间，具有 K'-结构 V'。如果 V 的属于对 V' 来说，则 V 的向量对于 K' 来说是有理数。如果 V 的向量子 K 空间 W 是由向量 K' 上有理数生成（在 K 上），则称其在 K' 上有理数。_

令 (v'_i)_{i \in I} 为 V' 在 K' 上的基，因此也是 V 在 K 上的基 (no. 1, 命题 1)。为了使 V 的向量 x = $\sum_i v'_i \xi_i$ 在 K' 上有理数，$\xi_i \in K'$ 对于所有 $i \in I$ 是充分必要的。

如果 W 是 V 的向量子 K 空间，在 K' 上有理数，则从定义 2 可以得出 $W' = W \cap V'$ 是 W 的向量子 K' 空间，其中 *生成* W 在 K 上；另一方面，W' 中在 K' 上自由的每个子集在 K' 上也是自由的，因为它包含在 V' 中（no. 1，命题 1）。由此可见 (no. 1, 命题 1) W' 是 W 上的 *K'-结构*，据说是由 V 上的 K'-结构 V'“诱导”的。

对于 V' 的每个向量子 K' 空间 W'，我们将用 W'.K 表示 W' 的元素线性组合的 V 由……组成向量子 K 空间，系数在 K 中。

#### 命题 2 {#alg-ii-s8-prop-2 .statement tag=05V4}

*令 V 为 K 上的右向量空间，V' 为 V 上的 K' 结构。 映射 W' \mapsto W'.K 为 V' 的向量子 K' 空间的集合的双射到 V 的向量子 K 空间的集合，其在 K' 上有理数且逆双射是 W \mapsto W \cap V'._

显然，双射$\lambda^{-1}: V \to V' \otimes_{\mathbf{K'}} \mathbf{K}$，双射$\lambda$的逆定义在no. 1，命题1，映射每个向量子K'空间W'的V'到其像在典范嵌入下$x' \mapsto x' \otimes 1$ 和 W'.K 到 W' $\otimes_{\mathbf{K'}} \mathbf{K}$；因此，命题 2 中的断言是定义 2 中的推论以及§ 7, no. 9、命题 19。

#### 推论 1 {#alg-ii-s8-prop-2-cor-1 .statement tag=05V5}

*V 的向量子 K 空间的每个和和每个交在 K' 上有理数都是有理数子空间在 K'* 上。

断言关于和是显而易见的。另一方面，如果$(W'_i)_{i \in I}$是$V'$的向量子$\mathbf{K}'$空间族，则$\left( \bigcap_{i \in I} W'_i \right) \otimes_{\mathbf{K}'} \mathbf{K} = \bigcap_{i \in I} (W_i \otimes_{\mathbf{K}'} \mathbf{K})$（§ 7, no. 7，命题14的推论），这证明了推论。

$V$ 的基 $B$ 在 $\mathbf{K}$ 上被称为*在 $\mathbf{K}'$* 上有理数*，如果它由向量组成，而向量在 $\mathbf{K}'$ 上是有理数。

#### 推论 2 {#alg-ii-s8-prop-2-cor-2 .statement tag=05V6}

*$\mathbf{K}$上的$V$的每个基在$\mathbf{K}'$上是有理数，是$V'$的基在$\mathbf{K}'$上。*

如果$W'$是由$B$生成的$V'$的向量子$\mathbf{K}'$空间，则$W'.\mathbf{K} = V = V'.\mathbf{K}$、从而$V' = W'$凭借命题2。

### 3. 线性映射的合理性

#### 定义 3 {#alg-ii-s8-def-3 .statement tag=05V7}

*令$V_1, V_2$分别为$\mathbf{K}$和$\mathbf{K}'$结构$V'_1, V'_2$的两个右向量空间。如果 $f(V'_1) \subset V'_2$，则 $\mathbf{K}$ 线性映射 $f : V_1 \to V_2$ 被认为在 $\mathbf{K}'$ 上是有理数。*

如果$V_3$是$\mathbf{K}$的第三个右向量空间，具有$\mathbf{K}'$结构$V'_3$和$\mathbf{K}$线性映射，$g : V_2 \to V_3$在$\mathbf{K}'$上是有理数，显然$g \circ f : V_1 \to V_3$在$\mathbf{K}'$上是有理数。

#### 命题 3 {#alg-ii-s8-prop-3 .statement tag=05V8}

*令$V_1, V_2$分别为$V_1, V_2$上$\mathbf{K}$和$V'_1, V'_2$$\mathbf{K}'$结构的两个右向量空间。 $V_1$（或$V_2$）在规范上与$V'_1 \otimes_{\mathbf{K}'} \mathbf{K}$（或$V'_2 \otimes_{\mathbf{K}'} \mathbf{K}$）（no. 1、命题 1）相同。

(i) *映射$f' \mapsto f' \otimes 1_{\mathbf{K}} = f'_{(\mathbf{K})}$是$\mathrm{Hom}_{\mathbf{K}'}(V'_1, V'_2)$的双射到$\mathbf{K}$的集合-$V_1$到$V_2$的线性映射，在$\mathbf{K}'$上是有理数； 逆双射与$\mathbf{K}'$上的每个$\mathbf{K}$线性映射$f : V_1 \to V_2$有理关联，$\mathbf{K}'$线性映射$f' : V'_1 \to V'_2$具有与$f$到$V'_1$的限制相同的图。

(ii) *对于$\mathbf{K}$-线性映射$f : V_1 \to V_2$有理$\mathbf{K}'$，

$$
f(V'_1) = f(V_1) \cap V'_2 \quad \text{and} \quad f^{-1}(V'_2) = V'_1 + \mathrm{Ker}(f).
$$

(i) 通过上述证明，显然，如果$f' : V'_1 \to V'_2$是$\mathbf{K}'$线性映射，则$f'_{(\mathbf{K})} = f' \otimes 1_{\mathbf{K}}$在$\mathbf{K}'$上是有理数，$f'$是映射，与$f'_{(\mathbf{K})}$到$V'_1$的限制具有相同的图。相反，如果$f : V_1 \to V_2$是$\mathbf{K}'$和$f' : V'_1 \to V'_2$上的$\mathbf{K}$线性映射有理数，则与$f$到$V'_1$、$f$和$f'_{(\mathbf{K})}$重合的限制具有相同的图$V'_1$，即$V_1$除$\mathbf{K}$的生成的系统，因此$f = f'_{(\mathbf{K})}$。

(ii) 如果$f = f' \otimes 1_{\mathbf{K}}$，则$f(V_1) = f(V'_1 \otimes_{\mathbf{K}'} \mathbf{K}) = f'(V'_1) \otimes_{\mathbf{K}'} \mathbf{K}$，并且如$f'(V'_1) \subset V'_2, f(V'_1) = f'(V'_1) \cap V'_2$ (§ 7, no. 9，命题 19)；紧接着是公式$f^{-1}(V'_2) = V'_1 + \mathrm{Ker}(f)$。

#### 推论 1 {#alg-ii-s8-prop-3-cor-1 .statement tag=05V9}

命题3、$\operatorname{Im}(f) = (\operatorname{Im}(f'))_{(\mathbf{K})}$中的记号，
$$
\operatorname{Ker}(f') = (\operatorname{Ker}(f'))_{(\mathbf{K})}, \quad \operatorname{Coker}(f) = (\operatorname{Coker}(f'))_{(\mathbf{K})}.
$$
特别是，对于$f$是单射的（或满射，零），$f'$是单射的是必要且充分的。如果 $f$ 是双射，则其逆映射在 $\mathbf{K}'$ 上是有理数。

这是 § 7, no. 9 的特例，命题 18 的推论。

#### 推论 2 {#alg-ii-s8-prop-3-cor-2 .statement tag=05VA}

令$f : V_1 \to V_2$为$\mathbf{K}'$上的$\mathbf{K}$线性映射有理数。 For every vector sub-$\mathbf{K}$-space $W_1$ of $V_1$ (resp. $W_2$ of $V_2$) rational over $\mathbf{K}'$, $f(W_1)$ (resp. $f^{-1}(W_2)$) is a vector sub-$\mathbf{K}$-space of $V_2$ (resp. $V_1$) rational over $\mathbf{K}'$.

在命题 3 的记号中，对于$V'_1$、$f'_{(\mathbf{K})}(W'_1 \otimes_{\mathbf{K}'} \mathbf{K}) = f'(W'_1) \otimes_{\mathbf{K}'} \mathbf{K}$的每个向量子$\mathbf{K}'$空间$W'_1$； 从而断言与 $W_1$ 相关（no. 2、命题 2）。另一方面，令$W'_2$为$V'_2$的向量子$\mathbf{K}'$空间，并令$g'$为规范$\mathbf{K}'$线性映射$V'_2 \to V'_2/W'_2$；然后$f'(W'_2) = \operatorname{Ker}(g' \circ f')$；因此，根据推论 1，
$$
{f'_{(\mathbf{K})}}^{-1}(W'_2 \otimes_{\mathbf{K}'} \mathbf{K}) = {f'}^{-1}(W'_2) \otimes_{\mathbf{K}'} \mathbf{K},
$$
从而断言与 $W_2$ 相关。

令$V_1, V_2$分别为两个右向量$\mathbf{K}$空间与$\mathbf{K}'$结构$V'_1, V'_2$。 $V'_1 \times V'_2$是$V_1 \times V_2$上的$\mathbf{K}'$结构，即直接的，称为$\mathbf{K}'$结构$V'_1$和$V'_2$的乘积。

#### 命题 4 {#alg-ii-s8-prop-4 .statement tag=05VB}

对于$\mathbf{K}$线性映射$f : V_1 \to V_2$在$\mathbf{K}'$上有理数，对于$V_1 \times V_2$上的乘积$\mathbf{K}'$结构，其图$\Gamma$在$\mathbf{K}'$上有理数是必要且充分的。

设$g$从$V_1$到$V_1 \times V_2$为映射$x_1 \mapsto (x_1, f(x_1))$；这是一个 $\mathbf{K}$ 线性映射，使得 $\Gamma = g(V_1)$；如果$f$对于$\mathbf{K}'$是有理数，则根据推论2到命题3，$\Gamma$也是有理数。相反，假设$\Gamma$对于$\mathbf{K}'$是有理数，并让它具有由$V_1 \times V_2$上的结构导出的$\mathbf{K}'$结构；紧随定义，投影$\mathrm{pr}_1, \mathrm{pr}_2$的限制$p_1, p_2$到$\Gamma$，是$\mathbf{K}$线性映射，$\Gamma$的$\mathbf{K}'$到$V_1$的有理数分别为$V_2$。由于$p_1$是双射，它的逆映射$q_1$在$\mathbf{K}'$上是有理数（推论1到命题3），因此$f = p_2 \circ q_1$也是如此。

### 4.理性线性形式

令$V$为右向量空间超过$\mathbf{K}$，并具有$\mathbf{K}'$结构$V'$。由于$K'_d$是向量$\mathbf{K}$-空间$K_d$的$\mathbf{K}'$结构，我们可以将定义线性形式$x^* \in V^*$，有理数$\mathbf{K}'$，作为$V$的线性映射化为$K_d$，有理数超过$\mathbf{K}'$

V 和 K_d 上的 K' 结构。凭借no. 3、命题 3、集合，这些线性形式中的R'是复合映射下V'的对偶V'*的像

（一）$$ {V'}^* \xrightarrow{\phi} K \otimes_{K'} {V'}^* \xrightarrow{\upsilon} V^* $$

其中$\phi({x'}^*) = 1 \otimes {x'}^*$和$\upsilon(\xi \otimes {x'}^*)$是V上的线性形式$y^*$，使得$y^*(x') = \xi \langle {x'}^*, x' \rangle$对于所有$x' \in V'$（§ 5, no. 4）。我们知道这个映射是单射的（§ 7, no. 9、命题20和19）并且显然R'是V*的左向量子K'空间；此外，R'在K'上自由的每个子集在K上都是自由的。但一般来说，R'不一定在K上生成V*，因此在V*上不是定义K'结构（习题2）。然而，如果 V 在 K 上为有限维 n，V'* 在 K' 和 R' 上为维数 n，则定义典型地是 V* 上的 K' 结构。

#### 命题 5 {#alg-ii-s8-prop-5 .statement tag=05VC}

设 V 是 K 上的右向量空间，V' 是 V 上的 K' 结构，W 是 V 的向量子 K 空间。为了使 W 在 K' 上有理数，必要且充分的是，存在有理线性形式在 K' 上的集合 H \子集 V^*，使得 W 是 V 中 H 的正交（§ 2, no. 4）。

令 H 为 V* 的子集，其元素是 K' 上的有理数线性形式。对于所有$x^* \in H$，$x^*$的核是V的向量子K空间，K'上有理数（no. 3，推论2到命题3）；因此，这些核中的交也是V的向量子K空间，K'上的有理数（no. 2，推论1到命题2）。

相反，令 W 为 V 有理数在 K' 上的向量子 K 空间，以便 W 被标识为 $W' \otimes_{K'} K$，其中 $W' = W \cap V'$ (no. 2, 命题 2)。对于线性形式${x'}^* \in {V'}^*$在W'上的零，必要且充分的是线性形式$x^* \in V^*$（1）下的对应在W上是零，对于no. 3，推论I为命题3，

$$
\operatorname{Ker}(x^*) = (\operatorname{Ker}({x'}^*)) \otimes_{K'} K \quad \text{and} \quad \operatorname{Ker}(x^{*\prime}) = (\operatorname{Ker}(x^*)) \cap V'.
$$

令 H' 为 V'* 中 W' 的正交；我们知道 (§ 7, no. 5, 定理 7) W' 是 V' 中 H' 的正交；如果在映射 (1) 下，H 是 V* 中 H' 的像，则根据上面的结论，W 是 V 中 H 的正交，考虑到 no. 7，推论到命题 14。

### 5. 线性系统的应用

#### 命题 6 {#alg-ii-s8-prop-6 .statement tag=05VD}

(i) 给定系统齐次线性方程

(2)
$$
\sum_{i \in I} \alpha_{\mu i} \xi_i = 0 \quad (\mu \in M)
$$
其系数$\alpha_{\mu i}$属于到K'，K的元素的这个系统由……组成的每个解$(\xi_i)$为线性组合，K中的系数为解$(\xi'_i)$ (2) K' 的元素的由……组成。

(ii) *给定系统线性方程*

$$
\sum_{i \in I} \alpha_{\mu i} \xi_i = \beta_\mu \quad (\mu \in M)
$$

*其系数* $\alpha_{\mu i}$ *和右侧* $\beta_\mu$ *属于到* $K'$，*如果存在* $K$ 的元素解到系统由……组成，*也存在* $K'$ 元素解由……组成。

(i) 对于每个集合 S，让右侧向量 K 空间$K_d^{(S)}$ 被赋予$K'$-结构$K_{d'}^{(S)}$。令$f$为$K_d^{(I)}$的K-线性映射进入$K_d^{(M)}$映射，对于所有$\mu \in M$，每向量$(\xi_i)_{i \in I}$到向量$(\zeta_\mu)_{\mu \in M}$由$\zeta_\mu = \sum_{i \in I} \alpha_{\mu i} \xi_i$定义。显然 $f$ 比 $K'$ 有理数； 核 V，即系统 (2) 的 K 中的解的集合，是$K'$ 上$K_d^{(I)}$ 有理数的子空间（no. 3，推论 2 到命题 3），因此生成$K'$ 中的 (2) 的解。

(ii) 我们将 K 视为左向量 $K'$-空间；存在 K 的 $K'$-线性投影算子 $p$ 到其向量子空间 $K'_s$ (§ 7, no. 3, 命题 4)；若$(\xi_i)$是K中(3)的解，则$\sum_{i \in I} \alpha_{\mu i} p(\xi_i) = p \left( \sum_{i \in I} \alpha_{\mu i} \xi_i \right) = p(\beta_\mu) = \beta_\mu$，证明$(p(\xi_i))$是$K'$中(3)的解。

如果命题 6 对于 K 和 $K'$ 成立，则环 K 被称为（左）在子环 $K'$ 上“忠实平坦”；我们稍后会详细研究这个概念（*交换代数*，I, § 3）。

### 6. 最小的域理性

令 V 为具有 $K'$ 结构 $V'$ 的右向量 K 空间。对于每个域 L 使得 $K' \subset L \subset K$，我们写 $V_L = V'.L$；显然，$V'$在$K'$上的每个基都是V在K上的基和$V_L$在L上的基。因此，$V_L$是V上的L结构，$V'$是$V_L$上的$K'$结构。

#### 命题 7 {#alg-ii-s8-prop-7 .statement tag=05VE}

(i) *令 V 为具有 K' 结构 V' 的右向量 K 空间。对于每个向量 $x \in V$（分别为 V 的每个向量子 K 空间 W），K 包含 $K'$ 的子域 L 的集合，并且使得 $x$（分别为 W）在 L 上是有理数，并且至少有元素 $K'(x)$（分别为$K'(W)$）。

(ii) *令$V_1, V_2$分别为两个右向量 K-空间，且分别具有K'-结构$V_1', V_2'$。对于$V_1$到$V_2$的每个K-线性映射 f，K 包含$K'$的子域 L 的集合，并且使得f在L上是有理数，并且具有至少元素$K'(f)$*。

我们首先证明断言 (i) 对于向量 $x \in V$。令 B 为 V 有理数在 $K'$ 上的基；对于每个域 L，B 是 $V'$ 的基超过 $K'$ 以及 $V_L$ 的基超过 L，使得 $K' \subset L \subset K$；为了使$x = \sum_{b \in B} b \xi_b$在L上有理数，$\xi_b$属于到L（no. 2），因此最小的域L，其中性质是域*由K'生成*，并且$\xi_b$为$b \in B$。

接下来我们证明(ii)。令$B_1, B_2$分别为$V_1, V_2$的基，对$K'$有理数并写，对于所有$b_1 \in B_1, f(b_1) = \sum_{b_2 \in B_2} b_2 \alpha_{b_2 b_1}$（*族$(\alpha_{b_2 b_1})$只是$f$相对于基$B_1$的*矩阵*，并且$B_2$；cf.§ 10, no. 4*）。由于对于每个域，$B_1$（或$B_2$）在L上是$(V_1)_L$（或$(V_2)_L$）的基，使得$K' \subset L \subset K$，对于$f$在L上是有理数，$\alpha_{b_2 b_1}$是充分必要的属于至 L；因此，最小的域与性质是由 K' 和 $b_1 \in B_1, b_2 \in B_2$ 的 $\alpha_{b_2 b_1}$ *生成*的域。

最后，要为V的子空间W建立断言(i)，我们首先要证明以下引理：

#### 引理 1 {#alg-ii-s8-lem-1 .statement tag=05VF}

*Let V be a right 向量 K-space with a K'-structure V' and W 向量 sub-K-space of V. There exist two 向量 sub-K-spaces $W_1, W_2$ of V, rational over K', such that V is 直和 of $W_1$ and $W_2$ and, if V is identified with $W_1 \times W_2$，W是$W_1$的K-线性映射g到$W_2$的图。*

令 B 为 K' 上 V 有理数的基。 § 7, no. 1的应用定理2，到W的基超过K，视为V的自由子集，以及该自由子集和B的生成的系统并，可见存在B 的子集 C，使得 V 是 W 的直和和 C 生成的 V 的子空间 $W_2$。还令 $W_1$ 是 $B - C$ 生成的 V 的子空间。由于$B \subset V'$，显然$W_1$和$W_2$对于K'是有理数。此外，对于所有$x \in W_1$，存在且仅有一个$W_2$的向量$g(x)$使得$x + g(x) \in W$，因为V是W的直和和$W_2$；那么 W 是 g 的图，并且 g 是 K 线性的，因为 W 是 V 的向量子 K 空间。

证明了引理，可知W 在K 包含于 K' 的子域 L 上是有理数当且仅当g 在L (no. 3, 命题 4) 上是有理数。 最小的域 $K'(g)$ 使得 g 在 $K'(g)$ 上是有理数，因此也是最小的域，其中 W 是有理数。

### 7. 判据理性

对于 K 的每个子域 L，令 $\mathrm{End}_L(K)$ 表示 K 的自同态环被视为 L 上的 *左向量空间*；如果 L 包含于 K'，$\mathrm{End}_L(K)$ 是 $\mathrm{End}_{K'}(K)$ 的子环。对于 $\mathrm{End}_{K'}(K)$ 的每个子集 $\mathscr{M}$，都存在一个 K 包含于 K' 的 *最大的子域* L，并且使得 $\mathscr{M}$ 包含在 $\mathrm{End}_L(K)$ 中，即 $\xi \in K$ 的集合使得 $\phi(\xi \eta) = \xi \cdot \phi(\eta)$对于所有$\eta \in K$和所有$\phi \in \mathscr{M}$（立即验证这个集合是环，另一方面，前面的关系中的$\xi^{-1} \eta$是替换$\eta$，当$\xi \neq 0$时我们得到$\phi(\xi^{-1} \eta) = \xi^{-1} \cdot \phi(\eta)$）。我们将把这个域称为K中$\mathscr{M}$的*中心化器*，并用$\chi(\mathscr{M})$表示。

现在令 V 为具有 K' 结构 V' 的右向量 K 空间。对于所有$\phi \in \mathrm{End}_{K'}(K)$，存在且仅有一个$\mathbf{Z}$模V的自同态$\phi_v$，使得$\phi_V(x'.\xi) = x'.\phi(\xi)$对于$x' \in V'$和$\xi \in K$：对于no. 1中，$\mathbf{Z}$同构$\lambda$定义$V' \otimes_{K'} K$到V，其中映射、$x' \otimes \xi$到$x'.\xi$且$\phi_V$必然等于$\lambda \circ (1_{V'} \otimes \phi) \circ \lambda^{-1}$。

#### 定理 1 {#alg-ii-s8-thm-1 .statement tag=05VG}

*设$\mathscr{M}$为$\mathrm{End}_{K'}(K)$的子集和K的$L = \chi(\mathscr{M})$子域，即$\mathscr{M}$的扶正器。*

(i) *令 V 为具有 K' 结构的右向量 K 空间。为了使向量 $x \in V$ 对 L 有理数，$\phi_V(x.\eta) = x.\phi(\eta)$ 对于所有 $\phi \in \mathscr{M}$ 和所有 $\eta \in K$ 是充分必要的。为了使 V 的向量子 K 空间 W 在 L 上有理数，$\phi_V(W) \subset W$ 对于所有 $\phi \in \mathscr{M}$ 是充分必要的。*

(ii) *令 $V_1, V_2$ 为两个右向量 K 空间，每个都有一个 K' 结构。为了使$V_1$到$V_2$的K-线性映射 f在L上是有理数，$f(\phi_{V_1}(x_1)) = \phi_{V_2}(f(x_1))$对于所有$x_1 \in V_1$和所有$\phi \in \mathscr{M}$是必要且充分的。*

我们首先证明 x 的断言 (i)。令 B 为 K' 上 V 有理数的基并写为 $x = \sum_{b \in B} b.\xi_b$；那么，对于$\phi \in \mathscr{M}$和$\eta \in K$，

$$
\phi_V(x.\eta) - x.\phi(\eta) = \sum_{b \in B} b.(\phi(\xi_b\eta) - \xi_b.\phi(\eta))
$$

因此，关系

“对于所有$\phi \in \mathscr{M}$和所有$\eta \in K$，$\phi_V(x.\eta) = x.\phi(\eta)$”

和

“对于所有 $\phi \in \mathscr{M}$、所有 $b \in B$ 以及所有 $\eta \in K$、$\phi(\xi_b\eta) = \xi_b.\phi(\eta)$”

是等价的。其中第二个关系意味着对于所有$b \in B$，$\xi_b \in \chi(\mathscr{M})$，这证明了(i)的第一个断言。

接下来我们证明(ii)。为了使 f 在 L 上有理数，对于所有 $x'_1 \in V_1$ 在 K' 上有理数，$f(x'_1)$ 是向量在 $V_2$ 在 L 上有理数；这意味着$f(x_1)$对于L上的向量$x_1$是有理数$V_1$有理数超过L，这样向量是线性组合，L中的系数是向量有理数超过K'。上面的条件通过参数的第一个部分等价于关系

$$
f(x'_1).\phi(\eta) = \phi_{V_2}(f(x'_1).\eta) \quad \text{for } \phi \in \mathscr{M} \text{ and } \eta \in K
$$

也可以写成

$$
f(\phi_{V_1}(x'_1.\eta)) = \phi_{V_2}(f(x'_1.\eta)) \quad \text{for } \phi \in \mathscr{M} \text{ and } \eta \in K.
$$

由于 $V_1$ 的每个元素都是线性组合，且 $V_1$ 的元素的 K 中的系数超过 K' 有理数，条件 (5) 等价于

$$
f(\phi_{V_1}(x_1)) = \phi_{V_2}(f(x_1))
$$

对于所有 $x_1 \in V_1$ 和所有 $\phi \in \mathscr{M}$。

最后，为了证明（i）中的第二个断言，我们使用no. 6，引理1：W是K-线性映射$g : W_1 \to W_2$的图，并且W在当且仅当映射g在L（no. 3，命题4）上是有理数时才是有理数。通过 (ii)，要使 g 对 L 有理数，对于所有 $x_1 \in W_1$ 和所有 $\phi \in \mathscr{M}$，$g(\phi_{W_1}(x_1)) = \phi_{W_2}(g(x_1))$ 是充分必要的；如$\phi_v = \phi_{W_1} \times \phi_{W_2}$，上面的条件表示对于所有$\phi \in \mathscr{M}$，g的图W在$\phi_v$下是稳定的。

### 习题{#alg-ii-s8-exercises}

§ 8](exercises/s8/)参见[习题。
