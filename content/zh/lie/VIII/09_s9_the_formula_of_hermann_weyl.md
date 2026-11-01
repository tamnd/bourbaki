---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 9
section_title: The formula of Hermann Weyl
lang: zh
source: lie-vii-ix
book_pages: 152-159, 253-260
pdf_pages: 0160-0167, 0261-0268
extraction: native
subsections:
    - "no": 1
      title: CHARACTERS OF FINITE DIMENSIONAL $\mathfrak{g}$-MODULES
      page: 152
      pdf_page: 160
    - "no": 2
      title: DIMENSIONS OF SIMPLE $\mathfrak{g}$-MODULES
      page: 154
      pdf_page: 162
    - "no": 3
      title: MULTIPLICITIES OF WEIGHTS OF SIMPLE $\mathfrak{g}$-MODULES
      page: 156
      pdf_page: 164
    - "no": 4
      title: DECOMPOSITION OF TENSOR PRODUCTS OF SIMPLE $\mathfrak{g}$-MODULES
      page: 157
      pdf_page: 165
statements: 12
exercises: 16
content_sha256: 7eac7ccceb8eb741790f0f9a110cf3f31738fd7bb70bf00090fabfeaf9c96cd8
translated_from: content/en/lie/VIII/09_s9_the_formula_of_hermann_weyl.md
translation_method: google
source_content_sha256: 16e58934b12a0ac3234fd1dee9446b6558b2edb33a94c1d55bbd2fbd906273b2
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 7f4ed5db9c80df419c4d7e4466a274ea10b8d4b350fd99469e38583d6c806324
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 9。 魏尔公式

在本段中，我们保留了§6和§7的通用记号。

### 1. 特征标有限维$\mathfrak{g}$-模块

令 $(e^{\lambda})_{\lambda\in\mathfrak{h}^*}$ 为环 $\mathbf{Z}[\mathfrak{h}^*]$ 中的典范基。给出因子上离散拓扑从$\mathfrak{h}^*$到$\mathbf{Z}$乘积拓扑的所有映射的空间$\mathbf{Z}^{\mathfrak{h}^*}$。如果$\varphi \in \mathbf{Z}^{\mathfrak{h}^*}$，则族$(\varphi (\nu )e^{\nu})_{\nu\in\mathfrak{h}^*}$是可求和的，并且

$$
\varphi =\sum_{\nu\in\mathfrak{h}^*}\varphi (\nu )e^{\nu}
$$

令$\mathbf{Z}\langle P\rangle$为$\varphi \in \mathbf{Z}^{\mathfrak{h}^*}$的集合，其支撑包含在形式$\nu -P_+$的集合的有限并中，其中$\nu \in \mathfrak{h}^*$。然后$\mathbf{Z}[P]\subset \mathbf{Z}\langle P\rangle  \subset \mathbf{Z}^{\mathfrak{h}^*}$。 定义在 $\mathbf{Z}\langle P\rangle$ 环结构上通过放置来扩展$\mathbf{Z}[P]$，对于 $\varphi , \psi \in \mathbf{Z}\langle P\rangle$ 和 $\nu \in \mathfrak{h}^*$，

$$
(\varphi \psi )(\nu ) =\sum_{\mu\in\mathfrak{h}^*}\varphi (\mu)\psi (\nu -\mu)
$$

（$(\varphi (\mu)\psi (\nu -\mu))_{\mu\in\mathfrak{h}^*}$家庭有有限支撑，因为条件满足于$\varphi$和$\psi$的支持）。如果$\varphi =\sum_{\nu}x_{\nu}e^{\nu}$和$\psi =\sum_{\nu}y_{\nu}e^{\nu}$，则$\varphi \psi =\sum_{\nu ,\mu}x_{\nu}y_\mu e^{\nu+\mu}$。

让$\nu \in \mathfrak{h}^*$。 $\nu$的划分转化为正根是一个族$(n_{\alpha})_{\alpha\in R_+}$，其中$n_{\alpha}$是整数$\geq 0$使得$\nu =\sum_{\alpha\in R_+}n_{\alpha}\alpha$。我们将$\nu$的划分的$\mathfrak{P}(\nu )$数表示为正根。我们有

$$
\mathfrak{P}(\nu )>0\Leftarrow \Rightarrow \nu \in Q_+
$$

在本段中，我们用 K 表示 $\mathbf{Z}\langle P\rangle :$ 的以下元素

$$
K =\sum_{\gamma\in Q_+}\mathfrak{P}(\gamma )e^{-\gamma}
$$

