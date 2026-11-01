---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 13
section_title: Classical splittable simple Lie algebras
lang: zh
source: lie-vii-ix
book_pages: 189-218, 266-271
pdf_pages: 0197-0226, 0274-0279
extraction: native+ocr
subsections:
    - "no": 1
      title: ALGEBRAS OF TYPE A$_{\boldsymbol{l}}$ ($\boldsymbol{l}\geq$ 1)
      page: 190
      pdf_page: 198
    - "no": 2
      title: ALGEBRAS OF TYPE B$_{\boldsymbol{l}}$ ($\boldsymbol{l}\geq$ 1)
      page: 195
      pdf_page: 203
    - "no": 3
      title: ALGEBRAS OF TYPE C$_{\boldsymbol{l}}$ ($\boldsymbol{l}\geq$ 1)
      page: 204
      pdf_page: 212
    - "no": 4
      title: ALGEBRAS OF TYPE $\boldsymbol{D}_{\boldsymbol{l}}$ ($\boldsymbol{l}\geq$ 2)
      page: 211
      pdf_page: 219
statements: 2
exercises: 19
content_sha256: 032b8fc8e96b7b40e3a478caf92d58b44bcee63818de08f4a0dab12500a7846d
translated_from: content/en/lie/VIII/13_s13_classical_splittable_simple_lie_algebras.md
translation_method: google
source_content_sha256: 6374fb400438df5a36d2c913925fb0624256c5324de93a908a0b9247182f92f3
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 06bf765732566174a864f656789cb11da426e9ff005b7f29d63e711318c54366
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 13。经典可拆分简单李代数

在本段中，我们明确地描述了对于经典可分割简单李代数的每个型：

这个型、它的维数和它的分裂嘉当的(I)代数

子代数；

(II) 它的同根；

(III) 博雷尔子代数及其抛物线子代数；

(IV) 其基本简单表示；

(V) 其基本简单表示的那些是

正交或辛；

(VI) 代数不变量多项式函数；

(VII)群Aut$\mathfrak{g}$、Aut$_0\mathfrak{g}$、Aut$_e\mathfrak{g}$的某些性质；

(VIII)限制杀戮形式至嘉当子代数；

(IX) 谢瓦利阶。

### 1. 代数型 A$_{\boldsymbol{l}}$ ($\boldsymbol{l}\geq$ 1)

(I) 令$k$上的V为维数$l+ 1$向量空间，并令$\mathfrak{g}$为踪迹的V自同态代数$\mathfrak{s}\mathfrak{l}(V)$ 零。令$(e_i)_{1\leq i\leq l+1}$为V中的基；与$\mathfrak{g}$的元素相关联的映射关于该基的矩阵是$\mathfrak{g}$与踪迹零的矩阵的代数$\mathfrak{s}\mathfrak{l}(l+ 1, k)$的标识。我们知道$\mathfrak{g}$是半单（第I, §6, no. 7章，第8条命题）。

回想一下（代数，II, §10, no. 3章），$E_{ij}$表示矩阵$(\alpha_{mp})$，这样$\alpha_{ij}= 1$和$\alpha_{mp}= 0$代表$(m, p)\not= (i, j)$。 矩阵

$$
E_{ij}(1\leq i, j\leq l+ 1, i\not=j)
$$

$$
E_{i,i}-E_{i+1,i+1}(1\leq i\leq l)
$$

形式基共$\mathfrak{g}$。因此

dim$\mathfrak{g}=l(l+ 2)$.

令$\widehat{\mathfrak{h}}$为$\mathfrak{g}\mathfrak{l}(l+ 1, k)$的对角线元素的集合； 序列$(E_{ii})_{1\leq i\leq l+1}$是向量空间$\widehat{\mathfrak{h}}$中的基；设$(\widehat{\varepsilon}_i)_{1\leq i\leq l+1}$是$\widehat{\mathfrak{h}}^*$对$(E_{ii})_{1\leq i\leq l+1}$的基。对于所有$h\in \widehat{\mathfrak{h}}$，

$$
[h, E_{ij}] = (\widehat{\varepsilon}_i(h)-\widehat{\varepsilon}_j(h))E_{ij} \tag{1}
$$

由章。 I, §1, no. 2，公式 (5)。 令$\mathfrak{h}$为迹线零的$\widehat{\mathfrak{h}}$元素集合，并放入$\varepsilon_i= \widehat{\varepsilon}_i|\mathfrak{h}$。 那么$\mathfrak{h}$就是$\mathfrak{g}$的嘉当子代数（第VII, §2, no. 1，例4章）。 关系(1)证明这个嘉当子代数是分裂，$(\mathfrak{g},\mathfrak{h})$的根是$\varepsilon_i-\varepsilon_j(i\not=j)$。 设$\widehat{\mathfrak{h}}^*_0$为$\widehat{\mathfrak{h}}^*$和的元素的集合，其相对于$(\widehat{\varepsilon}_i)$的坐标为零。 从$\widehat{\mathfrak{h}}^*_0$到$\mathfrak{h}^*$的映射$\lambda  \rightarrow \lambda |\mathfrak{h}$是双射的。 因而，$(\mathfrak{g},\mathfrak{h})$的根系R是型$A_l$（第VI, §4, no. 7章）。 因而，$\mathfrak{g}$ 很简单（§3, no. 2，第 6 条命题的 Cor.1）。 因而，$\mathfrak{g}$是型$A_l$的可分割简单李代数。

在基本自同构下，$\mathfrak{g}$ 的每个分裂嘉当子代数 $\mathfrak{h}'$ 都是 $\mathfrak{h}$ 的变换（§3, no. 3，Prop. 10 的 Cor.）。 由于Aut$_e\mathfrak{g}$是$\mathfrak{g}$的自同构$x \rightarrow sxs^{-1}$和$s\in \mathbf{S}\mathbf{L}(V)$的集合（第VII, §3, no. 1，注2；cf.也（VII）），因此存在基 V的$\beta$使得$\mathfrak{h}'$是$\mathfrak{g}$的元素的集合$\mathfrak{h}_{\beta}$，其中矩阵相对于基$\beta$是对角线。 由于$\mathfrak{h}_{\beta}$包含元素与不同的特征值，V的唯一向量子空间在$\mathfrak{h}_{\beta}$的元素下稳定是由$\beta$的子集生成的。 由此可见，映射$\beta  \rightarrow \mathfrak{h}_{\beta}$诱导由V的分解的集合代入维数的$l+ 1$子空间的直和商双射得集合分裂嘉当子代数 $\mathfrak{g}$。 (II) 设$\alpha =\varepsilon_i-\varepsilon_j(i\not=j)$为根。 我们有$\mathfrak{g}^{\alpha}=kE_{ij}$。 自从

$$
[E_{ij}, E_{ji}] =E_{ii}-E_{jj}
$$

从 $\alpha (E_{ii}-E_{jj}) = 2$ 开始，我们有 (§2, no. 2, Th. 1 (ii))

$$
H_{\alpha}=E_{ii}-E_{jj}
$$

(III) 放入$\alpha_1=\varepsilon_1-\varepsilon_2, \alpha_2=\varepsilon_2-\varepsilon_3, . . . , \alpha_l=\varepsilon_l-\varepsilon_{l+1}$。由章。 VI, §4，没有。 $7.I, (\alpha_1, . . . , \alpha_l)$是R的基B；相对于 B 的正根是 $i < j$ 的 $\varepsilon_i-\varepsilon_j$。 相应的博雷尔子代数$\mathfrak{b}$是轨迹零的上三角矩阵的集合。

V中的标志是向量子空间V的集合，与$\{0\}$和V不同，完全按包含排序。 V 的标志包含阶集合。最大标志为集合 $\{W_1, . . . ,W_l\}$，其中 $W_i$ 是 $i$ 维向量子空间且

$$
W_1\subset  \cdots  \subset W_l
$$

对于例，如果$V_i$表示$e_1, . . . , e_i$生成的V的子空间，则$\{V_1, . . . ,V_l\}$是最大标志。

It is immediate that $\mathfrak{b}$ is the set of elements of $\mathfrak{g}$ leaving stable the elements of the maximal flag $\{V_1, . . . ,V_l\}$. 相反，由于$\mathfrak{b}$包含$\mathfrak{h}$和矩阵$E_{ij}$对于$i < j$，我们看到$V_i$是$\mathfrak{b}$下唯一稳定的非平凡向量子空间。

现在让 $\delta$ 成为 V 中的最大标志。由上可知，$\mathfrak{g}$的元素的集合$\mathfrak{b}_{\delta}$保持稳定，$\delta$的所有元素是$\mathfrak{g}$的博雷尔子代数。由于$\mathfrak{g}$的每个博雷尔子代数是基本自同构下$\mathfrak{b}$的变换，我们看到映射$\delta  \rightarrow \mathfrak{b}_{\delta}$是从最大标志的集合到博雷尔子代数的集合的双射 $\mathfrak{g}$。

