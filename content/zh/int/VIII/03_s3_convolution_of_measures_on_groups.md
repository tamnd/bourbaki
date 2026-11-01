---
book: int
book_title: Integration
chapter: VIII
chapter_title: CONVOLUTION AND REPRESENTATIONS
section: 3
section_title: Convolution of measures on groups
lang: zh
source: int-vii-ix
book_pages: INT VIII.18-INT VIII.24, INT VIII.61-INT VIII.65
pdf_pages: 0118-0124, 0161-0165
extraction: ocr
subsections:
    - "no": 1
      title: Algebras of measures
      page: 18
      pdf_page: 118
    - "no": 2
      title: The case of a group operating on a space
      page: 21
      pdf_page: 121
    - "no": 3
      title: Convolution and linear representations
      page: 22
      pdf_page: 122
statements: 16
exercises: 13
content_sha256: f623685fe3c5cb415a35041b396c446990bff63ca3e311909a62c585b57f30e9
translated_from: content/en/int/VIII/03_s3_convolution_of_measures_on_groups.md
translation_method: google
source_content_sha256: fbb17d2d8dfca6f7e44cfa7592c87c0769532c38cc2550dc3a50ed837fd6ab29
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: b8803f15902e2f655ddeb1e3bb645c0fb04bf7302d500133d4f009eb1cdcee6c
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 3。 群上的测量卷积

### 1. 代数措施

令 G 为局部紧致群。可以一劳永逸地理解，如果 G 上的度量 $\mu_1, \ldots, \mu_n$ 对于映射也是可卷积的

$$
(x_1, x_2, \ldots, x_n) \mapsto x_1 x_2 \cdots x_n;
$$

正是通过这个映射，卷积乘积$*_{i} \mu_i$将始终被采用。如果$s \in G, t \in G$，那么

(1)
$$
\varepsilon_s * \varepsilon_t = \varepsilon_{st}.
$$

如果$s \in G$和$\mu \in \mathscr{M}(G)$，那么

(2)
$$
\varepsilon_s * \mu = \gamma(s) \mu
$$
(3)
$$
\mu * \varepsilon_s = \delta(s^{-1}) \mu
$$

由 §1, No. 1, 例 3. 如果 G 为阿贝尔的，则称 $\mu_1$ 和 $\mu_2$ 可卷积，等价于说 $\mu_2$ 和 $\mu_1$ 可卷积，则有 $\mu_1 * \mu_2 = \mu_2 * \mu_1$。当 G 不是阿贝尔的时，$\mu_1$ 和 $\mu_2$ 可能是可卷积的，而 $\mu_2$ 和 $\mu_1$ 则不然（Exer. 12）。

#### 命题 1 {#int-viii-s3-prop-1 .statement tag=09JB}

— 令 G 为局部紧致群，$\lambda, \mu, \nu$ 在 G 上测量 $\neq 0$。

(i) 如果$\lambda, \mu, \nu$是可卷积的，那么$\lambda$和$\mu$、$|\lambda| * |\mu|$和$\nu$、$\mu$和$\nu$、$\lambda$和$|\mu| * |\nu|$也是可卷积的，并且有一个

$$
\lambda * \mu * \nu = (\lambda * \mu) * \nu = \lambda * (\mu * \nu).
$$

(ii) 如果$\lambda$和$\mu$是可卷积的，以及$|\lambda| * |\mu|$和$\nu$，那么$\lambda, \mu, \nu$是可卷积的。类似地，如果$\mu$和$\nu$是可卷积的，$\lambda$和$|\mu| * |\nu|$也是如此。

这是从§1, No. 2 的第 1 条命题得出的。

G 上可以存在测度$\lambda, \mu, \nu$，使得卷积乘积、$\lambda * \mu$、$(\lambda * \mu) * \nu$、$\mu * \nu$、$\lambda * (\mu * \nu)$ 都已定义，但$(\lambda * \mu) * \nu \neq \lambda * (\mu * \nu)$ (cf. Exer.4)。

