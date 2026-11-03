---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 12
section_title: Chevalley orders
lang: zh
source: lie-vii-ix
book_pages: 173-189
pdf_pages: 0181-0197
extraction: native
subsections:
    - "no": 1
      title: LATTICES AND ORDERS
      page: 173
      pdf_page: 181
    - "no": 2
      title: DIVIDED POWERS IN A BIGEBRA
      page: 173
      pdf_page: 181
    - "no": 3
      title: INTEGRAL VARIANT OF THE POINCARÉ-BIRKHOFF-WITT THEOREM
      page: 174
      pdf_page: 182
    - "no": 4
      title: 'EXAMPLE: POLYNOMIALS WITH INTEGER VALUES'
      page: 176
      pdf_page: 184
    - "no": 5
      title: SOME FORMULAS
      page: 178
      pdf_page: 186
    - "no": 6
      title: BIORDERS IN THE ENVELOPING ALGEBRA OF A SPLIT REDUCTIVE LIE ALGEBRA
      page: 180
      pdf_page: 188
    - "no": 7
      title: CHEVALLEY ORDERS
      page: 185
      pdf_page: 193
    - "no": 8
      title: ADMISSIBLE LATTICES
      page: 187
      pdf_page: 195
statements: 34
exercises: 0
content_sha256: dd536d90056f253586449c49abcdb0fa8afd4317619c6f4a5a3faa6a2fb95098
translated_from: content/en/lie/VIII/12_s12_chevalley_orders.md
translation_method: google
source_content_sha256: 50f43a34a9ae42cb38e10e1f32022dc1fddb5d2b07911570fec5baa09a40ebdf
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 6d3cd832bd199ea8836375111a20e6ce22d414dbf65905dbbe9429b1dca76586
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 12。 Chevalley 阶

### 1. 格与序

