---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 6
section_title: Inverse and direct limits of modules
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 284-291, 399-400
pdf_pages: 0308-0315, 0423-0424
extraction: ocr
subsections:
    - "no": 1
      title: INVERSE LIMITS OF MODULES
      page: 284
      pdf_page: 308
    - "no": 2
      title: DIRECT LIMITS OF MODULES
      page: 286
      pdf_page: 310
    - "no": 3
      title: TENSOR PRODUCT OF DIRECT LIMITS
      page: 289
      pdf_page: 313
statements: 17
exercises: 4
content_sha256: 7c7990f575590f85e5b917aaeed17f43d078e206e632ba44d4bdf09b2db4ddbf
translated_from: content/en/alg/II/06_s6_inverse_and_direct_limits_of_modules.md
translation_method: google
source_content_sha256: 2682c7eae62790237d64df767969f62d7aa7d61ceec717b4af26629c4a2f746a
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: ed17704e4ad2bfc2ad14769e4c5a980050f85b0bd3114374f5e4f6729043a7cd
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 6。 模的逆与直极限

在本段中，我将在 I 上表示非空预序集合和 $\alpha \leq \beta$ 预序关系。另外提到的除非，逆矩阵和直接系统具有索引集合 I。

### 1. 逆极限的模

令$(A_\alpha, \phi_{\alpha \beta})$为环(I, § 10, no. 1)的逆系，可交换的群(加法写)(I, § 10, no. 1)的$(E_\alpha, f_{\alpha \beta})$逆系，并假设每个$E_\alpha$都有一个左$A_\alpha$模块结构；此外，假设$\alpha \leq \beta$$(f_{\alpha \beta}, \phi_{\alpha \beta})$是$E_\beta$到$E_\alpha$（§ 1, no. 13）的二态性，在其他字中
$$
f_{\alpha \beta}(\lambda_\beta x_\beta) = \phi_{\alpha \beta}(\lambda_\beta) f_{\alpha \beta}(x_\beta),
$$
对于$x_\beta \in E_\beta$、$\lambda_\beta \in A_\beta$；那么从I, § 10, no. 2可以得出$E = \lim \leftarrow E_\alpha$比$A = \lim \leftarrow A_\alpha$有左模结构。对于所有$\alpha \in I$，令$f : E \to E_\alpha$、$\phi_\alpha : A \to A_\alpha$为典范映射；那么$(f_\alpha, \phi_\alpha)$是E到$E_\alpha$的二态性。我们可以说，$(E_\alpha, f_{\alpha\beta})$是左$A_\alpha$模块*的*逆系，而$A$模块$E$是它的*逆极限*。

令$(E'_\alpha, f'_{\alpha\beta})$为左侧$A_\alpha$模块的另一个逆系，对于所有$\alpha$，令$u_\alpha : E'_\alpha \to E_\alpha$为*$A_\alpha$-线性*映射，这些映射形成*逆系*；那么 $u = \lim u_\alpha$ 是 $\lim E'_\alpha$ 到 $\lim E_\alpha$ 的 *$A$-线性* 映射。

而且：

#### 命题 1 {#alg-ii-s6-prop-1 .statement tag=05QX}

*令*$(E_\alpha, f_{\alpha\beta}),\ (E'_\alpha, f'_{\alpha\beta}),\ (E''_\alpha, f''_{\alpha\beta})$*为$A_\alpha$-模块中的三个逆系和*$(u_\alpha),\ (v_\alpha)$*$A_\alpha$-线性映射中的两个逆系，使得序列*

$$
0 \longrightarrow E'_\alpha \xrightarrow{u_\alpha} E_\alpha \xrightarrow{v_\alpha} E''_\alpha
$$

*对于所有$\alpha$都是准确的。* *然后，写* $u = \lim u_\alpha,\ v = \lim v_\alpha$，*序列*

$$
0 \longrightarrow \lim E'_\alpha \xrightarrow{u} \lim E_\alpha \xrightarrow{v} \lim E''_\alpha
$$

*准确*。

