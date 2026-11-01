---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 2
section_title: Root system of a split semi-simple Lie algebra
lang: zh
source: lie-vii-ix
book_pages: 77-86, 226-229
pdf_pages: 0085-0094, 0234-0237
extraction: native
subsections:
    - "no": 1
      title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
      page: 77
      pdf_page: 85
    - "no": 2
      title: ROOTS OF A SPLIT SEMI-SIMPLE LIE ALGEBRA
      page: 78
      pdf_page: 86
    - "no": 3
      title: INVARIANT BILINEAR FORMS
      page: 83
      pdf_page: 91
    - "no": 4
      title: THE COEFFICIENTS N$_{\boldsymbol{\alpha \beta }}$
      page: 83
      pdf_page: 91
statements: 28
exercises: 11
content_sha256: bf9930a93f236f5546471cde35b810828610fbd2ae45499b1337ae574ba0b313
translated_from: content/en/lie/VIII/02_s2_root_system_of_a_split_semi_simple_lie.md
translation_method: google
source_content_sha256: 5b8fba70b72c8f243ecb19eff11bd99a4fc4e1594703137b927fa6344b3f9e7f
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 886ebab8a4104fd277dab78d332352c2526a809c0f40f022a37422c35af236a0
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 2。 根系分裂的半单李代数

### 1. 分裂的半单李代数

#### 定义 1 {#lie-viii-s2-def-1 .statement tag=00YK}

设$\mathfrak{g}$为半单李代数。如果对于所有 $x\in \mathfrak{h}$，ad$_{\mathfrak{g}}x$ 可三角化，则 $\mathfrak{g}$ 的嘉当子代数 $\mathfrak{h}$ 称为分裂。如果半单李代数具有分裂嘉当子代数，则称为可拆分。 分裂的半单李代数是对 $(\mathfrak{g},\mathfrak{h})$，其中$\mathfrak{g}$ 是半单李代数，$\mathfrak{h}$ 是$\mathfrak{g}$ 的分裂嘉当子代数。

#### 注 1 {#lie-viii-s2-n1-rem-1 .statement tag=00YL}

设$\mathfrak{g}$为半单李代数，$\mathfrak{h}$嘉当子代数/$\mathfrak{g}$。对于所有 $x\in \mathfrak{h}$，ad$_{\mathfrak{g}}x$ 为半单（第 VII, §2, no. 4 章，第 2 章）。因此，说 $\mathfrak{h}$ 是分裂意味着 ad$_{\mathfrak{g}}x$ 对于所有 $x\in \mathfrak{h}$ 都是可对角化的。

#### 注 2 {#lie-viii-s2-n1-rem-2 .statement tag=00YM}

如果$k$是代数闭的，则每个半单李代数$\mathfrak{g}$都是可分割的，并且$\mathfrak{g}$的每个嘉当子代数都是分裂。当$k$非代数闭时，存在不可分半单李代数 (Exerc. $2a$)$)$；此外，如果$\mathfrak{g}$是可分割的，则$\mathfrak{g}$中可能存在嘉当子代数不是分裂（Exerc.$2b$）$)$。

#### 注 3 {#lie-viii-s2-n1-rem-3 .statement tag=00YN}

令$\mathfrak{g}$为半单李代数、$\mathfrak{g}$的$\mathfrak{h}$嘉当子代数，以及$\rho$为$\mathfrak{g}$的有限维单射表示，使得$\rho (\mathfrak{h})$可对角化。那么 ad$_{\mathfrak{g}}x$ 对于所有 $x\in \mathfrak{h}$（第 VII, §2, no. 1，例 2 章）可对角化，因此 $\mathfrak{h}$ 是分裂。

#### 注 4 {#lie-viii-s2-n1-rem-4 .statement tag=00YO}

我们将看到（§3, no. 3，Prop. 10 的Cor.），如果$\mathfrak{h},\mathfrak{h}'$是$\mathfrak{g}$的分裂嘉当子代数，则存在$\mathfrak{g}$的初等自同构将$\mathfrak{h}$变换为$\mathfrak{h}'$。

#### 注 5 {#lie-viii-s2-n1-rem-5 .statement tag=00YP}

设 $\mathfrak{g}$ 为约简李代数。然后$\mathfrak{g}=\mathfrak{c}\times \mathfrak{s}$，其中$\mathfrak{c}$是$\mathfrak{g}$的中心，$\mathfrak{s}=\mathscr{D}\mathfrak{g}$是半单。 $\mathfrak{g}$中的嘉当子代数是形式$\mathfrak{h}=\mathfrak{c}\times \mathfrak{h}'$中的子代数，其中$\mathfrak{h}'$是$\mathfrak{s}$中的嘉当子代数（第VII, §2, no. 1章，第2条）。如果$\mathfrak{h}'$相对于$\mathfrak{s}$是分裂，则$\mathfrak{h}$称为分裂。这以明显的方式导致可分割的定义或还原的分裂的代数。

### 2. 根分裂的半单李代数

在这个数中，$(\mathfrak{g},\mathfrak{h})$表示分裂的半单李代数。

对于任何$\lambda \in \mathfrak{h}^*$，用$\mathfrak{g}^{\lambda}(\mathfrak{h})$表示，或者简单地用$\mathfrak{g}^{\lambda}$表示，$\mathfrak{g}$相对于$\lambda$的主要子空间（cf.章节VII, §1, no. 3）。回想一下$\mathfrak{g}^0=\mathfrak{h}$（第VII, §2, no. 1章，第4条命题），$\mathfrak{g}$是$\mathfrak{g}^{\lambda}$的直和（第VII, §1, no. 3章，第8和9条命题），$\mathfrak{g}^{\lambda}$是$x\in \mathfrak{g}$的集合，这样$[h, x] =\lambda (h)x$ 对于所有 $h\in \mathfrak{h}$（第 VII, §2, no. 4，第 2 章第 1 章），并且 $\mathfrak{g}$ 上的 $\mathfrak{h}$ 的权是 $\mathfrak{h}$ 上的线性形式 $\lambda$，使得 $\mathfrak{g}^{\lambda}\not= 0$ （第VII, §1, no. 1章）。

