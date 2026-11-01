---
book: int
book_title: Integration
chapter: VI
chapter_title: VECTORIAL INTEGRATION
section: 0
section_title: Complements on topological vector spaces
appendix: true
lang: zh
source: int-i-vi
pdf_pages: 0443-0447
extraction: ocr
subsections:
    - "no": 1
      title: Bilinear forms and linear mappings
      page: 0
      pdf_page: 443
    - "no": 2
      title: Some types of spaces having the property (GDF)
      page: 54
      pdf_page: 445
statements: 6
exercises: 0
content_sha256: a212010e3a33f945bb4ce710ecf43f903673dee7f5d8cad5789233f71ec52a26
translated_from: content/en/int/VI/A_a_complements_on_topological_vector_spaces.md
translation_method: google
source_content_sha256: 02f42b389f24a36ddcc58d04da30cbfa4dd5961e3192d18701403d3e92f17929
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: f0115d05fb445224cb5e3cd4373f07c004ca2522a1e2fc5ef92666b94ea3d118
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 附录

# 拓扑补集向量空间

### 1. 双线性形式和线性映射

令$(F_1, G_1), (F_2, G_2)$为（实数或复数）向量空间的两个对分离对偶性（TVS，II, §6, No. 1）；假设每个空间都配备了相应的弱拓扑（*loc.cit.*，No. 2）；如果A和B是这些空间中的任何两个，像往常一样，我们用A到B中的连续线性映射的$\mathscr{L}(A; B)$向量空间表示，并用$A \times B$上*单独连续*双线性形式的$\mathfrak{B}(A, B)$向量空间表示。

对于$F_1 \times F_2$上的每个单独连续的双线性形式$\Phi$，$x_1 \mapsto \Phi(x_1, x_2)$是$F_1$上的连续线性形式，因此存在且仅一个元素${}^r\Phi(x_2) \in G_1$使得

$$
\Phi(x_1, x_2) = \langle x_1, {}^r\Phi(x_2) \rangle
$$

对于$x_1 \in F_1, x_2 \in F_2$（TVS，III, §5, No. 1，（1））。此外，这个公式表明映射$x_2 \mapsto {}^r\Phi(x_2)$对于$F_2$和$G_1$的（弱）拓扑是线性且连续的。相反，对于$F_2$到$G_1$的每个连续线性映射$u$，$(x_1, x_2) \mapsto \Phi(x_1, x_2) = \langle x_1, u(x_2) \rangle$是$F_1 \times F_2$和${}^r\Phi = u$上的单独连续双线性形式。因此 $\mathfrak{B}(F_1, F_2)$ 的定义同构 $r : \Phi \mapsto {}^r\Phi$ 到$\mathscr{L}(F_2; G_1)$，据说是*规范*。

同样，公式

$$
\Phi(x_1, x_2) = \langle {}^l\Phi(x_1), x_2 \rangle
$$

将$\mathfrak{B}(F_1, F_2)$的定义*典范同构*$l : \Phi \mapsto {}^l\Phi$放到$\mathscr{L}(F_1; G_2)$上；显然有交换律图表

$$
\begin{array}{ccc}
\mathscr{B}(F_1, F_2) & & \\
l & l^{-1} & r^{-1} \\
& & \\
\mathscr{L}(F_1; G_2) & \xleftarrow{t} & \mathscr{L}(F_2; G_1)
\end{array}
$$

其中$t$是转置$u \mapsto {}^t u$的同构。鉴于$G_1$和$G_2$上的弱拓扑定义，而且直接的，当$\mathscr{B}(F_1, F_2)$、$\mathscr{L}(F_1; G_2)$、$\mathscr{L}(F_2; G_1)$配备逐点收敛的拓扑时，前面图表中的同构为同构拓扑向量空间结构。

