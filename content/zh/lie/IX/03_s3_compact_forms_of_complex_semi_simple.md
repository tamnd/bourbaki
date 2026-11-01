---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 3
section_title: Compact forms of complex semi-simple Lie algebras
lang: zh
source: lie-vii-ix
book_pages: 296-303, 394-396
pdf_pages: 0303-0310, 0401-0403
extraction: native+ocr
subsections:
    - "no": 1
      title: REAL FORMS
      page: 296
      pdf_page: 303
    - "no": 2
      title: REAL FORMS ASSOCIATED TO A CHEVALLEY SYSTEM
      page: 297
      pdf_page: 304
    - "no": 3
      title: CONJUGACY OF COMPACT FORMS
      page: 299
      pdf_page: 306
    - "no": 4
      title: 'EXAMPLE I: COMPACT ALGEBRAS OF TYPE A$_{\boldsymbol{n}}$'
      page: 300
      pdf_page: 307
    - "no": 5
      title: 'EXAMPLE II: COMPACT ALGEBRAS OF TYPE B$_{\boldsymbol{n}}\mathbf{A}\mathbf{N}\mathbf{D}$ $\mathbf{D}_{\boldsymbol{n}}$'
      page: 301
      pdf_page: 308
    - "no": 6
      title: COMPACT GROUPS OF RANK 1
      page: 302
      pdf_page: 309
statements: 17
exercises: 9
content_sha256: c991aa1997acf877c5364717ad0a26352229f850f883a214d1b16071d742e771
translated_from: content/en/lie/IX/03_s3_compact_forms_of_complex_semi_simple.md
translation_method: google
source_content_sha256: bf0ebd0cda151170c108a2f9b899a1c59ba20dd5f6195c4caf5f17e7cc05a3cd
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 0465955b6a29050f6e3449c57606b0e87c030d992cea664cb0bb30f8112edc2b
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 3。 紧形式复半单李代数

### 1. 真实形式

如果$\mathfrak{a}$是复数李代数，我们用$\mathfrak{a}_{[\mathbf{R}]}$（或有时用$\mathfrak{a}$）表示由标量限制获得的实数李代数。 如果$\mathfrak{g}$是实数李代数，我们用$\mathfrak{g}_{(\mathbf{C})}$（或有时用$\mathfrak{g}_{\mathbf{C}}$）表示由标量扩张获得的复数李代数$\mathbf{C}\otimes_{\mathbf{R}}\mathfrak{g}$。 The homomorphisms of real Lie algebras $\mathfrak{g}\rightarrow \mathfrak{a}_{[\mathbf{R}]}$ correspond bijectively to the homomorphisms of complex Lie algebras $\mathfrak{g}_{(\mathbf{C})}\rightarrow \mathfrak{a}:$ if $f:\mathfrak{g}\rightarrow \mathfrak{a}_{[\mathbf{R}]}$ and $g:\mathfrak{g}_{(\mathbf{C})}\rightarrow \mathfrak{a}$ correspond, we have $f(x) =g(1\otimes x)$ and $g(\lambda \otimes x) =\lambda f(x)$ for $x\in \mathfrak{g}, \lambda \in \mathbf{C}$.

#### 定义 1 {#lie-ix-s3-def-1 .statement tag=01B1}

令 $\mathfrak{a}$ 为复数李代数。 $\mathfrak{a}$的实数形式是$\mathfrak{a}$的实数子代数$\mathfrak{g}$，它是$\mathbf{C}$向量空间$\mathfrak{a}($代数上的$\mathbf{R}$结构，第1章。 II, §8, no. 1，防御。 1）。

这意味着与典范嵌入 $\mathfrak{g}\rightarrow \mathfrak{a}_{[\mathbf{R}]}$ 关联的复数李代数 $\mathfrak{g}_{(\mathbf{C})}\rightarrow \mathfrak{a}$ 的同态是双射的。因此，当且仅当实数向量空间 $\mathfrak{a}$ 的子空间 $\mathfrak{g}$ 和$i\mathfrak{g}$ 互补时，$\mathfrak{a}$ 的实数子代数 $\mathfrak{g}$ 才是$\mathfrak{a}$ 的实数形式。 $\mathfrak{a}$ 相对于实数形式 $\mathfrak{g}$ 的共轭是映射 $\sigma :\mathfrak{a}\rightarrow \mathfrak{a}$，使得

$$
\sigma (x+iy) =x-iy,x, y\in \mathfrak{g} \tag{1}
$$

#### 命题 1 {#lie-ix-s3-prop-1 .statement tag=01JF}

$a)$ 令$\mathfrak{g}$ 为$\mathfrak{a}$ 和$\sigma$ 的实形式，是$\mathfrak{a}$ 相对于$\mathfrak{g}$ 的共轭。然后：

$\sigma^2=$ ID$_{\mathfrak{a}}, \sigma (\lambda x+\mu y) = \overline{\lambda \sigma}(x) + \overline{\mu\sigma}(y),[\sigma (x), \sigma (y)] =\sigma [x, y]$ (2)

