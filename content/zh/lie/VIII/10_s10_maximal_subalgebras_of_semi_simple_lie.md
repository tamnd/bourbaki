---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 10
section_title: Maximal subalgebras of semi-simple Lie algebras
lang: zh
source: lie-vii-ix
book_pages: 159-163, 260-261
pdf_pages: 0167-0171, 0268-0269
extraction: native
statements: 8
exercises: 7
content_sha256: ff5eff7fe411642a92ada1eb87365ecca3828e8d1ef8b97f549e3a0bbdf7f2c7
translated_from: content/en/lie/VIII/10_s10_maximal_subalgebras_of_semi_simple_lie.md
translation_method: google
source_content_sha256: 345f66620b2c4fae05d0eb5d76aa4f165ea7875de6e8bd6a97f18302eec6a845
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: a2408c08112a7ae28ad8f5f8476b612a00072d874b942020ac4b44bb54cacf6f
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 10。 极大子代数 / 半单李代数

#### 定理 1 {#lie-viii-s10-thm-1 .statement tag=016L}

令 V 为有限维向量空间，$\mathfrak{g}$ $\mathfrak{g}\mathfrak{l}(V),\mathfrak{q}$ $\mathfrak{g}$ 的谎言子代数中的还原谎言子代数以及 $\Phi$ 双线性形式 $(x, y) \rightarrow$ Tr($xy$) 上$\mathfrak{g}\times \mathfrak{g}$。假设$\mathfrak{q}$相对于$\Phi$的正交补$\mathfrak{n}$是$\mathfrak{g}$的子代数、V的幂零自同态的由……组成。那么$\mathfrak{q}$是$\mathfrak{g}$的抛物线子代数。

$a)\mathfrak{q}$ 是$\mathfrak{g}:$ 中$\mathfrak{n}$ 的标准化器，令$\mathfrak{p}$ 为该标准化器。设$x\in \mathfrak{q}$和$y\in \mathfrak{n}$；对于所有 $z\in \mathfrak{q}$，我们有 $[z, x]\in \mathfrak{q}$，所以

$$
\Phi ([x, y], z) =\Phi (y,[z, x]) = 0
$$

其他字，$[x, y]\in \mathfrak{n}$。因此$\mathfrak{q}\subset \mathfrak{p}$。由于$\mathfrak{n}$是V的幂零自同态的$\mathfrak{p}$由……组成的理想，因此P相对于$\Phi$与$\mathfrak{n}$正交（第I，no. 3，Prop. $4d$）$)$。由于$\Phi$是非简并的$^4,\mathfrak{p}\subset \mathfrak{q}$，因此我们的断言。

b) $\mathfrak{g}\mathfrak{l}(V)$ 中存在还原谎言子代数 $\mathfrak{m}$，使得 $\mathfrak{q}$ 是 $\mathfrak{m}$ 的半直乘积，且 $\mathfrak{n}:$ 令 $\mathfrak{n}_V(\mathfrak{q})$ 为 $\mathfrak{q}$ 的理想最大的由……组成幂零自同态 V。那么$\mathfrak{n}_V(\mathfrak{q})$包含$\mathfrak{n}$，它与$\mathfrak{q}($loc正交。引）；因此$\mathfrak{n}=\mathfrak{n}_V(\mathfrak{q})$。此外，$\mathfrak{g}$在$\mathfrak{g}\mathfrak{l}(V)$中被还原为假设，因此可分解（第VII, §5, no. 1章，命题2）；由于 $\mathfrak{q}$ 是 $\mathfrak{g}$ 的交，并且在 $\mathfrak{g}\mathfrak{l}$(V) 中使用 $\mathfrak{n}$ 标准化器，因此它是可分解李代数（参见第 3 条命题第 1 条）。因此，我们的断言源自第 7 章的命题 7。 VII, §5, no. 3。

选择嘉当子代数$\mathfrak{h}$共$\mathfrak{m}$；用$\mathfrak{g}_1$表示$\mathfrak{h}$在$\mathfrak{g}$中的交换子，并放入$\mathfrak{q}_1=\mathfrak{q}\cap \mathfrak{g}_1,\mathfrak{n}_1=\mathfrak{n}\cap \mathfrak{g}_1$。

c) 李代数 $\mathfrak{g}_1,\mathfrak{q}_1$ 和 $\mathfrak{n}_1$ 满足与 $\mathfrak{g},\mathfrak{q}$ 和 $\mathfrak{n}:$ 相同的假设，因为 $\mathfrak{m}$ 在 $\mathfrak{g}\mathfrak{l}$(V) 中可还原，$\mathfrak{h}$ 是可交换的并且由半单组成V 的自同态（第 VII, §2, no. 4 章，第 2 章第 3 章）。因而，$\mathfrak{g}_1=\mathfrak{g}^0(\mathfrak{h})$在$\mathfrak{g}$（第VII, §1, no. 3章，第11条命题）中是可还原的，因此在$\mathfrak{g}\mathfrak{l}(V)$（第I, §6, no. 6章，第7条命题第2条）中也是可还原的。显然$\mathfrak{n}_1$是由

