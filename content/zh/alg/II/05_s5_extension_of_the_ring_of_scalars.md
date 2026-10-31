---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 5
section_title: Extension of the ring of scalars
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 277-284, 398-399
pdf_pages: 0301-0308, 0422-0423
extraction: ocr
subsections:
    - "no": 1
      title: EXTENSION OF THE RING OF SCALARS OF A MODULE
      page: 277
      pdf_page: 301
    - "no": 2
      title: RELATIONS BETWEEN RESTRICTION AND EXTENSION OF THE RING OF SCALARS
      page: 280
      pdf_page: 304
    - "no": 3
      title: EXTENSION OF THE RING OF OPERATORS OF A HOMOMORPHISM MODULE
      page: 282
      pdf_page: 306
    - "no": 4
      title: DUAL OF A MODULE OBTAINED BY EXTENSION OF SCALARS
      page: 283
      pdf_page: 307
    - "no": 5
      title: A CRITERION FOR FINITENESS
      page: 284
      pdf_page: 308
statements: 13
exercises: 7
content_sha256: 61588f7f521e0d845856e4423b043ab47381a23fe4368e339359564441287e5b
translated_from: content/en/alg/II/05_s5_extension_of_the_ring_of_scalars.md
translation_method: google
source_content_sha256: 77418857e92cac7b8d57a775fbe6a401b2e7ca09da87ea0dd014ebf83b887e38
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: 74c3527833fd50da04d044511b2c33f55246c1eeb31132caa20fb7c8c6365b20
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 5。标量的环的扩张

### 1. 模标量中的环的扩张

设$A, B$为两个环和$\rho : A \to B$环同态；我们考虑由这个同态（$§ 1$，no. 13）定义的正确$A$模块$\rho^*(B_d)$；这个$A$模块也有一个左$B$模块结构，即$B_s$的结构，并且，正如$B$中$a \in A, b, b'$的$b'(b\rho(a)) = (b'b)\rho(a)$一样，$B$上的这两个模结构是兼容的（$§ 1$，no. 14）。这允许我们，对于每个左$A$-模块$E$，到定义张量积$\rho_*(B_d) \otimes_A E$上的左$B$-模块结构，使得$B$和$x \in E$中的$\beta, \beta'$有$\beta'(\beta \otimes x) = (\beta'\beta) \otimes x$ （$§ 3$，no. 3）。这个左$B$模块据说是通过$\rho$*将标量的环扩展到$B$*从$E$派生出来的，如果不引起混淆的话，它用$\rho^*(E)$或$E_{(B)}$表示。

#### 命题 1 {#alg-ii-s5-prop-1 .statement tag=05QD}

*对于$E$的每个左$A$-模块$E$、映射$\phi : x \mapsto 1 \otimes x$进入$A$-模块$\rho_*(\rho^*(E))$是$A$线性且集合$\phi(E)$生成 $B$-模块$\rho^*(E)$。此外，对于$E$到$A$-模块$\rho_*(F)$的每个左$B$-模块$F$和每个$A$-线性映射$f$，存在且仅有一个$B$-线性映射$\bar{f}$ $\rho^*(E)$ 转换为 $F$，这样 $\bar{f}(1 \otimes x) = f(x)$ 对于所有 $x \in E$。*

$B$可以通过$\rho$被视为$(B, A)$双模；那么有一个规范的 $\mathbf{Z}$-模块同构

(1)
$$
\operatorname{Hom}_B(B \otimes_A E, F) \to \operatorname{Hom}_A(E, \operatorname{Hom}_B(B_s, F))
$$
正如在 $§ 4$、no. 1、命题 1 中所见。但是左侧 $A$ 模块 $\operatorname{Hom}_B(B_s, F)$ 被规范地标识为 $\rho^*(F)$：对于，通过定义 ($§ 1$，no. 14)，有对应到元素$y \in F$同态$\theta(y) : B_s \to F$使得$(\theta(y))(1) = y$；对于所有$\lambda \in A$，因此$B_s$的对应到$\rho(\lambda)y \in F$同态$\mu \mapsto \mu \rho(\lambda)y$进入$F$，这只是$\operatorname{Hom}_B(B_s, F)$上左侧$A$模块结构的$\lambda \theta(y)$ （$§ 1$，no. 14）。使用此识别，我们获得*规范* $\mathbf{Z}$-模块*同构*，（1）的逆