对于$\lambda , \mu\in \mathbf{C},x, y\in \mathfrak{a}$。 $\mathfrak{a}$属于到$\mathfrak{g}$的元素$x$当且仅当$\sigma (x) =x$。

b) 设 $\sigma :\mathfrak{a}\rightarrow \mathfrak{a}$ 为映射满足 (2)。那么$\sigma$的固定点的集合$\mathfrak{g}$是$\mathfrak{a}$的实形式，$\sigma$是$\mathfrak{a}$相对于$\mathfrak{g}$的共轭。

证明是直接的。

注，如果B表示$\mathfrak{a}$的杀戮形式，且$\mathfrak{g}$是$\mathfrak{a}$的实数形式，则B到$\mathfrak{g}$的限制就是$\mathfrak{g}$的杀戮形式；特别是，B 在 $\mathfrak{g}\times \mathfrak{g}$ 上是实值。假设$\mathfrak{a}$是可还原的；那么实数李代数$\mathfrak{g}$是紧的当且仅当B到$\mathfrak{g}$的限制为负数(§1, no. 3)。在这种情况下，我们说$\mathfrak{g}$是$\mathfrak{a}$的紧实数形式。

### 2. 真实形式与切瓦利系统相关

在这个数中，我们考虑分裂的半单李代数$(\mathfrak{a},\mathfrak{h})$超过域$\mathbf{C}$（第VIII, §2, no. 1章），以及根系$R(\mathfrak{a},\mathfrak{h}) = R$和Chevalley系统 $(X_{\alpha})_{\alpha\in R}$ / $(\mathfrak{a},\mathfrak{h})$（第 VIII, §2, no. 4 章，定义 3）。

回想一下（前述），对于所有 $\alpha \in R$，重合与$\mathfrak{h}$ 上的$-$Id$_{\mathfrak{h}}$ 和映射 $X_{\alpha}$ 到$X_{-\alpha}$ 的线性映射 $\theta :\mathfrak{a}\rightarrow \mathfrak{a}$ 是自同构共 $\mathfrak{a}$。此外（参见第 7 条提案），如果 $\alpha , \beta , \alpha +\beta$ 是根，则

$$
[X_{\alpha}, X_{\beta}] = N_{\alpha ,\beta}X_{\alpha+\beta} \tag{3}
$$

与 $N_{\alpha ,\beta}\in \mathbf{R}^*$ 和

$$
N_{-\alpha ,-\beta}= N_{\alpha ,\beta} \tag{4}
$$

用$\mathfrak{h}_0$表示$H\in \mathfrak{h}$的$\mathfrak{h}$由……组成的实向量子空间，使得$\alpha (H)\in \mathbf{R}$对于所有$\alpha \in R$。那么$\mathfrak{h}_0$是复杂向量空间$\mathfrak{h}$上的$\mathbf{R}$结构，我们对所有$\alpha \in R$有$[X_{\alpha}, X_{-\alpha}]\in \mathfrak{h}_0$，并且$\mathfrak{a}$到$\mathfrak{h}_0$的杀戮形式B的限制正在分离正数（第VIII, §2, no. 2、注2章）。而且，

$B(H, X_{\alpha}) = 0,B(X_{\alpha}, X_{\beta}) = 0$ 如果 $\alpha +\beta \not= 0,B(X_{\alpha}, X_{-\alpha})<0$ (5)

（第 VIII, §2, no. 2、第 1 条和no. 4、引理 3）。

#### 命题 2 {#lie-ix-s3-prop-2 .statement tag=01JG}

$a)$ $\mathfrak{a}$ 的真正向量子空间 $\mathfrak{a}_0=\mathfrak{h}_0+\sum_{\alpha\in R}\mathbf{R}X_{\alpha}$ 是

$\mathfrak{a}$的实数形式，其中$\mathfrak{h}_0$为嘉当子代数。 对$(\mathfrak{a}_0,\mathfrak{h}_0)$是分裂的半单实数李代数，其中$(X_{\alpha})$是Chevalley系统。

b) 令$\sigma$为$\mathfrak{a}$相对于$\mathfrak{a}_0$的共轭。然后$\sigma \circ \theta =\theta \circ \sigma$。 $\sigma \circ \theta$的固定点的集合是$\mathfrak{a}$的紧实数形式$\mathfrak{a}_u$，其中$i\mathfrak{h}_0$是嘉当子代数。

部分 a) 紧接着前面的内容。我们证明b）。由于$\sigma \circ \theta$和$\theta \circ \sigma$是从$\mathfrak{a}$到$\mathfrak{a}$的两个半线性映射，即$\mathfrak{a}_0$上的重合，因此它们重合。现在$\sigma \circ \theta$满足no. 1的条件(2)，因此是$\mathfrak{a}$相对于$x\in \mathfrak{a}$的实形式$\mathfrak{a}_u$由……组成的共轭，使得$\sigma \circ \theta (x) =x$（命题1）。对于所有 $\alpha \in R$ 投入

$$
u_{\alpha}=X_{\alpha}+X_{-\alpha},v_{\alpha}=i(X_{\alpha}-X_{-\alpha}) \tag{6}
$$

