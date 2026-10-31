---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 4
section_title: Relations between tensor products and homomorphism modules
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 267-276, 396-398
pdf_pages: 0291-0300, 0420-0422
extraction: ocr
subsections:
    - "no": 1
      title: THE ISOMORPHISMS $\operatorname{Hom}_B(E \otimes_A F, G) \to \operatorname{Hom}_A(F, \operatorname{Hom}_B(E, G))$ AND $\operatorname{Hom}_c(E \otimes_A F, G) \to \operatorname{Hom}_A(E, \operatorname{Hom}_c(F, G))$
      page: 267
      pdf_page: 291
    - "no": 2
      title: THE HOMOMORPHISM** $E^* \otimes_A F \to \mathrm{Hom}_A(E, F)$
      page: 268
      pdf_page: 292
    - "no": 3
      title: TRACE OF AN ENDOMORPHISM
      page: 273
      pdf_page: 297
    - "no": 4
      title: THE HOMOMORPHISM $\operatorname{Hom}_c(E_1, F_1) \otimes_c \operatorname{Hom}_c(E_2, F_2) \to \operatorname{Hom}_c(E_1 \otimes_c E_2, F_1 \otimes_c F_2)$
      page: 274
      pdf_page: 298
statements: 15
exercises: 9
content_sha256: d7ad1bf03a98ac8771e4c2133d164adecd733b62e5f24f2ba584fd7cef6c7c71
translated_from: content/en/alg/II/04_s4_relations_between_tensor_products_and.md
translation_method: google
source_content_sha256: 426a0db21fa5ed22b6760dc79332adbd1c61d03bf2c3a4f077a67b035b99eabb
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 1aabfd97cdc0d75295047736cb0846f114c0911cdfbb7613ff380cc5244d9b93
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 4。 关系张量积和同态模之间

### 1. 同构 $\operatorname{Hom}_B(E \otimes_A F, G) \to \operatorname{Hom}_A(F, \operatorname{Hom}_B(E, G))$ 和 $\operatorname{Hom}_c(E \otimes_A F, G) \to \operatorname{Hom}_A(E, \operatorname{Hom}_c(F, G))$

设E为右A-模，F左A-模，G为$\mathbf{Z}$模，H为映射$f : E \times F \to G$的$\mathbf{Z}$模，它们是$\mathbf{Z}$双线性和满足

(1)
$$
f(x \lambda, y) = f(x, \lambda y) \quad \text{for } x \in E, y \in F, \lambda \in A.
$$

已经看出（§ 3, no. 1，命题 1）存在一个规范的$\mathbf{Z}$-模块同态

(2)
$$
H \to \operatorname{Hom}_{\mathbf{Z}}(E \otimes_A F, G).
$$

另一方面，$\operatorname{Hom}_{\mathbf{Z}}(E, G)$定义了左A-模结构，$\operatorname{Hom}_{\mathbf{Z}}(F, G)$（§ 3, no. 3）定义了右A-模结构；因此，我们可以考虑$\mathbf{Z}$模块$\operatorname{Hom}_A(E, \operatorname{Hom}_{\mathbf{Z}}(F, G))$和$\operatorname{Hom}_A(F, \operatorname{Hom}_{\mathbf{Z}}(E, G))$。 $E \times F$到G的映射$f$规范地等同于E到集合的映射到F到G的映射的$G^F$（*集合理论*，II, § 5, no. 2）；通过将后者映射属于表达为 $\operatorname{Hom}_A(E, \operatorname{Hom}_{\mathbf{Z}}(F, G))$，我们精确地得到$f$ 是双向可加的，条件 (1)； 从而还有典范同构

(3)
$$
H \to \operatorname{Hom}_A(E, \operatorname{Hom}_{\mathbf{Z}}(F, G))
$$
类似地也定义了典范同构

(4)
$$
H \to \operatorname{Hom}_A(F, \operatorname{Hom}_{\mathbf{Z}}(E, G)).
$$

