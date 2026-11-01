---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 6
section_title: Real and complex Lie groups
lang: zh
source: lie-i-iii
book_pages: 304-326, 383-391
pdf_pages: 0322-0344, 0401-0409
extraction: ocr
subsections:
    - "no": 1
      title: PASSAGE FROM LIE ALGEBRA MORPHISMS TO LIE GROUP MORPHISMS
      page: 304
      pdf_page: 322
    - "no": 2
      title: INTEGRAL SUBGROUPS
      page: 306
      pdf_page: 324
    - "no": 3
      title: PASSAGE FROM LIE ALGEBRAS TO LIE GROUPS
      page: 310
      pdf_page: 328
    - "no": 4
      title: EXPONENTIAL MAPPING
      page: 311
      pdf_page: 329
    - "no": 5
      title: APPLICATION TO LINEAR REPRESENTATIONS
      page: 315
      pdf_page: 333
    - "no": 6
      title: NORMAL INTEGRAL SUBGROUPS
      page: 316
      pdf_page: 334
    - "no": 7
      title: PRIMITIVES OF DIFFERENTIAL FORMS WITH VALUES IN A LIE ALGEBRA
      page: 318
      pdf_page: 336
    - "no": 8
      title: PASSAGE FROM LAWS OF INFINITESIMAL OPERATION TO LAWS OF OPERATION
      page: 318
      pdf_page: 336
    - "no": 9
      title: EXPONENTIAL MAPPING IN THE LINEAR GROUP
      page: 320
      pdf_page: 338
    - "no": 10
      title: COMPLEXIFICATION OF A FINITE-DIMENSIONAL REAL LIE GROUP
      page: 322
      pdf_page: 340
statements: 71
exercises: 30
content_sha256: 49ed56cb4e63a83cabe904f9f51f7faf2b83b2b41c5100191341e9b510066651
translated_from: content/en/lie/III/06_s6_real_and_complex_lie_groups.md
translation_method: google
source_content_sha256: e472279781ec8c0c5cc2af6e1e4dd1a20a67a73d7a8042acdd1dea73f6ae558d
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 8cc1a4abec58d48e3ac593a6433cd220a9ab496b6d5cd0dc749a0a5656e86618
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 6。真实而复杂李群

在本段中，假设 K 等于 $\mathbf{R}$ 或 $\mathbf{C}$。

### 1. 从李代数态射到李群态射

#### 引理 1 {#lie-iii-s6-lem-1 .statement tag=0AE8}

*令 G 为单连通†拓扑群，W 为 E、H 群和 $W^3$ 的 f 映射的对称连通开邻域到 H，使得*

$$
f(xyz) = f(x)f(y)f(z)
$$

*对于 W 中的 x、y、z。存在 G 的态射 $f'$ 到 H 中，使得 $f' \mid W = f \mid W$。*

对于$(g, h) \in G \times H$和U，W中e的开邻域，对于$u \in U$，令$A(g, h, U)$为$(gu, hf(u)) \in G \times H$的集合。然后是$(g, h) \in A(g, h, U)$和$A(g, h, U_1) \cap A(g, h, U_2) = A(g, h, U_1 \cap U_2)$。令 $(s, t) \in A(g, h, U)$；然后 $s = gu$ 和 $t = hf(u)$ $u \in U$； W 中存在 e 的开邻域 $U'$，使得 $uU' \in U$；那么，对于$u' \in U'$，

$$
(su', tf(u')) = (guu', hf(uu')) \in A(g, h, U)
$$

† 参见。 *一般拓扑*的章XI（出现）。在此章中证明，若$G_1, G_2$拓扑连通群，则$\phi$是$G_1$到$G_2$与离散核的开连续同态，且$G_2$单连通，则$\phi$为同胚。另一方面，回想一下简单连接的空间是连通的。

因此$A(s, t, U') \subset A(g, h, U)$。那么$G \times H$上的拓扑的$A(g, h, U)$形式基。我们用拓扑表示$Y$集合$G \times H$，并用$p$表示$Y$的规范投影到$G$，它是开放的。 $p$到$A(g, h, U)$的限制是$A(g, h, U)$到$gU$的同胚。因此$(Y, p)$是$G$的覆盖空间。令$Y_0$为$A(e, e, W)$生成的$Y$的子群，并令$\mathfrak{B}$为$A(e, e, U)$的集合。显然，$\mathfrak{B}$满足*一般拓扑*、章III, § 1, no. 2的条件（GV$_1'$）和（GV$_1''$）。 $y \in Y_0$的集合$Y_0'$使得$Y_0$的映射$z \mapsto yzy^{-1}$和$z \mapsto y^{-1}zy$进入$Y_0$在$(e, e)$处是$Y_0$的子群连续。让$w \in W$。 $W$到$G$的映射$w' \mapsto ww'w^{-1}$是连续的，因此映射

$$
(w', f(w')) \mapsto (ww'w^{-1}, f(ww'w^{-1}))
$$

$A(e, e, W)$ 到 $Y$ 在 $(e, e)$ 连续。现在$f(ww'w^{-1}) = f(w)f(w')f(w^{-1})$，因此$(ww'w^{-1}, f(ww'w^{-1})) = (w, f(w))(w', f(w'))(w, f(w))^{-1}$。

作为$w^{-1} \in W$，我们看到$(w, f(w)) \in Y_0'$。因此，$A(e, e, W) \subset Y_0'$，所以$Y_0' = Y_0$。 群$Y_0$，加上滤波器基$\mathfrak{B}$，因此满足*通用拓扑*、章III, § 1, no. 2的条件（GV$_{III}'$）。作为

$$
(g, h).A(e, e, U) = A(g, h, U),
$$

$Y_0$ 是拓扑群，由于 $A(e, e, W)$ 是连通的，因此它也是连通的。那么$p(Y_0)$是$G$、从而$p(Y_0) = G$的开子群，因为$G$是连通的。 $p \mid Y_0$ 的核是离散的。由于$G$是单连通的，$p \mid Y_0$是$Y_0$到$G$的同胚。因此$Y_0$是$G$的态射$f'$到$H$的图。适用于 $g \in W$、$(g, f(g)) \in A(e, e, W) \subset Y_0$、从而 $f'(g) = f'(g)$。

#### 定理 1 {#lie-iii-s6-thm-1 .statement tag=0AE9}

*设$G$和$H$为李群和$h$，$L(G)$到$L(H)$的连续态射。假设 $G$ 是单连通的。那么$G$到$H$中存在且仅有一个李群态射$\phi$使得$h = L(\phi)$。*

$\phi$ 的存在性由引理 1 和§ 4, no. 1、定理 1 (i) 推出。 $\phi$ 的唯一性由§ 4, no. 1、定理 1 (ii) 得出，并且$G$ 是相连的。

#### 推论{#lie-iii-s6-n1-cor-1 .statement tag=0AEA}

*令$G$为有限维单连通李群。存在 $G$ 的有限维解析线性表示，其核是离散的。*

存在 (章 I, § 7, 定理 2) 有限维向量空间 $E$ 和 $L(G)$ 的单射态射 $h$ 进入李代数 $\mathrm{End}(E)$。到定理 1，存在$G$的态射$\phi$进入$\mathbf{GL}(E)$，使得$L(\phi) = h$。因此 $\phi$ 是沉浸式的，因此它的核是离散的。

#### 注 {#lie-iii-s6-n1-rem-1 .statement tag=0AEB}

(1) 存在有限维单连通李群，且无有限维单射解析线性表示 (习题 2)。

(2) 存在有限维连通李群$G$，使得$G$的每个有限维解析线性表示都有非离散核（习题3和4）。

### 2. 积分子群

#### 定义 1 {#lie-iii-s6-def-1 .statement tag=0AEC}

设G为李群。 G 的积分子群是子群 H，并连接了李群结构，使得 H 到 G 的典范嵌入是浸没。

G 的一参数子群是 G 的一维积分子群。

设 H 是 G 的子群和 H 的 i 典范嵌入到 G 中的积分。然后将 L(H) 的 L(i) 定义同构放到 L(G) 的谎言子代数上，承认拓扑补充。 L(H) 与L(i) 下的像进行标识。

#### 例 {#lie-iii-s6-n2-exa-1 .statement tag=0AED}

(1) G 的连通李子群是 G 的积分子群。

(2) 假设G是有限维的。令 H 为 G 的子群；我们给它由 G (§ 4, no. 5, 定义 3) 上的李群结构诱导的结构。那么它的恒等分量 H_0 是 G 的积分子群，且子代数与 H 相切，e 为 L(H_0) (§ 4, no. 5, 命题 9 (ii))。

(3) 令 G 为复数李群，H 为 G 的积分子群，G_1（或 H_1）为 G（或 H）的基础实李群。那么H_1是G_1的积分子群，L(H_1)是L(H)的底层实数李代数。

#### 定理 2 {#lie-iii-s6-thm-2 .statement tag=0AEE}

设G为李群。

(i) 映射 H ↦ L(H) 是 G 的积分子群的集合的双射到 L(G) 的李子子代数的集合，承认拓扑补充。

(ii) 令 H 为 G 的积分子群。G 与李代数 L(H) 连接的每个李子群胚芽都是 H 的开子流形，其中生成 H。

(a) 设 h 是 L(G) 的谎言子代数，承认拓扑补充。令 H_1 为 G 的李子群胚芽，使得 L(H_1) = h (§ 4, 定理 3)。可以选择H_1以使其连接。令 H 为 H_1 生成的 G 的子群。 H 上存在（§ 1，命题 22 的推论）李群结构，使得 H_1 是 H 的开子流形，并且 H 到 G 的典范嵌入是浸没。由于 H_1 连通，因此 H 连通，因此是 G 的积分子群。则 L(H) = L(H_1) = h。这证明了 (i) 中考虑的映射是满射的。

(b) 令 H 为 G 的积分子群，N_1 为 G 与李代数 L(H) 连接的李子群胚芽。由于 H 典范嵌入进入 G 是浸没，因此存在 H 的开子群胚芽 H_1，它同时是 G 的子流形，因此是 G 的李子群胚芽，具有李代数 L(H)。另一方面，令N为N_1生成的G的子群；由证明的部分(a)，它具有G的积分子群的结构，使得N_1是N的开子流形。由§ 4，定理3，H_1∩N_1在H_1和N_1中开。因此，由 H_1 ∩ N_1 生成的 G 的子群一方面等于 H，另一方面等于 N。因此李群 H 和 N 相等。这证明了(ii)，也证明了(i)中考虑的映射是单射的。