$^4$ 令$\mathfrak{z}$为$\mathfrak{g}$相对于$\Phi$的正交补集；这是$\mathfrak{n}$中包含的$\mathfrak{g}$的理想，因而$\mathfrak{z}$的每个元素都是幂零的。 $\mathfrak{g}$的恒等式表示是半单（第7章第I, §6，Cor.1）。因而$\mathfrak{z}= 0$（第I, §4, no. 3、引理2章）。 幂零自同态 V。由于$\mathfrak{h}$是$\mathfrak{q}$的子代数，在$\mathfrak{g}\mathfrak{l}$(V)中约简，$\mathfrak{h}$在$\mathfrak{q}$上的伴随表示是半单；由构造，$\mathfrak{q}_1$是ad$_{\mathfrak{q}}(\mathfrak{h})$的不变量的集合，所以$\mathfrak{q}=\mathfrak{q}_1+ [\mathfrak{h},\mathfrak{q}]$（第I, §3, no. 5章，第6条命题）。自从

$$
\Phi (\mathfrak{g}_1,[\mathfrak{h},\mathfrak{q}]) =\Phi ([\mathfrak{h},\mathfrak{g}_1],\mathfrak{q}) = 0
$$

$\mathfrak{g}_1$的元素与$\mathfrak{q}_1$正交当且仅当它与$\mathfrak{q}$正交；因而，$\mathfrak{n}_1=\mathfrak{g}_1\cap \mathfrak{n}$是$\mathfrak{q}_1$在$\mathfrak{g}_1$中的正交补集。

d) $\mathfrak{m}$的嘉当子代数$\mathfrak{h}$是$\mathfrak{g}:$的嘉当子代数我们有$\mathfrak{q}=\mathfrak{m}\oplus \mathfrak{n}$和$\mathfrak{h}=\mathfrak{m}\cap \mathfrak{g}_1$，所以$\mathfrak{q}_1=\mathfrak{h}\oplus \mathfrak{n}_1$是直接的。此外，$[\mathfrak{h},\mathfrak{n}_1] = 0,\mathfrak{h}$是可交换的，$\mathfrak{n}_1$是幂零的，所以李代数$\mathfrak{q}_1$是幂零的。由a) 且$c),\mathfrak{q}_1$是$\mathfrak{n}_1$在$\mathfrak{g}_1$的标准化； 更不必说$,\mathfrak{q}_1$ 等于$\mathfrak{g}_1$ 中的归一化器，因此是$\mathfrak{g}_1$ 的嘉当子代数。由于 $\mathfrak{g}_1$ 在 $\mathfrak{g}\mathfrak{l}$(V) 中被还原，因此可以从 Cor. 3 Th。第 2 章VII, §2, no. 4，即$\mathfrak{q}_1$由V的半单自同态组成；因而，由于$\mathfrak{n}_1$是由幂零自同态和V组成，所以我们有$\mathfrak{n}_1= 0$。因而，$\mathfrak{h}=\mathfrak{q}_1$是$\mathfrak{g}_1$的嘉当子代数，并且由于$\mathfrak{g}_1$标准化了$\mathfrak{h}$，我们有$\mathfrak{h}=\mathfrak{g}_1$。这样，我们就证明了$\mathfrak{h}$的每一个元素都是$\mathfrak{g}$的半单元素，$\mathfrak{h}$在$\mathfrak{g}$中的交换子等于$\mathfrak{h}$；由此可见 $\mathfrak{h}=\mathfrak{g}^0(\mathfrak{h})$，因而 $\mathfrak{h}$ 是 $\mathfrak{g}$ 的嘉当子代数。