令V为$\mathbf{Q}$向量空间。 A lattice in V is a free $\mathbf{Z}$-submodule $\mathscr{V}$ of V such that the $\mathbf{Q}$-linear 映射 $\alpha_{\mathscr{V},V}:\mathscr{V}\otimes_{\mathbf{Z}}\mathbf{Q}\rightarrow V$ induced by 单射 of $\mathscr{V}$ into V is bijective. When V is finite dimensional, this is the same as 说 that $\mathscr{V}$ is a $\mathbf{Z}$-submodule of finite 型 which 生成 the $\mathbf{Q}$-vector space V (recall that a torsion-free $\mathbf{Z}$-module of finite 型代数免费，VII, §4, no. 4，第 2 章）；此外，在这种情况下，我们的定义是第1章交换代数的特例。 VII, §4, no. 1，防御。 1（前述，例 3）。如果W是V的向量子空间，且$\mathscr{V}$是V中的格子，则$\mathscr{V}\cap W$是W中的格子。

If V is a $\mathbf{Q}$-algebra, 阶 in V is a lattice $\mathscr{V}$ in the underlying 向量空间 that is a $\mathbf{Z}$-subalgebra of V; 映射 $\alpha_{\mathscr{V},V}$ 则为 $\mathbf{Q}$ 代数的同构。如果V是单位$\mathbf{Q}$代数，则V中的单位阶是V包含单位元中的阶。

假设 V 是一个 $\mathbf{Q}$-bigebra，具有余积 $c$ 和余单位 $\gamma$。如果$\mathscr{V}$是向量空间V中的格，则规范的映射$i:\mathscr{V}\otimes_{\mathbf{Z}}\mathscr{V}\rightarrow V\otimes_{\mathbf{Q}}V$是单射的； V中的双序是单位代数V中的单位阶$\mathscr{V}$，使得$\gamma (\mathscr{V})\subset \mathbf{Z}$和$c(\mathscr{V})\subset i(\mathscr{V}\otimes_{\mathbf{Z}}\mathscr{V})$； 映射

$\gamma_{\mathscr{V}}:\mathscr{V}\rightarrow \mathbf{Z}$ 和 $c_{\mathscr{V}}:\mathscr{V}\rightarrow \mathscr{V}\otimes_{\mathbf{Z}}\mathscr{V}$

由$\gamma$和$c$诱导给出$\mathbf{Z}$-bigebra的$\mathscr{V}$结构，映射$\alpha_{\mathscr{V},V}$则为$\mathbf{Q}$-bigebra的同构。

### 2. 双代数中的分次幂

设 A 为单位 $k$ 代数，$x\in A,d\in k,n\in \mathbf{N}$。放

$$
x(x-d). . .(x-d(n-1))^{n-1}
$$

$$
x^{(n,d)}==\prod(x-id)/(i+ 1) \tag{1}
$$

$n$！

$i=0$

In particular, $x^{(0,d)}= 1,x^{(1,d)}=x$.我们同意 $x^{(n,d)}= 0$ 对应 $n$ 整数 $<0$。放

$x^{(n)}=x^{(n,0)}=xn^n$! (2)

$(nx)=x^{(n,1)}=x(x-1). . .n($！$x-n+ 1)$。 (3)

#### 命题 1 {#lie-viii-s12-prop-1 .statement tag=017V}

设 A 是一个大数，其中余积 $c$，并且 $x$ 是 A 的原语元素（第 II, §1, no. 2）。那么

$$
c(x^{(n,d)}) =\sum x^{(p,d)}\otimes x^{(q,d)} \tag{4}
$$

$p\in \mathbf{N},q\in \mathbf{N},p+q=n$

命题对于 $n\leq 0$ 来说是微不足道的。我们以归纳对$n$争论。如果公式 (4) 对于 $n$ 为真，则

$$
(n+ 1)c(x^{(n+1,d)}) =c(x-dn)c(x^{(n,d)})
$$

$$
= (x\otimes 1 + 1\otimes x-dn1\otimes 1)c(x^{(n,d)})
$$

$$
=\sum_{p+q=n}[xx^{(p,d)}\otimes x^{(q,d)}+x^{(p,d)}\otimes xx^{(q,d)}-(p+q)dx^{(p,d)}\otimes x^{(q,d)}]
$$

$$
=\sum_{p+q=n}(x-pd)x^{(p,d)}\otimes x^{(q,d)}+\sum_{p+q=n}x^{(p,d)}\otimes (x-qd)x^{(q,d)}
$$

$$
=\sum_{p+q=n}(p+ 1)x^{(p+1,d)}\otimes x^{(q,d)}+\sum_{p+q=n}(q+ 1)x^{(p,d)}\otimes x^{(q+1,d)}
$$

$$
=\sum_{r+s=n+1}rx^{(r,d)}\otimes x^{(s,d)}+\sum_{r+s=n+1}sx^{(r,d)}\otimes x^{(s,d)}
$$

$$
= (n+ 1)\sum_{r+s=n+1}x^{(r,d)}\otimes x^{(s,d)}
$$

因此公式 (4) 代表$n+ 1$。

### 3. Integral variant of the poincarÉ-birkhoff-witt 定理

Let $\mathfrak{g}$ be a finite dimensional $\mathbf{Q}$-Lie algebra, $U(\mathfrak{g})$ its enveloping bigebra. If I is 全序集, $\mathbf{x}= (x_i)_{i\in I}$ a family of 元素 of $\mathfrak{g}$, and $\mathbf{n}=$ $(n_i)_{i\in I}\in \mathbf{N}^{(I)}$ a multi-index, put

$\mathbf{x}^{(\mathbf{n})}=\prod x\overset{ni}{n_{i}}$！$^{^i}$, (5)

$i\in I$

乘积 being calculated in $U(\mathfrak{g})$ in accordance with the ordered 集合 I.

#### 定理 1 {#lie-viii-s12-thm-1 .statement tag=017W}

Let $\mathscr{U}$ be 双序 in the bigebra $U(\mathfrak{g})$. Let $\mathscr{G}=\mathscr{U}\cap \mathfrak{g}$, which is 阶 in 李代数 $\mathfrak{g}$.设$(x_i)_{i\in I}$为$\mathscr{G}$的基。给I总共阶，并假设对于所有$\mathbf{n}\in \mathbf{N}^I$，元素$[\mathbf{n}]$为$\mathscr{U}$，这样$[\mathbf{n}]-\mathbf{x}^{(\mathbf{n})}$在$U(\mathfrak{g})$中有过滤$<|\mathbf{n}|$。那么，$\mathbf{n}\in \mathbf{N}^I$的$[\mathbf{n}]$家族是$\mathbf{Z}$模块$\mathscr{U}$的基。

For $p\in \mathbf{N}$, let $U_p(\mathfrak{g})$ be 集合 of 元素 of $U(\mathfrak{g})$ of filtration $\leq p$;然后像在 $\mathbf{x}^{(\mathbf{n})}$ 的 $U_p(\mathfrak{g})/U_{p-1}(\mathfrak{g})$ 中，使得这个 $\mathbf{Q}$ 向量空间的 $|\mathbf{n}|=p$ 形式基 （第 I, §2, no. 7，第 1 章）； hence the $[\mathbf{n}]$ 形式基 of the $\mathbf{Q}$-vector space $U(\mathfrak{g})$. It remains to prove the following 断言 (in which we put $M =\mathbf{N}^I$)$:$

(*) if $u\in \mathscr{U}, (a_{\mathbf{n}})\in \mathbf{Z}^{(M)}$, and $d\in$ **N --**$\{0\}$ are such that

$$
du=\sum_{\mathbf{n}\in M}a_{\mathbf{n}}[\mathbf{n}] \tag{6}
$$

然后$d$除各$a_{\mathbf{n}}$。

对于每个整数$r\geq 0$，引入迭代的余积

$$
c_i:\mathscr{U}\rightarrow \mathbf{T}^r(\mathscr{U}) =\mathscr{U}\otimes \mathscr{U}\otimes  \cdots  \otimes \mathscr{U}
$$

by 定义, $c_0$ is 余单位 of $\mathscr{U},c_1=$ Id$_{\mathscr{U}},c_2=c$ (余积 of $\mathscr{U}$), and, for $r\geq 2,c_{r+1}$ is defined as the composite $p\circ (c_r\otimes 1)\circ c:$

$$
\mathscr{U}\longrightarrow^c\mathscr{U}\otimes_{\mathbf{Z}}\mathscr{U}^c\longrightarrow^{^r\otimes 1}\mathbf{T}^r(\mathscr{U})\otimes_{\mathbf{Z}}\mathscr{U}\longrightarrow^p\mathbf{T}^{r+1}(\mathscr{U})
$$

其中$p$是通过在代数$\mathbf{T}(\mathscr{U})$中使用乘法来定义的。此外，考虑$\mathscr{U}$到$\mathscr{U}^+=$ Ker $c_0$的规范投影$\pi$，以及复合

$$
c^+_r=\mathbf{T}^r(\pi )\circ c_r:\mathscr{U}\rightarrow \mathbf{T}^r(\mathscr{U}^+)
$$

#### 引理 1 {#lie-viii-s12-lem-1 .statement tag=017X}

让$\mathbf{n}\in \mathbf{N}^I$。如果$|\mathbf{n}|< r$，则$c^+_r([\mathbf{n}]) = 0$。如果$|\mathbf{n}|=r$，那么

$$
c^+_r([\mathbf{n}]) =\sum_{\varphi}x_{\varphi(1)}\otimes x_{\varphi(2)}\otimes  \cdots  \otimes x_{\varphi(r)} \tag{7}
$$

其中从$\{1,2, . . . , r\}$到I的映射中的$\varphi$属于到集合，各需要值$i\in In_i$次。

根据命题 1，

$$
c_r(\mathbf{x}^{(\mathbf{n})}) =\sum\mathbf{x}^{(\mathbf{p}_1)}\otimes  \cdots  \otimes \mathbf{x}^{(\mathbf{p}_r)}
$$

其中 M 的 $r$ 元素的序列 $(\mathbf{p}_1, . . . ,\mathbf{p}_r)$ 的扩展与集合之和，使得 $\mathbf{p}_1+\cdots +\mathbf{p}_r=\mathbf{n}$。鉴于章。 II, §1, no. 3，第 6 条命题，映射 $c^+_r$，从 $U(\mathfrak{g})$ 到 $\mathbf{T}^r(U^+(\mathfrak{g}))$ 通过线性扩展至映射，在 $U_{r-1}(\mathfrak{g})$ 上消失。由此可见，对于$r\geq  |\mathbf{n}|$，

$$
c^+_r([\mathbf{n}]) =c^+_r(\mathbf{x}^{(\mathbf{n})}) =\sum\pi (\mathbf{x}^{(\mathbf{p}_1)})\otimes  \cdots  \otimes \pi (\mathbf{x}^{(\mathbf{p}_r)}) \tag{8}
$$

对于$r >|\mathbf{n}|$，关系$\mathbf{p}_1+\cdots +\mathbf{p}_r=\mathbf{n}$意味着$\mathbf{p}_i$中至少有一个是零，所以$c^+_r([\mathbf{n}]) = 0$。对于 $r=|\mathbf{n}|$，(8) 的第三个成员的唯一非零项是那些 $|\mathbf{p}_1|=\cdots =|\mathbf{p}_r|= 1$，因此是 (7)。

我们回到Th的证明。 1. 我们保留(*)的记号，并通过$|\mathbf{n}|$降序归纳，证明$d$除$a_{\mathbf{n}}$，当$|\mathbf{n}|$为足够大时，这是清楚的。如果 $d$ 除 $a_{\mathbf{n}}$ 对于 $|\mathbf{n}|> r$ 那么，把

$$
u'=u-\sum_{|\mathbf{n}|>r}(a_{\mathbf{n}}/d)[\mathbf{n}]\in \mathscr{U}
$$

我们有

$$
du'=\sum_{|\mathbf{n}|\leq r}a_{\mathbf{n}}[\mathbf{n}] \tag{9}
$$

对于从 $\{1,2, . . . , r\}$ 到 I 的任意映射 $\varphi$，将

$$
e_{\varphi}=x_{\varphi(1)}\otimes  \cdots  \otimes x_{\varphi(r)}
$$

和$a_{\varphi}=a_{\mathbf{n}}$，其中$\mathbf{n}=$（卡$\varphi^{-1}(i)$）$_{i\in I}$。由引理 1，(9) 意味着

$$
dc^+_r(u') =\sum_{\varphi\in I^r}a_{\varphi}e_{\varphi} \tag{10}
$$

所以$c^+_r(u')\in \mathbf{T}^r(\mathscr{U}^+)\cap \mathbf{Q}\mathbf{T}^r(\mathscr{G})$。但$\mathscr{U}^+$的子模$\mathscr{G}$是直因子（代数，第VII, §4, no. 3章，第1章的Cor.），所以子模$\mathbf{T}^r(\mathscr{G})$是$\mathbf{T}^r(\mathscr{U}^+)$的直因子，因此$c^+_r(u')\in \mathbf{T}^r(\mathscr{G})$。另一方面，$\mathscr{G}$的$x_i$形式基除以假设，因此$\mathbf{T}^r(\mathscr{G})$的$e_{\varphi}$形式基。那么(10)证明$d$除$a_{\varphi}$，即$a_{\mathbf{n}}$对应$|\mathbf{n}|=r$。这就证明了(*)。

### 4. 例：具有整数值的多项式

令 V 为有限维$\mathbf{Q}$向量空间，$V^*$其对偶，$\mathscr{V}$V中的格，$\mathscr{V}^*$$\mathscr{V}$的对偶$\mathbf{Z}$-模，可以用$V^*,\mathbf{S}(V)$对称矩阵中的格规范地识别代数 / V，以及

$$
\lambda :\mathbf{S}(V)\rightarrow A(V^*)
$$

从 $\mathbf{S}(V)$ 到$V^*($代数上多项式函数代数的正则双射，第 1 章IV, §5, no. 11，备注1)。 如果我们将认同 $A(V^*\times V^*)$ 与 $A(V^*)\otimes_{\mathbf{Q}}A(V^*)$ 组合，则将 $\mathbf{S}(V)$ 的 $\lambda$ 变换余积转换为映射 $A(V^*)\rightarrow A(V^*\times V^*)$，并与 $V^*$ 上的多项式函数 $\varphi$ 相关联多项式函数

$$
(x, y) \rightarrow \varphi (x+y)
$$

$V^*\times V^*($代数，第 1 章IV, §5, no. 11、注2)。

用元素$\mathbf{S}(V)$由……组成$(^{\mathscr{V}}_{\mathbf{Z}})$子集表示，其中$\mathscr{V}^*$上取整数值的对应到多项式映射从$V^*$到$\mathbf{Q}$。

#### 命题 2 {#lie-viii-s12-prop-2 .statement tag=017Y}

(i) $(^{\mathscr{V}}_{\mathbf{Z}})$ 是大数$\mathbf{S}(V)$ 中的双序，以及$(^{\mathscr{V}}_{\mathbf{Z}})\cap V =\mathscr{V}$。

(ii) $\mathbf{Z}$-代数$(^{\mathscr{V}}_{\mathbf{Z}})$由$h\in \mathscr{V}, n\in \mathbf{N}$的$(^h_n)$生成。

(iii) 如果$(h_1, . . . , h_r)$是$\mathscr{V}$中的基，则元素

$$
(h)(h_1)(h_r)
$$

= $\cdots$,

$$
\mathbf{n}n_1n_r
$$

其中$\mathbf{Z}$模块$(^{\mathscr{V}}_{\mathbf{Z}})$的$\mathbf{n}= (n_1, . . . , n_r)$属于到$\mathbf{N}^r$、形式基。

对于$m\in \mathbf{N}$，输入$\mathbf{S}_m(V) =\sum_{i\leq m}\mathbf{S}^i$(V)、$\mathbf{S}_m(\mathscr{V}) =\sum_{i\leq m}\mathbf{S}^i(\mathscr{V})$。 代数，第 1 章IV, §5, no. 9、第 15 号提案和注、

$\mathbf{S}_m(\mathscr{V})\subset \mathbf{S}_m(V)\cap (\mathscr{V}\mathbf{Z})\subset m1$！$\mathbf{S}_m(\mathscr{V})$

所以$(^{\mathscr{V}}_{\mathbf{Z}})\cap V =\mathscr{V}$。由于$\mathbf{S}_m(\mathscr{V})$是$\mathbf{S}_m$(V)中的格，$\mathbf{S}_m(V)\cap (_{\mathbf{Z}}^{\mathscr{V}})$也是$\mathbf{S}_m(V)$中的格。另一方面，$\mathbf{S}_m(V)\cap (^{\mathscr{V}}_{\mathbf{Z}})$是$\mathbf{S}_{m+1}(V)\cap (_{\mathbf{Z}}^{\mathscr{V}})$的直因子（因为商是无扭转的），因此它承认一个补集，它是一个自由的$\mathbf{Z}$模。由此可见 $(^{\mathscr{V}}_{\mathbf{Z}})$ 是一个免费的 $\mathbf{Z}$ 模块。很明显，这是代数$\mathbf{S}(V)$中的一个单位阶。令$(u_n)_{n\in\mathbf{N}}$为$\mathbf{Z}$模块$(^{\mathscr{V}}_{\mathbf{Z}})$的基。这也是$\mathbf{Q}$模块$\mathbf{S}(V)$的基，并且对于所有

$$
\varphi \in \mathbf{S}(V\times V) =\mathbf{S}(V)\otimes_{\mathbf{Q}}\mathbf{S}(V)
$$

存在$\mathbf{S}(V)$ 的元素的唯一序列 $(v_n)$ 使得$\varphi =\sum u_n\otimes v_n$。如上，认同$\mathbf{S}(V)$与$A(V^*)$以及$\mathbf{S}(V)\otimes \mathbf{S}(V)$与$A(V^*\times V^*)$。如果 $\varphi \in (^{\mathscr{V}\times\mathscr{V}}_{\mathbf{Z}})$、多项式函数 $x \rightarrow \varphi (x, y)$ 属于至 $(^{\mathscr{V}}_{\mathbf{Z}})$ 对于所有 $y\in \mathscr{V}^*$。由此可见，对于所有$n$和所有$y\in \mathscr{V}^*$，$v_n(y)\in \mathbf{Z}$，对于其他字，对于$v_n\in (^{\mathscr{V}}_{\mathbf{Z}})$。这就证明了余积映射$(^{\mathscr{V}}_{\mathbf{Z}})$到$(_{\mathbf{Z}}^{\mathscr{V}})\otimes_{\mathbf{Z}}(_{\mathbf{Z}}^{\mathscr{V}})$。如果$h\in \mathscr{V}$和$n\in \mathbf{N}$，则$(_n^h)$映射$u\in \mathscr{V}^*$到整数$(^{u(h)}_n)$，所以$(^h_n)\in (_{\mathbf{Z}}^{\mathscr{V}})$。 断言 (iii) 现在由应用 Th 获得。 1 到交换律李代数 V，并且 (ii) 如下。

#### 推论 {#lie-viii-s12-n4-cor-1 .statement tag=017Z}

令 X 为不定式。多项式$(^X_n)$，其中多项式$P\in k[X]$的$\mathbf{Z}$模由……组成的$n\in \mathbf{N}$、形式基使得$P(\mathbf{Z})\subset \mathbf{Z}$。

如果$P(\mathbf{Z})\subset \mathbf{Z}$，拉格朗日插值公式（代数，第IV, §2, no. 1，第6章）表明P属于到$\mathbf{Q}$的系数；因此，我们可以假设 $k=\mathbf{Q}$ 并将命题 2 应用于 $V =\mathbf{Q},\mathscr{V}=\mathbf{Z}$。

### 5. 一些公式

在这个数中，A表示单位结合词代数。如果$x\in A$，我们写广告$x$而不是广告$_Ax$。

#### 引理 2 {#lie-viii-s12-lem-2 .statement tag=0180}

如果$x, y\in A$和$n\in \mathbf{N}$，

（广告$nx$！）$^ny=\sum(-1)^qxp^p$！ $yxq^q$！ =$\sum(-1)^qx^{(p)}yx^{(q)}$。 (11)

$p+q=np+q=n$

事实上，如果我们用 $L_x$ 和 $R_x$ 映射 $z \rightarrow xz$ 和 $z \rightarrow zx$ 表示从 A 到 A，我们有，因为 $L_x$ 和 $R_x$ 通勤，

$n1$！（广告$x$）$^n=n1$！$(L_x-R_x)^n=\sum_{p+q=n}(-1)^qp1$！ $L^p_xq1$！ $R^q_x$。

#### 引理 3 {#lie-viii-s12-lem-3 .statement tag=0181}

令 $x, h\in A$ 和 $\lambda \in k$ 满足 (ad $h$)$x=\lambda x$。对于所有 $n\in \mathbf{N}$ 和所有 $P\in k[X]$，我们有

$$
P(h)x^{(n)}=x^{(n)}P(h+n\lambda ) \tag{12}
$$

由于 ad $h$ 是 A 的推导并且由于 (ad $h$)$x$ 与 $x$ 通勤，我们有

（广告$h$）$x^n=nx^{n-1}$（（广告$h$）$x$）$=n\lambda x^n$，（13）所以

（广告$h$）$x^{(n)}=n\lambda x^{(n)}$。

因此，公式 (12) 由特殊情况得出

$$
P(h)x=xP(h+\lambda ) \tag{14}
$$

替换 $x$ $x^{(n)}$ 和 $\lambda$ $n\lambda$。只要在$P = X^m$时证明(14)，在$m$上通过归纳就可以了。 $m= 0,1$时就清楚了。如果 (14) 对于 $P = X^m$ 成立，则

$$
h^{m+1}x=h.h^mx=hx(h+\lambda )^m=x(h+\lambda )^{m+1}
$$

这就证明了(12)。

#### 引理 4 {#lie-viii-s12-lem-4 .statement tag=0182}

令 $x, y, h\in A$ 为

$$
[y, x] =h,[h, x] = 2x,[h, y] =-2y \tag{15}
$$

(i) 对于 $m, n\in \mathbf{N}$，我们有

$$
_{(n)(m)}\sum_{(m-p)}(m+n-p-1-h)_{(n-p)}
$$

$xy$ = $yx$。 (16)

$$
p
$$

$p\geq 0$

(ii) 设 $A'$ 为 A 的 $\mathbf{Z}$ 子代数，由 $x^{(m)}$ 和 $m\in \mathbf{N}$ 的 $y^{(m)}$ 生成。然后 $(^h_n)\in A'$ 对于所有 $n\in \mathbf{N}$。

公式 (16) 可以写成等价的形式

$$
_{(n)(m)}\sum_{(m-p)}(m+n-p-1-h)_{(n-p)}
$$

（广告$x$）$y$ = $yx.(17_m)$

$$
p
$$

$p\geq 1$

这对于 $m= 0$ 来说是微不足道的。我们通过归纳对$m$进行争论。从$(17_m)$，我们得到

$(m+$ 1)(广告 $x^{(n)}$)$y^{(m+1)}=$ (广告 $x^{(n)}$)$y^{(m)}.y+y^{(m)}$。(广告 $x^{(n)}$)$y$ (18)

$$
_{(m-p)}(m+n-p-1-h)_{(n-p)(m)}-
$$

$$
=\sum yxy+y(n-1-h)x^{(n1)}
$$

$$
p
$$

$p\geq 1$

（§1, no. 1，引理1）。现在，应用相同的引理，然后是引理3，

我们有

$$
(m+n-p-1-h)_{(n-p)}
$$

$$
xy
$$

$$
p
$$

$$
(m+n-p-1-h)_{(n-p)}-_-
$$

=$(yx+ (n-p-1-h)x^{(np1)})$

$$
p
$$

$$
(m+n-p+ 1-h)_{(n-p)}
$$

$$
=yx
$$

$$
p
$$

$$
(m+n-p-1-h)_{--}
$$

+ $(n-p-1-h)x^{(np1)}$。

$$
p
$$

将其代入式(18)，我们得到

$(m+$ 1)(广告$x^{(n)}$)$y^{(m+1)}$

$$
_-(m+n-p+ 1-h)_-
$$

$$
=\sum(m-p+ 1)y^{(mp+1)}x^{(np)}
$$

$$
p
$$

$p\geq 1$

$$
_-(m+n-p-1-h)_{--}
$$

$+\sum y^{(mp)}(n-p-1-h)x^{(np1)}$

$$
p
$$

$p\geq 1$

$$
+y^{(m)}(n-1-h)x^{(n-1)}
$$

$$
_-(m+n-p+ 1-h)_-
$$

$=\sum(m-p+ 1)y^{(mp+1)}x^{(np)}$

$$
p
$$

$p\geq 1$

$$
_{(m-p)}(m+n-p-1-h)_{--}
$$

$+\sum y(n-p-1-h)x^{(np1)}$。

$$
p
$$

$p\geq 0$ Changing $p$ to $p-1$ in the second sum, and regrouping the terms, we obtain

$(m+$ 1)(广告 $x^{(n)}$)$y^{(m+1)}=\sum_{p\geq 1}y^{(m-p+1)}A_px^{(n-p)}$ (19)

和

$$
(m+n-p+ 1-h)(m+n-p-h)
$$

$A_p= (m-p+ 1)+ (n-p-h)$。

$$
pp-1
$$

代入$z=m+n-p-h$，也可以写成

$A_p=p1$！$(m-p+ 1)(z+ 1)z(z-1). . .(z-p+ 2)$

+ 1 $(z-m)z(z-1). . .(z-p+ 2)$

$(p-$1）！

$=p1$！ $z(z-1). . .(z-p+ 2)[(m-p+ 1)(z+ 1) +p(z-m)]$

$$
(z)((m+ 1) +n-p-1-h)
$$

$$
= (m+ 1)= (m+ 1)
$$

$$
pp
$$

将其代入 (19)，我们得到 $(17_{m+1})$，因此 (i)。

假设 $(^h_p)\in A'$ 对应 $p < n$。然后，对于次数$< n$的所有$P\in \mathbf{Q}[T]$，使得$P(\mathbf{Z})\subset \mathbf{Z}$，我们有$P(h)\in A'$（no. 4，Prop.2的Cor.）。因此，鉴于 (16) 和 $m=n$，

$$
(h)(n-1-h)
$$

$(-1)^n$=

$$
nn
$$

$$
^{n-1}_-(2n-p-1-h)_-'
$$

$=-x^{(n)}y^{(n)}+\sum y^{(np)}x^{(np)}\in A$;

$$
p
$$

$p=0$

因此 (ii) $n$ 归纳。

### 6. 双序在分裂约化李代数的代数的包络线中

令$\mathfrak{g}$是$\mathfrak{g}$的$\mathbf{Q},\mathfrak{h}$分裂嘉当子代数的约李代数，以及$R = R(\mathfrak{g},\mathfrak{h}) ($§2, no. 1、注5）。

#### 定义 1 {#lie-viii-s12-def-1 .statement tag=0183}

如果对于所有 $\alpha \in R$，我们有 $H_{\alpha}\in \mathscr{H}$ 和 $\alpha (\mathscr{H})\subset \mathbf{Z}$，则 $\mathfrak{h}$ 中的格子 $\mathscr{H}$ 被认为是允许的（相对于 $\mathfrak{g}$）。

#### 注 1 {#lie-viii-s12-n6-rem-1 .statement tag=0184}

设 B 为 R 的基。当且仅当 $H_{\alpha}\in \mathscr{H}$ 和 $\alpha (\mathscr{H})\subset \mathbf{Z}$ 对于所有 $\alpha \in B$ 时，$\mathfrak{h}$ 中的格$\mathscr{H}$ 是允许的。

#### 注 2 {#lie-viii-s12-n6-rem-2 .statement tag=0185}

设$\mathfrak{c}$为$\mathfrak{g}$中的中心。那么，当且仅当 $Q(R^{\vee})\subset \mathscr{H}\subset P(R^{\vee})\oplus \mathfrak{c}$ 时，$\mathfrak{h}$ 中的格$\mathscr{H}$ 是允许的。那么格子$\mathscr{H}\cap \mathscr{D}\mathfrak{g}$在$\mathscr{D}\mathfrak{g}$的嘉当子代数$\mathfrak{h}\cap \mathscr{D}\mathfrak{g}$中是允许的。可能存在允许的格子$\mathscr{H}$使得$\mathscr{H}\not= (\mathscr{H}\cap \mathscr{D}\mathfrak{g})\oplus (\mathscr{H}\cap \mathfrak{c})$(cf.§13, no. 1.IX)。

#### 注 3 {#lie-viii-s12-n6-rem-3 .statement tag=0186}

如果 $\mathfrak{g}$ 是半单，则 $\mathfrak{h}$ 中允许的格子是 $\mathfrak{h}$ 的子群 $\mathscr{H}$，使得 $Q(R^{\vee})\subset \mathscr{H}\subset P(R^{\vee})$。

在这个数的其余部分，我们假设固定分裂约化李代数$(\mathfrak{g},\mathfrak{h})$，$R = R(\mathfrak{g},\mathfrak{h})$的基B，并且对于每个$\alpha \in B$，对$(x_{\alpha}, y_{\alpha})$，

$$
y_{\alpha}\in \mathfrak{g}^{-\alpha},x_{\alpha}\in \mathfrak{g}^{\alpha},[y_{\alpha}, x_{\alpha}] =H_{\alpha} \tag{20}
$$

如果我们用 $x_{\alpha}$（分别是 $y_{\alpha}$）生成的 $\mathfrak{g}$ 的 $\mathfrak{n}_+$（分别是 $\mathfrak{n}_-$）子代数表示，我们知道（§3, no. 3，命题 9 (iii)）

$$
\mathfrak{g}=\mathfrak{n}_-\oplus \mathfrak{h}\oplus \mathfrak{n}_+ \tag{21}
$$

$$
U(\mathfrak{g}) = U(\mathfrak{n}_-)\otimes_{\mathbf{Q}}U(\mathfrak{h})\otimes_{\mathbf{Q}}U(\mathfrak{n}_+) \tag{22}
$$

（其中$U(\mathfrak{g}), . .$.是$\mathfrak{g}, . . .$的包络代数）。

用$\mathscr{U}_+$表示由$\alpha \in B$和$n\in \mathbf{N}$的$x^{(n)}_{\alpha}$生成的$U(\mathfrak{n}_+)$的$\mathbf{Z}$子代数。令 W 为正根相对于 B 的 $R, R_+$ 集合的 Weyl 群。

#### 引理 5 {#lie-viii-s12-lem-5 .statement tag=0187}

(i) $\mathscr{U}_+$ 是向量空间 $U(\mathfrak{n}_+)$ 中的格子。

(ii) 对于所有$\alpha \in B$，我们有$\mathscr{U}_+\cap U(\mathfrak{g}^{\alpha}) =\bigoplus_{n\in\mathbf{N}}\mathbf{Z}x^{(n)}_{\alpha}$。

通过定义，$\mathscr{U}_+$由元素生成为$\mathbf{Z}$模块

$x(\varphi \mathbf{n})$ = $1\leq \prod i\leq rx(\varphi n((ii)$))

其中 $r\in \mathbf{N},\varphi = (\varphi (i))\in B^r$ 和 $\mathbf{n}= (n(i))\in \mathbf{N}^r$。给出代数 $U(\mathfrak{n}_+)$ 型 Q(R) 的分级，其中每个 $\mathfrak{g}^{\alpha}(\alpha \in R_+)$ 是次数 $\alpha$ 的齐次。前面型的单项式 $x^{(\mathbf{n})}_{\varphi}$ 是齐次的次数

$$
\sum_{1\leq i\leq r}n(i)\varphi (i)\in Q(R)
$$

具有给定次数 $q$ 的此类单项式数量有限，并且在 $\mathbf{Q}$ 上生成次数为 $q$ 的 $U(\mathfrak{n}_+)$ 齐次分量。 这就证明了(i)。

如果$\alpha \in B,\mathscr{U}_+\cap U(\mathfrak{g}^{\alpha})$包含在次数的齐次分量的和中，即$\alpha$的倍数；因此，根据前面的内容，$\mathscr{U}_+\cap U(\mathfrak{g}^{\alpha})$由$x^{(\mathbf{n})}_{\varphi}$生成，使得$\sum n(i)\varphi (i)\in \mathbf{N}\alpha$，这对所有$i$强制$\varphi (i) =\alpha$（因为B是R的基），所以

$x^{(\mathbf{n})}_{\varphi}=x^{(n(1))}_{\alpha}. . . x^{(n(r))}_{\alpha}=(n(1) +n$(1)!$\cdots . . . n+(nr$)!$(r$))! $x^{(n(1)+\cdot \cdot \cdot+n(r))}_{\alpha}$。

因此，$\mathscr{U}_+\cap \mathscr{U}(\mathfrak{g}^{\alpha})\subset \bigoplus_n\mathbf{Z}x^{(n)}_{\alpha}$，因此 (ii)。 Q.E.D.

在本段的其余部分中，如果E和F是$U(\mathfrak{g})$的$\mathbf{Z}$子模块，我们用$E.F$表示由产品$ab$生成的$\mathbf{Z}$子模块$U(\mathfrak{g})$，其中$a\in E, b\in F$。

#### 命题 3 {#lie-viii-s12-prop-3 .statement tag=0188}

令$\mathscr{H}$为$\mathfrak{h}$中的许用格子。令$\mathscr{U}_+,\mathscr{U}_-,\mathscr{U}_0$为$U(\mathfrak{g})$分别由元素$x_{\alpha}^{(n)}$$(\alpha \in B,n\in \mathbf{N}),y_{\alpha}^{(n)}(\alpha \in B, n\in \mathbf{N}),(^h_n)(h\in \mathscr{H}, n\in \mathbf{N})$生成的$\mathbf{Z}$-子代数。令$\mathscr{U}$为$\mathscr{U}_+,\mathscr{U}_-,\mathscr{U}_0$生成的$U(\mathfrak{g})$的$\mathbf{Z}$子代数。

(i) $\mathscr{U}$ 在大数$U(\mathfrak{g})$ 中是双序。

(ii) 我们有 $\mathscr{U}=\mathscr{U}_-.\mathscr{U}_0.\mathscr{U}_+,\mathscr{U}\cap \mathfrak{h}=\mathscr{H}$，并且对于所有 $\alpha \in B$，

$$
\mathscr{U}\cap \mathfrak{g}^{\alpha}=\mathbf{Z}x_{\alpha},V\cap \mathfrak{g}^{-\alpha}=\mathbf{Z}y_{\alpha}
$$

根据引理 5 和命题$2,\mathscr{U}_+,\mathscr{U}_-,\mathscr{U}_0$ 分别是$\mathbf{Q}$-代数$U(\mathfrak{n}_+),U(\mathfrak{n}_-),U(\mathfrak{h})$ 中的阶，并且

$$
(\pm h+q)
$$

$\in \mathscr{U}_0$ $h\in \mathscr{H}, q\in \mathbf{Z}, p\in \mathbf{N}$。 (23)

$$
p
$$

输入$\mathscr{L}=\mathscr{U}_-.\mathscr{U}_0.\mathscr{U}_+\subset U(\mathfrak{g})$。由(22)可知，$\mathscr{L}$是$U(\mathfrak{g})$中的格。到构造，

$$
\mathscr{U}_-.\mathscr{L}\subset \mathscr{L} \tag{24}
$$

$$
\mathscr{L}.\mathscr{U}_+\subset \mathscr{L} \tag{25}
$$

而引理 3 和 (23) 意味着

$$
\mathscr{U}_0.\mathscr{L}\subset \mathscr{L} \tag{26}
$$

$$
\mathscr{L}.\mathscr{U}_0\subset \mathscr{L} \tag{27}
$$

让$\alpha \in B, n\in \mathbf{N}, r\in \mathbf{N}, \varphi = (\varphi (i))\in B^r$，并且

$$
(m(1), . . . , m(r))\in \mathbf{N}^r
$$

我们表明

$$
x^{(n)}_{\alpha}y_{\varphi(1)}^{(m(1))}. . . y_{\varphi(r)}^{(m(r))}\in \mathscr{L} \tag{28}
$$

或者等价地，鉴于（25），

$$
[x^{(n)}_{\alpha}, y^{(m(1))}_{\varphi(1)}. . . y_{\varphi(r)}^{(m(r))}]\in \mathscr{L} \tag{29}
$$

我们在归纳对$r$争论。要研究的括号是和 / 项

$(m(1))(m(k))(n)(m(k+1))(m(k+2))(m(r))$

$y_{\varphi(1)}. . . y_{\varphi(k)}[x_{\alpha}, y_{\varphi(k+1)}]y_{\varphi(k+2)}. . . y_{\varphi(r)}$。 (30) 对于$\alpha \not=\varphi (k+ 1),x_{\alpha}$和$y_{\varphi(k+1)}$通勤，所以$[x^{(n)}_{\alpha}, y^{(m(k+1))}_{\varphi(k+1)}] = 0$。如果$\alpha =\varphi (k+ 1)$，则表达式(30)通过(17)，是形式的表达式中的和

$(m(1))(m(k))(m(k+1)-p)(q-h)(n-p)(m(k+2))(m(r))$

$$
y_{\varphi(1)}. . . y_{\varphi(k)}y_{\varphi(k+1)}x_{\alpha}y_{\varphi(k+2)}. . . y_{\varphi(r)} \tag{31}
$$

$$
p
$$

其中 $q\in \mathbf{Z}, p\in$ **N --** $\{0\}, h\in \mathscr{H}$。 归纳假设与(24)和(26)一起证明表达式(31)属于到$\mathscr{L}$。由此我们证明了(28)。

由 (28)，$x^{(n)}_{\alpha}\mathscr{U}_-\subset \mathscr{L}$；因此，通过 (25) 和 (27)，$x^{(n)}_{\alpha}\mathscr{L}\subset \mathscr{L}$，所以 $\mathscr{U}_+.\mathscr{L}\subset \mathscr{L}$ 和

$$
\mathscr{L}.\mathscr{L}\subset \mathscr{U}_-.\mathscr{U}_0.\mathscr{L}\subset \mathscr{U}_-.\mathscr{L}\subset \mathscr{L}
$$

因此，$\mathscr{L}$是$U(\mathfrak{g})$的$\mathbf{Z}$子代数，因此$\mathscr{U}=\mathscr{L}$。如果$c$是$U(\mathfrak{g}),c(\mathscr{U})\subset \mathscr{U}\otimes_{\mathbf{Z}}\mathscr{U}$的余积（no. 2，命题1）。设$\gamma$为$U(\mathfrak{g})$的余单位。从$\gamma (x^{(n)}_{\alpha}) =\gamma (y^{(n)}_{\alpha}) =\gamma ((^h_n))= 0$到$n >0$，我们有$\gamma (\mathscr{U})\subset \mathbf{Z}$。这就证明了(i)。另一方面，

$$
\mathscr{U}\cap \mathfrak{h}=\mathscr{L}\cap \mathfrak{h}=\mathscr{U}_0\cap \mathfrak{h}=\mathscr{H}
$$

根据no. 4第2号提案；同样，

$$
\mathscr{U}\cap \mathfrak{g}^{\alpha}=\mathscr{U}_+\cap \mathfrak{g}^{\alpha}=\mathbf{Z}x_{\alpha}
$$

由引理 5. 这就证明了 (ii)。

#### 注 4 {#lie-viii-s12-n6-rem-4 .statement tag=0189}

根据§4, no. 4的第5条，$\mathfrak{g}$存在唯一的自同构$\theta$，使得$\theta (x_{\alpha}) =y_{\alpha}$和$\theta (y_{\alpha}) =x_{\alpha}$适用于所有$\alpha \in B$，$\theta (h) =-h$适用于所有$h\in \mathfrak{h}$；我们有$\theta^2= 1$。通过 $\mathscr{U}$ 的构造，我们看到 $U(\mathfrak{g})$ 的自同构扩展 $\theta$ 使 $\mathscr{U}$ 保持稳定。

#### 推论 1 {#lie-viii-s12-prop-3-cor-1 .statement tag=018A}

把$\mathscr{G}=\mathscr{U}\cap \mathfrak{g}$。那么$\mathscr{G}$就是李代数$\mathfrak{g}$中的阶，在$\theta$下稳定。我们有$\mathscr{G}=\mathscr{H}+\sum_{\alpha\in R}(\mathscr{G}\cap \mathfrak{g}^{\alpha})$。对于所有$\alpha \in B$和所有$n\in \mathbf{N}$，映射（广告$x_{\alpha}$）$^n/n$！，（广告$y_{\alpha}$）$^n/n$！保持 $\mathscr{U}$ 和 $\mathscr{G}$ 稳定。

第一个断言是清楚的。第二个是考虑型 Q(R) 在$U(\mathfrak{g})$ 和$\mathscr{U}$ 上的毕业。第三个来自引理 2 of no. 5。

#### 推论 2 {#lie-viii-s12-prop-3-cor-2 .statement tag=018B}

让$w\in W$。存在$\mathfrak{g}$的基本自同构$\varphi$，它与$\theta$可交换，使$\mathscr{G}$和$\mathscr{U}$稳定，以及扩展$w$。

处理$w$为形式$s_{\alpha}(\alpha \in B)$的情况就足够了。 注首先，ad $x_{\alpha}$ 和 ad $y_{\alpha}$ 在 $U(\mathfrak{g})$ 上局部幂零，在其他字中，对于所有 $u\in U(\mathfrak{g})$ 存在整数 $n$，使得 (ad $x_{\alpha}$)$^nu=$ (ad $y_{\alpha}$）$^nu= 0$。

这使我们能够定义自同构 $e^{adx_{\alpha}}=\sum_{n=0}^{\infty}\frac{1}{n!}$(ad $x_{\alpha}$)$^n$ 和 $e^{ady_{\alpha}}$ of $U(\mathfrak{g})$；我们立即验证$U(\mathfrak{g})$中的这些自同构保持$\mathscr{U}$稳定。把$\varphi_1=e^{adx_{\alpha}}e^{ady_{\alpha}}e^{adx_{\alpha}},\varphi_2=e^{ady_{\alpha}}e^{adx_{\alpha}}e^{ady_{\alpha}}$。我们有 $\varphi_1|\mathfrak{g}=$ $\varphi_2|\mathfrak{g}($§2, no. 2，公式 (1))，所以 $\varphi_1=\varphi_2$。输入$\varphi_1=\varphi_2=\varphi$。我们有$\theta \varphi \theta^{-1}=\varphi$，所以$\theta$和$\varphi$通勤。另一方面，$\varphi |\mathfrak{h}=w$乘§2, no. 2，引理1。

#### 推论 3 {#lie-viii-s12-prop-3-cor-3 .statement tag=018C}

让$\alpha \in R$。如果$x\in \mathscr{G}\cap \mathfrak{g}^{\alpha}$和$n\in \mathbf{N}$，我们有$x^{(n)}\in \mathscr{U}$，和（广告$x$）$^n/n$！使 $\mathscr{G}$ 和 $\mathscr{U}$ 保持稳定。

如果 $\alpha \in B$、$\mathscr{U}$ 的构造和 Cor 是清楚的。 1. 在一般情况下，存在$w\in W$使得$w(\alpha )\in B$（第VI, §1, no. 5章，第15条命题）。由科. 2、存在$\mathfrak{g}$的自同构$\varphi$，使得$\mathscr{G}$和$\mathscr{U}$保持稳定，并且将$\mathfrak{g}^{\alpha}$带到$\mathfrak{g}^{w(\alpha)}$，因此推论乘以结构的迁移。

#### 推论 4 {#lie-viii-s12-prop-3-cor-4 .statement tag=018D}

在 $(\mathfrak{g},\mathfrak{h}) ($§2, no. 4 中存在 Chevalley 系统 $(X_{\alpha})_{\alpha\in R}$，Def。 3) 使得$X_{\alpha}=x_{\alpha}$和$X_{-\alpha}=y_{\alpha}$对应$\alpha \in B$。对于每个具有这些属性的 Chevalley 系统 $(X'_{\alpha})_{\alpha\in R}$，并且对于所有 $\alpha \in R,X'_{\alpha}$ 是 $\mathscr{G}\cap \mathfrak{g}^{\alpha}$ 的基。

对于$\alpha \in B$，输入$X_{\alpha}=x_{\alpha}, X_{-\alpha}=y_{\alpha}$。对于$\alpha \in R_+$ **--** B，选择 a $w\in W$，使得$\mathfrak{g}$的$w(\alpha )\in B$和自同构$\varphi$，使得$\theta \varphi =\varphi \theta ,\varphi (\mathscr{G}) =\mathscr{G}$和$\varphi (h) =w^{-1}(h)$对于$h\in \mathfrak{h}$（Cor.2）；输入$X_{\alpha}=\varphi (x_{w(\alpha)}), X_{-\alpha}=\varphi (y_{w(\alpha)})$。然后

$$
[X_{-\alpha}, X_{\alpha}] =\varphi ([y_{w(\alpha)}, x_{w(\alpha)}]) =\varphi (H_{w(\alpha)}) =w^{-1}(H_{w(\alpha)}) =H_{\alpha}
$$

$$
\theta (X_{\alpha}) =\theta \varphi (x_{w(\alpha)}) =\varphi \theta (x_{w(\alpha)}) =\varphi (y_{w(\alpha)}) =X_{-\alpha}
$$

所以 $(X_{\alpha})_{\alpha\in R}$ 是 Chevalley 系统。而且，

$$
\mathscr{G}\cap \mathfrak{g}^{\alpha}=\varphi (\mathscr{G}\cap \mathfrak{g}^{w(\alpha)}) =\varphi (\mathbf{Z}x_{w(\alpha)}) =\mathbf{Z}X_{\alpha} \tag{32}
$$

$$
\mathscr{G}\cap \mathfrak{g}^{-\alpha}=\varphi (\mathscr{G}\cap \mathfrak{g}^{-w(\alpha)}) =\varphi (\mathbf{Z}y_{w(\alpha)}) =\mathbf{Z}X_{-\alpha} \tag{33}
$$

令 $(X'_{\alpha})_{\alpha\in R}$ 为 Chevalley 系统，使得 $X'_{\alpha}=x_{\alpha}, X'_{-\alpha}=y_{\alpha}$ 对应 $\alpha \in B$。令 S 为 $\alpha \in R$ 的集合，使得 $X'_{\alpha}=\pm X_{\alpha}$。根据第7条命题§2, no. 4，S是根的闭集合。从 $S\supset B\cup (-B)$ 开始，我们有 S = R（第 VI, §1, no. 6 章，第 19 条命题）。因此，根据 (32) 和 (33)，我们对所有 $\alpha \in R$ 都有 $\mathscr{G}\cap \mathfrak{g}^{\alpha}=\mathbf{Z}X'_{\alpha}$。

#### 注 5 {#lie-viii-s12-n6-rem-5 .statement tag=018E}

令 $(X_{\alpha})_{\alpha\in R}$ 为上面构建的 Chevalley 系统。如果$\alpha , \beta , \alpha +\beta \in R$并且如果我们放入$[X_{\alpha}, X_{\beta}] = N_{\alpha ,\beta}X_{\alpha+\beta}$，我们有$[X_{\alpha}, X_{\beta}]\in$$\mathscr{G}\cap \mathfrak{g}^{\alpha+\beta}$，并且我们恢复了$N_{\alpha ,\beta}\in \mathbf{Z}$的事实（cf.§2, no. 4，第7条）。

#### 注 6 {#lie-viii-s12-n6-rem-6 .statement tag=018F}

我们在经过中获得了Chevalley系统存在的新证明（cf.§4, no. 4，Prop.5的Cor.），独立于引理4，§2。

### 7. 谢瓦利阶

令$(\mathfrak{g},\mathfrak{h})$为分裂约化李代数超过$\mathbf{Q}, R$其根系。 选择：

a) $\mathfrak{h}$ 中的允许格$\mathscr{H}$ (no. 6, Def. 1);

b) 对于所有 $\alpha \in R$，$\mathfrak{g}^{\alpha}$ 中的格$\mathscr{G}^{\alpha}$。

输入$\mathscr{G}=\mathscr{H}\oplus \sum_{\alpha\in R}\mathscr{G}^{\alpha}$。这是$\mathfrak{g}$中的一个格子。用 $\mathscr{U}$ 表示 $\mathbf{Z}$-子代数

$U(\mathfrak{g})$由$(^h_n)(h\in \mathscr{H}, n\in \mathbf{N})$和$x^{(n)}(x\in \mathscr{G}^{\alpha}, \alpha \in R$、$n\in \mathbf{N})$生成。最后，对于 $\alpha \in R$ 和 $x\in \mathfrak{g}^{\alpha}$ **--** $\{0\}$，将

$w_{\alpha}(x) =$（扩展广告$x$）（扩展广告$y$）（扩展广告$x$），

其中$y$是$\mathfrak{g}^{-\alpha}$的唯一元素，使得$[y, x] =H_{\alpha}$。有了这些记号：

#### 定理 2 {#lie-viii-s12-thm-2 .statement tag=018G}

以下条件是等效的：

(i) 存在 $(\mathfrak{g},\mathfrak{h})$ 的 Chevalley 系统 $(X_{\alpha})_{\alpha\in R}$，使得 $\mathscr{G}_{\alpha}=\mathbf{Z}X_{\alpha}$ 对于所有 $\alpha \in R$。

(ii) $\mathscr{U}\cap \mathfrak{g}=\mathscr{G}$ 和 $[\mathscr{G}^{\alpha},\mathscr{G}^{-\alpha}] =\mathbf{Z}H_{\alpha}$ 对于所有 $\alpha \in R$。

(iii) 对于所有$\alpha \in R, x\in \mathscr{G}^{\alpha}, n\in \mathbf{N}$、自同态（广告$x$）$^n/n$！ $\mathfrak{g}$映射$\mathscr{G}$至$\mathscr{G}$和$[\mathscr{G}^{\alpha},\mathscr{G}^{-\alpha}] =\mathbf{Z}H_{\alpha}$。

(iv) 对于所有$\alpha \in R$和$\mathscr{G}^{\alpha},w_{\alpha}(x)$映射$\mathscr{G}$到$\mathscr{G}($的每个基$x$，即对于所有$\beta \in R)$，映射$\mathscr{G}^{\beta}$到$\mathscr{G}^{s_{\alpha}(\beta)}$。

(i) $=\Rightarrow$ (ii)：令$(X_{\alpha})_{\alpha\in R}$为$(\mathfrak{g},\mathfrak{h})$中的Chevalley系统，使得$\mathscr{G}^{\alpha}=$$\mathbf{Z}X_{\alpha}$对于所有$\alpha \in R$，并令B为R的基。对于$\alpha \in B$，放入$x_{\alpha}=X_{\alpha}, y_{\alpha}=$ $X_{-\alpha}$。令$\mathscr{U}'$为双序，由no. 6到$\mathscr{H}$、$x_{\alpha}$和$y_{\alpha}$的命题3相关联。显然$\mathscr{U}'\subset \mathscr{U}$。由科. $3,x^{(n)}\in \mathscr{U}'$ 提案 3 和 4 适用于所有 $\alpha \in R,x\in \mathscr{G}^{\alpha}$ 和 $n\in \mathbf{N}$。因此$\mathscr{U}=\mathscr{U}'$，证明了(ii)。

(ii) $=\Rightarrow$ (iii)：通过 no. 5 的引理 2 可以清楚地看出这一点。

(iii) $=\Rightarrow$ (iv)：令$\alpha \in R$且令$x$为$\mathscr{G}^{\alpha}$的基。从$[\mathscr{G}^{\alpha},\mathscr{G}^{-\alpha}] =\mathbf{Z}H_{\alpha}$开始，唯一的$y\in \mathfrak{g}^{-\alpha}$使得$[y, x] =H_{\alpha}$属于到$\mathscr{G}^{-\alpha}$。由于 exp ad $x$ 和 exp ad $y$ 在 (iii) 时使 $\mathscr{G}$ 保持稳定，$w_{\alpha}(x)$ 也是如此。

(iv) $=\Rightarrow$ (i)：令 B 为 R 的基。对于所有 $\alpha \in B$，$\mathscr{G}^{\alpha}$ 选择基 $x_{\alpha}$。令$y_{\alpha}\in \mathscr{G}^{-\alpha}$ 使得$[y_{\alpha}, x_{\alpha}] =H_{\alpha}$。到 §1, no. 5，公式 (5)，我们有 $y_{\alpha}=w_{\alpha}(x_{\alpha}).x_{\alpha}$，所以 $y_{\alpha}$ 是基的$\mathscr{G}^{-\alpha}$ 到 (iv)。令$\mathscr{G}'$为由$\mathscr{H}$、$x_{\alpha}$和$y_{\alpha}$定义的$\mathfrak{g}$中的阶（no. 6，第3命题的Cor.1）。那么$\mathscr{G}'$就稳定在(ad $x_{\alpha}$)$^n/n$!,(ad $y_{\alpha}$)$^n/n$!下（loc. cit.），因此位于 $w_{\alpha}(x_{\alpha})$ 之下。

现在让$\beta \in R$。存在 $\alpha_0, \alpha_1, . . . , \alpha_r\in B$ 使得

$$
\beta =s_{\alpha_r}s_{\alpha_{r-1}}. . . s_{\alpha_1}(\alpha_0)
$$

（第 VI, §1, no. 5 章，提案 15）。然后通过(iv) $w_{\alpha_r}(x_{\alpha_r}).w_{\alpha_{r-1}}(x_{\alpha_{r-1}}). . . w_{\alpha_1}(x_{\alpha_1})$ 映射 $\mathscr{G}^{\alpha_0}$ 到$\mathscr{G}^{\beta}$，并通过前面的映射 $\mathscr{G}'\cap \mathfrak{g}^{\alpha_0}$ 到$\mathscr{G}'\cap \mathfrak{g}^{\beta}$。从$\mathscr{G}'\cap \mathfrak{g}^{\alpha_0}=\mathscr{G}^{\alpha_0}$（提案3（ii））开始，我们有$\mathscr{G}'\cap \mathfrak{g}^{\beta}=\mathscr{G}^{\beta}$。因此

$$
\mathscr{G}'=\mathscr{H}\oplus \sum_{\beta\in R}(\mathscr{G}'\cap \mathfrak{g}^{\beta}) =\mathscr{H}\oplus \sum_{\beta\in R}\mathscr{G}^{\beta}=\mathscr{G}
$$

和科。第 3 号提案第 4 条结论证明。

#### 定义 2 {#lie-viii-s12-def-2 .statement tag=018H}

当 Th 的条件 (i) 至 (iv) 时。 2个都满意，$\mathscr{G}$据说是$(\mathfrak{g},\mathfrak{h})$的Chevalley阶。

#### 注 {#lie-viii-s12-n7-rem-1 .statement tag=018I}

$(\mathfrak{g},\mathfrak{h})$中的Chevalley阶始终存在。事实上，Chevalley 阶是形式 $\mathscr{H}\oplus \sum_{\alpha\in R}\mathbf{Z}X_{\alpha}$ 的集合，其中 $(X_{\alpha})_{\alpha\in R}$ 是 $(\mathfrak{g},\mathfrak{h})$ 中的 Chevalley 系统，$\mathscr{H}$ 是 $\mathfrak{h}$ 中的格子，这样

$$
Q(R^{\vee})\subset \mathscr{H}\subset P(R^{\vee})\oplus \mathfrak{c}
$$

$(\mathfrak{c}$ 是中心 / $\mathfrak{g})$。

#### 定理 3 {#lie-viii-s12-thm-3 .statement tag=018J}

我们保留no. 7开头的记号，并假设$\mathscr{G}$是$(\mathfrak{g},\mathfrak{h})$中的Chevalley阶。

(i) $\mathscr{U}$ 是 $U(\mathfrak{g})$ 中的双序。

(ii) 令 B 为 R 的基，且$(X_{\alpha})_{\alpha\in B\cup(-B)}$为$\mathfrak{g}$的元素族，使得$\mathscr{G}^{\alpha}=\mathbf{Z}X_{\alpha}$对应于$\alpha \in B\cup (-B)$。 $\mathbf{Z}$代数$\mathscr{U}$由$(^h_n)$和$X_{\alpha}^{(n)}(h\in \mathscr{H}, \alpha \in B\cup (-B), n\in \mathbf{N})$生成。如果$\mathfrak{g}$是半单且$\mathscr{H}= Q(R^{\vee})$，则$\mathbf{Z}$代数$\mathscr{U}$由$X_{\alpha}^{(n)}(\alpha \in B\cup (-B), n\in \mathbf{N})$生成。

(iii) 令 B 为 R 的基，正根、$R_-=-R_+,\mathfrak{n}_+=\sum_{\alpha\in R_+}\mathfrak{g}^{\alpha},\mathfrak{n}_-=\sum_{\alpha\in R_-}\mathfrak{g}^{\alpha}$ 的$R_+$ 相应的集合。然后，

$$
\mathscr{U}= (\mathscr{U}\cap U(\mathfrak{n}_-)).(\mathscr{U}\cap U(\mathfrak{h})).(\mathscr{U}\cap U(\mathfrak{n}_+))
$$

设$(h_i)_{i\in I}$为$\mathscr{H}$中的基。对于所有$\alpha \in R$，令$X_{\alpha}$为$\mathscr{G}^{\alpha}$的基。给集合 $I\cup R$ 总计阶 （我们假设 $I\cap R =\emptyset$ ）。对于$\lambda \in I\cup R$和$n\in \mathbf{N}$，如果$\lambda \in I,e^{\langle n\rangle}_{\lambda}=X_{\lambda}^{(n)}$如果$\lambda \in R$，则输入$e^{\langle n\rangle}_{\lambda}=(^{h_{\lambda}}_n)$。然后是乘积$\prod_{\lambda\in I\cup R}e^{\langle n_{\lambda}\rangle}_{\lambda}$，其中$(n_{\lambda})$属于到$\mathbf{N}^{I\cup R}$，$\mathbf{Z}$模块$\mathscr{U}$的形式基。这

乘积$\prod_{\lambda\in I}(^{h_{\lambda}}_{n_{\lambda}})$，其中$\mathbf{Z}$模块$\mathscr{U}\cap U(\mathfrak{h})$的$(n_{\lambda})$属于到$\mathbf{N}^I$、形式基。 乘积$\prod_{\lambda\in R_+}X_{\lambda}^{(n_{\lambda})}$，其中$\mathbf{Z}$模块$\mathscr{U}\cap U(\mathfrak{n}_+)$的$(n_{\lambda})$属于到$\mathbf{N}^{R_+}$、形式基。

令 B 和 $(X_{\alpha})_{\alpha\in B\cup(-B)}$ 如 (ii) 中那样，并且使得$[X_{-\alpha}, X_{\alpha}] =H_{\alpha}$。令$\mathscr{U}'$为$U(\mathfrak{g})$由$(_n^h)$和$X_{\alpha}^{(n)}$$(h\in \mathscr{H}, \alpha \in B\cup (-B), n\in \mathbf{N})$生成的$\mathbf{Z}$子代数。我们在Th的证明看到过。 2、(i)$=\Rightarrow$(ii)，$\mathscr{U}'$等于$\mathscr{U}$，在$U(\mathfrak{g})$中为双序。这证明了 (i) 和 (ii) 的第一个断言；第二个来自引理 4 (ii)。 断言 (iii) 由 Th 得出。 1 (no. 3) 和提案 3 (no. 6)。

### 8. 容许格子

推广向量空间采用的术语，如果存在M的基使得$u$的矩阵相对于该基是对角的，则称模M的自同态$u$可对角化的。

#### 引理 6 {#lie-viii-s12-lem-6 .statement tag=018K}

设 M 是 M 的有限型、$u$ 自同态和 $M\otimes_{\mathbf{Z}}\mathbf{Q}$ 的 $v$ 自同态 $u\otimes 1$ 的自由$\mathbf{Z}$模。假设 $(^v_n)(M)\subset M$ 对于所有 $n\in \mathbf{N}$。那么$u$可对角化的。

a) 对于任意多项式 $P\in \mathbf{Q}[T]$ 使得 $P(\mathbf{Z})\subset \mathbf{Z}$，我们有 $P(v)(M)\subset M$（no. 4，命题 2 的修正），因此得到 $P(v)\in \mathbf{Z}$。

b) 用$\chi_v(t) =t^d+\alpha_1t^{d-1}+\cdots$表示$v$的特征多项式。让$k\in \mathbf{Z}, n\in \mathbf{N}$。 应用 a) 代入多项式 $(^{T-k}_n)$，我们看到数

$a_n=$ det $(v-k)=1_d$ det($v-k$) det($v-k-1$)$. .$。检测($v-k-n+ 1$)

$n(n$！）

$$
=\frac{(-1)^n}{4}\chi_v(k)\chi_v(k+ 1). . . \chi_v(k+n-1)
$$

$(n$！）

是整数。取$k-1<-\alpha_1/d$。然后

$$
\chi_v(k+n-1) =n^d+ (\alpha_1+ (k-1)d)n^{d-1}+\cdots
$$

和

$$
|a_n|=\frac{|\chi_v(k + n- 1)|}{d}|a_{n-1}|
$$

$$
n
$$

因而，如果$a_n\not= 0$对于所有$n\in \mathbf{N}$，$|a_n|$的序列对于$n$足够大来说就是严格递减，这是荒谬的。由此可见 $v$ 有整数特征值 $\lambda$。输入$M'=$ Ker($u-\lambda .1$) 和$M''= M/M'$。那么$M'$是交，其中M为向量子空间为$M\otimes_{\mathbf{Z}}\mathbf{Q}$，因而$\mathbf{Z}$模$M''$是有限型的无扭力，因此也没有秩$< d$。由$d$的归纳和由$u$引发的$M''$的应用归纳假设到自同态争论，我们结论认为代数闭扩张中$v$的所有特征值 $\mathbf{Q}$ 是整数。

c) 我们证明$v$是可对角化的。令$\lambda$为$v$的特征值，并令$x\in M\otimes_{\mathbf{Z}}\mathbf{Q}$为$(v-\lambda )^2x= 0$。我们有$v(vx-\lambda x) =\lambda (vx-\lambda x)$，所以

$n1$！$(v-\lambda -n+ 1)(v-\lambda -n+ 2). . .(v-\lambda -1)(v-\lambda )x$

$$
=\frac{(-1)^{n-1}}{n}(vx-\lambda x)
$$

通过a)，这意味着$vx-\lambda x\in nM$对于所有$n\in \mathbf{N}$，因而$(v-\lambda )x= 0$。

d) 令$\lambda$为$v$的特征值，并令$\lambda -a, \lambda +b$为$\mathbf{Z}$包含中的区间，所有特征值为$v$。考虑多项式