(2)
$$
\delta : \operatorname{Hom}_A(E, \rho_*(F)) \to \operatorname{Hom}_B(\rho^*(E), F)
$$
从定义可以立即得出，如果 $\delta(f) = \bar{f}$，则对于所有 $x \in E$ 来说，$\bar{f}(1 \otimes x) = f(x)$。特别是，映射$\phi_E : x \mapsto 1 \otimes x$只是
(3)
$$
\phi_E = \delta^{-1}(1_{\rho^*(E)}).
$$

因此命题1得证。 映射 $\phi_E : E \to \rho_*(\rho^*(E))$ 被称为*规范*。

#### 注 {#alg-ii-s5-n1-rem-1 .statement tag=05QE}

(1) 命题 1 表明$E_{(B)}$和$\phi_E$的有序对由……组成是普遍映射问题的解（集合理论，IV, § 3, no. 1），其中$\Sigma$是左B-模结构的类（态射是B-线性映射），$\alpha$映射是E到B-模的A-线性映射。

(2) 如果 E 是$(A, (C'_i); (D'_j))$-多模且 F 是$(B, (C''_h); (D''_k))$-多模，则同构 (2) 相对于两侧（$§ 1$、no. 14 和 $§ 3$、no. 4）的 $((D'_j, (C''_h); (C'_i), (D''_k))$-多模结构是线性的。

(3) 设E为左A-模，$a$A的双面理想和$\rho : A \to A/a$典范同态。在$§ 3$、no. 6的记号中，推论2到命题6，A-模$E/aE$被$a$湮灭，因此具有规范的左$(A/a)$模块结构（$§ 1$， no. 12); $§ 3$、no. 6中定义的典范映射$\pi : \rho^*(E) \to E/aE$是直接的，对于$(A/a)$模块结构，推论2到命题6是同构。

#### 推论{#alg-ii-s5-n1-cor-1 .statement tag=05QF}

*设E、E'为二左A-模；对于每个A-线性映射$u : E \to E'$，$v = l_B \otimes u$是唯一的B-线性映射，它呈现可交换的图表*

$$
\begin{array}{ccc}
E & \xrightarrow{\phi_E} & E_{(B)} \\
| & & | \\
u \downarrow & & v \downarrow \\
E' & \xrightarrow{\phi_{E'}} & E'_{(B)}
\end{array}
$$