现在假设 E 和 G 也有左（右）B-模结构，并且 E 上的 A-模和 B-模结构是兼容的。那么 $E \otimes_A F$ 典型地具有左（或右）B-模结构 (§ 3, no. 4)，而另一方面 $\operatorname{Hom}_B(E, G)$ 典型地具有左A-模结构 (§ 1, no. 14)。因此，我们可以考虑$\mathbf{Z}$-模块$\operatorname{Hom}_B(E \otimes_A F, G)$和$\operatorname{Hom}_A(F, \operatorname{Hom}_B(E, G))$，它们分别是$\operatorname{Hom}_{\mathbf{Z}}(E \otimes_A F, G)$和$\operatorname{Hom}_A(F, \operatorname{Hom}_{\mathbf{Z}}(E, G))$的子模（§ 2, no. 1，定理2）。我们分别考察条件、映射、$f \in H$在同构（2）和（4）$\operatorname{Hom}_B(E \otimes_A F, G)$的元素和$\operatorname{Hom}_A(E, \operatorname{Hom}_B(F, G))$的元素下分别有什么像；在这两种情况下，我们发现*相同* 条件

$$
f(\beta x, y) = \beta f(x, y)
$$
（分别$f(x \beta, y) = f(x, y) \beta$）

对于$x \in E, y \in F, \beta \in B$。

类似地，假设 F 和 G 是左（右）C 模块，并且 F 上的 A-模和 C 模块结构是兼容的。那么，要使映射$f \in H$分别具有$\mathrm{Hom}_C(E \otimes_A F, G)$或$\mathrm{Hom}_A(E, \mathrm{Hom}_C(F, G))$的(2)或(3)元素下的像，则满足与条件相同是充分必要的

$$
f(x, \gamma y) = \gamma f(x, y)
$$
（分别$f(x, y \gamma) = f(x, y) \gamma$）

对于$x \in E, y \in F, \gamma \in C$。

因此，我们得出以下结果（在上面介绍的记号中）：

#### 命题 1 {#alg-ii-s4-prop-1 .statement tag=05PP}

(a) *设 E 为 (B, A) 双模，F 左A-模且 G 左B-模。对于每个映射$g \in \mathrm{Hom}_B(E \otimes_A F, G)$，令$g'$是F的映射进入由$(g'(y))(x) = g(x \otimes y)$为$x \in E, y \in F$定义的$\mathrm{Hom}_B(E, G)$。 映射 $g \mapsto g'$ 是同构*

(5)
$$
\beta : \mathrm{Hom}_B(E \otimes_A F, G) \to \mathrm{Hom}_A(F, \mathrm{Hom}_B(E, G)).
$$

(b) *设 E 为右A-模，F 为 (A, C) 双模，G 为右 C 模。对于每个映射$h \in \mathrm{Hom}_C(E \otimes_A F, G)$，令$h'$是E的映射进入由$(h'(x))(y) = h(x \otimes y)$为$x \in E, y \in F$定义的$\mathrm{Hom}_C(F, G)$。 映射 $h \mapsto h'$ 是同构*

(6)
$$
\gamma : \mathrm{Hom}_C(E \otimes_A F, G) \to \mathrm{Hom}_A(E, \mathrm{Hom}_C(F, G)).
$$

特别地，B和C可以被认为是环A的中心中的子环$\Gamma$；那么对于每个 $\Gamma$-模块 G，三个 $\Gamma$-模块

$$
\mathrm{Hom}_\Gamma(E \otimes_A F, G), \quad \mathrm{Hom}_A(E, \mathrm{Hom}_\Gamma(F, G)), \quad \mathrm{Hom}_A(F, \mathrm{Hom}_\Gamma(E, G))
$$

与 $\Gamma$-*双线性* 映射的 $E \times F$ 的 $\Gamma$ 模规范同构到 G，其中满足 (1)。更具体地说：

#### 推论{#alg-ii-s4-n1-cor-1 .statement tag=05PQ}

*如果C为交换环且E、F、G为三个C模块，则C模块*
$$
\mathrm{Hom}_C(E \otimes_C F, G), \qquad \mathrm{Hom}_C(E, \mathrm{Hom}_C(F, G)),
$$
$$
\mathrm{Hom}_C(F, \mathrm{Hom}_C(E, G)), \qquad \mathscr{L}_2(E, F; G)
$$
*是规范同构的。*

### 2.同态**$E^* \otimes_A F \to \mathrm{Hom}_A(E, F)$