$$
(T-\lambda -1)(T-\lambda -2). . .(T-\lambda -b)
$$

$$
P(T) = (-1)^b
$$

$b$！

$$
(T-\lambda + 1)(T-\lambda + 2). . .(T-\lambda +a)
$$

$$
\times
$$

$a$！

我们有 $\mu\in \mathbf{Z}\cap (\lambda -a, \lambda +b)$ 和 $\mu\not=\lambda$ 的 $P(\mathbf{Z})\subset \mathbf{Z},P(\lambda ) = 1,P(\mu) = 0$。 $a), P(v)(M)\subset M$。通过$c), P(v)$是$M\otimes_{\mathbf{Z}}\mathbf{Q}$的投影到特征空间相应的到$\lambda$。 Q.E.D.

#### 注 1 {#lie-viii-s12-n8-rem-1 .statement tag=018L}

如果我们仅假设$v$与整数特征值可对角化，则$u$不一定可对角化（例如，对所有$(x, y)\in M$取$M =\mathbf{Z}^2$和$u(x, y) =$$(y, x)$）。

令$\mathfrak{g},\mathfrak{h},R,\mathscr{H},\mathscr{G}^{\alpha},\mathscr{G},\mathscr{U}$与no. 7相同，并假设$\mathscr{G}$是$(\mathfrak{g},\mathfrak{h})$中的Chevalley阶。