#### 注 1 {#lie-iii-s6-n2-rem-1 .statement tag=0AEF}

令 H 为 G 的积分子群。令 Y 为与 L(H) 相关的 G 的左叶。如果$g \in G$，则让$gH$由$\gamma(g)$从H上派生出流形结构。通过可微分解析流形，R，9.3.2，$gH$的典范嵌入到Y中是态射。这个态射是étale。因此，Y 的最大连通叶是模 H 的左陪集。

#### 命题 1 {#lie-iii-s6-prop-1 .statement tag=0AEG}

*设G和M为李群，H为G的子群和M的$\phi$态射积分到G中，使得$L(\phi)(L(M)) \subset L(H)$。假设M是连通的。那么$\phi(M) \subset H$和$\phi$，视为M到H的映射，是李群态射。*

在注 1 的记号中，$\phi$ 是 M 的态射到 Y 中（*可微分和解析流形*，R，9.3.2），因此 $\phi(M) \subset H$ 因为 M 是连通的。

#### 推论 1 {#lie-iii-s6-prop-1-cor-1 .statement tag=0AEH}

*设G和H为G的李群、$\phi$李群态射到H、$\phi$和$h = L(\phi)$的N核。假设 G 是连通的并且 H 是有限维的。*
(i) *N 是 G 和 $L(N) = \mathrm{Ker}\ h$ 的谎言子群。*
(ii) *令 H' 为 H 与李代数 Im h 的积分子群。然后$\phi(G) = H'$.*
(iii) *当经过与李群同构的商为李群同构时，将 G/N 的映射转化为由$\phi$ 导出的 H'。*

(i) 已被证明(§ 3, no. 8,命题28)。

当经过为商时，令$\psi$为G/N到H中的李群态射，由$\phi$导出；这是一种沉浸感（§ 3, no. 8，命题28）。通过命题 1，$\psi$ 是 G/N 的李群态射进入 H'。这个态射是 étale，因此 $\psi(G/N) = H'$ 因为 H' 是连通的；这就证明了(ii)。则$\psi : G/N \to H'$是双射且是李群同构，从而证明(iii)。

#### 推论 2 {#lie-iii-s6-prop-1-cor-2 .statement tag=0AEI}

*设G为李群，H_1和H_2对G进行积分子群。如果$L(H_2) \subset L(H_1)$，则H_2是H_1的子群积分。*

设$i_1 : H_1 \to G, i_2 : H_2 \to G$为典范嵌入。然后
$$
L(i_2)(L(H_2)) = L(H_2) \subset L(H_1).
$$
到命题 1 时，$i_2$ 是将$H_2$ 的映射解析为 $H_1$，甚至将 $H_2$ 浸入 $H_1$，因为 $L(i_2)$ 是 $L(H_2)$ 的同构到$L(H_1)$ 的子代数承认拓扑补充。

#### 推论 3 {#lie-iii-s6-prop-1-cor-3 .statement tag=0AEJ}

*设G是有限维李群和$(H_i)_{i \in I}$G的李子群族。那么$H = \bigcap_{i \in I} H_i$是G的李子群并且*
$$
L(H) = \bigcap_{i \in I} L(H_i).
$$
存在I的有限子集 J，使得$\bigcap_{i \in J} L(H_i)$等于所有L(H_i)中的交 M。我们知道 H^* = \bigcap_{i \in J} H_i 是一个谎言子群，使得 L(H^*) = M (§ 3, no. 8，推论 2 到命题 29)。令 H_0 为 H^* 的恒等分量。它是 G 的谎言子群且 L(H_0) = M。根据推论 2，对于所有 i，H_0 \子集 H_i，因此 H_0 \子集 H \子集 H^*，从而推论。

#### 推论 4 {#lie-iii-s6-prop-1-cor-4 .statement tag=0AEK}

*设 G 为有限维连通李群。以下条件是等效的：*
(i) *G 是幺模*（整的，章 VII, § 1, no. 3，定义 3）；
(ii) *det Ad g = 1，对于 G* 中的所有 g；
(iii) *Tr ad a = 0 对于L(G)* 中的所有 a。

映射 g \mapsto det Ad g 是 G 到 K* 的态射 $\phi$。 § 3、命题 35 (no. 10) 和 44 (no. 12)，$L(\phi)a = Tr\ ad\ a$ 适合所有 $a \in L(G)$。显然，Im $L(\phi) = \{0\}$ 或 K。在第一种（或第二种）情况下，根据推论 1，Im $\phi = \{1\}$（或 Im $\phi = K^*$），因此 G 是 § 3, no. 16 的单模（或非单模），推论为命题 55。

#### 命题 2 {#lie-iii-s6-prop-2 .statement tag=0AEL}

*设 G 为有限维李群，H 为 G 的积分子群。以下条件是等效的：*
(i) *H 关闭*；
(ii) H 上的 *拓扑由 G* 上的拓扑诱导；
(iii) *H 是 G* 的谎言子群。
(i) $\Rightarrow$ (iii)：源自§ 1、命题 2 (iv) (no. 1) 和 14 (iii) (no. 7)。
(iii) $\Rightarrow$ (ii)：显而易见。
(ii) $\Rightarrow$ (i)：如果 H 上的拓扑由 G 上的拓扑引发，则 H 是封闭的，因为 H 是完备的 (§ 1, no. 1, 命题 1)。

#### 命题 3 {#lie-iii-s6-prop-3 .statement tag=0AEM}

*设 G 为李群，H 为 G 的积分子群，M 为非空连通解析流形，M 的 f 映射进入 G 和 r \in N_K。考虑以下条件：*
(i) *f 为类 C^r 且 f(M) \子集 H*；
(ii) *f(M) \子集 H 和 f，被认为是 M 到 H 的映射，是类 C^r*；
(iii) *f 为类 C^r，f(M) 满足 H 并且 T_m(M) 的像包含在 f(m).L(H) 中，对于 M* 中的所有 m。

*然后 (ii) $\Leftrightarrow$ (iii) $\Rightarrow$ (i)。如果 H 上的拓扑承认可数基，则三个条件是等价的。*
(ii) $\Rightarrow$ (i) 和 (ii) $\Rightarrow$ (iii)：显而易见。
(iii)$\Rightarrow$(ii)：假设条件(iii)成立。通过*可微分和解析流形*，R，9.2.8，f是M的类C^r的态射进入与L(H)相关的左叶状结构。当 M 连通时，f(M) \子集 H。

如果 H 上的拓扑承认可数基，条件 (i) 意味着 f 是 M 的类 C^r 的映射到 H 中（*可微分和解析流形*，R，9.2.8）；因此 (i) $\Rightarrow$ (ii)。

#### 推论 1 {#lie-iii-s6-prop-3-cor-1 .statement tag=0AEN}

设 G 为有限维李群，H 为 G 的积分子群。则在 e (§ 4, no. 5, 定义 2 和 3) 处与 H 相切的李线子代数为 L(H)，且 H 上的李群结构为由 G 上的结构引起。

由于 H 是连通且有限维的，因此它的拓扑承认可数的基。

#### 推论 2 {#lie-iii-s6-prop-3-cor-2 .statement tag=0AEO}

设G为李群，H_1和H_2对G的积分子群。假设H_1上的拓扑承认可数基。然后

$$
H_2 \subset H_1 \Leftrightarrow L(H_2) \subset L(H_1)
$$

并且，如果这些条件成立，则H_2是H_1的积分子群。

最后一个断言和蕴涵 $L(H_2) \subset L(H_1) \Rightarrow H_2 \subset H_1$ 从推论 2 到命题 1。逆命题蕴涵从命题 3。

#### 推论 3 {#lie-iii-s6-prop-3-cor-3 .statement tag=0AEP}

令 G 为李群以及 H_1 和 H_2 对 G 的积分子群，其中拓扑承认可数基。如果H_1和H_2具有相同的底层集合，则H_1和H_2上的李群结构相同。

这是从推论 2 得出的。

#### 注 2 {#lie-iii-s6-n2-rem-2 .statement tag=0AEQ}

令 G 为有限维李群。设H是G的子群。我们滥用语言，可以说，如果H上存在李群结构S，则H是G的子群积分，使得H与S一起是G的子群积分。根据推论3到命题3，如果S存在，则S是唯一的。

#### 注 3 {#lie-iii-s6-n2-rem-3 .statement tag=0AER}

设V为类C^r中的流形。令 M 为 V 的子集，并且 M 的 x 和 y 元素。考虑以下性质：

P_{M, x, y}：存在 I, x_0, x_1, \ldots, x_n, f_1, \ldots, f_n 使得： (a) I 是 \mathbf{K} 的连通开子集； (b) x_0, \ldots, x_n 在 M 中，x_0 = x, x_n = y； (c) 对于 1 \leq i \leq n，f_i 是 I 的类 C^r 的映射到 V，其中需要值 x_{i-1} 和 x_i 和 f_i(I) \子集 M。

如果对于 M 的所有元素 x, y，性质 P_{M, x, y} 成立，我们可以说 M 是 V 的C^r 连接子集。

#### 命题 4 {#lie-iii-s6-prop-4 .statement tag=0AES}

令 G 为 G 的有限维李群且 H 子群。令 r \in \mathbf{N}_\mathbf{K}。以下条件是等价的：
(i) H 是 G 的积分子群；
(ii) 与 G 上的李群结构连接，H 相连；
(iii) H 是 C^r 连接的。
(iii)\右箭头(i)：显而易见。
(i) \右箭头 (iii)：假设 H 有李群结构，使得 H 是 G 的子群积分。使用注 3 的记号，y \in H 中的集合使得性质 P_{H, e, y} 成立H 的子群。由于 H 是连通的，因此子群等于 H，因此满足条件 (iii)。