设 A、B 为两个环、E 左A-模、F 左B-模，G 为 (A, B)-*双模*。 $\mathbf{Z}$-模块 $\mathrm{Hom}_A(E, G)$ 具有规范的*右* B-*模* 结构 (§ 1, no. 14)，使得 $(u\beta)(x) = u(x)\beta$ 对应 $\beta \in B$、$u \in \mathrm{Hom}_A(E, G)$、$x \in E$。另一方面，$G \otimes_B F$ 典型地具有 *左A-模* 结构 (§ 3, no. 4)。我们将定义一个*典范的$\mathbf{Z}$同态*

$$
\nu : \mathrm{Hom}_A(E, G) \otimes_B F \to \mathrm{Hom}_A(E, G \otimes_B F).
$$

为此，我们考虑，对于所有$y \in F$和所有$u \in \mathrm{Hom}_A(E, G)$，将$E$的映射$\nu'(u, y) : x \mapsto u(x) \otimes y$放到$G \otimes_B F$上。立即验证$\nu'(u, y)$是$A$线性映射，并且$\nu'$是$\mathrm{Hom}_A(E, G) \times F$到$\mathrm{Hom}_A(E, G \otimes_B F)$的$\mathbf{Z}$双线性映射；此外，对于所有$\beta \in B$，$\nu'(u\beta, y)$和$\nu'(u, \beta y)$是相等的，对于$(u(x)\beta) \otimes y = u(x) \otimes (\beta y)$。我们结论 (§ 3, no. 1, 命题 1) 存在所需的同态$\nu$，使得$\nu(u \otimes y)$是$A$线性映射$x \mapsto u(x) \otimes y$。

立即验证，如果$E$是$(A, (C'_i); (D'_j))$-多模块，$F$是$(B, (C''_h); (D''_k))$-多模块并且$G$是$(A, (C'''_1); B, (D'''_m))$-多模块，则映射(7)是$((D'_j), (C''_h), (C'''_1); (C'_i), (D''_k), (D'''_m))$-多模块同态。

#### 命题 2 {#alg-ii-s4-prop-2 .statement tag=05PR}

(i) *当 $F$ 是射影*（分别是*有限生成射影*）*B-模，典范同态 (7) 是单射*（分别是*双射的*）。

(ii) *当 $E$ 是有限生成射影$A$-模时，典范同态 (7) 是双射*。

(i) 修复$E$和$G$，对于*每个*剩下的$B$-模块$F$，我们写

$$
T(F) = \mathrm{Hom}_A(E, G) \otimes_B F, \quad T'(F) = \mathrm{Hom}_A(E, G \otimes_B F);
$$

对于每个左边的$B$-模块同态$u : F \to F'$，我们写$T(u) = 1 \otimes u$（这里的1表示$\mathrm{Hom}_A(E, G)$的恒等映射），

$$
T'(u) = \mathrm{Hom}(1_E, 1_G \otimes u);
$$

另一方面，我们写 $\nu_F$ 而不是 $\nu$。那么我们有以下引理：

#### 引理 1 {#alg-ii-s4-lem-1 .statement tag=05PS}

*对于每个同态 $u : F \to F'$、图表*

$$
\begin{array}{ccc}
T(F) & \xrightarrow{\nu_F} & T'(F) \\
\downarrow T(u) & & \downarrow T'(u) \\
T(F') & \xrightarrow{\nu_{F'}} & T'(F')
\end{array}
$$

是*可交换的*。

验证为直接的。

#### 引理 2 {#alg-ii-s4-lem-2 .statement tag=05PT}

令$M, N$为$F$和$i : M \to F, j : N \to F$典范嵌入中的两个补子模。 图表

$$
\begin{array}{ccc}
T(M) \oplus T(N) & \xrightarrow{\nu_M \oplus \nu_N} & T'(M) \oplus T'(N) \\
\downarrow T(i) + T(j) & & \downarrow T'(i) + T'(j) \\
T(F) & \xrightarrow{\nu_F} & T'(F)
\end{array}
$$

是可交换的，垂直箭头是双射的。

交换律源自引理1，另一个断言源自§ 1, no. 6，推论2至命题6和§ 3, no. 7、命题7。

#### 引理 3 {#alg-ii-s4-lem-3 .statement tag=05PU}