由上式可知，$e)\mathfrak{q}$是$\mathfrak{g}:$的抛物线子代数，$\mathfrak{h}$是$\mathfrak{g},\mathfrak{n}$的嘉当子代数，由$\mathfrak{g}$的幂零元和$[\mathfrak{h},\mathfrak{n}]\subset \mathfrak{n}$组成。设$\overline{k}$为$k$中的代数闭包；通过定义，$\mathfrak{q}$ 在 $\mathfrak{g}$ 中是抛物线，当且仅当 $\overline{k}\otimes_k\mathfrak{q}$ 是 $\overline{k}\otimes_k\mathfrak{g}$ 的抛物线子代数。上述属性由标量的扩张保留，对于证明，我们可以将自己限制在$\mathfrak{h}$是分裂的情况。令R为$(\mathfrak{g},\mathfrak{h})$中的根系；根据§3, no. 1的命题2(v)，存在R的子集 P，使得$P\cap (-P) =\emptyset$和$\mathfrak{n}=\sum_{\alpha\in P}\mathfrak{g}^{\alpha}$。

令$P'$为根$\alpha$的集合，使得$-\alpha  \notin P$；我们有$P'\cup (-P') = R$，$\mathfrak{n}$在$\mathfrak{g}$中的正交补$\mathfrak{q}$等于$\mathfrak{h}+\sum_{\alpha\in P'}\mathfrak{g}^{\alpha}$。我们有

证明$\mathfrak{q}$是抛物线。 Q.E.D.

#### 引理 1 {#lie-viii-s10-lem-1 .statement tag=016M}

令 $\mathfrak{g}$ 为半单李代数，V 向量空间，$\rho$ 线性表示 ($\mathfrak{g}$) 在 V，D 向量子空间 (V$,\mathfrak{h}$) $\mathfrak{g},\mathfrak{s}$ 的嘉当子代数（分别为 $\mathfrak{s}'$） $x\in \mathfrak{h}$ 的集合，使得 $\rho (x)D\subset D$（分别为 $\rho (x)D = 0$），以及 $\mathfrak{g}$ 上的 $\Phi$ 双线性形式与 $^5$ 相关联$\rho$。

(i) 如果$\mathfrak{h}$是分裂，向量子空间$\mathfrak{s}$和$\mathfrak{h}$的$\mathfrak{s}'$在$\mathbf{Q}$上是有理数。

(ii) 如果 $\rho$ 是单射的，$\Phi$ 到 $\mathfrak{s}$（或 $\mathfrak{s}'$）的限制是非简并的。

假设嘉当子代数$\mathfrak{h}$为分裂。令$d$为D的维数；把$W =\bigwedge^d(V)$和$\sigma =\bigwedge^d(\rho )$；还用 D 的 $(e_1, . . . , e_d)$ 基和$e=e_1\wedge  \cdots  \wedge e_d$ 表示与 D 相关的可分解 $d$ 向量。令 P 相对于 $\mathfrak{h}$ 为 $\sigma$ 的权的集合；用 $W^\mu$ 子空间表示

$^5$ 在其他字中，$\Phi (x, y) =$ Tr($\rho (x)\rho (y)$) 代表$x, y\in \mathfrak{g}$。 W 与权 $\mu$ 相关联，并放置 $e=\sum_{\mu\in P}e^\mu$（对于所有的$e^\mu\in W^\mu$