现在令 $E, F$ 为两个 Hausdorff 局部凸空间、$E', F'$ 它们各自的对偶；我们用配备了弱拓扑$\sigma(E, E')$，$\sigma(F, F')$的$E_\sigma, F_\sigma$空间$E, F$表示，并用配备了弱拓扑$\sigma(E', E)$，$\sigma(F', F)$的$E'_s, F'_s$空间$E', F'$表示。 因此，前面的注在三个空间、$\mathscr{B}(E_\sigma, F'_s)$、$\mathscr{L}(E_\sigma; F_\sigma)$和$\mathscr{L}(F'_s; E'_s)$之间建立了典范同构，并且还在三个空间$\mathscr{B}(E_\sigma, F_\sigma)$、$\mathscr{L}(E_\sigma; F'_s)$和$\mathscr{L}(F_\sigma; E'_s)$之间建立了典范同构。 人们会发现，$\mathscr{B}(E_\sigma, F_\sigma)$也等于$E \times F$上单独连续的双线性形式的空间$\mathscr{B}(E, F)$（$E$和$F$配备了它们的原始拓扑），因为$E$（分别为$F$）上的每个连续线性形式都是连续的$E_\sigma$（分别$F_\sigma$），反之亦然（TVS、II, §6, No. 1 和 No. 2，第 3 条）。

令$\mathscr{B}(E, F)$为$E \times F$上连续双线性形式的空间（$E$和$F$配备其原始拓扑）；然后$\mathscr{B}(E, F) \subset \mathscr{B}(E, F)$。

#### 命题 1 {#int-vi-a0-prop-1 .statement tag=09CS}

*对于双线性形式$\Phi \in \mathscr{B}(E, F)$到属于到$\mathscr{B}(E, F)$，$E$中存在0邻域是充分必要的，其${}^l \Phi$下的像是$F'$的等连续子集。*

因为，说$\Phi$是连续的意味着$E$（或$F$）中存在0的平衡凸邻域$V$（或$W$），使得$|\Phi(x, y)| \leq 1$对于$x \in V$，$y \in W$；可以将$x \in V$、$y \in W$写成$|\langle {}^l \Phi(x), y \rangle| \leq 1$，也可以写成${}^l \Phi(V) \subset W^\circ$； 从而命题，考虑到$F'$的每个等连续子集都包含在$F$中0邻域的极坐标中。

#### 推论 {#int-vi-a0-n1-cor-1 .statement tag=09CT}

*如果$\Phi$是$E \times F$上的连续双线性形式，则${}^l \Phi$是$E$的连续线性映射进入$F$的强对偶$F'_b$。此外，如果 $E$ 和 $F$ 被标准化为空间，则 $\|{}^l \Phi\| = \|\Phi\|$。*

第一个断言由命题 1 得出，事实上$F'_b$ 中 0 的每个邻域都吸收了 $F'$ 的每个等连续子集。如果 $E$ 和 $F$ 被标准化，那么

$$
\|\Phi\| = \sup_{\|x\| \leq 1, \|y\| \leq 1} |\Phi(x, y)| = \sup_{\|x\| \leq 1} \left( \sup_{\|y\| \leq 1} |\langle l \Phi(x), y \rangle| \right)
= \sup_{\|x\| \leq 1} \|l \Phi(x)\| = \|l \Phi\|,
$$

从而第二个断言。

交换E和F的作用，得到类似于命题1及其推论线性映射$r \Phi$的结果；我们把陈述它们的任务留给了读者。

### 2. 空间中的一些型具有性质 (GDF)

我们已经知道每个 Fréchet 空间都有性质 (GDF)（TVS，I, §3, No. 3，Th.1 的 Cor. 5）。

#### 命题 2 {#int-vi-a0-prop-2 .statement tag=09CU}

— 令 E 为向量空间，$(F_\alpha)_{\alpha \in A}$ 具有性质 (GDF) 的局部紧致空间族，对于每个$\alpha \in A$，令 $h_\alpha$ 为 E 中 $F_\alpha$ 的线性映射。如果 E 配备有最精细的局部凸拓扑，则使得$h_\alpha$连续，则 E 有性质 (GDF)。

令E的$u$为Banach空间B中的线性映射，使得$u$的图$\Gamma$的点的每个收敛序列的$E \times B$中的每个极限也为属于 $\Gamma$。足以证明，对于每个$\alpha \in A$，$u \circ h_\alpha$在$F_\alpha$上连续（TVS，II, §4, No. 4，命题5）。现在，令$(x_n)$为$F_\alpha$的元素的序列，具有极限$a$，并且序列$\left(u(h_\alpha(x_n))\right)$具有极限$b \in B$。由于$h_\alpha$是连续的，$h_\alpha(a)$是E中序列$(h_\alpha(x_n))$的极限；因此，通过假设 $b = u(h_\alpha(a))$，并且由于 $F_\alpha$ 有性质 (GDF)，$u \circ h_\alpha$ 是连续的。

#### 推论{#int-vi-a0-n2-cor-1 .statement tag=09CV}

— 具有性质 (GDF) 的局部凸空间的每个商空间都具有性质 (GDF)。

#### 命题 3 {#int-vi-a0-prop-3 .statement tag=09CW}

— 自反 Fréchet 空间的强对偶有性质 (GDF)。

这是提案 2 的推论和以下引理（或 TVS、IV, §3, No. 4、提案 4）：

#### 引理 {#int-vi-a0-n2-lem-1 .statement tag=09CX}

设 F 为 Fréchet 空间，$F'$ 为强对偶，$F''$ 为对偶。如果$F''$的每个子集，以$\sigma(F'', F')$为界，都包含在F的有界子集的闭包（对于$\sigma(F'', F')$）中，则$F'$是Banach 空间的序列的直极限。

例如，令 $(V_n)$ 为 F 中 0 的凸、平衡、闭邻域的递减基本序列。对于每个整数 $n$，令 $G_n$ 为$F'$ 的线性子空间，由 $V_n$ 的极$V_n^\circ$ 生成。在$G_n$中，$V_n^\circ$是吸收凸集合，因此其标距$p_n$在$G_n$上为范数；此外，$V_n^\circ$是强对偶$F'$的完整子集（TVS，III, §3, No. 8，第11条命题）；因此$G_n$，配备范数$p_n$，是Banach空间（GT，III, §3, No. 5，第9号提案的Cor.2）。我们将证明$F'$上的强拓扑是$G_n$上这些Banach空间拓扑的直极限，或者再次证明，对于$F'$的强闭、平衡、凸子集U作为0的强邻域，它吸收每个$V_n^\circ$。显然这个条件是必须的；要想证明它是充分的，只要证明 U 包含一桶 $F'$ 就足够了。事实上，它在 $F''$ 中的极点 $U^\circ$ 将被限制为 $\sigma(F'', F')$，因此，通过假设，将包含在 F 的有界子集 B 的闭包（对于 $\sigma(F'', F')$）中，从中可以结论 U（对于$\sigma(F', F'')$ 是封闭的） 包含于 0 的强邻域$B^\circ$（TVS、II, §6, No. 3、Th.1 和§8, No. 4）。