#### 定义 3 {#lie-viii-s12-def-3 .statement tag=018M}

令 E 为 $\mathfrak{g}$ 模。如果满足以下条件，则 E 中的格 $\mathscr{E}$ 被认为是可接受的（相对于 $\mathscr{G}$）：

(i) $\mathscr{U}$映射$\mathscr{E}$至$\mathscr{E}$；

(ii) 对于所有 $\alpha \in R, x\in \mathscr{G}^{\alpha}, n\in \mathbf{N}, h\in \mathscr{H}$，$\mathscr{E}$ 在 $(^h_n)$ 和 $x^{(n)}$ 下是稳定的。

#### 注 2 {#lie-viii-s12-n8-rem-2 .statement tag=018N}

令$\rho$为$\mathfrak{g}$在$U(\mathfrak{g})$上的伴随表示。令 $\alpha , x, n, h$ 如上面 (ii) 中所示。我们有$\rho (x^{(n)}).\mathscr{U}\subset \mathscr{U}$乘引理2。另一方面，如果$p\in \mathbf{N}$，

$((h))_{(n)}($广告$h)_{(n)}(n\alpha (h))_{(n)}$

$\rho x$ = $x$ = $x$

$$
ppp
$$

(no. 5, 公式 (13))，所以$\rho ((^h_p)).\mathscr{U}\subset \mathscr{U}$。这证明了$\mathscr{U}$是$U(\mathfrak{g})$中的一个容许格，并且由此得出$\mathscr{G}$是$\mathfrak{g}$中的一个容许格（对于伴随表示）。