令$\rho$为$G$上的下半连续有限函数$> 0$，使得$\rho(st) \leq \rho(s)\rho(t)$适用于$G$中的所有$s, t$。我们用$G$上的$\lambda$测度的$\mathscr{M}^\rho(G)$向量空间表示，使得$\rho$是$\lambda$可积，并用$\| \lambda \|_\rho$（或简单地$\| \lambda \|$）范数$\int_G \rho(s) d|\lambda|(s)$表示空间。当$\rho = 1$时，在$G$恢复集合$\mathscr{M}^1(G)$的有界措施。

#### 命题 2 {#int-viii-s3-prop-2 .statement tag=09JC}

(i) *$\mathscr{M}^\rho(G)$ 中的任意两个元素都是可卷积的。*
(ii) *对于卷积，对于范数$\| \lambda \|$，$\mathscr{M}^\rho(G)$是完全规范的代数，承认$\varepsilon_e$为单位元元素。*
(iii) $\mathscr{C}'(G)$ *是子代数 / $\mathscr{M}^\rho(G)$*。

令$\lambda, \mu$在$\mathscr{M}^\rho(G)$中，并证明$\lambda$和$\mu$是可卷积的。让$f \in \mathscr{K}_+(G)$。由于 $\rho$ 是 $> 0$ 及下半连续，因此存在常数 $k > 0$ 使得 $f \leq k\rho$。然后

$$
\int^* f(st) d|\lambda|(s) d|\mu|(t) \leq k \int^* \rho(st) d|\lambda|(s) d|\mu|(t)
$$
$$
\leq k \int^* \rho(s)\rho(t) d|\lambda|(s) d|\mu|(t)
$$
$$
= k \left( \int^* \rho(s) d|\lambda|(s) \right) \left( \int^* \rho(t) d|\mu|(t) \right)
$$

（第 V, §8, No. 3 章，第 8 号提案第 1 条）。因此$(s,t) \mapsto f(st)$是$(\lambda \otimes \mu)$可积的，因此$\lambda$和$\mu$是可卷积的。另一方面，使用 Ch. V（§1，第 4 条命题，§6，第 2 条命题，§8，第 8 条命题第 1 条），并且事实上 $(s,t) \mapsto \rho(s)\rho(t)$ 在 $G \times G$ 中是下半连续的，有

$$
\int_G^* \rho(s) d|\lambda * \mu|(s) = \int_G^* \rho(s) d|\lambda * \mu|(s)
$$
$$
\leq \int_{G \times G}^* \rho(st) d|\lambda|(s) d|\mu|(t) \leq \int_{G \times G}^* \rho(s)\rho(t) d|\lambda|(s) d|\mu|(t)
$$
$$
= \int_{G \times G}^* \rho(s)\rho(t) d|\lambda|(s) d|\mu|(t) = \| \lambda \| \cdot \| \mu \|.
$$

人们看到$\lambda * \mu \in \mathscr{M}^\rho(G)$和$\| \lambda * \mu \| \leq \| \lambda \| \cdot \| \mu \|$。根据命题 1，$\mathscr{M}^\rho(G)$ 为代数。 映射 $\lambda \mapsto \rho \cdot \lambda$ is an isometric 线性映射 $\theta$ of $\mathscr{M}^\rho(G)$ into $\mathscr{M}^1(G)$;如果$\mu \in \mathscr{M}^1(G)$，则局部有界且上半连续的$1/\rho$是局部$\mu$可积，$\rho$是$(1/\rho) \cdot \mu$可积，因此$(1/\rho) \cdot \mu \in \mathscr{M}^\rho(G)$；这证明 $\theta$ 是满射；因此$\mathscr{M}^\rho(G)$是完全规范的代数。最后，很明显，对于$\mathscr{M}^\rho(G)$来说，$\varepsilon_e$是单位元元素，$\mathscr{C}'(G)$是$\mathscr{M}^\rho(G)$的子代数（§1, No. 4，Prop.5的Cor.）。

If $\rho = 1$, Prop. 2, (i) and (ii) also follow from §1, Prop. 2.

#### 命题 3 {#int-viii-s3-prop-3 .statement tag=09JD}