*作为* $u_\alpha^{-1}(0) = \{0\}$ *对于所有$\alpha$，它从集合理论、III, § 7, no. 2、命题 2 得出* $u^{-1}(0) = \{0\}$，*因此* $u$ *是单射的；进一步地，*$E_\alpha$*的子集的*$u_\alpha(E'_\alpha)$*形式逆系以及因此*$u(\lim E'_\alpha) = \lim u_\alpha(E'_\alpha)$。 *作为* $u_\alpha(E'_\alpha) = v_\alpha^{-1}(0)$ *通过假设，* $v^{-1}(0) = \lim u_\alpha(E'_\alpha) = u(\lim E'_\alpha)$（*集合理论*，III, § 7, no. 2，命题 2），*完成证明*。

#### 注 {#alg-ii-s6-n1-rem-1 .statement tag=05QY}

(1) 命题 1 及其证明对于任意 *群* 均有效，变换或记号除外。

(2) 注如果有正合序列

$$
0 \longrightarrow E'_\alpha \xrightarrow{u_\alpha} E_\alpha \xrightarrow{v_\alpha} E''_\alpha \longrightarrow 0
$$

*它不一定遵循*序列

$$
0 \longrightarrow \lim E'_\alpha \xrightarrow{u} \lim E_\alpha \xrightarrow{v} \lim E''_\alpha \longrightarrow 0
$$

*准确；在其他字中，满射线性映射的逆系的逆极限不一定是满射*（cf.习题1）。

现在假设$A_\alpha$等于*相同的环*$A$，并且$\phi_{\alpha\beta}$等于$1_A$；那么对于 $A$ 模块中的每个逆系 $(E_\alpha, f_{\alpha\beta})$，$E = \lim E_\alpha$ 是一个 $A$ 模块。令$F$为$A$模，对于所有$\alpha$，令$u_\alpha : F \to E_\alpha$为$A$线性映射，使得$(u_\alpha)$为映射的逆系；那么$u = \lim u_\alpha$是$F$到$\lim E_\alpha$的$A$线性映射。 *相反*，对于每个$A$-线性映射$v : F \to \lim E_\alpha$，$v_\alpha = f_\alpha \circ v$族是$A$-线性映射的逆系，使得$v = \lim_{\leftarrow} v_\alpha$。另一方面，我们注对于$\alpha \leq \beta$映射

$$
\operatorname{Hom}(1_F, f_{\alpha \beta}) = \bar{f}_{\alpha \beta}: \operatorname{Hom}_A(F, E_\beta) \to \operatorname{Hom}_A(F, E_\alpha)
$$

是一个$\mathbf{Z}$-模块同态，使得$(\operatorname{Hom}_A(F, E_\alpha), \bar{f}_{\alpha \beta})$是$\mathbf{Z}$-模块*的*逆系；由于$\bar{f}_{\alpha \beta}(v_\beta) = f_{\alpha \beta} \circ v_\beta$，因此上述注可以表示为：

#### 命题 2 {#alg-ii-s6-prop-2 .statement tag=05QZ}

*对于$A$*模块中的每个逆系* $(E_\alpha, f_{\alpha \beta})$ *和每个$A$*-模块$F$，*典范映射* $u \mapsto (f_\alpha \circ u)$ *是一个$\mathbf{Z}$*-模块*同构*

(2)

$$
l_F: \operatorname{Hom}_A(F, \lim_{\leftarrow} E_\alpha) \to \lim_{\leftarrow} \operatorname{Hom}_A(F, E_\alpha).
$$

#### 推论{#alg-ii-s6-n1-cor-1 .statement tag=05R0}

*对于每个$A$*-模块同态$v: F \to F'$，*