(iii) ⇒ (ii): 假设条件 (iii) 满足，并令H 为G 上李群结构诱导的结构。令h 与H 在e 处子代数相切。 H 的单位分量 H_0 是 G 的积分子群，使得 L(H_0) = h。我们证明 H = H_0。只需证明以下内容即可：设 I 为 K 的连通开子集，类的 f 映射 I 的C^r 到 G 中，使得 f(I) ⊂ H 和 λ 和 μ 的两个点 I；如果 f(λ) ∈ H_0，则 f(μ) ∈ H_0。但是，对于所有 v ∈ I，(T_v f)(K) ⊂ f(v)h 除以 h 的定义，因此我们的断言由命题 3 得出。

#### 注 4 {#lie-iii-s6-n2-rem-4 .statement tag=0AET}

如果K = R，G的积分子群也可以表征为子群，它与G上的积分拓扑弧向连通（§ 8，习题4）。然而，子群可以连通，但不能积分（交换代数、章VI, § 9、习题2）。

#### 推论{#lie-iii-s6-n2-cor-1 .statement tag=0AEU}

设G是有限维李群，H_1和H_2是G的两个积分子群。H_1和H_2生成的G的子群和G的子群（H_1，H_2）是G的子群积分。

G 的子群 (G, G) 并不总是闭集 (§ 9, 习题 6)。

回想一下（§ 3, no. 11，推论 5 到命题 41），如果 a 是有限维代数，则 Aut(a) 是 GL(a) 的谎言子代数，并且 L(Aut(a)) 是 a 的推导的李代数。

#### 定义 2 {#lie-iii-s6-def-2 .statement tag=0AEV}

令 a 为有限维李代数。设 Ad(a) 或 Int(a) 表示 Aut(a) 与李代数 ad(a) 的积分子群。这个群的元素称为a的内自同构。

通过迁移或结构，ad(a) 在 Aut(a) 下是不变的，因此 Int(a) 在 Aut(a) 中是正规的。根据§ 4, no. 4、推论1到命题8以及Int(a)连通的事实，Int(a)的元素是形式exp ad x的自同构的有限乘积，其中x ∈ a。一般来说，Int(a) 不是 Aut(a) (习题 14) 的谎言子群。

### 3. 从李代数到李群的通道

#### 定理 3 {#lie-iii-s6-thm-3 .statement tag=0AEW}

(i) 如果L是有限维李代数，则存在单连通李群 G，使得L(G)与L同构。

(ii) 令 G_1 和 G_2 为两个连通的李群，其中 G_1 单连通。设 f 为 L(G_1) 的同构到 L(G_2)，G_1 的 φ 态射到 G_2，使得 L(φ) = f 且 φ 的 N 核。那么N是G_1的中心的离散子群和G_1/N到G_2的态射，从φ是李群同构导出。如果G_2是单连通的，则φ为同构。

令 L 为有限维李代数。存在有限维向量空间 E，使得 L 可以用 End(E) 的谎言子代数来识别（章 I, § 7，定理 2）。设 H 为 GL(E) 的积分子群，其中

李代数L。令 $\hat{H}$ 为其通用覆盖 ($§ 1$, no. 9, *注*)。那么$L(\hat{H})$同构于L、从而(i)。

令 $G_1, G_2, f, \phi, N$ 如 (ii) 中所示。那么$\phi$是étale，因此$\phi(G_1)$是$G_2$的开子群，因此$\phi(G_1) = G_2$。另一方面，N 是离散的，因此包含在 $G_1$ 的中心中（*整的*、章 VII、$§ 3$、引理 4）。显然，从$\phi$派生出$G_1/N$到$G_2$的态射是李群同构。如果$G_2$是单连通的，则$G_1$到$G_2$的每个étale映射都是单射的，因此$N = \{e\}$。

#### 命题 5 {#lie-iii-s6-prop-5 .statement tag=0AEX}

*设 G 为连通的实李群。假设$L(G)$有一个复范数李代数结构$L'$与其真实范数李代数结构兼容。 G 上存在且仅存在一个与实李群结构和李代数 $L'$ 兼容的复数李群结构。*

由$§ 4$，no. 2，推论2到定理2，足以证明$L'$的结构在Ad G下是不变的。设$\phi$是G的映射指数。由$§ 4$，no. 4，推论3(i)至命题8，$L(G)$中存在0的邻域V，使得$L'$的结构在Ad$\phi(V)$下不变。但 Ad $\phi(V)$ 生成 G 因为 G 是连通的。

如果不假设 G 是连通的（习题 7），命题 5 的结论不一定成立。

#### 命题 6 {#lie-iii-s6-prop-6 .statement tag=0AEY}

*设 G 为连通复形李群。如果 G 是紧致的，则 G 是可交换的。*

G 到 $\mathscr{L}(L(G))$ 的全纯映射 $g \mapsto \mathrm{Ad}\,g$ 是常数（*可微且解析流形*，R，3.3.7），因此对于所有$a \in L(G)$（$§ 3$，no. 12，$\mathrm{ad}\,a = 0$， 命题44）。因此 G 是可交换的（$§ 4$，推论 3 到定理 1）。

### 4. 指数映射

#### 定理 4 {#lie-iii-s6-thm-4 .statement tag=0AEZ}

*设G为李群。存在且仅有一个定义在 $L(G)$ 上的 G 指数映射。*