*其中$\phi_E$和$\phi_{E'}$是典范映射。*

应用命题 1 足以满足 A 同态$\phi_{E'} \circ u : E \to E'_{(B)}$。

上述推论中定义的映射$v$用$\rho^*(u)$或$u_{(B)}$表示。

如果$E''$是第三个左A-模且$v : E' \to E''$A-线性映射，则直接的

$$
(v \circ u)_{(B)} = v_{(B)} \circ u_{(B)}.
$$

扩展模运算符的环是*传递* 运算；准确地说：

#### 命题 2 {#alg-ii-s5-prop-2 .statement tag=05QG}

*令$\rho : A \to B,\ \sigma : B \to C$为环同态。对于每一个左A-模 E，存在且仅有一个 C 同态*

$$(4)$$
$$
\sigma^*(\rho^*(E)) \to (\sigma \circ \rho)^*(E)
$$
*对于所有$x \in E$，映射$1 \otimes (1 \otimes x)$到$1 \otimes x$，并且这个同态是双射的。*

$\sigma^*(\rho^*(E))$和$(\sigma \circ \rho)^*(E)$的底层$\mathbf{Z}$模块分别是$C \otimes_B (B \otimes_A E)$和$C \otimes_A E$。存在一个规范的$\mathbf{Z}$同构$C \otimes_B (B \otimes_A E) \to (C \otimes_B B) \otimes_A E$（$§ 3$，no. 8，命题8），这也是左侧C-模结构两侧的C同构。此外，

C-模 $C \otimes_B B$ 在同构下被规范地标识为 C-模 $C_s$，其中映射 $\gamma \otimes \beta$ 到 $\gamma \sigma(\beta)$（§ 3, no. 4、命题 4），并且这个同构也是同构对于$\rho$定义的$C \otimes_B B$上的右A-模结构和$\sigma \circ \rho$定义的C上的右A-模结构。于是典范同构

$$
(C \otimes_B B) \otimes_A E \to C \otimes_A E
$$

得到，并与同构组合

$$
C \otimes_B (B \otimes_A E) \to (C \otimes_B B) \otimes_A E
$$

之前定义，就获得了所需的典范同构。

如果$\phi, \phi'$和$\phi''$分别表示典范映射、$E \to \rho^*(E), \rho^*(E \to) \sigma^*(\rho^*(E))$和$E \to (\sigma \circ \rho)^*(E)$，则$\phi' \circ \phi$与命题2的典范同构下的$\phi''$进行识别。

#### 命题 3 {#alg-ii-s5-prop-3 .statement tag=05QH}

*设A、B为两个交换环、$\rho : A \to B$环同态，E、E'为两个A-模。存在且仅有一个 B 同态*

$$
E_{(B)} \otimes_B E'_{(B)} \to (E \otimes_A E')_{(B)}
$$

*映射* $(1 \otimes x) \otimes (1 \otimes x')$ *到* $1 \otimes (x \otimes x')$ *为* $x \in E, x' \in E'$，*这个同态是双射*。

(5) 的左边可以写成 $(B \otimes_A E) \otimes_B (B \otimes_A E')$ 并用 $(E \otimes_A B) \otimes_B (B \otimes_A E')$ 来表示，因为 A 和 B 是可交换的；后者乘积依次用$E \otimes_A (B \otimes_B B) \otimes_A E'$、$E \otimes_A (B \otimes_A E')$、$E \otimes_A (E' \otimes_A B)$和$(E \otimes_A E') \otimes_A B$，使用张量积的结合性（§ 3, no. 8，命题8），命题4，§ 3, no. 4，和A 和 B 的交换律。所需的同构是连续典范同构的合成。

显然，如果S是E的生成的系统，则典范映射$E \to E_{(B)}$下S的像是$E_{(B)}$的生成的系统；特别是，如果 E 为有限生成A-模，则 $E_{(B)}$ 是有限生成的 B-模。

#### 命题 4 {#alg-ii-s5-prop-4 .statement tag=05QI}

*设E为A-模，承认基* $(a_\lambda)_{\lambda \in L}$； *如果*$\phi : x \mapsto 1 \otimes x$*是E的典范映射到*$\rho^*(E)$，*那么*$(\phi(a_\lambda))_{\lambda \in L}$*是*$\rho^*(E)$的基。 *如果* $\rho$ *是单射的，那么* $\phi$ 也是单射的。

第一个断言紧随§ 3, no. 7，推论1到命题7。此外，对于有限支撑A的元素的每个家庭$(\xi_\lambda)_{\lambda \in L}$，

$$
\phi \left( \sum_{\lambda \in L} \xi_\lambda a_\lambda \right) = \sum_{\lambda \in L} \rho(\xi_\lambda) \phi(a_\lambda)
$$

因此，对于所有 $\lambda \in L$，关系 $\phi \left( \sum_{\lambda \in L} \xi_\lambda a_\lambda \right) = 0$ 等价于 $\rho(\xi_\lambda) = 0$，从而第二个断言。

#### 推论{#alg-ii-s5-n1-cor-2 .statement tag=05QJ}