然后由$i\mathfrak{h}_0$、$u_{\alpha}$和$v_{\alpha}$生成$\mathbf{R}$向量空间$\mathfrak{a}_u$。更准确地说，如果我们选择R的一个C室，那么

$$
\mathfrak{a}_u=i\mathfrak{h}_0\oplus \bigoplus_{\alpha\in R_+(C)}(\mathbf{R}u_{\alpha}+\mathbf{R}v_{\alpha}) \tag{7}
$$

显然$i\mathfrak{h}_0$是$\mathfrak{a}_u$的嘉当子代数，还有待证明B到$\mathfrak{a}_u$的限制为负数。现在$i\mathfrak{h}_0$和形式$\mathbf{R}u_{\alpha}\oplus \mathbf{R}v_{\alpha}$的不同子空间关于B正交，由(5)可知； B 到 $i\mathfrak{h}_0$ 的限制为负，并且

$$
B(u_{\alpha}, u_{\alpha}) = B(v_{\alpha}, v_{\alpha}) = 2B(X_{\alpha}, X_{-\alpha})<0,B(u_{\alpha}, v_{\alpha}) = 0 \tag{8}
$$

因此得出结论。

#### 注 {#lie-ix-s3-n2-rem-1 .statement tag=01B2}

有了前面的记号，我们就有了下面的公式：

$$
[h, u_{\alpha}] =-i\alpha (h)v_{\alpha},[h, v_{\alpha}] =i\alpha (h)u_{\alpha},[u_{\alpha}, v_{\alpha}] = 2iH_{\alpha},(h\in \mathfrak{h}) \tag{9}
$$

$$
[u_{\alpha}, u_{\beta}] = N_{\alpha ,\beta}u_{\alpha+\beta}+ N_{\alpha ,-\beta}u_{\alpha-\beta},\alpha \not=\pm \beta \tag{10}
$$

$$
[v_{\alpha}, v_{\beta}] =-N_{\alpha ,\beta}u_{\alpha+\beta}+ N_{\alpha ,-\beta}u_{\alpha-\beta},\alpha \not=\pm \beta \tag{11}
$$

$$
[u_{\alpha}, v_{\beta}] = N_{\alpha ,\beta}v_{\alpha+\beta}-N_{\alpha ,-\beta}v_{\alpha-\beta},\alpha \not=\pm \beta \tag{12}
$$

（在最后三个公式中，像往常一样，如果$\gamma +\delta$不是根，则可以理解为$N_{\gamma ,\delta}= 0$）。

注即$\sum\mathbf{R}u_{\alpha}$是$\mathfrak{a}$的实数子代数，即$\mathfrak{a}_0\cap \mathfrak{a}_u$。

令 Q(R) 为 R 的根权的群（第VI, §1, no. 9章）。回想一下，任何同态$\gamma : Q(R)\rightarrow \mathbf{C}^*$都与$\mathfrak{a}$的基本自同构$f(\gamma )$相关联，这样$f(\gamma )(h) =h$适用于所有$h\in \mathfrak{h}$和$f(\gamma )X_{\alpha}=$$\gamma (\alpha )X_{\alpha}$（第VIII, §5, no. 2章）。

#### 命题 3 {#lie-ix-s3-prop-3 .statement tag=01B3}

令$\mathfrak{g}$为$\mathfrak{a}$的紧实数形式，使得$\mathfrak{g}\cap \mathfrak{h}=i\mathfrak{h}_0$。存在同态$\gamma : Q(R)\rightarrow \mathbf{R}^*_+$使得$\mathfrak{g}=f(\gamma )(\mathfrak{a}_u)$。

令 $\tau$ 为 $\mathfrak{a}$ 相对于 $\mathfrak{g}$ 的共轭。 假设$\tau (x) =x$为$x\in i\mathfrak{h}_0$，所以$\tau (x) =-x$为$x\in \mathfrak{h}_0$。因此，对于所有$\alpha \in R$和所有$h\in \mathfrak{h}_0$，

$$
[h, \tau (X_{\alpha})] = [-\tau (h), \tau (X_{\alpha})] =-\tau ([h, X_{\alpha}]) =-\tau (\alpha (h)X_{\alpha})
$$

由此可见，$[h, \tau (X_{\alpha})] =-\alpha (h)\tau (X_{\alpha})$适用于所有$h\in \mathfrak{h}_0$，因此也适用于所有$h\in \mathfrak{h}$。因此存在$c_{\alpha}\in \mathbf{C}^*$使得$\tau (X_{\alpha}) =c_{\alpha}X_{-\alpha}$。由于$[X_{\alpha}, X_{-\alpha}]\in \mathfrak{h}_0$，我们有$[\tau (X_{\alpha}), \tau (X_{-\alpha})] =-[X_{\alpha}, X_{-\alpha}]$，所以$c_{\alpha}c_{-\alpha}$ = 1；类似地，如果$\alpha , \beta , \alpha +\beta$是根，公式（3）和（4）给出$c_{\alpha+\beta}=c_{\alpha}c_{\beta}$。由章。 VI, §1, no. 6，科。根据第 19 条命题 2，存在同态 $\delta : Q(R)\rightarrow \mathbf{C}^*$，使得 $\delta (\alpha ) =c_{\alpha}$ 对于所有 $\alpha \in R$。