*令 $\mu_1, \ldots, \mu_n$ 为 G 上的度量。如果除最多一个之外的所有 $\mu_i$ 都具有紧支撑，则 $\mu_i$ 是可卷积的。*

For, let $S_i$ be the support of $\mu_i$, and suppose that $S_i$ is compact for $i \neq i_0$.令 K 为 G 的紧致子集。 $(x_1, \ldots, x_n) \in \prod_i S_i$ 的集合使得 $x_1 x_2 \cdots x_n \in K$ 是紧致的，因为条件 $x_i \in S_i$ 对于所有 $i$、$x_1 x_2 \cdots x_n \in K$ 意味着

$$
x_{i_0} \in S_{i_0-1}^{-1} \cdots S_1^{-1} K S_n^{-1} \cdots S_{i_0+1}^{-1} .
$$

因此 $\mu_i$ 是可卷积的（§1, No. 4，命题 4）。

#### 命题 4 {#int-viii-s3-prop-4 .statement tag=09JE}

*映射 $(\lambda, \mu) \mapsto \lambda * \mu$ (resp. $(\lambda, \mu) \mapsto \mu * \lambda$), where $\lambda \in \mathscr{C}'(G)$, $\mu \in \mathscr{M}(G)$, 定义 on $\mathscr{M}(G)$ 结构 of a left (resp. right) 模 over 代数 $\mathscr{C}'(G)$.*

This follows from Props. 1 和 3。

#### 命题 5 {#int-viii-s3-prop-5 .statement tag=09JF}

*令 $\lambda$ 为 G 上的左（或右）Haar 测度，以及 $\mu \in \mathscr{M}^1(G)$。那么 $\mu$ 和 $\lambda$（分别为 $\lambda$ 和 $\mu$）是可卷积的，并且 $\mu * \lambda = \mu(1)\lambda$（分别为 $\lambda * \mu = \mu(1)\lambda$）。*

我们可以假设$\mu \geqslant 0$。 Let $f \in \mathscr{K}_+(G)$.当$\lambda$是左哈尔测度时，

$$
\int^* d\mu(x) \int^* f(xy)\, d\lambda(y) = \int^* d\mu(x) \int f(y)\, d\lambda(y) = \lambda(f)\|\mu\| ,
$$

因此函数 $(x, y) \mapsto f(xy)$ 是 $(\mu \otimes \lambda)$ 可积的，其对 $\mu \otimes \lambda$ 的积分是 $\lambda(f)\|\mu\|$。当 $\lambda$ 是正确的哈尔测度时，人们也会提出类似的观点。

#### 命题 6 {#int-viii-s3-prop-6 .statement tag=09JG}

*令$\mu$和$\nu$为G上的两个可卷积测度。令$\chi$为G在$\mathbf{C}^*$中的连续表示。那么$\chi \cdot \mu$和$\chi \cdot \nu$是可卷积的并且$(\chi \cdot \mu) * (\chi \cdot \nu) = \chi \cdot (\mu * \nu)$。*

让$f \in \mathscr{K}(G)$。那么$f\chi \in \mathscr{K}(G)$，因此函数

$$
(x, y) \mapsto f(xy)\chi(xy) = f(xy)\chi(x)\chi(y)
$$

在$G \times G$上可积$\mu \otimes \nu$；因此函数 $(x, y) \mapsto f(xy)$ 可积为 $(\chi \cdot \mu) \otimes (\chi \cdot \nu)$；因此 $\chi \cdot \mu$ 和 $\chi \cdot \nu$ 是可卷积的。而且，

$$
\langle \chi \cdot \mu * \chi \cdot \nu, f \rangle = \int f(xy)\chi(x)\chi(y)\, d\mu(x)\, d\nu(y)
= \int (f\chi)(xy)\, d\mu(x)\, d\nu(y) = \langle \mu * \nu, \chi f \rangle ,
$$

从而$(\chi \cdot \mu) * (\chi \cdot \nu) = \chi \cdot (\mu * \nu)$。

#### 命题 7 {#int-viii-s3-prop-7 .statement tag=09JH}