#### 定义 2 {#lie-viii-s2-def-2 .statement tag=00YQ}

$(\mathfrak{g},\mathfrak{h})$ 的根是$\mathfrak{g}$ 上$\mathfrak{h}$ 的非零权。

用$R(\mathfrak{g},\mathfrak{h})$表示，或简称为R，$(\mathfrak{g},\mathfrak{h})$根集合。我们有

$$
\mathfrak{g}=\mathfrak{h}\oplus \bigoplus_{\alpha\in R}\mathfrak{g}^{\alpha}
$$

#### 命题 1 {#lie-viii-s2-prop-1 .statement tag=00YR}

令$\alpha ,\beta$为$(\mathfrak{g},\mathfrak{h})$的根，并令$\langle \cdot ,\cdot \rangle$为$\mathfrak{g}($上的非简并不变对称双线性形式，用于例对$\mathfrak{g})$的杀戮形式。

(i) 如果 $\alpha +\beta \not= 0,\mathfrak{g}^{\alpha}$ 和 $\mathfrak{g}^{\beta}$ 正交。 $\langle \cdot ,\cdot \rangle$到$\mathfrak{g}^{\alpha}\times \mathfrak{g}^{-\alpha}$的限制是非简并的。 $\langle \cdot ,\cdot \rangle$到$\mathfrak{h}$的限制是非简并的。

(ii) 设 $x\in \mathfrak{g}^{\alpha},y\in \mathfrak{g}^{-\alpha}$ 和 $h\in \mathfrak{h}$。然后 $[x, y]\in \mathfrak{h}$ 和

$$
\langle h,[x, y]\rangle =\alpha (h)\langle x, y\rangle
$$

断言(i)是第10章第10(iii)条提案的一个特例。 VII, §1, no. 3。如果$x\in \mathfrak{g}^{\alpha},y\in \mathfrak{g}^{-\alpha}$和$h\in \mathfrak{h}$，我们有$[x, y]\in \mathfrak{g}^{\alpha-\alpha}=\mathfrak{h}$，并且

$$
\langle h,[x, y]\rangle =\langle [h, x], y\rangle =\langle \alpha (h)x, y\rangle =\alpha (h)\langle x, y\rangle
$$

#### 定理 1 {#lie-viii-s2-thm-1 .statement tag=00YS}

令 $\alpha$ 为 $(\mathfrak{g},\mathfrak{h})$ 的根。

(i) 向量空间 $\mathfrak{g}^{\alpha}$ 等于维数 1。

(ii) $\mathfrak{h}$的向量子空间$\mathfrak{h}_{\alpha}= [\mathfrak{g}^{\alpha},\mathfrak{g}^{-\alpha}]$是维数1。包含唯一元素$H_{\alpha}$使得$\alpha (H_{\alpha}) = 2$。

(iii) 向量子空间 $\mathfrak{s}_{\alpha}=\mathfrak{h}_{\alpha}+\mathfrak{g}^{\alpha}+\mathfrak{g}^{-\alpha}$ 是 $\mathfrak{g}$ 的谎言子代数。

(iv) 如果$X_{\alpha}$是$\mathfrak{g}^{\alpha}$的非零元素，则存在唯一的$X_{-\alpha}\in \mathfrak{g}^{-\alpha}$使得$[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$。令$\varphi$为从$\mathfrak{s}\mathfrak{l}(2, k)$到$\mathfrak{g}$的线性映射，需要$X_+$到$X_{\alpha},X_-$到$X_{-\alpha}$，以及$H$到$H_{\alpha}$；那么$\varphi$就是从李代数$\mathfrak{s}\mathfrak{l}(2, k)$到李代数$\mathfrak{s}_{\alpha}$的同构。

a) 令$h_{\alpha}$为$\mathfrak{h}$的唯一元素，使得$\alpha (h) =\langle h_{\alpha}, h\rangle$对于所有$h\in \mathfrak{h}$。根据提案 $1, [x, y] =\langle x, y\rangle h_{\alpha}$ 适用于所有 $x\in \mathfrak{g}^{\alpha},y\in \mathfrak{g}^{-\alpha}$；另一方面$\langle \mathfrak{g}^{\alpha},\mathfrak{g}^{-\alpha}\rangle  \not= 0$。因此$\mathfrak{h}_{\alpha}= [\mathfrak{g}^{\alpha},\mathfrak{g}^{-\alpha}] =kh_{\alpha}$。

b) 选择$x\in \mathfrak{g}^{\alpha},y\in \mathfrak{g}^{-\alpha}$使得$\langle x, y\rangle = 1$，所以$[x, y] =h_{\alpha}$。回想一下$[h_{\alpha}, x] =\alpha (h_{\alpha})x, [h_{\alpha}, y] =-\alpha (h_{\alpha})y$。如果$\alpha (h_{\alpha}) = 0$，则$kx+ky+kh_{\alpha}$是$\mathfrak{g}$的幂零子代数$\mathfrak{t}$；由于$h_{\alpha}\in [\mathfrak{t},\mathfrak{t}]$，ad$_{\mathfrak{g}}h_{\alpha}$是幂零的（第I, §5, no. 3，第1章），这是荒谬的，因为ad$_{\mathfrak{g}}h_{\alpha}$非零半单。所以$\alpha (h_{\alpha})\not= 0$。因此存在唯一的$H_{\alpha}\in \mathfrak{h}_{\alpha}$使得$\alpha (H_{\alpha}) = 2$，这证明了(ii)。

c) 选择 $\mathfrak{g}^{\alpha}$ 的非零元素 $X_{\alpha}$。存在$X_{-\alpha}\in \mathfrak{g}^{-\alpha}$使得$[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$（从$[X_{\alpha},\mathfrak{g}^{-\alpha}] =\mathfrak{h}_{\alpha}$到$b$）$)$。然后