$\mu\in P)$；最后，令$P'$为权$\mu$的集合，使得$e^\mu\not= 0$，并令$P''$为$P'$的元素之差的集合。设$x$在$\mathfrak{h}$中；那么$x$属于到$\mathfrak{s}$当且仅当$k$中存在$c$使得$\rho (x).e=c.e$（第VII, §5, no. 4，引理2（i））。从$\rho (x).e^\mu=\mu(x).e^\mu$开始，我们看到$x\in \mathfrak{s}$相当于关系“对于所有$\mu\in P''$来说$\mu(x) = 0$”。现在，$\mathfrak{h}$的$\mathbf{Q}$结构是$\mathfrak{h}$的$\mathbf{Q}$向量子空间$\mathfrak{h}_{\mathbf{Q}}$，由共根$H_{\alpha}$生成，并且$P''$中的所有$\mu$取有理值 $\mathfrak{h}_{\mathbf{Q}}$；由此得出（代数，第II, §8, no. 4，第 5 条命题）$\mathfrak{s}$ 是 $\mathfrak{h}$ 有理数超过 $\mathbf{Q}$ 的子空间。

对于任何权$\mu\in P$，令$p_\mu$是投影到与分解$V =\bigoplus_{\mu\in P}V^\mu$相关联的$V^\mu$；用 $\mu\in P$ 的 $P_1$ 集合表示，使得

$p_\mu(D)\not= 0$。 $\mathfrak{s}'$为$P_1$元素核($\mathfrak{h}$)交为直接的；与$\mathfrak{s}$相同，$\mathfrak{s}'$是$\mathfrak{h}$有理数超过$\mathbf{Q}$的子空间。这就证明了(i)。

通过标量的扩张，足以证明(ii)何时$k$是代数闭的，因此当$\mathfrak{h}$是分裂时。设$\mathfrak{m}$是$\mathfrak{h}$有理数$\mathbf{Q}$的向量子空间；对于$\mathfrak{m}_{\mathbf{Q}}=\mathfrak{m}\cap \mathfrak{h}_{\mathbf{Q}}$中的所有非零$x$，我们通过Cor得到$\Phi (x, x)>0$。 §7, no. 1 的第 1 号提案。 $\Phi$到$\mathfrak{m}_{\mathbf{Q}}$的限制是非简并的，因此$\Phi$到$\mathfrak{m}$的限制也是非简并的，因为$\mathfrak{m}$与$k\otimes_{\mathbf{Q}}\mathfrak{m}_{\mathbf{Q}}$自然同构。

#### 定义 1 {#lie-viii-s10-def-1 .statement tag=016N}

设$\mathfrak{q}$是半单李代数$\mathfrak{g}$的谎言子代数。那么，如果对于所有$x\in \mathfrak{q}$、半单以及$x$在$\mathfrak{g}$属于到$\mathfrak{q}$中的幂零分量，则称$\mathfrak{q}$在$\mathfrak{g}$中可分解。用$\mathfrak{q}$的根的元素$x$的$\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q})$集合表示，使得ad$_{\mathfrak{g}}x$幂零的。

令 $\rho$ 为 $\mathfrak{g}$ 在有限维向量空间 V 上的单射表示。我们知道（第 I, §6, no. 3，第 3 章）$\mathfrak{g}$ 的元素 $x$ 是半单（或幂零）当且仅当 V 的自同态 $\rho (x)$ 是半单（或幂零）。幂零的）。紧接着，代数$\mathfrak{q}$可分解为$\mathfrak{g}$当且仅当$\rho (\mathfrak{q})$是第1章定义1意义上的$\mathfrak{g}\mathfrak{l}(V)$的可分解子代数。 VII, §5, no. 1。与第 52 章的记号 VII, §5, no. 3，我们还有

$$
\rho (\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q})) =\mathfrak{n}_V(\rho (\mathfrak{q}))
$$

#### 定理 2 {#lie-viii-s10-thm-2 .statement tag=016O}

