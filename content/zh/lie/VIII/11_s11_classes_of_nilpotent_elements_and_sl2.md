---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 11
section_title: Classes of nilpotent elements and sl2 -triplets
lang: zh
source: lie-vii-ix
book_pages: 163-173, 261-266
pdf_pages: 0171-0181, 0269-0274
extraction: native+ocr
subsections:
    - "no": 1
      title: DEFINITION OF $\mathfrak{s}\mathfrak{l}_{2}$-TRIPLETS
      page: 163
      pdf_page: 171
    - "no": 2
      title: $\mathfrak{s}\mathfrak{l}_{2}$-TRIPLETS IN SEMI-SIMPLE LIE ALGEBRAS
      page: 165
      pdf_page: 173
    - "no": 3
      title: SIMPLE ELEMENTS
      page: 167
      pdf_page: 175
    - "no": 4
      title: PRINCIPAL ELEMENTS
      page: 170
      pdf_page: 178
statements: 29
exercises: 17
content_sha256: 7a9f18494cea9745ca4b4a039f561ece5e8ae3b6f85eee85879a1ac6d050047a
translated_from: content/en/lie/VIII/11_s11_classes_of_nilpotent_elements_and_sl2.md
translation_method: google
source_content_sha256: c1241130b0c6145fe39e8ebf582c74a6fd108d7391d43fb0cba572e8a86bff67
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: a8eb2d6a57f8b05cb009e93cc98dd5c329a113496967bb96e811d2f9c41a8ca0
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 11。 幂零元和 $\mathfrak{s}\mathfrak{l}_{2}$-三胞胎的类

在本段中，$\mathfrak{g}$表示有限维李代数。

### 1. 定义 OF $\mathfrak{s}\mathfrak{l}_{2}$-三元组

#### 定义 1 {#lie-viii-s11-def-1 .statement tag=0170}

$\mathfrak{g}$中的$\mathfrak{s}\mathfrak{l}_2$三元组是$\mathfrak{g}$的元素的序列$(x, h, y)$，与$(0,0,0)$不同，这样

$$
[h, x] = 2x,[h, y] =-2y,[x, y] =-h
$$

设$(x, h, y)$是$\mathfrak{g}$中的$\mathfrak{s}\mathfrak{l}_2$三元组。 从$\mathfrak{s}\mathfrak{l}(2, k)$到$\mathfrak{g}$的线性映射$\tau$使得$\tau (X_+) =x, \tau (H) =h, \tau (X_-) =y$是同态，它是非零的，因此是单射的（因为$\mathfrak{s}\mathfrak{l}(2, k)$是简单的），并且具有像$kx+kh+ky$。 We thus obtain a canonical bijection from the set of $\mathfrak{s}\mathfrak{l}_2$-triplets in $\mathfrak{g}$ to the set of injective homomorphisms from $\mathfrak{s}\mathfrak{l}(2, k)$ to $\mathfrak{g}$. 如果$\mathfrak{g}$是半单，并且$(x, h, y)$是$\mathfrak{g}$中的$\mathfrak{s}\mathfrak{l}_2$三元组，则$x$和$y$是$\mathfrak{g}$的幂零元，$h$是半单元素 $\mathfrak{g}$（第 1 章） I, §6, no. 3，命题 4）。

#### 引理 1 {#lie-viii-s11-lem-1 .statement tag=0171}

让$x, h, y, y'\in \mathfrak{g}$。如果$(x, h, y)$和$(x, h, y')$是$\mathfrak{g}$中的$\mathfrak{s}\mathfrak{l}_2$三元组，则$y=y'$。