现在我们证明每个 $c_{\alpha}$ 都是严格正的。事实上，$c_{\alpha}B(X_{\alpha}, X_{-\alpha}) =$$B(X_{\alpha}, \tau (X_{\alpha}))$，并且由于$B(X_{\alpha}, X_{-\alpha})$是负数，因此足以证明$B(z, \tau (z))<0$对于$\mathfrak{a}$的每个非零元素$z$；但$\mathfrak{a}$的每个元素都可以写成$x+iy$，$x$和$y$在$\mathfrak{g}$中，并且

$$
B(x+iy, \tau (x+iy)) = B(x+iy, x-iy) = B(x, x) + B(y, y)
$$

因此，B 到 $\mathfrak{g}$ 的规定断言、限制为负，并以假设分隔。

由此可见，同态$\delta$在$\mathbf{R}^*_+$中取值；因此存在同态$\gamma : Q(R)\rightarrow \mathbf{R}^*_+$使得$\delta =\gamma^{-2}$。那么$f(\gamma )^{-1}(\mathfrak{g})$就是$\mathfrak{a}$的实数形式； 相应的共轭是$\tau '=f(\gamma )^{-1}\circ \tau \circ f(\gamma )$。对于所有$\alpha \in R$，我们有

$$
\tau '(X_{\alpha}) =f(\gamma )^{-1}(\tau (c^{-1/2}_{\alpha}X_{\alpha})) =f(\gamma )^{-1}(c^{1/2}_{\alpha}X_{-\alpha}) =X_{-\alpha}
$$

$\tau '(h) =\tau (h) =h$ 为 $h\in i\mathfrak{h}_0$；由此可见，$\tau '$是相对于$\mathfrak{a}_u$的共轭，因此是$f(\gamma )^{-1}(\mathfrak{g}) =\mathfrak{a}_u$。

### 3. 紧形式的共轭

#### 定理 1 {#lie-ix-s3-thm-1 .statement tag=01B4}

令$\mathfrak{a}$为复半单李代数。

a$)\mathfrak{a}$ 具有紧凑（或可拆分）实数形式。

b) 群 Int($\mathfrak{a}$) 可传递地对 $\mathfrak{a}$ 的紧凑（可拆分）实数形式的集合进行操作。

令$\mathfrak{h}$为$\mathfrak{a}$的嘉当子代数。那么 $(\mathfrak{a},\mathfrak{h})$ 就是分裂的（第 VIII, §2, no. 1、注 2），并且有一个 Chevalley 系统 $(X_{\alpha})$（第 VIII, §4, no. 4 章，Prop. 5 的 Cor.）。 部分 a) 现在由命题 2 得出。令 $\mathfrak{g}$ 为 $\mathfrak{a}$ 的紧实数形式；我们证明存在 $v\in$ Int($\mathfrak{a}$) 使得$v(\mathfrak{a}_u) =\mathfrak{g}$。设$\mathfrak{t}$为$\mathfrak{g}$的嘉当子代数；那么$\mathfrak{t}_{(\mathbf{C})}$是$\mathfrak{a}$的嘉当子代数；由于 Int($\mathfrak{a}$) 对 $\mathfrak{a}$ 的嘉当子代数集合进行传递运算（第 VII, §3, no. 2，第 1 章），我们被简化为$\mathfrak{t}_{(\mathbf{C})}=\mathfrak{h}$ 的情况。由于$\mathfrak{g}$是紧形式，自同态和$h$的特征值，对于$h\in \mathfrak{t}$来说，纯粹是虚数（§1, no. 3，命题1），所以根$\alpha \in R$映射 $\mathfrak{t}$至$i\mathbf{R}$；这意味着$\mathfrak{t}=i\mathfrak{h}_0$。那么，根据命题3 (no. 2)，存在$v\in$ Int($\mathfrak{a}$)使得$v(\mathfrak{a}_u) =\mathfrak{g}$，因此在紧形式的情况下为b)。最后，令$\mathfrak{m}_1$和$\mathfrak{m}_2$为$\mathfrak{a}$的两个可分割实数形式。存在框架$(\mathfrak{m}_1,\mathfrak{h}_1,B_1,(X_{\alpha}^1))$和$(\mathfrak{m}_2,\mathfrak{h}_2,B_2,(X_{\alpha}^2))$（第VIII, §4, no. 1章）。这些扩展以明显的方式变为基$e_1$和$e_2$$\mathfrak{a}$。 $\mathfrak{a}$中的自同构即映射$e_1$至$e_2$映射$\mathfrak{m}_1$至$\mathfrak{m}_2$；因此，应用第 1 章第 5 条就足够了。 VIII, §5, no. 3，获取Aut$_0(\mathfrak{a}) =$Int($\mathfrak{a}$)中元素$u$的存在性使得$u(\mathfrak{m}_1) =\mathfrak{m}_2$。

#### 注 {#lie-ix-s3-n3-rem-1 .statement tag=01B5}

稍后我们将看到实形式复半单李代数的一般分类。