*对于每个射影 A-模 E，B-模* $\rho^*(E)$ *都是射影。如果进一步* $\rho$ *是单射的，则 E 的典范映射到* $\rho^*(E)$ *是单射的。*

到假设时，存在自由A-模 M 包含 E，并且其中 E 承认补充 F。 紧接着从§ 3, no. 7、命题 7 可以得出$M_{(B)}$ 与$E_{(B)}$ 和$F_{(B)}$ 的直和相同，并且如果$\phi$和$\psi$是典范映射$E \to E_{(B)}$和$F \to F_{(B)}$，典范映射$M \to M_{(B)}$只是$x + y \mapsto \phi(x) + \psi(y)$。将命题 4 应用于 A-模 M 立即得出推论。

当 E 为右A-模时，我们类似地写为 $\rho^*(E) = E \otimes_A \rho_*(B_s)$，这次将 B 视为 (A, B) 双模，并且 $\rho^*(E)$ 上的右B-模结构使得 $\beta \in B' \ \beta' \in B$ 和 $x \in E$ 为 $(x \otimes \beta)\beta' = x \otimes (\beta\beta')$。我们留给读者的任务是，将右模的结果相应的说明为这一数字的结果。以及以下内容。

注 (4)。考虑由 $\rho$ 定义的左A-模 $\rho_*(B_s)$，对于每个左A-模 E，考虑 $\mathbf{Z}$ 模
$$
\tilde{\rho}(E) = \operatorname{Hom}_A(\rho_*(B_s), E).
$$
由于$\rho_*(B_s)$有右B-模结构，左B-模结构是在$\tilde{\rho}(E)$（§ 1, no. 14）上导出的，因此，如果$u \in \tilde{\rho}(E)$和$b' \in B$，则$b'u$是同态$b \mapsto u(bb')$ $\rho_*(B_s)$ 进入 E。我们进一步定义 A-线性映射，称为规范
$$
\eta : \rho_*(\tilde{\rho}(E)) \to E
$$
与 E 中的每个同态 $u \in \tilde{\rho}(E)$ 元素 $u(1)$ 相关联。由于 B 可以通过 $\rho$ 被视为 (A, B)-双模，因此对于每个左B-模 F，都有一个规范的 $\mathbf{Z}$-模同构
$$
\operatorname{Hom}_A(\rho_*(B_s) \otimes_B F, E) \to \operatorname{Hom}_B(F, \operatorname{Hom}_A(\rho_*(B_s), E))
$$
（§ 1, no. 1，命题1）。由于左A-模 $\rho^*(B_s) \otimes_B F$ 凭借 § 3, no. 4、命题 4 被规范地识别为 $\rho_*(F)$，因此我们获得规范的 $\mathbf{Z}$-模同构，即上述的逆
$$
\operatorname{Hom}_B(F, \tilde{\rho}(E)) \to \operatorname{Hom}_A(\rho_*(F), E)
$$
将 F 的每 B-线性映射 g 关联到 $\tilde{\rho}(E)$ 复合映射 $\eta \circ g$，被视为 $\rho_*(F)$ 的 A-线性映射关联到 E。特别是，在命题 2 的假设下，如果 F 被 $\sigma_*(C_s)$ 替换，我们得到一个规范C-同构
$$
\tilde{\sigma}(\tilde{\rho}(E)) \to (\sigma \circ \rho)^*(E).
$$

### 2. 标量的环的限制和扩张之间的关系

设$\rho : A \to B$为环同态。对于每个左A-模 E，一个规范的 A-线性映射
$$
\phi_E : E \to \rho_*(\rho^*(E))
$$
在no. 1中定义，使得$\phi_E(x) = 1 \otimes x$。现在我们考虑左B-模 F 和应用命题 1 (no. 1) 到同态 $l_{\rho_*(F)} : \rho_*(F) \to \rho_*(F)$：我们得到 B-线性映射

$$
\psi_F : \rho^*(\rho_*(F)) \to F
$$

等于 $\delta(l_{\rho_*(F)})$ 因此，对于所有 $y \in F$ 和所有 $\beta \in B$，
$\psi_F(\beta \otimes y) = \beta y$。

#### 命题 5 {#alg-ii-s5-prop-5 .statement tag=05QK}

*设E为左A-模，F为左B-模；复合映射*

$$
\rho^*(E) \xrightarrow{\rho^*(\phi_E)} \rho^*(\rho_*(\rho^*(E))) \xrightarrow{\psi_{\rho^*(E)}} \rho^*(E)
$$
$$
\rho_*(E) \xrightarrow{\phi_{\rho_*(F)}} \rho_*(\rho^*(\rho_*(F))) \xrightarrow{\rho_*(\psi_F)} \rho_*(F)
$$

*分别等于$\rho^*(E)$和$\rho_*(F)$的恒等映射。*

我们给出证明，对于例，对于(12)；对于所有 $x \in E$、映射 $\rho^*(\phi_E)$ 映射 $1 \otimes x$ 至元素 $1 \otimes (1 \otimes x)$ 和映射 $\psi_{\rho^*(E)}$ 映射 $1 \otimes (1 \otimes x)$ 至元素 $1 \otimes x$；结论是根据形式$1 \otimes x$生成B-模$\rho^*(E)$的元素得出；对于 (13) 来说证明更简单。

#### 推论 {#alg-ii-s5-n2-cor-1 .statement tag=05QL}

*映射 $\rho^*(\phi_E)$ 和 $\phi_{\rho_*(F)}^*$ 是单射，分别是认同 $\rho^*(E)$ 与直因子的 $\rho^*(\rho_*(\rho^*(E)))$ 和 $\rho_*(F)$ 与直因子的 $\rho_*(\rho^*(\rho_*(F)))$。*

这是命题 5 和 § 1, no. 9 的推论，推论 2 到命题 15。

#### 命题 6 {#alg-ii-s5-prop-6 .statement tag=05QM}

*设 E 为左A-模，F 右B-模。存在且仅有一个$\mathbf{Z}$-同态*

$$
\rho_*(F) \otimes_A E \to F \otimes_B \rho^*(E)
$$

*对于所有$x \in E$和所有$y \in F$，映射$y \otimes x$到$y \otimes (1 \otimes x)$，并且这个同态是双射的。*

通过定义，(14)的右侧是$F \otimes_B (B \otimes_A E)$，其中B被视为(B,A)-双模，并且在§ 3, no. 8、命题8中定义了规范的$\mathbf{Z}$同构$(F \otimes_B B) \otimes_A E \to F \otimes_B (B \otimes_A E)$；另一方面，§ 3, no. 4、命题 4 的典范同构$F \to F \otimes_B B$，对于两侧的右A-模结构来说，是同构，由$\rho$定义。 从而所需的同构。

当 A 和 B *可交换*时，同构 (14) 是 *A-模* 同构

$$
\rho_*(F) \otimes_A E \to \rho_*(F \otimes_B \rho^*(E)).
$$

### 3. 同态模运营商的环中的扩张

令 $A$ 为*可交换* 环、$B$ 环、$\rho : A \to B$ 环同态和 $E, F$ 两个 $A$ 模块；由于$B$是一个$(A, A)$双模（通过$\rho$）并且$F$可以被认为是一个$(A, A)$-双模，因此在$\mathbf{Z}$-模块上有$B \otimes_A F$*两个*$A$-模块结构，其下分别$a(b \otimes y) = (\rho(a)b) \otimes y$ 和 $a(b \otimes y) = b \otimes (ay)$ 对应 $a \in A,\ b \in B,\ y \in F$。我们将用$G'$和$G''$来表示这样定义的两个$A$模块；而且$G'$只是$A$模块$\rho_*(\rho^*(F))$。

既然如此，在§ 4, no. 2、公式的典范同态的定义、公式(7)中，我们将$A$的替换$B$、环$B$的$B$模$F$视为$A$-模通过$\rho$和$G$通过$F$视为$(A, A)$双模；由于 $A$ 是可交换的，我们可以将获得的*规范* $\mathbf{Z}$*-同态* 写为

$$
(15) \quad B \otimes_A \operatorname{Hom}_A(E, F) \to \operatorname{Hom}_A(E, G'').
$$

另一方面 (no. 1, 公式 (2))，有一个*规范* $\mathbf{Z}$*-同构*

$$
(16) \quad \operatorname{Hom}_A(E, G') = \operatorname{Hom}_A(E, \rho_*(\rho^*(F))) \to \operatorname{Hom}_B(\rho^*(E), \rho^*(F)).
$$

现在假设$\rho(A)$包含在$B$的*中心*中，在这种情况下，$\rho$也被称为*中心*同态*（或者$\rho$被称为定义一个$A$*-代数*结构） $B$、cf.III, § 1, no. 3)*。那么$G'$和$G''$的$A$模结构是*相同的*并且组合同态(16)和(15)，我们因此得到一个规范的$\mathbf{Z}$*-同态*

$$
(17) \quad \omega : B \otimes_A \operatorname{Hom}_A(E, F) \to \operatorname{Hom}_B(E_{(B)}, F_{(B)})
$$

其特点是，对于所有 $u \in \operatorname{Hom}_A(E, F)$ 和所有 $b \in B$

$$
(18) \quad \omega(b \otimes u) = r_b \otimes u,
$$

其中$r_b$表示$B$中右乘法乘以$b$。

此外，$\omega$是*中心*同态的假设意味着$(bb')\rho(a) = b\rho(a))b'$对于$B$和$a \in A$中的$b,\ b'$；在其他字中，$B_d$的*正确*$B$模块结构与其$A$模块结构*相容的；因此，$B \otimes_A \operatorname{Hom}_A(E, F)$上的定义*右*$B$*-模块*结构（§ 3, no. 4）以及$F_{(B)} = B \otimes_A F$上，最后，由于$F_{(B)}$上的左和右$B$-模块结构*相容的*，所以*右* $B$*-模块* 结构也在 $\operatorname{Hom}_B(E_{(B)}, F_{(B)})$ (§ 1, no. 14) 上获得。然后立即验证（17）是这些结构的*正确*$B$*-模块*同态*。

#### 命题 7 {#alg-ii-s5-prop-7 .statement tag=05QN}

*令$A$为交换环、$B$环、$\rho : A \to B$一个中央同态和$E, F$两个$A$模块。*

(i) *如果 B 是射影*（分别是*有限生成射影*）*A*-模，同态 (17) 是单射*（分别是*双射的*）。

(ii) *如果 E 是有限生成的射影 A* 模，则同态* (17) *是双射*。

由于 (16) 是双射，命题由 § 4, no. 2 推出。 命题 2，应用于典范同态 (15)。

### 4. 由扩张标量获得模的对偶

设 A、B 为两个环、$\rho : A \to B$ 环同态，E 左A-模且 E* 为对偶。我们将定义一个规范的 B-*线性* 映射

$$
v_E : (E^*)_{(B)} \to (E_{(B)})^*.
$$

(19) 的左侧可写为 $\mathrm{Hom}_A(E, A) \otimes_A \rho_* (B_s)$，其中，在 $\mathrm{Hom}_A(E, A)$ 中，A 被视为 (A, A) 双模。然后有一个规范的 $\mathbf{Z}$ 同态 ($§ 4$, no. 2, 公式 (7))

$$
v : \mathrm{Hom}_A(E, A) \otimes_A \rho_* (B_s) \to \mathrm{Hom}_A(E, A \otimes_A \rho_* (B_s)) = \mathrm{Hom}_A(E, \rho_* (B_s))
$$

典范同构给出$§ 3$、no. 4、命题4的标识。另一方面，(19)的右侧可写为$\mathrm{Hom}_B(\rho_* (B_d) \otimes_A E, B_s)$；由于 B 是 (B, A)-双模，因此存在规范的 $\mathbf{Z}$ 同构 ($§ 4$, no. 1, 命题 1)

$$
\beta : \mathrm{Hom}_B(\rho_* (B_d) \otimes_A E, B_s) \to \mathrm{Hom}_A(E, \mathrm{Hom}_B(B_s, B_s))
$$

$\mathrm{Hom}_B(B_s, B_s)$ 被规范地标识为 A-模，与 $\rho_* (B_s)$（参见no. 1、命题 1 的证明）。考虑到这些识别，我们得到同态 $v_E$；很容易验证这个同态的特征在于方程

$$
\langle \xi \otimes x, v_E(x^* \otimes \eta) \rangle = \xi_p (\langle x, x^* \rangle) \eta,
$$

对于 B 中的 $x \in E, x^* \in E^*, \xi, \eta$，这立即表明 $v_E$ 是 B-*线性*。此外，对于每 A-线性映射 $u : E \to F$ 图表

$$
\begin{array}{ccc}
(F^*)_{(B)} & \xrightarrow{v_F} & (F_{(B)})^* \\
(tu)_{(B)} \downarrow & & \downarrow t(u_{(B)}) \\
(E^*)_{(B)} & \xrightarrow{v_E} & (E_{(B)})^*
\end{array}
$$

是可交换的。

#### 命题 8 {#alg-ii-s5-prop-8 .statement tag=05QO}

*如果 A-模* E、$\rho_* (B_s)$ *之一是射影且有限生成的，则同态* $v_E$ *是双射*。

这是从上面和 § 4, no. 2、命题 2 得出的。

特别假设E是有限生成的自由A-模，并令$(e_i)_{1 \leq i \leq n}$是E的基和$(e_i^*)$对偶基；然后$(E^*)_{(B)}$的典范同构(19)映射基$(e_i^* \otimes 1)$到基$(1 \otimes e_i)$的对偶基$E_{(B)}$。

### 5. 有限性准则

#### 命题 9 {#alg-ii-s5-prop-9 .statement tag=05QP}

设 B 为环，B 的 A 子环，P 为射影左A-模。那么，如果$P_{(B)}$是有限生成的B-模，则P本身就是有限生成A-模。

我们知道（§ 2, no. 6，命题 12），存在 P 的元素的族$(a_\lambda)_{\lambda \in L}$ 和对偶 P* 的元素的$(a_\lambda^*)_{\lambda \in L}$族，使得对于所有$x \in P$，$\langle x, a_\lambda^* \rangle$族属于有限支撑并且$x = \sum_\lambda \langle x, a_\lambda^* \rangle a_\lambda$。由于$P_{(B)}$是有限生成的，因此存在P的元素的有限族$(y_i)_{i \in I}$，使得$P_{(B)}$由元素$1 \otimes y_i$生成。对于每个指标 i，家庭 $\langle y_i, a_\lambda^* \rangle$ 有有限支撑。因此，存在 L 的有限子集 H，使得 $\langle y_i, a_\lambda^* \rangle = 0$ 对于 $i \in I$ 和 $\lambda \notin H$。自从
$$
\langle 1 \otimes y_i, 1 d_B \otimes a_\lambda^* \rangle = \langle y_i, a_\lambda^* \rangle,
$$
由此可见 $1 d_B \otimes a_\lambda^* = 0$ 对应 $\lambda \notin H$。因此，对于所有 $x \in P$，
$$
\langle x, a_\lambda^* \rangle = \langle 1 \otimes x, 1_B \otimes a_\lambda^* \rangle = 0
$$
$\lambda \notin H$。这表明A-模 P 由$a_\lambda$ 生成，使得$\lambda \in H$。

### 习题{#alg-ii-s5-exercises}

§ 5](exercises/s5/)参见[习题。