#### 注 3 {#lie-viii-s12-n8-rem-3 .statement tag=018O}

设 E 为有限维 $\mathfrak{g}$ 模，$\mathscr{E}$ E 中的容许格，$\mathfrak{c}$ 中心 of $\mathfrak{g}$。到引理 6，$\mathfrak{c}$ 定义的每个元素都是 E 的对角化自同态。因此 E 是半单（第 I, §6, no. 5，第 4 章）。因此，E 是简单 $\mathscr{D}\mathfrak{g}$ 模的直和，其中 $\mathfrak{c}$ 诱导同位。到引理 $6,\mathscr{E}=\oplus (\mathscr{E}\cap E^{\lambda})$ 并且，对于 E 的所有权 $\lambda$，我们有

$$
\lambda (\mathscr{H})\subset \mathbf{Z}
$$

#### 注 4 {#lie-viii-s12-n8-rem-4 .statement tag=018P}

如果$\mathfrak{g}$是半单和$\mathscr{H}= Q(R^{\vee})$，则Def的条件(i)和(ii)。 3 是等价的，由 Th 表示。 3（二），至

(iii) 对于所有 $\alpha \in R, x\in \mathscr{G}^{\alpha}, n\in \mathbf{N}$，$\mathscr{E}$ 在 $x^{(n)}$ 下稳定。