*设G和G'是两个局部紧的群，u是G在G'中的连续表示，并且$\mu_1, \ldots, \mu_n$对G的测量，都是$\neq 0$。那么下面的断言是等价的：
(i) $u$ 对于所有 i 来说是 $\mu_i$-正确的，并且度量 $u(|\mu_i|)$ 是可卷积的；
(ii) $\mu_i$ 是可卷积的，$u$ 适用于 $*_{i}(|\mu_i|)$。
当这些条件满足后，

$$
*_{i} u(\mu_i) = u(*_{i} \mu_i).
$$

这是从 §1, No. 2，Cor. 得出的。提案 1。

#### 推论{#int-viii-s3-n1-cor-1 .statement tag=09JI}

*设 G 为 G 上的局部紧致群，$\mu_1, \ldots, \mu_n$ 的度量。为了使序列 $(\mu_i)_{1 \leq i \leq n}$ 可卷积，序列 $(\check{\mu}_{n-i})_{0 \leq i \leq n-1}$ 是可卷积的充分必要，在这种情况下*

$$
(\mu_1 * \cdots * \mu_n)^{\vee} = \check{\mu}_n * \cdots * \check{\mu}_1.
$$

这是从命题 7 中得出的，考虑到 G 的同构 $x \mapsto x^{-1}$ 到相反的群。

### 2. 群在空间上运行的案例

令 X 为局部紧致空间，其上局部紧致群 G 在左侧连续运算

$$
(s, x) \mapsto s \cdot x.
$$

如果 $\mu_1, \ldots, \mu_n$ 是 G 上的测度，$\nu$ 是 X 上的测度，如果它们对于 $G^n \times X$ 的映射 $(s_1, \ldots, s_n, x) \mapsto s_1 \cdots s_n x$ 进入X 是这样，那么这些将被认为是可卷积的，并且它们的卷积乘积可以这样理解映射。

如果$s \in G$和$x \in X$，那么

(4)
$$
\varepsilon_s * \varepsilon_x = \varepsilon_{sx}.
$$

如果$s \in G$和$\mu \in \mathscr{M}(X)$，那么

(5)
$$
\varepsilon_s * \mu = \gamma(s)\mu
$$
§1, No. 1、例 3。

#### 命题 8 {#int-viii-s3-prop-8 .statement tag=09JJ}

— 设$\mu$为$G$的测度，$\nu$为$X$的测度。
(i) 如果 $\mu$ 具有紧支持，则 $\mu$ 和 $\nu$ 是可卷积的。
(ii) 如果$\nu$有紧支持，并且$G$在$X$中正确运行，那么$\mu$和$\nu$是可卷积的。
这是从§1, No. 4 的第 4 号提案得出的。

#### 命题 9 {#int-viii-s3-prop-9 .statement tag=09JK}

— 对于卷积，$\mathscr{M}^1(X)$ 是 $\mathscr{M}^1(G)$ 上的左模，而 $\mathscr{M}(X)$ 和 $\mathscr{C}'(X)$ 是 $\mathscr{C}'(G)$ 上的左模。
这是从 Prop. 8 和 §1，Props. 8 得出的。 1、3 和 Cor。提案 5。

#### 命题 10 {#int-viii-s3-prop-10 .statement tag=09JL}

— 令$\mu$为$G$的测度，$\nu$为$X$、$\mu$和$\nu$的可卷积测度。假设在加法中存在$X$上的正测度$\beta$，使得对于每个$s \in G$，$\gamma(s)\nu$有基$\beta$。那么$\mu * \nu$有基$\beta$。
令 $K$ 为 $X$ 的 $\beta$ 可忽略不计的紧致子集。那么对于每个$s \in G$，$K$ 就是$\gamma(s)|\nu|$，可以忽略不计。现在，
$$
|\mu| * |\nu| = \int_G (\varepsilon_s * |\nu|) d|\mu|(s)
$$
（§1, No. 5，命题 7），而映射 $s \mapsto \varepsilon_s * |\nu|$ 是模糊连续的（§2，命题 6）。因此 $K$ 是 $|\mu| * |\nu|$-可以忽略不计。 V, §3, No. 3，周四。 1. 因此 $|\mu| * |\nu|$ 有基 $\beta$（第 V, §5, No. 5，第 2 章）。