事实上，$y-y'\in$ Ker(ad$_{\mathfrak{g}}x$) 和 (ad$_{\mathfrak{g}}h$)$(y-y') =-2(y-y')$。但是对于每个整数 $p >0 ($§1, no. 2，ad$_{\mathfrak{g}}x$ 在 Ker($p+$ ad$_{\mathfrak{g}}h$) 上是单射的，Cor。提案 2）。

#### 引理 2 {#lie-viii-s11-lem-2 .statement tag=0172}

令 $\mathfrak{n}$ 为 $\mathfrak{g}$ 的子代数，这样，对于所有 $n\in \mathfrak{n}$，ad$_{\mathfrak{g}}(n)$ 是幂零的。设$h\in \mathfrak{g}$使得$[h,\mathfrak{n}] =\mathfrak{n}$。然后$e^{ad_{\mathfrak{g}}\mathfrak{n}}.h=h+\mathfrak{n}$。

显然$e^{ad_{\mathfrak{g}}(\mathfrak{n})}.h\subset h+\mathfrak{n}$。我们将证明，如果$v\in \mathfrak{n}$，则$h+v\in e^{ad_{\mathfrak{g}}(\mathfrak{n})}.h$。只要证明 $h+v\in e^{ad_{\mathfrak{g}}(\mathfrak{n})}.h+\mathscr{C}0\mathfrak{n}$ 对于所有 $p\geq 1$ 就足够了（因为 $\mathscr{C}^p\mathfrak{n}= 0$ 对于足够大 $p$）。自$\mathscr{C}^1\mathfrak{n}=\mathfrak{n}$以来，这对于$p= 1$来说是清楚的。现在假设我们已经证明了$y_p\in \mathfrak{n}$和$z_p\in \mathscr{C}^p\mathfrak{n}$的存在性使得$h+v=e^{ad_{\mathfrak{g}}y_p}.h+z_p$。由于 (ad$_{\mathfrak{g}}h$)$(\mathfrak{n}) =\mathfrak{n}$、(ad$_{\mathfrak{g}}h$)$|\mathfrak{n}$ 是从 $\mathfrak{n}$ 到 $\mathfrak{n}$ 的双射，因此它的限制到 $\mathscr{C}^p\mathfrak{n}$ 使得 $\mathscr{C}^p\mathfrak{n}$ 稳定，也是双射的；因而，存在$z\in \mathscr{C}^p\mathfrak{n}$使得$z_p= [z, h]$。然后

$$
e^{ad_{\mathfrak{g}}(y_p+z)}h-e^{ad_{\mathfrak{g}}y_p}h\in [z, h] +\mathscr{C}^{p+1}\mathfrak{n}
$$

所以

$$
e^{ad_{\mathfrak{g}}(y_p+z)}h\in h+v-z_p+ [z, h] +\mathscr{C}^{p+1}\mathfrak{n}=h+v+\mathscr{C}^{p+1}\mathfrak{n}
$$

这在 $p$ 上通过归纳建立了我们的断言。

#### 引理 3 {#lie-viii-s11-lem-3 .statement tag=0173}

让 $x\in \mathfrak{g},\mathfrak{p}=$ Ker(ad $x$)$,\mathfrak{q}=$ Im(ad $x$)。那么$[\mathfrak{p},\mathfrak{q}]\subset \mathfrak{q}$，$\mathfrak{p}\cap \mathfrak{q}$就是$\mathfrak{g}$的子代数。

如果$u\in \mathfrak{p}$和$v\in \mathfrak{q}$，则存在$w\in \mathfrak{g}$使得$v= [x, w]$，所以

$$
[u, v] = [u,[x, w]] = [x,[u, w]]-[[x, u], w] = [x,[u, w]]\in \mathfrak{q}
$$

另一方面，$\mathfrak{p}$是$\mathfrak{g}$的子代数，所以$[\mathfrak{p}\cap \mathfrak{q},\mathfrak{p}\cap \mathfrak{q}]\subset \mathfrak{p}\cap \mathfrak{q}$。

#### 引理 4 {#lie-viii-s11-lem-4 .statement tag=0174}

设$(x, h, y)$和$(x, h', y')$为$\mathfrak{g}$中的$\mathfrak{s}\mathfrak{l}_2$三元组。存在 $z\in \mathfrak{g}$ 使得 ad$_{\mathfrak{g}}z$ 幂零且使得

$$
e^{ad_{\mathfrak{g}}z}x=x,e^{ad_{\mathfrak{g}}z}h=h',e^{ad_{\mathfrak{g}}z}y=y'
$$

让 $\mathfrak{n}=$ Ker(ad $x$)$\cap$ Im(ad $x$)。对于所有$p\in \mathbf{Z}$，设$\mathfrak{g}_p=$ Ker(ad $h-p$)。到§1, no. 3（应用于$\mathfrak{g}$上$kx+ky+kh$的伴随表示），我们有$\mathfrak{n}\subset \sum_{p>0}\mathfrak{g}_p$，所以ad$_{\mathfrak{g}}n$对于所有$n\in \mathfrak{n}$和$[h,\mathfrak{n}] =\mathfrak{n}$来说是幂零的。我们有$[x, h'-h] = 0$和$[x, y-y'] =h'-h$，所以$h'-h\in \mathfrak{n}$。通过引理 2 和 3，存在 $z\in \mathfrak{n}$ 使得 $e^{ad_{\mathfrak{g}}z}h=h'$。从$z\in$ Ker ad$_{\mathfrak{g}}x$开始，我们有$e^{ad_{\mathfrak{g}}z}x=x$。 引理 1 现在证明$e^{ad_{\mathfrak{g}}z}y=y'$。 Q.E.D.

设G为$\mathfrak{g}$的自同构中的群。然后，如果存在 $g\in G$ 使得 $gx=x'$、$gh=h', gy=y'$，则两个 $\mathfrak{s}\mathfrak{l}_2$ 三元组 $(x, h, y)$、$(x', h', y')$ 被称为 G 共轭。

#### 命题 1 {#lie-viii-s11-prop-1 .statement tag=0175}