$$
\bar{v}_\alpha = \operatorname{Hom}(v, 1_{E_\alpha}): \operatorname{Hom}(F', E_\alpha) \to \operatorname{Hom}(F, E_\alpha)
$$

*$\mathbf{Z}$*的形式逆系-线性映射*和图表*

(3)

$$
\begin{array}{ccc}
\operatorname{Hom}(F', \lim_{\leftarrow} E_\alpha) & \xrightarrow{l_{F'}} & \lim_{\leftarrow} \operatorname{Hom}(F', E_\alpha) \\
\downarrow \operatorname{Hom}(v, 1_E) & & \downarrow \lim_{\leftarrow} \bar{v}_\alpha \\
\operatorname{Hom}(F, \lim_{\leftarrow} E_\alpha) & \xrightarrow{l_F} & \lim_{\leftarrow} \operatorname{Hom}(F, E_\alpha)
\end{array}
$$

*是可交换的*。

对于所有$u \in \operatorname{Hom}(F', \lim_{\leftarrow} E_\alpha)$，$l_F(u \circ v) = (f_\alpha \circ u \circ v)$乘以定义和交换律，图表(3)紧随定义而来。

### 2. 直极限的模

*从此以后我被认为是正确的。*

令$(A_\alpha, \phi_{\beta \alpha})$为环(I, § 10, no. 3)的直接系统，可交换的群(加法写)(I, § 10, no. 3)的$(E_\alpha, f_{\beta \alpha})$直接系统，并假设每个$E_\alpha$都有一个*左$A_\alpha$*-模块结构；此外，假设对于$\alpha \leq \beta$，$(f_{\beta \alpha}, \phi_{\beta \alpha})$是$E_\alpha$到$E_\beta$（§ 1, no. 13）的*二态*，在其他字中

(4)

$$
f_{\beta \alpha}(\lambda_\alpha x_\alpha) = \phi_{\beta \alpha}(\lambda_\alpha) f_{\beta \alpha}(x_\alpha)
$$

对于$x_\alpha \in E_\alpha, \lambda_\alpha \in A_\alpha$；那么 $E = \lim_{\longrightarrow} E_\alpha$ 的 *左模* 结构超过 $A = \lim_{\longrightarrow} A_\alpha$ (I, § 10, no. 4)。对于所有$\alpha \in I$，令$f_\alpha: E_\alpha \to E, \phi_\alpha: A_\alpha \to A$为典范映射；那么$(f_\alpha, \phi_\alpha)$是$E_\alpha$到$E$的*二态*。我们可以说$(E_\alpha, f_{\beta \alpha})$是左$A_\alpha$*模块的*直接系统，$A$*模块$E$是它的*直极限*。

令$(E'_\alpha, f'_{\beta \alpha})$为左$A_\alpha$*模块的另一个直接系统，并且对于所有$\alpha$，令$u_\alpha : E'_\alpha \to E_\alpha$为$A_\alpha$线性映射，这些映射形成直接系统；那么$u = \lim \to u_\alpha$是$\lim \to E'_\alpha$到$\lim \to E_\alpha$的$A$线性映射。

此外：

#### 命题 3 {#alg-ii-s6-prop-3 .statement tag=05R1}

*令*$(E_\alpha, f_{\beta \alpha}), (E'_\alpha, f'_{\beta \alpha}), (E''_\alpha, f''_{\beta \alpha})$*为*$A_\alpha$*-模块中的三个直接系统和*$(u_\alpha), (v_\alpha)$**$A_\alpha$*中的两个直接系统-线性映射，使得序列*

$$
E'_\alpha \xrightarrow{u_\alpha} E_\alpha \xrightarrow{v_\alpha} E''_\alpha
$$

*对所有人来说都是准确的*$\alpha$。 *然后，写*$u = \lim \to u_\alpha, v = \lim \to v_\alpha$，*序列*

$$
\lim \to E'_\alpha \xrightarrow{u} \lim \to E_\alpha \xrightarrow{v} \lim \to E''_\alpha
$$

*准确。*

$u(\lim \to E'_\alpha) = \lim \to u_\alpha(E'_\alpha)$ *和* $v^{-1}(0) = \lim \to v_\alpha^{-1}(0)$ *（集合理论，III, § 7, no. 6，命题 7 的推论）。*

宽松地说，命题 3 也可以用说表示，*经过到直极限保持精确性*。

#### 命题 4 {#alg-ii-s6-prop-4 .statement tag=05R2}

*让*$(E_\alpha, f_{\beta \alpha})$*成为*$A_\alpha$*模块的直接系统，$E = \lim \to E_\alpha$*其直极限和*$\phi_\alpha : A_\alpha \to A$*和*$f_\alpha : E_\alpha \to E$*典范映射对于所有*$\alpha \in I$。 *如果，对于所有* $\alpha \in I$、$S_\alpha$ *是* $E_\alpha$ 的生成的系统，*则* $S = \bigcup_{\alpha \in I} f_\alpha(S_\alpha)$ *是* $E$ 的生成的系统。

每个$x \in E$ *是形式* $f_\alpha(x_\alpha)$ *对于一些* $\alpha \in I$ *和一些* $x_\alpha \in E_\alpha$ *和假设* $x = \sum_i \lambda^{(i)}_\alpha y^{(i)}_\alpha$，*其中* $\lambda^{(i)}_\alpha \in A_\alpha$ *和* $y^{(i)}_\alpha \in S_\alpha$； *写*$\lambda^{(i)} = \phi_\alpha(\lambda^{(i)}_\alpha)$，$y^{(i)} = f_\alpha(y^{(i)}_\alpha)$，*我们得到*$x = \sum_i \lambda^{(i)} y^{(i)}$。

#### 命题 5 {#alg-ii-s6-prop-5 .statement tag=05R3}

*根据命题 4 的假设和记号，假设对于所有* $\alpha \in I$，$E_\alpha$ *是一个家庭* $(M^\lambda_\alpha)_{\alpha \in L}$ *的直和* 子模（索引集合* $L$ *独立于* $\alpha$) *和那个* $f_{\beta \alpha}(M^\lambda_\alpha) \subset M^\lambda_\alpha$ *为了* $\alpha \leq \beta$ *和所有* $\lambda \in L$。 *那么*$E$*是子模*$M^\lambda = \lim \to M^\lambda_\alpha$$(\lambda \in L)$中的直和。

从命题 4 可以得出，$E$ 是$M^\lambda$ 的和。 令$(y^\lambda)_{\lambda \in L}$ *成为一个家庭，使得* $y^\lambda \in M^\lambda$ *对于所有人* $\lambda \in L$ *且其支持是有限的，并假设* $\sum_\lambda y^\lambda = 0$。 *根据集合理论，III, § 7, no. 5，引理1，存在*$\alpha \in I$*和*$(x^\lambda_\alpha)_{\alpha \in L}$*的有限支撑由……组成*$E_\alpha$*的元素*使得*$x^\lambda_\alpha \in M^\lambda_\alpha$*和* $y^\lambda = f_\alpha(x^\lambda_\alpha)$ *对于所有人* $\lambda \in L$。 *关系* $f_\alpha \left( \sum_{\lambda \in L} x^\lambda_\alpha \right) = 0$ *暗示存在a* $\beta \geq \alpha$ *使得* $f_{\beta \alpha} \left( \sum_{\lambda \in L} x^\lambda_\alpha \right) = 0$ *(集合理论, III, § 7, no. 5, 引理 1)，可写为$\sum_{\lambda \in L} x_\beta^\lambda = 0$，其中$x_\beta^\lambda = f_{\beta \alpha}(x_\alpha^\lambda) \in M_\beta^\lambda$乘假设；因此$x_\beta^\lambda = 0$对于所有$\lambda \in L$，因此$y^\lambda = f_\beta(x_\beta^\lambda) = 0$对于所有$\lambda \in L$，这证明$M^\lambda$的和是直接的。

#### 推论{#alg-ii-s6-n2-cor-1 .statement tag=05R4}

*令*$(P_\alpha)$*为*$E_\alpha$*的子集直接系统并且令*$P = \lim \overrightarrow{P_\alpha}$。 *如果，对于所有* $\alpha \in I$、$P_\alpha$ *是* $E_\alpha$ 的免费子集（或基），*则* $P$ *是* $E$ 的免费子集（或基）。

第二个断言紧随第一个命题4。因此，足以证明如果$P_\alpha$是免费的，则$P$的不同元素的每个子集$\{ y^{(i)} \}_{1 \leq i \leq n}$由……组成都是免费的。存在$\alpha \in I$和元素$x_\alpha^{(i)} \in P_\alpha$，使得$y^{(i)} = f_\alpha(x_\alpha^{(i)})$对应$1 \leq i \leq n$（*集合理论*，III, § 7, no. 5，引理1）；如果$\sum_i \lambda^{(i)} y^{(i)} = 0$，可以假设$\lambda^{(i)} = \phi_\alpha(\lambda_\alpha^{(i)})$对应$1 \leq i \leq n$，因此$f_\alpha \left( \sum_i \lambda_\beta^{(i)} x_\beta^{(i)} \right) = 0$；这意味着$\sum_i \lambda_\beta^{(i)} x_\beta^{(i)} = 0$对于某些$\beta \geq \alpha$来说，其中$\lambda_\beta^{(i)} = \phi_{\beta \alpha}(\lambda_\alpha^{(i)})$、$x_\beta^{(i)} = f_{\beta \alpha}(x_\alpha^{(i)})$和$x_\beta^{(i)}$、属于到$P_\beta$并且从$y^{(i)} = f_\beta(x_\beta^{(i)})$开始是不同的；然后$\lambda_\beta^{(i)} = 0$换$1 \leq i \leq n$，从而
$$
\lambda^{(i)} = \phi_\beta(\lambda_\beta^{(i)}) = 0
$$
$1 \leq i \leq n$。

现在假设所有环$A_\alpha$都等于*相同的环*$A$以及$\phi_{\beta \alpha}$到$1_A$；那么，对于 $A$ 模块中的每一个直接系统 $(E_\alpha, f_{\beta \alpha})$，$E = \lim \overrightarrow{E_\alpha}$ 都是一个 $A$ 模块。令$F$为$A$-模，对于所有$\alpha$，让$u_\alpha : E_\alpha \to F$为$A$-线性映射，使得$(u_\alpha)$为映射的直接系统；那么$u = \lim \overrightarrow{u_\alpha}$是$E$到$F$的$A$线性映射。 *相反*，对于每个$A$-线性映射$v : \lim \overrightarrow{E_\alpha} \to F$，$v_\alpha = v \circ f_\alpha$族是$A$-线性映射的直接系统，使得$v = \lim \overrightarrow{v_\alpha}$。另一方面，我们注 $\alpha \leq \beta$ 映射
$$
\operatorname{Hom}(f_{\beta \alpha}, 1_F) = \bar{f}_{\alpha \beta} : \operatorname{Hom}_A(E_\beta, F) \to \operatorname{Hom}_A(E_\alpha, F)
$$
是一个$\mathbf{Z}$-模块同态，使得$(\operatorname{Hom}_A(E_\alpha, F), \bar{f}_{\alpha \beta})$是*逆系*$\mathbf{Z}$*-模块*；为$\bar{f}_{\alpha \beta}(v_\beta) = v_\beta \circ f_{\beta \alpha}$，则上述注可表示为：

#### 命题 6 {#alg-ii-s6-prop-6 .statement tag=05R5}

*对于每个直接系统* $(E_\alpha, f_{\beta \alpha})$ *of* $A$*-模块和每个* $A$*-模块* $F$，*典范映射* $u \mapsto (u \circ f_\alpha)$ *是一个* $\mathbf{Z}$*-模块同构*
$$
d_F : \operatorname{Hom}_A(\lim \overrightarrow{E_\alpha}, F) \to \lim \leftarrow \operatorname{Hom}_A(E_\alpha, F).
$$

#### 推论 1 {#alg-ii-s6-prop-6-cor-1 .statement tag=05R6}

*对于每个* $A$*-模块同态* $v : F \to F'$，*该*
$$
\bar{v}_\alpha = \operatorname{Hom}(1_{E_\alpha}, v) : \operatorname{Hom}(E_\alpha, F) \to \operatorname{Hom}(E_\alpha, F')
$$

$\mathbf{Z}$线性映射的形式逆系和图表

$$
\begin{array}{ccc}
\operatorname{Hom}(\lim E_\alpha, F) & \xrightarrow{d_F} & \lim \operatorname{Hom}(E_\alpha, F) \\
\downarrow \operatorname{Hom}(1_E, v) & & \downarrow \lim \overline{v}_\alpha \\
\operatorname{Hom}(\lim E_\alpha, F') & \xrightarrow{d_{F'}} & \lim \operatorname{Hom}(E_\alpha, F')
\end{array}
$$

是可交换的。

对于所有 $u \in \operatorname{Hom}(\lim E_\alpha, F)$、$d_{F'}(v \circ u) = (v \circ u \circ f_\alpha)$、定义和交换律，图表 (6) 则紧随定义。

#### 推论 2 {#alg-ii-s6-prop-6-cor-2 .statement tag=05R7}

*如果* $(E_\alpha, f_{\beta \alpha})$ *是左* $A$*-模块的直接系统，并且* $E = \lim \longrightarrow E_\alpha$、$(E_\alpha^*, t f_{\beta \alpha})$ *是右* $A$*-模块的逆系，并且* $\lim \leftarrow E_\alpha^*$ *规范地同构于* $E^*$。

#### 注 {#alg-ii-s6-n2-rem-1 .statement tag=05R8}

设$E$是$A$*模块，并且*$(M_\alpha)_{\alpha \in I}$*递增是*$E$的子模族，使得*$E$*是*$M_\alpha$的并；如果$j_{\beta \alpha}: M_\alpha \to M_\beta$（对于$\alpha \leq \beta$）和$j_\alpha: M_\alpha \to E$ *是典范嵌入，则直接的* $j = \lim \longrightarrow j_\alpha$ *是* $\lim \longrightarrow M_\alpha$ *上的同构 * $E$ *（集合理论， III, § 7, no. 6、注 1)*。特别是，每个$A$*-模块都是其*有限生成*子模的右有向族的直极限。

### 3.张量积直极限

令 $(A_\alpha, \rho_{\beta \alpha})$ 为环的直接系统，$(E_\alpha, f_{\beta \alpha})$（分别为 $(F_\alpha, g_{\beta \alpha})$）为右（分别为左）$A_\alpha$*-模块的直接系统。对于$\alpha \leq \beta$，有一个$\mathbf{Z}$*-模块同态*

$$
f_{\beta \alpha} \otimes g_{\beta \alpha}: E_\alpha \otimes_{A_\alpha} F_\alpha \to (E_\beta)_{[A_\alpha]} \otimes_{A_\alpha} (F_\beta)_{[A_\alpha]}
$$

另一方面，有一个规范的 $\mathbf{Z}$*-模块同态*

$$
(E_\beta)_{[A_\alpha]} \otimes_{A_\alpha} (F_\beta)_{[A_\alpha]} \to E_\beta \otimes_{A_\beta} F_\beta
$$

相应的至环同态$\rho_{\beta \alpha}$（$§ 3$、no. 3、命题2）； 从而通过合成，我们得到一个$\mathbf{Z}$*-模块同态*

$$
h_{\beta \alpha}: E_\alpha \otimes_{A_\alpha} F_\alpha \to E_\beta \otimes_{A_\beta} F_\beta
$$

其中映射张量积$x_\alpha \otimes y_\alpha$至$f_{\beta \alpha}(x_\alpha) \otimes g_{\beta \alpha}(y_\alpha)$。显然

$$
(E_\alpha \otimes_{A_\alpha} F_\alpha, h_{\beta \alpha})
$$

是 *直接系统* 个 $\mathbf{Z}$* 个模块。让*$A = \lim \longrightarrow A_\alpha$，$E = \lim \longrightarrow E_\alpha$，$F = \lim \longrightarrow F_\alpha$*和*

设$\rho_\alpha : A_\alpha \to A, f_\alpha : E_\alpha \to E, g_\alpha : F_\alpha \to F$为典范映射。如上，定义了一个$\mathbf{Z}$-线性映射$\pi_\alpha : E_\alpha \otimes_{A_\alpha} F_\alpha \to E \otimes_A F$，其中映射张量积$x_\alpha \otimes y_\alpha$到$f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha)$，映射形式直接系统为直接的。这样我们就得到了$\mathbf{Z}$-线性映射
$$
\pi = \lim \pi_\alpha : \lim (E_\alpha \otimes_{A_\alpha} F_\alpha) \to E \otimes_A F.
$$

#### 命题 7 {#alg-ii-s6-prop-7 .statement tag=05R9}

*$\mathbf{Z}$-线性映射 (7) 是双射的。*

我们集合$P = \lim (E_\alpha \otimes_{A_\alpha} F_\alpha)$，并且对于所有$\alpha \in I$，令$h_\alpha : E_\alpha \otimes_{A_\alpha} F_\alpha \to P$为典范映射。另一方面，对于所有 $\alpha \in I$，让
$$
t_\alpha : E_\alpha \times F_\alpha \to E_\alpha \otimes_{A_\alpha} F_\alpha
$$
是规范的$\mathbf{Z}$-双线性映射；对于$\alpha \leq \beta$，
$$
t_\beta(f_{\beta \alpha}(x_\alpha), g_{\beta \alpha}(y_\alpha)) = f_{\beta \alpha}(x_\alpha) \otimes g_{\beta \alpha}(y_\alpha) = h_{\beta \alpha}(t_\alpha(x_\alpha, y_\alpha))
$$
因此 $(t_\alpha)$ 是映射的直接系统。将$\lim (E_\alpha \times F_\alpha)$与$E \times F$（*集合理论*，III, § 7, no. 7，命题10）进行规范地识别，我们推导出映射$t = \lim t_\alpha : E \times F \to P$，使得
$$
t(f_\alpha(x_\alpha), g_\alpha(y_\alpha)) = h_\alpha(t_\alpha(x_\alpha, y_\alpha)) = h_\alpha(x_\alpha \otimes y_\alpha).
$$
考虑*集合理论*、III, § 7, no. 5、引理1，立即看出$t$是$\mathbf{Z}$双线性；此外，对于$x \in E, y \in F, \lambda \in A$，存在$\alpha \in I$使得$x = f_\alpha(x_\alpha), y = g_\alpha(y_\alpha), \lambda = \rho_\alpha(\lambda_\alpha)$与$\lambda_\alpha \in A_\alpha, x_\alpha \in E_\alpha, y_\alpha \in F_\alpha$（*集合理论*，III, § 3, no. 7，引理1）； 从而
$$
t(x \lambda, y) = h_\alpha((x_\alpha \lambda_\alpha) \otimes y_\alpha) = h_\alpha(x_\alpha \otimes (\lambda_\alpha y_\alpha)) = t(x, \lambda y).
$$
因此，存在且仅有一个$\mathbf{Z}$-线性映射$\pi' : E \otimes_A F \to P$，使得$\pi'(x \otimes y) = t(x, y)$ (§ 3, no. 1, 命题 1)。此外，通过定义
$$
\pi'(\pi(h_\alpha(x_\alpha \otimes y_\alpha))) = \pi'(f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha)) = h_\alpha(x_\alpha \otimes y_\alpha)
$$
$$
\pi(\pi'(f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha))) = \pi(h_\alpha(x_\alpha \otimes y_\alpha)) = f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha)
$$
并且作为形式 $f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha)$（分别为 $h_\alpha(x_\alpha \otimes y_\alpha)$）生成的元素，$\mathbf{Z}$-模块 $E \otimes_A F$（分别为 $P$）、$\pi' \circ \pi$ 和 $\pi \circ \pi'$ 为恒等映射。