### 3. 卷积和线性表示

#### 命题 11 {#int-viii-s3-prop-11 .statement tag=09JM}

— 令$G$为局部紧致群，$E$为准完全局部凸空间，$U$为$G$在$E$中的连续表示。
(i) 如果$\lambda \in \mathscr{C}'(G)$，$\mu \in \mathscr{C}'(G)$，则$U(\lambda * \mu) = U(\lambda)U(\mu)$。
(ii) 假设$E$是Banach空间，并让$\rho(s) = \|U(s)\|$代表$s \in G$。如果$\lambda \in \mathscr{M}^\rho(G)$，$\mu \in \mathscr{M}^\rho(G)$，则$U(\lambda * \mu) = U(\lambda)U(\mu)$。
让$\lambda, \mu$在$\mathscr{C}'(G)$中。对于任何 $x \in E$ 的人来说，应用尤其是 Props。第 1 章和第 4 章VI, §1, No. 1,
$$
U(\lambda * \mu)x = \int_G U(s)x\, d(\lambda * \mu)(s)
$$
$$
= \int_{G \times G} U(st)x\, d\lambda(s)\, d\mu(t) = \int_{G \times G} U(s)U(t)x\, d\lambda(s)\, d\mu(t)
$$
$$
= \int_G U(\lambda)U(t)x\, d\mu(t) = U(\lambda) \int_G U(t)x\, d\mu(t) = U(\lambda)U(\mu)x ,
$$
从而（一）。类似的论证可以应用于情况(ii)。

由于 G 仍然是局部紧致群，我们假设 G 在局部紧致空间 X 中连续在左侧运算。这个定义（§2, No. 4）是G在$\mathscr{M}(X)$中的连续线性表示$\gamma$（配备$\mathscr{H}(X)$中紧致收敛的拓扑）。

#### 命题 12 {#int-viii-s3-prop-12 .statement tag=09JN}

*如果$\lambda \in \mathscr{C}'(G)$和$\mu \in \mathscr{M}(X)$，那么*

$$
\gamma(\lambda)\mu = \lambda * \mu.
$$

根据§1, No. 5第7号提案，

$$
\lambda * \mu = \int_G (\varepsilon_s * \mu) d\lambda(s).
$$

现在，$\varepsilon_s * \mu = \gamma(s)\mu$（No. 2，公式（5））和

$$
\int_G (\gamma(s)\mu) d\lambda(s) = \gamma(\lambda)\mu
$$

定义共 $\gamma(\lambda)$。

#### 推论{#int-viii-s3-n3-cor-1 .statement tag=09JO}

* $\mathscr{C}'(G) \times \mathscr{M}(X)$到$\mathscr{M}(X)$的映射$(\lambda, \mu) \mapsto \lambda * \mu$相对于$\mathscr{C}'(G)$的等连续子集和$\mathscr{M}(X)$的紧致子集是次连续的（$\mathscr{C}'(G)$和$\mathscr{M}(X)$配备紧致收敛的拓扑）分别为$\mathscr{C}(G)$和$\mathscr{H}(X)$）。*

因为，$\mathscr{M}(X)$配备了$\mathscr{H}(X)$的紧收敛拓扑，是准完备的。因此，$\mathscr{C}'(G) \times \mathscr{M}(X)$到$\mathscr{M}(X)$的映射$(\lambda, \mu) \mapsto \gamma(\lambda)\mu$相对于$\mathscr{C}'(G)$的等连续子集和$\mathscr{M}(X)$(§2, No. 6)的紧致子集是低连续的。那么应用提案 12 就足够了。

#### 注 {#int-viii-s3-n3-rem-1 .statement tag=09JP}

— 1) 设 $\lambda_0 \in \mathscr{C}'(G)$。 $\mathscr{M}(X)$到$\mathscr{M}(X)$的映射$\mu \mapsto \lambda_0 * \mu$隐约是连续的。设 $f \in \mathscr{H}(X)$。一个有