$$
[H_{\alpha}, X_{\alpha}] =\alpha (H_{\alpha})X_{\alpha}= 2X_{\alpha},[H_{\alpha}, X_{-\alpha}] =-\alpha (H_{\alpha})X_{-\alpha}=-2X_{-\alpha}
$$

$$
[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}
$$

因此$kX_{\alpha}+kX_{-\alpha}+kH_{\alpha}$是$\mathfrak{g}$的子代数，并且从$\mathfrak{s}\mathfrak{l}(2, k)$到$kX_{\alpha}+kX_{-\alpha}+kH_{\alpha}$的线性映射$\varphi$使得$\varphi (X_+) =X_{\alpha},\varphi (X_-) =X_{-\alpha}$，$\varphi (H) =H_{\alpha}$是李代数的同构。

d) 假设暗淡$\mathfrak{g}^{\alpha}>1$。令 $y$ 为 $\mathfrak{g}^{-\alpha}$ 的非零元素。存在 $\mathfrak{g}_{\alpha}$ 的非零元素 $X_{\alpha}$，使得 $\langle y, X_{\alpha}\rangle = 0$。 选择$X_{-\alpha}$如c)中，并考虑从$\mathfrak{s}\mathfrak{l}(2, k)$到$\mathfrak{g}$的表示$\rho :u \rightarrow$和$_{\mathfrak{g}}\varphi (u)$。我们有

$$
\rho (H)y= [\varphi (H), y] = [H_{\alpha}, y] =-2y
$$

$$
\rho (X_+)y= [\varphi (X_+), y] = [X_{\alpha}, y] =\langle X_{\alpha}, y\rangle h_{\alpha}= 0
$$

因此，$y$对于权$-2$的$\rho$来说是原语，这是与……矛盾§1, no. 2的第2条命题。这就证明了(i)。

e) 断言 (iii) 现在是 c) 的推论。另一方面，如果$X_{\alpha}$是$\mathfrak{g}^{\alpha}$的非零元素，则c)中构造的元素$X_{-\alpha}$是$\mathfrak{g}^{-\alpha}$的唯一元素，使得$[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$自昏暗$\mathfrak{g}^{-\alpha}= 1$以来。 (iv) 的最后一个断言是c) 的推论。 Q.E.D.

记号 $h_{\alpha},H_{\alpha},\mathfrak{s}_{\alpha}$ 将在下文中保留。 （对于定义$h_{\alpha}$，我们取$\langle \cdot ,\cdot \rangle$等于杀戮形式。）如果$X_{\alpha}$是$\mathfrak{g}^{\alpha}$的非零元素，则Th的同构$\varphi$。 1 和 $\mathfrak{g}$ 上 $\mathfrak{s}\mathfrak{l}(2, k)$ 的表示 $u \rightarrow$ ad$_{\mathfrak{g}}\varphi (u)$ 将被认为与 $X_{\alpha}$ 相关联。

#### 推论{#lie-viii-s2-n2-cor-1 .statement tag=00YT}

令$\Phi$为$\mathfrak{g}$的杀戮形式。对于所有$a, b\in \mathfrak{h}$，

$$
\Phi (a, b) =\sum_{\gamma\in R}\gamma (a)\gamma (b)
$$

事实上，ad $a$.ad $b$ 使每个 $\mathfrak{g}^{\gamma}$ 保持稳定，并且其限制到 $\mathfrak{g}^{\gamma}$ 是位似，比率为 $\gamma (a)\gamma (b)$；如果$\gamma \not= 0$，则变暗$\mathfrak{g}^{\gamma}= 1$。

#### 命题 2 {#lie-viii-s2-prop-2 .statement tag=00YU}

让$\alpha , \beta \in R$。

（一）$\beta (H_{\alpha})\in \mathbf{Z}$。

(ii) 如果$\Phi$表示$\mathfrak{g},\Phi (H_{\alpha}, H_{\beta})\in \mathbf{Z}$的杀戮形式。

令$X_{\alpha}$为$\mathfrak{g}^{\alpha}$的非零元素，并令$\rho$为与$X_{\alpha}$伴随的$\mathfrak{g}$上的$\mathfrak{s}\mathfrak{l}(2, k)$的表示。 $\rho (H)$中的特征值为0，$\beta (H_{\alpha})$为$\beta \in R$。因此 (i) 从 §1, no. 2 得出，Cor.提案 2 的断言 (ii) 由 (i) 和 Cor. 得出。的 Th。 1.Q.E.D.