#### 推论 1 {#lie-ix-s3-thm-1-cor-1 .statement tag=01B6}

令$\mathfrak{g}$和$\mathfrak{g}'$为两个紧实李代数。那么 $\mathfrak{g}$ 和 $\mathfrak{g}'$ 同构当且仅当复数李代数 $\mathfrak{g}_{(\mathbf{C})}$ 和 $\mathfrak{g}'_{(\mathbf{C})}$ 同构的。

条件显然是必要的。相反，假设 $\mathfrak{g}_{(\mathbf{C})}$ 和 $\mathfrak{g}'_{(\mathbf{C})}$ 同构。令$\mathfrak{c}$（分别$\mathfrak{c}'$）为$\mathfrak{g}$（分别$\mathfrak{g}'$）和$\mathfrak{s}$（分别$\mathfrak{s}'$）的中心和$\mathfrak{g}$（分别$\mathfrak{g}'$）的派生代数。那么$\mathfrak{c}_{(\mathbf{C})}$和$\mathfrak{c}'_{(\mathbf{C})}$分别是$\mathfrak{g}_{(\mathbf{C})}$和$\mathfrak{g}'_{(\mathbf{C})}$的中心，因此是同构的；由此可见交换代数 $\mathfrak{c}$ 和 $\mathfrak{c}'$ 是同构的。类似地，$\mathfrak{s}_{(\mathbf{C})}$和$\mathfrak{s}'_{(\mathbf{C})}$是同构的，因此$\mathfrak{s}$和$\mathfrak{s}'$是两个同构复半单李代数的紧实数形式，与Th同构。 $1b)$。

#### 推论 2 {#lie-ix-s3-thm-1-cor-2 .statement tag=01B7}

令 $\mathfrak{a}$ 为复数李代数。以下条件是等效的：

(i) $\mathfrak{a}$ 是还原的。

(ii) 存在紧实李代数 $\mathfrak{g}$，使得$\mathfrak{a}$与$\mathfrak{g}_{(\mathbf{C})}$同构。

(iii) 存在紧李群 G，使得$\mathfrak{a}$同构于$L(G)_{(\mathbf{C})}$。

由Def。 §1, no. 3、条件 (ii) 和 (iii) 中的 1 是等效的并暗示 (i)。如果 $\mathfrak{a}$ 是还原的，它是交换代数的直接乘积，它显然有一个紧实数形式，而半单代数有一个 Th。 $1a)$，因此 (i) 意味着 (ii)。

#### 推论 3 {#lie-ix-s3-thm-1-cor-3 .statement tag=01B8}

令$\mathfrak{a}_1$和$\mathfrak{a}_2$为两个复半单李代数。 $\mathfrak{a}_1\times \mathfrak{a}_2$ 的紧实数形式为乘积 $\mathfrak{g}_1\times \mathfrak{g}_2$，其中 $i= 1,2,\mathfrak{g}_i$ 是 $\mathfrak{a}_i$ 的紧实数形式。

事实上，存在 $\mathfrak{a}_1$（或 $\mathfrak{a}_2$）的紧实数形式 $\mathfrak{g}_1$（或 $\mathfrak{g}_2$）；那么$\mathfrak{g}_1\times \mathfrak{g}_2$是$\mathfrak{a}_1\times \mathfrak{a}_2$的紧实数形式。现在可以从 Th 得出推论。 $1b)$，适用于$\mathfrak{a}_1,\mathfrak{a}_2$和$\mathfrak{a}_1\times \mathfrak{a}_2$。

注源自 Cor. 3 上面的紧实李代数$\mathfrak{g}$是简单的当且仅当复杂的李代数$\mathfrak{g}_{(\mathbf{C})}$是简单的。如果$\mathfrak{g}_{(\mathbf{C})}$是型$A_n$或$B_n,. .$，我们说$\mathfrak{g}$是型$A_n$或$B_n,. .$。 （第VIII, §2, no. 2章）。由科.上面 1 中，两个紧简实数李代数同构当且仅当它们的型相同。

令 G 为几乎简单连通的紧李群（第 III, §9, no. 8 章，定义 3）。我们说G是型$A_n$，或$B_n,. .$。，如果它的李代数是型，$A_n$，或$B_n,. .$。。两个简单连接的几乎简单的紧李群同构当且仅当它们相同型。

### 4. 例 I: 紧代数型 A$_{\boldsymbol{n}}$

令V为有限维复数向量空间，$\Phi$为V上的分离正值厄米特形式。 The unitary group associated to $\Phi$ (cf. Algebra, Chap. IX) is the subgroup $\mathbf{U}(\Phi )$ of $\mathbf{G}\mathbf{L}(V)$ consisting of the automorphisms of the complex Hilbert space $(V, \Phi )$; this is a (real) Lie subgroup of the group $\mathbf{G}\mathbf{L}$(V), whose Lie algebra is the subalgebra $\mathfrak{u}(\Phi )$ of the real Lie algebra $\mathfrak{g}\mathfrak{l}(V)$ consisting of the endomorphisms $x$ of V such that $x^*=-x$ (Chap. III, §3, no. 10, Cor. 2 of Prop. 37), where $x^*$ denotes the adjoint of $x$ relative to $\Phi$. 由于群 $\mathbf{U}(\Phi )$ 是紧致的（§1，第 $1$）$,\mathfrak{u}(\Phi )$ 是紧实李代数。 同样，特殊酉群$\mathbf{S}\mathbf{U}(\Phi ) =\mathbf{U}(\Phi )\cap \mathbf{S}\mathbf{L}(V)$是$\mathbf{S}\mathbf{L}$(V)的紧李子群，其李代数是$\mathfrak{s}\mathfrak{u}(\Phi ) =\mathfrak{u}(\Phi )\cap \mathfrak{s}\mathfrak{l}(V)$。