宽松地说，命题 7 可以用说来表示，*张量积与直极限*可交换，并且通常通过同构$\pi$来标识（7）的两侧。

#### 推论 1 {#alg-ii-s6-prop-7-cor-1 .statement tag=05RA}

*令*$(E'_\alpha, f'_{\beta \alpha})$（或$(F'_\alpha, g'_{\alpha \beta})$）*为右*（或*左*）的另一个直接系统*$A_\alpha$*-*模；对于所有* $\alpha \in I$，*让* $u_\alpha : E_\alpha \to E'_\alpha$（或$v_\alpha : F_\alpha \to F'_\alpha$）*成为*

$A_\alpha$-线性映射，使得$(u_\alpha)$（分别为$(v_\alpha)$）为直接系统。那么$(u_\alpha \oplus v_\alpha)$是$\mathbf{Z}$线性映射的直接系统和图表

$$
\begin{array}{ccc}
\lim(E_\alpha \otimes_{A_\alpha} F_\alpha) & \longrightarrow & (\lim E_\alpha) \otimes_A (\lim F_\alpha) \\
\downarrow & & \downarrow \\
\lim(u_\alpha \otimes v_\alpha) & & (\lim u_\alpha) \otimes (\lim v_\alpha) \\
\lim(E'_\alpha \otimes_{A_\alpha} F'_\alpha) & \longrightarrow & (\lim E'_\alpha) \otimes_A (\lim F'_\alpha)
\end{array}
$$