在引理 2 的假设下，对于$\nu_F$ 是单射的（或满射的），$\nu_M$ 和$\nu_N$ 是单射的（或满射的）是必要且充分的。

这是从引理 2 和§ 1, no. 6，推论1 到命题 6 得出的。

那么引理 3 与§ 2, no. 2、命题 4 一起表明，只要考虑$F$ 是自由模的情况就足够了。但是，如果$(b_\mu)$是$F$的基，则$\mathrm{Hom}_A(E, G) \otimes_B F$的每个元素可以唯一地写为$\sum_\mu u_\mu \otimes b_\mu$，其中$u_\mu \in \mathrm{Hom}_A(E, G)$（§ 3, no. 7，推论1到命题7）；这个元素在$\nu$下的像就是$A$-线性映射$x \mapsto \sum_\mu u_\mu(x) \otimes b_\mu$；对于所有$x \in E$，不能为零，对于所有$x \in E$和所有$\mu$，除非$u_\mu(x) = 0$，相当于对于所有$\mu$，说即$u_\mu = 0$；因此 $\nu$ 是单射的。当$F$也承认有限的基时，引理3表明（通过$F$的基中元素的数上的归纳），要证明$\nu$是满射的，这样做就足够了当$F = B_s$时；但在这种情况下，(7) 的两侧被规范地标识为 $\mathrm{Hom}_A(E, G)$ (§ 3, no. 4, 命题 4)，并且 $\nu$ 成为恒等式。

(ii) 为了在 $E$ 是射影且有限生成时显示命题，这次我们修复 $F$ 和 $G$ 并写入，对于每个左 $A$-模块 $E$，

$$
T(E) = \mathrm{Hom}_A(E, G) \otimes_B F, \qquad T'(E) = \mathrm{Hom}_A(E, G \otimes_B F)
$$

并且，对于每个左$A$-模块同态$v : E \to E'$，

$$
T(v) = \mathrm{Hom}(v, 1_G) \otimes 1_F, \qquad T'(v) = \mathrm{Hom}(v, 1_G \otimes 1_F);
$$

另一方面，我们写 $\nu_E$ 而不是 $\nu$。然后我们有两个引理：

#### 引理 4 {#alg-ii-s4-lem-4 .statement tag=05PV}

对于每个同态 $v : E \to E'$、图表

$$
\begin{array}{ccc}
T(E') & \xrightarrow{\nu_{E'}} & T'(E') \\
\downarrow T(v) & & \downarrow T'(v) \\
T(E) & \xrightarrow{\nu_E} & T'(E)
\end{array}
$$

是可交换的。

#### 引理 5 {#alg-ii-s4-lem-5 .statement tag=05PW}

令$M$和$N$是$E$和$p : E \to M, q : E \to N$中的两个补子模，即规范的投影。 图表

$$
\begin{array}{ccc}
T(M) \oplus T(N) & \xrightarrow{\nu_M \oplus \nu_N} & T'(M) \oplus T'(N) \\
\downarrow T(p) + T(q) & & \downarrow T'(p) + T'(q) \\
T(E) & \xrightarrow{\nu_E} & T'(E)
\end{array}
$$

是可交换的，垂直箭头是双射的。

考虑到§ 1, no. 6、推论2至命题6、§ 2, no. 1、命题1和§ 3, no. 7、命题7，它们被证明为引理1和2。

然后证明的余数按照(i)进行，并减少到$E = A_s$的情况；然后，(7) 的两侧被规范地标识为 $G \otimes_B F$，并且 $\nu$ 成为恒等式。

特别是取$B = A$和$G$$(A, A)$-双模块${}_sA_d$（$§ 3$，no. 4），这样正确的$A$-模块$\mathrm{Hom}_A(E, {}_sA_d)$就是$E$和$({}_sA_d) \otimes_A F$的对偶$E^*$被规范地识别与 $F$ ($§ 3$, no. 4, 命题 4)。 同态 (7) 然后成为规范的 $\mathbf{Z}$ 同态

$$(11)$$
$$
\theta : E^* \otimes_A F \to \mathrm{Hom}_A(E, F)
$$
$\theta(x^* \otimes y)$ 是 $E$ 的线性映射变成 $F$
$$
x \mapsto \langle x, x^* \rangle y.
$$