令 $\beta$ 为 V 中的基。根据 (I) 和前面的内容，博雷尔子代数包含 $\mathfrak{h}_{\beta}$ 是相应的到最大标志，其中每个元素是由$\beta$ 的子集生成的。这些标志对应通过以下方式双射到$\beta$上的总阶：$\beta$上的总阶$\omega$与标志$\{W_1, . . . ,W_l\}$相关联，其中$W_i$是由第一个生成的向量子空间 $i$ 元素共 $\beta$ 阶 $\omega$。因为有 $(l+$ 1)！ $\beta$上总共阶，我们恢复了存在$(l+$的事实1)！ $(\mathfrak{s}\mathfrak{l}(V),\mathfrak{h}_{\beta}) ($§3, no. 3、注中的博雷尔子代数）。

设$\gamma$为V中的一面旗帜。由于$\gamma$包含在最大标志中，因而$\mathfrak{g}$的元素的集合$\mathfrak{p}_{\gamma}$离开稳定的$\gamma$的元素是$\mathfrak{g}$的抛物线子代数。我们证明，在 $\mathfrak{p}_{\gamma}$ 下唯一稳定的非平凡向量子空间是 $\gamma$ 的元素。为此，我们可以假设 $\gamma =\{V_{i_1}, . . . ,V_{i_q}\}$ 和 $1\leq i_1<\cdots < i_q\leq l$。把$i_0= 0, i_{q+1}=l+ 1$。非空区间

$$
i_0+ 1, i_1, i_1+ 1, i_2, . . . , i_q+ 1, i_{q+1}
$$

$\{1, . . . , l+ 1\}$的形式划分，因此阶$l+ 1$的任何平方矩阵都可以写成块矩阵$(X_{ab})_{1\leq a,b\leq q+1}$。 代数$\mathfrak{p}_{\gamma}$则为$\mathfrak{s}\mathfrak{l}(l+ 1, k)$的元素$(X_{ab})_{1\leq a,b\leq q+1}$之集合$\mathfrak{p}_{i_1,...,i_q}$，使得$X_{ab}= 0$为$a > b$。由于$\mathfrak{p}_{i_1,...,i_q}\supset \mathfrak{b}$，在$\mathfrak{p}_{i_1,...,i_q}$下稳定的非平凡向量子空间是$V_i$之一；如果$i_k< i < i_{k+1}$，代数$\mathfrak{p}_{i_1,...,i_q}$包含于$E_{i_{k+1},i}$和$V_i$不稳定，因此我们的断言。

因而，最大标志$\{V_1, . . . ,V_l\}$中包含的$2^l$标志产生$2^l$不同的抛物线子代数包含$\mathfrak{b}$；因为正好有 $2^l$ 抛物线子代数包含 $\mathfrak{b}($§3, no. 4, 注)，因此映射 $\gamma  \rightarrow \mathfrak{p}_{\gamma}$ 是双射来自集合的标志$\mathfrak{g}$ 的抛物线子代数的V 至集合。此外，$\mathfrak{p}_{\gamma}\supset \mathfrak{p}_{\gamma'}$当且仅当$\gamma \subset \gamma '$。

回想一下抛物线子代数 $\mathfrak{p}=\mathfrak{p}_{i_1,...,i_q}(1\leq i_1<\cdots < i_q\leq l)$。令$\mathfrak{s}$（或$\mathfrak{n}$）为$\mathfrak{s}\mathfrak{l}(l+ 1, k)$中$(X_{ab})_{1\leq a,b\leq q+1}$的集合，使得$X_{ab}= 0$对应于$a\not=b$（或$a\geq b$）。根据§3, no. 4的第13条命题，我们有$\mathfrak{p}=\mathfrak{s}\oplus \mathfrak{n}$，子代数，$\mathfrak{s}$在$\mathfrak{g}$中被还原，而$\mathfrak{n}$既是最大的幂零理想又是$\mathfrak{p}$的幂零根。

(IV) 对于$r= 1,2, . . . , l$，设$\varpi_r=\varepsilon_1+\cdots +\varepsilon_r$。我们有$\varpi_i(H_{\alpha_j}) =\delta_{ij}$，所以$\varpi_r$是基本的权相应的到$\alpha_r$。

令$\sigma$为$\mathfrak{g}$在V上的恒等式表示。 $\sigma$的外部幂$\bigwedge^r\sigma$是$E =\bigwedge^r(V)$上的表示。让$(e_1, . . . , e_{l+1})$成为V中选择的基。 $e_{i_1}\wedge  \cdots  \wedge e_{i_r}$，其中 E 的 $i_1<\cdots < i_r$、形式基。如果 $h\in \mathfrak{h}$，

$$
(\bigwedge^r\sigma )(h).e_{i_1}\wedge  \cdots  \wedge e_{i_r}= (\varepsilon_{i_1}+\cdots +\varepsilon_{i_r})(h)e_{i_1}\wedge  \cdots  \wedge e_{i_r}
$$

因而，每个权都是重数，$1,\varpi_r$是$\bigwedge^r\sigma$的权，并且每个其他权都是形式$\varpi_r-\mu$，其中$\mu$是正部首权。因而，$\varpi_r$是$\bigwedge^r\sigma$的最高权，而$e_1\wedge \cdots \wedge e_r$是原语元素。由章。 VI, §4, no. 7.IX，Weyl 群可以与对称群识别

$$
\{\varepsilon_1, . . . , \varepsilon_{l+1}\}
$$

Weyl 群下的 $\varpi_r$ 的轨道因此包含所有 $\varepsilon_{i_1}+\cdots +\varepsilon_{i_r}$ 和 $i_1<\cdots < i_r$。由原语元素$e_1\wedge  \cdots  \wedge e_r$生成的简单子模因此承认所有$\varepsilon_{i_1}+\cdots +\varepsilon_{i_r}$为权，因此等于E。因而，$\bigwedge^r\sigma$与最高权$\varpi_r$不可约。

因而，表示$\bigwedge^r\sigma (1\leq r\leq l)$是基本的表示。我们有暗淡（$\bigwedge^r\sigma$）$=(^{l+1}_r)$。

(V) 我们有$w_0(\alpha_1) =-\alpha_l, w_0(\alpha_2) =-\alpha_{l-1}, . .$。 （第VI, §4, no. 7，XI），所以

$$
-w_0(\varpi_1) =\varpi_l,-w_0(\varpi_2) =\varpi_{l-1}, . . .
$$

让

$$
\omega =n_1\varpi_1+\cdots +n_l\varpi_l(n_1, . . . , n_l\in \mathbf{N})
$$

成为主导权。那么，简单的表示与最高权 $\omega$ 正交或辛当且仅当

$$
n_1=n_l,n_2=n_{l-1}, . .
$$

（§7, no. 5，提案 12）。特别是，如果 $l$ 是偶数，则 $\mathfrak{s}\mathfrak{l}(l+ 1, k)$ 的基数表示都不是正交或辛的。如果 $l$ 是奇数，则 $i\not= (l+ 1)/2$ 的表示 $\bigwedge^i\sigma$ 既不正交也不辛；由章。 $\varpi_{(l+1)/2}$相对于$(\alpha_1, . . . , \alpha_l)$的坐标VI, §4, no. 7.VI、和为

$$
\frac{1}{l + 1}[\frac{l + 1}{2}(1 + 2 +\cdots +\frac{l- 1}{2})+\frac{l + 1}{2}(1 + 2 +\cdots +\frac{l + 1}{2})]
$$

$$
= 1 + 2 +\cdots +\frac{l- 1}{2}+\frac{l + 1}{4}
$$

so $\bigwedge^{(l+1)/2}\sigma$ is orthogonal if $l\equiv  -1$ (mod. 4) and symplectic if $l\equiv 1$ (mod. 4) (§7, no. 5, Prop. 12). 最后的结果可以如下变得更加精确。 选择 $\bigwedge^{l+1}(V)$ 中的非零元素 $e$。 乘法在外部代数 V 定义双线性映射

$$
\bigwedge^{(l+1)/2}(V)\times \bigwedge^{(l+1)/2}(V)
$$

到$\bigwedge^{l+1}$(V)，可以写成$(u, v) \rightarrow \Phi (u, v)e$，其中$\Phi$是$\bigwedge^{(l+1)/2}(V)$上的双线性形式。立即验证$\Phi$非零，在$\mathfrak{g}$下不变（因此非简并），如果$(l+ 1)/2$是偶数则对称，如果$(l+ 1)/2$是奇数则交错的。

(VI) 对于所有$x\in \mathfrak{g}$，$\sigma (x) =x$的特征多项式可以写成

$$
T^{l+1}+f_2(x)T^{l-1}+f_3(x)T^{l-2}+\cdots +f_{l+1}(x)
$$

其中$f_2, . . . , f_{l+1}$在$\mathfrak{g}($§8, no. 3、引理2)下是多项式函数不变的。

如果$x=\xi_1E_{11}+\cdots +\xi_{l+1}E_{l+1l+1}\in \mathfrak{h}$，则$f_i(x)$直到符号为止都是次数$2, . . . , l+ 1$的$\xi_1, . . . , \xi_{l+1}$的初等对称函数。因此，由章。 VI, §4, no. 7.IX，$\mathbf{S}(\mathfrak{h}^*)$的元素的$f_i|\mathfrak{h}$生成代数在Weyl群下不变量，并且是代数独立的。因此，多项式函数的(§8, no. 3，命题$3$)$f_2, f_3, . . . , f_{l+1}$生成代数在$\mathfrak{g}$下是不变的，并且是代数独立的。

(VII) 对于所有$g\in \mathbf{G}\mathbf{L}(l+ 1, k)$，令$\varphi_k(g) =\varphi (g)$为自同构$x \rightarrow gxg^{-1}$ / $\mathfrak{g}$。那么从$\mathbf{G}\mathbf{L}(l+ 1, k)$到Aut($\mathfrak{g}$)，$\varphi$就是同态。我们有

$\varphi (\mathbf{S}\mathbf{L}(l+ 1, k)) =$ 自动$_e(\mathfrak{g})$

（第VII, §3, no. 1、注2章）。设$\overline{k}$为$k$的代数闭包。我们有

$$
\mathbf{G}\mathbf{L}(l+ 1,\overline{k}) = \overline{k}^*.\mathbf{S}\mathbf{L}(l+ 1,\overline{k})
$$

所以$\varphi_{\overline{k}}(\mathbf{G}\mathbf{L}(l+ 1,\overline{k})) =\varphi_{\overline{k}}(\mathbf{S}\mathbf{L}(l+ 1,\overline{k})) =$自动$_e(\mathfrak{g}\otimes_k\overline{k})$；由此可见 $\varphi (\mathbf{G}\mathbf{L}(l+ 1, k))\subset$ Aut$_0(\mathfrak{g})$。另一方面，根据§7, no. 1的第2号命题，Aut$_0(\mathfrak{g})\subset \varphi (\mathbf{G}\mathbf{L}(l+ 1, k))$适用于$\mathfrak{g}$的恒等式表示。因此，

自动$_0(\mathfrak{g}) =\varphi (\mathbf{G}\mathbf{L}(l+ 1, k))$。

$\varphi$核是与阶$l+1$每矩阵可交换的$\mathbf{G}\mathbf{L}(l+ 1, k)$元素集合，即可逆标量矩阵的集合$k^*$。因此，Aut$_0(\mathfrak{g})$可以与群$\mathbf{G}\mathbf{L}(l+ 1, k)/k^*=\mathbf{P}\mathbf{G}\mathbf{L}(l+ 1, k)$识别。 $\varphi '=\varphi |\mathbf{S}\mathbf{L}(l+ 1, k)$的核是$\mu_{l+1}(k)$，其中$\mu_{l+1}(k)$表示$k$中单位元的$(l+$1)第根中的集合。因此，Aut$_e(\mathfrak{g})$可以被识别为群$\mathbf{S}\mathbf{L}(l+ 1, k)/\mu_{l+1}(k) =\mathbf{P}\mathbf{S}\mathbf{L}(l+ 1, k)$。另一方面，我们有正合序列

1 $\longrightarrow \mathbf{S}\mathbf{L}(l+ 1, k)\longrightarrow \mathbf{G}\mathbf{L}(l+ 1, k)\longrightarrow^{det}k^*\longrightarrow$ 1

det下的$k^*$的像是$k^{*l+1}$。由此可见，有典范同构

自动$_0(\mathfrak{g})/$自动$_e(\mathfrak{g})\longrightarrow \mathbf{P}\mathbf{G}\mathbf{L}(l+ 1, k)/\mathbf{P}\mathbf{S}\mathbf{L}(l+ 1, k)$

$$
\longrightarrow \mathbf{G}\mathbf{L}(l+ 1, k)/k^*.\mathbf{S}\mathbf{L}(l+ 1, k)\longrightarrow k^*/k^{*l+1}
$$

如果 $k$ = $\mathbf{R}$，如果 $l+ 1$ 是奇数，我们可以看到 Aut$_0(\mathfrak{g}) =$ Aut$_e(\mathfrak{g})$；如果 $l+ 1$ 是偶数，则 Aut$_0(\mathfrak{g})/$Aut$_e(\mathfrak{g})$ 同构于 $\mathbf{Z}/2\mathbf{Z}$。

与$5,f(T_{\mathbf{Q}})$的记号是$\mathfrak{g}$的自同构集合即诱导在$\mathfrak{h}$上的恒等式，因此等于$\varphi$(D)，其中D是对角线元素的集合 $\mathbf{G}\mathbf{L}(l+ 1, k) ($§5，提案 4）。令$D'$为$\mathbf{S}\mathbf{L}(l+ 1, k)$的对角线元素的集合。根据§5的第3条命题，以及Aut$_e(\mathfrak{g})$的确定，我们有$f(q(T_P))\subset \varphi (D')$。我们证明$f(q(T_P)) =\varphi (D')$。让

$\lambda_1$ 0

$d=$。 ..

0 $\lambda_{l+1}$

是元素 / $D'$。对于所有 $i$ 和 $j$，存在 $\zeta \in$ Hom(Q(R)$, k^*$) $= T_Q$，使得$\zeta (\varepsilon_i-\varepsilon_j) =\lambda_i\lambda^{-1}_j$。很容易验证$f(\zeta ) =\varphi (d)$。由章。 VI, §4, no. 7.VIII，P(R)由Q(R)和元素$\varepsilon =\varepsilon_1$生成，其$P(R)/Q(R)$中的像为阶$l+ 1$；但是

$$
\zeta ((l+ 1)\varepsilon ) =\zeta ((\varepsilon_1-\varepsilon_2) + (\varepsilon_1-\varepsilon_3) +\cdots + (\varepsilon_1-\varepsilon_{l+1}))
$$

$$
=\lambda^l_1\lambda^{-1}_2\lambda^{-1}_3. . . \lambda^{-1}_{l+1}=\lambda^{l+1}_1
$$

所以从 P(R) 到 $k^*$ $\zeta$ 扩展到同态。这就证明了$\zeta \in q(T_P)$，所以$\varphi (d)\in f(q(T_P))$。

回想一下（§5, no. 3，第 5 条命题第 2 条），对于 $l= 1$，Aut($\mathfrak{g}$) $=$ Aut$_0(\mathfrak{g})$，对于 $l\geq 2$，Aut($\mathfrak{g}$)$/$Aut$_0(\mathfrak{g})$ 同构于 $\mathbf{Z}/2\mathbf{Z}$。如果$l\geq 2$（第VI, §4, no. 7.XI），则映射$\theta :x \rightarrow  -^tx$是$\mathfrak{s}\mathfrak{l}(l+ 1, k)$和$a_0=\theta |\mathfrak{h}\notin W$的自同构，所以$a_0$的类 Aut($\mathfrak{g}$)$/$Aut$_0(\mathfrak{g})$ 是这个群的非平凡元素（§5, no. 2，命题 4）。

杀戮形式的(VIII)限制到$\mathfrak{h}$是

$$
\Phi (\xi_1E_{11}+\cdots +\xi_{l+1}E_{l+1,l+1}, \xi '_1E_{11}+\cdots +\xi '_{l+1}E_{l+1,l+1})
$$

$$
=\sum_{i\not=j}(\xi_i-\xi_j)(\xi '_i-\xi '_j) =\sum_{i,j}(\xi_i-\xi_j)(\xi '_i-\xi '_j)
$$

$$
= (l+ 1)\sum_i\xi_i\xi '_i+ (l+ 1)\sum_j\xi_j\xi '_j-2(\sum_i\xi_i)(\sum_j\xi '_j
$$

$$
= 2(l+ 1)\sum_i\xi_i\xi '_i
$$

(IX) 对于 $1\leq i < j\leq l+ 1$，输入

$$
X_{\varepsilon_i-\varepsilon_j}=E_{ij}X_{\varepsilon_j-\varepsilon_i}=-E_{ji}
$$

然后，对于所有$\alpha \in R$，我们有$[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$和$\theta (X_{\alpha}) =X_{-\alpha}$（其中$\theta$是（VII）中引入的自同构$x \rightarrow  -^tx$）。因而，$(X_{\alpha})_{\alpha\in R}$ 是 $(\mathfrak{g},\mathfrak{h})$ 中的 Chevalley 系统。

取$k=\mathbf{Q}$。 $\mathfrak{h}($§12, no. 6，Def. 中允许的格子。 1) 是位于 $E_{ii}-E_{i+1,i+1}$ 生成的 $\mathbf{Z}$-模 $Q(R^{\vee})$ 之间，即矩阵属于到 $\mathfrak{s}\mathfrak{l}(l+ 1,\mathbf{Z})$ 对角线的由……组成和由 $\mathbf{Z}$-模 $P(R^{\vee})$ 生成的$Q(R^{\vee})$和$E_{11}-(l+ 1)^{-1}\sum E_{ii}$（第VI, §4, no. 7.VIII），即形式$x+ (l+ 1)^{-1}a.1$的轨迹零的对角线矩阵的由……组成，其中$x$有整数条目和$a\in \mathbf{Z}$。由此可见，$\mathfrak{s}\mathfrak{l}(l+1,\mathbf{Z})$ 是 $(\mathfrak{g},\mathfrak{h})$ 中的 Chevalley 阶，与许用格子 $Q(R^{\vee})$ 和 Chevalley 系统 $(X_{\alpha})$ 相关。很容易验证$\bigwedge^r\mathbf{Z}^{l+1}$是$\bigwedge^r\mathbf{Q}^{l+1}$相对于$\mathfrak{s}\mathfrak{l}(l+ 1,\mathbf{Z}) ($§12, no. 8的容许格，Def。 3）。

另一方面，$\mathfrak{g}\mathfrak{l}(l+ 1,\mathbf{Z})$ 是分裂的还原代数 $\mathfrak{g}\mathfrak{l}(l+ 1,\mathbf{Q})$ 中的 Chevalley 阶；它的投影到$\mathfrak{s}\mathfrak{l}(l+ 1,\mathbf{Q})$平行于$\mathfrak{g}\mathfrak{l}(l+1,\mathbf{Q})$的中心$\mathbf{Q}.1$是$(\mathfrak{g},\mathfrak{h})$中的Chevalley阶由$\mathfrak{h}$中的允许晶格$P(R^{\vee})$和Chevalley系统$(X_{\alpha})$定义。我们注认为$\mathfrak{g}\mathfrak{l}(l+ 1,\mathbf{Z})$不是其交的直和与$\mathfrak{s}\mathfrak{l}(l+ 1,\mathbf{Q})$和中心的$\mathfrak{g}\mathfrak{l}(l+ 1,\mathbf{Q})$。

### 2. 代数型 B$_{\boldsymbol{l}}$ ($\boldsymbol{l}\geq$ 1)

(I) 令V为有限维向量空间，而$\Psi$为V上的非简并对称双线性形式。 集合 / 自同态 $x$ / V，使得$\Psi (xv, v') +\Psi (v, xv') = 0$对于所有$v, v'\in V$来说是$\mathfrak{s}\mathfrak{l}$(V)的谎言子代数，半单对于昏暗的$V\not= 2$ （第 I, §6, no. 7 章，第 9 条命题）。我们用 $\mathfrak{o}(\Psi )$ 表示它，并将其称为与 $\Psi$ 关联的正交李代数。

假设V是奇数维数$2l+ 1\geq 3$，$\Psi$是最大指标$l$。用 Q 表示二次形式，使得 $\Psi$ 与 Q 相关联。对于 $x\in V$，我们有 $Q(x) =\frac{1}{2}\Psi (x, x)$。 代数，第 1 章IX, §4, no. 2、V可以写成两个最大全各向同性子空间 F和$F'$的直和以及$F + F'$的正交补G，它是非各向同性的一维。在$\Psi$乘以一个非零常数之前，我们可以假设存在$e_0\in G$使得$\Psi (e_0, e_0) =-2$。另一方面，F 和 $F'$ 通过 $\Psi$ 具有对偶性；设 $(e_i)_{1\leq i\leq l}$ 为 F 的基，且 $(e_{-i})_{1\leq i\leq l}$ 对偶基为 $F'$。然后

$$
(e_1, . . . , e_l, e_0, e_{-l}, . . . , e_{-1})
$$

是 V 中的基；我们有

$$
Q(\sum x_ie_i)=-x^2_0+\sum_{i=1}^{i=l}x_ix_{-i}
$$

相对于该基，$\Psi$矩阵为阶$2l+ 1$平方矩阵

0 0 $\cdots$ 0 1

0 0 $s$ 0 0 $\cdots$ 1 0

$S=$0$-2$0$,s=$……。 .. ... ...,

$s$ 0 0 0 1 $\cdots$ 0 0

1 0 $\cdots$ 0 0

其中$s$是阶$l$的平方矩阵，其所有条目都是零，除了第二个对角线$^6$上的条目等于1。具有上述属性的V的基将被称为维特基共 V。然后可以将代数$\mathfrak{g}=\mathfrak{o}(\Psi )$与方阵$a$或阶$2l+ 1$的代数$\mathfrak{o}_S(2l+ 1, k)$进行识别，使得$a=-S^{-1}aS($代数，第1章。 IX, §1, no. 10、公式 (50))。简单计算可知，$\mathfrak{g}$ 是集合 / 矩阵 / 形式

$$
A2s^txB
$$

$y$ 0 $x$ (2)

$$
C2s^tyD
$$

其中 $x$ 和 $y$ 是 1 行的矩阵，$l$ 列和 $A, B, C, D$ 是阶 $l$ 的方阵，这样 $B=-s^tBs, C=-s^tCs$ 和 $D=-s^tAs$。由于映射 $A \rightarrow s^tAs$ 从 $\mathbf{M}_l(k)$ 到自身是关于第二条对角线的对称性，因此可以得出

昏暗$\mathfrak{g}= 2l+l^2+ 2\frac{l(l-1)}{2}=l(2l+ 1)$。

令$\mathfrak{h}$为$\mathfrak{g}$的对角线元素的集合。这是 $\mathfrak{g}$ 中的交换子代数，其中基元素

$^6$ 平方矩阵 $(a_{ij})_{1\leq i,j\leq n}$ 的第二条对角线是 $a_{ij}$ 的族，使得

$$
i+j=n+ 1
$$

$$
H_i=E_{i,i}-E_{-i,-i}(1\leq i\leq l)
$$

令$(\varepsilon_i)$为$\mathfrak{h}^*$对$(H_i)$的基。放

$$
X_{\varepsilon_i}= 2E_{i,0}+E_{0,-i}(1\leq i\leq l)
$$

$X_{-\varepsilon_i}$ = $-2E_{-i,0}-E_{0,i}(1\leq i\leq l)$

$X_{\varepsilon_i-\varepsilon_j}$ = $E_{i,j}-E_{-j,-i}(1\leq i < j\leq l)$

$X_{\varepsilon_j-\varepsilon_i}$ = $-E_{j,i}+E_{-i,-j}(1\leq i < j\leq l)$ (3)

$X_{\varepsilon_i+\varepsilon_j}$ = $E_{i,-j}-E_{j,-i}(1\leq i < j\leq l)$

$X_{-\varepsilon_i-\varepsilon_j}$ = $-E_{-j,i}+E_{-i,j}(1\leq i < j\leq l)$。

很容易验证这些元素形式基是$\mathfrak{g}$中$\mathfrak{h}$的补集，并且对于$h\in \mathfrak{h}$，

$$
[h, X_{\alpha}] =\alpha (h)X_{\alpha} \tag{4}
$$

对于所有$\alpha \in R$，其中R是$\pm \varepsilon_i$和$\pm \varepsilon_i\pm \varepsilon_j(1\leq i < j\leq l)$的集合。由此可见，$\mathfrak{h}$ 等于其在 $\mathfrak{g}$ 中的归一化器，因此是 $\mathfrak{g}$ 的嘉当子代数，$\mathfrak{h}$ 是分裂，$(\mathfrak{g},\mathfrak{h})$ 的根是 R 的元素。 根系 R $(\mathfrak{g},\mathfrak{h})$ 的 $l\geq 2$ 为型 $B_l$，$l= 1$ 的型 $A_1$（也称为型 $B_1$）（第 1 章） VI, §4, no. 5.I，扩展到案例$l= 1$）。因而，$\mathfrak{g}$是型$B_l$的可拆分简单李代数。

$\mathfrak{o}(\Psi )$的每个分裂嘉当子代数都是$\mathfrak{h}$的变换乘以$\mathfrak{o}(\Psi )$的基本自同构，因此乘以$\mathbf{O}(\Psi )$的元素(cf.(VII))，因此是$\mathfrak{g}$的元素集合$\mathfrak{h}_{\beta}$，其矩阵相对于V的威特基$\beta$是对角的。我们立即验证$\mathfrak{h}_{\beta}$下唯一的向量子空间不变量是由$\beta$的子集生成的。

如果 $l= 1$、代数 $\mathfrak{o}(\Psi )$ 和 $\mathfrak{s}\mathfrak{l}(2, k)$ 具有相同的根系，因此是同构的（cf. 也是 §1，练习 16）。从现在开始，我们假设$l\geq 2$。

(II) 根系 $R^{\vee}$ 由第 1 章确定。 VI, §4, no. 5.V，我们发现

$$
H_{\varepsilon_i}= 2H_i, H_{\varepsilon_i-\varepsilon_j}=H_i-H_j, H_{\varepsilon_i+\varepsilon_j}=H_i+H_j
$$

(III) 放入$\alpha_1=\varepsilon_1-\varepsilon_2, . . . , \alpha_{l-1}=\varepsilon_{l-1}-\varepsilon_l, \alpha_l=\varepsilon_l$。由章。 VI, §4, no. 5.II，$(\alpha_1, . . . , \alpha_l)$是R的基B；相对于 B 的正根是 $\varepsilon_i$ 和 $\varepsilon_i\pm \varepsilon_j(i < j)$。 相应的博雷尔子代数 $\mathfrak{b}$ 是$\mathfrak{g}$ 中上三角矩阵的集合。

立即验证，V中唯一不同于$\{0\}$和V在$\mathfrak{b}$下稳定的向量子空间是最大标志相应的到基$(e_i)$的元素，即完全各向同性子空间$V_1, . . . ,V_l$，其中$V_i$由$e_1, . . . , e_i$生成，与其正交补集$V_{-1}, . . . ,V_{-i}:$一起，$V_i$的正交补集$V_{-i}$由$e_1, . . . , e_l, e_0, e_{-l}, . . . , e_{-i-1}$生成，并且不完全各向同性。另一方面，如果 $\mathfrak{g}$ 的元素离开稳定的向量子空间，则它的正交补集离开稳定。因而，$\mathfrak{b}$是$\mathfrak{g}$的元素的集合，留下稳定的元素标志$\{V_1, . . . ,V_l\}$。

如果一个标志的每个元素完全各向同性，则该标志被称为各向同性。 标志$\{V_1, . . . ,V_l\}$是最大各向同性标志。 Since the group $\mathbf{O}(\Psi )$ operates transitively both on the Borel subalgebras of $\mathfrak{g}$ (cf. (VII)) and on the maximal isotropic flags (Algebra, Chap. IX, §4, no. 3, Th. 1), we see that, for any maximal isotropic flag $\delta$ in V, the set $\mathfrak{b}_{\delta}$ of elements of $\mathfrak{g}$ leaving stable the elements of $\delta$ is a Borel subalgebra of $\mathfrak{g}$ and that the map $\delta  \rightarrow \mathfrak{b}_{\delta}$ is a bijection from the set of maximal isotropic flags to the set of Borel subalgebras of $\mathfrak{g}$.

令$\delta$为各向同性标志，令$\mathfrak{p}_{\delta}$为$\mathfrak{g}$的元素的集合，留下稳定的$\delta$的元素。如果$\delta \subset  \{V_1, . . . ,V_l\}$，则$\mathfrak{p}_{\delta}$是$\mathfrak{g}$包含$\mathfrak{b}$的抛物线子代数，容易验证在$\mathfrak{p}_{\delta}$下唯一完全各向同性的子空间$\not=\{0\}$稳定的是元素 $\delta$。这给出了 $2^l$ 抛物线子代数的 $\mathfrak{g}$ 包含 $\mathfrak{b}$。由上可知，从V各向同性标志的集合到$\mathfrak{g}$抛物线子代数的集合，映射$\delta  \rightarrow \mathfrak{p}_{\delta}$为双射。此外，$\mathfrak{p}_{\delta}\subset \mathfrak{p}_{\delta'}$当且仅当$\delta \supset \delta '$。

（IV）基本权相应的到$\alpha_1, . . . , \alpha_l$是，由第1章。 VI, §4, no. 5.VI,

$$
\varpi_i=\varepsilon_1+\cdots +\varepsilon_i(1\leq i\leq l-1)
$$

$$
\varpi_l=\frac{1}{2}(\varepsilon_1+\cdots +\varepsilon_l)
$$

令$\sigma$为$\mathfrak{g}$在V上的恒等式表示。外部幂$\bigwedge^r\sigma$在$E =\bigwedge^rV$运行。如果$h\in \mathfrak{h}$，

$\sigma (h).e_i=\varepsilon_i(h)e_i$ $1\leq i\leq l$

$$
\sigma (h).e_0= 0
$$

$\sigma (h).e_{-i}=-\varepsilon_i(h)e_{-i}$ 换$1\leq i\leq l$。

由此可见，对于$1\leq r\leq l,\varepsilon_1+\cdots +\varepsilon_r$是$\bigwedge^r\sigma$的最高权，权$\varepsilon_1+\cdots +\varepsilon_r$的元素是与$e_1\wedge  \cdots  \wedge$$e_r$的比例。我们将证明，对于$1\leq r\leq l-1$，表示$\bigwedge^r\sigma$是最高权$\varpi_r$的$\mathfrak{g}$的基本表示。为此，只要证明 $\bigwedge^r\sigma$ 对于 $0\leq r\leq 2l+ 1$ 是不可约的。但是双线性形式 $\Phi$ 在 $\bigwedge^rV\times \bigwedge^{2l+1-r}V$ 上定义为

$$
x\wedge y=\Phi (x, y)e_1\wedge  \cdots  \wedge e_l\wedge e_0\wedge e_{-l}\wedge  \cdots  \wedge e_{-1}
$$

在$\mathfrak{g}$下是不变的，并且使$\bigwedge^rV$和$\bigwedge^{2l+1-r}V$具有对偶性。因此，表示$\bigwedge^{2l+1-r}\sigma$是$\bigwedge^r\sigma$的对偶，足以证明$\bigwedge^r\sigma$对于$0\leq r\leq l$的不可约性，或者$\bigwedge^rV$包含$e_1\wedge  \cdots  \wedge e_r$的最小的子空间$T_r$而稳定在$\mathfrak{g}$以下的是$\bigwedge^rV$的整体。这是 $r= 0$ 和 $r= 1$ 的直接的 (cf. 公式 (2))。对于$r= 2$（因此$l\geq 2$），表示$\bigwedge^2\sigma$和$\mathfrak{g}$的伴随表示（不可约）具有相同的维数$l(2l+ 1)$和相同的最高权$\varepsilon_1+\varepsilon_2$ （第 VI, §4, no. 5.IV）。我们结论认为$\bigwedge^2\sigma$等价于伴随表示，因此是不可约的。这证明了我们的断言对于$l= 1$和$l= 2$。

我们现在通过归纳对$l$进行论证，并假设$l\geq r\geq 3$。我们注首先如果W是奇数维数的V的非各向同性子空间，则与$W'$正交补，$\Psi$对W的限制$\Psi_W$是非简并的并且$\mathfrak{o}(\Psi_W)$可以是识别出$\mathfrak{g}$的子代数、元素的由……组成于$W'$消失。如果暗淡$W<$暗淡V，并且如果$\Psi_W$最大为指标，则归纳假设意味着如果$T_r$包含为形式$w'\wedge w$的非零元素，则$w'\in \bigwedge^{r-k}W'$ 和 $w\in \bigwedge^kW (0\leq k\leq r)$，然后 $T_r$ 包含 $w'\wedge \bigwedge^kW:$ 事实上，对于所有 $a\in \mathfrak{o}(\Psi_W)$，我们都有 $a.(w'\wedge w) =w'\wedge a.w$。我们通过归纳在$p\in 0, r$上展示$T_r$包含元素

$$
x=e_{i_1}\wedge  \cdots  \wedge e_{i_{r-p}}\wedge e_{j_1}\wedge  \cdots  \wedge e_{j_p}
$$

对于 $1\leq i_1<\cdots < i_{r-p}\leq l$ 和 $-l\leq j_1<\cdots < j_p\leq 0$。对于$p= 0$，这是根据$\mathfrak{g}\mathfrak{l}(F)$在$\bigwedge^rF$（no. 1）上的运算的不可约性得出的，因为

$\mathfrak{g}$ 包含元素使$F = V_l=\sum_{i=1}^lke_i$固定并在其上引入任何自同态 (cf. 公式 (2))。如果$p= 1$，则令$q\in (1, l)$使得$q\not=-j_1$并且存在$\lambda \in 1, r-p$和$q=i_{\lambda}$；如果$p\geq 2$，则令$q\in 1, l$使得$-q\in  \{j_1, . . . , j_p\}$。如有必要，对$e_i$进行排列，我们可以假设$q= 1$。现在取 $W'=ke_1+ke_{-1}$ 的正交补集作为 W。如果$p= 1$，我们有$x\in e_1\wedge \bigwedge^{r-1}W$；从$T_r$包含$e_1\wedge  \cdots  \wedge e_r$开始，我们看到$T_r$包含$x$。如果$p\geq 2$，则$x\in e_{-1}\wedge \bigwedge^{r-1}W$或$x\in e_1\wedge e_{-1}\wedge \bigwedge^{r-2}W$；从$T_r$包含$e_{-1}\wedge e_2\wedge  \cdots  \wedge e_{r-1}$和$e_{-1}\wedge e_1\wedge e_2\wedge  \cdots  \wedge e_{r-2}$到归纳假设，我们看到$T_r$包含$x$，从而完成了证明。

对于 $\bigwedge^r\sigma$ 的不可约性另一个证明，请参阅 Exerc。 6.

我们现在将确定基本表示与最高权$\varpi_l$。

#### 引理 1 {#lie-viii-s13-lem-1 .statement tag=018T}

令V为有限维向量空间，Q为V$,\Psi$上的非简并二次形式，与Q相关的对称双线性形式，C(Q)相对于V的克利福德代数 Q$,f_0$ 规范映射的复合

$$
\mathfrak{o}(\Psi )\longrightarrow \mathfrak{g}\mathfrak{l}(V)\longrightarrow V\otimes V^*\longrightarrow V\otimes V\longrightarrow C^+(Q)
$$

（第一个是典范嵌入，第三个由$V^*$到V相应的到$\Psi$由典范同构定义，第四个由C(Q)、cf.中的乘法定义代数，第IX, § 9, no. 1）。把$f=\frac{1}{2}f_0$。

(i) 如果 $(e_r),(e'_r)$ 是 V 的基，使得 $\Psi (e_r, e'_s) =\delta_{rs}$，则对于所有 $a\in \mathfrak{o}(\Psi )$，我们有 $f_0(a) =$ $\sum_r(ae_r)e'_r$。

(ii) 如果$a, b\in \mathfrak{o}(\Psi )$，我们有$\sum_r(ae_r)(be'_r) =-\sum_r(abe_r)e'_r$。

(iii) 如果$a\in \mathfrak{o}(\Psi )$和$v\in V$，我们有$[f(a), v] =av$。

(iv) 如果$a, b\in \mathfrak{o}(\Psi )$，我们有$[f(a), f(b)] =f([a, b])$。

(v) $f(\mathfrak{o}(\Psi ))$ 生成联想词代数 $C^+(Q)$。

(vi) 设 N 为左 $C^+(Q)$ 模，且从 $C^+(Q)$ 到 End$_k(N)$ $\rho$ 相应的同态。那么$\rho \circ f$是N上$\mathfrak{o}(\Psi )$的表示。如果N是简单的，$\rho \circ f$是不可约的。

断言 (i) 很清楚。如果$a, b\in \mathfrak{o}(\Psi )$，我们有（放入$\Psi (x, y) =\langle x, y\rangle$）$:$

$$
\sum_r(ae_r)(be'_r) =\sum_{r,s,t}\langle ae_r, e'_s\rangle \langle be'_r, e_t\rangle e_se'_t=\sum_{r,s,t}\langle e_r, ae'_s\rangle \langle e'_r, be_t\rangle e_se'_t
$$

$$
=\sum_{s,t}\langle ae'_s, be_t\rangle e_se'_t=-\sum_{s,t}\langle e'_s, abe_t\rangle e_se'_t=-\sum_t(abe_t)e'_t
$$

这就证明了(ii)。接下来，对于所有 $v\in V$，我们有 (i)，

1 $''$

$$
[f(a), v] =\sum((ae_r)e_rv-v(ae_r)e_r)
$$

2

= $1\sum^r((ae_r)e'_rv+ (ae_r)ve'_r-(ae_r)ve'_r-v(ae_r)e'_r)$

2

$r$

1 $''$

= $\sum((ae_r)\langle e_r, v\rangle  - \langle ae_r, v\rangle e_r)$

2

= $1a(\sum^r\langle e'_r, v\rangle e_r)+1\sum\langle e_r, av\rangle e'_r=1av+1av=av$,

2 $_r$ 2 $_r$ 2 2

这就证明了(iii)。然后

$[f(a), f(b)] =[f(a),\frac{1}{2}\sum(be_r)e'_r]$ 由 (i)

$r$

$=\frac{1}{2}\sum([f(a), be_r]e'_r+ (be_r)[f(a), e'_r])$ $=\frac{1}{2}\sum^r((abe_r)e'_r+ (be_r)(ae'_r))$ 由 (iii)

$r$

$=\frac{1}{2}\sum((abe_r)e'_r-(bae_r)e'_r)$ 由 (ii)

$r$

$=f([a, b])$ 由 (i)

这就证明了(iv)。为了证明(v)，我们可以通过扩展标量，假设$k$是代数闭的。 选择，然后V的基$(e_r)$，使得$\Psi (e_r, e_s) =\delta_{rs}$，所以$e'_r=e_r$。如果 $i\not=j$，则 $E_{ij}-E_{ji}\in \mathfrak{o}(\Psi )$ 且

$$
f(E_{ij}-E_{ji}) =\frac{1}{2}(e_ie_j-e_je_i) =e_ie_j
$$

但是$e_ie_j$生成$C^+(Q)$。

断言 (vi) 由 (iv) 和 (v) 得出。 Q.E.D.

现在回想一下在这个数开头使用的记号。将$\widetilde{V} = F + F'$放入$\widetilde{Q}$（分别为$\widetilde{\Psi}$）为Q（分别为$\Psi$）到$\widetilde{V}$的限制。那么$\widetilde{Q}$是维数$2l$的空间$\widetilde{V}$上的最大指标$l$的非简并二次形式，并且Clifford代数$C( \widetilde{Q})$是中心单代数维数 $2^{2l}($代数，第 1 章IX, §9, no. 4，周四。 2）。令 N 为由 $e_{-1}, . . . , e_{-l}$ 生成的最大各向同性子空间 $F'$ 的外代数。 认同 F 与 $F'$ 的对偶通过 $\Psi$ 和 $x\in F'$（分别为 $y\in F$）表示为 $\lambda (x)$（分别为 $\lambda (y)$）左外部乘积与 $x$（分别为左内部） N 中的乘积与 $y$)；如果$a_1, . . . , a_k\in F'$，那么

$$
\lambda (x).(a_1\wedge  \cdots  \wedge a_k) =x\wedge a_1\wedge  \cdots  \wedge a_k
$$

$$
\lambda (y).(a_1\wedge  \cdots  \wedge a_k) =\sum_{i=1}^k(-1)^{i-1}\Psi (a_i, y)a_1\wedge  \cdots  \wedge a_{i-1}\wedge a_{i+1}\wedge  \cdots  \wedge a_k
$$

很容易验证 $\lambda (x)^2=\lambda (y)^2= 0$ 并且

$$
\lambda (x)\lambda (y) +\lambda (y)\lambda (x) =\Psi (x, y).1
$$

由此可见（代数，IX, §9, no. 1），存在从$C( \widetilde{Q})$到End(N)延伸映射$\lambda : F\cup F'\rightarrow$End(N)的唯一同态（再次用$\lambda$表示）。由于暗淡$N = 2^l$和$C( \widetilde{Q})$有一个独特的类单模，维数$2^l($代数，第1章。 IX, §9, no. 4，周四。 2), $\lambda$定义的N上$C( \widetilde{Q})$的表示是不可约的，并且是$C( \widetilde{Q}) ($loc的旋量表示。引用。）。

现在考虑映射$\mu:v \rightarrow e_0v$从$\widetilde{V}$到$C^+(Q)$。对于$v\in \widetilde{V}$，我们有

$$
(e_0v)^2=-e^2_0v^2=-Q(e_0)Q(v) = Q(v) = \widetilde{Q}(v)
$$

$\mu$ 扩展与同态唯一，再次用 $\mu$ 表示，从 $C( \widetilde{Q})$ 到 $C^+(Q)$。因为 $C( \widetilde{Q})$ 很简单并且因为

昏暗$C^+(Q) =$ 昏暗$C( \widetilde{Q}) = 2^{2l}$，

我们看到$\mu$是同构。因而，N 上的$\lambda \circ \mu^{-1}$ 定义一个简单的$C^+$(Q) 模结构和$\rho =\lambda \circ \mu^{-1}\circ f$ 是N 上$\mathfrak{g}$ 的不可约表示 (引理 1 (vi))。

另一方面，鉴于引理 1 (i)，我们有

$$
f(H_i) =\frac{1}{2}(e_ie_{-i}-e_{-i}e_i)
$$

从$e_ie_{-i}=-e^2_0e_ie_{-i}=e_0e_ie_0e_{-i}$和$e_ie_{-i}+e_{-i}e_i= 1$开始，我们有

$_{-1}$ 1 1

$$
\mu\circ f(H_i) =-e_{-i}e_i=-+e_ie_{-i}
$$

2 2 我们推断，对于 $1\leq i_1<\cdots < i_k\leq l:$

$\rho (H)(e\wedge  \cdots  \wedge e) =\{-\frac{1}{2}e_{-i_1}\wedge  \cdots  \wedge e_{-i_k}$ 如果$i\in  \{i_1, . . . , i_k\}$

$^{i-i_1}-_{i_k}\frac{1}{2}e_{-i_1}\wedge  \cdots  \wedge e_{-i_k}$ 如果$i \notin  \{i_1, . . . i_k\}$

$h\in \mathfrak{h}$

$$
\rho (h)(e_{-i_1}\wedge  \cdots  \wedge e_{-i_k}) \tag{5}
$$

$$
= (\frac{1}{2}(\varepsilon_1+\cdots +\varepsilon_l)-(\varepsilon_{i_1}+\cdots +\varepsilon_{i_k}))(h)(e_{-i_1}\wedge  \cdots  \wedge e_{-i_k})
$$

这表明$\rho$的最高权是$\varpi_l$。我们称$\rho$为$\mathfrak{g}$的旋量表示。 注其权都是简单的（而且$\varpi_l$是极小权）。

(V) 我们有 $w_0=-1$，因而 $\mathfrak{g}$ 的每个有限维简单表示都是正交或辛的。由章。 VI, §4, no. 5.VI、$\varpi_r$相对于$(\alpha_1, . . . , \alpha_l)$的坐标和对于$1\leq r\leq l-1:$是积分，因而，表示与$\bigwedge^r\sigma$是正交的。此外，它留下了$\Psi$到$\bigwedge^rV$的不变扩张$\Psi_{(r)}$。

对于旋量表示，$\varpi_l$相对于$(\alpha_1, . . . , \alpha_l)$的坐标和是$\frac{1}{2}(1 +\cdots +l) =\frac{l(l+1)}{4}($loc。引用。）。因此，它对于 $l\equiv 0$ 或 $-1$ (mod. 4) 是正交的，对于 $l\equiv 1$ 或 2 (mod. 4) 是辛的。事实上，考虑$N =\bigwedge F'$上的双线性形式$\Phi$定义如下：如果$x\in \bigwedge^pF'$和$y\in \bigwedge^qF'$，则放置$\Phi (x, y) = 0$如果$p+q\not=l$和

$$
x\wedge y= (-1)^{^{p(p+1)}_2}\Phi (x, y)e_{-1}\wedge  \cdots  \wedge e_{-r}
$$

如果$p+q=l$。很容易验证$\Phi$是非简并的，并且对于$l\equiv 0,-1$（模4）和交错的对于$l\equiv 1,2$（模4）是正交的。另一方面，鉴于引理 1 (i)，

$$
f(X_{\varepsilon_i}) =e_0e_i,f(X_{-\varepsilon_i}) =-e_0e_{-i}
$$

$1\leq i\leq l$ 和

$$
f(X_{\varepsilon_i-\varepsilon_j}) =\frac{1}{2}(e_ie_{-j}-e_{-j}e_i) =e_ie_{-j}=e_0e_ie_0e_{-j}
$$

对于$1\leq i < j\leq l$，类似地

$$
f(X_{\varepsilon_j-\varepsilon_i}) =-e_0e_je_0e_{-i}, f(X_{\varepsilon_i+\varepsilon_j}) =e_0e_ie_0e_j, f(X_{-\varepsilon_i-\varepsilon_j}) =e_0e_{-i}e_0e_{-j}
$$

因此

$$
\mu^{-1}\circ f(X_{\varepsilon_i}) =e_i,\mu^{-1}f(X_{-\varepsilon_i}) =-e_{-i}
$$

和

$\mu^{-1}\circ f(X_{\pm\varepsilon_i\pm\varepsilon_j}) =ce_{\pm i}e_{\pm j}$ 为 $1\leq i, j\leq l, i\not=j$ 与 $c\in  \{1,-1\}$。现在可以轻松验证$\Phi$实际上是$\mathfrak{g}$不变（cf.Exerc.18）。

(VI) 对于$x\in \mathfrak{g}$，$\sigma (x)$的特征多项式取形式

$$
T^{2l+1}+f_1(x)T^{2l}+f_2(x)T^{2l-1}+\cdots +f_{2l+1}(x)
$$

其中$f_1, . . . , f_{2l+1}$在$\mathfrak{g}$上是不变的多项式函数。

如果 $x=\xi_1H_1+\cdots +\xi_lH_l\in \mathfrak{h}$，则 $f_i(x)$ 是 $\xi_1, . . . , \xi_l,-\xi_1, . . . ,-\xi_l$ 的初等对称函数；这些对称的函数是奇数次数中的零，并且

$$
T^{2l+1}+f_2(x)T^{2l-1}+f_4(x)T^{2l-3}+\cdots +f_{2l}(x)T = T(T^2-\xi_1^2). . .(T^2-\xi^2_l)
$$

因此 $f_2, . . . , f_{2l}$ 是 $\xi_1^2, . . . , \xi_l^2$ 的初等对称函数，它们在代数上独立于 $\mathbf{S}(\mathfrak{h}^*)^W$ 的生成元（第 VI, §4, no. 5.IX）。鉴于§8, no. 3，Th。 1 (i)，我们看到$f_1=f_3=f_5=\cdots = 0$和$(f_2, f_4, . . . , f_{2l})$是$\mathfrak{g}$上不变量多项式函数的代数自由族生成的代数。

(VII) 由于 Dynkin 图的唯一自同构是恒等，因此我们有 Aut($\mathfrak{g}$) $=$ Aut$_0(\mathfrak{g})$。

令$\Sigma$为V相对于$\Psi$的相似度的群。对于所有$g\in \Sigma$，令$\varphi (g)$为自同构$x \rightarrow gxg^{-1}$/$\mathfrak{g}$。那么从$\Sigma$到Aut($\mathfrak{g}$)$\varphi$就是同态。我们证明它是满射的。令 $\alpha \in$ Aut($\mathfrak{g}$) $=$ Aut$_0(\mathfrak{g})$。根据§7, no. 1的命题2，存在$s\in \mathbf{G}\mathbf{L}(V)$，使得$\alpha (x) =sxs^{-1}$对于所有$x\in \mathfrak{g}$。然后将$s$变换$\Psi$转化为V上的双线性形式$\Psi '$，这在$\mathfrak{g}$下是不变的，因此与$\Psi ($§7, no. 5成比例，命题12）。这就证明了$s\in \Sigma$。

由于$\mathfrak{g}$的恒等式表示是不可约的，它与标量（§6, no. 1，命题1）的交换律约化，所以$\varphi$的核是$k^*$。因此，群Aut($\mathfrak{g}$)$=$Aut$_0(\mathfrak{g})$可以与$\Sigma /k^*$识别。但是，它是从代数，第 1 章得出的。 IX, §6, no. 5，群$\Sigma$是群$k^*$和$\mathbf{S}\mathbf{O}(\Psi )$中的乘积；因此Aut($\mathfrak{g}$) $=$ Aut$_0(\mathfrak{g})$可以与$\mathbf{S}\mathbf{O}(\Psi )$识别。

令 $\mathbf{O}^+_0(\Psi )$ 为 $\Psi ($代数的简化正交群，第 1 章。 IX, §9, no. 5）。由于$\mathbf{S}\mathbf{O}(\Psi )/\mathbf{O}^+_0(\Psi )$是可交换的（前述），群Aut$_e(\mathfrak{g})$包含在$\mathbf{O}^+_0(\Psi ) ($§11, no. 2，命题3）；事实上，它等于它（练习7）。

(VIII) $\mathfrak{h}^*$ 上的规范双线性形式 $\Phi_R$ 由下式给出

$\Phi_R(\xi_1\varepsilon_1+\cdots +\xi_l\varepsilon_l, \xi '\varepsilon_1+\cdots +\xi '\varepsilon_l) =$ 1 $(\xi_1\xi '+\cdots +\xi_l\xi ')$

$$
^1l\overline{4l- 2}^1l
$$

（第 VI, §4, no. 5.V）。由$\Phi_R$定义的从$\mathfrak{h}$到$\mathfrak{h}^*$的同构需要$H_i$到$(4l-2).\varepsilon_i$。因此，$\Phi_R$的逆形式，即杀戮形式的限制到$\mathfrak{h}$，是

$$
\Phi (\xi_1H_1+\cdots +\xi_lH_l, \xi '_1H_1+\cdots +\xi '_lH_l) = (4l-2)(\xi_1\xi '_1+\cdots +\xi_l\xi '_l)
$$

(IX) 回想一下公式 (3) 定义的$X_{\alpha}(\alpha \in R)$。很容易验证$[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$对应$\alpha \in R$。另一方面，令M为矩阵$I+E_{0,0}$；自 $M=S^tM^{-1}S$、映射

$$
\theta :g \rightarrow  -M^{-1t}gM
$$

对于所有$\alpha \in R$，是$\mathfrak{g}$和$\theta (X_{\alpha}) =X_{-\alpha}$的自同构。因而，$(X_{\alpha})$ 是 $(\mathfrak{g},\mathfrak{h})$ 中的 Chevalley 系统。

假设$k=\mathbf{Q}$。 嘉当子代数$\mathfrak{h}$有两个允许的格子：由$H_{\alpha}$生成的格子$Q(R^{\vee})$和由$H_i$生成的格子$P(R^{\vee})$，由$\mathfrak{h}$中的对角线矩阵和整数条目组成。由此可见，$\mathfrak{o}_S(2l+ 1,\mathbf{Z})$（$\mathfrak{g}$中矩阵的集合，具有整数条目）是$\mathfrak{g}$中的Chevalley阶$P(R^{\vee}) +\sum\mathbf{Z}.X_{\alpha}$。从$(X_{\pm\varepsilon_i})^2= 2E_{\pm i,\mp i},(X_{\pm\varepsilon_i})^3= 0$和$(X_{\pm\varepsilon_i\pm\varepsilon_j})^2= 0$开始，我们看到维特基$(e_i)_{-l\leq i\leq l}$生成的格$\mathscr{V}$是V中$\mathfrak{o}_S(2l+ 1,\mathbf{Z})$的可接受格。 $\bigwedge^rV$中的$\bigwedge^r\mathscr{V}$也是如此。

现在考虑 $N =\bigwedge F'$ 上 $\mathfrak{g}$ 的旋量表示 $\rho$。由于它的权没有映射$P(R^{\vee})$到$\mathbf{Z}$，所以它没有$\mathfrak{o}_S(2l+ 1,\mathbf{Z})$的允许格子。另一方面，由 N 的典范基 $(e_{-i_1}\wedge  \cdots  \wedge e_{-i_k})$（对于 $1\leq i_1<\cdots < i_k\leq l$）生成的格子 $\mathscr{N}$ 是 Chevalley 阶 $\mathscr{G}= Q(R^{\vee}) +\sum_{\alpha\in R}\mathbf{Z}.X_{\alpha}$ 的可接受格子。事实上，$\mathscr{N}$在直接的下是稳定的

外部乘积与$e_{-i}$，内部乘积与$e_i$（适用于$1\leq i\leq l$）。 (V) 的公式则表明$\mathscr{N}$在$\rho (\mathscr{G})$下是稳定的。此外，由于$\rho (X_{\alpha})^2= 0$对于所有$\alpha \in R$，因而$\mathscr{N}$是可接受的。

### 3. 代数型 C$_{\boldsymbol{l}}$ ($\boldsymbol{l}\geq$ 1)

(I) 设$\Psi$为有限维$2l\geq 2$的向量空间V上的非简并交错的双线性形式； 集合 / 自同态 $x$ / V，使得所有$v, v'\in V$的$\Psi (xv, v') +\Psi (v, xv') = 0$是半单李子代数 / $\mathfrak{s}\mathfrak{l}(V)$（第I, §6, no. 7章，第9条）。我们用 $\mathfrak{s}\mathfrak{p}(\Psi )$ 表示它，并将其称为与 $\Psi$ 相关的辛李代数。

代数，Cap。 IX, §4, no. 2、V可以写成两个最大全各向同性子空间 F和$F'$的直和，它们相对于$\Psi$具有对偶性。设 $(e_i)_{1\leq i\leq l}$ 为 F 的基，且 $(e_{-i})_{1\leq i\leq l}$ 对偶基为 $F'$。然后

$$
(e_1, . . . , e_l, e_{-l}, . . . , e_{-1})
$$

是 V 中的基；我们说它是 V 的维特基（或辛基）。相对于此基$\Psi$矩阵为阶$2l$平方矩阵

$$
(0s)
$$

$J=-s$0

其中 $s$ 是阶 $l$ 的平方矩阵，其所有条目都是零，除了第二条对角线上等于 1 的条目，cf. no. 2.I。

代数$\mathfrak{g}=\mathfrak{s}\mathfrak{p}(\Psi )$可以与方阵$a$或阶$2l$的代数$\mathfrak{s}\mathfrak{p}(2l, k)$识别，使得$a=-J^{-1t}aJ=J^taJ($代数，第1章。 IX, §1, no. 10, 公式 (50)), 即形式

$$
(AB)
$$

$$
a=C-s^tAs
$$

其中$A, B, C$是阶$l$中的方阵，使得$B=s^tBs$和$C=$$c^tCs$；在其他字、$B$和$C$关于第二条对角线对称。由此可见

昏暗$\mathfrak{g}=l^2+ 2\frac{l(l + 1)}{2}=l(2l+ 1)$。

令$\mathfrak{h}$为$\mathfrak{g}$中对角线矩阵的集合。这是 $\mathfrak{g}$ 中的交换子代数，其中 $1\leq i\leq l$ 为基元素 $H_i=E_{i,i}-E_{-i,-i}$。令 $(\varepsilon_i)_{1\leq i\leq l}$ 为 $(H_i)$ 中的对偶基。对于 $1\leq i < j\leq l$，输入

$X_{2\varepsilon_i}$ = $E_{i,-i}$

$X_{-2\varepsilon_i}$ = $-E_{-i,i}$

$X_{\varepsilon_i-\varepsilon_j}$ = $E_{i,j}-E_{-j,-i}$

$X_{-\varepsilon_i+\varepsilon_j}$ = $-E_{j,i}+E_{-i,-j}$ (6)

$X_{\varepsilon_i+\varepsilon_j}$ = $E_{i,-j}+E_{j,-i}$

$X_{-\varepsilon_i-\varepsilon_j}$ = $-E_{-i,j}-E_{-j,i}$。

很容易验证，元素形式基是$\mathfrak{g}$中$\mathfrak{h}$的补集，并且对于$h\in \mathfrak{h}$，

$$
[h, X_{\alpha}] =\alpha (h)X_{\alpha} \tag{7}
$$

对于所有$\alpha \in R$，其中R是$\pm 2\varepsilon_i$和$\pm \varepsilon_i\pm \varepsilon_j(i < j)$的集合。由此可见，$\mathfrak{h}$等于其在$\mathfrak{g}$中的标准化器，因此是$\mathfrak{g}$的嘉当子代数，$\mathfrak{h}$是分裂，$(\mathfrak{g},\mathfrak{h})$的根是R的元素。根系 $(\mathfrak{g},\mathfrak{h})$的R对于$l\geq 2$来说是型$C_l$，对于$l= 1$来说是型$A_1$（在型$C_1$的其他字）（第1章） VI, §4, no. 6.I扩展到案例$l= 1$）。因而，$\mathfrak{g}$是型$C_l$的可拆分简单李代数。

Every splitting Cartan subalgebra of $\mathfrak{g}$ is transformed into $\mathfrak{h}$ by an elementary automorphism, hence by an element of the symplectic group $\mathbf{S}\mathbf{p}(\Psi )$ (cf. (VII)), and consequently is the set $\mathfrak{h}_{\beta}$ of elements of $\mathfrak{g}$ whose matrix with respect to a Witt basis $\beta$ of $\mathfrak{g}$ is diagonal. 立即验证，V中唯一在$\mathfrak{h}_{\beta}$下稳定的向量子空间是由$\beta$中的子集生成的。

我们有$\mathfrak{s}\mathfrak{p}(2, k) =\mathfrak{s}\mathfrak{l}(2, k)$。另一方面，代数$\mathfrak{s}\mathfrak{p}(4, k)$和$\mathfrak{o}_S(5, k)$具有相同的根系，因此是同构的（cf.练习3）。从现在开始，我们假设$l\geq 2$。

(II) 根系 $R^{\vee}$ 由第 1 章确定。 VI, §4, no. 6.I 和 6.V；我们发现

$$
H_{2\varepsilon_i}=H_i, H_{\varepsilon_i-\varepsilon_j}=H_i-H_j, H_{\varepsilon_i+\varepsilon_j}=H_i+H_j
$$

(III) 放入$\alpha_1=\varepsilon_1-\varepsilon_2, . . . , \alpha_{l-1}=\varepsilon_{l-1}-\varepsilon_l, \alpha_l= 2\varepsilon_l$。由章。 VI, §4, no. 6.II，$\{\alpha_1, . . . , \alpha_l\}$是R的基B；相对于 B 的正根是 $2\varepsilon_i$ 和 $\varepsilon_i\pm \varepsilon_j(i < j)$。 相应的博雷尔子代数 $\mathfrak{b}$ 是$\mathfrak{g}$ 中上三角矩阵的集合。

设$\delta$为V中的各向同性标志（即，其元素对于$\Psi$来说都是完全各向同性的子空间），并令$\mathfrak{p}_{\delta}$为$\mathfrak{g}$的元素的子代数由……组成保持稳定元素共 $\delta$。 We show as in no. 2.III that the map $\delta  \rightarrow \mathfrak{p}_{\delta}$ is a bijection from the set of isotropic flags (resp. the maximum isotropic flags) to the set of parabolic (resp. Borel) subalgebras of $\mathfrak{g}$; we have $\mathfrak{p}_{\delta}\supset \mathfrak{p}_{\delta'}$ if and only if $\delta \subset \delta '$.

(IV) 基本的权相应的到 $\alpha_1, . . . , \alpha_l$ 是，第 1 章。 VI, §4, no. 6.VI，$\varpi_i=\varepsilon_1+\cdots +\varepsilon_i(1\leq i\leq l)$。

我们将展示权$\varpi_r$的基本表示$\sigma_r$如何实现为$\bigwedge^r\sigma$的子表示，其中$\sigma$是V上$\mathfrak{g}$的恒等式表示，为此我们将研究分解表示 $\bigwedge\sigma$ $\mathfrak{g}$ 外部代数 $\bigwedge V$。

令$(e^*_i)$为$V^*$对$(e_i)$的基。 交错的双线性形式 $\Psi$ 可以与元素 $\Gamma^*\in \bigwedge^2V^*($代数识别，第 1 章。 III, §7, no. 4、命题 7 和§11, no. 10）并且很容易验证

$$
\Gamma^*=-\sum_{i=1}^le^*_i\wedge e^*_{-i}
$$

设$\Psi^*$为$\Psi$的逆形式（代数，第IX, §1, no. 7）；就是直接的

$$
\Psi^*(e^*_i, e^*_j) = 0
$$

对于$i\not=-j$，$\Psi^*(e^*_i, e^*_{-i}) =-1$对于$1\leq i\leq l$。如果我们认同 $\Psi^*$ 和元素 $\Gamma \in \bigwedge^2V$，那么

$$
\Gamma =\sum_{i=1}^le_i\wedge e_{-i}
$$

由左外部乘积和 $\Gamma$ 给出的 $\bigwedge V$ 的 $X_-$ 自同态表示，并用左内部乘积和 $-\Gamma^*:$ 给出的 $\bigwedge V$ 的 $X_+$ 自同态表示

$$
X_-u=(\sum_{i=1}^le_i\wedge e_{-i})\wedge u
$$

$$
X_+u=(\sum_{i=1}^le^*_i\wedge e^*_{-i})\wedge u
$$

对于计算$X_+$和$X_-$，按以下方式引入$\bigwedge V$的基：对于由$1, l$的三个不相交的子集组成的任意三元组$(A,B,C)$，将

$$
e_{A,B,C}=e_{a_1}\wedge  \cdots  \wedge e_{a_m}\wedge e_{-b_1}\wedge  \cdots  \wedge e_{-b_n}\wedge e_{c_1}\wedge e_{-c_1}\wedge  \cdots  \wedge e_{c_p}\wedge e_{-c_p}
$$

其中$(a_1, . . . , a_m)$（或$(b_1, . . . , b_n),(c_1, . . . , c_p)$）是排列在递增阶中的A（或$B,C$）的元素。这样我们就得到了$\bigwedge V$的基，简单的计算表明：

$$
X_-.e_{A,B,C}=\sum e_{A,B,C\cup \{j\}} \tag{8}
$$

$j\in 1,l ,j \notin A\cup B\cup C$

$$
X_+.e_{A,B,C}=-\sum_{j\in C}e_{A,B,C-\{j\}} \tag{9}
$$

设$H$为$\bigwedge V$的自同态，即约化到乘法乘$(l-r)$在$\bigwedge^rV (0\leq r\leq 2l)$上。验证（cf.练习19）是很容易的

$$
[X_+, X_-] =-H
$$

$$
[H, X_+] = 2X_+
$$

$$
[H, X_-] =-2X_-
$$

In other words, the vector subspace $\mathfrak{s}$ generated by $X_+, X_-$ and $H$ is a Lie subalgebra of End($\bigwedge V$), isomorphic to $\mathfrak{s}\mathfrak{l}(2, k)$, and $\bigwedge^rV$ is the subspace of elements of weight $l-r$. 用原语元素的$\bigwedge^rV$由……组成的$E_r$子空间表示，即$E_r= (\bigwedge^rV)\cap$Ker$X_+$。 从§1得出，对于$r < l$，$X_-$到$\bigwedge^rV$的限制是单射的，对于$r\leq l$，$\bigwedge^rV$分解为直和

$$
\bigwedge^rV = E_r\oplus X_-(E_{r-2})\oplus X_-^2(E_{r-4})\oplus  \cdots
$$

$$
= E_r\oplus X_-(\bigwedge^{r-2}V)
$$

这特别表明 $E_r=(^{2l}_r)-(_{r-2}^{2l})$ 对于 $0\leq r\leq l$ 来说是暗淡的。

另一方面，$\mathfrak{s}\mathfrak{p}(\Psi )$的定义表明$\Gamma^*$被$\sigma$的对偶的第二个外幂湮灭。同样，$\Gamma$被$\bigwedge^2\sigma$湮灭。我们立即推断出$X_+$和$X_-$，以及$H$，与自同态$\bigwedge\sigma (g)$通勤$g\in \mathfrak{g}$。因而，$0\leq r\leq l$的子空间$E_r$在$\bigwedge^r\sigma$下是稳定的；我们将证明$\bigwedge^r\sigma$到$E_r$的限制是权$\varpi_r(1\leq r\leq l)$的基本表示$\sigma_r$。

我们注首先$\bigwedge^r\sigma$相对于$\mathfrak{h}$的权是

$$
\varepsilon_{i_1}+\cdots +\varepsilon_{i_k}-(\varepsilon_{j_1}+\cdots +\varepsilon_{j_{r-k}})
$$

其中$i_1, . . . , i_k$（分别为$j_1, . . . , j_{r-k}$）不同于元素或$1, l$；因而，$\bigwedge^r\sigma$的最高权确实是

$$
\varpi_r=\varepsilon_1+\cdots +\varepsilon_r
$$

权 $\overline{\varpi}_r$中的向量与$e_1\wedge\cdots\wedge e_r=e_{\{1,\ldots,r\},\varnothing,\varnothing}$成比例。 公式 (9) 可知$e_1\wedge\cdots\wedge e_r\in E_r$。因而，只要证明$\bigwedge^r\sigma$到$E_r$的限制是不可约的即可。

如果$s\in\mathbf{Sp}(\Psi)$、$s$到$\bigwedge V$（或$\bigwedge V^*$）的扩张固定了$\Gamma$（或$\Gamma^*$），因此与$X_+$和$X_-$通勤并使$E_r$保持稳定。因而，$E_r$包含向量子空间$F_r$由$e_1\wedge\cdots\wedge e_r$的变换通过$\mathbf{Sp}(\Psi)$生成。维特的定理表明，这些是非零可分解的$r$向量，使得$V$的相应的向量子空间是完全各向同性的子空间、$r$向量，我们称之为各向同性。

#### 引理 2 {#lie-viii-s13-lem-2 .statement tag=01K8}

对于 $1\leq r\leq\ell$，令 $F_r$ 为由各向同性 $r$ 向量生成的 $\bigwedge^r V$ 的子空间。然后

$$
\bigwedge^r V=F_r+X_-\left(\bigwedge^{r-2}V\right)
=F_r+\left(\sum_{i=1}^{\ell}e_i\wedge e_{-i}\right)\wedge\bigwedge^{r-2}V.
$$

我们首先展示引理 2 如何蕴含我们的断言。由于$F_r\subset E_r$和$E_r\cap X_-\left(\bigwedge^{r-2}V\right)=\{0\}$，引理意味着$F_r=E_r$。另一方面，设 $s\in\mathbf{Sp}(\Psi)$； $\operatorname{End}(V)$的自同构$a\mapsto sas^{-1}$保留了$\mathfrak{g}$和诱导在$\operatorname{Aut}_0(\mathfrak{g})$的元素上（cf.（§7, no. 1，命题2），因此每不可约表示都有变换） $\mathfrak{g}$ 转换为等价的表示（§7, no. 1，命题 2）。由于 $e_1\wedge\cdots\wedge e_r$ 属于为 $\bigwedge^r\sigma$ 的不可约分量，并且由于 $E_r=F_r$ 是由 $e_1\wedge\cdots\wedge e_r$ 的变换和 $\mathbf{Sp}(\Psi)$ 生成，因此如下$\mathfrak{g}$在$E_r$上的表示是同型的，但是它的最高权$\overline{\varpi}_r$的重数是$1$，所以它是不可约的。

仍有待证明引理。 $r=1$ 是清楚的。我们通过归纳论证，并假设$r\geq 2$。到归纳假设，我们减少到证明

$$
F_{r-1}\wedge V\subset F_r+\Gamma\wedge\bigwedge^{r-2}V,
$$

或者，如果 $y$ 是可分解的 $(r-1)$-向量且 $x\in V$，则

$$
z=y\wedge x\in F_r+\Gamma\wedge\bigwedge^{r-2}V.
$$

令$(f_i)_{1\leq\pm i\leq\ell}$为$V$的维特基，使得$y=f_1\wedge\cdots\wedge f_{r-1}$。当$x=f_i$时执行证明就足够了。如果 $i\notin[1-r,-1]$，则$r$向量$f_1\wedge\cdots\wedge f_{r-1}\wedge f_i$是各向同性的。否则，我们可以假设，如有必要，右$f_i$重新编号，即$i=1-r$。那么$\Gamma=\displaystyle\sum_{j=1}^{\ell}f_j\wedge f_{-j}$，所以

$$
f_{r-1}\wedge f_{1-r}
=
\frac{1}{\ell-r+2}
\left(
\Gamma-\sum_{i=1}^{r-2}f_i\wedge f_{-i}
+\sum_{j=r}^{\ell}(f_{r-1}\wedge f_{1-r}-f_j\wedge f_{-j})
\right),
$$

$$
z=
\frac{1}{\ell-r+2}\Gamma\wedge f_1\wedge\cdots\wedge f_{r-2}
+
\frac{1}{\ell-r+2}\sum_{j=r}^{\ell}
(f_1\wedge\cdots\wedge f_{r-2})\wedge
(f_{r-1}\wedge f_{1-r}-f_j\wedge f_{-j}).
$$

但是

$$
f_{r-1}\wedge f_{1-r}-f_j\wedge f_{-j}= (f_{r-1}+f_j)\wedge (f_{1-r}-f_{-j})-f_j\wedge f_{1-r}+f_{r-1}\wedge f_{-j}
$$

我们立即验证 $r$-向量

$$
f_1\wedge  \cdots  \wedge f_{r-2}\wedge (f_{r-1}+f_j)\wedge (f_{1-r}-f_{-j})
$$

$f_1\wedge  \cdots  \wedge f_{r-2}\wedge f_j\wedge f_{1-r}$ 和 $f_1\wedge  \cdots  \wedge f_{r-1}\wedge f_{-j}$

$r\leq j\leq l$ 各向同性。因而，$z\in F_r+\Gamma \wedge \bigwedge^{r-2}V$，完成证明。

(V) 我们有 $w_0=-1$，因而 $\mathfrak{g}$ 的每个有限维简单表示都是正交或辛的。由章。 $\varpi_r$相对于$(\alpha_1, . . . , \alpha_l)$的坐标VI, §4, no. 6.VI、和为

$$
r
$$

$$
1 + 2 +\cdots + (r-1) +r+r+\cdots +r+
$$

2

所以$\sigma_r$对于$r$偶数是正交的，对于$r$奇数是辛的。

自 $e_1\wedge  \cdots  \wedge e_r$ 和 $e_{-1}\wedge  \cdots  \wedge e_{-r}$ 属于至 $E_r$ 及之后

$$
\Psi_{(r)}(e_1\wedge  \cdots  \wedge e_r, e_{-1}\wedge  \cdots  \wedge e_{-r}) = 1
$$

我们看到 $\Psi_{(r)}$ 到 $E_r$ 的限制不为零：即，直到常数因子、双线性形式；如果$r$是偶数，则它是对称的；如果$r$是奇数，则交错的是对称的；并且在$\sigma_r$下是不变的。

(VI) 对于所有$x\in \mathfrak{g}$，$\sigma (x)$的特征多项式取形式

$$
T^{2l}+f_1(x)T^{2l-1}+\cdots +f_{2l}(x)
$$

其中$f_1, . . . , f_{2l}$在$\mathfrak{g}$上是不变的多项式函数。

如果 $x=\xi_1H_1+\cdots +\xi_lH_l\in \mathfrak{h}$，$f_i(x)$ 是 $\xi_1, . . . , \xi_l,-\xi_1, . . . ,-\xi_l$ 的初等对称函数；这些对称的函数是奇数次数中的零，并且

$$
T^{2l}+f_2(x)T^{2l-2}+\cdots +f_{2l}(x) = (T^2-\xi_1^2). . .(T^2-\xi^2_l)
$$

如 no. 2.VI 所示，$f_1=f_3=f_5=\cdots = 0$，以及

$$
(f_2, f_4, . . . , f_{2l})
$$

是$\mathfrak{g}$上不变量多项式函数的代数自由族生成的代数。

(VII) 由于 Dynkin 图的唯一自同构是恒等，因此我们有 Aut($\mathfrak{g}$) $=$ Aut$_0(\mathfrak{g})$。

令$\Sigma$为V相对于$\Psi ($代数的相似度群，第1章。 IX, §6，no. 5 结束）。如no. 2.VII所示，$\mathfrak{g}$的自同构是映射$x \rightarrow sxs^{-1}$，其中$s\in \Sigma$，因此Aut($\mathfrak{g}$)$=$Aut$_0(\mathfrak{g})$可以识别为$\Sigma /k^*$。

对于所有$s\in \Sigma$，令$\mu(s)$为乘子除以$s$。从 $\Sigma$ 到 $k^*/k^{*2}$ 映射 $s \rightarrow \mu(s)$ mod $k^{*2}$ 是同态，其核包含 $k^*.1$，因此给出同态 $\lambda$ $\Sigma /k^*$至$k^*/k^{*2}$。我们有$\mathbf{S}\mathbf{p}(\Psi )\cap k^*=\{1,-1\}$。考虑序列 / 同态

1$\longrightarrow \mathbf{S}\mathbf{p}(\Psi )/\{1,-1\}\longrightarrow^{\iota}\Sigma /k^*\longrightarrow^{\lambda}k^*/k^{*2}\longrightarrow 1$。 (10) 映射$\iota$是单射的，且Im($\iota$)$\subset$Ker$\lambda$自$\mathbf{S}\mathbf{p}(\Psi )$的元素乘子为1。若$s\in \Sigma$的乘子为元素 $k^{*2}$，存在$\nu \in k^*$使得$\nu s\in \mathbf{S}\mathbf{p}(\Psi )$；因而，Im($\iota$)$=$Ker($\lambda$)。综上所述，序列(10)是准确的。我们认同$\mathbf{S}\mathbf{p}(\Psi )/\{1,-1\}$与子群$\Sigma /k^*$。由于$k^*/k^{*2}$是可交换的，$\Sigma /k^*$的$\mathbf{S}\mathbf{p}(\Psi )/\{1,-1\}$包含导出群。因而，Aut$_e(\mathfrak{g})$包含在$\mathbf{S}\mathbf{p}(\Psi )/\{1,-1\}($§11, no. 2，命题3）中。事实上，它等于它，并且 Aut($\mathfrak{g}$)$/$Aut$_e(\mathfrak{g})$ 被识别为$k^*/k^{*2}$（练习 9）。

(VIII) $\mathfrak{h}^*$ 上的规范双线性形式 $\Phi_R$ 由下式给出

$$
\Phi_R(\xi_1\varepsilon_1+\cdots +\xi_l\varepsilon_l, \xi '_1\varepsilon_1+\cdots +\xi '_l\varepsilon_l) =\frac{1}{4(l + 1)}(\xi_1\xi '_1+\cdots +\xi_l\xi '_l)
$$

（第 VI, §4, no. 6.V）。因而，$\Phi_R$的逆形式，即杀戮形式的限制到$\mathfrak{h}$，是

$$
\Phi (\xi_1H_1+\cdots +\xi_lH_l, \xi '_1H_1+\cdots +\xi '_lH_l) = 4(l+ 1)(\xi_1\xi '_1+\cdots +\xi_l\xi '_l)
$$

(IX) 回想一下由公式$(6) (\alpha \in R)$定义的$X_{\alpha}$。很容易验证$[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$对应$\alpha \in R$。另一方面，对于所有 $\alpha \in R$，映射 $\theta :a \rightarrow  -^ta$ 是 $\mathfrak{g}$ 和 $\theta (X_{\alpha}) =X_{-\alpha}$ 中的自同构。因而，$(X_{\alpha})_{\alpha\in R}$ 是 $(\mathfrak{g},\mathfrak{h})$ 中的 Chevalley 系统。

假设$k=\mathbf{Q}$。 嘉当子代数 $\mathfrak{h}$ 有两个允许的格子 $Q(R^{\vee}) =\sum_{i=1}^l\mathbf{Z}.H_i$ 和 $P(R^{\vee}) = Q(R^{\vee}) +\frac{1}{2}\mathbf{Z}.\sum_{i=1}^lH_i$（第 VI, §4,

no. 5.VIII 章）。我们看到$Q(R^{\vee})$是矩阵的集合，其中整数条目属于到$\mathfrak{h}$。因而，Chevalley 阶 $Q(R^{\vee}) +\sum_{\alpha\in R}\mathbf{Z}.X_{\alpha}$ 是 $\mathfrak{g}$ 中矩阵的集合 $\mathfrak{s}\mathfrak{p}(2l,\mathbf{Z})$，其中有整数条目。

考虑约简李代数 $\mathfrak{s}\mathfrak{p}(\Psi ) +\mathbf{Q}.1$。很容易看出，其元素和整数条目中的集合是Chevalley阶，其投影到$\mathfrak{s}\mathfrak{p}(\Psi )$平行于$\mathbf{Q}.1$是Chevalley阶$P(R^{\vee}) +\sum\mathbf{Z}.X_{\alpha}$。

最后，为所有$\alpha \in R$提供$X_{\alpha}^2= 0$。由此可见，由 $e_i$ 生成的 V 中的格子 $\mathscr{V}$ 对于 Chevalley 阶 $\mathfrak{s}\mathfrak{p}(2l,\mathbf{Z})$ 是可接受的。这同样适用于$E_r$中的$E_r\cap \bigwedge^r\mathscr{V}$格子。

最后，$E_r$ 具有 Chevalley 阶的可接受格子

$$
P(R^{\vee}) +\sum\mathbf{Z}.X_{\alpha}
$$

仅当 $r$ 为偶数时；那么$E_r\cap \bigwedge^r\mathscr{V}$就是这样一个格子。

### 4. 代数型 $\boldsymbol{D}_{\boldsymbol{l}}$ ($\boldsymbol{l}\geq$ 2)

(I) 令V为维数$2l\geq 4$的向量空间，并令$\Psi$为V上最大指标$l$的非简并对称双线性形式。 代数，第 1 章IX, §4, no. 2、V 可以写成两个最大完全各向同性子空间 F 和$F'$ 的直和。令 $(e_i)_{1\leq i\leq l}$ 为 F 的基且为 $F'$ 的$(e_{-i})_{1\leq i\leq l}$ 对偶基（对于由 $\Psi$ 定义的 F 与 $F'$ 之间的对偶性）。那么$e_1, . . . , e_l, e_{-l}, . . . , e_{-1}$就是V的基；我们将其称为 V 的维特基。 $\Psi$的矩阵相对于此基是平方矩阵阶$2l$的S，其所有条目都是零，除了位于第二个对角线上的条目，它们等于1。代数 $\mathfrak{g}=\mathfrak{o}(\Psi )$可以与阶$2l$的方阵$g$的代数$\mathfrak{o}_S(2l, k)$识别，使得$g=-S^tgS$。它有维数$l(2l-1)$。简单计算可知，$\mathfrak{g}$是集合 / 矩阵 / 形式

$$
(AB)
$$

$$
CD
$$

其中$A, B, C, D$是阶$l$的方阵，使得$B=-s^tBs, C=$$-s^tCs$和$D=-s^tAs(s$是阶$l$的矩阵，其所有条目都是零，除了位于第二条对角线等于 1)。

令$\mathfrak{h}$为矩阵属于到$\mathfrak{g}$的对角线集合。这是$\mathfrak{g}$的交换子代数，基由元素$H_i=E_{i,i}-E_{-i,-i}$组成$1\leq i\leq l$。令$(\varepsilon_i)$为$\mathfrak{h}^*$对$(H_i)$的基。对于 $1\leq i < j\leq l$，

$X_{\varepsilon_i-\varepsilon_j}$ = $E_{i,j}-E_{-j,-i}$

$X_{-\varepsilon_i+\varepsilon_j}$ = $-E_{j,i}+E_{-i,-j}$

$X_{\varepsilon_i+\varepsilon_j}$ = $E_{i,-j}-E_{j,-i}$ (11)

$X_{-\varepsilon_i-\varepsilon_j}$ = $-E_{-j,i}+E_{-i,j}$。

这些元素形式基是$\mathfrak{g}$中$\mathfrak{h}$的补集。对于$h\in \mathfrak{h}$，

$$
[h, X_{\alpha}] =\alpha (h)X_{\alpha}
$$

对于所有$\alpha \in R$，其中R是$\pm \varepsilon_i\pm \varepsilon_j(i < j)$的集合。因而，$\mathfrak{h}$是$\mathfrak{g}$的分裂嘉当子代数，$(\mathfrak{g},\mathfrak{h})$的根是R的元素。因而，$(\mathfrak{g},\mathfrak{h})$的根系R是型$D_l$ $l\geq 3$，型$A_1\times A_1$（型$D_2$的其他字）为$l= 2$（第VI, §4, no. 8.I章扩展到案例$l= 2$）。因而，如果$l\geq 3$，则$\mathfrak{g}$是型$D_l$的可拆分简单李代数。

$\mathfrak{g}$ 的每个分裂嘉当子代数都会通过 $\mathfrak{g}$ 的基本自同构转换为 $\mathfrak{h}$，因此通过 $\mathbf{O}(\Psi )$ 的元素 (cf. (VII)) 转换为$\mathfrak{g}$的元素集合$\mathfrak{h}_{\beta}$，其矩阵相对于V的维特基$\beta$是对角线。我们立即验证$\mathfrak{h}_{\beta}$下唯一的子空间不变量是由$\beta$的子集生成的。

由于代数 $\mathfrak{o}_S(4, k)$ 和 $\mathfrak{s}\mathfrak{l}(2, k)\times \mathfrak{s}\mathfrak{l}(2, k)$ 具有相同的根系，因此它们是同构的。类似地，$\mathfrak{o}_S(6, k)$和$\mathfrak{s}\mathfrak{l}(4, k)$是同构的（cf.也是Exerc.3）。从现在开始，我们假设$l\geq 3$。 （II）我们确定$R^{\vee}$通过第1章。 VI, §4, no. 8。V。我们发现

$$
H_{\varepsilon_i-\varepsilon_j}=H_i-H_j,H_{\varepsilon_i+\varepsilon_j}=H_i+H_j
$$

（III）放入$\alpha_1=\varepsilon_1-\varepsilon_2, \alpha_2=\varepsilon_2-\varepsilon_3, . . . , \alpha_{l-1}=\varepsilon_{l-1}-\varepsilon_l, \alpha_l=\varepsilon_{l-1}+\varepsilon_l$。由章。 VI, §4, no. 8.II，$(\alpha_1, . . . , \alpha_l)$是R的基B；相对于 B 的正根是 $\varepsilon_i\pm \varepsilon_j(i < j)$。 相应的博雷尔子代数$\mathfrak{b}$是上三角矩阵属于到$\mathfrak{g}$的集合。

很容易验证，$\mathfrak{b}$下唯一非平凡的向量子空间不变量是完全各向同性子空间$V_1, . . . ,V_l,V'_l$，其中$V_i$由$e_1, . . . , e_i$生成，$V'_l$由$e_1, . . . , e_{l-1}, e_{-l}$生成，并且$V_1, . . . ,V_{l-1}$ 的正交补集$V_{-1}, . . . ,V_{-l+1}$； $V_i$ 的正交补$V_{-i}$ 由$e_1, . . . , e_l, e_{-l}, . . . , e_{-(i+1)}$ 生成。但直接的计算表明，如果元素$a\in \mathfrak{g}$保持$V_{l-1}$稳定，则其矩阵为形式

$$
AxB
$$

$(\lambda$ 0 $)$

0 0 $-\lambda y$

0 0 $D$

其中$A, B, D$是阶$l-1,x$（或$y$）的方阵，是矩阵，有2个列和$l-1$行（分别是2行和$l-1$列），以及$\lambda \in k$。 由此可见，$a$ 使 $V_l$ 和 $V'_l$ 保持稳定。 因而，$\mathfrak{b}$ 是 $a\in \mathfrak{g}$ 的集合，使各向同性标志 $(V_1, . . . ,V_{l-1})$ 的所有元素保持稳定。 注前面和维特的定理（代数，第IX, §4, no. 3，第1章）意味着$V_l$和$V'_l$是唯一最大的完全各向同性子空间包含$V_{l-1}$。

如果一个各向同性标志是由维数 $1, . . . , l-1$ 的 $l-1$ 完全各向同性子空间组成，我们说各向同性标志是准最大的。然后我们在no. 2中看到，对于任何准最大各向同性标志$\delta$，$a\in \mathfrak{g}$的集合$\mathfrak{b}_{\delta}$，离开$\delta$的元素稳定是$\mathfrak{g}$的博雷尔子代数，并且映射 $\delta  \rightarrow \mathfrak{b}_{\delta}$是从准最大各向同性标志的集合到博雷尔子代数的集合的双射。

We say that an isotropic flag is proper if it does not contain both a subspace of dimension $l$ and a subspace of dimension $l-1$. 令$\delta$为这样一个各向同性标志，并令$\mathfrak{p}_{\delta}$为$a\in \mathfrak{g}$的集合，留下$\delta$的稳定元素。 若$\delta \subset  \{V_1, . . . ,V_l,V'_l\}$，则$\mathfrak{p}_{\delta}$是$\mathfrak{g}$、包含于$\mathfrak{b}$的抛物线子代数，容易验证在$\mathfrak{p}_{\delta}$下唯一完全各向同性的子空间、$\not=\{0\}$稳定的是$\delta$的元素。 由于$\{V_1, . . . ,V_l,V'_l\}$和包含$V_{l-1}$中包含$2^{l-2}$正确的各向同性标志（分别为$V_l$、$V'_l$、包含于，既不是$V_{l-1}$，也不是$V_l$，也不是$V'_l$），这给出$2^l$抛物线子代数包含$\mathfrak{b}$。 如上所述，从真各向同性旗的集合到$\mathfrak{g}$的抛物线子代数的集合，映射$\delta  \rightarrow \mathfrak{p}_{\delta}$为双射。

(IV) 基本的权相应的到 $\alpha_1, . . . , \alpha_l$ 是，第 1 章。 VI, §4, no. 8.VI,

$$
\varpi_i=\varepsilon_1+\varepsilon_2+\cdots +\varepsilon_i(1\leq i\leq l-2)
$$

$$
\varpi_{l-1}=\frac{1}{2}(\varepsilon_1+\varepsilon_2+. . .+\varepsilon_{l-2}+\varepsilon_{l-1}-\varepsilon_l)
$$

$$
\varpi_l=\frac{1}{2}(\varepsilon_1+\varepsilon_2+. . .+\varepsilon_{l-2}+\varepsilon_{l-1}+\varepsilon_l)
$$

令$\sigma$为$\mathfrak{g}$在V上的恒等式表示。外部幂$\bigwedge^r\sigma$在$E =\bigwedge^r(V)$上运行。如果$h\in \mathfrak{h}$，我们有

$$
\sigma (h)e_i=\varepsilon_i(h)e_i,\sigma (h)e_{-i}=-\varepsilon_i(h)e_{-i}
$$

对于$1\leq i\leq l$。由此可见，$1\leq r\leq l,\varepsilon_1+\cdots +\varepsilon_r$是$\bigwedge^r\sigma$的最高权，权$\varepsilon_1+\cdots +\varepsilon_r$的元素是与$e_1\wedge  \cdots  \wedge e_r$成比例的值。

我们将证明，对于$1\leq r\leq l-2$，表示$\bigwedge^r\sigma$是权$\varpi_r$的基本表示。

为此，只需证明 $\bigwedge^r\sigma$ 对于 $1\leq r\leq l-1$ 是不可约的（注表示 $\bigwedge^l\sigma$ 不是不可约的，cf. 练习 10），或者最小的子空间 $T_r$ $\bigwedge^rV$包含$e_1\wedge  \cdots  \wedge e_r$稳定在$\mathfrak{g}$以下是$\bigwedge^rV$的整体。这是 $r= 1$ 的直接的。对于$r= 2$，我们在no. 2中看到$\bigwedge^2\sigma$等价于$\mathfrak{g}$的伴随表示，这是不可约的，因为$\mathfrak{g}$是简单的。 证明是通过归纳对$l$争论来完成的，如no. 2，但假设$l-1\geq r\geq 3$。

我们现在要去确定最高权$\varpi_{l-1}$和$\varpi_l$的基本表示。令 Q 为二次方形式 $x \rightarrow \frac{1}{2}\Psi (x, x)$。我们在no. 2.IV中定义了$N =\bigwedge F'$上的Clifford代数C(Q)的旋量表示$\lambda$。我们立即验证，对于$p$偶数（或奇数），由$\bigwedge^pF'$的和给出的N的子空间$N_+$（或$N_-$）在$\lambda$至$C^+(Q)$的限制下是稳定的。因而，$N_+$和$N_-$上$C^+(Q)$的表示$\lambda_+$和$\lambda_-$分别是$C^+(Q) ($代数的半旋量表示，第1章。 IX, §9, no. 4);它们是不可约的，维数$2^{l-1}$且不等价。令$\rho_+=\lambda_+\circ f$和$\rho_-=\lambda_-\circ f$为$\mathfrak{g}$中的相应的不可约表示（no. 2，引理 1 (vi)）。鉴于引理 1 (i)，我们有

$$
f(H_i) =\frac{1}{2}(e_ie_{-i}-e_{-i}e_i) =e_ie_{-i}-\frac{1}{2}=\frac{1}{2}-e_{-i}e_i
$$

我们看到，如no. 2.IV，对于$h\in \mathfrak{h}$和$1\leq i_1<\cdots < i_k\leq l$，

$$
\lambda \circ f(h)(e_{-i_1}\wedge  \cdots  \wedge e_{-i_k})
$$

$$
= (\frac{1}{2}(\varepsilon_1+\cdots +\varepsilon_l)-(\varepsilon_{i_1}+\cdots +\varepsilon_{i_k}))(h)(e_{-i_1}\wedge  \cdots  \wedge e_{-i_k})
$$

因而，$\rho_+$（或$\rho_-$）的最高权为$\varpi_l$（或$\varpi_{l-1}$）。

我们说$\rho_+$和$\rho_-$是$\mathfrak{g}$的半旋量表示。他们所有的权都很简单。我们还说$\rho =\lambda \circ f=\rho_+\oplus \rho_-$是$\mathfrak{g}$的旋量表示。

(V) 对于$1\leq r\leq l-2$，基本表示$\bigwedge^r\sigma$是正交的：它留下$\Psi$到$\bigwedge^rV$的不变扩张。

现在考虑 $\mathfrak{g}$ 的旋量表示 $\rho$。我们在no. 2中证明，对于$1\leq i, j\leq l, i\not=j$，

$$
f(X_{\varepsilon_i-\varepsilon_j}) =\pm e_ie_{-j}
$$

$$
f(X_{\varepsilon_i+\varepsilon_j}) =\pm e_ie_j
$$

$$
f(X_{-\varepsilon_i-\varepsilon_j}) =\pm e_{-i}e_{-j}
$$

由此可见，no. 2.V中引入的非简并双线性形式$\Phi$在$\rho (\mathfrak{g})$下是不变的。因此，旋量表示$\rho$留下不变的非简并形式，它对于$l\equiv 0,-1$（模4）对称，对于$l\equiv 1,2$（模4）对称交错的。

如果 $l$ 是偶数，$\Phi$ 到 $N_+$ 和 $N_-$ 的限制是非简并的，半旋量表示对于 $l\equiv 0$ (mod. 4) 是正交的，对于 $l\equiv 2$ (mod. 4) 是辛的。此外，我们注$w_0=-1$（第VI, §4, no. 8.XI）。

另一方面，如果 $l$ 是奇数，则 $N_+$ 和 $N_-$ 对于 $\Phi$ 是完全各向同性的。此外，$-w_0(\alpha_i) =\alpha_i$对于$1\leq i\leq l-2,-w_0(\alpha_l) =\alpha_{l-1}$和$-w_0(\alpha_{l-1}) =\alpha_l$（第VI, §4, no. 8.XI），因此$-w_0(\varpi_l) =\varpi_{l-1}$和半旋量表示既不正交也不辛；它们中的每一个都与另一个的对偶同构。

(VI) 对于所有$x\in \mathfrak{g}$，$\sigma (x)$的特征多项式取形式

$$
T^{2l}+f_1(x)T^{2l-1}+\cdots +f_{2l}(x)
$$

我们在no. 3中看到$f_1=f_3=f_5=\cdots = 0$。由章。 VI, §4, no. 8。IX 和 §8, no. 3，Th。 1、$\mathfrak{g}$上存在多项式函数$\widetilde{f}$，使得$\mathfrak{g}$上的不变量多项式函数的$f_2, f_4, . . . , f_{2l-2},\widetilde{f}$生成代数$I(\mathfrak{g}^*)$在代数上独立，进一步$\widetilde{f}^2= (-1)^lf_{2l}$。

对于所有$x\in \mathfrak{g}$，我们有$^t(Sx) =^txS=-Sx$，所以我们可以考虑Pf($Sx$)，它是$x$的多项式函数。现在：

$f_{2l}(x) =$ det($x$) $= (-1)^l$ det($Sx$) $= (-1)^l$(Pf($Sx$))$^2$。

因此，我们可以取 $\widetilde{f}(x) =$ Pf($Sx$)。

(VII) 回想一下（§5, no. 3，命题 5 的修正 1），Aut($\mathfrak{g}$)$/$Aut$_0(\mathfrak{g})$ 可以与 $(\mathfrak{g},\mathfrak{h})$ 的 Dynkin 图 D 的群 Aut(D) 或自同构进行识别。 When $l\not= 4$, Aut(D) is the group of order 2 consisting of the permutations of $\alpha_1, . . . , \alpha_l$ that leave $\alpha_1, . . . , \alpha_{l-2}$ fixed. 当$l= 4$时，Aut(D)由$\alpha_1, . . . , \alpha_4$的置换组成，而$\alpha_2$固定；它与$\mathfrak{S}_3$同构的（cf.章节VI, §4, no. 8.XI）。 在所有情况下，保持 $\alpha_1$ 固定的 Aut(D) 由……组成元素的子群为阶 2。 我们用 Aut($\mathfrak{g}$) 的 Aut$'(\mathfrak{g})$ 相应的子群表示；我们有 Aut$'(\mathfrak{g}) =$ Aut($\mathfrak{g}$) if $l\not= 4$ 和 (Aut($\mathfrak{g}$) $:$ Aut$'(\mathfrak{g})$) $= 3$ if $l= 4$；而且，

（自动$'(\mathfrak{g}) :$自动$_0(\mathfrak{g})$）$= 2$。

元素 $s\in$ Aut($\mathfrak{g}$) 属于到 Aut$'(\mathfrak{g})$ 当且仅当 $\sigma \circ s$ 等价于 $\sigma$ （这源于$\varpi_1$ 是 $\sigma$ 的最高权 ）。我们结论就像no. 2.VII一样，Aut$'(\mathfrak{g})$可以与$\Sigma /k^*$识别，其中$\Sigma$是V相对于$\Psi$的相似性的群。

令$s\in \Sigma$，并令$\lambda (s)$为$s$的乘子。如果 $s$ 是正数，我们有 det($s$) $=\lambda (s)^l$；如果 $s$ 是逆数，我们有 det($s$) $=-\lambda (s)^l$（代数，第 IX, §6, no. 5 章）。 $\Sigma$ 中指标 2 的直接相似性形式子群 $\Sigma_0$；我们有$\Sigma_0\supset k^*$。 群 $\Sigma_0/k^*$ 等于 Aut$'(\mathfrak{g}) =\Sigma /k^*$ 的子群 Aut$_0(\mathfrak{g})$。事实上，当 $k$ 代数闭合时就足以验证这一点：在这种情况下，Aut$_0(\mathfrak{g}) =$ Aut$_e(\mathfrak{g})$ 等于它的导出群（§11, no. 2，命题 3），因此包含在 $\Sigma_0/k^*$ 中，并且因为它们都是指标 2 $\Sigma /k^*$，它们是平等的。

另一方面，如no. 3.VII，有正合序列

$$
1\longrightarrow \mathbf{S}\mathbf{O}(\Psi )/\{1,-1\} \longrightarrow \Sigma_0/k^*\longrightarrow k^*/k^{*2}\longrightarrow 1
$$

认同 $\mathbf{S}\mathbf{O}(\Psi )/\{1,-1\}$ 与 $\Sigma_0/k^*=$ Aut$_0(\mathfrak{g})$ 的子群。由于 $k^*/k^{*2}$ 是可交换的，所以我们有 Aut$_e(\mathfrak{g})\subset \mathbf{S}\mathbf{O}(\Psi )/\{1,-1\}$。事实上，可以证明（练习11）Aut$_e(\mathfrak{g})$等于$\Psi ($代数的简化正交群$\mathbf{O}^+_0(\Psi )$的$\mathbf{S}\mathbf{O}(\Psi )/\{1,-1\}$中的像，第1章。 IX, §9, no. 5）。

(VIII) $\mathfrak{h}^*$ 上的规范双线性形式 $\Phi_R$ 由下式给出

$''$ 1 $''$

$$
\Phi_R(\xi_1\varepsilon_1+\cdots +\xi_l\varepsilon_l, \xi_1\varepsilon_1+\cdots +\xi_l\varepsilon_l) =(\xi_1\xi +\cdots +\xi_l\xi )
$$

$$
\overline{4(l- 1)}^1l
$$

（第 VI, §4, no. 8.V）。因而，杀戮形式到$\mathfrak{h}$的限制是

$$
\Phi (\xi_1H_1+\cdots +\xi_lH_l, \xi '_1H_1+\cdots +\xi '_lH_l) = 4(l-1)(\xi_1\xi '_1+\cdots +\xi_l\xi '_l)
$$

(IX) 回想一下公式 (11) 定义的$X_{\alpha}(\alpha \in R)$。我们很容易验证$[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$对应$\alpha \in R$。另一方面，对于所有 $\alpha \in R$，映射 $\theta :a \rightarrow  -^ta$ 是 $\mathfrak{g}$ 和 $\theta (X_{\alpha}) =X_{-\alpha}$ 中的自同构。因而 $(X_{\alpha})_{\alpha\in R}$ 是 $(\mathfrak{g},\mathfrak{h})$ 中的 Chevalley 系统。

假设$k=\mathbf{Q}$。由章。如果 $l$ 是奇数，VI, §4, no. 8.VIII、子代数 $\mathfrak{h}$ 有 3 个允许的格子，如果 $l$ 是偶数，则有 4 个允许的格子。特别是，由$H_i$生成的晶格$\mathscr{H}$是允许的。但这个格子是 $\mathfrak{g}$ 中对角线矩阵的集合，有整数个条目。由此可见，$\mathfrak{o}_S(2l,\mathbf{Z})$ 是 $\mathfrak{g}$ 中的 Chevalley 阶 $\mathscr{H}+\sum\mathbf{Z}.X_{\alpha}$。由于$X_{\alpha}^2= 0$对于所有$\alpha \in R$，我们看到由Witt基$(e_i)$生成的V中的格子$\mathscr{V}$是V中对于$\mathfrak{o}_S(2l,\mathbf{Z})$的可接受格子。 $\bigwedge^rV$中的$\bigwedge^r\mathscr{V}$也是如此。

另一方面，如果我们将 $P(R^{\vee}) =\mathbf{Z}.\frac{1}{2}\sum_{i=1}^lH_i+\mathscr{H}$ 作为容许格，将 $\mathscr{G}= P(R^{\vee}) +\sum\mathbf{Z}.X_{\alpha}$ 作为 Chevalley 阶，我们会发现，仅当 $r$ 是偶数时，$\bigwedge^rV$ 才具有容许格； $\bigwedge^r\mathscr{V}$ 则可以接受。

考虑约简李代数 $\mathfrak{o}(\Psi ) +\mathbf{Q}.1$；我们立即看到格子$\widetilde{\mathscr{G}}= (\mathfrak{o}(\Psi ) +\mathbf{Q}.1)\cap \mathfrak{g}\mathfrak{l}(2l,\mathbf{Z})$是Chevalley阶。 Chevalley 阶 $\mathscr{G}$ 是 $\widetilde{\mathscr{G}}$ 的投影到 $\mathfrak{o}(\Psi )$ 上，与中心 $\mathbf{Q}.1$ 平行。

最后，我们在no. 2中看到，由$e_{-i_1}\wedge  \cdots  \wedge e_{-i_{2k}}$（分别$e_{-i_1}\wedge  \cdots  \wedge e_{-i_{2k+1}}$）生成的晶格$\mathscr{N}_+$（分别$\mathscr{N}_-$）对于谢瓦利阶$Q(R^{\vee}) +\sum_{\alpha\in R}\mathbf{Z}.X_{\alpha}$的半旋量表示是可接受的。另一方面，$\mathscr{N}_+$和$\mathscr{N}_-$对于$\mathfrak{o}_S(2l,\mathbf{Z})$没有可接受的格子。

表1

如果相应的简单表示是正交的（分别为辛，分别为既不正交也不辛），我们就将每个基数权数 1（分别为 $-1,0$）关联起来。这个数的计算本质上已经在§13中针对型$A_l,B_l,C_l,D_l$给出了。 型 $E_6,E_7,E_8,F_4,G_2$ 的结果也如下所示（只需应用 §7、第 12 条提案和VI, §4 章第 9.VI、9.XI、10.VI、 10.XI、11.VI、11.XI、12.VI、12.XI、13.VI、13.XI）。

$$
A_l(l\geq 1)B_l(l\geq 2)
$$

$\{0r\not=\frac{l+1}{2}\varpi_r$ 1 $r\not=l$

$$
\varpi_r
$$

$$
(-1)^rr=\frac{l+1}{2}\varpi_l(-1)^{l(l+1)/2}
$$

$$
C_l(l\geq 2)D_l(l\geq 2)
$$

$\varpi_r(-1)^r\varpi_r$ 1 $r\not=l-1, l$

$\{0$ 如果 $l$ 是奇数

如果 $l$ 是偶数，则$\varpi_l$ 和 $\varpi_{l-1}(-1)^{l/2}$

$$
E_6E_7E_8F_4G_2
$$

$\varpi_1$ 0 $\varpi_1$ 1 $\varpi_1$ 1 $\varpi_1$ 1 $\varpi_1$ 1

$\varpi_2$ 1 $\varpi_2-1\varpi_2$ 1 $\varpi_2$ 1 $\varpi_2$ 1

$\varpi_3$ 0 $\varpi_3$ 1 $\varpi_3$ 1 $\varpi_3$ 1

$\varpi_4$ 1 $\varpi_4$ 1 $\varpi_4$ 1 $\varpi_4$ 1

$\varpi_5$ 0 $\varpi_5-1\varpi_5$ 1

$\varpi_6$ 0 $\varpi_6$ 1 $\varpi_6$ 1

$\varpi_7-1\varpi_7$1

$\varpi_8$1

表2

我们将相应的简单表示的每个基本权维数联系起来，通过Th计算。 2 个§9。

$$
A_l(l\geq 1)B_l(l\geq 2)
$$

$$
(l+ 1)(2l+ 1)
$$

$$
\varpi_r(1\leq r\leq l)\varpi_r(1\leq r\leq l-1)
$$

$$
rr
$$

$$
\varpi_l2^l
$$

$$
C_l(l\geq 2)D_l(l\geq 2)
$$

$$
(2l)(2l)(2l)
$$

$$
\varpi_r(1\leq r\leq l)-\varpi_r(1\leq r\leq l-2)
$$

$$
rr-2r
$$

$$
\varpi_{l-1}2^{l-1}
$$

$$
\varpi_l2^{l-1}
$$

$$
E_6E_7
$$

$$
\varpi_127 = 3^3\varpi_1133 = 7.19
$$

$$
\varpi_278 = 2.3.13\varpi_2912 = 2^4.3.19
$$

$$
\varpi_3351 = 3^3.13\varpi_38645 = 5.7.13.19
$$

$$
\varpi_42925 = 3^2.5^2.13\varpi_4365750 = 2.5^3.7.11.19
$$

$$
\varpi_5351 = 3^3.13\varpi_527664 = 2^4.7.13.19
$$

$$
\varpi_627 = 3^3\varpi_61539 = 3^4.19
$$

$$
\varpi_756 = 2^3.7
$$

$$
E_8F_4
$$

$$
\varpi_13875 = 5^3.31\varpi_152 = 2^2.13
$$

$$
\varpi_2147250 = 2.5^3.19.31\varpi_21274 = 2.7^2.13
$$

$$
\varpi_36696000 = 2^6.3^3.5^3.31\varpi_3273 = 3.7.13
$$

$$
\varpi_46899079264 = 2^5.3.7^2.11^2.17.23.31\varpi_426 = 2.13
$$

$$
\varpi_5146325270 = 2.3.5.7^2.13^2.19.31
$$

$$
\varpi_62450240 = 2^6.5.13.19.31
$$

$$
\varpi_730380 = 2^2.5.7^2.31G_2
$$

$\varpi_8248 = 2^3.31\varpi_1$7

$$
\varpi_214 = 2.7
$$

### 习题 {#lie-viii-s13-exercises}

参见[习题为 § 13](exercises/s13/)。