令$\alpha \in R,X_{\alpha}$为$\mathfrak{g}^{-\alpha}$的$\mathfrak{g}^{\alpha},X_{-\alpha}$元素的非零元素，使得$[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$和$\mathfrak{g}$上的$\mathfrak{s}\mathfrak{l}(2, k)$的$\rho$表示与$X_{\alpha}$相关联。设$\pi$为$\mathfrak{g}$上$\mathbf{S}\mathbf{L}(2, k)$的表示，与$\rho ($§1, no. 4兼容，Th。 2）。由于 ad $X_{\alpha}$ 是幂零的（第 VII, §1, no. 3 章，命题 10 (iv)），$\pi (e^{X_+}) =e^{adX_{\alpha}}$ 是 $\mathfrak{g}$ 的初等自同构。类似地，$\pi (e^{X_-}) =$$e^{adX_{-\alpha}}$是$\mathfrak{g}$的初等自同构。因此$\pi (\mathbf{S}\mathbf{L}(2, k))\subset$Aut$_e(\mathfrak{g})$。我们利用§1, no. 5的记号$\theta (t)$。对于$t\in k^*$，输入

$$
\theta_{\alpha}(t) =\pi (\theta (t)) =e^{adtX_{\alpha}}e^{adt^{-1}X_{-\alpha}}e^{adtX_{\alpha}} \tag{1}
$$

#### 引理 1 {#lie-viii-s2-lem-1 .statement tag=00YV}

(i) 对于所有$h\in \mathfrak{h},\theta_{\alpha}(t).h=h-\alpha (h)H_{\alpha}$。

(ii) 对于所有$\beta \in R,\theta_{\alpha}(t)(\mathfrak{g}^{\beta}) =\mathfrak{g}^{\beta-\beta(H_{\alpha})\alpha}$。

(iii) 如果 $\alpha , \beta \in R,\beta -\beta (H_{\alpha})\alpha \in R$。

让$h\in \mathfrak{h}$。如果$\alpha (h) = 0, [X_{\alpha}, h] = [X_{-\alpha}, h] = 0$，那么$\theta_{\alpha}(t).h=h$。另一方面，§1, no. 5的公式(5)表明$\theta_{\alpha}(t).H_{\alpha}=-H_{\alpha}$。这就证明了断言(i)。由此可见 $\theta_{\alpha}(t)^2|\mathfrak{h}=$ Id。如果$x\in \mathfrak{g}^{\beta}$和$h\in \mathfrak{h}$，

$$
[h, \theta_{\alpha}(t)x] =\theta_{\alpha}(t).[\theta_{\alpha}(t)h, x]-\beta (\theta_{\alpha}(t)h).\theta_{\alpha}(t)x
$$

$$
= (\beta (h)-\alpha (h)\beta (H_{\alpha})).\theta_{\alpha}(t)x
$$

$$
= (\beta -\beta (H_{\alpha})\alpha )(h).\theta_{\alpha}(t)x
$$

所以$\theta_{\alpha}(t)x\in \mathfrak{g}^{\beta-\beta(H_{\alpha})\alpha}$。这就证明了(ii)。 断言 (iii) 由 (ii) 得出。

#### 定理 2 {#lie-viii-s2-thm-2 .statement tag=00YW}

(i) 集合 $R = R(\mathfrak{g},\mathfrak{h})$ 是 $\mathfrak{h}^*$ 中的约化根系。

(ii) 设 $\alpha \in R$。从$\mathfrak{h}^*$到$\mathfrak{h}^*$的映射$s_{\alpha ,H_{\alpha}}:\lambda  \rightarrow \lambda -\lambda (H_{\alpha})\alpha$是$\mathfrak{h}^*$的唯一反射$s$，这样$s(\alpha ) =-\alpha$和$s(R) = R$。对于所有 $t\in k^*$，$s$ 是转置 / $\theta_{\alpha}(t)|\mathfrak{h}$。

首先，R 生成 $\mathfrak{h}^*$，因为如果$h\in \mathfrak{h}$对于所有$\alpha \in R$来说是$\alpha (h) = 0$，那么$h= 0$，因此$h= 0$，因为$\mathfrak{g}$的中心是零。 定义、$0\notin R$。让$\alpha \in R$。由于$\alpha (H_{\alpha}) = 2,s=s_{\alpha ,H_{\alpha}}$是$s(\alpha ) =-\alpha$的反射。然后 $s(R) = R$ 乘以引理 1 (iii)，以及 $\beta (H_{\alpha})\in \mathbf{Z}$ 对于所有 $\beta \in R$（提案 2 (i)）。这表明R是$\mathfrak{h}^*$中的根系。对于所有 $h\in \mathfrak{h}$ 和 $\lambda \in \mathfrak{h}^*$，

$$
\langle s(\lambda ), h\rangle =\langle \lambda -\lambda (H_{\alpha})\alpha , h\rangle =\langle \lambda , h-\alpha (h)H_{\alpha}\rangle =\langle \lambda , \theta_{\alpha}(t)h\rangle
$$

所以$s$是$\theta_{\alpha}(t)|\mathfrak{h}$的转置。最后，我们证明根系 R 被减少了。设$\alpha \in R$和$y\in \mathfrak{g}^{2\alpha}$。自$3\alpha  \notin R$（第VI, §1, no. 3章，提案$8$）$, [X_{\alpha}, y] = 0$；另一方面，$[X_{-\alpha}, y]\in \mathfrak{g}^{-\alpha+2\alpha}=\mathfrak{g}^{\alpha}=kX_{\alpha}$，所以$[X_{\alpha},[X_{-\alpha}, y]] = 0$；因此

$$
4y= 2\alpha (H_{\alpha})y= [H_{\alpha}, y] =-[[X_{\alpha}, X_{-\alpha}], y] = 0
$$

所以$y= 0$和$\mathfrak{g}^{2\alpha}= 0$。在其他字中，$2\alpha$不是根。 Q.E.D.

认同 $\mathfrak{h}$ 与 $\mathfrak{h}^{**}$ 规范一致。与第 4 章的记号一起。 VI, §1, no. 1，然后我们就有了，到 Th。 2(二)、

$H_{\alpha}=\alpha^{\vee}$ 对于所有$\alpha \in R$。 (2)

The $H_{\alpha}$ thus form the root system $R^{\vee}$ in $\mathfrak{h}$ inverse to R.

我们将调用$(\mathfrak{g},\mathfrak{h})$的$R(\mathfrak{g},\mathfrak{h})$根系。反射$s_{\alpha ,H_{\alpha}}$将简单地用$s_{\alpha}$表示。 Weyl 群、权的群、Coxeter 数 $. .$。 $R(\mathfrak{g},\mathfrak{h})$ 称为Weyl 群、权的群、Coxeter 数 $. .$。 $(\mathfrak{g},\mathfrak{h})$。正如第 1 章中那样。 VI, §1, no. 1，我们认为Weyl群不仅在$\mathfrak{h}^*$上运行，而且在$\mathfrak{h}$上运行结构的迁移，因此$s_{\alpha}=\theta_{\alpha}(t)|\mathfrak{h}$。由于$\theta_{\alpha}(t)$是$\mathfrak{g}$的初等自同构，我们有：

#### 推论{#lie-viii-s2-n2-cor-2 .statement tag=00YX}

$(\mathfrak{g},\mathfrak{h})$ 的 Weyl 群的每个元素，在 $\mathfrak{h}$ 上运行，是 $\mathfrak{g}$ 的初等自同构的限制到 $\mathfrak{h}$。

对于该结果的逆命题，请参见§5, no. 2，命题 4。

#### 注 1 {#lie-viii-s2-n2-rem-1 .statement tag=00YY}

If $\mathfrak{h}_{\mathbf{Q}}$ (resp. $\mathfrak{h}^*_{\mathbf{Q}}$) denotes the $\mathbf{Q}$-vector subspace of $\mathfrak{h}$ (resp. $\mathfrak{h}^*$) generated by the $H_{\alpha}$ (resp. the $\alpha$ ), where $\alpha \in R$, then $\mathfrak{h}$ (resp. $\mathfrak{h}^*$) can be identified canonically with $\mathfrak{h}_{\mathbf{Q}}\otimes_{\mathbf{Q}}k$ (resp. with $\mathfrak{h}^*_{\mathbf{Q}}\otimes_{\mathbf{Q}}k$) and $\mathfrak{h}^*_{\mathbf{Q}}$ can be identified with the dual of $\mathfrak{h}_{\mathbf{Q}}$ (Chap. VI, §1, no. 1, Prop. 1). 我们将$\mathfrak{h}_{\mathbf{Q}}$和$\mathfrak{h}^*_{\mathbf{Q}}$称为$\mathfrak{h}$和$\mathfrak{h}^*($代数上的规范$\mathbf{Q}$结构，第1章。 II, §8, no. 1，防御。 1）。 当我们提到$\mathfrak{h}$的向量子空间的$\mathbf{Q}$-有理性，$\mathfrak{h}$的线性形式等等，我们指的是这些结构，除非，我们另有说明。 当我们提到$R(\mathfrak{g},\mathfrak{h})$的Weyl室或面时，我们将在$\mathfrak{h}_{\mathbf{Q}}\otimes_{\mathbf{Q}}\mathbf{R}$或$\mathfrak{h}^*_{\mathbf{Q}}\otimes_{\mathbf{Q}}\mathbf{R}$工作，我们将用$\mathfrak{h}_{\mathbf{R}}$和$\mathfrak{h}^*_{\mathbf{R}}$表示。

#### 注 2 {#lie-viii-s2-n2-rem-2 .statement tag=00YZ}

$\mathfrak{h}$ 定义中的根系 $R^{\vee}$ $\mathfrak{h}$ 上的非简并对称双线性形式 $\beta$（第 VI, §1, no. 1 章，第 3 条命题），即形式 $(a, b) \rightarrow$ $\sum_{\alpha\in R}\langle \alpha , a\rangle \langle \alpha , b\rangle$。由科。至 Th。 1、这个形式只是其中的限制

杀死形式到$\mathfrak{h}$。 $\beta |\mathfrak{h}_{\mathbf{Q}}\times \mathfrak{h}_{\mathbf{Q}}$到$\mathfrak{h}_{\mathbf{Q}}\otimes_{\mathbf{Q}}\mathbf{R}$的扩张是正非简并的（第VI, §1, no. 1章，命题3）。另一方面，我们看到$\mathfrak{g}$上的杀戮形式的限制到$\mathfrak{h}$的$\mathfrak{h}^*$的逆形式是R的规范双线性形式$\Phi_R$（第VI, §1, no. 12章）。

令$(\mathfrak{g}_1,\mathfrak{h}_1), (\mathfrak{g}_2,\mathfrak{h}_2)$为分裂的半单李代数、$\varphi$同构，从$\mathfrak{g}_1$到$\mathfrak{g}_2$，使得$\varphi (\mathfrak{h}_1) =\mathfrak{h}_2$。到结构迁移，映射$\varphi |\mathfrak{h}_1$转置需要$R(\mathfrak{g}_2,\mathfrak{h}_2)$到$R(\mathfrak{g}_1,\mathfrak{h}_1)$。

#### 命题 3 {#lie-viii-s2-prop-3 .statement tag=00Z0}

设$\mathfrak{g}$为$\mathfrak{g}$的半单李代数、$\mathfrak{h}_1$和$\mathfrak{h}_2$分裂嘉当子代数。从$\mathfrak{h}^*_1$到$\mathfrak{h}^*_2$存在同构需要$R(\mathfrak{g},\mathfrak{h}_1)$到$R(\mathfrak{g},\mathfrak{h}_2)$。

（要获得更精确的结果，请参阅第 10 号提案的§3, no. 3 和第 5 号提案§5, no. 3）。

设$k'$为$k,\mathfrak{g}'=\mathfrak{g}\otimes_kk',\mathfrak{h}'_i=\mathfrak{h}_i\otimes_kk'$的代数闭包。那么$R(\mathfrak{g}',\mathfrak{h}'_i)$就是从$\mathfrak{h}^*_i$到$\mathfrak{h}^*_i\otimes_kk'={\mathfrak{h}'_i}^*$在映射$\lambda  \rightarrow \lambda \otimes 1$下$R(\mathfrak{g},\mathfrak{h}_i)$的像。由章。 VII, §3, no. 2，周四。 1，存在$\mathfrak{g}'$的自同构需要$\mathfrak{h}'_1$到$\mathfrak{h}'_2$，因此同构$\varphi$从${\mathfrak{h}'_1}^*$到${\mathfrak{h}'_2}^*$需要$R(\mathfrak{g}',\mathfrak{h}'_1)$到$R(\mathfrak{g}',\mathfrak{h}'_2)$。然后$\varphi |\mathfrak{h}^*_1$将$R(\mathfrak{g},\mathfrak{h}_1)$带到$R(\mathfrak{g},\mathfrak{h}_2)$，因此将$\mathfrak{h}^*_1$带到$\mathfrak{h}^*_2$。 Q.E.D.

根据命题 3，$(\mathfrak{g},\mathfrak{h})$ 的根系，直至同构，仅取决于$\mathfrak{g}$，而不取决于$\mathfrak{h}$。 In the same way, the Weyl group, group of weights $. .$. of $(\mathfrak{g},\mathfrak{h})$ are simply called, by abuse of language, the Weyl group, group of weights $. .$. of $\mathfrak{g}$ (cf. also §5, no. 3, Remark 2). 如果$\mathfrak{g}$的Dynkin图是型$A_l$或$B_l,. .$。 （cf.章VI, §4, no. 2，第3章），我们说$\mathfrak{g}$是型$A_l$，或$B_l,. .$..

回想一下，如果$\alpha$和$\beta$是线性独立的根、集合与$j\in \mathbf{Z}$，使得$\beta +j\alpha \in R$是$\mathbf{Z}$包含0的区间$[-q, p]$，其中$p-q=$$-\langle \beta , \alpha^{\vee}\rangle =-\beta (H_{\alpha})$（第1章） VI, §1, no. 3，提案 9）。

#### 命题 4 {#lie-viii-s2-prop-4 .statement tag=00Z1}

令$\alpha$和$\beta$线性无关根。令$p$（分别$q$）为最大的整数$j$，使得$\beta +j\alpha$（分别$\beta -j\alpha$）为根。

(i) $\mathfrak{g}$ 的向量子空间 $\sum_{-q\leq j\leq p}\mathfrak{g}^{\beta+j\alpha}$ 是维数 $p+q+ 1$ 的简单$\mathfrak{s}_{\alpha}$ 模块。

(ii) 如果$\alpha +\beta$是根，则$[\mathfrak{g}^{\alpha},\mathfrak{g}^{\beta}] =\mathfrak{g}^{\alpha+\beta}$。

令$X_{\alpha}$（或$x$）为$\mathfrak{g}^{\alpha}$（或$\mathfrak{g}^{\beta+p\alpha}$）的非零元素。然后

$$
[X_{\alpha}, x]\in \mathfrak{g}^{\beta+(p+1)\alpha}= 0
$$

$$
[H_{\alpha}, x] = (\beta (H_{\alpha}) +p\alpha (H_{\alpha}))x= (-p+q+ 2p)x= (p+q)x
$$

因此，对于与 $X_{\alpha}$ 伴随的 $\mathfrak{g}$ 上的 $\mathfrak{s}\mathfrak{l}(2, k)$ 的表示，$x$ 是权 $p+q$ 的原语；但$\mathfrak{s}\mathfrak{l}(2, k$)-模块$\sum_{-q\leq j\leq p}\mathfrak{g}^{\beta+j\alpha}$是维数$p+q+ 1$；因此它很简单（§1, no. 2，命题 2）。如果$\alpha +\beta \in R$，则$p\geq 1$，因此$\mathfrak{g}^{\beta}$的元素不是原始的，因此$[X_{\alpha},\mathfrak{g}^{\beta}]\not= 0$。从$[\mathfrak{g}^{\alpha},\mathfrak{g}^{\beta}]\subset$$\mathfrak{g}^{\alpha+\beta}$开始，我们终于看到了$[\mathfrak{g}^{\alpha},\mathfrak{g}^{\beta}] =\mathfrak{g}^{\alpha+\beta}$。

#### 注 3 {#lie-viii-s2-n2-rem-3 .statement tag=00Z2}

回想一下，章。 VI, §1, no. 3，科。 9号命题中，整数$p+q+ 1$只能取值$1,2,3,4$。

#### 注 4 {#lie-viii-s2-n2-rem-4 .statement tag=00Z3}

令$(\mathfrak{g},\mathfrak{h})$为分裂约化李代数、$\mathfrak{c}$中心/$\mathfrak{g},\mathfrak{g}'=\mathscr{D}\mathfrak{g}$、$\mathfrak{h}'=\mathfrak{h}\cap \mathfrak{g}'$。然后$\mathfrak{h}=\mathfrak{c}\times \mathfrak{h}'$，我们认同$\mathfrak{h}^{'*}$和向量子空间$\mathfrak{h}^*$。对于任何$\lambda \in \mathfrak{h}^*$使得$\lambda \not= 0$，相对于$\lambda$的主子空间$\mathfrak{g}^{\lambda}$等于${\mathfrak{g}'}^{\lambda|\mathfrak{h}'}$。 $\mathfrak{g}$ 上$\mathfrak{h}$ 的非零权称为$(\mathfrak{g},\mathfrak{h})$ 的根；每个根都会在$\mathfrak{c}$消失。用$(\mathfrak{g},\mathfrak{h})$根$R(\mathfrak{g},\mathfrak{h})$集合表示；它可以用 $R(\mathfrak{g}',\mathfrak{h}')$ 来规范地识别。让$\alpha \in R(\mathfrak{g},\mathfrak{h})$。我们将$\mathfrak{g}$上的$\mathfrak{s}\mathfrak{l}(2, k)$的定义$h_{\alpha},H_{\alpha}$、$\mathfrak{s}_{\alpha}$、同构$\mathfrak{s}\mathfrak{l}(2, k)\rightarrow \mathfrak{s}_{\alpha}$和表示与$\alpha$相关联，如半单情况一样。

### 3. INVARIANT BILINEAR FORMS

#### 命题 5 {#lie-viii-s2-prop-5 .statement tag=00Z4}

令$(\mathfrak{g},\mathfrak{h})$为分裂的半单李代数，$\Phi$为$\mathfrak{g}$上的不变对称双线性形式，W为$(\mathfrak{g},\mathfrak{h})$的Weyl群。那么$\Phi$到$\mathfrak{h}$的限制$\Phi '$在W下是不变的。此外，如果$\Phi$是非简并的，$\Phi '$也是非简并的。

令$\alpha \in R$，令$X_{\alpha}$为$\mathfrak{g}^{\alpha},\rho$的非零元素，与$\mathfrak{g}$上$\mathfrak{s}\mathfrak{l}(2, k)$的关联表示，以及$\mathfrak{g}$上$\mathbf{S}\mathbf{L}(2, k)$的$\pi$表示兼容$\rho$。那么$\Phi$在$\rho$下是不变的，因此在$\pi ($§1, no. 4下是不变的）。特别是，$\Phi '$ 在 $\theta_{\alpha}(t)|\mathfrak{h}$ (no. 2) 下是不变的，因此在 W 下，最后一个断言由命题 1 (i) 得出。

#### 命题 6 {#lie-viii-s2-prop-6 .statement tag=00Z5}

令$(\mathfrak{g},\mathfrak{h})$为分裂的半单李代数，$\Phi$为$\mathfrak{g}$上的非简并不变对称双线性形式。对于所有$\alpha \in R$，令$X_{\alpha}$为$\mathfrak{g}^{\alpha}$的非零元素。令$(H_i)_{i\in I}$为$\mathfrak{h}$的基，且$(H'_i)_{i\in I}$基为$\mathfrak{h}$，使得$\Phi (H_i, H'_j) =\delta_{ij}$。 $\mathfrak{g}$（第I, §3, no. 7）的包络线代数中与$\Phi$相关联的卡西米尔元素则为

$$
\sum\frac{1}{\Phi(X_{\alpha}, X_{-\alpha})}X_{\alpha}X_{-\alpha}+\sum H_iH'_i
$$

$\alpha \in Ri\in I$

事实上，根据提案，$1,\Phi (H_i, X_{\alpha}) =\Phi (H'_i, X_{\alpha}) = 0$适用于所有$i\in I,\alpha \in R$，$\Phi (\frac{1}{\Phi(X_{\alpha},X_{-\alpha})}X_{\alpha}, X_{-\beta})=\delta_{\alpha \beta}$适用于所有$\alpha , \beta \in R$。

### 4. 系数 N$_{\boldsymbol{\alpha \beta }}$

在这个数中，我们再次用$(\mathfrak{g},\mathfrak{h})$分裂的半单李代数来表示。

#### 引理 2 {#lie-viii-s2-lem-2 .statement tag=00Z6}

存在一个族$(X_{\alpha})_{\alpha\in R}$，对于所有$\alpha \in R$，

$X_{\alpha}\in \mathfrak{g}^{\alpha}$ 和 $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$。

令$R_1$为R的子集，使得$R = R_1\cup (-R_1)$和$R_1\cap (-R_1) =\emptyset$。对于 $\alpha \in R_1$、选择 $\mathfrak{g}^{\alpha}$ 的任意非零元素 $X_{\alpha}$。存在唯一的$X_{-\alpha}\in \mathfrak{g}^{-\alpha}$使得$[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$（Th.1（iv））。然后

$$
[X_{-\alpha}, X_{\alpha}] =H_{\alpha}=-H_{-\alpha}.Q.E.D
$$

如果$(X_{\alpha})_{\alpha\in R}$是引理2个家庭满足条件，那么最一般的家庭满足这些条件就是$(t_{\alpha}X_{\alpha})_{\alpha\in R}$，其中$t_{\alpha}\in k^*$和$t_{\alpha}t_{-\alpha}= 1$代表所有$\alpha \in R$。

在这个数的其余部分中，我们用$(X_{\alpha})_{\alpha\in R}$表示引理2的族满足条件。我们用$\langle \cdot ,\cdot \rangle$表示$\mathfrak{g}$上的非简并不变对称双线性形式。

每个$x\in \mathfrak{g}$都可以唯一地写成形式

$$
x=h+\sum_{\alpha\in R}\mu_{\alpha}X_{\alpha}(h\in \mathfrak{h}, \mu_{\alpha}\in k)
$$

两个这样的元素的括号可以通过以下公式来计算：

$$
[h, X_{\alpha}] =\alpha (h)X_{\alpha}
$$

0 如果 $\alpha +\beta  \notin R\cup  \{0\}$

$[X_{\alpha}, X_{\beta}] =-H_{\alpha}$如果$\alpha +\beta = 0$

$N_{\alpha \beta}X_{\alpha+\beta}$ 如果 $\alpha +\beta \in R$

$N_{\alpha \beta}$ $k$ 的非零元素。

#### 引理 3 {#lie-viii-s2-lem-3 .statement tag=00Z7}

对于所有$\alpha \in R$，

$$
\langle X_{\alpha}, X_{-\alpha}\rangle =-\frac{1}{2}\langle H_{\alpha}, H_{\alpha}\rangle
$$

确实，

$$
2\langle X_{\alpha}, X_{-\alpha}\rangle =\langle \alpha (H_{\alpha})X_{\alpha}, X_{-\alpha}\rangle =\langle [H_{\alpha}, X_{\alpha}], X_{-\alpha}\rangle
$$

$$
=\langle H_{\alpha},[X_{\alpha}, X_{-\alpha}]\rangle =-\langle H_{\alpha}, H_{\alpha}\rangle
$$

#### 引理 4 {#lie-viii-s2-lem-4 .statement tag=00Z8}

令$\alpha , \beta \in R$ 使得$\alpha +\beta \in R$。令$p$（或$q$）为最大的整数$j$，使得$\beta +j\alpha \in R$（或$\beta -j\alpha \in R$）。然后，

$$
N_{\alpha ,\beta}N_{-\alpha ,\alpha+\beta}=-p(q+ 1) \tag{3}
$$

$$
N_{-\alpha ,\alpha+\beta}\langle H_{\beta}, H_{\beta}\rangle =-N_{-\alpha ,-\beta}\langle H_{\alpha+\beta}, H_{\alpha+\beta}\rangle \tag{4}
$$

$$
N_{\alpha ,\beta}N_{-\alpha ,-\beta}= (q+ 1)^2 \tag{5}
$$

令 $\rho$ 为 $\mathfrak{s}\mathfrak{l}(2, k)$ 在由 $X_{\alpha}$ 定义的 $\mathfrak{g}$ 上的表示。 元素 $e=X_{\beta+p\alpha}$ 是权 $p+q$ 的原语（命题 4 (i)）。放

$e_n=(-n1)$！ $^n\rho (X_-)^ne$ 换$n\geq 0$。

根据§1第1条，

（广告$X_{\alpha}$）$e_p= (q+ 1)e_{p-1}$

（广告$X_{-\alpha}$）（广告$X_{\alpha}$）$e_p=-p(q+ 1)e_p$。

这证明了(3)，因为$e_p$是$\mathfrak{g}^{\beta}$的非零元素。

形式 $\langle \cdot ,\cdot \rangle$ 不变，我们有

$$
\langle [X_{-\alpha}, X_{\alpha+\beta}], X_{-\beta}\rangle =-\langle X_{\alpha+\beta},[X_{-\alpha}, X_{-\beta}]\rangle
$$

所以

$$
N_{-\alpha ,\alpha+\beta}\langle X_{\beta}, X_{-\beta}\rangle =-N_{-\alpha ,-\beta}\langle X_{\alpha+\beta}, X_{-\alpha-\beta}\rangle
$$

鉴于引理 3，证明 (4)。

$\langle \cdot ,\cdot \rangle$ 到 $\mathfrak{h}$ 的限制在 Weyl 群（命题 5）下是非简并且不变的。 认同$\mathfrak{h}$和$\mathfrak{h}^*$通过这个限制。如果$\gamma \in R,H_{\gamma}$与$2\gamma /\langle \gamma , \gamma \rangle$相同（第VI, §1, no. 1、引理2章）；因此，对于所有 $\gamma , \delta \in R$，

$$
\langle \gamma , \gamma \rangle \langle H_{\delta}, H_{\delta}\rangle
$$

$$
\overline{\langle\delta , \delta\rangle}=\overline{\langle H_{\gamma}, H_{\gamma}\rangle} \tag{6}
$$

现在，由章。 VI, §1, no. 3，提案 10，

$$
\frac{\langle\alpha + \beta , \alpha + \beta\rangle}{\langle\beta , \beta\rangle}=\frac{q + 1}{p} \tag{7}
$$

因此，由 (3), (4), (6), (7),

$$
N_{\alpha ,\beta}N_{-\alpha ,-\beta}=-N_{\alpha ,\beta}N_{-\alpha ,\alpha+\beta}\frac{\langle H_{\beta}, H_{\beta}\rangle}{\langle H_{\alpha+\beta}, H_{\alpha+\beta}\rangle}
$$

$$
=-N_{\alpha ,\beta}N_{-\alpha ,\alpha+\beta}\frac{q + 1}{p}= (q+ 1)^2
$$

#### 定义 3 {#lie-viii-s2-def-3 .statement tag=00Z9}

$(\mathfrak{g},\mathfrak{h})$ 的 Chevalley 系统是一个$(X_{\alpha})_{\alpha\in R}$ 族，使得

(i) $X_{\alpha}\in \mathfrak{g}^{\alpha}$ 对于所有 $\alpha \in R$；

(ii) $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ 对于所有 $\alpha \in R$；

(iii) 从$\mathfrak{g}$到$\mathfrak{g}$的线性映射等于$\mathfrak{h}$上的$-1$，并且对于所有$\alpha \in R$需要$X_{\alpha}$到$X_{-\alpha}$，是$\mathfrak{g}$的自同构。

这个定义的扩张对于$(\mathfrak{g},\mathfrak{h})$是分裂的还原的情况是直接的。

我们将证明（§4, no. 4，Prop. 5 的 Cor.）$(\mathfrak{g},\mathfrak{h})$ 的 Chevalley 系统存在。

#### 命题 7 {#lie-viii-s2-prop-7 .statement tag=00ZA}

令 $(X_{\alpha})_{\alpha\in R}$ 为 $(\mathfrak{g},\mathfrak{h})$ 的 Chevalley 系统。我们保留引理 4 中的记号。然后，$N_{-\alpha ,-\beta}= N_{\alpha ,\beta}$ 和$N_{\alpha ,\beta}=\pm (q+ 1)$ 代表$\alpha , \beta , \alpha +\beta \in R$。

令 $\varphi$ 为 Def 中考虑的 $\mathfrak{g}$ 中的自同构。 3（三）。然后

$$
N_{-\alpha ,-\beta}X_{-\alpha-\beta}= [X_{-\alpha}, X_{-\beta}] = [\varphi (X_{\alpha}), \varphi (X_{\beta})] =\varphi ([X_{\alpha}, X_{\beta}])
$$

$$
=\varphi (N_{\alpha ,\beta}X_{\alpha+\beta}) = N_{\alpha ,\beta}X_{-\alpha-\beta}
$$

所以$N_{-\alpha ,-\beta}= N_{\alpha ,\beta}$。现在$N_{\alpha ,\beta}=\pm (q+ 1)$乘以(5)。

#### 命题 8 {#lie-viii-s2-prop-8 .statement tag=00ZB}

令 $(X_{\alpha})_{\alpha\in R}$ 为 $(\mathfrak{g},\mathfrak{h})$ 的 Chevalley 系统。设 M 是 $\mathfrak{h}$ 包含于 $H_{\alpha}$ 的$\mathbf{Z}$子模，并包含在$R^{\vee}$的权的群中。令$\mathfrak{g}_{\mathbf{Z}}$为由M和$X_{\alpha}$生成的$\mathfrak{g}$的$\mathbf{Z}$子模。那么$\mathfrak{g}_{\mathbf{Z}}$是$\mathfrak{g}$的$\mathbf{Z}$-谎言子代数，并且从$\mathfrak{g}_{\mathbf{Z}}\otimes_{\mathbf{Z}}k$到$\mathfrak{g}$的规范映射是同构。

如果$\alpha , \beta \in R$使得$\alpha +\beta \in R$，则$N_{\alpha ,\beta}\in \mathbf{Z}$（命题7）。另一方面，如果$\alpha \in R$和$h\in M$，则$\alpha (h)\in \mathbf{Z}$（第VI, §1, no. 9章）。这证明$\mathfrak{g}_{\mathbf{Z}}$是$\mathfrak{g}$的$\mathbf{Z}$谎言子代数。另一方面，M 是一个自由的阿贝尔的群的秩暗淡$\mathfrak{h}($代数，第 1 章。 VII, §3，周四。 1)，所以$\mathfrak{g}_{\mathbf{Z}}$是秩dim$\mathfrak{g}$的免费阿贝尔的群；这意味着最后一个断言。

### 习题{#lie-viii-s2-exercises}

参见[习题为 § 2](exercises/s2/)。