注 (1)。 $§ 2$、no. 6、命题 12 中给出的*射影* $A$-模的刻画也可以表示如下：对于左$A$-模$E$射影，典范同态是充要的
$$
\theta_E : E^* \otimes_A E \to \mathrm{Hom}_A(E, E) = \mathrm{End}_A(E)
$$
使得$\theta_E$的$1_E$属于到像。

#### 推论 {#alg-ii-s4-n2-cor-1 .statement tag=05PX}

(i) *当 $F$ 是射影*（分别是*有限生成射影*）*模、典范同态* (11) *是单射*（分别是*双射的*）。
(ii) *当 $E$ 为有限生成射影模时，典范同态* (11) *是双射*。

即使$E$和$F$都是有限生成的，$\theta$也不一定是满射的，如例$A = \mathbf{Z}, E = F = \mathbf{Z}/2\mathbf{Z}$所示； (11) 的右侧非零但$E^* = 0$。另一方面，可以在 $E$ 是*自由*的情况下给出例，但 (11) 既不是单射也不是满射 (习题 3(b))。

当E承认有限的基$(e_i)$时，$\theta$的逆同构$\theta^{-1}$可以明确地找到如下。设$(e_i^*)$为$(e_i)$(§ 2, no. 6)中的对偶基；对于所有 $u \in \mathrm{Hom}(E, F)$ 以及所有 $x = \sum_i \xi_i e_i$ 和 $\xi_i \in A$，

$$
u(x) = \sum_i \xi_i u(e_i) = \sum_i \langle x, e_i^* \rangle u(e_i)
$$

因此$u = \sum_i \theta(e_i^* \otimes u(e_i))$，在其他字

$$
\theta^{-1}(u) = \sum_i e_i^* \otimes u(e_i).
$$

特别是，如果进一步$F = E$，可以看出恒等映射$1_E$的$\theta_E^{-1}$下的像是元素$\sum_i e_i^* \otimes e_i$，因此在E中考虑基$(e_i)$*独立*。

注另一方面，当E为有限生成射影模时，$\mathrm{End}_A(E)$上的*环* 结构可以通过$\theta_E^{-1}$传输到$E^* \otimes_A E$；立即验证，对于E中的$x, y$，$E^*$中的$x^*, y^*$，环$\mathrm{End}_A(E)$，

$$
\theta_E(x^* \otimes x) \circ \theta_E(y^* \otimes y) = \theta_E((y^* \langle y, x^* \rangle) \otimes x).
$$

*注* (2)。令 E 为*右* A-模； 替换 E 通过(11)中的$E^*$，我们得到一个规范的$\mathbf{Z}$同态

$$
E^{**} \otimes_A F \to \mathrm{Hom}_A(E^*, F).
$$

另一方面，存在规范的A-同态$c_E : E \to E^{**}$，从而，存在$\mathbf{Z}$-同态$c_E \otimes 1_F : E \otimes_A F \to E^{**} \otimes_A F$；将后者与同态 (14) 组合，我们因此获得规范的 $\mathbf{Z}$ 同态

$$
\theta' : E \otimes_A F \to \mathrm{Hom}_A(E^*, F)
$$

使得 $\theta'(x \otimes y)$ 为线性映射

$$
x^* \mapsto \langle x, x^* \rangle y.
$$

如果 E *和* F 是*射影* 模，则映射 (15) 是*内射*。因为 $c_E$ 是单射的（§ 2, no. 7，推论 4 到命题 13），并且由于 F 是射影，$\mathbf{Z}$ 同态 $c_E \otimes 1_F : E \otimes_A F \to E^{**} \otimes_A F$ 也是单射的（§ 3, no. 7，推论 6 到命题 7）；最后可知(命题2)同态(14)是单射的，从而结论。

如果 E 是*射影*且*有限生成*，则映射 (15) 是*双射的*，因为它所组成的两个映射则为双射（§ 2, no. 7，推论 4 到上面的命题 13 和命题 2）。

### 3. 自同态的踪迹

令 $C$ 为*可交换* 环，而 $E$ 为 $C$ 模。 $E^* \times E$到$C$的映射$(x^*, x) \mapsto \langle x, x^* \rangle$则为$C$*-双线性*，因为对于所有$\gamma \in C$、$\langle \gamma x, x^* \rangle = \gamma \langle x, x^* \rangle$和$\langle x, x^* \gamma \rangle = \langle x, x^* \rangle \gamma$；我们推导出一个规范的 $C$*-线性* 映射