当$V =\mathbf{C}^n$和$\Phi$是通常的厄米特形式（其中$\mathbf{C}^n$的典范基是正交的）时，我们写$\mathbf{U}(n,\mathbf{C}),\mathbf{S}\mathbf{U}(n,\mathbf{C}),\mathfrak{u}(n,\mathbf{C}),\mathfrak{s}\mathfrak{u}(n,\mathbf{C})$而不是$\mathbf{U}(\Phi ),\mathbf{S}\mathbf{U}(\Phi ),\mathfrak{u}(\Phi ),\mathfrak{s}\mathfrak{u}(\Phi )$。 $\mathbf{U}(n,\mathbf{C})$（或$\mathfrak{u}(n,\mathbf{C})$）的元素是矩阵$A\in M_n(\mathbf{C})$，使得$A.^t\overline{A}=I_n$（或$A=-^t\overline{A}$），被称为酉（或反厄米特）。

#### 命题 4 {#lie-ix-s3-prop-4 .statement tag=01B9}

a) 复数李代数$\mathfrak{s}\mathfrak{l}(V)$的紧实数形式是代数$\mathfrak{s}\mathfrak{u}(\Phi )$，其中复数向量空间V上分离正厄米特形式的$\Phi$属于到集合。

b) 代数 $\mathfrak{u}(\Phi )$ 是 $\mathfrak{g}\mathfrak{l}(V)$ 的紧实数形式。

设$\Phi$为V上的分离正值厄米特形式。 对于所有$x\in \mathfrak{g}\mathfrak{l}$(V)，放入$\sigma (x) =-x^*$（其中$x^*$是$x$相对于$\Phi$的伴随）。 那么$\sigma$满足no. 1命题1的条件(2)，因此$\mathfrak{g}\mathfrak{l}(V)$（$\mathfrak{s}\mathfrak{l}(V)$）上$\sigma$的固定点的集合$\mathfrak{u}(\Phi )$（$\mathfrak{s}\mathfrak{u}(\Phi )$）是紧实数形式共 $\mathfrak{g}\mathfrak{l}(V)$（分别为 $\mathfrak{s}\mathfrak{l}(V)$）。 由于$\mathbf{G}\mathbf{L}(V)$在V（代数，第IX）上的分离正厄米特形式的集合以及$\mathfrak{s}\mathfrak{l}(V)$（no. 3，第1章）的紧致实数形式的集合上进行传递操作和第 VIII, §13, no. 1 (VII))，命题 4 得到证明。

#### 推论{#lie-ix-s3-n4-cor-1 .statement tag=01BA}

型 $A_n(n\geq 1)$ 的每个紧简实数李代数都同构于 $\mathfrak{s}\mathfrak{u}(n+ 1,\mathbf{C})$。

事实上，型$A_n$的每个复数李代数都同构于$\mathfrak{s}\mathfrak{l}(n+ 1,\mathbf{C})$（第VIII, §13, no. 1章）。

#### 注 1 {#lie-ix-s3-n4-rem-1 .statement tag=01BB}

我们有$\mathfrak{g}\mathfrak{l}(V) =\mathfrak{s}\mathfrak{l}(V)\times \mathbf{C}.1_V,\mathfrak{u}(\Phi ) =\mathfrak{s}\mathfrak{u}(\Phi )\times \mathbf{R}.i1_V$； $\mathfrak{g}\mathfrak{l}(V)$ 的紧实数形式是$\mathfrak{s}\mathfrak{u}(\Phi )\times \mathbf{R}.\alpha 1_V,\alpha \in \mathbf{C}^*$。

#### 注 2 {#lie-ix-s3-n4-rem-2 .statement tag=01BC}

如果复合体李代数$\mathfrak{a}=\mathfrak{s}\mathfrak{l}(n,\mathbf{C})$配备了第1章中介绍的分裂和Chevalley系统。 VIII, §13, no. 1 (IX)，那么，记号在no. 2中，

$$
\mathfrak{a}_u=\mathfrak{s}\mathfrak{u}(n,\mathbf{C}),\mathfrak{a}_0=\mathfrak{s}\mathfrak{l}(n,\mathbf{R}),\mathfrak{a}_u\cap \mathfrak{a}_0=\mathfrak{o}(n,\mathbf{R})
$$

### 5. 例II：紧代数型B$_{\boldsymbol{n}}\mathbf{A}\mathbf{N}\mathbf{D}$$\mathbf{D}_{\boldsymbol{n}}$