令$\mathfrak{g}$为半单李代数，幂零元的$\mathfrak{g}$由……组成的$\mathfrak{n}$子代数，$\mathfrak{q}$$\mathfrak{g}$中$\mathfrak{n}$的归一化器。假设$\mathfrak{n}$是$\mathfrak{q}$的根部幂零元的集合。那么$\mathfrak{q}$是抛物线。

注首先，$\mathfrak{q}$ 是可分解的（第 VII, §5, no. 1 章，第 3 条命题第 1 条）。由 Th. 1、只要证明$\mathfrak{q}$是$\mathfrak{n}$相对于$\mathfrak{g}$的Killing形式$\Phi$的正交补$\mathfrak{n}^0$即可。我们知道$\mathfrak{q}\subset \mathfrak{n}^0$（第I, §4, no. 3章，提案$4d$）$)$。由章。 VII, §5, no. 3，第7条命题，$\mathfrak{q}$存在子代数$\mathfrak{m}$，在$\mathfrak{g}$约简，使得$\mathfrak{q}$是$\mathfrak{m}$和$\mathfrak{n}$的半直接乘积。我们证明$\Phi$到$\mathfrak{m}$的限制是非简并的。设$\mathfrak{c}$为$\mathfrak{m}$中的中心。我们有第 19 章的$\Phi ([\mathfrak{m},\mathfrak{m}],\mathfrak{c}) = 0$。 I, §5, no. 5，第 5 章，以及 $\Phi$ 到 $[\mathfrak{m},\mathfrak{m}]$ 的限制是非退化的。 I, §6, no. 1，命题 1。 $\Phi$ 到 $\mathfrak{c}$ 中的限制是否是非简并的，还有待观察。设$\mathfrak{k}$为$[\mathfrak{m},\mathfrak{m}]$的嘉当子代数；则 $\mathfrak{k}\oplus \mathfrak{c}$ 在 $\mathfrak{g}$ 中可交换且可还原。令 $\mathfrak{h}$ 为 $\mathfrak{g}$ 包含于 $\mathfrak{k}\oplus \mathfrak{c}$ 中的嘉当子代数（第 VII, §2, no. 3 章，第 10 条命题）。那么$\mathfrak{h}\cap \mathfrak{q}$就是$\mathfrak{q}$包含于$\mathfrak{k}\oplus \mathfrak{c}$的交换子代数，而ad$_{\mathfrak{q}}x$对于所有$x\in \mathfrak{h}\cap \mathfrak{q}$来说就是半单；因而$\mathfrak{h}\cap \mathfrak{q}$包含在$\mathfrak{q}$的嘉当子代数$\mathfrak{h}'$中（第VII, §2, no. 3章，第10条命题）；令$f$为$\mathfrak{q}$的投影到$\mathfrak{m}$，以及核$\mathfrak{n}$；那么$f(\mathfrak{h}')$是$\mathfrak{m}$的嘉当子代数（第VII, §2, no. 1章，第4条命题第2条）包含于$\mathfrak{k}\oplus \mathfrak{c}$，因此等于$\mathfrak{k}\oplus \mathfrak{c}$；这证明了$f(\mathfrak{h}\cap \mathfrak{q}) =\mathfrak{k}\oplus \mathfrak{c}$，并且由于$\mathfrak{h}$的每个元素都是$\mathfrak{g}$中的半单，所以我们有$\mathfrak{h}\cap \mathfrak{q}=\mathfrak{k}\oplus \mathfrak{c}$。因而，

$\mathfrak{c}=\{x\in \mathfrak{h}|[x,\mathfrak{n}]\subset \mathfrak{n}$ 和 $[x,[\mathfrak{m},\mathfrak{m}]] = 0\}$。

到引理 1，$\Phi$到$\mathfrak{c}$的限制是非简并的。