是可交换的。

验证为直接的。

令$(A'_\alpha, \rho'_{\beta\alpha})$为环的另一个直接系统，并假设每个$E_\alpha$是$(A'_\alpha, A_\alpha)$双模，$f_{\beta\alpha}$对于$\alpha \leq \beta$是$(A'_\alpha, A_\alpha)$线性。那么，如果我们写 $A' = \lim A'_\alpha$，则根据推论 1，同构 (7) 相对于两侧左侧的 $A'$ 模块结构是*线性的。这可以立即推广到任意多模块。

特别是，如果$A_\alpha$是*可交换的*，则$A = \lim A_\alpha$是可交换的并且同构(7)是*A-模同构*。

#### 推论 2 {#alg-ii-s6-prop-7-cor-2 .statement tag=05RB}

*设*$(E_\alpha, f_{\beta\alpha})$*为右*$A_\alpha$*-模块的直接系统，并让*$E'_\alpha = E_\alpha \otimes_{A_\alpha} A$*为通过典范同态*$\rho_\alpha : A_\alpha \to A$将标量的环扩展到*$A = \lim A_\alpha$*所获得的*$A$*-模块。 *那么* $(E'_\alpha, f_{\beta\alpha} \otimes 1_A)$ *是右* $A$*模块的直接系统，*其直极限规范地同构于* $\lim E_\alpha$。