令 V 为有限维实数向量空间，Q 为 V 上的分离正二次方形式。 The orthogonal group associated to Q (Algebra, Chap. IX) is the subgroup $\mathbf{O}(Q)$ of $\mathbf{G}\mathbf{L}(V)$ consisting of the automorphisms of the real Hilbert space $(V,Q)$; this is a Lie subgroup of $\mathbf{G}\mathbf{L}$(V), whose Lie algebra is the subalgebra $\mathfrak{o}(Q)$ of $\mathfrak{g}\mathfrak{l}(V)$ consisting of the endomorphisms $x$ of V such that $x^*=-x$ (Chap. III, §3, no. 10, Cor. 2 of Prop. $37$)$,x^*$ denoting the adjoint of $x$ relative to Q. 由于群$\mathbf{O}(Q)$是紧致的，$\mathfrak{o}(Q)$因此是紧实李代数。 把$\mathbf{S}\mathbf{O}(Q) =\mathbf{O}(Q)\cap \mathbf{S}\mathbf{L}(V)$；这是 $\mathbf{O}(Q)$ 的有限指标的闭子群（如果 $V\not= 0$ 暗淡，则为指标 2），因此也有李代数 $\mathfrak{o}(Q)$。

当$V =\mathbf{R}^n$和Q是通常的二次形式（其中$\mathbf{R}^n$的典范基是正交的）时，我们写成$\mathbf{O}(n,\mathbf{R}),\mathbf{S}\mathbf{O}(n,\mathbf{R}),\mathfrak{o}(n,\mathbf{R})$而不是$\mathbf{O}(Q),\mathbf{S}\mathbf{O}(Q),\mathfrak{o}(Q)$。 $\mathbf{O}(n,\mathbf{R})$（或$\mathfrak{o}(n,\mathbf{R})$）的元素是矩阵$A\in M_n(\mathbf{R})$，使得$A.^tA=I_n$（或$A=-^tA$），这被称为正交（或反对称）。

令 $V_{(\mathbf{C})}$ 为与 V 关联的复数向量空间，并令 $Q_{(\mathbf{C})}$ 为与 Q 伴随的 $V_{(\mathbf{C})}$ 上的二次方形式。 认同 $\mathfrak{g}\mathfrak{l}(V)_{(\mathbf{C})}$ 与 $\mathfrak{g}\mathfrak{l}(V_{(\mathbf{C})})$；那么 $\mathfrak{o}(Q)_{(\mathbf{C})}$ 就等于 $\mathfrak{o}(Q_{(\mathbf{C})}):$ 这很清楚，因为从 $\mathfrak{g}\mathfrak{l}(V_{(\mathbf{C})})$ 到自身的映射 $x \rightarrow x^*+x$ 是 $\mathbf{C}$ 线性的。由于如果暗淡$V = 2n+ 1$、$n\geq 1$，则$\mathfrak{o}(Q_{(\mathbf{C})})$是型$B_n$，如果暗淡$V = 2n,n\geq 3$，则型$D_n$（第VIII, §13章，第2和4），我们推论：

#### 命题 5 {#lie-ix-s3-prop-5 .statement tag=01BD}

Every compact simple real Lie algebra of type $B_n,n\geq 1$ (resp. of type $D_n,n\geq 3$) is isomorphic to $\mathfrak{o}(2n+ 1,\mathbf{R})$ (resp. $\mathfrak{o}(2n,\mathbf{R})$).

### 6. COMPACT GROUPS OF RANK 1

作者：将军拓扑，第 1 章VIII, §1, no. 4、命题3、命题4和注4，拓扑群$\mathbf{S}\mathbf{U}(2,\mathbf{C})$同构于范数1四元数的拓扑群$\mathbf{S}_3$，以及$\mathbf{S}\mathbf{U}(2,\mathbf{C})$的商矩阵 $I_2$ 和$-I_2$ 的子群 Z 由……组成与拓扑群 $\mathbf{S}\mathbf{O}(3,\mathbf{R})$同构的。 Z确实是$\mathbf{S}\mathbf{U}(2,\mathbf{C}):$中心的注，从$\mathbf{H}=\mathbf{R}.\mathbf{S}_3$开始，群$\mathbf{S}_3$中心元素在代数中心$\mathbf{R}$ $\mathbf{H}$，因此属于到群，有两个元素$\mathbf{S}_3\cap \mathbf{R}=\{-1,1\}$。

#### 命题 6 {#lie-ix-s3-prop-6 .statement tag=01BE}

秩 1 的每个紧致半单实李代数同构于$\mathfrak{s}\mathfrak{u}(2,\mathbf{C})$和$\mathfrak{o}(3,\mathbf{R})$。 秩 1 的每个连通的半单紧李群如果是单连通，则与 $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ 同构的，否则与 $\mathbf{S}\mathbf{O}(3,\mathbf{R})$ 同构的。