$$
\langle \lambda_0 * \mu, f \rangle = \int f(sx) d\lambda_0(s) d\mu(x) = \langle \mu, g \rangle,
$$

其中$g(x) = \int f(sx) d\lambda_0(s)$。现在，$g$ 是连续的（第 VII, §1, No. 1、引理 1）。另一方面，令 S 为$\lambda_0$ 的支持度，K 为$f$ 的支持度。 条件 $sx \in K$ 和 $s \in S$ 意味着 $x \in S^{-1}K$；因此$g$的支持度包含在$S^{-1}K$中，因此$g \in \mathscr{H}(X)$。那么$\langle \lambda_0 * \mu, f \rangle = \langle \mu, g \rangle$就是$\mu$的模糊连续的函数，这就证明了我们的断言。

2）令$\mu_0 \in \mathscr{M}(X)$。对于拓扑$\sigma(\mathscr{C}'(G), \mathscr{C}(G))$和$\sigma(\mathscr{M}(X), \mathscr{H}(X))$，$\mathscr{C}'(G)$到$\mathscr{M}(X)$的映射$\lambda \mapsto \lambda * \mu_0$是连续的。设 $f \in \mathscr{K}(X)$。 设定$h(s) = \int f(sx)\, d\mu_0(x)$，我们有$\langle f, \lambda * \mu_0 \rangle = \langle h, \lambda \rangle$和$h \in \mathscr{C}(G)$（第VII, §1, No. 1，引理1）。

#### 命题 13 {#int-viii-s3-prop-13 .statement tag=09JQ}

*映射* $(s, \mu) \mapsto \gamma(s)\mu$ *of* $G \times \mathscr{M}_+(X)$ *进入* $\mathscr{M}_+(X)$ *当集合* $\mathscr{M}_+(X)$ *右* $X$ *的积极措施配备了模糊拓扑*时，它是连续的。

从$\gamma(s)\mu = \gamma(ss_0^{-1})\gamma(s_0)\mu$开始，由*注1*得出，只需证明映射在形式$(e, \mu_0)$的点与$\mu_0 \in \mathscr{M}_+(X)$的连续性即可。给定函数$f \in \mathscr{K}(X)$和数$\varepsilon > 0$，因此需要证明G中存在e的邻域U和$\mathscr{M}_+(X)$中的$\mu_0$的邻域W，使得关系$s \in U, \mu \in W$意味着

$$
\left| \int f(sx)\, d\mu(x) - \int f(x)\, d\mu_0(x) \right| \leq \varepsilon .
$$

令V为$f$在X中的支持度K的紧邻域，并令$\varphi \in \mathscr{K}_+(X)$使得V上的$\varphi(x) = 1$；在$\mathscr{M}_+(X)$中存在$\mu_0$的邻域$W_0$，使得$a = \sup_{\mu \in W_0} \mu(V)$是有限的：只需取$\mu \in \mathscr{M}_+(X)$的$W_0$集合使得$|\langle \varphi, \mu - \mu_0 \rangle| \leq 1$即可。由于映射 $(s, x) \mapsto sx$ 是连续的，因此另一方面，G 中的 e 存在紧邻$U_0$，使得对于所有 $s \in U_0$ 都有 $sK \subset V$；那么函数$(s, x) \mapsto f(sx)$在$U_0 \times V$中均匀连续，因此存在e的邻域$U \subset U_0$，使得$|f(sx) - f(x)| \leq \varepsilon / 2a$对于所有$s \in U$和$x \in V$。对于 $s \in U$ 和 $\mu \in W_0$，因此我们有

$$
\left| \int f(sx)\, d\mu(x) - \int f(x)\, d\mu(x) \right| \leq \varepsilon / 2 ;
$$

如果$W \subset W_0$是$\mu_0$在$\mathscr{M}_+(X)$中由$\mu \in W_0$测度形成的邻域，使得$\left| \int f(x)\, d\mu(x) - \int f(x)\, d\mu_0(x) \right| \leq \varepsilon / 2$、U和W满足要求。

### 习题 {#int-viii-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