它足以满足应用命题 7，其中 $F_\alpha$ 环 $A$ 通过 $\rho_\alpha$ 被视为 $(A_\alpha, A)$ 双模。

#### 推论 3 {#alg-ii-s6-prop-7-cor-3 .statement tag=05RC}

*设*$A$*为环，右*$A$*-模块和*$F$*左*$A$*-模块的*$(E_\alpha, f_{\beta\alpha})$*直接系统。 *那么* $\mathbf{Z}$*-模块* $\lim (E_\alpha \otimes_A F)$ *和* $(\lim E_\alpha) \otimes_A F$ *是规范同构的*。

对于命题 7 中的所有$\alpha \in I$，取$A_\alpha = A$ 和$F_\alpha = F$ 就足够了。

特别是，如果 $\rho : A \to B$ 是环同态，则 $\lim \rho^*(E_\alpha)$ 和 $\rho^*(\lim E_\alpha)$ 是规范同构的。

#### 推论 4 {#alg-ii-s6-prop-7-cor-4 .statement tag=05RD}

*设* $M$ *为右* $A$*-模，$N$ *左* $A$*-模，$(x_i)_{1 \leq i \leq n}$ *元素的族* $M$，$(y_i)_{1 \leq i \leq n}$ *元素的族* $N$，*使得*$\sum_i (x_i \otimes y_i) = 0$*在*$M \otimes_A N$。 *然后存在一个有限生成的子模* $M_1$ *(resp. $N_1$) of* $M$ *(resp. $N$) 包含 the* $x_i$ *(resp. the* $y_i$) *并且这样* $\sum_i (x_i \otimes y_i) = 0$*在*$M_1 \otimes_A N_1$。

$M$（分别$N$）被规范地等同于其有限生成的子模包含和$x_i$（分别$y_i$）的右有向族的直极限，并且足以应用*集合理论， III, § 7, no. 5, 引理 1.*

### 习题 {#alg-ii-s6-exercises}

§ 6](exercises/s6/)参见[习题。