$$
\tau : E^* \otimes_C E \to C
$$

这样 $\tau(x^* \otimes x) = \langle x, x^* \rangle$ (§ 3, no. 5)。现在还假设 $E$ 是一个*有限生成的射影* $C$ 模； no. 2的典范同构 (11) 是一个$C$*-模块* 同构，因此我们可以通过在$C$-模块上传输结构*规范线性形式* $\mathrm{Tr} = \tau \circ \theta_E^{-1}$来实现定义 $\mathrm{End}_C(E)$。对于所有$u \in \mathrm{End}_C(E)$，标量$\mathrm{Tr}(u)$称为自同态$u$的*迹*；每个$u \in \mathrm{End}_C(E)$都可以写成形式$x \mapsto \sum_i \langle x, x_i^* \rangle y_i$，其中$x_i^* \in E^*$和$y_i \in E_i$凭借no. 2，命题2的推论；然后

$$
\mathrm{Tr}(u) = \sum_i \langle y_i, x_i^* \rangle \quad \text{(cf. § 10, no. 11).}
$$

定义，

$$
\mathrm{Tr}(u + v) = \mathrm{Tr}(u) + \mathrm{Tr}(v)
$$
$$
\mathrm{Tr}(\gamma u) = \gamma \mathrm{Tr}(u)
$$

对于 $\mathrm{End}_C(E)$ 和 $\gamma \in C$ 中的 $u, v$。此外：

#### 命题 3 {#alg-ii-s4-prop-3 .statement tag=05PY}

*令$C$为交换环、$E, F$两个有限生成的射影$C$*-模块*以及$u : E \to F$和$v : F \to E$两个线性映射；那么*

$$
\mathrm{Tr}(v \circ u) = \mathrm{Tr}(u \circ v).
$$

两个映射$(u, v) \mapsto \mathrm{Tr}(u \circ v), (u, v) \mapsto \mathrm{Tr}(v \circ u)$

$$
\mathrm{Hom}_C(E, F) \times \mathrm{Hom}_C(F, E)
$$

到$C$是$C$*-双线性*；因此，当$u$为形式$x \mapsto \langle x, a^* \rangle b$且$v$为形式$y \mapsto \langle y, b^* \rangle a$且$a \in E, a^* \in E^*, b \in F, b^* \in F^*$时，足以验证(20)。但$v \circ u$是映射$x \mapsto \langle x, a^* \rangle \langle b, b^* \rangle a$和$u \circ v$映射$y \mapsto \langle y, b^* \rangle \langle a, a^* \rangle b$。 公式 (17) 表明(20) 两侧的值等于$\langle a, a^* \rangle \langle b, b^* \rangle$。

#### 推论 {#alg-ii-s4-n3-cor-1 .statement tag=05PZ}

*如果$u_1, \ldots, u_p$是$E$中的自同态，那么*

$$
\mathrm{Tr}(u_1 \circ u_2 \circ \cdots \circ u_p) = \mathrm{Tr}(u_i \circ u_{i+1} \circ \cdots \circ u_p \circ u_1 \circ \cdots \circ u_{i-1})
$$

*for* $1 \leq i \leq p$（“循环置换下轨迹的不变性”）。

将 (20) 应用于乘积即可

$$(u_1 \circ u_2 \circ \cdots \circ u_{i-1}) \circ (u_i \circ u_{i+1} \circ \cdots \circ u_p).$$

注另一方面，这不一定是真的

$$\operatorname{Tr}(u \circ v \circ w) = \operatorname{Tr}(u \circ w \circ v)$$

三个自同态 $u, v, w$ E。

### 4.同态$\operatorname{Hom}_c(E_1, F_1) \otimes_c \operatorname{Hom}_c(E_2, F_2) \to \operatorname{Hom}_c(E_1 \otimes_c E_2, F_1 \otimes_c F_2)$

设C是一个*可交换的*环和$E_1, E_2, F_1, F_2$四个C模块；在 § 3, no. 5, 公式 (13) 中，我们定义了一个规范的 C-模块同态