设G为$\mathfrak{g}$包含Aut$_e(\mathfrak{g})$自同构群。设$(x, h, y)$和$(x', h', y')$为$\mathfrak{g}$中的$\mathfrak{s}\mathfrak{l}_2$三元组。让

$$
\mathfrak{t}=kx+kh+ky,\mathfrak{t}'=kx'+kh'+ky'
$$

考虑以下条件：

(i) $x$和$x'$是G-共轭；

(ii) $(x, h, y)$和$(x', h', y')$是G共轭；

(iii) $\mathfrak{t}$ 和 $\mathfrak{t}'$ 是 G-共轭。

我们有 (i) $\Leftarrow \Rightarrow$ (ii) $=\Rightarrow$ (iii)。如果 $k$ 是代数闭的，则三个条件是等价的。

(i) $\Leftarrow \Rightarrow$ (ii)：这是从引理 4 得出的。

(ii) $=\Rightarrow$ (iii)：这很清楚。

我们假设 $k$ 是代数封闭的，并证明 (iii) $=\Rightarrow$ (i)。我们首先处理$\mathfrak{t}=\mathfrak{t}'=\mathfrak{g}=\mathfrak{s}\mathfrak{l}(2, k)$的情况。由于 ad$_{\mathfrak{g}}x$ 是幂零的，$k^2$ 的自同态 $x$ 也是幂零的（第 I, §6 第 3 章），因此存在矩阵 $A\in \mathbf{G}\mathbf{L}(2, k)$ 使得 $AxA^{-1}=X$，因此存在自同构 $\alpha$ $\mathfrak{s}\mathfrak{l}(2, k)$使得$\alpha (x) =x'$；现在$\alpha \in$Aut$_e(\mathfrak{g}) ($§5, no. 3，Cor.提案 5 中的 2）。现在我们讨论一般情况；我们假设$\mathfrak{t}$和$\mathfrak{t}'$是G共轭，并证明$x$和$x'$是G共轭。我们可以假设$\mathfrak{t}=\mathfrak{t}'$。由上可知，存在$\beta \in$Aut$_e(\mathfrak{t})$使得$\beta x=x'$。现在，如果 $t\in \mathfrak{t}$ 使得 ad$_{\mathfrak{t}}t$ 幂零，则 ad$_{\mathfrak{g}}t$ 幂零；所以 Aut$_e(\mathfrak{g})$ 的 $\beta$ 扩展到元素。

#### 注 {#lie-viii-s11-n1-rem-1 .statement tag=0176}

如果我们仅假设$k=k^2$（cf.练习1），则命题1的三个条件是等价的。

### 2.$\mathfrak{s}\mathfrak{l}_{2}$-半单李代数的三胞胎

#### 引理 5 {#lie-viii-s11-lem-5 .statement tag=0177}

令V为有限维向量空间，A和B自同态为V。假设 A 幂零且 $[A,[A,B]] = 0$。那么AB是幂零的。

输入$C = [A,B]$。从$[A,C] = 0$开始，

$[A$，公元前$^p] = [A,B]C^p= C^{p+1}$

每整数 $p\geq 0$。因而，对于$p\geq 1$，Tr(C$^p$) $= 0$，证明C是幂零的（代数，第VII, §3, no. 5章，第13号提案的Cor.4）。现在令$\overline{k}$为$k$的代数闭包，并令$\lambda \in \overline{k},x\in V\otimes_k\overline{k}$为AB$x=\lambda x$，$x\not= 0$。 关系 $[[B,A],A] = 0$ 显示每个整数 $p\geq 0$ 都有 $[B,A^p] =p[B,A]A^{p-1}$。令$r$为最小的整数，使得$A^rx= 0$。然后

$\lambda A^{r-1}x= A^{r-1}$AB$x= A^rBx=$BA$^rx-[B,A^r]x=-r[B,A]A^{r-1}x$。

由于$[B,A]$是幂零的，并且由于$A^{r-1}x\not= 0$，这证明了$\lambda = 0$。因而，AB 的所有特征值都是零，因此是引理。

#### 引理 6 {#lie-viii-s11-lem-6 .statement tag=0178}

令$h, x\in \mathfrak{g}$满足$[h, x] = 2x$和$h\in$（广告$x$）$(\mathfrak{g})$。那么存在$y\in \mathfrak{g}$使得$(x, h, y)$要么是$(0,0,0)$要么是$\mathfrak{s}\mathfrak{l}_2$三元组。

设$\mathfrak{g}'$为可解李代数$kh+kx$。从$x\in [\mathfrak{g}',\mathfrak{g}']$开始，ad$_{\mathfrak{g}}x$是幂零的（第I, §5, no. 3章，第1章）；令$\mathfrak{n}$为其核。由于 [ad $h$，ad $x] =$ 2 ad $x$，我们有 (ad $h$)$\mathfrak{n}\subset \mathfrak{n}$。令 $z\in \mathfrak{g}$ 等于 $h=-[x, z]$。对于任意整数 $n\geq 0$，输入$M_n=$（广告$x$）$^n\mathfrak{g}$。如果 $n >0$，我们有 (§1, no. 1, 引理 1)

[广告$z$,(广告$x$)$^n] =n$((广告$h$)$-n+$1)(广告$x$)$^{n-1}$

所以，如果$u\in M_{n-1}$，

$n$((广告$h$)$-n+ 1$)$u\in$(广告$z$)(广告$x$)$u+ M_n$。

由于 (ad $h$)$\mathfrak{n}\subset \mathfrak{n}$，因而

（（广告$h$）$-n+ 1$）$(\mathfrak{n}\cap M_{n-1})\subset \mathfrak{n}\cap M_n$。

由于 ad $x$ 是幂零的，$M_n= 0$ 对于足够大 $n$。因而，广告 $h|\mathfrak{n}$ 的特征值为整数 $\geq 0$。因而，广告$h+ 2$到$\mathfrak{n}$的限制是可逆的。

现在 $[h, z] + 2z\in \mathfrak{n}$ 以来

$$
[x,[h, z] + 2z] = [[x, h], z] + [h,[x, z]] + 2[x, z]
$$

$$
= [-2x, z] + [h,-h] + 2[x, z] = 0
$$

因此存在$z'\in \mathfrak{n}$使得$[h, z'] + 2z'= [h, z] + 2z$，即$[h, y] =-2y$，放入$y=z-z'$。从$[x, y] = [x, z] =-h$开始，完成证明。

#### 命题 2（雅各布森-莫罗佐夫）{#lie-viii-s11-prop-2 .statement tag=0179}

假设$\mathfrak{g}$是半单。令 $x$ 为 $\mathfrak{g}$ 的非零幂零元。存在$h, y\in \mathfrak{g}$使得$(x, h, y)$是$\mathfrak{s}\mathfrak{l}_2$三元组。

让$\mathfrak{n}=$ Ker（广告$x$）$^2$。如果 $z\in \mathfrak{n}$，则 [ad $x$，[ad $x$，ad $z]] =$ ad([$x,[x, z]]$) $= 0$。到引理 5，ad $x\circ$ ad $z$ 幂零的，因此 Tr(ad $x\circ$ ad $z$) $= 0$。这表明，关于$\mathfrak{g}$的杀戮形式$\Phi$，$x$与$\mathfrak{n}$正交。自从

$\Phi$((广告$x$)$^2y, y'$)$=\Phi (y$,(广告$x$)$^2y')$

对于所有 $y, y'\in \mathfrak{g}$，并且由于 $\Phi$ 是非简并的，$\mathfrak{n}$ 的正交补集是 (ad $x$)$^2$ 的像。因此存在$y'\in \mathfrak{g}$使得$x=$（广告$x$）$^2y'$。放

$$
h=-2[x, y']
$$

我们有$[h, x] = 2x$和$h\in$（广告$x$）$(\mathfrak{g})$。现在应用引理6就足够了。

#### 推论{#lie-viii-s11-n2-cor-1 .statement tag=017A}

假设$\mathfrak{g}$是半单。设G为$\mathfrak{g}$包含Aut$_e(\mathfrak{g})$自同构群。 映射与$\mathfrak{g}$幂零元$x$定义中的任何$\mathfrak{s}\mathfrak{l}_2$三元组$(x, h, y)$相关联，通过从G-共轭类的集合求商双射非零幂零元的 G 共轭类的$\mathfrak{s}\mathfrak{l}_2$-三元组到集合。

这是从命题 1 和 2 得出的。

#### 引理 7 {#lie-viii-s11-lem-7 .statement tag=017B}

令 K 为交换域，且至少有 4 个元素。令 G 为矩阵 $(\alpha 0\alpha \beta_{-1})$ 的群，其中 $\alpha \in K^*,\beta \in K$。设$G'$为群

矩阵使得$\alpha = 1$。然后$G'= (G,G)$。

如果$\alpha , \alpha '\in K^*$和$\beta , \beta '\in K$，

$$
(\alpha \beta )((\alpha '\beta ')((\alpha \beta )^{-1}(\alpha '\beta ')^{-1}
$$

0 $\alpha^{-1}$ 0 $\alpha^{'-1}$ 0 $\alpha^{-1}$ 0 $\alpha^{'-1}$

$$
=(1-\alpha '\beta '-{\alpha \beta \alpha '}^2+\alpha^2\alpha '\beta '+\alpha \beta )
$$

0 1

特别是，

$(1\beta )((\alpha '$0$)((1\beta )^{-1}(\alpha '$0$)^{-1}=(1\beta (1-{\alpha '}^2))$。

0 1 0 $\alpha^{'-1}$ 0 1 0 $\alpha^{'-1}$ 0 1

但存在$\alpha '_0\in K^*$使得$\alpha '_0\not= 1$和$\alpha '_0\not=-1$，然后$k.(1-{\alpha '_0}^2)$$=k$，因此引理。

#### 命题 3 {#lie-viii-s11-prop-3 .statement tag=017C}

假设$\mathfrak{g}$是半单。 群 Aut$_e(\mathfrak{g})$ 等于其导出群。如果 $\mathfrak{g}$ 可拆分，则 Aut$_e(\mathfrak{g})$ 是 Aut$_0(\mathfrak{g})$ 的导出群。

令 $x$ 为 $\mathfrak{g}$ 的非零幂零元。 选择$h, y\in \mathfrak{g}$使得$(x, h, y)$是$\mathfrak{s}\mathfrak{l}_2$三元组（命题2）。 $(x, h, y)$生成的$\mathfrak{g}$的子代数$\mathfrak{s}$可以用$\mathfrak{s}\mathfrak{l}(2, k)$来识别。令$\rho$为$\mathfrak{s}=\mathfrak{s}\mathfrak{l}(2, k)$在$\mathfrak{g}$上的表示$z \rightarrow$和$_{\mathfrak{g}}z$，并令$\pi$为与$\rho ($§1, no. 4兼容的$\mathbf{S}\mathbf{L}(2, k)$的表示）。 $\pi$的像由exp($t$ ad$_{\mathfrak{g}}x$)和exp($t$ ad$_{\mathfrak{g}}y$)与$t\in k($代数生成，第1章。 III, §8, no. 9，提案 17），因此包含在 Aut$_e(\mathfrak{g})$ 中。由于 $\mathbf{S}\mathbf{L}(2, k)$ 等于其导出群（引理 7 和前述），exp(ad$_{\mathfrak{g}}x$) 属于到 Aut$_e(\mathfrak{g})$ 的导出群 G。因此Aut$_e(\mathfrak{g})$等于G。现在假设$\mathfrak{g}$是可分割的。由于Aut$_0(\mathfrak{g})/$Aut$_e(\mathfrak{g})$是可交换的（§5, no. 3，注3），所以上式证明Aut$_0(\mathfrak{g})$的导出群是Aut$_e(\mathfrak{g})$。

### 3.简单元素

#### 定义 2 {#lie-viii-s11-def-2 .statement tag=017D}

如果存在$x, y\in \mathfrak{g}$使得$(x, h, y)$是$\mathfrak{g}$中的$\mathfrak{s}\mathfrak{l}_2$三元组，则称$\mathfrak{g}$的元素$h$是简单的。

我们还说$h$是$\mathfrak{s}\mathfrak{l}_2$三元组$(x, h, y)$的简单元素。

#### 命题 4 {#lie-viii-s11-prop-4 .statement tag=017E}

令$h$为$\mathfrak{g}$的非零元素。那么$h$是简单的当且仅当存在$x\in \mathfrak{g}$使得$[h, x] = 2x$和$h\in$（广告$x$）$(\mathfrak{g})$。

条件显然是必要的。 引理6就够了。

#### 命题 5 {#lie-viii-s11-prop-5 .statement tag=017F}

假设$\mathfrak{g}$可拆分半单。令$\mathfrak{h}$为$\mathfrak{g}$的分裂嘉当子代数，$(\mathfrak{g},\mathfrak{h})$的根为R集合，以及R的B基。令$h$为$\mathfrak{g}$的简单元素属于至 $\mathfrak{h}$。那么$h$是Aut$_e(\mathfrak{g},\mathfrak{h})$下的共轭到$\mathfrak{h}$的元素$h'$，这样对于所有$\alpha \in B$来说$\alpha (h')\in  \{0,1,2\}$。

特征值广告$_{\mathfrak{g}}h$属于至$\mathbf{Z}($§1, no. 2，Cor.提案 2）。因此$h\in \mathfrak{h}_{\mathbf{Q}}$。存在 $(\mathfrak{g},\mathfrak{h})$ 的 Weyl 群的元素 $w$，使得 $\alpha (wh)\geq 0$ 对于所有 $\alpha \in B$（第 VI, §1, no. 5，第 2 (i) 章）。鉴于§2, no. 2，Cor。的 Th。 2、我们简化为所有$\alpha \in B$都为$\alpha (h)\in \mathbf{N}$的情况。令$R_+$为相对于B的正根的集合，以及$R_-=-R_+$。 形式 $(x, h, y)$ 的$\mathfrak{g}$中存在$\mathfrak{s}\mathfrak{l}_2$三元组。令 T 为根 $\beta$ 中的集合，使得 $\beta (h) =-2$。然后是$T\subset R_-$和$y\in \sum_{\beta\in T}\mathfrak{g}^{\beta}$。假设有

存在$\alpha \in B$使得$\alpha (h)>2$。对于所有$\beta \in T$，我们有$(\alpha +\beta )(h)>0$，所以$\alpha +\beta  \notin R_-$和$\alpha +\beta \not= 0$；另一方面，从$\beta \in R_-$和$\alpha \in B$开始，我们有$\alpha +\beta  \notin R_+$；因此$\alpha +\beta  \notin R\cup  \{0\}$，所以$[\mathfrak{g}^{\alpha},\mathfrak{g}^{\beta}] = 0$。因此，$[y,\mathfrak{g}^{\alpha}] = 0$。但 ad$_{\mathfrak{g}}y|\mathfrak{g}^{\alpha}$ 是单射的，因为 $\alpha (h)>0 ($§1, no. 2，Cor。提案 2）。这个矛盾证明了$\alpha (h)\leq 2$对于所有$\alpha \in B$。

#### 推论{#lie-viii-s11-n3-cor-1 .statement tag=017G}

如果$k$是代数闭的并且如果$\mathfrak{g}$是秩$l$半单，$\mathfrak{g}$的简单元素共轭类数，相对于Aut$_e(\mathfrak{g})$，至多是$3^l$。

事实上，$\mathfrak{g}$的每个半单元素在Aut$_e(\mathfrak{g})$到$\mathfrak{h}$的元素下都是共轭。

#### 引理 8 {#lie-viii-s11-lem-8 .statement tag=017H}

假设 $k$ 是代数闭集，并且 $\mathfrak{g}$ 是半单。令$h$为$\mathfrak{g}$的半单元素，使得广告$h$的特征值是有理数。令 $\mathfrak{g}^0=$ Ker(ad $h$)$,\mathfrak{g}^2=$ Ker(ad $h-2$)。令$G_h$为$\mathfrak{g}$的初等自同构的集合，使$h$固定。令$x\in \mathfrak{g}^2$ 使得$[x,\mathfrak{g}^0] =\mathfrak{g}^2$。然后$G_hx$包含子集$\mathfrak{g}^2$，在Zariski拓扑密集且开放。

设$\mathfrak{h}$为$\mathfrak{g}^0$中的嘉当子代数。这是 $\mathfrak{g}$ 包含 $h$ 中的嘉当子代数（第 VII, §2, no. 3 章，提案 10）。我们有$h\in \mathfrak{h}_{\mathbf{Q}}$。设R为根权的$(\mathfrak{g},\mathfrak{h}), Q$群的根系。 R 存在基 B，使得对于所有 $\alpha \in B$ 都有 $\alpha (h)\geq 0$。

令 U 为 $z\in \mathfrak{h}$ 的集合，使得对于所有 $\alpha \in B$ 为 $\alpha (z)\not= 0$。令$(H'_{\alpha})_{\alpha\in B}$为$\mathfrak{h}$对偶于B的基。如果$z\in U$，则存在从Q到$k^*$取任何$\gamma \in Q$到$\prod_{\alpha\in B}\alpha (z)^{\gamma(H'_{\alpha})}$的同态。根据§5，提案 2 和 4，

向量空间 $\mathfrak{g}$ 的自同态 $\varphi (z)$，其中 $\mathfrak{g}^{\gamma}$ 位似上的诱导与比率 $\prod_{\alpha\in B}\alpha (z)^{\gamma(H'_{\alpha})}$ 是 $\mathfrak{g}$ 的初等自同构，这显然

属于至$G_h$。

让$s\in \mathfrak{h}$。如果$\gamma \in R$使得$\mathfrak{g}^{\gamma}\cap \mathfrak{g}^2\not= 0$，

$$
2 =\gamma (h) =\gamma (\sum_{\alpha\in B}\alpha (h)H'_{\alpha})=\sum_{\alpha\in B}\alpha (h)\gamma (H'_{\alpha})
$$

由于$\alpha (h)\geq 0$对于所有$\alpha \in B$，并且由于$\gamma (H'_{\alpha})$是整数，或者所有$\geq 0$或所有$\leq 0$，所以我们对所有$\alpha \in B$有$\gamma (H'_{\alpha})\in \mathbf{N}$。因此，我们可以考虑（对于$z\in \mathfrak{h}$）向量空间$\mathfrak{g}^2$的自同态$\psi (z)$，诱导在$\mathfrak{g}^{\gamma}\cap \mathfrak{g}^2$位似上，比率为$\prod_{\alpha\in B}\alpha (z)^{\gamma(H'_{\alpha})}$。从 $\mathfrak{h}$ 到 End($\mathfrak{g}^2$) 的映射 $z \rightarrow \psi (z)$ 是多项式。对于$z\in U$，我们有$\psi (z) =\varphi (z)|\mathfrak{g}^2$。

令 $\gamma_1, . . . , \gamma_r$ 为 $(\mathfrak{g},\mathfrak{h})$ 消失在 $h$ 上的不同根。 如果$y_1\in \mathfrak{g}^{\gamma_1}, . . .$，$y_r\in \mathfrak{g}^{\gamma_r}$，我们有$e^{ady_1}. . . e^{ady_r}\in G_h$。 We can thus define a map $\rho$ from $\mathfrak{h}\times \mathfrak{g}^{\gamma_1}\times  \cdots  \times \mathfrak{g}^{\gamma_r}$ to $\mathfrak{g}^2$ by putting

$$
\rho (z, y_1, . . . , y_r) =\psi (z)e^{ady_1}. . . e^{ady_r}x
$$

对于$z\in \mathfrak{h}, y_1\in \mathfrak{g}^{\gamma_1}, . . . , y_r\in \mathfrak{g}^{\gamma_r}$。这个映射是多项式，$\rho (U,\mathfrak{g}^{\gamma_1}, . . . ,\mathfrak{g}^{\gamma_r})$$\subset G_hx$。由章。 VII，应用程序。 I，命题3和4，只要证明$\rho$的切线映射在点处是满射的。

现在令 T 为 $z \rightarrow \psi (z)$ 在 $h_0=\sum_{\alpha\in B}H'_{\alpha}$ 的切线映射。那么$T(z)$就是$\mathfrak{g}^{\gamma}\cap \mathfrak{g}^2$位似上的诱导与$\mathfrak{g}^2$的自同态之比

$$
\sum_{\alpha\in B}\gamma (H'_{\alpha})\alpha (h_0)^{\gamma(H'_{\alpha})-1}\alpha (z)\prod_{\beta\in B,\beta\not=\alpha}\beta (h_0)^{\gamma(H'_{\alpha})}=\sum_{\alpha\in B}\gamma (H'_{\alpha})\alpha (z) =\gamma (z)
$$

因此，$z \rightarrow \rho (z,0, . . . ,0)$在$h_0$的切线映射为映射$z \rightarrow [z, x]$；它的像是$[x,\mathfrak{h}]$。 映射 $y_1 \rightarrow \rho (h_0, y_1,0, . . . ,0)$ 在 0 点的切线映射为映射 $y_1 \rightarrow \psi (h_0)[y_1, x]$；最后一个映射有像$\psi (h_0)[x,\mathfrak{g}^{\gamma_1}] = [x,\mathfrak{g}^{\gamma_1}]$。同样，映射 $y_i \rightarrow \rho (h_0,0, . . . ,0, y_i,0, . . . ,0)$ 在 0 处的切线映射有像 $[x,\mathfrak{g}^{\gamma_i}]$。最后，$\rho$在$(h_0,0, . . . ,0)$处的切线映射有像

$$
[x,\mathfrak{h}+\mathfrak{g}^{\gamma_1}+\cdots +\mathfrak{g}^{\gamma_r}] = [x,\mathfrak{g}^0] =\mathfrak{g}^2.Q.E.D
$$

\*群 $G_h$ 是代数群与李代数和 $\mathfrak{g}^0$。\*

#### 命题 6 {#lie-viii-s11-prop-6 .statement tag=017I}

假设 $k$ 是代数封闭的，并且 $\mathfrak{g}$ 是半单。设G为$\mathfrak{g}$包含Aut$_e(\mathfrak{g})$自同构群。设 $(x, h, y)$ 和 $(x', h', y')$ 为 $\mathfrak{g}$ 中的 $\mathfrak{s}\mathfrak{l}_2$ 三元组。以下条件是等效的：

(i) $h$和$h'$是G-共轭；

(ii) $(x, h, y)$ 和 $(x', h', y')$ 是 G-共轭。

我们只需证明蕴涵 (i) $=\Rightarrow$ (ii)，我们就立即还原为$h=h'$ 的情况。引入$\mathfrak{g}^2$和$G_h$，如引理8。我们有$x\in \mathfrak{g}^2$和$[x,\mathfrak{g}^0] =\mathfrak{g}^2$，由§1, no. 2，Cor。命题 2. 因而 $\mathfrak{g}^2$ 的$G_hx$ 包含子集在 Zariski 拓扑中是密集且开放的，$G_hx'$ 也是如此。所以存在$a\in G_h$使得$a(x) =x'$。我们有 $a(h) =h$，因此有 $a(y) =y'$（no. 1，引理 1）。

#### 推论 1 {#lie-viii-s11-prop-6-cor-1 .statement tag=017J}

映射通过从$\mathfrak{s}\mathfrak{l}_2$三元组的G-共轭类的集合到简单的G-共轭类的集合的商双射与任何$\mathfrak{s}\mathfrak{l}_2$三元组关联它的简单元素定义元素。

#### 推论 2 {#lie-viii-s11-prop-6-cor-2 .statement tag=017K}

若rk($\mathfrak{g}$)$=l$，共轭类的数，相对于Aut$_e(\mathfrak{g})$，$\mathfrak{g}$的非零幂零元至多为$3^l$。

这是从 Cor 得出的。 1、科。提案 2 和 Cor。提案 5。

#### 推论 3 {#lie-viii-s11-prop-6-cor-3 .statement tag=017L}

若rk($\mathfrak{g}$)$=l$，则共轭类的数，相对于Aut$_e(\mathfrak{g})$，与$\mathfrak{s}\mathfrak{l}(2, k)$同构的$\mathfrak{g}$的子代数至多为$3^l$。

这是从 Cor 得出的。 1、提案 1 和 Cor。提案 5。

### 4.主元素

#### 定义 3 {#lie-viii-s11-def-3 .statement tag=017M}

假设$\mathfrak{g}$是半单。

(i) 如果 Ker ad $x$ 的维数是 $\mathfrak{g}$ 的秩，则 $\mathfrak{g}$ 的幂零元 $x$ 被认为是本金。

(ii) 如果 $h$ 是正则且$h$ 的特征值在 $k$ 属于到$2\mathbf{Z}$ 的代数闭包中，则称$\mathfrak{g}$ 的简单元素 $h$ 为主要。

(iii) 如果$\mathfrak{g}$的长度被视为模除以$kx+kh+ky$，等于$\mathfrak{g}$的秩，则$\mathfrak{g}$的$\mathfrak{s}\mathfrak{l}_2$三元组$(x, h, y)$被认为是主要的。

#### 命题 7 {#lie-viii-s11-prop-7 .statement tag=017N}

假设$\mathfrak{g}$是半单。设$(x, h, y)$是$\mathfrak{g}$中的$\mathfrak{s}\mathfrak{l}_2$三元组。以下条件是等效的：

(i) $x$ 为主；

(ii) $h$ 为主；

(iii) $(x, h, y)$ 为主。

对于 $p\in \mathbf{Z}$，令 $\mathfrak{g}^p=$ Ker(ad $h-p$)。让$\mathfrak{g}'=\sum_{p\in\mathbf{Z}}\mathfrak{g}^{2p}$。如果 $\mathfrak{g}$ 被认为是

$\mathfrak{a}=kx+kh+ky,\mathfrak{g}'$之上的模是单数维数简单子模和（§1, no. 2，Prop.2的Cor.）。令$l$（分别$l'$）为$\mathfrak{g}$（分别$\mathfrak{g}'$）的长度，被视为$\mathfrak{a}$模块。到§1, no. 2，

昏暗（Ker ad $x$）$=l\geq l'=$ 昏暗（Ker ad $h$）$\geq$ rk（$\mathfrak{g}$）。

(i) 和 (iii) 的等价紧随其后。另一方面，条件(ii)意味着dim(Ker ad$h$)$=$rk($\mathfrak{g}$)和$\mathfrak{g}'=\mathfrak{g}$，在其他字中

昏暗（Ker ad $h$）$=$ rk（$\mathfrak{g}$）和$l=l'$。 (ii) 的等价和其他条件如下。

#### 命题 8 {#lie-viii-s11-prop-8 .statement tag=017O}

假设$\mathfrak{g}$是半单$\not= 0$。令 $\mathfrak{h}$ 为 $\mathfrak{g}$ 的分裂嘉当子代数，$(\mathfrak{g},\mathfrak{h})$ 的 R 根系，$,h^0$ 元素的 B 基，$\mathfrak{h}$ 使得$\alpha (h^0) = 2$ 对于所有$\alpha \in B$。

(i) 元素 $h^0$ 简单又原则。

(ii) $\mathfrak{g}$的元素$x$，使得存在形式$(x, h^0, y)$的$\mathfrak{s}\mathfrak{l}_2$三元组是$\sum_{\alpha\in B}\mathfrak{g}^{\alpha}$的元素，并且在每个$\mathfrak{g}^{\alpha}$中具有非零分量。

元素 $h^0$ 是在 §7, no. 5、引理 2（cf. loc. cit.、公式 (1)）中考虑的。由此引理可以得出，$h^0$是简单原理，并且如果$x\in \sum_{\alpha\in B}\mathfrak{g}^{\alpha}$在每个$\mathfrak{g}^{\alpha}$中有一个非零分量，则存在形式$(x, h^0, y)$的$\mathfrak{s}\mathfrak{l}_2$三元组。相反，令 $(x, h^0, y)$ 为 $\mathfrak{s}\mathfrak{l}_2$ 三元组。我们有$[h^0, x] = 2x$，所以$x\in \sum_{\gamma\in R,\gamma(h^0)=2}\mathfrak{g}^{\gamma}=\sum_{\alpha\in B}\mathfrak{g}^{\alpha}$。同样，$y\in \sum_{\alpha\in B}\mathfrak{g}^{-\alpha}$。写

$h^0=\sum_{\alpha\in B}a_{\alpha}H_{\alpha}$ 其中 $a_{\alpha}>0$ 对于所有 $\alpha \in B$，

$x=\sum_{\alpha\in B}X_{\alpha}$ 其中 $X_{\alpha}\in \mathfrak{g}^{\alpha}$ 代表所有 $\alpha \in B$，

$y=\sum_{\alpha\in B}X_{-\alpha}$，其中$X_{-\alpha}\in \mathfrak{g}^{-\alpha}$代表所有$\alpha \in B$。

然后

$$
\sum_{\alpha\in B}a_{\alpha}H_{\alpha}=h^0= [y, x] =\sum_{\alpha ,\beta\in B}[X_{-\beta}, X_{\alpha}] =\sum_{\alpha\in B}[X_{-\alpha}, X_{\alpha}]
$$

所以 $[X_{-\alpha}, X_{\alpha}]\not= 0$ 对于所有$\alpha \in B$。

#### 推论{#lie-viii-s11-n4-cor-1 .statement tag=017P}

在可分割的半单李代数中，存在主体幂零元。

在不可分割的半单李代数中，0可能是唯一的幂零元。

#### 命题 9 {#lie-viii-s11-prop-9 .statement tag=017Q}

假设 $k$ 是代数闭集，并且 $\mathfrak{g}$ 是半单。 $\mathfrak{g}$ 的所有主要简单（或幂零）元素都是 Aut$_e(\mathfrak{g})$ 下的共轭。

我们保留第 8 条命题的记号。令$h$ 为主要简单元素。它是 Aut$_e(\mathfrak{g})$ 下的共轭到 $h'\in \mathfrak{h}$，使得所有 $\alpha \in B$ 都有 $\alpha (h')\in  \{0,1,2\}$（no. 3，提案 5）。由于$h'$是原则简单的，$\alpha (h')\not= 0$和$\alpha (h')\in 2\mathbf{Z}$适用于所有$\alpha \in B$，因此$\alpha (h') = 2$适用于所有$\alpha \in B$，因此$h'=h^0$。这证明了断言对于简单的元素。

令$x, x'$为主幂零元。存在$\mathfrak{s}\mathfrak{l}_2$-三元组$(x, h, y)$、$(x', h', y')$。根据命题，$7,h$和$h'$是主要简单的，因此共轭在前面的Aut$_e(\mathfrak{g})$下。所以$x$和$x'$在Aut$_e(\mathfrak{g})$下是共轭（命题6）。

#### 引理 9 {#lie-viii-s11-lem-9 .statement tag=017R}

有了第8条命题的记号，把$\mathfrak{g}^p=$ Ker(ad $h^0-p$)换成$p\in \mathbf{Z}$。令 $\mathfrak{g}^2_*$ 为 $\mathfrak{g}^2=\sum_{\alpha\in B}\mathfrak{g}^{\alpha}$ 的元素中的集合，其分量非零

每个$\mathfrak{g}^{\alpha}$。令$R_+$为相对于B$,\mathfrak{n}_+=\sum_{\alpha\in R_+}\mathfrak{g}^{\alpha}$和$x\in \mathfrak{g}^2_*$为正根的集合。然后$e^{ad\mathfrak{n}_+}.x=x+ [\mathfrak{n}_+,\mathfrak{n}_+]$。

很明显$e^{ad\mathfrak{n}_+}.x\subset x+ [\mathfrak{n}_+,\mathfrak{n}_+]$。我们证明，如果$v\in [\mathfrak{n}_+,\mathfrak{n}_+]$，则$x+v\in e^{ad\mathfrak{n}_+}.x$。把$\mathfrak{n}^{(p)}=\sum_{r\geq p}\mathfrak{g}^{2r}$；足以证明

$$
x+v\in e^{ad\mathfrak{n}_+}.x+\mathfrak{n}^{(p)}
$$

对于所有$p\geq 2$。自 $\mathfrak{n}^{(2)}$ $= [\mathfrak{n}_+,\mathfrak{n}_+] ($§3, no. 3，第 9 (iii) 条提案以来，这对于 $p= 2$ 来说是清楚的。假设我们已经找到$z\in \mathfrak{n}_+$使得$v+x-e^{adz}.x\in$$\mathfrak{n}^{(p)}$。由于存在形式 $(x, h^0, y)$（第 8 条命题）的 $\mathfrak{s}\mathfrak{l}_2$ 三元组，§1, no. 2，Cor.命题 2 证明 $[x,\mathfrak{g}^{2p-2}] =\mathfrak{g}^{2p}$；因此，存在$z'\in \mathfrak{g}^{2p-2}\subset \mathfrak{n}_+$使得

$$
v+x-e^{adz}.x\in [z', x] +\mathfrak{n}^{(p+1)}
$$

所以$v+x\in e^{ad(z+z')}.x+\mathfrak{n}^{(p+1)}$，而我们的断言是由归纳建立的。

#### 命题 10 {#lie-viii-s11-prop-10 .statement tag=017S}

假设$\mathfrak{g}$是半单。设$\mathfrak{h}$为$\mathfrak{g}$的分裂嘉当子代数，$(\mathfrak{g},\mathfrak{h})$的R根系，R的B基，相对于B的正根的$R_+$集合，并且$\mathfrak{n}_+=\sum_{\alpha\in R_+}\mathfrak{g}^{\alpha}$。主要的幂零元属于到$\mathfrak{n}_+$是$\mathfrak{n}_+$的元素，对于所有$\alpha \in B$来说，$\mathfrak{g}^{\alpha}$中有一个非零分量。

命题8和引理9证明这样的元素是主幂零的。我们证明逆命题。显然我们可以假设 $\mathfrak{g}$ 是简单的。令$h^0$和$\mathfrak{g}^p$如命题8和引理9。令$\omega$为最高根，并代入$\omega (h^0) = 2q$；我们有$q=h-1$，其中$h$是R的Coxeter数，cf.。 VI, §1, no. 11, Prop. 31. Then $\mathfrak{g}^{2q}=\mathfrak{g}^{\omega},\mathfrak{g}^{-2q}=\mathfrak{g}^{-\omega}$, and $\mathfrak{g}^{2k}= 0$ for $|k|> q$.存在一个主$\mathfrak{s}\mathfrak{l}_2$-三元组$(x^0, h^0, y^0)$。由 §1, no. 2 提供，Cor.根据第 2 条，(ad $x^0$)$^{2q}(\mathfrak{g}^{-\omega}) =\mathfrak{g}^{\omega}$，所以 (ad $x^0$)$^{2q}\not= 0$。 Let $x$ be a principal 幂零元 of $\mathfrak{g}$ 属于 to $\mathfrak{n}_+$.如果$\overline{k}$是$k,x\otimes 1$的代数闭包，并且$x^0\otimes 1$是共轭在$\mathfrak{g}\otimes_k\overline{k}$的自同构之下（命题9），那么（ad$x$）$^{2q}\not= 0$。存在 $\lambda \in R$ 使得 (ad $x$)$^{2q}\mathfrak{g}^{\lambda}\not= 0$。将$x=\sum_{n\geq 1}x_n$放入$x_n\in \mathfrak{g}^{2n}$。

然后

（广告$x$）$^{2q}\mathfrak{g}^{\lambda}\subset$（广告$x_1$）$^{2q}\mathfrak{g}^{\lambda}+\sum_{k>4q+\lambda(h^0)}\mathfrak{g}^k=$（广告$x_1$）$^{2q}\mathfrak{g}^{\lambda}$，自$4q+\lambda (h^0)\geq 4q-2q= 2q$开始。现在（广告$x_1$）$^{2q}\mathfrak{g}^{\lambda}\subset \mathfrak{g}^{4q+\lambda(h^0)}$，其中$\lambda =-\omega$。因此，（广告$x_1$）$^{2q}\mathfrak{g}^{-\omega}=\mathfrak{g}^{\omega}$。对于所有 $\alpha \in$ B（第 VI, §1, no. 8、注），我们有 $\omega =\sum_{\alpha\in B}n_{\alpha}\alpha$ 和 $n_{\alpha}>0$。如果存在$\alpha_0\in B$使得$x_1\in$

$\sum\mathfrak{g}^{\alpha}$、关系

$\alpha \in B,\alpha \not=\alpha_0$

$$
\omega  \notin  -\omega +\sum_{\alpha\in B,\alpha\not=\alpha_0}k\alpha
$$

意味着 $\mathfrak{g}^{\omega}\not\subset$ (ad $x_1$)$^p\mathfrak{g}^{-\omega}$ 对于所有 $p$；这是荒谬的，所以$\mathfrak{g}^{\alpha}$中$x_1$的分量对于所有$\alpha \in B$来说都是非零的。

### 习题 {#lie-viii-s11-exercises}

§ 11](exercises/s11/)参见[习题。