令$\mathfrak{q}^0$为$\mathfrak{g}$中$\mathfrak{q}$相对于$\Phi$的正交补集。上式证明$\mathfrak{q}\cap \mathfrak{q}^0=\mathfrak{n}$。假设$\mathfrak{q}\not=\mathfrak{q}^0$，则$\mathfrak{q}^0\not=\mathfrak{n}$（和$\mathfrak{q}^0\supset \mathfrak{n}$）。由于 ad$_{\mathfrak{g}}\mathfrak{n}$ 使 $\mathfrak{q}$ 保持稳定，因而 ad$_{\mathfrak{g}}\mathfrak{n}$ 使 $\mathfrak{q}^0$ 保持稳定；恩格尔的定理证明存在$x\in \mathfrak{q}^0$使得$x \notin \mathfrak{n}$和$[x,\mathfrak{n}]\subset \mathfrak{n}$。但$x\in \mathfrak{q}^0\cap \mathfrak{q}=\mathfrak{n}$，矛盾了。因而$\mathfrak{q}=\mathfrak{n}^0$。

#### 推论 1 {#lie-viii-s10-thm-2-cor-1 .statement tag=016P}

令$\mathfrak{q}$为与$\mathfrak{g}$不同的$\mathfrak{g}$子代数集合极大元素。那么 $\mathfrak{q}$ 在 $\mathfrak{g}$ 中要么是抛物线要么是约简。

我们可以假设对于某些有限维向量空间 V，$\mathfrak{g}$ 是 $\mathfrak{g}\mathfrak{l}(V)$ 的谎言子代数。令 $\mathfrak{e}(\mathfrak{q})\subset \mathfrak{g}$ 为 $\mathfrak{q}$ 中的可分解包络。如果$\mathfrak{e}(\mathfrak{q}) =\mathfrak{g},\mathfrak{q}$是$\mathfrak{g}$的理想（第VII, §5, no. 2章，命题4），则半单，因而$\mathfrak{q}$在$\mathfrak{g}$中可约化。假设$\mathfrak{e}(\mathfrak{q})\not=\mathfrak{g}$。那么$\mathfrak{e}(\mathfrak{q}) =\mathfrak{q}$，所以$\mathfrak{q}$是可分解的。假设 $\mathfrak{q}$ 不能约化于 $\mathfrak{g}$。令$\mathfrak{n}$为$\mathfrak{q}$的根号的幂零元的集合。然后$\mathfrak{n}\not= 0$（第VII, §5, no. 3章，第7（i）号提案）。令$\mathfrak{p}$为$\mathfrak{g}$中$\mathfrak{n}$的归一化器。然后是$\mathfrak{p}\supset \mathfrak{q}$和$\mathfrak{p}\not=\mathfrak{g}$，因为$\mathfrak{g}$是半单。因而$\mathfrak{p}=\mathfrak{q}$。因而 $\mathfrak{q}$ 是抛物线 (Th. 1)。

#### 推论 2 {#lie-viii-s10-thm-2-cor-2 .statement tag=016Q}

令 $\mathfrak{n}$ 为 $\mathfrak{g}$ 由……组成幂零元中的子代数。存在 $\mathfrak{g}$ 的抛物线子代数 $\mathfrak{q}$，具有以下性质：

(i) $\mathfrak{n}\subset \mathfrak{n}_{\mathfrak{g}}(\mathfrak{q})$；

(ii) $\mathfrak{g}$中$\mathfrak{n}$的归一化项包含在$\mathfrak{q}$中；

(iii) $\mathfrak{g}$的每自同构留下$\mathfrak{n}$不变，留下$\mathfrak{q}$不变。

如果$\mathfrak{g}$可分割，则$\mathfrak{n}$包含在$\mathfrak{g}$的博雷尔子代数中。