在 $L(G)$ 中存在 0 的凸开邻域 U，并且在 U 上定义 G 的指数映射。可以假设，通过选择足够小的 U，
$$
\phi((\lambda + \lambda')a) = \phi(\lambda a)\phi(\lambda'a)
$$
对于 K 中的 $a \in L(G)$、$\lambda, \lambda'$、U 中的 $\lambda a, \lambda'a, (\lambda + \lambda')a$。

让$a \in L(G)$。存在整数$n > 0$使得$\frac{1}{n} a \in U$。如果 m 是另一个整数使得 $\frac{1}{m} a \in U$，则 $\frac{1}{nm} a \in U$ 和关系 (1) 意味着
$$
\phi\left(\frac{1}{n} a\right) = \left(\phi\left(\frac{1}{nm} a\right)\right)^m, \quad \phi\left(\frac{1}{m} a\right) = \left(\phi\left(\frac{1}{nm} a\right)\right)^n;
$$

因此$\left( \phi \left( \frac{1}{n} a \right) \right)^n = \left( \phi \left( \frac{1}{m} a \right) \right)^m$。存在$\phi$的扩张$\psi : L(G) \to G$使得$\psi(a) = \left( \phi \left( \frac{1}{n} a \right) \right)^n$对于$a \in L(G)$和$n$整数$> 0$使得$\frac{1}{n} a \in U$。显然 $\psi$ 是解析的，并且是 $G$ 的指数映射。如果$\psi' : L(G) \to G$是$G$的指数映射，则$\psi$和$\psi'$重合在邻域上为0，因此它们相等，因为$L(G)$是连通的。

今后，当我们谈到$G$的*指数映射*时，我们指的是在定理4中考虑的映射。如果不存在混淆的风险，它将用$\exp_G$或$\exp$表示。

#### 例 {#lie-iii-s6-n4-exa-1 .statement tag=0AF0}

令 $A$ 为完全规范单位结合律代数。那么$\exp_{A^*}$就是章II, § 7, no. 3定义的指数映射。

#### 命题 7 {#lie-iii-s6-prop-7 .statement tag=0AF1}

*令 $G$ 为李群，且 $L(G)$ 为 $a$ 元素。 $K$的映射$\lambda \mapsto \exp(\lambda a)$到$G$的结果是李群$K$到$G$的唯一态射$\phi$，使得$(T_0 \phi)1 = a$。

$K \times K$的映射$(\lambda, \lambda') \mapsto \exp(\lambda a) \exp(\lambda' a)$和$(\lambda, \lambda') \mapsto \exp(\lambda + \lambda') a$进入$G$是解析的，重合在$(0, 0)$的邻域上。由于$K \times K$相连，因此这些映射相等。因此$\phi : \lambda \mapsto \exp(\lambda a)$是$K$到$G$的李群态射。 0 到 $\lambda \mapsto \lambda a$ 处的切线映射为映射 $\lambda \mapsto \lambda a$；和$T_e(\exp) = \mathrm{Id}_{L(G)}$；因此$(T_0 \phi)1 = a$。 命题的唯一性断言由定理 1 得出。*

#### 命题 8 {#lie-iii-s6-prop-8 .statement tag=0AF2}

*令$G$为李群。对于$L(G)$和$n$整数中的所有$x, y$，

$$
\exp(x + y) = \lim_{n \to + \infty} \left( \left( \exp \frac{1}{n} x \right) \left( \exp \frac{1}{n} y \right) \right)^n
$$

$$
\exp[x, y] = \lim_{n \to + \infty} \left( \left( \exp \frac{1}{n} x \right) \left( \exp \frac{1}{n} y \right) \left( \exp \frac{1}{n} x \right)^{-1} \left( \exp \frac{1}{n} y \right)^{-1} \right)^{n^2}.
$$

到命题 7，这是从 § 4, no. 3 的命题 4 开始，取$\lambda = \frac{1}{n}$。

#### 命题 9 {#lie-iii-s6-prop-9 .statement tag=0AF3}

*令 $G$ 为复数李群，$G'$ 为底层实李群。然后$\exp_G = \exp_{G'}$。

这是从§ 4, no. 3的命题5以及$\exp_G$和$\exp_{G'}$的解析性得出的。

#### 命题 10 {#lie-iii-s6-prop-10 .statement tag=0AF4}

*设$G$和$H$为李群和$\phi$态射，将$G$代入$H$。
（一）$\phi \circ \exp_G = \exp_H \circ L(\phi)$。
(ii) *如果$G$是$H$的积分子群，则$\exp_G = \exp_H | L(G)$。*

指数映射

等式(i)的两侧将$L(G)$的映射解析为$H$，其中重合在0的邻域中（$§ 4$，命题8，no. 4），因此相等。 断言 (ii) 是 (i) 的特例。

#### 推论 1 {#lie-iii-s6-prop-10-cor-1 .statement tag=0AF5}

*令$G$为李群，$G'$是$G$和$a \in L(G)$的谎言子群。以下条件是等效的*：
（一）$a \in L(G')$；
(ii) $\exp(\lambda a) \in G'$ 对于所有 $\lambda \in K$ 和 $|\lambda|$ 足够小；
(iii) $\exp(\lambda a) \in G$ 对于所有 $\lambda \in K$。
论证如$§ 4$、no. 4、推论1至命题8。

#### 推论 2 {#lie-iii-s6-prop-10-cor-2 .statement tag=0AF6}

*令$G$为李群，$H$为$G$和$a \in L(G)$的积分子群。考虑以下条件*：
(i) $a \in L(H)$；
(ii) $\exp_G(\lambda a) \in H$ 对于所有 $\lambda \in K$。
*然后 (i) $\Rightarrow$ (ii)。如果 $H$ 的拓扑承认可数基，则 (i) $\Leftrightarrow$ (ii)*。
设 $i$ 为 $H$ 的典范嵌入到 $G$。如果$a \in L(H)$，那么
$$
\exp_G(\lambda a) = (\exp_G \circ L(i))(\lambda a) = (i \circ \exp_H)(\lambda a) \in H.
$$
因此 (i) $\Rightarrow$ (ii)。当 $H$ 具有可数基时，逆命题由命题 3 得出。

#### 推论 3 {#lie-iii-s6-prop-10-cor-3 .statement tag=0AF7}

*令 $G$ 为李群、$\rho$ $G$、$x \in L(G)$ 和 $g \in G$ 的解析线性表示。
(i) $\rho(\exp x) = \exp L(\rho)x$；
(ii) $\mathrm{Ad}(\exp x) = \exp \mathrm{ad}\, x$；
（三）$g(\exp x)g^{-1} = \exp(\mathrm{Ad}\, g.x)$。
论证如$§ 4$，no. 4，推论2和3至命题8。

#### 推论 4 {#lie-iii-s6-prop-10-cor-4 .statement tag=0AF8}

*令$G$为有限维连通的李群*。
（一）$\mathrm{Int}(L(G)) = \mathrm{Ad}(G)$。
(ii) *令$Z$为$G$中的中心。那么$Z$是$G$的谎言子群，其李代数是$L(G)$的中心。当经过与李群同构* 时，将$G/Z$ 的映射转化为$\mathrm{Int}\, L(G)$，由$g \mapsto \mathrm{Ad}\, g$ 派生。
断言 (i) 由推论 3 (ii) 和注之后定义 2. 设$g \in G$。在阶 $\mathrm{Ad}\, g = \mathrm{Id}_{L(G)}$ 中，$\mathrm{Int}\, g$ 重合与 $\mathrm{Id}_G$ 在 $e$ 的邻域上 ($§ 4$, no. 1, 定理 1 (ii)) 是必要且充分的，因此在整个$G$；在其他字中，$g \in Z$是必要且充分的。然后 (ii) 由推论 1 得出命题 1。

#### 定义 3 {#lie-iii-s6-def-3 .statement tag=0AF9}

*令$G$为有限维连通的李群。 李群 $\mathrm{Int}(L(G)) = \mathrm{Ad}(G)$ 称为$G$* 的伴随群。

#### 命题 11 {#lie-iii-s6-prop-11 .statement tag=0AFA}

*设 $G$ 为连通交换律李群*。
(i) *exp 是添加剂李群 $L(G)$ 到 $G$* 的 étale 态射。

(ii) *如果 K = \mathbf{R} 并且 G 是有限维的，则 G 同构于形式 $\mathbf{R}^p \times \mathbf{T}^q$ ($p, q$ 整数 $\geqslant 0$) 的李群。*

根据 Hausdorff 公式，$(\exp x)(\exp y) = \exp(x + y)$ 对于 $x, y$ 足够接近 0，因此对于 $L(G)$ 中的所有 $x, y$ 通过解析延拓。因此 $\exp$ 是群同态并且是 étale 因为

$$
T_e(\exp) = \mathrm{Id}_{L(G)}.
$$

因此(i)。 断言 (ii) 源自 (i) 和*一般拓扑*、章 VII, § 1、命题 9。

#### 命题 12 {#lie-iii-s6-prop-12 .statement tag=0AFB}

*设 G 为李群和 $L = L(G)$。对于所有$x \in L$，令$T_x(L)$与$L$等价，这样$\exp$在$x$的右微分$\varpi(x)$就是$L$到$L$的线性映射。对于所有$x \in L$，

$$
\varpi(x) = \sum_{n \geqslant 0} \frac{1}{(n + 1)!} (\mathrm{ad}\ x)^n.
$$

两侧是 $x$ 的解析函数，并且对于足够接近 0 的 $x$ 是相等的（§ 4, no. 3、命题 6）。

#### 注 {#lie-iii-s6-n4-rem-1 .statement tag=0AFC}

$\varpi(x) \cdot (\mathrm{ad}\ x) = \exp \mathrm{ad}\ x - 1$。我们通过滥用记号来写道，

$$
\varpi(x) = \frac{\exp \mathrm{ad}\ x - 1}{\mathrm{ad}\ x}.
$$

#### 推论{#lie-iii-s6-n4-cor-1 .statement tag=0AFD}

*设 G 为复数李群和 $x \in L(G)$。 $x$ 到 $\exp_G$ 的切线映射有核 $\bigoplus_{n \in \mathbf{Z} - \{0\}} \mathrm{Ker}(\mathrm{ad}\ x - 2i\pi n)$。

积分函数$z \mapsto \sum_{n \geqslant 0} \frac{1}{(n + 1)!} z^n$，等于$z \neq 0$的$\frac{e^z - 1}{z}$，承认$2\pi i \mathbf{Z} - \{0\}$的零点，都是简单的零。然后从命题 12 和以下引理得出推论：

#### 引理 2 {#lie-iii-s6-lem-2 .statement tag=0AFE}

*设 E 为复数 Banach 空间，u 元素为 $\mathscr{L}(E)$，S 为 u 在 $\mathscr{L}(E)$ 中的谱（谱理论，章 I, § 1, no. 2），f 为开邻域上的全纯复数函数 S 的 $\Omega$。假设 f 在 $\Omega$ 中只允许有限的数不同的零 $z_1, \ldots, z_n$，多重性 $h_1, \ldots, h_n$。那么 $\mathrm{Ker}\ f(u)$ 就是 $1 \leqslant i \leqslant n$ 的 $\mathrm{Ker}(u - z_i)^{h_i}$ 的直和。

（对于 $f(u)$ 的定义，请参阅光谱理论，章 I, § 4, no. 8。）

$\Omega$ 上存在全纯函数 g，处处非零，因此 $f(z) = (z - z_1)^{h_1} \ldots (z - z_n)^{h_n} g(z)$。然后$g(u)g^{-1}(u) = g^{-1}(u)g(u) = 1$，因此$\mathrm{Ker}\ f(u) = \mathrm{Ker} \prod_{i=1}^n (u - z_i)^{h_i}$。将 $\mathrm{Ker}\ f(u)$ 视为 $\mathbf{C}[X]$ 模块，通过外法则 $(h, x) \mapsto h(u)x$ 对应 $h \in \mathbf{C}[X]$、$x \in \mathrm{Ker}\ f(u)$，我们看到 Ker $f(u)$ 是 $\mathrm{Ker}(u - z_i)^{n_i}$ 的直和，使用 *代数*， 章VII, § 2, no. 1、命题1。

### 5. 申请线性表示

#### 命题 13 {#lie-iii-s6-prop-13 .statement tag=0AFF}

*令 $G$ 为连接的李群和 $\varphi$ $G$ 的解析线性表示在完全可规范空间 $E$ 上。令$E_1, E_2$为$E$的两个闭向量子空间，使得$E_2 \subset E_1$。以下条件是等效的：*

(i) $\varphi(g)x \equiv x \pmod{E_2}$ 对于所有 $g \in G$ 和所有 $x \in E_1$；
(ii) $L(\varphi)(L(G))$ 映射 $E_1$ 变为$E_2$。

$$
\begin{align*}
&\varphi(g)x \equiv x \quad (\text{mod } E_2) \quad \text{for all } g \in G \text{ and all } x \in E_1 \\
\Leftrightarrow &\varphi(\exp a)x \equiv x \quad (\text{mod } E_2) \quad \text{for all } a \in L(G) \text{ and all } x \in E_1 \\
\Leftrightarrow &(\exp L(\varphi)a)x \equiv x \quad (\text{mod } E_2) \quad \text{for all } a \in L(G) \text{ and all } x \in E_1.
\end{align*}
$$

另一方面，如果$u \in \mathscr{L}(E)$，那么

$$
\begin{align*}
&\exp(\lambda u)x \equiv x \quad (\text{mod } E_2) \quad \text{for all } \lambda \in K \text{ and all } x \in E_1 \\
\Leftrightarrow &u(E_1) \subset E_2
\end{align*}
$$

从而命题。

#### 推论 1 {#lie-iii-s6-prop-13-cor-1 .statement tag=0AFG}

*为了使$E_1$稳定在$\varphi$下，$E_1$稳定在$L(\varphi)$下是必要且充分的。*

用命题 13 取$E_1 = E_2$就够了。

#### 推论 2 {#lie-iii-s6-prop-13-cor-2 .statement tag=0AFH}

*假设$\varphi$是有限维的。为了使$\varphi$简单（或半单），$L(\varphi)$简单（或半单）是必要且充分的。*

这是从推论 1 得出的。

#### 推论 3 {#lie-iii-s6-prop-13-cor-3 .statement tag=0AFI}

*让$x \in E$。为了使$x$在$\varphi(G)$下不变，$x$被$L(\varphi)(L(G))$湮灭是充分必要的（即$x$在$L(\varphi)$下在章、I, § 3、定义意义上不变） 3).*

在命题 13 中取$E_1 = Kx$ 和$E_2 = 0$ 就足够了。

#### 推论 4 {#lie-iii-s6-prop-13-cor-4 .statement tag=0AFJ}

*令 $\varphi'$ 为另一个在完全规范空间 $E'$ 上解析 $G$ 的线性表示。让$T \in \mathscr{L}(E, E')$。以下条件是等效的：*

(i) $T\varphi(g) = \varphi'(g)T$ 对于所有 $g \in G$；
(ii) $TL(\varphi)(a) = L(\varphi')(a)T$ 对于所有 $a \in L(G)$。

令$\sigma$为$\mathscr{L}(E, E')$上$G$的线性表示，源自$\varphi$和$\varphi'$（§ 3, no. 11，推论1至命题41）。 条件 (i) 意味着$T$ 在$\sigma(G)$ 下不变。 条件 (ii) 意味着$T$ 被$L(\sigma)(L(G))$ 湮灭。那么应用推论 3 就足够了。

#### 推论 5 {#lie-iii-s6-prop-13-cor-5 .statement tag=0AFK}

假设 $\rho$ 和 $\rho'$ 是有限维的。为了使$\rho$和$\rho'$等价，$L(\rho)$和$L(\rho')$等价是充分必要的。

这是推论4的一个特例。

#### 推论 6 {#lie-iii-s6-prop-13-cor-6 .statement tag=0AFL}

假设 $G$ 是有限维的。让$t \in U(G)$。为了使$L_t$（或$R_t$）右（或左）不变，$U(G)$的$t$属于到中心是必要且充分的。

为了使$L_t$（或$R_t$）右（或左）不变，$\varepsilon_g * t = t * \varepsilon_g$对于所有$g \in G$是必要且充分的，即$(\mathrm{Int}\, g)_* t = t$。存在整数$n$使得$t \in U_n(G)$。根据推论3和§ 3, no. 12的命题 45，$(\mathrm{Int}\, g)_* t = t$对于所有$g \in G$当且仅当$[a, t] = 0$对于所有$a \in L(G)$，即当且仅当$t$与$U(G)$通勤。

### 6. 正态积分子群

#### 引理 3 {#lie-iii-s6-lem-3 .statement tag=0AFM}

令$G$为李群、$H_1$和$H_2$积分子群，其中拓扑承认可数基和$g \in G$。然后

$$
g H_1 g^{-1} = H_2 \Leftrightarrow (\mathrm{Ad}\, g)(L(H_1)) = L(H_2).
$$

$\mathrm{Ad}\, g = T_e(\mathrm{Int}\, g)$。因此，通过结构的迁移，$(\mathrm{Int}\, g)(H_1)$有李代数$(\mathrm{Ad}\, g)(L(H_1))$。由于$H_1$和$H_2$有可数的基，所以说集合$H_2$和$(\mathrm{Int}\, g)(H_1)$相等相当于说积分子群$H_2$和$(\mathrm{Int}\, g)(H_1)$相等（no. 2，推论 3 至命题 3）。然后从定理 2 (i) 得出引理。

#### 命题 14 {#lie-iii-s6-prop-14 .statement tag=0AFN}

令$G$为李群，且$H$为子群的积分，拓扑承认可数基。以下条件是等效的：
(i) $H$在$G$中是正常的；
(ii) $L(H)$ 在 $\mathrm{Ad}(G)$ 下不变。
如果再连接$G$，这些条件等价于：
(iii) $L(H)$是$L(G)$的理想。
如果进一步$G$是单连通的，并且$L(H)$是$L(G)$中的有限余维，那么这些条件意味着$H$是$G$的谎言子群，并且$G/H$是单连通的。

等价 (i) $\Leftrightarrow$ (ii) 由引理 3 得出。如果进一步连接$G$，条件 (ii) 等价于说，$L(H)$ 在$\mathrm{ad}\, L(G)$ 下稳定（no. 5，推论 1 为命题 13 和 § 3, no. 12、命题 44）。

假设$G$是单连通的，并且$L(H)$是$L(G)$中有限余维的理想。通过no. 3的定理 3，存在单连通李群$G'$，使得$L(G')$与$L(G)/L(H)$同构的。存在$L(G)$到$L(G')$和核$L(H)$的连续态射$f$。通过no. 1的定理 1，存在$G$的态射$\phi$进入$G'$，使得$L(\phi) = f$。这个态射是一个淹没，因此它的核$N$是$G$的谎言子群使得$L(N) = \mathrm{Ker}\, f = L(H)$。因此，$H$是$N$的恒等分量，因此是G的谎言子群。设$\psi$是$G/H$的态射到从$\phi$导出的$G'$，当经过为商时。这个态射是étale；由于 G 是单连通的，$\psi$ 是 $G/H$ 的同构到 $G'$。

#### 推论 1 {#lie-iii-s6-prop-14-cor-1 .statement tag=0AFO}

*设 G 为有限维单连通李群。令 m, h 为 L(G) 的谎言子代数，使得 L(G) 是 m 通过 h 的半直乘积。设M、H为G的相应的积分子代数。则M和H是G的单联子群，并且作为李群，G是M与H的半直乘积。*

到命题 14 时，H 是 G 的正规李子群，并且李群 G/H 是单连通的。令 $\pi$ 为 G 在 G/H 上的规范态射。 M 中存在 G/H 的态射 $\theta$，使得 $L(\theta)$ 是 $L(G)/L(H) = L(G)/h$ 到 $L(M) = m$ 的典范同构。然后

$$
L(\pi \circ \theta) = L(\pi) \circ L(\theta) = \mathrm{Id}_{L(G/H)}
$$

因此$\pi \circ \theta = \mathrm{Id}_{G/H}$。由no. 1，推论1到命题1，$\theta(G/H) = M$。通过§ 1, no. 4的命题8，M是G的谎言子群，李群G是H对M的半直乘积。

#### 推论 2 {#lie-iii-s6-prop-14-cor-2 .statement tag=0AFP}

*设 G 为有限维单连通李群，H 为 G 的正常连通李子群，$\pi$ G 到 G/H 的规范态射。

(i) 存在 G/H 到 G 的解析映射 $\varphi$，使得 $\pi \circ \varphi = \mathrm{Id}_{G/H}$。

(ii) 对于具有 (i) 属性的每个映射 $\varphi$，$H \times (G/H)$ 的映射 $(h, m) \mapsto h \varphi(m)$ 进入 G 是解析的流形的同构。

(iii) H 和 G/H 是简单连接的。

让$n = \dim G - \dim H$。对于$n = 0$，推论是显而易见的。我们在 n 上争论归纳。

假设存在与 L(G) 和 L(H) 不同的理想L(G) 包含 L(H)。令 H' 是 G 的相应的连接的李子子群。令$\pi_1 : G \to G/H'$ 和$\pi_2 : H' \to H'/H$ 为规范的态射。到归纳假设，存在解析映射$\rho_1 : G/H' \to G$、$\rho_2 : H'/H \to H'$，使得$\pi_1 \circ \rho_1 = \mathrm{Id}_{G/H'}$、$\pi_2 \circ \rho_2 = \mathrm{Id}_{H'/H}$。让

$$
\pi_3 : G/H \to G/H'
$$

成为规范的态射。如果$x \in G/H$和y是G中x的代表，则y和$\rho_1(\pi_3(x))$具有相同的典范像模H'，因此$x^{-1} \pi(\rho_1(\pi_3(x))) \in H'/H$。让

$$
\rho(x) = \rho_1(\pi_3(x)) \rho_2(\pi(\rho_1(\pi_3(x))))^{-1} x \in G.
$$

显然 $\rho$ 是 G/H 到 G 的解析映射且

$$
\pi(\rho(x)) = \pi(\rho_1(\pi_3(x))) \pi_2(\rho_2(\pi(\rho_1(\pi_3(x))))^{-1} x)) \\
= \pi(\rho_1(\pi_3(x))) \pi(\rho_1(\pi_3(x)))^{-1} x = x.
$$

如果现在 L(G) 包含 L(H) 的唯一理想是 L(G) 和 L(H)，则李代数 $L(G)/L(H)$ 要么是一维的，要么是简单的。在这两种情况下，$L(G)$都是子代数乘以$L(H)$的半直接乘积；这在第一种情况下很明显，在第二种情况下，这是从章I, § 6，推论3到定理5。断言（i）然后从推论1得出。

断言 (ii) 是显而易见的。 断言 (iii) 由 (i) 和 (ii) 得出。

当 G 是无限维或者 H 不是正规的（习题 8 和 15）时，推论 2 的结论不再必然成立。

#### 推论 3 {#lie-iii-s6-prop-14-cor-3 .statement tag=0AFQ}

*设 G 为有限维连通李群，H 为 G 的正常连通李子群。$\pi_1(H)$ 到 $\pi_1(G)$ 的规范态射是单射的。*

令$G_1$为G的通用覆盖，将$G_1$的$\lambda$典范映射覆盖到G上。$G_1$的李代数与$L(G)$标识。 $G_1$的谎言子群$\lambda^{-1}(H)$在$G_1$中是正常的，其李代数是$L(H)$。令$H_1$为$\lambda^{-1}(H)$和$\lambda_1 = \lambda | H_1$的恒等分量。那么 $L(H_1) = L(H)$ 因而 $\lambda_1$ 是 $H_1$ 的 étale 态射到 H 上。另一方面，$H_1$ 是单连通的（推论 2），因此与 H 的通用覆盖一致。然后，通过 *General 拓扑*，章 XI，$\pi_1(H)$到$\pi_1(G)$的规范态射被识别为Ker $\lambda_1$到Ker $\lambda$的典范嵌入。

### 7. 形式与值李代数的微分原语

#### 命题 15 {#lie-iii-s6-prop-15 .statement tag=0AFR}

*设 G 为李群，M 流形为类 $C^r$ ($r \geq 2$)，且 $\alpha$ 为类 $C^{r-1}$ 和次数 1 的微分形式，其中值 $L(G)$，使得$d\alpha + [\alpha]^2 = 0$。假设 M 是单连通的。对于所有$x \in M$和所有$s \in G$，M到G的类$C^{r-1}$中存在且仅有一个映射f，使得$f(x) = s$和$f^{-1} \cdot df = \alpha$。

f 的唯一性从§ 3, no. 17、推论 2 到命题 59 以及 M 是连通的事实。我们证明f的存在性。存在M的开覆盖$(U_i)_{i \in I}$，并且对于所有$i \in I$，类$C^{r-1}$的映射$g_i : U_i \to G$，使得$g_i^{-1} \cdot dg = \alpha$在$U_i$上（§ 4, no. 6，定理5）。到§ 3, no. 17，推论2到命题59，$g_i g_j^{-1}$在$U_i \cap U_j$上局部恒定。让$g_i g_j^{-1} = g_{ij}$。令 $G_d$ 为群 G，并具有离散的拓扑。 $g_{ij} : U_i \cap U_j \to G_d$ 是连续的，$g_{ij} g_{jk} = g_{ik}$ 在 $U_i \cap U_j \cap U_k$ 上。由于M是单连通的，因此在$U_i \cap U_j$上存在连续的映射$\lambda_i : U_i \to G_d$使得$g_i g_j^{-1} = \lambda_i \lambda_j^{-1}$。令g为M到G的映射，其限制到$U_i$对于所有$i \in I$来说是$\lambda_i^{-1} g_i$。这个映射是类$C^{r-1}$和$g^{-1} dg = \alpha$。由$f = s(g(x))^{-1} g$定义的M到G的映射 f满足条件$f^{-1} \cdot df = \alpha$和$f(x) = s$。

### 8. 从无穷小运算的律到运算的律

#### 引理 4 {#lie-iii-s6-lem-4 .statement tag=0AFS}

*设 G 为 G 在 X 上左（或右）运算的连通拓扑群、X 豪斯多夫拓扑空间和 $f_1, f_2$ 律，使得对于所有 $x \in X$、映射* $G$到$X$的$s \mapsto f_1(s, x),\ s \mapsto f_2(s, x)$是连续的。假设$G \times X$中存在$\{e\} \times X$的邻域$V$，使得$f_1$和$V$上存在$f_2$重合。然后$f_1 = f_2$。

令$x \in X$和$A$为$g \in G$的集合，使得$f_1(g, x) = f_2(g, x)$。然后$A$在$G$关闭。另一方面，设 $g \in A$；我们写$y = f_1(g, x) = f_2(g, x)$。在$G$中存在$e$的邻域$U$，使得$f_1(t, y) = f_2(t, y)$对于$t \in U$，在其他字中使得$f_1(t', x) = f_2(t', x)$对于$t' \in Ug$（或$gU$）。因此$A$在$G$开放，因此$A = G$开放。

#### 命题 16 {#lie-iii-s6-prop-16 .statement tag=0AFT}

Let G be a connected Lie group, X a Hausdorff manifold of class C^r and f_1, f_2 laws of left (resp. right) operation of class C^r of G on X. 如果与 f_1 和 f_2 相关的无穷小运算的律相等，则 f_1 = f_2。

由§ 4, no. 7，推论命题 11，在G \times X 中存在\{e\} \times X 的邻域 V，使得f_1 和f_2 重合在V 上。因此 f_1 = f_2 (引理 4)。

#### 引理 5 {#lie-iii-s6-lem-5 .statement tag=0AFU}

设 G 为单连通拓扑群，X 豪斯多夫拓扑空间，U 为 G 中 e 的开邻域，\psi 为 U \times X 到 X 的连续映射，使得 \psi(e, x) = x 和 \psi(s, \psi(t, x)) = \psi(st, x) 对于所有 x \in X 和 s, t 在 U 中，使得 st \in U。令 W 为 e 的对称连通开邻域，使得 W^3 \子集 U。在 X 上存在且仅有一个 G 的连续左运算 \psi' 的律，使得\psi' 和 \psi 重合在 W \times X 上。如果 G 为李群且 X 流形为类 C^r，且 \psi 为类 C^r，则 \psi' 为类 C^r。

\psi 上的唯一性由引理 4 得出。令 P 为 X 的置换群。对于 u \in W^3，映射 x \mapsto \psi(u, x) 是 P 的元素 f(u) 并且

$$ f(u_1u_2u_3) = f(u_1)f(u_2)f(u_3) $$

对于W中的u_1，u_2，u_3。no. 1的应用引理1，我们将G的态射f'转化为P，其中扩展f|W。设 \psi'(g, x) = f'(g)(x) 对于所有 (g, x) \in G \times X。那么\psi'就是G在X上的左运算的律，其中重合与W上的\psi\乘以X。由于 \psi'(g, \psi'(g', x)) = \psi'(gg', x) 对于 (g, g', x) \in G \times G \times X，\psi 在 W \times X 上的连续性意味着 \psi' 在 gW \times X 上对于所有 g \in G 都是连续的。因此 \psi' 是连续的。如果\psi是类C^r，那么类似地可以看出\psi'是类C^r。

#### 定理 5 {#lie-iii-s6-thm-5 .statement tag=0AFV}

设 G 为单连通李群，X 类 C^r (r \geq 2) 的紧致流形和类的左（或右）无穷小运算的 \mapsto D_a 律 X 上L(G) 的C^{r-1}。在X上，G的类C^{r-1}的左（或右）运算存在且仅有一个律，使得无穷小运算的相关律是映射到D_a。

唯一性由命题 16推出。由§ 4, no. 7，推论1到定理 6，G \times X中存在\{e\} \times X的邻域 V和左侧的律块（右）X上G的类C^{r-1}的运算，定义在V上，使得无穷小运算的相关律是一个\mapsto D_a。由于 X 是紧致的，V 可以假设为形式 U × X，其中 U 是 G 中 e 的开邻域。那么应用引理 5 就足够了。

### 9. 线性群中的指数映射

#### 命题 17 {#lie-iii-s6-prop-17 .statement tag=0AFW}

设 Δ 为 z ε C 的集合，使得 −π < J(z) < π 且 z ε C 的 Δ' 集合不是实数 ≤ 0。设 E 为 C 上的完全可范空间和 x ε 的 A (resp. A') 集合 L(E)，其频谱 Sp(x) 包含在 Δ（或 Δ'）中。则 A（分别为 A'）是 L(E)（分别为 GL(E)）的开子集，并且映射 exp: A → A' 且对数：A' → A（谱理论，章 I, § 4, no. 9）是解析流形的逆同构。

这是从光谱理论章 I, § 4、命题 10 和 no. 9 得出的。

#### 定理 6 {#lie-iii-s6-thm-6 .statement tag=0AFX}

设 E 为实数或复数希尔伯特空间，U 为 E 的酉群。

(i) L(E) 的厄米特元素的集合 H 是，在实数范数空间结构的情况下，L(E) 的闭向量子空间承认拓扑补充。

(ii) GL(E) 的元素 ≥ 0 的集合 H' 是 GL(E) 的实解析子流形。

(iii) 映射 exp 的限制到 H 是 H 到 H' 的实解析流形的同构。

(iv) H × U 的映射 (h, u) ↦ (exp h)u 代入 GL(E) 是实解析流形的同构。

回想一下，如果 x ∈ L(E)，则 x* 表示 x 的伴随。令 H_1 为 x ∈ L(E) 的集合，使得 x* = −x。 公式 x = $\frac{1}{2}(x + x^*) + \frac{1}{2}(x - x^*)$证明，以其实范数空间结构，L(E)是H和H_1、从而(i)的拓扑直和。

假设 K = C。在命题 17 的记号中，H' 是 h ∈ H ∩ A' 的集合，使得 Sp h ⊂ R^*_+。由于 exp(R) = R^*_+，(ii) 和 (iii) 由命题 17 和谱理论、章 I, § 4、命题 8 和 § 6, no. 5 得出。 映射 (h, u) ↦ y = (exp h)u of H × U into GL(E) 根据谱理论，章 I, § 6, 命题 15，是实解析的。 映射 y ↦ h = $\frac{1}{2} \log(y y^*)$ 是实解析，映射 y ↦ u = (exp h)^{-1}y 也是实解析。因此(iv)。

假设 K = R。令 Ē 为 E 的复数希尔伯特空间，并将 Ē 的 J 映射 ψ + iη ↦ ψ − iη（对于 ψ，E 中的 η）复化为 Ē。设 Ũ、Ũ'、Ũ 表示为 Ē 定义的集合，就像 H、H'、U 为 E 定义的那样。则 H（分别为 H'、U）用 x ∈ Ũ（分别为 Ũ'、Ũ）的集合来标识，使得 JxJ^{-1} = x。然后，性质 (ii)、(iii) 和 (iv) 可以很容易地从 (i) 以及复杂情况下的类似性质得出。

#### 命题 18 {#lie-iii-s6-prop-18 .statement tag=0AFY}

令 E 为 C 上的完全可范空间，v ∈ L(E) 且 g = exp v。假设 Sp(v) 包含点 2iπn 中没有一个，且 n ∈ Z − {0}。那么，对于所有 x ∈ E，条件 vx = 0 和 gx = x 是等价的。

这是从 no. 4 的引理 2 得出的，应用于函数 z ↦ e^z − 1。

#### 推论 1 {#lie-iii-s6-prop-18-cor-1 .statement tag=0AFZ}

*设E是$E^n$到E的连续n线性映射的$\mathbf{C}$和F空间上的完全可规范空间。对于所有$v \in \mathscr{L}(E)$，令$\sigma(v)$是由*定义的$\mathscr{L}(F)$的元素

$$
(\sigma(v)f)(x_1, \ldots, x_n) = v(f(x_1, \ldots, x_n)) - \sum_{i=1}^n f(x_1, \ldots, vx_i, \ldots, x_n).
$$

*对于所有$g \in \mathbf{GL}(E)$，令$\rho(g)$为由*定义的$\mathbf{GL}(F)$的元素

$$
(\rho(g)f)(x_1, \ldots, x_n) = g(f(g^{-1}x_1, \ldots, g^{-1}x_n)).
$$

*令$u \in \mathscr{L}(E)$使得每个$z \in \mathrm{Sp}\,u$满足$|\mathscr{J}(z)| < \frac{2\pi}{n+1}$。那么，对于所有 $f \in F$，条件 $\sigma(u)f = 0$ 和 $\rho(\exp u)f = f$ 是等价的。*

$\mathbf{L}(\rho) = \sigma$（§ 3, no. 11，推论 1 到命题 41），因此

$$
\rho(\exp u) = \exp \sigma(u)
$$

（no. 4，推论 3 至命题 10）。到命题18就足以证明$\mathrm{Sp}\,\sigma(u)$不满足$2i\pi(\mathbf{Z} - \{0\})$。但这是从以下引理得出的：

#### 引理 6 {#lie-iii-s6-lem-6 .statement tag=0AG0}

*如果$v \in \mathscr{L}(E)$，则$\mathrm{Sp}\,\sigma(v) \subset \mathrm{Sp}\,v + \mathrm{Sp}\,v + \cdots + \mathrm{Sp}\,v$，其中和包含$n+1$项。*

我们定义元素$v_0, v_1, \ldots, v_n$的$\mathscr{L}(F)$通过写作，为所有$f \in F$，

$$
\begin{align*}
(v_0f)(x_1, \ldots, x_n) &= v(f(x_1, \ldots, x_n)) \\
(v_if)(x_1, \ldots, v_n) &= -f(x_1, \ldots, vx_i, \ldots, x_n) \quad \text{for } 1 \leq i \leq n.
\end{align*}
$$

那么 $\sigma(v) = \sum_{i=0}^n v_i$ 和 $v_i$ 是成对可置换的。设A为$v_i$生成的$\mathscr{L}(F)$的总闭子代数；它是可交换的 (*谱理论*, 章 I, § 1, no. 4) 和 $\mathrm{Sp}_{\mathscr{L}(F)} v' = \mathrm{Sp}_A v' \subset \sum_{i=0}^n \mathrm{Sp}\,v_i$ (*谱理论*, 章 I, § 3, 命题 3 (ii))。现在，如果$\lambda \in \mathbf{C}$使得$v - \lambda$是可逆的，那么显然$v_i - \lambda_i$是可逆的，因此对于所有$i$来说$\mathrm{Sp}\,v_i \subset \mathrm{Sp}\,v$是可逆的。

#### 推论 2 {#lie-iii-s6-prop-18-cor-2 .statement tag=0AG1}

*设 E 是 $\mathbf{C}$ 和 $w \in \mathscr{L}(E)$ 上的完全可范数代数。假设每个$z \in \mathrm{Sp}\,w$满足$|\mathscr{J}(z)| < \frac{2\pi}{3}$。以下条件是等效的：*
(i) *w 是 E 的推导；*
(ii) *exp w 是 E 的自同构。*
这是从 E 的 $n = 2$ 和 $f$ 乘法的推论 1 得出的。

#### 命题 19 {#lie-iii-s6-prop-19 .statement tag=0AG2}

令 E 为 $\mathbf{C}$、$v \in \mathscr{L}(E)$ 和 $g = \exp v$ 上的完全可范空间。假设每个$z \in \mathrm{Sp}\, v$都满足$-\pi < \mathscr{J}(z) < \pi$。那么，对于$E$的每个闭向量子空间$E'$，条件$v(E') \subset E'$和$g(E') = E'$是等价的。

条件$v(E') \subset E'$意味着$g(E') \subset E'$和$g^{-1}(E') \subset E'$，因此意味着$g(E') = E'$。假设$g(E') = E'$。我们使用命题 17 的记号 $\Delta, \Delta'$。由于$\mathrm{Sp}\, v$ 是$\Delta$ 的紧凑子集，因此存在一个紧凑矩形$Q = (a, b) \times (a', b')$，使得$\mathrm{Sp}\, v \subset Q \subset \Delta$。 集合 $\Delta - Q$ 已连接。因此 $\mathrm{Sp}\, g \subset \exp Q \subset \Delta'$、集合 $\exp Q$ 是紧致的，集合 $\Delta' - \exp Q$ 是连通的。后者的关闭包含 $]-\infty, 0]$ 因此

$$
(\Delta' - \exp Q) \cup ]-\infty, 0] = \mathbf{C} - \exp Q
$$

已连接。那么$\exp Q$是多项式凸的（*光谱理论*，章I, § 3，推论2到命题9），因此函数$\log$，在$\Delta'$上定义，是$\mathscr{O}(\exp Q)$中的极限多项式函数（*光谱理论*、章I, § 4、命题3）。因此，$v = \log g$是形式$P(g)$的元素的$\mathscr{L}(E)$中的极限，其中$P$是多项式（*光谱理论*，章I, § 4，定理3）。作为$P(g)(E') \subset E'$，可以得出$v(E') \subset E'$。

#### 推论{#lie-iii-s6-n9-cor-1 .statement tag=0AG3}

令 E 为 $\mathbf{C}$、$v \in \mathscr{L}(E)$ 和 $g = \exp v$ 上的完全范数空间。假设每个$z \in \mathrm{Sp}\, v$满足$-\frac{\pi}{2} < \mathscr{J}(z) < \frac{\pi}{2}$。那么，对于$\mathscr{L}(E)$的每个闭向量子空间M，条件$gMg^{-1} = M$和$[v, M] \subset M$是等价的。

令 $F = \mathscr{L}(E)$、$g'$ 为 F 的映射 $f \mapsto gfg^{-1}$ 入 F，$v'$ 为 F 的映射 $f \mapsto [v, f]$ 入 F。则 $g' = \exp v'$ (no. 4，推论 3 至命题 10 及§ 3, no. 11，推论 1 至命题 41)。 引理 6 证明$-\pi < \mathscr{J}(z) < \pi$ 对于所有$z \in \mathrm{Sp}\, v'$。那么就足以应用命题 19。

### 10. 有限维的复化实李群

#### 引理 7 {#lie-iii-s6-lem-7 .statement tag=0AG4}

设 B 为群，A 为 B 的正常子群，C 群 $B/A$，$i : A \to B$ 和 $p : B \to C$ 为规范的态射。令$A'$为群，并将A的$f$同态代入$A'$。设$\omega$为B的态射，代入$A'$的自同构群。假设对于$a \in A'$、$a' \in A'$、$b \in B$，

$$
f\left(bab^{-1}\right) = \omega(b)f(a), \quad \omega(a)a' = f(a)a'f(a)^{-1}.
$$

令 $B''$ 为 B 通过 $A'$ 相对于 $\omega$ 的半直接乘积，q 为 $B''$ 在 B 上的规范态射。

(i) A 的映射 $a \mapsto (f(a^{-1}), i(a))$ 到 $B''$ 是 A 的态射到 $B''$ 的普通子群 D。设$B' = B''/D$和$i' : A' \to B'$、$g : B \to B'$为$A'$和B的态射，将$B'$取$A'$的典范嵌入和B除以$B''$的商。

(ii) 当经过除以$B'$的态射除以C的商时，将$B''$的态射$p \circ q$化为C定义。

(iii) $i'$ 是单射，$p'$ 是满射，$\mathrm{Ker}(p') = \mathrm{Im}(i')$ 以及以下图表是可交换的

$$
\begin{array}{ccc}
A & \xrightarrow{i} & B \xrightarrow{p} C \\
f \downarrow & & g \downarrow \mathrm{Id}_C \\
A' & \xrightarrow{i'} & B' \xrightarrow{p'} C.
\end{array}
$$

(iv) *如果* $b \in B$ 和 $a' \in A'$，则
$$
g(b)i'(a')g(b)^{-1} = i'(\omega(b)a').
$$

(i) 对于$A$中的$a_1, a_2$，我们在$B''$中有，
$$
(f(a_1^{-1}), i(a_1))(f(a_2^{-1}), i(a_2)) = (f(a_1^{-1})(\omega(a_1)f(a_2^{-1})), i(a_1)i(a_2))
= (f(a_1^{-1})f(a_1a_2^{-1}a_1^{-1}), i(a_1a_2))
= (f((a_1a_2)^{-1}, i(a_1a_2))
$$
因此 $a \mapsto (f(a^{-1}), i(a))$ 是 $A$ 到 $B''$ 的同态 $h$。设$a \in A$，$a' \in A'$，$b \in B$；然后，在$B''$，
$$
bh(a)b^{-1} = bf(a^{-1})ab^{-1} = (\omega(b)f(a^{-1}))(bab^{-1})
= f(ba^{-1}b^{-1})(bab^{-1}) = h(bab^{-1})
$$
$$
a'h(a){a'}^{-1} = a'f(a^{-1})a{a'}^{-1} = a'f(a^{-1})(\omega(a){a'}^{-1})a
= a'f(a^{-1})f(a){a'}^{-1}f(a^{-1})a = h(a)
$$
因此 $h(A) = D$ 在 $B''$ 中是正常的。