到假设，对于每个整数$n$，都存在数$\lambda_n > 0$，使得$\lambda_n V_n^\circ \subset \frac{1}{2}U$；令$A_n$为$i \leq n$的$\lambda_i V_i^\circ$的并的凸包络。然后每$n$对应$A_n \subset \frac{1}{2}U$；令 W 为 $A_n$ 的并； W是一个凸出的、平衡的、吸收性的集合，包含在$\frac{1}{2}U$中，并且足以表明它的强封闭性（它是一个桶）包含在U中。

因而，令$x'$是$F'$的点，而不是属于到U。由于每个$V_n^\circ$对于$\sigma(F', F)$来说都是紧致的，$A_n$也是如此（TVS，II, §2, No. 6，命题15），并且从$x' \notin 2A_n$开始，存在元素 $x_n$ 属于到 F 中$A_n$ 的极点，使得 $\langle x', x_n \rangle = 2$（TVS，II, §5, No. 3，命题 4）。 序列$(x_n)$在F中有界：对于每个$y' \in F'$属于到一些$V_k^\circ$，因而$|\langle y', x_n \rangle| \leq \lambda_k^{-1}$对于$n \geq k$，从而我们的断言（TVS，IV, §1, No. 1，提案1）。令 C 为 F 包含所有$x_n$ 中的有界平衡凸集合；那么$C^\circ$是$F'$中0的邻域，$F''$中$C^\circ$的极$C^{\circ\circ}$对于$\sigma(F'', F')$来说是紧致的（TVS，III, §3, No. 4，第4条命题的Cor.2和第7条命题No. 5）。因而，可以看到序列$(x_n)$在$F''$中对于$\sigma(F'', F')$有一个集群点$x''$；显然，$\langle x', x'' \rangle = 2$，另一方面，对于每个$n$，$x''$属于到$F''$中$A_n$的极点，因此到$F''$中W的$W^\circ$极点。由此，$x' \notin W^{\circ\circ}$的一个结论，因此不在$\sigma(F', F'')$的W闭包中（TVS，II, §6, No. 3，Th.1和§8, No. 4），因而*更不必说*对于强拓扑，完成证明。

习题