（21）$\lambda : \operatorname{Hom}(E_1, F_1) \otimes \operatorname{Hom}(E_2, F_2) \to \operatorname{Hom}(E_1 \otimes E_2, F_1 \otimes F_2)$。

#### 命题 4 {#alg-ii-s4-prop-4 .statement tag=05Q0}

*当有序对* $(E_1, E_2), (E_1, F_1), (E_2, F_2)$ *之一由有限生成的射影C模组成时，典范同态* (21) *是双射的。*

显然，对于有序对$(E_1, F_1)$和$(E_1, E_2)$执行证明就足够了。

我们首先考虑有序对$(E_1, F_1)$的情况；我们修复$E_2, F_1, F_2$并为*每个*C-模块$T(E) = \operatorname{Hom}(E, F_1) \otimes_c \operatorname{Hom}(E_2, F_2)$和$T'(E) = \operatorname{Hom}(E \otimes E_2, F_1 \otimes F_2)$编写，并且对于每个C-同态$v : E \to E'$，

$$T(v) = \operatorname{Hom}(v, 1_{F_1}) \otimes 1_{\operatorname{Hom}(E_2, F_2)}$$

和

$$T'(v) = \operatorname{Hom}(v \otimes 1_{E_2}, 1_{F_1 \otimes F_2}).$$

那么*引理 4 和 5* (no. 2)（*其中 v* 被 $\lambda$ 代替）*有效*并且由完全类似的方法证明。

接下来我们修复$E_2$和$F_2$，这次为每个C-模块F写入，

$$T(F) = \operatorname{Hom}(C, F) \otimes_c \operatorname{Hom}(E_2, F_2)$$ 和 $T'(F) = \operatorname{Hom}(C \otimes E_2, F \otimes F_2)$，并且对于每个 C 同态 $u : F \to F'$，

$$T(u) = \operatorname{Hom}(1_C, u) \otimes 1_{\operatorname{Hom}(E_2, F_2)}$$

和

$$T'(u) = \operatorname{Hom}(1_C \otimes 1_{E_2}, u \otimes 1_{F_2}).$$

这次立即验证*引理 1 和 2* (no. 2)（*其中$\lambda$始终替换 v*）*有效*。

既然如此，当$E_1 = C$和$F_1$是射影且有限生成时，我们首先显示命题。 no. 2的参数（基于引理 1和2），与上面的注、约化一起到证明命题，当也$F_1 = C$时；那么$\operatorname{Hom}(E_1, F_1), E_1 \otimes E_2$和$F_1 \otimes F_2$分别用C，$E_2$和$F_2$来识别（§ 3, no. 4，命题4）； (21) 的两侧

同态$\operatorname{Hom}_c(E_1, F_1) \otimes_c \operatorname{Hom}(E_2, F_2)$

然后都用$\operatorname{Hom}(E_2, F_2)$和之后这些标识进行规范标识，经验证$\lambda$成为身份。

我们现在假设 $F_1$ 是射影且有限生成的； no. 2（此时取决于引理 4和5）约化证明对于$E_1$任何有限生成射影模到$E_1 = C$的情况，即处理的第一个情况。

对于有序对$(E_1, E_2)$，过程类似，这次应用引理4和5两次；我们把细节留给读者。