第一个断言源自 Cor。提案 4 和提案 5。由于 $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ 同胚于 $\mathbf{S}_3($General 拓扑，第 1 章VIII, §1, no. 4, 注 4)，因此是单连通的（概述拓扑，第 XI 章，准备中），秩 1 的每个单连通紧凑半单李群同构于 $\mathbf{S}\mathbf{U}(2,\mathbf{C})$； 秩 1 的每个非单连通的连通紧凑半单李群同构于 Z 的$\mathbf{S}\mathbf{U}(2,\mathbf{C})$除以子群的商，但不约化与单位元素，因此与$\mathbf{S}\mathbf{O}(3,\mathbf{R})$同构的。

#### 注{#lie-ix-s3-n6-rem-1 .statement tag=01BF}

上面我们已经看到，$\mathbf{S}\mathbf{U}(2,\mathbf{C})$是单连通的，$\pi_1(\mathbf{S}\mathbf{O}(3,\mathbf{R}))$是阶2。稍后我们将看到这些结果分别推广到$\mathbf{S}\mathbf{U}(n,\mathbf{C}) (n\geq 1)$和$\mathbf{S}\mathbf{O}(n,\mathbf{R}) (n\geq 3)$（cf.还有§3，练习4和5）。

回想一下（第VIII, §1, no. 1章），$\mathfrak{s}\mathfrak{l}(2,\mathbf{C})$的典范基是基$(X_+, X_-, H)$，其中

$(01)(00)(1$ 0 $)$

$X_+=$ 0 0 $, X_-=-1$ 0 $, H=$ 0 $-1$。

因此，我们获得 $\mathfrak{su}(2,\mathbf C)$ 的基 $(U,V,iH)$，也称为规范，通过将
$$
U=X_++X_-=
\begin{pmatrix}
0&1\\
-1&0
\end{pmatrix},
\qquad
V=i(X_+-X_-)=
\begin{pmatrix}
0&i\\
i&0
\end{pmatrix},
$$
$$
iH=
\begin{pmatrix}
i&0\\
0&-i
\end{pmatrix}.
$$

我们有
$$
[iH,U]=2V,\qquad [iH,V]=-2U,\qquad [U,V]=2iH.
\tag{13}
$$

如果 B 表示 $\mathfrak{su}(2,\mathbf C)$ 直接的的杀戮形式计算得出
$$
\mathrm{B}(aU+bV+ciH,a'U+b'V+c'iH)=-8(aa'+bb'+cc'),
\tag{14}
$$
因此，如果我们将认同$\mathfrak{su}(2,\mathbf C)$与$\mathbf R^3$通过典范基，$\mathbf{SU}(2,\mathbf C)$定义同态$\mathbf{SU}(2,\mathbf C)\to\mathbf{SO}(3,\mathbf R)$（上面的cf.）的伴随表示。

进一步地，$\mathbf RiH$是$\mathfrak{su}(2,\mathbf C)$的嘉当子代数的注，对应对其的$\mathbf{SU}(2,\mathbf C)$的最大环面T由对角线矩阵组成
$$
\begin{pmatrix}
a&0\\
0&\bar a
\end{pmatrix},
$$
其中 $a\bar a=1$，指数映射
$$
\exp:\mathbf RiH\longrightarrow T
$$
映射$xH$，$x\in\mathbf Ri$，至矩阵
$$
\begin{pmatrix}
\exp(x)&0\\
0&\exp(-x)
\end{pmatrix},
$$
因此有核 $\mathbf Z.K$，其中 K 是 $\mathfrak{su}(2,\mathbf C)$ 的元素定义为
$$
K=2\pi iH=
\begin{pmatrix}
2\pi i&0\\
0&-2\pi i
\end{pmatrix}.
\tag{15}
$$

此外，$\mathbf{SU}(2,\mathbf C)$的中心由恒等式和$\exp(K/2)$组成。

放
$$
\theta=
\begin{pmatrix}
0&-1\\
1&0
\end{pmatrix}
\in\mathbf{SU}(2,\mathbf C).
\tag{16}
$$

由章。 VIII, §1, no. 5,
$$
\theta^2=
\begin{pmatrix}
-1&0\\
0&-1
\end{pmatrix},
\qquad
(\mathrm{Int}\,\theta)t=t^{-1},\quad t\in T,
\tag{17}
$$
$$
(\mathrm{Ad}\,\theta)X_+=X_-,
\qquad
(\mathrm{Ad}\,\theta)X_-=X_+,
\qquad
(\mathrm{Ad}\,\theta)U=U,
\qquad
(\mathrm{Ad}\,\theta)V=-V.
\tag{18}
$$

最后，对于 $t=
\begin{pmatrix}
a&0\\
0&\bar a
\end{pmatrix}
\in T$，我们有
$$
(\mathrm{Ad}\,t)X_+=a^2X_+,
\qquad
(\mathrm{Ad}\,t)X_-=a^{-2}X_-,
\qquad
(\mathrm{Ad}\,t)H=H,
\tag{19}
$$
$$
(\mathrm{Ad}\,t)U=\mathscr{R}(a^2)U+\mathscr{I}(a^2)V,
\qquad
(\mathrm{Ad}\,t)V=-\mathscr{I}(a^2)U+\mathscr{R}(a^2)V.
\tag{20}
$$

### 习题 {#lie-ix-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