(ii) 对于$a \in A$，
$$
(p \circ q)(h(a)) = p(q(f(a^{-1})a)) = p(a) = e
$$
因此 $p \circ q$ 在 $D$ 上是微不足道的。

(iii) 令$a' \in A'$使得$i'(a') = e$；那么$a' \in D$，因此存在$a \in A$使得$a' = f(a^{-1})a$；这意味着 $a = e$、从而 $a' = e$；因此 $i'$ 是单射的。由于 $p$ 和 $q$ 是满射，因此 $p'$ 是满射。

让$r$表示$B''$到$B'$的规范态射。设$a' \in A'$、$b \in B$和$b' = r(a'b)$。若$b' \in \mathrm{Im}(i')$，则存在$a'_1 \in A'$使得$b' = r(a'_1)$；那么存在$a \in A$使得$a'b = a'_1f(a^{-1})a$，从而$b = a \in A$并且
$$
p'(b') = p(q(a'b)) = p(b) = e;
$$
因此，$\mathrm{Im}(i') \subset \mathrm{Ker}(p')$。我们保留记号$a', b, b'$，但假设$b' \in \mathrm{Ker}(p')$；然后$e = p'(b') = p(q(a'b)) = p(b)$，因此$b \in A$，从而
$$
b' = r(a'f(b)f(b^{-1})b) = r(a'f(b)) \in \mathrm{Im}(i');
$$
因此$\mathrm{Ker}(p') \subset \mathrm{Im}(i')$。

如果$a \in A$，那么
$$
i'(f(a)) = r(f(a)) = r(f(a)f(a^{-1})a) = r(a) = g(i(a)).
$$

如果$b \in B$，那么
$$
p'(g(b)) = p(b)
$$
因此图表 (4) 是可交换的。

(iv)设$b \in B, a' \in A'$。然后
$$
g(b)i'(a')g(b)^{-1} = r(b)r(a')r(b)^{-1} = r(ba'b^{-1})
= r(\omega(b)a') = i'(\omega(b)a').
$$

#### 命题 20 {#lie-iii-s6-prop-20 .statement tag=0AG5}

*设 G 为有限维实李群。*

(i) *在$\tilde{G}$中存在一个复数李群$\tilde{G}$和一个$\mathbf{R}$解析态射$\gamma$，具有以下属性：对于每个复数李群H和每个$\mathbf{R}$解析态射 G 的 $\phi$ 转化为 H，存在且仅有一个 $\mathbf{C}$ 解析态射 $\psi$ $\tilde{G}$ 转化为 H，使得 $\phi = \psi \circ \gamma$。*

(ii) *如果$(\tilde{G}', \gamma')$与$(\tilde{G}, \gamma)$具有相同的性质，则存在且仅有一个$\tilde{G}$的同构$\theta$到$\tilde{G}'$使得$\theta \circ \gamma = \gamma'$。*

(iii) *$\mathbf{C}$-$L(G) \otimes \mathbf{C}$到$L(\tilde{G})$的线性映射，其中扩展$L(\gamma)$是满射；特别是$\dim_{\mathbf{C}}(\tilde{G}) \leq \dim_{\mathbf{R}}(G)$.*

断言 (ii) 是显而易见的。我们用性质 (i) 和 (iii) 证明有序对 $(\tilde{G}, \gamma)$ 的存在性。

(a) 首先假设 G 是连通的。令 $g = L(G)$、$g_C = g \otimes_{\mathbf{R}} \mathbf{C}$ 为 g、S（或 S'）单连通实数（或复数）李群与李代数 g（或 $g_C$）和 $\sigma$ S 的唯一 $\mathbf{R}$ 解析态射的复化S'使得$L(\sigma)$是g到$g_C$的典范嵌入。令 $\pi$ 为 S 在 G 上的唯一$\mathbf{R}$解析态射，使得 $L(\pi) = \mathrm{Id}_{L(G)}$ 且 F = Ker $\pi$。

$$
\begin{array}{ccc}
S & \xrightarrow{\sigma} & S' \\
\downarrow \pi & & \downarrow \lambda \\
G & \xrightarrow{\gamma} & G \\
& \searrow \phi & \swarrow \psi \\
& & H
\end{array}
$$

对于每一个复数李群 H 和每个 $\mathbf{R}$-解析态射 $\phi$ G 到 H，$L(\phi): g \to L(H)$ 都有一个唯一的 $\mathbf{C}$-线性扩张到 $g_C$ 并且这个扩张是形式 $L(\phi^*)$，其中 $\phi^*$ 是 S' 到 H 的 $\mathbf{C}$ 解析态射。然后
$$
L(\phi \circ \pi) = L(\phi) \circ L(\pi) = L(\phi) = L(\phi^*) \circ L(\sigma) = L(\phi^* \circ \sigma)
$$
因此$\phi \circ \pi = \phi^* \circ \sigma$。因此$\phi^*(\sigma(F)) = \phi(\pi(F)) = \{e\}$，从而
$$
\sigma(F) \subset \mathrm{Ker}\, \phi^*.
$$
令 P 为变量 $\phi$ 的 $\mathrm{Ker}\, \phi^*$ 的交。这是 S' 的正常谎言子群（no. 2，推论 3 到命题 1）。设 $\tilde{G} = S'/P$ 和 λ: S' → Ġ 为规范的态射。则 σ(F) ⊂ P，因此存在且仅有一个 G 到 Ġ 的 R 解析态射 γ，使得 γ ∘ π = λ ∘ σ。如果 ψ: Ġ → H 表示当经过为商时从 φ* 导出的态射，则

$$(\varphi \circ \gamma) \circ \pi = \psi \circ (\lambda \circ \sigma) = \varphi^* \circ \sigma = \varphi \circ \pi$$

从而 ψ ∘ γ = φ。显然，L(ψ) 以及 ψ 由等式 ψ ∘ γ = φ 唯一确定。这样我们就证明了有序对 (\tilde{G}, γ) 具有性质 (i) 和 (iii)。

(b) 现在我们讨论一般情况。设 F 为 G 的恒等分量，M = G/F，i: F → G 和 p: G → M 为规范态射。我们将证明的部分 (a) 应用于 F。我们得到有序对 (\tilde{F}, δ)。对于所有 g ∈ G，Int g|F = ω'(g) 是 F 的自同构。通过 \tilde{F} 的泛性质，复数李群 \tilde{F} 中存在且仅有一个自同构 ω(g)，使得 δ ∘ ω'(g) = ω(g) ∘ δ。显然 ω 是 G 到 Aut(\tilde{H}) 的态射。如果 g ∈ G 且 f ∈ F，则

$$\delta(gf g^{-1}) = (\delta \circ \omega'(g))(f) = (\omega(g) \circ \delta)(f) = \omega(g)(\delta(f)).$$

如果 f ∈ F，则 δ ∘ (Int_F f) = (Int_\tilde{F} δ(f)) ∘ δ 并且 Int_\tilde{F} δ(f) 是复数李群 \tilde{F} 的自同构；因此 Int_\tilde{F} δ(f) = ω(f)。

因此可以应用引理 7，得到图表

$$
\begin{array}{ccccc}
F & \xrightarrow{i} & G & \xrightarrow{p} & M \\
\downarrow{\delta} & & \downarrow{\gamma} & & \downarrow{\mathrm{Id}} \\
\tilde{F} & \xrightarrow{\tilde{i}} & \tilde{G} & \xrightarrow{\tilde{p}} & M.
\end{array}
$$

令 \tilde{F} 通过 ī 与 \tilde{G} 的正常子群等价。 群 \tilde{G} 由 \tilde{F} 和 γ(G) 生成；因此，由\tilde{G}的元素定义的\tilde{F}的自同构是复数李群结构的自同构。到§ 1, no. 9，命题 18，\tilde{G} 上存在且仅有一个复数李群结构，使得\tilde{F} 是\tilde{G} 的开谎言子群。从此以后 \tilde{G} 将具有这个结构。由于 δ 是 R 解析的，因此 γ 是 R 解析的。

有序对 (\tilde{G}, γ) 的性质 (iii) 为命题。我们证明它有性质 (i)。设 H 为复数李群，ψ 为 G 到 H 的 R 解析态射。存在 \tilde{F} 到 H 的 C 解析态射 η，使得 η ∘ δ = φ|F。令 g ∈ G。 映射

$$f \mapsto \eta(\omega(g)f), \quad f \mapsto \phi(g)\eta(f)\phi(g)^{-1}$$

将 \tilde{F} 转化为 H 是C-解析态射；它们重合在 δ(F) 上，对于，如果 f' ∈ F，则

$$\phi(g)\eta(\delta(f'))\phi(g)^{-1} = \phi(g)\phi(f')\phi(g)^{-1} = \phi(gf'g^{-1})$$
$$= \eta(\delta(gf'g^{-1})) = \eta(\omega(g)\delta(f'));$$

因此 $\eta(\omega(g)f) = \phi(g)\eta(f)\phi(g)^{-1}$ 对于所有 $g \in G$ 和所有 $f \in \tilde{F}$。如果$G'$表示$G$相对于$\tilde{F}$相对于$\omega$的半直接乘积，则存在群$G'$到$H$的态射$\zeta$，其中重合与$\phi$ 搭配$G$ 以及$\eta$ 搭配$\tilde{F}$。对于$f \in F$，
$$
\zeta(\delta(f^{-1})f) = \eta(\delta(f^{-1}))\phi(f) = \phi(f^{-1})\phi(f) = e.
$$
因此，$\zeta$定义在经过上除以$\tilde{G}$的商态射$\psi$除以$H$。然后$\psi \circ \gamma = \phi$和$\psi \circ \tilde{i} = \eta$；后者不等式意味着$\psi$是$\mathbf{C}$解析的。

最后，让$\psi'$是$\tilde{G}$的$\mathbf{C}$解析态射到$H$，使得$\phi = \phi' \circ \gamma$。然后
$$
\psi' \circ \tilde{i} \circ \delta = \psi' \circ \gamma \circ i = \phi \circ i = \psi \circ \tilde{i} \circ \delta
$$
因此$\psi' \circ \tilde{i} = \psi \circ \tilde{i}$。由于$\tilde{G}$是由$\tilde{i}(\tilde{F})$和$\gamma(G)$生成的，$\psi' = \psi$。

#### 定义 4 {#lie-iii-s6-def-4 .statement tag=0AG6}

$(G, \gamma)$，或简称为$\tilde{G}$，被称为$G$的万能复化。

#### 注 {#lie-iii-s6-n10-rem-1 .statement tag=0AG7}

(1) 设$(\tilde{G}, \gamma)$为$G$的万复化。令$G_0$（或$\tilde{G}_0$）为$G$（或$\tilde{G}$）的恒等分量。通过命题 20 的证明，$(\tilde{G}_0, \gamma|G_0)$ 是$G_0$ 和复合态射的万有复化
$$
G \to \tilde{G} \to \tilde{G}/\tilde{G}_0
$$
定义在经过上除以 $G/G_0$ 的商同构到 $\tilde{G}/\tilde{G}_0$。

(2) 假设$G$是单连通的。令 $g = L(G)$、$g_C$ 为$g$、$S'$ 的单连通复形李群与李代数 $g_C$ 和 $G$ 的$\sigma$ 态射复化为 $S'$，使得$L(\sigma)$ 是 $g$ 的典范嵌入变成 $g_C$。我们再次使用命题20、部分(a)的证明记号。如果$H = S'$和$\phi = \sigma$，则$\phi^* = \mathrm{Id}_{S'}$。因此$(S', \sigma)$是$G$的万有复数。 注 $\sigma$ 不是一般单射 (习题 16)；然而*它的核是离散的*，因为$L(\sigma)$是单射的。另一方面，令$\theta$为由$g$定义的$g_C$的对合，并令$\eta$为$S'$的基础实李群的相应的自同构；设${S'}^\eta$为$S'$点集合在$\eta$下不变；这是 $S'$ 的真实谎言子群和李代数 $g$（§ 3, no. 8，推论 1 到命题 29）。根据no. 1，推论1到命题1，$\sigma(G)$是$S'$与李代数$g$的实积分子群，因此$\sigma(G)$*是*${S'}^\eta$的恒等分量；特别是$\sigma(G)$是$S'$的真实谎言子群。

### 习题 {#lie-iii-s6-exercises}

参见[习题为 § 6](exercises/s6/)。