注当 $E_1 = C^{(I)}$、$E_2 = C^{(J)}$ 自由时（无论是否有限生成），则 $\operatorname{Hom}(E_1, F_1) = F_1^I$、$\operatorname{Hom}(E_2, F_2 = F_2^J$ 和
$$
\operatorname{Hom}(E_1 \otimes E_2, F_1 \otimes F_2) = (F_1 \otimes F_2)^{I \times J}
$$
到典范同构和 (21) 之内，则与 § 3, no. 7 的典范同态 (22) 的特殊情况相同。

当 $E_2 = C$, 典范同态 (21) 给出时，之后将 $\operatorname{Hom}(E_2, F_2)$ 与 $F_2$ 识别，将 $E_1 \otimes E_2$ 与 $E_1$, 典范同态识别
$$
\operatorname{Hom}(E, F) \otimes G \to \operatorname{Hom}(E, F \otimes G)
$$
对于任何三个$C$-模块$E, F, G$，这只是$A = B = C$的no. 2的同态(7)。

注当 $F = C$ 典范同态 (22) 再次给出 (11) (no. 2) 对于交换环的情况。

现在假设$F_1 = F_2 = C$；由于$F_1 \otimes F_2$与$C$等同，所以有这次典范同态
$$
\mu : E^* \otimes F^* \to (E \otimes F)^*
$$
对于两个$C$-模块$E, F$；对于$x^* \in E^*, y^* \in F^*$，$x^* \otimes y^*$在典范同态（23）下的像是线性形式$u$在$E \otimes F$上，这样
$$
u(x \otimes y) = \langle x, x^* \rangle \langle y, y^* \rangle.
$$
此外，如果$E_1, E_2, F_1, F_2$是四个$C$模块，$f : E_1 \to E_2, g : F_1 \to F_2$是两个线性映射，则从(24)可以立即得出图表
$$
\begin{array}{ccc}
E_2^* \otimes F_2^* & \xrightarrow{\mu} & (E_2 \otimes F_2)^* \\
t_f \otimes t_g \downarrow & & \downarrow t_{(f \otimes g)} \\
E_1^* \otimes F_1^* & \xrightarrow{\mu} & (E_1 \otimes F_1)^*
\end{array}
$$
是*可交换的*。

#### 推论 1 {#alg-ii-s4-prop-4-cor-1 .statement tag=05Q1}

*如果模 E, F 之一是射影且有限生成的，则典范同态 (23) 是双射的。*

#### 推论 2 {#alg-ii-s4-prop-4-cor-2 .statement tag=05Q2}

*设E₁、E2为两个有限生成的射影C模，E₁的u₁自同态和E2的u2自同态；那么*

$$
\text{Tr}(u_1 \otimes u_2) = \text{Tr}(u_1)\text{Tr}(u_2).
$$

根据线性，只需考虑 u₁ 为形式 $x_1 \mapsto \langle x_1, x_1^* \rangle y_1$ 且 u2 为形式 $x_2 \mapsto \langle x_2, x_2^* \rangle y_2$ 的情况即可；那么$u_1 \otimes u_2$下$x_1 \otimes x_2$的像除以定义

$$
\langle x_1, x_1^* \rangle \langle x_2, x_2^* \rangle (y_1 \otimes y_2) = \langle x_1 \otimes x_2, x_1^* \otimes x_2^* \rangle (y_1 \otimes y_2)
$$

$x_1^* \otimes x_2^*$ 被规范地标识为 $\mu$，元素为 $(E_1 \otimes E_2)^*$。由于 $\langle y_1 \otimes y_2, x_1^* \otimes x_2^* \rangle = \langle y_1, x_1^* \rangle \langle y_2, x_2^* \rangle$，公式 (26) 在这种情况下由 (17) 得出。

#### 注 {#alg-ii-s4-n4-rem-1 .statement tag=05Q3}

如果E、F、G是任意三个C模，则立即验证图表

$$
\begin{array}{ccc}
E^* \otimes F^* \otimes G^* & \xrightarrow{\mu \otimes 1} & (E \otimes F)^* \otimes G^* \\
1 \otimes \mu \downarrow & & \downarrow \mu \\
E^* \otimes (F \otimes G)^* & \xrightarrow{\mu} & (E \otimes F \otimes G)^*
\end{array}
$$

凭借公式 (24) 是*可交换的*。

我们注还指出，在C-模块E、F上没有任何假设，有规范的*同构*

(28) $$(E \otimes F)^* \to \text{Hom}(E, F^*)$$
(29) $$(E \otimes F)^* \to \text{Hom}(F, E^*)$$

对于 G = C，A = B = C，这只是 no. 1 的同构 (6) 和 (5)。

因此，在 E × F 上的 *双线性形式*、E 到 F* 的 *同态和 F 到 E* 的 *同态之间定义了规范的一对一对应：如果 u（或 v）是 E 到 F* 的同态（或 F 到 E* 的相应的），相应的双线性形式由下式给出

$$(x, y) \mapsto \langle y, u(x) \rangle \quad (\text{resp. } (x, y) \mapsto \langle x, v(y) \rangle).$$

### 习题{#alg-ii-s4-exercises}

§ 4](exercises/s4/)参见[习题。