现在回想一下（第 VI, §3, no. 3 章，命题 2）

$$
d=\prod_{\alpha\in R_+}(e^{\alpha /2}-e^{-\alpha /2}) =\sum_{w\in W}\varepsilon (w)e^{w\rho}
$$

是 $\mathbf{Z}[P]$ 的反不变量元素。

#### 引理 1 {#lie-viii-s9-lem-1 .statement tag=015T}

在环$\mathbf{Z}\langle P\rangle$，我们有$K.\prod_{\alpha\in R_+}(1-e^{-\alpha}) = Ke^{-\rho}d= 1$。

确实，

$$
K =\prod_{\alpha\in R_+}(e^0+e^{-\alpha}+e^{-2\alpha}+\cdots )
$$

所以

$$
Ke^{-\rho}d=\prod_{\alpha\in R_+}(1 +e^{-\alpha}+e^{-2\alpha}+\cdots )\prod_{\alpha\in R_+}(1-e^{-\alpha}) = 1
$$

#### 引理 2 {#lie-viii-s9-lem-2 .statement tag=015U}

让$\lambda \in \mathfrak{h}^*$。 模$Z(\lambda ) ($§6, no. 3）承认特征标是$\mathbf{Z}\langle P\rangle$的元素，我们有$d$。第 $Z(\lambda ) =e^{\lambda+\rho}$。

令$\alpha_1, . . . , \alpha_q$不同于元素或$R_+$。 $Z(\lambda ) ($§6 的$X_{-\alpha_1}^{n_1}X_{-\alpha_2}^{n_2}. . . X_{-\alpha_q}^{n_q}\otimes 1$ 形式基，第 6 (iii) 条提案）。对于$h\in \mathfrak{h}$，我们有

$$
h.(X_{-\alpha_1}^{n_1}X_{-\alpha_2}^{n_2}. . .X_{-\alpha_q}^{n_q}\otimes 1)
$$

$$
= [h, X_{-\alpha_1}^{n_1}. . . X_{-\alpha_q}^{n_q}]\otimes 1 + (X_{-\alpha_1}^{n_1}. . . X_{-\alpha_q}^{n_q})\otimes h.1
$$

$$
= (\lambda -n_1\alpha_1- \cdots  -n_q\alpha_q)(h)(X_{-\alpha_1}^{n_1}. . . X_{-\alpha_q}^{n_q}\otimes 1)
$$

因此，$Z(\lambda )^{\lambda-\mu}$的维数是$\mathfrak{P}(\mu)$。这证明 ch $Z(\lambda )$ 已定义，是 $\mathbf{Z}\langle P\rangle$ 的元素，并且

第 $Z(\lambda ) =\sum_\mu\mathfrak{P}(\mu)e^{\lambda-\mu}= Ke^{\lambda}$。

现在只需应用引理 1即可。

#### 引理 3 {#lie-viii-s9-lem-3 .statement tag=015V}

设 M 是一个 $\mathfrak{g}$ 模，它承认特征标 ch(M)，其支持包含在集合 $\mu-P_+$ 的有限并中。令U为$\mathfrak{g}$的包络代数，U$,\lambda_0\in \mathfrak{h}^*$的Z中心，以及从Z到$k($§8的$\chi_{\lambda_0}$相应的同态，Cor。 1 Th。 2）。假设对于所有 $z\in Z,z_M$ 都是位似，比率为 $\chi_{\lambda_0}(z)$。令$D_M$为$\lambda \in W(\lambda_0+\rho )-\rho$的集合，使得$\lambda + Q_+$满足Supp(ch M)。那么 ch(M) 是 ch $Z(\lambda )$ 对于 $\lambda \in D_M$ 的 $\mathbf{Z}$ 线性组合。

如果 Supp(ch M) 为空，则引理清零。假设 Supp(ch $M$)$\not=\emptyset$。令$\lambda$为该支撑的极大元素，并设置暗淡$M^{\lambda}=m$。从$(Z(\lambda ))^m$到M存在$\mathfrak{g}$同态$\varphi$，其中映射$(Z(\lambda )^{\lambda})^m$双射到$M^{\lambda}($§6, no. 3，命题6（i））。因此，$Z(\lambda )$的中心特征标是$\chi_{\lambda_0}$，所以$\lambda \in W(\lambda_0+\rho )-\rho ($§8, no. 5，Cor。 1 Th。 2）。这证明了$D_M\not=\emptyset$，并且允许我们通过卡$D_M$上的归纳进行争论。设L和N为$\varphi$的核和余核。那么我们有正合序列的 $\mathfrak{g}$ 同态：

$$
0\rightarrow L\rightarrow (Z(\lambda ))^m\rightarrow M\rightarrow N\rightarrow 0
$$

所以

ch(M) $=-$ch(L) $+m$ ch $Z(\lambda ) +$ ch(N)

（§7, no. 7，公式（6））。 集合 Supp(ch L) 和 Supp(ch N) 包含在集合 $\mu-P_+$ 的有限并中。对于 $z\in Z,z_L$ 和 $z_N$ 来说，是同位比 $\chi_{\lambda_0}(z)$。显然，$D_N\subset D_M$。另一方面，$(\lambda + Q_+)\cap$Supp(ch $M$)$=\{\lambda \}$和$\lambda  \notin$Supp(ch N)，所以$\lambda  \notin D_N$和

卡$D_N<$卡$D_M$。

另一方面，L是$(Z(\lambda ))^m$中的子模；如果 $\lambda '\in D_L$，则 $\lambda '+ Q_+$ 满足 Supp(ch $L$)$\subset$ Supp ch $Z(\lambda )$，因此 $\lambda \in \lambda '+ Q_+($§6, no. 1，命题 1 (ii))；由此可见$D_L\subset D_M$。从$L\cap (Z(\lambda )^{\lambda})^m= 0$开始，我们有$\lambda  \notin D_L$，所以

卡$D_L<$ 卡$D_M$。

现在申请归纳假设就足够了。

#### 定理 1（H. Weyl 的特征标公式）{#lie-viii-s9-thm-1 .statement tag=015W}

设 M 为有限维简单 $\mathfrak{g}$ 模，且 $\lambda$ 为最高权。然后

$(\sum_{w\in W}\varepsilon (w)e^{w\rho})$.ch $M =\sum_{w\in W}\varepsilon (w)e^{w(\lambda+\rho)}$.

当记号为引理 3 时，M 的中心特征标为 $\chi_{\lambda}($§6, no. 4，命题 7）。因此，通过引理 2 和 $3,d$.ch M 是 $e^{\mu+\rho}$ 的 $\mathbf{Z}$ 线性组合，使得

$$
\mu+\rho \in W(\lambda +\rho )
$$

另一方面，由 §7, no. 7，引理 $7,d$.ch M 是反不变的，其唯一的最大值项是 $e^{\lambda+\rho}$，因此是定理。

#### 例 {#lie-viii-s9-n1-exa-1 .statement tag=015X}

取$\mathfrak{g}=\mathfrak{s}\mathfrak{l}(2, k),\mathfrak{h}=kH$。令$\alpha$为$(\mathfrak{g},\mathfrak{h})$的根，使得$\alpha (H) = 2$。 $\mathfrak{g}$-模块$V(m)$有最高权$(m/2)\alpha$。因此

ch(V($m$)) $= (e^{(m/2)\alpha+^1_2\alpha}-e^{-(m/2)\alpha-^1_2\alpha})/(e^{^1_2\alpha}-e^{-^1_2\alpha})$

$$
=e^{-(m/2)\alpha}.(e^{(m+1)\alpha}-1)/(e^{\alpha}-1)
$$

$$
=e^{-(m/2)\alpha}(e^{m\alpha}+e^{(m-1)\alpha}+\cdots + 1)
$$

$$
=e^{(m/2)\alpha}+e^{(m-2)\alpha /2}+\cdots +e^{-(m/2)\alpha}
$$

这也很容易从§1, no. 2，提案 2 得出。

### 2. 维数简单 $\mathfrak{g}$ 模块

如果$\mu\in \mathfrak{h}^*$，则放入$J(e^\mu) =\sum_{w\in W}\varepsilon (w)e^{w\mu}$，cf. VI, §3, no. 3。

#### 定理 2 {#lie-viii-s9-thm-2 .statement tag=015Y}

设 E 为有限维简单 $\mathfrak{g}$ 模，$\lambda$ 为最高权，$(\cdot  | \cdot )$ 为 $\mathfrak{h}^*$ 上的 W 不变非简并正对称双线性形式。然后：

$$
\prod\langle \lambda +\rho , H_{\alpha}\rangle \prod((\lambda |\alpha ))
$$

昏暗E = = 1 +。

$$
_{\alpha\in R_+}\langle \rho , H_{\alpha}\rangle_{\alpha\in R_+}\overline{(\rho|\alpha)}
$$

设 T 为不定式。对于所有$\nu \in P$，用$f_{\nu}$同态表示从$\mathbf{Z}[P]$到$\mathbf{R}[[T]]$，对于所有$\mu\in P$需要$e^\mu$到$e^{(\nu|\mu)T}$。那么dim E就是级数$f_{\nu}$(ch E)的常数项。

对于所有$\mu, \nu \in P$，我们有

$$
f_{\nu}(J(e^\mu)) =\sum_{w\in W}\varepsilon (w)e^{(\nu|w\mu)T}
$$

$$
=\sum_{w\in W}\varepsilon (w)e^{(w^{-1}\nu|\mu)T}=f_\mu(J(e^{\nu}))
$$

特别是，鉴于第一章。 VI, §3, no. 3、公式 (3)、

$$
f_{\rho}(J(e^\mu)) =f_\mu(J(e^{\rho})) =e^{(\mu|\rho)T}\prod_{\alpha\in R_+}(1-e^{-(\mu|\alpha)T})
$$

因此，设定卡(R$_+$)$= N$，

$f_{\rho}(J(e^\mu))\equiv T^N\prod_{\alpha\in R}(\mu|\alpha )$（模$T^{N+1}\mathbf{R}[[T]]$）。

等式 $J(e^{\lambda+\rho}) =$ ch(E)$.J(e^{\rho})$ (Th.1) 因此意味着

$T^N\prod_{\alpha\in R_+}(\lambda +\rho |\alpha )\equiv f_{\rho}$(ch $E$)$.T^N\prod_{\alpha\in R_+}(\rho |\alpha )$ (mod $T^{N+1}\mathbf{R}[[T]]$)

所以

昏暗$E =((\prod_{\alpha\in R_+}(\lambda +\rho |\alpha ))/((\prod_{\alpha\in R_+}(\rho |\alpha ))=\prod_{\alpha\in R_+}(1 +\frac{(\lambda|\alpha)}{(\rho|\alpha)})$。

现在，如果$\alpha \in R_+,\alpha$可以与$\mathfrak{h}_{\mathbf{R}}$与$H_{\alpha}$成比例的元素识别，那么

$$
(\lambda +\rho |\alpha )/(\rho |\alpha ) =\langle \lambda +\rho , H_{\alpha}\rangle /\langle \rho , H_{\alpha}\rangle
$$

#### 例 1 {#lie-viii-s9-n2-exa-1 .statement tag=015Z}

在no. 1的例中，我们发现

昏暗$V(m) =(\frac{m}{2}\alpha +\frac{\alpha}{2})(H_{\alpha})/\frac{\alpha}{2}(H_{\alpha}) =m+ 1$，

我们在§1就知道了。

#### 例 2 {#lie-viii-s9-n2-exa-2 .statement tag=0160}

取$\mathfrak{g}$为型$G_2$的可分割简单李代数并采用第1章的记号。 VI，板IX。给出 $\mathfrak{h}^*_{\mathbf{R}}$ W 不变正对称形式 $(\cdot  | \cdot )$，使得 $(\alpha_1|\alpha_1) = 1$。然后 $\rho =\varpi_1+\varpi_2$ 和

$$
(\varpi_1|\alpha_1) =\frac{1}{2},(\varpi_1|\alpha_2) = 0,(\varpi_1|\alpha_2+\alpha_1) =\frac{1}{2}
$$

$$
(\varpi_1|\alpha_2+ 2\alpha_1) = 1,(\varpi_1|\alpha_2+ 3\alpha_1) =\frac{3}{2},(\varpi_1|2\alpha_2+ 3\alpha_1) =\frac{3}{2}
$$

$$
(\varpi_2|\alpha_1) = 0,(\varpi_2|\alpha_2) =\frac{3}{2},(\varpi_2|\alpha_2+\alpha_1) =\frac{3}{2}
$$

$$
(\varpi_2|\alpha_2+ 2\alpha_1) =\frac{3}{2},(\varpi_2|\alpha_2+ 3\alpha_1) =\frac{3}{2},(\varpi_2|2\alpha_2+ 3\alpha_1) = 3
$$

因此，如果$n_1, n_2$是整数$\geq 0$，则最高权$n_1\varpi_1+n_2\varpi_2$的简单表示的维数是

$$
(1 +\frac{n_1/2}{1\overline{2}})((1 +\frac{3n_2/2}{3\overline{2}})((1 +\frac{n_1/2 + 3n_2/2}{_{1\overline{2}} + \frac{3}{2}})((1 +\frac{n_1 + 3n_2/2}{1 +^{3\overline{2}}})
$$

$$
\times (1 +\frac{3n_1/2 + 3n_2/2}{_{3\overline{2}} + \frac{3}{2}})((1 +3n_1\frac{/_3}{2}2 + 3+ 3n_2)
$$

$$
= (1 +n_1)(1 +n_2)(1 +\frac{n_1 + 3n_2}{4})((1 +\frac{2n_1 + 3n_2}{5})((1 +\frac{n_1 + n_2}{2})
$$

$$
\times (1 +\frac{n_1 + 2n_2}{3})
$$

$$
(1+n_1)(1+n_2)(2+n_1+n_2)(3+n_1+2n_2)(4+n_1+3n_2)(5+2n_1+3n_2)
$$

=。

5！

特别是，最高权 $\varpi_1$（分别为$\varpi_2$）的基数表示为维数 7（分别为14）。

### 3. 简单 $\mathfrak{g}$ 模块的权的多重性

#### 命题 1 {#lie-viii-s9-prop-1 .statement tag=0161}

让$\omega \in P_{++}$。对于所有$\lambda \in P$，$E(\omega )$中$\lambda$的重数是

$$
m_{\lambda}=\sum_{w\in W}\varepsilon (w)\mathfrak{P}(w(\omega +\rho )-(\lambda +\rho ))
$$

由 Th. 1 和引理 1，

通道 $E(\omega ) = Ke^{-\rho}d$ 通道 $E(\omega ) = Ke^{-\rho}\sum_{w\in W}\varepsilon (w)e^{w(\omega+\rho)}$

所以

通道 $E(\omega ) =\sum_{w\in W,\gamma\in Q_+}\varepsilon (w)\mathfrak{P}(\gamma )e^{-\rho+w(\omega+\rho)-\gamma}$

和

$$
m_{\lambda}=\sum\varepsilon (w)\mathfrak{P}(\gamma )
$$

$w\in W,\gamma \in Q_+,\gamma =-\lambda -\rho +w(\omega +\rho )$

#### 推论{#lie-viii-s9-n3-cor-1 .statement tag=0162}

如果$\lambda$是$E(\omega )$的权，与$\omega$不同，

$$
m_{\lambda}=-\sum_{w\in W,w\not=1}\varepsilon (w)m_{\lambda+\rho-w\rho}
$$

使用 $\omega = 0$ 应用命题 1。如果 $\mu\in P$**--** $\{0\}$，我们发现

$$
0 =\sum_{w\in W}\varepsilon (w)\mathfrak{P}(w\rho +\mu-\rho )
$$

因此

$$
\mathfrak{P}(\mu) =-\sum_{w\in W,w\not=1}\varepsilon (w)\mathfrak{P}(\mu+w\rho -\rho ) \tag{1}
$$

命题 1 还给出

$$
m_{\lambda}=-\sum_{w\in W}\varepsilon (w)\sum_{w'\in W,w'\not=1}\varepsilon (w')\mathfrak{P}(w(\omega +\rho )-(\lambda +\rho ) +w'\rho -\rho )
$$

从 $w(\omega +\rho )\not=\lambda +\rho$ 开始，对于所有 $w\in W ($§7，提案 5 (iii)）。因此，

$$
m_{\lambda}=-\sum_{w'\in W,w'\not=1}\varepsilon (w')\sum_{w\in W}\varepsilon (w)\mathfrak{P}(w(\omega +\rho )-(\lambda +\rho -w'\rho +\rho ))
$$

$=-\sum_{w'\in W,w'\not=1}\varepsilon (w')m_{\lambda+\rho-w'\rho}$（提案$.1$）。

### 4. 分解张量积简单 $\mathfrak{g}$ 模块

#### 命题 2 {#lie-viii-s9-prop-2 .statement tag=0163}

让$\lambda , \mu\in P_{++}$。在 $\mathscr{R}(\mathfrak{g})$ 中，我们有

$$
[\lambda ].[\mu] =\sum_{\nu\in P_{++}}m(\lambda , \mu, \nu )[\nu ]
$$

和

$$
m(\lambda , \mu, \nu ) =\sum_{w,w'\in W}\varepsilon (ww')\mathfrak{P}(w(\lambda +\rho ) +w'(\mu+\rho )-(\nu + 2\rho ))
$$

令$E,F$为最高权$\lambda , \mu$的有限维简单$\mathfrak{g}$模。令$l_{\nu}$为最高权$\nu$的$E\otimes F$同型成分的长度。足以证明

$$
l_{\nu}=\sum_{w,w'\in W}\varepsilon (ww')\mathfrak{P}(w(\lambda +\rho ) +w'(\mu+\rho )-(\nu + 2\rho )) \tag{2}
$$

放入 $c_1=$ ch(E) $=\sum_{\sigma\in P}m_{\sigma}e^{\sigma},c_2=$ ch(F) 和 $d= J(e^{\rho})$，其中 J 的定义如 no. 2 中所示。我们有 $\sum_{\xi\in P_{++}}l_{\xi}$ch[$\xi ] =$ ch(E $\otimes F$) $=c_1c_2$

因而，之后乘以 $d$ 并使用 Th。 1、

$$
\sum_{\xi\in P_{++}}l_{\xi}J(e^{\xi+\rho}) =c_1J(e^{\mu+\rho}) =(\sum_{\sigma\in P}m_{\sigma}e^{\sigma})((\sum_{w\in W}\varepsilon (w)e^{w(\mu+\rho)}) \tag{3}
$$

$$
=\sum_{\tau\in P}(\sum_{w\in W}\varepsilon (w)m_{\tau+\rho-w(\mu+\rho)})e^{\tau+\rho}
$$

现在，如果 $\xi \in P_{++},\xi +\rho$ 属于到 B 定义的腔室（第 VI, §1, no. 10）；因而，对于所有不同于 1 的 $w\in W$，我们有 $w(\xi +\rho )\notin P_{++}$。因而，$\sum_{\xi\in P_{++}}l_{\xi}J(e^{\xi+\rho})$中$e^{\nu+\rho}$的系数等于$l_{\nu}$。鉴于(3)，我们得到

$$
l_{\nu}=\sum_{w\in W}\varepsilon (w)m_{\nu+\rho-w(\mu+\rho)}
$$

也就是说，根据命题 1，

$$
l_{\nu}=\sum_{w,w'\in W}\varepsilon (w)\varepsilon (w')\mathfrak{P}(w'(\lambda +\rho )-(\nu +\rho -w(\mu+\rho ) +\rho ))
$$

这就证明了(2)。

#### 例 {#lie-viii-s9-n4-exa-1 .statement tag=0164}

我们回到no. 1的例。让 $\lambda = (n/2)\alpha , \mu= (p/2)\alpha$、$\nu = (q/2)\alpha$ 与 $n\geq p$。我们有

$$
m(\lambda , \mu, \nu ) =\mathfrak{P}(\frac{n}{2}\alpha +\frac{\alpha}{2}+\frac{p}{2}\alpha +\frac{\alpha}{2}-\frac{q}{2}\alpha -\alpha )
$$

$$
-\mathfrak{P}(\frac{n}{2}\alpha +\frac{\alpha}{2}-\frac{p}{2}\alpha -\frac{\alpha}{2}-\frac{q}{2}\alpha -\alpha )
$$

$$
-\mathfrak{P}(-\frac{n}{2}\alpha -\frac{\alpha}{2}+\frac{p}{2}\alpha +\frac{\alpha}{2}-\frac{q}{2}\alpha -\alpha )
$$

$$
+\mathfrak{P}(-\frac{n}{2}\alpha -\frac{\alpha}{2}-\frac{p}{2}\alpha -\frac{\alpha}{2}-\frac{q}{2}\alpha -\alpha )
$$

$$
=\mathfrak{P}(\frac{n + p-q}{2}\alpha )-\mathfrak{P}(\frac{n-p-q- 2}{2}\alpha )
$$

如果 $n+p+q$ 不能被 2 整除，或者 $q\geq n+p$，则为零。如果

$$
q=n+p-2r
$$

对于 $r$ 整数 $\geq 0$，我们有

$$
m(\lambda , \mu, \nu ) =\mathfrak{P}(r\alpha )-\mathfrak{P}((r-p-1)\alpha )
$$

因此如果$r\leq p$则为$m(\lambda , \mu, \nu ) = 1$，如果$r > p$则为$m(\lambda , \mu, \nu ) = 0$。最后，$\mathfrak{g}$-模块$V(n)\otimes V(p)$同构于

$$
V(n+p)\oplus V(n+p-2)\oplus V(n+p-4)\oplus  \cdots  \oplus V(n-p)
$$

（克莱布什-戈登公式）。

### 习题 {#lie-viii-s9-exercises}

所有考虑的 $\mathfrak{g}$ 模块都被假定为有限维。

参见[习题为 § 9](exercises/s9/)。