#### 注 5 {#lie-viii-s12-n8-rem-5 .statement tag=018Q}

设 B 为 R 的基；在上述条件 (i) 和 (ii) 中，“$\alpha \in$ R”可以替换为“$\alpha \in B\cup (-$B)”（loc. cit）。

#### 定理 4 {#lie-viii-s12-thm-4 .statement tag=018R}

令 E 为有限维 $\mathfrak{g}$ 模。以下条件是等效的：

(i) E 有一个容许格；

(ii) $\mathscr{H}$ 定义的每个元素与整数特征值的可对角化的自同态。

(i) $=\Rightarrow$ (ii)：这是从注 3 得出的。

(ii) $=\Rightarrow$ (i)：我们假设条件 (ii) 满足并证明(i)。 由 Th.第4章。 I, §6, no. 5，我们可以假设$\mathfrak{c}$定义的元素与E同位，并且E是一个简单的$\mathscr{D}\mathfrak{g}$模。 设 B 为 R 的基，且 $\mathfrak{g}$ 的 $\mathfrak{g}=\mathfrak{n}_-\oplus \mathfrak{h}\oplus \mathfrak{n}_+$ 相应的分解。 令$\lambda$为$\mathscr{D}\mathfrak{g}$模块E的最高权，并令$e\in E^{\lambda}$ **--** $\{0\}$。 输入$\mathscr{E}=\mathscr{U}.e$。 显然$\mathscr{U}.\mathscr{E}\subset \mathscr{E}$。 由于 E 很简单，因此 $U(\mathfrak{g}).e= E$ 以及 $\mathscr{E}$ 生成 E 都是 $\mathbf{Q}$ 向量空间。 对于$h\in \mathscr{H}$和$n\in \mathbf{N}$，我们有$(^h_n)e=(^{\lambda(h)}_n)e\in \mathbf{Z}e$，所以

$$
(\mathscr{U}\cap U(\mathfrak{h})).e=\mathbf{Z}e
$$

从 $U(\mathfrak{n}_+).e= 0$ 开始，我们根据命题 3 得到 $\mathscr{E}= (\mathscr{U}\cap U(\mathfrak{n}_-)).e$。 3 (iii) $\mathscr{E}$ 是有限型的 $\mathbf{Z}$ 模。

#### 推论 {#lie-viii-s12-n8-cor-1 .statement tag=018S}

如果$\mathfrak{g}$是半单和$\mathscr{H}= Q(R^{\vee})$，则每个有限维$\mathfrak{g}$模都有一个容许格。