令$\mathfrak{q}_1$为$\mathfrak{g}$中$\mathfrak{n}$的归一化器。这是 $\mathfrak{g}$ 的可分解子代数。让$\mathfrak{n}_1=\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q}_1)$。 定义归纳$\mathfrak{q}_i$为$\mathfrak{g}$中$\mathfrak{n}_{i-1}$的归一化项，并且$\mathfrak{n}_i$等于$\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q}_i)$。 序列$(\mathfrak{n},\mathfrak{n}_1,\mathfrak{n}_2, . . .)$和$(\mathfrak{q}_1,\mathfrak{q}_2, . . .)$是递增。存在$j$使得$\mathfrak{q}_j=\mathfrak{q}_{j+1}$，在其他字$\mathfrak{q}_j$是$\mathfrak{g}$中$\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q}_j)$的归一化器。因而 $\mathfrak{q}_j$ 是抛物线 (Th. 1)。我们有$\mathfrak{n}\subset \mathfrak{n}_j=$$\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q}_j)$和$\mathfrak{q}_1\subset \mathfrak{q}_j$； $\mathfrak{g}$ 的每个自同构留下 $\mathfrak{n}$ 不变，显然留下 $\mathfrak{n}_1,\mathfrak{n}_2, . .$。和$\mathfrak{q}_1,\mathfrak{q}_2, . .$。不变量。如果 $\mathfrak{g}$ 是可分割的，$\mathfrak{q}_j$ 包含博雷尔子代数 $\mathfrak{b}$，因而（§3, no. 4，命题 13），我们有 $\mathfrak{b}\supset \mathfrak{n}_{\mathfrak{g}}(\mathfrak{q}_j)\supset \mathfrak{n}$。

#### 定理 3 {#lie-viii-s10-thm-3 .statement tag=016R}

假设 $k$ 是代数封闭的。令 $\mathfrak{g}$ 为半单李代数。设$\mathfrak{a}$是$\mathfrak{g}$的可解子代数。存在 $\mathfrak{g}$ 包含于 $\mathfrak{a}$ 中的博雷尔子代数。

由章。 VII, §5, no. 2，科。根据命题 4 的 1 (ii)，我们可以假设 $\mathfrak{a}$ 是可分解的。存在$\mathfrak{g}$的交换子代数$\mathfrak{t}$，半单元素的由……组成，使得$\mathfrak{a}$是$\mathfrak{t}$和$\mathfrak{n}_{\mathfrak{g}}(\mathfrak{a})$的半直接乘积（第1章） VII, §5, no. 3，第 6 条第 2 条）。存在（Th.2的Cor.2）$\mathfrak{g}$的抛物线子代数$\mathfrak{q}$使得$\mathfrak{n}_{\mathfrak{g}}(\mathfrak{a})\subset \mathfrak{n}_{\mathfrak{g}}(\mathfrak{q})$，并且$\mathfrak{g}$中的$\mathfrak{n}_{\mathfrak{g}}(\mathfrak{a})$的归一化器包含在$\mathfrak{q}$中； 更不必说$,\mathfrak{a}\subset \mathfrak{q}$。令$\mathfrak{b}$为$\mathfrak{q}$中包含的$\mathfrak{g}$的博雷尔子代数，以及$\mathfrak{b}$中包含的$\mathfrak{g}$的$\mathfrak{h}$嘉当子代数。那么$\mathfrak{h}$是$\mathfrak{q}$的嘉当子代数，因此存在$s\in$Aut$_e(\mathfrak{q})$使得$s(\mathfrak{t})\subset \mathfrak{h}$（第VII, §2, no. 3，第10章和第VII, §3, no. 2，第1章）。我们有 $s(\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q})) =\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q})$（第 VII, §3, no. 1、注 1 章），所以

$$
s(\mathfrak{a}) =s(\mathfrak{t}) +s(\mathfrak{n}_{\mathfrak{g}}(\mathfrak{a}))\subset \mathfrak{h}+s(\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q})) =\mathfrak{h}+\mathfrak{n}_{\mathfrak{g}}(\mathfrak{q})\subset \mathfrak{b}
$$

#### 推论{#lie-viii-s10-n0-cor-1 .statement tag=016S}

如果 $k$ 是代数封闭的，则 $\mathfrak{g}$ 的每个最大可解子代数都是博雷尔子代数。

### 习题{#lie-viii-s10-exercises}

§ 10](exercises/s10/)参见[习题。
